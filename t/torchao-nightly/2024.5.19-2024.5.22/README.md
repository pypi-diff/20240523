# Comparing `tmp/torchao_nightly-2024.5.19-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/torchao_nightly-2024.5.22-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,109 +1,110 @@
-Zip file size: 415398 bytes, number of entries: 107
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 02:38 torchao/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 02:38 torchao_nightly-2024.5.19.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 02:38 torchao_nightly.libs/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 02:38 torchao/csrc/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 02:38 torchao/dtypes/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 02:38 torchao/kernel/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 02:38 torchao/prototype/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 02:38 torchao/quantization/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 02:38 torchao/sparsity/
--rwxr-xr-x  2.0 unx   810656 b- defN 24-May-19 02:38 torchao/_C.cpython-39-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      426 b- defN 24-May-19 02:38 torchao/__init__.py
--rw-r--r--  2.0 unx     4792 b- defN 24-May-19 02:38 torchao/ops.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 02:38 torchao/csrc/cuda/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 02:38 torchao/csrc/fp6_llm/
--rw-r--r--  2.0 unx       74 b- defN 24-May-19 02:38 torchao/csrc/init.cpp
--rw-r--r--  2.0 unx      251 b- defN 24-May-19 02:38 torchao/csrc/nms.cpp
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 02:38 torchao/csrc/cuda/fp6_llm/
--rw-r--r--  2.0 unx     5554 b- defN 24-May-19 02:38 torchao/csrc/cuda/nms.cu
--rw-r--r--  2.0 unx     9437 b- defN 24-May-19 02:38 torchao/csrc/cuda/fp6_llm/fp6_linear.cu
--rw-r--r--  2.0 unx     9472 b- defN 24-May-19 02:38 torchao/csrc/cuda/fp6_llm/weight_quant.cu
--rw-r--r--  2.0 unx      479 b- defN 24-May-19 02:38 torchao/csrc/fp6_llm/fp6_llm.cpp
--rw-r--r--  2.0 unx     9210 b- defN 24-May-19 02:38 torchao/csrc/fp6_llm/weight_prepacking.cpp
--rw-r--r--  2.0 unx      136 b- defN 24-May-19 02:38 torchao/dtypes/__init__.py
--rw-r--r--  2.0 unx    33918 b- defN 24-May-19 02:38 torchao/dtypes/nf4tensor.py
--rw-r--r--  2.0 unx    12448 b- defN 24-May-19 02:38 torchao/dtypes/uint4.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-19 02:38 torchao/kernel/__init__.py
--rw-r--r--  2.0 unx     7389 b- defN 24-May-19 02:38 torchao/kernel/autotuner.py
--rw-r--r--  2.0 unx     3238 b- defN 24-May-19 02:38 torchao/kernel/intmm.py
--rw-r--r--  2.0 unx    11678 b- defN 24-May-19 02:38 torchao/kernel/intmm_triton.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 02:38 torchao/prototype/common/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 02:38 torchao/prototype/dora/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 02:38 torchao/prototype/galore/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 02:38 torchao/prototype/hqq/
--rw-r--r--  2.0 unx        0 b- defN 24-May-19 02:38 torchao/prototype/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-19 02:38 torchao/prototype/common/__init__.py
--rw-r--r--  2.0 unx     7071 b- defN 24-May-19 02:38 torchao/prototype/common/profiling_tools.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 02:38 torchao/prototype/dora/kernels/
--rw-r--r--  2.0 unx        0 b- defN 24-May-19 02:38 torchao/prototype/dora/__init__.py
--rw-r--r--  2.0 unx     6639 b- defN 24-May-19 02:38 torchao/prototype/dora/dora_layer.py
--rw-r--r--  2.0 unx     3972 b- defN 24-May-19 02:38 torchao/prototype/dora/dora_profile.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-19 02:38 torchao/prototype/dora/kernels/__init__.py
--rw-r--r--  2.0 unx     4846 b- defN 24-May-19 02:38 torchao/prototype/dora/kernels/common.py
--rw-r--r--  2.0 unx    15366 b- defN 24-May-19 02:38 torchao/prototype/dora/kernels/custom_autotune.py
--rw-r--r--  2.0 unx     7641 b- defN 24-May-19 02:38 torchao/prototype/dora/kernels/matmul.py
--rw-r--r--  2.0 unx    16439 b- defN 24-May-19 02:38 torchao/prototype/dora/kernels/smallk.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 02:38 torchao/prototype/galore/kernels/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 02:38 torchao/prototype/galore/optim/
--rw-r--r--  2.0 unx       23 b- defN 24-May-19 02:38 torchao/prototype/galore/__init__.py
--rw-r--r--  2.0 unx     3195 b- defN 24-May-19 02:38 torchao/prototype/galore/utils.py
--rw-r--r--  2.0 unx      210 b- defN 24-May-19 02:38 torchao/prototype/galore/kernels/__init__.py
--rw-r--r--  2.0 unx    10675 b- defN 24-May-19 02:38 torchao/prototype/galore/kernels/adam_downproj_fused.py
--rw-r--r--  2.0 unx     4722 b- defN 24-May-19 02:38 torchao/prototype/galore/kernels/adam_step.py
--rw-r--r--  2.0 unx    15180 b- defN 24-May-19 02:38 torchao/prototype/galore/kernels/custom_autotune.py
--rw-r--r--  2.0 unx    11641 b- defN 24-May-19 02:38 torchao/prototype/galore/kernels/matmul.py
--rw-r--r--  2.0 unx     5978 b- defN 24-May-19 02:38 torchao/prototype/galore/kernels/quant.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-19 02:38 torchao/prototype/galore/optim/__init__.py
--rw-r--r--  2.0 unx    15716 b- defN 24-May-19 02:38 torchao/prototype/galore/optim/galore_torch.py
--rw-r--r--  2.0 unx       50 b- defN 24-May-19 02:38 torchao/prototype/hqq/__init__.py
--rw-r--r--  2.0 unx     7658 b- defN 24-May-19 02:38 torchao/prototype/hqq/hqq_tinygemm_linear.py
--rw-r--r--  2.0 unx    14227 b- defN 24-May-19 02:38 torchao/prototype/hqq/kernels.py
--rw-r--r--  2.0 unx     5512 b- defN 24-May-19 02:38 torchao/prototype/hqq/mixed_mm.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 02:38 torchao/quantization/prototype/
--rw-r--r--  2.0 unx    50342 b- defN 24-May-19 02:38 torchao/quantization/GPTQ.py
--rw-r--r--  2.0 unx     1700 b- defN 24-May-19 02:38 torchao/quantization/__init__.py
--rw-r--r--  2.0 unx    19369 b- defN 24-May-19 02:38 torchao/quantization/autoquant.py
--rw-r--r--  2.0 unx     2747 b- defN 24-May-19 02:38 torchao/quantization/dynamic_quant.py
--rw-r--r--  2.0 unx     7110 b- defN 24-May-19 02:38 torchao/quantization/quant_api.py
--rw-r--r--  2.0 unx    32825 b- defN 24-May-19 02:38 torchao/quantization/quant_primitives.py
--rw-r--r--  2.0 unx     9159 b- defN 24-May-19 02:38 torchao/quantization/smoothquant.py
--rw-r--r--  2.0 unx    42347 b- defN 24-May-19 02:38 torchao/quantization/subclass.py
--rw-r--r--  2.0 unx      754 b- defN 24-May-19 02:38 torchao/quantization/unified.py
--rw-r--r--  2.0 unx     3169 b- defN 24-May-19 02:38 torchao/quantization/utils.py
--rw-r--r--  2.0 unx     2742 b- defN 24-May-19 02:38 torchao/quantization/weight_only.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-19 02:38 torchao/quantization/prototype/__init__.py
--rw-r--r--  2.0 unx    12816 b- defN 24-May-19 02:38 torchao/quantization/prototype/qat.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 02:38 torchao/sparsity/prototype/
--rw-r--r--  2.0 unx      508 b- defN 24-May-19 02:38 torchao/sparsity/__init__.py
--rw-r--r--  2.0 unx     1077 b- defN 24-May-19 02:38 torchao/sparsity/sparse_api.py
--rw-r--r--  2.0 unx     1708 b- defN 24-May-19 02:38 torchao/sparsity/utils.py
--rw-r--r--  2.0 unx     4156 b- defN 24-May-19 02:38 torchao/sparsity/wanda.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 02:38 torchao/sparsity/prototype/pruner/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 02:38 torchao/sparsity/prototype/scheduler/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 02:38 torchao/sparsity/prototype/sparsifier/
--rw-r--r--  2.0 unx      843 b- defN 24-May-19 02:38 torchao/sparsity/prototype/__init__.py
--rw-r--r--  2.0 unx     9107 b- defN 24-May-19 02:38 torchao/sparsity/prototype/dynamic_quant_sparse.py
--rw-r--r--  2.0 unx     3388 b- defN 24-May-19 02:38 torchao/sparsity/prototype/pruner/FPGM_pruner.py
--rw-r--r--  2.0 unx      273 b- defN 24-May-19 02:38 torchao/sparsity/prototype/pruner/__init__.py
--rw-r--r--  2.0 unx    10873 b- defN 24-May-19 02:38 torchao/sparsity/prototype/pruner/base_structured_sparsifier.py
--rw-r--r--  2.0 unx     2050 b- defN 24-May-19 02:38 torchao/sparsity/prototype/pruner/lstm_saliency_pruner.py
--rw-r--r--  2.0 unx     1967 b- defN 24-May-19 02:38 torchao/sparsity/prototype/pruner/match_utils.py
--rw-r--r--  2.0 unx     1818 b- defN 24-May-19 02:38 torchao/sparsity/prototype/pruner/parametrization.py
--rw-r--r--  2.0 unx    18992 b- defN 24-May-19 02:38 torchao/sparsity/prototype/pruner/prune_functions.py
--rw-r--r--  2.0 unx     1327 b- defN 24-May-19 02:38 torchao/sparsity/prototype/pruner/saliency_pruner.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-19 02:38 torchao/sparsity/prototype/scheduler/__init__.py
--rw-r--r--  2.0 unx     6348 b- defN 24-May-19 02:38 torchao/sparsity/prototype/scheduler/base_scheduler.py
--rw-r--r--  2.0 unx     3873 b- defN 24-May-19 02:38 torchao/sparsity/prototype/scheduler/cubic_scheduler.py
--rw-r--r--  2.0 unx     2018 b- defN 24-May-19 02:38 torchao/sparsity/prototype/scheduler/lambda_scheduler.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-19 02:38 torchao/sparsity/prototype/sparsifier/__init__.py
--rw-r--r--  2.0 unx    13762 b- defN 24-May-19 02:38 torchao/sparsity/prototype/sparsifier/base_sparsifier.py
--rw-r--r--  2.0 unx     2189 b- defN 24-May-19 02:38 torchao/sparsity/prototype/sparsifier/nearly_diagonal_sparsifier.py
--rw-r--r--  2.0 unx     4786 b- defN 24-May-19 02:38 torchao/sparsity/prototype/sparsifier/utils.py
--rw-r--r--  2.0 unx     8853 b- defN 24-May-19 02:38 torchao/sparsity/prototype/sparsifier/weight_norm_sparsifier.py
--rw-r--r--  2.0 unx     1453 b- defN 24-May-19 02:38 torchao_nightly-2024.5.19.dist-info/LICENSE
--rw-r--r--  2.0 unx     7128 b- defN 24-May-19 02:38 torchao_nightly-2024.5.19.dist-info/METADATA
--rw-r--r--  2.0 unx      148 b- defN 24-May-19 02:38 torchao_nightly-2024.5.19.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-May-19 02:38 torchao_nightly-2024.5.19.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     7983 b- defN 24-May-19 02:38 torchao_nightly-2024.5.19.dist-info/RECORD
-107 files, 1377635 bytes uncompressed, 399574 bytes compressed:  71.0%
+Zip file size: 415886 bytes, number of entries: 108
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:57 torchao/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:57 torchao_nightly-2024.5.22.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:57 torchao_nightly.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:57 torchao/csrc/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:57 torchao/dtypes/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:57 torchao/kernel/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:57 torchao/prototype/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:57 torchao/quantization/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:57 torchao/sparsity/
+-rwxr-xr-x  2.0 unx   810656 b- defN 24-May-22 22:57 torchao/_C.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      426 b- defN 24-May-22 22:57 torchao/__init__.py
+-rw-r--r--  2.0 unx     4792 b- defN 24-May-22 22:57 torchao/ops.py
+-rw-r--r--  2.0 unx      860 b- defN 24-May-22 22:57 torchao/utils.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:57 torchao/csrc/cuda/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:57 torchao/csrc/fp6_llm/
+-rw-r--r--  2.0 unx       74 b- defN 24-May-22 22:57 torchao/csrc/init.cpp
+-rw-r--r--  2.0 unx      251 b- defN 24-May-22 22:57 torchao/csrc/nms.cpp
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:57 torchao/csrc/cuda/fp6_llm/
+-rw-r--r--  2.0 unx     5554 b- defN 24-May-22 22:57 torchao/csrc/cuda/nms.cu
+-rw-r--r--  2.0 unx     9437 b- defN 24-May-22 22:57 torchao/csrc/cuda/fp6_llm/fp6_linear.cu
+-rw-r--r--  2.0 unx     9472 b- defN 24-May-22 22:57 torchao/csrc/cuda/fp6_llm/weight_quant.cu
+-rw-r--r--  2.0 unx      479 b- defN 24-May-22 22:57 torchao/csrc/fp6_llm/fp6_llm.cpp
+-rw-r--r--  2.0 unx     9210 b- defN 24-May-22 22:57 torchao/csrc/fp6_llm/weight_prepacking.cpp
+-rw-r--r--  2.0 unx      136 b- defN 24-May-22 22:57 torchao/dtypes/__init__.py
+-rw-r--r--  2.0 unx    33918 b- defN 24-May-22 22:57 torchao/dtypes/nf4tensor.py
+-rw-r--r--  2.0 unx    12448 b- defN 24-May-22 22:57 torchao/dtypes/uint4.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-22 22:57 torchao/kernel/__init__.py
+-rw-r--r--  2.0 unx     7389 b- defN 24-May-22 22:57 torchao/kernel/autotuner.py
+-rw-r--r--  2.0 unx     3238 b- defN 24-May-22 22:57 torchao/kernel/intmm.py
+-rw-r--r--  2.0 unx    11678 b- defN 24-May-22 22:57 torchao/kernel/intmm_triton.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:57 torchao/prototype/common/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:57 torchao/prototype/dora/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:57 torchao/prototype/galore/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:57 torchao/prototype/hqq/
+-rw-r--r--  2.0 unx        0 b- defN 24-May-22 22:57 torchao/prototype/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-22 22:57 torchao/prototype/common/__init__.py
+-rw-r--r--  2.0 unx     7071 b- defN 24-May-22 22:57 torchao/prototype/common/profiling_tools.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:57 torchao/prototype/dora/kernels/
+-rw-r--r--  2.0 unx        0 b- defN 24-May-22 22:57 torchao/prototype/dora/__init__.py
+-rw-r--r--  2.0 unx     6639 b- defN 24-May-22 22:57 torchao/prototype/dora/dora_layer.py
+-rw-r--r--  2.0 unx     3972 b- defN 24-May-22 22:57 torchao/prototype/dora/dora_profile.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-22 22:57 torchao/prototype/dora/kernels/__init__.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-May-22 22:57 torchao/prototype/dora/kernels/common.py
+-rw-r--r--  2.0 unx    15366 b- defN 24-May-22 22:57 torchao/prototype/dora/kernels/custom_autotune.py
+-rw-r--r--  2.0 unx     7641 b- defN 24-May-22 22:57 torchao/prototype/dora/kernels/matmul.py
+-rw-r--r--  2.0 unx    16439 b- defN 24-May-22 22:57 torchao/prototype/dora/kernels/smallk.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:57 torchao/prototype/galore/kernels/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:57 torchao/prototype/galore/optim/
+-rw-r--r--  2.0 unx       23 b- defN 24-May-22 22:57 torchao/prototype/galore/__init__.py
+-rw-r--r--  2.0 unx     3195 b- defN 24-May-22 22:57 torchao/prototype/galore/utils.py
+-rw-r--r--  2.0 unx      210 b- defN 24-May-22 22:57 torchao/prototype/galore/kernels/__init__.py
+-rw-r--r--  2.0 unx    10675 b- defN 24-May-22 22:57 torchao/prototype/galore/kernels/adam_downproj_fused.py
+-rw-r--r--  2.0 unx     4722 b- defN 24-May-22 22:57 torchao/prototype/galore/kernels/adam_step.py
+-rw-r--r--  2.0 unx    15180 b- defN 24-May-22 22:57 torchao/prototype/galore/kernels/custom_autotune.py
+-rw-r--r--  2.0 unx    11641 b- defN 24-May-22 22:57 torchao/prototype/galore/kernels/matmul.py
+-rw-r--r--  2.0 unx     5978 b- defN 24-May-22 22:57 torchao/prototype/galore/kernels/quant.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-22 22:57 torchao/prototype/galore/optim/__init__.py
+-rw-r--r--  2.0 unx    15716 b- defN 24-May-22 22:57 torchao/prototype/galore/optim/galore_torch.py
+-rw-r--r--  2.0 unx       50 b- defN 24-May-22 22:57 torchao/prototype/hqq/__init__.py
+-rw-r--r--  2.0 unx     7658 b- defN 24-May-22 22:57 torchao/prototype/hqq/hqq_tinygemm_linear.py
+-rw-r--r--  2.0 unx    14227 b- defN 24-May-22 22:57 torchao/prototype/hqq/kernels.py
+-rw-r--r--  2.0 unx     5512 b- defN 24-May-22 22:57 torchao/prototype/hqq/mixed_mm.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:57 torchao/quantization/prototype/
+-rw-r--r--  2.0 unx    50342 b- defN 24-May-22 22:57 torchao/quantization/GPTQ.py
+-rw-r--r--  2.0 unx     1700 b- defN 24-May-22 22:57 torchao/quantization/__init__.py
+-rw-r--r--  2.0 unx    19369 b- defN 24-May-22 22:57 torchao/quantization/autoquant.py
+-rw-r--r--  2.0 unx     2747 b- defN 24-May-22 22:57 torchao/quantization/dynamic_quant.py
+-rw-r--r--  2.0 unx     7110 b- defN 24-May-22 22:57 torchao/quantization/quant_api.py
+-rw-r--r--  2.0 unx    32825 b- defN 24-May-22 22:57 torchao/quantization/quant_primitives.py
+-rw-r--r--  2.0 unx     9159 b- defN 24-May-22 22:57 torchao/quantization/smoothquant.py
+-rw-r--r--  2.0 unx    42347 b- defN 24-May-22 22:57 torchao/quantization/subclass.py
+-rw-r--r--  2.0 unx      754 b- defN 24-May-22 22:57 torchao/quantization/unified.py
+-rw-r--r--  2.0 unx     3169 b- defN 24-May-22 22:57 torchao/quantization/utils.py
+-rw-r--r--  2.0 unx     2742 b- defN 24-May-22 22:57 torchao/quantization/weight_only.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-22 22:57 torchao/quantization/prototype/__init__.py
+-rw-r--r--  2.0 unx    12816 b- defN 24-May-22 22:57 torchao/quantization/prototype/qat.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:57 torchao/sparsity/prototype/
+-rw-r--r--  2.0 unx      508 b- defN 24-May-22 22:57 torchao/sparsity/__init__.py
+-rw-r--r--  2.0 unx     1077 b- defN 24-May-22 22:57 torchao/sparsity/sparse_api.py
+-rw-r--r--  2.0 unx     1708 b- defN 24-May-22 22:57 torchao/sparsity/utils.py
+-rw-r--r--  2.0 unx     4156 b- defN 24-May-22 22:57 torchao/sparsity/wanda.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:57 torchao/sparsity/prototype/pruner/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:57 torchao/sparsity/prototype/scheduler/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-22 22:57 torchao/sparsity/prototype/sparsifier/
+-rw-r--r--  2.0 unx      843 b- defN 24-May-22 22:57 torchao/sparsity/prototype/__init__.py
+-rw-r--r--  2.0 unx     9107 b- defN 24-May-22 22:57 torchao/sparsity/prototype/dynamic_quant_sparse.py
+-rw-r--r--  2.0 unx     3388 b- defN 24-May-22 22:57 torchao/sparsity/prototype/pruner/FPGM_pruner.py
+-rw-r--r--  2.0 unx      273 b- defN 24-May-22 22:57 torchao/sparsity/prototype/pruner/__init__.py
+-rw-r--r--  2.0 unx    10873 b- defN 24-May-22 22:57 torchao/sparsity/prototype/pruner/base_structured_sparsifier.py
+-rw-r--r--  2.0 unx     2050 b- defN 24-May-22 22:57 torchao/sparsity/prototype/pruner/lstm_saliency_pruner.py
+-rw-r--r--  2.0 unx     1967 b- defN 24-May-22 22:57 torchao/sparsity/prototype/pruner/match_utils.py
+-rw-r--r--  2.0 unx     1818 b- defN 24-May-22 22:57 torchao/sparsity/prototype/pruner/parametrization.py
+-rw-r--r--  2.0 unx    18992 b- defN 24-May-22 22:57 torchao/sparsity/prototype/pruner/prune_functions.py
+-rw-r--r--  2.0 unx     1327 b- defN 24-May-22 22:57 torchao/sparsity/prototype/pruner/saliency_pruner.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-22 22:57 torchao/sparsity/prototype/scheduler/__init__.py
+-rw-r--r--  2.0 unx     6348 b- defN 24-May-22 22:57 torchao/sparsity/prototype/scheduler/base_scheduler.py
+-rw-r--r--  2.0 unx     3873 b- defN 24-May-22 22:57 torchao/sparsity/prototype/scheduler/cubic_scheduler.py
+-rw-r--r--  2.0 unx     2018 b- defN 24-May-22 22:57 torchao/sparsity/prototype/scheduler/lambda_scheduler.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-22 22:57 torchao/sparsity/prototype/sparsifier/__init__.py
+-rw-r--r--  2.0 unx    13762 b- defN 24-May-22 22:57 torchao/sparsity/prototype/sparsifier/base_sparsifier.py
+-rw-r--r--  2.0 unx     2189 b- defN 24-May-22 22:57 torchao/sparsity/prototype/sparsifier/nearly_diagonal_sparsifier.py
+-rw-r--r--  2.0 unx     4786 b- defN 24-May-22 22:57 torchao/sparsity/prototype/sparsifier/utils.py
+-rw-r--r--  2.0 unx     8853 b- defN 24-May-22 22:57 torchao/sparsity/prototype/sparsifier/weight_norm_sparsifier.py
+-rw-r--r--  2.0 unx     1453 b- defN 24-May-22 22:57 torchao_nightly-2024.5.22.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7128 b- defN 24-May-22 22:57 torchao_nightly-2024.5.22.dist-info/METADATA
+-rw-r--r--  2.0 unx      148 b- defN 24-May-22 22:57 torchao_nightly-2024.5.22.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-22 22:57 torchao_nightly-2024.5.22.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     8056 b- defN 24-May-22 22:57 torchao_nightly-2024.5.22.dist-info/RECORD
+108 files, 1378568 bytes uncompressed, 399954 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
 Filename: torchao/
 Comment: 
 
-Filename: torchao_nightly-2024.5.19.dist-info/
+Filename: torchao_nightly-2024.5.22.dist-info/
 Comment: 
 
 Filename: torchao_nightly.libs/
 Comment: 
 
 Filename: torchao/csrc/
 Comment: 
@@ -30,14 +30,17 @@
 
 Filename: torchao/__init__.py
 Comment: 
 
 Filename: torchao/ops.py
 Comment: 
 
+Filename: torchao/utils.py
+Comment: 
+
 Filename: torchao/csrc/cuda/
 Comment: 
 
 Filename: torchao/csrc/fp6_llm/
 Comment: 
 
 Filename: torchao/csrc/init.cpp
@@ -300,23 +303,23 @@
 
 Filename: torchao/sparsity/prototype/sparsifier/utils.py
 Comment: 
 
 Filename: torchao/sparsity/prototype/sparsifier/weight_norm_sparsifier.py
 Comment: 
 
-Filename: torchao_nightly-2024.5.19.dist-info/LICENSE
+Filename: torchao_nightly-2024.5.22.dist-info/LICENSE
 Comment: 
 
-Filename: torchao_nightly-2024.5.19.dist-info/METADATA
+Filename: torchao_nightly-2024.5.22.dist-info/METADATA
 Comment: 
 
-Filename: torchao_nightly-2024.5.19.dist-info/WHEEL
+Filename: torchao_nightly-2024.5.22.dist-info/WHEEL
 Comment: 
 
-Filename: torchao_nightly-2024.5.19.dist-info/top_level.txt
+Filename: torchao_nightly-2024.5.22.dist-info/top_level.txt
 Comment: 
 
-Filename: torchao_nightly-2024.5.19.dist-info/RECORD
+Filename: torchao_nightly-2024.5.22.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## torchao/_C.cpython-39-x86_64-linux-gnu.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --symbols {}

```diff
@@ -327,89 +327,89 @@
    323: 0000000000018570  1207 FUNC    WEAK   DEFAULT   12 _ZN5torch8autograd13make_variableEN2at6TensorEbb
    324: 000000000001df30    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl16getDefaultStreamENS_6DeviceE
    325: 0000000000015420    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2geERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
    326: 0000000000017030    37 FUNC    WEAK   DEFAULT   12 _ZN3c1015VariableVersion14VersionCounterD0Ev
    327: 00000000000b57b8    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEEE
    328: 0000000000023850  1122 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIN3c108ArgumentESaIS1_EED1Ev
    329: 0000000000016300   164 FUNC    WEAK   DEFAULT   12 _ZN5torch7LibraryD2Ev
-   330: 0000000000035000   109 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE
-   331: 000000000001e350    33 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl12getNewStreamENS_6DeviceEi
-   332: 0000000000015570    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl8floordivERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   333: 000000000001df20    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl12getNewStreamENS_6DeviceEi
-   334: 00000000000251e0    19 FUNC    WEAK   DEFAULT   12 _ZNSt19bad_optional_accessD1Ev
-   335: 00000000000b58d0    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEEE
-   336: 0000000000014ea0    16 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl10nested_intEv
-   337: 00000000000153f0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl4ceilEv
-   338: 000000000001e010     1 FUNC    WEAK   DEFAULT   12 _ZN3c104cuda4impl13CUDAGuardImplD1Ev
-   339: 00000000000172b0   162 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_11SymNodeImplENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev
-   340: 00000000000163b0   307 FUNC    WEAK   DEFAULT   12 _ZN9__gnu_cxx12__to_xstringISscEET_PFiPT0_mPKS2_P13__va_list_tagEmS5_z
-   341: 0000000000020930  1085 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl18uncheckedSetDeviceENS_6DeviceE
-   342: 00000000000178b0   299 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIN3c109AliasInfoESaIS1_EED1Ev
-   343: 0000000000014e80     9 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl20guard_size_obliviousEPKcl
-   344: 00000000000195a0   405 FUNC    GLOBAL DEFAULT   12 _Z13cast_fp16_fp6PtPh
-   345: 00000000000264d0    68 FUNC    WEAK   DEFAULT   12 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EPKS3_OS6_
-   346: 000000000001dff0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl16synchronizeEventEPv
-   347: 000000000001df60    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl11deviceCountEv
-   348: 00000000000b56b0    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEEE
-   349: 000000000001eca0   202 FUNC    WEAK   DEFAULT   12 _ZN3c1014DispatchKeySetC1ENS_11DispatchKeyE
-   350: 000000000001f1a0   853 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKlEE4callERKS3_S5_
-   351: 000000000001a700   951 FUNC    GLOBAL DEFAULT   12 _ZN7torchao25weight_matrix_dequant_cpuEN2at6TensorES1_
-   352: 00000000000b6ec0     0 NOTYPE  GLOBAL DEFAULT   27 _end
-   353: 0000000000015800   164 FUNC    WEAK   DEFAULT   12 _ZN5torch6detail16TorchLibraryInitD1Ev
-   354: 000000000001df70    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl6recordEPPvRKNS_6StreamEaNS_9EventFlagE
-   355: 00000000000251d0     8 FUNC    WEAK   DEFAULT   12 _ZNKSt19bad_optional_access4whatEv
-   356: 00000000000b5420    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1014OperatorKernelE
-   357: 00000000000197f0  2955 FUNC    GLOBAL DEFAULT   12 _Z25DeQuantMatrix_FP6_To_FP16P6__halfPhmmS0_
-   358: 0000000000026600   119 FUNC    WEAK   DEFAULT   12 _ZNSt10_HashtableIP7_objectS1_SaIS1_ENSt8__detail9_IdentityESt8equal_toIS1_ESt4hashIS1_ENS3_18_Mod_range_hashingENS3_20_Default_ranged_hashENS3_20_Prime_rehash_policyENS3_17_Hashtable_traitsILb0ELb1ELb1EEEED1Ev
-   359: 000000000001e760   651 FUNC    WEAK   DEFAULT   12 _ZN3c1010ValueErrorD1Ev
-   360: 000000000001f090   123 FUNC    WEAK   DEFAULT   12 _ZNSt15basic_stringbufIcSt11char_traitsIcESaIcEED2Ev
-   361: 0000000000026da0   354 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIPcSaIS0_EE17_M_realloc_insertIJRKS0_EEEvN9__gnu_cxx17__normal_iteratorIPS0_S2_EEDpOT_
-   362: 0000000000015120    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl5cloneEv
-   363: 00000000000b5488   472 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1011SymNodeImplE
-   364: 000000000001e0f0   269 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl11elapsedTimeEPvS3_a
-   365: 000000000001df40    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl23getStreamFromGlobalPoolENS_6DeviceEb
-   366: 000000000001e040     1 FUNC    WEAK   DEFAULT   12 _ZN3c104impl16VirtualGuardImplD2Ev
-   367: 00000000000348c0    29 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1020intrusive_ptr_targetE
-   368: 00000000000155d0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7truedivERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   369: 0000000000036190    19 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1010ValueErrorE
-   370: 0000000000017010    19 FUNC    WEAK   DEFAULT   12 _ZN3c1015VariableVersion14VersionCounterD1Ev
-   371: 0000000000023850  1122 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIN3c108ArgumentESaIS1_EED2Ev
-   372: 0000000000015c70   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi8EEfEvPK5uint4PK6__halfS7_PT0_mmmi
-   373: 00000000000156c0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7is_boolEv
-   374: 0000000000037720    47 OBJECT  WEAK   DEFAULT   14 _ZTSSt11_Mutex_baseILN9__gnu_cxx12_Lock_policyE2EE
-   375: 0000000000026730    56 FUNC    WEAK   DEFAULT   12 _ZNSt13_Bvector_baseISaIbEE13_M_deallocateEv
-   376: 00000000000251e0    19 FUNC    WEAK   DEFAULT   12 _ZNSt19bad_optional_accessD2Ev
-   377: 0000000000018410    95 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev
-   378: 000000000001e250   113 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl16synchronizeEventEPv
-   379: 00000000000b5688    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1014OperatorKernelE
-   380: 000000000001df80    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl5blockEPvRKNS_6StreamE
-   381: 00000000000184f0   122 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEEC2EPS2_
-   382: 000000000001e010     1 FUNC    WEAK   DEFAULT   12 _ZN3c104cuda4impl13CUDAGuardImplD2Ev
-   383: 0000000000015060    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl9wrap_boolEb
-   384: 000000000001a380   895 FUNC    GLOBAL DEFAULT   12 _ZN7torchao15fp16_to_fp6_cpuEN2at6TensorE
-   385: 0000000000015240    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl13is_contiguousENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
-   386: 0000000000016dc0   338 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKjEE4callERKS3_S5_
-   387: 0000000000022570   482 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl17synchronizeStreamERKNS_6StreamE
-   388: 0000000000015740    29 FUNC    WEAK   DEFAULT   12 _ZN3c1018getFakeTypePtrCopyIlEENS_4Type24SingletonOrSharedTypePtrIS1_EEv
-   389: 0000000000014ec0    16 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl12constant_intEv
-   390: 0000000000023ee0   183 FUNC    GLOBAL DEFAULT   12 _Z20BitInterleaving_4bitPh
-   391: 00000000000178b0   299 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIN3c109AliasInfoESaIS1_EED2Ev
-   392: 00000000000150f0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl9sym_floatEv
-   393: 0000000000021ff0   945 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKNS_10DeviceTypeES3_EE4callERKS3_S6_S9_
-   394: 00000000000362a0    24 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorERKS0_S2_dE
-   395: 000000000001e090    91 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl9setDeviceENS_6DeviceE
-   396: 0000000000014e60     1 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_target17release_resourcesEv
-   397: 00000000000b5948    24 OBJECT  WEAK   DEFAULT   21 _ZTISt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE
-   398: 0000000000018d20   212 FUNC    WEAK   DEFAULT   12 _ZN3c106detail30inferFunctionSchemaFromFunctorIPFN2at6TensorES3_S3_S3_lEEESt10unique_ptrINS_14FunctionSchemaESt14default_deleteIS7_EEv
-   399: 0000000000019740   171 FUNC    GLOBAL DEFAULT   12 _Z29weight_prepacking_fp16_to_fp6PtPhmm
-   400: 0000000000015800   164 FUNC    WEAK   DEFAULT   12 _ZN5torch6detail16TorchLibraryInitD2Ev
-   401: 0000000000015210    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl30is_channels_last_contiguous_2dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
-   402: 000000000001e2e0   106 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl14exchangeStreamENS_6StreamE
-   403: 0000000000016170   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi8EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi
-   404: 000000000001bed0  8158 FUNC    GLOBAL DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220210nms_kernelERKN2at6TensorES4_d
+   330: 000000000001e5c0   204 FUNC    WEAK   DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py
+   331: 0000000000035000   109 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE
+   332: 000000000001e350    33 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl12getNewStreamENS_6DeviceEi
+   333: 0000000000015570    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl8floordivERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   334: 000000000001df20    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl12getNewStreamENS_6DeviceEi
+   335: 00000000000251e0    19 FUNC    WEAK   DEFAULT   12 _ZNSt19bad_optional_accessD1Ev
+   336: 00000000000b58d0    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEEE
+   337: 0000000000014ea0    16 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl10nested_intEv
+   338: 00000000000153f0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl4ceilEv
+   339: 000000000001e010     1 FUNC    WEAK   DEFAULT   12 _ZN3c104cuda4impl13CUDAGuardImplD1Ev
+   340: 00000000000172b0   162 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_11SymNodeImplENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev
+   341: 00000000000163b0   307 FUNC    WEAK   DEFAULT   12 _ZN9__gnu_cxx12__to_xstringISscEET_PFiPT0_mPKS2_P13__va_list_tagEmS5_z
+   342: 0000000000020930  1085 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl18uncheckedSetDeviceENS_6DeviceE
+   343: 00000000000178b0   299 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIN3c109AliasInfoESaIS1_EED1Ev
+   344: 0000000000014e80     9 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl20guard_size_obliviousEPKcl
+   345: 00000000000195a0   405 FUNC    GLOBAL DEFAULT   12 _Z13cast_fp16_fp6PtPh
+   346: 00000000000264d0    68 FUNC    WEAK   DEFAULT   12 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EPKS3_OS6_
+   347: 000000000001dff0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl16synchronizeEventEPv
+   348: 000000000001df60    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl11deviceCountEv
+   349: 00000000000b56b0    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEEE
+   350: 000000000001eca0   202 FUNC    WEAK   DEFAULT   12 _ZN3c1014DispatchKeySetC1ENS_11DispatchKeyE
+   351: 000000000001f1a0   853 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKlEE4callERKS3_S5_
+   352: 000000000001a700   951 FUNC    GLOBAL DEFAULT   12 _ZN7torchao25weight_matrix_dequant_cpuEN2at6TensorES1_
+   353: 00000000000b6ec0     0 NOTYPE  GLOBAL DEFAULT   27 _end
+   354: 0000000000015800   164 FUNC    WEAK   DEFAULT   12 _ZN5torch6detail16TorchLibraryInitD1Ev
+   355: 000000000001df70    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl6recordEPPvRKNS_6StreamEaNS_9EventFlagE
+   356: 00000000000251d0     8 FUNC    WEAK   DEFAULT   12 _ZNKSt19bad_optional_access4whatEv
+   357: 00000000000b5420    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1014OperatorKernelE
+   358: 00000000000197f0  2955 FUNC    GLOBAL DEFAULT   12 _Z25DeQuantMatrix_FP6_To_FP16P6__halfPhmmS0_
+   359: 0000000000026600   119 FUNC    WEAK   DEFAULT   12 _ZNSt10_HashtableIP7_objectS1_SaIS1_ENSt8__detail9_IdentityESt8equal_toIS1_ESt4hashIS1_ENS3_18_Mod_range_hashingENS3_20_Default_ranged_hashENS3_20_Prime_rehash_policyENS3_17_Hashtable_traitsILb0ELb1ELb1EEEED1Ev
+   360: 000000000001e760   651 FUNC    WEAK   DEFAULT   12 _ZN3c1010ValueErrorD1Ev
+   361: 000000000001f090   123 FUNC    WEAK   DEFAULT   12 _ZNSt15basic_stringbufIcSt11char_traitsIcESaIcEED2Ev
+   362: 0000000000026da0   354 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIPcSaIS0_EE17_M_realloc_insertIJRKS0_EEEvN9__gnu_cxx17__normal_iteratorIPS0_S2_EEDpOT_
+   363: 0000000000015120    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl5cloneEv
+   364: 00000000000b5488   472 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1011SymNodeImplE
+   365: 000000000001e0f0   269 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl11elapsedTimeEPvS3_a
+   366: 000000000001df40    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl23getStreamFromGlobalPoolENS_6DeviceEb
+   367: 000000000001e040     1 FUNC    WEAK   DEFAULT   12 _ZN3c104impl16VirtualGuardImplD2Ev
+   368: 00000000000348c0    29 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1020intrusive_ptr_targetE
+   369: 00000000000155d0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7truedivERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   370: 0000000000036190    19 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1010ValueErrorE
+   371: 0000000000017010    19 FUNC    WEAK   DEFAULT   12 _ZN3c1015VariableVersion14VersionCounterD1Ev
+   372: 0000000000023850  1122 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIN3c108ArgumentESaIS1_EED2Ev
+   373: 0000000000015c70   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi8EEfEvPK5uint4PK6__halfS7_PT0_mmmi
+   374: 00000000000156c0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7is_boolEv
+   375: 0000000000037720    47 OBJECT  WEAK   DEFAULT   14 _ZTSSt11_Mutex_baseILN9__gnu_cxx12_Lock_policyE2EE
+   376: 0000000000026730    56 FUNC    WEAK   DEFAULT   12 _ZNSt13_Bvector_baseISaIbEE13_M_deallocateEv
+   377: 00000000000251e0    19 FUNC    WEAK   DEFAULT   12 _ZNSt19bad_optional_accessD2Ev
+   378: 0000000000018410    95 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev
+   379: 000000000001e250   113 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl16synchronizeEventEPv
+   380: 00000000000b5688    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1014OperatorKernelE
+   381: 000000000001df80    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl5blockEPvRKNS_6StreamE
+   382: 00000000000184f0   122 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEEC2EPS2_
+   383: 000000000001e010     1 FUNC    WEAK   DEFAULT   12 _ZN3c104cuda4impl13CUDAGuardImplD2Ev
+   384: 0000000000015060    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl9wrap_boolEb
+   385: 000000000001a380   895 FUNC    GLOBAL DEFAULT   12 _ZN7torchao15fp16_to_fp6_cpuEN2at6TensorE
+   386: 0000000000015240    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl13is_contiguousENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
+   387: 0000000000016dc0   338 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKjEE4callERKS3_S5_
+   388: 0000000000022570   482 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl17synchronizeStreamERKNS_6StreamE
+   389: 0000000000015740    29 FUNC    WEAK   DEFAULT   12 _ZN3c1018getFakeTypePtrCopyIlEENS_4Type24SingletonOrSharedTypePtrIS1_EEv
+   390: 0000000000014ec0    16 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl12constant_intEv
+   391: 0000000000023ee0   183 FUNC    GLOBAL DEFAULT   12 _Z20BitInterleaving_4bitPh
+   392: 00000000000178b0   299 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIN3c109AliasInfoESaIS1_EED2Ev
+   393: 00000000000150f0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl9sym_floatEv
+   394: 0000000000021ff0   945 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKNS_10DeviceTypeES3_EE4callERKS3_S6_S9_
+   395: 00000000000362a0    24 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorERKS0_S2_dE
+   396: 000000000001e090    91 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl9setDeviceENS_6DeviceE
+   397: 0000000000014e60     1 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_target17release_resourcesEv
+   398: 00000000000b5948    24 OBJECT  WEAK   DEFAULT   21 _ZTISt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE
+   399: 0000000000018d20   212 FUNC    WEAK   DEFAULT   12 _ZN3c106detail30inferFunctionSchemaFromFunctorIPFN2at6TensorES3_S3_S3_lEEESt10unique_ptrINS_14FunctionSchemaESt14default_deleteIS7_EEv
+   400: 0000000000019740   171 FUNC    GLOBAL DEFAULT   12 _Z29weight_prepacking_fp16_to_fp6PtPhmm
+   401: 0000000000015800   164 FUNC    WEAK   DEFAULT   12 _ZN5torch6detail16TorchLibraryInitD2Ev
+   402: 0000000000015210    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl30is_channels_last_contiguous_2dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
+   403: 000000000001e2e0   106 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl14exchangeStreamENS_6StreamE
+   404: 0000000000016170   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi8EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi
    405: 0000000000017480    95 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEE6reset_Ev
    406: 00000000000153c0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl5floorEv
    407: 0000000000014fd0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11guard_floatEPKcl
    408: 000000000001e760   651 FUNC    WEAK   DEFAULT   12 _ZN3c1010ValueErrorD2Ev
    409: 00000000000b6a80     0 NOTYPE  GLOBAL DEFAULT   26 _edata
    410: 0000000000026600   119 FUNC    WEAK   DEFAULT   12 _ZNSt10_HashtableIP7_objectS1_SaIS1_ENSt8__detail9_IdentityESt8equal_toIS1_ESt4hashIS1_ENS3_18_Mod_range_hashingENS3_20_Default_ranged_hashENS3_20_Prime_rehash_policyENS3_17_Hashtable_traitsILb0ELb1ELb1EEEED2Ev
    411: 0000000000035120    21 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorES0_S0_E
@@ -431,162 +431,162 @@
    427: 0000000000015540    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3modERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
    428: 0000000000026b30   109 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIbSaIbEE9push_backEb
    429: 0000000000026570   141 FUNC    WEAK   DEFAULT   12 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EPKS3_RKS6_
    430: 00000000000242a0  1638 FUNC    GLOBAL DEFAULT   12 _Z24weight_matrix_prepackingPiS_mm
    431: 0000000000025370   167 FUNC    WEAK   DEFAULT   12 _ZN3c106detail30inferFunctionSchemaFromFunctorIPFN2at6TensorES3_EEESt10unique_ptrINS_14FunctionSchemaESt14default_deleteIS7_EEv
    432: 000000000001aac0  1331 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKNS_10ScalarTypeES3_EE4callERKS3_S6_S9_
    433: 00000000000152d0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7sym_andERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   434: 000000000001e690   204 FUNC    WEAK   DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py
-   435: 00000000000162b0    70 FUNC    WEAK   DEFAULT   12 _ZNK3c1010TensorImpl6deviceEv
-   436: 00000000000272f0   354 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIP11_typeobjectSaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_
-   437: 000000000001f500   917 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKS3_EE4callES5_S5_
-   438: 000000000001dfd0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl21recordDataPtrOnStreamERKNS_7DataPtrERKNS_6StreamE
-   439: 0000000000013990  3958 FUNC    GLOBAL DEFAULT   12 _Z17fp6_linear_kernelP11CUstream_stPK5uint4PK6__halfS6_PS4_mmmPfi
-   440: 000000000001dfa0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl12destroyEventEPva
-   441: 000000000001e450    29 FUNC    WEAK   DEFAULT   12 _ZN3c1018getFakeTypePtrCopyIdEENS_4Type24SingletonOrSharedTypePtrIS1_EEv
-   442: 000000000001e380    34 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl23getStreamFromGlobalPoolENS_6DeviceEb
-   443: 000000000001b7e0   606 FUNC    WEAK   DEFAULT   12 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_ES5_NS_4guts8typelist8typelistIJS5_EEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE
-   444: 0000000000018470   122 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEEC2EPS1_
-   445: 0000000000014e90     9 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11expect_trueEPKcl
-   446: 0000000000016b10   684 FUNC    WEAK   DEFAULT   12 _ZN2at5emptyEN3c108ArrayRefIlEENS0_13TensorOptionsESt8optionalINS0_12MemoryFormatEE
-   447: 0000000000014f40    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl8has_hintEv
-   448: 0000000000015180    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl27is_channels_last_strides_3dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
-   449: 0000000000022760   945 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKlS3_EE4callERKS3_S5_S8_
-   450: 0000000000015760    70 FUNC    WEAK   DEFAULT   12 _ZN3c1014getTypePtrCopyIN2at6TensorEEENS_4Type24SingletonOrSharedTypePtrIS3_EEv
-   451: 00000000000184f0   122 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEEC1EPS2_
-   452: 0000000000015db0   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi
-   453: 0000000000015690    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl8is_floatEv
-   454: 00000000000201d0  1882 FUNC    WEAK   DEFAULT   12 _ZN2at8indexing11TensorIndexD1Ev
-   455: 000000000001dfe0    16 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl11elapsedTimeEPvS2_a
-   456: 0000000000017100    19 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImplD1Ev
-   457: 0000000000017630   552 FUNC    WEAK   DEFAULT   12 _ZSt11make_uniqueIN5torch8autograd12AutogradMetaEJPN3c1010TensorImplERbEENSt9_MakeUniqIT_E15__single_objectEDpOT0_
-   458: 000000000001b070    37 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED0Ev
-   459: 0000000000023cc0   126 FUNC    GLOBAL DEFAULT   12 _Z24Padding_8_FP6_To_8_BytesPhS_
-   460: 00000000000154e0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2neERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   461: 0000000000020100   205 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEED0Ev
-   462: 0000000000022f80  2042 FUNC    WEAK   DEFAULT   12 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS5_S7_dES5_NS_4guts8typelist8typelistIJS7_S7_dEEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISN_EE
-   463: 0000000000017860    74 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_10TensorImplENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev
-   464: 00000000000348e0    20 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1011SymNodeImplE
-   465: 0000000000018b50   458 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIN3c106IValueESaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_
-   466: 000000000001ed70   223 FUNC    WEAK   DEFAULT   12 _ZNK3c1010TensorImpl4sizeEl
-   467: 00000000000b5660    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1015VariableVersion14VersionCounterE
-   468: 00000000000b53e0    16 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1020intrusive_ptr_targetE
-   469: 000000000001ee50   561 FUNC    WEAK   DEFAULT   12 _ZNK2at10TensorBase7optionsEv
-   470: 0000000000014f00     6 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11is_symbolicEv
-   471: 00000000000170d0    37 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED0Ev
-   472: 000000000001fc50   979 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl6recordEPPvRKNS_6StreamEaNS_9EventFlagE
-   473: 000000000001e4f0   204 FUNC    WEAK   DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py
-   474: 0000000000032c5c     0 FUNC    GLOBAL DEFAULT   13 _fini
-   475: 0000000000014ed0     5 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl13constant_boolEv
-   476: 00000000000349e0    25 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorES0_S0_S0_lE
-   477: 00000000000361c0    38 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104impl24DeviceGuardImplInterfaceE
-   478: 0000000000014ef0     3 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11is_constantEv
-   479: 0000000000036220   119 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEEE
-   480: 00000000000377a0    52 OBJECT  WEAK   DEFAULT   14 _ZTSSt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE
-   481: 000000000001e490    86 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl10queryEventEPv
-   482: 0000000000034900    40 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1015VariableVersion14VersionCounterE
-   483: 0000000000010000     0 FUNC    GLOBAL DEFAULT    9 _init
-   484: 00000000000155a0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3powERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   485: 00000000000169d0   318 FUNC    WEAK   DEFAULT   12 _ZN3c106IValue7destroyEv
-   486: 0000000000015330    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7sym_maxERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   487: 00000000000174e0    82 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_10TensorImplENS_19UndefinedTensorImplEE6reset_Ev
-   488: 000000000001ded0    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl14exchangeDeviceENS_6DeviceE
-   489: 0000000000015090    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl10wrap_floatEd
-   490: 0000000000017100    19 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImplD2Ev
-   491: 000000000001eca0   202 FUNC    WEAK   DEFAULT   12 _ZN3c1014DispatchKeySetC2ENS_11DispatchKeyE
-   492: 00000000000b5750    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE
-   493: 00000000000201d0  1882 FUNC    WEAK   DEFAULT   12 _ZN2at8indexing11TensorIndexD2Ev
-   494: 000000000001b050    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED1Ev
-   495: 0000000000020030   197 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEED1Ev
-   496: 00000000000b5938    16 OBJECT  WEAK   DEFAULT   21 _ZTISt11_Mutex_baseILN9__gnu_cxx12_Lock_policyE2EE
-   497: 0000000000034960   123 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEEE
-   498: 000000000001def0    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl9setDeviceENS_6DeviceE
-   499: 000000000001e050    31 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl9getStreamENS_6DeviceE
-   500: 0000000000015000    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl10guard_boolEPKcl
-   501: 0000000000026520    66 FUNC    WEAK   DEFAULT   12 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EOS6_PKS3_
-   502: 00000000000b5790    16 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104impl24DeviceGuardImplInterfaceE
-   503: 0000000000017400   123 FUNC    WEAK   DEFAULT   12 _ZNSt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE10_M_releaseEv
-   504: 0000000000024910  2235 FUNC    GLOBAL DEFAULT   12 _ZN7torchao28weight_matrix_prepacking_cpuEN2at6TensorE
-   505: 0000000000023d40    28 FUNC    GLOBAL DEFAULT   12 _Z31Extract_2_Bits_From_4_PaddedFP6hhhh
-   506: 0000000000018470   122 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEEC1EPS1_
-   507: 0000000000015270    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7sym_iteERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEES7_
-   508: 0000000000015030    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl9guard_intEPKcl
-   509: 00000000000b57d0    16 OBJECT  WEAK   DEFAULT   21 _ZTIFN2at6TensorERKS0_S2_dE
-   510: 00000000000170b0    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED1Ev
-   511: 0000000000016ff0    23 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_targetD0Ev
-   512: 0000000000016030   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi
-   513: 00000000000179e0  2600 FUNC    WEAK   DEFAULT   12 _ZN3c1014FunctionSchemaD1Ev
-   514: 000000000001b020    37 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEED0Ev
-   515: 00000000000b6a80     0 NOTYPE  GLOBAL DEFAULT   27 __bss_start
-   516: 0000000000017360   155 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11expect_sizeEPKcl
-   517: 0000000000025c90    43 FUNC    WEAK   DEFAULT   12 _ZNKSt9type_info9hash_codeEv
-   518: 00000000000b6ce4     4 OBJECT  UNIQUE DEFAULT   27 _ZZN3c104cuda13warning_stateEvE14warning_state_
-   519: 0000000000023d80   341 FUNC    GLOBAL DEFAULT   12 _Z20BitInterleaving_2bitPh
-   520: 00000000000b56f0    16 OBJECT  WEAK   DEFAULT   21 _ZTIFN2at6TensorES0_E
-   521: 0000000000015510    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2eqERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   522: 00000000000152a0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7sym_notEv
-   523: 0000000000017080    37 FUNC    WEAK   DEFAULT   12 _ZN3c1014OperatorKernelD0Ev
-   524: 000000000001b4f0   751 FUNC    WEAK   DEFAULT   12 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_ES5_NS_4guts8typelist8typelistIJS5_S5_EEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE
-   525: 0000000000027630  1684 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIbSaIbEE14_M_fill_insertESt13_Bit_iteratormb
+   434: 00000000000162b0    70 FUNC    WEAK   DEFAULT   12 _ZNK3c1010TensorImpl6deviceEv
+   435: 00000000000272f0   354 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIP11_typeobjectSaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_
+   436: 000000000001f500   917 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKS3_EE4callES5_S5_
+   437: 000000000001dfd0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl21recordDataPtrOnStreamERKNS_7DataPtrERKNS_6StreamE
+   438: 0000000000013990  3958 FUNC    GLOBAL DEFAULT   12 _Z17fp6_linear_kernelP11CUstream_stPK5uint4PK6__halfS6_PS4_mmmPfi
+   439: 000000000001dfa0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl12destroyEventEPva
+   440: 000000000001e450    29 FUNC    WEAK   DEFAULT   12 _ZN3c1018getFakeTypePtrCopyIdEENS_4Type24SingletonOrSharedTypePtrIS1_EEv
+   441: 000000000001e380    34 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl23getStreamFromGlobalPoolENS_6DeviceEb
+   442: 000000000001b7e0   606 FUNC    WEAK   DEFAULT   12 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_ES5_NS_4guts8typelist8typelistIJS5_EEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE
+   443: 0000000000018470   122 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEEC2EPS1_
+   444: 0000000000014e90     9 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11expect_trueEPKcl
+   445: 0000000000016b10   684 FUNC    WEAK   DEFAULT   12 _ZN2at5emptyEN3c108ArrayRefIlEENS0_13TensorOptionsESt8optionalINS0_12MemoryFormatEE
+   446: 0000000000014f40    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl8has_hintEv
+   447: 0000000000015180    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl27is_channels_last_strides_3dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
+   448: 0000000000022760   945 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKlS3_EE4callERKS3_S5_S8_
+   449: 0000000000015760    70 FUNC    WEAK   DEFAULT   12 _ZN3c1014getTypePtrCopyIN2at6TensorEEENS_4Type24SingletonOrSharedTypePtrIS3_EEv
+   450: 00000000000184f0   122 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEEC1EPS2_
+   451: 0000000000015db0   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi
+   452: 0000000000015690    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl8is_floatEv
+   453: 00000000000201d0  1882 FUNC    WEAK   DEFAULT   12 _ZN2at8indexing11TensorIndexD1Ev
+   454: 000000000001dfe0    16 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl11elapsedTimeEPvS2_a
+   455: 0000000000017100    19 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImplD1Ev
+   456: 0000000000017630   552 FUNC    WEAK   DEFAULT   12 _ZSt11make_uniqueIN5torch8autograd12AutogradMetaEJPN3c1010TensorImplERbEENSt9_MakeUniqIT_E15__single_objectEDpOT0_
+   457: 000000000001b070    37 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED0Ev
+   458: 0000000000023cc0   126 FUNC    GLOBAL DEFAULT   12 _Z24Padding_8_FP6_To_8_BytesPhS_
+   459: 00000000000154e0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2neERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   460: 0000000000020100   205 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEED0Ev
+   461: 0000000000022f80  2042 FUNC    WEAK   DEFAULT   12 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS5_S7_dES5_NS_4guts8typelist8typelistIJS7_S7_dEEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISN_EE
+   462: 0000000000017860    74 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_10TensorImplENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev
+   463: 00000000000348e0    20 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1011SymNodeImplE
+   464: 0000000000018b50   458 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIN3c106IValueESaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_
+   465: 000000000001ed70   223 FUNC    WEAK   DEFAULT   12 _ZNK3c1010TensorImpl4sizeEl
+   466: 00000000000b5660    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1015VariableVersion14VersionCounterE
+   467: 00000000000b53e0    16 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1020intrusive_ptr_targetE
+   468: 000000000001ee50   561 FUNC    WEAK   DEFAULT   12 _ZNK2at10TensorBase7optionsEv
+   469: 0000000000014f00     6 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11is_symbolicEv
+   470: 00000000000170d0    37 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED0Ev
+   471: 000000000001fc50   979 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl6recordEPPvRKNS_6StreamEaNS_9EventFlagE
+   472: 0000000000032c5c     0 FUNC    GLOBAL DEFAULT   13 _fini
+   473: 0000000000014ed0     5 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl13constant_boolEv
+   474: 00000000000349e0    25 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorES0_S0_S0_lE
+   475: 00000000000361c0    38 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104impl24DeviceGuardImplInterfaceE
+   476: 0000000000014ef0     3 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11is_constantEv
+   477: 0000000000036220   119 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEEE
+   478: 00000000000377a0    52 OBJECT  WEAK   DEFAULT   14 _ZTSSt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE
+   479: 000000000001e490    86 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl10queryEventEPv
+   480: 0000000000034900    40 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1015VariableVersion14VersionCounterE
+   481: 0000000000010000     0 FUNC    GLOBAL DEFAULT    9 _init
+   482: 00000000000155a0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3powERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   483: 00000000000169d0   318 FUNC    WEAK   DEFAULT   12 _ZN3c106IValue7destroyEv
+   484: 0000000000015330    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7sym_maxERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   485: 00000000000174e0    82 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_10TensorImplENS_19UndefinedTensorImplEE6reset_Ev
+   486: 000000000001ded0    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl14exchangeDeviceENS_6DeviceE
+   487: 0000000000015090    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl10wrap_floatEd
+   488: 0000000000017100    19 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImplD2Ev
+   489: 000000000001eca0   202 FUNC    WEAK   DEFAULT   12 _ZN3c1014DispatchKeySetC2ENS_11DispatchKeyE
+   490: 00000000000b5750    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE
+   491: 00000000000201d0  1882 FUNC    WEAK   DEFAULT   12 _ZN2at8indexing11TensorIndexD2Ev
+   492: 000000000001b050    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED1Ev
+   493: 0000000000020030   197 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEED1Ev
+   494: 00000000000b5938    16 OBJECT  WEAK   DEFAULT   21 _ZTISt11_Mutex_baseILN9__gnu_cxx12_Lock_policyE2EE
+   495: 0000000000034960   123 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEEE
+   496: 000000000001def0    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl9setDeviceENS_6DeviceE
+   497: 000000000001e050    31 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl9getStreamENS_6DeviceE
+   498: 0000000000015000    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl10guard_boolEPKcl
+   499: 0000000000026520    66 FUNC    WEAK   DEFAULT   12 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EOS6_PKS3_
+   500: 00000000000b5790    16 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104impl24DeviceGuardImplInterfaceE
+   501: 0000000000017400   123 FUNC    WEAK   DEFAULT   12 _ZNSt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE10_M_releaseEv
+   502: 0000000000024910  2235 FUNC    GLOBAL DEFAULT   12 _ZN7torchao28weight_matrix_prepacking_cpuEN2at6TensorE
+   503: 0000000000023d40    28 FUNC    GLOBAL DEFAULT   12 _Z31Extract_2_Bits_From_4_PaddedFP6hhhh
+   504: 0000000000018470   122 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEEC1EPS1_
+   505: 0000000000015270    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7sym_iteERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEES7_
+   506: 0000000000015030    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl9guard_intEPKcl
+   507: 00000000000b57d0    16 OBJECT  WEAK   DEFAULT   21 _ZTIFN2at6TensorERKS0_S2_dE
+   508: 00000000000170b0    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED1Ev
+   509: 0000000000016ff0    23 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_targetD0Ev
+   510: 0000000000016030   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi
+   511: 00000000000179e0  2600 FUNC    WEAK   DEFAULT   12 _ZN3c1014FunctionSchemaD1Ev
+   512: 000000000001b020    37 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEED0Ev
+   513: 00000000000b6a80     0 NOTYPE  GLOBAL DEFAULT   27 __bss_start
+   514: 0000000000017360   155 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11expect_sizeEPKcl
+   515: 0000000000025c90    43 FUNC    WEAK   DEFAULT   12 _ZNKSt9type_info9hash_codeEv
+   516: 00000000000b6ce4     4 OBJECT  UNIQUE DEFAULT   27 _ZZN3c104cuda13warning_stateEvE14warning_state_
+   517: 0000000000023d80   341 FUNC    GLOBAL DEFAULT   12 _Z20BitInterleaving_2bitPh
+   518: 00000000000b56f0    16 OBJECT  WEAK   DEFAULT   21 _ZTIFN2at6TensorES0_E
+   519: 0000000000015510    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2eqERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   520: 00000000000152a0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7sym_notEv
+   521: 0000000000017080    37 FUNC    WEAK   DEFAULT   12 _ZN3c1014OperatorKernelD0Ev
+   522: 000000000001b4f0   751 FUNC    WEAK   DEFAULT   12 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_ES5_NS_4guts8typelist8typelistIJS5_S5_EEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE
+   523: 0000000000027630  1684 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIbSaIbEE14_M_fill_insertESt13_Bit_iteratormb
+   524: 000000000001e690   204 FUNC    WEAK   DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py
+   525: 000000000001e4f0   204 FUNC    WEAK   DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py
    526: 000000000001b0a0   101 FUNC    WEAK   DEFAULT   12 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_ES5_NS_4guts8typelist8typelistIJS5_EEEEES6_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES5_
    527: 0000000000015300    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl6sym_orERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
    528: 000000000001dec0     9 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl4typeEv
    529: 0000000000025230   311 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIhSaIhEE17_M_realloc_insertIJRKhEEEvN9__gnu_cxx17__normal_iteratorIPhS1_EEDpOT_
-   530: 000000000001e5c0   204 FUNC    WEAK   DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py
-   531: 0000000000015480    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2ltERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   532: 000000000001df90    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl10queryEventEPv
-   533: 000000000001fa40   528 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl5blockEPvRKNS_6StreamE
-   534: 0000000000015600    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3mulERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   535: 000000000001e020    24 FUNC    WEAK   DEFAULT   12 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS5_S7_dES5_NS_4guts8typelist8typelistIJS7_S7_dEEEEES8_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES7_S7_d
-   536: 00000000000b58f8    24 OBJECT  WEAK   DEFAULT   21 _ZTISt19bad_optional_access
-   537: 000000000001b050    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED2Ev
-   538: 00000000000151b0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl27is_channels_last_strides_2dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
-   539: 0000000000020030   197 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEED2Ev
-   540: 0000000000013980     5 FUNC    GLOBAL DEFAULT   12 _Z16SplitK_ReductionP6__halfPfmmi
-   541: 000000000002b6b0   478 FUNC    WEAK   DEFAULT   12 _ZNSt8__detail9_Map_baseISsSt4pairIKSsPvESaIS4_ENS_10_Select1stESt8equal_toISsESt4hashISsENS_18_Mod_range_hashingENS_20_Default_ranged_hashENS_20_Prime_rehash_policyENS_17_Hashtable_traitsILb1ELb0ELb1EEELb1EEixEOSs
-   542: 000000000001e200    68 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl21recordDataPtrOnStreamERKNS_7DataPtrERKNS_6StreamE
-   543: 000000000001e000     6 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl4typeEv
-   544: 00000000000b5700    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE
-   545: 0000000000014f70    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl5bool_Ev
-   546: 00000000000350a0   115 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE
-   547: 0000000000026770   959 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIbSaIbEE13_M_insert_auxESt13_Bit_iteratorb
-   548: 00000000000b57e0    48 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1010ValueErrorE
-   549: 00000000000158b0   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EEfEvPK5uint4PK6__halfS7_PT0_mmmi
-   550: 0000000000035070    18 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorES0_E
-   551: 0000000000034930    23 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1014OperatorKernelE
-   552: 0000000000026470    95 FUNC    WEAK   DEFAULT   12 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EOS6_S7_
-   553: 000000000001e3b0    31 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl16getDefaultStreamENS_6DeviceE
-   554: 00000000000154b0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2gtERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   555: 000000000001dfc0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl17synchronizeStreamERKNS_6StreamE
-   556: 00000000000b5728    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE
-   557: 00000000000170b0    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED2Ev
-   558: 00000000000b5408    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1015VariableVersion14VersionCounterE
-   559: 0000000000015390    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3negEv
-   560: 0000000000016f20   197 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_targetD1Ev
-   561: 00000000000179e0  2600 FUNC    WEAK   DEFAULT   12 _ZN3c1014FunctionSchemaD2Ev
-   562: 0000000000014910  1355 FUNC    GLOBAL DEFAULT   12 _ZN7torchao23fp6_linear_forward_cudaEN2at6TensorES1_S1_l
-   563: 000000000001b000    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEED1Ev
-   564: 000000000001e2d0     5 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl11deviceCountEv
-   565: 00000000000b5810   192 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104cuda4impl13CUDAGuardImplE
-   566: 0000000000014fa0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl4int_Ev
-   567: 0000000000015720    29 FUNC    WEAK   DEFAULT   12 _ZN3c1014getTypePtrCopyIlEENS_4Type24SingletonOrSharedTypePtrIS1_EEv
-   568: 000000000001df00    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl18uncheckedSetDeviceENS_6DeviceE
-   569: 0000000000017540   237 FUNC    WEAK   DEFAULT   12 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_S5_lES5_NS_4guts8typelist8typelistIJS5_S5_S5_lEEEEES6_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES5_S5_S5_l
-   570: 0000000000013890   228 FUNC    GLOBAL DEFAULT   12 _Z47__device_stub__Z16SplitK_ReductionP6__halfPfmmiP6__halfPfmmi
-   571: 000000000001f8a0   193 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl9getDeviceEv
-   572: 0000000000017060    19 FUNC    WEAK   DEFAULT   12 _ZN3c1014OperatorKernelD1Ev
-   573: 0000000000018e00  1012 FUNC    WEAK   DEFAULT   12 _ZN3c104impl34call_functor_with_args_from_stack_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_S5_lES5_NS_4guts8typelist8typelistIJS5_S5_S5_lEEEEELb0EJLm0ELm1ELm2ELm3EEJS5_S5_S5_lEEENSt5decayINS8_21infer_function_traitsIT_E4type11return_typeEE4typeEPNS_14OperatorKernelENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISP_EESt16integer_sequenceImJXspT1_EEEPNSA_IJDpT2_EEE
-   574: 00000000000b56d8    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE
-   575: 00000000000164f0   896 FUNC    WEAK   DEFAULT   12 _ZNK3c106IValue7tagKindEv
-   576: 0000000000015ef0   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi2EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi
-   577: 000000000001f110   139 FUNC    WEAK   DEFAULT   12 _ZNSt15basic_stringbufIcSt11char_traitsIcESaIcEED0Ev
-   578: 000000000001e080    10 FUNC    WEAK   DEFAULT   12 _ZN3c104impl16VirtualGuardImplD0Ev
-   579: 0000000000036200    32 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104cuda4impl13CUDAGuardImplE
-   580: 0000000000022b20  1113 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJRKcRKPS2_S4_S6_S4_EE4callES3_S6_S6_S6_S6_
-   581: 0000000000015660    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3addERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   530: 0000000000015480    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2ltERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   531: 000000000001df90    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl10queryEventEPv
+   532: 000000000001fa40   528 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl5blockEPvRKNS_6StreamE
+   533: 0000000000015600    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3mulERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   534: 000000000001e020    24 FUNC    WEAK   DEFAULT   12 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS5_S7_dES5_NS_4guts8typelist8typelistIJS7_S7_dEEEEES8_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES7_S7_d
+   535: 00000000000b58f8    24 OBJECT  WEAK   DEFAULT   21 _ZTISt19bad_optional_access
+   536: 000000000001b050    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED2Ev
+   537: 00000000000151b0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl27is_channels_last_strides_2dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
+   538: 0000000000020030   197 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEED2Ev
+   539: 0000000000013980     5 FUNC    GLOBAL DEFAULT   12 _Z16SplitK_ReductionP6__halfPfmmi
+   540: 000000000002b6b0   478 FUNC    WEAK   DEFAULT   12 _ZNSt8__detail9_Map_baseISsSt4pairIKSsPvESaIS4_ENS_10_Select1stESt8equal_toISsESt4hashISsENS_18_Mod_range_hashingENS_20_Default_ranged_hashENS_20_Prime_rehash_policyENS_17_Hashtable_traitsILb1ELb0ELb1EEELb1EEixEOSs
+   541: 000000000001e200    68 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl21recordDataPtrOnStreamERKNS_7DataPtrERKNS_6StreamE
+   542: 000000000001e000     6 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl4typeEv
+   543: 00000000000b5700    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE
+   544: 0000000000014f70    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl5bool_Ev
+   545: 00000000000350a0   115 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE
+   546: 0000000000026770   959 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIbSaIbEE13_M_insert_auxESt13_Bit_iteratorb
+   547: 00000000000b57e0    48 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1010ValueErrorE
+   548: 00000000000158b0   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EEfEvPK5uint4PK6__halfS7_PT0_mmmi
+   549: 0000000000035070    18 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorES0_E
+   550: 0000000000034930    23 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1014OperatorKernelE
+   551: 0000000000026470    95 FUNC    WEAK   DEFAULT   12 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EOS6_S7_
+   552: 000000000001e3b0    31 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl16getDefaultStreamENS_6DeviceE
+   553: 00000000000154b0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2gtERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   554: 000000000001dfc0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl17synchronizeStreamERKNS_6StreamE
+   555: 00000000000b5728    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE
+   556: 00000000000170b0    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED2Ev
+   557: 00000000000b5408    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1015VariableVersion14VersionCounterE
+   558: 0000000000015390    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3negEv
+   559: 0000000000016f20   197 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_targetD1Ev
+   560: 00000000000179e0  2600 FUNC    WEAK   DEFAULT   12 _ZN3c1014FunctionSchemaD2Ev
+   561: 0000000000014910  1355 FUNC    GLOBAL DEFAULT   12 _ZN7torchao23fp6_linear_forward_cudaEN2at6TensorES1_S1_l
+   562: 000000000001b000    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEED1Ev
+   563: 000000000001e2d0     5 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl11deviceCountEv
+   564: 00000000000b5810   192 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104cuda4impl13CUDAGuardImplE
+   565: 0000000000014fa0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl4int_Ev
+   566: 0000000000015720    29 FUNC    WEAK   DEFAULT   12 _ZN3c1014getTypePtrCopyIlEENS_4Type24SingletonOrSharedTypePtrIS1_EEv
+   567: 000000000001df00    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl18uncheckedSetDeviceENS_6DeviceE
+   568: 0000000000017540   237 FUNC    WEAK   DEFAULT   12 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_S5_lES5_NS_4guts8typelist8typelistIJS5_S5_S5_lEEEEES6_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES5_S5_S5_l
+   569: 0000000000013890   228 FUNC    GLOBAL DEFAULT   12 _Z47__device_stub__Z16SplitK_ReductionP6__halfPfmmiP6__halfPfmmi
+   570: 000000000001f8a0   193 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl9getDeviceEv
+   571: 0000000000017060    19 FUNC    WEAK   DEFAULT   12 _ZN3c1014OperatorKernelD1Ev
+   572: 0000000000018e00  1012 FUNC    WEAK   DEFAULT   12 _ZN3c104impl34call_functor_with_args_from_stack_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_S5_lES5_NS_4guts8typelist8typelistIJS5_S5_S5_lEEEEELb0EJLm0ELm1ELm2ELm3EEJS5_S5_S5_lEEENSt5decayINS8_21infer_function_traitsIT_E4type11return_typeEE4typeEPNS_14OperatorKernelENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISP_EESt16integer_sequenceImJXspT1_EEEPNSA_IJDpT2_EEE
+   573: 00000000000b56d8    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE
+   574: 00000000000164f0   896 FUNC    WEAK   DEFAULT   12 _ZNK3c106IValue7tagKindEv
+   575: 0000000000015ef0   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi2EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi
+   576: 000000000001f110   139 FUNC    WEAK   DEFAULT   12 _ZNSt15basic_stringbufIcSt11char_traitsIcESaIcEED0Ev
+   577: 000000000001e080    10 FUNC    WEAK   DEFAULT   12 _ZN3c104impl16VirtualGuardImplD0Ev
+   578: 0000000000036200    32 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104cuda4impl13CUDAGuardImplE
+   579: 0000000000022b20  1113 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJRKcRKPS2_S4_S6_S4_EE4callES3_S6_S6_S6_S6_
+   580: 0000000000015660    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3addERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   581: 000000000001bed0  8158 FUNC    GLOBAL DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219310nms_kernelERKN2at6TensorES4_d
    582: 000000000001e3d0   123 FUNC    WEAK   DEFAULT   12 _ZNK3c1010TensorImpl11size_customEl
    583: 000000000001df50    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl14exchangeStreamENS_6StreamE
    584: 00000000000b57a0    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104cuda4impl13CUDAGuardImplE
    585: 0000000000020d70  4722 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl12destroyEventEPva
    586: 0000000000023fa0   765 FUNC    GLOBAL DEFAULT   12 _Z25Assign_32_FP6_To_4_ThreadPSt6vectorIhSaIhEES2_PhS3_S3_S3_
    587: 0000000000016300   164 FUNC    WEAK   DEFAULT   12 _ZN5torch7LibraryD1Ev
    588: 0000000000018a30   275 FUNC    WEAK   DEFAULT   12 _ZN5torch5emptyEN3c108ArrayRefIlEENS0_13TensorOptionsESt8optionalINS0_12MemoryFormatEE
@@ -605,15 +605,15 @@
    601: 00000000000157b0    70 FUNC    WEAK   DEFAULT   12 _ZN3c1018getFakeTypePtrCopyIN2at6TensorEEENS_4Type24SingletonOrSharedTypePtrIS3_EEv
    602: 00000000000b5778    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1010ValueErrorE
    603: 0000000000014e70     3 FUNC    WEAK   DEFAULT   12 _ZNK3c1011SymNodeImpl13is_nested_intEv
 
 Symbol table '.symtab' contains 840 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
-     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS tmpxft_00000877_00000000-6_fp6_linear.compute_86.cudafe1.cpp
+     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS tmpxft_0000086e_00000000-6_fp6_linear.compute_86.cudafe1.cpp
      2: 0000000000037988     0 NOTYPE  LOCAL  DEFAULT   15 fatbinData
      3: 00000000000133d0   568 FUNC    LOCAL  DEFAULT   12 _Z9Kernel_ExI12TilingConfigILi4ELi1ELi8EEfEvP11CUstream_stPK5uint4PK6__halfS9_PT0_mmmi
      4: 00000000000b6aa0     8 OBJECT  LOCAL  DEFAULT   27 _ZGVZ9Kernel_ExI12TilingConfigILi4ELi1ELi8EEfEvP11CUstream_stPK5uint4PK6__halfS9_PT0_mmmiE8SHMEM_SZ
      5: 00000000000b6aa8     8 OBJECT  LOCAL  DEFAULT   27 _ZZ9Kernel_ExI12TilingConfigILi4ELi1ELi8EEfEvP11CUstream_stPK5uint4PK6__halfS9_PT0_mmmiE8SHMEM_SZ
      6: 0000000000013610    12 FUNC    LOCAL  DEFAULT   12 _ZL26__cudaUnregisterBinaryUtilv
      7: 00000000000b6b20     8 OBJECT  LOCAL  DEFAULT   27 _ZL20__cudaFatCubinHandle
      8: 0000000000013620   549 FUNC    LOCAL  DEFAULT   12 _Z9Kernel_ExI12TilingConfigILi4ELi1ELi8EE6__halfEvP11CUstream_stPK5uint4PKS2_S9_PT0_mmmi.constprop.0
@@ -633,49 +633,49 @@
     22: 00000000000b6b10     8 OBJECT  LOCAL  DEFAULT   27 _ZGVZ9Kernel_ExI12TilingConfigILi4ELi1ELi1EE6__halfEvP11CUstream_stPK5uint4PKS2_S9_PT0_mmmiE8SHMEM_SZ
     23: 00000000000b6b18     8 OBJECT  LOCAL  DEFAULT   27 _ZZ9Kernel_ExI12TilingConfigILi4ELi1ELi1EE6__halfEvP11CUstream_stPK5uint4PKS2_S9_PT0_mmmiE8SHMEM_SZ
     24: 0000000000011d80   502 FUNC    LOCAL  DEFAULT   12 _ZL24__sti____cudaRegisterAllv
     25: 00000000000b6a38    24 OBJECT  LOCAL  DEFAULT   26 _ZL15__fatDeviceText
     26: 0000000000034a00     1 OBJECT  LOCAL  DEFAULT   14 _ZN6thrust6system6detail10sequentialL3seqE
     27: 0000000000034a08     8 OBJECT  LOCAL  DEFAULT   14 _ZN3c10L45autograd_dispatch_keyset_with_ADInplaceOrViewE
     28: 00000000000113a0    24 FUNC    LOCAL  DEFAULT   12 _ZN7torchao23fp6_linear_forward_cudaEN2at6TensorES1_S1_l.cold
-    29: 0000000000011f80   408 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_tmpxft_00000877_00000000_6_fp6_linear.compute_86.cudafe1.cpp
+    29: 0000000000011f80   408 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_tmpxft_0000086e_00000000_6_fp6_linear.compute_86.cudafe1.cpp
     30: 00000000000b6ba0     1 OBJECT  LOCAL  DEFAULT   27 _ZStL8__ioinit
     31: 00000000000b6b40    96 OBJECT  LOCAL  DEFAULT   27 _ZN7torchaoL45TORCH_LIBRARY_IMPL_static_init_torchao_CUDA_2E
-    32: 00000000000113b8    77 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_tmpxft_00000877_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold
-    33: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS tmpxft_00000878_00000000-6_weight_quant.compute_86.cudafe1.cpp
+    32: 00000000000113b8    77 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_tmpxft_0000086e_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold
+    33: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS tmpxft_0000086f_00000000-6_weight_quant.compute_86.cudafe1.cpp
     34: 000000000009d658     0 NOTYPE  LOCAL  DEFAULT   15 fatbinData
     35: 0000000000019550    12 FUNC    LOCAL  DEFAULT   12 _ZL26__cudaUnregisterBinaryUtilv
     36: 00000000000b6bc0     8 OBJECT  LOCAL  DEFAULT   27 _ZL20__cudaFatCubinHandle
     37: 0000000000019560    50 FUNC    LOCAL  DEFAULT   12 _ZNSs4_Rep10_M_disposeERKSaIcE.part.0
     38: 0000000000011405    69 FUNC    LOCAL  DEFAULT   12 _Z13cast_fp16_fp6PtPh.cold
     39: 000000000001144a    69 FUNC    LOCAL  DEFAULT   12 _Z29weight_prepacking_fp16_to_fp6PtPhmm.cold
     40: 0000000000012120    91 FUNC    LOCAL  DEFAULT   12 _ZL24__sti____cudaRegisterAllv
     41: 00000000000b6a50    24 OBJECT  LOCAL  DEFAULT   26 _ZL15__fatDeviceText
     42: 0000000000035135     1 OBJECT  LOCAL  DEFAULT   14 _ZN6thrust6system6detail10sequentialL3seqE
     43: 000000000001148f    16 FUNC    LOCAL  DEFAULT   12 _ZN7torchao15fp16_to_fp6_cpuEN2at6TensorE.cold
     44: 000000000001149f    16 FUNC    LOCAL  DEFAULT   12 _ZN7torchao25weight_matrix_dequant_cpuEN2at6TensorES1_.cold
-    45: 0000000000012180   919 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_tmpxft_00000878_00000000_6_weight_quant.compute_86.cudafe1.cpp
+    45: 0000000000012180   919 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_tmpxft_0000086f_00000000_6_weight_quant.compute_86.cudafe1.cpp
     46: 00000000000b6c40     1 OBJECT  LOCAL  DEFAULT   27 _ZStL8__ioinit
     47: 00000000000b6be0    96 OBJECT  LOCAL  DEFAULT   27 _ZN7torchaoL44TORCH_LIBRARY_IMPL_static_init_torchao_CPU_2E
-    48: 00000000000114af   119 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_tmpxft_00000878_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold
-    49: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS tmpxft_00000879_00000000-6_nms.compute_86.cudafe1.cpp
+    48: 00000000000114af   119 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_tmpxft_0000086f_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold
+    49: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS tmpxft_00000870_00000000-6_nms.compute_86.cudafe1.cpp
     50: 000000000009de68     0 NOTYPE  LOCAL  DEFAULT   15 fatbinData
     51: 000000000001ba40   624 FUNC    LOCAL  DEFAULT   12 _ZN3c10L8toStringENS_10ScalarTypeE
     52: 000000000001bcb0    12 FUNC    LOCAL  DEFAULT   12 _ZL26__cudaUnregisterBinaryUtilv
     53: 00000000000b6c60     8 OBJECT  LOCAL  DEFAULT   27 _ZL20__cudaFatCubinHandle
     54: 000000000001bcc0    50 FUNC    LOCAL  DEFAULT   12 _ZNSs4_Rep10_M_disposeERKSaIcE.part.0
     55: 0000000000012520   226 FUNC    LOCAL  DEFAULT   12 _ZL24__sti____cudaRegisterAllv
     56: 00000000000b6a68    24 OBJECT  LOCAL  DEFAULT   26 _ZL15__fatDeviceText
     57: 00000000000352c4     1 OBJECT  LOCAL  DEFAULT   14 _ZN6thrust6system6detail10sequentialL3seqE
     58: 000000000001bd00   460 FUNC    LOCAL  DEFAULT   12 _ZN3c106SymInt8release_Ev.part.0
-    59: 0000000000011526   949 FUNC    LOCAL  DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220210nms_kernelERKN2at6TensorES4_d.cold
-    60: 0000000000012610   445 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_tmpxft_00000879_00000000_6_nms.compute_86.cudafe1.cpp
+    59: 0000000000011526   949 FUNC    LOCAL  DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219310nms_kernelERKN2at6TensorES4_d.cold
+    60: 0000000000012610   445 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_tmpxft_00000870_00000000_6_nms.compute_86.cudafe1.cpp
     61: 00000000000b6ce0     1 OBJECT  LOCAL  DEFAULT   27 _ZStL8__ioinit
     62: 00000000000b6c80    96 OBJECT  LOCAL  DEFAULT   27 _ZN7torchaoL45TORCH_LIBRARY_IMPL_static_init_torchao_CUDA_2E
-    63: 00000000000118db    77 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_tmpxft_00000879_00000000_6_nms.compute_86.cudafe1.cpp.cold
+    63: 00000000000118db    77 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_tmpxft_00000870_00000000_6_nms.compute_86.cudafe1.cpp.cold
     64: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS fp6_llm.cpp
     65: 0000000000011928    39 FUNC    LOCAL  DEFAULT   12 _ZNSs4_Rep10_M_disposeERKSaIcE.part.0
     66: 00000000000127d0  1768 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_fp6_llm.cpp
     67: 00000000000b6d00    96 OBJECT  LOCAL  DEFAULT   27 _ZL44TORCH_LIBRARY_FRAGMENT_static_init_torchao_2
     68: 000000000001194f   238 FUNC    LOCAL  DEFAULT   12 _GLOBAL__sub_I_fp6_llm.cpp.cold
     69: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS weight_prepacking.cpp
     70: 0000000000011a3e    39 FUNC    LOCAL  DEFAULT   12 _ZNSs4_Rep10_M_disposeERKSaIcE.part.0
@@ -853,35 +853,35 @@
    242: 00000000000349e0    25 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorES0_S0_S0_lE
    243: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_DelItemString
    244: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterVar@libcudart.so.12
    245: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Py_Dealloc
    246: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt9basic_iosIcSt11char_traitsIcEE5clearESt12_Ios_Iostate@GLIBCXX_3.4
    247: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyByteArray_AsString
    248: 000000000001e020    24 FUNC    WEAK   DEFAULT   12 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS5_S7_dES5_NS_4guts8typelist8typelistIJS7_S7_dEEEEES8_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES7_S7_d
-   249: 000000000001e5c0   204 FUNC    WEAK   DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py
-   250: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strdup@GLIBC_2.2.5
-   251: 000000000001e2d0     5 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl11deviceCountEv
-   252: 0000000000014f00     6 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11is_symbolicEv
-   253: 0000000000019200   835 FUNC    WEAK   DEFAULT   12 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_S5_lES5_NS_4guts8typelist8typelistIJS5_S5_S5_lEEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE
-   254: 00000000000b5910    40 OBJECT  WEAK   DEFAULT   21 _ZTVSt19bad_optional_access
-   255: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyModule_Create2
-   256: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_begin_catch@CXXABI_1.3
-   257: 0000000000015360    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7sym_minERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   258: 0000000000015210    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl30is_channels_last_contiguous_2dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
-   259: 000000000001df50    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl14exchangeStreamENS_6StreamE
-   260: 000000000001e490    86 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl10queryEventEPv
-   261: 00000000000174e0    82 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_10TensorImplENS_19UndefinedTensorImplEE6reset_Ev
-   262: 000000000001f090   123 FUNC    WEAK   DEFAULT   12 _ZNSt15basic_stringbufIcSt11char_traitsIcESaIcEED2Ev
-   263: 00000000000152d0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7sym_andERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   264: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt9exceptionD2Ev@GLIBCXX_3.4
-   265: 00000000000272f0   354 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIP11_typeobjectSaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_
-   266: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyByteArray_Type
-   267: 0000000000015540    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3modERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   268: 00000000000164f0   896 FUNC    WEAK   DEFAULT   12 _ZNK3c106IValue7tagKindEv
-   269: 000000000001df10    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl9getStreamENS_6DeviceE
+   249: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strdup@GLIBC_2.2.5
+   250: 000000000001e2d0     5 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl11deviceCountEv
+   251: 0000000000014f00     6 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11is_symbolicEv
+   252: 0000000000019200   835 FUNC    WEAK   DEFAULT   12 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_S5_lES5_NS_4guts8typelist8typelistIJS5_S5_S5_lEEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE
+   253: 00000000000b5910    40 OBJECT  WEAK   DEFAULT   21 _ZTVSt19bad_optional_access
+   254: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyModule_Create2
+   255: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_begin_catch@CXXABI_1.3
+   256: 0000000000015360    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7sym_minERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   257: 0000000000015210    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl30is_channels_last_contiguous_2dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
+   258: 000000000001df50    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl14exchangeStreamENS_6StreamE
+   259: 000000000001e490    86 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl10queryEventEPv
+   260: 00000000000174e0    82 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_10TensorImplENS_19UndefinedTensorImplEE6reset_Ev
+   261: 000000000001f090   123 FUNC    WEAK   DEFAULT   12 _ZNSt15basic_stringbufIcSt11char_traitsIcESaIcEED2Ev
+   262: 00000000000152d0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7sym_andERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   263: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt9exceptionD2Ev@GLIBCXX_3.4
+   264: 00000000000272f0   354 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIP11_typeobjectSaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_
+   265: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyByteArray_Type
+   266: 0000000000015540    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3modERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   267: 00000000000164f0   896 FUNC    WEAK   DEFAULT   12 _ZNK3c106IValue7tagKindEv
+   268: 000000000001df10    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl9getStreamENS_6DeviceE
+   269: 000000000001e5c0   204 FUNC    WEAK   DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py
    270: 0000000000032c5c     0 FUNC    GLOBAL DEFAULT   13 _fini
    271: 0000000000025c90    43 FUNC    WEAK   DEFAULT   12 _ZNKSt9type_info9hash_codeEv
    272: 0000000000016f20   197 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_targetD1Ev
    273: 0000000000017860    74 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_10TensorImplENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev
    274: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_SetAttrString
    275: 000000000001dfa0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl12destroyEventEPva
    276: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyType_IsSubtype
@@ -930,42 +930,42 @@
    319: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaPushCallConfiguration@libcudart.so.12
    320: 00000000000151e0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl30is_channels_last_contiguous_3dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
    321: 000000000001b000    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEED2Ev
    322: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND memset@GLIBC_2.2.5
    323: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyBaseObject_Type
    324: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c106detail14torchCheckFailEPKcS2_jS2_
    325: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt13runtime_errorC1EPKc
-   326: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTISt12out_of_range@GLIBCXX_3.4
-   327: 0000000000023cc0   126 FUNC    GLOBAL DEFAULT   12 _Z24Padding_8_FP6_To_8_BytesPhS_
-   328: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZSt17rethrow_exceptionNSt15__exception_ptr13exception_ptrE@CXXABI_1.3.3
-   329: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZN3c104impl8GPUTrace13gpuTraceStateE
-   330: 0000000000017400   123 FUNC    WEAK   DEFAULT   12 _ZNSt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE10_M_releaseEv
-   331: 0000000000015000    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl10guard_boolEPKcl
-   332: 0000000000026600   119 FUNC    WEAK   DEFAULT   12 _ZNSt10_HashtableIP7_objectS1_SaIS1_ENSt8__detail9_IdentityESt8equal_toIS1_ESt4hashIS1_ENS3_18_Mod_range_hashingENS3_20_Default_ranged_hashENS3_20_Prime_rehash_policyENS3_17_Hashtable_traitsILb0ELb1ELb1EEEED1Ev
-   333: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTISt12length_error@GLIBCXX_3.4
-   334: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNKSs4findEcm@GLIBCXX_3.4
-   335: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK3c106IValue23reportToTensorTypeErrorEv
-   336: 00000000000b6ec0     0 NOTYPE  GLOBAL DEFAULT   27 _end
-   337: 0000000000013890   228 FUNC    GLOBAL DEFAULT   12 _Z47__device_stub__Z16SplitK_ReductionP6__halfPfmmiP6__halfPfmmi
-   338: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs9push_backEc@GLIBCXX_3.4
-   339: 000000000001f500   917 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKS3_EE4callES5_S5_
-   340: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTVSt19basic_ostringstreamIcSt11char_traitsIcESaIcEE@GLIBCXX_3.4
-   341: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_WriteUnraisable
-   342: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThread_tss_create
-   343: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strlen@GLIBC_2.2.5
-   344: 000000000001aac0  1331 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKNS_10ScalarTypeES3_EE4callERKS3_S6_S9_
-   345: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt15__exception_ptr13exception_ptrC1ERKS0_@CXXABI_1.3.3
-   346: 00000000000195a0   405 FUNC    GLOBAL DEFAULT   12 _Z13cast_fp16_fp6PtPh
-   347: 0000000000034930    23 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1014OperatorKernelE
-   348: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3
-   349: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_HasAttrString
-   350: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTVSt9bad_alloc@GLIBCXX_3.4
-   351: 0000000000015b30   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EEfEvPK5uint4PK6__halfS7_PT0_mmmi
-   352: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_guard_abort@CXXABI_1.3
-   353: 000000000001e690   204 FUNC    WEAK   DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py
+   326: 000000000001bed0  8158 FUNC    GLOBAL DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219310nms_kernelERKN2at6TensorES4_d
+   327: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTISt12out_of_range@GLIBCXX_3.4
+   328: 0000000000023cc0   126 FUNC    GLOBAL DEFAULT   12 _Z24Padding_8_FP6_To_8_BytesPhS_
+   329: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZSt17rethrow_exceptionNSt15__exception_ptr13exception_ptrE@CXXABI_1.3.3
+   330: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZN3c104impl8GPUTrace13gpuTraceStateE
+   331: 0000000000017400   123 FUNC    WEAK   DEFAULT   12 _ZNSt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE10_M_releaseEv
+   332: 0000000000015000    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl10guard_boolEPKcl
+   333: 0000000000026600   119 FUNC    WEAK   DEFAULT   12 _ZNSt10_HashtableIP7_objectS1_SaIS1_ENSt8__detail9_IdentityESt8equal_toIS1_ESt4hashIS1_ENS3_18_Mod_range_hashingENS3_20_Default_ranged_hashENS3_20_Prime_rehash_policyENS3_17_Hashtable_traitsILb0ELb1ELb1EEEED1Ev
+   334: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTISt12length_error@GLIBCXX_3.4
+   335: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNKSs4findEcm@GLIBCXX_3.4
+   336: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK3c106IValue23reportToTensorTypeErrorEv
+   337: 00000000000b6ec0     0 NOTYPE  GLOBAL DEFAULT   27 _end
+   338: 0000000000013890   228 FUNC    GLOBAL DEFAULT   12 _Z47__device_stub__Z16SplitK_ReductionP6__halfPfmmiP6__halfPfmmi
+   339: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs9push_backEc@GLIBCXX_3.4
+   340: 000000000001f500   917 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKS3_EE4callES5_S5_
+   341: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTVSt19basic_ostringstreamIcSt11char_traitsIcESaIcEE@GLIBCXX_3.4
+   342: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_WriteUnraisable
+   343: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThread_tss_create
+   344: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strlen@GLIBC_2.2.5
+   345: 000000000001aac0  1331 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKNS_10ScalarTypeES3_EE4callERKS3_S6_S9_
+   346: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt15__exception_ptr13exception_ptrC1ERKS0_@CXXABI_1.3.3
+   347: 00000000000195a0   405 FUNC    GLOBAL DEFAULT   12 _Z13cast_fp16_fp6PtPh
+   348: 0000000000034930    23 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1014OperatorKernelE
+   349: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3
+   350: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_HasAttrString
+   351: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTVSt9bad_alloc@GLIBCXX_3.4
+   352: 0000000000015b30   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EEfEvPK5uint4PK6__halfS7_PT0_mmmi
+   353: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_guard_abort@CXXABI_1.3
    354: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaStreamQuery@libcudart.so.12
    355: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cudaRegisterFatBinary@libcudart.so.12
    356: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c1010TensorType3getEv
    357: 000000000001df80    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl5blockEPvRKNS_6StreamE
    358: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c106SymIntC1ENS_13intrusive_ptrINS_11SymNodeImplENS_6detail34intrusive_target_default_null_typeIS2_EEEE
    359: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104cuda14ExchangeDeviceEa
    360: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104cuda20setCurrentCUDAStreamENS0_10CUDAStreamE
@@ -996,31 +996,31 @@
    385: 000000000001e380    34 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl23getStreamFromGlobalPoolENS_6DeviceEb
    386: 000000000001df20    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl12getNewStreamENS_6DeviceEi
    387: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSsC1EPKcmRKSaIcE@GLIBCXX_3.4
    388: 0000000000014ee0    16 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl12maybe_as_intEv
    389: 0000000000017080    37 FUNC    WEAK   DEFAULT   12 _ZN3c1014OperatorKernelD0Ev
    390: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCapsule_GetContext
    391: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK2at10TensorBase21__dispatch_contiguousEN3c1012MemoryFormatE
-   392: 000000000001e4f0   204 FUNC    WEAK   DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py
-   393: 0000000000014f70    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl5bool_Ev
-   394: 000000000001dfc0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl17synchronizeStreamERKNS_6StreamE
-   395: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN2at4_ops19empty_memory_format4callEN3c108ArrayRefINS2_6SymIntEEESt8optionalINS2_10ScalarTypeEES6_INS2_6LayoutEES6_INS2_6DeviceEES6_IbES6_INS2_12MemoryFormatEE
-   396: 0000000000015120    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl5cloneEv
-   397: 00000000000b5420    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1014OperatorKernelE
-   398: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs6appendEPKcm@GLIBCXX_3.4
-   399: 0000000000016ff0    23 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_targetD0Ev
-   400: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs4swapERSs@GLIBCXX_3.4
-   401: 00000000000b5660    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1015VariableVersion14VersionCounterE
-   402: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyType_Lookup
-   403: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThreadState_Clear
-   404: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Clear
-   405: 0000000000027630  1684 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIbSaIbEE14_M_fill_insertESt13_Bit_iteratormb
-   406: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_throw@CXXABI_1.3
-   407: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaStreamSynchronize@libcudart.so.12
-   408: 00000000000362a0    24 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorERKS0_S2_dE
+   392: 0000000000014f70    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl5bool_Ev
+   393: 000000000001dfc0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl17synchronizeStreamERKNS_6StreamE
+   394: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN2at4_ops19empty_memory_format4callEN3c108ArrayRefINS2_6SymIntEEESt8optionalINS2_10ScalarTypeEES6_INS2_6LayoutEES6_INS2_6DeviceEES6_IbES6_INS2_12MemoryFormatEE
+   395: 0000000000015120    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl5cloneEv
+   396: 00000000000b5420    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1014OperatorKernelE
+   397: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs6appendEPKcm@GLIBCXX_3.4
+   398: 0000000000016ff0    23 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_targetD0Ev
+   399: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs4swapERSs@GLIBCXX_3.4
+   400: 00000000000b5660    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1015VariableVersion14VersionCounterE
+   401: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyType_Lookup
+   402: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThreadState_Clear
+   403: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Clear
+   404: 0000000000027630  1684 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIbSaIbEE14_M_fill_insertESt13_Bit_iteratormb
+   405: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_throw@CXXABI_1.3
+   406: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaStreamSynchronize@libcudart.so.12
+   407: 00000000000362a0    24 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorERKS0_S2_dE
+   408: 000000000001e4f0   204 FUNC    WEAK   DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py
    409: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCapsule_New
    410: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyMem_Calloc
    411: 000000000001b050    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED1Ev
    412: 000000000001f1a0   853 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKlEE4callERKS3_S5_
    413: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN2at4_ops11sort_stable4callERKNS_6TensorESt8optionalIbElb
    414: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZSt20__throw_length_errorPKc@GLIBCXX_3.4
    415: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN5torch7LibraryC1ENS0_4KindESsSt8optionalIN3c1011DispatchKeyEEPKcj
@@ -1048,250 +1048,250 @@
    437: 00000000000b5778    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1010ValueErrorE
    438: 00000000000b5728    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE
    439: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyType_Ready
    440: 00000000000b58f8    24 OBJECT  WEAK   DEFAULT   21 _ZTISt19bad_optional_access
    441: 0000000000035000   109 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE
    442: 0000000000015420    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2geERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
    443: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c105ErrorC2ENS_14SourceLocationESs
-   444: 00000000000b53f0    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1011SymNodeImplE
-   445: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZSt24__throw_out_of_range_fmtPKcz
-   446: 00000000000158b0   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EEfEvPK5uint4PK6__halfS7_PT0_mmmi
-   447: 00000000000170d0    37 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED0Ev
-   448: 0000000000015240    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl13is_contiguousENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
-   449: 0000000000017120    37 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImplD0Ev
-   450: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs6assignERKSs@GLIBCXX_3.4
-   451: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs6assignEPKcm@GLIBCXX_3.4
-   452: 0000000000015300    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl6sym_orERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   453: 00000000000155a0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3powERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   454: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c106detail23torchInternalAssertFailEPKcS2_jS2_RKSs
-   455: 00000000000255a0   291 FUNC    GLOBAL DEFAULT   12 PyInit__C
-   456: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs6appendERKSs@GLIBCXX_3.4
-   457: 0000000000035120    21 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorES0_S0_E
-   458: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTuple_GetItem
-   459: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt15__exception_ptrneERKNS_13exception_ptrES2_@CXXABI_1.3.3
-   460: 0000000000024910  2235 FUNC    GLOBAL DEFAULT   12 _ZN7torchao28weight_matrix_prepacking_cpuEN2at6TensorE
-   461: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyObject_GetDictPtr
-   462: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK2at6Tensor5indexESt16initializer_listINS_8indexing11TensorIndexEE
-   463: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_atexit@GLIBC_2.2.5
-   464: 00000000000b5688    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1014OperatorKernelE
-   465: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK2at10TensorBase8data_ptrIlEEPT_v
-   466: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTuple_SetItem
-   467: 0000000000015c70   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi8EEfEvPK5uint4PK6__halfS7_PT0_mmmi
-   468: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThread_tss_get
-   469: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Restore
-   470: 0000000000019740   171 FUNC    GLOBAL DEFAULT   12 _Z29weight_prepacking_fp16_to_fp6PtPhmm
-   471: 0000000000018a30   275 FUNC    WEAK   DEFAULT   12 _ZN5torch5emptyEN3c108ArrayRefIlEENS0_13TensorOptionsESt8optionalINS0_12MemoryFormatEE
-   472: 0000000000016300   164 FUNC    WEAK   DEFAULT   12 _ZN5torch7LibraryD1Ev
-   473: 000000000001e010     1 FUNC    WEAK   DEFAULT   12 _ZN3c104cuda4impl13CUDAGuardImplD1Ev
-   474: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_pure_virtual@CXXABI_1.3
-   475: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __pthread_key_create@GLIBC_2.2.5
-   476: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt15__exception_ptr13exception_ptr4swapERS0_@CXXABI_1.3.3
-   477: 0000000000015090    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl10wrap_floatEd
-   478: 000000000001fc50   979 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl6recordEPPvRKNS_6StreamEaNS_9EventFlagE
-   479: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNR5torch7Library5_implEPKcONS_11CppFunctionENS_17_RegisterOrVerifyE
-   480: 0000000000026570   141 FUNC    WEAK   DEFAULT   12 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EPKS3_RKS6_
-   481: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSsC1ERKSaIcE@GLIBCXX_3.4
-   482: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104cuda9GetDeviceEPa
-   483: 0000000000015760    70 FUNC    WEAK   DEFAULT   12 _ZN3c1014getTypePtrCopyIN2at6TensorEEENS_4Type24SingletonOrSharedTypePtrIS3_EEv
-   484: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs4_Rep10_M_destroyERKSaIcE@GLIBCXX_3.4
-   485: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt15__exception_ptr13exception_ptrD1Ev@CXXABI_1.3.3
-   486: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN2at4_ops12index_select4callERKNS_6TensorElS4_
-   487: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThread_tss_alloc
-   488: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTISt16nested_exception@CXXABI_1.3.5
-   489: 0000000000015450    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2leERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   490: 000000000001ded0    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl14exchangeDeviceENS_6DeviceE
-   491: 000000000001df30    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl16getDefaultStreamENS_6DeviceE
-   492: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN6caffe28TypeMeta26error_unsupported_typemetaES0_
-   493: 00000000000156c0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7is_boolEv
-   494: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTISt13runtime_error@GLIBCXX_3.4
-   495: 0000000000017060    19 FUNC    WEAK   DEFAULT   12 _ZN3c1014OperatorKernelD1Ev
-   496: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaGetErrorString@libcudart.so.12
-   497: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt13runtime_errorC1ERKSs@GLIBCXX_3.4
-   498: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN2at4_ops6narrow4callERKNS_6TensorElN3c106SymIntES6_
-   499: 00000000000154e0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2neERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   500: 0000000000018570  1207 FUNC    WEAK   DEFAULT   12 _ZN5torch8autograd13make_variableEN2at6TensorEbb
-   501: 000000000001f110   139 FUNC    WEAK   DEFAULT   12 _ZNSt15basic_stringbufIcSt11char_traitsIcESaIcEED0Ev
-   502: 0000000000017010    19 FUNC    WEAK   DEFAULT   12 _ZN3c1015VariableVersion14VersionCounterD1Ev
-   503: 000000000001e760   651 FUNC    WEAK   DEFAULT   12 _ZN3c1010ValueErrorD1Ev
-   504: 0000000000014fd0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11guard_floatEPKcl
-   505: 0000000000026470    95 FUNC    WEAK   DEFAULT   12 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EOS6_S7_
-   506: 00000000000348e0    20 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1011SymNodeImplE
-   507: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZSt16__ostream_insertIcSt11char_traitsIcEERSt13basic_ostreamIT_T0_ES6_PKS3_l@GLIBCXX_3.4.9
-   508: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
-   509: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCFunction_Type
-   510: 00000000000170b0    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED2Ev
-   511: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSsC1ERKSsmm@GLIBCXX_3.4
-   512: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyGILState_GetThisThreadState
-   513: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyBytes_AsStringAndSize
-   514: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND memcmp@GLIBC_2.2.5
-   515: 0000000000017480    95 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEE6reset_Ev
-   516: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_AsEncodedString
-   517: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNKSs7compareEPKc@GLIBCXX_3.4
-   518: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK2at10TensorBase8data_ptrIN3c104HalfEEEPT_v
-   519: 0000000000017100    19 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImplD2Ev
-   520: 0000000000014f40    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl8has_hintEv
-   521: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTuple_New
-   522: 0000000000015ef0   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi2EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi
-   523: 0000000000015800   164 FUNC    WEAK   DEFAULT   12 _ZN5torch6detail16TorchLibraryInitD1Ev
-   524: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_CallFunctionObjArgs
-   525: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104impl23ExcludeDispatchKeyGuardC1ENS_14DispatchKeySetE
-   526: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK2at10TensorBase8data_ptrIhEEPT_v
-   527: 00000000000251d0     8 FUNC    WEAK   DEFAULT   12 _ZNKSt19bad_optional_access4whatEv
-   528: 00000000000b5948    24 OBJECT  WEAK   DEFAULT   21 _ZTISt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE
-   529: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaEventSynchronize@libcudart.so.12
-   530: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104cuda20getDefaultCUDAStreamEa
-   531: 00000000000242a0  1638 FUNC    GLOBAL DEFAULT   12 _Z24weight_matrix_prepackingPiS_mm
-   532: 00000000000162b0    70 FUNC    WEAK   DEFAULT   12 _ZNK3c1010TensorImpl6deviceEv
-   533: 0000000000026770   959 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIbSaIbEE13_M_insert_auxESt13_Bit_iteratorb
-   534: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c10lsERSoNS_10DeviceTypeE
-   535: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTTSt19basic_ostringstreamIcSt11char_traitsIcESaIcEE@GLIBCXX_3.4
-   536: 000000000001f970   195 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl14exchangeDeviceENS_6DeviceE
-   537: 0000000000014e60     1 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_target17release_resourcesEv
-   538: 000000000002b580   294 FUNC    WEAK   DEFAULT   12 _ZNSt10_HashtableISsSt4pairIKSsPvESaIS3_ENSt8__detail10_Select1stESt8equal_toISsESt4hashISsENS5_18_Mod_range_hashingENS5_20_Default_ranged_hashENS5_20_Prime_rehash_policyENS5_17_Hashtable_traitsILb1ELb0ELb1EEEE9_M_rehashEmRKm
-   539: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_ImportError
-   540: 0000000000015480    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2ltERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   541: 0000000000014e70     3 FUNC    WEAK   DEFAULT   12 _ZNK3c1011SymNodeImpl13is_nested_intEv
-   542: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt19basic_ostringstreamIcSt11char_traitsIcESaIcEEC1Ev
-   543: 00000000000b56d8    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE
-   544: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Occurred
-   545: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThreadState_DeleteCurrent
-   546: 00000000000172b0   162 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_11SymNodeImplENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev
-   547: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK2at10TensorBase8data_ptrIiEEPT_v
-   548: 0000000000016030   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi
-   549: 00000000000b56f0    16 OBJECT  WEAK   DEFAULT   21 _ZTIFN2at6TensorES0_E
-   550: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaEventRecord@libcudart.so.12
-   551: 000000000001b070    37 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED0Ev
-   552: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyWeakref_NewRef
-   553: 000000000002b6b0   478 FUNC    WEAK   DEFAULT   12 _ZNSt8__detail9_Map_baseISsSt4pairIKSsPvESaIS4_ENS_10_Select1stESt8equal_toISsESt4hashISsENS_18_Mod_range_hashingENS_20_Default_ranged_hashENS_20_Prime_rehash_policyENS_17_Hashtable_traitsILb1ELb0ELb1EEELb1EEixEOSs
-   554: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK3c105Error4whatEv
-   555: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSsC1EPKcRKSaIcE@GLIBCXX_3.4
-   556: 000000000001e2e0   106 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl14exchangeStreamENS_6StreamE
-   557: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs7reserveEm@GLIBCXX_3.4
-   558: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaFuncSetAttribute@libcudart.so.12
-   559: 000000000001b020    37 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEED0Ev
-   560: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_AsUTF8String
-   561: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyEval_GetBuiltins
-   562: 0000000000020d70  4722 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl12destroyEventEPva
-   563: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTISt14overflow_error@GLIBCXX_3.4
-   564: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_ValueError
-   565: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND printf@GLIBC_2.2.5
-   566: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs7replaceEmmPKcm@GLIBCXX_3.4
-   567: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt13runtime_errorC2ERKSs@GLIBCXX_3.4
-   568: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN5torch3jit11parseSchemaERKSs
-   569: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104warnERKNS_7WarningE
-   570: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSsC1ERKSs@GLIBCXX_3.4
-   571: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND memcpy@GLIBC_2.14
-   572: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaEventCreateWithFlags@libcudart.so.12
-   573: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTIN10__cxxabiv115__forced_unwindE@CXXABI_1.3.2
-   574: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt9bad_allocD1Ev@GLIBCXX_3.4
-   575: 0000000000020030   197 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEED1Ev
-   576: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs6appendEmc@GLIBCXX_3.4
-   577: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCapsule_GetName
-   578: 00000000000159f0   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi2EEfEvPK5uint4PK6__halfS7_PT0_mmmi
-   579: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs6appendERKSsmm@GLIBCXX_3.4
-   580: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZSt17__throw_bad_allocv@GLIBCXX_3.4
-   581: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _Znwm@GLIBCXX_3.4
-   582: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_OverflowError
-   583: 000000000001dfe0    16 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl11elapsedTimeEPvS2_a
-   584: 000000000001e080    10 FUNC    WEAK   DEFAULT   12 _ZN3c104impl16VirtualGuardImplD0Ev
-   585: 0000000000014fa0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl4int_Ev
-   586: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
-   587: 00000000000179e0  2600 FUNC    WEAK   DEFAULT   12 _ZN3c1014FunctionSchemaD2Ev
-   588: 0000000000026520    66 FUNC    WEAK   DEFAULT   12 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EOS6_PKS3_
-   589: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND free@GLIBC_2.2.5
-   590: 000000000001e050    31 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl9getStreamENS_6DeviceE
-   591: 000000000001e760   651 FUNC    WEAK   DEFAULT   12 _ZN3c1010ValueErrorD2Ev
-   592: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt19basic_ostringstreamIcSt11char_traitsIcESaIcEED1Ev@GLIBCXX_3.4
-   593: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTVSt15basic_stringbufIcSt11char_traitsIcESaIcEE@GLIBCXX_3.4
-   594: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5
-   595: 0000000000036220   119 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEEE
-   596: 000000000001df90    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl10queryEventEPv
-   597: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_Type
-   598: 0000000000036530    24 OBJECT  WEAK   DEFAULT   14 _ZTSSt19bad_optional_access
-   599: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTISt12domain_error@GLIBCXX_3.4
-   600: 0000000000016870   338 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKiEE4callERKS3_S5_
-   601: 0000000000016dc0   338 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKjEE4callERKS3_S5_
-   602: 000000000001eca0   202 FUNC    WEAK   DEFAULT   12 _ZN3c1014DispatchKeySetC2ENS_11DispatchKeyE
-   603: 0000000000020030   197 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEED2Ev
-   604: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCMethod_New
-   605: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaGetLastError@libcudart.so.12
-   606: 00000000000b56b0    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEEE
-   607: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK3c1017SymbolicShapeMeta18init_is_contiguousEv
-   608: 0000000000014e80     9 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl20guard_size_obliviousEPKcl
-   609: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNKSt13runtime_error4whatEv@GLIBCXX_3.4
-   610: 00000000000b6a80     0 NOTYPE  GLOBAL DEFAULT   27 __bss_start
-   611: 0000000000013980     5 FUNC    GLOBAL DEFAULT   12 _Z16SplitK_ReductionP6__halfPfmmi
-   612: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyException_SetContext
-   613: 000000000001dff0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl16synchronizeEventEPv
-   614: 0000000000023850  1122 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIN3c108ArgumentESaIS1_EED2Ev
-   615: 00000000000155d0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7truedivERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   616: 00000000000b5438    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEEE
-   617: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyGILState_Ensure
-   618: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyEval_AcquireThread
-   619: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_SetString
-   620: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_CallObject
-   621: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThread_tss_set
-   622: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_demangle@CXXABI_1.3
-   623: 000000000001e070    10 FUNC    WEAK   DEFAULT   12 _ZN3c104cuda4impl13CUDAGuardImplD0Ev
-   624: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN5torch11CppFunctionD1Ev
-   625: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN2at4_ops15to_dtype_layout4callERKNS_6TensorESt8optionalIN3c1010ScalarTypeEES5_INS6_6LayoutEES5_INS6_6DeviceEES5_IbEbbS5_INS6_12MemoryFormatEE
-   626: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSolsEi@GLIBCXX_3.4
-   627: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNR5torch7Library4_defEON3c1014FunctionSchemaEPNS1_12OperatorNameERKSt6vectorIN2at3TagESaIS8_EENS_17_RegisterOrVerifyE
-   628: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaStreamWaitEvent@libcudart.so.12
-   629: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZN3c104cuda20CUDACachingAllocator9allocatorE
-   630: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_guard_acquire@CXXABI_1.3
-   631: 00000000000b58d0    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEEE
-   632: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104cuda17getStreamFromPoolEia
-   633: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt16invalid_argumentC1EPKc
-   634: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_IsInstance
-   635: 000000000001e000     6 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl4typeEv
-   636: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt16invalid_argumentD1Ev@GLIBCXX_3.4
-   637: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTISt16invalid_argument@GLIBCXX_3.4
-   638: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
-   639: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c1021AutogradMetaInterfaceD2Ev
-   640: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyMem_Free
-   641: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThreadState_Get
-   642: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZSt17current_exceptionv@CXXABI_1.3.3
-   643: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSo9_M_insertIlEERSoT_@GLIBCXX_3.4.9
-   644: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_allocate_exception@CXXABI_1.3
-   645: 0000000000022570   482 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl17synchronizeStreamERKNS_6StreamE
-   646: 0000000000035070    18 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorES0_E
-   647: 0000000000023780   204 FUNC    WEAK   DEFAULT   12 _ZN3c106detail30inferFunctionSchemaFromFunctorIPFN2at6TensorERKS3_S5_dEEESt10unique_ptrINS_14FunctionSchemaESt14default_deleteIS9_EEv
-   648: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyType_Type
-   649: 000000000001def0    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl9setDeviceENS_6DeviceE
-   650: 000000000001df40    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl23getStreamFromGlobalPoolENS_6DeviceEb
-   651: 00000000000156f0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl6is_intEv
-   652: 0000000000015600    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3mulERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
-   653: 00000000000163b0   307 FUNC    WEAK   DEFAULT   12 _ZN9__gnu_cxx12__to_xstringISscEET_PFiPT0_mPKS2_P13__va_list_tagEmS5_z
-   654: 0000000000022b20  1113 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJRKcRKPS2_S4_S6_S4_EE4callES3_S6_S6_S6_S6_
-   655: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThreadState_New
-   656: 000000000001fa40   528 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl5blockEPvRKNS_6StreamE
-   657: 000000000001dfd0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl21recordDataPtrOnStreamERKNS_7DataPtrERKNS_6StreamE
-   658: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTVN5torch8autograd12AutogradMetaE
-   659: 0000000000014ed0     5 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl13constant_boolEv
-   660: 00000000000b5790    16 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104impl24DeviceGuardImplInterfaceE
-   661: 00000000000b5460    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1020intrusive_ptr_targetE
-   662: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_Repr
-   663: 0000000000014ea0    16 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl10nested_intEv
-   664: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyProperty_Type
-   665: 00000000000251e0    19 FUNC    WEAK   DEFAULT   12 _ZNSt19bad_optional_accessD1Ev
-   666: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyFrame_GetLineNumber
-   667: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strchr@GLIBC_2.2.5
-   668: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZdlPvm
-   669: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_NormalizeException
-   670: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_ClearWeakRefs
-   671: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_Next
-   672: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt9basic_iosIcSt11char_traitsIcEE4initEPSt15basic_streambufIcS1_E@GLIBCXX_3.4
-   673: 00000000000184f0   122 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEEC2EPS2_
-   674: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTISt9bad_alloc@GLIBCXX_3.4
-   675: 00000000000b5408    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1015VariableVersion14VersionCounterE
-   676: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNKSt15basic_stringbufIcSt11char_traitsIcESaIcEE3strEv@GLIBCXX_3.4
-   677: 00000000000b5938    16 OBJECT  WEAK   DEFAULT   21 _ZTISt11_Mutex_baseILN9__gnu_cxx12_Lock_policyE2EE
-   678: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs9_M_mutateEmmm@GLIBCXX_3.4
-   679: 000000000001bed0  8158 FUNC    GLOBAL DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220210nms_kernelERKN2at6TensorES4_d
+   444: 000000000001e690   204 FUNC    WEAK   DEFAULT   12 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py
+   445: 00000000000b53f0    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1011SymNodeImplE
+   446: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZSt24__throw_out_of_range_fmtPKcz
+   447: 00000000000158b0   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EEfEvPK5uint4PK6__halfS7_PT0_mmmi
+   448: 00000000000170d0    37 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED0Ev
+   449: 0000000000015240    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl13is_contiguousENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
+   450: 0000000000017120    37 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImplD0Ev
+   451: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs6assignERKSs@GLIBCXX_3.4
+   452: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs6assignEPKcm@GLIBCXX_3.4
+   453: 0000000000015300    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl6sym_orERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   454: 00000000000155a0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3powERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   455: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c106detail23torchInternalAssertFailEPKcS2_jS2_RKSs
+   456: 00000000000255a0   291 FUNC    GLOBAL DEFAULT   12 PyInit__C
+   457: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs6appendERKSs@GLIBCXX_3.4
+   458: 0000000000035120    21 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorES0_S0_E
+   459: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTuple_GetItem
+   460: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt15__exception_ptrneERKNS_13exception_ptrES2_@CXXABI_1.3.3
+   461: 0000000000024910  2235 FUNC    GLOBAL DEFAULT   12 _ZN7torchao28weight_matrix_prepacking_cpuEN2at6TensorE
+   462: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _PyObject_GetDictPtr
+   463: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK2at6Tensor5indexESt16initializer_listINS_8indexing11TensorIndexEE
+   464: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_atexit@GLIBC_2.2.5
+   465: 00000000000b5688    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1014OperatorKernelE
+   466: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK2at10TensorBase8data_ptrIlEEPT_v
+   467: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTuple_SetItem
+   468: 0000000000015c70   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi8EEfEvPK5uint4PK6__halfS7_PT0_mmmi
+   469: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThread_tss_get
+   470: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Restore
+   471: 0000000000019740   171 FUNC    GLOBAL DEFAULT   12 _Z29weight_prepacking_fp16_to_fp6PtPhmm
+   472: 0000000000018a30   275 FUNC    WEAK   DEFAULT   12 _ZN5torch5emptyEN3c108ArrayRefIlEENS0_13TensorOptionsESt8optionalINS0_12MemoryFormatEE
+   473: 0000000000016300   164 FUNC    WEAK   DEFAULT   12 _ZN5torch7LibraryD1Ev
+   474: 000000000001e010     1 FUNC    WEAK   DEFAULT   12 _ZN3c104cuda4impl13CUDAGuardImplD1Ev
+   475: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_pure_virtual@CXXABI_1.3
+   476: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __pthread_key_create@GLIBC_2.2.5
+   477: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt15__exception_ptr13exception_ptr4swapERS0_@CXXABI_1.3.3
+   478: 0000000000015090    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl10wrap_floatEd
+   479: 000000000001fc50   979 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl6recordEPPvRKNS_6StreamEaNS_9EventFlagE
+   480: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNR5torch7Library5_implEPKcONS_11CppFunctionENS_17_RegisterOrVerifyE
+   481: 0000000000026570   141 FUNC    WEAK   DEFAULT   12 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EPKS3_RKS6_
+   482: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSsC1ERKSaIcE@GLIBCXX_3.4
+   483: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104cuda9GetDeviceEPa
+   484: 0000000000015760    70 FUNC    WEAK   DEFAULT   12 _ZN3c1014getTypePtrCopyIN2at6TensorEEENS_4Type24SingletonOrSharedTypePtrIS3_EEv
+   485: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs4_Rep10_M_destroyERKSaIcE@GLIBCXX_3.4
+   486: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt15__exception_ptr13exception_ptrD1Ev@CXXABI_1.3.3
+   487: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN2at4_ops12index_select4callERKNS_6TensorElS4_
+   488: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThread_tss_alloc
+   489: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTISt16nested_exception@CXXABI_1.3.5
+   490: 0000000000015450    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2leERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   491: 000000000001ded0    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl14exchangeDeviceENS_6DeviceE
+   492: 000000000001df30    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl16getDefaultStreamENS_6DeviceE
+   493: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN6caffe28TypeMeta26error_unsupported_typemetaES0_
+   494: 00000000000156c0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7is_boolEv
+   495: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTISt13runtime_error@GLIBCXX_3.4
+   496: 0000000000017060    19 FUNC    WEAK   DEFAULT   12 _ZN3c1014OperatorKernelD1Ev
+   497: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaGetErrorString@libcudart.so.12
+   498: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt13runtime_errorC1ERKSs@GLIBCXX_3.4
+   499: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN2at4_ops6narrow4callERKNS_6TensorElN3c106SymIntES6_
+   500: 00000000000154e0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2neERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   501: 0000000000018570  1207 FUNC    WEAK   DEFAULT   12 _ZN5torch8autograd13make_variableEN2at6TensorEbb
+   502: 000000000001f110   139 FUNC    WEAK   DEFAULT   12 _ZNSt15basic_stringbufIcSt11char_traitsIcESaIcEED0Ev
+   503: 0000000000017010    19 FUNC    WEAK   DEFAULT   12 _ZN3c1015VariableVersion14VersionCounterD1Ev
+   504: 000000000001e760   651 FUNC    WEAK   DEFAULT   12 _ZN3c1010ValueErrorD1Ev
+   505: 0000000000014fd0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl11guard_floatEPKcl
+   506: 0000000000026470    95 FUNC    WEAK   DEFAULT   12 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EOS6_S7_
+   507: 00000000000348e0    20 OBJECT  WEAK   DEFAULT   14 _ZTSN3c1011SymNodeImplE
+   508: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZSt16__ostream_insertIcSt11char_traitsIcEERSt13basic_ostreamIT_T0_ES6_PKS3_l@GLIBCXX_3.4.9
+   509: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
+   510: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCFunction_Type
+   511: 00000000000170b0    19 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED2Ev
+   512: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSsC1ERKSsmm@GLIBCXX_3.4
+   513: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyGILState_GetThisThreadState
+   514: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyBytes_AsStringAndSize
+   515: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND memcmp@GLIBC_2.2.5
+   516: 0000000000017480    95 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEE6reset_Ev
+   517: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_AsEncodedString
+   518: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNKSs7compareEPKc@GLIBCXX_3.4
+   519: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK2at10TensorBase8data_ptrIN3c104HalfEEEPT_v
+   520: 0000000000017100    19 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImplD2Ev
+   521: 0000000000014f40    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl8has_hintEv
+   522: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyTuple_New
+   523: 0000000000015ef0   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi2EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi
+   524: 0000000000015800   164 FUNC    WEAK   DEFAULT   12 _ZN5torch6detail16TorchLibraryInitD1Ev
+   525: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_CallFunctionObjArgs
+   526: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104impl23ExcludeDispatchKeyGuardC1ENS_14DispatchKeySetE
+   527: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK2at10TensorBase8data_ptrIhEEPT_v
+   528: 00000000000251d0     8 FUNC    WEAK   DEFAULT   12 _ZNKSt19bad_optional_access4whatEv
+   529: 00000000000b5948    24 OBJECT  WEAK   DEFAULT   21 _ZTISt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE
+   530: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaEventSynchronize@libcudart.so.12
+   531: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104cuda20getDefaultCUDAStreamEa
+   532: 00000000000242a0  1638 FUNC    GLOBAL DEFAULT   12 _Z24weight_matrix_prepackingPiS_mm
+   533: 00000000000162b0    70 FUNC    WEAK   DEFAULT   12 _ZNK3c1010TensorImpl6deviceEv
+   534: 0000000000026770   959 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIbSaIbEE13_M_insert_auxESt13_Bit_iteratorb
+   535: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c10lsERSoNS_10DeviceTypeE
+   536: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTTSt19basic_ostringstreamIcSt11char_traitsIcESaIcEE@GLIBCXX_3.4
+   537: 000000000001f970   195 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl14exchangeDeviceENS_6DeviceE
+   538: 0000000000014e60     1 FUNC    WEAK   DEFAULT   12 _ZN3c1020intrusive_ptr_target17release_resourcesEv
+   539: 000000000002b580   294 FUNC    WEAK   DEFAULT   12 _ZNSt10_HashtableISsSt4pairIKSsPvESaIS3_ENSt8__detail10_Select1stESt8equal_toISsESt4hashISsENS5_18_Mod_range_hashingENS5_20_Default_ranged_hashENS5_20_Prime_rehash_policyENS5_17_Hashtable_traitsILb1ELb0ELb1EEEE9_M_rehashEmRKm
+   540: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_ImportError
+   541: 0000000000015480    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl2ltERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   542: 0000000000014e70     3 FUNC    WEAK   DEFAULT   12 _ZNK3c1011SymNodeImpl13is_nested_intEv
+   543: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt19basic_ostringstreamIcSt11char_traitsIcESaIcEEC1Ev
+   544: 00000000000b56d8    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE
+   545: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_Occurred
+   546: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThreadState_DeleteCurrent
+   547: 00000000000172b0   162 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_11SymNodeImplENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev
+   548: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK2at10TensorBase8data_ptrIiEEPT_v
+   549: 0000000000016030   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi
+   550: 00000000000b56f0    16 OBJECT  WEAK   DEFAULT   21 _ZTIFN2at6TensorES0_E
+   551: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaEventRecord@libcudart.so.12
+   552: 000000000001b070    37 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED0Ev
+   553: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyWeakref_NewRef
+   554: 000000000002b6b0   478 FUNC    WEAK   DEFAULT   12 _ZNSt8__detail9_Map_baseISsSt4pairIKSsPvESaIS4_ENS_10_Select1stESt8equal_toISsESt4hashISsENS_18_Mod_range_hashingENS_20_Default_ranged_hashENS_20_Prime_rehash_policyENS_17_Hashtable_traitsILb1ELb0ELb1EEELb1EEixEOSs
+   555: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK3c105Error4whatEv
+   556: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSsC1EPKcRKSaIcE@GLIBCXX_3.4
+   557: 000000000001e2e0   106 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl14exchangeStreamENS_6StreamE
+   558: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs7reserveEm@GLIBCXX_3.4
+   559: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaFuncSetAttribute@libcudart.so.12
+   560: 000000000001b020    37 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEED0Ev
+   561: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_AsUTF8String
+   562: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyEval_GetBuiltins
+   563: 0000000000020d70  4722 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl12destroyEventEPva
+   564: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTISt14overflow_error@GLIBCXX_3.4
+   565: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_ValueError
+   566: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND printf@GLIBC_2.2.5
+   567: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs7replaceEmmPKcm@GLIBCXX_3.4
+   568: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt13runtime_errorC2ERKSs@GLIBCXX_3.4
+   569: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN5torch3jit11parseSchemaERKSs
+   570: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104warnERKNS_7WarningE
+   571: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSsC1ERKSs@GLIBCXX_3.4
+   572: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND memcpy@GLIBC_2.14
+   573: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaEventCreateWithFlags@libcudart.so.12
+   574: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTIN10__cxxabiv115__forced_unwindE@CXXABI_1.3.2
+   575: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt9bad_allocD1Ev@GLIBCXX_3.4
+   576: 0000000000020030   197 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEED1Ev
+   577: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs6appendEmc@GLIBCXX_3.4
+   578: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCapsule_GetName
+   579: 00000000000159f0   311 FUNC    WEAK   DEFAULT   12 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi2EEfEvPK5uint4PK6__halfS7_PT0_mmmi
+   580: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs6appendERKSsmm@GLIBCXX_3.4
+   581: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZSt17__throw_bad_allocv@GLIBCXX_3.4
+   582: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _Znwm@GLIBCXX_3.4
+   583: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_OverflowError
+   584: 000000000001dfe0    16 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl11elapsedTimeEPvS2_a
+   585: 000000000001e080    10 FUNC    WEAK   DEFAULT   12 _ZN3c104impl16VirtualGuardImplD0Ev
+   586: 0000000000014fa0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl4int_Ev
+   587: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
+   588: 00000000000179e0  2600 FUNC    WEAK   DEFAULT   12 _ZN3c1014FunctionSchemaD2Ev
+   589: 0000000000026520    66 FUNC    WEAK   DEFAULT   12 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EOS6_PKS3_
+   590: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND free@GLIBC_2.2.5
+   591: 000000000001e050    31 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl9getStreamENS_6DeviceE
+   592: 000000000001e760   651 FUNC    WEAK   DEFAULT   12 _ZN3c1010ValueErrorD2Ev
+   593: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt19basic_ostringstreamIcSt11char_traitsIcESaIcEED1Ev@GLIBCXX_3.4
+   594: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTVSt15basic_stringbufIcSt11char_traitsIcESaIcEE@GLIBCXX_3.4
+   595: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5
+   596: 0000000000036220   119 OBJECT  WEAK   DEFAULT   14 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEEE
+   597: 000000000001df90    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl10queryEventEPv
+   598: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_Type
+   599: 0000000000036530    24 OBJECT  WEAK   DEFAULT   14 _ZTSSt19bad_optional_access
+   600: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTISt12domain_error@GLIBCXX_3.4
+   601: 0000000000016870   338 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKiEE4callERKS3_S5_
+   602: 0000000000016dc0   338 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJPKcRKjEE4callERKS3_S5_
+   603: 000000000001eca0   202 FUNC    WEAK   DEFAULT   12 _ZN3c1014DispatchKeySetC2ENS_11DispatchKeyE
+   604: 0000000000020030   197 FUNC    WEAK   DEFAULT   12 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEED2Ev
+   605: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCMethod_New
+   606: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaGetLastError@libcudart.so.12
+   607: 00000000000b56b0    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEEE
+   608: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNK3c1017SymbolicShapeMeta18init_is_contiguousEv
+   609: 0000000000014e80     9 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl20guard_size_obliviousEPKcl
+   610: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNKSt13runtime_error4whatEv@GLIBCXX_3.4
+   611: 00000000000b6a80     0 NOTYPE  GLOBAL DEFAULT   27 __bss_start
+   612: 0000000000013980     5 FUNC    GLOBAL DEFAULT   12 _Z16SplitK_ReductionP6__halfPfmmi
+   613: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyException_SetContext
+   614: 000000000001dff0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl16synchronizeEventEPv
+   615: 0000000000023850  1122 FUNC    WEAK   DEFAULT   12 _ZNSt6vectorIN3c108ArgumentESaIS1_EED2Ev
+   616: 00000000000155d0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl7truedivERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   617: 00000000000b5438    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEEE
+   618: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyGILState_Ensure
+   619: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyEval_AcquireThread
+   620: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_SetString
+   621: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_CallObject
+   622: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThread_tss_set
+   623: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_demangle@CXXABI_1.3
+   624: 000000000001e070    10 FUNC    WEAK   DEFAULT   12 _ZN3c104cuda4impl13CUDAGuardImplD0Ev
+   625: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN5torch11CppFunctionD1Ev
+   626: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN2at4_ops15to_dtype_layout4callERKNS_6TensorESt8optionalIN3c1010ScalarTypeEES5_INS6_6LayoutEES5_INS6_6DeviceEES5_IbEbbS5_INS6_12MemoryFormatEE
+   627: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSolsEi@GLIBCXX_3.4
+   628: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNR5torch7Library4_defEON3c1014FunctionSchemaEPNS1_12OperatorNameERKSt6vectorIN2at3TagESaIS8_EENS_17_RegisterOrVerifyE
+   629: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaStreamWaitEvent@libcudart.so.12
+   630: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZN3c104cuda20CUDACachingAllocator9allocatorE
+   631: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_guard_acquire@CXXABI_1.3
+   632: 00000000000b58d0    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEEE
+   633: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c104cuda17getStreamFromPoolEia
+   634: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt16invalid_argumentC1EPKc
+   635: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_IsInstance
+   636: 000000000001e000     6 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl4typeEv
+   637: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt16invalid_argumentD1Ev@GLIBCXX_3.4
+   638: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTISt16invalid_argument@GLIBCXX_3.4
+   639: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
+   640: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c1021AutogradMetaInterfaceD2Ev
+   641: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyMem_Free
+   642: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThreadState_Get
+   643: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZSt17current_exceptionv@CXXABI_1.3.3
+   644: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSo9_M_insertIlEERSoT_@GLIBCXX_3.4.9
+   645: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_allocate_exception@CXXABI_1.3
+   646: 0000000000022570   482 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl17synchronizeStreamERKNS_6StreamE
+   647: 0000000000035070    18 OBJECT  WEAK   DEFAULT   14 _ZTSFN2at6TensorES0_E
+   648: 0000000000023780   204 FUNC    WEAK   DEFAULT   12 _ZN3c106detail30inferFunctionSchemaFromFunctorIPFN2at6TensorERKS3_S5_dEEESt10unique_ptrINS_14FunctionSchemaESt14default_deleteIS9_EEv
+   649: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyType_Type
+   650: 000000000001def0    10 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl9setDeviceENS_6DeviceE
+   651: 000000000001df40    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl23getStreamFromGlobalPoolENS_6DeviceEb
+   652: 00000000000156f0    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl6is_intEv
+   653: 0000000000015600    35 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl3mulERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
+   654: 00000000000163b0   307 FUNC    WEAK   DEFAULT   12 _ZN9__gnu_cxx12__to_xstringISscEET_PFiPT0_mPKS2_P13__va_list_tagEmS5_z
+   655: 0000000000022b20  1113 FUNC    WEAK   DEFAULT   12 _ZN3c106detail12_str_wrapperIJRKcRKPS2_S4_S6_S4_EE4callES3_S6_S6_S6_S6_
+   656: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyThreadState_New
+   657: 000000000001fa40   528 FUNC    WEAK   DEFAULT   12 _ZNK3c104cuda4impl13CUDAGuardImpl5blockEPvRKNS_6StreamE
+   658: 000000000001dfd0    13 FUNC    WEAK   DEFAULT   12 _ZNK3c104impl16VirtualGuardImpl21recordDataPtrOnStreamERKNS_7DataPtrERKNS_6StreamE
+   659: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTVN5torch8autograd12AutogradMetaE
+   660: 0000000000014ed0     5 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl13constant_boolEv
+   661: 00000000000b5790    16 OBJECT  WEAK   DEFAULT   21 _ZTIN3c104impl24DeviceGuardImplInterfaceE
+   662: 00000000000b5460    40 OBJECT  WEAK   DEFAULT   21 _ZTVN3c1020intrusive_ptr_targetE
+   663: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_Repr
+   664: 0000000000014ea0    16 FUNC    WEAK   DEFAULT   12 _ZN3c1011SymNodeImpl10nested_intEv
+   665: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyProperty_Type
+   666: 00000000000251e0    19 FUNC    WEAK   DEFAULT   12 _ZNSt19bad_optional_accessD1Ev
+   667: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyFrame_GetLineNumber
+   668: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND strchr@GLIBC_2.2.5
+   669: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZdlPvm
+   670: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyErr_NormalizeException
+   671: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyObject_ClearWeakRefs
+   672: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyDict_Next
+   673: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSt9basic_iosIcSt11char_traitsIcEE4initEPSt15basic_streambufIcS1_E@GLIBCXX_3.4
+   674: 00000000000184f0   122 FUNC    WEAK   DEFAULT   12 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEEC2EPS2_
+   675: 0000000000000000     0 OBJECT  GLOBAL DEFAULT  UND _ZTISt9bad_alloc@GLIBCXX_3.4
+   676: 00000000000b5408    24 OBJECT  WEAK   DEFAULT   21 _ZTIN3c1015VariableVersion14VersionCounterE
+   677: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNKSt15basic_stringbufIcSt11char_traitsIcESaIcEE3strEv@GLIBCXX_3.4
+   678: 00000000000b5938    16 OBJECT  WEAK   DEFAULT   21 _ZTISt11_Mutex_baseILN9__gnu_cxx12_Lock_policyE2EE
+   679: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZNSs9_M_mutateEmmm@GLIBCXX_3.4
    680: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyCapsule_GetPointer
    681: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _ZN3c1010TensorImpl17set_autograd_metaESt10unique_ptrINS_21AutogradMetaInterfaceESt14default_deleteIS2_EE
    682: 000000000001f090   123 FUNC    WEAK   DEFAULT   12 _ZNSt15basic_stringbufIcSt11char_traitsIcESaIcEED1Ev
    683: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Py_NoneStruct
    684: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __cxa_guard_release@CXXABI_1.3
    685: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND cudaEventQuery@libcudart.so.12
    686: 0000000000023ee0   183 FUNC    GLOBAL DEFAULT   12 _Z20BitInterleaving_4bitPh
```

### readelf --wide --relocs {}

```diff
@@ -41,15 +41,15 @@
 00000000000b69e8  0000000000000008 R_X86_64_RELATIVE                         b5990
 00000000000b6a40  0000000000000008 R_X86_64_RELATIVE                         37988
 00000000000b6a58  0000000000000008 R_X86_64_RELATIVE                         9d658
 00000000000b6a70  0000000000000008 R_X86_64_RELATIVE                         9de68
 00000000000b53e0  0000003800000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3 + 10
 00000000000b5790  0000003800000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3 + 10
 00000000000b5938  0000003800000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3 + 10
-00000000000b53e8  0000016f00000001 R_X86_64_64            00000000000348c0 _ZTSN3c1020intrusive_ptr_targetE + 0
+00000000000b53e8  0000017000000001 R_X86_64_64            00000000000348c0 _ZTSN3c1020intrusive_ptr_targetE + 0
 00000000000b53f0  0000010e00000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 + 10
 00000000000b5408  0000010e00000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 + 10
 00000000000b5420  0000010e00000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 + 10
 00000000000b5438  0000010e00000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 + 10
 00000000000b56d8  0000010e00000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 + 10
 00000000000b5700  0000010e00000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 + 10
 00000000000b5778  0000010e00000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 + 10
@@ -58,391 +58,391 @@
 00000000000b58f8  0000010e00000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 + 10
 00000000000b5948  0000010e00000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 + 10
 00000000000b5960  0000010e00000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 + 10
 00000000000b5978  0000010e00000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 + 10
 00000000000b5990  0000010e00000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 + 10
 00000000000b59a8  0000010e00000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 + 10
 00000000000b59c0  0000010e00000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 + 10
-00000000000b53f8  000001d000000001 R_X86_64_64            00000000000348e0 _ZTSN3c1011SymNodeImplE + 0
-00000000000b5400  000001d400000001 R_X86_64_64            00000000000b53e0 _ZTIN3c1020intrusive_ptr_targetE + 0
-00000000000b5418  000001d400000001 R_X86_64_64            00000000000b53e0 _ZTIN3c1020intrusive_ptr_targetE + 0
-00000000000b5430  000001d400000001 R_X86_64_64            00000000000b53e0 _ZTIN3c1020intrusive_ptr_targetE + 0
-00000000000b5468  000001d400000001 R_X86_64_64            00000000000b53e0 _ZTIN3c1020intrusive_ptr_targetE + 0
-00000000000b5410  000001e200000001 R_X86_64_64            0000000000034900 _ZTSN3c1015VariableVersion14VersionCounterE + 0
-00000000000b5428  0000022700000001 R_X86_64_64            0000000000034930 _ZTSN3c1014OperatorKernelE + 0
-00000000000b5440  000001f100000001 R_X86_64_64            0000000000034960 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEEE + 0
-00000000000b5448  0000016400000001 R_X86_64_64            00000000000b5420 _ZTIN3c1014OperatorKernelE + 0
-00000000000b5690  0000016400000001 R_X86_64_64            00000000000b5420 _ZTIN3c1014OperatorKernelE + 0
-00000000000b56e8  0000016400000001 R_X86_64_64            00000000000b5420 _ZTIN3c1014OperatorKernelE + 0
-00000000000b5710  0000016400000001 R_X86_64_64            00000000000b5420 _ZTIN3c1014OperatorKernelE + 0
-00000000000b57c8  0000016400000001 R_X86_64_64            00000000000b5420 _ZTIN3c1014OperatorKernelE + 0
+00000000000b53f8  000001cf00000001 R_X86_64_64            00000000000348e0 _ZTSN3c1011SymNodeImplE + 0
+00000000000b5400  000001d300000001 R_X86_64_64            00000000000b53e0 _ZTIN3c1020intrusive_ptr_targetE + 0
+00000000000b5418  000001d300000001 R_X86_64_64            00000000000b53e0 _ZTIN3c1020intrusive_ptr_targetE + 0
+00000000000b5430  000001d300000001 R_X86_64_64            00000000000b53e0 _ZTIN3c1020intrusive_ptr_targetE + 0
+00000000000b5468  000001d300000001 R_X86_64_64            00000000000b53e0 _ZTIN3c1020intrusive_ptr_targetE + 0
+00000000000b5410  000001e000000001 R_X86_64_64            0000000000034900 _ZTSN3c1015VariableVersion14VersionCounterE + 0
+00000000000b5428  0000022600000001 R_X86_64_64            0000000000034930 _ZTSN3c1014OperatorKernelE + 0
+00000000000b5440  000001ef00000001 R_X86_64_64            0000000000034960 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEEE + 0
+00000000000b5448  0000016500000001 R_X86_64_64            00000000000b5420 _ZTIN3c1014OperatorKernelE + 0
+00000000000b5690  0000016500000001 R_X86_64_64            00000000000b5420 _ZTIN3c1014OperatorKernelE + 0
+00000000000b56e8  0000016500000001 R_X86_64_64            00000000000b5420 _ZTIN3c1014OperatorKernelE + 0
+00000000000b5710  0000016500000001 R_X86_64_64            00000000000b5420 _ZTIN3c1014OperatorKernelE + 0
+00000000000b57c8  0000016500000001 R_X86_64_64            00000000000b5420 _ZTIN3c1014OperatorKernelE + 0
 00000000000b5450  0000004300000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__function_type_infoE@CXXABI_1.3 + 10
 00000000000b56f0  0000004300000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__function_type_infoE@CXXABI_1.3 + 10
 00000000000b5718  0000004300000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__function_type_infoE@CXXABI_1.3 + 10
 00000000000b57d0  0000004300000001 R_X86_64_64            0000000000000000 _ZTVN10__cxxabiv120__function_type_infoE@CXXABI_1.3 + 10
-00000000000b5458  000001dc00000001 R_X86_64_64            00000000000349e0 _ZTSFN2at6TensorES0_S0_S0_lE + 0
-00000000000b5470  0000023000000001 R_X86_64_64            0000000000016f20 _ZN3c1020intrusive_ptr_targetD1Ev + 0
-00000000000b5478  000001ff00000001 R_X86_64_64            0000000000016ff0 _ZN3c1020intrusive_ptr_targetD0Ev + 0
-00000000000b5480  0000018c00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
-00000000000b54a8  0000018c00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
-00000000000b5680  0000018c00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
-00000000000b56a8  0000018c00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
-00000000000b56d0  0000018c00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
-00000000000b5748  0000018c00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
-00000000000b5770  0000018c00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
-00000000000b58f0  0000018c00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
-00000000000b5e68  0000018c00000006 R_X86_64_GLOB_DAT      0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
+00000000000b5458  000001da00000001 R_X86_64_64            00000000000349e0 _ZTSFN2at6TensorES0_S0_S0_lE + 0
+00000000000b5470  0000022f00000001 R_X86_64_64            0000000000016f20 _ZN3c1020intrusive_ptr_targetD1Ev + 0
+00000000000b5478  000001fd00000001 R_X86_64_64            0000000000016ff0 _ZN3c1020intrusive_ptr_targetD0Ev + 0
+00000000000b5480  0000018d00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
+00000000000b54a8  0000018d00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
+00000000000b5680  0000018d00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
+00000000000b56a8  0000018d00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
+00000000000b56d0  0000018d00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
+00000000000b5748  0000018d00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
+00000000000b5770  0000018d00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
+00000000000b58f0  0000018d00000001 R_X86_64_64            0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
+00000000000b5e70  0000018d00000006 R_X86_64_GLOB_DAT      0000000000014e60 _ZN3c1020intrusive_ptr_target17release_resourcesEv + 0
 00000000000b5490  0000025000000001 R_X86_64_64            00000000000b53f0 _ZTIN3c1011SymNodeImplE + 0
-00000000000b5498  000001c800000001 R_X86_64_64            0000000000017100 _ZN3c1011SymNodeImplD1Ev + 0
+00000000000b5498  000001c700000001 R_X86_64_64            0000000000017100 _ZN3c1011SymNodeImplD1Ev + 0
 00000000000b54a0  000001a000000001 R_X86_64_64            0000000000017120 _ZN3c1011SymNodeImplD0Ev + 0
-00000000000b5df8  000001a000000006 R_X86_64_GLOB_DAT      0000000000017120 _ZN3c1011SymNodeImplD0Ev + 0
+00000000000b5e00  000001a000000006 R_X86_64_GLOB_DAT      0000000000017120 _ZN3c1011SymNodeImplD0Ev + 0
 00000000000b54b0  0000013500000001 R_X86_64_64            00000000000156f0 _ZN3c1011SymNodeImpl6is_intEv + 0
-00000000000b54b8  0000017500000001 R_X86_64_64            00000000000156c0 _ZN3c1011SymNodeImpl7is_boolEv + 0
-00000000000b54c0  000001c500000001 R_X86_64_64            0000000000015690 _ZN3c1011SymNodeImpl8is_floatEv + 0
+00000000000b54b8  0000017600000001 R_X86_64_64            00000000000156c0 _ZN3c1011SymNodeImpl7is_boolEv + 0
+00000000000b54c0  000001c400000001 R_X86_64_64            0000000000015690 _ZN3c1011SymNodeImpl8is_floatEv + 0
 00000000000b54c8  0000025b00000001 R_X86_64_64            0000000000014e70 _ZNK3c1011SymNodeImpl13is_nested_intEv + 0
-00000000000b54d0  0000024500000001 R_X86_64_64            0000000000015660 _ZN3c1011SymNodeImpl3addERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
+00000000000b54d0  0000024400000001 R_X86_64_64            0000000000015660 _ZN3c1011SymNodeImpl3addERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
 00000000000b54d8  0000019f00000001 R_X86_64_64            0000000000015630 _ZN3c1011SymNodeImpl3subERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
-00000000000b54e0  0000021600000001 R_X86_64_64            0000000000015600 _ZN3c1011SymNodeImpl3mulERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
-00000000000b54e8  0000017000000001 R_X86_64_64            00000000000155d0 _ZN3c1011SymNodeImpl7truedivERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
-00000000000b54f0  000001e400000001 R_X86_64_64            00000000000155a0 _ZN3c1011SymNodeImpl3powERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
-00000000000b54f8  0000014c00000001 R_X86_64_64            0000000000015570 _ZN3c1011SymNodeImpl8floordivERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
+00000000000b54e0  0000021500000001 R_X86_64_64            0000000000015600 _ZN3c1011SymNodeImpl3mulERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
+00000000000b54e8  0000017100000001 R_X86_64_64            00000000000155d0 _ZN3c1011SymNodeImpl7truedivERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
+00000000000b54f0  000001e200000001 R_X86_64_64            00000000000155a0 _ZN3c1011SymNodeImpl3powERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
+00000000000b54f8  0000014d00000001 R_X86_64_64            0000000000015570 _ZN3c1011SymNodeImpl8floordivERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
 00000000000b5500  000001ab00000001 R_X86_64_64            0000000000015540 _ZN3c1011SymNodeImpl3modERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
-00000000000b5508  0000020900000001 R_X86_64_64            0000000000015510 _ZN3c1011SymNodeImpl2eqERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
-00000000000b5510  000001cc00000001 R_X86_64_64            00000000000154e0 _ZN3c1011SymNodeImpl2neERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
-00000000000b5518  0000022a00000001 R_X86_64_64            00000000000154b0 _ZN3c1011SymNodeImpl2gtERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
-00000000000b5520  0000021300000001 R_X86_64_64            0000000000015480 _ZN3c1011SymNodeImpl2ltERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
+00000000000b5508  0000020700000001 R_X86_64_64            0000000000015510 _ZN3c1011SymNodeImpl2eqERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
+00000000000b5510  000001cb00000001 R_X86_64_64            00000000000154e0 _ZN3c1011SymNodeImpl2neERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
+00000000000b5518  0000022900000001 R_X86_64_64            00000000000154b0 _ZN3c1011SymNodeImpl2gtERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
+00000000000b5520  0000021200000001 R_X86_64_64            0000000000015480 _ZN3c1011SymNodeImpl2ltERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
 00000000000b5528  0000013800000001 R_X86_64_64            0000000000015450 _ZN3c1011SymNodeImpl2leERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
 00000000000b5530  0000014500000001 R_X86_64_64            0000000000015420 _ZN3c1011SymNodeImpl2geERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
-00000000000b5538  0000015100000001 R_X86_64_64            00000000000153f0 _ZN3c1011SymNodeImpl4ceilEv + 0
+00000000000b5538  0000015200000001 R_X86_64_64            00000000000153f0 _ZN3c1011SymNodeImpl4ceilEv + 0
 00000000000b5540  0000019600000001 R_X86_64_64            00000000000153c0 _ZN3c1011SymNodeImpl5floorEv + 0
-00000000000b5548  0000022f00000001 R_X86_64_64            0000000000015390 _ZN3c1011SymNodeImpl3negEv + 0
+00000000000b5548  0000022e00000001 R_X86_64_64            0000000000015390 _ZN3c1011SymNodeImpl3negEv + 0
 00000000000b5550  0000024f00000001 R_X86_64_64            0000000000015360 _ZN3c1011SymNodeImpl7sym_minERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
-00000000000b5558  000001e600000001 R_X86_64_64            0000000000015330 _ZN3c1011SymNodeImpl7sym_maxERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
+00000000000b5558  000001e400000001 R_X86_64_64            0000000000015330 _ZN3c1011SymNodeImpl7sym_maxERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
 00000000000b5560  0000020f00000001 R_X86_64_64            0000000000015300 _ZN3c1011SymNodeImpl6sym_orERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
 00000000000b5568  000001b100000001 R_X86_64_64            00000000000152d0 _ZN3c1011SymNodeImpl7sym_andERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE + 0
-00000000000b5570  0000020a00000001 R_X86_64_64            00000000000152a0 _ZN3c1011SymNodeImpl7sym_notEv + 0
-00000000000b5578  000001fb00000001 R_X86_64_64            0000000000015270 _ZN3c1011SymNodeImpl7sym_iteERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEES7_ + 0
-00000000000b5580  0000018100000001 R_X86_64_64            0000000000015240 _ZN3c1011SymNodeImpl13is_contiguousENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_ + 0
-00000000000b5588  0000019100000001 R_X86_64_64            0000000000015210 _ZN3c1011SymNodeImpl30is_channels_last_contiguous_2dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_ + 0
+00000000000b5570  0000020800000001 R_X86_64_64            00000000000152a0 _ZN3c1011SymNodeImpl7sym_notEv + 0
+00000000000b5578  000001f900000001 R_X86_64_64            0000000000015270 _ZN3c1011SymNodeImpl7sym_iteERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEES7_ + 0
+00000000000b5580  0000018200000001 R_X86_64_64            0000000000015240 _ZN3c1011SymNodeImpl13is_contiguousENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_ + 0
+00000000000b5588  0000019200000001 R_X86_64_64            0000000000015210 _ZN3c1011SymNodeImpl30is_channels_last_contiguous_2dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_ + 0
 00000000000b5590  0000025800000001 R_X86_64_64            00000000000151e0 _ZN3c1011SymNodeImpl30is_channels_last_contiguous_3dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_ + 0
-00000000000b5598  0000021a00000001 R_X86_64_64            00000000000151b0 _ZN3c1011SymNodeImpl27is_channels_last_strides_2dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_ + 0
-00000000000b55a0  000001c000000001 R_X86_64_64            0000000000015180 _ZN3c1011SymNodeImpl27is_channels_last_strides_3dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_ + 0
+00000000000b5598  0000021900000001 R_X86_64_64            00000000000151b0 _ZN3c1011SymNodeImpl27is_channels_last_strides_2dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_ + 0
+00000000000b55a0  000001bf00000001 R_X86_64_64            0000000000015180 _ZN3c1011SymNodeImpl27is_channels_last_strides_3dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_ + 0
 00000000000b55a8  0000013c00000001 R_X86_64_64            0000000000015150 _ZN3c1011SymNodeImpl28is_non_overlapping_and_denseENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_ + 0
-00000000000b55b0  0000016a00000001 R_X86_64_64            0000000000015120 _ZN3c1011SymNodeImpl5cloneEv + 0
-00000000000b55b8  0000018800000001 R_X86_64_64            00000000000150f0 _ZN3c1011SymNodeImpl9sym_floatEv + 0
+00000000000b55b0  0000016b00000001 R_X86_64_64            0000000000015120 _ZN3c1011SymNodeImpl5cloneEv + 0
+00000000000b55b8  0000018900000001 R_X86_64_64            00000000000150f0 _ZN3c1011SymNodeImpl9sym_floatEv + 0
 00000000000b55c0  0000025200000001 R_X86_64_64            00000000000150c0 _ZN3c1011SymNodeImpl8wrap_intEl + 0
-00000000000b55c8  000001e900000001 R_X86_64_64            0000000000015090 _ZN3c1011SymNodeImpl10wrap_floatEd + 0
-00000000000b55d0  0000017f00000001 R_X86_64_64            0000000000015060 _ZN3c1011SymNodeImpl9wrap_boolEb + 0
-00000000000b55d8  000001fc00000001 R_X86_64_64            0000000000015030 _ZN3c1011SymNodeImpl9guard_intEPKcl + 0
-00000000000b55e0  000001f400000001 R_X86_64_64            0000000000015000 _ZN3c1011SymNodeImpl10guard_boolEPKcl + 0
+00000000000b55c8  000001e700000001 R_X86_64_64            0000000000015090 _ZN3c1011SymNodeImpl10wrap_floatEd + 0
+00000000000b55d0  0000018000000001 R_X86_64_64            0000000000015060 _ZN3c1011SymNodeImpl9wrap_boolEb + 0
+00000000000b55d8  000001fa00000001 R_X86_64_64            0000000000015030 _ZN3c1011SymNodeImpl9guard_intEPKcl + 0
+00000000000b55e0  000001f200000001 R_X86_64_64            0000000000015000 _ZN3c1011SymNodeImpl10guard_boolEPKcl + 0
 00000000000b55e8  0000019700000001 R_X86_64_64            0000000000014fd0 _ZN3c1011SymNodeImpl11guard_floatEPKcl + 0
-00000000000b55f0  0000015700000001 R_X86_64_64            0000000000014e80 _ZN3c1011SymNodeImpl20guard_size_obliviousEPKcl + 0
-00000000000b55f8  000001bd00000001 R_X86_64_64            0000000000014e90 _ZN3c1011SymNodeImpl11expect_trueEPKcl + 0
-00000000000b5600  0000020400000001 R_X86_64_64            0000000000017360 _ZN3c1011SymNodeImpl11expect_sizeEPKcl + 0
-00000000000b5608  0000023600000001 R_X86_64_64            0000000000014fa0 _ZN3c1011SymNodeImpl4int_Ev + 0
-00000000000b5610  0000022100000001 R_X86_64_64            0000000000014f70 _ZN3c1011SymNodeImpl5bool_Ev + 0
-00000000000b5618  000001bf00000001 R_X86_64_64            0000000000014f40 _ZN3c1011SymNodeImpl8has_hintEv + 0
+00000000000b55f0  0000015800000001 R_X86_64_64            0000000000014e80 _ZN3c1011SymNodeImpl20guard_size_obliviousEPKcl + 0
+00000000000b55f8  000001bc00000001 R_X86_64_64            0000000000014e90 _ZN3c1011SymNodeImpl11expect_trueEPKcl + 0
+00000000000b5600  0000020200000001 R_X86_64_64            0000000000017360 _ZN3c1011SymNodeImpl11expect_sizeEPKcl + 0
+00000000000b5608  0000023500000001 R_X86_64_64            0000000000014fa0 _ZN3c1011SymNodeImpl4int_Ev + 0
+00000000000b5610  0000022000000001 R_X86_64_64            0000000000014f70 _ZN3c1011SymNodeImpl5bool_Ev + 0
+00000000000b5618  000001be00000001 R_X86_64_64            0000000000014f40 _ZN3c1011SymNodeImpl8has_hintEv + 0
 00000000000b5620  0000013d00000001 R_X86_64_64            0000000000014f10 _ZN3c1011SymNodeImpl3strEv + 0
-00000000000b5628  0000015000000001 R_X86_64_64            0000000000014ea0 _ZN3c1011SymNodeImpl10nested_intEv + 0
+00000000000b5628  0000015100000001 R_X86_64_64            0000000000014ea0 _ZN3c1011SymNodeImpl10nested_intEv + 0
 00000000000b5630  0000013200000001 R_X86_64_64            0000000000014eb0 _ZN3c1011SymNodeImpl16nested_int_coeffEv + 0
-00000000000b5638  0000018500000001 R_X86_64_64            0000000000014ec0 _ZN3c1011SymNodeImpl12constant_intEv + 0
-00000000000b5640  000001db00000001 R_X86_64_64            0000000000014ed0 _ZN3c1011SymNodeImpl13constant_boolEv + 0
+00000000000b5638  0000018600000001 R_X86_64_64            0000000000014ec0 _ZN3c1011SymNodeImpl12constant_intEv + 0
+00000000000b5640  000001d900000001 R_X86_64_64            0000000000014ed0 _ZN3c1011SymNodeImpl13constant_boolEv + 0
 00000000000b5648  000001a400000001 R_X86_64_64            0000000000014ee0 _ZN3c1011SymNodeImpl12maybe_as_intEv + 0
-00000000000b5650  000001de00000001 R_X86_64_64            0000000000014ef0 _ZN3c1011SymNodeImpl11is_constantEv + 0
-00000000000b5658  000001d600000001 R_X86_64_64            0000000000014f00 _ZN3c1011SymNodeImpl11is_symbolicEv + 0
-00000000000b5668  0000022e00000001 R_X86_64_64            00000000000b5408 _ZTIN3c1015VariableVersion14VersionCounterE + 0
-00000000000b5670  0000017200000001 R_X86_64_64            0000000000017010 _ZN3c1015VariableVersion14VersionCounterD1Ev + 0
+00000000000b5650  000001dc00000001 R_X86_64_64            0000000000014ef0 _ZN3c1011SymNodeImpl11is_constantEv + 0
+00000000000b5658  000001d500000001 R_X86_64_64            0000000000014f00 _ZN3c1011SymNodeImpl11is_symbolicEv + 0
+00000000000b5668  0000022d00000001 R_X86_64_64            00000000000b5408 _ZTIN3c1015VariableVersion14VersionCounterE + 0
+00000000000b5670  0000017300000001 R_X86_64_64            0000000000017010 _ZN3c1015VariableVersion14VersionCounterD1Ev + 0
 00000000000b5678  0000014600000001 R_X86_64_64            0000000000017030 _ZN3c1015VariableVersion14VersionCounterD0Ev + 0
-00000000000b5698  0000023c00000001 R_X86_64_64            0000000000017060 _ZN3c1014OperatorKernelD1Ev + 0
-00000000000b56a0  0000020b00000001 R_X86_64_64            0000000000017080 _ZN3c1014OperatorKernelD0Ev + 0
+00000000000b5698  0000023b00000001 R_X86_64_64            0000000000017060 _ZN3c1014OperatorKernelD1Ev + 0
+00000000000b56a0  0000020900000001 R_X86_64_64            0000000000017080 _ZN3c1014OperatorKernelD0Ev + 0
 00000000000b56b8  000001a100000001 R_X86_64_64            00000000000b5438 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEEE + 0
-00000000000b56c0  000001fe00000001 R_X86_64_64            00000000000170b0 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED1Ev + 0
-00000000000b56c8  000001d700000001 R_X86_64_64            00000000000170d0 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED0Ev + 0
-00000000000b56e0  0000014a00000001 R_X86_64_64            0000000000035000 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE + 0
-00000000000b56f8  0000022600000001 R_X86_64_64            0000000000035070 _ZTSFN2at6TensorES0_E + 0
-00000000000b5708  0000022200000001 R_X86_64_64            00000000000350a0 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE + 0
+00000000000b56c0  000001fc00000001 R_X86_64_64            00000000000170b0 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED1Ev + 0
+00000000000b56c8  000001d600000001 R_X86_64_64            00000000000170d0 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED0Ev + 0
+00000000000b56e0  0000014b00000001 R_X86_64_64            0000000000035000 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE + 0
+00000000000b56f8  0000022500000001 R_X86_64_64            0000000000035070 _ZTSFN2at6TensorES0_E + 0
+00000000000b5708  0000022100000001 R_X86_64_64            00000000000350a0 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE + 0
 00000000000b5720  0000019b00000001 R_X86_64_64            0000000000035120 _ZTSFN2at6TensorES0_S0_E + 0
-00000000000b5730  0000023e00000001 R_X86_64_64            00000000000b56d8 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE + 0
-00000000000b5738  0000023300000001 R_X86_64_64            000000000001b000 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEED1Ev + 0
-00000000000b5740  0000020200000001 R_X86_64_64            000000000001b020 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEED0Ev + 0
-00000000000b5758  0000022000000001 R_X86_64_64            00000000000b5700 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE + 0
-00000000000b5760  000001ee00000001 R_X86_64_64            000000000001b050 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED1Ev + 0
-00000000000b5768  000001ca00000001 R_X86_64_64            000000000001b070 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED0Ev + 0
-00000000000b5780  0000017100000001 R_X86_64_64            0000000000036190 _ZTSN3c1010ValueErrorE + 0
+00000000000b5730  0000023d00000001 R_X86_64_64            00000000000b56d8 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE + 0
+00000000000b5738  0000023200000001 R_X86_64_64            000000000001b000 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEED1Ev + 0
+00000000000b5740  0000020000000001 R_X86_64_64            000000000001b020 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEED0Ev + 0
+00000000000b5758  0000021f00000001 R_X86_64_64            00000000000b5700 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE + 0
+00000000000b5760  000001ec00000001 R_X86_64_64            000000000001b050 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED1Ev + 0
+00000000000b5768  000001c900000001 R_X86_64_64            000000000001b070 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED0Ev + 0
+00000000000b5780  0000017200000001 R_X86_64_64            0000000000036190 _ZTSN3c1010ValueErrorE + 0
 00000000000b5788  0000012b00000001 R_X86_64_64            0000000000000000 _ZTIN3c105ErrorE + 0
-00000000000b5798  000001dd00000001 R_X86_64_64            00000000000361c0 _ZTSN3c104impl24DeviceGuardImplInterfaceE + 0
-00000000000b57a8  0000024300000001 R_X86_64_64            0000000000036200 _ZTSN3c104cuda4impl13CUDAGuardImplE + 0
-00000000000b57b0  000001f600000001 R_X86_64_64            00000000000b5790 _ZTIN3c104impl24DeviceGuardImplInterfaceE + 0
-00000000000b57c0  000001df00000001 R_X86_64_64            0000000000036220 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEEE + 0
-00000000000b57d8  0000018a00000001 R_X86_64_64            00000000000362a0 _ZTSFN2at6TensorERKS0_S2_dE + 0
+00000000000b5798  000001db00000001 R_X86_64_64            00000000000361c0 _ZTSN3c104impl24DeviceGuardImplInterfaceE + 0
+00000000000b57a8  0000024200000001 R_X86_64_64            0000000000036200 _ZTSN3c104cuda4impl13CUDAGuardImplE + 0
+00000000000b57b0  000001f400000001 R_X86_64_64            00000000000b5790 _ZTIN3c104impl24DeviceGuardImplInterfaceE + 0
+00000000000b57c0  000001dd00000001 R_X86_64_64            0000000000036220 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEEE + 0
+00000000000b57d8  0000018b00000001 R_X86_64_64            00000000000362a0 _ZTSFN2at6TensorERKS0_S2_dE + 0
 00000000000b57e8  0000025a00000001 R_X86_64_64            00000000000b5778 _ZTIN3c1010ValueErrorE + 0
 00000000000b5de0  0000025a00000006 R_X86_64_GLOB_DAT      00000000000b5778 _ZTIN3c1010ValueErrorE + 0
-00000000000b57f0  0000016700000001 R_X86_64_64            000000000001e760 _ZN3c1010ValueErrorD1Ev + 0
-00000000000b5e38  0000016700000006 R_X86_64_GLOB_DAT      000000000001e760 _ZN3c1010ValueErrorD1Ev + 0
+00000000000b57f0  0000016800000001 R_X86_64_64            000000000001e760 _ZN3c1010ValueErrorD1Ev + 0
+00000000000b5e40  0000016800000006 R_X86_64_GLOB_DAT      000000000001e760 _ZN3c1010ValueErrorD1Ev + 0
 00000000000b57f8  0000013e00000001 R_X86_64_64            000000000001e9f0 _ZN3c1010ValueErrorD0Ev + 0
 00000000000b5800  0000009c00000001 R_X86_64_64            0000000000000000 _ZNK3c105Error4whatEv + 0
 00000000000b5808  000001a200000001 R_X86_64_64            000000000001deb0 _ZNK3c105Error22what_without_backtraceEv + 0
 00000000000b5818  0000024800000001 R_X86_64_64            00000000000b57a0 _ZTIN3c104cuda4impl13CUDAGuardImplE + 0
-00000000000b5820  0000021f00000001 R_X86_64_64            000000000001e000 _ZNK3c104cuda4impl13CUDAGuardImpl4typeEv + 0
+00000000000b5820  0000021e00000001 R_X86_64_64            000000000001e000 _ZNK3c104cuda4impl13CUDAGuardImpl4typeEv + 0
 00000000000b5828  0000025600000001 R_X86_64_64            000000000001f970 _ZNK3c104cuda4impl13CUDAGuardImpl14exchangeDeviceENS_6DeviceE + 0
-00000000000b5830  0000023b00000001 R_X86_64_64            000000000001f8a0 _ZNK3c104cuda4impl13CUDAGuardImpl9getDeviceEv + 0
-00000000000b5838  0000018b00000001 R_X86_64_64            000000000001e090 _ZNK3c104cuda4impl13CUDAGuardImpl9setDeviceENS_6DeviceE + 0
-00000000000b5840  0000015500000001 R_X86_64_64            0000000000020930 _ZNK3c104cuda4impl13CUDAGuardImpl18uncheckedSetDeviceENS_6DeviceE + 0
-00000000000b5848  000001f300000001 R_X86_64_64            000000000001e050 _ZNK3c104cuda4impl13CUDAGuardImpl9getStreamENS_6DeviceE + 0
-00000000000b5850  0000022900000001 R_X86_64_64            000000000001e3b0 _ZNK3c104cuda4impl13CUDAGuardImpl16getDefaultStreamENS_6DeviceE + 0
-00000000000b5858  000001ba00000001 R_X86_64_64            000000000001e380 _ZNK3c104cuda4impl13CUDAGuardImpl23getStreamFromGlobalPoolENS_6DeviceEb + 0
-00000000000b5860  0000014b00000001 R_X86_64_64            000000000001e350 _ZNK3c104cuda4impl13CUDAGuardImpl12getNewStreamENS_6DeviceEi + 0
-00000000000b5868  0000019200000001 R_X86_64_64            000000000001e2e0 _ZNK3c104cuda4impl13CUDAGuardImpl14exchangeStreamENS_6StreamE + 0
+00000000000b5830  0000023a00000001 R_X86_64_64            000000000001f8a0 _ZNK3c104cuda4impl13CUDAGuardImpl9getDeviceEv + 0
+00000000000b5838  0000018c00000001 R_X86_64_64            000000000001e090 _ZNK3c104cuda4impl13CUDAGuardImpl9setDeviceENS_6DeviceE + 0
+00000000000b5840  0000015600000001 R_X86_64_64            0000000000020930 _ZNK3c104cuda4impl13CUDAGuardImpl18uncheckedSetDeviceENS_6DeviceE + 0
+00000000000b5848  000001f100000001 R_X86_64_64            000000000001e050 _ZNK3c104cuda4impl13CUDAGuardImpl9getStreamENS_6DeviceE + 0
+00000000000b5850  0000022800000001 R_X86_64_64            000000000001e3b0 _ZNK3c104cuda4impl13CUDAGuardImpl16getDefaultStreamENS_6DeviceE + 0
+00000000000b5858  000001b900000001 R_X86_64_64            000000000001e380 _ZNK3c104cuda4impl13CUDAGuardImpl23getStreamFromGlobalPoolENS_6DeviceEb + 0
+00000000000b5860  0000014c00000001 R_X86_64_64            000000000001e350 _ZNK3c104cuda4impl13CUDAGuardImpl12getNewStreamENS_6DeviceEi + 0
+00000000000b5868  0000019300000001 R_X86_64_64            000000000001e2e0 _ZNK3c104cuda4impl13CUDAGuardImpl14exchangeStreamENS_6StreamE + 0
 00000000000b5870  0000024900000001 R_X86_64_64            0000000000020d70 _ZNK3c104cuda4impl13CUDAGuardImpl12destroyEventEPva + 0
-00000000000b5878  000001d800000001 R_X86_64_64            000000000001fc50 _ZNK3c104cuda4impl13CUDAGuardImpl6recordEPPvRKNS_6StreamEaNS_9EventFlagE + 0
-00000000000b5880  0000021500000001 R_X86_64_64            000000000001fa40 _ZNK3c104cuda4impl13CUDAGuardImpl5blockEPvRKNS_6StreamE + 0
-00000000000b5888  000001e100000001 R_X86_64_64            000000000001e490 _ZNK3c104cuda4impl13CUDAGuardImpl10queryEventEPv + 0
-00000000000b5890  0000023400000001 R_X86_64_64            000000000001e2d0 _ZNK3c104cuda4impl13CUDAGuardImpl11deviceCountEv + 0
+00000000000b5878  000001d700000001 R_X86_64_64            000000000001fc50 _ZNK3c104cuda4impl13CUDAGuardImpl6recordEPPvRKNS_6StreamEaNS_9EventFlagE + 0
+00000000000b5880  0000021400000001 R_X86_64_64            000000000001fa40 _ZNK3c104cuda4impl13CUDAGuardImpl5blockEPvRKNS_6StreamE + 0
+00000000000b5888  000001df00000001 R_X86_64_64            000000000001e490 _ZNK3c104cuda4impl13CUDAGuardImpl10queryEventEPv + 0
+00000000000b5890  0000023300000001 R_X86_64_64            000000000001e2d0 _ZNK3c104cuda4impl13CUDAGuardImpl11deviceCountEv + 0
 00000000000b5898  0000025500000001 R_X86_64_64            00000000000223b0 _ZNK3c104cuda4impl13CUDAGuardImpl11queryStreamERKNS_6StreamE + 0
-00000000000b58a0  0000018300000001 R_X86_64_64            0000000000022570 _ZNK3c104cuda4impl13CUDAGuardImpl17synchronizeStreamERKNS_6StreamE + 0
-00000000000b58a8  0000017a00000001 R_X86_64_64            000000000001e250 _ZNK3c104cuda4impl13CUDAGuardImpl16synchronizeEventEPv + 0
-00000000000b58b0  0000021e00000001 R_X86_64_64            000000000001e200 _ZNK3c104cuda4impl13CUDAGuardImpl21recordDataPtrOnStreamERKNS_7DataPtrERKNS_6StreamE + 0
-00000000000b58b8  0000016c00000001 R_X86_64_64            000000000001e0f0 _ZNK3c104cuda4impl13CUDAGuardImpl11elapsedTimeEPvS3_a + 0
-00000000000b58c0  0000015200000001 R_X86_64_64            000000000001e010 _ZN3c104cuda4impl13CUDAGuardImplD1Ev + 0
+00000000000b58a0  0000018400000001 R_X86_64_64            0000000000022570 _ZNK3c104cuda4impl13CUDAGuardImpl17synchronizeStreamERKNS_6StreamE + 0
+00000000000b58a8  0000017b00000001 R_X86_64_64            000000000001e250 _ZNK3c104cuda4impl13CUDAGuardImpl16synchronizeEventEPv + 0
+00000000000b58b0  0000021d00000001 R_X86_64_64            000000000001e200 _ZNK3c104cuda4impl13CUDAGuardImpl21recordDataPtrOnStreamERKNS_7DataPtrERKNS_6StreamE + 0
+00000000000b58b8  0000016d00000001 R_X86_64_64            000000000001e0f0 _ZNK3c104cuda4impl13CUDAGuardImpl11elapsedTimeEPvS3_a + 0
+00000000000b58c0  0000015300000001 R_X86_64_64            000000000001e010 _ZN3c104cuda4impl13CUDAGuardImplD1Ev + 0
 00000000000b58c8  0000025100000001 R_X86_64_64            000000000001e070 _ZN3c104cuda4impl13CUDAGuardImplD0Ev + 0
 00000000000b58d8  0000014700000001 R_X86_64_64            00000000000b57b8 _ZTIN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEEE + 0
-00000000000b58e0  000001ef00000001 R_X86_64_64            0000000000020030 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEED1Ev + 0
-00000000000b58e8  000001cd00000001 R_X86_64_64            0000000000020100 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEED0Ev + 0
+00000000000b58e0  000001ed00000001 R_X86_64_64            0000000000020030 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEED1Ev + 0
+00000000000b58e8  000001cc00000001 R_X86_64_64            0000000000020100 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEED0Ev + 0
 00000000000b5900  000001a800000001 R_X86_64_64            0000000000036530 _ZTSSt19bad_optional_access + 0
 00000000000b5908  0000002300000001 R_X86_64_64            0000000000000000 _ZTISt9exception@GLIBCXX_3.4 + 0
 00000000000b59b8  0000002300000001 R_X86_64_64            0000000000000000 _ZTISt9exception@GLIBCXX_3.4 + 0
 00000000000b5d30  0000002300000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt9exception@GLIBCXX_3.4 + 0
 00000000000b6a30  0000002300000001 R_X86_64_64            0000000000000000 _ZTISt9exception@GLIBCXX_3.4 + 0
-00000000000b5918  0000021800000001 R_X86_64_64            00000000000b58f8 _ZTISt19bad_optional_access + 0
-00000000000b5920  0000014e00000001 R_X86_64_64            00000000000251e0 _ZNSt19bad_optional_accessD1Ev + 0
+00000000000b5918  0000021700000001 R_X86_64_64            00000000000b58f8 _ZTISt19bad_optional_access + 0
+00000000000b5920  0000014f00000001 R_X86_64_64            00000000000251e0 _ZNSt19bad_optional_accessD1Ev + 0
 00000000000b5928  0000024e00000001 R_X86_64_64            0000000000025200 _ZNSt19bad_optional_accessD0Ev + 0
-00000000000b5930  0000016300000001 R_X86_64_64            00000000000251d0 _ZNKSt19bad_optional_access4whatEv + 0
-00000000000b5940  0000017600000001 R_X86_64_64            0000000000037720 _ZTSSt11_Mutex_baseILN9__gnu_cxx12_Lock_policyE2EE + 0
-00000000000b5950  000001e000000001 R_X86_64_64            00000000000377a0 _ZTSSt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE + 0
-00000000000b5958  000001f000000001 R_X86_64_64            00000000000b5938 _ZTISt11_Mutex_baseILN9__gnu_cxx12_Lock_policyE2EE + 0
+00000000000b5930  0000016400000001 R_X86_64_64            00000000000251d0 _ZNKSt19bad_optional_access4whatEv + 0
+00000000000b5940  0000017700000001 R_X86_64_64            0000000000037720 _ZTSSt11_Mutex_baseILN9__gnu_cxx12_Lock_policyE2EE + 0
+00000000000b5950  000001de00000001 R_X86_64_64            00000000000377a0 _ZTSSt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE + 0
+00000000000b5958  000001ee00000001 R_X86_64_64            00000000000b5938 _ZTISt11_Mutex_baseILN9__gnu_cxx12_Lock_policyE2EE + 0
 00000000000b5970  0000007f00000001 R_X86_64_64            0000000000000000 _ZTISt13runtime_error@GLIBCXX_3.4 + 0
-00000000000b5e30  0000007f00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt13runtime_error@GLIBCXX_3.4 + 0
-00000000000b59d0  0000018d00000001 R_X86_64_64            00000000000b5948 _ZTISt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE + 0
+00000000000b5e38  0000007f00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt13runtime_error@GLIBCXX_3.4 + 0
+00000000000b59d0  0000018e00000001 R_X86_64_64            00000000000b5948 _ZTISt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE + 0
 00000000000b59f8  000000be00000001 R_X86_64_64            0000000000000000 _ZNKSt13runtime_error4whatEv@GLIBCXX_3.4 + 0
 00000000000b5a28  000000be00000001 R_X86_64_64            0000000000000000 _ZNKSt13runtime_error4whatEv@GLIBCXX_3.4 + 0
 00000000000b5a00  0000007300000001 R_X86_64_64            0000000000000000 __cxa_pure_virtual@CXXABI_1.3 + 0
 00000000000b5cb8  0000000200000006 R_X86_64_GLOB_DAT      0000000000000000 PyInstanceMethod_Type + 0
-00000000000b5cc0  0000021700000006 R_X86_64_GLOB_DAT      000000000001e020 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS5_S7_dES5_NS_4guts8typelist8typelistIJS7_S7_dEEEEES8_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES7_S7_d + 0
-00000000000b5cc8  0000021200000006 R_X86_64_GLOB_DAT      000000000001e5c0 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py + 0
-00000000000b5cd0  0000013100000006 R_X86_64_GLOB_DAT      0000000000019200 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_S5_lES5_NS_4guts8typelist8typelistIJS5_S5_S5_lEEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE + 0
-00000000000b5cd8  000001a900000006 R_X86_64_GLOB_DAT      00000000000b5910 _ZTVSt19bad_optional_access + 0
-00000000000b5ce0  0000000c00000006 R_X86_64_GLOB_DAT      0000000000000000 PyByteArray_Type + 0
+00000000000b5cc0  0000021600000006 R_X86_64_GLOB_DAT      000000000001e020 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS5_S7_dES5_NS_4guts8typelist8typelistIJS7_S7_dEEEEES8_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES7_S7_d + 0
+00000000000b5cc8  0000013100000006 R_X86_64_GLOB_DAT      0000000000019200 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_S5_lES5_NS_4guts8typelist8typelistIJS5_S5_S5_lEEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE + 0
+00000000000b5cd0  000001a900000006 R_X86_64_GLOB_DAT      00000000000b5910 _ZTVSt19bad_optional_access + 0
+00000000000b5cd8  0000000c00000006 R_X86_64_GLOB_DAT      0000000000000000 PyByteArray_Type + 0
+00000000000b5ce0  0000014a00000006 R_X86_64_GLOB_DAT      000000000001e5c0 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py + 0
 00000000000b5ce8  0000025900000006 R_X86_64_GLOB_DAT      00000000000157b0 _ZN3c1018getFakeTypePtrCopyIN2at6TensorEEENS_4Type24SingletonOrSharedTypePtrIS3_EEv + 0
 00000000000b5cf0  0000001000000006 R_X86_64_GLOB_DAT      0000000000000000 _ZN3c1019UndefinedTensorImpl10_singletonE + 0
-00000000000b5cf8  000001ce00000006 R_X86_64_GLOB_DAT      0000000000022f80 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS5_S7_dES5_NS_4guts8typelist8typelistIJS7_S7_dEEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISN_EE + 0
+00000000000b5cf8  000001cd00000006 R_X86_64_GLOB_DAT      0000000000022f80 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS5_S7_dES5_NS_4guts8typelist8typelistIJS7_S7_dEEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISN_EE + 0
 00000000000b5d00  0000014100000006 R_X86_64_GLOB_DAT      000000000001b110 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_ES5_NS_4guts8typelist8typelistIJS5_S5_EEEEES6_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES5_S5_ + 0
 00000000000b5d08  0000001400000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_RuntimeError + 0
-00000000000b5d10  0000018000000006 R_X86_64_GLOB_DAT      000000000001a380 _ZN7torchao15fp16_to_fp6_cpuEN2at6TensorE + 0
+00000000000b5d10  0000018100000006 R_X86_64_GLOB_DAT      000000000001a380 _ZN7torchao15fp16_to_fp6_cpuEN2at6TensorE + 0
 00000000000b5d18  0000001e00000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_MemoryError + 0
 00000000000b5d20  0000001f00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTVN3c105ErrorE + 0
 00000000000b5d28  0000002000000006 R_X86_64_GLOB_DAT      0000000000000000 _ZNSs4_Rep20_S_empty_rep_storageE@GLIBCXX_3.4 + 0
-00000000000b5d38  0000020600000006 R_X86_64_GLOB_DAT      00000000000b6ce4 _ZZN3c104cuda13warning_stateEvE14warning_state_ + 0
+00000000000b5d38  0000020400000006 R_X86_64_GLOB_DAT      00000000000b6ce4 _ZZN3c104cuda13warning_stateEvE14warning_state_ + 0
 00000000000b5d40  0000002400000006 R_X86_64_GLOB_DAT      0000000000000000 _ZN3c104impl26device_guard_impl_registryE + 0
 00000000000b5d48  0000002900000006 R_X86_64_GLOB_DAT      0000000000000000 PyBaseObject_Type + 0
-00000000000b5d50  0000002c00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt12out_of_range@GLIBCXX_3.4 + 0
+00000000000b5d50  0000024500000006 R_X86_64_GLOB_DAT      000000000001bed0 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219310nms_kernelERKN2at6TensorES4_d + 0
+00000000000b5d58  0000002c00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt12out_of_range@GLIBCXX_3.4 + 0
 00000000000b6a08  0000002c00000001 R_X86_64_64            0000000000000000 _ZTISt12out_of_range@GLIBCXX_3.4 + 0
-00000000000b5d58  0000002e00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZN3c104impl8GPUTrace13gpuTraceStateE + 0
-00000000000b5d60  0000002f00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt12length_error@GLIBCXX_3.4 + 0
+00000000000b5d60  0000002e00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZN3c104impl8GPUTrace13gpuTraceStateE + 0
+00000000000b5d68  0000002f00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt12length_error@GLIBCXX_3.4 + 0
 00000000000b6a00  0000002f00000001 R_X86_64_64            0000000000000000 _ZTISt12length_error@GLIBCXX_3.4 + 0
-00000000000b5d68  0000003300000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTVSt19basic_ostringstreamIcSt11char_traitsIcESaIcEE@GLIBCXX_3.4 + 0
-00000000000b5d70  0000003a00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTVSt9bad_alloc@GLIBCXX_3.4 + 0
-00000000000b5d78  0000019e00000006 R_X86_64_GLOB_DAT      0000000000015b30 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EEfEvPK5uint4PK6__halfS7_PT0_mmmi + 0
-00000000000b5d80  000001b200000006 R_X86_64_GLOB_DAT      000000000001e690 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py + 0
-00000000000b5d88  000001fd00000006 R_X86_64_GLOB_DAT      00000000000b57d0 _ZTIFN2at6TensorERKS0_S2_dE + 0
+00000000000b5d70  0000003300000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTVSt19basic_ostringstreamIcSt11char_traitsIcESaIcEE@GLIBCXX_3.4 + 0
+00000000000b5d78  0000003a00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTVSt9bad_alloc@GLIBCXX_3.4 + 0
+00000000000b5d80  0000019e00000006 R_X86_64_GLOB_DAT      0000000000015b30 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EEfEvPK5uint4PK6__halfS7_PT0_mmmi + 0
+00000000000b5d88  000001fb00000006 R_X86_64_GLOB_DAT      00000000000b57d0 _ZTIFN2at6TensorERKS0_S2_dE + 0
 00000000000b5d90  000001a700000006 R_X86_64_GLOB_DAT      00000000000b5718 _ZTIFN2at6TensorES0_S0_E + 0
-00000000000b5d98  000001c400000006 R_X86_64_GLOB_DAT      0000000000015db0 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi + 0
-00000000000b5da0  000001d900000006 R_X86_64_GLOB_DAT      000000000001e4f0 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py + 0
-00000000000b5da8  000001d300000006 R_X86_64_GLOB_DAT      00000000000b5660 _ZTVN3c1015VariableVersion14VersionCounterE + 0
-00000000000b5db0  0000015f00000006 R_X86_64_GLOB_DAT      000000000001a700 _ZN7torchao25weight_matrix_dequant_cpuEN2at6TensorES1_ + 0
+00000000000b5d98  000001c300000006 R_X86_64_GLOB_DAT      0000000000015db0 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi + 0
+00000000000b5da0  000001d200000006 R_X86_64_GLOB_DAT      00000000000b5660 _ZTVN3c1015VariableVersion14VersionCounterE + 0
+00000000000b5da8  0000020d00000006 R_X86_64_GLOB_DAT      000000000001e4f0 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py + 0
+00000000000b5db0  0000016000000006 R_X86_64_GLOB_DAT      000000000001a700 _ZN7torchao25weight_matrix_dequant_cpuEN2at6TensorES1_ + 0
 00000000000b5db8  0000006100000006 R_X86_64_GLOB_DAT      0000000000000000 vsnprintf@GLIBC_2.2.5 + 0
 00000000000b5dc0  0000020e00000006 R_X86_64_GLOB_DAT      000000000001b0a0 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_ES5_NS_4guts8typelist8typelistIJS5_EEEEES6_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES5_ + 0
 00000000000b5dc8  0000013300000006 R_X86_64_GLOB_DAT      00000000000b5450 _ZTIFN2at6TensorES0_S0_S0_lE + 0
 00000000000b5dd0  0000006200000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_TypeError + 0
-00000000000b5dd8  0000016b00000006 R_X86_64_GLOB_DAT      00000000000b5488 _ZTVN3c1011SymNodeImplE + 0
-00000000000b5de8  0000022c00000006 R_X86_64_GLOB_DAT      00000000000b5728 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE + 0
-00000000000b5df0  0000022500000006 R_X86_64_GLOB_DAT      00000000000158b0 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EEfEvPK5uint4PK6__halfS7_PT0_mmmi + 0
-00000000000b5e00  000001f800000006 R_X86_64_GLOB_DAT      0000000000024910 _ZN7torchao28weight_matrix_prepacking_cpuEN2at6TensorE + 0
-00000000000b5e08  0000017b00000006 R_X86_64_GLOB_DAT      00000000000b5688 _ZTVN3c1014OperatorKernelE + 0
-00000000000b5e10  0000017400000006 R_X86_64_GLOB_DAT      0000000000015c70 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi8EEfEvPK5uint4PK6__halfS7_PT0_mmmi + 0
-00000000000b5e18  0000007400000006 R_X86_64_GLOB_DAT      0000000000000000 __pthread_key_create@GLIBC_2.2.5 + 0
-00000000000b5e20  000001c200000006 R_X86_64_GLOB_DAT      0000000000015760 _ZN3c1014getTypePtrCopyIN2at6TensorEEENS_4Type24SingletonOrSharedTypePtrIS3_EEv + 0
-00000000000b5e28  0000007d00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt16nested_exception@CXXABI_1.3.5 + 0
+00000000000b5dd8  0000016c00000006 R_X86_64_GLOB_DAT      00000000000b5488 _ZTVN3c1011SymNodeImplE + 0
+00000000000b5de8  0000022b00000006 R_X86_64_GLOB_DAT      00000000000b5728 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE + 0
+00000000000b5df0  0000020c00000006 R_X86_64_GLOB_DAT      000000000001e690 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py + 0
+00000000000b5df8  0000022400000006 R_X86_64_GLOB_DAT      00000000000158b0 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EEfEvPK5uint4PK6__halfS7_PT0_mmmi + 0
+00000000000b5e08  000001f600000006 R_X86_64_GLOB_DAT      0000000000024910 _ZN7torchao28weight_matrix_prepacking_cpuEN2at6TensorE + 0
+00000000000b5e10  0000017c00000006 R_X86_64_GLOB_DAT      00000000000b5688 _ZTVN3c1014OperatorKernelE + 0
+00000000000b5e18  0000017500000006 R_X86_64_GLOB_DAT      0000000000015c70 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi8EEfEvPK5uint4PK6__halfS7_PT0_mmmi + 0
+00000000000b5e20  0000007400000006 R_X86_64_GLOB_DAT      0000000000000000 __pthread_key_create@GLIBC_2.2.5 + 0
+00000000000b5e28  000001c100000006 R_X86_64_GLOB_DAT      0000000000015760 _ZN3c1014getTypePtrCopyIN2at6TensorEEENS_4Type24SingletonOrSharedTypePtrIS3_EEv + 0
+00000000000b5e30  0000007d00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt16nested_exception@CXXABI_1.3.5 + 0
 00000000000b6a20  0000007d00000001 R_X86_64_64            0000000000000000 _ZTISt16nested_exception@CXXABI_1.3.5 + 0
-00000000000b5e40  0000008400000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
-00000000000b5e48  0000008500000006 R_X86_64_GLOB_DAT      0000000000000000 PyCFunction_Type + 0
-00000000000b5e50  0000024000000006 R_X86_64_GLOB_DAT      0000000000015ef0 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi2EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi + 0
-00000000000b5e58  0000016100000006 R_X86_64_GLOB_DAT      0000000000015800 _ZN5torch6detail16TorchLibraryInitD1Ev + 0
-00000000000b5e60  0000009400000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTTSt19basic_ostringstreamIcSt11char_traitsIcESaIcEE@GLIBCXX_3.4 + 0
-00000000000b5e70  0000009500000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_ImportError + 0
-00000000000b5e78  0000020000000006 R_X86_64_GLOB_DAT      0000000000016030 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi + 0
-00000000000b5e80  0000020800000006 R_X86_64_GLOB_DAT      00000000000b56f0 _ZTIFN2at6TensorES0_E + 0
-00000000000b5e88  000000a200000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt14overflow_error@GLIBCXX_3.4 + 0
+00000000000b5e48  0000008400000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
+00000000000b5e50  0000008500000006 R_X86_64_GLOB_DAT      0000000000000000 PyCFunction_Type + 0
+00000000000b5e58  0000023f00000006 R_X86_64_GLOB_DAT      0000000000015ef0 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi2EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi + 0
+00000000000b5e60  0000016200000006 R_X86_64_GLOB_DAT      0000000000015800 _ZN5torch6detail16TorchLibraryInitD1Ev + 0
+00000000000b5e68  0000009400000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTTSt19basic_ostringstreamIcSt11char_traitsIcESaIcEE@GLIBCXX_3.4 + 0
+00000000000b5e78  0000009500000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_ImportError + 0
+00000000000b5e80  000001fe00000006 R_X86_64_GLOB_DAT      0000000000016030 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi + 0
+00000000000b5e88  0000020600000006 R_X86_64_GLOB_DAT      00000000000b56f0 _ZTIFN2at6TensorES0_E + 0
+00000000000b5e90  000000a200000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt14overflow_error@GLIBCXX_3.4 + 0
 00000000000b6a10  000000a200000001 R_X86_64_64            0000000000000000 _ZTISt14overflow_error@GLIBCXX_3.4 + 0
-00000000000b5e90  000000a300000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_ValueError + 0
-00000000000b5e98  000000ad00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZNSt9bad_allocD1Ev@GLIBCXX_3.4 + 0
-00000000000b5ea0  0000013900000006 R_X86_64_GLOB_DAT      00000000000159f0 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi2EEfEvPK5uint4PK6__halfS7_PT0_mmmi + 0
-00000000000b5ea8  000000b300000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_OverflowError + 0
-00000000000b5eb0  000000b400000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
-00000000000b5eb8  000000b700000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTVSt15basic_stringbufIcSt11char_traitsIcESaIcEE@GLIBCXX_3.4 + 0
-00000000000b5ec0  000000b800000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
-00000000000b5ec8  000000b900000006 R_X86_64_GLOB_DAT      0000000000000000 PyDict_Type + 0
-00000000000b5ed0  000000ba00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt12domain_error@GLIBCXX_3.4 + 0
+00000000000b5e98  000000a300000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_ValueError + 0
+00000000000b5ea0  000000ad00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZNSt9bad_allocD1Ev@GLIBCXX_3.4 + 0
+00000000000b5ea8  0000013900000006 R_X86_64_GLOB_DAT      00000000000159f0 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi2EEfEvPK5uint4PK6__halfS7_PT0_mmmi + 0
+00000000000b5eb0  000000b300000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_OverflowError + 0
+00000000000b5eb8  000000b400000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
+00000000000b5ec0  000000b700000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTVSt15basic_stringbufIcSt11char_traitsIcESaIcEE@GLIBCXX_3.4 + 0
+00000000000b5ec8  000000b800000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
+00000000000b5ed0  000000b900000006 R_X86_64_GLOB_DAT      0000000000000000 PyDict_Type + 0
+00000000000b5ed8  000000ba00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt12domain_error@GLIBCXX_3.4 + 0
 00000000000b69f8  000000ba00000001 R_X86_64_64            0000000000000000 _ZTISt12domain_error@GLIBCXX_3.4 + 0
-00000000000b5ed8  0000015c00000006 R_X86_64_GLOB_DAT      00000000000b56b0 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEEE + 0
-00000000000b5ee0  0000021c00000006 R_X86_64_GLOB_DAT      0000000000013980 _Z16SplitK_ReductionP6__halfPfmmi + 0
-00000000000b5ee8  000000cb00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZN3c104cuda20CUDACachingAllocator9allocatorE + 0
-00000000000b5ef0  0000014f00000006 R_X86_64_GLOB_DAT      00000000000b58d0 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEEE + 0
-00000000000b5ef8  000000d000000006 R_X86_64_GLOB_DAT      0000000000000000 _ZNSt16invalid_argumentD1Ev@GLIBCXX_3.4 + 0
-00000000000b5f00  000000d100000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt16invalid_argument@GLIBCXX_3.4 + 0
+00000000000b5ee0  0000015d00000006 R_X86_64_GLOB_DAT      00000000000b56b0 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEEE + 0
+00000000000b5ee8  0000021b00000006 R_X86_64_GLOB_DAT      0000000000013980 _Z16SplitK_ReductionP6__halfPfmmi + 0
+00000000000b5ef0  000000cb00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZN3c104cuda20CUDACachingAllocator9allocatorE + 0
+00000000000b5ef8  0000015000000006 R_X86_64_GLOB_DAT      00000000000b58d0 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEEE + 0
+00000000000b5f00  000000d000000006 R_X86_64_GLOB_DAT      0000000000000000 _ZNSt16invalid_argumentD1Ev@GLIBCXX_3.4 + 0
+00000000000b5f08  000000d100000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt16invalid_argument@GLIBCXX_3.4 + 0
 00000000000b6a18  000000d100000001 R_X86_64_64            0000000000000000 _ZTISt16invalid_argument@GLIBCXX_3.4 + 0
-00000000000b5f08  000000d200000006 R_X86_64_GLOB_DAT      0000000000000000 __gmon_start__ + 0
-00000000000b5f10  000000d900000006 R_X86_64_GLOB_DAT      0000000000000000 PyType_Type + 0
-00000000000b5f18  000000db00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTVN5torch8autograd12AutogradMetaE + 0
-00000000000b5f20  0000019d00000006 R_X86_64_GLOB_DAT      00000000000b5460 _ZTVN3c1020intrusive_ptr_targetE + 0
-00000000000b5f28  000000dd00000006 R_X86_64_GLOB_DAT      0000000000000000 PyProperty_Type + 0
-00000000000b5f30  000000e500000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt9bad_alloc@GLIBCXX_3.4 + 0
+00000000000b5f10  000000d200000006 R_X86_64_GLOB_DAT      0000000000000000 __gmon_start__ + 0
+00000000000b5f18  000000d900000006 R_X86_64_GLOB_DAT      0000000000000000 PyType_Type + 0
+00000000000b5f20  000000db00000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTVN5torch8autograd12AutogradMetaE + 0
+00000000000b5f28  0000019d00000006 R_X86_64_GLOB_DAT      00000000000b5460 _ZTVN3c1020intrusive_ptr_targetE + 0
+00000000000b5f30  000000dd00000006 R_X86_64_GLOB_DAT      0000000000000000 PyProperty_Type + 0
+00000000000b5f38  000000e500000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt9bad_alloc@GLIBCXX_3.4 + 0
 00000000000b6a28  000000e500000001 R_X86_64_64            0000000000000000 _ZTISt9bad_alloc@GLIBCXX_3.4 + 0
-00000000000b5f38  0000019400000006 R_X86_64_GLOB_DAT      000000000001bed0 _ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220210nms_kernelERKN2at6TensorES4_d + 0
 00000000000b5f40  000000ea00000006 R_X86_64_GLOB_DAT      0000000000000000 _Py_NoneStruct + 0
-00000000000b5f48  0000020c00000006 R_X86_64_GLOB_DAT      000000000001b4f0 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_ES5_NS_4guts8typelist8typelistIJS5_S5_EEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE + 0
+00000000000b5f48  0000020a00000006 R_X86_64_GLOB_DAT      000000000001b4f0 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_ES5_NS_4guts8typelist8typelistIJS5_S5_EEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE + 0
 00000000000b5f50  000000f400000006 R_X86_64_GLOB_DAT      0000000000000000 _ZNSt8ios_base4InitD1Ev@GLIBCXX_3.4 + 0
-00000000000b5f58  000001ec00000006 R_X86_64_GLOB_DAT      00000000000b5750 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE + 0
+00000000000b5f58  000001ea00000006 R_X86_64_GLOB_DAT      00000000000b5750 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEEE + 0
 00000000000b5f60  000000f800000006 R_X86_64_GLOB_DAT      0000000000000000 _Py_NotImplementedStruct + 0
 00000000000b5f68  000000ff00000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_SystemError + 0
 00000000000b5f70  0000010200000006 R_X86_64_GLOB_DAT      0000000000000000 PyCapsule_Type + 0
-00000000000b5f78  000001b900000006 R_X86_64_GLOB_DAT      000000000001e450 _ZN3c1018getFakeTypePtrCopyIdEENS_4Type24SingletonOrSharedTypePtrIS1_EEv + 0
+00000000000b5f78  000001b800000006 R_X86_64_GLOB_DAT      000000000001e450 _ZN3c1018getFakeTypePtrCopyIdEENS_4Type24SingletonOrSharedTypePtrIS1_EEv + 0
 00000000000b5f80  0000010700000006 R_X86_64_GLOB_DAT      0000000000000000 _ZNSt13runtime_errorD1Ev@GLIBCXX_3.4 + 0
 00000000000b5f88  0000010d00000006 R_X86_64_GLOB_DAT      0000000000000000 PyExc_IndexError + 0
-00000000000b5f90  0000023900000006 R_X86_64_GLOB_DAT      0000000000017540 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_S5_lES5_NS_4guts8typelist8typelistIJS5_S5_S5_lEEEEES6_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES5_S5_S5_l + 0
-00000000000b5f98  0000019300000006 R_X86_64_GLOB_DAT      0000000000016170 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi8EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi + 0
-00000000000b5fa0  0000023700000006 R_X86_64_GLOB_DAT      0000000000015720 _ZN3c1014getTypePtrCopyIlEENS_4Type24SingletonOrSharedTypePtrIS1_EEv + 0
+00000000000b5f90  0000023800000006 R_X86_64_GLOB_DAT      0000000000017540 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_S5_lES5_NS_4guts8typelist8typelistIJS5_S5_S5_lEEEEES6_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES5_S5_S5_l + 0
+00000000000b5f98  0000019400000006 R_X86_64_GLOB_DAT      0000000000016170 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi8EE6__halfEvPK5uint4PKS2_S7_PT0_mmmi + 0
+00000000000b5fa0  0000023600000006 R_X86_64_GLOB_DAT      0000000000015720 _ZN3c1014getTypePtrCopyIlEENS_4Type24SingletonOrSharedTypePtrIS1_EEv + 0
 00000000000b5fa8  0000011400000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTVSt15basic_streambufIcSt11char_traitsIcEE@GLIBCXX_3.4 + 0
-00000000000b5fb0  0000018400000006 R_X86_64_GLOB_DAT      0000000000015740 _ZN3c1018getFakeTypePtrCopyIlEENS_4Type24SingletonOrSharedTypePtrIS1_EEv + 0
-00000000000b5fb8  000001bb00000006 R_X86_64_GLOB_DAT      000000000001b7e0 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_ES5_NS_4guts8typelist8typelistIJS5_EEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE + 0
-00000000000b5fc0  0000022400000006 R_X86_64_GLOB_DAT      00000000000b57e0 _ZTVN3c1010ValueErrorE + 0
-00000000000b5fc8  0000023500000006 R_X86_64_GLOB_DAT      00000000000b5810 _ZTVN3c104cuda4impl13CUDAGuardImplE + 0
+00000000000b5fb0  0000018500000006 R_X86_64_GLOB_DAT      0000000000015740 _ZN3c1018getFakeTypePtrCopyIlEENS_4Type24SingletonOrSharedTypePtrIS1_EEv + 0
+00000000000b5fb8  000001ba00000006 R_X86_64_GLOB_DAT      000000000001b7e0 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_ES5_NS_4guts8typelist8typelistIJS5_EEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE + 0
+00000000000b5fc0  0000022300000006 R_X86_64_GLOB_DAT      00000000000b57e0 _ZTVN3c1010ValueErrorE + 0
+00000000000b5fc8  0000023400000006 R_X86_64_GLOB_DAT      00000000000b5810 _ZTVN3c104cuda4impl13CUDAGuardImplE + 0
 00000000000b5fd0  0000012000000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTVSt9basic_iosIcSt11char_traitsIcEE@GLIBCXX_3.4 + 0
 00000000000b5fd8  0000012300000006 R_X86_64_GLOB_DAT      0000000000000000 _ZN3c104impl8GPUTrace9haveStateE + 0
-00000000000b5fe0  0000023200000006 R_X86_64_GLOB_DAT      0000000000014910 _ZN7torchao23fp6_linear_forward_cudaEN2at6TensorES1_S1_l + 0
+00000000000b5fe0  0000023100000006 R_X86_64_GLOB_DAT      0000000000014910 _ZN7torchao23fp6_linear_forward_cudaEN2at6TensorES1_S1_l + 0
 00000000000b5fe8  0000024600000006 R_X86_64_GLOB_DAT      000000000001e3d0 _ZNK3c1010TensorImpl11size_customEl + 0
 00000000000b5ff0  0000013f00000006 R_X86_64_GLOB_DAT      000000000001e470 _ZN3c1014getTypePtrCopyIdEENS_4Type24SingletonOrSharedTypePtrIS1_EEv + 0
 00000000000b5ff8  0000013000000006 R_X86_64_GLOB_DAT      0000000000000000 _ZTISt11range_error@GLIBCXX_3.4 + 0
 00000000000b69f0  0000013000000001 R_X86_64_64            0000000000000000 _ZTISt11range_error@GLIBCXX_3.4 + 0
 00000000000b69c0  000000f100000001 R_X86_64_64            0000000000000000 __gxx_personality_v0@CXXABI_1.3 + 0
 00000000000b69d0  000000ac00000001 R_X86_64_64            0000000000000000 _ZTIN10__cxxabiv115__forced_unwindE@CXXABI_1.3.2 + 0
 
 Relocation section '.rela.plt' at offset 0xdd48 contains 309 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-00000000000b6018  000001d200000007 R_X86_64_JUMP_SLOT     000000000001ed70 _ZNK3c1010TensorImpl4sizeEl + 0
+00000000000b6018  000001d100000007 R_X86_64_JUMP_SLOT     000000000001ed70 _ZNK3c1010TensorImpl4sizeEl + 0
 00000000000b6020  0000000100000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK2at10TensorBase8data_ptrIdEEPT_v + 0
 00000000000b6028  0000000300000007 R_X86_64_JUMP_SLOT     0000000000000000 PyDict_DelItemString + 0
 00000000000b6030  0000000400000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaRegisterVar@libcudart.so.12 + 0
 00000000000b6038  0000000500000007 R_X86_64_JUMP_SLOT     0000000000000000 _Py_Dealloc + 0
 00000000000b6040  0000000600000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt9basic_iosIcSt11char_traitsIcEE5clearESt12_Ios_Iostate@GLIBCXX_3.4 + 0
 00000000000b6048  0000000700000007 R_X86_64_JUMP_SLOT     0000000000000000 PyByteArray_AsString + 0
 00000000000b6050  0000000800000007 R_X86_64_JUMP_SLOT     0000000000000000 strdup@GLIBC_2.2.5 + 0
 00000000000b6058  0000000900000007 R_X86_64_JUMP_SLOT     0000000000000000 PyModule_Create2 + 0
 00000000000b6060  0000000a00000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_begin_catch@CXXABI_1.3 + 0
-00000000000b6068  000001e700000007 R_X86_64_JUMP_SLOT     00000000000174e0 _ZN3c1013intrusive_ptrINS_10TensorImplENS_19UndefinedTensorImplEE6reset_Ev + 0
+00000000000b6068  000001e500000007 R_X86_64_JUMP_SLOT     00000000000174e0 _ZN3c1013intrusive_ptrINS_10TensorImplENS_19UndefinedTensorImplEE6reset_Ev + 0
 00000000000b6070  0000000b00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt9exceptionD2Ev@GLIBCXX_3.4 + 0
-00000000000b6078  000001b400000007 R_X86_64_JUMP_SLOT     00000000000272f0 _ZNSt6vectorIP11_typeobjectSaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_ + 0
-00000000000b6080  0000020500000007 R_X86_64_JUMP_SLOT     0000000000025c90 _ZNKSt9type_info9hash_codeEv + 0
-00000000000b6088  0000023000000007 R_X86_64_JUMP_SLOT     0000000000016f20 _ZN3c1020intrusive_ptr_targetD1Ev + 0
-00000000000b6090  000001cf00000007 R_X86_64_JUMP_SLOT     0000000000017860 _ZN3c1013intrusive_ptrINS_10TensorImplENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev + 0
+00000000000b6078  000001b300000007 R_X86_64_JUMP_SLOT     00000000000272f0 _ZNSt6vectorIP11_typeobjectSaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_ + 0
+00000000000b6080  0000020300000007 R_X86_64_JUMP_SLOT     0000000000025c90 _ZNKSt9type_info9hash_codeEv + 0
+00000000000b6088  0000022f00000007 R_X86_64_JUMP_SLOT     0000000000016f20 _ZN3c1020intrusive_ptr_targetD1Ev + 0
+00000000000b6090  000001ce00000007 R_X86_64_JUMP_SLOT     0000000000017860 _ZN3c1013intrusive_ptrINS_10TensorImplENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev + 0
 00000000000b6098  0000000d00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_SetAttrString + 0
 00000000000b60a0  0000000e00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyType_IsSubtype + 0
 00000000000b60a8  0000000f00000007 R_X86_64_JUMP_SLOT     0000000000000000 memmove@GLIBC_2.2.5 + 0
-00000000000b60b0  000001c100000007 R_X86_64_JUMP_SLOT     0000000000022760 _ZN3c106detail12_str_wrapperIJPKcRKlS3_EE4callERKS3_S5_S8_ + 0
+00000000000b60b0  000001c000000007 R_X86_64_JUMP_SLOT     0000000000022760 _ZN3c106detail12_str_wrapperIJPKcRKlS3_EE4callERKS3_S5_S8_ + 0
 00000000000b60b8  0000001100000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_Fetch + 0
 00000000000b60c0  0000001200000007 R_X86_64_JUMP_SLOT     0000000000000000 PyException_SetTraceback + 0
 00000000000b60c8  0000001300000007 R_X86_64_JUMP_SLOT     0000000000000000 __assert_fail@GLIBC_2.2.5 + 0
-00000000000b60d0  000001be00000007 R_X86_64_JUMP_SLOT     0000000000016b10 _ZN2at5emptyEN3c108ArrayRefIlEENS0_13TensorOptionsESt8optionalINS0_12MemoryFormatEE + 0
+00000000000b60d0  000001bd00000007 R_X86_64_JUMP_SLOT     0000000000016b10 _ZN2at5emptyEN3c108ArrayRefIlEENS0_13TensorOptionsESt8optionalINS0_12MemoryFormatEE + 0
 00000000000b60d8  0000001500000007 R_X86_64_JUMP_SLOT     0000000000000000 PyDict_Copy + 0
 00000000000b60e0  000001ac00000007 R_X86_64_JUMP_SLOT     0000000000026b30 _ZNSt6vectorIbSaIbEE9push_backEb + 0
 00000000000b60e8  0000001600000007 R_X86_64_JUMP_SLOT     0000000000000000 _PyThreadState_UncheckedGet + 0
-00000000000b60f0  000001b700000007 R_X86_64_JUMP_SLOT     0000000000013990 _Z17fp6_linear_kernelP11CUstream_stPK5uint4PK6__halfS6_PS4_mmmPfi + 0
+00000000000b60f0  000001b600000007 R_X86_64_JUMP_SLOT     0000000000013990 _Z17fp6_linear_kernelP11CUstream_stPK5uint4PK6__halfS6_PS4_mmmPfi + 0
 00000000000b60f8  0000001700000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK3c107SymBool10guard_boolEPKcl + 0
 00000000000b6100  0000001800000007 R_X86_64_JUMP_SLOT     0000000000000000 PyDict_Size + 0
 00000000000b6108  0000001900000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaUnregisterFatBinary@libcudart.so.12 + 0
 00000000000b6110  0000001a00000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaEventDestroy@libcudart.so.12 + 0
 00000000000b6118  0000001b00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104cuda20getCurrentCUDAStreamEa + 0
 00000000000b6120  0000001c00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK3c108SymFloat11guard_floatEPKcl + 0
 00000000000b6128  0000001d00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c106detail12infer_schema20make_function_schemaENS_8ArrayRefINS1_11ArgumentDefEEES4_ + 0
-00000000000b6130  000001fa00000007 R_X86_64_JUMP_SLOT     0000000000018470 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEEC1EPS1_ + 0
+00000000000b6130  000001f800000007 R_X86_64_JUMP_SLOT     0000000000018470 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEEC1EPS1_ + 0
 00000000000b6138  0000002100000007 R_X86_64_JUMP_SLOT     0000000000000000 PyUnicode_FromString + 0
 00000000000b6140  0000002200000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104cuda29c10_cuda_check_implementationEiPKcS2_ib + 0
 00000000000b6148  0000002500000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104cuda17getStreamFromPoolEba + 0
 00000000000b6150  0000002600000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c10ltERKNS_6SymIntEi + 0
 00000000000b6158  0000002700000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaPushCallConfiguration@libcudart.so.12 + 0
 00000000000b6160  0000002800000007 R_X86_64_JUMP_SLOT     0000000000000000 memset@GLIBC_2.2.5 + 0
 00000000000b6168  0000002a00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c106detail14torchCheckFailEPKcS2_jS2_ + 0
 00000000000b6170  0000002b00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt13runtime_errorC1EPKc + 0
-00000000000b6178  000001cb00000007 R_X86_64_JUMP_SLOT     0000000000023cc0 _Z24Padding_8_FP6_To_8_BytesPhS_ + 0
+00000000000b6178  000001ca00000007 R_X86_64_JUMP_SLOT     0000000000023cc0 _Z24Padding_8_FP6_To_8_BytesPhS_ + 0
 00000000000b6180  0000002d00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZSt17rethrow_exceptionNSt15__exception_ptr13exception_ptrE@CXXABI_1.3.3 + 0
-00000000000b6188  000001f700000007 R_X86_64_JUMP_SLOT     0000000000017400 _ZNSt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE10_M_releaseEv + 0
-00000000000b6190  0000016600000007 R_X86_64_JUMP_SLOT     0000000000026600 _ZNSt10_HashtableIP7_objectS1_SaIS1_ENSt8__detail9_IdentityESt8equal_toIS1_ESt4hashIS1_ENS3_18_Mod_range_hashingENS3_20_Default_ranged_hashENS3_20_Prime_rehash_policyENS3_17_Hashtable_traitsILb0ELb1ELb1EEEED1Ev + 0
+00000000000b6188  000001f500000007 R_X86_64_JUMP_SLOT     0000000000017400 _ZNSt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE10_M_releaseEv + 0
+00000000000b6190  0000016700000007 R_X86_64_JUMP_SLOT     0000000000026600 _ZNSt10_HashtableIP7_objectS1_SaIS1_ENSt8__detail9_IdentityESt8equal_toIS1_ESt4hashIS1_ENS3_18_Mod_range_hashingENS3_20_Default_ranged_hashENS3_20_Prime_rehash_policyENS3_17_Hashtable_traitsILb0ELb1ELb1EEEED1Ev + 0
 00000000000b6198  0000003000000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNKSs4findEcm@GLIBCXX_3.4 + 0
 00000000000b61a0  0000003100000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK3c106IValue23reportToTensorTypeErrorEv + 0
-00000000000b61a8  0000023a00000007 R_X86_64_JUMP_SLOT     0000000000013890 _Z47__device_stub__Z16SplitK_ReductionP6__halfPfmmiP6__halfPfmmi + 0
+00000000000b61a8  0000023900000007 R_X86_64_JUMP_SLOT     0000000000013890 _Z47__device_stub__Z16SplitK_ReductionP6__halfPfmmiP6__halfPfmmi + 0
 00000000000b61b0  0000003200000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs9push_backEc@GLIBCXX_3.4 + 0
-00000000000b61b8  000001b500000007 R_X86_64_JUMP_SLOT     000000000001f500 _ZN3c106detail12_str_wrapperIJPKcRKS3_EE4callES5_S5_ + 0
+00000000000b61b8  000001b400000007 R_X86_64_JUMP_SLOT     000000000001f500 _ZN3c106detail12_str_wrapperIJPKcRKS3_EE4callES5_S5_ + 0
 00000000000b61c0  0000003400000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_WriteUnraisable + 0
 00000000000b61c8  0000003500000007 R_X86_64_JUMP_SLOT     0000000000000000 PyThread_tss_create + 0
 00000000000b61d0  0000003600000007 R_X86_64_JUMP_SLOT     0000000000000000 strlen@GLIBC_2.2.5 + 0
 00000000000b61d8  0000003700000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt15__exception_ptr13exception_ptrC1ERKS0_@CXXABI_1.3.3 + 0
-00000000000b61e0  0000015800000007 R_X86_64_JUMP_SLOT     00000000000195a0 _Z13cast_fp16_fp6PtPh + 0
+00000000000b61e0  0000015900000007 R_X86_64_JUMP_SLOT     00000000000195a0 _Z13cast_fp16_fp6PtPh + 0
 00000000000b61e8  0000003900000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_HasAttrString + 0
 00000000000b61f0  0000003b00000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_guard_abort@CXXABI_1.3 + 0
 00000000000b61f8  0000003c00000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaStreamQuery@libcudart.so.12 + 0
 00000000000b6200  0000003d00000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaRegisterFatBinary@libcudart.so.12 + 0
 00000000000b6208  0000003e00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c1010TensorType3getEv + 0
 00000000000b6210  0000003f00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c106SymIntC1ENS_13intrusive_ptrINS_11SymNodeImplENS_6detail34intrusive_target_default_null_typeIS2_EEEE + 0
 00000000000b6218  0000004000000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104cuda14ExchangeDeviceEa + 0
 00000000000b6220  0000004100000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104cuda20setCurrentCUDAStreamENS0_10CUDAStreamE + 0
 00000000000b6228  0000004200000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt13runtime_errorD2Ev@GLIBCXX_3.4 + 0
-00000000000b6230  000001c900000007 R_X86_64_JUMP_SLOT     0000000000017630 _ZSt11make_uniqueIN5torch8autograd12AutogradMetaEJPN3c1010TensorImplERbEENSt9_MakeUniqIT_E15__single_objectEDpOT0_ + 0
+00000000000b6230  000001c800000007 R_X86_64_JUMP_SLOT     0000000000017630 _ZSt11make_uniqueIN5torch8autograd12AutogradMetaEJPN3c1010TensorImplERbEENSt9_MakeUniqIT_E15__single_objectEDpOT0_ + 0
 00000000000b6238  0000004400000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN2at4_ops9to_device4callERKNS_6TensorEN3c106DeviceENS5_10ScalarTypeEbbSt8optionalINS5_12MemoryFormatEE + 0
 00000000000b6240  0000004500000007 R_X86_64_JUMP_SLOT     0000000000000000 PyBytes_AsString + 0
-00000000000b6248  0000017700000007 R_X86_64_JUMP_SLOT     0000000000026730 _ZNSt13_Bvector_baseISaIbEE13_M_deallocateEv + 0
+00000000000b6248  0000017800000007 R_X86_64_JUMP_SLOT     0000000000026730 _ZNSt13_Bvector_baseISaIbEE13_M_deallocateEv + 0
 00000000000b6250  0000004600000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs12_M_leak_hardEv@GLIBCXX_3.4 + 0
 00000000000b6258  0000004700000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c106detail23torchInternalAssertFailEPKcS2_jS2_S2_ + 0
 00000000000b6260  0000004800000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSo9_M_insertImEERSoT_@GLIBCXX_3.4.9 + 0
 00000000000b6268  0000004900000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZSt11_Hash_bytesPKvmm@CXXABI_1.3.5 + 0
 00000000000b6270  0000004a00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNKSs5rfindEPKcmm@GLIBCXX_3.4 + 0
 00000000000b6278  0000004b00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNKSs17find_first_not_ofEPKcmm@GLIBCXX_3.4 + 0
 00000000000b6280  0000004c00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyByteArray_Size + 0
-00000000000b6288  000001c600000007 R_X86_64_JUMP_SLOT     00000000000201d0 _ZN2at8indexing11TensorIndexD1Ev + 0
+00000000000b6288  000001c500000007 R_X86_64_JUMP_SLOT     00000000000201d0 _ZN2at8indexing11TensorIndexD1Ev + 0
 00000000000b6290  0000004d00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZdlPv@GLIBCXX_3.4 + 0
 00000000000b6298  0000004e00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSsC1EPKcmRKSaIcE@GLIBCXX_3.4 + 0
 00000000000b62a0  0000004f00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyCapsule_GetContext + 0
 00000000000b62a8  0000005000000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK2at10TensorBase21__dispatch_contiguousEN3c1012MemoryFormatE + 0
 00000000000b62b0  0000005100000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN2at4_ops19empty_memory_format4callEN3c108ArrayRefINS2_6SymIntEEESt8optionalINS2_10ScalarTypeEES6_INS2_6LayoutEES6_INS2_6DeviceEES6_IbES6_INS2_12MemoryFormatEE + 0
 00000000000b62b8  0000005200000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs6appendEPKcm@GLIBCXX_3.4 + 0
 00000000000b62c0  0000005300000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs4swapERSs@GLIBCXX_3.4 + 0
 00000000000b62c8  0000005400000007 R_X86_64_JUMP_SLOT     0000000000000000 _PyType_Lookup + 0
 00000000000b62d0  0000005500000007 R_X86_64_JUMP_SLOT     0000000000000000 PyThreadState_Clear + 0
 00000000000b62d8  0000005600000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_Clear + 0
-00000000000b62e0  0000020d00000007 R_X86_64_JUMP_SLOT     0000000000027630 _ZNSt6vectorIbSaIbEE14_M_fill_insertESt13_Bit_iteratormb + 0
+00000000000b62e0  0000020b00000007 R_X86_64_JUMP_SLOT     0000000000027630 _ZNSt6vectorIbSaIbEE14_M_fill_insertESt13_Bit_iteratormb + 0
 00000000000b62e8  0000005700000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_throw@CXXABI_1.3 + 0
 00000000000b62f0  0000005800000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaStreamSynchronize@libcudart.so.12 + 0
 00000000000b62f8  0000005900000007 R_X86_64_JUMP_SLOT     0000000000000000 PyCapsule_New + 0
 00000000000b6300  0000005a00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyMem_Calloc + 0
-00000000000b6308  0000015e00000007 R_X86_64_JUMP_SLOT     000000000001f1a0 _ZN3c106detail12_str_wrapperIJPKcRKlEE4callERKS3_S5_ + 0
+00000000000b6308  0000015f00000007 R_X86_64_JUMP_SLOT     000000000001f1a0 _ZN3c106detail12_str_wrapperIJPKcRKlEE4callERKS3_S5_ + 0
 00000000000b6310  0000005b00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN2at4_ops11sort_stable4callERKNS_6TensorESt8optionalIbElb + 0
 00000000000b6318  0000005c00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZSt20__throw_length_errorPKc@GLIBCXX_3.4 + 0
 00000000000b6320  0000005d00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN5torch7LibraryC1ENS0_4KindESsSt8optionalIN3c1011DispatchKeyEEPKcj + 0
 00000000000b6328  0000005e00000007 R_X86_64_JUMP_SLOT     0000000000000000 _Unwind_Resume@GCC_3.0 + 0
 00000000000b6330  0000005f00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyBytes_Size + 0
 00000000000b6338  0000006000000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104cuda12device_countEv + 0
-00000000000b6340  0000020700000007 R_X86_64_JUMP_SLOT     0000000000023d80 _Z20BitInterleaving_2bitPh + 0
+00000000000b6340  0000020500000007 R_X86_64_JUMP_SLOT     0000000000023d80 _Z20BitInterleaving_2bitPh + 0
 00000000000b6348  0000006300000007 R_X86_64_JUMP_SLOT     0000000000000000 PyType_Ready + 0
 00000000000b6350  0000006400000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c105ErrorC2ENS_14SourceLocationESs + 0
 00000000000b6358  0000006500000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZSt24__throw_out_of_range_fmtPKcz + 0
 00000000000b6360  0000006600000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs6assignERKSs@GLIBCXX_3.4 + 0
 00000000000b6368  0000006700000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs6assignEPKcm@GLIBCXX_3.4 + 0
 00000000000b6370  0000006800000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c106detail23torchInternalAssertFailEPKcS2_jS2_RKSs + 0
 00000000000b6378  0000006900000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs6appendERKSs@GLIBCXX_3.4 + 0
@@ -451,15 +451,15 @@
 00000000000b6390  0000006c00000007 R_X86_64_JUMP_SLOT     0000000000000000 _PyObject_GetDictPtr + 0
 00000000000b6398  0000006d00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK2at6Tensor5indexESt16initializer_listINS_8indexing11TensorIndexEE + 0
 00000000000b63a0  0000006e00000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_atexit@GLIBC_2.2.5 + 0
 00000000000b63a8  0000006f00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK2at10TensorBase8data_ptrIlEEPT_v + 0
 00000000000b63b0  0000007000000007 R_X86_64_JUMP_SLOT     0000000000000000 PyTuple_SetItem + 0
 00000000000b63b8  0000007100000007 R_X86_64_JUMP_SLOT     0000000000000000 PyThread_tss_get + 0
 00000000000b63c0  0000007200000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_Restore + 0
-00000000000b63c8  0000018f00000007 R_X86_64_JUMP_SLOT     0000000000019740 _Z29weight_prepacking_fp16_to_fp6PtPhmm + 0
+00000000000b63c8  0000019000000007 R_X86_64_JUMP_SLOT     0000000000019740 _Z29weight_prepacking_fp16_to_fp6PtPhmm + 0
 00000000000b63d0  0000024c00000007 R_X86_64_JUMP_SLOT     0000000000018a30 _ZN5torch5emptyEN3c108ArrayRefIlEENS0_13TensorOptionsESt8optionalINS0_12MemoryFormatEE + 0
 00000000000b63d8  0000024b00000007 R_X86_64_JUMP_SLOT     0000000000016300 _ZN5torch7LibraryD1Ev + 0
 00000000000b63e0  0000007500000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt15__exception_ptr13exception_ptr4swapERS0_@CXXABI_1.3.3 + 0
 00000000000b63e8  0000007600000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNR5torch7Library5_implEPKcONS_11CppFunctionENS_17_RegisterOrVerifyE + 0
 00000000000b63f0  000001ad00000007 R_X86_64_JUMP_SLOT     0000000000026570 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EPKS3_RKS6_ + 0
 00000000000b63f8  0000007700000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSsC1ERKSaIcE@GLIBCXX_3.4 + 0
 00000000000b6400  0000007800000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104cuda9GetDeviceEPa + 0
@@ -468,15 +468,15 @@
 00000000000b6418  0000007b00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN2at4_ops12index_select4callERKNS_6TensorElS4_ + 0
 00000000000b6420  0000007c00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyThread_tss_alloc + 0
 00000000000b6428  0000007e00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN6caffe28TypeMeta26error_unsupported_typemetaES0_ + 0
 00000000000b6430  0000008000000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaGetErrorString@libcudart.so.12 + 0
 00000000000b6438  0000008100000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt13runtime_errorC1ERKSs@GLIBCXX_3.4 + 0
 00000000000b6440  0000008200000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN2at4_ops6narrow4callERKNS_6TensorElN3c106SymIntES6_ + 0
 00000000000b6448  0000014300000007 R_X86_64_JUMP_SLOT     0000000000018570 _ZN5torch8autograd13make_variableEN2at6TensorEbb + 0
-00000000000b6450  0000022800000007 R_X86_64_JUMP_SLOT     0000000000026470 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EOS6_S7_ + 0
+00000000000b6450  0000022700000007 R_X86_64_JUMP_SLOT     0000000000026470 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EOS6_S7_ + 0
 00000000000b6458  0000008300000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZSt16__ostream_insertIcSt11char_traitsIcEERSt13basic_ostreamIT_T0_ES6_PKS3_l@GLIBCXX_3.4.9 + 0
 00000000000b6460  0000008600000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSsC1ERKSsmm@GLIBCXX_3.4 + 0
 00000000000b6468  0000008700000007 R_X86_64_JUMP_SLOT     0000000000000000 PyGILState_GetThisThreadState + 0
 00000000000b6470  0000008800000007 R_X86_64_JUMP_SLOT     0000000000000000 PyBytes_AsStringAndSize + 0
 00000000000b6478  0000008900000007 R_X86_64_JUMP_SLOT     0000000000000000 memcmp@GLIBC_2.2.5 + 0
 00000000000b6480  0000019500000007 R_X86_64_JUMP_SLOT     0000000000017480 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEE6reset_Ev + 0
 00000000000b6488  0000008a00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyUnicode_AsEncodedString + 0
@@ -485,26 +485,26 @@
 00000000000b64a0  0000008d00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyTuple_New + 0
 00000000000b64a8  0000008e00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_CallFunctionObjArgs + 0
 00000000000b64b0  0000008f00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104impl23ExcludeDispatchKeyGuardC1ENS_14DispatchKeySetE + 0
 00000000000b64b8  0000009000000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK2at10TensorBase8data_ptrIhEEPT_v + 0
 00000000000b64c0  0000009100000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaEventSynchronize@libcudart.so.12 + 0
 00000000000b64c8  0000009200000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104cuda20getDefaultCUDAStreamEa + 0
 00000000000b64d0  000001ae00000007 R_X86_64_JUMP_SLOT     00000000000242a0 _Z24weight_matrix_prepackingPiS_mm + 0
-00000000000b64d8  000001b300000007 R_X86_64_JUMP_SLOT     00000000000162b0 _ZNK3c1010TensorImpl6deviceEv + 0
-00000000000b64e0  0000022300000007 R_X86_64_JUMP_SLOT     0000000000026770 _ZNSt6vectorIbSaIbEE13_M_insert_auxESt13_Bit_iteratorb + 0
+00000000000b64d8  000001b200000007 R_X86_64_JUMP_SLOT     00000000000162b0 _ZNK3c1010TensorImpl6deviceEv + 0
+00000000000b64e0  0000022200000007 R_X86_64_JUMP_SLOT     0000000000026770 _ZNSt6vectorIbSaIbEE13_M_insert_auxESt13_Bit_iteratorb + 0
 00000000000b64e8  0000009300000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c10lsERSoNS_10DeviceTypeE + 0
 00000000000b64f0  0000013a00000007 R_X86_64_JUMP_SLOT     000000000002b580 _ZNSt10_HashtableISsSt4pairIKSsPvESaIS3_ENSt8__detail10_Select1stESt8equal_toISsESt4hashISsENS5_18_Mod_range_hashingENS5_20_Default_ranged_hashENS5_20_Prime_rehash_policyENS5_17_Hashtable_traitsILb1ELb0ELb1EEEE9_M_rehashEmRKm + 0
 00000000000b64f8  0000009600000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt19basic_ostringstreamIcSt11char_traitsIcESaIcEEC1Ev + 0
 00000000000b6500  0000009700000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_Occurred + 0
 00000000000b6508  0000009800000007 R_X86_64_JUMP_SLOT     0000000000000000 PyThreadState_DeleteCurrent + 0
-00000000000b6510  0000015300000007 R_X86_64_JUMP_SLOT     00000000000172b0 _ZN3c1013intrusive_ptrINS_11SymNodeImplENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev + 0
+00000000000b6510  0000015400000007 R_X86_64_JUMP_SLOT     00000000000172b0 _ZN3c1013intrusive_ptrINS_11SymNodeImplENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev + 0
 00000000000b6518  0000009900000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK2at10TensorBase8data_ptrIiEEPT_v + 0
 00000000000b6520  0000009a00000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaEventRecord@libcudart.so.12 + 0
 00000000000b6528  0000009b00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyWeakref_NewRef + 0
-00000000000b6530  0000021d00000007 R_X86_64_JUMP_SLOT     000000000002b6b0 _ZNSt8__detail9_Map_baseISsSt4pairIKSsPvESaIS4_ENS_10_Select1stESt8equal_toISsESt4hashISsENS_18_Mod_range_hashingENS_20_Default_ranged_hashENS_20_Prime_rehash_policyENS_17_Hashtable_traitsILb1ELb0ELb1EEELb1EEixEOSs + 0
+00000000000b6530  0000021c00000007 R_X86_64_JUMP_SLOT     000000000002b6b0 _ZNSt8__detail9_Map_baseISsSt4pairIKSsPvESaIS4_ENS_10_Select1stESt8equal_toISsESt4hashISsENS_18_Mod_range_hashingENS_20_Default_ranged_hashENS_20_Prime_rehash_policyENS_17_Hashtable_traitsILb1ELb0ELb1EEELb1EEixEOSs + 0
 00000000000b6538  0000009d00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSsC1EPKcRKSaIcE@GLIBCXX_3.4 + 0
 00000000000b6540  0000009e00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs7reserveEm@GLIBCXX_3.4 + 0
 00000000000b6548  0000009f00000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaFuncSetAttribute@libcudart.so.12 + 0
 00000000000b6550  000000a000000007 R_X86_64_JUMP_SLOT     0000000000000000 PyUnicode_AsUTF8String + 0
 00000000000b6558  000000a100000007 R_X86_64_JUMP_SLOT     0000000000000000 PyEval_GetBuiltins + 0
 00000000000b6560  000000a400000007 R_X86_64_JUMP_SLOT     0000000000000000 printf@GLIBC_2.2.5 + 0
 00000000000b6568  000000a500000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs7replaceEmmPKcm@GLIBCXX_3.4 + 0
@@ -515,19 +515,19 @@
 00000000000b6590  000000aa00000007 R_X86_64_JUMP_SLOT     0000000000000000 memcpy@GLIBC_2.14 + 0
 00000000000b6598  000000ab00000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaEventCreateWithFlags@libcudart.so.12 + 0
 00000000000b65a0  000000ae00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs6appendEmc@GLIBCXX_3.4 + 0
 00000000000b65a8  000000af00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyCapsule_GetName + 0
 00000000000b65b0  000000b000000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs6appendERKSsmm@GLIBCXX_3.4 + 0
 00000000000b65b8  000000b100000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZSt17__throw_bad_allocv@GLIBCXX_3.4 + 0
 00000000000b65c0  000000b200000007 R_X86_64_JUMP_SLOT     0000000000000000 _Znwm@GLIBCXX_3.4 + 0
-00000000000b65c8  000001f500000007 R_X86_64_JUMP_SLOT     0000000000026520 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EOS6_PKS3_ + 0
+00000000000b65c8  000001f300000007 R_X86_64_JUMP_SLOT     0000000000026520 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EOS6_PKS3_ + 0
 00000000000b65d0  000000b500000007 R_X86_64_JUMP_SLOT     0000000000000000 free@GLIBC_2.2.5 + 0
 00000000000b65d8  000000b600000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt19basic_ostringstreamIcSt11char_traitsIcESaIcEED1Ev@GLIBCXX_3.4 + 0
 00000000000b65e0  000001aa00000007 R_X86_64_JUMP_SLOT     0000000000016870 _ZN3c106detail12_str_wrapperIJPKcRKiEE4callERKS3_S5_ + 0
-00000000000b65e8  0000018200000007 R_X86_64_JUMP_SLOT     0000000000016dc0 _ZN3c106detail12_str_wrapperIJPKcRKjEE4callERKS3_S5_ + 0
+00000000000b65e8  0000018300000007 R_X86_64_JUMP_SLOT     0000000000016dc0 _ZN3c106detail12_str_wrapperIJPKcRKjEE4callERKS3_S5_ + 0
 00000000000b65f0  000000bb00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyCMethod_New + 0
 00000000000b65f8  000000bc00000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaGetLastError@libcudart.so.12 + 0
 00000000000b6600  000000bd00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK3c1017SymbolicShapeMeta18init_is_contiguousEv + 0
 00000000000b6608  000000bf00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyException_SetContext + 0
 00000000000b6610  000000c000000007 R_X86_64_JUMP_SLOT     0000000000000000 PyGILState_Ensure + 0
 00000000000b6618  000000c100000007 R_X86_64_JUMP_SLOT     0000000000000000 PyEval_AcquireThread + 0
 00000000000b6620  000000c200000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_SetString + 0
@@ -546,16 +546,16 @@
 00000000000b6688  000000d300000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c1021AutogradMetaInterfaceD2Ev + 0
 00000000000b6690  000000d400000007 R_X86_64_JUMP_SLOT     0000000000000000 PyMem_Free + 0
 00000000000b6698  000000d500000007 R_X86_64_JUMP_SLOT     0000000000000000 PyThreadState_Get + 0
 00000000000b66a0  000000d600000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZSt17current_exceptionv@CXXABI_1.3.3 + 0
 00000000000b66a8  000000d700000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSo9_M_insertIlEERSoT_@GLIBCXX_3.4.9 + 0
 00000000000b66b0  000000d800000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_allocate_exception@CXXABI_1.3 + 0
 00000000000b66b8  0000013400000007 R_X86_64_JUMP_SLOT     0000000000023780 _ZN3c106detail30inferFunctionSchemaFromFunctorIPFN2at6TensorERKS3_S5_dEEESt10unique_ptrINS_14FunctionSchemaESt14default_deleteIS9_EEv + 0
-00000000000b66c0  0000015400000007 R_X86_64_JUMP_SLOT     00000000000163b0 _ZN9__gnu_cxx12__to_xstringISscEET_PFiPT0_mPKS2_P13__va_list_tagEmS5_z + 0
-00000000000b66c8  0000024400000007 R_X86_64_JUMP_SLOT     0000000000022b20 _ZN3c106detail12_str_wrapperIJRKcRKPS2_S4_S6_S4_EE4callES3_S6_S6_S6_S6_ + 0
+00000000000b66c0  0000015500000007 R_X86_64_JUMP_SLOT     00000000000163b0 _ZN9__gnu_cxx12__to_xstringISscEET_PFiPT0_mPKS2_P13__va_list_tagEmS5_z + 0
+00000000000b66c8  0000024300000007 R_X86_64_JUMP_SLOT     0000000000022b20 _ZN3c106detail12_str_wrapperIJRKcRKPS2_S4_S6_S4_EE4callES3_S6_S6_S6_S6_ + 0
 00000000000b66d0  000000da00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyThreadState_New + 0
 00000000000b66d8  000000dc00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_Repr + 0
 00000000000b66e0  000000de00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyFrame_GetLineNumber + 0
 00000000000b66e8  000000df00000007 R_X86_64_JUMP_SLOT     0000000000000000 strchr@GLIBC_2.2.5 + 0
 00000000000b66f0  000000e000000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZdlPvm + 0
 00000000000b66f8  000000e100000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_NormalizeException + 0
 00000000000b6700  000000e200000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_ClearWeakRefs + 0
@@ -564,85 +564,85 @@
 00000000000b6718  000000e600000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNKSt15basic_stringbufIcSt11char_traitsIcESaIcEE3strEv@GLIBCXX_3.4 + 0
 00000000000b6720  000000e700000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs9_M_mutateEmmm@GLIBCXX_3.4 + 0
 00000000000b6728  000000e800000007 R_X86_64_JUMP_SLOT     0000000000000000 PyCapsule_GetPointer + 0
 00000000000b6730  000000e900000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c1010TensorImpl17set_autograd_metaESt10unique_ptrINS_21AutogradMetaInterfaceESt14default_deleteIS2_EE + 0
 00000000000b6738  0000014000000007 R_X86_64_JUMP_SLOT     000000000001f090 _ZNSt15basic_stringbufIcSt11char_traitsIcESaIcEED1Ev + 0
 00000000000b6740  000000eb00000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_guard_release@CXXABI_1.3 + 0
 00000000000b6748  000000ec00000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaEventQuery@libcudart.so.12 + 0
-00000000000b6750  0000018600000007 R_X86_64_JUMP_SLOT     0000000000023ee0 _Z20BitInterleaving_4bitPh + 0
+00000000000b6750  0000018700000007 R_X86_64_JUMP_SLOT     0000000000023ee0 _Z20BitInterleaving_4bitPh + 0
 00000000000b6758  000000ed00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZStlsISt11char_traitsIcEERSt13basic_ostreamIcT_ES5_PKc@GLIBCXX_3.4 + 0
 00000000000b6760  000000ee00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c107WarningC1ESt7variantIJNS0_11UserWarningENS0_18DeprecationWarningEEERKNS_14SourceLocationESsb + 0
 00000000000b6768  000000ef00000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaRegisterFatBinaryEnd@libcudart.so.12 + 0
 00000000000b6770  000000f000000007 R_X86_64_JUMP_SLOT     0000000000000000 PyInstanceMethod_New + 0
 00000000000b6778  000000f200000007 R_X86_64_JUMP_SLOT     0000000000000000 PyDict_New + 0
 00000000000b6780  000000f300000007 R_X86_64_JUMP_SLOT     0000000000000000 PyCapsule_SetPointer + 0
-00000000000b6788  000001e500000007 R_X86_64_JUMP_SLOT     00000000000169d0 _ZN3c106IValue7destroyEv + 0
+00000000000b6788  000001e300000007 R_X86_64_JUMP_SLOT     00000000000169d0 _ZN3c106IValue7destroyEv + 0
 00000000000b6790  000000f500000007 R_X86_64_JUMP_SLOT     0000000000000000 PyGILState_Release + 0
 00000000000b6798  000000f600000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaEventElapsedTime@libcudart.so.12 + 0
 00000000000b67a0  000000f700000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSspLEPKc@GLIBCXX_3.4 + 0
 00000000000b67a8  000000f900000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt8ios_baseD2Ev@GLIBCXX_3.4 + 0
 00000000000b67b0  000000fa00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs6insertEmPKcm@GLIBCXX_3.4 + 0
-00000000000b67b8  000001f900000007 R_X86_64_JUMP_SLOT     0000000000023d40 _Z31Extract_2_Bits_From_4_PaddedFP6hhhh + 0
-00000000000b67c0  0000016500000007 R_X86_64_JUMP_SLOT     00000000000197f0 _Z25DeQuantMatrix_FP6_To_FP16P6__halfPhmmS0_ + 0
+00000000000b67b8  000001f700000007 R_X86_64_JUMP_SLOT     0000000000023d40 _Z31Extract_2_Bits_From_4_PaddedFP6hhhh + 0
+00000000000b67c0  0000016600000007 R_X86_64_JUMP_SLOT     00000000000197f0 _Z25DeQuantMatrix_FP6_To_FP16P6__halfPhmmS0_ + 0
 00000000000b67c8  000000fb00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK2at10TensorBase8data_ptrIfEEPT_v + 0
 00000000000b67d0  000000fc00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN2at4_ops10empty_like4callERKNS_6TensorESt8optionalIN3c1010ScalarTypeEES5_INS6_6LayoutEES5_INS6_6DeviceEES5_IbES5_INS6_12MemoryFormatEE + 0
 00000000000b67d8  000000fd00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSs4_Rep9_S_createEmmRKSaIcE@GLIBCXX_3.4 + 0
 00000000000b67e0  000000fe00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_SetItem + 0
-00000000000b67e8  0000018e00000007 R_X86_64_JUMP_SLOT     0000000000018d20 _ZN3c106detail30inferFunctionSchemaFromFunctorIPFN2at6TensorES3_S3_S3_lEEESt10unique_ptrINS_14FunctionSchemaESt14default_deleteIS7_EEv + 0
+00000000000b67e8  0000018f00000007 R_X86_64_JUMP_SLOT     0000000000018d20 _ZN3c106detail30inferFunctionSchemaFromFunctorIPFN2at6TensorES3_S3_S3_lEEESt10unique_ptrINS_14FunctionSchemaESt14default_deleteIS7_EEv + 0
 00000000000b67f0  0000010000000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt6localeC1Ev@GLIBCXX_3.4 + 0
 00000000000b67f8  0000021100000007 R_X86_64_JUMP_SLOT     0000000000025230 _ZNSt6vectorIhSaIhEE17_M_realloc_insertIJRKhEEEvN9__gnu_cxx17__normal_iteratorIPhS1_EEDpOT_ + 0
 00000000000b6800  0000014800000007 R_X86_64_JUMP_SLOT     0000000000023850 _ZNSt6vectorIN3c108ArgumentESaIS1_EED1Ev + 0
 00000000000b6808  0000010100000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c10neERKNS_6SymIntEi + 0
-00000000000b6810  000001c300000007 R_X86_64_JUMP_SLOT     00000000000184f0 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEEC1EPS2_ + 0
+00000000000b6810  000001c200000007 R_X86_64_JUMP_SLOT     00000000000184f0 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEEC1EPS2_ + 0
 00000000000b6818  0000010300000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_end_catch@CXXABI_1.3 + 0
 00000000000b6820  000001a300000007 R_X86_64_JUMP_SLOT     0000000000023d60 _Z31Extract_4_Bits_From_2_PaddedFP6hh + 0
 00000000000b6828  0000010400000007 R_X86_64_JUMP_SLOT     0000000000000000 strcmp@GLIBC_2.2.5 + 0
 00000000000b6830  0000010500000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104cuda9SetDeviceEa + 0
 00000000000b6838  0000010600000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_rethrow@CXXABI_1.3 + 0
 00000000000b6840  0000025300000007 R_X86_64_JUMP_SLOT     0000000000016f20 _ZN3c1020intrusive_ptr_targetD2Ev + 0
 00000000000b6848  0000024a00000007 R_X86_64_JUMP_SLOT     0000000000023fa0 _Z25Assign_32_FP6_To_4_ThreadPSt6vectorIhSaIhEES2_PhS3_S3_S3_ + 0
-00000000000b6850  0000016900000007 R_X86_64_JUMP_SLOT     0000000000026da0 _ZNSt6vectorIPcSaIS0_EE17_M_realloc_insertIJRKS0_EEEvN9__gnu_cxx17__normal_iteratorIPS0_S2_EEDpOT_ + 0
+00000000000b6850  0000016a00000007 R_X86_64_JUMP_SLOT     0000000000026da0 _ZNSt6vectorIPcSaIS0_EE17_M_realloc_insertIJRKS0_EEEvN9__gnu_cxx17__normal_iteratorIPS0_S2_EEDpOT_ + 0
 00000000000b6858  0000010800000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNKSs4findEPKcmm@GLIBCXX_3.4 + 0
-00000000000b6860  0000023d00000007 R_X86_64_JUMP_SLOT     0000000000018e00 _ZN3c104impl34call_functor_with_args_from_stack_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_S5_lES5_NS_4guts8typelist8typelistIJS5_S5_S5_lEEEEELb0EJLm0ELm1ELm2ELm3EEJS5_S5_S5_lEEENSt5decayINS8_21infer_function_traitsIT_E4type11return_typeEE4typeEPNS_14OperatorKernelENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISP_EESt16integer_sequenceImJXspT1_EEEPNSA_IJDpT2_EEE + 0
+00000000000b6860  0000023c00000007 R_X86_64_JUMP_SLOT     0000000000018e00 _ZN3c104impl34call_functor_with_args_from_stack_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_S5_lES5_NS_4guts8typelist8typelistIJS5_S5_S5_lEEEEELb0EJLm0ELm1ELm2ELm3EEJS5_S5_S5_lEEENSt5decayINS8_21infer_function_traitsIT_E4type11return_typeEE4typeEPNS_14OperatorKernelENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISP_EESt16integer_sequenceImJXspT1_EEEPNSA_IJDpT2_EEE + 0
 00000000000b6868  0000010900000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaRegisterFunction@libcudart.so.12 + 0
-00000000000b6870  0000015600000007 R_X86_64_JUMP_SLOT     00000000000178b0 _ZNSt6vectorIN3c109AliasInfoESaIS1_EED1Ev + 0
+00000000000b6870  0000015700000007 R_X86_64_JUMP_SLOT     00000000000178b0 _ZNSt6vectorIN3c109AliasInfoESaIS1_EED1Ev + 0
 00000000000b6878  000001af00000007 R_X86_64_JUMP_SLOT     0000000000025370 _ZN3c106detail30inferFunctionSchemaFromFunctorIPFN2at6TensorES3_EEESt10unique_ptrINS_14FunctionSchemaESt14default_deleteIS7_EEv + 0
 00000000000b6880  0000010a00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c107IntType3getEv + 0
 00000000000b6888  0000010b00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyFrame_GetBack + 0
 00000000000b6890  0000010c00000007 R_X86_64_JUMP_SLOT     0000000000000000 __cudaPopCallConfiguration@libcudart.so.12 + 0
 00000000000b6898  0000010f00000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_free_exception@CXXABI_1.3 + 0
-00000000000b68a0  0000015900000007 R_X86_64_JUMP_SLOT     00000000000264d0 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EPKS3_OS6_ + 0
+00000000000b68a0  0000015a00000007 R_X86_64_JUMP_SLOT     00000000000264d0 _ZStplIcSt11char_traitsIcESaIcEESbIT_T0_T1_EPKS3_OS6_ + 0
 00000000000b68a8  0000011000000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c106detail14torchCheckFailEPKcS2_jRKSs + 0
 00000000000b68b0  0000011100000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104cuda14MaybeSetDeviceEa + 0
 00000000000b68b8  0000011200000007 R_X86_64_JUMP_SLOT     0000000000000000 PyEval_SaveThread + 0
-00000000000b68c0  0000020100000007 R_X86_64_JUMP_SLOT     00000000000179e0 _ZN3c1014FunctionSchemaD1Ev + 0
-00000000000b68c8  000001d100000007 R_X86_64_JUMP_SLOT     0000000000018b50 _ZNSt6vectorIN3c106IValueESaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_ + 0
+00000000000b68c0  000001ff00000007 R_X86_64_JUMP_SLOT     00000000000179e0 _ZN3c1014FunctionSchemaD1Ev + 0
+00000000000b68c8  000001d000000007 R_X86_64_JUMP_SLOT     0000000000018b50 _ZNSt6vectorIN3c106IValueESaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_ + 0
 00000000000b68d0  0000011300000007 R_X86_64_JUMP_SLOT     0000000000000000 PyFrame_GetCode + 0
 00000000000b68d8  0000011500000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c106detail19maybe_wrap_dim_slowIlEET_S2_S2_b + 0
 00000000000b68e0  0000011600000007 R_X86_64_JUMP_SLOT     0000000000000000 PyCapsule_SetContext + 0
 00000000000b68e8  0000011700000007 R_X86_64_JUMP_SLOT     0000000000000000 cudaLaunchKernel@libcudart.so.12 + 0
-00000000000b68f0  000001d500000007 R_X86_64_JUMP_SLOT     000000000001ee50 _ZNK2at10TensorBase7optionsEv + 0
+00000000000b68f0  000001d400000007 R_X86_64_JUMP_SLOT     000000000001ee50 _ZNK2at10TensorBase7optionsEv + 0
 00000000000b68f8  0000011800000007 R_X86_64_JUMP_SLOT     0000000000000000 Py_GetVersion + 0
 00000000000b6900  0000011900000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNKSs16find_last_not_ofEPKcmm@GLIBCXX_3.4 + 0
 00000000000b6908  0000011a00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_GC_UnTrack + 0
 00000000000b6910  0000011b00000007 R_X86_64_JUMP_SLOT     0000000000000000 __dynamic_cast@CXXABI_1.3 + 0
 00000000000b6918  0000011c00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt6localeD1Ev@GLIBCXX_3.4 + 0
-00000000000b6920  0000018900000007 R_X86_64_JUMP_SLOT     0000000000021ff0 _ZN3c106detail12_str_wrapperIJPKcRKNS_10DeviceTypeES3_EE4callERKS3_S6_S9_ + 0
+00000000000b6920  0000018a00000007 R_X86_64_JUMP_SLOT     0000000000021ff0 _ZN3c106detail12_str_wrapperIJPKcRKNS_10DeviceTypeES3_EE4callERKS3_S6_S9_ + 0
 00000000000b6928  0000011d00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt8ios_baseC2Ev@GLIBCXX_3.4 + 0
 00000000000b6930  0000011e00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNSt8ios_base4InitC1Ev@GLIBCXX_3.4 + 0
 00000000000b6938  0000011f00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK3c104cuda10CUDAStream6streamEv + 0
 00000000000b6940  0000012100000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_GetAttrString + 0
 00000000000b6948  0000012200000007 R_X86_64_JUMP_SLOT     0000000000000000 PyException_SetCause + 0
 00000000000b6950  0000012400000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNKSt8__detail20_Prime_rehash_policy14_M_need_rehashEmmm@GLIBCXX_3.4.18 + 0
 00000000000b6958  0000019c00000007 R_X86_64_JUMP_SLOT     000000000001b1c0 _ZNSt6vectorIN3c106IValueESaIS1_EE8_M_eraseEN9__gnu_cxx17__normal_iteratorIPS1_S3_EES7_ + 0
 00000000000b6960  0000012500000007 R_X86_64_JUMP_SLOT     0000000000000000 PyObject_Str + 0
 00000000000b6968  0000012600000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c109FloatType3getEv + 0
 00000000000b6970  0000012700000007 R_X86_64_JUMP_SLOT     0000000000000000 PyDict_GetItemWithError + 0
 00000000000b6978  0000012800000007 R_X86_64_JUMP_SLOT     0000000000000000 PyErr_Format + 0
 00000000000b6980  0000012900000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104impl23ExcludeDispatchKeyGuardD1Ev + 0
 00000000000b6988  0000012a00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZNK3c106SymInt9guard_intEPKcl + 0
-00000000000b6990  0000015500000007 R_X86_64_JUMP_SLOT     0000000000020930 _ZNK3c104cuda4impl13CUDAGuardImpl18uncheckedSetDeviceENS_6DeviceE + 0
-00000000000b6998  0000017900000007 R_X86_64_JUMP_SLOT     0000000000018410 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev + 0
+00000000000b6990  0000015600000007 R_X86_64_JUMP_SLOT     0000000000020930 _ZNK3c104cuda4impl13CUDAGuardImpl18uncheckedSetDeviceENS_6DeviceE + 0
+00000000000b6998  0000017a00000007 R_X86_64_JUMP_SLOT     0000000000018410 _ZN3c1013intrusive_ptrINS_14OperatorKernelENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev + 0
 00000000000b69a0  0000012c00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZSt9terminatev@GLIBCXX_3.4 + 0
 00000000000b69a8  0000012d00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyUnicode_AsUTF8AndSize + 0
 00000000000b69b0  0000012e00000007 R_X86_64_JUMP_SLOT     0000000000000000 PyTuple_Size + 0
 00000000000b69b8  0000012f00000007 R_X86_64_JUMP_SLOT     0000000000000000 _ZN3c104cuda21warn_or_error_on_syncEv + 0
```

### readelf --wide --dynamic {}

```diff
@@ -9,15 +9,15 @@
  0x0000000000000001 (NEEDED)             Shared library: [libc10_cuda.so]
  0x0000000000000001 (NEEDED)             Shared library: [libtorch_cuda.so]
  0x0000000000000001 (NEEDED)             Shared library: [libstdc++.so.6]
  0x0000000000000001 (NEEDED)             Shared library: [libm.so.6]
  0x0000000000000001 (NEEDED)             Shared library: [libgcc_s.so.1]
  0x0000000000000001 (NEEDED)             Shared library: [libpthread.so.0]
  0x0000000000000001 (NEEDED)             Shared library: [libc.so.6]
- 0x000000000000000f (RPATH)              Library rpath: [/__w/_temp/conda_environment_9144442527/lib]
+ 0x000000000000000f (RPATH)              Library rpath: [/__w/_temp/conda_environment_9183319250/lib]
  0x000000000000000c (INIT)               0x10000
  0x000000000000000d (FINI)               0x32c5c
  0x0000000000000019 (INIT_ARRAY)         0xb5318
  0x000000000000001b (INIT_ARRAYSZ)       88 (bytes)
  0x000000000000001a (FINI_ARRAY)         0xb5370
  0x000000000000001c (FINI_ARRAYSZ)       8 (bytes)
  0x000000006ffffef5 (GNU_HASH)           0x260
```

### readelf --wide --notes {}

```diff
@@ -1,4 +1,4 @@
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 3b4ca28c83b01547369f670de876b82322299b92
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 2da96c753672aa67267b76231c60524e187755e5
```

### strings --all --bytes=8 {}

```diff
@@ -306,17 +306,17 @@
 _ZN3c104cuda20getDefaultCUDAStreamEa
 _ZNK3c1010TensorImpl11size_customEl
 _ZN3c1018getFakeTypePtrCopyIdEENS_4Type24SingletonOrSharedTypePtrIS1_EEv
 _ZN3c109FloatType3getEv
 _ZN3c1014getTypePtrCopyIdEENS_4Type24SingletonOrSharedTypePtrIS1_EEv
 _ZNK3c104cuda4impl13CUDAGuardImpl10queryEventEPv
 cudaEventQuery
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py
 _ZN3c1010ValueErrorD2Ev
 _ZTVN3c105ErrorE
 _ZNSt9exceptionD2Ev
 _ZN3c1010ValueErrorD1Ev
 _ZN3c1010ValueErrorD0Ev
 _ZN3c1014DispatchKeySetC2ENS_11DispatchKeyE
 _ZN3c1014DispatchKeySetC1ENS_11DispatchKeyE
@@ -361,15 +361,15 @@
 cudaStreamQuery
 _ZNK3c104cuda4impl13CUDAGuardImpl17synchronizeStreamERKNS_6StreamE
 _ZZN3c104cuda13warning_stateEvE14warning_state_
 cudaStreamSynchronize
 _ZN3c104cuda21warn_or_error_on_syncEv
 _ZN3c106detail12_str_wrapperIJPKcRKlS3_EE4callERKS3_S5_S8_
 _ZN3c106detail12_str_wrapperIJRKcRKPS2_S4_S6_S4_EE4callES3_S6_S6_S6_S6_
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220210nms_kernelERKN2at6TensorES4_d
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219310nms_kernelERKN2at6TensorES4_d
 _ZTVN3c104cuda4impl13CUDAGuardImplE
 _ZN2at4_ops11sort_stable4callERKNS_6TensorESt8optionalIbElb
 _ZN2at4_ops12index_select4callERKNS_6TensorElS4_
 _ZNK2at10TensorBase21__dispatch_contiguousEN3c1012MemoryFormatE
 _ZN2at4_ops15to_dtype_layout4callERKNS_6TensorESt8optionalIN3c1010ScalarTypeEES5_INS6_6LayoutEES5_INS6_6DeviceEES5_IbEbbS5_INS6_12MemoryFormatEE
 _ZNK2at10TensorBase8data_ptrIlEEPT_v
 _ZN2at4_ops6narrow4callERKNS_6TensorElN3c106SymIntES6_
@@ -602,15 +602,15 @@
 GLIBCXX_3.4.18
 CXXABI_1.3.2
 CXXABI_1.3.5
 GLIBCXX_3.4.9
 CXXABI_1.3.3
 CXXABI_1.3
 GLIBCXX_3.4
-/__w/_temp/conda_environment_9144442527/lib
+/__w/_temp/conda_environment_9183319250/lib
 AVAUATUSH
 []A\A]A^A_
 AVAUATUSH
 []A\A]A^A_
 []A\A]A^A_
 []A\A]A^A_
 AWAVAUATUSH
@@ -727,15 +727,15 @@
 ([]A\A]A^A_
 ([]A\A]A^A_
 AWAVAUATI
 []A\A]A^A_
 D$ H9D$Xu
 AWAVAUATUSH
 []A\A]A^A_
-/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/core/SymNodeImpl.h
+/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/core/SymNodeImpl.h
 has_hint
 guard_float
 guard_bool
 guard_int
 wrap_bool
 wrap_float
 wrap_int
@@ -746,15 +746,15 @@
 is_channels_last_contiguous_3d
 is_channels_last_contiguous_2d
 is_contiguous
 floordiv
 is_float
 tensor does not have a device
 device_default
-/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/core/TensorImpl.h
+/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/core/TensorImpl.h
 cudaError_t fp6_linear_kernel(cudaStream_t, const uint4*, const half*, const half*, half*, size_t, size_t, size_t, float*, int)
 /__w/ao/ao/pytorch/ao/torchao/csrc/cuda/fp6_llm/fp6_linear.cu
 FP6LLM_API Error: Unsupported N dimension %d!
 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi8EEfEvPK5uint4PK6__halfS7_PT0_mmmi
 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EEfEvPK5uint4PK6__halfS7_PT0_mmmi
 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi2EEfEvPK5uint4PK6__halfS7_PT0_mmmi
 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EEfEvPK5uint4PK6__halfS7_PT0_mmmi
@@ -778,60 +778,60 @@
 PyObject
 Uninitialized
 Quantizer
 Generator
 InvalidTag(
 unexpected tag 
 isIntrusivePtr
-static_cast<uint32_t>(tag) < kNumTags INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":1315, please report a bug to PyTorch. 
-/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h
+static_cast<uint32_t>(tag) < kNumTags INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":1315, please report a bug to PyTorch. 
+/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h
 TTarget violates the invariant that refcount > 0  =>  weakcount > 0
-owning_ptr == NullType::singleton() || owning_ptr->refcount_.load() == 0 || owning_ptr->weakcount_.load() INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/util/intrusive_ptr.h":483, please report a bug to PyTorch. 
-/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/util/intrusive_ptr.h
+owning_ptr == NullType::singleton() || owning_ptr->refcount_.load() == 0 || owning_ptr->weakcount_.load() INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/util/intrusive_ptr.h":483, please report a bug to PyTorch. 
+/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/util/intrusive_ptr.h
 Operators taking TensorOptions cannot take a TensorOptions with options.requires_grad set as true. This isn't implemented yet.
-/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/ATen/core/CheckMemoryFormat.h
+/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/ATen/core/CheckMemoryFormat.h
 check_tensor_options_and_extract_memory_format
 Cannot set memory_format both in TensorOptions and explicit argument; please delete the redundant setter.
 IntArrayRef contains an int that cannot be represented as a SymInt: 
-/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/core/SymIntArrayRef.h
+/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/core/SymIntArrayRef.h
 created ArrayRef with nullptr and non-zero length! std::optional relies on this being illegal
-Data != nullptr || Length == 0 INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/util/ArrayRef.h":62, please report a bug to PyTorch. 
-/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/util/ArrayRef.h
+Data != nullptr || Length == 0 INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/util/ArrayRef.h":62, please report a bug to PyTorch. 
+/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/util/ArrayRef.h
 fromIntArrayRefSlow
 debugCheckNullptrInvariant
 Tried to destruct an intrusive_ptr_target that still has intrusive_ptr to it; refcount was 
-refcount_.load() == 0 || refcount_.load() >= detail::kImpracticallyHugeReferenceCount INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/util/intrusive_ptr.h":118, please report a bug to PyTorch. 
+refcount_.load() == 0 || refcount_.load() >= detail::kImpracticallyHugeReferenceCount INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/util/intrusive_ptr.h":118, please report a bug to PyTorch. 
 Tried to destruct an intrusive_ptr_target that still has weak_intrusive_ptr to it
-weakcount_.load() == 1 || weakcount_.load() == 0 || weakcount_.load() == detail::kImpracticallyHugeReferenceCount - 1 || weakcount_.load() == detail::kImpracticallyHugeReferenceCount INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/util/intrusive_ptr.h":133, please report a bug to PyTorch. 
+weakcount_.load() == 1 || weakcount_.load() == 0 || weakcount_.load() == detail::kImpracticallyHugeReferenceCount - 1 || weakcount_.load() == detail::kImpracticallyHugeReferenceCount INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/util/intrusive_ptr.h":133, please report a bug to PyTorch. 
 ~intrusive_ptr_target
-self_impl INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/variable.h":305, please report a bug to PyTorch. 
-/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/variable.h
+self_impl INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/variable.h":305, please report a bug to PyTorch. 
+/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/variable.h
 Only Tensors of floating point and complex dtype can require gradients
 AutogradMeta
 set_requires_grad
 intrusive_ptr: Newly-created target had non-zero refcounts. Does its constructor do something strange like incref or create an intrusive_ptr from `this`?
-target_->refcount_ == 0 && target_->weakcount_ == 0 INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/util/intrusive_ptr.h":319, please report a bug to PyTorch. 
+target_->refcount_ == 0 && target_->weakcount_ == 0 INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/util/intrusive_ptr.h":319, please report a bug to PyTorch. 
 intrusive_ptr
 TensorImpl with nullptr is not supported
 intrusive_ptr: Cannot increase refcount after it reached zero.
-new_refcount != 1 INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/util/intrusive_ptr.h":274, please report a bug to PyTorch. 
+new_refcount != 1 INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/util/intrusive_ptr.h":274, please report a bug to PyTorch. 
 vector::_M_realloc_insert
 expected int
-0 INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":652, please report a bug to PyTorch. 
+0 INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":652, please report a bug to PyTorch. 
 N3c1020intrusive_ptr_targetE
 N3c1011SymNodeImplE
 N3c1015VariableVersion14VersionCounterE
 N3c1014OperatorKernelE
 N3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEEE
 FN2at6TensorES0_S0_S0_lE
 Input value out of range for FP6.
 void DeQuantMatrix_FP6_To_FP16(half*, unsigned char*, size_t, size_t, half*)
 /__w/ao/ao/pytorch/ao/torchao/csrc/cuda/fp6_llm/weight_quant.cu
 _ZN46_INTERNAL_4c03c64a_15_weight_quant_cu_f5655ced6thrust6system6detail10sequential3seqE
-extra_meta_ && extra_meta_->symbolic_shape_meta_ INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/core/TensorImpl.h":1723, please report a bug to PyTorch. 
+extra_meta_ && extra_meta_->symbolic_shape_meta_ INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/core/TensorImpl.h":1723, please report a bug to PyTorch. 
 Expected fp6_tensor.size(1) % 3 == 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected fp16_scale.size(0) == OC to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 (K * 6 % 8) should be 0
 weight must be 2-dimensional
 fp16_to_fp6_cpu
 weight must be FP16
 symbolic_shape_meta
@@ -861,63 +861,63 @@
 scores must be a CUDA tensor
 dimension 0, got 
 CUDAGuardImpl
 " not implemented for '
 operator()
 slice step cannot be zero
 torchao::nms
-d.is_cuda() INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/cuda/impl/CUDAGuardImpl.h":53, please report a bug to PyTorch. 
-/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/cuda/impl/CUDAGuardImpl.h
+d.is_cuda() INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/cuda/impl/CUDAGuardImpl.h":53, please report a bug to PyTorch. 
+/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/cuda/impl/CUDAGuardImpl.h
 setDevice
 Both events must be recorded before calculating elapsed time.
 elapsedTime
 Expected stream_.device_type() == DeviceType::CUDA to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
-/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/cuda/CUDAStream.h
+/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/cuda/CUDAStream.h
 CUDAStream
 synchronizeEvent
 queryEvent
 There is an error in the layout calculation logic.
-is_mkldnn() INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/core/TensorImpl.h":1290, please report a bug to PyTorch. 
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py
-_ZN41_INTERNAL_5b2e9259_6_nms_cu_a1cad1bf_22026thrust6system6detail10sequential3seqE
-is_heap_allocated() INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/core/SymInt.h":89, please report a bug to PyTorch. 
-/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/core/SymInt.h
+is_mkldnn() INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/core/TensorImpl.h":1290, please report a bug to PyTorch. 
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py
+_ZN41_INTERNAL_5b2e9259_6_nms_cu_43d10e94_21936thrust6system6detail10sequential3seqE
+is_heap_allocated() INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/core/SymInt.h":89, please report a bug to PyTorch. 
+/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/core/SymInt.h
 /__w/ao/ao/pytorch/ao/torchao/csrc/cuda/nms.cu
 boxes should be a 2d tensor, got 
 boxes should have 4 elements in dimension 1, got 
 scores should be a 1d tensor, got 
 boxes and scores should have same number of elements in 
-t == DeviceType::CUDA INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/cuda/impl/CUDAGuardImpl.h":28, please report a bug to PyTorch. 
+t == DeviceType::CUDA INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/cuda/impl/CUDAGuardImpl.h":28, please report a bug to PyTorch. 
 cannot create std::vector larger than max_size()
-/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/ATen/TensorIndexing.h
+/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/ATen/TensorIndexing.h
 getDevice
 validate
 Device index must be -1 or non-negative, got 
-index_ >= -1 INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/core/Device.h":177, please report a bug to PyTorch. 
-/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/core/Device.h
-d.is_cuda() INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/cuda/impl/CUDAGuardImpl.h":34, please report a bug to PyTorch. 
+index_ >= -1 INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/core/Device.h":177, please report a bug to PyTorch. 
+/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/core/Device.h
+d.is_cuda() INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/cuda/impl/CUDAGuardImpl.h":34, please report a bug to PyTorch. 
 exchangeDevice
 Event device index 
 createEvent
  does not match recording stream's device index 
 CUDA event received unknown flag
 CUDA warning: 
 uncheckedSetDevice
 destroyEvent
  devices
 getDeviceGuardImpl
 PyTorch is not linked with support for 
-/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/core/impl/DeviceGuardImplInterface.h
+/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/core/impl/DeviceGuardImplInterface.h
 stream_synchronize
-/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/cuda/CUDAFunctions.h
+/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/cuda/CUDAFunctions.h
 Expected ptr_->is_float() to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
-/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/c10/core/SymFloat.h
-0 INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9144442527/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":540, please report a bug to PyTorch. 
+/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/c10/core/SymFloat.h
+0 INTERNAL ASSERT FAILED at "/__w/_temp/conda_environment_9183319250/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":540, please report a bug to PyTorch. 
 expected double
 toDouble
 N3c1010ValueErrorE
 N3c104impl24DeviceGuardImplInterfaceE
 N3c104cuda4impl13CUDAGuardImplE
 N3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS4_S6_dES4_NS_4guts8typelist8typelistIJS6_S6_dEEEEE
 FN2at6TensorERKS0_S2_dE
@@ -1402,113 +1402,113 @@
 .nv.global
 _ZN46_INTERNAL_4c03c64a_15_weight_quant_cu_f5655ced6thrust6system6detail10sequential3seqE
 .debug_frame
 .shstrtab
 .symtab_shndx
 .nv.uft.entry
 .nv.info
-.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py
-.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py
-.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py
 .nv.global
-.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py
-.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py
-.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py
-.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py
-.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py
-.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py
-.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py
-.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py
-.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py
+.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py
+.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py
+.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py
+.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py
+.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py
+.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py
+.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py
+.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py
 .debug_frame
 .rel.debug_frame
 .rela.debug_frame
 .shstrtab
 .symtab_shndx
 .nv.uft.entry
 .nv.info
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py
-.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py
-.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py
-.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py
 .nv.global
-_ZN41_INTERNAL_5b2e9259_6_nms_cu_a1cad1bf_22026thrust6system6detail10sequential3seqE
-$_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py$__cuda_sm3x_div_rn_noftz_f32_slowpath
-$___ZZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_PyE11block_boxes__537
-.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py
-.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py
-.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py
-.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py
-$_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py$__cuda_sm3x_div_rn_noftz_f32_slowpath
-$___ZZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_PyE11block_boxes__284
-.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py
-.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py
-.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py
-.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py
-$_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py$__cuda_sm20_div_f64_slowpath_v2
-$___ZZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_PyE11block_boxes__31
-.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py
+_ZN41_INTERNAL_5b2e9259_6_nms_cu_43d10e94_21936thrust6system6detail10sequential3seqE
+$_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py$__cuda_sm3x_div_rn_noftz_f32_slowpath
+$___ZZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_PyE11block_boxes__537
+.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py
+.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py
+.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py
+.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py
+$_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py$__cuda_sm3x_div_rn_noftz_f32_slowpath
+$___ZZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_PyE11block_boxes__284
+.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py
+.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py
+.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py
+.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py
+$_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py$__cuda_sm20_div_f64_slowpath_v2
+$___ZZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_PyE11block_boxes__31
+.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py
 .debug_frame
 .rel.debug_frame
 .rela.debug_frame
 .shstrtab
 .symtab_shndx
 .nv.uft.entry
 .nv.info
-.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py
-.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py
-.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py
 .nv.global
-.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py
-.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py
-.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py
-.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py
-.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py
-.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py
-.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py
-.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py
-.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py
+.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py
+.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py
+.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py
+.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py
+.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py
+.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py
+.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py
+.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py
 .debug_frame
 .rel.debug_frame
 .rela.debug_frame
 .shstrtab
 .symtab_shndx
 .nv.uft.entry
 .nv.info
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py
-.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py
-.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py
-.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py
+.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py
 .nv.global
-_ZN41_INTERNAL_5b2e9259_6_nms_cu_a1cad1bf_22026thrust6system6detail10sequential3seqE
-$_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py$__cuda_sm3x_div_rn_noftz_f32_slowpath
-$___ZZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_PyE11block_boxes__537
-.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py
-.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py
-.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py
-.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py
-$_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py$__cuda_sm3x_div_rn_noftz_f32_slowpath
-$___ZZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_PyE11block_boxes__284
-.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py
-.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py
-.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py
-.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py
-$_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py$__cuda_sm20_div_f64_slowpath_v2
-$___ZZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_PyE11block_boxes__31
-.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py
+_ZN41_INTERNAL_5b2e9259_6_nms_cu_43d10e94_21936thrust6system6detail10sequential3seqE
+$_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py$__cuda_sm3x_div_rn_noftz_f32_slowpath
+$___ZZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_PyE11block_boxes__537
+.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py
+.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py
+.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py
+.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py
+$_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py$__cuda_sm3x_div_rn_noftz_f32_slowpath
+$___ZZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_PyE11block_boxes__284
+.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py
+.text._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py
+.nv.info._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py
+.nv.shared._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py
+$_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py$__cuda_sm20_div_f64_slowpath_v2
+$___ZZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_PyE11block_boxes__31
+.nv.constant0._ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py
 .debug_frame
 .rel.debug_frame
 .rela.debug_frame
 GCC: (GNU) 9.3.1 20200408 (Red Hat 9.3.1-2)
 GCC: (GNU) 4.8.5 20150623 (Red Hat 4.8.5-44)
-tmpxft_00000877_00000000-6_fp6_linear.compute_86.cudafe1.cpp
+tmpxft_0000086e_00000000-6_fp6_linear.compute_86.cudafe1.cpp
 fatbinData
 _Z9Kernel_ExI12TilingConfigILi4ELi1ELi8EEfEvP11CUstream_stPK5uint4PK6__halfS9_PT0_mmmi
 _ZGVZ9Kernel_ExI12TilingConfigILi4ELi1ELi8EEfEvP11CUstream_stPK5uint4PK6__halfS9_PT0_mmmiE8SHMEM_SZ
 _ZZ9Kernel_ExI12TilingConfigILi4ELi1ELi8EEfEvP11CUstream_stPK5uint4PK6__halfS9_PT0_mmmiE8SHMEM_SZ
 _ZL26__cudaUnregisterBinaryUtilv
 _ZL20__cudaFatCubinHandle
 _Z9Kernel_ExI12TilingConfigILi4ELi1ELi8EE6__halfEvP11CUstream_stPK5uint4PKS2_S9_PT0_mmmi.constprop.0
@@ -1528,32 +1528,32 @@
 _ZGVZ9Kernel_ExI12TilingConfigILi4ELi1ELi1EE6__halfEvP11CUstream_stPK5uint4PKS2_S9_PT0_mmmiE8SHMEM_SZ
 _ZZ9Kernel_ExI12TilingConfigILi4ELi1ELi1EE6__halfEvP11CUstream_stPK5uint4PKS2_S9_PT0_mmmiE8SHMEM_SZ
 _ZL24__sti____cudaRegisterAllv
 _ZL15__fatDeviceText
 _ZN6thrust6system6detail10sequentialL3seqE
 _ZN3c10L45autograd_dispatch_keyset_with_ADInplaceOrViewE
 _ZN7torchao23fp6_linear_forward_cudaEN2at6TensorES1_S1_l.cold
-_GLOBAL__sub_I_tmpxft_00000877_00000000_6_fp6_linear.compute_86.cudafe1.cpp
+_GLOBAL__sub_I_tmpxft_0000086e_00000000_6_fp6_linear.compute_86.cudafe1.cpp
 _ZStL8__ioinit
 _ZN7torchaoL45TORCH_LIBRARY_IMPL_static_init_torchao_CUDA_2E
-_GLOBAL__sub_I_tmpxft_00000877_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold
-tmpxft_00000878_00000000-6_weight_quant.compute_86.cudafe1.cpp
+_GLOBAL__sub_I_tmpxft_0000086e_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold
+tmpxft_0000086f_00000000-6_weight_quant.compute_86.cudafe1.cpp
 _Z13cast_fp16_fp6PtPh.cold
 _Z29weight_prepacking_fp16_to_fp6PtPhmm.cold
 _ZN7torchao15fp16_to_fp6_cpuEN2at6TensorE.cold
 _ZN7torchao25weight_matrix_dequant_cpuEN2at6TensorES1_.cold
-_GLOBAL__sub_I_tmpxft_00000878_00000000_6_weight_quant.compute_86.cudafe1.cpp
+_GLOBAL__sub_I_tmpxft_0000086f_00000000_6_weight_quant.compute_86.cudafe1.cpp
 _ZN7torchaoL44TORCH_LIBRARY_IMPL_static_init_torchao_CPU_2E
-_GLOBAL__sub_I_tmpxft_00000878_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold
-tmpxft_00000879_00000000-6_nms.compute_86.cudafe1.cpp
+_GLOBAL__sub_I_tmpxft_0000086f_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold
+tmpxft_00000870_00000000-6_nms.compute_86.cudafe1.cpp
 _ZN3c10L8toStringENS_10ScalarTypeE
 _ZN3c106SymInt8release_Ev.part.0
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220210nms_kernelERKN2at6TensorES4_d.cold
-_GLOBAL__sub_I_tmpxft_00000879_00000000_6_nms.compute_86.cudafe1.cpp
-_GLOBAL__sub_I_tmpxft_00000879_00000000_6_nms.compute_86.cudafe1.cpp.cold
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219310nms_kernelERKN2at6TensorES4_d.cold
+_GLOBAL__sub_I_tmpxft_00000870_00000000_6_nms.compute_86.cudafe1.cpp
+_GLOBAL__sub_I_tmpxft_00000870_00000000_6_nms.compute_86.cudafe1.cpp.cold
 _GLOBAL__sub_I_fp6_llm.cpp
 _ZL44TORCH_LIBRARY_FRAGMENT_static_init_torchao_2
 _GLOBAL__sub_I_fp6_llm.cpp.cold
 _Z24weight_matrix_prepackingPiS_mm.cold
 _ZN7torchao28weight_matrix_prepacking_cpuEN2at6TensorE.cold
 _GLOBAL__sub_I_weight_prepacking.cpp
 _GLOBAL__sub_I_weight_prepacking.cpp.cold
@@ -1713,15 +1713,14 @@
 _ZTSFN2at6TensorES0_S0_S0_lE
 PyDict_DelItemString
 __cudaRegisterVar@libcudart.so.12
 _Py_Dealloc
 _ZNSt9basic_iosIcSt11char_traitsIcEE5clearESt12_Ios_Iostate@GLIBCXX_3.4
 PyByteArray_AsString
 _ZN3c104impl28wrap_kernel_functor_unboxed_INS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorERKS5_S7_dES5_NS_4guts8typelist8typelistIJS7_S7_dEEEEES8_E4callEPNS_14OperatorKernelENS_14DispatchKeySetES7_S7_d
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIN3c104HalfEEEvidPKT_Py
 strdup@GLIBC_2.2.5
 _ZNK3c104cuda4impl13CUDAGuardImpl11deviceCountEv
 _ZN3c1011SymNodeImpl11is_symbolicEv
 _ZN3c104impl31make_boxed_from_unboxed_functorINS0_6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES5_S5_S5_lES5_NS_4guts8typelist8typelistIJS5_S5_S5_lEEEEELb0EE4callEPNS_14OperatorKernelERKNS_14OperatorHandleENS_14DispatchKeySetEPSt6vectorINS_6IValueESaISL_EE
 _ZTVSt19bad_optional_access
 PyModule_Create2
 __cxa_begin_catch@CXXABI_1.3
@@ -1734,14 +1733,15 @@
 _ZN3c1011SymNodeImpl7sym_andERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
 _ZNSt9exceptionD2Ev@GLIBCXX_3.4
 _ZNSt6vectorIP11_typeobjectSaIS1_EE17_M_realloc_insertIJS1_EEEvN9__gnu_cxx17__normal_iteratorIPS1_S3_EEDpOT_
 PyByteArray_Type
 _ZN3c1011SymNodeImpl3modERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
 _ZNK3c106IValue7tagKindEv
 _ZNK3c104impl16VirtualGuardImpl9getStreamENS_6DeviceE
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIN3c104HalfEEEvidPKT_Py
 _ZNKSt9type_info9hash_codeEv
 _ZN3c1020intrusive_ptr_targetD1Ev
 _ZN3c1013intrusive_ptrINS_10TensorImplENS_6detail34intrusive_target_default_null_typeIS1_EEE6reset_Ev
 PyObject_SetAttrString
 _ZNK3c104impl16VirtualGuardImpl12destroyEventEPva
 PyType_IsSubtype
 memmove@GLIBC_2.2.5
@@ -1789,14 +1789,15 @@
 __cudaPushCallConfiguration@libcudart.so.12
 _ZN3c1011SymNodeImpl30is_channels_last_contiguous_3dENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEED2Ev
 memset@GLIBC_2.2.5
 PyBaseObject_Type
 _ZN3c106detail14torchCheckFailEPKcS2_jS2_
 _ZNSt13runtime_errorC1EPKc
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219310nms_kernelERKN2at6TensorES4_d
 _ZTISt12out_of_range@GLIBCXX_3.4
 _Z24Padding_8_FP6_To_8_BytesPhS_
 _ZSt17rethrow_exceptionNSt15__exception_ptr13exception_ptrE@CXXABI_1.3.3
 _ZN3c104impl8GPUTrace13gpuTraceStateE
 _ZNSt16_Sp_counted_baseILN9__gnu_cxx12_Lock_policyE2EE10_M_releaseEv
 _ZN3c1011SymNodeImpl10guard_boolEPKcl
 _ZNSt10_HashtableIP7_objectS1_SaIS1_ENSt8__detail9_IdentityESt8equal_toIS1_ESt4hashIS1_ENS3_18_Mod_range_hashingENS3_20_Default_ranged_hashENS3_20_Prime_rehash_policyENS3_17_Hashtable_traitsILb0ELb1ELb1EEEED1Ev
@@ -1815,15 +1816,14 @@
 _Z13cast_fp16_fp6PtPh
 _ZTSN3c1014OperatorKernelE
 _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3
 PyObject_HasAttrString
 _ZTVSt9bad_alloc@GLIBCXX_3.4
 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi4EEfEvPK5uint4PK6__halfS7_PT0_mmmi
 __cxa_guard_abort@CXXABI_1.3
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIdEEvidPKT_Py
 cudaStreamQuery@libcudart.so.12
 __cudaRegisterFatBinary@libcudart.so.12
 _ZN3c1010TensorType3getEv
 _ZNK3c104impl16VirtualGuardImpl5blockEPvRKNS_6StreamE
 _ZN3c106SymIntC1ENS_13intrusive_ptrINS_11SymNodeImplENS_6detail34intrusive_target_default_null_typeIS2_EEEE
 _ZN3c104cuda14ExchangeDeviceEa
 _ZN3c104cuda20setCurrentCUDAStreamENS0_10CUDAStreamE
@@ -1854,15 +1854,14 @@
 _ZNK3c104cuda4impl13CUDAGuardImpl23getStreamFromGlobalPoolENS_6DeviceEb
 _ZNK3c104impl16VirtualGuardImpl12getNewStreamENS_6DeviceEi
 _ZNSsC1EPKcmRKSaIcE@GLIBCXX_3.4
 _ZN3c1011SymNodeImpl12maybe_as_intEv
 _ZN3c1014OperatorKernelD0Ev
 PyCapsule_GetContext
 _ZNK2at10TensorBase21__dispatch_contiguousEN3c1012MemoryFormatE
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220215nms_kernel_implIfEEvidPKT_Py
 _ZN3c1011SymNodeImpl5bool_Ev
 _ZNK3c104impl16VirtualGuardImpl17synchronizeStreamERKNS_6StreamE
 _ZN2at4_ops19empty_memory_format4callEN3c108ArrayRefINS2_6SymIntEEESt8optionalINS2_10ScalarTypeEES6_INS2_6LayoutEES6_INS2_6DeviceEES6_IbES6_INS2_12MemoryFormatEE
 _ZN3c1011SymNodeImpl5cloneEv
 _ZTIN3c1014OperatorKernelE
 _ZNSs6appendEPKcm@GLIBCXX_3.4
 _ZN3c1020intrusive_ptr_targetD0Ev
@@ -1871,14 +1870,15 @@
 _PyType_Lookup
 PyThreadState_Clear
 PyErr_Clear
 _ZNSt6vectorIbSaIbEE14_M_fill_insertESt13_Bit_iteratormb
 __cxa_throw@CXXABI_1.3
 cudaStreamSynchronize@libcudart.so.12
 _ZTSFN2at6TensorERKS0_S2_dE
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIfEEvidPKT_Py
 PyCapsule_New
 PyMem_Calloc
 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_ES4_NS_4guts8typelist8typelistIJS4_S4_EEEED1Ev
 _ZN3c106detail12_str_wrapperIJPKcRKlEE4callERKS3_S5_
 _ZN2at4_ops11sort_stable4callERKNS_6TensorESt8optionalIbElb
 _ZSt20__throw_length_errorPKc@GLIBCXX_3.4
 _ZN5torch7LibraryC1ENS0_4KindESsSt8optionalIN3c1011DispatchKeyEEPKcj
@@ -1906,14 +1906,15 @@
 _ZTIN3c1010ValueErrorE
 _ZTVN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE
 PyType_Ready
 _ZTISt19bad_optional_access
 _ZTSN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_ES4_NS_4guts8typelist8typelistIJS4_EEEEE
 _ZN3c1011SymNodeImpl2geERKNS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEE
 _ZN3c105ErrorC2ENS_14SourceLocationESs
+_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_43d10e94_219315nms_kernel_implIdEEvidPKT_Py
 _ZTIN3c1011SymNodeImplE
 _ZSt24__throw_out_of_range_fmtPKcz
 _Z17QUANT_GEMM_KernelI12TilingConfigILi4ELi1ELi1EEfEvPK5uint4PK6__halfS7_PT0_mmmi
 _ZN3c104impl6detail31WrapFunctionIntoRuntimeFunctor_IPFN2at6TensorES4_S4_S4_lES4_NS_4guts8typelist8typelistIJS4_S4_S4_lEEEED0Ev
 _ZN3c1011SymNodeImpl13is_contiguousENS_8ArrayRefINS_13intrusive_ptrIS0_NS_6detail34intrusive_target_default_null_typeIS0_EEEEEES7_
 _ZN3c1011SymNodeImplD0Ev
 _ZNSs6assignERKSs@GLIBCXX_3.4
@@ -2139,15 +2140,14 @@
 _ZNSt9basic_iosIcSt11char_traitsIcEE4initEPSt15basic_streambufIcS1_E@GLIBCXX_3.4
 _ZN3c1013intrusive_ptrINS_15VariableVersion14VersionCounterENS_6detail34intrusive_target_default_null_typeIS2_EEEC2EPS2_
 _ZTISt9bad_alloc@GLIBCXX_3.4
 _ZTIN3c1015VariableVersion14VersionCounterE
 _ZNKSt15basic_stringbufIcSt11char_traitsIcESaIcEE3strEv@GLIBCXX_3.4
 _ZTISt11_Mutex_baseILN9__gnu_cxx12_Lock_policyE2EE
 _ZNSs9_M_mutateEmmm@GLIBCXX_3.4
-_ZN7torchao43_GLOBAL__N__5b2e9259_6_nms_cu_a1cad1bf_220210nms_kernelERKN2at6TensorES4_d
 PyCapsule_GetPointer
 _ZN3c1010TensorImpl17set_autograd_metaESt10unique_ptrINS_21AutogradMetaInterfaceESt14default_deleteIS2_EE
 _ZNSt15basic_stringbufIcSt11char_traitsIcESaIcEED1Ev
 _Py_NoneStruct
 __cxa_guard_release@CXXABI_1.3
 cudaEventQuery@libcudart.so.12
 _Z20BitInterleaving_4bitPh
```

### readelf --wide --decompress --hex-dump=.gnu.hash {}

```diff
@@ -1,161 +1,161 @@
 
 Hex dump of section '.gnu.hash':
   0x00000260 07010000 31010000 20000000 0b000000 ....1... .......
   0x00000270 0002a400 81000010 08900400 89b68001 ................
   0x00000280 2c080000 e8840003 00800001 e4050404 ,...............
-  0x00000290 848c81b7 40120050 404b8971 90310808 ....@..P@K.q.1..
+  0x00000290 848c81b7 40120050 404ba975 90310808 ....@..P@K.u.1..
   0x000002a0 0340000c 5888844c 6243a419 1c274311 .@..X..LbC...'C.
   0x000002b0 b1810100 00088004 8aa80411 70040110 ............p...
-  0x000002c0 03a9390c 2c8cd424 1602d0c1 c0326ba0 ..9.,..$.....2k.
+  0x000002c0 23a9390c 2c8cd424 1602d0c1 c0326ba0 #.9.,..$.....2k.
   0x000002d0 0884d69b 84200a23 02400a42 01608005 ..... .#.@.B.`..
   0x000002e0 721d0a96 83885808 10801010 400e041c r.....X.....@...
-  0x000002f0 00042040 82012210 1321d848 36884042 .. @.."..!.H6.@B
+  0x000002f0 0004a000 80012210 1321d848 36880042 ......"..!.H6..B
   0x00000300 30800000 e00881c3 0302e181 4100032b 0...........A..+
   0x00000310 000c8125 05583404 18980888 12815810 ...%.X4.......X.
   0x00000320 00200002 30240211 20c81000 1c80c608 . ..0$.. .......
   0x00000330 4c800058 01963001 01030260 50188080 L..X..0....`P...
-  0x00000340 10102005 20a18250 0c482300 8915a200 .. . ..P.H#.....
+  0x00000340 10102005 20a18250 0c482100 81158000 .. . ..P.H!.....
   0x00000350 b402cb82 801642e4 12808302 44282062 ......B.....D( b
   0x00000360 9a80400c 6b0e328d 04104209 00002080 ..@.k.2...B... .
   0x00000370 31010000 36010000 00000000 38010000 1...6.......8...
   0x00000380 3a010000 00000000 00000000 00000000 :...............
   0x00000390 3c010000 3d010000 40010000 41010000 <...=...@...A...
   0x000003a0 00000000 00000000 00000000 42010000 ............B...
   0x000003b0 43010000 44010000 00000000 45010000 C...D.......E...
   0x000003c0 46010000 49010000 00000000 00000000 F...I...........
-  0x000003d0 4a010000 4c010000 4d010000 4f010000 J...L...M...O...
-  0x000003e0 52010000 53010000 55010000 00000000 R...S...U.......
-  0x000003f0 56010000 57010000 58010000 5a010000 V...W...X...Z...
-  0x00000400 5c010000 5e010000 00000000 00000000 \...^...........
-  0x00000410 60010000 62010000 00000000 00000000 `...b...........
-  0x00000420 63010000 64010000 66010000 68010000 c...d...f...h...
-  0x00000430 6a010000 00000000 6b010000 6c010000 j.......k...l...
-  0x00000440 6e010000 6f010000 70010000 00000000 n...o...p.......
-  0x00000450 00000000 72010000 00000000 00000000 ....r...........
-  0x00000460 74010000 00000000 77010000 78010000 t.......w...x...
-  0x00000470 7a010000 7c010000 7f010000 80010000 z...|...........
-  0x00000480 85010000 87010000 88010000 00000000 ................
-  0x00000490 89010000 8a010000 00000000 8d010000 ................
-  0x000004a0 8f010000 90010000 91010000 94010000 ................
+  0x000003d0 4a010000 4d010000 4e010000 50010000 J...M...N...P...
+  0x000003e0 53010000 54010000 56010000 00000000 S...T...V.......
+  0x000003f0 57010000 58010000 59010000 5b010000 W...X...Y...[...
+  0x00000400 5d010000 5f010000 00000000 00000000 ]..._...........
+  0x00000410 61010000 63010000 00000000 00000000 a...c...........
+  0x00000420 64010000 65010000 67010000 69010000 d...e...g...i...
+  0x00000430 6b010000 00000000 6c010000 6d010000 k.......l...m...
+  0x00000440 6f010000 70010000 71010000 00000000 o...p...q.......
+  0x00000450 00000000 73010000 00000000 00000000 ....s...........
+  0x00000460 75010000 00000000 78010000 79010000 u.......x...y...
+  0x00000470 7b010000 7d010000 80010000 81010000 {...}...........
+  0x00000480 86010000 88010000 89010000 00000000 ................
+  0x00000490 8a010000 8b010000 00000000 8e010000 ................
+  0x000004a0 90010000 91010000 92010000 00000000 ................
   0x000004b0 00000000 95010000 00000000 96010000 ................
   0x000004c0 9b010000 00000000 9d010000 9e010000 ................
   0x000004d0 00000000 a0010000 a2010000 00000000 ................
   0x000004e0 00000000 a4010000 a5010000 00000000 ................
   0x000004f0 00000000 a6010000 a7010000 a9010000 ................
   0x00000500 ab010000 00000000 ac010000 ad010000 ................
-  0x00000510 af010000 b0010000 b1010000 b2010000 ................
-  0x00000520 b3010000 00000000 b4010000 b6010000 ................
-  0x00000530 00000000 00000000 b7010000 b8010000 ................
-  0x00000540 ba010000 bd010000 be010000 c0010000 ................
-  0x00000550 c1010000 00000000 00000000 00000000 ................
-  0x00000560 c2010000 c4010000 c5010000 00000000 ................
-  0x00000570 c9010000 cb010000 ce010000 cf010000 ................
-  0x00000580 00000000 d0010000 00000000 d1010000 ................
-  0x00000590 00000000 d2010000 d4010000 d6010000 ................
-  0x000005a0 00000000 d7010000 d9010000 da010000 ................
-  0x000005b0 00000000 00000000 db010000 00000000 ................
-  0x000005c0 dc010000 00000000 de010000 00000000 ................
-  0x000005d0 df010000 00000000 00000000 e0010000 ................
-  0x000005e0 e4010000 e5010000 e6010000 00000000 ................
-  0x000005f0 00000000 e7010000 e9010000 ea010000 ................
-  0x00000600 00000000 ee010000 ef010000 f0010000 ................
-  0x00000610 f2010000 f3010000 00000000 00000000 ................
-  0x00000620 f4010000 00000000 f7010000 fa010000 ................
-  0x00000630 00000000 fd010000 fe010000 00000000 ................
-  0x00000640 ff010000 02020000 03020000 04020000 ................
-  0x00000650 05020000 00000000 06020000 08020000 ................
-  0x00000660 00000000 09020000 0a020000 0d020000 ................
-  0x00000670 00000000 0e020000 0f020000 11020000 ................
-  0x00000680 00000000 00000000 12020000 13020000 ................
-  0x00000690 16020000 00000000 17020000 1b020000 ................
-  0x000006a0 1d020000 1f020000 21020000 25020000 ........!...%...
-  0x000006b0 00000000 00000000 00000000 27020000 ............'...
-  0x000006c0 28020000 00000000 29020000 2a020000 (.......)...*...
-  0x000006d0 2f020000 30020000 33020000 00000000 /...0...3.......
-  0x000006e0 34020000 00000000 36020000 00000000 4.......6.......
-  0x000006f0 37020000 38020000 39020000 3a020000 7...8...9...:...
-  0x00000700 00000000 00000000 3e020000 3f020000 ........>...?...
+  0x00000510 af010000 b0010000 b1010000 00000000 ................
+  0x00000520 b2010000 00000000 b3010000 b5010000 ................
+  0x00000530 00000000 00000000 b6010000 b7010000 ................
+  0x00000540 b9010000 bc010000 bd010000 bf010000 ................
+  0x00000550 c0010000 00000000 00000000 00000000 ................
+  0x00000560 c1010000 c3010000 c4010000 00000000 ................
+  0x00000570 c8010000 ca010000 cd010000 ce010000 ................
+  0x00000580 00000000 cf010000 00000000 d0010000 ................
+  0x00000590 00000000 d1010000 d3010000 d5010000 ................
+  0x000005a0 00000000 d6010000 00000000 d8010000 ................
+  0x000005b0 00000000 00000000 d9010000 00000000 ................
+  0x000005c0 da010000 00000000 dc010000 00000000 ................
+  0x000005d0 dd010000 00000000 00000000 de010000 ................
+  0x000005e0 e2010000 e3010000 e4010000 00000000 ................
+  0x000005f0 00000000 e5010000 e7010000 e8010000 ................
+  0x00000600 00000000 ec010000 ed010000 ee010000 ................
+  0x00000610 f0010000 f1010000 00000000 00000000 ................
+  0x00000620 f2010000 00000000 f5010000 f8010000 ................
+  0x00000630 00000000 fb010000 fc010000 00000000 ................
+  0x00000640 fd010000 00020000 01020000 02020000 ................
+  0x00000650 03020000 00000000 04020000 06020000 ................
+  0x00000660 00000000 07020000 08020000 0b020000 ................
+  0x00000670 0c020000 0d020000 0f020000 11020000 ................
+  0x00000680 00000000 00000000 00000000 12020000 ................
+  0x00000690 15020000 00000000 16020000 1a020000 ................
+  0x000006a0 1c020000 1e020000 20020000 24020000 ........ ...$...
+  0x000006b0 00000000 00000000 00000000 26020000 ............&...
+  0x000006c0 27020000 00000000 28020000 29020000 '.......(...)...
+  0x000006d0 2e020000 2f020000 32020000 00000000 ..../...2.......
+  0x000006e0 33020000 00000000 35020000 00000000 3.......5.......
+  0x000006f0 36020000 37020000 38020000 39020000 6...7...8...9...
+  0x00000700 00000000 00000000 3d020000 3e020000 ........=...>...
   0x00000710 00000000 00000000 00000000 00000000 ................
-  0x00000720 41020000 00000000 00000000 00000000 A...............
-  0x00000730 00000000 42020000 00000000 44020000 ....B.......D...
-  0x00000740 00000000 46020000 47020000 4b020000 ....F...G...K...
+  0x00000720 40020000 00000000 00000000 00000000 @...............
+  0x00000730 00000000 41020000 00000000 43020000 ....A.......C...
+  0x00000740 00000000 45020000 47020000 4b020000 ....E...G...K...
   0x00000750 4c020000 00000000 00000000 00000000 L...............
   0x00000760 4d020000 00000000 4f020000 54020000 M.......O...T...
   0x00000770 55020000 00000000 57020000 00000000 U.......W.......
   0x00000780 59020000 00000000 5b020000 ee75e894 Y.......[....u..
   0x00000790 a6f48746 a2282fda eac1b783 6d6fd341 ...F.(/.....mo.A
   0x000007a0 5c994e79 e7ea9b05 8403e52b 4b2a81a5 \.Ny.......+K*..
   0x000007b0 9a7aa625 83c81559 0b953746 1c6153fd .z.%...Y..7F.aS.
   0x000007c0 ba2fdfb8 5d3965c4 034e8d3f cb252176 ./..]9e..N.?.%!v
   0x000007d0 edaedc77 abd2f46e cf536567 81f1d544 ...w...n.Seg...D
   0x000007e0 ceb5ef4d d890ab41 65246ad6 3f4fc4e8 ...M...Ae$j.?O..
-  0x000007f0 4a812065 fd0a4894 5fe5cd9f b834db7d J. e..H._....4.}
-  0x00000800 0be195aa a47c409b be2c5ecf 837853ce .....|@..,^..xS.
-  0x00000810 f1faad2c 12cb1f67 d1c43ad0 6b908c99 ...,...g..:.k...
-  0x00000820 592125c6 4fef45a0 701a5425 f9bc202a Y!%.O.E.p.T%.. *
-  0x00000830 560f641f 3d571b4b 5e494e62 47e9e4a9 V.d.=W.K^INbG...
-  0x00000840 289fb23b a10757a6 bae3927c ab8f8b8c (..;..W....|....
-  0x00000850 d784d5f6 49b4049e d6a9b069 492607ee ....I......iI&..
-  0x00000860 d8223690 fb33dfb8 42528d3f 999bbb4c ."6..3..BR.?...L
-  0x00000870 17a8c695 c5a5e423 aa2fa53b c9491703 .......#./.;.I..
-  0x00000880 2db3dc77 355d7595 7cddfae6 f75e326b -..w5]u.|....^2k
-  0x00000890 10baef4d a5286ad6 10c3a2f6 6ecc0770 ...M.(j.....n..p
-  0x000008a0 2bd5f6bf 4f92fe78 4ae595aa 91db71b0 +...O..xJ.....q.
-  0x000008b0 9a828e22 a5b96994 f695ffaf 5832c56e ..."..i.....X2.n
-  0x000008c0 31ffad2c 9b910321 baba2758 8426ec49 1..,...!..'X.&.I
-  0x000008d0 26dbfe15 c4a3521f 41f6acd4 c8e1185c &.....R.A......\
-  0x000008e0 f1ec498a 992525c6 f991741f e7505f11 ..I..%%...t..P_.
-  0x000008f0 e2493c34 f06acdd9 e7787ebb e64655ff .I<4.j...x~..FU.
-  0x00000900 f7890bcc 53a553bf eb938b8c 16cbae90 ....S.S.........
-  0x00000910 6a5f0533 2f067b51 d18e4106 1dbd544d j_.3/.{Q..A...TM
+  0x000007f0 aa02b2b7 4a812065 fd0a4894 5fe5cd9f ....J. e..H._...
+  0x00000800 b834db7d 0be195aa a47c409b be2c5ecf .4.}.....|@..,^.
+  0x00000810 837853ce f1faad2c 12cb1f67 d1c43ad0 .xS....,...g..:.
+  0x00000820 6b908c99 592125c6 4fef45a0 701a5425 k...Y!%.O.E.p.T%
+  0x00000830 f9bc202a 560f641f 3d571b4b 5e494e62 .. *V.d.=W.K^INb
+  0x00000840 47e9e4a9 289fb23b a10757a6 bae3927c G...(..;..W....|
+  0x00000850 ab8f8b8c d784d5f6 49b4049e d6a9b069 ........I......i
+  0x00000860 492607ee d8223690 fb33dfb8 42528d3f I&..."6..3..BR.?
+  0x00000870 999bbb4c 17a8c695 c5a5e423 aa2fa53b ...L.......#./.;
+  0x00000880 c9491703 2db3dc77 355d7595 7cddfae6 .I..-..w5]u.|...
+  0x00000890 f75e326b 10baef4d a5286ad6 10c3a2f6 .^2k...M.(j.....
+  0x000008a0 6ecc0770 2bd5f6bf 4f92fe78 4ae595aa n..p+...O..xJ...
+  0x000008b0 91db71b0 9a828e22 a5b96994 f695ffaf ..q...."..i.....
+  0x000008c0 5832c56e 31ffad2c 9b910321 baba2758 X2.n1..,...!..'X
+  0x000008d0 8426ec49 26dbfe15 c4a3521f 41f6acd4 .&.I&.....R.A...
+  0x000008e0 c8e1185c f1ec498a 992525c6 f991741f ...\..I..%%...t.
+  0x000008f0 e7505f11 e2493c34 f06acdd9 e7787ebb .P_..I<4.j...x~.
+  0x00000900 e64655ff f7890bcc 53a553bf eb938b8c .FU.....S.S.....
+  0x00000910 16cbae90 6a5f0533 2f067b51 1dbd544d ....j_.3/.{Q..TM
   0x00000920 0822b67c 0eaeb36e 3c38dfb8 4245d5ec .".|...n<8..BE..
   0x00000930 19273690 9e6352ae 7b7304f6 b91fc917 .'6..cR.{s......
   0x00000940 8cb2e115 ff17ac59 a4aebeb5 113fbeb3 .......Y.....?..
   0x00000950 b252bb2e 63ef1bef bf27cc22 51beef4d .R..c....'."Q..M
   0x00000960 8b18ff4f 949ad083 f3ba40f5 961ffd61 ...O......@....a
   0x00000970 27f92483 f5fa92bf 2148e42f 06b96a6e '.$.....!H./..jn
   0x00000980 69413d51 e116b884 2d66413f a52d0132 iA=Q....-fA?.-.2
-  0x00000990 21f45278 5d661733 b624fcd0 27547eb8 !.Rx]f.3.$..'T~.
-  0x000009a0 55f4092b 3b7a3c7c 226ba1b1 39eb67aa U..+;z<|"k..9.g.
-  0x000009b0 8c2db72e 5a14dfdc ab23603f cf7da59d .-..Z....#`?.}..
-  0x000009c0 600444eb 17a30a3f ab31a18d 790b4835 `.D....?.1..y.H5
-  0x000009d0 c611c5c7 b709706c 89533e2c 9a424223 ......pl.S>,.BB#
-  0x000009e0 66cfdc15 a6105e81 e7b2beb5 dce3f77e f.....^........~
-  0x000009f0 3b65ab31 66be899f 86d7b7ee c5d978b1 ;e.1f.........x.
-  0x00000a00 d7ac2aff 2db36874 a31a6fbf 53f43a63 ..*.-.ht..o.S.:c
-  0x00000a10 1c9b8bcd 2fa68be0 2a2a5e38 538bdc2b ..../...**^8S..+
-  0x00000a20 716a5c04 deb23359 1be17196 e3ae39da qj\...3Y..q...9.
-  0x00000a30 ebd3ef0e eb1e26db ac662293 415c57ca ......&..f".A\W.
-  0x00000a40 d98f9c4a 63bcf6ad b0be5902 ae46d3f5 ...Jc.....Y..F..
-  0x00000a50 8c5bccde b98df10e 0be16ca3 5b657489 .[........l.[et.
-  0x00000a60 b75ac029 06028a59 afa20bd5 8faf1362 .Z.)...Y.......b
-  0x00000a70 26b7beb5 864fbf5a 3a2f9c7b a7d3dc15 &....O.Z:/.{....
-  0x00000a80 7b69ab31 07de78b1 a0e33888 9b1f6861 {i.1..x...8...ha
-  0x00000a90 2d8f5471 2175c7e1 44cf4de1 586bebc4 -.Tq!u..D.M.Xk..
-  0x00000aa0 f71d0d80 20854e9c 72418a9d b30a7245 .... .N.rA....rE
-  0x00000ab0 0afb0a3d 3cac53b3 bbd7a8ad 19a51d1f ...=<.S.........
-  0x00000ac0 1fb73359 78383bb9 aac4333c 6f78e0a2 ..3Yx8;...3<ox..
-  0x00000ad0 cf865ca0 d971581c abc0bb5b 777d8f87 ..\..qX....[w}..
-  0x00000ae0 2255f253 af9b9f85 73259f9f 0b446fa5 "U.S....s%...Do.
-  0x00000af0 f0150db5 64e29b05 49fe7d14 815b2598 ....d...I.}..[%.
+  0x00000990 5d661733 b624fcd0 27547eb8 55f4092b ]f.3.$..'T~.U..+
+  0x000009a0 3b7a3c7c 226ba1b1 39eb67aa 8c2db72e ;z<|"k..9.g..-..
+  0x000009b0 5a14dfdc ab23603f cf7da59d 600444eb Z....#`?.}..`.D.
+  0x000009c0 17a30a3f ab31a18d 790b4835 c611c5c7 ...?.1..y.H5....
+  0x000009d0 b709706c 89533e2c 9a424223 66cfdc15 ..pl.S>,.BB#f...
+  0x000009e0 a6105e81 e7b2beb5 dce3f77e 3b65ab31 ..^........~;e.1
+  0x000009f0 66be899f 86d7b7ee c5d978b1 d7ac2aff f.........x...*.
+  0x00000a00 2db36874 a31a6fbf 53f43a63 1c9b8bcd -.ht..o.S.:c....
+  0x00000a10 2fa68be0 2a2a5e38 538bdc2b 716a5c04 /...**^8S..+qj\.
+  0x00000a20 deb23359 1be17196 ebd3ef0e eb1e26db ..3Y..q.......&.
+  0x00000a30 ac662293 415c57ca d98f9c4a 63bcf6ad .f".A\W....Jc...
+  0x00000a40 b0be5902 ae46d3f5 8c5bccde b98df10e ..Y..F...[......
+  0x00000a50 0be16ca3 5b657489 b75ac029 06028a59 ..l.[et..Z.)...Y
+  0x00000a60 afa20bd5 8faf1362 26b7beb5 864fbf5a .......b&....O.Z
+  0x00000a70 3a2f9c7b a7d3dc15 7b69ab31 07de78b1 :/.{....{i.1..x.
+  0x00000a80 a0e33888 9b1f6861 2d8f5471 2175c7e1 ..8...ha-.Tq!u..
+  0x00000a90 44cf4de1 586bebc4 f71d0d80 20854e9c D.M.Xk...... .N.
+  0x00000aa0 72418a9d b30a7245 0afb0a3d 3cac53b3 rA....rE...=<.S.
+  0x00000ab0 bbd7a8ad 19a51d1f 1fb73359 78383bb9 ..........3Yx8;.
+  0x00000ac0 aac4333c 6f78e0a2 cf865ca0 d971581c ..3<ox....\..qX.
+  0x00000ad0 abc0bb5b 777d8f87 2255f253 af9b9f85 ...[w}.."U.S....
+  0x00000ae0 73259f9f 0b446fa5 f0150db5 64e29b05 s%...Do.....d...
+  0x00000af0 49fe7d14 815b2598 55d1d8b9 168cbf1b I.}..[%.U.......
   0x00000b00 d7675445 30acd6f9 f9fce865 1f81e828 .gTE0......e...(
-  0x00000b10 77149fec b4332c58 6af69c28 bb717818 w....3,Xj..(.qx.
-  0x00000b20 03e6a81f 6060f79e 281622e0 bc6dab31 ....``..(."..m.1
-  0x00000b30 abe5c9af 46e278b1 2190d23a bad19060 ....F.x.!..:...`
-  0x00000b40 99d64e51 3c498574 ed2137bd f0b2ca4f ..NQ<I.t.!7....O
-  0x00000b50 761836ed 1af13f51 bb91c17d 2ae6506d v.6...?Q...}*.Pm
-  0x00000b60 bd7a7cec 61ddc83b e3282996 93b3cf6b .z|.a..;.()....k
-  0x00000b70 ae211d71 802aa546 ce81b900 60bb3359 .!.q.*.F....`.3Y
-  0x00000b80 c362f9d8 1f7ef0fc b83c3bb9 b07ce0a2 .b...~...<;..|..
-  0x00000b90 51b924fe 0f8b5ca0 80a75118 0fc93a72 Q.$...\...Q...:r
-  0x00000ba0 af19fbdc 6544aaee a72f0bd1 457d6eff ....eD.../..E}n.
-  0x00000bb0 66522973 4eafc9c6 a4e69b05 c9e113b3 fR)sN...........
-  0x00000bc0 412acdb3 7eaf37a5 e9239031 c1498d3f A*..~.7..#.1.I.?
-  0x00000bd0 aaaadc77 6d711e42 02c6816c 5f73fbe0 ...wmq.B...l_s..
+  0x00000b10 b4332c58 6af69c28 bb717818 03e6a81f .3,Xj..(.qx.....
+  0x00000b20 6060f79e 281622e0 bc6dab31 abe5c9af ``..(."..m.1....
+  0x00000b30 46e278b1 2190d23a bad19060 99d64e51 F.x.!..:...`..NQ
+  0x00000b40 3c498574 ed2137bd f0b2ca4f 761836ed <I.t.!7....Ov.6.
+  0x00000b50 1af13f51 bb91c17d 2ae6506d bd7a7cec ..?Q...}*.Pm.z|.
+  0x00000b60 61ddc83b e3282996 93b3cf6b ae211d71 a..;.()....k.!.q
+  0x00000b70 802aa546 ce81b900 60bb3359 c362f9d8 .*.F....`.3Y.b..
+  0x00000b80 1f7ef0fc b83c3bb9 b07ce0a2 51b924fe .~...<;..|..Q.$.
+  0x00000b90 0f8b5ca0 80a75118 0fc93a72 af19fbdc ..\...Q...:r....
+  0x00000ba0 6544aaee a72f0bd1 457d6eff 66522973 eD.../..E}n.fR)s
+  0x00000bb0 4eafc9c6 a4e69b05 c9e113b3 412acdb3 N...........A*..
+  0x00000bc0 7eaf37a5 e9239031 c1498d3f aaaadc77 ~.7..#.1.I.?...w
+  0x00000bd0 6d711e42 02c6816c 5f73fbe0 84128378 mq.B...l_s.....x
   0x00000be0 656cdc0f a6c0fd4e a2a26a4c e6041b27 el.....N..jL...'
   0x00000bf0 1127dad8 fd4ac4e8 efdd0fd2 028bbdff .'...J..........
   0x00000c00 c9dc95aa f4df8617 d84ae7c5 aef6ad2c .........J.....,
   0x00000c10 6248eba2 fb403bb9 518f5ca0 18110eb9 bH...@;.Q.\.....
   0x00000c20 734113b9 d43aa1a2 1717866e c00448cc sA...:.....n..H.
   0x00000c30 6d60aa82 e919a750                   m`.....P
```

### readelf --wide --decompress --hex-dump=.dynstr {}

```diff
@@ -1172,27 +1172,27 @@
   0x00008de8 70655074 72495331 5f454576 005f5a4e pePtrIS1_EEv._ZN
   0x00008df8 4b336331 30346375 64613469 6d706c31 K3c104cuda4impl1
   0x00008e08 33435544 41477561 7264496d 706c3130 3CUDAGuardImpl10
   0x00008e18 71756572 79457665 6e744550 76006375 queryEventEPv.cu
   0x00008e28 64614576 656e7451 75657279 005f5a4e daEventQuery._ZN
   0x00008e38 37746f72 6368616f 34335f47 4c4f4241 7torchao43_GLOBA
   0x00008e48 4c5f5f4e 5f5f3562 32653932 35395f36 L__N__5b2e9259_6
-  0x00008e58 5f6e6d73 5f63755f 61316361 64316266 _nms_cu_a1cad1bf
-  0x00008e68 5f323230 3231356e 6d735f6b 65726e65 _220215nms_kerne
+  0x00008e58 5f6e6d73 5f63755f 34336431 30653934 _nms_cu_43d10e94
+  0x00008e68 5f323139 3331356e 6d735f6b 65726e65 _219315nms_kerne
   0x00008e78 6c5f696d 706c4966 45457669 64504b54 l_implIfEEvidPKT
   0x00008e88 5f507900 5f5a4e37 746f7263 68616f34 _Py._ZN7torchao4
   0x00008e98 335f474c 4f42414c 5f5f4e5f 5f356232 3_GLOBAL__N__5b2
-  0x00008ea8 65393235 395f365f 6e6d735f 63755f61 e9259_6_nms_cu_a
-  0x00008eb8 31636164 3162665f 32323032 31356e6d 1cad1bf_220215nm
+  0x00008ea8 65393235 395f365f 6e6d735f 63755f34 e9259_6_nms_cu_4
+  0x00008eb8 33643130 6539345f 32313933 31356e6d 3d10e94_219315nm
   0x00008ec8 735f6b65 726e656c 5f696d70 6c494e33 s_kernel_implIN3
   0x00008ed8 63313034 48616c66 45454576 6964504b c104HalfEEEvidPK
   0x00008ee8 545f5079 005f5a4e 37746f72 6368616f T_Py._ZN7torchao
   0x00008ef8 34335f47 4c4f4241 4c5f5f4e 5f5f3562 43_GLOBAL__N__5b
   0x00008f08 32653932 35395f36 5f6e6d73 5f63755f 2e9259_6_nms_cu_
-  0x00008f18 61316361 64316266 5f323230 3231356e a1cad1bf_220215n
+  0x00008f18 34336431 30653934 5f323139 3331356e 43d10e94_219315n
   0x00008f28 6d735f6b 65726e65 6c5f696d 706c4964 ms_kernel_implId
   0x00008f38 45457669 64504b54 5f507900 5f5a4e33 EEvidPKT_Py._ZN3
   0x00008f48 63313031 3056616c 75654572 726f7244 c1010ValueErrorD
   0x00008f58 32457600 5f5a5456 4e336331 30354572 2Ev._ZTVN3c105Er
   0x00008f68 726f7245 005f5a4e 53743965 78636570 rorE._ZNSt9excep
   0x00008f78 74696f6e 44324576 005f5a4e 33633130 tionD2Ev._ZN3c10
   0x00008f88 31305661 6c756545 72726f72 44314576 10ValueErrorD1Ev
@@ -1334,16 +1334,16 @@
   0x00009808 335f5335 5f53385f 005f5a4e 33633130 3_S5_S8_._ZN3c10
   0x00009818 36646574 61696c31 325f7374 725f7772 6detail12_str_wr
   0x00009828 61707065 72494a52 4b63524b 5053325f apperIJRKcRKPS2_
   0x00009838 53345f53 365f5334 5f454534 63616c6c S4_S6_S4_EE4call
   0x00009848 4553335f 53365f53 365f5336 5f53365f ES3_S6_S6_S6_S6_
   0x00009858 005f5a4e 37746f72 6368616f 34335f47 ._ZN7torchao43_G
   0x00009868 4c4f4241 4c5f5f4e 5f5f3562 32653932 LOBAL__N__5b2e92
-  0x00009878 35395f36 5f6e6d73 5f63755f 61316361 59_6_nms_cu_a1ca
-  0x00009888 64316266 5f323230 3231306e 6d735f6b d1bf_220210nms_k
+  0x00009878 35395f36 5f6e6d73 5f63755f 34336431 59_6_nms_cu_43d1
+  0x00009888 30653934 5f323139 3331306e 6d735f6b 0e94_219310nms_k
   0x00009898 65726e65 6c45524b 4e326174 3654656e ernelERKN2at6Ten
   0x000098a8 736f7245 53345f64 005f5a54 564e3363 sorES4_d._ZTVN3c
   0x000098b8 31303463 75646134 696d706c 31334355 104cuda4impl13CU
   0x000098c8 44414775 61726449 6d706c45 005f5a4e DAGuardImplE._ZN
   0x000098d8 32617434 5f6f7073 3131736f 72745f73 2at4_ops11sort_s
   0x000098e8 7461626c 65346361 6c6c4552 4b4e535f table4callERKNS_
   0x000098f8 3654656e 736f7245 5374386f 7074696f 6TensorESt8optio
@@ -1842,9 +1842,9 @@
   0x0000b7c8 5f332e34 2e313800 43585841 42495f31 _3.4.18.CXXABI_1
   0x0000b7d8 2e332e32 00435858 4142495f 312e332e .3.2.CXXABI_1.3.
   0x0000b7e8 3500474c 49424358 585f332e 342e3900 5.GLIBCXX_3.4.9.
   0x0000b7f8 43585841 42495f31 2e332e33 00435858 CXXABI_1.3.3.CXX
   0x0000b808 4142495f 312e3300 474c4942 4358585f ABI_1.3.GLIBCXX_
   0x0000b818 332e3400 2f5f5f77 2f5f7465 6d702f63 3.4./__w/_temp/c
   0x0000b828 6f6e6461 5f656e76 69726f6e 6d656e74 onda_environment
-  0x0000b838 5f393134 34343432 3532372f 6c696200 _9144442527/lib.
+  0x0000b838 5f393138 33333139 3235302f 6c696200 _9183319250/lib.
```

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.init {}

```diff
@@ -2,13 +2,13 @@
 
 
 Disassembly of section .init:
 
 0000000000010000 <_init>:
 _init():
 	sub    $0x8,%rsp
-	mov    0xa5efd(%rip),%rax        
+	mov    0xa5f05(%rip),%rax        
 	test   %rax,%rax
 	je     10015 <_init+0x15>
 	call   11398 <__gmon_start__@plt>
 	add    $0x8,%rsp
 	ret
```

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt.got {}

```diff
@@ -4,17 +4,17 @@
 Disassembly of section .plt.got:
 
 0000000000011380 <vsnprintf@plt>:
 	jmp    *0xa4a32(%rip)        
 	xchg   %ax,%ax
 
 0000000000011388 <__cxa_finalize@plt>:
-	jmp    *0xa4b32(%rip)        
+	jmp    *0xa4b3a(%rip)        
 	xchg   %ax,%ax
 
 0000000000011390 <SplitK_Reduction(__half*, float*, unsigned long, unsigned long, int)@plt>:
-	jmp    *0xa4b4a(%rip)        
+	jmp    *0xa4b52(%rip)        
 	xchg   %ax,%ax
 
 0000000000011398 <__gmon_start__@plt>:
-	jmp    *0xa4b6a(%rip)        
+	jmp    *0xa4b72(%rip)        
 	xchg   %ax,%ax
```

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -8,45 +8,45 @@
 	mov    %r12,%rdi
 	call   100d0 <c10::intrusive_ptr<c10::TensorImpl, c10::UndefinedTensorImpl>::reset_()@plt>
 	mov    %r13,%rdi
 	call   100d0 <c10::intrusive_ptr<c10::TensorImpl, c10::UndefinedTensorImpl>::reset_()@plt>
 	mov    %rbx,%rdi
 	call   10650 <_Unwind_Resume@plt>
 
-00000000000113b8 <_GLOBAL__sub_I_tmpxft_00000877_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold>:
-_GLOBAL__sub_I_tmpxft_00000877_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold():
+00000000000113b8 <_GLOBAL__sub_I_tmpxft_0000086e_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold>:
+_GLOBAL__sub_I_tmpxft_0000086e_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold():
 	mov    %r12,%rdi
 	call   11330 <c10::intrusive_ptr<c10::OperatorKernel, c10::detail::intrusive_target_default_null_type<c10::OperatorKernel> >::reset_()@plt>
 	lea    0xa5779(%rip),%rdi        
 	call   107b0 <torch::Library::~Library()@plt>
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	mov    0x10(%rsp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    0xa4944(%rip),%rdi        
-	je     113f0 <_GLOBAL__sub_I_tmpxft_00000877_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold+0x38>
+	je     113f0 <_GLOBAL__sub_I_tmpxft_0000086e_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold+0x38>
 	lea    0x6(%rsp),%rsi
 	call   13850 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	mov    %rbp,%rdi
 	mov    %rbx,%rbp
 	call   10c80 <torch::CppFunction::~CppFunction()@plt>
-	jmp    113c0 <_GLOBAL__sub_I_tmpxft_00000877_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold+0x8>
+	jmp    113c0 <_GLOBAL__sub_I_tmpxft_0000086e_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold+0x8>
 
 0000000000011405 <cast_fp16_fp6(unsigned short*, unsigned char*) [clone .cold]>:
 cast_fp16_fp6(unsigned short*, unsigned char*) [clone .cold]:
 	mov    $0x10,%edi
 	call   10d60 <__cxa_allocate_exception@plt>
 	lea    0x235fa(%rip),%rsi        
 	mov    %rax,%rdi
 	mov    %rax,%r12
 	call   10cf0 <std::invalid_argument::invalid_argument(char const*)@plt>
-	mov    0xa4ad0(%rip),%rdx        
-	mov    0xa4ad1(%rip),%rsi        
+	mov    0xa4ad8(%rip),%rdx        
+	mov    0xa4ad9(%rip),%rsi        
 	mov    %r12,%rdi
 	call   105d0 <__cxa_throw@plt>
 	mov    %rax,%rbp
 	mov    %r12,%rdi
 	call   11130 <__cxa_free_exception@plt>
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
@@ -55,16 +55,16 @@
 weight_prepacking_fp16_to_fp6(unsigned short*, unsigned char*, unsigned long, unsigned long) [clone .cold]:
 	mov    $0x10,%edi
 	call   10d60 <__cxa_allocate_exception@plt>
 	lea    0x238f4(%rip),%rsi        
 	mov    %rax,%rdi
 	mov    %rax,%rbp
 	call   10cf0 <std::invalid_argument::invalid_argument(char const*)@plt>
-	mov    0xa4a8b(%rip),%rdx        
-	mov    0xa4a8c(%rip),%rsi        
+	mov    0xa4a93(%rip),%rdx        
+	mov    0xa4a94(%rip),%rsi        
 	mov    %rbp,%rdi
 	call   105d0 <__cxa_throw@plt>
 	mov    %rax,%r12
 	mov    %rbp,%rdi
 	call   11130 <__cxa_free_exception@plt>
 	mov    %r12,%rdi
 	call   10650 <_Unwind_Resume@plt>
@@ -79,45 +79,45 @@
 000000000001149f <torchao::weight_matrix_dequant_cpu(at::Tensor, at::Tensor) [clone .cold]>:
 torchao::weight_matrix_dequant_cpu(at::Tensor, at::Tensor) [clone .cold]:
 	mov    %r13,%rdi
 	call   100d0 <c10::intrusive_ptr<c10::TensorImpl, c10::UndefinedTensorImpl>::reset_()@plt>
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
 
-00000000000114af <_GLOBAL__sub_I_tmpxft_00000878_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold>:
-_GLOBAL__sub_I_tmpxft_00000878_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold():
+00000000000114af <_GLOBAL__sub_I_tmpxft_0000086f_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold>:
+_GLOBAL__sub_I_tmpxft_0000086f_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold():
 	mov    %r12,%rdi
 	call   11180 <c10::FunctionSchema::~FunctionSchema()@plt>
 	mov    %r13,%rdi
 	call   11330 <c10::intrusive_ptr<c10::OperatorKernel, c10::detail::intrusive_target_default_null_type<c10::OperatorKernel> >::reset_()@plt>
 	lea    0xa571a(%rip),%rdi        
 	call   107b0 <torch::Library::~Library()@plt>
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	mov    0xa0(%rsp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    0xa4842(%rip),%rdi        
-	je     114f2 <_GLOBAL__sub_I_tmpxft_00000878_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x43>
+	je     114f2 <_GLOBAL__sub_I_tmpxft_0000086f_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x43>
 	lea    0x30(%rsp),%rsi
 	call   19560 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	mov    %rbp,%rdi
 	mov    %rbx,%rbp
 	call   10c80 <torch::CppFunction::~CppFunction()@plt>
-	jmp    114bf <_GLOBAL__sub_I_tmpxft_00000878_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x10>
+	jmp    114bf <_GLOBAL__sub_I_tmpxft_0000086f_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x10>
 	mov    %r12,%rdi
 	call   11180 <c10::FunctionSchema::~FunctionSchema()@plt>
 	mov    %r13,%rdi
 	call   11330 <c10::intrusive_ptr<c10::OperatorKernel, c10::detail::intrusive_target_default_null_type<c10::OperatorKernel> >::reset_()@plt>
-	jmp    114bf <_GLOBAL__sub_I_tmpxft_00000878_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x10>
+	jmp    114bf <_GLOBAL__sub_I_tmpxft_0000086f_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x10>
 	mov    %rbp,%rdi
 	mov    %rbx,%rbp
 	call   10c80 <torch::CppFunction::~CppFunction()@plt>
-	jmp    114bf <_GLOBAL__sub_I_tmpxft_00000878_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x10>
+	jmp    114bf <_GLOBAL__sub_I_tmpxft_0000086f_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x10>
 
 0000000000011526 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double) [clone .cold]>:
 torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double) [clone .cold]:
 	mov    -0x1b0(%rbp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    0xa47f0(%rip),%rdi        
 	je     11542 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double) [clone .cold]+0x1c>
@@ -205,15 +205,15 @@
 	mov    %rax,(%rbx)
 	mov    -0x210(%rbp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    0xa463a(%rip),%rdi        
 	je     116fc <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double) [clone .cold]+0x1d6>
 	mov    -0x2d8(%rbp),%rsi
 	call   1bcc0 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>
-	mov    0xa4735(%rip),%rdx        
+	mov    0xa473d(%rip),%rdx        
 	mov    0xa46d6(%rip),%rsi        
 	mov    %rbx,%rdi
 	call   105d0 <__cxa_throw@plt>
 	mov    %rax,%rbx
 	mov    $0x3,%eax
 	shl    $0x3e,%rax
 	cmp    %rax,-0x170(%rbp)
@@ -301,38 +301,38 @@
 	jmp    115f6 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double) [clone .cold]+0xd0>
 	mov    -0x190(%rbp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    0xa4458(%rip),%rdi        
 	jne    1153a <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double) [clone .cold]+0x14>
 	jmp    11542 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double) [clone .cold]+0x1c>
 
-00000000000118db <_GLOBAL__sub_I_tmpxft_00000879_00000000_6_nms.compute_86.cudafe1.cpp.cold>:
-_GLOBAL__sub_I_tmpxft_00000879_00000000_6_nms.compute_86.cudafe1.cpp.cold():
+00000000000118db <_GLOBAL__sub_I_tmpxft_00000870_00000000_6_nms.compute_86.cudafe1.cpp.cold>:
+_GLOBAL__sub_I_tmpxft_00000870_00000000_6_nms.compute_86.cudafe1.cpp.cold():
 	mov    0x10(%rsp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    0xa443d(%rip),%rdi        
-	je     118f7 <_GLOBAL__sub_I_tmpxft_00000879_00000000_6_nms.compute_86.cudafe1.cpp.cold+0x1c>
+	je     118f7 <_GLOBAL__sub_I_tmpxft_00000870_00000000_6_nms.compute_86.cudafe1.cpp.cold+0x1c>
 	lea    0x6(%rsp),%rsi
 	call   1bcc0 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	mov    %rbp,%rdi
 	mov    %rbx,%rbp
 	call   10c80 <torch::CppFunction::~CppFunction()@plt>
-	jmp    11914 <_GLOBAL__sub_I_tmpxft_00000879_00000000_6_nms.compute_86.cudafe1.cpp.cold+0x39>
+	jmp    11914 <_GLOBAL__sub_I_tmpxft_00000870_00000000_6_nms.compute_86.cudafe1.cpp.cold+0x39>
 	mov    %r12,%rdi
 	call   11330 <c10::intrusive_ptr<c10::OperatorKernel, c10::detail::intrusive_target_default_null_type<c10::OperatorKernel> >::reset_()@plt>
 	lea    0xa5365(%rip),%rdi        
 	call   107b0 <torch::Library::~Library()@plt>
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
 
 0000000000011928 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>:
 std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]:
-	cmpq   $0x0,0xa44e8(%rip)        
+	cmpq   $0x0,0xa44f0(%rip)        
 	je     1193c <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x14>
 	or     $0xffffffff,%eax
 	lock xadd %eax,0x10(%rdi)
 	jmp    11945 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x1d>
 	mov    0x10(%rdi),%eax
 	lea    -0x1(%rax),%edx
 	mov    %edx,0x10(%rdi)
@@ -402,15 +402,15 @@
 	lea    0x12(%rsp),%rsi
 	call   11928 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>
 	jmp    11967 <_GLOBAL__sub_I_fp6_llm.cpp.cold+0x18>
 	nop
 
 0000000000011a3e <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>:
 std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]:
-	cmpq   $0x0,0xa43d2(%rip)        
+	cmpq   $0x0,0xa43da(%rip)        
 	je     11a52 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x14>
 	or     $0xffffffff,%eax
 	lock xadd %eax,0x10(%rdi)
 	jmp    11a5b <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x1d>
 	mov    0x10(%rdi),%eax
 	lea    -0x1(%rax),%edx
 	mov    %edx,0x10(%rdi)
@@ -539,15 +539,15 @@
 	push   %rax
 	call   10d60 <__cxa_allocate_exception@plt>
 	mov    %r12,%rsi
 	mov    %rax,%rdi
 	mov    %rax,%rbp
 	call   102e0 <std::runtime_error::runtime_error(char const*)@plt>
 	mov    0xa434f(%rip),%rdx        
-	mov    0xa41f8(%rip),%rsi        
+	mov    0xa4200(%rip),%rsi        
 	mov    %rbp,%rdi
 	call   105d0 <__cxa_throw@plt>
 	mov    %rax,%r12
 	mov    %rbp,%rdi
 	call   11130 <__cxa_free_exception@plt>
 	mov    %r12,%rdi
 	call   10650 <_Unwind_Resume@plt>
@@ -561,15 +561,15 @@
 	push   %rax
 	call   10d60 <__cxa_allocate_exception@plt>
 	mov    %r12,%rsi
 	mov    %rax,%rdi
 	mov    %rax,%rbp
 	call   10870 <std::runtime_error::runtime_error(std::string const&)@plt>
 	mov    0xa4307(%rip),%rdx        
-	mov    0xa41b0(%rip),%rsi        
+	mov    0xa41b8(%rip),%rsi        
 	mov    %rbp,%rdi
 	call   105d0 <__cxa_throw@plt>
 	mov    %rax,%r12
 	mov    %rbp,%rdi
 	call   11130 <__cxa_free_exception@plt>
 	mov    %r12,%rdi
 	call   10650 <_Unwind_Resume@plt>
@@ -592,15 +592,15 @@
 	call   11130 <__cxa_free_exception@plt>
 	mov    %r12,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	nop
 
 0000000000011ce6 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>:
 std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]:
-	cmpq   $0x0,0xa412a(%rip)        
+	cmpq   $0x0,0xa4132(%rip)        
 	je     11cfa <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x14>
 	or     $0xffffffff,%eax
 	lock xadd %eax,0x10(%rdi)
 	jmp    11d03 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x1d>
 	mov    0x10(%rdi),%eax
 	lea    -0x1(%rax),%edx
 	mov    %edx,0x10(%rdi)
@@ -648,49 +648,49 @@
 	xor    %r9d,%r9d
 	mov    $0xffffffff,%r8d
 	push   $0x0
 	lea    0x215e7(%rip),%rcx        
 	mov    %rax,%rdi
 	mov    %rax,%rbp
 	push   $0x0
-	mov    0xa4060(%rip),%rsi        # b5e10 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 8>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa01a0>
+	mov    0xa4068(%rip),%rsi        # b5e18 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 8>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa01a8>
 	mov    %rcx,%rdx
 	push   $0x0
 	mov    %rax,0xa4d64(%rip)        
 	call   110d0 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
 	mov    %rbp,%rdi
 	xor    %r9d,%r9d
 	push   $0x0
 	lea    0x2160c(%rip),%rcx        
-	mov    0xa3f9d(%rip),%rsi        # b5d78 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 4>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0248>
+	mov    0xa3fa5(%rip),%rsi        # b5d80 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 4>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0250>
 	mov    $0xffffffff,%r8d
 	push   $0x0
 	mov    %rcx,%rdx
 	push   $0x0
 	push   $0x0
 	call   110d0 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
 	mov    %rbp,%rdi
 	xor    %r9d,%r9d
 	push   $0x0
 	lea    0x21636(%rip),%rcx        
-	mov    0xa4097(%rip),%rsi        # b5ea0 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa04b0>
+	mov    0xa409f(%rip),%rsi        # b5ea8 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa04b8>
 	mov    $0xffffffff,%r8d
 	push   $0x0
 	mov    %rcx,%rdx
 	push   $0x0
 	push   $0x0
 	call   110d0 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
 	mov    %rbp,%rdi
 	xor    %r9d,%r9d
 	push   $0x0
 	lea    0x21660(%rip),%rcx        
-	mov    0xa3fb9(%rip),%rsi        # b5df0 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0540>
+	mov    0xa3fc1(%rip),%rsi        # b5df8 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0548>
 	mov    $0xffffffff,%r8d
 	push   $0x0
 	mov    %rcx,%rdx
 	push   $0x0
 	push   $0x0
 	call   110d0 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
@@ -706,27 +706,27 @@
 	push   $0x0
 	call   110d0 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
 	mov    %rbp,%rdi
 	xor    %r9d,%r9d
 	push   $0x0
 	lea    0x216b4(%rip),%rcx        
-	mov    0xa3fe5(%rip),%rsi        # b5e78 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 4>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9fe48>
+	mov    0xa3fed(%rip),%rsi        # b5e80 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 4>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9fe50>
 	mov    $0xffffffff,%r8d
 	push   $0x0
 	mov    %rcx,%rdx
 	push   $0x0
 	push   $0x0
 	call   110d0 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
 	mov    %rbp,%rdi
 	xor    %r9d,%r9d
 	push   $0x0
 	lea    0x216de(%rip),%rcx        
-	mov    0xa3f8f(%rip),%rsi        # b5e50 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9ff60>
+	mov    0xa3f97(%rip),%rsi        # b5e58 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9ff68>
 	mov    $0xffffffff,%r8d
 	push   $0x0
 	mov    %rcx,%rdx
 	push   $0x0
 	push   $0x0
 	call   110d0 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
@@ -742,15 +742,15 @@
 	push   $0x0
 	call   110d0 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
 	mov    %rbp,%rdi
 	xor    %r9d,%r9d
 	push   $0x0
 	lea    0x21732(%rip),%rcx        
-	mov    0xa3fc3(%rip),%rsi        
+	mov    0xa3fcb(%rip),%rsi        
 	mov    $0xffffffff,%r8d
 	push   $0x0
 	mov    %rcx,%rdx
 	push   $0x0
 	push   $0x0
 	call   110d0 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
@@ -768,16 +768,16 @@
 	pop    %rdx
 	call   10ed0 <__cudaRegisterFatBinaryEnd@plt>
 	lea    0x16a0(%rip),%rdi        
 	pop    %rbp
 	jmp    32c40 <atexit>
 	cs nopw 0x0(%rax,%rax,1)
 
-0000000000011f80 <_GLOBAL__sub_I_tmpxft_00000877_00000000_6_fp6_linear.compute_86.cudafe1.cpp>:
-_GLOBAL__sub_I_tmpxft_00000877_00000000_6_fp6_linear.compute_86.cudafe1.cpp():
+0000000000011f80 <_GLOBAL__sub_I_tmpxft_0000086e_00000000_6_fp6_linear.compute_86.cudafe1.cpp>:
+_GLOBAL__sub_I_tmpxft_0000086e_00000000_6_fp6_linear.compute_86.cudafe1.cpp():
 	push   %r12
 	lea    0xa4c17(%rip),%rdi        
 	push   %rbp
 	push   %rbx
 	sub    $0x60,%rsp
 	call   11260 <std::ios_base::Init::Init()@plt>
 	mov    0xa3fb5(%rip),%rdi        
@@ -802,31 +802,31 @@
 	lea    0x2131c(%rip),%r8        
 	lea    0xa4b3d(%rip),%rdi        
 	call   10640 <torch::Library::Library(torch::Library::Kind, std::string, std::optional<c10::DispatchKey>, char const*, unsigned int)@plt>
 	mov    0x10(%rsp),%rax
 	mov    0xa3d14(%rip),%rbx        
 	lea    -0x18(%rax),%rdi
 	cmp    %rbx,%rdi
-	jne    120e9 <_GLOBAL__sub_I_tmpxft_00000877_00000000_6_fp6_linear.compute_86.cudafe1.cpp+0x169>
+	jne    120e9 <_GLOBAL__sub_I_tmpxft_0000086e_00000000_6_fp6_linear.compute_86.cudafe1.cpp+0x169>
 	mov    $0x18,%edi
 	movb   $0x0,0x12(%rsp)
 	call   10b80 <operator new(unsigned long)@plt>
 	movq   $0x0,0x8(%rax)
 	mov    %rax,%rsi
 	lea    0x18(%rsp),%r12
-	mov    0xa3e91(%rip),%rax        # b5ed8 <vtable for c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >@@Base+0x828>
+	mov    0xa3e99(%rip),%rax        # b5ee0 <vtable for c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >@@Base+0x830>
 	mov    %r12,%rdi
 	add    $0x10,%rax
 	mov    %rax,(%rsi)
 	mov    0xa3f88(%rip),%rax        
 	mov    %rax,0x10(%rsi)
 	call   10260 <c10::intrusive_ptr<c10::OperatorKernel, c10::detail::intrusive_target_default_null_type<c10::OperatorKernel> >::intrusive_ptr(c10::OperatorKernel*)@plt>
 	lea    0x48(%rsp),%rdi
 	movb   $0x1,0x40(%rsp)
-	mov    0xa3c5e(%rip),%rax        # b5cd0 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x9cad0>
+	mov    0xa3c56(%rip),%rax        # b5cc8 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x9cac8>
 	movq   $0x0,0x30(%rsp)
 	mov    %rax,0x20(%rsp)
 	mov    0xa3f09(%rip),%rax        # b5f90 <c10::impl::wrap_kernel_functor_unboxed_<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >, at::Tensor (at::Tensor, at::Tensor, at::Tensor, long)>::call(c10::OperatorKernel*, c10::DispatchKeySet, at::Tensor, at::Tensor, at::Tensor, long)@@Base+0x9ea50>
 	mov    %rax,0x28(%rsp)
 	mov    0xa3d35(%rip),%rax        
 	mov    %rax,0x38(%rsp)
 	call   10fd0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long)>()@plt>
@@ -835,34 +835,34 @@
 	lea    0x216ae(%rip),%rsi        
 	mov    %rbp,%rdx
 	lea    0xa4a8c(%rip),%rdi        
 	mov    %rax,0x50(%rsp)
 	call   107d0 <torch::Library::_impl(char const*, torch::CppFunction&&, torch::_RegisterOrVerify) &@plt>
 	mov    %rbp,%rdi
 	call   10c80 <torch::CppFunction::~CppFunction()@plt>
-	mov    0xa3d8b(%rip),%rdi        
+	mov    0xa3d93(%rip),%rdi        
 	lea    0xa32a4(%rip),%rdx        
 	lea    0xa4a65(%rip),%rsi        
 	call   10740 <__cxa_atexit@plt>
 	add    $0x60,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	ret
 	lea    0x6(%rsp),%rsi
 	call   13850 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>
-	jmp    12021 <_GLOBAL__sub_I_tmpxft_00000877_00000000_6_fp6_linear.compute_86.cudafe1.cpp+0xa1>
+	jmp    12021 <_GLOBAL__sub_I_tmpxft_0000086e_00000000_6_fp6_linear.compute_86.cudafe1.cpp+0xa1>
 	mov    %rax,%rbp
-	jmp    113c0 <_GLOBAL__sub_I_tmpxft_00000877_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold+0x8>
+	jmp    113c0 <_GLOBAL__sub_I_tmpxft_0000086e_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold+0x8>
 	mov    %rax,%rbp
-	jmp    113d4 <_GLOBAL__sub_I_tmpxft_00000877_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold+0x1c>
+	jmp    113d4 <_GLOBAL__sub_I_tmpxft_0000086e_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold+0x1c>
 	mov    %rax,%rbx
-	jmp    113f8 <_GLOBAL__sub_I_tmpxft_00000877_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold+0x40>
+	jmp    113f8 <_GLOBAL__sub_I_tmpxft_0000086e_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold+0x40>
 	mov    %rax,%rbp
-	jmp    113b8 <_GLOBAL__sub_I_tmpxft_00000877_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold>
+	jmp    113b8 <_GLOBAL__sub_I_tmpxft_0000086e_00000000_6_fp6_linear.compute_86.cudafe1.cpp.cold>
 	nopl   0x0(%rax,%rax,1)
 
 0000000000012120 <__sti____cudaRegisterAll()>:
 __sti____cudaRegisterAll():
 	sub    $0x8,%rsp
 	lea    0xa4925(%rip),%rdi        
 	call   10400 <__cudaRegisterFatBinary@plt>
@@ -881,16 +881,16 @@
 	pop    %rdx
 	call   10ed0 <__cudaRegisterFatBinaryEnd@plt>
 	lea    0x73de(%rip),%rdi        
 	add    $0x8,%rsp
 	jmp    32c40 <atexit>
 	nopl   0x0(%rax,%rax,1)
 
-0000000000012180 <_GLOBAL__sub_I_tmpxft_00000878_00000000_6_weight_quant.compute_86.cudafe1.cpp>:
-_GLOBAL__sub_I_tmpxft_00000878_00000000_6_weight_quant.compute_86.cudafe1.cpp():
+0000000000012180 <_GLOBAL__sub_I_tmpxft_0000086f_00000000_6_weight_quant.compute_86.cudafe1.cpp>:
+_GLOBAL__sub_I_tmpxft_0000086f_00000000_6_weight_quant.compute_86.cudafe1.cpp():
 	push   %r15
 	lea    0xa4ab7(%rip),%rdi        
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
 	push   %rbx
@@ -919,26 +919,26 @@
 	lea    0x2287d(%rip),%r8        
 	lea    0xa49ce(%rip),%rdi        
 	call   10640 <torch::Library::Library(torch::Library::Kind, std::string, std::optional<c10::DispatchKey>, char const*, unsigned int)@plt>
 	mov    0xa0(%rsp),%rax
 	mov    0xa3b02(%rip),%rbx        
 	lea    -0x18(%rax),%rdi
 	cmp    %rbx,%rdi
-	jne    124c8 <_GLOBAL__sub_I_tmpxft_00000878_00000000_6_weight_quant.compute_86.cudafe1.cpp+0x348>
+	jne    124c8 <_GLOBAL__sub_I_tmpxft_0000086f_00000000_6_weight_quant.compute_86.cudafe1.cpp+0x348>
 	mov    $0x18,%edi
 	movb   $0x0,0x52(%rsp)
 	call   10b80 <operator new(unsigned long)@plt>
 	mov    %rax,%rsi
 	lea    0x58(%rsp),%r13
 	lea    0x30(%rsp),%r14
 	movq   $0x0,0x8(%rax)
 	mov    0xa3b8a(%rip),%rax        # b5de8 <vtable for c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >@@Base+0x6c0>
 	mov    %r13,%rdi
 	lea    0x20(%rsp),%r15
-	movq   0xa3bb2(%rip),%xmm0        # b5e20 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<at::Tensor>()@@Base+0xa06c0>
+	movq   0xa3bba(%rip),%xmm0        # b5e28 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<at::Tensor>()@@Base+0xa06c8>
 	add    $0x10,%rax
 	movhps 0xa3a6f(%rip),%xmm0        # b5ce8 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getFakeTypePtrCopy<at::Tensor>()@@Base+0xa0538>
 	mov    %rax,(%rsi)
 	mov    0xa3a8d(%rip),%rax        
 	movaps %xmm0,(%rsp)
 	mov    %rax,0x10(%rsi)
 	call   10260 <c10::intrusive_ptr<c10::OperatorKernel, c10::detail::intrusive_target_default_null_type<c10::OperatorKernel> >::intrusive_ptr(c10::OperatorKernel*)@plt>
@@ -950,15 +950,15 @@
 	mov    $0x1,%edx
 	mov    %r12,%rdi
 	movq   $0x0,0x70(%rsp)
 	mov    %rax,0x60(%rsp)
 	mov    0xa3afb(%rip),%rax        # b5dc0 <c10::impl::wrap_kernel_functor_unboxed_<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >, at::Tensor (at::Tensor)>::call(c10::OperatorKernel*, c10::DispatchKeySet, at::Tensor)@@Base+0x9ad20>
 	movb   $0x1,0x80(%rsp)
 	mov    %rax,0x68(%rsp)
-	mov    0xa3ba7(%rip),%rax        
+	mov    0xa3baf(%rip),%rax        
 	movaps %xmm0,0x20(%rsp)
 	mov    %rax,0x78(%rsp)
 	movaps %xmm0,0x30(%rsp)
 	call   10250 <c10::detail::infer_schema::make_function_schema(c10::ArrayRef<c10::detail::infer_schema::ArgumentDef>, c10::ArrayRef<c10::detail::infer_schema::ArgumentDef>)@plt>
 	mov    $0x48,%edi
 	call   10b80 <operator new(unsigned long)@plt>
 	movzwl 0xe0(%rsp),%edx
@@ -1033,45 +1033,45 @@
 	movups %xmm6,0x20(%rax)
 	movups %xmm7,0x30(%rax)
 	lea    0x18(%rbx),%rax
 	mov    %rax,0x90(%rsp)
 	call   107d0 <torch::Library::_impl(char const*, torch::CppFunction&&, torch::_RegisterOrVerify) &@plt>
 	mov    %rbp,%rdi
 	call   10c80 <torch::CppFunction::~CppFunction()@plt>
-	mov    0xa39b5(%rip),%rdi        
+	mov    0xa39bd(%rip),%rdi        
 	lea    0xa2ece(%rip),%rdx        
 	lea    0xa472f(%rip),%rsi        
 	call   10740 <__cxa_atexit@plt>
 	add    $0xf8,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	lea    0x30(%rsp),%rsi
 	call   19560 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>
-	jmp    12233 <_GLOBAL__sub_I_tmpxft_00000878_00000000_6_weight_quant.compute_86.cudafe1.cpp+0xb3>
+	jmp    12233 <_GLOBAL__sub_I_tmpxft_0000086f_00000000_6_weight_quant.compute_86.cudafe1.cpp+0xb3>
 	mov    %rax,%rbp
-	jmp    114bf <_GLOBAL__sub_I_tmpxft_00000878_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x10>
+	jmp    114bf <_GLOBAL__sub_I_tmpxft_0000086f_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x10>
 	mov    %rax,%rbp
-	jmp    114d3 <_GLOBAL__sub_I_tmpxft_00000878_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x24>
+	jmp    114d3 <_GLOBAL__sub_I_tmpxft_0000086f_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x24>
 	mov    %rax,%rbx
-	jmp    114fa <_GLOBAL__sub_I_tmpxft_00000878_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x4b>
+	jmp    114fa <_GLOBAL__sub_I_tmpxft_0000086f_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x4b>
 	mov    %rax,%rbp
-	jmp    11507 <_GLOBAL__sub_I_tmpxft_00000878_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x58>
+	jmp    11507 <_GLOBAL__sub_I_tmpxft_0000086f_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x58>
 	mov    %rax,%rbp
-	jmp    1150f <_GLOBAL__sub_I_tmpxft_00000878_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x60>
+	jmp    1150f <_GLOBAL__sub_I_tmpxft_0000086f_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x60>
 	mov    %rax,%rbx
-	jmp    11519 <_GLOBAL__sub_I_tmpxft_00000878_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x6a>
+	jmp    11519 <_GLOBAL__sub_I_tmpxft_0000086f_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x6a>
 	mov    %rax,%rbp
-	jmp    114af <_GLOBAL__sub_I_tmpxft_00000878_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold>
+	jmp    114af <_GLOBAL__sub_I_tmpxft_0000086f_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold>
 	mov    %rax,%rbp
-	jmp    114b7 <_GLOBAL__sub_I_tmpxft_00000878_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x8>
+	jmp    114b7 <_GLOBAL__sub_I_tmpxft_0000086f_00000000_6_weight_quant.compute_86.cudafe1.cpp.cold+0x8>
 	nopw   0x0(%rax,%rax,1)
 
 0000000000012520 <__sti____cudaRegisterAll()>:
 __sti____cudaRegisterAll():
 	push   %rbp
 	lea    0xa4540(%rip),%rdi        
 	call   10400 <__cudaRegisterFatBinary@plt>
@@ -1079,37 +1079,37 @@
 	xor    %r9d,%r9d
 	mov    $0xffffffff,%r8d
 	push   $0x0
 	lea    0x2314f(%rip),%rcx        
 	mov    %rax,%rdi
 	mov    %rax,%rbp
 	push   $0x0
-	mov    0xa3778(%rip),%rsi        # b5cc8 <void torchao::(anonymous namespace)::nms_kernel_impl<c10::Half>(int, double, c10::Half const*, unsigned long long*)@@Base+0x97708>
+	mov    0xa3790(%rip),%rsi        # b5ce0 <void torchao::(anonymous namespace)::nms_kernel_impl<c10::Half>(int, double, c10::Half const*, unsigned long long*)@@Base+0x97720>
 	mov    %rcx,%rdx
 	push   $0x0
 	mov    %rax,0xa4704(%rip)        
 	call   110d0 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
 	mov    %rbp,%rdi
 	xor    %r9d,%r9d
 	push   $0x0
 	lea    0x23184(%rip),%rcx        
-	mov    0xa3825(%rip),%rsi        # b5da0 <void torchao::(anonymous namespace)::nms_kernel_impl<float>(int, double, float const*, unsigned long long*)@@Base+0x978b0>
+	mov    0xa382d(%rip),%rsi        # b5da8 <void torchao::(anonymous namespace)::nms_kernel_impl<float>(int, double, float const*, unsigned long long*)@@Base+0x978b8>
 	mov    $0xffffffff,%r8d
 	push   $0x0
 	mov    %rcx,%rdx
 	push   $0x0
 	push   $0x0
 	call   110d0 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
 	mov    %rbp,%rdi
 	xor    %r9d,%r9d
 	push   $0x0
 	lea    0x231ae(%rip),%rcx        
-	mov    0xa37d7(%rip),%rsi        # b5d80 <void torchao::(anonymous namespace)::nms_kernel_impl<double>(int, double, double const*, unsigned long long*)@@Base+0x976f0>
+	mov    0xa3847(%rip),%rsi        # b5df0 <void torchao::(anonymous namespace)::nms_kernel_impl<double>(int, double, double const*, unsigned long long*)@@Base+0x97760>
 	mov    $0xffffffff,%r8d
 	push   $0x0
 	mov    %rcx,%rdx
 	push   $0x0
 	push   $0x0
 	call   110d0 <__cudaRegisterFunction@plt>
 	add    $0x20,%rsp
@@ -1128,16 +1128,16 @@
 	call   10ed0 <__cudaRegisterFatBinaryEnd@plt>
 	lea    0x96b4(%rip),%rdi        
 	pop    %rbp
 	jmp    32c40 <atexit>
 	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
-0000000000012610 <_GLOBAL__sub_I_tmpxft_00000879_00000000_6_nms.compute_86.cudafe1.cpp>:
-_GLOBAL__sub_I_tmpxft_00000879_00000000_6_nms.compute_86.cudafe1.cpp():
+0000000000012610 <_GLOBAL__sub_I_tmpxft_00000870_00000000_6_nms.compute_86.cudafe1.cpp>:
+_GLOBAL__sub_I_tmpxft_00000870_00000000_6_nms.compute_86.cudafe1.cpp():
 	push   %r12
 	lea    0xa46c7(%rip),%rdi        
 	push   %rbp
 	push   %rbx
 	sub    $0x60,%rsp
 	call   11260 <std::ios_base::Init::Init()@plt>
 	mov    0xa3925(%rip),%rdi        
@@ -1162,26 +1162,26 @@
 	lea    0x2329c(%rip),%r8        
 	lea    0xa45ed(%rip),%rdi        
 	call   10640 <torch::Library::Library(torch::Library::Kind, std::string, std::optional<c10::DispatchKey>, char const*, unsigned int)@plt>
 	mov    0x10(%rsp),%rax
 	mov    0xa3684(%rip),%rbx        
 	lea    -0x18(%rax),%rdi
 	cmp    %rbx,%rdi
-	jne    12779 <_GLOBAL__sub_I_tmpxft_00000879_00000000_6_nms.compute_86.cudafe1.cpp+0x169>
+	jne    12779 <_GLOBAL__sub_I_tmpxft_00000870_00000000_6_nms.compute_86.cudafe1.cpp+0x169>
 	mov    $0x18,%edi
 	movb   $0x0,0x12(%rsp)
 	call   10b80 <operator new(unsigned long)@plt>
 	movq   $0x0,0x8(%rax)
 	mov    %rax,%rsi
 	lea    0x18(%rsp),%r12
-	mov    0xa3819(%rip),%rax        # b5ef0 <vtable for c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >@@Base+0x620>
+	mov    0xa3821(%rip),%rax        # b5ef8 <vtable for c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >@@Base+0x628>
 	mov    %r12,%rdi
 	add    $0x10,%rax
 	mov    %rax,(%rsi)
-	mov    0xa3850(%rip),%rax        
+	mov    0xa3668(%rip),%rax        
 	mov    %rax,0x10(%rsi)
 	call   10260 <c10::intrusive_ptr<c10::OperatorKernel, c10::detail::intrusive_target_default_null_type<c10::OperatorKernel> >::intrusive_ptr(c10::OperatorKernel*)@plt>
 	lea    0x48(%rsp),%rdi
 	movb   $0x1,0x40(%rsp)
 	mov    0xa35f6(%rip),%rax        # b5cf8 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x92d78>
 	movq   $0x0,0x30(%rsp)
 	mov    %rax,0x20(%rsp)
@@ -1195,44 +1195,44 @@
 	lea    0x22ae9(%rip),%rsi        
 	mov    %rbp,%rdx
 	lea    0xa453c(%rip),%rdi        
 	mov    %rax,0x50(%rsp)
 	call   107d0 <torch::Library::_impl(char const*, torch::CppFunction&&, torch::_RegisterOrVerify) &@plt>
 	mov    %rbp,%rdi
 	call   10c80 <torch::CppFunction::~CppFunction()@plt>
-	mov    0xa36fb(%rip),%rdi        
+	mov    0xa3703(%rip),%rdi        
 	lea    0xa2c14(%rip),%rdx        
 	lea    0xa4515(%rip),%rsi        
 	call   10740 <__cxa_atexit@plt>
 	add    $0x60,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	ret
-	cmpq   $0x0,0xa3697(%rip)        
-	je     127a2 <_GLOBAL__sub_I_tmpxft_00000879_00000000_6_nms.compute_86.cudafe1.cpp+0x192>
+	cmpq   $0x0,0xa369f(%rip)        
+	je     127a2 <_GLOBAL__sub_I_tmpxft_00000870_00000000_6_nms.compute_86.cudafe1.cpp+0x192>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
-	jg     126b1 <_GLOBAL__sub_I_tmpxft_00000879_00000000_6_nms.compute_86.cudafe1.cpp+0xa1>
+	jg     126b1 <_GLOBAL__sub_I_tmpxft_00000870_00000000_6_nms.compute_86.cudafe1.cpp+0xa1>
 	lea    0x6(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
-	jmp    126b1 <_GLOBAL__sub_I_tmpxft_00000879_00000000_6_nms.compute_86.cudafe1.cpp+0xa1>
+	jmp    126b1 <_GLOBAL__sub_I_tmpxft_00000870_00000000_6_nms.compute_86.cudafe1.cpp+0xa1>
 	mov    -0x8(%rax),%edx
 	lea    -0x1(%rdx),%ecx
 	mov    %ecx,-0x8(%rax)
-	jmp    1278b <_GLOBAL__sub_I_tmpxft_00000879_00000000_6_nms.compute_86.cudafe1.cpp+0x17b>
+	jmp    1278b <_GLOBAL__sub_I_tmpxft_00000870_00000000_6_nms.compute_86.cudafe1.cpp+0x17b>
 	mov    %rax,%rbp
-	jmp    118db <_GLOBAL__sub_I_tmpxft_00000879_00000000_6_nms.compute_86.cudafe1.cpp.cold>
+	jmp    118db <_GLOBAL__sub_I_tmpxft_00000870_00000000_6_nms.compute_86.cudafe1.cpp.cold>
 	mov    %rax,%rbx
-	jmp    118ff <_GLOBAL__sub_I_tmpxft_00000879_00000000_6_nms.compute_86.cudafe1.cpp.cold+0x24>
+	jmp    118ff <_GLOBAL__sub_I_tmpxft_00000870_00000000_6_nms.compute_86.cudafe1.cpp.cold+0x24>
 	mov    %rax,%rbp
-	jmp    1190c <_GLOBAL__sub_I_tmpxft_00000879_00000000_6_nms.compute_86.cudafe1.cpp.cold+0x31>
+	jmp    1190c <_GLOBAL__sub_I_tmpxft_00000870_00000000_6_nms.compute_86.cudafe1.cpp.cold+0x31>
 	mov    %rax,%rbp
-	jmp    11914 <_GLOBAL__sub_I_tmpxft_00000879_00000000_6_nms.compute_86.cudafe1.cpp.cold+0x39>
+	jmp    11914 <_GLOBAL__sub_I_tmpxft_00000870_00000000_6_nms.compute_86.cudafe1.cpp.cold+0x39>
 	nopl   (%rax)
 
 00000000000127d0 <_GLOBAL__sub_I_fp6_llm.cpp>:
 _GLOBAL__sub_I_fp6_llm.cpp():
 	push   %r15
 	lea    0x20feb(%rip),%rsi        
 	push   %r14
@@ -1420,15 +1420,15 @@
 	lea    -0x18(%rax),%rdi
 	cmp    %rbx,%rdi
 	jne    12b73 <_GLOBAL__sub_I_fp6_llm.cpp+0x3a3>
 	mov    0x20(%rsp),%rdi
 	test   %rdi,%rdi
 	je     12b2b <_GLOBAL__sub_I_fp6_llm.cpp+0x35b>
 	call   10520 <operator delete(void*)@plt>
-	mov    0xa3326(%rip),%rdi        
+	mov    0xa332e(%rip),%rdi        
 	lea    0xa283f(%rip),%rdx        
 	lea    0xa41c0(%rip),%rsi        
 	call   10740 <__cxa_atexit@plt>
 	add    $0x98,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
@@ -1437,124 +1437,124 @@
 	pop    %r15
 	ret
 	movq   %rax,%xmm2
 	movb   $0x1,0xa41cd(%rip)        
 	punpcklqdq %xmm2,%xmm0
 	movaps %xmm0,0xa41b2(%rip)        
 	jmp    12875 <_GLOBAL__sub_I_fp6_llm.cpp+0xa5>
-	cmpq   $0x0,0xa329d(%rip)        
+	cmpq   $0x0,0xa32a5(%rip)        
 	je     12e42 <_GLOBAL__sub_I_fp6_llm.cpp+0x672>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     12b1c <_GLOBAL__sub_I_fp6_llm.cpp+0x34c>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    12b1c <_GLOBAL__sub_I_fp6_llm.cpp+0x34c>
-	cmpq   $0x0,0xa3279(%rip)        
+	cmpq   $0x0,0xa3281(%rip)        
 	je     12e34 <_GLOBAL__sub_I_fp6_llm.cpp+0x664>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	lea    0x18(%rsp),%r12
 	test   %edx,%edx
 	jg     12845 <_GLOBAL__sub_I_fp6_llm.cpp+0x75>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    12845 <_GLOBAL__sub_I_fp6_llm.cpp+0x75>
-	cmpq   $0x0,0xa3249(%rip)        
+	cmpq   $0x0,0xa3251(%rip)        
 	je     12e26 <_GLOBAL__sub_I_fp6_llm.cpp+0x656>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     128bb <_GLOBAL__sub_I_fp6_llm.cpp+0xeb>
 	lea    0x12(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    128bb <_GLOBAL__sub_I_fp6_llm.cpp+0xeb>
-	cmpq   $0x0,0xa321c(%rip)        
+	cmpq   $0x0,0xa3224(%rip)        
 	je     12dae <_GLOBAL__sub_I_fp6_llm.cpp+0x5de>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     12910 <_GLOBAL__sub_I_fp6_llm.cpp+0x140>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    12910 <_GLOBAL__sub_I_fp6_llm.cpp+0x140>
-	cmpq   $0x0,0xa31f1(%rip)        
+	cmpq   $0x0,0xa31f9(%rip)        
 	je     12da0 <_GLOBAL__sub_I_fp6_llm.cpp+0x5d0>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     12922 <_GLOBAL__sub_I_fp6_llm.cpp+0x152>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    12922 <_GLOBAL__sub_I_fp6_llm.cpp+0x152>
-	cmpq   $0x0,0xa31c6(%rip)        
+	cmpq   $0x0,0xa31ce(%rip)        
 	je     12e18 <_GLOBAL__sub_I_fp6_llm.cpp+0x648>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     12972 <_GLOBAL__sub_I_fp6_llm.cpp+0x1a2>
 	lea    0x12(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    12972 <_GLOBAL__sub_I_fp6_llm.cpp+0x1a2>
-	cmpq   $0x0,0xa3199(%rip)        
+	cmpq   $0x0,0xa31a1(%rip)        
 	je     12e0a <_GLOBAL__sub_I_fp6_llm.cpp+0x63a>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     129ba <_GLOBAL__sub_I_fp6_llm.cpp+0x1ea>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    129ba <_GLOBAL__sub_I_fp6_llm.cpp+0x1ea>
-	cmpq   $0x0,0xa316e(%rip)        
+	cmpq   $0x0,0xa3176(%rip)        
 	je     12dfc <_GLOBAL__sub_I_fp6_llm.cpp+0x62c>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     129cc <_GLOBAL__sub_I_fp6_llm.cpp+0x1fc>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    129cc <_GLOBAL__sub_I_fp6_llm.cpp+0x1fc>
-	cmpq   $0x0,0xa3143(%rip)        
+	cmpq   $0x0,0xa314b(%rip)        
 	je     12dee <_GLOBAL__sub_I_fp6_llm.cpp+0x61e>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     12a1c <_GLOBAL__sub_I_fp6_llm.cpp+0x24c>
 	lea    0x12(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    12a1c <_GLOBAL__sub_I_fp6_llm.cpp+0x24c>
-	cmpq   $0x0,0xa3116(%rip)        
+	cmpq   $0x0,0xa311e(%rip)        
 	je     12de0 <_GLOBAL__sub_I_fp6_llm.cpp+0x610>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     12a64 <_GLOBAL__sub_I_fp6_llm.cpp+0x294>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    12a64 <_GLOBAL__sub_I_fp6_llm.cpp+0x294>
-	cmpq   $0x0,0xa30eb(%rip)        
+	cmpq   $0x0,0xa30f3(%rip)        
 	je     12dd2 <_GLOBAL__sub_I_fp6_llm.cpp+0x602>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     12a76 <_GLOBAL__sub_I_fp6_llm.cpp+0x2a6>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    12a76 <_GLOBAL__sub_I_fp6_llm.cpp+0x2a6>
-	cmpq   $0x0,0xa30c0(%rip)        
+	cmpq   $0x0,0xa30c8(%rip)        
 	je     12dc7 <_GLOBAL__sub_I_fp6_llm.cpp+0x5f7>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     12ac6 <_GLOBAL__sub_I_fp6_llm.cpp+0x2f6>
 	lea    0x12(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    12ac6 <_GLOBAL__sub_I_fp6_llm.cpp+0x2f6>
-	cmpq   $0x0,0xa3097(%rip)        
+	cmpq   $0x0,0xa309f(%rip)        
 	je     12dbc <_GLOBAL__sub_I_fp6_llm.cpp+0x5ec>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     12b0e <_GLOBAL__sub_I_fp6_llm.cpp+0x33e>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -1674,46 +1674,46 @@
 	movq   $0x0,0x8(%rax)
 	mov    %rax,%rsi
 	lea    0x18(%rsp),%r12
 	mov    0xa2e87(%rip),%rax        # b5de8 <vtable for c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >@@Base+0x6c0>
 	mov    %r12,%rdi
 	add    $0x10,%rax
 	mov    %rax,(%rsi)
-	mov    0xa2e8e(%rip),%rax        
+	mov    0xa2e96(%rip),%rax        
 	mov    %rax,0x10(%rsi)
 	call   10260 <c10::intrusive_ptr<c10::OperatorKernel, c10::detail::intrusive_target_default_null_type<c10::OperatorKernel> >::intrusive_ptr(c10::OperatorKernel*)@plt>
 	lea    0x48(%rsp),%rdi
 	movb   $0x1,0x40(%rsp)
 	mov    0xa302c(%rip),%rax        # b5fb8 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x9a7d8>
 	movq   $0x0,0x30(%rsp)
 	mov    %rax,0x20(%rsp)
 	mov    0xa2e1f(%rip),%rax        # b5dc0 <c10::impl::wrap_kernel_functor_unboxed_<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >, at::Tensor (at::Tensor)>::call(c10::OperatorKernel*, c10::DispatchKeySet, at::Tensor)@@Base+0x9ad20>
 	mov    %rax,0x28(%rsp)
-	mov    0xa2ed3(%rip),%rax        
+	mov    0xa2edb(%rip),%rax        
 	mov    %rax,0x38(%rsp)
 	call   110f0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (*)(at::Tensor)>()@plt>
 	lea    0x18(%rbx),%rax
 	xor    %ecx,%ecx
 	lea    0x23546(%rip),%rsi        
 	mov    %rbp,%rdx
 	lea    0xa3d92(%rip),%rdi        
 	mov    %rax,0x50(%rsp)
 	call   107d0 <torch::Library::_impl(char const*, torch::CppFunction&&, torch::_RegisterOrVerify) &@plt>
 	mov    %rbp,%rdi
 	call   10c80 <torch::CppFunction::~CppFunction()@plt>
-	mov    0xa2e71(%rip),%rdi        
+	mov    0xa2e79(%rip),%rdi        
 	lea    0xa238a(%rip),%rdx        
 	lea    0xa3d6b(%rip),%rsi        
 	call   10740 <__cxa_atexit@plt>
 	add    $0x60,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	ret
-	cmpq   $0x0,0xa2e0d(%rip)        
+	cmpq   $0x0,0xa2e15(%rip)        
 	je     1302c <_GLOBAL__sub_I_weight_prepacking.cpp+0x16c>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     12f3b <_GLOBAL__sub_I_weight_prepacking.cpp+0x7b>
 	lea    0x6(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -1813,58 +1813,58 @@
 	lea    -0x18(%rax),%rdi
 	cmp    %rbx,%rdi
 	jne    1321c <_GLOBAL__sub_I_nms.cpp+0x18c>
 	mov    0x10(%rsp),%rdi
 	test   %rdi,%rdi
 	je     131d8 <_GLOBAL__sub_I_nms.cpp+0x148>
 	call   10520 <operator delete(void*)@plt>
-	mov    0xa2c79(%rip),%rdi        
+	mov    0xa2c81(%rip),%rdi        
 	lea    0xa2192(%rip),%rdx        
 	lea    0xa3c73(%rip),%rsi        
 	call   10740 <__cxa_atexit@plt>
 	add    $0x88,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	ret
 	movq   %rax,%xmm2
 	movb   $0x1,0xa3c84(%rip)        
 	punpcklqdq %xmm2,%xmm0
 	movaps %xmm0,0xa3c69(%rip)        
 	jmp    13131 <_GLOBAL__sub_I_nms.cpp+0xa1>
-	cmpq   $0x0,0xa2bf4(%rip)        
+	cmpq   $0x0,0xa2bfc(%rip)        
 	je     132c7 <_GLOBAL__sub_I_nms.cpp+0x237>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     131c9 <_GLOBAL__sub_I_nms.cpp+0x139>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    131c9 <_GLOBAL__sub_I_nms.cpp+0x139>
-	cmpq   $0x0,0xa2bd0(%rip)        
+	cmpq   $0x0,0xa2bd8(%rip)        
 	je     132bc <_GLOBAL__sub_I_nms.cpp+0x22c>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	lea    0x8(%rsp),%r12
 	test   %edx,%edx
 	jg     13101 <_GLOBAL__sub_I_nms.cpp+0x71>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    13101 <_GLOBAL__sub_I_nms.cpp+0x71>
-	cmpq   $0x0,0xa2ba4(%rip)        
+	cmpq   $0x0,0xa2bac(%rip)        
 	je     132e0 <_GLOBAL__sub_I_nms.cpp+0x250>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     13174 <_GLOBAL__sub_I_nms.cpp+0xe4>
 	lea    0x2(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    13174 <_GLOBAL__sub_I_nms.cpp+0xe4>
-	cmpq   $0x0,0xa2b7b(%rip)        
+	cmpq   $0x0,0xa2b83(%rip)        
 	je     132d5 <_GLOBAL__sub_I_nms.cpp+0x245>
 	or     $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     131bb <_GLOBAL__sub_I_nms.cpp+0x12b>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -1897,15 +1897,15 @@
 
 0000000000013310 <deregister_tm_clones>:
 deregister_tm_clones():
 	lea    0xa3721(%rip),%rdi        
 	lea    0xa371a(%rip),%rax        
 	cmp    %rdi,%rax
 	je     13338 <deregister_tm_clones+0x28>
-	mov    0xa2b86(%rip),%rax        
+	mov    0xa2b8e(%rip),%rax        
 	test   %rax,%rax
 	je     13338 <deregister_tm_clones+0x28>
 	jmp    *%rax
 	nopl   0x0(%rax)
 	ret
 	nopl   0x0(%rax)
 
@@ -1916,28 +1916,28 @@
 	sub    %rdi,%rsi
 	mov    %rsi,%rax
 	shr    $0x3f,%rsi
 	sar    $0x3,%rax
 	add    %rax,%rsi
 	sar    $1,%rsi
 	je     13378 <register_tm_clones+0x38>
-	mov    0xa2ad5(%rip),%rax        
+	mov    0xa2add(%rip),%rax        
 	test   %rax,%rax
 	je     13378 <register_tm_clones+0x38>
 	jmp    *%rax
 	nopw   0x0(%rax,%rax,1)
 	ret
 	nopl   0x0(%rax)
 
 0000000000013380 <__do_global_dtors_aux>:
 __do_global_dtors_aux():
 	cmpb   $0x0,0xa36f9(%rip)        
 	jne    133b8 <__do_global_dtors_aux+0x38>
 	push   %rbp
-	cmpq   $0x0,0xa2b2e(%rip)        
+	cmpq   $0x0,0xa2b36(%rip)        
 	mov    %rsp,%rbp
 	je     133a3 <__do_global_dtors_aux+0x23>
 	lea    0xa1fda(%rip),%rdi        
 	call   11388 <__cxa_finalize@plt>
 	call   13310 <deregister_tm_clones>
 	movb   $0x1,0xa36d1(%rip)        
 	pop    %rbp
@@ -1967,15 +1967,15 @@
 	push   %rbx
 	mov    %r9,%rbx
 	sub    $0xe8,%rsp
 	movzbl 0xa36a6(%rip),%eax        # b6aa0 <guard variable for Kernel_Ex<TilingConfig<4, 1, 8>, float>(CUstream_st*, uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	test   %al,%al
 	je     13488 <void Kernel_Ex<TilingConfig<4, 1, 8>, float>(CUstream_st*, uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)+0xb8>
 	mov    0xa36a0(%rip),%edx        # b6aa8 <Kernel_Ex<TilingConfig<4, 1, 8>, float>(CUstream_st*, uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
-	mov    0xa2a01(%rip),%rdi        # b5e10 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 8>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa01a0>
+	mov    0xa2a09(%rip),%rdi        # b5e18 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 8>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa01a8>
 	mov    $0x8,%esi
 	call   10a90 <cudaFuncSetAttribute@plt>
 	mov    0x120(%rsp),%rax
 	mov    %rbp,%r9
 	mov    0xa367d(%rip),%r8        # b6aa8 <Kernel_Ex<TilingConfig<4, 1, 8>, float>(CUstream_st*, uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	movabs $0x100000080,%rdx
 	mov    $0x1,%ecx
@@ -2054,15 +2054,15 @@
 	mov    %rax,0x70(%rsp)
 	mov    %rax,0x7c(%rsp)
 	movaps %xmm0,0xd0(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    13471 <void Kernel_Ex<TilingConfig<4, 1, 8>, float>(CUstream_st*, uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)+0xa1>
 	push   0x50(%rsp)
-	mov    0xa283f(%rip),%rdi        # b5e10 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 8>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa01a0>
+	mov    0xa2847(%rip),%rdi        # b5e18 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 8>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa01a8>
 	push   0x50(%rsp)
 	mov    0x8c(%rsp),%rcx
 	mov    0x94(%rsp),%r8d
 	mov    0x80(%rsp),%rsi
 	mov    0x88(%rsp),%edx
 	lea    0xb0(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -2192,15 +2192,15 @@
 	pop    %rdx
 	jmp    136b8 <void Kernel_Ex<TilingConfig<4, 1, 8>, __half>(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int) [clone .constprop.0]+0x98>
 	nop
 	cs nopw 0x0(%rax,%rax,1)
 
 0000000000013850 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>:
 std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]:
-	cmpq   $0x0,0xa25c0(%rip)        
+	cmpq   $0x0,0xa25c8(%rip)        
 	je     13870 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x20>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x10(%rdi)
 	test   %eax,%eax
 	jle    1387d <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x2d>
 	ret
 	nopl   0x0(%rax)
@@ -2244,15 +2244,15 @@
 	mov    %rax,0x4c(%rsp)
 	movl   $0x1,0x54(%rsp)
 	movaps %xmm0,0x80(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    1396c <__device_stub__Z16SplitK_ReductionP6__halfPfmmi(__half*, float*, unsigned long, unsigned long, int)+0xdc>
 	push   0x38(%rsp)
-	mov    0xa259a(%rip),%rdi        
+	mov    0xa25a2(%rip),%rdi        
 	push   0x38(%rsp)
 	mov    0x5c(%rsp),%rcx
 	mov    0x64(%rsp),%r8d
 	mov    0x50(%rsp),%rsi
 	mov    0x58(%rsp),%edx
 	lea    0x80(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -2359,15 +2359,15 @@
 	jne    13ef0 <fp6_linear_kernel(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, float*, int)+0x560>
 	movzbl 0xa2f83(%rip),%eax        # b6ab0 <guard variable for Kernel_Ex<TilingConfig<4, 1, 4>, float>(CUstream_st*, uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	test   %al,%al
 	je     14368 <fp6_linear_kernel(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, float*, int)+0x9d8>
 	mov    0xa2f7d(%rip),%edx        # b6ab8 <Kernel_Ex<TilingConfig<4, 1, 4>, float>(CUstream_st*, uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	mov    $0x8,%esi
 	mov    %r11,0x8(%rsp)
-	mov    0xa222c(%rip),%rdi        # b5d78 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 4>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0248>
+	mov    0xa2234(%rip),%rdi        # b5d80 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 4>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0250>
 	call   10a90 <cudaFuncSetAttribute@plt>
 	mov    (%rsp),%rax
 	mov    %rbp,%r9
 	mov    0xa2f59(%rip),%r8        # b6ab8 <Kernel_Ex<TilingConfig<4, 1, 4>, float>(CUstream_st*, uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	movabs $0x100000080,%rdx
 	mov    $0x1,%ecx
 	mov    $0x1,%esi
@@ -2427,15 +2427,15 @@
 	mov    %rax,0x80(%rsp)
 	mov    %rax,0x8c(%rsp)
 	movaps %xmm0,0xe0(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    13a41 <fp6_linear_kernel(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, float*, int)+0xb1>
 	push   0x60(%rsp)
-	mov    0xa20ae(%rip),%rdi        # b5d78 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 4>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0248>
+	mov    0xa20b6(%rip),%rdi        # b5d80 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 4>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0250>
 	push   0x60(%rsp)
 	mov    0x9c(%rsp),%rcx
 	mov    0xa4(%rsp),%r8d
 	mov    0x90(%rsp),%rsi
 	mov    0x98(%rsp),%edx
 	lea    0xc0(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -2447,15 +2447,15 @@
 	jne    13efd <fp6_linear_kernel(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, float*, int)+0x56d>
 	movzbl 0xa2db7(%rip),%eax        # b6ad0 <guard variable for Kernel_Ex<TilingConfig<4, 1, 1>, float>(CUstream_st*, uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	test   %al,%al
 	je     143b0 <fp6_linear_kernel(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, float*, int)+0xa20>
 	mov    0xa2db1(%rip),%edx        # b6ad8 <Kernel_Ex<TilingConfig<4, 1, 1>, float>(CUstream_st*, uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	mov    $0x8,%esi
 	mov    %r11,0x8(%rsp)
-	mov    0xa20b8(%rip),%rdi        # b5df0 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0540>
+	mov    0xa20c0(%rip),%rdi        # b5df8 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0548>
 	call   10a90 <cudaFuncSetAttribute@plt>
 	mov    (%rsp),%rax
 	mov    %rbp,%r9
 	mov    0xa2d8d(%rip),%r8        # b6ad8 <Kernel_Ex<TilingConfig<4, 1, 1>, float>(CUstream_st*, uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	movabs $0x100000080,%rdx
 	mov    $0x1,%ecx
 	mov    $0x1,%esi
@@ -2515,15 +2515,15 @@
 	mov    %rax,0x80(%rsp)
 	mov    %rax,0x8c(%rsp)
 	movaps %xmm0,0xe0(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    13a41 <fp6_linear_kernel(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, float*, int)+0xb1>
 	push   0x60(%rsp)
-	mov    0xa1f3a(%rip),%rdi        # b5df0 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0540>
+	mov    0xa1f42(%rip),%rdi        # b5df8 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0548>
 	push   0x60(%rsp)
 	mov    0x9c(%rsp),%rcx
 	mov    0xa4(%rsp),%r8d
 	mov    0x90(%rsp),%rsi
 	mov    0x98(%rsp),%edx
 	lea    0xc0(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -2555,15 +2555,15 @@
 	jne    13b12 <fp6_linear_kernel(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, float*, int)+0x182>
 	movzbl 0xa2b59(%rip),%eax        # b6ac0 <guard variable for Kernel_Ex<TilingConfig<4, 1, 2>, float>(CUstream_st*, uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	test   %al,%al
 	je     147e0 <fp6_linear_kernel(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, float*, int)+0xe50>
 	mov    0xa2b53(%rip),%edx        # b6ac8 <Kernel_Ex<TilingConfig<4, 1, 2>, float>(CUstream_st*, uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	mov    $0x8,%esi
 	mov    %r11,0x8(%rsp)
-	mov    0xa1f1a(%rip),%rdi        # b5ea0 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa04b0>
+	mov    0xa1f22(%rip),%rdi        # b5ea8 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa04b8>
 	call   10a90 <cudaFuncSetAttribute@plt>
 	mov    (%rsp),%rax
 	mov    %rbp,%r9
 	mov    0xa2b2f(%rip),%r8        # b6ac8 <Kernel_Ex<TilingConfig<4, 1, 2>, float>(CUstream_st*, uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	movabs $0x100000080,%rdx
 	mov    $0x1,%ecx
 	mov    $0x1,%esi
@@ -2623,15 +2623,15 @@
 	mov    %rax,0x80(%rsp)
 	mov    %rax,0x8c(%rsp)
 	movaps %xmm0,0xe0(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    13a41 <fp6_linear_kernel(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, float*, int)+0xb1>
 	push   0x60(%rsp)
-	mov    0xa1d9c(%rip),%rdi        # b5ea0 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa04b0>
+	mov    0xa1da4(%rip),%rdi        # b5ea8 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa04b8>
 	push   0x60(%rsp)
 	mov    0x9c(%rsp),%rcx
 	mov    0xa4(%rsp),%r8d
 	mov    0x90(%rsp),%rsi
 	mov    0x98(%rsp),%edx
 	lea    0xc0(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -2645,15 +2645,15 @@
 	jne    14320 <fp6_linear_kernel(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, float*, int)+0x990>
 	movzbl 0xa2995(%rip),%eax        # b6af0 <guard variable for Kernel_Ex<TilingConfig<4, 1, 4>, __half>(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	test   %al,%al
 	je     143f0 <fp6_linear_kernel(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, float*, int)+0xa60>
 	mov    0xa298f(%rip),%edx        # b6af8 <Kernel_Ex<TilingConfig<4, 1, 4>, __half>(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	mov    $0x8,%esi
 	mov    %r11,0x8(%rsp)
-	mov    0xa1cfe(%rip),%rdi        # b5e78 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 4>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9fe48>
+	mov    0xa1d06(%rip),%rdi        # b5e80 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 4>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9fe50>
 	call   10a90 <cudaFuncSetAttribute@plt>
 	mov    (%rsp),%rax
 	mov    %rbp,%r9
 	mov    0xa296b(%rip),%r8        # b6af8 <Kernel_Ex<TilingConfig<4, 1, 4>, __half>(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	movabs $0x100000080,%rdx
 	mov    $0x1,%ecx
 	mov    $0x1,%esi
@@ -2710,15 +2710,15 @@
 	mov    %rax,0x80(%rsp)
 	mov    %rax,0x8c(%rsp)
 	movaps %xmm0,0xe0(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    13aa9 <fp6_linear_kernel(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, float*, int)+0x119>
 	push   0x60(%rsp)
-	mov    0xa1b94(%rip),%rdi        # b5e78 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 4>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9fe48>
+	mov    0xa1b9c(%rip),%rdi        # b5e80 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 4>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9fe50>
 	push   0x60(%rsp)
 	mov    0x9c(%rsp),%rcx
 	mov    0xa4(%rsp),%r8d
 	mov    0x90(%rsp),%rsi
 	mov    0x98(%rsp),%edx
 	lea    0xc0(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -2784,15 +2784,15 @@
 	jne    14602 <fp6_linear_kernel(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, float*, int)+0xc72>
 	movzbl 0xa26bf(%rip),%eax        # b6b00 <guard variable for Kernel_Ex<TilingConfig<4, 1, 2>, __half>(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	test   %al,%al
 	je     14820 <fp6_linear_kernel(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, float*, int)+0xe90>
 	mov    0xa26b9(%rip),%edx        # b6b08 <Kernel_Ex<TilingConfig<4, 1, 2>, __half>(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	mov    $0x8,%esi
 	mov    %r11,0x8(%rsp)
-	mov    0xa19f0(%rip),%rdi        # b5e50 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9ff60>
+	mov    0xa19f8(%rip),%rdi        # b5e58 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9ff68>
 	call   10a90 <cudaFuncSetAttribute@plt>
 	mov    (%rsp),%rax
 	mov    %rbp,%r9
 	mov    0xa2695(%rip),%r8        # b6b08 <Kernel_Ex<TilingConfig<4, 1, 2>, __half>(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)::SHMEM_SZ>
 	movabs $0x100000080,%rdx
 	mov    $0x1,%ecx
 	mov    $0x1,%esi
@@ -2849,15 +2849,15 @@
 	mov    %rax,0x80(%rsp)
 	mov    %rax,0x8c(%rsp)
 	movaps %xmm0,0xe0(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    13aa9 <fp6_linear_kernel(CUstream_st*, uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, float*, int)+0x119>
 	push   0x60(%rsp)
-	mov    0xa1886(%rip),%rdi        # b5e50 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9ff60>
+	mov    0xa188e(%rip),%rdi        # b5e58 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9ff68>
 	push   0x60(%rsp)
 	mov    0x9c(%rsp),%rcx
 	mov    0xa4(%rsp),%r8d
 	mov    0x90(%rsp),%rsi
 	mov    0x98(%rsp),%edx
 	lea    0xc0(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -3913,15 +3913,15 @@
 	push   %r12
 	mov    %rdi,%r12
 	call   10410 <c10::TensorType::get()@plt>
 	movq   (%rax),%xmm0
 	mov    0x8(%rax),%rax
 	test   %rax,%rax
 	je     15786 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<at::Tensor>()+0x26>
-	cmpq   $0x0,0xa0699(%rip)        
+	cmpq   $0x0,0xa06a1(%rip)        
 	je     157a0 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<at::Tensor>()+0x40>
 	lock addl $0x1,0x8(%rax)
 	movq   %rax,%xmm1
 	mov    %r12,%rax
 	punpcklqdq %xmm1,%xmm0
 	movups %xmm0,(%r12)
 	pop    %r12
@@ -3936,15 +3936,15 @@
 	push   %r12
 	mov    %rdi,%r12
 	call   10410 <c10::TensorType::get()@plt>
 	movq   (%rax),%xmm0
 	mov    0x8(%rax),%rax
 	test   %rax,%rax
 	je     157d6 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getFakeTypePtrCopy<at::Tensor>()+0x26>
-	cmpq   $0x0,0xa0649(%rip)        
+	cmpq   $0x0,0xa0651(%rip)        
 	je     157f0 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getFakeTypePtrCopy<at::Tensor>()+0x40>
 	lock addl $0x1,0x8(%rax)
 	movq   %rax,%xmm1
 	mov    %r12,%rax
 	punpcklqdq %xmm1,%xmm0
 	movups %xmm0,(%r12)
 	pop    %r12
@@ -4055,15 +4055,15 @@
 	mov    %rax,0x50(%rsp)
 	mov    %rax,0x5c(%rsp)
 	movaps %xmm0,0xb0(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    159df <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)+0x12f>
 	push   0x48(%rsp)
-	mov    0xa0437(%rip),%rdi        # b5df0 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0540>
+	mov    0xa043f(%rip),%rdi        # b5df8 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 1>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0548>
 	push   0x48(%rsp)
 	mov    0x6c(%rsp),%rcx
 	mov    0x74(%rsp),%r8d
 	mov    0x60(%rsp),%rsi
 	mov    0x68(%rsp),%edx
 	lea    0x90(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -4119,15 +4119,15 @@
 	mov    %rax,0x50(%rsp)
 	mov    %rax,0x5c(%rsp)
 	movaps %xmm0,0xb0(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    15b1f <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)+0x12f>
 	push   0x48(%rsp)
-	mov    0xa03a7(%rip),%rdi        # b5ea0 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa04b0>
+	mov    0xa03af(%rip),%rdi        # b5ea8 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa04b8>
 	push   0x48(%rsp)
 	mov    0x6c(%rsp),%rcx
 	mov    0x74(%rsp),%r8d
 	mov    0x60(%rsp),%rsi
 	mov    0x68(%rsp),%edx
 	lea    0x90(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -4183,15 +4183,15 @@
 	mov    %rax,0x50(%rsp)
 	mov    %rax,0x5c(%rsp)
 	movaps %xmm0,0xb0(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    15c5f <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 4>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)+0x12f>
 	push   0x48(%rsp)
-	mov    0xa013f(%rip),%rdi        # b5d78 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 4>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0248>
+	mov    0xa0147(%rip),%rdi        # b5d80 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 4>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa0250>
 	push   0x48(%rsp)
 	mov    0x6c(%rsp),%rcx
 	mov    0x74(%rsp),%r8d
 	mov    0x60(%rsp),%rsi
 	mov    0x68(%rsp),%edx
 	lea    0x90(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -4247,15 +4247,15 @@
 	mov    %rax,0x50(%rsp)
 	mov    %rax,0x5c(%rsp)
 	movaps %xmm0,0xb0(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    15d9f <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 8>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)+0x12f>
 	push   0x48(%rsp)
-	mov    0xa0097(%rip),%rdi        # b5e10 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 8>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa01a0>
+	mov    0xa009f(%rip),%rdi        # b5e18 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 8>, float>(uint4 const*, __half const*, __half const*, float*, unsigned long, unsigned long, unsigned long, int)@@Base+0xa01a8>
 	push   0x48(%rsp)
 	mov    0x6c(%rsp),%rcx
 	mov    0x74(%rsp),%r8d
 	mov    0x60(%rsp),%rsi
 	mov    0x68(%rsp),%edx
 	lea    0x90(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -4375,15 +4375,15 @@
 	mov    %rax,0x50(%rsp)
 	mov    %rax,0x5c(%rsp)
 	movaps %xmm0,0xb0(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    1601f <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)+0x12f>
 	push   0x48(%rsp)
-	mov    0x9fe57(%rip),%rdi        # b5e50 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9ff60>
+	mov    0x9fe5f(%rip),%rdi        # b5e58 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 2>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9ff68>
 	push   0x48(%rsp)
 	mov    0x6c(%rsp),%rcx
 	mov    0x74(%rsp),%r8d
 	mov    0x60(%rsp),%rsi
 	mov    0x68(%rsp),%edx
 	lea    0x90(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -4439,15 +4439,15 @@
 	mov    %rax,0x50(%rsp)
 	mov    %rax,0x5c(%rsp)
 	movaps %xmm0,0xb0(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    1615f <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 4>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)+0x12f>
 	push   0x48(%rsp)
-	mov    0x9fd3f(%rip),%rdi        # b5e78 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 4>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9fe48>
+	mov    0x9fd47(%rip),%rdi        # b5e80 <void QUANT_GEMM_Kernel<TilingConfig<4, 1, 4>, __half>(uint4 const*, __half const*, __half const*, __half*, unsigned long, unsigned long, unsigned long, int)@@Base+0x9fe50>
 	push   0x48(%rsp)
 	mov    0x6c(%rsp),%rcx
 	mov    0x74(%rsp),%r8d
 	mov    0x60(%rsp),%rsi
 	mov    0x68(%rsp),%edx
 	lea    0x90(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -4889,34 +4889,34 @@
 	call   108b0 <std::basic_ostream<char, std::char_traits<char> >& std::__ostream_insert<char, std::char_traits<char> >(std::basic_ostream<char, std::char_traits<char> >&, char const*, long)@plt>
 	mov    (%rbx),%esi
 	mov    %rbp,%rdi
 	call   10ca0 <std::ostream::operator<<(int)@plt>
 	lea    0x18(%rsp),%rsi
 	mov    %r12,%rdi
 	call   10e30 <std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >::str() const@plt>
-	mov    0x9f494(%rip),%rax        # b5d68 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x9f49c(%rip),%rax        # b5d70 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	lea    0x40(%rax),%rdx
 	add    $0x18,%rax
 	movq   %rax,%xmm0
-	mov    0x9f5d0(%rip),%rax        # b5eb8 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x9f5d8(%rip),%rax        # b5ec0 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	mov    %rdx,0x68(%rsp)
 	add    $0x10,%rax
 	movq   %rax,%xmm1
 	mov    0x60(%rsp),%rax
 	punpcklqdq %xmm1,%xmm0
 	lea    -0x18(%rax),%rdi
 	cmp    0x9f41e(%rip),%rdi        
 	movaps %xmm0,0x10(%rsp)
 	jne    169a0 <c10::detail::_str_wrapper<char const*, int const&>::call(char const* const&, int const&)+0x130>
 	mov    0x9f68c(%rip),%rax        # b5fa8 <vtable for std::basic_streambuf<char, std::char_traits<char> >@GLIBCXX_3.4>
 	lea    0x50(%rsp),%rdi
 	add    $0x10,%rax
 	mov    %rax,0x18(%rsp)
 	call   11230 <std::locale::~locale()@plt>
-	mov    0x9f52a(%rip),%rax        # b5e60 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x9f532(%rip),%rax        # b5e68 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	lea    0x68(%rsp),%rdi
 	mov    0x8(%rax),%rdx
 	mov    0x10(%rax),%rax
 	mov    %rdx,0x10(%rsp)
 	mov    -0x18(%rdx),%rdx
 	mov    %rax,0x10(%rsp,%rdx,1)
 	mov    0x9f678(%rip),%rax        # b5fd0 <vtable for std::basic_ios<char, std::char_traits<char> >@GLIBCXX_3.4>
@@ -5238,34 +5238,34 @@
 	call   108b0 <std::basic_ostream<char, std::char_traits<char> >& std::__ostream_insert<char, std::char_traits<char> >(std::basic_ostream<char, std::char_traits<char> >&, char const*, long)@plt>
 	mov    (%rbx),%esi
 	mov    %rbp,%rdi
 	call   104c0 <std::ostream& std::ostream::_M_insert<unsigned long>(unsigned long)@plt>
 	lea    0x18(%rsp),%rsi
 	mov    %r12,%rdi
 	call   10e30 <std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >::str() const@plt>
-	mov    0x9ef44(%rip),%rax        # b5d68 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x9ef4c(%rip),%rax        # b5d70 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	lea    0x40(%rax),%rdx
 	add    $0x18,%rax
 	movq   %rax,%xmm0
-	mov    0x9f080(%rip),%rax        # b5eb8 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x9f088(%rip),%rax        # b5ec0 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	mov    %rdx,0x68(%rsp)
 	add    $0x10,%rax
 	movq   %rax,%xmm1
 	mov    0x60(%rsp),%rax
 	punpcklqdq %xmm1,%xmm0
 	lea    -0x18(%rax),%rdi
 	cmp    0x9eece(%rip),%rdi        
 	movaps %xmm0,0x10(%rsp)
 	jne    16ef0 <c10::detail::_str_wrapper<char const*, unsigned int const&>::call(char const* const&, unsigned int const&)+0x130>
 	mov    0x9f13c(%rip),%rax        # b5fa8 <vtable for std::basic_streambuf<char, std::char_traits<char> >@GLIBCXX_3.4>
 	lea    0x50(%rsp),%rdi
 	add    $0x10,%rax
 	mov    %rax,0x18(%rsp)
 	call   11230 <std::locale::~locale()@plt>
-	mov    0x9efda(%rip),%rax        # b5e60 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x9efe2(%rip),%rax        # b5e68 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	lea    0x68(%rsp),%rdi
 	mov    0x8(%rax),%rdx
 	mov    0x10(%rax),%rax
 	mov    %rdx,0x10(%rsp)
 	mov    -0x18(%rdx),%rdx
 	mov    %rax,0x10(%rsp,%rdx,1)
 	mov    0x9f128(%rip),%rax        # b5fd0 <vtable for std::basic_ios<char, std::char_traits<char> >@GLIBCXX_3.4>
@@ -5299,15 +5299,15 @@
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   0x0(%rax)
 
 0000000000016f20 <c10::intrusive_ptr_target::~intrusive_ptr_target()>:
 :intrusive_ptr_target::~intrusive_ptr_target():
 	push   %rbx
 	sub    $0x20,%rsp
-	mov    0x9eff4(%rip),%rax        
+	mov    0x9effc(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	mov    0x8(%rdi),%eax
 	test   %eax,%eax
 	je     16f44 <c10::intrusive_ptr_target::~intrusive_ptr_target()+0x24>
 	mov    0x8(%rdi),%eax
 	cmp    $0xffffffe,%eax
@@ -5361,72 +5361,72 @@
 	mov    $0x10,%esi
 	pop    %rbp
 	jmp    10de0 <operator delete(void*, unsigned long)@plt>
 	nopw   0x0(%rax,%rax,1)
 
 0000000000017010 <c10::VariableVersion::VersionCounter::~VersionCounter()>:
 :VariableVersion::VersionCounter::~VersionCounter():
-	mov    0x9ed91(%rip),%rax        
+	mov    0x9ed89(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	jmp    11080 <c10::intrusive_ptr_target::~intrusive_ptr_target()@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
 0000000000017030 <c10::VariableVersion::VersionCounter::~VersionCounter()>:
 :VariableVersion::VersionCounter::~VersionCounter():
-	mov    0x9ed71(%rip),%rax        
+	mov    0x9ed69(%rip),%rax        
 	push   %rbp
 	mov    %rdi,%rbp
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	call   11080 <c10::intrusive_ptr_target::~intrusive_ptr_target()@plt>
 	mov    %rbp,%rdi
 	mov    $0x18,%esi
 	pop    %rbp
 	jmp    10de0 <operator delete(void*, unsigned long)@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	nop
 
 0000000000017060 <c10::OperatorKernel::~OperatorKernel()>:
 :OperatorKernel::~OperatorKernel():
-	mov    0x9eda1(%rip),%rax        
+	mov    0x9eda9(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	jmp    11080 <c10::intrusive_ptr_target::~intrusive_ptr_target()@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
 0000000000017080 <c10::OperatorKernel::~OperatorKernel()>:
 :OperatorKernel::~OperatorKernel():
-	mov    0x9ed81(%rip),%rax        
+	mov    0x9ed89(%rip),%rax        
 	push   %rbp
 	mov    %rdi,%rbp
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	call   11080 <c10::intrusive_ptr_target::~intrusive_ptr_target()@plt>
 	mov    %rbp,%rdi
 	mov    $0x10,%esi
 	pop    %rbp
 	jmp    10de0 <operator delete(void*, unsigned long)@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	nop
 
 00000000000170b0 <c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >::~WrapFunctionIntoRuntimeFunctor_()>:
 :impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >::~WrapFunctionIntoRuntimeFunctor_():
-	mov    0x9ed51(%rip),%rax        
+	mov    0x9ed59(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	jmp    11080 <c10::intrusive_ptr_target::~intrusive_ptr_target()@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
 00000000000170d0 <c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >::~WrapFunctionIntoRuntimeFunctor_()>:
 :impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor, at::Tensor, long> >::~WrapFunctionIntoRuntimeFunctor_():
-	mov    0x9ed31(%rip),%rax        
+	mov    0x9ed39(%rip),%rax        
 	push   %rbp
 	mov    %rdi,%rbp
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	call   11080 <c10::intrusive_ptr_target::~intrusive_ptr_target()@plt>
 	mov    %rbp,%rdi
 	mov    $0x18,%esi
@@ -5484,34 +5484,34 @@
 	mov    (%rbx),%rsi
 	mov    %rbp,%rdi
 	mov    -0x18(%rsi),%rdx
 	call   108b0 <std::basic_ostream<char, std::char_traits<char> >& std::__ostream_insert<char, std::char_traits<char> >(std::basic_ostream<char, std::char_traits<char> >&, char const*, long)@plt>
 	lea    0x18(%rsp),%rsi
 	mov    %r12,%rdi
 	call   10e30 <std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >::str() const@plt>
-	mov    0x9ebaf(%rip),%rax        # b5d68 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x9ebb7(%rip),%rax        # b5d70 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	lea    0x40(%rax),%rdx
 	add    $0x18,%rax
 	movq   %rax,%xmm0
-	mov    0x9eceb(%rip),%rax        # b5eb8 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x9ecf3(%rip),%rax        # b5ec0 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	mov    %rdx,0x68(%rsp)
 	add    $0x10,%rax
 	movq   %rax,%xmm1
 	mov    0x60(%rsp),%rax
 	punpcklqdq %xmm1,%xmm0
 	lea    -0x18(%rax),%rdi
 	cmp    0x9eb39(%rip),%rdi        
 	movaps %xmm0,0x10(%rsp)
 	jne    17280 <c10::detail::_str_wrapper<char const*, std::string const&>::call(char const* const&, std::string const&)+0x130>
 	mov    0x9eda7(%rip),%rax        # b5fa8 <vtable for std::basic_streambuf<char, std::char_traits<char> >@GLIBCXX_3.4>
 	lea    0x50(%rsp),%rdi
 	add    $0x10,%rax
 	mov    %rax,0x18(%rsp)
 	call   11230 <std::locale::~locale()@plt>
-	mov    0x9ec45(%rip),%rax        # b5e60 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x9ec4d(%rip),%rax        # b5e68 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	lea    0x68(%rsp),%rdi
 	mov    0x8(%rax),%rdx
 	mov    0x10(%rax),%rax
 	mov    %rdx,0x10(%rsp)
 	mov    -0x18(%rdx),%rdx
 	mov    %rax,0x10(%rsp,%rdx,1)
 	mov    0x9ed93(%rip),%rax        # b5fd0 <vtable for std::basic_ios<char, std::char_traits<char> >@GLIBCXX_3.4>
@@ -5560,29 +5560,29 @@
 	mov    (%rdi),%rax
 	mov    0xc(%rax),%eax
 	cmp    $0x1,%eax
 	je     172f8 <c10::intrusive_ptr<c10::SymNodeImpl, c10::detail::intrusive_target_default_null_type<c10::SymNodeImpl> >::reset_()+0x48>
 	mov    (%rdi),%rdi
 	mov    (%rdi),%rax
 	mov    0x10(%rax),%rax
-	cmp    0x9eb83(%rip),%rax        
+	cmp    0x9eb8b(%rip),%rax        
 	jne    17340 <c10::intrusive_ptr<c10::SymNodeImpl, c10::detail::intrusive_target_default_null_type<c10::SymNodeImpl> >::reset_()+0x90>
 	lock subl $0x1,0xc(%rdi)
 	je     172f8 <c10::intrusive_ptr<c10::SymNodeImpl, c10::detail::intrusive_target_default_null_type<c10::SymNodeImpl> >::reset_()+0x48>
 	add    $0x8,%rsp
 	pop    %rbx
 	pop    %rbp
 	ret
 	nopl   (%rax)
 	mov    (%rbx),%rbp
 	test   %rbp,%rbp
 	je     172ee <c10::intrusive_ptr<c10::SymNodeImpl, c10::detail::intrusive_target_default_null_type<c10::SymNodeImpl> >::reset_()+0x3e>
 	mov    0x0(%rbp),%rax
 	mov    0x8(%rax),%rax
-	cmp    0x9eae9(%rip),%rax        
+	cmp    0x9eaf1(%rip),%rax        
 	jne    17347 <c10::intrusive_ptr<c10::SymNodeImpl, c10::detail::intrusive_target_default_null_type<c10::SymNodeImpl> >::reset_()+0x97>
 	mov    0x9eac0(%rip),%rax        
 	mov    %rbp,%rdi
 	add    $0x10,%rax
 	mov    %rax,0x0(%rbp)
 	call   11080 <c10::intrusive_ptr_target::~intrusive_ptr_target()@plt>
 	add    $0x8,%rsp
@@ -5659,15 +5659,15 @@
 
 0000000000017400 <std::_Sp_counted_base<(__gnu_cxx::_Lock_policy)2>::_M_release()>:
 std::_Sp_counted_base<(__gnu_cxx::_Lock_policy)2>::_M_release():
 	push   %rbp
 	mov    %rdi,%rbp
 	push   %rbx
 	sub    $0x8,%rsp
-	mov    0x9ea08(%rip),%rbx        
+	mov    0x9ea10(%rip),%rbx        
 	test   %rbx,%rbx
 	je     17430 <std::_Sp_counted_base<(__gnu_cxx::_Lock_policy)2>::_M_release()+0x30>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x8(%rdi)
 	cmp    $0x1,%eax
 	je     1743e <std::_Sp_counted_base<(__gnu_cxx::_Lock_policy)2>::_M_release()+0x3e>
 	add    $0x8,%rsp
@@ -5716,15 +5716,15 @@
 	mov    %rdi,%rbx
 	mov    0xc(%rax),%eax
 	cmp    $0x1,%eax
 	je     174c0 <c10::intrusive_ptr<c10::VariableVersion::VersionCounter, c10::detail::intrusive_target_default_null_type<c10::VariableVersion::VersionCounter> >::reset_()+0x40>
 	mov    (%rdi),%rdi
 	mov    (%rdi),%rax
 	mov    0x10(%rax),%rax
-	cmp    0x9e9b8(%rip),%rax        
+	cmp    0x9e9c0(%rip),%rax        
 	jne    174d8 <c10::intrusive_ptr<c10::VariableVersion::VersionCounter, c10::detail::intrusive_target_default_null_type<c10::VariableVersion::VersionCounter> >::reset_()+0x58>
 	lock subl $0x1,0xc(%rdi)
 	je     174c0 <c10::intrusive_ptr<c10::VariableVersion::VersionCounter, c10::detail::intrusive_target_default_null_type<c10::VariableVersion::VersionCounter> >::reset_()+0x40>
 	pop    %rbx
 	ret
 	nopl   0x0(%rax,%rax,1)
 	mov    (%rbx),%rdi
@@ -5851,15 +5851,15 @@
 	push   %rbp
 	push   %rbx
 	sub    $0x10,%rsp
 	movzbl (%rdx),%ebx
 	mov    (%rsi),%r13
 	call   10b80 <operator new(unsigned long)@plt>
 	mov    0x9e6d2(%rip),%r14        
-	mov    0x9e8bb(%rip),%rdx        
+	mov    0x9e8c3(%rip),%rdx        
 	mov    %rax,%rbp
 	lea    0x10(%rdx),%rcx
 	lea    0x18(%r14),%rax
 	movb   $0x0,0x7a(%rbp)
 	movq   %rax,%xmm1
 	movq   %rcx,%xmm0
 	mov    0x9e673(%rip),%rax        
@@ -5941,15 +5941,15 @@
 	mov    0x40(%rbp),%rdi
 	test   %rdi,%rdi
 	je     177c2 <std::_MakeUniq<torch::autograd::AutogradMeta>::__single_object std::make_unique<torch::autograd::AutogradMeta, c10::TensorImpl*, bool&>(c10::TensorImpl*&&, bool&)+0x192>
 	call   10310 <std::_Sp_counted_base<(__gnu_cxx::_Lock_policy)2>::_M_release()@plt>
 	mov    0x30(%rbp),%rdi
 	test   %rdi,%rdi
 	je     177eb <std::_MakeUniq<torch::autograd::AutogradMeta>::__single_object std::make_unique<torch::autograd::AutogradMeta, c10::TensorImpl*, bool&>(c10::TensorImpl*&&, bool&)+0x1bb>
-	cmpq   $0x0,0x9e645(%rip)        
+	cmpq   $0x0,0x9e64d(%rip)        
 	lea    0xc(%rdi),%rdx
 	je     1784d <std::_MakeUniq<torch::autograd::AutogradMeta>::__single_object std::make_unique<torch::autograd::AutogradMeta, c10::TensorImpl*, bool&>(c10::TensorImpl*&&, bool&)+0x21d>
 	or     $0xffffffff,%eax
 	lock xadd %eax,(%rdx)
 	sub    $0x1,%eax
 	jne    177eb <std::_MakeUniq<torch::autograd::AutogradMeta>::__single_object std::make_unique<torch::autograd::AutogradMeta, c10::TensorImpl*, bool&>(c10::TensorImpl*&&, bool&)+0x1bb>
 	mov    (%rdi),%rax
@@ -6231,26 +6231,26 @@
 	movzbl 0x40(%r12),%edx
 	test   %dl,%dl
 	jne    180a0 <c10::FunctionSchema::~FunctionSchema()+0x6c0>
 	cmpq   $0x0,0x20(%r12)
 	je     17c27 <c10::FunctionSchema::~FunctionSchema()+0x247>
 	mov    0x20(%r12),%rbp
 	je     17c27 <c10::FunctionSchema::~FunctionSchema()+0x247>
-	mov    0x9e20d(%rip),%r13        
+	mov    0x9e215(%rip),%r13        
 	test   %r13,%r13
 	je     181d8 <c10::FunctionSchema::~FunctionSchema()+0x7f8>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x8(%rbp)
 	cmp    $0x1,%eax
 	je     181a0 <c10::FunctionSchema::~FunctionSchema()+0x7c0>
 	cmpq   $0x0,0x10(%r12)
 	je     17c59 <c10::FunctionSchema::~FunctionSchema()+0x279>
 	mov    0x10(%r12),%rbp
 	je     17c59 <c10::FunctionSchema::~FunctionSchema()+0x279>
-	mov    0x9e1db(%rip),%r13        
+	mov    0x9e1e3(%rip),%r13        
 	test   %r13,%r13
 	je     18188 <c10::FunctionSchema::~FunctionSchema()+0x7a8>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x8(%rbp)
 	cmp    $0x1,%eax
 	je     18150 <c10::FunctionSchema::~FunctionSchema()+0x770>
 	mov    (%r12),%rax
@@ -6384,26 +6384,26 @@
 	movzbl 0x40(%r12),%edx
 	test   %dl,%dl
 	jne    17fa0 <c10::FunctionSchema::~FunctionSchema()+0x5c0>
 	cmpq   $0x0,0x20(%r12)
 	je     17eb7 <c10::FunctionSchema::~FunctionSchema()+0x4d7>
 	mov    0x20(%r12),%rbp
 	je     17eb7 <c10::FunctionSchema::~FunctionSchema()+0x4d7>
-	mov    0x9df7d(%rip),%r13        
+	mov    0x9df85(%rip),%r13        
 	test   %r13,%r13
 	je     18088 <c10::FunctionSchema::~FunctionSchema()+0x6a8>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x8(%rbp)
 	cmp    $0x1,%eax
 	je     18050 <c10::FunctionSchema::~FunctionSchema()+0x670>
 	cmpq   $0x0,0x10(%r12)
 	je     17ee5 <c10::FunctionSchema::~FunctionSchema()+0x505>
 	mov    0x10(%r12),%rbp
 	je     17ee5 <c10::FunctionSchema::~FunctionSchema()+0x505>
-	mov    0x9df4b(%rip),%r13        
+	mov    0x9df53(%rip),%r13        
 	test   %r13,%r13
 	je     17f88 <c10::FunctionSchema::~FunctionSchema()+0x5a8>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x8(%rbp)
 	cmp    $0x1,%eax
 	je     17f50 <c10::FunctionSchema::~FunctionSchema()+0x570>
 	mov    (%r12),%rax
@@ -6592,25 +6592,25 @@
 	jmp    17c27 <c10::FunctionSchema::~FunctionSchema()+0x247>
 	nopl   (%rax)
 	mov    0x8(%rbp),%eax
 	lea    -0x1(%rax),%edx
 	mov    %edx,0x8(%rbp)
 	jmp    17c1e <c10::FunctionSchema::~FunctionSchema()+0x23e>
 	cs nopw 0x0(%rax,%rax,1)
-	cmpq   $0x0,0x9dc20(%rip)        
+	cmpq   $0x0,0x9dc28(%rip)        
 	je     18250 <c10::FunctionSchema::~FunctionSchema()+0x870>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     17c6e <c10::FunctionSchema::~FunctionSchema()+0x28e>
 	lea    0x28(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    17c6e <c10::FunctionSchema::~FunctionSchema()+0x28e>
 	nopl   0x0(%rax,%rax,1)
-	cmpq   $0x0,0x9dbf0(%rip)        
+	cmpq   $0x0,0x9dbf8(%rip)        
 	je     18260 <c10::FunctionSchema::~FunctionSchema()+0x880>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     17efd <c10::FunctionSchema::~FunctionSchema()+0x51d>
 	lea    0x28(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -6729,15 +6729,15 @@
 	mov    %rdi,%rbx
 	mov    0xc(%rax),%eax
 	cmp    $0x1,%eax
 	je     18450 <c10::intrusive_ptr<c10::OperatorKernel, c10::detail::intrusive_target_default_null_type<c10::OperatorKernel> >::reset_()+0x40>
 	mov    (%rdi),%rdi
 	mov    (%rdi),%rax
 	mov    0x10(%rax),%rax
-	cmp    0x9da28(%rip),%rax        
+	cmp    0x9da30(%rip),%rax        
 	jne    18468 <c10::intrusive_ptr<c10::OperatorKernel, c10::detail::intrusive_target_default_null_type<c10::OperatorKernel> >::reset_()+0x58>
 	lock subl $0x1,0xc(%rdi)
 	je     18450 <c10::intrusive_ptr<c10::OperatorKernel, c10::detail::intrusive_target_default_null_type<c10::OperatorKernel> >::reset_()+0x40>
 	pop    %rbx
 	ret
 	nopl   0x0(%rax,%rax,1)
 	mov    (%rbx),%rdi
@@ -6892,15 +6892,15 @@
 	lea    0x10(%rsp),%r14
 	mov    (%r15),%rax
 	mov    0xd8(%rax),%r8
 	mov    %r8,(%rsp)
 	call   10b80 <operator new(unsigned long)@plt>
 	mov    %r13,%rdi
 	mov    %rax,%rsi
-	mov    0x9d736(%rip),%rax        
+	mov    0x9d72e(%rip),%rax        
 	movq   $0x0,0x8(%rsi)
 	add    $0x10,%rax
 	movl   $0x0,0x10(%rsi)
 	mov    %rax,(%rsi)
 	call   11020 <c10::intrusive_ptr<c10::VariableVersion::VersionCounter, c10::detail::intrusive_target_default_null_type<c10::VariableVersion::VersionCounter> >::intrusive_ptr(c10::VariableVersion::VersionCounter*)@plt>
 	mov    (%rsp),%r8
 	movzbl %bpl,%ecx
@@ -7035,15 +7035,15 @@
 	mov    $0x10,%edi
 	call   10d60 <__cxa_allocate_exception@plt>
 	lea    0x1bde6(%rip),%rsi        
 	mov    %rax,%rdi
 	mov    %rax,%r15
 	call   102e0 <std::runtime_error::runtime_error(char const*)@plt>
 	mov    0x9d6b4(%rip),%rdx        
-	mov    0x9d55d(%rip),%rsi        
+	mov    0x9d565(%rip),%rsi        
 	mov    %r15,%rdi
 	call   105d0 <__cxa_throw@plt>
 	mov    %rax,%rbp
 	jmp    188e5 <torch::autograd::make_variable(at::Tensor, bool, bool)+0x375>
 	mov    %rax,%rbp
 	jmp    18905 <torch::autograd::make_variable(at::Tensor, bool, bool)+0x395>
 	mov    0x28(%rsp),%rdi
@@ -7062,15 +7062,15 @@
 	mov    $0x10,%edi
 	call   10d60 <__cxa_allocate_exception@plt>
 	lea    0x1bd7a(%rip),%rsi        
 	mov    %rax,%rdi
 	mov    %rax,%r14
 	call   102e0 <std::runtime_error::runtime_error(char const*)@plt>
 	mov    0x9d648(%rip),%rdx        
-	mov    0x9d4f1(%rip),%rsi        
+	mov    0x9d4f9(%rip),%rsi        
 	mov    %r14,%rdi
 	call   105d0 <__cxa_throw@plt>
 	mov    %rax,%rbp
 	jmp    189c4 <torch::autograd::make_variable(at::Tensor, bool, bool)+0x454>
 	mov    %rax,%rbx
 	jmp    189ee <torch::autograd::make_variable(at::Tensor, bool, bool)+0x47e>
 	mov    %rax,%rbp
@@ -7349,15 +7349,15 @@
 std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (*)(at::Tensor, at::Tensor, at::Tensor, long)>():
 	push   %r12
 	mov    $0x1,%r8d
 	mov    %rdi,%r12
 	mov    $0x4,%edx
 	push   %rbp
 	sub    $0xa8,%rsp
-	movq   0x9d0e0(%rip),%xmm0        # b5e20 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<at::Tensor>()@@Base+0xa06c0>
+	movq   0x9d0e8(%rip),%xmm0        # b5e28 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<at::Tensor>()@@Base+0xa06c8>
 	movq   0x9d258(%rip),%xmm1        # b5fa0 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<long>()@@Base+0xa0880>
 	lea    0x50(%rsp),%rbp
 	mov    %rsp,%rcx
 	lea    0x10(%rsp),%rsi
 	movhps 0x9cf8c(%rip),%xmm0        # b5ce8 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getFakeTypePtrCopy<at::Tensor>()@@Base+0xa0538>
 	movhps 0x9d24d(%rip),%xmm1        # b5fb0 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getFakeTypePtrCopy<long>()@@Base+0xa0870>
 	mov    %rbp,%rdi
@@ -7843,15 +7843,15 @@
 __cudaUnregisterBinaryUtil():
 	mov    0x9d669(%rip),%rdi        
 	jmp    10210 <__cudaUnregisterFatBinary@plt>
 	nopl   0x0(%rax)
 
 0000000000019560 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>:
 std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]:
-	cmpq   $0x0,0x9c8b0(%rip)        
+	cmpq   $0x0,0x9c8b8(%rip)        
 	je     19580 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x20>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x10(%rdi)
 	test   %eax,%eax
 	jle    1958d <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x2d>
 	ret
 	nopl   0x0(%rax)
@@ -9229,34 +9229,34 @@
 	mov    %r13,%rsi
 	mov    %rbp,%rdi
 	mov    %rax,%rdx
 	call   108b0 <std::basic_ostream<char, std::char_traits<char> >& std::__ostream_insert<char, std::char_traits<char> >(std::basic_ostream<char, std::char_traits<char> >&, char const*, long)@plt>
 	lea    0x18(%rsp),%rsi
 	mov    %r12,%rdi
 	call   10e30 <std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >::str() const@plt>
-	mov    0x9b1d1(%rip),%rax        # b5d68 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x9b1d9(%rip),%rax        # b5d70 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	lea    0x40(%rax),%rdx
 	add    $0x18,%rax
 	movq   %rax,%xmm0
-	mov    0x9b30d(%rip),%rax        # b5eb8 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x9b315(%rip),%rax        # b5ec0 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	mov    %rdx,0x68(%rsp)
 	add    $0x10,%rax
 	movq   %rax,%xmm1
 	mov    0x60(%rsp),%rax
 	punpcklqdq %xmm1,%xmm0
 	lea    -0x18(%rax),%rdi
 	cmp    0x9b15b(%rip),%rdi        
 	movaps %xmm0,0x10(%rsp)
 	jne    1afc0 <c10::detail::_str_wrapper<char const*, c10::ScalarType const&, char const*>::call(char const* const&, c10::ScalarType const&, char const* const&)+0x500>
 	mov    0x9b3c9(%rip),%rax        # b5fa8 <vtable for std::basic_streambuf<char, std::char_traits<char> >@GLIBCXX_3.4>
 	lea    0x50(%rsp),%rdi
 	add    $0x10,%rax
 	mov    %rax,0x18(%rsp)
 	call   11230 <std::locale::~locale()@plt>
-	mov    0x9b267(%rip),%rax        # b5e60 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x9b26f(%rip),%rax        # b5e68 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	lea    0x68(%rsp),%rdi
 	mov    0x8(%rax),%rdx
 	mov    0x10(%rax),%rax
 	mov    %rdx,0x10(%rsp)
 	mov    -0x18(%rdx),%rdx
 	mov    %rax,0x10(%rsp,%rdx,1)
 	mov    0x9b3b5(%rip),%rax        # b5fd0 <vtable for std::basic_ios<char, std::char_traits<char> >@GLIBCXX_3.4>
@@ -9436,48 +9436,48 @@
 	mov    %r12,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
 000000000001b000 <c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >::~WrapFunctionIntoRuntimeFunctor_()>:
 :impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >::~WrapFunctionIntoRuntimeFunctor_():
-	mov    0x9ae01(%rip),%rax        
+	mov    0x9ae09(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	jmp    11080 <c10::intrusive_ptr_target::~intrusive_ptr_target()@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
 000000000001b020 <c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >::~WrapFunctionIntoRuntimeFunctor_()>:
 :impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor> >::~WrapFunctionIntoRuntimeFunctor_():
-	mov    0x9ade1(%rip),%rax        
+	mov    0x9ade9(%rip),%rax        
 	push   %rbp
 	mov    %rdi,%rbp
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	call   11080 <c10::intrusive_ptr_target::~intrusive_ptr_target()@plt>
 	mov    %rbp,%rdi
 	mov    $0x18,%esi
 	pop    %rbp
 	jmp    10de0 <operator delete(void*, unsigned long)@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	nop
 
 000000000001b050 <c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor> >::~WrapFunctionIntoRuntimeFunctor_()>:
 :impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor> >::~WrapFunctionIntoRuntimeFunctor_():
-	mov    0x9adb1(%rip),%rax        
+	mov    0x9adb9(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	jmp    11080 <c10::intrusive_ptr_target::~intrusive_ptr_target()@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
 000000000001b070 <c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor> >::~WrapFunctionIntoRuntimeFunctor_()>:
 :impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor, at::Tensor), at::Tensor, c10::guts::typelist::typelist<at::Tensor, at::Tensor> >::~WrapFunctionIntoRuntimeFunctor_():
-	mov    0x9ad91(%rip),%rax        
+	mov    0x9ad99(%rip),%rax        
 	push   %rbp
 	mov    %rdi,%rbp
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	call   11080 <c10::intrusive_ptr_target::~intrusive_ptr_target()@plt>
 	mov    %rbp,%rdi
 	mov    $0x18,%esi
@@ -10248,15 +10248,15 @@
 __cudaUnregisterBinaryUtil():
 	mov    0x9afa9(%rip),%rdi        
 	jmp    10210 <__cudaUnregisterFatBinary@plt>
 	nopl   0x0(%rax)
 
 000000000001bcc0 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>:
 std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]:
-	cmpq   $0x0,0x9a150(%rip)        
+	cmpq   $0x0,0x9a158(%rip)        
 	je     1bce0 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x20>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x10(%rdi)
 	test   %eax,%eax
 	jle    1bced <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x2d>
 	ret
 	nopl   0x0(%rax)
@@ -10311,23 +10311,23 @@
 	nopl   (%rax)
 	mov    0xc(%rbp),%eax
 	lea    0xc(%rbp),%rbx
 	cmp    $0x1,%eax
 	je     1bdb3 <c10::SymInt::release_() [clone .part.0]+0xb3>
 	mov    0x0(%rbp),%rax
 	mov    0x10(%rax),%rax
-	cmp    0x9a0bd(%rip),%rax        
+	cmp    0x9a0c5(%rip),%rax        
 	jne    1be20 <c10::SymInt::release_() [clone .part.0]+0x120>
 	lock subl $0x1,(%rbx)
 	jne    1bd51 <c10::SymInt::release_() [clone .part.0]+0x51>
 	mov    0x0(%rbp),%rax
 	mov    0x8(%rax),%rax
-	cmp    0x9a036(%rip),%rax        
+	cmp    0x9a03e(%rip),%rax        
 	jne    1be10 <c10::SymInt::release_() [clone .part.0]+0x110>
-	mov    0x9a155(%rip),%rax        
+	mov    0x9a15d(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,0x0(%rbp)
 	mov    0x8(%rbp),%eax
 	test   %eax,%eax
 	je     1bde8 <c10::SymInt::release_() [clone .part.0]+0xe8>
 	mov    0x8(%rbp),%eax
 	cmp    $0xffffffe,%eax
@@ -11290,15 +11290,15 @@
 	mov    -0x1d8(%rbp),%edx
 	mov    %r12,%r9
 	mov    -0x1e0(%rbp),%rsi
 	push   -0x218(%rbp)
 	mov    -0x1d0(%rbp),%rcx
 	mov    %edx,-0x1a8(%rbp)
 	mov    -0x1c8(%rbp),%r8d
-	mov    0x98c41(%rip),%rdi        # b5cc8 <void torchao::(anonymous namespace)::nms_kernel_impl<c10::Half>(int, double, c10::Half const*, unsigned long long*)@@Base+0x97708>
+	mov    0x98c59(%rip),%rdi        # b5ce0 <void torchao::(anonymous namespace)::nms_kernel_impl<c10::Half>(int, double, c10::Half const*, unsigned long long*)@@Base+0x97720>
 	mov    %rsi,-0x1b0(%rbp)
 	mov    %rcx,-0x1c0(%rbp)
 	mov    %r8d,-0x1b8(%rbp)
 	call   111d0 <cudaLaunchKernel@plt>
 	jmp    1d231 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x1361>
 	cs nopw 0x0(%rax,%rax,1)
 	mov    -0x1f4(%rbp),%ecx
@@ -11354,15 +11354,15 @@
 	mov    -0x1d8(%rbp),%edx
 	mov    %r12,%r9
 	mov    -0x1e0(%rbp),%rsi
 	push   -0x218(%rbp)
 	mov    -0x1d0(%rbp),%rcx
 	mov    %edx,-0x1a8(%rbp)
 	mov    -0x1c8(%rbp),%r8d
-	mov    0x98b89(%rip),%rdi        # b5da0 <void torchao::(anonymous namespace)::nms_kernel_impl<float>(int, double, float const*, unsigned long long*)@@Base+0x978b0>
+	mov    0x98b91(%rip),%rdi        # b5da8 <void torchao::(anonymous namespace)::nms_kernel_impl<float>(int, double, float const*, unsigned long long*)@@Base+0x978b8>
 	mov    %rsi,-0x1b0(%rbp)
 	mov    %rcx,-0x1c0(%rbp)
 	mov    %r8d,-0x1b8(%rbp)
 	call   111d0 <cudaLaunchKernel@plt>
 	pop    %r10
 	pop    %r11
 	jmp    1c672 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x7a2>
@@ -11574,15 +11574,15 @@
 	mov    %rcx,%r14
 	cmp    %rcx,%rdi
 	jne    1da1a <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x1b4a>
 	mov    -0x1d0(%rbp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    %r14,%rdi
 	je     1c23d <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x36d>
-	cmpq   $0x0,0x987e4(%rip)        
+	cmpq   $0x0,0x987ec(%rip)        
 	je     1da47 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x1b77>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     1c23d <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x36d>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -11673,15 +11673,15 @@
 	mov    -0x1d8(%rbp),%edx
 	mov    %r12,%r9
 	mov    -0x1e0(%rbp),%rsi
 	push   -0x218(%rbp)
 	mov    -0x1d0(%rbp),%rcx
 	mov    %edx,-0x1a8(%rbp)
 	mov    -0x1c8(%rbp),%r8d
-	mov    0x98529(%rip),%rdi        # b5d80 <void torchao::(anonymous namespace)::nms_kernel_impl<double>(int, double, double const*, unsigned long long*)@@Base+0x976f0>
+	mov    0x98599(%rip),%rdi        # b5df0 <void torchao::(anonymous namespace)::nms_kernel_impl<double>(int, double, double const*, unsigned long long*)@@Base+0x97760>
 	mov    %rsi,-0x1b0(%rbp)
 	mov    %rcx,-0x1c0(%rbp)
 	mov    %r8d,-0x1b8(%rbp)
 	call   111d0 <cudaLaunchKernel@plt>
 	jmp    1d231 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x1361>
 	mov    (%rdi),%rax
 	call   *0x70(%rax)
@@ -11784,15 +11784,15 @@
 	mov    %rax,%rbx
 	jmp    1c492 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x5c2>
 	xor    %edx,%edx
 	xor    %edi,%edi
 	call   111b0 <long c10::detail::maybe_wrap_dim_slow<long>(long, long, bool)@plt>
 	mov    %rax,%rbx
 	jmp    1d8a9 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x19d9>
-	cmpq   $0x0,0x983f6(%rip)        
+	cmpq   $0x0,0x983fe(%rip)        
 	je     1da55 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x1b85>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     1d618 <torchao::(anonymous namespace)::nms_kernel(at::Tensor const&, at::Tensor const&, double)+0x1748>
 	lea    -0x210(%rbp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -12317,15 +12317,15 @@
 :cuda::impl::CUDAGuardImpl::recordDataPtrOnStream(c10::DataPtr const&, c10::Stream const&) const:
 	cmpb   $0x1,(%rdx)
 	movzbl 0x1(%rdx),%eax
 	mov    0x8(%rdx),%rcx
 	jne    1e224 <c10::cuda::impl::CUDAGuardImpl::recordDataPtrOnStream(c10::DataPtr const&, c10::Stream const&) const+0x24>
 	mov    $0x1,%edx
 	mov    %al,%dh
-	mov    0x97ccd(%rip),%rax        
+	mov    0x97cd5(%rip),%rax        
 	mov    (%rax),%rdi
 	mov    (%rdi),%rax
 	jmp    *0x78(%rax)
 	push   %rax
 	lea    0x1722c(%rip),%rcx        
 	mov    $0x43,%edx
 	lea    0x172d0(%rip),%rsi        
@@ -12339,15 +12339,15 @@
 	test   %rsi,%rsi
 	je     1e2c0 <c10::cuda::impl::CUDAGuardImpl::synchronizeEvent(void*) const+0x70>
 	mov    0x97d7c(%rip),%rax        
 	push   %rbp
 	mov    %rsi,%rbp
 	cmpb   $0x0,(%rax)
 	je     1e274 <c10::cuda::impl::CUDAGuardImpl::synchronizeEvent(void*) const+0x24>
-	mov    0x97aec(%rip),%rax        
+	mov    0x97af4(%rip),%rax        
 	mov    (%rax),%rax
 	test   %rax,%rax
 	jne    1e2a0 <c10::cuda::impl::CUDAGuardImpl::synchronizeEvent(void*) const+0x50>
 	mov    %rbp,%rdi
 	call   10980 <cudaEventSynchronize@plt>
 	mov    $0x1,%r8d
 	pop    %rbp
@@ -12581,15 +12581,15 @@
 	mov    %rax,0x3c(%rsp)
 	movl   $0x1,0x44(%rsp)
 	movaps %xmm0,0x70(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    1e5b4 <void torchao::(anonymous namespace)::nms_kernel_impl<float>(int, double, float const*, unsigned long long*)+0xc4>
 	push   0x28(%rsp)
-	mov    0x9780f(%rip),%rdi        # b5da0 <void torchao::(anonymous namespace)::nms_kernel_impl<float>(int, double, float const*, unsigned long long*)@@Base+0x978b0>
+	mov    0x97817(%rip),%rdi        # b5da8 <void torchao::(anonymous namespace)::nms_kernel_impl<float>(int, double, float const*, unsigned long long*)@@Base+0x978b8>
 	push   0x28(%rsp)
 	mov    0x4c(%rsp),%rcx
 	mov    0x54(%rsp),%r8d
 	mov    0x40(%rsp),%rsi
 	mov    0x48(%rsp),%edx
 	lea    0x70(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -12627,15 +12627,15 @@
 	mov    %rax,0x3c(%rsp)
 	movl   $0x1,0x44(%rsp)
 	movaps %xmm0,0x70(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    1e684 <void torchao::(anonymous namespace)::nms_kernel_impl<c10::Half>(int, double, c10::Half const*, unsigned long long*)+0xc4>
 	push   0x28(%rsp)
-	mov    0x97667(%rip),%rdi        # b5cc8 <void torchao::(anonymous namespace)::nms_kernel_impl<c10::Half>(int, double, c10::Half const*, unsigned long long*)@@Base+0x97708>
+	mov    0x9767f(%rip),%rdi        # b5ce0 <void torchao::(anonymous namespace)::nms_kernel_impl<c10::Half>(int, double, c10::Half const*, unsigned long long*)@@Base+0x97720>
 	push   0x28(%rsp)
 	mov    0x4c(%rsp),%rcx
 	mov    0x54(%rsp),%r8d
 	mov    0x40(%rsp),%rsi
 	mov    0x48(%rsp),%edx
 	lea    0x70(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -12673,15 +12673,15 @@
 	mov    %rax,0x3c(%rsp)
 	movl   $0x1,0x44(%rsp)
 	movaps %xmm0,0x70(%rsp)
 	call   11120 <__cudaPopCallConfiguration@plt>
 	test   %eax,%eax
 	jne    1e754 <void torchao::(anonymous namespace)::nms_kernel_impl<double>(int, double, double const*, unsigned long long*)+0xc4>
 	push   0x28(%rsp)
-	mov    0x9764f(%rip),%rdi        # b5d80 <void torchao::(anonymous namespace)::nms_kernel_impl<double>(int, double, double const*, unsigned long long*)@@Base+0x976f0>
+	mov    0x976bf(%rip),%rdi        # b5df0 <void torchao::(anonymous namespace)::nms_kernel_impl<double>(int, double, double const*, unsigned long long*)@@Base+0x97760>
 	push   0x28(%rsp)
 	mov    0x4c(%rsp),%rcx
 	mov    0x54(%rsp),%r8d
 	mov    0x40(%rsp),%rsi
 	mov    0x48(%rsp),%edx
 	lea    0x70(%rsp),%r9
 	call   111d0 <cudaLaunchKernel@plt>
@@ -12710,26 +12710,26 @@
 	jne    1e920 <c10::ValueError::~ValueError()+0x1c0>
 	mov    0x38(%r12),%rbp
 	test   %rbp,%rbp
 	jne    1e8f0 <c10::ValueError::~ValueError()+0x190>
 	mov    0x30(%r12),%rbp
 	test   %rbp,%rbp
 	je     1e7d0 <c10::ValueError::~ValueError()+0x70>
-	mov    0x97664(%rip),%r13        
+	mov    0x9766c(%rip),%r13        
 	test   %r13,%r13
 	je     1e888 <c10::ValueError::~ValueError()+0x128>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x8(%rbp)
 	cmp    $0x1,%eax
 	je     1e89a <c10::ValueError::~ValueError()+0x13a>
 	mov    0x18(%r12),%r13
 	mov    0x10(%r12),%rbp
 	cmp    %rbp,%r13
 	je     1e80f <c10::ValueError::~ValueError()+0xaf>
-	cmpq   $0x0,0x97631(%rip)        
+	cmpq   $0x0,0x97639(%rip)        
 	lea    0xf(%rsp),%r14
 	je     1e848 <c10::ValueError::~ValueError()+0xe8>
 	xchg   %ax,%ax
 	mov    0x0(%rbp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    %rbx,%rdi
 	jne    1e8d0 <c10::ValueError::~ValueError()+0x170>
@@ -12809,25 +12809,25 @@
 	cmp    %rbx,%rdi
 	jne    1e9b0 <c10::ValueError::~ValueError()+0x250>
 	mov    $0x8,%esi
 	mov    %rbp,%rdi
 	call   10de0 <operator delete(void*, unsigned long)@plt>
 	jmp    1e7a3 <c10::ValueError::~ValueError()+0x43>
 	nopl   0x0(%rax)
-	cmpq   $0x0,0x974f0(%rip)        
+	cmpq   $0x0,0x974f8(%rip)        
 	je     1e9a0 <c10::ValueError::~ValueError()+0x240>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     1e795 <c10::ValueError::~ValueError()+0x35>
 	lea    0xf(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    1e795 <c10::ValueError::~ValueError()+0x35>
 	nopl   0x0(%rax,%rax,1)
-	cmpq   $0x0,0x974c0(%rip)        
+	cmpq   $0x0,0x974c8(%rip)        
 	je     1e990 <c10::ValueError::~ValueError()+0x230>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     1e82e <c10::ValueError::~ValueError()+0xce>
 	lea    0xf(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -12844,15 +12844,15 @@
 	jmp    1e964 <c10::ValueError::~ValueError()+0x204>
 	nopl   0x0(%rax,%rax,1)
 	mov    -0x8(%rax),%edx
 	lea    -0x1(%rdx),%ecx
 	mov    %ecx,-0x8(%rax)
 	jmp    1e934 <c10::ValueError::~ValueError()+0x1d4>
 	nopl   0x0(%rax,%rax,1)
-	cmpq   $0x0,0x97460(%rip)        
+	cmpq   $0x0,0x97468(%rip)        
 	je     1e9e0 <c10::ValueError::~ValueError()+0x280>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     1e90a <c10::ValueError::~ValueError()+0x1aa>
 	lea    0xf(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -12883,26 +12883,26 @@
 	jne    1ebc0 <c10::ValueError::~ValueError()+0x1d0>
 	mov    0x38(%rbp),%r12
 	test   %r12,%r12
 	jne    1eb90 <c10::ValueError::~ValueError()+0x1a0>
 	mov    0x30(%rbp),%r12
 	test   %r12,%r12
 	je     1ea60 <c10::ValueError::~ValueError()+0x70>
-	mov    0x973d6(%rip),%r13        
+	mov    0x973de(%rip),%r13        
 	test   %r13,%r13
 	je     1eb20 <c10::ValueError::~ValueError()+0x130>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x8(%r12)
 	cmp    $0x1,%eax
 	je     1eb36 <c10::ValueError::~ValueError()+0x146>
 	mov    0x18(%rbp),%r13
 	mov    0x10(%rbp),%r12
 	cmp    %r12,%r13
 	je     1ea9e <c10::ValueError::~ValueError()+0xae>
-	cmpq   $0x0,0x973a3(%rip)        
+	cmpq   $0x0,0x973ab(%rip)        
 	lea    0xf(%rsp),%r14
 	je     1eae0 <c10::ValueError::~ValueError()+0xf0>
 	nopl   0x0(%rax)
 	mov    (%r12),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    %rbx,%rdi
 	jne    1eb70 <c10::ValueError::~ValueError()+0x180>
@@ -12985,25 +12985,25 @@
 	cmp    %rbx,%rdi
 	jne    1ec58 <c10::ValueError::~ValueError()+0x268>
 	mov    $0x8,%esi
 	mov    %r12,%rdi
 	call   10de0 <operator delete(void*, unsigned long)@plt>
 	jmp    1ea32 <c10::ValueError::~ValueError()+0x42>
 	nopl   0x0(%rax,%rax,1)
-	cmpq   $0x0,0x97250(%rip)        
+	cmpq   $0x0,0x97258(%rip)        
 	je     1ec48 <c10::ValueError::~ValueError()+0x258>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     1ea25 <c10::ValueError::~ValueError()+0x35>
 	lea    0xf(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    1ea25 <c10::ValueError::~ValueError()+0x35>
 	nopl   0x0(%rax,%rax,1)
-	cmpq   $0x0,0x97220(%rip)        
+	cmpq   $0x0,0x97228(%rip)        
 	je     1ec38 <c10::ValueError::~ValueError()+0x248>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     1eabc <c10::ValueError::~ValueError()+0xcc>
 	lea    0xf(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -13020,15 +13020,15 @@
 	jmp    1ec04 <c10::ValueError::~ValueError()+0x214>
 	nopl   0x0(%rax,%rax,1)
 	mov    -0x8(%rax),%edx
 	lea    -0x1(%rdx),%ecx
 	mov    %ecx,-0x8(%rax)
 	jmp    1ebd4 <c10::ValueError::~ValueError()+0x1e4>
 	nopl   0x0(%rax,%rax,1)
-	cmpq   $0x0,0x971b8(%rip)        
+	cmpq   $0x0,0x971c0(%rip)        
 	je     1ec88 <c10::ValueError::~ValueError()+0x298>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     1eba9 <c10::ValueError::~ValueError()+0x1b9>
 	lea    0xf(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -13308,15 +13308,15 @@
 	nopl   0x0(%rax,%rax,1)
 
 000000000001f090 <std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >::~basic_stringbuf()>:
 std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >::~basic_stringbuf():
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x10,%rsp
-	mov    0x96e19(%rip),%rax        # b5eb8 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x96e21(%rip),%rax        # b5ec0 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	mov    0x48(%rdi),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    0x96c73(%rip),%rdi        
 	jne    1f0d8 <std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >::~basic_stringbuf()+0x48>
 	mov    0x96eea(%rip),%rax        # b5fa8 <vtable for std::basic_streambuf<char, std::char_traits<char> >@GLIBCXX_3.4>
@@ -13324,15 +13324,15 @@
 	add    $0x10,%rax
 	mov    %rax,(%rbx)
 	call   11230 <std::locale::~locale()@plt>
 	add    $0x10,%rsp
 	pop    %rbx
 	ret
 	nopl   0x0(%rax)
-	cmpq   $0x0,0x96d38(%rip)        
+	cmpq   $0x0,0x96d40(%rip)        
 	je     1f100 <std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >::~basic_stringbuf()+0x70>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     1f0b7 <std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >::~basic_stringbuf()+0x27>
 	lea    0xf(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -13345,15 +13345,15 @@
 	nopl   0x0(%rax,%rax,1)
 
 000000000001f110 <std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >::~basic_stringbuf()>:
 std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >::~basic_stringbuf():
 	push   %rbp
 	mov    %rdi,%rbp
 	sub    $0x10,%rsp
-	mov    0x96d99(%rip),%rax        # b5eb8 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x96da1(%rip),%rax        # b5ec0 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	mov    0x48(%rdi),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    0x96bf3(%rip),%rdi        
 	jne    1f168 <std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >::~basic_stringbuf()+0x58>
 	mov    0x96e6a(%rip),%rax        # b5fa8 <vtable for std::basic_streambuf<char, std::char_traits<char> >@GLIBCXX_3.4>
@@ -13364,15 +13364,15 @@
 	mov    %rbp,%rdi
 	mov    $0x50,%esi
 	call   10de0 <operator delete(void*, unsigned long)@plt>
 	add    $0x10,%rsp
 	pop    %rbp
 	ret
 	nopw   0x0(%rax,%rax,1)
-	cmpq   $0x0,0x96ca8(%rip)        
+	cmpq   $0x0,0x96cb0(%rip)        
 	je     1f190 <std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >::~basic_stringbuf()+0x80>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     1f137 <std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >::~basic_stringbuf()+0x27>
 	lea    0xf(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -13405,25 +13405,25 @@
 	xor    %esi,%esi
 	movaps %xmm0,0x170(%rsp)
 	add    $0x10,%rax
 	movaps %xmm0,0x180(%rsp)
 	mov    %rax,0x88(%rsp)
 	xor    %eax,%eax
 	mov    %ax,0x168(%rsp)
-	mov    0x96c55(%rip),%rax        # b5e60 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x96c5d(%rip),%rax        # b5e68 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movq   $0x0,0x160(%rsp)
 	mov    0x8(%rax),%r15
 	mov    0x10(%rax),%rax
 	mov    -0x18(%r15),%rdi
 	mov    %r15,0x30(%rsp)
 	mov    %rax,(%rsp)
 	add    %rbx,%rdi
 	mov    %rax,(%rdi)
 	call   10e20 <std::basic_ios<char, std::char_traits<char> >::init(std::basic_streambuf<char, std::char_traits<char> >*)@plt>
-	mov    0x96b2a(%rip),%rax        # b5d68 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x96b32(%rip),%rax        # b5d70 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	lea    0x38(%rsp),%r13
 	lea    0x18(%rax),%rcx
 	add    $0x40,%rax
 	mov    %rax,0x88(%rsp)
 	mov    0x96d4e(%rip),%rax        # b5fa8 <vtable for std::basic_streambuf<char, std::char_traits<char> >@GLIBCXX_3.4>
 	movq   %rcx,%xmm0
 	mov    %rcx,0x8(%rsp)
@@ -13435,15 +13435,15 @@
 	mov    %rax,0x18(%rsp)
 	movaps %xmm0,0x30(%rsp)
 	pxor   %xmm0,%xmm0
 	movaps %xmm0,0x40(%rsp)
 	movaps %xmm0,0x50(%rsp)
 	movaps %xmm0,0x60(%rsp)
 	call   10fe0 <std::locale::locale()@plt>
-	mov    0x96c16(%rip),%rax        # b5eb8 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x96c1e(%rip),%rax        # b5ec0 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	mov    %r13,%rsi
 	mov    %rbp,%rdi
 	movl   $0x10,0x78(%rsp)
 	add    $0x10,%rax
 	mov    %rax,0x38(%rsp)
 	mov    0x96a68(%rip),%rax        
 	add    $0x18,%rax
@@ -13475,19 +13475,19 @@
 	mov    -0x18(%rdx),%rdx
 	cmp    %r8,%rax
 	ja     1f3f0 <c10::detail::_str_wrapper<char const*, long const&>::call(char const* const&, long const&)+0x250>
 	sub    %rcx,%r8
 	xor    %esi,%esi
 	mov    %r12,%rdi
 	call   10ad0 <std::string::replace(unsigned long, unsigned long, char const*, unsigned long)@plt>
-	mov    0x96a18(%rip),%rax        # b5d68 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x96a20(%rip),%rax        # b5d70 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movq   0x8(%rsp),%xmm0
 	add    $0x40,%rax
 	mov    %rax,0x88(%rsp)
-	mov    0x96b4f(%rip),%rax        # b5eb8 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x96b57(%rip),%rax        # b5ec0 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	add    $0x10,%rax
 	movq   %rax,%xmm2
 	mov    0x80(%rsp),%rax
 	punpcklqdq %xmm2,%xmm0
 	lea    -0x18(%rax),%rdi
 	cmp    0x9699f(%rip),%rdi        
 	movaps %xmm0,0x30(%rsp)
@@ -13531,15 +13531,15 @@
 	jmp    1f2f3 <c10::detail::_str_wrapper<char const*, long const&>::call(char const* const&, long const&)+0x153>
 	nopl   0x0(%rax)
 	lea    0x80(%rsp),%rsi
 	mov    %r12,%rdi
 	call   106c0 <std::string::assign(std::string const&)@plt>
 	jmp    1f349 <c10::detail::_str_wrapper<char const*, long const&>::call(char const* const&, long const&)+0x1a9>
 	nopl   (%rax)
-	cmpq   $0x0,0x969d0(%rip)        
+	cmpq   $0x0,0x969d8(%rip)        
 	je     1f470 <c10::detail::_str_wrapper<char const*, long const&>::call(char const* const&, long const&)+0x2d0>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     1f394 <c10::detail::_str_wrapper<char const*, long const&>::call(char const* const&, long const&)+0x1f4>
 	mov    %r13,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -13604,25 +13604,25 @@
 	xor    %esi,%esi
 	movaps %xmm0,0x170(%rsp)
 	add    $0x10,%rax
 	movaps %xmm0,0x180(%rsp)
 	mov    %rax,0x88(%rsp)
 	xor    %eax,%eax
 	mov    %ax,0x168(%rsp)
-	mov    0x968f5(%rip),%rax        # b5e60 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x968fd(%rip),%rax        # b5e68 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movq   $0x0,0x160(%rsp)
 	mov    0x8(%rax),%r15
 	mov    0x10(%rax),%rax
 	mov    -0x18(%r15),%rdi
 	mov    %r15,0x30(%rsp)
 	mov    %rax,(%rsp)
 	add    %rbx,%rdi
 	mov    %rax,(%rdi)
 	call   10e20 <std::basic_ios<char, std::char_traits<char> >::init(std::basic_streambuf<char, std::char_traits<char> >*)@plt>
-	mov    0x967ca(%rip),%rax        # b5d68 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x967d2(%rip),%rax        # b5d70 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	lea    0x38(%rsp),%r13
 	lea    0x18(%rax),%rcx
 	add    $0x40,%rax
 	mov    %rax,0x88(%rsp)
 	mov    0x969ee(%rip),%rax        # b5fa8 <vtable for std::basic_streambuf<char, std::char_traits<char> >@GLIBCXX_3.4>
 	movq   %rcx,%xmm0
 	mov    %rcx,0x8(%rsp)
@@ -13634,15 +13634,15 @@
 	mov    %rax,0x18(%rsp)
 	movaps %xmm0,0x30(%rsp)
 	pxor   %xmm0,%xmm0
 	movaps %xmm0,0x40(%rsp)
 	movaps %xmm0,0x50(%rsp)
 	movaps %xmm0,0x60(%rsp)
 	call   10fe0 <std::locale::locale()@plt>
-	mov    0x968b6(%rip),%rax        # b5eb8 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x968be(%rip),%rax        # b5ec0 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	mov    %r13,%rsi
 	mov    %rbp,%rdi
 	movl   $0x10,0x78(%rsp)
 	add    $0x10,%rax
 	mov    %rax,0x38(%rsp)
 	mov    0x96708(%rip),%rax        
 	add    $0x18,%rax
@@ -13680,19 +13680,19 @@
 	mov    -0x18(%rdx),%rdx
 	cmp    %r8,%rax
 	ja     1f770 <c10::detail::_str_wrapper<char const*, char const* const&>::call(char const* const&, char const* const&)+0x270>
 	sub    %rcx,%r8
 	xor    %esi,%esi
 	mov    %r12,%rdi
 	call   10ad0 <std::string::replace(unsigned long, unsigned long, char const*, unsigned long)@plt>
-	mov    0x966a1(%rip),%rax        # b5d68 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x966a9(%rip),%rax        # b5d70 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movq   0x8(%rsp),%xmm0
 	add    $0x40,%rax
 	mov    %rax,0x88(%rsp)
-	mov    0x967d8(%rip),%rax        # b5eb8 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x967e0(%rip),%rax        # b5ec0 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	add    $0x10,%rax
 	movq   %rax,%xmm2
 	mov    0x80(%rsp),%rax
 	punpcklqdq %xmm2,%xmm0
 	lea    -0x18(%rax),%rdi
 	cmp    0x96628(%rip),%rdi        
 	movaps %xmm0,0x30(%rsp)
@@ -13745,15 +13745,15 @@
 	jmp    1f653 <c10::detail::_str_wrapper<char const*, char const* const&>::call(char const* const&, char const* const&)+0x153>
 	nopl   0x0(%rax)
 	lea    0x80(%rsp),%rsi
 	mov    %r12,%rdi
 	call   106c0 <std::string::assign(std::string const&)@plt>
 	jmp    1f6c0 <c10::detail::_str_wrapper<char const*, char const* const&>::call(char const* const&, char const* const&)+0x1c0>
 	nopl   (%rax)
-	cmpq   $0x0,0x96630(%rip)        
+	cmpq   $0x0,0x96638(%rip)        
 	je     1f810 <c10::detail::_str_wrapper<char const*, char const* const&>::call(char const* const&, char const* const&)+0x310>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     1f70b <c10::detail::_str_wrapper<char const*, char const* const&>::call(char const* const&, char const* const&)+0x20b>
 	mov    %r13,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -13953,15 +13953,15 @@
 	lea    0x162ab(%rip),%rdx        
 	mov    %eax,%edi
 	lea    0x1586e(%rip),%rsi        
 	call   10280 <c10::cuda::c10_cuda_check_implementation(int, char const*, char const*, int, bool)@plt>
 	mov    0x964b2(%rip),%rax        
 	cmpb   $0x0,(%rax)
 	je     1fb3a <c10::cuda::impl::CUDAGuardImpl::block(void*, c10::Stream const&) const+0xfa>
-	mov    0x96226(%rip),%rax        
+	mov    0x9622e(%rip),%rax        
 	mov    (%rax),%rax
 	test   %rax,%rax
 	jne    1fb70 <c10::cuda::impl::CUDAGuardImpl::block(void*, c10::Stream const&) const+0x130>
 	movsbl %bpl,%edi
 	call   11060 <c10::cuda::SetDevice(signed char)@plt>
 	mov    $0x1,%r8d
 	mov    $0x36,%ecx
@@ -14087,15 +14087,15 @@
 	mov    %eax,%edi
 	lea    0x1562b(%rip),%rsi        
 	call   10280 <c10::cuda::c10_cuda_check_implementation(int, char const*, char const*, int, bool)@plt>
 	mov    0x8(%rsp),%rax
 	cmpb   $0x0,(%rbx)
 	mov    %rax,0x0(%rbp)
 	je     1fd83 <c10::cuda::impl::CUDAGuardImpl::record(void**, c10::Stream const&, signed char, c10::EventFlag) const+0x133>
-	mov    0x95fe1(%rip),%rax        
+	mov    0x95fe9(%rip),%rax        
 	mov    (%rax),%rax
 	test   %rax,%rax
 	jne    1fe50 <c10::cuda::impl::CUDAGuardImpl::record(void**, c10::Stream const&, signed char, c10::EventFlag) const+0x200>
 	movsbl %r12b,%edi
 	call   11060 <c10::cuda::SetDevice(signed char)@plt>
 	mov    $0x1,%r8d
 	mov    $0x36,%ecx
@@ -14122,15 +14122,15 @@
 	lea    0x15ff4(%rip),%rdx        
 	mov    %eax,%edi
 	lea    0x15596(%rip),%rsi        
 	call   10280 <c10::cuda::c10_cuda_check_implementation(int, char const*, char const*, int, bool)@plt>
 	mov    0x961da(%rip),%rbx        
 	cmpb   $0x0,(%rbx)
 	je     1fd28 <c10::cuda::impl::CUDAGuardImpl::record(void**, c10::Stream const&, signed char, c10::EventFlag) const+0xd8>
-	mov    0x95f4a(%rip),%rax        
+	mov    0x95f52(%rip),%rax        
 	mov    (%rax),%rax
 	test   %rax,%rax
 	je     1fd28 <c10::cuda::impl::CUDAGuardImpl::record(void**, c10::Stream const&, signed char, c10::EventFlag) const+0xd8>
 	mov    (%rax),%rdi
 	mov    %r13,%rdx
 	mov    $0x1,%esi
 	mov    (%rdi),%rax
@@ -14245,15 +14245,15 @@
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
 0000000000020030 <c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >::~WrapFunctionIntoRuntimeFunctor_()>:
 :impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >::~WrapFunctionIntoRuntimeFunctor_():
 	push   %rbx
 	sub    $0x20,%rsp
-	mov    0x95ee4(%rip),%rax        
+	mov    0x95eec(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	mov    0x8(%rdi),%eax
 	test   %eax,%eax
 	je     20054 <c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >::~WrapFunctionIntoRuntimeFunctor_()+0x24>
 	mov    0x8(%rdi),%eax
 	cmp    $0xffffffe,%eax
@@ -14298,15 +14298,15 @@
 	cs nopw 0x0(%rax,%rax,1)
 	nop
 
 0000000000020100 <c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >::~WrapFunctionIntoRuntimeFunctor_()>:
 :impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >::~WrapFunctionIntoRuntimeFunctor_():
 	push   %rbx
 	sub    $0x20,%rsp
-	mov    0x95e14(%rip),%rax        
+	mov    0x95e1c(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	mov    0x8(%rdi),%eax
 	test   %eax,%eax
 	je     20124 <c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >::~WrapFunctionIntoRuntimeFunctor_()+0x24>
 	mov    0x8(%rdi),%eax
 	cmp    $0xffffffe,%eax
@@ -14406,23 +14406,23 @@
 	jne    20204 <at::indexing::TensorIndex::~TensorIndex()+0x34>
 	mov    0xc(%rdi),%eax
 	lea    0xc(%rdi),%rbp
 	cmp    $0x1,%eax
 	je     202ca <at::indexing::TensorIndex::~TensorIndex()+0xfa>
 	mov    (%rdi),%rax
 	mov    0x10(%rax),%rax
-	cmp    0x95baf(%rip),%rax        
+	cmp    0x95bb7(%rip),%rax        
 	jne    2060f <at::indexing::TensorIndex::~TensorIndex()+0x43f>
 	lock subl $0x1,0x0(%rbp)
 	jne    20204 <at::indexing::TensorIndex::~TensorIndex()+0x34>
 	mov    (%rdi),%rax
 	mov    0x8(%rax),%rax
-	cmp    0x95b20(%rip),%rax        
+	cmp    0x95b28(%rip),%rax        
 	jne    2063f <at::indexing::TensorIndex::~TensorIndex()+0x46f>
-	mov    0x95c3b(%rip),%rax        
+	mov    0x95c43(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	mov    0x8(%rdi),%eax
 	test   %eax,%eax
 	je     20301 <at::indexing::TensorIndex::~TensorIndex()+0x131>
 	mov    0x8(%rdi),%eax
 	cmp    $0xffffffe,%eax
@@ -14459,23 +14459,23 @@
 	jne    2021b <at::indexing::TensorIndex::~TensorIndex()+0x4b>
 	mov    0xc(%rdi),%eax
 	lea    0xc(%rdi),%rbp
 	cmp    $0x1,%eax
 	je     203a2 <at::indexing::TensorIndex::~TensorIndex()+0x1d2>
 	mov    (%rdi),%rax
 	mov    0x10(%rax),%rax
-	cmp    0x95ad7(%rip),%rax        
+	cmp    0x95adf(%rip),%rax        
 	jne    205fe <at::indexing::TensorIndex::~TensorIndex()+0x42e>
 	lock subl $0x1,0x0(%rbp)
 	jne    2021b <at::indexing::TensorIndex::~TensorIndex()+0x4b>
 	mov    (%rdi),%rax
 	mov    0x8(%rax),%rax
-	cmp    0x95a48(%rip),%rax        
+	cmp    0x95a50(%rip),%rax        
 	jne    20631 <at::indexing::TensorIndex::~TensorIndex()+0x461>
-	mov    0x95b63(%rip),%rax        
+	mov    0x95b6b(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	mov    0x8(%rdi),%eax
 	test   %eax,%eax
 	je     203d9 <at::indexing::TensorIndex::~TensorIndex()+0x209>
 	mov    0x8(%rdi),%eax
 	cmp    $0xffffffe,%eax
@@ -14512,23 +14512,23 @@
 	jne    20232 <at::indexing::TensorIndex::~TensorIndex()+0x62>
 	mov    0xc(%rdi),%eax
 	lea    0xc(%rdi),%rbp
 	cmp    $0x1,%eax
 	je     2047a <at::indexing::TensorIndex::~TensorIndex()+0x2aa>
 	mov    (%rdi),%rax
 	mov    0x10(%rax),%rax
-	cmp    0x959ff(%rip),%rax        
+	cmp    0x95a07(%rip),%rax        
 	jne    205ed <at::indexing::TensorIndex::~TensorIndex()+0x41d>
 	lock subl $0x1,0x0(%rbp)
 	jne    20232 <at::indexing::TensorIndex::~TensorIndex()+0x62>
 	mov    (%rdi),%rax
 	mov    0x8(%rax),%rax
-	cmp    0x95970(%rip),%rax        
+	cmp    0x95978(%rip),%rax        
 	jne    20638 <at::indexing::TensorIndex::~TensorIndex()+0x468>
-	mov    0x95a8b(%rip),%rax        
+	mov    0x95a93(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	mov    0x8(%rdi),%eax
 	test   %eax,%eax
 	je     204b1 <at::indexing::TensorIndex::~TensorIndex()+0x2e1>
 	mov    0x8(%rdi),%eax
 	cmp    $0xffffffe,%eax
@@ -14565,23 +14565,23 @@
 	jne    20248 <at::indexing::TensorIndex::~TensorIndex()+0x78>
 	mov    0xc(%rdi),%eax
 	lea    0xc(%rdi),%rbx
 	cmp    $0x1,%eax
 	je     20551 <at::indexing::TensorIndex::~TensorIndex()+0x381>
 	mov    (%rdi),%rax
 	mov    0x10(%rax),%rax
-	cmp    0x95927(%rip),%rax        
+	cmp    0x9592f(%rip),%rax        
 	jne    20620 <at::indexing::TensorIndex::~TensorIndex()+0x450>
 	lock subl $0x1,(%rbx)
 	jne    20248 <at::indexing::TensorIndex::~TensorIndex()+0x78>
 	mov    (%rdi),%rax
 	mov    0x8(%rax),%rax
-	cmp    0x95899(%rip),%rax        
+	cmp    0x958a1(%rip),%rax        
 	jne    20646 <at::indexing::TensorIndex::~TensorIndex()+0x476>
-	mov    0x959b4(%rip),%rax        
+	mov    0x959bc(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	mov    0x8(%rdi),%eax
 	test   %eax,%eax
 	je     20588 <at::indexing::TensorIndex::~TensorIndex()+0x3b8>
 	mov    0x8(%rdi),%eax
 	cmp    $0xffffffe,%eax
@@ -14810,25 +14810,25 @@
 	xor    %esi,%esi
 	movaps %xmm0,0x180(%rsp)
 	add    $0x10,%rax
 	movaps %xmm0,0x190(%rsp)
 	mov    %rax,0x98(%rsp)
 	xor    %eax,%eax
 	mov    %ax,0x178(%rsp)
-	mov    0x95498(%rip),%rax        # b5e60 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x954a0(%rip),%rax        # b5e68 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movq   $0x0,0x170(%rsp)
 	mov    0x8(%rax),%rbx
 	mov    0x10(%rax),%rax
 	mov    -0x18(%rbx),%rdi
 	mov    %rbx,0x40(%rsp)
 	mov    %rax,(%rsp)
 	add    %rbp,%rdi
 	mov    %rax,(%rdi)
 	call   10e20 <std::basic_ios<char, std::char_traits<char> >::init(std::basic_streambuf<char, std::char_traits<char> >*)@plt>
-	mov    0x9536d(%rip),%rax        # b5d68 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x95375(%rip),%rax        # b5d70 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	lea    0x80(%rsp),%r13
 	lea    0x48(%rsp),%r15
 	mov    %r13,%rdi
 	lea    0x18(%rax),%rcx
 	add    $0x40,%rax
 	mov    %rax,0x98(%rsp)
 	mov    0x95586(%rip),%rax        # b5fa8 <vtable for std::basic_streambuf<char, std::char_traits<char> >@GLIBCXX_3.4>
@@ -14839,15 +14839,15 @@
 	punpcklqdq %xmm1,%xmm0
 	movaps %xmm0,0x40(%rsp)
 	pxor   %xmm0,%xmm0
 	movaps %xmm0,0x50(%rsp)
 	movaps %xmm0,0x60(%rsp)
 	movaps %xmm0,0x70(%rsp)
 	call   10fe0 <std::locale::locale()@plt>
-	mov    0x9545b(%rip),%rax        # b5eb8 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x95463(%rip),%rax        # b5ec0 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	mov    %r15,%rsi
 	mov    %r14,%rdi
 	movl   $0x10,0x88(%rsp)
 	add    $0x10,%rax
 	mov    %rax,0x48(%rsp)
 	mov    0x952aa(%rip),%rax        
 	add    $0x18,%rax
@@ -14879,19 +14879,19 @@
 	mov    -0x18(%rdx),%rdx
 	cmp    %r8,%rax
 	ja     20c40 <c10::cuda::impl::CUDAGuardImpl::uncheckedSetDevice(c10::Device) const+0x310>
 	sub    %rcx,%r8
 	xor    %esi,%esi
 	mov    %r12,%rdi
 	call   10ad0 <std::string::replace(unsigned long, unsigned long, char const*, unsigned long)@plt>
-	mov    0x95253(%rip),%rax        # b5d68 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x9525b(%rip),%rax        # b5d70 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movq   0x8(%rsp),%xmm0
 	add    $0x40,%rax
 	mov    %rax,0x98(%rsp)
-	mov    0x9538a(%rip),%rax        # b5eb8 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x95392(%rip),%rax        # b5ec0 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	add    $0x10,%rax
 	movq   %rax,%xmm2
 	mov    0x90(%rsp),%rax
 	punpcklqdq %xmm2,%xmm0
 	lea    -0x18(%rax),%rdi
 	cmp    0x951da(%rip),%rdi        
 	movaps %xmm0,0x40(%rsp)
@@ -14931,15 +14931,15 @@
 	lea    -0x18(%rax),%rdi
 	cmp    0x95132(%rip),%rdi        
 	jne    20c8d <c10::cuda::impl::CUDAGuardImpl::uncheckedSetDevice(c10::Device) const+0x35d>
 	mov    0x18(%rsp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    0x9511c(%rip),%rdi        
 	je     20952 <c10::cuda::impl::CUDAGuardImpl::uncheckedSetDevice(c10::Device) const+0x22>
-	cmpq   $0x0,0x951fe(%rip)        
+	cmpq   $0x0,0x95206(%rip)        
 	je     20ce1 <c10::cuda::impl::CUDAGuardImpl::uncheckedSetDevice(c10::Device) const+0x3b1>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     20952 <c10::cuda::impl::CUDAGuardImpl::uncheckedSetDevice(c10::Device) const+0x22>
 	mov    %rbp,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -14960,24 +14960,24 @@
 	call   10080 <std::basic_ios<char, std::char_traits<char> >::clear(std::_Ios_Iostate)@plt>
 	jmp    20ac2 <c10::cuda::impl::CUDAGuardImpl::uncheckedSetDevice(c10::Device) const+0x192>
 	nopl   0x0(%rax)
 	lea    0x90(%rsp),%rsi
 	mov    %r12,%rdi
 	call   106c0 <std::string::assign(std::string const&)@plt>
 	jmp    20b0e <c10::cuda::impl::CUDAGuardImpl::uncheckedSetDevice(c10::Device) const+0x1de>
-	cmpq   $0x0,0x95183(%rip)        
+	cmpq   $0x0,0x9518b(%rip)        
 	je     20cef <c10::cuda::impl::CUDAGuardImpl::uncheckedSetDevice(c10::Device) const+0x3bf>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     20bfc <c10::cuda::impl::CUDAGuardImpl::uncheckedSetDevice(c10::Device) const+0x2cc>
 	lea    0x17(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    20bfc <c10::cuda::impl::CUDAGuardImpl::uncheckedSetDevice(c10::Device) const+0x2cc>
-	cmpq   $0x0,0x95158(%rip)        
+	cmpq   $0x0,0x95160(%rip)        
 	je     20cfa <c10::cuda::impl::CUDAGuardImpl::uncheckedSetDevice(c10::Device) const+0x3ca>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     20b59 <c10::cuda::impl::CUDAGuardImpl::uncheckedSetDevice(c10::Device) const+0x229>
 	mov    %r15,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -15045,15 +15045,15 @@
 	call   11060 <c10::cuda::SetDevice(signed char)@plt>
 	mov    %eax,%ebp
 	test   %eax,%eax
 	jne    217a8 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0xa38>
 	mov    0x95217(%rip),%rax        
 	cmpb   $0x0,(%rax)
 	je     20dd5 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x65>
-	mov    0x94f8b(%rip),%rax        
+	mov    0x94f93(%rip),%rax        
 	mov    (%rax),%rax
 	test   %rax,%rax
 	jne    20e18 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0xa8>
 	mov    %r12,%rdi
 	call   10220 <cudaEventDestroy@plt>
 	mov    %eax,%ebp
 	test   %eax,%eax
@@ -15093,27 +15093,27 @@
 	xor    %edx,%edx
 	xor    %esi,%esi
 	pxor   %xmm0,%xmm0
 	mov    %dx,0x478(%rsp)
 	mov    %rax,0x8(%rsp)
 	add    $0x10,%rax
 	mov    %rax,0x398(%rsp)
-	mov    0x94fda(%rip),%rax        # b5e60 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x94fe2(%rip),%rax        # b5e68 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movaps %xmm0,0x480(%rsp)
 	mov    0x8(%rax),%rbx
 	mov    0x10(%rax),%rax
 	movaps %xmm0,0x490(%rsp)
 	movq   $0x0,0x470(%rsp)
 	mov    -0x18(%rbx),%rdi
 	mov    %rbx,0x340(%rsp)
 	mov    %rax,0x28(%rsp)
 	add    %r12,%rdi
 	mov    %rax,(%rdi)
 	call   10e20 <std::basic_ios<char, std::char_traits<char> >::init(std::basic_streambuf<char, std::char_traits<char> >*)@plt>
-	mov    0x94e9b(%rip),%rax        # b5d68 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x94ea3(%rip),%rax        # b5d70 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	lea    0x348(%rsp),%r15
 	lea    0x18(%rax),%rcx
 	mov    %rax,0x18(%rsp)
 	add    $0x40,%rax
 	mov    %rax,0x398(%rsp)
 	mov    0x950b7(%rip),%rax        # b5fa8 <vtable for std::basic_streambuf<char, std::char_traits<char> >@GLIBCXX_3.4>
 	movq   %rcx,%xmm0
@@ -15127,15 +15127,15 @@
 	mov    %rax,0x38(%rsp)
 	movaps %xmm0,0x340(%rsp)
 	pxor   %xmm0,%xmm0
 	movaps %xmm0,0x350(%rsp)
 	movaps %xmm0,0x360(%rsp)
 	movaps %xmm0,0x370(%rsp)
 	call   10fe0 <std::locale::locale()@plt>
-	mov    0x94f6b(%rip),%rax        # b5eb8 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x94f73(%rip),%rax        # b5ec0 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	mov    %r15,%rsi
 	mov    %r14,%rdi
 	mov    0x94dce(%rip),%r13        
 	movl   $0x10,0x388(%rsp)
 	mov    %rax,0x20(%rsp)
 	add    $0x10,%rax
 	mov    %rax,0x348(%rsp)
@@ -15221,15 +15221,15 @@
 	lea    -0x18(%rax),%rdi
 	cmp    %r13,%rdi
 	jne    21c57 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0xee7>
 	mov    0x70(%rsp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    %r13,%rdi
 	je     20de3 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x73>
-	cmpq   $0x0,0x94cf3(%rip)        
+	cmpq   $0x0,0x94cfb(%rip)        
 	je     21db3 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x1043>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     20de3 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x73>
 	mov    %rbp,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -15248,26 +15248,26 @@
 	xor    %esi,%esi
 	movaps %xmm0,0x5e0(%rsp)
 	mov    %rax,0x8(%rsp)
 	add    $0x10,%rax
 	mov    %rax,0x4f8(%rsp)
 	xor    %eax,%eax
 	mov    %ax,0x5d8(%rsp)
-	mov    0x94cb2(%rip),%rax        # b5e60 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x94cba(%rip),%rax        # b5e68 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movaps %xmm0,0x5f0(%rsp)
 	movq   $0x0,0x5d0(%rsp)
 	mov    0x8(%rax),%rbx
 	mov    0x10(%rax),%rax
 	mov    -0x18(%rbx),%rdi
 	mov    %rbx,0x4a0(%rsp)
 	mov    %rax,0x28(%rsp)
 	add    %rbp,%rdi
 	mov    %rax,(%rdi)
 	call   10e20 <std::basic_ios<char, std::char_traits<char> >::init(std::basic_streambuf<char, std::char_traits<char> >*)@plt>
-	mov    0x94b7b(%rip),%rax        # b5d68 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x94b83(%rip),%rax        # b5d70 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	lea    0x4a8(%rsp),%r15
 	lea    0x18(%rax),%rcx
 	mov    %rax,0x18(%rsp)
 	add    $0x40,%rax
 	mov    %rax,0x4f8(%rsp)
 	mov    0x94d97(%rip),%rax        # b5fa8 <vtable for std::basic_streambuf<char, std::char_traits<char> >@GLIBCXX_3.4>
 	movq   %rcx,%xmm0
@@ -15281,15 +15281,15 @@
 	mov    %rax,0x38(%rsp)
 	movaps %xmm0,0x4a0(%rsp)
 	pxor   %xmm0,%xmm0
 	movaps %xmm0,0x4b0(%rsp)
 	movaps %xmm0,0x4c0(%rsp)
 	movaps %xmm0,0x4d0(%rsp)
 	call   10fe0 <std::locale::locale()@plt>
-	mov    0x94c4b(%rip),%rax        # b5eb8 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x94c53(%rip),%rax        # b5ec0 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	mov    %r15,%rsi
 	mov    %r14,%rdi
 	mov    0x94aae(%rip),%r13        
 	movl   $0x10,0x4e8(%rsp)
 	mov    %rax,0x20(%rsp)
 	add    $0x10,%rax
 	mov    %rax,0x4a8(%rsp)
@@ -15375,15 +15375,15 @@
 	lea    -0x18(%rax),%rdi
 	cmp    %r13,%rdi
 	jne    21d12 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0xfa2>
 	mov    0x78(%rsp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    %r13,%rdi
 	je     20df7 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x87>
-	cmpq   $0x0,0x949d3(%rip)        
+	cmpq   $0x0,0x949db(%rip)        
 	je     21e07 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x1097>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     20df7 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x87>
 	mov    %rbp,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -15402,28 +15402,28 @@
 	xor    %esi,%esi
 	pxor   %xmm0,%xmm0
 	mov    %si,0x1b8(%rsp)
 	xor    %esi,%esi
 	mov    %rax,0x8(%rsp)
 	add    $0x10,%rax
 	mov    %rax,0xd8(%rsp)
-	mov    0x94995(%rip),%rax        # b5e60 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x9499d(%rip),%rax        # b5e68 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movaps %xmm0,0x1c0(%rsp)
 	mov    0x8(%rax),%rcx
 	mov    0x10(%rax),%rax
 	movaps %xmm0,0x1d0(%rsp)
 	movq   $0x0,0x1b0(%rsp)
 	mov    -0x18(%rcx),%rdi
 	mov    %rcx,0x80(%rsp)
 	mov    %rcx,0x30(%rsp)
 	add    %r14,%rdi
 	mov    %rax,0x38(%rsp)
 	mov    %rax,(%rdi)
 	call   10e20 <std::basic_ios<char, std::char_traits<char> >::init(std::basic_streambuf<char, std::char_traits<char> >*)@plt>
-	mov    0x94851(%rip),%rax        # b5d68 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x94859(%rip),%rax        # b5d70 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	lea    0x88(%rsp),%r14
 	lea    0x18(%rax),%rcx
 	mov    %rax,0x18(%rsp)
 	add    $0x40,%rax
 	mov    %rax,0xd8(%rsp)
 	mov    0x94a6d(%rip),%rax        # b5fa8 <vtable for std::basic_streambuf<char, std::char_traits<char> >@GLIBCXX_3.4>
 	movq   %rcx,%xmm0
@@ -15437,15 +15437,15 @@
 	mov    %rax,0x48(%rsp)
 	movaps %xmm0,0x80(%rsp)
 	pxor   %xmm0,%xmm0
 	movaps %xmm0,0x90(%rsp)
 	movaps %xmm0,0xa0(%rsp)
 	movaps %xmm0,0xb0(%rsp)
 	call   10fe0 <std::locale::locale()@plt>
-	mov    0x94921(%rip),%rax        # b5eb8 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x94929(%rip),%rax        # b5ec0 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	mov    %r14,%rsi
 	mov    %r15,%rdi
 	mov    0x94784(%rip),%r13        
 	movl   $0x10,0xc8(%rsp)
 	mov    %rax,0x20(%rsp)
 	add    $0x10,%rax
 	mov    %rax,0x88(%rsp)
@@ -15532,15 +15532,15 @@
 	lea    -0x18(%rax),%rdi
 	cmp    %r13,%rdi
 	jne    21c25 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0xeb5>
 	mov    0x60(%rsp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    %r13,%rdi
 	je     20da8 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x38>
-	cmpq   $0x0,0x9469b(%rip)        
+	cmpq   $0x0,0x946a3(%rip)        
 	je     21d9a <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x102a>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     20da8 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x38>
 	mov    %rbp,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -15559,27 +15559,27 @@
 	xor    %ecx,%ecx
 	xor    %esi,%esi
 	pxor   %xmm0,%xmm0
 	mov    %cx,0x318(%rsp)
 	mov    %rax,0x8(%rsp)
 	add    $0x10,%rax
 	mov    %rax,0x238(%rsp)
-	mov    0x9465d(%rip),%rax        # b5e60 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x94665(%rip),%rax        # b5e68 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movaps %xmm0,0x320(%rsp)
 	mov    0x8(%rax),%rbx
 	mov    0x10(%rax),%rax
 	movaps %xmm0,0x330(%rsp)
 	movq   $0x0,0x310(%rsp)
 	mov    -0x18(%rbx),%rdi
 	mov    %rbx,0x1e0(%rsp)
 	mov    %rax,0x30(%rsp)
 	add    %r15,%rdi
 	mov    %rax,(%rdi)
 	call   10e20 <std::basic_ios<char, std::char_traits<char> >::init(std::basic_streambuf<char, std::char_traits<char> >*)@plt>
-	mov    0x9451e(%rip),%rax        # b5d68 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x94526(%rip),%rax        # b5d70 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	lea    0x1e8(%rsp),%r15
 	lea    0x18(%rax),%rcx
 	mov    %rax,0x18(%rsp)
 	add    $0x40,%rax
 	mov    %rax,0x238(%rsp)
 	mov    0x9473a(%rip),%rax        # b5fa8 <vtable for std::basic_streambuf<char, std::char_traits<char> >@GLIBCXX_3.4>
 	movq   %rcx,%xmm0
@@ -15593,15 +15593,15 @@
 	mov    %rax,0x40(%rsp)
 	movaps %xmm0,0x1e0(%rsp)
 	pxor   %xmm0,%xmm0
 	movaps %xmm0,0x1f0(%rsp)
 	movaps %xmm0,0x200(%rsp)
 	movaps %xmm0,0x210(%rsp)
 	call   10fe0 <std::locale::locale()@plt>
-	mov    0x945ee(%rip),%rax        # b5eb8 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x945f6(%rip),%rax        # b5ec0 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	mov    %r15,%rsi
 	mov    %r14,%rdi
 	mov    0x94451(%rip),%r13        
 	movl   $0x10,0x228(%rsp)
 	mov    %rax,0x20(%rsp)
 	add    $0x10,%rax
 	mov    %rax,0x1e8(%rsp)
@@ -15687,15 +15687,15 @@
 	lea    -0x18(%rax),%rdi
 	cmp    %r13,%rdi
 	jne    21ce3 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0xf73>
 	mov    0x68(%rsp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    %r13,%rdi
 	je     20dba <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x4a>
-	cmpq   $0x0,0x9436d(%rip)        
+	cmpq   $0x0,0x94375(%rip)        
 	je     21dcf <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x105f>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     20dba <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x4a>
 	mov    %rbp,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -15771,78 +15771,78 @@
 	call   106c0 <std::string::assign(std::string const&)@plt>
 	jmp    21015 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x2a5>
 	nopl   (%rax)
 	lea    0x230(%rsp),%rsi
 	mov    %r15,%rdi
 	call   106c0 <std::string::assign(std::string const&)@plt>
 	jmp    21996 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0xc26>
-	cmpq   $0x0,0x941eb(%rip)        
+	cmpq   $0x0,0x941f3(%rip)        
 	je     21dc1 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x1051>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     21763 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x9f3>
 	lea    0x1e0(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    21763 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x9f3>
-	cmpq   $0x0,0x941b9(%rip)        
+	cmpq   $0x0,0x941c1(%rip)        
 	je     21deb <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x107b>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     2110b <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x39b>
 	lea    0x1e0(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    2110b <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x39b>
-	cmpq   $0x0,0x94187(%rip)        
+	cmpq   $0x0,0x9418f(%rip)        
 	je     21e23 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x10b3>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     216a9 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x939>
 	mov    %rbp,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    216a9 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x939>
-	cmpq   $0x0,0x9415a(%rip)        
+	cmpq   $0x0,0x94162(%rip)        
 	je     21ddd <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x106d>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     2105b <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x2eb>
 	mov    %rbp,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    2105b <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x2eb>
-	cmpq   $0x0,0x9412d(%rip)        
+	cmpq   $0x0,0x94135(%rip)        
 	je     21e15 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x10a5>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     21a91 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0xd21>
 	mov    0x28(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    21a91 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0xd21>
-	cmpq   $0x0,0x940fe(%rip)        
+	cmpq   $0x0,0x94106(%rip)        
 	je     21df9 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x1089>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     2142b <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x6bb>
 	lea    0x1e0(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    2142b <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x6bb>
-	cmpq   $0x0,0x940cc(%rip)        
+	cmpq   $0x0,0x940d4(%rip)        
 	je     21e31 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x10c1>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     219dc <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0xc6c>
 	mov    %rbp,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
 	jmp    219dc <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0xc6c>
-	cmpq   $0x0,0x9409f(%rip)        
+	cmpq   $0x0,0x940a7(%rip)        
 	je     21da8 <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x1038>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     2137b <c10::cuda::impl::CUDAGuardImpl::destroyEvent(void*, signed char) const+0x60b>
 	mov    %r12,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -16019,25 +16019,25 @@
 	xor    %esi,%esi
 	movaps %xmm0,0x180(%rsp)
 	add    $0x10,%rax
 	movaps %xmm0,0x190(%rsp)
 	mov    %rax,0x98(%rsp)
 	xor    %eax,%eax
 	mov    %ax,0x178(%rsp)
-	mov    0x93dfe(%rip),%rax        # b5e60 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x93e06(%rip),%rax        # b5e68 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movq   $0x0,0x170(%rsp)
 	mov    0x8(%rax),%r15
 	mov    0x10(%rax),%rax
 	mov    -0x18(%r15),%rdi
 	mov    %r15,0x40(%rsp)
 	mov    %rax,0x8(%rsp)
 	add    %rbp,%rdi
 	mov    %rax,(%rdi)
 	call   10e20 <std::basic_ios<char, std::char_traits<char> >::init(std::basic_streambuf<char, std::char_traits<char> >*)@plt>
-	mov    0x93cd2(%rip),%rax        # b5d68 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x93cda(%rip),%rax        # b5d70 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	lea    0x48(%rsp),%r14
 	lea    0x18(%rax),%rbx
 	add    $0x40,%rax
 	mov    %rax,0x98(%rsp)
 	mov    0x93ef6(%rip),%rax        # b5fa8 <vtable for std::basic_streambuf<char, std::char_traits<char> >@GLIBCXX_3.4>
 	movq   %rbx,%xmm0
 	mov    %rbx,0x10(%rsp)
@@ -16048,15 +16048,15 @@
 	punpcklqdq %xmm1,%xmm0
 	movaps %xmm0,0x40(%rsp)
 	pxor   %xmm0,%xmm0
 	movaps %xmm0,0x50(%rsp)
 	movaps %xmm0,0x60(%rsp)
 	movaps %xmm0,0x70(%rsp)
 	call   10fe0 <std::locale::locale()@plt>
-	mov    0x93dc0(%rip),%rax        # b5eb8 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x93dc8(%rip),%rax        # b5ec0 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	mov    %r14,%rsi
 	mov    %r13,%rdi
 	movl   $0x10,0x88(%rsp)
 	add    $0x10,%rax
 	mov    %rax,0x48(%rsp)
 	mov    0x93c0f(%rip),%rax        
 	add    $0x18,%rax
@@ -16099,19 +16099,19 @@
 	mov    -0x18(%rdx),%rdx
 	cmp    %r8,%rax
 	ja     22278 <c10::detail::_str_wrapper<char const*, c10::DeviceType const&, char const*>::call(char const* const&, c10::DeviceType const&, char const* const&)+0x288>
 	sub    %rcx,%r8
 	xor    %esi,%esi
 	mov    %r12,%rdi
 	call   10ad0 <std::string::replace(unsigned long, unsigned long, char const*, unsigned long)@plt>
-	mov    0x93b93(%rip),%rax        # b5d68 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x93b9b(%rip),%rax        # b5d70 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movq   0x10(%rsp),%xmm0
 	add    $0x40,%rax
 	mov    %rax,0x98(%rsp)
-	mov    0x93cca(%rip),%rax        # b5eb8 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x93cd2(%rip),%rax        # b5ec0 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	add    $0x10,%rax
 	movq   %rax,%xmm2
 	mov    0x90(%rsp),%rax
 	punpcklqdq %xmm2,%xmm0
 	lea    -0x18(%rax),%rdi
 	cmp    0x93b1a(%rip),%rdi        
 	movaps %xmm0,0x40(%rsp)
@@ -16164,15 +16164,15 @@
 	jmp    22151 <c10::detail::_str_wrapper<char const*, c10::DeviceType const&, char const*>::call(char const* const&, c10::DeviceType const&, char const* const&)+0x161>
 	nopl   0x0(%rax)
 	lea    0x90(%rsp),%rsi
 	mov    %r12,%rdi
 	call   106c0 <std::string::assign(std::string const&)@plt>
 	jmp    221ce <c10::detail::_str_wrapper<char const*, c10::DeviceType const&, char const*>::call(char const* const&, c10::DeviceType const&, char const* const&)+0x1de>
 	nopl   (%rax)
-	cmpq   $0x0,0x93b28(%rip)        
+	cmpq   $0x0,0x93b30(%rip)        
 	je     22318 <c10::detail::_str_wrapper<char const*, c10::DeviceType const&, char const*>::call(char const* const&, c10::DeviceType const&, char const* const&)+0x328>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     22219 <c10::detail::_str_wrapper<char const*, c10::DeviceType const&, char const*>::call(char const* const&, c10::DeviceType const&, char const* const&)+0x229>
 	mov    %r14,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -16368,15 +16368,15 @@
 	mov    0x9374f(%rip),%rax        
 	mov    (%rax),%eax
 	test   %eax,%eax
 	jne    22690 <c10::cuda::impl::CUDAGuardImpl::synchronizeStream(c10::Stream const&) const+0x120>
 	mov    0x939de(%rip),%rax        
 	cmpb   $0x0,(%rax)
 	je     2260e <c10::cuda::impl::CUDAGuardImpl::synchronizeStream(c10::Stream const&) const+0x9e>
-	mov    0x93752(%rip),%rax        
+	mov    0x9375a(%rip),%rax        
 	mov    (%rax),%rax
 	test   %rax,%rax
 	jne    22670 <c10::cuda::impl::CUDAGuardImpl::synchronizeStream(c10::Stream const&) const+0x100>
 	mov    %r12,%rdi
 	call   105e0 <cudaStreamSynchronize@plt>
 	mov    %eax,%edi
 	mov    $0x1,%r8d
@@ -16480,25 +16480,25 @@
 	xor    %esi,%esi
 	movaps %xmm0,0x180(%rsp)
 	add    $0x10,%rax
 	movaps %xmm0,0x190(%rsp)
 	mov    %rax,0x98(%rsp)
 	xor    %eax,%eax
 	mov    %ax,0x178(%rsp)
-	mov    0x9368e(%rip),%rax        # b5e60 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x93696(%rip),%rax        # b5e68 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movq   $0x0,0x170(%rsp)
 	mov    0x8(%rax),%r15
 	mov    0x10(%rax),%rax
 	mov    -0x18(%r15),%rdi
 	mov    %r15,0x40(%rsp)
 	mov    %rax,0x8(%rsp)
 	add    %rbp,%rdi
 	mov    %rax,(%rdi)
 	call   10e20 <std::basic_ios<char, std::char_traits<char> >::init(std::basic_streambuf<char, std::char_traits<char> >*)@plt>
-	mov    0x93562(%rip),%rax        # b5d68 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x9356a(%rip),%rax        # b5d70 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	lea    0x48(%rsp),%r14
 	lea    0x18(%rax),%rbx
 	add    $0x40,%rax
 	mov    %rax,0x98(%rsp)
 	mov    0x93786(%rip),%rax        # b5fa8 <vtable for std::basic_streambuf<char, std::char_traits<char> >@GLIBCXX_3.4>
 	movq   %rbx,%xmm0
 	mov    %rbx,0x10(%rsp)
@@ -16509,15 +16509,15 @@
 	punpcklqdq %xmm1,%xmm0
 	movaps %xmm0,0x40(%rsp)
 	pxor   %xmm0,%xmm0
 	movaps %xmm0,0x50(%rsp)
 	movaps %xmm0,0x60(%rsp)
 	movaps %xmm0,0x70(%rsp)
 	call   10fe0 <std::locale::locale()@plt>
-	mov    0x93650(%rip),%rax        # b5eb8 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x93658(%rip),%rax        # b5ec0 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	mov    %r14,%rsi
 	mov    %r13,%rdi
 	movl   $0x10,0x88(%rsp)
 	add    $0x10,%rax
 	mov    %rax,0x48(%rsp)
 	mov    0x9349f(%rip),%rax        
 	add    $0x18,%rax
@@ -16560,19 +16560,19 @@
 	mov    -0x18(%rdx),%rdx
 	cmp    %r8,%rax
 	ja     229e8 <c10::detail::_str_wrapper<char const*, long const&, char const*>::call(char const* const&, long const&, char const* const&)+0x288>
 	sub    %rcx,%r8
 	xor    %esi,%esi
 	mov    %r12,%rdi
 	call   10ad0 <std::string::replace(unsigned long, unsigned long, char const*, unsigned long)@plt>
-	mov    0x93423(%rip),%rax        # b5d68 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x9342b(%rip),%rax        # b5d70 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movq   0x10(%rsp),%xmm0
 	add    $0x40,%rax
 	mov    %rax,0x98(%rsp)
-	mov    0x9355a(%rip),%rax        # b5eb8 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x93562(%rip),%rax        # b5ec0 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	add    $0x10,%rax
 	movq   %rax,%xmm2
 	mov    0x90(%rsp),%rax
 	punpcklqdq %xmm2,%xmm0
 	lea    -0x18(%rax),%rdi
 	cmp    0x933aa(%rip),%rdi        
 	movaps %xmm0,0x40(%rsp)
@@ -16625,15 +16625,15 @@
 	jmp    228c1 <c10::detail::_str_wrapper<char const*, long const&, char const*>::call(char const* const&, long const&, char const* const&)+0x161>
 	nopl   0x0(%rax)
 	lea    0x90(%rsp),%rsi
 	mov    %r12,%rdi
 	call   106c0 <std::string::assign(std::string const&)@plt>
 	jmp    2293e <c10::detail::_str_wrapper<char const*, long const&, char const*>::call(char const* const&, long const&, char const* const&)+0x1de>
 	nopl   (%rax)
-	cmpq   $0x0,0x933b8(%rip)        
+	cmpq   $0x0,0x933c0(%rip)        
 	je     22a88 <c10::detail::_str_wrapper<char const*, long const&, char const*>::call(char const* const&, long const&, char const* const&)+0x328>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     22989 <c10::detail::_str_wrapper<char const*, long const&, char const*>::call(char const* const&, long const&, char const* const&)+0x229>
 	mov    %r14,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -16702,25 +16702,25 @@
 	xor    %esi,%esi
 	movaps %xmm0,0x190(%rsp)
 	add    $0x10,%rax
 	movaps %xmm0,0x1a0(%rsp)
 	mov    %rax,0xa8(%rsp)
 	xor    %eax,%eax
 	mov    %ax,0x188(%rsp)
-	mov    0x932c6(%rip),%rax        # b5e60 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x932ce(%rip),%rax        # b5e68 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movq   $0x0,0x180(%rsp)
 	mov    0x8(%rax),%r15
 	mov    0x10(%rax),%rax
 	mov    -0x18(%r15),%rdi
 	mov    %r15,0x50(%rsp)
 	mov    %rax,0x8(%rsp)
 	add    %rbp,%rdi
 	mov    %rax,(%rdi)
 	call   10e20 <std::basic_ios<char, std::char_traits<char> >::init(std::basic_streambuf<char, std::char_traits<char> >*)@plt>
-	mov    0x9319a(%rip),%rax        # b5d68 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x931a2(%rip),%rax        # b5d70 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	lea    0x58(%rsp),%r13
 	lea    0x18(%rax),%rcx
 	add    $0x40,%rax
 	mov    %rax,0xa8(%rsp)
 	mov    0x933be(%rip),%rax        # b5fa8 <vtable for std::basic_streambuf<char, std::char_traits<char> >@GLIBCXX_3.4>
 	movq   %rcx,%xmm0
 	mov    %rcx,0x10(%rsp)
@@ -16732,15 +16732,15 @@
 	mov    %rax,0x38(%rsp)
 	movaps %xmm0,0x50(%rsp)
 	pxor   %xmm0,%xmm0
 	movaps %xmm0,0x60(%rsp)
 	movaps %xmm0,0x70(%rsp)
 	movaps %xmm0,0x80(%rsp)
 	call   10fe0 <std::locale::locale()@plt>
-	mov    0x93280(%rip),%rax        # b5eb8 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x93288(%rip),%rax        # b5ec0 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	mov    %r13,%rsi
 	mov    %rbx,%rdi
 	movl   $0x10,0x98(%rsp)
 	add    $0x10,%rax
 	mov    %rax,0x58(%rsp)
 	mov    0x930cf(%rip),%rax        
 	add    $0x18,%rax
@@ -16805,19 +16805,19 @@
 	mov    -0x18(%rdx),%rdx
 	cmp    %r8,%rax
 	ja     22e10 <c10::detail::_str_wrapper<char const&, char const* const&, char const*, char const* const&, char const*>::call(char const&, char const* const&, char const* const&, char const* const&, char const* const&)+0x2f0>
 	sub    %rcx,%r8
 	xor    %esi,%esi
 	mov    %r12,%rdi
 	call   10ad0 <std::string::replace(unsigned long, unsigned long, char const*, unsigned long)@plt>
-	mov    0x92ffa(%rip),%rax        # b5d68 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x93002(%rip),%rax        # b5d70 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movq   0x10(%rsp),%xmm0
 	add    $0x40,%rax
 	mov    %rax,0xa8(%rsp)
-	mov    0x93131(%rip),%rax        # b5eb8 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x93139(%rip),%rax        # b5ec0 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	add    $0x10,%rax
 	movq   %rax,%xmm2
 	mov    0xa0(%rsp),%rax
 	punpcklqdq %xmm2,%xmm0
 	lea    -0x18(%rax),%rdi
 	cmp    0x92f81(%rip),%rdi        
 	movaps %xmm0,0x50(%rsp)
@@ -16886,15 +16886,15 @@
 	jmp    22cae <c10::detail::_str_wrapper<char const&, char const* const&, char const*, char const* const&, char const*>::call(char const&, char const* const&, char const* const&, char const* const&, char const* const&)+0x18e>
 	nopl   0x0(%rax)
 	lea    0xa0(%rsp),%rsi
 	mov    %r12,%rdi
 	call   106c0 <std::string::assign(std::string const&)@plt>
 	jmp    22d67 <c10::detail::_str_wrapper<char const&, char const* const&, char const*, char const* const&, char const*>::call(char const&, char const* const&, char const* const&, char const* const&, char const* const&)+0x247>
 	nopl   (%rax)
-	cmpq   $0x0,0x92f50(%rip)        
+	cmpq   $0x0,0x92f58(%rip)        
 	je     22ef0 <c10::detail::_str_wrapper<char const&, char const* const&, char const*, char const* const&, char const*>::call(char const&, char const* const&, char const* const&, char const* const&, char const* const&)+0x3d0>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     22db2 <c10::detail::_str_wrapper<char const&, char const* const&, char const*, char const* const&, char const*>::call(char const&, char const* const&, char const* const&, char const* const&, char const* const&)+0x292>
 	mov    %r14,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -17164,26 +17164,26 @@
 	mov    0x38(%rsp),%rax
 	mov    0xc(%rax),%eax
 	cmp    $0x1,%eax
 	je     23339 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x3b9>
 	mov    0x38(%rsp),%rdi
 	mov    (%rdi),%rax
 	mov    0x10(%rax),%rax
-	cmp    0x92b40(%rip),%rax        
+	cmp    0x92b48(%rip),%rax        
 	jne    233f8 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x478>
 	lock subl $0x1,0xc(%rdi)
 	jne    23044 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0xc4>
 	mov    0x38(%rsp),%rdi
 	test   %rdi,%rdi
 	je     23044 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0xc4>
 	mov    (%rdi),%rax
 	mov    0x8(%rax),%rax
-	cmp    0x92aa3(%rip),%rax        
+	cmp    0x92aab(%rip),%rax        
 	jne    234a4 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x524>
-	mov    0x92bbe(%rip),%rax        
+	mov    0x92bc6(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	mov    0x8(%rdi),%eax
 	test   %eax,%eax
 	je     2337e <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x3fe>
 	mov    0x8(%rdi),%eax
 	cmp    $0xffffffe,%eax
@@ -17221,26 +17221,26 @@
 	mov    0x18(%rsp),%rax
 	mov    0xc(%rax),%eax
 	cmp    $0x1,%eax
 	je     23441 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x4c1>
 	mov    0x18(%rsp),%rdi
 	mov    (%rdi),%rax
 	mov    0x10(%rax),%rax
-	cmp    0x92a38(%rip),%rax        
+	cmp    0x92a40(%rip),%rax        
 	jne    23500 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x580>
 	lock subl $0x1,0xc(%rdi)
 	jne    23019 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x99>
 	mov    0x18(%rsp),%rdi
 	test   %rdi,%rdi
 	je     23019 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x99>
 	mov    (%rdi),%rax
 	mov    0x8(%rax),%rax
-	cmp    0x9299b(%rip),%rax        
+	cmp    0x929a3(%rip),%rax        
 	jne    2350c <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x58c>
-	mov    0x92ab6(%rip),%rax        
+	mov    0x92abe(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	mov    0x8(%rdi),%eax
 	test   %eax,%eax
 	je     23486 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoRuntimeFunctor_<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double), at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)+0x506>
 	mov    0x8(%rdi),%eax
 	cmp    $0xffffffe,%eax
@@ -17409,15 +17409,15 @@
 std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (*)(at::Tensor const&, at::Tensor const&, double)>():
 	push   %r12
 	mov    $0x1,%r8d
 	mov    %rdi,%r12
 	mov    $0x3,%edx
 	push   %rbp
 	sub    $0x98,%rsp
-	movq   0x92680(%rip),%xmm0        # b5e20 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<at::Tensor>()@@Base+0xa06c0>
+	movq   0x92688(%rip),%xmm0        # b5e28 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<at::Tensor>()@@Base+0xa06c8>
 	movq   0x92848(%rip),%xmm1        # b5ff0 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<double>()@@Base+0x97b80>
 	lea    0x40(%rsp),%rbp
 	mov    %rsp,%rcx
 	lea    0x10(%rsp),%rsi
 	movhps 0x9252c(%rip),%xmm0        # b5ce8 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getFakeTypePtrCopy<at::Tensor>()@@Base+0xa0538>
 	movhps 0x927b5(%rip),%xmm1        # b5f78 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getFakeTypePtrCopy<double>()@@Base+0x97b28>
 	mov    %rbp,%rdi
@@ -17576,27 +17576,27 @@
 	movzbl 0x40(%rbp),%eax
 	test   %al,%al
 	jne    23b10 <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x2c0>
 	cmpq   $0x0,0x20(%rbp)
 	je     23a90 <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x240>
 	mov    0x20(%rbp),%r12
 	je     23a90 <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x240>
-	mov    0x923ae(%rip),%rbx        
+	mov    0x923b6(%rip),%rbx        
 	test   %rbx,%rbx
 	je     23bf8 <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x3a8>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x8(%r12)
 	cmp    $0x1,%eax
 	je     23c0e <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x3be>
 	nopl   0x0(%rax,%rax,1)
 	cmpq   $0x0,0x10(%rbp)
 	je     23ac8 <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x278>
 	mov    0x10(%rbp),%r12
 	je     23ac8 <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x278>
-	mov    0x92374(%rip),%rbx        
+	mov    0x9237c(%rip),%rbx        
 	test   %rbx,%rbx
 	je     23ba8 <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x358>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x8(%r12)
 	cmp    $0x1,%eax
 	je     23bbe <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x36e>
 	nopw   0x0(%rax,%rax,1)
@@ -17692,15 +17692,15 @@
 	cmp    $0x1,%eax
 	jne    23a90 <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x240>
 	mov    (%r12),%rax
 	mov    %r12,%rdi
 	call   *0x18(%rax)
 	jmp    23a90 <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x240>
 	nopl   0x0(%rax)
-	cmpq   $0x0,0x921c8(%rip)        
+	cmpq   $0x0,0x921d0(%rip)        
 	je     23c78 <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x428>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     23add <std::vector<c10::Argument, std::allocator<c10::Argument> >::~vector()+0x28d>
 	lea    0x1f(%rsp),%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -18577,27 +18577,27 @@
 	xor    %esi,%esi
 	movaps %xmm0,0x190(%rsp)
 	mov    %rax,0x8(%rsp)
 	add    $0x10,%rax
 	mov    %rax,0xa8(%rsp)
 	xor    %eax,%eax
 	mov    %ax,0x188(%rsp)
-	mov    0x9137c(%rip),%rax        # b5e60 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x91384(%rip),%rax        # b5e68 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movaps %xmm0,0x1a0(%rsp)
 	movq   $0x0,0x180(%rsp)
 	mov    0x8(%rax),%rbx
 	mov    0x10(%rax),%rax
 	mov    -0x18(%rbx),%rdi
 	mov    %rbx,0x50(%rsp)
 	mov    %rbx,0x28(%rsp)
 	add    %rbp,%rdi
 	mov    %rax,0x30(%rsp)
 	mov    %rax,(%rdi)
 	call   10e20 <std::basic_ios<char, std::char_traits<char> >::init(std::basic_streambuf<char, std::char_traits<char> >*)@plt>
-	mov    0x91243(%rip),%rbx        # b5d68 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x9124b(%rip),%rbx        # b5d70 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	lea    0x58(%rsp),%r15
 	lea    0x40(%rbx),%rax
 	lea    0x18(%rbx),%rcx
 	mov    %rax,0xa8(%rsp)
 	mov    0x91467(%rip),%rax        # b5fa8 <vtable for std::basic_streambuf<char, std::char_traits<char> >@GLIBCXX_3.4>
 	movq   %rcx,%xmm0
 	mov    %rcx,0x38(%rsp)
@@ -18610,15 +18610,15 @@
 	mov    %rax,0x10(%rsp)
 	movaps %xmm0,0x50(%rsp)
 	pxor   %xmm0,%xmm0
 	movaps %xmm0,0x60(%rsp)
 	movaps %xmm0,0x70(%rsp)
 	movaps %xmm0,0x80(%rsp)
 	call   10fe0 <std::locale::locale()@plt>
-	mov    0x91324(%rip),%rax        # b5eb8 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x9132c(%rip),%rax        # b5ec0 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	mov    %r15,%rsi
 	mov    %r14,%rdi
 	movl   $0x10,0x98(%rsp)
 	mov    %rax,0x18(%rsp)
 	add    $0x10,%rax
 	mov    %rax,0x58(%rsp)
 	mov    0x9116e(%rip),%rax        
@@ -18704,27 +18704,27 @@
 	xor    %esi,%esi
 	pxor   %xmm0,%xmm0
 	mov    %si,0x188(%rsp)
 	xor    %esi,%esi
 	mov    %rax,0x8(%rsp)
 	add    $0x10,%rax
 	mov    %rax,0xa8(%rsp)
-	mov    0x910fc(%rip),%rax        # b5e60 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x91104(%rip),%rax        # b5e68 <VTT for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	movaps %xmm0,0x190(%rsp)
 	mov    0x8(%rax),%r13
 	mov    0x10(%rax),%rax
 	movaps %xmm0,0x1a0(%rsp)
 	movq   $0x0,0x180(%rsp)
 	mov    -0x18(%r13),%rdi
 	mov    %r13,0x50(%rsp)
 	mov    %rax,0x28(%rsp)
 	add    %rbp,%rdi
 	mov    %rax,(%rdi)
 	call   10e20 <std::basic_ios<char, std::char_traits<char> >::init(std::basic_streambuf<char, std::char_traits<char> >*)@plt>
-	mov    0x90fc0(%rip),%rbx        # b5d68 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x90fc8(%rip),%rbx        # b5d70 <vtable for std::basic_ostringstream<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	lea    0x58(%rsp),%r15
 	lea    0x40(%rbx),%rax
 	lea    0x18(%rbx),%rcx
 	mov    %rax,0xa8(%rsp)
 	mov    0x911e4(%rip),%rax        # b5fa8 <vtable for std::basic_streambuf<char, std::char_traits<char> >@GLIBCXX_3.4>
 	movq   %rcx,%xmm0
 	mov    %rcx,0x30(%rsp)
@@ -18737,15 +18737,15 @@
 	mov    %rax,0x10(%rsp)
 	movaps %xmm0,0x50(%rsp)
 	pxor   %xmm0,%xmm0
 	movaps %xmm0,0x60(%rsp)
 	movaps %xmm0,0x70(%rsp)
 	movaps %xmm0,0x80(%rsp)
 	call   10fe0 <std::locale::locale()@plt>
-	mov    0x910a1(%rip),%rax        # b5eb8 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
+	mov    0x910a9(%rip),%rax        # b5ec0 <vtable for std::basic_stringbuf<char, std::char_traits<char>, std::allocator<char> >@GLIBCXX_3.4>
 	mov    %r15,%rsi
 	mov    %r14,%rdi
 	movl   $0x10,0x98(%rsp)
 	mov    %rax,0x18(%rsp)
 	add    $0x10,%rax
 	mov    %rax,0x58(%rsp)
 	mov    0x90eeb(%rip),%rax        
@@ -18889,15 +18889,15 @@
 	jmp    24967 <torchao::weight_matrix_prepacking_cpu(at::Tensor)+0x57>
 	nopl   0x0(%rax)
 	lea    0xa0(%rsp),%rsi
 	mov    %r12,%rdi
 	call   106c0 <std::string::assign(std::string const&)@plt>
 	jmp    24ed4 <torchao::weight_matrix_prepacking_cpu(at::Tensor)+0x5c4>
 	nopl   (%rax)
-	cmpq   $0x0,0x90d48(%rip)        
+	cmpq   $0x0,0x90d50(%rip)        
 	je     2515a <torchao::weight_matrix_prepacking_cpu(at::Tensor)+0x84a>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     24cb2 <torchao::weight_matrix_prepacking_cpu(at::Tensor)+0x3a2>
 	mov    %r15,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -18912,15 +18912,15 @@
 	nopl   0x0(%rax)
 	xor    %edx,%edx
 	mov    %rax,%rsi
 	xor    %edi,%edi
 	call   111b0 <long c10::detail::maybe_wrap_dim_slow<long>(long, long, bool)@plt>
 	lea    0x0(,%rax,8),%rbx
 	jmp    24f9e <torchao::weight_matrix_prepacking_cpu(at::Tensor)+0x68e>
-	cmpq   $0x0,0x90cdf(%rip)        
+	cmpq   $0x0,0x90ce7(%rip)        
 	je     25168 <torchao::weight_matrix_prepacking_cpu(at::Tensor)+0x858>
 	mov    $0xffffffff,%edx
 	lock xadd %edx,-0x8(%rax)
 	test   %edx,%edx
 	jg     24f13 <torchao::weight_matrix_prepacking_cpu(at::Tensor)+0x603>
 	mov    %r15,%rsi
 	call   10810 <std::string::_Rep::_M_destroy(std::allocator<char> const&)@plt>
@@ -18961,24 +18961,24 @@
 std::bad_optional_access::what() const:
 	lea    0x1123c(%rip),%rax        
 	ret
 	nopl   0x0(%rax,%rax,1)
 
 00000000000251e0 <std::bad_optional_access::~bad_optional_access()>:
 std::bad_optional_access::~bad_optional_access():
-	mov    0x90af1(%rip),%rax        
+	mov    0x90ae9(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	jmp    100e0 <std::exception::~exception()@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
 0000000000025200 <std::bad_optional_access::~bad_optional_access()>:
 std::bad_optional_access::~bad_optional_access():
-	mov    0x90ad1(%rip),%rax        
+	mov    0x90ac9(%rip),%rax        
 	push   %rbp
 	mov    %rdi,%rbp
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	call   100e0 <std::exception::~exception()@plt>
 	mov    %rbp,%rdi
 	mov    $0x8,%esi
@@ -19083,15 +19083,15 @@
 std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (*)(at::Tensor)>():
 	push   %r12
 	mov    $0x1,%r8d
 	mov    %rdi,%r12
 	mov    $0x1,%edx
 	push   %rbp
 	sub    $0x78,%rsp
-	movq   0x90a93(%rip),%xmm0        # b5e20 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<at::Tensor>()@@Base+0xa06c0>
+	movq   0x90a9b(%rip),%xmm0        # b5e28 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<at::Tensor>()@@Base+0xa06c8>
 	lea    0x20(%rsp),%rbp
 	lea    0x10(%rsp),%rcx
 	mov    %rsp,%rsi
 	movhps 0x90947(%rip),%xmm0        # b5ce8 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getFakeTypePtrCopy<at::Tensor>()@@Base+0xa0538>
 	mov    %rbp,%rdi
 	movaps %xmm0,(%rsp)
 	movaps %xmm0,0x10(%rsp)
@@ -19121,15 +19121,15 @@
 	call   11180 <c10::FunctionSchema::~FunctionSchema()@plt>
 	mov    %r12,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	nopw   0x0(%rax,%rax,1)
 
 0000000000025420 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]>:
 std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]:
-	cmpq   $0x0,0x909f0(%rip)        
+	cmpq   $0x0,0x909f8(%rip)        
 	je     25440 <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x20>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x10(%rdi)
 	test   %eax,%eax
 	jle    2544d <std::string::_Rep::_M_dispose(std::allocator<char> const&) [clone .part.0]+0x2d>
 	ret
 	nopl   0x0(%rax)
@@ -19228,15 +19228,15 @@
 	push   %r12
 	push   %rbp
 	sub    $0x18,%rsp
 	call   111f0 <Py_GetVersion@plt>
 	cmpb   $0x33,(%rax)
 	mov    %rax,%rcx
 	je     255e0 <PyInit__C+0x40>
-	mov    0x908b5(%rip),%rax        
+	mov    0x908bd(%rip),%rax        
 	lea    0x117f0(%rip),%rdx        
 	lea    0x117f7(%rip),%rsi        
 	mov    (%rax),%rdi
 	xor    %eax,%eax
 	call   112f0 <PyErr_Format@plt>
 	xor    %eax,%eax
 	add    $0x18,%rsp
@@ -19287,27 +19287,27 @@
 	je     11c9b <PyInit__C.cold>
 	jmp    11ca7 <PyInit__C.cold+0xc>
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
 00000000000256d0 <pybind11_static_get>:
 pybind11_static_get():
-	mov    0x90851(%rip),%rax        
+	mov    0x90859(%rip),%rax        
 	mov    %rdx,%rsi
 	mov    0x110(%rax),%rax
 	jmp    *%rax
 	cs nopw 0x0(%rax,%rax,1)
 	nopl   (%rax)
 
 00000000000256f0 <pybind11_static_set>:
 pybind11_static_set():
 	mov    0x8(%rsi),%rax
 	testb  $0x80,0xab(%rax)
 	cmove  %rax,%rsi
-	mov    0x90822(%rip),%rax        
+	mov    0x9082a(%rip),%rax        
 	jmp    *0x118(%rax)
 	nopl   0x0(%rax)
 
 0000000000025710 <std::_Sp_counted_deleter<pybind11::detail::error_fetch_and_normalize*, void (*)(pybind11::detail::error_fetch_and_normalize*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>::~_Sp_counted_deleter()>:
 std::_Sp_counted_deleter<pybind11::detail::error_fetch_and_normalize*, void (*)(pybind11::detail::error_fetch_and_normalize*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>::~_Sp_counted_deleter():
 	ret
 	cs nopw 0x0(%rax,%rax,1)
@@ -19401,15 +19401,15 @@
 	sub    $0x8,%rsp
 	call   10590 <_PyType_Lookup@plt>
 	test   %rax,%rax
 	je     25824 <pybind11_meta_getattro+0x24>
 	mov    0x9049a(%rip),%rdx        
 	cmp    %rdx,0x8(%rax)
 	je     25848 <pybind11_meta_getattro+0x48>
-	mov    0x906e5(%rip),%rax        
+	mov    0x906ed(%rip),%rax        
 	mov    %r12,%rsi
 	mov    %rbp,%rdi
 	mov    0x90(%rax),%rax
 	add    $0x8,%rsp
 	pop    %rbp
 	pop    %r12
 	jmp    *%rax
@@ -19533,15 +19533,15 @@
 	push   %rbp
 	mov    %rdi,%rbp
 	push   %rbx
 	mov    0x10(%rdi),%r12
 	mov    %rax,(%rdi)
 	test   %r12,%r12
 	je     25a07 <pybind11::error_already_set::~error_already_set()+0x37>
-	mov    0x90427(%rip),%rbx        
+	mov    0x9042f(%rip),%rbx        
 	test   %rbx,%rbx
 	je     25a20 <pybind11::error_already_set::~error_already_set()+0x50>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x8(%r12)
 	cmp    $0x1,%eax
 	je     25a32 <pybind11::error_already_set::~error_already_set()+0x62>
 	mov    %rbp,%rdi
@@ -19584,15 +19584,15 @@
 	push   %rbp
 	mov    %rdi,%rbp
 	push   %rbx
 	mov    0x10(%rdi),%r12
 	mov    %rax,(%rdi)
 	test   %r12,%r12
 	je     25aa7 <pybind11::error_already_set::~error_already_set()+0x37>
-	mov    0x90387(%rip),%rbx        
+	mov    0x9038f(%rip),%rbx        
 	test   %rbx,%rbx
 	je     25ab8 <pybind11::error_already_set::~error_already_set()+0x48>
 	mov    $0xffffffff,%eax
 	lock xadd %eax,0x8(%r12)
 	cmp    $0x1,%eax
 	je     25aca <pybind11::error_already_set::~error_already_set()+0x5a>
 	pop    %rbx
@@ -22338,15 +22338,15 @@
 	mov    %rdi,%r12
 	mov    0x8(%rbp),%rdi
 	mov    0xa8(%rdi),%rax
 	test   $0x10000000,%eax
 	jne    281b8 <pybind11::detail::type_caster<std::string, void>& pybind11::detail::load_type<std::string, void>(pybind11::detail::type_caster<std::string, void>&, pybind11::handle const&)+0xb8>
 	test   $0x8000000,%eax
 	jne    28220 <pybind11::detail::type_caster<std::string, void>& pybind11::detail::load_type<std::string, void>(pybind11::detail::type_caster<std::string, void>&, pybind11::handle const&)+0x120>
-	mov    0x8db9a(%rip),%rsi        
+	mov    0x8db92(%rip),%rsi        
 	cmp    %rsi,%rdi
 	je     28158 <pybind11::detail::type_caster<std::string, void>& pybind11::detail::load_type<std::string, void>(pybind11::detail::type_caster<std::string, void>&, pybind11::handle const&)+0x58>
 	call   10140 <PyType_IsSubtype@plt>
 	test   %eax,%eax
 	je     2824d <pybind11::detail::type_caster<std::string, void>& pybind11::detail::load_type<std::string, void>(pybind11::detail::type_caster<std::string, void>&, pybind11::handle const&)+0x14d>
 	mov    %rbp,%rdi
 	call   10090 <PyByteArray_AsString@plt>
@@ -23093,15 +23093,15 @@
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	ret
 	mov    %rax,%rbp
 	jmp    28d2d <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0xdd>
 	call   100c0 <__cxa_begin_catch@plt>
-	mov    0x8d142(%rip),%rdx        
+	mov    0x8d14a(%rip),%rdx        
 	mov    0x8d043(%rip),%rsi        
 	mov    $0xfffffffffffffffe,%rcx
 	mov    %rax,%rdi
 	mov    %rax,%r12
 	call   11220 <__dynamic_cast@plt>
 	mov    %rax,%rdi
 	test   %rax,%rax
@@ -23118,65 +23118,65 @@
 	jmp    28cc5 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x75>
 	call   11030 <__cxa_end_catch@plt>
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	mov    %rax,%rbp
 	jmp    28dee <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x19e>
 	call   100c0 <__cxa_begin_catch@plt>
-	mov    0x8d0da(%rip),%rdx        
-	mov    0x8d133(%rip),%rsi        
+	mov    0x8d0e2(%rip),%rdx        
+	mov    0x8d13b(%rip),%rsi        
 	mov    $0xfffffffffffffffe,%rcx
 	mov    %rax,%rdi
 	mov    %rax,%r12
 	call   11220 <__dynamic_cast@plt>
 	mov    %rax,%rdi
 	test   %rax,%rax
 	je     28d77 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x127>
 	mov    %rbp,%rsi
 	call   29120 <bool pybind11::detail::handle_nested_exception<std::nested_exception, 0>(std::nested_exception const&, std::__exception_ptr::exception_ptr const&)>
 	mov    (%r12),%rax
 	mov    %r12,%rdi
 	call   *0x10(%rax)
 	mov    %rax,%rsi
-	mov    0x8d11d(%rip),%rax        
+	mov    0x8d125(%rip),%rax        
 	mov    (%rax),%rdi
 	call   25ea0 <pybind11::detail::raise_err(_object*, char const*)>
 	jmp    28cc5 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x75>
 	call   100c0 <__cxa_begin_catch@plt>
-	mov    0x8d084(%rip),%rdx        
+	mov    0x8d08c(%rip),%rdx        
 	mov    0x8d24d(%rip),%rsi        
 	mov    $0xfffffffffffffffe,%rcx
 	mov    %rax,%rdi
 	mov    %rax,%r12
 	call   11220 <__dynamic_cast@plt>
 	mov    %rax,%rdi
 	test   %rax,%rax
 	je     28dcd <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x17d>
 	mov    %rbp,%rsi
 	call   29120 <bool pybind11::detail::handle_nested_exception<std::nested_exception, 0>(std::nested_exception const&, std::__exception_ptr::exception_ptr const&)>
 	mov    (%r12),%rax
 	mov    %r12,%rdi
 	call   *0x10(%rax)
 	mov    %rax,%rsi
-	mov    0x8d0af(%rip),%rax        
+	mov    0x8d0b7(%rip),%rax        
 	mov    (%rax),%rdi
 	call   25ea0 <pybind11::detail::raise_err(_object*, char const*)>
 	jmp    28cc5 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x75>
 	call   11030 <__cxa_end_catch@plt>
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	mov    %rax,%rbp
 	call   11030 <__cxa_end_catch@plt>
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	mov    %rax,%rbp
 	jmp    29075 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x425>
 	call   100c0 <__cxa_begin_catch@plt>
-	mov    0x8d009(%rip),%rdx        
-	mov    0x8cf2a(%rip),%rsi        
+	mov    0x8d011(%rip),%rdx        
+	mov    0x8cf32(%rip),%rsi        
 	mov    $0xfffffffffffffffe,%rcx
 	mov    %rax,%rdi
 	mov    %rax,%r12
 	call   11220 <__dynamic_cast@plt>
 	mov    %rax,%rdi
 	test   %rax,%rax
 	je     28e48 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x1f8>
@@ -23187,16 +23187,16 @@
 	call   *0x10(%rax)
 	mov    %rax,%rsi
 	mov    0x8d12c(%rip),%rax        
 	mov    (%rax),%rdi
 	call   25ea0 <pybind11::detail::raise_err(_object*, char const*)>
 	jmp    28cc5 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x75>
 	call   100c0 <__cxa_begin_catch@plt>
-	mov    0x8cfb3(%rip),%rdx        
-	mov    0x8d0b4(%rip),%rsi        
+	mov    0x8cfbb(%rip),%rdx        
+	mov    0x8d0bc(%rip),%rsi        
 	mov    $0xfffffffffffffffe,%rcx
 	mov    %rax,%rdi
 	mov    %rax,%r12
 	call   11220 <__dynamic_cast@plt>
 	mov    %rax,%rdi
 	test   %rax,%rax
 	je     28e9e <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x24e>
@@ -23210,15 +23210,15 @@
 	mov    (%rax),%rdi
 	call   25ea0 <pybind11::detail::raise_err(_object*, char const*)>
 	jmp    28cc5 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x75>
 	call   100c0 <__cxa_begin_catch@plt>
 	mov    %rax,%r12
 	test   %rax,%rax
 	je     28ef9 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x2a9>
-	mov    0x8cf55(%rip),%rdx        
+	mov    0x8cf5d(%rip),%rdx        
 	mov    %rax,%rdi
 	mov    $0xfffffffffffffffe,%rcx
 	lea    0x8ca7c(%rip),%rsi        
 	call   11220 <__dynamic_cast@plt>
 	mov    %rax,%rdi
 	test   %rax,%rax
 	je     28ef9 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x2a9>
@@ -23233,87 +23233,87 @@
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	mov    %rax,%rbp
 	call   11030 <__cxa_end_catch@plt>
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	call   100c0 <__cxa_begin_catch@plt>
-	mov    0x8cef4(%rip),%rdx        
-	mov    0x8cfc5(%rip),%rsi        
+	mov    0x8cefc(%rip),%rdx        
+	mov    0x8cfcd(%rip),%rsi        
 	mov    $0xfffffffffffffffe,%rcx
 	mov    %rax,%rdi
 	mov    %rax,%r12
 	call   11220 <__dynamic_cast@plt>
 	mov    %rax,%rdi
 	test   %rax,%rax
 	je     28f5d <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x30d>
 	mov    %rbp,%rsi
 	call   29120 <bool pybind11::detail::handle_nested_exception<std::nested_exception, 0>(std::nested_exception const&, std::__exception_ptr::exception_ptr const&)>
 	mov    (%r12),%rax
 	mov    %r12,%rdi
 	call   *0x10(%rax)
 	mov    %rax,%rsi
-	mov    0x8cf1f(%rip),%rax        
+	mov    0x8cf27(%rip),%rax        
 	mov    (%rax),%rdi
 	call   25ea0 <pybind11::detail::raise_err(_object*, char const*)>
 	jmp    28cc5 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x75>
 	call   100c0 <__cxa_begin_catch@plt>
-	mov    0x8ce9e(%rip),%rdx        
-	mov    0x8cf3f(%rip),%rsi        
+	mov    0x8cea6(%rip),%rdx        
+	mov    0x8cf47(%rip),%rsi        
 	mov    $0xfffffffffffffffe,%rcx
 	mov    %rax,%rdi
 	mov    %rax,%r12
 	call   11220 <__dynamic_cast@plt>
 	mov    %rax,%rdi
 	test   %rax,%rax
 	je     28fb3 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x363>
 	mov    %rbp,%rsi
 	call   29120 <bool pybind11::detail::handle_nested_exception<std::nested_exception, 0>(std::nested_exception const&, std::__exception_ptr::exception_ptr const&)>
 	mov    (%r12),%rax
 	mov    %r12,%rdi
 	call   *0x10(%rax)
 	mov    %rax,%rsi
-	mov    0x8cec9(%rip),%rax        
+	mov    0x8ced1(%rip),%rax        
 	mov    (%rax),%rdi
 	call   25ea0 <pybind11::detail::raise_err(_object*, char const*)>
 	jmp    28cc5 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x75>
 	mov    %rax,%rbp
 	jmp    290d6 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x486>
 	call   100c0 <__cxa_begin_catch@plt>
-	mov    0x8ce40(%rip),%rdx        
+	mov    0x8ce48(%rip),%rdx        
 	mov    $0xfffffffffffffffe,%rcx
 	lea    0x8c9b2(%rip),%rsi        
 	mov    %rax,%rdi
 	mov    %rax,%rbx
 	call   11220 <__dynamic_cast@plt>
 	mov    %rax,%rdi
 	test   %rax,%rax
 	je     29011 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x3c1>
 	mov    %rbp,%rsi
 	call   29120 <bool pybind11::detail::handle_nested_exception<std::nested_exception, 0>(std::nested_exception const&, std::__exception_ptr::exception_ptr const&)>
 	mov    0x8(%rbx),%rdi
 	call   28bc0 <pybind11::detail::error_fetch_and_normalize::restore()>
 	jmp    28cc5 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x75>
 	call   100c0 <__cxa_begin_catch@plt>
-	mov    0x8cdfd(%rip),%rdx        
-	mov    0x8cd2e(%rip),%rsi        
+	mov    0x8ce05(%rip),%rdx        
+	mov    0x8cd36(%rip),%rsi        
 	mov    $0xfffffffffffffffe,%rcx
 	mov    %rax,%rdi
 	mov    %rax,%r12
 	call   11220 <__dynamic_cast@plt>
 	mov    %rax,%rdi
 	test   %rax,%rax
 	je     29054 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x404>
 	mov    %rbp,%rsi
 	call   29120 <bool pybind11::detail::handle_nested_exception<std::nested_exception, 0>(std::nested_exception const&, std::__exception_ptr::exception_ptr const&)>
 	mov    (%r12),%rax
 	mov    %r12,%rdi
 	call   *0x10(%rax)
 	mov    %rax,%rsi
-	mov    0x8ce28(%rip),%rax        
+	mov    0x8ce30(%rip),%rax        
 	mov    (%rax),%rdi
 	call   25ea0 <pybind11::detail::raise_err(_object*, char const*)>
 	jmp    28cc5 <pybind11::detail::translate_exception(std::__exception_ptr::exception_ptr)+0x75>
 	call   11030 <__cxa_end_catch@plt>
 	mov    %rbp,%rdi
 	call   10650 <_Unwind_Resume@plt>
 	mov    %rax,%rbp
@@ -23856,15 +23856,15 @@
 	call   25cc0 <pybind11::handle::dec_ref() const &>
 	mov    0x20(%rsp),%rsi
 	test   %rsi,%rsi
 	je     29f20 <pybind11::detail::get_internals()+0x6f0>
 	mov    0x8(%rsi),%rax
 	testb  $0x20,0xab(%rax)
 	jne    299a0 <pybind11::detail::get_internals()+0x170>
-	mov    0x8c5d4(%rip),%rdi        
+	mov    0x8c5dc(%rip),%rdi        
 	xor    %edx,%edx
 	xor    %eax,%eax
 	call   10950 <PyObject_CallFunctionObjArgs@plt>
 	mov    %rax,0x18(%rsp)
 	test   %rax,%rax
 	je     2a230 <pybind11::detail::get_internals()+0xa00>
 	lea    0x20(%rsp),%r15
@@ -24010,15 +24010,15 @@
 	lea    0xd128(%rip),%rdi        
 	mov    %rcx,0x8(%rax)
 	mov    %rdx,(%rax)
 	mov    %rax,0x150(%rbp)
 	mov    (%rbx),%rax
 	mov    %rax,0x8(%rsp)
 	call   10270 <PyUnicode_FromString@plt>
-	mov    0x8c2fd(%rip),%r14        
+	mov    0x8c305(%rip),%r14        
 	mov    %rax,0x28(%rsp)
 	xor    %esi,%esi
 	mov    %r14,%rdi
 	call   *0x130(%r14)
 	mov    %rax,%rbp
 	test   %rax,%rax
 	je     2a224 <pybind11::detail::get_internals()+0x9f4>
@@ -24031,15 +24031,15 @@
 	mov    %rdx,(%rax)
 	mov    %rax,0x358(%rbp)
 	lea    0xd0bc(%rip),%rax        
 	lea    -0x4594(%rip),%rcx        
 	mov    %rbp,%rdi
 	mov    %rax,0x18(%rbp)
 	movq   %rcx,%xmm0
-	mov    0x8c2b1(%rip),%rax        
+	mov    0x8c2b9(%rip),%rax        
 	movq   $0x40600,0xa8(%rbp)
 	addq   $0x1,(%rax)
 	mov    %rax,0x100(%rbp)
 	lea    -0x45a4(%rip),%rax        
 	movq   %rax,%xmm3
 	punpcklqdq %xmm3,%xmm0
 	movups %xmm0,0x110(%rbp)
@@ -24962,15 +24962,15 @@
 	call   10590 <_PyType_Lookup@plt>
 	mov    %rax,%r14
 	call   29830 <pybind11::detail::get_internals()>
 	test   %r14,%r14
 	je     2aae9 <pybind11_meta_setattro+0x29>
 	test   %r13,%r13
 	jne    2ab10 <pybind11_meta_setattro+0x50>
-	mov    0x8b420(%rip),%rax        
+	mov    0x8b428(%rip),%rax        
 	mov    %r13,%rdx
 	mov    %r12,%rsi
 	mov    %rbp,%rdi
 	mov    0x98(%rax),%rax
 	pop    %rbp
 	pop    %r12
 	pop    %r13
@@ -26375,15 +26375,15 @@
 	cmp    %rdi,%rbp
 	jne    2be50 <pybind11_meta_dealloc+0x40>
 	mov    0x10(%rcx),%rdx
 	mov    0x18(%rcx),%rax
 	sub    %rdx,%rax
 	cmp    $0x8,%rax
 	je     2bea0 <pybind11_meta_dealloc+0x90>
-	mov    0x8a08a(%rip),%rax        
+	mov    0x8a092(%rip),%rax        
 	mov    %rbp,%rdi
 	call   *0x30(%rax)
 	add    $0x38,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
@@ -27057,15 +27057,15 @@
 	mov    %ax,0x5c(%r15)
 	mov    0x78(%r15),%rax
 	test   %rax,%rax
 	je     2cd7e <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0x9ee>
 	mov    0x8(%rax),%rdi
 	cmp    0x8928f(%rip),%rdi        
 	je     2d358 <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0xfc8>
-	mov    0x89412(%rip),%rsi        
+	mov    0x8941a(%rip),%rsi        
 	cmp    %rsi,%rdi
 	je     2cd70 <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0x9e0>
 	call   10140 <PyType_IsSubtype@plt>
 	mov    %eax,%r8d
 	mov    0x78(%r15),%rax
 	test   %r8d,%r8d
 	jne    2cd70 <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0x9e0>
@@ -27559,15 +27559,15 @@
 	jmp    2c844 <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0x4b4>
 	nopl   0x0(%rax)
 	mov    0x10(%rax),%rax
 	mov    %rax,0x78(%r15)
 	test   %rax,%rax
 	je     2cd7e <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0x9ee>
 	mov    0x8(%rax),%rdi
-	mov    0x88ad4(%rip),%rsi        
+	mov    0x88adc(%rip),%rsi        
 	cmp    %rsi,%rdi
 	jne    2ca3f <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0x6af>
 	jmp    2cd70 <pybind11::cpp_function::initialize_generic(std::unique_ptr<pybind11::detail::function_record, pybind11::cpp_function::InitializingFunctionRecordDeleter>&&, char const*, std::type_info const* const*, unsigned long)+0x9e0>
 	nopw   0x0(%rax,%rax,1)
 	lea    0x80(%rsp),%rdi
 	mov    %r14,%rdx
 	call   110a0 <void std::vector<char*, std::allocator<char*> >::_M_realloc_insert<char* const&>(__gnu_cxx::__normal_iterator<char**, std::vector<char*, std::allocator<char*> > >, char* const&)@plt>
@@ -28793,15 +28793,15 @@
 	push   %r15
 	push   %r14
 	push   %r13
 	push   %r12
 	push   %rbp
 	push   %rbx
 	sub    $0x28,%rsp
-	mov    0x875cb(%rip),%rax        
+	mov    0x875d3(%rip),%rax        
 	call   *0x80(%rax)
 	mov    %rax,%r12
 	test   %rax,%rax
 	je     2ea0d <pybind11_meta_call+0xdd>
 	mov    0x8(%rax),%rdi
 	call   2e5e0 <pybind11::detail::all_type_info(_typeobject*)>
 	mov    0x8(%rax),%rcx
@@ -30058,18 +30058,18 @@
 	pop    %rbx
 	pop    %rbp
 	ret
 	lea    0x77af(%rip),%rdi        
 	call   11c0b <pybind11::pybind11_fail(char const*)>
 	mov    $0x8,%edi
 	call   10d60 <__cxa_allocate_exception@plt>
-	mov    0x86221(%rip),%rdx        
-	mov    0x862b2(%rip),%rsi        
+	mov    0x86229(%rip),%rdx        
+	mov    0x862ba(%rip),%rsi        
 	mov    %rax,%rdi
-	mov    0x860e8(%rip),%rax        
+	mov    0x860f0(%rip),%rax        
 	add    $0x10,%rax
 	mov    %rax,(%rdi)
 	call   105d0 <__cxa_throw@plt>
 	cs nopw 0x0(%rax,%rax,1)
 	xchg   %ax,%ax
 
 000000000002fca0 <pybind11_object_new>:
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -1,12 +1,12 @@
 
 Hex dump of section '.rodata':
   0x00033000 4e594900 00000000 2f5f5f77 2f5f7465 NYI...../__w/_te
   0x00033010 6d702f63 6f6e6461 5f656e76 69726f6e mp/conda_environ
-  0x00033020 6d656e74 5f393134 34343432 3532372f ment_9144442527/
+  0x00033020 6d656e74 5f393138 33333139 3235302f ment_9183319250/
   0x00033030 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
   0x00033040 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00033050 682f696e 636c7564 652f6331 302f636f h/include/c10/co
   0x00033060 72652f53 796d4e6f 6465496d 706c2e68 re/SymNodeImpl.h
   0x00033070 00686173 5f68696e 7400626f 6f6c5f00 .has_hint.bool_.
   0x00033080 696e745f 00677561 72645f66 6c6f6174 int_.guard_float
   0x00033090 00677561 72645f62 6f6f6c00 67756172 .guard_bool.guar
@@ -32,16 +32,16 @@
   0x000331d0 77007472 75656469 76006d75 6c007375 w.truediv.mul.su
   0x000331e0 62006164 64006973 5f666c6f 61740069 b.add.is_float.i
   0x000331f0 735f626f 6f6c0069 735f696e 74007465 s_bool.is_int.te
   0x00033200 6e736f72 20646f65 73206e6f 74206861 nsor does not ha
   0x00033210 76652061 20646576 69636500 64657669 ve a device.devi
   0x00033220 63655f64 65666175 6c740000 00000000 ce_default......
   0x00033230 2f5f5f77 2f5f7465 6d702f63 6f6e6461 /__w/_temp/conda
-  0x00033240 5f656e76 69726f6e 6d656e74 5f393134 _environment_914
-  0x00033250 34343432 3532372f 6c69622f 70797468 4442527/lib/pyth
+  0x00033240 5f656e76 69726f6e 6d656e74 5f393138 _environment_918
+  0x00033250 33333139 3235302f 6c69622f 70797468 3319250/lib/pyth
   0x00033260 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
   0x00033270 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x00033280 652f6331 302f636f 72652f54 656e736f e/c10/core/Tenso
   0x00033290 72496d70 6c2e6800 63756461 4572726f rImpl.h.cudaErro
   0x000332a0 725f7420 6670365f 6c696e65 61725f6b r_t fp6_linear_k
   0x000332b0 65726e65 6c286375 64615374 7265616d ernel(cudaStream
   0x000332c0 5f742c20 636f6e73 74207569 6e74342a _t, const uint4*
@@ -148,24 +148,24 @@
   0x00033910 69766550 74720072 65636c61 696d0000 ivePtr.reclaim..
   0x00033920 73746174 69635f63 6173743c 75696e74 static_cast<uint
   0x00033930 33325f74 3e287461 6729203c 206b4e75 32_t>(tag) < kNu
   0x00033940 6d546167 7320494e 5445524e 414c2041 mTags INTERNAL A
   0x00033950 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x00033960 222f5f5f 772f5f74 656d702f 636f6e64 "/__w/_temp/cond
   0x00033970 615f656e 7669726f 6e6d656e 745f3931 a_environment_91
-  0x00033980 34343434 32353237 2f6c6962 2f707974 44442527/lib/pyt
+  0x00033980 38333331 39323530 2f6c6962 2f707974 83319250/lib/pyt
   0x00033990 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
   0x000339a0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x000339b0 64652f41 54656e2f 636f7265 2f697661 de/ATen/core/iva
   0x000339c0 6c75652e 68223a31 3331352c 20706c65 lue.h":1315, ple
   0x000339d0 61736520 7265706f 72742061 20627567 ase report a bug
   0x000339e0 20746f20 5079546f 7263682e 20000000  to PyTorch. ...
   0x000339f0 2f5f5f77 2f5f7465 6d702f63 6f6e6461 /__w/_temp/conda
-  0x00033a00 5f656e76 69726f6e 6d656e74 5f393134 _environment_914
-  0x00033a10 34343432 3532372f 6c69622f 70797468 4442527/lib/pyth
+  0x00033a00 5f656e76 69726f6e 6d656e74 5f393138 _environment_918
+  0x00033a10 33333139 3235302f 6c69622f 70797468 3319250/lib/pyth
   0x00033a20 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
   0x00033a30 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x00033a40 652f4154 656e2f63 6f72652f 6976616c e/ATen/core/ival
   0x00033a50 75652e68 00000000 54546172 67657420 ue.h....TTarget 
   0x00033a60 76696f6c 61746573 20746865 20696e76 violates the inv
   0x00033a70 61726961 6e742074 68617420 72656663 ariant that refc
   0x00033a80 6f756e74 203e2030 20203d3e 20207765 ount > 0  =>  we
@@ -176,39 +176,39 @@
   0x00033ad0 722d3e72 6566636f 756e745f 2e6c6f61 r->refcount_.loa
   0x00033ae0 64282920 3d3d2030 207c7c20 6f776e69 d() == 0 || owni
   0x00033af0 6e675f70 74722d3e 7765616b 636f756e ng_ptr->weakcoun
   0x00033b00 745f2e6c 6f616428 2920494e 5445524e t_.load() INTERN
   0x00033b10 414c2041 53534552 54204641 494c4544 AL ASSERT FAILED
   0x00033b20 20617420 222f5f5f 772f5f74 656d702f  at "/__w/_temp/
   0x00033b30 636f6e64 615f656e 7669726f 6e6d656e conda_environmen
-  0x00033b40 745f3931 34343434 32353237 2f6c6962 t_9144442527/lib
+  0x00033b40 745f3931 38333331 39323530 2f6c6962 t_9183319250/lib
   0x00033b50 2f707974 686f6e33 2e392f73 6974652d /python3.9/site-
   0x00033b60 7061636b 61676573 2f746f72 63682f69 packages/torch/i
   0x00033b70 6e636c75 64652f63 31302f75 74696c2f nclude/c10/util/
   0x00033b80 696e7472 75736976 655f7074 722e6822 intrusive_ptr.h"
   0x00033b90 3a343833 2c20706c 65617365 20726570 :483, please rep
   0x00033ba0 6f727420 61206275 6720746f 20507954 ort a bug to PyT
   0x00033bb0 6f726368 2e200000 2f5f5f77 2f5f7465 orch. ../__w/_te
   0x00033bc0 6d702f63 6f6e6461 5f656e76 69726f6e mp/conda_environ
-  0x00033bd0 6d656e74 5f393134 34343432 3532372f ment_9144442527/
+  0x00033bd0 6d656e74 5f393138 33333139 3235302f ment_9183319250/
   0x00033be0 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
   0x00033bf0 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00033c00 682f696e 636c7564 652f6331 302f7574 h/include/c10/ut
   0x00033c10 696c2f69 6e747275 73697665 5f707472 il/intrusive_ptr
   0x00033c20 2e680000 00000000 4f706572 61746f72 .h......Operator
   0x00033c30 73207461 6b696e67 2054656e 736f724f s taking TensorO
   0x00033c40 7074696f 6e732063 616e6e6f 74207461 ptions cannot ta
   0x00033c50 6b652061 2054656e 736f724f 7074696f ke a TensorOptio
   0x00033c60 6e732077 69746820 6f707469 6f6e732e ns with options.
   0x00033c70 72657175 69726573 5f677261 64207365 requires_grad se
   0x00033c80 74206173 20747275 652e2054 68697320 t as true. This 
   0x00033c90 69736e27 7420696d 706c656d 656e7465 isn't implemente
   0x00033ca0 64207965 742e0000 2f5f5f77 2f5f7465 d yet.../__w/_te
   0x00033cb0 6d702f63 6f6e6461 5f656e76 69726f6e mp/conda_environ
-  0x00033cc0 6d656e74 5f393134 34343432 3532372f ment_9144442527/
+  0x00033cc0 6d656e74 5f393138 33333139 3235302f ment_9183319250/
   0x00033cd0 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
   0x00033ce0 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00033cf0 682f696e 636c7564 652f4154 656e2f63 h/include/ATen/c
   0x00033d00 6f72652f 43686563 6b4d656d 6f727946 ore/CheckMemoryF
   0x00033d10 6f726d61 742e6800 63686563 6b5f7465 ormat.h.check_te
   0x00033d20 6e736f72 5f6f7074 696f6e73 5f616e64 nsor_options_and
   0x00033d30 5f657874 72616374 5f6d656d 6f72795f _extract_memory_
@@ -221,16 +221,16 @@
   0x00033da0 72656475 6e64616e 74207365 74746572 redundant setter
   0x00033db0 2e000000 00000000 496e7441 72726179 ........IntArray
   0x00033dc0 52656620 636f6e74 61696e73 20616e20 Ref contains an 
   0x00033dd0 696e7420 74686174 2063616e 6e6f7420 int that cannot 
   0x00033de0 62652072 65707265 73656e74 65642061 be represented a
   0x00033df0 73206120 53796d49 6e743a20 00000000 s a SymInt: ....
   0x00033e00 2f5f5f77 2f5f7465 6d702f63 6f6e6461 /__w/_temp/conda
-  0x00033e10 5f656e76 69726f6e 6d656e74 5f393134 _environment_914
-  0x00033e20 34343432 3532372f 6c69622f 70797468 4442527/lib/pyth
+  0x00033e10 5f656e76 69726f6e 6d656e74 5f393138 _environment_918
+  0x00033e20 33333139 3235302f 6c69622f 70797468 3319250/lib/pyth
   0x00033e30 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
   0x00033e40 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x00033e50 652f6331 302f636f 72652f53 796d496e e/c10/core/SymIn
   0x00033e60 74417272 61795265 662e6800 00000000 tArrayRef.h.....
   0x00033e70 63726561 74656420 41727261 79526566 created ArrayRef
   0x00033e80 20776974 68206e75 6c6c7074 7220616e  with nullptr an
   0x00033e90 64206e6f 6e2d7a65 726f206c 656e6774 d non-zero lengt
@@ -238,24 +238,24 @@
   0x00033eb0 2072656c 69657320 6f6e2074 68697320  relies on this 
   0x00033ec0 6265696e 6720696c 6c656761 6c000000 being illegal...
   0x00033ed0 44617461 20213d20 6e756c6c 70747220 Data != nullptr 
   0x00033ee0 7c7c204c 656e6774 68203d3d 20302049 || Length == 0 I
   0x00033ef0 4e544552 4e414c20 41535345 52542046 NTERNAL ASSERT F
   0x00033f00 41494c45 44206174 20222f5f 5f772f5f AILED at "/__w/_
   0x00033f10 74656d70 2f636f6e 64615f65 6e766972 temp/conda_envir
-  0x00033f20 6f6e6d65 6e745f39 31343434 34323532 onment_914444252
-  0x00033f30 372f6c69 622f7079 74686f6e 332e392f 7/lib/python3.9/
+  0x00033f20 6f6e6d65 6e745f39 31383333 31393235 onment_918331925
+  0x00033f30 302f6c69 622f7079 74686f6e 332e392f 0/lib/python3.9/
   0x00033f40 73697465 2d706163 6b616765 732f746f site-packages/to
   0x00033f50 7263682f 696e636c 7564652f 6331302f rch/include/c10/
   0x00033f60 7574696c 2f417272 61795265 662e6822 util/ArrayRef.h"
   0x00033f70 3a36322c 20706c65 61736520 7265706f :62, please repo
   0x00033f80 72742061 20627567 20746f20 5079546f rt a bug to PyTo
   0x00033f90 7263682e 20000000 2f5f5f77 2f5f7465 rch. .../__w/_te
   0x00033fa0 6d702f63 6f6e6461 5f656e76 69726f6e mp/conda_environ
-  0x00033fb0 6d656e74 5f393134 34343432 3532372f ment_9144442527/
+  0x00033fb0 6d656e74 5f393138 33333139 3235302f ment_9183319250/
   0x00033fc0 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
   0x00033fd0 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00033fe0 682f696e 636c7564 652f6331 302f7574 h/include/c10/ut
   0x00033ff0 696c2f41 72726179 5265662e 68006672 il/ArrayRef.h.fr
   0x00034000 6f6d496e 74417272 61795265 66536c6f omIntArrayRefSlo
   0x00034010 77006465 62756743 6865636b 4e756c6c w.debugCheckNull
   0x00034020 70747249 6e766172 69616e74 00000000 ptrInvariant....
@@ -270,15 +270,15 @@
   0x000340b0 745f2e6c 6f616428 29203e3d 20646574 t_.load() >= det
   0x000340c0 61696c3a 3a6b496d 70726163 74696361 ail::kImpractica
   0x000340d0 6c6c7948 75676552 65666572 656e6365 llyHugeReference
   0x000340e0 436f756e 7420494e 5445524e 414c2041 Count INTERNAL A
   0x000340f0 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x00034100 222f5f5f 772f5f74 656d702f 636f6e64 "/__w/_temp/cond
   0x00034110 615f656e 7669726f 6e6d656e 745f3931 a_environment_91
-  0x00034120 34343434 32353237 2f6c6962 2f707974 44442527/lib/pyt
+  0x00034120 38333331 39323530 2f6c6962 2f707974 83319250/lib/pyt
   0x00034130 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
   0x00034140 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x00034150 64652f63 31302f75 74696c2f 696e7472 de/c10/util/intr
   0x00034160 75736976 655f7074 722e6822 3a313138 usive_ptr.h":118
   0x00034170 2c20706c 65617365 20726570 6f727420 , please report 
   0x00034180 61206275 6720746f 20507954 6f726368 a bug to PyTorch
   0x00034190 2e200000 00000000 54726965 6420746f . ......Tried to
@@ -298,38 +298,38 @@
   0x00034270 6e745f2e 6c6f6164 2829203d 3d206465 nt_.load() == de
   0x00034280 7461696c 3a3a6b49 6d707261 63746963 tail::kImpractic
   0x00034290 616c6c79 48756765 52656665 72656e63 allyHugeReferenc
   0x000342a0 65436f75 6e742049 4e544552 4e414c20 eCount INTERNAL 
   0x000342b0 41535345 52542046 41494c45 44206174 ASSERT FAILED at
   0x000342c0 20222f5f 5f772f5f 74656d70 2f636f6e  "/__w/_temp/con
   0x000342d0 64615f65 6e766972 6f6e6d65 6e745f39 da_environment_9
-  0x000342e0 31343434 34323532 372f6c69 622f7079 144442527/lib/py
+  0x000342e0 31383333 31393235 302f6c69 622f7079 183319250/lib/py
   0x000342f0 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
   0x00034300 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x00034310 7564652f 6331302f 7574696c 2f696e74 ude/c10/util/int
   0x00034320 72757369 76655f70 74722e68 223a3133 rusive_ptr.h":13
   0x00034330 332c2070 6c656173 65207265 706f7274 3, please report
   0x00034340 20612062 75672074 6f205079 546f7263  a bug to PyTorc
   0x00034350 682e2000 7e696e74 72757369 76655f70 h. .~intrusive_p
   0x00034360 74725f74 61726765 74000000 00000000 tr_target.......
   0x00034370 73656c66 5f696d70 6c20494e 5445524e self_impl INTERN
   0x00034380 414c2041 53534552 54204641 494c4544 AL ASSERT FAILED
   0x00034390 20617420 222f5f5f 772f5f74 656d702f  at "/__w/_temp/
   0x000343a0 636f6e64 615f656e 7669726f 6e6d656e conda_environmen
-  0x000343b0 745f3931 34343434 32353237 2f6c6962 t_9144442527/lib
+  0x000343b0 745f3931 38333331 39323530 2f6c6962 t_9183319250/lib
   0x000343c0 2f707974 686f6e33 2e392f73 6974652d /python3.9/site-
   0x000343d0 7061636b 61676573 2f746f72 63682f69 packages/torch/i
   0x000343e0 6e636c75 64652f74 6f726368 2f637372 nclude/torch/csr
   0x000343f0 632f6175 746f6772 61642f76 61726961 c/autograd/varia
   0x00034400 626c652e 68223a33 30352c20 706c6561 ble.h":305, plea
   0x00034410 73652072 65706f72 74206120 62756720 se report a bug 
   0x00034420 746f2050 79546f72 63682e20 00000000 to PyTorch. ....
   0x00034430 2f5f5f77 2f5f7465 6d702f63 6f6e6461 /__w/_temp/conda
-  0x00034440 5f656e76 69726f6e 6d656e74 5f393134 _environment_914
-  0x00034450 34343432 3532372f 6c69622f 70797468 4442527/lib/pyth
+  0x00034440 5f656e76 69726f6e 6d656e74 5f393138 _environment_918
+  0x00034450 33333139 3235302f 6c69622f 70797468 3319250/lib/pyth
   0x00034460 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
   0x00034470 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x00034480 652f746f 7263682f 63737263 2f617574 e/torch/csrc/aut
   0x00034490 6f677261 642f7661 72696162 6c652e68 ograd/variable.h
   0x000344a0 00000000 00000000 4f6e6c79 2054656e ........Only Ten
   0x000344b0 736f7273 206f6620 666c6f61 74696e67 sors of floating
   0x000344c0 20706f69 6e742061 6e642063 6f6d706c  point and compl
@@ -349,16 +349,16 @@
   0x000345a0 6d206074 68697360 3f000000 00000000 m `this`?.......
   0x000345b0 74617267 65745f2d 3e726566 636f756e target_->refcoun
   0x000345c0 745f203d 3d203020 26262074 61726765 t_ == 0 && targe
   0x000345d0 745f2d3e 7765616b 636f756e 745f203d t_->weakcount_ =
   0x000345e0 3d203020 494e5445 524e414c 20415353 = 0 INTERNAL ASS
   0x000345f0 45525420 4641494c 45442061 7420222f ERT FAILED at "/
   0x00034600 5f5f772f 5f74656d 702f636f 6e64615f __w/_temp/conda_
-  0x00034610 656e7669 726f6e6d 656e745f 39313434 environment_9144
-  0x00034620 34343235 32372f6c 69622f70 7974686f 442527/lib/pytho
+  0x00034610 656e7669 726f6e6d 656e745f 39313833 environment_9183
+  0x00034620 33313932 35302f6c 69622f70 7974686f 319250/lib/pytho
   0x00034630 6e332e39 2f736974 652d7061 636b6167 n3.9/site-packag
   0x00034640 65732f74 6f726368 2f696e63 6c756465 es/torch/include
   0x00034650 2f633130 2f757469 6c2f696e 74727573 /c10/util/intrus
   0x00034660 6976655f 7074722e 68223a33 31392c20 ive_ptr.h":319, 
   0x00034670 706c6561 73652072 65706f72 74206120 please report a 
   0x00034680 62756720 746f2050 79546f72 63682e20 bug to PyTorch. 
   0x00034690 00696e74 72757369 76655f70 74720000 .intrusive_ptr..
@@ -369,30 +369,30 @@
   0x000346e0 616e6e6f 7420696e 63726561 73652072 annot increase r
   0x000346f0 6566636f 756e7420 61667465 72206974 efcount after it
   0x00034700 20726561 63686564 207a6572 6f2e0000  reached zero...
   0x00034710 6e65775f 72656663 6f756e74 20213d20 new_refcount != 
   0x00034720 3120494e 5445524e 414c2041 53534552 1 INTERNAL ASSER
   0x00034730 54204641 494c4544 20617420 222f5f5f T FAILED at "/__
   0x00034740 772f5f74 656d702f 636f6e64 615f656e w/_temp/conda_en
-  0x00034750 7669726f 6e6d656e 745f3931 34343434 vironment_914444
-  0x00034760 32353237 2f6c6962 2f707974 686f6e33 2527/lib/python3
+  0x00034750 7669726f 6e6d656e 745f3931 38333331 vironment_918331
+  0x00034760 39323530 2f6c6962 2f707974 686f6e33 9250/lib/python3
   0x00034770 2e392f73 6974652d 7061636b 61676573 .9/site-packages
   0x00034780 2f746f72 63682f69 6e636c75 64652f63 /torch/include/c
   0x00034790 31302f75 74696c2f 696e7472 75736976 10/util/intrusiv
   0x000347a0 655f7074 722e6822 3a323734 2c20706c e_ptr.h":274, pl
   0x000347b0 65617365 20726570 6f727420 61206275 ease report a bu
   0x000347c0 6720746f 20507954 6f726368 2e200072 g to PyTorch. .r
   0x000347d0 65746169 6e5f0076 6563746f 723a3a5f etain_.vector::_
   0x000347e0 4d5f7265 616c6c6f 635f696e 73657274 M_realloc_insert
   0x000347f0 00657870 65637465 6420696e 7400746f .expected int.to
   0x00034800 496e7400 00000000 3020494e 5445524e Int.....0 INTERN
   0x00034810 414c2041 53534552 54204641 494c4544 AL ASSERT FAILED
   0x00034820 20617420 222f5f5f 772f5f74 656d702f  at "/__w/_temp/
   0x00034830 636f6e64 615f656e 7669726f 6e6d656e conda_environmen
-  0x00034840 745f3931 34343434 32353237 2f6c6962 t_9144442527/lib
+  0x00034840 745f3931 38333331 39323530 2f6c6962 t_9183319250/lib
   0x00034850 2f707974 686f6e33 2e392f73 6974652d /python3.9/site-
   0x00034860 7061636b 61676573 2f746f72 63682f69 packages/torch/i
   0x00034870 6e636c75 64652f41 54656e2f 636f7265 nclude/ATen/core
   0x00034880 2f697661 6c75652e 68223a36 35322c20 /ivalue.h":652, 
   0x00034890 706c6561 73652072 65706f72 74206120 please report a 
   0x000348a0 62756720 746f2050 79546f72 63682e20 bug to PyTorch. 
   0x000348b0 00000000 00000000 00000000 00000000 ................
@@ -437,15 +437,15 @@
   0x00034b20 45000000 00000000 65787472 615f6d65 E.......extra_me
   0x00034b30 74615f20 26262065 78747261 5f6d6574 ta_ && extra_met
   0x00034b40 615f2d3e 73796d62 6f6c6963 5f736861 a_->symbolic_sha
   0x00034b50 70655f6d 6574615f 20494e54 45524e41 pe_meta_ INTERNA
   0x00034b60 4c204153 53455254 20464149 4c454420 L ASSERT FAILED 
   0x00034b70 61742022 2f5f5f77 2f5f7465 6d702f63 at "/__w/_temp/c
   0x00034b80 6f6e6461 5f656e76 69726f6e 6d656e74 onda_environment
-  0x00034b90 5f393134 34343432 3532372f 6c69622f _9144442527/lib/
+  0x00034b90 5f393138 33333139 3235302f 6c69622f _9183319250/lib/
   0x00034ba0 70797468 6f6e332e 392f7369 74652d70 python3.9/site-p
   0x00034bb0 61636b61 6765732f 746f7263 682f696e ackages/torch/in
   0x00034bc0 636c7564 652f6331 302f636f 72652f54 clude/c10/core/T
   0x00034bd0 656e736f 72496d70 6c2e6822 3a313732 ensorImpl.h":172
   0x00034be0 332c2070 6c656173 65207265 706f7274 3, please report
   0x00034bf0 20612062 75672074 6f205079 546f7263  a bug to PyTorc
   0x00034c00 682e2000 00000000 45787065 63746564 h. .....Expected
@@ -556,25 +556,25 @@
   0x00035290 1069feff 0069feff 706afeff 606afeff .i...i..pj..`j..
   0x000352a0 506afeff 406afeff 7069feff 6069feff Pj..@j..pi..`i..
   0x000352b0 5069feff 4069feff d068feff c068feff Pi..@i...h...h..
   0x000352c0 e068feff 00000000 642e6973 5f637564 .h......d.is_cud
   0x000352d0 61282920 494e5445 524e414c 20415353 a() INTERNAL ASS
   0x000352e0 45525420 4641494c 45442061 7420222f ERT FAILED at "/
   0x000352f0 5f5f772f 5f74656d 702f636f 6e64615f __w/_temp/conda_
-  0x00035300 656e7669 726f6e6d 656e745f 39313434 environment_9144
-  0x00035310 34343235 32372f6c 69622f70 7974686f 442527/lib/pytho
+  0x00035300 656e7669 726f6e6d 656e745f 39313833 environment_9183
+  0x00035310 33313932 35302f6c 69622f70 7974686f 319250/lib/pytho
   0x00035320 6e332e39 2f736974 652d7061 636b6167 n3.9/site-packag
   0x00035330 65732f74 6f726368 2f696e63 6c756465 es/torch/include
   0x00035340 2f633130 2f637564 612f696d 706c2f43 /c10/cuda/impl/C
   0x00035350 55444147 75617264 496d706c 2e68223a UDAGuardImpl.h":
   0x00035360 35332c20 706c6561 73652072 65706f72 53, please repor
   0x00035370 74206120 62756720 746f2050 79546f72 t a bug to PyTor
   0x00035380 63682e20 00000000 2f5f5f77 2f5f7465 ch. ..../__w/_te
   0x00035390 6d702f63 6f6e6461 5f656e76 69726f6e mp/conda_environ
-  0x000353a0 6d656e74 5f393134 34343432 3532372f ment_9144442527/
+  0x000353a0 6d656e74 5f393138 33333139 3235302f ment_9183319250/
   0x000353b0 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
   0x000353c0 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x000353d0 682f696e 636c7564 652f6331 302f6375 h/include/c10/cu
   0x000353e0 64612f69 6d706c2f 43554441 47756172 da/impl/CUDAGuar
   0x000353f0 64496d70 6c2e6800 73657444 65766963 dImpl.h.setDevic
   0x00035400 65000000 00000000 426f7468 20657665 e.......Both eve
   0x00035410 6e747320 6d757374 20626520 7265636f nts must be reco
@@ -590,75 +590,75 @@
   0x000354b0 69732065 72726f72 206d6573 73616765 is error message
   0x000354c0 20626520 696d7072 6f766564 3f202049  be improved?  I
   0x000354d0 6620736f 2c20706c 65617365 20726570 f so, please rep
   0x000354e0 6f727420 616e2065 6e68616e 63656d65 ort an enhanceme
   0x000354f0 6e742072 65717565 73742074 6f205079 nt request to Py
   0x00035500 546f7263 682e2900 2f5f5f77 2f5f7465 Torch.)./__w/_te
   0x00035510 6d702f63 6f6e6461 5f656e76 69726f6e mp/conda_environ
-  0x00035520 6d656e74 5f393134 34343432 3532372f ment_9144442527/
+  0x00035520 6d656e74 5f393138 33333139 3235302f ment_9183319250/
   0x00035530 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
   0x00035540 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00035550 682f696e 636c7564 652f6331 302f6375 h/include/c10/cu
   0x00035560 64612f43 55444153 74726561 6d2e6800 da/CUDAStream.h.
   0x00035570 43554441 53747265 616d0073 796e6368 CUDAStream.synch
   0x00035580 726f6e69 7a654576 656e7400 71756572 ronizeEvent.quer
   0x00035590 79457665 6e74006c 61796f75 74000000 yEvent.layout...
   0x000355a0 54686572 65206973 20616e20 6572726f There is an erro
   0x000355b0 7220696e 20746865 206c6179 6f757420 r in the layout 
   0x000355c0 63616c63 756c6174 696f6e20 6c6f6769 calculation logi
   0x000355d0 632e0000 00000000 69735f6d 6b6c646e c.......is_mkldn
   0x000355e0 6e282920 494e5445 524e414c 20415353 n() INTERNAL ASS
   0x000355f0 45525420 4641494c 45442061 7420222f ERT FAILED at "/
   0x00035600 5f5f772f 5f74656d 702f636f 6e64615f __w/_temp/conda_
-  0x00035610 656e7669 726f6e6d 656e745f 39313434 environment_9144
-  0x00035620 34343235 32372f6c 69622f70 7974686f 442527/lib/pytho
+  0x00035610 656e7669 726f6e6d 656e745f 39313833 environment_9183
+  0x00035620 33313932 35302f6c 69622f70 7974686f 319250/lib/pytho
   0x00035630 6e332e39 2f736974 652d7061 636b6167 n3.9/site-packag
   0x00035640 65732f74 6f726368 2f696e63 6c756465 es/torch/include
   0x00035650 2f633130 2f636f72 652f5465 6e736f72 /c10/core/Tensor
   0x00035660 496d706c 2e68223a 31323930 2c20706c Impl.h":1290, pl
   0x00035670 65617365 20726570 6f727420 61206275 ease report a bu
   0x00035680 6720746f 20507954 6f726368 2e200000 g to PyTorch. ..
   0x00035690 5f5a4e37 746f7263 68616f34 335f474c _ZN7torchao43_GL
   0x000356a0 4f42414c 5f5f4e5f 5f356232 65393235 OBAL__N__5b2e925
-  0x000356b0 395f365f 6e6d735f 63755f61 31636164 9_6_nms_cu_a1cad
-  0x000356c0 3162665f 32323032 31356e6d 735f6b65 1bf_220215nms_ke
+  0x000356b0 395f365f 6e6d735f 63755f34 33643130 9_6_nms_cu_43d10
+  0x000356c0 6539345f 32313933 31356e6d 735f6b65 e94_219315nms_ke
   0x000356d0 726e656c 5f696d70 6c494e33 63313034 rnel_implIN3c104
   0x000356e0 48616c66 45454576 6964504b 545f5079 HalfEEEvidPKT_Py
   0x000356f0 00000000 00000000 5f5a4e37 746f7263 ........_ZN7torc
   0x00035700 68616f34 335f474c 4f42414c 5f5f4e5f hao43_GLOBAL__N_
   0x00035710 5f356232 65393235 395f365f 6e6d735f _5b2e9259_6_nms_
-  0x00035720 63755f61 31636164 3162665f 32323032 cu_a1cad1bf_2202
+  0x00035720 63755f34 33643130 6539345f 32313933 cu_43d10e94_2193
   0x00035730 31356e6d 735f6b65 726e656c 5f696d70 15nms_kernel_imp
   0x00035740 6c496645 45766964 504b545f 50790000 lIfEEvidPKT_Py..
   0x00035750 5f5a4e37 746f7263 68616f34 335f474c _ZN7torchao43_GL
   0x00035760 4f42414c 5f5f4e5f 5f356232 65393235 OBAL__N__5b2e925
-  0x00035770 395f365f 6e6d735f 63755f61 31636164 9_6_nms_cu_a1cad
-  0x00035780 3162665f 32323032 31356e6d 735f6b65 1bf_220215nms_ke
+  0x00035770 395f365f 6e6d735f 63755f34 33643130 9_6_nms_cu_43d10
+  0x00035780 6539345f 32313933 31356e6d 735f6b65 e94_219315nms_ke
   0x00035790 726e656c 5f696d70 6c496445 45766964 rnel_implIdEEvid
   0x000357a0 504b545f 50790000 5f5a4e34 315f494e PKT_Py.._ZN41_IN
   0x000357b0 5445524e 414c5f35 62326539 3235395f TERNAL_5b2e9259_
-  0x000357c0 365f6e6d 735f6375 5f613163 61643162 6_nms_cu_a1cad1b
-  0x000357d0 665f3232 30323674 68727573 74367379 f_22026thrust6sy
+  0x000357c0 365f6e6d 735f6375 5f343364 31306539 6_nms_cu_43d10e9
+  0x000357d0 345f3231 39333674 68727573 74367379 4_21936thrust6sy
   0x000357e0 7374656d 36646574 61696c31 30736571 stem6detail10seq
   0x000357f0 75656e74 69616c33 73657145 00000000 uential3seqE....
   0x00035800 69735f68 6561705f 616c6c6f 63617465 is_heap_allocate
   0x00035810 64282920 494e5445 524e414c 20415353 d() INTERNAL ASS
   0x00035820 45525420 4641494c 45442061 7420222f ERT FAILED at "/
   0x00035830 5f5f772f 5f74656d 702f636f 6e64615f __w/_temp/conda_
-  0x00035840 656e7669 726f6e6d 656e745f 39313434 environment_9144
-  0x00035850 34343235 32372f6c 69622f70 7974686f 442527/lib/pytho
+  0x00035840 656e7669 726f6e6d 656e745f 39313833 environment_9183
+  0x00035850 33313932 35302f6c 69622f70 7974686f 319250/lib/pytho
   0x00035860 6e332e39 2f736974 652d7061 636b6167 n3.9/site-packag
   0x00035870 65732f74 6f726368 2f696e63 6c756465 es/torch/include
   0x00035880 2f633130 2f636f72 652f5379 6d496e74 /c10/core/SymInt
   0x00035890 2e68223a 38392c20 706c6561 73652072 .h":89, please r
   0x000358a0 65706f72 74206120 62756720 746f2050 eport a bug to P
   0x000358b0 79546f72 63682e20 00000000 00000000 yTorch. ........
   0x000358c0 2f5f5f77 2f5f7465 6d702f63 6f6e6461 /__w/_temp/conda
-  0x000358d0 5f656e76 69726f6e 6d656e74 5f393134 _environment_914
-  0x000358e0 34343432 3532372f 6c69622f 70797468 4442527/lib/pyth
+  0x000358d0 5f656e76 69726f6e 6d656e74 5f393138 _environment_918
+  0x000358e0 33333139 3235302f 6c69622f 70797468 3319250/lib/pyth
   0x000358f0 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
   0x00035900 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x00035910 652f6331 302f636f 72652f53 796d496e e/c10/core/SymIn
   0x00035920 742e6800 00000000 2f5f5f77 2f616f2f t.h...../__w/ao/
   0x00035930 616f2f70 79746f72 63682f61 6f2f746f ao/pytorch/ao/to
   0x00035940 72636861 6f2f6373 72632f63 7564612f rchao/csrc/cuda/
   0x00035950 6e6d732e 63750000 626f7865 73207368 nms.cu..boxes sh
@@ -675,59 +675,59 @@
   0x00035a00 65206e75 6d626572 206f6620 656c656d e number of elem
   0x00035a10 656e7473 20696e20 00000000 00000000 ents in ........
   0x00035a20 74203d3d 20446576 69636554 7970653a t == DeviceType:
   0x00035a30 3a435544 4120494e 5445524e 414c2041 :CUDA INTERNAL A
   0x00035a40 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x00035a50 222f5f5f 772f5f74 656d702f 636f6e64 "/__w/_temp/cond
   0x00035a60 615f656e 7669726f 6e6d656e 745f3931 a_environment_91
-  0x00035a70 34343434 32353237 2f6c6962 2f707974 44442527/lib/pyt
+  0x00035a70 38333331 39323530 2f6c6962 2f707974 83319250/lib/pyt
   0x00035a80 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
   0x00035a90 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x00035aa0 64652f63 31302f63 7564612f 696d706c de/c10/cuda/impl
   0x00035ab0 2f435544 41477561 7264496d 706c2e68 /CUDAGuardImpl.h
   0x00035ac0 223a3238 2c20706c 65617365 20726570 ":28, please rep
   0x00035ad0 6f727420 61206275 6720746f 20507954 ort a bug to PyT
   0x00035ae0 6f726368 2e200000 63616e6e 6f742063 orch. ..cannot c
   0x00035af0 72656174 65207374 643a3a76 6563746f reate std::vecto
   0x00035b00 72206c61 72676572 20746861 6e206d61 r larger than ma
   0x00035b10 785f7369 7a652829 00000000 00000000 x_size()........
   0x00035b20 2f5f5f77 2f5f7465 6d702f63 6f6e6461 /__w/_temp/conda
-  0x00035b30 5f656e76 69726f6e 6d656e74 5f393134 _environment_914
-  0x00035b40 34343432 3532372f 6c69622f 70797468 4442527/lib/pyth
+  0x00035b30 5f656e76 69726f6e 6d656e74 5f393138 _environment_918
+  0x00035b40 33333139 3235302f 6c69622f 70797468 3319250/lib/pyth
   0x00035b50 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
   0x00035b60 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x00035b70 652f4154 656e2f54 656e736f 72496e64 e/ATen/TensorInd
   0x00035b80 6578696e 672e6800 67657444 65766963 exing.h.getDevic
   0x00035b90 65007661 6c696461 74650000 00000000 e.validate......
   0x00035ba0 44657669 63652069 6e646578 206d7573 Device index mus
   0x00035bb0 74206265 202d3120 6f72206e 6f6e2d6e t be -1 or non-n
   0x00035bc0 65676174 6976652c 20676f74 20000000 egative, got ...
   0x00035bd0 696e6465 785f203e 3d202d31 20494e54 index_ >= -1 INT
   0x00035be0 45524e41 4c204153 53455254 20464149 ERNAL ASSERT FAI
   0x00035bf0 4c454420 61742022 2f5f5f77 2f5f7465 LED at "/__w/_te
   0x00035c00 6d702f63 6f6e6461 5f656e76 69726f6e mp/conda_environ
-  0x00035c10 6d656e74 5f393134 34343432 3532372f ment_9144442527/
+  0x00035c10 6d656e74 5f393138 33333139 3235302f ment_9183319250/
   0x00035c20 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
   0x00035c30 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00035c40 682f696e 636c7564 652f6331 302f636f h/include/c10/co
   0x00035c50 72652f44 65766963 652e6822 3a313737 re/Device.h":177
   0x00035c60 2c20706c 65617365 20726570 6f727420 , please report 
   0x00035c70 61206275 6720746f 20507954 6f726368 a bug to PyTorch
   0x00035c80 2e200000 00000000 2f5f5f77 2f5f7465 . ....../__w/_te
   0x00035c90 6d702f63 6f6e6461 5f656e76 69726f6e mp/conda_environ
-  0x00035ca0 6d656e74 5f393134 34343432 3532372f ment_9144442527/
+  0x00035ca0 6d656e74 5f393138 33333139 3235302f ment_9183319250/
   0x00035cb0 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
   0x00035cc0 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00035cd0 682f696e 636c7564 652f6331 302f636f h/include/c10/co
   0x00035ce0 72652f44 65766963 652e6800 00000000 re/Device.h.....
   0x00035cf0 642e6973 5f637564 61282920 494e5445 d.is_cuda() INTE
   0x00035d00 524e414c 20415353 45525420 4641494c RNAL ASSERT FAIL
   0x00035d10 45442061 7420222f 5f5f772f 5f74656d ED at "/__w/_tem
   0x00035d20 702f636f 6e64615f 656e7669 726f6e6d p/conda_environm
-  0x00035d30 656e745f 39313434 34343235 32372f6c ent_9144442527/l
+  0x00035d30 656e745f 39313833 33313932 35302f6c ent_9183319250/l
   0x00035d40 69622f70 7974686f 6e332e39 2f736974 ib/python3.9/sit
   0x00035d50 652d7061 636b6167 65732f74 6f726368 e-packages/torch
   0x00035d60 2f696e63 6c756465 2f633130 2f637564 /include/c10/cud
   0x00035d70 612f696d 706c2f43 55444147 75617264 a/impl/CUDAGuard
   0x00035d80 496d706c 2e68223a 33342c20 706c6561 Impl.h":34, plea
   0x00035d90 73652072 65706f72 74206120 62756720 se report a bug 
   0x00035da0 746f2050 79546f72 63682e20 00657863 to PyTorch. .exc
@@ -746,24 +746,24 @@
   0x00035e70 6f794576 656e7400 20646576 69636573 oyEvent. devices
   0x00035e80 00676574 44657669 63654775 61726449 .getDeviceGuardI
   0x00035e90 6d706c00 71756572 79000000 00000000 mpl.query.......
   0x00035ea0 5079546f 72636820 6973206e 6f74206c PyTorch is not l
   0x00035eb0 696e6b65 64207769 74682073 7570706f inked with suppo
   0x00035ec0 72742066 6f722000 2f5f5f77 2f5f7465 rt for ./__w/_te
   0x00035ed0 6d702f63 6f6e6461 5f656e76 69726f6e mp/conda_environ
-  0x00035ee0 6d656e74 5f393134 34343432 3532372f ment_9144442527/
+  0x00035ee0 6d656e74 5f393138 33333139 3235302f ment_9183319250/
   0x00035ef0 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
   0x00035f00 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00035f10 682f696e 636c7564 652f6331 302f636f h/include/c10/co
   0x00035f20 72652f69 6d706c2f 44657669 63654775 re/impl/DeviceGu
   0x00035f30 61726449 6d706c49 6e746572 66616365 ardImplInterface
   0x00035f40 2e680073 74726561 6d5f7379 6e636872 .h.stream_synchr
   0x00035f50 6f6e697a 65000000 2f5f5f77 2f5f7465 onize.../__w/_te
   0x00035f60 6d702f63 6f6e6461 5f656e76 69726f6e mp/conda_environ
-  0x00035f70 6d656e74 5f393134 34343432 3532372f ment_9144442527/
+  0x00035f70 6d656e74 5f393138 33333139 3235302f ment_9183319250/
   0x00035f80 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
   0x00035f90 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00035fa0 682f696e 636c7564 652f6331 302f6375 h/include/c10/cu
   0x00035fb0 64612f43 55444146 756e6374 696f6e73 da/CUDAFunctions
   0x00035fc0 2e680000 00000000 45787065 63746564 .h......Expected
   0x00035fd0 20707472 5f2d3e69 735f666c 6f617428  ptr_->is_float(
   0x00035fe0 2920746f 20626520 74727565 2c206275 ) to be true, bu
@@ -771,24 +771,24 @@
   0x00036000 6f756c64 20746869 73206572 726f7220 ould this error 
   0x00036010 6d657373 61676520 62652069 6d70726f message be impro
   0x00036020 7665643f 20204966 20736f2c 20706c65 ved?  If so, ple
   0x00036030 61736520 7265706f 72742061 6e20656e ase report an en
   0x00036040 68616e63 656d656e 74207265 71756573 hancement reques
   0x00036050 7420746f 20507954 6f726368 2e290000 t to PyTorch.)..
   0x00036060 2f5f5f77 2f5f7465 6d702f63 6f6e6461 /__w/_temp/conda
-  0x00036070 5f656e76 69726f6e 6d656e74 5f393134 _environment_914
-  0x00036080 34343432 3532372f 6c69622f 70797468 4442527/lib/pyth
+  0x00036070 5f656e76 69726f6e 6d656e74 5f393138 _environment_918
+  0x00036080 33333139 3235302f 6c69622f 70797468 3319250/lib/pyth
   0x00036090 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
   0x000360a0 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x000360b0 652f6331 302f636f 72652f53 796d466c e/c10/core/SymFl
   0x000360c0 6f61742e 68000000 3020494e 5445524e oat.h...0 INTERN
   0x000360d0 414c2041 53534552 54204641 494c4544 AL ASSERT FAILED
   0x000360e0 20617420 222f5f5f 772f5f74 656d702f  at "/__w/_temp/
   0x000360f0 636f6e64 615f656e 7669726f 6e6d656e conda_environmen
-  0x00036100 745f3931 34343434 32353237 2f6c6962 t_9144442527/lib
+  0x00036100 745f3931 38333331 39323530 2f6c6962 t_9183319250/lib
   0x00036110 2f707974 686f6e33 2e392f73 6974652d /python3.9/site-
   0x00036120 7061636b 61676573 2f746f72 63682f69 packages/torch/i
   0x00036130 6e636c75 64652f41 54656e2f 636f7265 nclude/ATen/core
   0x00036140 2f697661 6c75652e 68223a35 34302c20 /ivalue.h":540, 
   0x00036150 706c6561 73652072 65706f72 74206120 please report a 
   0x00036160 62756720 746f2050 79546f72 63682e20 bug to PyTorch. 
   0x00036170 00657870 65637465 6420646f 75626c65 .expected double
```

### readelf --wide --decompress --hex-dump=.nv_fatbin {}

```diff
@@ -26202,236 +26202,236 @@
   0x0009def8 002e7368 73747274 6162002e 73747274 ..shstrtab..strt
   0x0009df08 6162002e 73796d74 6162002e 73796d74 ab..symtab..symt
   0x0009df18 61625f73 686e6478 002e6e76 2e756674 ab_shndx..nv.uft
   0x0009df28 2e656e74 7279002e 6e762e69 6e666f00 .entry..nv.info.
   0x0009df38 2e746578 742e5f5a 4e37746f 72636861 .text._ZN7torcha
   0x0009df48 6f34335f 474c4f42 414c5f5f 4e5f5f35 o43_GLOBAL__N__5
   0x0009df58 62326539 3235395f 365f6e6d 735f6375 b2e9259_6_nms_cu
-  0x0009df68 5f613163 61643162 665f3232 30323135 _a1cad1bf_220215
+  0x0009df68 5f343364 31306539 345f3231 39333135 _43d10e94_219315
   0x0009df78 6e6d735f 6b65726e 656c5f69 6d706c49 nms_kernel_implI
   0x0009df88 4e336331 30344861 6c664545 45766964 N3c104HalfEEEvid
   0x0009df98 504b545f 5079002e 6e762e69 6e666f2e PKT_Py..nv.info.
   0x0009dfa8 5f5a4e37 746f7263 68616f34 335f474c _ZN7torchao43_GL
   0x0009dfb8 4f42414c 5f5f4e5f 5f356232 65393235 OBAL__N__5b2e925
-  0x0009dfc8 395f365f 6e6d735f 63755f61 31636164 9_6_nms_cu_a1cad
-  0x0009dfd8 3162665f 32323032 31356e6d 735f6b65 1bf_220215nms_ke
+  0x0009dfc8 395f365f 6e6d735f 63755f34 33643130 9_6_nms_cu_43d10
+  0x0009dfd8 6539345f 32313933 31356e6d 735f6b65 e94_219315nms_ke
   0x0009dfe8 726e656c 5f696d70 6c494e33 63313034 rnel_implIN3c104
   0x0009dff8 48616c66 45454576 6964504b 545f5079 HalfEEEvidPKT_Py
   0x0009e008 002e6e76 2e736861 7265642e 5f5a4e37 ..nv.shared._ZN7
   0x0009e018 746f7263 68616f34 335f474c 4f42414c torchao43_GLOBAL
   0x0009e028 5f5f4e5f 5f356232 65393235 395f365f __N__5b2e9259_6_
-  0x0009e038 6e6d735f 63755f61 31636164 3162665f nms_cu_a1cad1bf_
-  0x0009e048 32323032 31356e6d 735f6b65 726e656c 220215nms_kernel
+  0x0009e038 6e6d735f 63755f34 33643130 6539345f nms_cu_43d10e94_
+  0x0009e048 32313933 31356e6d 735f6b65 726e656c 219315nms_kernel
   0x0009e058 5f696d70 6c494e33 63313034 48616c66 _implIN3c104Half
   0x0009e068 45454576 6964504b 545f5079 002e6e76 EEEvidPKT_Py..nv
   0x0009e078 2e676c6f 62616c00 2e6e762e 636f6e73 .global..nv.cons
   0x0009e088 74616e74 302e5f5a 4e37746f 72636861 tant0._ZN7torcha
   0x0009e098 6f34335f 474c4f42 414c5f5f 4e5f5f35 o43_GLOBAL__N__5
   0x0009e0a8 62326539 3235395f 365f6e6d 735f6375 b2e9259_6_nms_cu
-  0x0009e0b8 5f613163 61643162 665f3232 30323135 _a1cad1bf_220215
+  0x0009e0b8 5f343364 31306539 345f3231 39333135 _43d10e94_219315
   0x0009e0c8 6e6d735f 6b65726e 656c5f69 6d706c49 nms_kernel_implI
   0x0009e0d8 4e336331 30344861 6c664545 45766964 N3c104HalfEEEvid
   0x0009e0e8 504b545f 5079002e 74657874 2e5f5a4e PKT_Py..text._ZN
   0x0009e0f8 37746f72 6368616f 34335f47 4c4f4241 7torchao43_GLOBA
   0x0009e108 4c5f5f4e 5f5f3562 32653932 35395f36 L__N__5b2e9259_6
-  0x0009e118 5f6e6d73 5f63755f 61316361 64316266 _nms_cu_a1cad1bf
-  0x0009e128 5f323230 3231356e 6d735f6b 65726e65 _220215nms_kerne
+  0x0009e118 5f6e6d73 5f63755f 34336431 30653934 _nms_cu_43d10e94
+  0x0009e128 5f323139 3331356e 6d735f6b 65726e65 _219315nms_kerne
   0x0009e138 6c5f696d 706c4966 45457669 64504b54 l_implIfEEvidPKT
   0x0009e148 5f507900 2e6e762e 696e666f 2e5f5a4e _Py..nv.info._ZN
   0x0009e158 37746f72 6368616f 34335f47 4c4f4241 7torchao43_GLOBA
   0x0009e168 4c5f5f4e 5f5f3562 32653932 35395f36 L__N__5b2e9259_6
-  0x0009e178 5f6e6d73 5f63755f 61316361 64316266 _nms_cu_a1cad1bf
-  0x0009e188 5f323230 3231356e 6d735f6b 65726e65 _220215nms_kerne
+  0x0009e178 5f6e6d73 5f63755f 34336431 30653934 _nms_cu_43d10e94
+  0x0009e188 5f323139 3331356e 6d735f6b 65726e65 _219315nms_kerne
   0x0009e198 6c5f696d 706c4966 45457669 64504b54 l_implIfEEvidPKT
   0x0009e1a8 5f507900 2e6e762e 73686172 65642e5f _Py..nv.shared._
   0x0009e1b8 5a4e3774 6f726368 616f3433 5f474c4f ZN7torchao43_GLO
   0x0009e1c8 42414c5f 5f4e5f5f 35623265 39323539 BAL__N__5b2e9259
-  0x0009e1d8 5f365f6e 6d735f63 755f6131 63616431 _6_nms_cu_a1cad1
-  0x0009e1e8 62665f32 32303231 356e6d73 5f6b6572 bf_220215nms_ker
+  0x0009e1d8 5f365f6e 6d735f63 755f3433 64313065 _6_nms_cu_43d10e
+  0x0009e1e8 39345f32 31393331 356e6d73 5f6b6572 94_219315nms_ker
   0x0009e1f8 6e656c5f 696d706c 49664545 76696450 nel_implIfEEvidP
   0x0009e208 4b545f50 79002e6e 762e636f 6e737461 KT_Py..nv.consta
   0x0009e218 6e74302e 5f5a4e37 746f7263 68616f34 nt0._ZN7torchao4
   0x0009e228 335f474c 4f42414c 5f5f4e5f 5f356232 3_GLOBAL__N__5b2
-  0x0009e238 65393235 395f365f 6e6d735f 63755f61 e9259_6_nms_cu_a
-  0x0009e248 31636164 3162665f 32323032 31356e6d 1cad1bf_220215nm
+  0x0009e238 65393235 395f365f 6e6d735f 63755f34 e9259_6_nms_cu_4
+  0x0009e248 33643130 6539345f 32313933 31356e6d 3d10e94_219315nm
   0x0009e258 735f6b65 726e656c 5f696d70 6c496645 s_kernel_implIfE
   0x0009e268 45766964 504b545f 5079002e 74657874 EvidPKT_Py..text
   0x0009e278 2e5f5a4e 37746f72 6368616f 34335f47 ._ZN7torchao43_G
   0x0009e288 4c4f4241 4c5f5f4e 5f5f3562 32653932 LOBAL__N__5b2e92
-  0x0009e298 35395f36 5f6e6d73 5f63755f 61316361 59_6_nms_cu_a1ca
-  0x0009e2a8 64316266 5f323230 3231356e 6d735f6b d1bf_220215nms_k
+  0x0009e298 35395f36 5f6e6d73 5f63755f 34336431 59_6_nms_cu_43d1
+  0x0009e2a8 30653934 5f323139 3331356e 6d735f6b 0e94_219315nms_k
   0x0009e2b8 65726e65 6c5f696d 706c4964 45457669 ernel_implIdEEvi
   0x0009e2c8 64504b54 5f507900 2e6e762e 696e666f dPKT_Py..nv.info
   0x0009e2d8 2e5f5a4e 37746f72 6368616f 34335f47 ._ZN7torchao43_G
   0x0009e2e8 4c4f4241 4c5f5f4e 5f5f3562 32653932 LOBAL__N__5b2e92
-  0x0009e2f8 35395f36 5f6e6d73 5f63755f 61316361 59_6_nms_cu_a1ca
-  0x0009e308 64316266 5f323230 3231356e 6d735f6b d1bf_220215nms_k
+  0x0009e2f8 35395f36 5f6e6d73 5f63755f 34336431 59_6_nms_cu_43d1
+  0x0009e308 30653934 5f323139 3331356e 6d735f6b 0e94_219315nms_k
   0x0009e318 65726e65 6c5f696d 706c4964 45457669 ernel_implIdEEvi
   0x0009e328 64504b54 5f507900 2e6e762e 73686172 dPKT_Py..nv.shar
   0x0009e338 65642e5f 5a4e3774 6f726368 616f3433 ed._ZN7torchao43
   0x0009e348 5f474c4f 42414c5f 5f4e5f5f 35623265 _GLOBAL__N__5b2e
-  0x0009e358 39323539 5f365f6e 6d735f63 755f6131 9259_6_nms_cu_a1
-  0x0009e368 63616431 62665f32 32303231 356e6d73 cad1bf_220215nms
+  0x0009e358 39323539 5f365f6e 6d735f63 755f3433 9259_6_nms_cu_43
+  0x0009e368 64313065 39345f32 31393331 356e6d73 d10e94_219315nms
   0x0009e378 5f6b6572 6e656c5f 696d706c 49644545 _kernel_implIdEE
   0x0009e388 76696450 4b545f50 79002e6e 762e636f vidPKT_Py..nv.co
   0x0009e398 6e737461 6e74302e 5f5a4e37 746f7263 nstant0._ZN7torc
   0x0009e3a8 68616f34 335f474c 4f42414c 5f5f4e5f hao43_GLOBAL__N_
   0x0009e3b8 5f356232 65393235 395f365f 6e6d735f _5b2e9259_6_nms_
-  0x0009e3c8 63755f61 31636164 3162665f 32323032 cu_a1cad1bf_2202
+  0x0009e3c8 63755f34 33643130 6539345f 32313933 cu_43d10e94_2193
   0x0009e3d8 31356e6d 735f6b65 726e656c 5f696d70 15nms_kernel_imp
   0x0009e3e8 6c496445 45766964 504b545f 5079002e lIdEEvidPKT_Py..
   0x0009e3f8 64656275 675f6672 616d6500 2e72656c debug_frame..rel
   0x0009e408 2e646562 75675f66 72616d65 002e7265 .debug_frame..re
   0x0009e418 6c612e64 65627567 5f667261 6d650000 la.debug_frame..
   0x0009e428 2e736873 74727461 62002e73 74727461 .shstrtab..strta
   0x0009e438 62002e73 796d7461 62002e73 796d7461 b..symtab..symta
   0x0009e448 625f7368 6e647800 2e6e762e 7566742e b_shndx..nv.uft.
   0x0009e458 656e7472 79002e6e 762e696e 666f005f entry..nv.info._
   0x0009e468 5a4e3774 6f726368 616f3433 5f474c4f ZN7torchao43_GLO
   0x0009e478 42414c5f 5f4e5f5f 35623265 39323539 BAL__N__5b2e9259
-  0x0009e488 5f365f6e 6d735f63 755f6131 63616431 _6_nms_cu_a1cad1
-  0x0009e498 62665f32 32303231 356e6d73 5f6b6572 bf_220215nms_ker
+  0x0009e488 5f365f6e 6d735f63 755f3433 64313065 _6_nms_cu_43d10e
+  0x0009e498 39345f32 31393331 356e6d73 5f6b6572 94_219315nms_ker
   0x0009e4a8 6e656c5f 696d706c 494e3363 31303448 nel_implIN3c104H
   0x0009e4b8 616c6645 45457669 64504b54 5f507900 alfEEEvidPKT_Py.
   0x0009e4c8 2e746578 742e5f5a 4e37746f 72636861 .text._ZN7torcha
   0x0009e4d8 6f34335f 474c4f42 414c5f5f 4e5f5f35 o43_GLOBAL__N__5
   0x0009e4e8 62326539 3235395f 365f6e6d 735f6375 b2e9259_6_nms_cu
-  0x0009e4f8 5f613163 61643162 665f3232 30323135 _a1cad1bf_220215
+  0x0009e4f8 5f343364 31306539 345f3231 39333135 _43d10e94_219315
   0x0009e508 6e6d735f 6b65726e 656c5f69 6d706c49 nms_kernel_implI
   0x0009e518 4e336331 30344861 6c664545 45766964 N3c104HalfEEEvid
   0x0009e528 504b545f 5079002e 6e762e69 6e666f2e PKT_Py..nv.info.
   0x0009e538 5f5a4e37 746f7263 68616f34 335f474c _ZN7torchao43_GL
   0x0009e548 4f42414c 5f5f4e5f 5f356232 65393235 OBAL__N__5b2e925
-  0x0009e558 395f365f 6e6d735f 63755f61 31636164 9_6_nms_cu_a1cad
-  0x0009e568 3162665f 32323032 31356e6d 735f6b65 1bf_220215nms_ke
+  0x0009e558 395f365f 6e6d735f 63755f34 33643130 9_6_nms_cu_43d10
+  0x0009e568 6539345f 32313933 31356e6d 735f6b65 e94_219315nms_ke
   0x0009e578 726e656c 5f696d70 6c494e33 63313034 rnel_implIN3c104
   0x0009e588 48616c66 45454576 6964504b 545f5079 HalfEEEvidPKT_Py
   0x0009e598 002e6e76 2e736861 7265642e 5f5a4e37 ..nv.shared._ZN7
   0x0009e5a8 746f7263 68616f34 335f474c 4f42414c torchao43_GLOBAL
   0x0009e5b8 5f5f4e5f 5f356232 65393235 395f365f __N__5b2e9259_6_
-  0x0009e5c8 6e6d735f 63755f61 31636164 3162665f nms_cu_a1cad1bf_
-  0x0009e5d8 32323032 31356e6d 735f6b65 726e656c 220215nms_kernel
+  0x0009e5c8 6e6d735f 63755f34 33643130 6539345f nms_cu_43d10e94_
+  0x0009e5d8 32313933 31356e6d 735f6b65 726e656c 219315nms_kernel
   0x0009e5e8 5f696d70 6c494e33 63313034 48616c66 _implIN3c104Half
   0x0009e5f8 45454576 6964504b 545f5079 002e6e76 EEEvidPKT_Py..nv
   0x0009e608 2e676c6f 62616c00 5f5a4e34 315f494e .global._ZN41_IN
   0x0009e618 5445524e 414c5f35 62326539 3235395f TERNAL_5b2e9259_
-  0x0009e628 365f6e6d 735f6375 5f613163 61643162 6_nms_cu_a1cad1b
-  0x0009e638 665f3232 30323674 68727573 74367379 f_22026thrust6sy
+  0x0009e628 365f6e6d 735f6375 5f343364 31306539 6_nms_cu_43d10e9
+  0x0009e638 345f3231 39333674 68727573 74367379 4_21936thrust6sy
   0x0009e648 7374656d 36646574 61696c31 30736571 stem6detail10seq
   0x0009e658 75656e74 69616c33 73657145 00245f5a uential3seqE.$_Z
   0x0009e668 4e37746f 72636861 6f34335f 474c4f42 N7torchao43_GLOB
   0x0009e678 414c5f5f 4e5f5f35 62326539 3235395f AL__N__5b2e9259_
-  0x0009e688 365f6e6d 735f6375 5f613163 61643162 6_nms_cu_a1cad1b
-  0x0009e698 665f3232 30323135 6e6d735f 6b65726e f_220215nms_kern
+  0x0009e688 365f6e6d 735f6375 5f343364 31306539 6_nms_cu_43d10e9
+  0x0009e698 345f3231 39333135 6e6d735f 6b65726e 4_219315nms_kern
   0x0009e6a8 656c5f69 6d706c49 4e336331 30344861 el_implIN3c104Ha
   0x0009e6b8 6c664545 45766964 504b545f 5079245f lfEEEvidPKT_Py$_
   0x0009e6c8 5f637564 615f736d 33785f64 69765f72 _cuda_sm3x_div_r
   0x0009e6d8 6e5f6e6f 66747a5f 6633325f 736c6f77 n_noftz_f32_slow
   0x0009e6e8 70617468 00245f5f 5f5a5a4e 37746f72 path.$___ZZN7tor
   0x0009e6f8 6368616f 34335f47 4c4f4241 4c5f5f4e chao43_GLOBAL__N
   0x0009e708 5f5f3562 32653932 35395f36 5f6e6d73 __5b2e9259_6_nms
-  0x0009e718 5f63755f 61316361 64316266 5f323230 _cu_a1cad1bf_220
-  0x0009e728 3231356e 6d735f6b 65726e65 6c5f696d 215nms_kernel_im
+  0x0009e718 5f63755f 34336431 30653934 5f323139 _cu_43d10e94_219
+  0x0009e728 3331356e 6d735f6b 65726e65 6c5f696d 315nms_kernel_im
   0x0009e738 706c494e 33633130 3448616c 66454545 plIN3c104HalfEEE
   0x0009e748 76696450 4b545f50 79453131 626c6f63 vidPKT_PyE11bloc
   0x0009e758 6b5f626f 7865735f 5f353337 002e6e76 k_boxes__537..nv
   0x0009e768 2e636f6e 7374616e 74302e5f 5a4e3774 .constant0._ZN7t
   0x0009e778 6f726368 616f3433 5f474c4f 42414c5f orchao43_GLOBAL_
   0x0009e788 5f4e5f5f 35623265 39323539 5f365f6e _N__5b2e9259_6_n
-  0x0009e798 6d735f63 755f6131 63616431 62665f32 ms_cu_a1cad1bf_2
-  0x0009e7a8 32303231 356e6d73 5f6b6572 6e656c5f 20215nms_kernel_
+  0x0009e798 6d735f63 755f3433 64313065 39345f32 ms_cu_43d10e94_2
+  0x0009e7a8 31393331 356e6d73 5f6b6572 6e656c5f 19315nms_kernel_
   0x0009e7b8 696d706c 494e3363 31303448 616c6645 implIN3c104HalfE
   0x0009e7c8 45457669 64504b54 5f507900 5f706172 EEvidPKT_Py._par
   0x0009e7d8 616d005f 5a4e3774 6f726368 616f3433 am._ZN7torchao43
   0x0009e7e8 5f474c4f 42414c5f 5f4e5f5f 35623265 _GLOBAL__N__5b2e
-  0x0009e7f8 39323539 5f365f6e 6d735f63 755f6131 9259_6_nms_cu_a1
-  0x0009e808 63616431 62665f32 32303231 356e6d73 cad1bf_220215nms
+  0x0009e7f8 39323539 5f365f6e 6d735f63 755f3433 9259_6_nms_cu_43
+  0x0009e808 64313065 39345f32 31393331 356e6d73 d10e94_219315nms
   0x0009e818 5f6b6572 6e656c5f 696d706c 49664545 _kernel_implIfEE
   0x0009e828 76696450 4b545f50 79002e74 6578742e vidPKT_Py..text.
   0x0009e838 5f5a4e37 746f7263 68616f34 335f474c _ZN7torchao43_GL
   0x0009e848 4f42414c 5f5f4e5f 5f356232 65393235 OBAL__N__5b2e925
-  0x0009e858 395f365f 6e6d735f 63755f61 31636164 9_6_nms_cu_a1cad
-  0x0009e868 3162665f 32323032 31356e6d 735f6b65 1bf_220215nms_ke
+  0x0009e858 395f365f 6e6d735f 63755f34 33643130 9_6_nms_cu_43d10
+  0x0009e868 6539345f 32313933 31356e6d 735f6b65 e94_219315nms_ke
   0x0009e878 726e656c 5f696d70 6c496645 45766964 rnel_implIfEEvid
   0x0009e888 504b545f 5079002e 6e762e69 6e666f2e PKT_Py..nv.info.
   0x0009e898 5f5a4e37 746f7263 68616f34 335f474c _ZN7torchao43_GL
   0x0009e8a8 4f42414c 5f5f4e5f 5f356232 65393235 OBAL__N__5b2e925
-  0x0009e8b8 395f365f 6e6d735f 63755f61 31636164 9_6_nms_cu_a1cad
-  0x0009e8c8 3162665f 32323032 31356e6d 735f6b65 1bf_220215nms_ke
+  0x0009e8b8 395f365f 6e6d735f 63755f34 33643130 9_6_nms_cu_43d10
+  0x0009e8c8 6539345f 32313933 31356e6d 735f6b65 e94_219315nms_ke
   0x0009e8d8 726e656c 5f696d70 6c496645 45766964 rnel_implIfEEvid
   0x0009e8e8 504b545f 5079002e 6e762e73 68617265 PKT_Py..nv.share
   0x0009e8f8 642e5f5a 4e37746f 72636861 6f34335f d._ZN7torchao43_
   0x0009e908 474c4f42 414c5f5f 4e5f5f35 62326539 GLOBAL__N__5b2e9
-  0x0009e918 3235395f 365f6e6d 735f6375 5f613163 259_6_nms_cu_a1c
-  0x0009e928 61643162 665f3232 30323135 6e6d735f ad1bf_220215nms_
+  0x0009e918 3235395f 365f6e6d 735f6375 5f343364 259_6_nms_cu_43d
+  0x0009e928 31306539 345f3231 39333135 6e6d735f 10e94_219315nms_
   0x0009e938 6b65726e 656c5f69 6d706c49 66454576 kernel_implIfEEv
   0x0009e948 6964504b 545f5079 00245f5a 4e37746f idPKT_Py.$_ZN7to
   0x0009e958 72636861 6f34335f 474c4f42 414c5f5f rchao43_GLOBAL__
   0x0009e968 4e5f5f35 62326539 3235395f 365f6e6d N__5b2e9259_6_nm
-  0x0009e978 735f6375 5f613163 61643162 665f3232 s_cu_a1cad1bf_22
-  0x0009e988 30323135 6e6d735f 6b65726e 656c5f69 0215nms_kernel_i
+  0x0009e978 735f6375 5f343364 31306539 345f3231 s_cu_43d10e94_21
+  0x0009e988 39333135 6e6d735f 6b65726e 656c5f69 9315nms_kernel_i
   0x0009e998 6d706c49 66454576 6964504b 545f5079 mplIfEEvidPKT_Py
   0x0009e9a8 245f5f63 7564615f 736d3378 5f646976 $__cuda_sm3x_div
   0x0009e9b8 5f726e5f 6e6f6674 7a5f6633 325f736c _rn_noftz_f32_sl
   0x0009e9c8 6f777061 74680024 5f5f5f5a 5a4e3774 owpath.$___ZZN7t
   0x0009e9d8 6f726368 616f3433 5f474c4f 42414c5f orchao43_GLOBAL_
   0x0009e9e8 5f4e5f5f 35623265 39323539 5f365f6e _N__5b2e9259_6_n
-  0x0009e9f8 6d735f63 755f6131 63616431 62665f32 ms_cu_a1cad1bf_2
-  0x0009ea08 32303231 356e6d73 5f6b6572 6e656c5f 20215nms_kernel_
+  0x0009e9f8 6d735f63 755f3433 64313065 39345f32 ms_cu_43d10e94_2
+  0x0009ea08 31393331 356e6d73 5f6b6572 6e656c5f 19315nms_kernel_
   0x0009ea18 696d706c 49664545 76696450 4b545f50 implIfEEvidPKT_P
   0x0009ea28 79453131 626c6f63 6b5f626f 7865735f yE11block_boxes_
   0x0009ea38 5f323834 002e6e76 2e636f6e 7374616e _284..nv.constan
   0x0009ea48 74302e5f 5a4e3774 6f726368 616f3433 t0._ZN7torchao43
   0x0009ea58 5f474c4f 42414c5f 5f4e5f5f 35623265 _GLOBAL__N__5b2e
-  0x0009ea68 39323539 5f365f6e 6d735f63 755f6131 9259_6_nms_cu_a1
-  0x0009ea78 63616431 62665f32 32303231 356e6d73 cad1bf_220215nms
+  0x0009ea68 39323539 5f365f6e 6d735f63 755f3433 9259_6_nms_cu_43
+  0x0009ea78 64313065 39345f32 31393331 356e6d73 d10e94_219315nms
   0x0009ea88 5f6b6572 6e656c5f 696d706c 49664545 _kernel_implIfEE
   0x0009ea98 76696450 4b545f50 79005f5a 4e37746f vidPKT_Py._ZN7to
   0x0009eaa8 72636861 6f34335f 474c4f42 414c5f5f rchao43_GLOBAL__
   0x0009eab8 4e5f5f35 62326539 3235395f 365f6e6d N__5b2e9259_6_nm
-  0x0009eac8 735f6375 5f613163 61643162 665f3232 s_cu_a1cad1bf_22
-  0x0009ead8 30323135 6e6d735f 6b65726e 656c5f69 0215nms_kernel_i
+  0x0009eac8 735f6375 5f343364 31306539 345f3231 s_cu_43d10e94_21
+  0x0009ead8 39333135 6e6d735f 6b65726e 656c5f69 9315nms_kernel_i
   0x0009eae8 6d706c49 64454576 6964504b 545f5079 mplIdEEvidPKT_Py
   0x0009eaf8 002e7465 78742e5f 5a4e3774 6f726368 ..text._ZN7torch
   0x0009eb08 616f3433 5f474c4f 42414c5f 5f4e5f5f ao43_GLOBAL__N__
   0x0009eb18 35623265 39323539 5f365f6e 6d735f63 5b2e9259_6_nms_c
-  0x0009eb28 755f6131 63616431 62665f32 32303231 u_a1cad1bf_22021
+  0x0009eb28 755f3433 64313065 39345f32 31393331 u_43d10e94_21931
   0x0009eb38 356e6d73 5f6b6572 6e656c5f 696d706c 5nms_kernel_impl
   0x0009eb48 49644545 76696450 4b545f50 79002e6e IdEEvidPKT_Py..n
   0x0009eb58 762e696e 666f2e5f 5a4e3774 6f726368 v.info._ZN7torch
   0x0009eb68 616f3433 5f474c4f 42414c5f 5f4e5f5f ao43_GLOBAL__N__
   0x0009eb78 35623265 39323539 5f365f6e 6d735f63 5b2e9259_6_nms_c
-  0x0009eb88 755f6131 63616431 62665f32 32303231 u_a1cad1bf_22021
+  0x0009eb88 755f3433 64313065 39345f32 31393331 u_43d10e94_21931
   0x0009eb98 356e6d73 5f6b6572 6e656c5f 696d706c 5nms_kernel_impl
   0x0009eba8 49644545 76696450 4b545f50 79002e6e IdEEvidPKT_Py..n
   0x0009ebb8 762e7368 61726564 2e5f5a4e 37746f72 v.shared._ZN7tor
   0x0009ebc8 6368616f 34335f47 4c4f4241 4c5f5f4e chao43_GLOBAL__N
   0x0009ebd8 5f5f3562 32653932 35395f36 5f6e6d73 __5b2e9259_6_nms
-  0x0009ebe8 5f63755f 61316361 64316266 5f323230 _cu_a1cad1bf_220
-  0x0009ebf8 3231356e 6d735f6b 65726e65 6c5f696d 215nms_kernel_im
+  0x0009ebe8 5f63755f 34336431 30653934 5f323139 _cu_43d10e94_219
+  0x0009ebf8 3331356e 6d735f6b 65726e65 6c5f696d 315nms_kernel_im
   0x0009ec08 706c4964 45457669 64504b54 5f507900 plIdEEvidPKT_Py.
   0x0009ec18 245f5a4e 37746f72 6368616f 34335f47 $_ZN7torchao43_G
   0x0009ec28 4c4f4241 4c5f5f4e 5f5f3562 32653932 LOBAL__N__5b2e92
-  0x0009ec38 35395f36 5f6e6d73 5f63755f 61316361 59_6_nms_cu_a1ca
-  0x0009ec48 64316266 5f323230 3231356e 6d735f6b d1bf_220215nms_k
+  0x0009ec38 35395f36 5f6e6d73 5f63755f 34336431 59_6_nms_cu_43d1
+  0x0009ec48 30653934 5f323139 3331356e 6d735f6b 0e94_219315nms_k
   0x0009ec58 65726e65 6c5f696d 706c4964 45457669 ernel_implIdEEvi
   0x0009ec68 64504b54 5f507924 5f5f6375 64615f73 dPKT_Py$__cuda_s
   0x0009ec78 6d32305f 6469765f 6636345f 736c6f77 m20_div_f64_slow
   0x0009ec88 70617468 5f763200 245f5f5f 5a5a4e37 path_v2.$___ZZN7
   0x0009ec98 746f7263 68616f34 335f474c 4f42414c torchao43_GLOBAL
   0x0009eca8 5f5f4e5f 5f356232 65393235 395f365f __N__5b2e9259_6_
-  0x0009ecb8 6e6d735f 63755f61 31636164 3162665f nms_cu_a1cad1bf_
-  0x0009ecc8 32323032 31356e6d 735f6b65 726e656c 220215nms_kernel
+  0x0009ecb8 6e6d735f 63755f34 33643130 6539345f nms_cu_43d10e94_
+  0x0009ecc8 32313933 31356e6d 735f6b65 726e656c 219315nms_kernel
   0x0009ecd8 5f696d70 6c496445 45766964 504b545f _implIdEEvidPKT_
   0x0009ece8 50794531 31626c6f 636b5f62 6f786573 PyE11block_boxes
   0x0009ecf8 5f5f3331 002e6e76 2e636f6e 7374616e __31..nv.constan
   0x0009ed08 74302e5f 5a4e3774 6f726368 616f3433 t0._ZN7torchao43
   0x0009ed18 5f474c4f 42414c5f 5f4e5f5f 35623265 _GLOBAL__N__5b2e
-  0x0009ed28 39323539 5f365f6e 6d735f63 755f6131 9259_6_nms_cu_a1
-  0x0009ed38 63616431 62665f32 32303231 356e6d73 cad1bf_220215nms
+  0x0009ed28 39323539 5f365f6e 6d735f63 755f3433 9259_6_nms_cu_43
+  0x0009ed38 64313065 39345f32 31393331 356e6d73 d10e94_219315nms
   0x0009ed48 5f6b6572 6e656c5f 696d706c 49644545 _kernel_implIdEE
   0x0009ed58 76696450 4b545f50 79002e64 65627567 vidPKT_Py..debug
   0x0009ed68 5f667261 6d65002e 72656c2e 64656275 _frame..rel.debu
   0x0009ed78 675f6672 616d6500 2e72656c 612e6465 g_frame..rela.de
   0x0009ed88 6275675f 6672616d 65000000 00000000 bug_frame.......
   0x0009ed98 00000000 00000000 00000000 00000000 ................
   0x0009eda8 00000000 00000000 40000000 02100d00 ........@.......
@@ -28252,236 +28252,236 @@
   0x000a5f18 002e7368 73747274 6162002e 73747274 ..shstrtab..strt
   0x000a5f28 6162002e 73796d74 6162002e 73796d74 ab..symtab..symt
   0x000a5f38 61625f73 686e6478 002e6e76 2e756674 ab_shndx..nv.uft
   0x000a5f48 2e656e74 7279002e 6e762e69 6e666f00 .entry..nv.info.
   0x000a5f58 2e746578 742e5f5a 4e37746f 72636861 .text._ZN7torcha
   0x000a5f68 6f34335f 474c4f42 414c5f5f 4e5f5f35 o43_GLOBAL__N__5
   0x000a5f78 62326539 3235395f 365f6e6d 735f6375 b2e9259_6_nms_cu
-  0x000a5f88 5f613163 61643162 665f3232 30323135 _a1cad1bf_220215
+  0x000a5f88 5f343364 31306539 345f3231 39333135 _43d10e94_219315
   0x000a5f98 6e6d735f 6b65726e 656c5f69 6d706c49 nms_kernel_implI
   0x000a5fa8 4e336331 30344861 6c664545 45766964 N3c104HalfEEEvid
   0x000a5fb8 504b545f 5079002e 6e762e69 6e666f2e PKT_Py..nv.info.
   0x000a5fc8 5f5a4e37 746f7263 68616f34 335f474c _ZN7torchao43_GL
   0x000a5fd8 4f42414c 5f5f4e5f 5f356232 65393235 OBAL__N__5b2e925
-  0x000a5fe8 395f365f 6e6d735f 63755f61 31636164 9_6_nms_cu_a1cad
-  0x000a5ff8 3162665f 32323032 31356e6d 735f6b65 1bf_220215nms_ke
+  0x000a5fe8 395f365f 6e6d735f 63755f34 33643130 9_6_nms_cu_43d10
+  0x000a5ff8 6539345f 32313933 31356e6d 735f6b65 e94_219315nms_ke
   0x000a6008 726e656c 5f696d70 6c494e33 63313034 rnel_implIN3c104
   0x000a6018 48616c66 45454576 6964504b 545f5079 HalfEEEvidPKT_Py
   0x000a6028 002e6e76 2e736861 7265642e 5f5a4e37 ..nv.shared._ZN7
   0x000a6038 746f7263 68616f34 335f474c 4f42414c torchao43_GLOBAL
   0x000a6048 5f5f4e5f 5f356232 65393235 395f365f __N__5b2e9259_6_
-  0x000a6058 6e6d735f 63755f61 31636164 3162665f nms_cu_a1cad1bf_
-  0x000a6068 32323032 31356e6d 735f6b65 726e656c 220215nms_kernel
+  0x000a6058 6e6d735f 63755f34 33643130 6539345f nms_cu_43d10e94_
+  0x000a6068 32313933 31356e6d 735f6b65 726e656c 219315nms_kernel
   0x000a6078 5f696d70 6c494e33 63313034 48616c66 _implIN3c104Half
   0x000a6088 45454576 6964504b 545f5079 002e6e76 EEEvidPKT_Py..nv
   0x000a6098 2e676c6f 62616c00 2e6e762e 636f6e73 .global..nv.cons
   0x000a60a8 74616e74 302e5f5a 4e37746f 72636861 tant0._ZN7torcha
   0x000a60b8 6f34335f 474c4f42 414c5f5f 4e5f5f35 o43_GLOBAL__N__5
   0x000a60c8 62326539 3235395f 365f6e6d 735f6375 b2e9259_6_nms_cu
-  0x000a60d8 5f613163 61643162 665f3232 30323135 _a1cad1bf_220215
+  0x000a60d8 5f343364 31306539 345f3231 39333135 _43d10e94_219315
   0x000a60e8 6e6d735f 6b65726e 656c5f69 6d706c49 nms_kernel_implI
   0x000a60f8 4e336331 30344861 6c664545 45766964 N3c104HalfEEEvid
   0x000a6108 504b545f 5079002e 74657874 2e5f5a4e PKT_Py..text._ZN
   0x000a6118 37746f72 6368616f 34335f47 4c4f4241 7torchao43_GLOBA
   0x000a6128 4c5f5f4e 5f5f3562 32653932 35395f36 L__N__5b2e9259_6
-  0x000a6138 5f6e6d73 5f63755f 61316361 64316266 _nms_cu_a1cad1bf
-  0x000a6148 5f323230 3231356e 6d735f6b 65726e65 _220215nms_kerne
+  0x000a6138 5f6e6d73 5f63755f 34336431 30653934 _nms_cu_43d10e94
+  0x000a6148 5f323139 3331356e 6d735f6b 65726e65 _219315nms_kerne
   0x000a6158 6c5f696d 706c4966 45457669 64504b54 l_implIfEEvidPKT
   0x000a6168 5f507900 2e6e762e 696e666f 2e5f5a4e _Py..nv.info._ZN
   0x000a6178 37746f72 6368616f 34335f47 4c4f4241 7torchao43_GLOBA
   0x000a6188 4c5f5f4e 5f5f3562 32653932 35395f36 L__N__5b2e9259_6
-  0x000a6198 5f6e6d73 5f63755f 61316361 64316266 _nms_cu_a1cad1bf
-  0x000a61a8 5f323230 3231356e 6d735f6b 65726e65 _220215nms_kerne
+  0x000a6198 5f6e6d73 5f63755f 34336431 30653934 _nms_cu_43d10e94
+  0x000a61a8 5f323139 3331356e 6d735f6b 65726e65 _219315nms_kerne
   0x000a61b8 6c5f696d 706c4966 45457669 64504b54 l_implIfEEvidPKT
   0x000a61c8 5f507900 2e6e762e 73686172 65642e5f _Py..nv.shared._
   0x000a61d8 5a4e3774 6f726368 616f3433 5f474c4f ZN7torchao43_GLO
   0x000a61e8 42414c5f 5f4e5f5f 35623265 39323539 BAL__N__5b2e9259
-  0x000a61f8 5f365f6e 6d735f63 755f6131 63616431 _6_nms_cu_a1cad1
-  0x000a6208 62665f32 32303231 356e6d73 5f6b6572 bf_220215nms_ker
+  0x000a61f8 5f365f6e 6d735f63 755f3433 64313065 _6_nms_cu_43d10e
+  0x000a6208 39345f32 31393331 356e6d73 5f6b6572 94_219315nms_ker
   0x000a6218 6e656c5f 696d706c 49664545 76696450 nel_implIfEEvidP
   0x000a6228 4b545f50 79002e6e 762e636f 6e737461 KT_Py..nv.consta
   0x000a6238 6e74302e 5f5a4e37 746f7263 68616f34 nt0._ZN7torchao4
   0x000a6248 335f474c 4f42414c 5f5f4e5f 5f356232 3_GLOBAL__N__5b2
-  0x000a6258 65393235 395f365f 6e6d735f 63755f61 e9259_6_nms_cu_a
-  0x000a6268 31636164 3162665f 32323032 31356e6d 1cad1bf_220215nm
+  0x000a6258 65393235 395f365f 6e6d735f 63755f34 e9259_6_nms_cu_4
+  0x000a6268 33643130 6539345f 32313933 31356e6d 3d10e94_219315nm
   0x000a6278 735f6b65 726e656c 5f696d70 6c496645 s_kernel_implIfE
   0x000a6288 45766964 504b545f 5079002e 74657874 EvidPKT_Py..text
   0x000a6298 2e5f5a4e 37746f72 6368616f 34335f47 ._ZN7torchao43_G
   0x000a62a8 4c4f4241 4c5f5f4e 5f5f3562 32653932 LOBAL__N__5b2e92
-  0x000a62b8 35395f36 5f6e6d73 5f63755f 61316361 59_6_nms_cu_a1ca
-  0x000a62c8 64316266 5f323230 3231356e 6d735f6b d1bf_220215nms_k
+  0x000a62b8 35395f36 5f6e6d73 5f63755f 34336431 59_6_nms_cu_43d1
+  0x000a62c8 30653934 5f323139 3331356e 6d735f6b 0e94_219315nms_k
   0x000a62d8 65726e65 6c5f696d 706c4964 45457669 ernel_implIdEEvi
   0x000a62e8 64504b54 5f507900 2e6e762e 696e666f dPKT_Py..nv.info
   0x000a62f8 2e5f5a4e 37746f72 6368616f 34335f47 ._ZN7torchao43_G
   0x000a6308 4c4f4241 4c5f5f4e 5f5f3562 32653932 LOBAL__N__5b2e92
-  0x000a6318 35395f36 5f6e6d73 5f63755f 61316361 59_6_nms_cu_a1ca
-  0x000a6328 64316266 5f323230 3231356e 6d735f6b d1bf_220215nms_k
+  0x000a6318 35395f36 5f6e6d73 5f63755f 34336431 59_6_nms_cu_43d1
+  0x000a6328 30653934 5f323139 3331356e 6d735f6b 0e94_219315nms_k
   0x000a6338 65726e65 6c5f696d 706c4964 45457669 ernel_implIdEEvi
   0x000a6348 64504b54 5f507900 2e6e762e 73686172 dPKT_Py..nv.shar
   0x000a6358 65642e5f 5a4e3774 6f726368 616f3433 ed._ZN7torchao43
   0x000a6368 5f474c4f 42414c5f 5f4e5f5f 35623265 _GLOBAL__N__5b2e
-  0x000a6378 39323539 5f365f6e 6d735f63 755f6131 9259_6_nms_cu_a1
-  0x000a6388 63616431 62665f32 32303231 356e6d73 cad1bf_220215nms
+  0x000a6378 39323539 5f365f6e 6d735f63 755f3433 9259_6_nms_cu_43
+  0x000a6388 64313065 39345f32 31393331 356e6d73 d10e94_219315nms
   0x000a6398 5f6b6572 6e656c5f 696d706c 49644545 _kernel_implIdEE
   0x000a63a8 76696450 4b545f50 79002e6e 762e636f vidPKT_Py..nv.co
   0x000a63b8 6e737461 6e74302e 5f5a4e37 746f7263 nstant0._ZN7torc
   0x000a63c8 68616f34 335f474c 4f42414c 5f5f4e5f hao43_GLOBAL__N_
   0x000a63d8 5f356232 65393235 395f365f 6e6d735f _5b2e9259_6_nms_
-  0x000a63e8 63755f61 31636164 3162665f 32323032 cu_a1cad1bf_2202
+  0x000a63e8 63755f34 33643130 6539345f 32313933 cu_43d10e94_2193
   0x000a63f8 31356e6d 735f6b65 726e656c 5f696d70 15nms_kernel_imp
   0x000a6408 6c496445 45766964 504b545f 5079002e lIdEEvidPKT_Py..
   0x000a6418 64656275 675f6672 616d6500 2e72656c debug_frame..rel
   0x000a6428 2e646562 75675f66 72616d65 002e7265 .debug_frame..re
   0x000a6438 6c612e64 65627567 5f667261 6d650000 la.debug_frame..
   0x000a6448 2e736873 74727461 62002e73 74727461 .shstrtab..strta
   0x000a6458 62002e73 796d7461 62002e73 796d7461 b..symtab..symta
   0x000a6468 625f7368 6e647800 2e6e762e 7566742e b_shndx..nv.uft.
   0x000a6478 656e7472 79002e6e 762e696e 666f005f entry..nv.info._
   0x000a6488 5a4e3774 6f726368 616f3433 5f474c4f ZN7torchao43_GLO
   0x000a6498 42414c5f 5f4e5f5f 35623265 39323539 BAL__N__5b2e9259
-  0x000a64a8 5f365f6e 6d735f63 755f6131 63616431 _6_nms_cu_a1cad1
-  0x000a64b8 62665f32 32303231 356e6d73 5f6b6572 bf_220215nms_ker
+  0x000a64a8 5f365f6e 6d735f63 755f3433 64313065 _6_nms_cu_43d10e
+  0x000a64b8 39345f32 31393331 356e6d73 5f6b6572 94_219315nms_ker
   0x000a64c8 6e656c5f 696d706c 494e3363 31303448 nel_implIN3c104H
   0x000a64d8 616c6645 45457669 64504b54 5f507900 alfEEEvidPKT_Py.
   0x000a64e8 2e746578 742e5f5a 4e37746f 72636861 .text._ZN7torcha
   0x000a64f8 6f34335f 474c4f42 414c5f5f 4e5f5f35 o43_GLOBAL__N__5
   0x000a6508 62326539 3235395f 365f6e6d 735f6375 b2e9259_6_nms_cu
-  0x000a6518 5f613163 61643162 665f3232 30323135 _a1cad1bf_220215
+  0x000a6518 5f343364 31306539 345f3231 39333135 _43d10e94_219315
   0x000a6528 6e6d735f 6b65726e 656c5f69 6d706c49 nms_kernel_implI
   0x000a6538 4e336331 30344861 6c664545 45766964 N3c104HalfEEEvid
   0x000a6548 504b545f 5079002e 6e762e69 6e666f2e PKT_Py..nv.info.
   0x000a6558 5f5a4e37 746f7263 68616f34 335f474c _ZN7torchao43_GL
   0x000a6568 4f42414c 5f5f4e5f 5f356232 65393235 OBAL__N__5b2e925
-  0x000a6578 395f365f 6e6d735f 63755f61 31636164 9_6_nms_cu_a1cad
-  0x000a6588 3162665f 32323032 31356e6d 735f6b65 1bf_220215nms_ke
+  0x000a6578 395f365f 6e6d735f 63755f34 33643130 9_6_nms_cu_43d10
+  0x000a6588 6539345f 32313933 31356e6d 735f6b65 e94_219315nms_ke
   0x000a6598 726e656c 5f696d70 6c494e33 63313034 rnel_implIN3c104
   0x000a65a8 48616c66 45454576 6964504b 545f5079 HalfEEEvidPKT_Py
   0x000a65b8 002e6e76 2e736861 7265642e 5f5a4e37 ..nv.shared._ZN7
   0x000a65c8 746f7263 68616f34 335f474c 4f42414c torchao43_GLOBAL
   0x000a65d8 5f5f4e5f 5f356232 65393235 395f365f __N__5b2e9259_6_
-  0x000a65e8 6e6d735f 63755f61 31636164 3162665f nms_cu_a1cad1bf_
-  0x000a65f8 32323032 31356e6d 735f6b65 726e656c 220215nms_kernel
+  0x000a65e8 6e6d735f 63755f34 33643130 6539345f nms_cu_43d10e94_
+  0x000a65f8 32313933 31356e6d 735f6b65 726e656c 219315nms_kernel
   0x000a6608 5f696d70 6c494e33 63313034 48616c66 _implIN3c104Half
   0x000a6618 45454576 6964504b 545f5079 002e6e76 EEEvidPKT_Py..nv
   0x000a6628 2e676c6f 62616c00 5f5a4e34 315f494e .global._ZN41_IN
   0x000a6638 5445524e 414c5f35 62326539 3235395f TERNAL_5b2e9259_
-  0x000a6648 365f6e6d 735f6375 5f613163 61643162 6_nms_cu_a1cad1b
-  0x000a6658 665f3232 30323674 68727573 74367379 f_22026thrust6sy
+  0x000a6648 365f6e6d 735f6375 5f343364 31306539 6_nms_cu_43d10e9
+  0x000a6658 345f3231 39333674 68727573 74367379 4_21936thrust6sy
   0x000a6668 7374656d 36646574 61696c31 30736571 stem6detail10seq
   0x000a6678 75656e74 69616c33 73657145 00245f5a uential3seqE.$_Z
   0x000a6688 4e37746f 72636861 6f34335f 474c4f42 N7torchao43_GLOB
   0x000a6698 414c5f5f 4e5f5f35 62326539 3235395f AL__N__5b2e9259_
-  0x000a66a8 365f6e6d 735f6375 5f613163 61643162 6_nms_cu_a1cad1b
-  0x000a66b8 665f3232 30323135 6e6d735f 6b65726e f_220215nms_kern
+  0x000a66a8 365f6e6d 735f6375 5f343364 31306539 6_nms_cu_43d10e9
+  0x000a66b8 345f3231 39333135 6e6d735f 6b65726e 4_219315nms_kern
   0x000a66c8 656c5f69 6d706c49 4e336331 30344861 el_implIN3c104Ha
   0x000a66d8 6c664545 45766964 504b545f 5079245f lfEEEvidPKT_Py$_
   0x000a66e8 5f637564 615f736d 33785f64 69765f72 _cuda_sm3x_div_r
   0x000a66f8 6e5f6e6f 66747a5f 6633325f 736c6f77 n_noftz_f32_slow
   0x000a6708 70617468 00245f5f 5f5a5a4e 37746f72 path.$___ZZN7tor
   0x000a6718 6368616f 34335f47 4c4f4241 4c5f5f4e chao43_GLOBAL__N
   0x000a6728 5f5f3562 32653932 35395f36 5f6e6d73 __5b2e9259_6_nms
-  0x000a6738 5f63755f 61316361 64316266 5f323230 _cu_a1cad1bf_220
-  0x000a6748 3231356e 6d735f6b 65726e65 6c5f696d 215nms_kernel_im
+  0x000a6738 5f63755f 34336431 30653934 5f323139 _cu_43d10e94_219
+  0x000a6748 3331356e 6d735f6b 65726e65 6c5f696d 315nms_kernel_im
   0x000a6758 706c494e 33633130 3448616c 66454545 plIN3c104HalfEEE
   0x000a6768 76696450 4b545f50 79453131 626c6f63 vidPKT_PyE11bloc
   0x000a6778 6b5f626f 7865735f 5f353337 002e6e76 k_boxes__537..nv
   0x000a6788 2e636f6e 7374616e 74302e5f 5a4e3774 .constant0._ZN7t
   0x000a6798 6f726368 616f3433 5f474c4f 42414c5f orchao43_GLOBAL_
   0x000a67a8 5f4e5f5f 35623265 39323539 5f365f6e _N__5b2e9259_6_n
-  0x000a67b8 6d735f63 755f6131 63616431 62665f32 ms_cu_a1cad1bf_2
-  0x000a67c8 32303231 356e6d73 5f6b6572 6e656c5f 20215nms_kernel_
+  0x000a67b8 6d735f63 755f3433 64313065 39345f32 ms_cu_43d10e94_2
+  0x000a67c8 31393331 356e6d73 5f6b6572 6e656c5f 19315nms_kernel_
   0x000a67d8 696d706c 494e3363 31303448 616c6645 implIN3c104HalfE
   0x000a67e8 45457669 64504b54 5f507900 5f706172 EEvidPKT_Py._par
   0x000a67f8 616d005f 5a4e3774 6f726368 616f3433 am._ZN7torchao43
   0x000a6808 5f474c4f 42414c5f 5f4e5f5f 35623265 _GLOBAL__N__5b2e
-  0x000a6818 39323539 5f365f6e 6d735f63 755f6131 9259_6_nms_cu_a1
-  0x000a6828 63616431 62665f32 32303231 356e6d73 cad1bf_220215nms
+  0x000a6818 39323539 5f365f6e 6d735f63 755f3433 9259_6_nms_cu_43
+  0x000a6828 64313065 39345f32 31393331 356e6d73 d10e94_219315nms
   0x000a6838 5f6b6572 6e656c5f 696d706c 49664545 _kernel_implIfEE
   0x000a6848 76696450 4b545f50 79002e74 6578742e vidPKT_Py..text.
   0x000a6858 5f5a4e37 746f7263 68616f34 335f474c _ZN7torchao43_GL
   0x000a6868 4f42414c 5f5f4e5f 5f356232 65393235 OBAL__N__5b2e925
-  0x000a6878 395f365f 6e6d735f 63755f61 31636164 9_6_nms_cu_a1cad
-  0x000a6888 3162665f 32323032 31356e6d 735f6b65 1bf_220215nms_ke
+  0x000a6878 395f365f 6e6d735f 63755f34 33643130 9_6_nms_cu_43d10
+  0x000a6888 6539345f 32313933 31356e6d 735f6b65 e94_219315nms_ke
   0x000a6898 726e656c 5f696d70 6c496645 45766964 rnel_implIfEEvid
   0x000a68a8 504b545f 5079002e 6e762e69 6e666f2e PKT_Py..nv.info.
   0x000a68b8 5f5a4e37 746f7263 68616f34 335f474c _ZN7torchao43_GL
   0x000a68c8 4f42414c 5f5f4e5f 5f356232 65393235 OBAL__N__5b2e925
-  0x000a68d8 395f365f 6e6d735f 63755f61 31636164 9_6_nms_cu_a1cad
-  0x000a68e8 3162665f 32323032 31356e6d 735f6b65 1bf_220215nms_ke
+  0x000a68d8 395f365f 6e6d735f 63755f34 33643130 9_6_nms_cu_43d10
+  0x000a68e8 6539345f 32313933 31356e6d 735f6b65 e94_219315nms_ke
   0x000a68f8 726e656c 5f696d70 6c496645 45766964 rnel_implIfEEvid
   0x000a6908 504b545f 5079002e 6e762e73 68617265 PKT_Py..nv.share
   0x000a6918 642e5f5a 4e37746f 72636861 6f34335f d._ZN7torchao43_
   0x000a6928 474c4f42 414c5f5f 4e5f5f35 62326539 GLOBAL__N__5b2e9
-  0x000a6938 3235395f 365f6e6d 735f6375 5f613163 259_6_nms_cu_a1c
-  0x000a6948 61643162 665f3232 30323135 6e6d735f ad1bf_220215nms_
+  0x000a6938 3235395f 365f6e6d 735f6375 5f343364 259_6_nms_cu_43d
+  0x000a6948 31306539 345f3231 39333135 6e6d735f 10e94_219315nms_
   0x000a6958 6b65726e 656c5f69 6d706c49 66454576 kernel_implIfEEv
   0x000a6968 6964504b 545f5079 00245f5a 4e37746f idPKT_Py.$_ZN7to
   0x000a6978 72636861 6f34335f 474c4f42 414c5f5f rchao43_GLOBAL__
   0x000a6988 4e5f5f35 62326539 3235395f 365f6e6d N__5b2e9259_6_nm
-  0x000a6998 735f6375 5f613163 61643162 665f3232 s_cu_a1cad1bf_22
-  0x000a69a8 30323135 6e6d735f 6b65726e 656c5f69 0215nms_kernel_i
+  0x000a6998 735f6375 5f343364 31306539 345f3231 s_cu_43d10e94_21
+  0x000a69a8 39333135 6e6d735f 6b65726e 656c5f69 9315nms_kernel_i
   0x000a69b8 6d706c49 66454576 6964504b 545f5079 mplIfEEvidPKT_Py
   0x000a69c8 245f5f63 7564615f 736d3378 5f646976 $__cuda_sm3x_div
   0x000a69d8 5f726e5f 6e6f6674 7a5f6633 325f736c _rn_noftz_f32_sl
   0x000a69e8 6f777061 74680024 5f5f5f5a 5a4e3774 owpath.$___ZZN7t
   0x000a69f8 6f726368 616f3433 5f474c4f 42414c5f orchao43_GLOBAL_
   0x000a6a08 5f4e5f5f 35623265 39323539 5f365f6e _N__5b2e9259_6_n
-  0x000a6a18 6d735f63 755f6131 63616431 62665f32 ms_cu_a1cad1bf_2
-  0x000a6a28 32303231 356e6d73 5f6b6572 6e656c5f 20215nms_kernel_
+  0x000a6a18 6d735f63 755f3433 64313065 39345f32 ms_cu_43d10e94_2
+  0x000a6a28 31393331 356e6d73 5f6b6572 6e656c5f 19315nms_kernel_
   0x000a6a38 696d706c 49664545 76696450 4b545f50 implIfEEvidPKT_P
   0x000a6a48 79453131 626c6f63 6b5f626f 7865735f yE11block_boxes_
   0x000a6a58 5f323834 002e6e76 2e636f6e 7374616e _284..nv.constan
   0x000a6a68 74302e5f 5a4e3774 6f726368 616f3433 t0._ZN7torchao43
   0x000a6a78 5f474c4f 42414c5f 5f4e5f5f 35623265 _GLOBAL__N__5b2e
-  0x000a6a88 39323539 5f365f6e 6d735f63 755f6131 9259_6_nms_cu_a1
-  0x000a6a98 63616431 62665f32 32303231 356e6d73 cad1bf_220215nms
+  0x000a6a88 39323539 5f365f6e 6d735f63 755f3433 9259_6_nms_cu_43
+  0x000a6a98 64313065 39345f32 31393331 356e6d73 d10e94_219315nms
   0x000a6aa8 5f6b6572 6e656c5f 696d706c 49664545 _kernel_implIfEE
   0x000a6ab8 76696450 4b545f50 79005f5a 4e37746f vidPKT_Py._ZN7to
   0x000a6ac8 72636861 6f34335f 474c4f42 414c5f5f rchao43_GLOBAL__
   0x000a6ad8 4e5f5f35 62326539 3235395f 365f6e6d N__5b2e9259_6_nm
-  0x000a6ae8 735f6375 5f613163 61643162 665f3232 s_cu_a1cad1bf_22
-  0x000a6af8 30323135 6e6d735f 6b65726e 656c5f69 0215nms_kernel_i
+  0x000a6ae8 735f6375 5f343364 31306539 345f3231 s_cu_43d10e94_21
+  0x000a6af8 39333135 6e6d735f 6b65726e 656c5f69 9315nms_kernel_i
   0x000a6b08 6d706c49 64454576 6964504b 545f5079 mplIdEEvidPKT_Py
   0x000a6b18 002e7465 78742e5f 5a4e3774 6f726368 ..text._ZN7torch
   0x000a6b28 616f3433 5f474c4f 42414c5f 5f4e5f5f ao43_GLOBAL__N__
   0x000a6b38 35623265 39323539 5f365f6e 6d735f63 5b2e9259_6_nms_c
-  0x000a6b48 755f6131 63616431 62665f32 32303231 u_a1cad1bf_22021
+  0x000a6b48 755f3433 64313065 39345f32 31393331 u_43d10e94_21931
   0x000a6b58 356e6d73 5f6b6572 6e656c5f 696d706c 5nms_kernel_impl
   0x000a6b68 49644545 76696450 4b545f50 79002e6e IdEEvidPKT_Py..n
   0x000a6b78 762e696e 666f2e5f 5a4e3774 6f726368 v.info._ZN7torch
   0x000a6b88 616f3433 5f474c4f 42414c5f 5f4e5f5f ao43_GLOBAL__N__
   0x000a6b98 35623265 39323539 5f365f6e 6d735f63 5b2e9259_6_nms_c
-  0x000a6ba8 755f6131 63616431 62665f32 32303231 u_a1cad1bf_22021
+  0x000a6ba8 755f3433 64313065 39345f32 31393331 u_43d10e94_21931
   0x000a6bb8 356e6d73 5f6b6572 6e656c5f 696d706c 5nms_kernel_impl
   0x000a6bc8 49644545 76696450 4b545f50 79002e6e IdEEvidPKT_Py..n
   0x000a6bd8 762e7368 61726564 2e5f5a4e 37746f72 v.shared._ZN7tor
   0x000a6be8 6368616f 34335f47 4c4f4241 4c5f5f4e chao43_GLOBAL__N
   0x000a6bf8 5f5f3562 32653932 35395f36 5f6e6d73 __5b2e9259_6_nms
-  0x000a6c08 5f63755f 61316361 64316266 5f323230 _cu_a1cad1bf_220
-  0x000a6c18 3231356e 6d735f6b 65726e65 6c5f696d 215nms_kernel_im
+  0x000a6c08 5f63755f 34336431 30653934 5f323139 _cu_43d10e94_219
+  0x000a6c18 3331356e 6d735f6b 65726e65 6c5f696d 315nms_kernel_im
   0x000a6c28 706c4964 45457669 64504b54 5f507900 plIdEEvidPKT_Py.
   0x000a6c38 245f5a4e 37746f72 6368616f 34335f47 $_ZN7torchao43_G
   0x000a6c48 4c4f4241 4c5f5f4e 5f5f3562 32653932 LOBAL__N__5b2e92
-  0x000a6c58 35395f36 5f6e6d73 5f63755f 61316361 59_6_nms_cu_a1ca
-  0x000a6c68 64316266 5f323230 3231356e 6d735f6b d1bf_220215nms_k
+  0x000a6c58 35395f36 5f6e6d73 5f63755f 34336431 59_6_nms_cu_43d1
+  0x000a6c68 30653934 5f323139 3331356e 6d735f6b 0e94_219315nms_k
   0x000a6c78 65726e65 6c5f696d 706c4964 45457669 ernel_implIdEEvi
   0x000a6c88 64504b54 5f507924 5f5f6375 64615f73 dPKT_Py$__cuda_s
   0x000a6c98 6d32305f 6469765f 6636345f 736c6f77 m20_div_f64_slow
   0x000a6ca8 70617468 5f763200 245f5f5f 5a5a4e37 path_v2.$___ZZN7
   0x000a6cb8 746f7263 68616f34 335f474c 4f42414c torchao43_GLOBAL
   0x000a6cc8 5f5f4e5f 5f356232 65393235 395f365f __N__5b2e9259_6_
-  0x000a6cd8 6e6d735f 63755f61 31636164 3162665f nms_cu_a1cad1bf_
-  0x000a6ce8 32323032 31356e6d 735f6b65 726e656c 220215nms_kernel
+  0x000a6cd8 6e6d735f 63755f34 33643130 6539345f nms_cu_43d10e94_
+  0x000a6ce8 32313933 31356e6d 735f6b65 726e656c 219315nms_kernel
   0x000a6cf8 5f696d70 6c496445 45766964 504b545f _implIdEEvidPKT_
   0x000a6d08 50794531 31626c6f 636b5f62 6f786573 PyE11block_boxes
   0x000a6d18 5f5f3331 002e6e76 2e636f6e 7374616e __31..nv.constan
   0x000a6d28 74302e5f 5a4e3774 6f726368 616f3433 t0._ZN7torchao43
   0x000a6d38 5f474c4f 42414c5f 5f4e5f5f 35623265 _GLOBAL__N__5b2e
-  0x000a6d48 39323539 5f365f6e 6d735f63 755f6131 9259_6_nms_cu_a1
-  0x000a6d58 63616431 62665f32 32303231 356e6d73 cad1bf_220215nms
+  0x000a6d48 39323539 5f365f6e 6d735f63 755f3433 9259_6_nms_cu_43
+  0x000a6d58 64313065 39345f32 31393331 356e6d73 d10e94_219315nms
   0x000a6d68 5f6b6572 6e656c5f 696d706c 49644545 _kernel_implIdEE
   0x000a6d78 76696450 4b545f50 79002e64 65627567 vidPKT_Py..debug
   0x000a6d88 5f667261 6d65002e 72656c2e 64656275 _frame..rel.debu
   0x000a6d98 675f6672 616d6500 2e72656c 612e6465 g_frame..rela.de
   0x000a6da8 6275675f 6672616d 65000000 00000000 bug_frame.......
   0x000a6db8 00000000 00000000 00000000 00000000 ................
   0x000a6dc8 00000000 00000000 40000000 02100d00 ........@.......
```

### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,10 +1,10 @@
 
 Hex dump of section '.strtab':
-  0x00000000 00746d70 7866745f 30303030 30383737 .tmpxft_00000877
+  0x00000000 00746d70 7866745f 30303030 30383665 .tmpxft_0000086e
   0x00000010 5f303030 30303030 302d365f 6670365f _00000000-6_fp6_
   0x00000020 6c696e65 61722e63 6f6d7075 74655f38 linear.compute_8
   0x00000030 362e6375 64616665 312e6370 70006661 6.cudafe1.cpp.fa
   0x00000040 7462696e 44617461 005f5a39 4b65726e tbinData._Z9Kern
   0x00000050 656c5f45 78493132 54696c69 6e67436f el_ExI12TilingCo
   0x00000060 6e666967 494c6934 454c6931 454c6938 nfigILi4ELi1ELi8
   0x00000070 45456645 76503131 43557374 7265616d EEfEvP11CUstream
@@ -133,29 +133,29 @@
   0x00000820 5f6b6579 7365745f 77697468 5f414449 _keyset_with_ADI
   0x00000830 6e706c61 63654f72 56696577 45005f5a nplaceOrViewE._Z
   0x00000840 4e37746f 72636861 6f323366 70365f6c N7torchao23fp6_l
   0x00000850 696e6561 725f666f 72776172 645f6375 inear_forward_cu
   0x00000860 6461454e 32617436 54656e73 6f724553 daEN2at6TensorES
   0x00000870 315f5331 5f6c2e63 6f6c6400 5f474c4f 1_S1_l.cold._GLO
   0x00000880 42414c5f 5f737562 5f495f74 6d707866 BAL__sub_I_tmpxf
-  0x00000890 745f3030 30303038 37375f30 30303030 t_00000877_00000
+  0x00000890 745f3030 30303038 36655f30 30303030 t_0000086e_00000
   0x000008a0 3030305f 365f6670 365f6c69 6e656172 000_6_fp6_linear
   0x000008b0 2e636f6d 70757465 5f38362e 63756461 .compute_86.cuda
   0x000008c0 6665312e 63707000 5f5a5374 4c385f5f fe1.cpp._ZStL8__
   0x000008d0 696f696e 6974005f 5a4e3774 6f726368 ioinit._ZN7torch
   0x000008e0 616f4c34 35544f52 43485f4c 49425241 aoL45TORCH_LIBRA
   0x000008f0 52595f49 4d504c5f 73746174 69635f69 RY_IMPL_static_i
   0x00000900 6e69745f 746f7263 68616f5f 43554441 nit_torchao_CUDA
   0x00000910 5f324500 5f474c4f 42414c5f 5f737562 _2E._GLOBAL__sub
   0x00000920 5f495f74 6d707866 745f3030 30303038 _I_tmpxft_000008
-  0x00000930 37375f30 30303030 3030305f 365f6670 77_00000000_6_fp
+  0x00000930 36655f30 30303030 3030305f 365f6670 6e_00000000_6_fp
   0x00000940 365f6c69 6e656172 2e636f6d 70757465 6_linear.compute
   0x00000950 5f38362e 63756461 6665312e 6370702e _86.cudafe1.cpp.
   0x00000960 636f6c64 00746d70 7866745f 30303030 cold.tmpxft_0000
-  0x00000970 30383738 5f303030 30303030 302d365f 0878_00000000-6_
+  0x00000970 30383666 5f303030 30303030 302d365f 086f_00000000-6_
   0x00000980 77656967 68745f71 75616e74 2e636f6d weight_quant.com
   0x00000990 70757465 5f38362e 63756461 6665312e pute_86.cudafe1.
   0x000009a0 63707000 5f5a3133 63617374 5f667031 cpp._Z13cast_fp1
   0x000009b0 365f6670 36507450 682e636f 6c64005f 6_fp6PtPh.cold._
   0x000009c0 5a323977 65696768 745f7072 65706163 Z29weight_prepac
   0x000009d0 6b696e67 5f667031 365f746f 5f667036 king_fp16_to_fp6
   0x000009e0 50745068 6d6d2e63 6f6c6400 5f5a4e37 PtPhmm.cold._ZN7
@@ -163,46 +163,46 @@
   0x00000a00 5f667036 5f637075 454e3261 74365465 _fp6_cpuEN2at6Te
   0x00000a10 6e736f72 452e636f 6c64005f 5a4e3774 nsorE.cold._ZN7t
   0x00000a20 6f726368 616f3235 77656967 68745f6d orchao25weight_m
   0x00000a30 61747269 785f6465 7175616e 745f6370 atrix_dequant_cp
   0x00000a40 75454e32 61743654 656e736f 72455331 uEN2at6TensorES1
   0x00000a50 5f2e636f 6c64005f 474c4f42 414c5f5f _.cold._GLOBAL__
   0x00000a60 7375625f 495f746d 70786674 5f303030 sub_I_tmpxft_000
-  0x00000a70 30303837 385f3030 30303030 30305f36 00878_00000000_6
+  0x00000a70 30303836 665f3030 30303030 30305f36 0086f_00000000_6
   0x00000a80 5f776569 6768745f 7175616e 742e636f _weight_quant.co
   0x00000a90 6d707574 655f3836 2e637564 61666531 mpute_86.cudafe1
   0x00000aa0 2e637070 005f5a4e 37746f72 6368616f .cpp._ZN7torchao
   0x00000ab0 4c343454 4f524348 5f4c4942 52415259 L44TORCH_LIBRARY
   0x00000ac0 5f494d50 4c5f7374 61746963 5f696e69 _IMPL_static_ini
   0x00000ad0 745f746f 72636861 6f5f4350 555f3245 t_torchao_CPU_2E
   0x00000ae0 005f474c 4f42414c 5f5f7375 625f495f ._GLOBAL__sub_I_
-  0x00000af0 746d7078 66745f30 30303030 3837385f tmpxft_00000878_
+  0x00000af0 746d7078 66745f30 30303030 3836665f tmpxft_0000086f_
   0x00000b00 30303030 30303030 5f365f77 65696768 00000000_6_weigh
   0x00000b10 745f7175 616e742e 636f6d70 7574655f t_quant.compute_
   0x00000b20 38362e63 75646166 65312e63 70702e63 86.cudafe1.cpp.c
   0x00000b30 6f6c6400 746d7078 66745f30 30303030 old.tmpxft_00000
-  0x00000b40 3837395f 30303030 30303030 2d365f6e 879_00000000-6_n
+  0x00000b40 3837305f 30303030 30303030 2d365f6e 870_00000000-6_n
   0x00000b50 6d732e63 6f6d7075 74655f38 362e6375 ms.compute_86.cu
   0x00000b60 64616665 312e6370 70005f5a 4e336331 dafe1.cpp._ZN3c1
   0x00000b70 304c3874 6f537472 696e6745 4e535f31 0L8toStringENS_1
   0x00000b80 30536361 6c617254 79706545 005f5a4e 0ScalarTypeE._ZN
   0x00000b90 33633130 3653796d 496e7438 72656c65 3c106SymInt8rele
   0x00000ba0 6173655f 45762e70 6172742e 30005f5a ase_Ev.part.0._Z
   0x00000bb0 4e37746f 72636861 6f34335f 474c4f42 N7torchao43_GLOB
   0x00000bc0 414c5f5f 4e5f5f35 62326539 3235395f AL__N__5b2e9259_
-  0x00000bd0 365f6e6d 735f6375 5f613163 61643162 6_nms_cu_a1cad1b
-  0x00000be0 665f3232 30323130 6e6d735f 6b65726e f_220210nms_kern
+  0x00000bd0 365f6e6d 735f6375 5f343364 31306539 6_nms_cu_43d10e9
+  0x00000be0 345f3231 39333130 6e6d735f 6b65726e 4_219310nms_kern
   0x00000bf0 656c4552 4b4e3261 74365465 6e736f72 elERKN2at6Tensor
   0x00000c00 4553345f 642e636f 6c64005f 474c4f42 ES4_d.cold._GLOB
   0x00000c10 414c5f5f 7375625f 495f746d 70786674 AL__sub_I_tmpxft
-  0x00000c20 5f303030 30303837 395f3030 30303030 _00000879_000000
+  0x00000c20 5f303030 30303837 305f3030 30303030 _00000870_000000
   0x00000c30 30305f36 5f6e6d73 2e636f6d 70757465 00_6_nms.compute
   0x00000c40 5f38362e 63756461 6665312e 63707000 _86.cudafe1.cpp.
   0x00000c50 5f474c4f 42414c5f 5f737562 5f495f74 _GLOBAL__sub_I_t
-  0x00000c60 6d707866 745f3030 30303038 37395f30 mpxft_00000879_0
+  0x00000c60 6d707866 745f3030 30303038 37305f30 mpxft_00000870_0
   0x00000c70 30303030 3030305f 365f6e6d 732e636f 0000000_6_nms.co
   0x00000c80 6d707574 655f3836 2e637564 61666531 mpute_86.cudafe1
   0x00000c90 2e637070 2e636f6c 64005f47 4c4f4241 .cpp.cold._GLOBA
   0x00000ca0 4c5f5f73 75625f49 5f667036 5f6c6c6d L__sub_I_fp6_llm
   0x00000cb0 2e637070 005f5a4c 3434544f 5243485f .cpp._ZL44TORCH_
   0x00000cc0 4c494252 4152595f 46524147 4d454e54 LIBRARY_FRAGMENT
   0x00000cd0 5f737461 7469635f 696e6974 5f746f72 _static_init_tor
@@ -852,107 +852,107 @@
   0x00003510 736f7245 524b5335 5f53375f 64455335 sorERKS5_S7_dES5
   0x00003520 5f4e535f 34677574 73387479 70656c69 _NS_4guts8typeli
   0x00003530 73743874 7970656c 69737449 4a53375f st8typelistIJS7_
   0x00003540 53375f64 45454545 4553385f 45346361 S7_dEEEEES8_E4ca
   0x00003550 6c6c4550 4e535f31 344f7065 7261746f llEPNS_14Operato
   0x00003560 724b6572 6e656c45 4e535f31 34446973 rKernelENS_14Dis
   0x00003570 70617463 684b6579 53657445 53375f53 patchKeySetES7_S
-  0x00003580 375f6400 5f5a4e37 746f7263 68616f34 7_d._ZN7torchao4
-  0x00003590 335f474c 4f42414c 5f5f4e5f 5f356232 3_GLOBAL__N__5b2
-  0x000035a0 65393235 395f365f 6e6d735f 63755f61 e9259_6_nms_cu_a
-  0x000035b0 31636164 3162665f 32323032 31356e6d 1cad1bf_220215nm
-  0x000035c0 735f6b65 726e656c 5f696d70 6c494e33 s_kernel_implIN3
-  0x000035d0 63313034 48616c66 45454576 6964504b c104HalfEEEvidPK
-  0x000035e0 545f5079 00737472 64757040 474c4942 T_Py.strdup@GLIB
-  0x000035f0 435f322e 322e3500 5f5a4e4b 33633130 C_2.2.5._ZNK3c10
-  0x00003600 34637564 6134696d 706c3133 43554441 4cuda4impl13CUDA
-  0x00003610 47756172 64496d70 6c313164 65766963 GuardImpl11devic
-  0x00003620 65436f75 6e744576 005f5a4e 33633130 eCountEv._ZN3c10
-  0x00003630 31315379 6d4e6f64 65496d70 6c313169 11SymNodeImpl11i
-  0x00003640 735f7379 6d626f6c 69634576 005f5a4e s_symbolicEv._ZN
-  0x00003650 33633130 34696d70 6c33316d 616b655f 3c104impl31make_
-  0x00003660 626f7865 645f6672 6f6d5f75 6e626f78 boxed_from_unbox
-  0x00003670 65645f66 756e6374 6f72494e 53305f36 ed_functorINS0_6
-  0x00003680 64657461 696c3331 57726170 46756e63 detail31WrapFunc
-  0x00003690 74696f6e 496e746f 52756e74 696d6546 tionIntoRuntimeF
-  0x000036a0 756e6374 6f725f49 50464e32 61743654 unctor_IPFN2at6T
-  0x000036b0 656e736f 72455335 5f53355f 53355f6c ensorES5_S5_S5_l
-  0x000036c0 4553355f 4e535f34 67757473 38747970 ES5_NS_4guts8typ
-  0x000036d0 656c6973 74387479 70656c69 7374494a elist8typelistIJ
-  0x000036e0 53355f53 355f5335 5f6c4545 4545454c S5_S5_S5_lEEEEEL
-  0x000036f0 62304545 3463616c 6c45504e 535f3134 b0EE4callEPNS_14
-  0x00003700 4f706572 61746f72 4b65726e 656c4552 OperatorKernelER
-  0x00003710 4b4e535f 31344f70 65726174 6f724861 KNS_14OperatorHa
-  0x00003720 6e646c65 454e535f 31344469 73706174 ndleENS_14Dispat
-  0x00003730 63684b65 79536574 45505374 36766563 chKeySetEPSt6vec
-  0x00003740 746f7249 4e535f36 4956616c 75654553 torINS_6IValueES
-  0x00003750 6149534c 5f454500 5f5a5456 53743139 aISL_EE._ZTVSt19
-  0x00003760 6261645f 6f707469 6f6e616c 5f616363 bad_optional_acc
-  0x00003770 65737300 50794d6f 64756c65 5f437265 ess.PyModule_Cre
-  0x00003780 61746532 005f5f63 78615f62 6567696e ate2.__cxa_begin
-  0x00003790 5f636174 63684043 58584142 495f312e _catch@CXXABI_1.
-  0x000037a0 33005f5a 4e336331 30313153 796d4e6f 3._ZN3c1011SymNo
-  0x000037b0 6465496d 706c3773 796d5f6d 696e4552 deImpl7sym_minER
-  0x000037c0 4b4e535f 3133696e 74727573 6976655f KNS_13intrusive_
-  0x000037d0 70747249 53305f4e 535f3664 65746169 ptrIS0_NS_6detai
-  0x000037e0 6c333469 6e747275 73697665 5f746172 l34intrusive_tar
-  0x000037f0 6765745f 64656661 756c745f 6e756c6c get_default_null
-  0x00003800 5f747970 65495330 5f454545 45005f5a _typeIS0_EEEE._Z
-  0x00003810 4e336331 30313153 796d4e6f 6465496d N3c1011SymNodeIm
-  0x00003820 706c3330 69735f63 68616e6e 656c735f pl30is_channels_
-  0x00003830 6c617374 5f636f6e 74696775 6f75735f last_contiguous_
-  0x00003840 3264454e 535f3841 72726179 52656649 2dENS_8ArrayRefI
-  0x00003850 4e535f31 33696e74 72757369 76655f70 NS_13intrusive_p
-  0x00003860 74724953 305f4e53 5f366465 7461696c trIS0_NS_6detail
-  0x00003870 3334696e 74727573 6976655f 74617267 34intrusive_targ
-  0x00003880 65745f64 65666175 6c745f6e 756c6c5f et_default_null_
-  0x00003890 74797065 4953305f 45454545 45455337 typeIS0_EEEEEES7
-  0x000038a0 5f005f5a 4e4b3363 31303469 6d706c31 _._ZNK3c104impl1
-  0x000038b0 36566972 7475616c 47756172 64496d70 6VirtualGuardImp
-  0x000038c0 6c313465 78636861 6e676553 74726561 l14exchangeStrea
-  0x000038d0 6d454e53 5f365374 7265616d 45005f5a mENS_6StreamE._Z
-  0x000038e0 4e4b3363 31303463 75646134 696d706c NK3c104cuda4impl
-  0x000038f0 31334355 44414775 61726449 6d706c31 13CUDAGuardImpl1
-  0x00003900 30717565 72794576 656e7445 5076005f 0queryEventEPv._
-  0x00003910 5a4e3363 31303133 696e7472 75736976 ZN3c1013intrusiv
-  0x00003920 655f7074 72494e53 5f313054 656e736f e_ptrINS_10Tenso
-  0x00003930 72496d70 6c454e53 5f313955 6e646566 rImplENS_19Undef
-  0x00003940 696e6564 54656e73 6f72496d 706c4545 inedTensorImplEE
-  0x00003950 36726573 65745f45 76005f5a 4e537431 6reset_Ev._ZNSt1
-  0x00003960 35626173 69635f73 7472696e 67627566 5basic_stringbuf
-  0x00003970 49635374 31316368 61725f74 72616974 IcSt11char_trait
-  0x00003980 73496345 53614963 45454432 4576005f sIcESaIcEED2Ev._
-  0x00003990 5a4e3363 31303131 53796d4e 6f646549 ZN3c1011SymNodeI
-  0x000039a0 6d706c37 73796d5f 616e6445 524b4e53 mpl7sym_andERKNS
-  0x000039b0 5f313369 6e747275 73697665 5f707472 _13intrusive_ptr
-  0x000039c0 4953305f 4e535f36 64657461 696c3334 IS0_NS_6detail34
-  0x000039d0 696e7472 75736976 655f7461 72676574 intrusive_target
-  0x000039e0 5f646566 61756c74 5f6e756c 6c5f7479 _default_null_ty
-  0x000039f0 70654953 305f4545 4545005f 5a4e5374 peIS0_EEEE._ZNSt
-  0x00003a00 39657863 65707469 6f6e4432 45764047 9exceptionD2Ev@G
-  0x00003a10 4c494243 58585f33 2e34005f 5a4e5374 LIBCXX_3.4._ZNSt
-  0x00003a20 36766563 746f7249 5031315f 74797065 6vectorIP11_type
-  0x00003a30 6f626a65 63745361 4953315f 45453137 objectSaIS1_EE17
-  0x00003a40 5f4d5f72 65616c6c 6f635f69 6e736572 _M_realloc_inser
-  0x00003a50 74494a53 315f4545 45764e39 5f5f676e tIJS1_EEEvN9__gn
-  0x00003a60 755f6378 7831375f 5f6e6f72 6d616c5f u_cxx17__normal_
-  0x00003a70 69746572 61746f72 49505331 5f53335f iteratorIPS1_S3_
-  0x00003a80 45454470 4f545f00 50794279 74654172 EEDpOT_.PyByteAr
-  0x00003a90 7261795f 54797065 005f5a4e 33633130 ray_Type._ZN3c10
-  0x00003aa0 31315379 6d4e6f64 65496d70 6c336d6f 11SymNodeImpl3mo
-  0x00003ab0 6445524b 4e535f31 33696e74 72757369 dERKNS_13intrusi
-  0x00003ac0 76655f70 74724953 305f4e53 5f366465 ve_ptrIS0_NS_6de
-  0x00003ad0 7461696c 3334696e 74727573 6976655f tail34intrusive_
-  0x00003ae0 74617267 65745f64 65666175 6c745f6e target_default_n
-  0x00003af0 756c6c5f 74797065 4953305f 45454545 ull_typeIS0_EEEE
-  0x00003b00 005f5a4e 4b336331 30364956 616c7565 ._ZNK3c106IValue
-  0x00003b10 37746167 4b696e64 4576005f 5a4e4b33 7tagKindEv._ZNK3
-  0x00003b20 63313034 696d706c 31365669 72747561 c104impl16Virtua
-  0x00003b30 6c477561 7264496d 706c3967 65745374 lGuardImpl9getSt
-  0x00003b40 7265616d 454e535f 36446576 69636545 reamENS_6DeviceE
+  0x00003580 375f6400 73747264 75704047 4c494243 7_d.strdup@GLIBC
+  0x00003590 5f322e32 2e35005f 5a4e4b33 63313034 _2.2.5._ZNK3c104
+  0x000035a0 63756461 34696d70 6c313343 55444147 cuda4impl13CUDAG
+  0x000035b0 75617264 496d706c 31316465 76696365 uardImpl11device
+  0x000035c0 436f756e 74457600 5f5a4e33 63313031 CountEv._ZN3c101
+  0x000035d0 3153796d 4e6f6465 496d706c 31316973 1SymNodeImpl11is
+  0x000035e0 5f73796d 626f6c69 63457600 5f5a4e33 _symbolicEv._ZN3
+  0x000035f0 63313034 696d706c 33316d61 6b655f62 c104impl31make_b
+  0x00003600 6f786564 5f66726f 6d5f756e 626f7865 oxed_from_unboxe
+  0x00003610 645f6675 6e63746f 72494e53 305f3664 d_functorINS0_6d
+  0x00003620 65746169 6c333157 72617046 756e6374 etail31WrapFunct
+  0x00003630 696f6e49 6e746f52 756e7469 6d654675 ionIntoRuntimeFu
+  0x00003640 6e63746f 725f4950 464e3261 74365465 nctor_IPFN2at6Te
+  0x00003650 6e736f72 4553355f 53355f53 355f6c45 nsorES5_S5_S5_lE
+  0x00003660 53355f4e 535f3467 75747338 74797065 S5_NS_4guts8type
+  0x00003670 6c697374 38747970 656c6973 74494a53 list8typelistIJS
+  0x00003680 355f5335 5f53355f 6c454545 45454c62 5_S5_S5_lEEEEELb
+  0x00003690 30454534 63616c6c 45504e53 5f31344f 0EE4callEPNS_14O
+  0x000036a0 70657261 746f724b 65726e65 6c45524b peratorKernelERK
+  0x000036b0 4e535f31 344f7065 7261746f 7248616e NS_14OperatorHan
+  0x000036c0 646c6545 4e535f31 34446973 70617463 dleENS_14Dispatc
+  0x000036d0 684b6579 53657445 50537436 76656374 hKeySetEPSt6vect
+  0x000036e0 6f72494e 535f3649 56616c75 65455361 orINS_6IValueESa
+  0x000036f0 49534c5f 4545005f 5a545653 74313962 ISL_EE._ZTVSt19b
+  0x00003700 61645f6f 7074696f 6e616c5f 61636365 ad_optional_acce
+  0x00003710 73730050 794d6f64 756c655f 43726561 ss.PyModule_Crea
+  0x00003720 74653200 5f5f6378 615f6265 67696e5f te2.__cxa_begin_
+  0x00003730 63617463 68404358 58414249 5f312e33 catch@CXXABI_1.3
+  0x00003740 005f5a4e 33633130 31315379 6d4e6f64 ._ZN3c1011SymNod
+  0x00003750 65496d70 6c377379 6d5f6d69 6e45524b eImpl7sym_minERK
+  0x00003760 4e535f31 33696e74 72757369 76655f70 NS_13intrusive_p
+  0x00003770 74724953 305f4e53 5f366465 7461696c trIS0_NS_6detail
+  0x00003780 3334696e 74727573 6976655f 74617267 34intrusive_targ
+  0x00003790 65745f64 65666175 6c745f6e 756c6c5f et_default_null_
+  0x000037a0 74797065 4953305f 45454545 005f5a4e typeIS0_EEEE._ZN
+  0x000037b0 33633130 31315379 6d4e6f64 65496d70 3c1011SymNodeImp
+  0x000037c0 6c333069 735f6368 616e6e65 6c735f6c l30is_channels_l
+  0x000037d0 6173745f 636f6e74 6967756f 75735f32 ast_contiguous_2
+  0x000037e0 64454e53 5f384172 72617952 6566494e dENS_8ArrayRefIN
+  0x000037f0 535f3133 696e7472 75736976 655f7074 S_13intrusive_pt
+  0x00003800 72495330 5f4e535f 36646574 61696c33 rIS0_NS_6detail3
+  0x00003810 34696e74 72757369 76655f74 61726765 4intrusive_targe
+  0x00003820 745f6465 6661756c 745f6e75 6c6c5f74 t_default_null_t
+  0x00003830 79706549 53305f45 45454545 4553375f ypeIS0_EEEEEES7_
+  0x00003840 005f5a4e 4b336331 3034696d 706c3136 ._ZNK3c104impl16
+  0x00003850 56697274 75616c47 75617264 496d706c VirtualGuardImpl
+  0x00003860 31346578 6368616e 67655374 7265616d 14exchangeStream
+  0x00003870 454e535f 36537472 65616d45 005f5a4e ENS_6StreamE._ZN
+  0x00003880 4b336331 30346375 64613469 6d706c31 K3c104cuda4impl1
+  0x00003890 33435544 41477561 7264496d 706c3130 3CUDAGuardImpl10
+  0x000038a0 71756572 79457665 6e744550 76005f5a queryEventEPv._Z
+  0x000038b0 4e336331 30313369 6e747275 73697665 N3c1013intrusive
+  0x000038c0 5f707472 494e535f 31305465 6e736f72 _ptrINS_10Tensor
+  0x000038d0 496d706c 454e535f 3139556e 64656669 ImplENS_19Undefi
+  0x000038e0 6e656454 656e736f 72496d70 6c454536 nedTensorImplEE6
+  0x000038f0 72657365 745f4576 005f5a4e 53743135 reset_Ev._ZNSt15
+  0x00003900 62617369 635f7374 72696e67 62756649 basic_stringbufI
+  0x00003910 63537431 31636861 725f7472 61697473 cSt11char_traits
+  0x00003920 49634553 61496345 45443245 76005f5a IcESaIcEED2Ev._Z
+  0x00003930 4e336331 30313153 796d4e6f 6465496d N3c1011SymNodeIm
+  0x00003940 706c3773 796d5f61 6e644552 4b4e535f pl7sym_andERKNS_
+  0x00003950 3133696e 74727573 6976655f 70747249 13intrusive_ptrI
+  0x00003960 53305f4e 535f3664 65746169 6c333469 S0_NS_6detail34i
+  0x00003970 6e747275 73697665 5f746172 6765745f ntrusive_target_
+  0x00003980 64656661 756c745f 6e756c6c 5f747970 default_null_typ
+  0x00003990 65495330 5f454545 45005f5a 4e537439 eIS0_EEEE._ZNSt9
+  0x000039a0 65786365 7074696f 6e443245 7640474c exceptionD2Ev@GL
+  0x000039b0 49424358 585f332e 34005f5a 4e537436 IBCXX_3.4._ZNSt6
+  0x000039c0 76656374 6f724950 31315f74 7970656f vectorIP11_typeo
+  0x000039d0 626a6563 74536149 53315f45 4531375f bjectSaIS1_EE17_
+  0x000039e0 4d5f7265 616c6c6f 635f696e 73657274 M_realloc_insert
+  0x000039f0 494a5331 5f454545 764e395f 5f676e75 IJS1_EEEvN9__gnu
+  0x00003a00 5f637878 31375f5f 6e6f726d 616c5f69 _cxx17__normal_i
+  0x00003a10 74657261 746f7249 5053315f 53335f45 teratorIPS1_S3_E
+  0x00003a20 4544704f 545f0050 79427974 65417272 EDpOT_.PyByteArr
+  0x00003a30 61795f54 79706500 5f5a4e33 63313031 ay_Type._ZN3c101
+  0x00003a40 3153796d 4e6f6465 496d706c 336d6f64 1SymNodeImpl3mod
+  0x00003a50 45524b4e 535f3133 696e7472 75736976 ERKNS_13intrusiv
+  0x00003a60 655f7074 72495330 5f4e535f 36646574 e_ptrIS0_NS_6det
+  0x00003a70 61696c33 34696e74 72757369 76655f74 ail34intrusive_t
+  0x00003a80 61726765 745f6465 6661756c 745f6e75 arget_default_nu
+  0x00003a90 6c6c5f74 79706549 53305f45 45454500 ll_typeIS0_EEEE.
+  0x00003aa0 5f5a4e4b 33633130 36495661 6c756537 _ZNK3c106IValue7
+  0x00003ab0 7461674b 696e6445 76005f5a 4e4b3363 tagKindEv._ZNK3c
+  0x00003ac0 31303469 6d706c31 36566972 7475616c 104impl16Virtual
+  0x00003ad0 47756172 64496d70 6c396765 74537472 GuardImpl9getStr
+  0x00003ae0 65616d45 4e535f36 44657669 63654500 eamENS_6DeviceE.
+  0x00003af0 5f5a4e37 746f7263 68616f34 335f474c _ZN7torchao43_GL
+  0x00003b00 4f42414c 5f5f4e5f 5f356232 65393235 OBAL__N__5b2e925
+  0x00003b10 395f365f 6e6d735f 63755f34 33643130 9_6_nms_cu_43d10
+  0x00003b20 6539345f 32313933 31356e6d 735f6b65 e94_219315nms_ke
+  0x00003b30 726e656c 5f696d70 6c494e33 63313034 rnel_implIN3c104
+  0x00003b40 48616c66 45454576 6964504b 545f5079 HalfEEEvidPKT_Py
   0x00003b50 005f6669 6e69005f 5a4e4b53 74397479 ._fini._ZNKSt9ty
   0x00003b60 70655f69 6e666f39 68617368 5f636f64 pe_info9hash_cod
   0x00003b70 65457600 5f5a4e33 63313032 30696e74 eEv._ZN3c1020int
   0x00003b80 72757369 76655f70 74725f74 61726765 rusive_ptr_targe
   0x00003b90 74443145 76005f5a 4e336331 30313369 tD1Ev._ZN3c1013i
   0x00003ba0 6e747275 73697665 5f707472 494e535f ntrusive_ptrINS_
   0x00003bb0 31305465 6e736f72 496d706c 454e535f 10TensorImplENS_
@@ -1139,1076 +1139,1076 @@
   0x00004700 53345f45 45454544 32457600 6d656d73 S4_EEEED2Ev.mems
   0x00004710 65744047 4c494243 5f322e32 2e350050 et@GLIBC_2.2.5.P
   0x00004720 79426173 654f626a 6563745f 54797065 yBaseObject_Type
   0x00004730 005f5a4e 33633130 36646574 61696c31 ._ZN3c106detail1
   0x00004740 34746f72 63684368 65636b46 61696c45 4torchCheckFailE
   0x00004750 504b6353 325f6a53 325f005f 5a4e5374 PKcS2_jS2_._ZNSt
   0x00004760 31337275 6e74696d 655f6572 726f7243 13runtime_errorC
-  0x00004770 3145504b 63005f5a 54495374 31326f75 1EPKc._ZTISt12ou
-  0x00004780 745f6f66 5f72616e 67654047 4c494243 t_of_range@GLIBC
-  0x00004790 58585f33 2e34005f 5a323450 61646469 XX_3.4._Z24Paddi
-  0x000047a0 6e675f38 5f465036 5f546f5f 385f4279 ng_8_FP6_To_8_By
-  0x000047b0 74657350 68535f00 5f5a5374 31377265 tesPhS_._ZSt17re
-  0x000047c0 7468726f 775f6578 63657074 696f6e4e throw_exceptionN
-  0x000047d0 53743135 5f5f6578 63657074 696f6e5f St15__exception_
-  0x000047e0 70747231 33657863 65707469 6f6e5f70 ptr13exception_p
-  0x000047f0 74724540 43585841 42495f31 2e332e33 trE@CXXABI_1.3.3
-  0x00004800 005f5a4e 33633130 34696d70 6c384750 ._ZN3c104impl8GP
-  0x00004810 55547261 63653133 67707554 72616365 UTrace13gpuTrace
-  0x00004820 53746174 6545005f 5a4e5374 31365f53 StateE._ZNSt16_S
-  0x00004830 705f636f 756e7465 645f6261 7365494c p_counted_baseIL
-  0x00004840 4e395f5f 676e755f 63787831 325f4c6f N9__gnu_cxx12_Lo
-  0x00004850 636b5f70 6f6c6963 79453245 4531305f ck_policyE2EE10_
-  0x00004860 4d5f7265 6c656173 65457600 5f5a4e33 M_releaseEv._ZN3
-  0x00004870 63313031 3153796d 4e6f6465 496d706c c1011SymNodeImpl
-  0x00004880 31306775 6172645f 626f6f6c 45504b63 10guard_boolEPKc
-  0x00004890 6c005f5a 4e537431 305f4861 73687461 l._ZNSt10_Hashta
-  0x000048a0 626c6549 50375f6f 626a6563 7453315f bleIP7_objectS1_
-  0x000048b0 53614953 315f454e 5374385f 5f646574 SaIS1_ENSt8__det
-  0x000048c0 61696c39 5f496465 6e746974 79455374 ail9_IdentityESt
-  0x000048d0 38657175 616c5f74 6f495331 5f455374 8equal_toIS1_ESt
-  0x000048e0 34686173 68495331 5f454e53 335f3138 4hashIS1_ENS3_18
-  0x000048f0 5f4d6f64 5f72616e 67655f68 61736869 _Mod_range_hashi
-  0x00004900 6e67454e 53335f32 305f4465 6661756c ngENS3_20_Defaul
-  0x00004910 745f7261 6e676564 5f686173 68454e53 t_ranged_hashENS
-  0x00004920 335f3230 5f507269 6d655f72 65686173 3_20_Prime_rehas
-  0x00004930 685f706f 6c696379 454e5333 5f31375f h_policyENS3_17_
-  0x00004940 48617368 7461626c 655f7472 61697473 Hashtable_traits
-  0x00004950 494c6230 454c6231 454c6231 45454545 ILb0ELb1ELb1EEEE
-  0x00004960 44314576 005f5a54 49537431 326c656e D1Ev._ZTISt12len
-  0x00004970 6774685f 6572726f 7240474c 49424358 gth_error@GLIBCX
-  0x00004980 585f332e 34005f5a 4e4b5373 3466696e X_3.4._ZNKSs4fin
-  0x00004990 6445636d 40474c49 42435858 5f332e34 dEcm@GLIBCXX_3.4
-  0x000049a0 005f5a4e 4b336331 30364956 616c7565 ._ZNK3c106IValue
-  0x000049b0 32337265 706f7274 546f5465 6e736f72 23reportToTensor
-  0x000049c0 54797065 4572726f 72457600 5f656e64 TypeErrorEv._end
-  0x000049d0 005f5a34 375f5f64 65766963 655f7374 ._Z47__device_st
-  0x000049e0 75625f5f 5a313653 706c6974 4b5f5265 ub__Z16SplitK_Re
-  0x000049f0 64756374 696f6e50 365f5f68 616c6650 ductionP6__halfP
-  0x00004a00 666d6d69 50365f5f 68616c66 50666d6d fmmiP6__halfPfmm
-  0x00004a10 69005f5a 4e537339 70757368 5f626163 i._ZNSs9push_bac
-  0x00004a20 6b456340 474c4942 4358585f 332e3400 kEc@GLIBCXX_3.4.
-  0x00004a30 5f5a4e33 63313036 64657461 696c3132 _ZN3c106detail12
-  0x00004a40 5f737472 5f777261 70706572 494a504b _str_wrapperIJPK
-  0x00004a50 63524b53 335f4545 3463616c 6c455335 cRKS3_EE4callES5
-  0x00004a60 5f53355f 005f5a54 56537431 39626173 _S5_._ZTVSt19bas
-  0x00004a70 69635f6f 73747269 6e677374 7265616d ic_ostringstream
-  0x00004a80 49635374 31316368 61725f74 72616974 IcSt11char_trait
-  0x00004a90 73496345 53614963 45454047 4c494243 sIcESaIcEE@GLIBC
-  0x00004aa0 58585f33 2e340050 79457272 5f577269 XX_3.4.PyErr_Wri
-  0x00004ab0 7465556e 72616973 61626c65 00507954 teUnraisable.PyT
-  0x00004ac0 68726561 645f7473 735f6372 65617465 hread_tss_create
-  0x00004ad0 00737472 6c656e40 474c4942 435f322e .strlen@GLIBC_2.
-  0x00004ae0 322e3500 5f5a4e33 63313036 64657461 2.5._ZN3c106deta
-  0x00004af0 696c3132 5f737472 5f777261 70706572 il12_str_wrapper
-  0x00004b00 494a504b 63524b4e 535f3130 5363616c IJPKcRKNS_10Scal
-  0x00004b10 61725479 70654553 335f4545 3463616c arTypeES3_EE4cal
-  0x00004b20 6c45524b 53335f53 365f5339 5f005f5a lERKS3_S6_S9_._Z
-  0x00004b30 4e537431 355f5f65 78636570 74696f6e NSt15__exception
-  0x00004b40 5f707472 31336578 63657074 696f6e5f _ptr13exception_
-  0x00004b50 70747243 3145524b 53305f40 43585841 ptrC1ERKS0_@CXXA
-  0x00004b60 42495f31 2e332e33 005f5a31 33636173 BI_1.3.3._Z13cas
-  0x00004b70 745f6670 31365f66 70365074 5068005f t_fp16_fp6PtPh._
-  0x00004b80 5a54534e 33633130 31344f70 65726174 ZTSN3c1014Operat
-  0x00004b90 6f724b65 726e656c 45005f5a 54564e31 orKernelE._ZTVN1
-  0x00004ba0 305f5f63 78786162 69763131 375f5f63 0__cxxabiv117__c
-  0x00004bb0 6c617373 5f747970 655f696e 666f4540 lass_type_infoE@
-  0x00004bc0 43585841 42495f31 2e330050 794f626a CXXABI_1.3.PyObj
-  0x00004bd0 6563745f 48617341 74747253 7472696e ect_HasAttrStrin
-  0x00004be0 67005f5a 54565374 39626164 5f616c6c g._ZTVSt9bad_all
-  0x00004bf0 6f634047 4c494243 58585f33 2e34005f oc@GLIBCXX_3.4._
-  0x00004c00 5a313751 55414e54 5f47454d 4d5f4b65 Z17QUANT_GEMM_Ke
-  0x00004c10 726e656c 49313254 696c696e 67436f6e rnelI12TilingCon
-  0x00004c20 66696749 4c693445 4c693145 4c693445 figILi4ELi1ELi4E
-  0x00004c30 45664576 504b3575 696e7434 504b365f EfEvPK5uint4PK6_
-  0x00004c40 5f68616c 6653375f 5054305f 6d6d6d69 _halfS7_PT0_mmmi
-  0x00004c50 005f5f63 78615f67 75617264 5f61626f .__cxa_guard_abo
-  0x00004c60 72744043 58584142 495f312e 33005f5a rt@CXXABI_1.3._Z
-  0x00004c70 4e37746f 72636861 6f34335f 474c4f42 N7torchao43_GLOB
-  0x00004c80 414c5f5f 4e5f5f35 62326539 3235395f AL__N__5b2e9259_
-  0x00004c90 365f6e6d 735f6375 5f613163 61643162 6_nms_cu_a1cad1b
-  0x00004ca0 665f3232 30323135 6e6d735f 6b65726e f_220215nms_kern
-  0x00004cb0 656c5f69 6d706c49 64454576 6964504b el_implIdEEvidPK
-  0x00004cc0 545f5079 00637564 61537472 65616d51 T_Py.cudaStreamQ
-  0x00004cd0 75657279 406c6962 63756461 72742e73 uery@libcudart.s
-  0x00004ce0 6f2e3132 005f5f63 75646152 65676973 o.12.__cudaRegis
-  0x00004cf0 74657246 61744269 6e617279 406c6962 terFatBinary@lib
-  0x00004d00 63756461 72742e73 6f2e3132 005f5a4e cudart.so.12._ZN
-  0x00004d10 33633130 31305465 6e736f72 54797065 3c1010TensorType
-  0x00004d20 33676574 4576005f 5a4e4b33 63313034 3getEv._ZNK3c104
-  0x00004d30 696d706c 31365669 72747561 6c477561 impl16VirtualGua
-  0x00004d40 7264496d 706c3562 6c6f636b 45507652 rdImpl5blockEPvR
-  0x00004d50 4b4e535f 36537472 65616d45 005f5a4e KNS_6StreamE._ZN
-  0x00004d60 33633130 3653796d 496e7443 31454e53 3c106SymIntC1ENS
-  0x00004d70 5f313369 6e747275 73697665 5f707472 _13intrusive_ptr
-  0x00004d80 494e535f 31315379 6d4e6f64 65496d70 INS_11SymNodeImp
-  0x00004d90 6c454e53 5f366465 7461696c 3334696e lENS_6detail34in
-  0x00004da0 74727573 6976655f 74617267 65745f64 trusive_target_d
-  0x00004db0 65666175 6c745f6e 756c6c5f 74797065 efault_null_type
-  0x00004dc0 4953325f 45454545 005f5a4e 33633130 IS2_EEEE._ZN3c10
-  0x00004dd0 34637564 61313445 78636861 6e676544 4cuda14ExchangeD
-  0x00004de0 65766963 65456100 5f5a4e33 63313034 eviceEa._ZN3c104
-  0x00004df0 63756461 32307365 74437572 72656e74 cuda20setCurrent
-  0x00004e00 43554441 53747265 616d454e 53305f31 CUDAStreamENS0_1
-  0x00004e10 30435544 41537472 65616d45 005f5a54 0CUDAStreamE._ZT
-  0x00004e20 494e3363 31303230 696e7472 75736976 IN3c1020intrusiv
-  0x00004e30 655f7074 725f7461 72676574 45005f5a e_ptr_targetE._Z
-  0x00004e40 4e4b3363 31303545 72726f72 32327768 NK3c105Error22wh
-  0x00004e50 61745f77 6974686f 75745f62 61636b74 at_without_backt
-  0x00004e60 72616365 4576005f 5a544946 4e326174 raceEv._ZTIFN2at
-  0x00004e70 3654656e 736f7245 524b5330 5f53325f 6TensorERKS0_S2_
-  0x00004e80 6445005f 5a4e5374 31337275 6e74696d dE._ZNSt13runtim
-  0x00004e90 655f6572 726f7244 32457640 474c4942 e_errorD2Ev@GLIB
-  0x00004ea0 4358585f 332e3400 5f5a5374 31316d61 CXX_3.4._ZSt11ma
-  0x00004eb0 6b655f75 6e697175 65494e35 746f7263 ke_uniqueIN5torc
-  0x00004ec0 68386175 746f6772 61643132 4175746f h8autograd12Auto
-  0x00004ed0 67726164 4d657461 454a504e 33633130 gradMetaEJPN3c10
-  0x00004ee0 31305465 6e736f72 496d706c 45526245 10TensorImplERbE
-  0x00004ef0 454e5374 395f4d61 6b65556e 69714954 ENSt9_MakeUniqIT
-  0x00004f00 5f453135 5f5f7369 6e676c65 5f6f626a _E15__single_obj
-  0x00004f10 65637445 44704f54 305f005f 5a54564e ectEDpOT0_._ZTVN
-  0x00004f20 31305f5f 63787861 62697631 32305f5f 10__cxxabiv120__
-  0x00004f30 66756e63 74696f6e 5f747970 655f696e function_type_in
-  0x00004f40 666f4540 43585841 42495f31 2e33005f foE@CXXABI_1.3._
-  0x00004f50 5a4e3363 31303131 53796d4e 6f646549 ZN3c1011SymNodeI
-  0x00004f60 6d706c37 73796d5f 6e6f7445 76005f5a mpl7sym_notEv._Z
-  0x00004f70 4e326174 345f6f70 7339746f 5f646576 N2at4_ops9to_dev
-  0x00004f80 69636534 63616c6c 45524b4e 535f3654 ice4callERKNS_6T
-  0x00004f90 656e736f 72454e33 63313036 44657669 ensorEN3c106Devi
-  0x00004fa0 6365454e 53355f31 30536361 6c617254 ceENS5_10ScalarT
-  0x00004fb0 79706545 62625374 386f7074 696f6e61 ypeEbbSt8optiona
-  0x00004fc0 6c494e53 355f3132 4d656d6f 7279466f lINS5_12MemoryFo
-  0x00004fd0 726d6174 4545005f 5a54534e 33633130 rmatEE._ZTSN3c10
-  0x00004fe0 31355661 72696162 6c655665 7273696f 15VariableVersio
-  0x00004ff0 6e313456 65727369 6f6e436f 756e7465 n14VersionCounte
-  0x00005000 72450050 79427974 65735f41 73537472 rE.PyBytes_AsStr
-  0x00005010 696e6700 5f5a4e53 7431335f 42766563 ing._ZNSt13_Bvec
-  0x00005020 746f725f 62617365 49536149 62454531 tor_baseISaIbEE1
-  0x00005030 335f4d5f 6465616c 6c6f6361 74654576 3_M_deallocateEv
-  0x00005040 005f5a4e 53733132 5f4d5f6c 65616b5f ._ZNSs12_M_leak_
-  0x00005050 68617264 45764047 4c494243 58585f33 hardEv@GLIBCXX_3
-  0x00005060 2e34005f 5a544946 4e326174 3654656e .4._ZTIFN2at6Ten
-  0x00005070 736f7245 53305f53 305f4500 5f5a4e33 sorES0_S0_E._ZN3
-  0x00005080 63313031 3153796d 4e6f6465 496d706c c1011SymNodeImpl
-  0x00005090 3773796d 5f697465 45524b4e 535f3133 7sym_iteERKNS_13
-  0x000050a0 696e7472 75736976 655f7074 72495330 intrusive_ptrIS0
-  0x000050b0 5f4e535f 36646574 61696c33 34696e74 _NS_6detail34int
-  0x000050c0 72757369 76655f74 61726765 745f6465 rusive_target_de
-  0x000050d0 6661756c 745f6e75 6c6c5f74 79706549 fault_null_typeI
-  0x000050e0 53305f45 45454553 375f005f 5a4e3363 S0_EEEES7_._ZN3c
-  0x000050f0 31303664 65746169 6c323374 6f726368 106detail23torch
-  0x00005100 496e7465 726e616c 41737365 72744661 InternalAssertFa
-  0x00005110 696c4550 4b635332 5f6a5332 5f53325f ilEPKcS2_jS2_S2_
-  0x00005120 005f5a4e 33633130 31315379 6d4e6f64 ._ZN3c1011SymNod
-  0x00005130 65496d70 6c386973 5f666c6f 61744576 eImpl8is_floatEv
-  0x00005140 005f5a31 37515541 4e545f47 454d4d5f ._Z17QUANT_GEMM_
-  0x00005150 4b65726e 656c4931 3254696c 696e6743 KernelI12TilingC
-  0x00005160 6f6e6669 67494c69 34454c69 31454c69 onfigILi4ELi1ELi
-  0x00005170 31454536 5f5f6861 6c664576 504b3575 1EE6__halfEvPK5u
-  0x00005180 696e7434 504b5332 5f53375f 5054305f int4PKS2_S7_PT0_
-  0x00005190 6d6d6d69 005f5a4e 536f395f 4d5f696e mmmi._ZNSo9_M_in
-  0x000051a0 73657274 496d4545 52536f54 5f40474c sertImEERSoT_@GL
-  0x000051b0 49424358 585f332e 342e3900 5f5a5374 IBCXX_3.4.9._ZSt
-  0x000051c0 31315f48 6173685f 62797465 73504b76 11_Hash_bytesPKv
-  0x000051d0 6d6d4043 58584142 495f312e 332e3500 mm@CXXABI_1.3.5.
-  0x000051e0 5f5a4e4b 53733572 66696e64 45504b63 _ZNKSs5rfindEPKc
-  0x000051f0 6d6d4047 4c494243 58585f33 2e34005f mm@GLIBCXX_3.4._
-  0x00005200 5a4e4b53 73313766 696e645f 66697273 ZNKSs17find_firs
-  0x00005210 745f6e6f 745f6f66 45504b63 6d6d4047 t_not_ofEPKcmm@G
-  0x00005220 4c494243 58585f33 2e340050 79427974 LIBCXX_3.4.PyByt
-  0x00005230 65417272 61795f53 697a6500 5f5a4e32 eArray_Size._ZN2
-  0x00005240 61743869 6e646578 696e6731 3154656e at8indexing11Ten
-  0x00005250 736f7249 6e646578 44314576 005f5a64 sorIndexD1Ev._Zd
-  0x00005260 6c507640 474c4942 4358585f 332e3400 lPv@GLIBCXX_3.4.
-  0x00005270 5f5a4e4b 33633130 34637564 6134696d _ZNK3c104cuda4im
-  0x00005280 706c3133 43554441 47756172 64496d70 pl13CUDAGuardImp
-  0x00005290 6c323367 65745374 7265616d 46726f6d l23getStreamFrom
-  0x000052a0 476c6f62 616c506f 6f6c454e 535f3644 GlobalPoolENS_6D
-  0x000052b0 65766963 65456200 5f5a4e4b 33633130 eviceEb._ZNK3c10
-  0x000052c0 34696d70 6c313656 69727475 616c4775 4impl16VirtualGu
-  0x000052d0 61726449 6d706c31 32676574 4e657753 ardImpl12getNewS
-  0x000052e0 74726561 6d454e53 5f364465 76696365 treamENS_6Device
-  0x000052f0 4569005f 5a4e5373 43314550 4b636d52 Ei._ZNSsC1EPKcmR
-  0x00005300 4b536149 63454047 4c494243 58585f33 KSaIcE@GLIBCXX_3
-  0x00005310 2e34005f 5a4e3363 31303131 53796d4e .4._ZN3c1011SymN
-  0x00005320 6f646549 6d706c31 326d6179 62655f61 odeImpl12maybe_a
-  0x00005330 735f696e 74457600 5f5a4e33 63313031 s_intEv._ZN3c101
-  0x00005340 344f7065 7261746f 724b6572 6e656c44 4OperatorKernelD
-  0x00005350 30457600 50794361 7073756c 655f4765 0Ev.PyCapsule_Ge
-  0x00005360 74436f6e 74657874 005f5a4e 4b326174 tContext._ZNK2at
-  0x00005370 31305465 6e736f72 42617365 32315f5f 10TensorBase21__
-  0x00005380 64697370 61746368 5f636f6e 74696775 dispatch_contigu
-  0x00005390 6f757345 4e336331 3031324d 656d6f72 ousEN3c1012Memor
-  0x000053a0 79466f72 6d617445 005f5a4e 37746f72 yFormatE._ZN7tor
-  0x000053b0 6368616f 34335f47 4c4f4241 4c5f5f4e chao43_GLOBAL__N
-  0x000053c0 5f5f3562 32653932 35395f36 5f6e6d73 __5b2e9259_6_nms
-  0x000053d0 5f63755f 61316361 64316266 5f323230 _cu_a1cad1bf_220
-  0x000053e0 3231356e 6d735f6b 65726e65 6c5f696d 215nms_kernel_im
-  0x000053f0 706c4966 45457669 64504b54 5f507900 plIfEEvidPKT_Py.
-  0x00005400 5f5a4e33 63313031 3153796d 4e6f6465 _ZN3c1011SymNode
-  0x00005410 496d706c 35626f6f 6c5f4576 005f5a4e Impl5bool_Ev._ZN
-  0x00005420 4b336331 3034696d 706c3136 56697274 K3c104impl16Virt
-  0x00005430 75616c47 75617264 496d706c 31377379 ualGuardImpl17sy
-  0x00005440 6e636872 6f6e697a 65537472 65616d45 nchronizeStreamE
-  0x00005450 524b4e53 5f365374 7265616d 45005f5a RKNS_6StreamE._Z
-  0x00005460 4e326174 345f6f70 73313965 6d707479 N2at4_ops19empty
-  0x00005470 5f6d656d 6f72795f 666f726d 61743463 _memory_format4c
-  0x00005480 616c6c45 4e336331 30384172 72617952 allEN3c108ArrayR
-  0x00005490 6566494e 53325f36 53796d49 6e744545 efINS2_6SymIntEE
-  0x000054a0 45537438 6f707469 6f6e616c 494e5332 ESt8optionalINS2
-  0x000054b0 5f313053 63616c61 72547970 65454553 _10ScalarTypeEES
-  0x000054c0 365f494e 53325f36 4c61796f 75744545 6_INS2_6LayoutEE
-  0x000054d0 53365f49 4e53325f 36446576 69636545 S6_INS2_6DeviceE
-  0x000054e0 4553365f 49624553 365f494e 53325f31 ES6_IbES6_INS2_1
-  0x000054f0 324d656d 6f727946 6f726d61 74454500 2MemoryFormatEE.
-  0x00005500 5f5a4e33 63313031 3153796d 4e6f6465 _ZN3c1011SymNode
-  0x00005510 496d706c 35636c6f 6e654576 005f5a54 Impl5cloneEv._ZT
-  0x00005520 494e3363 31303134 4f706572 61746f72 IN3c1014Operator
-  0x00005530 4b65726e 656c4500 5f5a4e53 73366170 KernelE._ZNSs6ap
-  0x00005540 70656e64 45504b63 6d40474c 49424358 pendEPKcm@GLIBCX
-  0x00005550 585f332e 34005f5a 4e336331 30323069 X_3.4._ZN3c1020i
-  0x00005560 6e747275 73697665 5f707472 5f746172 ntrusive_ptr_tar
-  0x00005570 67657444 30457600 5f5a4e53 73347377 getD0Ev._ZNSs4sw
-  0x00005580 61704552 53734047 4c494243 58585f33 apERSs@GLIBCXX_3
-  0x00005590 2e34005f 5a54564e 33633130 31355661 .4._ZTVN3c1015Va
-  0x000055a0 72696162 6c655665 7273696f 6e313456 riableVersion14V
-  0x000055b0 65727369 6f6e436f 756e7465 7245005f ersionCounterE._
-  0x000055c0 50795479 70655f4c 6f6f6b75 70005079 PyType_Lookup.Py
-  0x000055d0 54687265 61645374 6174655f 436c6561 ThreadState_Clea
-  0x000055e0 72005079 4572725f 436c6561 72005f5a r.PyErr_Clear._Z
-  0x000055f0 4e537436 76656374 6f724962 53614962 NSt6vectorIbSaIb
-  0x00005600 45453134 5f4d5f66 696c6c5f 696e7365 EE14_M_fill_inse
-  0x00005610 72744553 7431335f 4269745f 69746572 rtESt13_Bit_iter
-  0x00005620 61746f72 6d62005f 5f637861 5f746872 atormb.__cxa_thr
-  0x00005630 6f774043 58584142 495f312e 33006375 ow@CXXABI_1.3.cu
-  0x00005640 64615374 7265616d 53796e63 68726f6e daStreamSynchron
-  0x00005650 697a6540 6c696263 75646172 742e736f ize@libcudart.so
-  0x00005660 2e313200 5f5a5453 464e3261 74365465 .12._ZTSFN2at6Te
-  0x00005670 6e736f72 45524b53 305f5332 5f644500 nsorERKS0_S2_dE.
-  0x00005680 50794361 7073756c 655f4e65 77005079 PyCapsule_New.Py
-  0x00005690 4d656d5f 43616c6c 6f63005f 5a4e3363 Mem_Calloc._ZN3c
-  0x000056a0 31303469 6d706c36 64657461 696c3331 104impl6detail31
-  0x000056b0 57726170 46756e63 74696f6e 496e746f WrapFunctionInto
-  0x000056c0 52756e74 696d6546 756e6374 6f725f49 RuntimeFunctor_I
-  0x000056d0 50464e32 61743654 656e736f 72455334 PFN2at6TensorES4
-  0x000056e0 5f53345f 4553345f 4e535f34 67757473 _S4_ES4_NS_4guts
-  0x000056f0 38747970 656c6973 74387479 70656c69 8typelist8typeli
-  0x00005700 7374494a 53345f53 345f4545 45454431 stIJS4_S4_EEEED1
-  0x00005710 4576005f 5a4e3363 31303664 65746169 Ev._ZN3c106detai
-  0x00005720 6c31325f 7374725f 77726170 70657249 l12_str_wrapperI
-  0x00005730 4a504b63 524b6c45 45346361 6c6c4552 JPKcRKlEE4callER
-  0x00005740 4b53335f 53355f00 5f5a4e32 6174345f KS3_S5_._ZN2at4_
-  0x00005750 6f707331 31736f72 745f7374 61626c65 ops11sort_stable
-  0x00005760 3463616c 6c45524b 4e535f36 54656e73 4callERKNS_6Tens
-  0x00005770 6f724553 74386f70 74696f6e 616c4962 orESt8optionalIb
-  0x00005780 456c6200 5f5a5374 32305f5f 7468726f Elb._ZSt20__thro
-  0x00005790 775f6c65 6e677468 5f657272 6f72504b w_length_errorPK
-  0x000057a0 6340474c 49424358 585f332e 34005f5a c@GLIBCXX_3.4._Z
-  0x000057b0 4e35746f 72636837 4c696272 61727943 N5torch7LibraryC
-  0x000057c0 31454e53 305f344b 696e6445 53735374 1ENS0_4KindESsSt
-  0x000057d0 386f7074 696f6e61 6c494e33 63313031 8optionalIN3c101
-  0x000057e0 31446973 70617463 684b6579 4545504b 1DispatchKeyEEPK
-  0x000057f0 636a005f 556e7769 6e645f52 6573756d cj._Unwind_Resum
-  0x00005800 65404743 435f332e 30005f5a 4e4b3363 e@GCC_3.0._ZNK3c
-  0x00005810 31303463 75646134 696d706c 31334355 104cuda4impl13CU
-  0x00005820 44414775 61726449 6d706c31 31717565 DAGuardImpl11que
-  0x00005830 72795374 7265616d 45524b4e 535f3653 ryStreamERKNS_6S
-  0x00005840 74726561 6d450050 79427974 65735f53 treamE.PyBytes_S
-  0x00005850 697a6500 5f5a5453 4e336331 3034696d ize._ZTSN3c104im
-  0x00005860 706c3664 65746169 6c333157 72617046 pl6detail31WrapF
-  0x00005870 756e6374 696f6e49 6e746f52 756e7469 unctionIntoRunti
-  0x00005880 6d654675 6e63746f 725f4950 464e3261 meFunctor_IPFN2a
-  0x00005890 74365465 6e736f72 4553345f 53345f45 t6TensorES4_S4_E
-  0x000058a0 53345f4e 535f3467 75747338 74797065 S4_NS_4guts8type
-  0x000058b0 6c697374 38747970 656c6973 74494a53 list8typelistIJS
-  0x000058c0 345f5334 5f454545 4545005f 5a4e3363 4_S4_EEEEE._ZN3c
-  0x000058d0 31303131 53796d4e 6f646549 6d706c31 1011SymNodeImpl1
-  0x000058e0 366e6573 7465645f 696e745f 636f6566 6nested_int_coef
-  0x000058f0 66457600 5f5a4e4b 33633130 34637564 fEv._ZNK3c104cud
-  0x00005900 6134696d 706c3133 43554441 47756172 a4impl13CUDAGuar
-  0x00005910 64496d70 6c313673 796e6368 726f6e69 dImpl16synchroni
-  0x00005920 7a654576 656e7445 5076005f 5a4e3363 zeEventEPv._ZN3c
-  0x00005930 31303463 75646131 32646576 6963655f 104cuda12device_
-  0x00005940 636f756e 74457600 5f5a4e4b 33633130 countEv._ZNK3c10
-  0x00005950 34637564 6134696d 706c3133 43554441 4cuda4impl13CUDA
-  0x00005960 47756172 64496d70 6c396765 74446576 GuardImpl9getDev
-  0x00005970 69636545 76005f5a 32304269 74496e74 iceEv._Z20BitInt
-  0x00005980 65726c65 6176696e 675f3262 69745068 erleaving_2bitPh
-  0x00005990 005f5a4e 37746f72 6368616f 32357765 ._ZN7torchao25we
-  0x000059a0 69676874 5f6d6174 7269785f 64657175 ight_matrix_dequ
-  0x000059b0 616e745f 63707545 4e326174 3654656e ant_cpuEN2at6Ten
-  0x000059c0 736f7245 53315f00 76736e70 72696e74 sorES1_.vsnprint
-  0x000059d0 6640474c 4942435f 322e322e 35005f5a f@GLIBC_2.2.5._Z
-  0x000059e0 4e336331 3034696d 706c3238 77726170 N3c104impl28wrap
-  0x000059f0 5f6b6572 6e656c5f 66756e63 746f725f _kernel_functor_
-  0x00005a00 756e626f 7865645f 494e5330 5f366465 unboxed_INS0_6de
-  0x00005a10 7461696c 33315772 61704675 6e637469 tail31WrapFuncti
-  0x00005a20 6f6e496e 746f5275 6e74696d 6546756e onIntoRuntimeFun
-  0x00005a30 63746f72 5f495046 4e326174 3654656e ctor_IPFN2at6Ten
-  0x00005a40 736f7245 53355f45 53355f4e 535f3467 sorES5_ES5_NS_4g
-  0x00005a50 75747338 74797065 6c697374 38747970 uts8typelist8typ
-  0x00005a60 656c6973 74494a53 355f4545 45454553 elistIJS5_EEEEES
-  0x00005a70 365f4534 63616c6c 45504e53 5f31344f 6_E4callEPNS_14O
-  0x00005a80 70657261 746f724b 65726e65 6c454e53 peratorKernelENS
-  0x00005a90 5f313444 69737061 7463684b 65795365 _14DispatchKeySe
-  0x00005aa0 74455335 5f005f5a 4e336331 30313556 tES5_._ZN3c1015V
-  0x00005ab0 61726961 626c6556 65727369 6f6e3134 ariableVersion14
-  0x00005ac0 56657273 696f6e43 6f756e74 65724430 VersionCounterD0
-  0x00005ad0 4576005f 5a4e3363 31303131 53796d4e Ev._ZN3c1011SymN
-  0x00005ae0 6f646549 6d706c37 73796d5f 6d617845 odeImpl7sym_maxE
-  0x00005af0 524b4e53 5f313369 6e747275 73697665 RKNS_13intrusive
-  0x00005b00 5f707472 4953305f 4e535f36 64657461 _ptrIS0_NS_6deta
-  0x00005b10 696c3334 696e7472 75736976 655f7461 il34intrusive_ta
-  0x00005b20 72676574 5f646566 61756c74 5f6e756c rget_default_nul
-  0x00005b30 6c5f7479 70654953 305f4545 4545005f l_typeIS0_EEEE._
-  0x00005b40 5a544946 4e326174 3654656e 736f7245 ZTIFN2at6TensorE
-  0x00005b50 53305f53 305f5330 5f6c4500 50794578 S0_S0_S0_lE.PyEx
-  0x00005b60 635f5479 70654572 726f7200 5f5a4e33 c_TypeError._ZN3
-  0x00005b70 63313031 3153796d 4e6f6465 496d706c c1011SymNodeImpl
-  0x00005b80 35666c6f 6f724576 005f5a54 494e3363 5floorEv._ZTIN3c
-  0x00005b90 31303463 75646134 696d706c 31334355 104cuda4impl13CU
-  0x00005ba0 44414775 61726449 6d706c45 005f5a4e DAGuardImplE._ZN
-  0x00005bb0 4b336331 3034696d 706c3136 56697274 K3c104impl16Virt
-  0x00005bc0 75616c47 75617264 496d706c 3138756e ualGuardImpl18un
-  0x00005bd0 63686563 6b656453 65744465 76696365 checkedSetDevice
-  0x00005be0 454e535f 36446576 69636545 005f5a4e ENS_6DeviceE._ZN
-  0x00005bf0 4b336331 30346375 64613469 6d706c31 K3c104cuda4impl1
-  0x00005c00 33435544 41477561 7264496d 706c3973 3CUDAGuardImpl9s
-  0x00005c10 65744465 76696365 454e535f 36446576 etDeviceENS_6Dev
-  0x00005c20 69636545 005f5a54 564e3363 31303131 iceE._ZTVN3c1011
-  0x00005c30 53796d4e 6f646549 6d706c45 005f5a54 SymNodeImplE._ZT
-  0x00005c40 494e3363 31303130 56616c75 65457272 IN3c1010ValueErr
-  0x00005c50 6f724500 5f5a5456 4e336331 3034696d orE._ZTVN3c104im
-  0x00005c60 706c3664 65746169 6c333157 72617046 pl6detail31WrapF
-  0x00005c70 756e6374 696f6e49 6e746f52 756e7469 unctionIntoRunti
-  0x00005c80 6d654675 6e63746f 725f4950 464e3261 meFunctor_IPFN2a
-  0x00005c90 74365465 6e736f72 4553345f 4553345f t6TensorES4_ES4_
-  0x00005ca0 4e535f34 67757473 38747970 656c6973 NS_4guts8typelis
-  0x00005cb0 74387479 70656c69 7374494a 53345f45 t8typelistIJS4_E
-  0x00005cc0 45454545 00507954 7970655f 52656164 EEEE.PyType_Read
-  0x00005cd0 79005f5a 54495374 31396261 645f6f70 y._ZTISt19bad_op
-  0x00005ce0 74696f6e 616c5f61 63636573 73005f5a tional_access._Z
-  0x00005cf0 54534e33 63313034 696d706c 36646574 TSN3c104impl6det
-  0x00005d00 61696c33 31577261 7046756e 6374696f ail31WrapFunctio
-  0x00005d10 6e496e74 6f52756e 74696d65 46756e63 nIntoRuntimeFunc
-  0x00005d20 746f725f 4950464e 32617436 54656e73 tor_IPFN2at6Tens
-  0x00005d30 6f724553 345f4553 345f4e53 5f346775 orES4_ES4_NS_4gu
-  0x00005d40 74733874 7970656c 69737438 74797065 ts8typelist8type
-  0x00005d50 6c697374 494a5334 5f454545 4545005f listIJS4_EEEEE._
-  0x00005d60 5a4e3363 31303131 53796d4e 6f646549 ZN3c1011SymNodeI
-  0x00005d70 6d706c32 67654552 4b4e535f 3133696e mpl2geERKNS_13in
-  0x00005d80 74727573 6976655f 70747249 53305f4e trusive_ptrIS0_N
-  0x00005d90 535f3664 65746169 6c333469 6e747275 S_6detail34intru
-  0x00005da0 73697665 5f746172 6765745f 64656661 sive_target_defa
-  0x00005db0 756c745f 6e756c6c 5f747970 65495330 ult_null_typeIS0
-  0x00005dc0 5f454545 45005f5a 4e336331 30354572 _EEEE._ZN3c105Er
-  0x00005dd0 726f7243 32454e53 5f313453 6f757263 rorC2ENS_14Sourc
-  0x00005de0 654c6f63 6174696f 6e455373 005f5a54 eLocationESs._ZT
-  0x00005df0 494e3363 31303131 53796d4e 6f646549 IN3c1011SymNodeI
-  0x00005e00 6d706c45 005f5a53 7432345f 5f746872 mplE._ZSt24__thr
-  0x00005e10 6f775f6f 75745f6f 665f7261 6e67655f ow_out_of_range_
-  0x00005e20 666d7450 4b637a00 5f5a3137 5155414e fmtPKcz._Z17QUAN
-  0x00005e30 545f4745 4d4d5f4b 65726e65 6c493132 T_GEMM_KernelI12
-  0x00005e40 54696c69 6e67436f 6e666967 494c6934 TilingConfigILi4
-  0x00005e50 454c6931 454c6931 45456645 76504b35 ELi1ELi1EEfEvPK5
-  0x00005e60 75696e74 34504b36 5f5f6861 6c665337 uint4PK6__halfS7
-  0x00005e70 5f505430 5f6d6d6d 69005f5a 4e336331 _PT0_mmmi._ZN3c1
-  0x00005e80 3034696d 706c3664 65746169 6c333157 04impl6detail31W
-  0x00005e90 72617046 756e6374 696f6e49 6e746f52 rapFunctionIntoR
-  0x00005ea0 756e7469 6d654675 6e63746f 725f4950 untimeFunctor_IP
-  0x00005eb0 464e3261 74365465 6e736f72 4553345f FN2at6TensorES4_
-  0x00005ec0 53345f53 345f6c45 53345f4e 535f3467 S4_S4_lES4_NS_4g
-  0x00005ed0 75747338 74797065 6c697374 38747970 uts8typelist8typ
-  0x00005ee0 656c6973 74494a53 345f5334 5f53345f elistIJS4_S4_S4_
-  0x00005ef0 6c454545 45443045 76005f5a 4e336331 lEEEED0Ev._ZN3c1
-  0x00005f00 30313153 796d4e6f 6465496d 706c3133 011SymNodeImpl13
-  0x00005f10 69735f63 6f6e7469 67756f75 73454e53 is_contiguousENS
-  0x00005f20 5f384172 72617952 6566494e 535f3133 _8ArrayRefINS_13
-  0x00005f30 696e7472 75736976 655f7074 72495330 intrusive_ptrIS0
-  0x00005f40 5f4e535f 36646574 61696c33 34696e74 _NS_6detail34int
-  0x00005f50 72757369 76655f74 61726765 745f6465 rusive_target_de
-  0x00005f60 6661756c 745f6e75 6c6c5f74 79706549 fault_null_typeI
-  0x00005f70 53305f45 45454545 4553375f 005f5a4e S0_EEEEEES7_._ZN
-  0x00005f80 33633130 31315379 6d4e6f64 65496d70 3c1011SymNodeImp
-  0x00005f90 6c443045 76005f5a 4e537336 61737369 lD0Ev._ZNSs6assi
-  0x00005fa0 676e4552 4b537340 474c4942 4358585f gnERKSs@GLIBCXX_
-  0x00005fb0 332e3400 5f5a4e53 73366173 7369676e 3.4._ZNSs6assign
-  0x00005fc0 45504b63 6d40474c 49424358 585f332e EPKcm@GLIBCXX_3.
-  0x00005fd0 34005f5a 4e336331 30313153 796d4e6f 4._ZN3c1011SymNo
-  0x00005fe0 6465496d 706c3673 796d5f6f 7245524b deImpl6sym_orERK
-  0x00005ff0 4e535f31 33696e74 72757369 76655f70 NS_13intrusive_p
-  0x00006000 74724953 305f4e53 5f366465 7461696c trIS0_NS_6detail
-  0x00006010 3334696e 74727573 6976655f 74617267 34intrusive_targ
-  0x00006020 65745f64 65666175 6c745f6e 756c6c5f et_default_null_
-  0x00006030 74797065 4953305f 45454545 005f5a4e typeIS0_EEEE._ZN
-  0x00006040 33633130 31315379 6d4e6f64 65496d70 3c1011SymNodeImp
-  0x00006050 6c33706f 7745524b 4e535f31 33696e74 l3powERKNS_13int
-  0x00006060 72757369 76655f70 74724953 305f4e53 rusive_ptrIS0_NS
-  0x00006070 5f366465 7461696c 3334696e 74727573 _6detail34intrus
-  0x00006080 6976655f 74617267 65745f64 65666175 ive_target_defau
-  0x00006090 6c745f6e 756c6c5f 74797065 4953305f lt_null_typeIS0_
-  0x000060a0 45454545 005f5a4e 33633130 36646574 EEEE._ZN3c106det
-  0x000060b0 61696c32 33746f72 6368496e 7465726e ail23torchIntern
-  0x000060c0 616c4173 73657274 4661696c 45504b63 alAssertFailEPKc
-  0x000060d0 53325f6a 53325f52 4b537300 5079496e S2_jS2_RKSs.PyIn
-  0x000060e0 69745f5f 43005f5a 4e537336 61707065 it__C._ZNSs6appe
-  0x000060f0 6e644552 4b537340 474c4942 4358585f ndERKSs@GLIBCXX_
-  0x00006100 332e3400 5f5a5453 464e3261 74365465 3.4._ZTSFN2at6Te
-  0x00006110 6e736f72 4553305f 53305f45 00507954 nsorES0_S0_E.PyT
-  0x00006120 75706c65 5f476574 4974656d 005f5a4e uple_GetItem._ZN
-  0x00006130 53743135 5f5f6578 63657074 696f6e5f St15__exception_
-  0x00006140 7074726e 6545524b 4e535f31 33657863 ptrneERKNS_13exc
-  0x00006150 65707469 6f6e5f70 74724553 325f4043 eption_ptrES2_@C
-  0x00006160 58584142 495f312e 332e3300 5f5a4e37 XXABI_1.3.3._ZN7
-  0x00006170 746f7263 68616f32 38776569 6768745f torchao28weight_
-  0x00006180 6d617472 69785f70 72657061 636b696e matrix_prepackin
-  0x00006190 675f6370 75454e32 61743654 656e736f g_cpuEN2at6Tenso
-  0x000061a0 7245005f 50794f62 6a656374 5f476574 rE._PyObject_Get
-  0x000061b0 44696374 50747200 5f5a4e4b 32617436 DictPtr._ZNK2at6
-  0x000061c0 54656e73 6f723569 6e646578 45537431 Tensor5indexESt1
-  0x000061d0 36696e69 7469616c 697a6572 5f6c6973 6initializer_lis
-  0x000061e0 74494e53 5f38696e 64657869 6e673131 tINS_8indexing11
-  0x000061f0 54656e73 6f72496e 64657845 45005f5f TensorIndexEE.__
-  0x00006200 6378615f 61746578 69744047 4c494243 cxa_atexit@GLIBC
-  0x00006210 5f322e32 2e35005f 5a54564e 33633130 _2.2.5._ZTVN3c10
-  0x00006220 31344f70 65726174 6f724b65 726e656c 14OperatorKernel
-  0x00006230 45005f5a 4e4b3261 74313054 656e736f E._ZNK2at10Tenso
-  0x00006240 72426173 65386461 74615f70 7472496c rBase8data_ptrIl
-  0x00006250 45455054 5f760050 79547570 6c655f53 EEPT_v.PyTuple_S
-  0x00006260 65744974 656d005f 5a313751 55414e54 etItem._Z17QUANT
-  0x00006270 5f47454d 4d5f4b65 726e656c 49313254 _GEMM_KernelI12T
-  0x00006280 696c696e 67436f6e 66696749 4c693445 ilingConfigILi4E
-  0x00006290 4c693145 4c693845 45664576 504b3575 Li1ELi8EEfEvPK5u
-  0x000062a0 696e7434 504b365f 5f68616c 6653375f int4PK6__halfS7_
-  0x000062b0 5054305f 6d6d6d69 00507954 68726561 PT0_mmmi.PyThrea
-  0x000062c0 645f7473 735f6765 74005079 4572725f d_tss_get.PyErr_
-  0x000062d0 52657374 6f726500 5f5a3239 77656967 Restore._Z29weig
-  0x000062e0 68745f70 72657061 636b696e 675f6670 ht_prepacking_fp
-  0x000062f0 31365f74 6f5f6670 36507450 686d6d00 16_to_fp6PtPhmm.
-  0x00006300 5f5a4e35 746f7263 6835656d 70747945 _ZN5torch5emptyE
-  0x00006310 4e336331 30384172 72617952 6566496c N3c108ArrayRefIl
-  0x00006320 45454e53 305f3133 54656e73 6f724f70 EENS0_13TensorOp
-  0x00006330 74696f6e 73455374 386f7074 696f6e61 tionsESt8optiona
-  0x00006340 6c494e53 305f3132 4d656d6f 7279466f lINS0_12MemoryFo
-  0x00006350 726d6174 4545005f 5a4e3574 6f726368 rmatEE._ZN5torch
-  0x00006360 374c6962 72617279 44314576 005f5a4e 7LibraryD1Ev._ZN
-  0x00006370 33633130 34637564 6134696d 706c3133 3c104cuda4impl13
-  0x00006380 43554441 47756172 64496d70 6c443145 CUDAGuardImplD1E
-  0x00006390 76005f5f 6378615f 70757265 5f766972 v.__cxa_pure_vir
-  0x000063a0 7475616c 40435858 4142495f 312e3300 tual@CXXABI_1.3.
-  0x000063b0 5f5f7074 68726561 645f6b65 795f6372 __pthread_key_cr
-  0x000063c0 65617465 40474c49 42435f32 2e322e35 eate@GLIBC_2.2.5
-  0x000063d0 005f5a4e 53743135 5f5f6578 63657074 ._ZNSt15__except
-  0x000063e0 696f6e5f 70747231 33657863 65707469 ion_ptr13excepti
-  0x000063f0 6f6e5f70 74723473 77617045 5253305f on_ptr4swapERS0_
-  0x00006400 40435858 4142495f 312e332e 33005f5a @CXXABI_1.3.3._Z
-  0x00006410 4e336331 30313153 796d4e6f 6465496d N3c1011SymNodeIm
-  0x00006420 706c3130 77726170 5f666c6f 61744564 pl10wrap_floatEd
-  0x00006430 005f5a4e 4b336331 30346375 64613469 ._ZNK3c104cuda4i
-  0x00006440 6d706c31 33435544 41477561 7264496d mpl13CUDAGuardIm
-  0x00006450 706c3672 65636f72 64455050 76524b4e pl6recordEPPvRKN
-  0x00006460 535f3653 74726561 6d45614e 535f3945 S_6StreamEaNS_9E
-  0x00006470 76656e74 466c6167 45005f5a 4e523574 ventFlagE._ZNR5t
-  0x00006480 6f726368 374c6962 72617279 355f696d orch7Library5_im
-  0x00006490 706c4550 4b634f4e 535f3131 43707046 plEPKcONS_11CppF
-  0x000064a0 756e6374 696f6e45 4e535f31 375f5265 unctionENS_17_Re
-  0x000064b0 67697374 65724f72 56657269 66794500 gisterOrVerifyE.
-  0x000064c0 5f5a5374 706c4963 53743131 63686172 _ZStplIcSt11char
-  0x000064d0 5f747261 69747349 63455361 49634545 _traitsIcESaIcEE
-  0x000064e0 53624954 5f54305f 54315f45 504b5333 SbIT_T0_T1_EPKS3
-  0x000064f0 5f524b53 365f005f 5a4e5373 43314552 _RKS6_._ZNSsC1ER
-  0x00006500 4b536149 63454047 4c494243 58585f33 KSaIcE@GLIBCXX_3
-  0x00006510 2e34005f 5a4e3363 31303463 75646139 .4._ZN3c104cuda9
-  0x00006520 47657444 65766963 65455061 005f5a4e GetDeviceEPa._ZN
-  0x00006530 33633130 31346765 74547970 65507472 3c1014getTypePtr
-  0x00006540 436f7079 494e3261 74365465 6e736f72 CopyIN2at6Tensor
-  0x00006550 4545454e 535f3454 79706532 3453696e EEENS_4Type24Sin
-  0x00006560 676c6574 6f6e4f72 53686172 65645479 gletonOrSharedTy
-  0x00006570 70655074 72495333 5f454576 005f5a4e pePtrIS3_EEv._ZN
-  0x00006580 5373345f 52657031 305f4d5f 64657374 Ss4_Rep10_M_dest
-  0x00006590 726f7945 524b5361 49634540 474c4942 royERKSaIcE@GLIB
-  0x000065a0 4358585f 332e3400 5f5a4e53 7431355f CXX_3.4._ZNSt15_
-  0x000065b0 5f657863 65707469 6f6e5f70 74723133 _exception_ptr13
-  0x000065c0 65786365 7074696f 6e5f7074 72443145 exception_ptrD1E
-  0x000065d0 76404358 58414249 5f312e33 2e33005f v@CXXABI_1.3.3._
-  0x000065e0 5a4e3261 74345f6f 70733132 696e6465 ZN2at4_ops12inde
-  0x000065f0 785f7365 6c656374 3463616c 6c45524b x_select4callERK
-  0x00006600 4e535f36 54656e73 6f72456c 53345f00 NS_6TensorElS4_.
-  0x00006610 50795468 72656164 5f747373 5f616c6c PyThread_tss_all
-  0x00006620 6f63005f 5a544953 7431366e 65737465 oc._ZTISt16neste
-  0x00006630 645f6578 63657074 696f6e40 43585841 d_exception@CXXA
-  0x00006640 42495f31 2e332e35 005f5a4e 33633130 BI_1.3.5._ZN3c10
-  0x00006650 31315379 6d4e6f64 65496d70 6c326c65 11SymNodeImpl2le
-  0x00006660 45524b4e 535f3133 696e7472 75736976 ERKNS_13intrusiv
-  0x00006670 655f7074 72495330 5f4e535f 36646574 e_ptrIS0_NS_6det
-  0x00006680 61696c33 34696e74 72757369 76655f74 ail34intrusive_t
-  0x00006690 61726765 745f6465 6661756c 745f6e75 arget_default_nu
-  0x000066a0 6c6c5f74 79706549 53305f45 45454500 ll_typeIS0_EEEE.
-  0x000066b0 5f5a4e4b 33633130 34696d70 6c313656 _ZNK3c104impl16V
-  0x000066c0 69727475 616c4775 61726449 6d706c31 irtualGuardImpl1
-  0x000066d0 34657863 68616e67 65446576 69636545 4exchangeDeviceE
-  0x000066e0 4e535f36 44657669 63654500 5f5a4e4b NS_6DeviceE._ZNK
-  0x000066f0 33633130 34696d70 6c313656 69727475 3c104impl16Virtu
-  0x00006700 616c4775 61726449 6d706c31 36676574 alGuardImpl16get
-  0x00006710 44656661 756c7453 74726561 6d454e53 DefaultStreamENS
-  0x00006720 5f364465 76696365 45005f5a 4e366361 _6DeviceE._ZN6ca
-  0x00006730 66666532 38547970 654d6574 61323665 ffe28TypeMeta26e
-  0x00006740 72726f72 5f756e73 7570706f 72746564 rror_unsupported
-  0x00006750 5f747970 656d6574 61455330 5f005f5a _typemetaES0_._Z
-  0x00006760 4e336331 30313153 796d4e6f 6465496d N3c1011SymNodeIm
-  0x00006770 706c3769 735f626f 6f6c4576 005f5a54 pl7is_boolEv._ZT
-  0x00006780 49537431 3372756e 74696d65 5f657272 ISt13runtime_err
-  0x00006790 6f724047 4c494243 58585f33 2e34005f or@GLIBCXX_3.4._
-  0x000067a0 5a4e3363 31303134 4f706572 61746f72 ZN3c1014Operator
-  0x000067b0 4b65726e 656c4431 45760063 75646147 KernelD1Ev.cudaG
-  0x000067c0 65744572 726f7253 7472696e 67406c69 etErrorString@li
-  0x000067d0 62637564 6172742e 736f2e31 32005f5a bcudart.so.12._Z
-  0x000067e0 4e537431 3372756e 74696d65 5f657272 NSt13runtime_err
-  0x000067f0 6f724331 45524b53 7340474c 49424358 orC1ERKSs@GLIBCX
-  0x00006800 585f332e 34005f5a 4e326174 345f6f70 X_3.4._ZN2at4_op
-  0x00006810 73366e61 72726f77 3463616c 6c45524b s6narrow4callERK
-  0x00006820 4e535f36 54656e73 6f72456c 4e336331 NS_6TensorElN3c1
-  0x00006830 30365379 6d496e74 4553365f 005f5a4e 06SymIntES6_._ZN
-  0x00006840 33633130 31315379 6d4e6f64 65496d70 3c1011SymNodeImp
-  0x00006850 6c326e65 45524b4e 535f3133 696e7472 l2neERKNS_13intr
-  0x00006860 75736976 655f7074 72495330 5f4e535f usive_ptrIS0_NS_
-  0x00006870 36646574 61696c33 34696e74 72757369 6detail34intrusi
-  0x00006880 76655f74 61726765 745f6465 6661756c ve_target_defaul
-  0x00006890 745f6e75 6c6c5f74 79706549 53305f45 t_null_typeIS0_E
-  0x000068a0 45454500 5f5a4e35 746f7263 68386175 EEE._ZN5torch8au
-  0x000068b0 746f6772 61643133 6d616b65 5f766172 tograd13make_var
-  0x000068c0 6961626c 65454e32 61743654 656e736f iableEN2at6Tenso
-  0x000068d0 72456262 005f5a4e 53743135 62617369 rEbb._ZNSt15basi
-  0x000068e0 635f7374 72696e67 62756649 63537431 c_stringbufIcSt1
-  0x000068f0 31636861 725f7472 61697473 49634553 1char_traitsIcES
-  0x00006900 61496345 45443045 76005f5a 4e336331 aIcEED0Ev._ZN3c1
-  0x00006910 30313556 61726961 626c6556 65727369 015VariableVersi
-  0x00006920 6f6e3134 56657273 696f6e43 6f756e74 on14VersionCount
-  0x00006930 65724431 4576005f 5a4e3363 31303130 erD1Ev._ZN3c1010
-  0x00006940 56616c75 65457272 6f724431 4576005f ValueErrorD1Ev._
-  0x00006950 5a4e3363 31303131 53796d4e 6f646549 ZN3c1011SymNodeI
-  0x00006960 6d706c31 31677561 72645f66 6c6f6174 mpl11guard_float
-  0x00006970 45504b63 6c005f5a 5374706c 49635374 EPKcl._ZStplIcSt
-  0x00006980 31316368 61725f74 72616974 73496345 11char_traitsIcE
-  0x00006990 53614963 45455362 49545f54 305f5431 SaIcEESbIT_T0_T1
-  0x000069a0 5f454f53 365f5337 5f005f5a 54534e33 _EOS6_S7_._ZTSN3
-  0x000069b0 63313031 3153796d 4e6f6465 496d706c c1011SymNodeImpl
-  0x000069c0 45005f5a 53743136 5f5f6f73 74726561 E._ZSt16__ostrea
-  0x000069d0 6d5f696e 73657274 49635374 31316368 m_insertIcSt11ch
-  0x000069e0 61725f74 72616974 73496345 45525374 ar_traitsIcEERSt
-  0x000069f0 31336261 7369635f 6f737472 65616d49 13basic_ostreamI
-  0x00006a00 545f5430 5f455336 5f504b53 335f6c40 T_T0_ES6_PKS3_l@
-  0x00006a10 474c4942 4358585f 332e342e 39005f49 GLIBCXX_3.4.9._I
-  0x00006a20 544d5f72 65676973 74657254 4d436c6f TM_registerTMClo
-  0x00006a30 6e655461 626c6500 50794346 756e6374 neTable.PyCFunct
-  0x00006a40 696f6e5f 54797065 005f5a4e 33633130 ion_Type._ZN3c10
-  0x00006a50 34696d70 6c366465 7461696c 33315772 4impl6detail31Wr
-  0x00006a60 61704675 6e637469 6f6e496e 746f5275 apFunctionIntoRu
-  0x00006a70 6e74696d 6546756e 63746f72 5f495046 ntimeFunctor_IPF
-  0x00006a80 4e326174 3654656e 736f7245 53345f53 N2at6TensorES4_S
-  0x00006a90 345f5334 5f6c4553 345f4e53 5f346775 4_S4_lES4_NS_4gu
-  0x00006aa0 74733874 7970656c 69737438 74797065 ts8typelist8type
-  0x00006ab0 6c697374 494a5334 5f53345f 53345f6c listIJS4_S4_S4_l
-  0x00006ac0 45454545 44324576 005f5a4e 53734331 EEEED2Ev._ZNSsC1
-  0x00006ad0 45524b53 736d6d40 474c4942 4358585f ERKSsmm@GLIBCXX_
-  0x00006ae0 332e3400 50794749 4c537461 74655f47 3.4.PyGILState_G
-  0x00006af0 65745468 69735468 72656164 53746174 etThisThreadStat
-  0x00006b00 65005079 42797465 735f4173 53747269 e.PyBytes_AsStri
-  0x00006b10 6e67416e 6453697a 65006d65 6d636d70 ngAndSize.memcmp
-  0x00006b20 40474c49 42435f32 2e322e35 005f5a4e @GLIBC_2.2.5._ZN
-  0x00006b30 33633130 3133696e 74727573 6976655f 3c1013intrusive_
-  0x00006b40 70747249 4e535f31 35566172 6961626c ptrINS_15Variabl
-  0x00006b50 65566572 73696f6e 31345665 7273696f eVersion14Versio
-  0x00006b60 6e436f75 6e746572 454e535f 36646574 nCounterENS_6det
-  0x00006b70 61696c33 34696e74 72757369 76655f74 ail34intrusive_t
-  0x00006b80 61726765 745f6465 6661756c 745f6e75 arget_default_nu
-  0x00006b90 6c6c5f74 79706549 53325f45 45453672 ll_typeIS2_EEE6r
-  0x00006ba0 65736574 5f457600 5079556e 69636f64 eset_Ev.PyUnicod
-  0x00006bb0 655f4173 456e636f 64656453 7472696e e_AsEncodedStrin
-  0x00006bc0 67005f5a 4e4b5373 37636f6d 70617265 g._ZNKSs7compare
-  0x00006bd0 45504b63 40474c49 42435858 5f332e34 EPKc@GLIBCXX_3.4
-  0x00006be0 005f5a4e 4b326174 31305465 6e736f72 ._ZNK2at10Tensor
-  0x00006bf0 42617365 38646174 615f7074 72494e33 Base8data_ptrIN3
-  0x00006c00 63313034 48616c66 45454550 545f7600 c104HalfEEEPT_v.
-  0x00006c10 5f5a4e33 63313031 3153796d 4e6f6465 _ZN3c1011SymNode
-  0x00006c20 496d706c 44324576 005f5a4e 33633130 ImplD2Ev._ZN3c10
-  0x00006c30 31315379 6d4e6f64 65496d70 6c386861 11SymNodeImpl8ha
-  0x00006c40 735f6869 6e744576 00507954 75706c65 s_hintEv.PyTuple
-  0x00006c50 5f4e6577 005f5a31 37515541 4e545f47 _New._Z17QUANT_G
-  0x00006c60 454d4d5f 4b65726e 656c4931 3254696c EMM_KernelI12Til
-  0x00006c70 696e6743 6f6e6669 67494c69 34454c69 ingConfigILi4ELi
-  0x00006c80 31454c69 32454536 5f5f6861 6c664576 1ELi2EE6__halfEv
-  0x00006c90 504b3575 696e7434 504b5332 5f53375f PK5uint4PKS2_S7_
-  0x00006ca0 5054305f 6d6d6d69 005f5a4e 35746f72 PT0_mmmi._ZN5tor
-  0x00006cb0 63683664 65746169 6c313654 6f726368 ch6detail16Torch
-  0x00006cc0 4c696272 61727949 6e697444 31457600 LibraryInitD1Ev.
-  0x00006cd0 50794f62 6a656374 5f43616c 6c46756e PyObject_CallFun
-  0x00006ce0 6374696f 6e4f626a 41726773 005f5a4e ctionObjArgs._ZN
-  0x00006cf0 33633130 34696d70 6c323345 78636c75 3c104impl23Exclu
-  0x00006d00 64654469 73706174 63684b65 79477561 deDispatchKeyGua
-  0x00006d10 72644331 454e535f 31344469 73706174 rdC1ENS_14Dispat
-  0x00006d20 63684b65 79536574 45005f5a 4e4b3261 chKeySetE._ZNK2a
-  0x00006d30 74313054 656e736f 72426173 65386461 t10TensorBase8da
-  0x00006d40 74615f70 74724968 45455054 5f76005f ta_ptrIhEEPT_v._
-  0x00006d50 5a4e4b53 74313962 61645f6f 7074696f ZNKSt19bad_optio
-  0x00006d60 6e616c5f 61636365 73733477 68617445 nal_access4whatE
-  0x00006d70 76005f5a 54495374 31365f53 705f636f v._ZTISt16_Sp_co
-  0x00006d80 756e7465 645f6261 7365494c 4e395f5f unted_baseILN9__
-  0x00006d90 676e755f 63787831 325f4c6f 636b5f70 gnu_cxx12_Lock_p
-  0x00006da0 6f6c6963 79453245 45006375 64614576 olicyE2EE.cudaEv
-  0x00006db0 656e7453 796e6368 726f6e69 7a65406c entSynchronize@l
-  0x00006dc0 69626375 64617274 2e736f2e 3132005f ibcudart.so.12._
-  0x00006dd0 5a4e3363 31303463 75646132 30676574 ZN3c104cuda20get
-  0x00006de0 44656661 756c7443 55444153 74726561 DefaultCUDAStrea
-  0x00006df0 6d456100 5f5a3234 77656967 68745f6d mEa._Z24weight_m
-  0x00006e00 61747269 785f7072 65706163 6b696e67 atrix_prepacking
-  0x00006e10 5069535f 6d6d005f 5a4e4b33 63313031 PiS_mm._ZNK3c101
-  0x00006e20 3054656e 736f7249 6d706c36 64657669 0TensorImpl6devi
-  0x00006e30 63654576 005f5a4e 53743676 6563746f ceEv._ZNSt6vecto
-  0x00006e40 72496253 61496245 4531335f 4d5f696e rIbSaIbEE13_M_in
-  0x00006e50 73657274 5f617578 45537431 335f4269 sert_auxESt13_Bi
-  0x00006e60 745f6974 65726174 6f726200 5f5a4e33 t_iteratorb._ZN3
-  0x00006e70 6331306c 73455253 6f4e535f 31304465 c10lsERSoNS_10De
-  0x00006e80 76696365 54797065 45005f5a 54545374 viceTypeE._ZTTSt
-  0x00006e90 31396261 7369635f 6f737472 696e6773 19basic_ostrings
-  0x00006ea0 74726561 6d496353 74313163 6861725f treamIcSt11char_
-  0x00006eb0 74726169 74734963 45536149 63454540 traitsIcESaIcEE@
-  0x00006ec0 474c4942 4358585f 332e3400 5f5a4e4b GLIBCXX_3.4._ZNK
-  0x00006ed0 33633130 34637564 6134696d 706c3133 3c104cuda4impl13
-  0x00006ee0 43554441 47756172 64496d70 6c313465 CUDAGuardImpl14e
-  0x00006ef0 78636861 6e676544 65766963 65454e53 xchangeDeviceENS
-  0x00006f00 5f364465 76696365 45005f5a 4e336331 _6DeviceE._ZN3c1
-  0x00006f10 30323069 6e747275 73697665 5f707472 020intrusive_ptr
-  0x00006f20 5f746172 67657431 3772656c 65617365 _target17release
-  0x00006f30 5f726573 6f757263 65734576 005f5a4e _resourcesEv._ZN
-  0x00006f40 53743130 5f486173 68746162 6c654953 St10_HashtableIS
-  0x00006f50 73537434 70616972 494b5373 50764553 sSt4pairIKSsPvES
-  0x00006f60 61495333 5f454e53 74385f5f 64657461 aIS3_ENSt8__deta
-  0x00006f70 696c3130 5f53656c 65637431 73744553 il10_Select1stES
-  0x00006f80 74386571 75616c5f 746f4953 73455374 t8equal_toISsESt
-  0x00006f90 34686173 68495373 454e5335 5f31385f 4hashISsENS5_18_
-  0x00006fa0 4d6f645f 72616e67 655f6861 7368696e Mod_range_hashin
-  0x00006fb0 67454e53 355f3230 5f446566 61756c74 gENS5_20_Default
-  0x00006fc0 5f72616e 6765645f 68617368 454e5335 _ranged_hashENS5
-  0x00006fd0 5f32305f 5072696d 655f7265 68617368 _20_Prime_rehash
-  0x00006fe0 5f706f6c 69637945 4e53355f 31375f48 _policyENS5_17_H
-  0x00006ff0 61736874 61626c65 5f747261 69747349 ashtable_traitsI
-  0x00007000 4c623145 4c623045 4c623145 45454539 Lb1ELb0ELb1EEEE9
-  0x00007010 5f4d5f72 65686173 68456d52 4b6d0050 _M_rehashEmRKm.P
-  0x00007020 79457863 5f496d70 6f727445 72726f72 yExc_ImportError
-  0x00007030 005f5a4e 33633130 31315379 6d4e6f64 ._ZN3c1011SymNod
-  0x00007040 65496d70 6c326c74 45524b4e 535f3133 eImpl2ltERKNS_13
-  0x00007050 696e7472 75736976 655f7074 72495330 intrusive_ptrIS0
-  0x00007060 5f4e535f 36646574 61696c33 34696e74 _NS_6detail34int
-  0x00007070 72757369 76655f74 61726765 745f6465 rusive_target_de
-  0x00007080 6661756c 745f6e75 6c6c5f74 79706549 fault_null_typeI
-  0x00007090 53305f45 45454500 5f5a4e4b 33633130 S0_EEEE._ZNK3c10
-  0x000070a0 31315379 6d4e6f64 65496d70 6c313369 11SymNodeImpl13i
-  0x000070b0 735f6e65 73746564 5f696e74 4576005f s_nested_intEv._
-  0x000070c0 5a4e5374 31396261 7369635f 6f737472 ZNSt19basic_ostr
-  0x000070d0 696e6773 74726561 6d496353 74313163 ingstreamIcSt11c
-  0x000070e0 6861725f 74726169 74734963 45536149 har_traitsIcESaI
-  0x000070f0 63454543 31457600 5f5a5449 4e336331 cEEC1Ev._ZTIN3c1
-  0x00007100 3034696d 706c3664 65746169 6c333157 04impl6detail31W
-  0x00007110 72617046 756e6374 696f6e49 6e746f52 rapFunctionIntoR
-  0x00007120 756e7469 6d654675 6e63746f 725f4950 untimeFunctor_IP
-  0x00007130 464e3261 74365465 6e736f72 4553345f FN2at6TensorES4_
-  0x00007140 4553345f 4e535f34 67757473 38747970 ES4_NS_4guts8typ
-  0x00007150 656c6973 74387479 70656c69 7374494a elist8typelistIJ
-  0x00007160 53345f45 45454545 00507945 72725f4f S4_EEEEE.PyErr_O
-  0x00007170 63637572 72656400 50795468 72656164 ccurred.PyThread
-  0x00007180 53746174 655f4465 6c657465 43757272 State_DeleteCurr
-  0x00007190 656e7400 5f5a4e33 63313031 33696e74 ent._ZN3c1013int
-  0x000071a0 72757369 76655f70 7472494e 535f3131 rusive_ptrINS_11
-  0x000071b0 53796d4e 6f646549 6d706c45 4e535f36 SymNodeImplENS_6
-  0x000071c0 64657461 696c3334 696e7472 75736976 detail34intrusiv
-  0x000071d0 655f7461 72676574 5f646566 61756c74 e_target_default
-  0x000071e0 5f6e756c 6c5f7479 70654953 315f4545 _null_typeIS1_EE
-  0x000071f0 45367265 7365745f 4576005f 5a4e4b32 E6reset_Ev._ZNK2
-  0x00007200 61743130 54656e73 6f724261 73653864 at10TensorBase8d
-  0x00007210 6174615f 70747249 69454550 545f7600 ata_ptrIiEEPT_v.
-  0x00007220 5f5a3137 5155414e 545f4745 4d4d5f4b _Z17QUANT_GEMM_K
-  0x00007230 65726e65 6c493132 54696c69 6e67436f ernelI12TilingCo
-  0x00007240 6e666967 494c6934 454c6931 454c6934 nfigILi4ELi1ELi4
-  0x00007250 4545365f 5f68616c 66457650 4b357569 EE6__halfEvPK5ui
-  0x00007260 6e743450 4b53325f 53375f50 54305f6d nt4PKS2_S7_PT0_m
-  0x00007270 6d6d6900 5f5a5449 464e3261 74365465 mmi._ZTIFN2at6Te
-  0x00007280 6e736f72 4553305f 45006375 64614576 nsorES0_E.cudaEv
-  0x00007290 656e7452 65636f72 64406c69 62637564 entRecord@libcud
-  0x000072a0 6172742e 736f2e31 32005f5a 4e336331 art.so.12._ZN3c1
-  0x000072b0 3034696d 706c3664 65746169 6c333157 04impl6detail31W
-  0x000072c0 72617046 756e6374 696f6e49 6e746f52 rapFunctionIntoR
-  0x000072d0 756e7469 6d654675 6e63746f 725f4950 untimeFunctor_IP
-  0x000072e0 464e3261 74365465 6e736f72 4553345f FN2at6TensorES4_
-  0x000072f0 53345f45 53345f4e 535f3467 75747338 S4_ES4_NS_4guts8
-  0x00007300 74797065 6c697374 38747970 656c6973 typelist8typelis
-  0x00007310 74494a53 345f5334 5f454545 45443045 tIJS4_S4_EEEED0E
-  0x00007320 76005079 5765616b 7265665f 4e657752 v.PyWeakref_NewR
-  0x00007330 6566005f 5a4e5374 385f5f64 65746169 ef._ZNSt8__detai
-  0x00007340 6c395f4d 61705f62 61736549 53735374 l9_Map_baseISsSt
-  0x00007350 34706169 72494b53 73507645 53614953 4pairIKSsPvESaIS
-  0x00007360 345f454e 535f3130 5f53656c 65637431 4_ENS_10_Select1
-  0x00007370 73744553 74386571 75616c5f 746f4953 stESt8equal_toIS
-  0x00007380 73455374 34686173 68495373 454e535f sESt4hashISsENS_
-  0x00007390 31385f4d 6f645f72 616e6765 5f686173 18_Mod_range_has
-  0x000073a0 68696e67 454e535f 32305f44 65666175 hingENS_20_Defau
-  0x000073b0 6c745f72 616e6765 645f6861 7368454e lt_ranged_hashEN
-  0x000073c0 535f3230 5f507269 6d655f72 65686173 S_20_Prime_rehas
-  0x000073d0 685f706f 6c696379 454e535f 31375f48 h_policyENS_17_H
-  0x000073e0 61736874 61626c65 5f747261 69747349 ashtable_traitsI
-  0x000073f0 4c623145 4c623045 4c623145 45454c62 Lb1ELb0ELb1EEELb
-  0x00007400 31454569 78454f53 73005f5a 4e4b3363 1EEixEOSs._ZNK3c
-  0x00007410 31303545 72726f72 34776861 74457600 105Error4whatEv.
-  0x00007420 5f5a4e53 73433145 504b6352 4b536149 _ZNSsC1EPKcRKSaI
-  0x00007430 63454047 4c494243 58585f33 2e34005f cE@GLIBCXX_3.4._
-  0x00007440 5a4e4b33 63313034 63756461 34696d70 ZNK3c104cuda4imp
-  0x00007450 6c313343 55444147 75617264 496d706c l13CUDAGuardImpl
-  0x00007460 31346578 6368616e 67655374 7265616d 14exchangeStream
-  0x00007470 454e535f 36537472 65616d45 005f5a4e ENS_6StreamE._ZN
-  0x00007480 53733772 65736572 7665456d 40474c49 Ss7reserveEm@GLI
-  0x00007490 42435858 5f332e34 00637564 6146756e BCXX_3.4.cudaFun
-  0x000074a0 63536574 41747472 69627574 65406c69 cSetAttribute@li
-  0x000074b0 62637564 6172742e 736f2e31 32005f5a bcudart.so.12._Z
-  0x000074c0 4e336331 3034696d 706c3664 65746169 N3c104impl6detai
-  0x000074d0 6c333157 72617046 756e6374 696f6e49 l31WrapFunctionI
-  0x000074e0 6e746f52 756e7469 6d654675 6e63746f ntoRuntimeFuncto
-  0x000074f0 725f4950 464e3261 74365465 6e736f72 r_IPFN2at6Tensor
-  0x00007500 4553345f 4553345f 4e535f34 67757473 ES4_ES4_NS_4guts
-  0x00007510 38747970 656c6973 74387479 70656c69 8typelist8typeli
-  0x00007520 7374494a 53345f45 45454544 30457600 stIJS4_EEEED0Ev.
-  0x00007530 5079556e 69636f64 655f4173 55544638 PyUnicode_AsUTF8
-  0x00007540 53747269 6e670050 79457661 6c5f4765 String.PyEval_Ge
-  0x00007550 74427569 6c74696e 73005f5a 4e4b3363 tBuiltins._ZNK3c
-  0x00007560 31303463 75646134 696d706c 31334355 104cuda4impl13CU
-  0x00007570 44414775 61726449 6d706c31 32646573 DAGuardImpl12des
-  0x00007580 74726f79 4576656e 74455076 61005f5a troyEventEPva._Z
-  0x00007590 54495374 31346f76 6572666c 6f775f65 TISt14overflow_e
-  0x000075a0 72726f72 40474c49 42435858 5f332e34 rror@GLIBCXX_3.4
-  0x000075b0 00507945 78635f56 616c7565 4572726f .PyExc_ValueErro
-  0x000075c0 72005f5a 4e537337 7265706c 61636545 r._ZNSs7replaceE
-  0x000075d0 6d6d504b 636d4047 4c494243 58585f33 mmPKcm@GLIBCXX_3
-  0x000075e0 2e34005f 5a4e5374 31337275 6e74696d .4._ZNSt13runtim
-  0x000075f0 655f6572 726f7243 3245524b 53734047 e_errorC2ERKSs@G
-  0x00007600 4c494243 58585f33 2e34005f 5a4e3574 LIBCXX_3.4._ZN5t
-  0x00007610 6f726368 336a6974 31317061 72736553 orch3jit11parseS
-  0x00007620 6368656d 6145524b 5373005f 5a4e3363 chemaERKSs._ZN3c
-  0x00007630 31303477 61726e45 524b4e53 5f375761 104warnERKNS_7Wa
-  0x00007640 726e696e 6745005f 5a4e5373 43314552 rningE._ZNSsC1ER
-  0x00007650 4b537340 474c4942 4358585f 332e3400 KSs@GLIBCXX_3.4.
-  0x00007660 6d656d63 70794047 4c494243 5f322e31 memcpy@GLIBC_2.1
-  0x00007670 34006375 64614576 656e7443 72656174 4.cudaEventCreat
-  0x00007680 65576974 68466c61 6773406c 69626375 eWithFlags@libcu
-  0x00007690 64617274 2e736f2e 3132005f 5a54494e dart.so.12._ZTIN
-  0x000076a0 31305f5f 63787861 62697631 31355f5f 10__cxxabiv115__
-  0x000076b0 666f7263 65645f75 6e77696e 64454043 forced_unwindE@C
-  0x000076c0 58584142 495f312e 332e3200 5f5a4e53 XXABI_1.3.2._ZNS
-  0x000076d0 74396261 645f616c 6c6f6344 31457640 t9bad_allocD1Ev@
-  0x000076e0 474c4942 4358585f 332e3400 5f5a4e33 GLIBCXX_3.4._ZN3
-  0x000076f0 63313034 696d706c 36646574 61696c33 c104impl6detail3
-  0x00007700 31577261 7046756e 6374696f 6e496e74 1WrapFunctionInt
-  0x00007710 6f52756e 74696d65 46756e63 746f725f oRuntimeFunctor_
-  0x00007720 4950464e 32617436 54656e73 6f724552 IPFN2at6TensorER
-  0x00007730 4b53345f 53365f64 4553345f 4e535f34 KS4_S6_dES4_NS_4
-  0x00007740 67757473 38747970 656c6973 74387479 guts8typelist8ty
-  0x00007750 70656c69 7374494a 53365f53 365f6445 pelistIJS6_S6_dE
-  0x00007760 45454544 31457600 5f5a4e53 73366170 EEED1Ev._ZNSs6ap
-  0x00007770 70656e64 456d6340 474c4942 4358585f pendEmc@GLIBCXX_
-  0x00007780 332e3400 50794361 7073756c 655f4765 3.4.PyCapsule_Ge
-  0x00007790 744e616d 65005f5a 31375155 414e545f tName._Z17QUANT_
-  0x000077a0 47454d4d 5f4b6572 6e656c49 31325469 GEMM_KernelI12Ti
-  0x000077b0 6c696e67 436f6e66 6967494c 6934454c lingConfigILi4EL
-  0x000077c0 6931454c 69324545 66457650 4b357569 i1ELi2EEfEvPK5ui
-  0x000077d0 6e743450 4b365f5f 68616c66 53375f50 nt4PK6__halfS7_P
-  0x000077e0 54305f6d 6d6d6900 5f5a4e53 73366170 T0_mmmi._ZNSs6ap
-  0x000077f0 70656e64 45524b53 736d6d40 474c4942 pendERKSsmm@GLIB
-  0x00007800 4358585f 332e3400 5f5a5374 31375f5f CXX_3.4._ZSt17__
-  0x00007810 7468726f 775f6261 645f616c 6c6f6376 throw_bad_allocv
-  0x00007820 40474c49 42435858 5f332e34 005f5a6e @GLIBCXX_3.4._Zn
-  0x00007830 776d4047 4c494243 58585f33 2e340050 wm@GLIBCXX_3.4.P
-  0x00007840 79457863 5f4f7665 72666c6f 77457272 yExc_OverflowErr
-  0x00007850 6f72005f 5a4e4b33 63313034 696d706c or._ZNK3c104impl
-  0x00007860 31365669 72747561 6c477561 7264496d 16VirtualGuardIm
-  0x00007870 706c3131 656c6170 73656454 696d6545 pl11elapsedTimeE
-  0x00007880 50765332 5f61005f 5a4e3363 31303469 PvS2_a._ZN3c104i
-  0x00007890 6d706c31 36566972 7475616c 47756172 mpl16VirtualGuar
-  0x000078a0 64496d70 6c443045 76005f5a 4e336331 dImplD0Ev._ZN3c1
-  0x000078b0 30313153 796d4e6f 6465496d 706c3469 011SymNodeImpl4i
-  0x000078c0 6e745f45 76005f49 544d5f64 65726567 nt_Ev._ITM_dereg
-  0x000078d0 69737465 72544d43 6c6f6e65 5461626c isterTMCloneTabl
-  0x000078e0 65005f5a 4e336331 30313446 756e6374 e._ZN3c1014Funct
-  0x000078f0 696f6e53 6368656d 61443245 76005f5a ionSchemaD2Ev._Z
-  0x00007900 5374706c 49635374 31316368 61725f74 StplIcSt11char_t
-  0x00007910 72616974 73496345 53614963 45455362 raitsIcESaIcEESb
-  0x00007920 49545f54 305f5431 5f454f53 365f504b IT_T0_T1_EOS6_PK
-  0x00007930 53335f00 66726565 40474c49 42435f32 S3_.free@GLIBC_2
-  0x00007940 2e322e35 005f5a4e 4b336331 30346375 .2.5._ZNK3c104cu
-  0x00007950 64613469 6d706c31 33435544 41477561 da4impl13CUDAGua
-  0x00007960 7264496d 706c3967 65745374 7265616d rdImpl9getStream
-  0x00007970 454e535f 36446576 69636545 005f5a4e ENS_6DeviceE._ZN
-  0x00007980 33633130 31305661 6c756545 72726f72 3c1010ValueError
-  0x00007990 44324576 005f5a4e 53743139 62617369 D2Ev._ZNSt19basi
-  0x000079a0 635f6f73 7472696e 67737472 65616d49 c_ostringstreamI
-  0x000079b0 63537431 31636861 725f7472 61697473 cSt11char_traits
-  0x000079c0 49634553 61496345 45443145 7640474c IcESaIcEED1Ev@GL
-  0x000079d0 49424358 585f332e 34005f5a 54565374 IBCXX_3.4._ZTVSt
-  0x000079e0 31356261 7369635f 73747269 6e676275 15basic_stringbu
-  0x000079f0 66496353 74313163 6861725f 74726169 fIcSt11char_trai
-  0x00007a00 74734963 45536149 63454540 474c4942 tsIcESaIcEE@GLIB
-  0x00007a10 4358585f 332e3400 5f5f6378 615f6669 CXX_3.4.__cxa_fi
-  0x00007a20 6e616c69 7a654047 4c494243 5f322e32 nalize@GLIBC_2.2
-  0x00007a30 2e35005f 5a54534e 33633130 34696d70 .5._ZTSN3c104imp
-  0x00007a40 6c366465 7461696c 33315772 61704675 l6detail31WrapFu
-  0x00007a50 6e637469 6f6e496e 746f5275 6e74696d nctionIntoRuntim
-  0x00007a60 6546756e 63746f72 5f495046 4e326174 eFunctor_IPFN2at
-  0x00007a70 3654656e 736f7245 524b5334 5f53365f 6TensorERKS4_S6_
-  0x00007a80 64455334 5f4e535f 34677574 73387479 dES4_NS_4guts8ty
-  0x00007a90 70656c69 73743874 7970656c 69737449 pelist8typelistI
-  0x00007aa0 4a53365f 53365f64 45454545 45005f5a JS6_S6_dEEEEE._Z
-  0x00007ab0 4e4b3363 31303469 6d706c31 36566972 NK3c104impl16Vir
-  0x00007ac0 7475616c 47756172 64496d70 6c313071 tualGuardImpl10q
-  0x00007ad0 75657279 4576656e 74455076 00507944 ueryEventEPv.PyD
-  0x00007ae0 6963745f 54797065 005f5a54 53537431 ict_Type._ZTSSt1
-  0x00007af0 39626164 5f6f7074 696f6e61 6c5f6163 9bad_optional_ac
-  0x00007b00 63657373 005f5a54 49537431 32646f6d cess._ZTISt12dom
-  0x00007b10 61696e5f 6572726f 7240474c 49424358 ain_error@GLIBCX
-  0x00007b20 585f332e 34005f5a 4e336331 30366465 X_3.4._ZN3c106de
-  0x00007b30 7461696c 31325f73 74725f77 72617070 tail12_str_wrapp
-  0x00007b40 6572494a 504b6352 4b694545 3463616c erIJPKcRKiEE4cal
-  0x00007b50 6c45524b 53335f53 355f005f 5a4e3363 lERKS3_S5_._ZN3c
-  0x00007b60 31303664 65746169 6c31325f 7374725f 106detail12_str_
-  0x00007b70 77726170 70657249 4a504b63 524b6a45 wrapperIJPKcRKjE
-  0x00007b80 45346361 6c6c4552 4b53335f 53355f00 E4callERKS3_S5_.
-  0x00007b90 5f5a4e33 63313031 34446973 70617463 _ZN3c1014Dispatc
-  0x00007ba0 684b6579 53657443 32454e53 5f313144 hKeySetC2ENS_11D
-  0x00007bb0 69737061 7463684b 65794500 5f5a4e33 ispatchKeyE._ZN3
-  0x00007bc0 63313034 696d706c 36646574 61696c33 c104impl6detail3
-  0x00007bd0 31577261 7046756e 6374696f 6e496e74 1WrapFunctionInt
-  0x00007be0 6f52756e 74696d65 46756e63 746f725f oRuntimeFunctor_
-  0x00007bf0 4950464e 32617436 54656e73 6f724552 IPFN2at6TensorER
-  0x00007c00 4b53345f 53365f64 4553345f 4e535f34 KS4_S6_dES4_NS_4
-  0x00007c10 67757473 38747970 656c6973 74387479 guts8typelist8ty
-  0x00007c20 70656c69 7374494a 53365f53 365f6445 pelistIJS6_S6_dE
-  0x00007c30 45454544 32457600 5079434d 6574686f EEED2Ev.PyCMetho
-  0x00007c40 645f4e65 77006375 64614765 744c6173 d_New.cudaGetLas
-  0x00007c50 74457272 6f72406c 69626375 64617274 tError@libcudart
-  0x00007c60 2e736f2e 3132005f 5a54564e 33633130 .so.12._ZTVN3c10
-  0x00007c70 34696d70 6c366465 7461696c 33315772 4impl6detail31Wr
-  0x00007c80 61704675 6e637469 6f6e496e 746f5275 apFunctionIntoRu
-  0x00007c90 6e74696d 6546756e 63746f72 5f495046 ntimeFunctor_IPF
-  0x00007ca0 4e326174 3654656e 736f7245 53345f53 N2at6TensorES4_S
-  0x00007cb0 345f5334 5f6c4553 345f4e53 5f346775 4_S4_lES4_NS_4gu
-  0x00007cc0 74733874 7970656c 69737438 74797065 ts8typelist8type
-  0x00007cd0 6c697374 494a5334 5f53345f 53345f6c listIJS4_S4_S4_l
-  0x00007ce0 45454545 45005f5a 4e4b3363 31303137 EEEEE._ZNK3c1017
-  0x00007cf0 53796d62 6f6c6963 53686170 654d6574 SymbolicShapeMet
-  0x00007d00 61313869 6e69745f 69735f63 6f6e7469 a18init_is_conti
-  0x00007d10 67756f75 73457600 5f5a4e33 63313031 guousEv._ZN3c101
-  0x00007d20 3153796d 4e6f6465 496d706c 32306775 1SymNodeImpl20gu
-  0x00007d30 6172645f 73697a65 5f6f626c 6976696f ard_size_oblivio
-  0x00007d40 75734550 4b636c00 5f5a4e4b 53743133 usEPKcl._ZNKSt13
-  0x00007d50 72756e74 696d655f 6572726f 72347768 runtime_error4wh
-  0x00007d60 61744576 40474c49 42435858 5f332e34 atEv@GLIBCXX_3.4
-  0x00007d70 005f5f62 73735f73 74617274 005f5a31 .__bss_start._Z1
-  0x00007d80 3653706c 69744b5f 52656475 6374696f 6SplitK_Reductio
-  0x00007d90 6e50365f 5f68616c 6650666d 6d690050 nP6__halfPfmmi.P
-  0x00007da0 79457863 65707469 6f6e5f53 6574436f yException_SetCo
-  0x00007db0 6e746578 74005f5a 4e4b3363 31303469 ntext._ZNK3c104i
-  0x00007dc0 6d706c31 36566972 7475616c 47756172 mpl16VirtualGuar
-  0x00007dd0 64496d70 6c313673 796e6368 726f6e69 dImpl16synchroni
-  0x00007de0 7a654576 656e7445 5076005f 5a4e5374 zeEventEPv._ZNSt
-  0x00007df0 36766563 746f7249 4e336331 30384172 6vectorIN3c108Ar
-  0x00007e00 67756d65 6e744553 61495331 5f454544 gumentESaIS1_EED
-  0x00007e10 32457600 5f5a4e33 63313031 3153796d 2Ev._ZN3c1011Sym
-  0x00007e20 4e6f6465 496d706c 37747275 65646976 NodeImpl7truediv
-  0x00007e30 45524b4e 535f3133 696e7472 75736976 ERKNS_13intrusiv
-  0x00007e40 655f7074 72495330 5f4e535f 36646574 e_ptrIS0_NS_6det
-  0x00007e50 61696c33 34696e74 72757369 76655f74 ail34intrusive_t
-  0x00007e60 61726765 745f6465 6661756c 745f6e75 arget_default_nu
-  0x00007e70 6c6c5f74 79706549 53305f45 45454500 ll_typeIS0_EEEE.
-  0x00007e80 5f5a5449 4e336331 3034696d 706c3664 _ZTIN3c104impl6d
-  0x00007e90 65746169 6c333157 72617046 756e6374 etail31WrapFunct
-  0x00007ea0 696f6e49 6e746f52 756e7469 6d654675 ionIntoRuntimeFu
-  0x00007eb0 6e63746f 725f4950 464e3261 74365465 nctor_IPFN2at6Te
-  0x00007ec0 6e736f72 4553345f 53345f53 345f6c45 nsorES4_S4_S4_lE
-  0x00007ed0 53345f4e 535f3467 75747338 74797065 S4_NS_4guts8type
-  0x00007ee0 6c697374 38747970 656c6973 74494a53 list8typelistIJS
-  0x00007ef0 345f5334 5f53345f 6c454545 45450050 4_S4_S4_lEEEEE.P
-  0x00007f00 7947494c 53746174 655f456e 73757265 yGILState_Ensure
-  0x00007f10 00507945 76616c5f 41637175 69726554 .PyEval_AcquireT
-  0x00007f20 68726561 64005079 4572725f 53657453 hread.PyErr_SetS
-  0x00007f30 7472696e 67005079 4f626a65 63745f43 tring.PyObject_C
-  0x00007f40 616c6c4f 626a6563 74005079 54687265 allObject.PyThre
-  0x00007f50 61645f74 73735f73 6574005f 5f637861 ad_tss_set.__cxa
-  0x00007f60 5f64656d 616e676c 65404358 58414249 _demangle@CXXABI
-  0x00007f70 5f312e33 005f5a4e 33633130 34637564 _1.3._ZN3c104cud
-  0x00007f80 6134696d 706c3133 43554441 47756172 a4impl13CUDAGuar
-  0x00007f90 64496d70 6c443045 76005f5a 4e35746f dImplD0Ev._ZN5to
-  0x00007fa0 72636831 31437070 46756e63 74696f6e rch11CppFunction
-  0x00007fb0 44314576 005f5a4e 32617434 5f6f7073 D1Ev._ZN2at4_ops
-  0x00007fc0 3135746f 5f647479 70655f6c 61796f75 15to_dtype_layou
-  0x00007fd0 74346361 6c6c4552 4b4e535f 3654656e t4callERKNS_6Ten
-  0x00007fe0 736f7245 5374386f 7074696f 6e616c49 sorESt8optionalI
-  0x00007ff0 4e336331 30313053 63616c61 72547970 N3c1010ScalarTyp
-  0x00008000 65454553 355f494e 53365f36 4c61796f eEES5_INS6_6Layo
-  0x00008010 75744545 53355f49 4e53365f 36446576 utEES5_INS6_6Dev
-  0x00008020 69636545 4553355f 49624562 6253355f iceEES5_IbEbbS5_
-  0x00008030 494e5336 5f31324d 656d6f72 79466f72 INS6_12MemoryFor
-  0x00008040 6d617445 45005f5a 4e536f6c 73456940 matEE._ZNSolsEi@
-  0x00008050 474c4942 4358585f 332e3400 5f5a4e52 GLIBCXX_3.4._ZNR
-  0x00008060 35746f72 6368374c 69627261 7279345f 5torch7Library4_
-  0x00008070 64656645 4f4e3363 31303134 46756e63 defEON3c1014Func
-  0x00008080 74696f6e 53636865 6d614550 4e53315f tionSchemaEPNS1_
-  0x00008090 31324f70 65726174 6f724e61 6d654552 12OperatorNameER
-  0x000080a0 4b537436 76656374 6f72494e 32617433 KSt6vectorIN2at3
-  0x000080b0 54616745 53614953 385f4545 4e535f31 TagESaIS8_EENS_1
-  0x000080c0 375f5265 67697374 65724f72 56657269 7_RegisterOrVeri
-  0x000080d0 66794500 63756461 53747265 616d5761 fyE.cudaStreamWa
-  0x000080e0 69744576 656e7440 6c696263 75646172 itEvent@libcudar
-  0x000080f0 742e736f 2e313200 5f5a4e33 63313034 t.so.12._ZN3c104
-  0x00008100 63756461 32304355 44414361 6368696e cuda20CUDACachin
-  0x00008110 67416c6c 6f636174 6f723961 6c6c6f63 gAllocator9alloc
-  0x00008120 61746f72 45005f5f 6378615f 67756172 atorE.__cxa_guar
-  0x00008130 645f6163 71756972 65404358 58414249 d_acquire@CXXABI
-  0x00008140 5f312e33 005f5a54 564e3363 31303469 _1.3._ZTVN3c104i
-  0x00008150 6d706c36 64657461 696c3331 57726170 mpl6detail31Wrap
-  0x00008160 46756e63 74696f6e 496e746f 52756e74 FunctionIntoRunt
-  0x00008170 696d6546 756e6374 6f725f49 50464e32 imeFunctor_IPFN2
-  0x00008180 61743654 656e736f 7245524b 53345f53 at6TensorERKS4_S
-  0x00008190 365f6445 53345f4e 535f3467 75747338 6_dES4_NS_4guts8
-  0x000081a0 74797065 6c697374 38747970 656c6973 typelist8typelis
-  0x000081b0 74494a53 365f5336 5f644545 45454500 tIJS6_S6_dEEEEE.
-  0x000081c0 5f5a4e33 63313034 63756461 31376765 _ZN3c104cuda17ge
-  0x000081d0 74537472 65616d46 726f6d50 6f6f6c45 tStreamFromPoolE
-  0x000081e0 6961005f 5a4e5374 3136696e 76616c69 ia._ZNSt16invali
-  0x000081f0 645f6172 67756d65 6e744331 45504b63 d_argumentC1EPKc
-  0x00008200 0050794f 626a6563 745f4973 496e7374 .PyObject_IsInst
-  0x00008210 616e6365 005f5a4e 4b336331 30346375 ance._ZNK3c104cu
-  0x00008220 64613469 6d706c31 33435544 41477561 da4impl13CUDAGua
-  0x00008230 7264496d 706c3474 79706545 76005f5a rdImpl4typeEv._Z
-  0x00008240 4e537431 36696e76 616c6964 5f617267 NSt16invalid_arg
-  0x00008250 756d656e 74443145 7640474c 49424358 umentD1Ev@GLIBCX
-  0x00008260 585f332e 34005f5a 54495374 3136696e X_3.4._ZTISt16in
-  0x00008270 76616c69 645f6172 67756d65 6e744047 valid_argument@G
-  0x00008280 4c494243 58585f33 2e34005f 5f676d6f LIBCXX_3.4.__gmo
-  0x00008290 6e5f7374 6172745f 5f005f5a 4e336331 n_start__._ZN3c1
-  0x000082a0 30323141 75746f67 7261644d 65746149 021AutogradMetaI
-  0x000082b0 6e746572 66616365 44324576 0050794d nterfaceD2Ev.PyM
-  0x000082c0 656d5f46 72656500 50795468 72656164 em_Free.PyThread
-  0x000082d0 53746174 655f4765 74005f5a 53743137 State_Get._ZSt17
-  0x000082e0 63757272 656e745f 65786365 7074696f current_exceptio
-  0x000082f0 6e764043 58584142 495f312e 332e3300 nv@CXXABI_1.3.3.
-  0x00008300 5f5a4e53 6f395f4d 5f696e73 65727449 _ZNSo9_M_insertI
-  0x00008310 6c454552 536f545f 40474c49 42435858 lEERSoT_@GLIBCXX
-  0x00008320 5f332e34 2e39005f 5f637861 5f616c6c _3.4.9.__cxa_all
-  0x00008330 6f636174 655f6578 63657074 696f6e40 ocate_exception@
-  0x00008340 43585841 42495f31 2e33005f 5a4e4b33 CXXABI_1.3._ZNK3
-  0x00008350 63313034 63756461 34696d70 6c313343 c104cuda4impl13C
-  0x00008360 55444147 75617264 496d706c 31377379 UDAGuardImpl17sy
-  0x00008370 6e636872 6f6e697a 65537472 65616d45 nchronizeStreamE
-  0x00008380 524b4e53 5f365374 7265616d 45005f5a RKNS_6StreamE._Z
-  0x00008390 5453464e 32617436 54656e73 6f724553 TSFN2at6TensorES
-  0x000083a0 305f4500 5f5a4e33 63313036 64657461 0_E._ZN3c106deta
-  0x000083b0 696c3330 696e6665 7246756e 6374696f il30inferFunctio
-  0x000083c0 6e536368 656d6146 726f6d46 756e6374 nSchemaFromFunct
-  0x000083d0 6f724950 464e3261 74365465 6e736f72 orIPFN2at6Tensor
-  0x000083e0 45524b53 335f5335 5f644545 45537431 ERKS3_S5_dEEESt1
-  0x000083f0 30756e69 7175655f 70747249 4e535f31 0unique_ptrINS_1
-  0x00008400 3446756e 6374696f 6e536368 656d6145 4FunctionSchemaE
-  0x00008410 53743134 64656661 756c745f 64656c65 St14default_dele
-  0x00008420 74654953 395f4545 76005079 54797065 teIS9_EEv.PyType
-  0x00008430 5f547970 65005f5a 4e4b3363 31303469 _Type._ZNK3c104i
-  0x00008440 6d706c31 36566972 7475616c 47756172 mpl16VirtualGuar
-  0x00008450 64496d70 6c397365 74446576 69636545 dImpl9setDeviceE
-  0x00008460 4e535f36 44657669 63654500 5f5a4e4b NS_6DeviceE._ZNK
-  0x00008470 33633130 34696d70 6c313656 69727475 3c104impl16Virtu
-  0x00008480 616c4775 61726449 6d706c32 33676574 alGuardImpl23get
-  0x00008490 53747265 616d4672 6f6d476c 6f62616c StreamFromGlobal
-  0x000084a0 506f6f6c 454e535f 36446576 69636545 PoolENS_6DeviceE
-  0x000084b0 62005f5a 4e336331 30313153 796d4e6f b._ZN3c1011SymNo
-  0x000084c0 6465496d 706c3669 735f696e 74457600 deImpl6is_intEv.
-  0x000084d0 5f5a4e33 63313031 3153796d 4e6f6465 _ZN3c1011SymNode
-  0x000084e0 496d706c 336d756c 45524b4e 535f3133 Impl3mulERKNS_13
-  0x000084f0 696e7472 75736976 655f7074 72495330 intrusive_ptrIS0
-  0x00008500 5f4e535f 36646574 61696c33 34696e74 _NS_6detail34int
-  0x00008510 72757369 76655f74 61726765 745f6465 rusive_target_de
-  0x00008520 6661756c 745f6e75 6c6c5f74 79706549 fault_null_typeI
-  0x00008530 53305f45 45454500 5f5a4e39 5f5f676e S0_EEEE._ZN9__gn
-  0x00008540 755f6378 7831325f 5f746f5f 78737472 u_cxx12__to_xstr
-  0x00008550 696e6749 53736345 45545f50 46695054 ingISscEET_PFiPT
-  0x00008560 305f6d50 4b53325f 5031335f 5f76615f 0_mPKS2_P13__va_
-  0x00008570 6c697374 5f746167 456d5335 5f7a005f list_tagEmS5_z._
-  0x00008580 5a4e3363 31303664 65746169 6c31325f ZN3c106detail12_
-  0x00008590 7374725f 77726170 70657249 4a524b63 str_wrapperIJRKc
-  0x000085a0 524b5053 325f5334 5f53365f 53345f45 RKPS2_S4_S6_S4_E
-  0x000085b0 45346361 6c6c4553 335f5336 5f53365f E4callES3_S6_S6_
-  0x000085c0 53365f53 365f0050 79546872 65616453 S6_S6_.PyThreadS
-  0x000085d0 74617465 5f4e6577 005f5a4e 4b336331 tate_New._ZNK3c1
-  0x000085e0 30346375 64613469 6d706c31 33435544 04cuda4impl13CUD
-  0x000085f0 41477561 7264496d 706c3562 6c6f636b AGuardImpl5block
-  0x00008600 45507652 4b4e535f 36537472 65616d45 EPvRKNS_6StreamE
-  0x00008610 005f5a4e 4b336331 3034696d 706c3136 ._ZNK3c104impl16
-  0x00008620 56697274 75616c47 75617264 496d706c VirtualGuardImpl
-  0x00008630 32317265 636f7264 44617461 5074724f 21recordDataPtrO
-  0x00008640 6e537472 65616d45 524b4e53 5f374461 nStreamERKNS_7Da
-  0x00008650 74615074 7245524b 4e535f36 53747265 taPtrERKNS_6Stre
-  0x00008660 616d4500 5f5a5456 4e35746f 72636838 amE._ZTVN5torch8
-  0x00008670 6175746f 67726164 31324175 746f6772 autograd12Autogr
-  0x00008680 61644d65 74614500 5f5a4e33 63313031 adMetaE._ZN3c101
-  0x00008690 3153796d 4e6f6465 496d706c 3133636f 1SymNodeImpl13co
-  0x000086a0 6e737461 6e745f62 6f6f6c45 76005f5a nstant_boolEv._Z
-  0x000086b0 54494e33 63313034 696d706c 32344465 TIN3c104impl24De
-  0x000086c0 76696365 47756172 64496d70 6c496e74 viceGuardImplInt
-  0x000086d0 65726661 63654500 5f5a5456 4e336331 erfaceE._ZTVN3c1
-  0x000086e0 30323069 6e747275 73697665 5f707472 020intrusive_ptr
-  0x000086f0 5f746172 67657445 0050794f 626a6563 _targetE.PyObjec
-  0x00008700 745f5265 7072005f 5a4e3363 31303131 t_Repr._ZN3c1011
-  0x00008710 53796d4e 6f646549 6d706c31 306e6573 SymNodeImpl10nes
-  0x00008720 7465645f 696e7445 76005079 50726f70 ted_intEv.PyProp
-  0x00008730 65727479 5f547970 65005f5a 4e537431 erty_Type._ZNSt1
-  0x00008740 39626164 5f6f7074 696f6e61 6c5f6163 9bad_optional_ac
-  0x00008750 63657373 44314576 00507946 72616d65 cessD1Ev.PyFrame
-  0x00008760 5f476574 4c696e65 4e756d62 65720073 _GetLineNumber.s
-  0x00008770 74726368 7240474c 4942435f 322e322e trchr@GLIBC_2.2.
-  0x00008780 35005f5a 646c5076 6d005079 4572725f 5._ZdlPvm.PyErr_
-  0x00008790 4e6f726d 616c697a 65457863 65707469 NormalizeExcepti
-  0x000087a0 6f6e0050 794f626a 6563745f 436c6561 on.PyObject_Clea
-  0x000087b0 72576561 6b526566 73005079 44696374 rWeakRefs.PyDict
-  0x000087c0 5f4e6578 74005f5a 4e537439 62617369 _Next._ZNSt9basi
-  0x000087d0 635f696f 73496353 74313163 6861725f c_iosIcSt11char_
-  0x000087e0 74726169 74734963 45453469 6e697445 traitsIcEE4initE
-  0x000087f0 50537431 35626173 69635f73 74726561 PSt15basic_strea
-  0x00008800 6d627566 49635331 5f454047 4c494243 mbufIcS1_E@GLIBC
-  0x00008810 58585f33 2e34005f 5a4e3363 31303133 XX_3.4._ZN3c1013
-  0x00008820 696e7472 75736976 655f7074 72494e53 intrusive_ptrINS
-  0x00008830 5f313556 61726961 626c6556 65727369 _15VariableVersi
-  0x00008840 6f6e3134 56657273 696f6e43 6f756e74 on14VersionCount
-  0x00008850 6572454e 535f3664 65746169 6c333469 erENS_6detail34i
-  0x00008860 6e747275 73697665 5f746172 6765745f ntrusive_target_
-  0x00008870 64656661 756c745f 6e756c6c 5f747970 default_null_typ
-  0x00008880 65495332 5f454545 43324550 53325f00 eIS2_EEEC2EPS2_.
-  0x00008890 5f5a5449 53743962 61645f61 6c6c6f63 _ZTISt9bad_alloc
-  0x000088a0 40474c49 42435858 5f332e34 005f5a54 @GLIBCXX_3.4._ZT
-  0x000088b0 494e3363 31303135 56617269 61626c65 IN3c1015Variable
-  0x000088c0 56657273 696f6e31 34566572 73696f6e Version14Version
-  0x000088d0 436f756e 74657245 005f5a4e 4b537431 CounterE._ZNKSt1
-  0x000088e0 35626173 69635f73 7472696e 67627566 5basic_stringbuf
-  0x000088f0 49635374 31316368 61725f74 72616974 IcSt11char_trait
-  0x00008900 73496345 53614963 45453373 74724576 sIcESaIcEE3strEv
-  0x00008910 40474c49 42435858 5f332e34 005f5a54 @GLIBCXX_3.4._ZT
-  0x00008920 49537431 315f4d75 7465785f 62617365 ISt11_Mutex_base
-  0x00008930 494c4e39 5f5f676e 755f6378 7831325f ILN9__gnu_cxx12_
-  0x00008940 4c6f636b 5f706f6c 69637945 32454500 Lock_policyE2EE.
-  0x00008950 5f5a4e53 73395f4d 5f6d7574 61746545 _ZNSs9_M_mutateE
-  0x00008960 6d6d6d40 474c4942 4358585f 332e3400 mmm@GLIBCXX_3.4.
-  0x00008970 5f5a4e37 746f7263 68616f34 335f474c _ZN7torchao43_GL
-  0x00008980 4f42414c 5f5f4e5f 5f356232 65393235 OBAL__N__5b2e925
-  0x00008990 395f365f 6e6d735f 63755f61 31636164 9_6_nms_cu_a1cad
-  0x000089a0 3162665f 32323032 31306e6d 735f6b65 1bf_220210nms_ke
-  0x000089b0 726e656c 45524b4e 32617436 54656e73 rnelERKN2at6Tens
-  0x000089c0 6f724553 345f6400 50794361 7073756c orES4_d.PyCapsul
+  0x00004770 3145504b 63005f5a 4e37746f 72636861 1EPKc._ZN7torcha
+  0x00004780 6f34335f 474c4f42 414c5f5f 4e5f5f35 o43_GLOBAL__N__5
+  0x00004790 62326539 3235395f 365f6e6d 735f6375 b2e9259_6_nms_cu
+  0x000047a0 5f343364 31306539 345f3231 39333130 _43d10e94_219310
+  0x000047b0 6e6d735f 6b65726e 656c4552 4b4e3261 nms_kernelERKN2a
+  0x000047c0 74365465 6e736f72 4553345f 64005f5a t6TensorES4_d._Z
+  0x000047d0 54495374 31326f75 745f6f66 5f72616e TISt12out_of_ran
+  0x000047e0 67654047 4c494243 58585f33 2e34005f ge@GLIBCXX_3.4._
+  0x000047f0 5a323450 61646469 6e675f38 5f465036 Z24Padding_8_FP6
+  0x00004800 5f546f5f 385f4279 74657350 68535f00 _To_8_BytesPhS_.
+  0x00004810 5f5a5374 31377265 7468726f 775f6578 _ZSt17rethrow_ex
+  0x00004820 63657074 696f6e4e 53743135 5f5f6578 ceptionNSt15__ex
+  0x00004830 63657074 696f6e5f 70747231 33657863 ception_ptr13exc
+  0x00004840 65707469 6f6e5f70 74724540 43585841 eption_ptrE@CXXA
+  0x00004850 42495f31 2e332e33 005f5a4e 33633130 BI_1.3.3._ZN3c10
+  0x00004860 34696d70 6c384750 55547261 63653133 4impl8GPUTrace13
+  0x00004870 67707554 72616365 53746174 6545005f gpuTraceStateE._
+  0x00004880 5a4e5374 31365f53 705f636f 756e7465 ZNSt16_Sp_counte
+  0x00004890 645f6261 7365494c 4e395f5f 676e755f d_baseILN9__gnu_
+  0x000048a0 63787831 325f4c6f 636b5f70 6f6c6963 cxx12_Lock_polic
+  0x000048b0 79453245 4531305f 4d5f7265 6c656173 yE2EE10_M_releas
+  0x000048c0 65457600 5f5a4e33 63313031 3153796d eEv._ZN3c1011Sym
+  0x000048d0 4e6f6465 496d706c 31306775 6172645f NodeImpl10guard_
+  0x000048e0 626f6f6c 45504b63 6c005f5a 4e537431 boolEPKcl._ZNSt1
+  0x000048f0 305f4861 73687461 626c6549 50375f6f 0_HashtableIP7_o
+  0x00004900 626a6563 7453315f 53614953 315f454e bjectS1_SaIS1_EN
+  0x00004910 5374385f 5f646574 61696c39 5f496465 St8__detail9_Ide
+  0x00004920 6e746974 79455374 38657175 616c5f74 ntityESt8equal_t
+  0x00004930 6f495331 5f455374 34686173 68495331 oIS1_ESt4hashIS1
+  0x00004940 5f454e53 335f3138 5f4d6f64 5f72616e _ENS3_18_Mod_ran
+  0x00004950 67655f68 61736869 6e67454e 53335f32 ge_hashingENS3_2
+  0x00004960 305f4465 6661756c 745f7261 6e676564 0_Default_ranged
+  0x00004970 5f686173 68454e53 335f3230 5f507269 _hashENS3_20_Pri
+  0x00004980 6d655f72 65686173 685f706f 6c696379 me_rehash_policy
+  0x00004990 454e5333 5f31375f 48617368 7461626c ENS3_17_Hashtabl
+  0x000049a0 655f7472 61697473 494c6230 454c6231 e_traitsILb0ELb1
+  0x000049b0 454c6231 45454545 44314576 005f5a54 ELb1EEEED1Ev._ZT
+  0x000049c0 49537431 326c656e 6774685f 6572726f ISt12length_erro
+  0x000049d0 7240474c 49424358 585f332e 34005f5a r@GLIBCXX_3.4._Z
+  0x000049e0 4e4b5373 3466696e 6445636d 40474c49 NKSs4findEcm@GLI
+  0x000049f0 42435858 5f332e34 005f5a4e 4b336331 BCXX_3.4._ZNK3c1
+  0x00004a00 30364956 616c7565 32337265 706f7274 06IValue23report
+  0x00004a10 546f5465 6e736f72 54797065 4572726f ToTensorTypeErro
+  0x00004a20 72457600 5f656e64 005f5a34 375f5f64 rEv._end._Z47__d
+  0x00004a30 65766963 655f7374 75625f5f 5a313653 evice_stub__Z16S
+  0x00004a40 706c6974 4b5f5265 64756374 696f6e50 plitK_ReductionP
+  0x00004a50 365f5f68 616c6650 666d6d69 50365f5f 6__halfPfmmiP6__
+  0x00004a60 68616c66 50666d6d 69005f5a 4e537339 halfPfmmi._ZNSs9
+  0x00004a70 70757368 5f626163 6b456340 474c4942 push_backEc@GLIB
+  0x00004a80 4358585f 332e3400 5f5a4e33 63313036 CXX_3.4._ZN3c106
+  0x00004a90 64657461 696c3132 5f737472 5f777261 detail12_str_wra
+  0x00004aa0 70706572 494a504b 63524b53 335f4545 pperIJPKcRKS3_EE
+  0x00004ab0 3463616c 6c455335 5f53355f 005f5a54 4callES5_S5_._ZT
+  0x00004ac0 56537431 39626173 69635f6f 73747269 VSt19basic_ostri
+  0x00004ad0 6e677374 7265616d 49635374 31316368 ngstreamIcSt11ch
+  0x00004ae0 61725f74 72616974 73496345 53614963 ar_traitsIcESaIc
+  0x00004af0 45454047 4c494243 58585f33 2e340050 EE@GLIBCXX_3.4.P
+  0x00004b00 79457272 5f577269 7465556e 72616973 yErr_WriteUnrais
+  0x00004b10 61626c65 00507954 68726561 645f7473 able.PyThread_ts
+  0x00004b20 735f6372 65617465 00737472 6c656e40 s_create.strlen@
+  0x00004b30 474c4942 435f322e 322e3500 5f5a4e33 GLIBC_2.2.5._ZN3
+  0x00004b40 63313036 64657461 696c3132 5f737472 c106detail12_str
+  0x00004b50 5f777261 70706572 494a504b 63524b4e _wrapperIJPKcRKN
+  0x00004b60 535f3130 5363616c 61725479 70654553 S_10ScalarTypeES
+  0x00004b70 335f4545 3463616c 6c45524b 53335f53 3_EE4callERKS3_S
+  0x00004b80 365f5339 5f005f5a 4e537431 355f5f65 6_S9_._ZNSt15__e
+  0x00004b90 78636570 74696f6e 5f707472 31336578 xception_ptr13ex
+  0x00004ba0 63657074 696f6e5f 70747243 3145524b ception_ptrC1ERK
+  0x00004bb0 53305f40 43585841 42495f31 2e332e33 S0_@CXXABI_1.3.3
+  0x00004bc0 005f5a31 33636173 745f6670 31365f66 ._Z13cast_fp16_f
+  0x00004bd0 70365074 5068005f 5a54534e 33633130 p6PtPh._ZTSN3c10
+  0x00004be0 31344f70 65726174 6f724b65 726e656c 14OperatorKernel
+  0x00004bf0 45005f5a 54564e31 305f5f63 78786162 E._ZTVN10__cxxab
+  0x00004c00 69763131 375f5f63 6c617373 5f747970 iv117__class_typ
+  0x00004c10 655f696e 666f4540 43585841 42495f31 e_infoE@CXXABI_1
+  0x00004c20 2e330050 794f626a 6563745f 48617341 .3.PyObject_HasA
+  0x00004c30 74747253 7472696e 67005f5a 54565374 ttrString._ZTVSt
+  0x00004c40 39626164 5f616c6c 6f634047 4c494243 9bad_alloc@GLIBC
+  0x00004c50 58585f33 2e34005f 5a313751 55414e54 XX_3.4._Z17QUANT
+  0x00004c60 5f47454d 4d5f4b65 726e656c 49313254 _GEMM_KernelI12T
+  0x00004c70 696c696e 67436f6e 66696749 4c693445 ilingConfigILi4E
+  0x00004c80 4c693145 4c693445 45664576 504b3575 Li1ELi4EEfEvPK5u
+  0x00004c90 696e7434 504b365f 5f68616c 6653375f int4PK6__halfS7_
+  0x00004ca0 5054305f 6d6d6d69 005f5f63 78615f67 PT0_mmmi.__cxa_g
+  0x00004cb0 75617264 5f61626f 72744043 58584142 uard_abort@CXXAB
+  0x00004cc0 495f312e 33006375 64615374 7265616d I_1.3.cudaStream
+  0x00004cd0 51756572 79406c69 62637564 6172742e Query@libcudart.
+  0x00004ce0 736f2e31 32005f5f 63756461 52656769 so.12.__cudaRegi
+  0x00004cf0 73746572 46617442 696e6172 79406c69 sterFatBinary@li
+  0x00004d00 62637564 6172742e 736f2e31 32005f5a bcudart.so.12._Z
+  0x00004d10 4e336331 30313054 656e736f 72547970 N3c1010TensorTyp
+  0x00004d20 65336765 74457600 5f5a4e4b 33633130 e3getEv._ZNK3c10
+  0x00004d30 34696d70 6c313656 69727475 616c4775 4impl16VirtualGu
+  0x00004d40 61726449 6d706c35 626c6f63 6b455076 ardImpl5blockEPv
+  0x00004d50 524b4e53 5f365374 7265616d 45005f5a RKNS_6StreamE._Z
+  0x00004d60 4e336331 30365379 6d496e74 4331454e N3c106SymIntC1EN
+  0x00004d70 535f3133 696e7472 75736976 655f7074 S_13intrusive_pt
+  0x00004d80 72494e53 5f313153 796d4e6f 6465496d rINS_11SymNodeIm
+  0x00004d90 706c454e 535f3664 65746169 6c333469 plENS_6detail34i
+  0x00004da0 6e747275 73697665 5f746172 6765745f ntrusive_target_
+  0x00004db0 64656661 756c745f 6e756c6c 5f747970 default_null_typ
+  0x00004dc0 65495332 5f454545 45005f5a 4e336331 eIS2_EEEE._ZN3c1
+  0x00004dd0 30346375 64613134 45786368 616e6765 04cuda14Exchange
+  0x00004de0 44657669 63654561 005f5a4e 33633130 DeviceEa._ZN3c10
+  0x00004df0 34637564 61323073 65744375 7272656e 4cuda20setCurren
+  0x00004e00 74435544 41537472 65616d45 4e53305f tCUDAStreamENS0_
+  0x00004e10 31304355 44415374 7265616d 45005f5a 10CUDAStreamE._Z
+  0x00004e20 54494e33 63313032 30696e74 72757369 TIN3c1020intrusi
+  0x00004e30 76655f70 74725f74 61726765 7445005f ve_ptr_targetE._
+  0x00004e40 5a4e4b33 63313035 4572726f 72323277 ZNK3c105Error22w
+  0x00004e50 6861745f 77697468 6f75745f 6261636b hat_without_back
+  0x00004e60 74726163 65457600 5f5a5449 464e3261 traceEv._ZTIFN2a
+  0x00004e70 74365465 6e736f72 45524b53 305f5332 t6TensorERKS0_S2
+  0x00004e80 5f644500 5f5a4e53 74313372 756e7469 _dE._ZNSt13runti
+  0x00004e90 6d655f65 72726f72 44324576 40474c49 me_errorD2Ev@GLI
+  0x00004ea0 42435858 5f332e34 005f5a53 7431316d BCXX_3.4._ZSt11m
+  0x00004eb0 616b655f 756e6971 7565494e 35746f72 ake_uniqueIN5tor
+  0x00004ec0 63683861 75746f67 72616431 32417574 ch8autograd12Aut
+  0x00004ed0 6f677261 644d6574 61454a50 4e336331 ogradMetaEJPN3c1
+  0x00004ee0 30313054 656e736f 72496d70 6c455262 010TensorImplERb
+  0x00004ef0 45454e53 74395f4d 616b6555 6e697149 EENSt9_MakeUniqI
+  0x00004f00 545f4531 355f5f73 696e676c 655f6f62 T_E15__single_ob
+  0x00004f10 6a656374 4544704f 54305f00 5f5a5456 jectEDpOT0_._ZTV
+  0x00004f20 4e31305f 5f637878 61626976 3132305f N10__cxxabiv120_
+  0x00004f30 5f66756e 6374696f 6e5f7479 70655f69 _function_type_i
+  0x00004f40 6e666f45 40435858 4142495f 312e3300 nfoE@CXXABI_1.3.
+  0x00004f50 5f5a4e33 63313031 3153796d 4e6f6465 _ZN3c1011SymNode
+  0x00004f60 496d706c 3773796d 5f6e6f74 4576005f Impl7sym_notEv._
+  0x00004f70 5a4e3261 74345f6f 70733974 6f5f6465 ZN2at4_ops9to_de
+  0x00004f80 76696365 3463616c 6c45524b 4e535f36 vice4callERKNS_6
+  0x00004f90 54656e73 6f72454e 33633130 36446576 TensorEN3c106Dev
+  0x00004fa0 69636545 4e53355f 31305363 616c6172 iceENS5_10Scalar
+  0x00004fb0 54797065 45626253 74386f70 74696f6e TypeEbbSt8option
+  0x00004fc0 616c494e 53355f31 324d656d 6f727946 alINS5_12MemoryF
+  0x00004fd0 6f726d61 74454500 5f5a5453 4e336331 ormatEE._ZTSN3c1
+  0x00004fe0 30313556 61726961 626c6556 65727369 015VariableVersi
+  0x00004ff0 6f6e3134 56657273 696f6e43 6f756e74 on14VersionCount
+  0x00005000 65724500 50794279 7465735f 41735374 erE.PyBytes_AsSt
+  0x00005010 72696e67 005f5a4e 53743133 5f427665 ring._ZNSt13_Bve
+  0x00005020 63746f72 5f626173 65495361 49624545 ctor_baseISaIbEE
+  0x00005030 31335f4d 5f646561 6c6c6f63 61746545 13_M_deallocateE
+  0x00005040 76005f5a 4e537331 325f4d5f 6c65616b v._ZNSs12_M_leak
+  0x00005050 5f686172 64457640 474c4942 4358585f _hardEv@GLIBCXX_
+  0x00005060 332e3400 5f5a5449 464e3261 74365465 3.4._ZTIFN2at6Te
+  0x00005070 6e736f72 4553305f 53305f45 005f5a4e nsorES0_S0_E._ZN
+  0x00005080 33633130 31315379 6d4e6f64 65496d70 3c1011SymNodeImp
+  0x00005090 6c377379 6d5f6974 6545524b 4e535f31 l7sym_iteERKNS_1
+  0x000050a0 33696e74 72757369 76655f70 74724953 3intrusive_ptrIS
+  0x000050b0 305f4e53 5f366465 7461696c 3334696e 0_NS_6detail34in
+  0x000050c0 74727573 6976655f 74617267 65745f64 trusive_target_d
+  0x000050d0 65666175 6c745f6e 756c6c5f 74797065 efault_null_type
+  0x000050e0 4953305f 45454545 53375f00 5f5a4e33 IS0_EEEES7_._ZN3
+  0x000050f0 63313036 64657461 696c3233 746f7263 c106detail23torc
+  0x00005100 68496e74 65726e61 6c417373 65727446 hInternalAssertF
+  0x00005110 61696c45 504b6353 325f6a53 325f5332 ailEPKcS2_jS2_S2
+  0x00005120 5f005f5a 4e336331 30313153 796d4e6f _._ZN3c1011SymNo
+  0x00005130 6465496d 706c3869 735f666c 6f617445 deImpl8is_floatE
+  0x00005140 76005f5a 31375155 414e545f 47454d4d v._Z17QUANT_GEMM
+  0x00005150 5f4b6572 6e656c49 31325469 6c696e67 _KernelI12Tiling
+  0x00005160 436f6e66 6967494c 6934454c 6931454c ConfigILi4ELi1EL
+  0x00005170 69314545 365f5f68 616c6645 76504b35 i1EE6__halfEvPK5
+  0x00005180 75696e74 34504b53 325f5337 5f505430 uint4PKS2_S7_PT0
+  0x00005190 5f6d6d6d 69005f5a 4e536f39 5f4d5f69 _mmmi._ZNSo9_M_i
+  0x000051a0 6e736572 74496d45 4552536f 545f4047 nsertImEERSoT_@G
+  0x000051b0 4c494243 58585f33 2e342e39 005f5a53 LIBCXX_3.4.9._ZS
+  0x000051c0 7431315f 48617368 5f627974 6573504b t11_Hash_bytesPK
+  0x000051d0 766d6d40 43585841 42495f31 2e332e35 vmm@CXXABI_1.3.5
+  0x000051e0 005f5a4e 4b537335 7266696e 6445504b ._ZNKSs5rfindEPK
+  0x000051f0 636d6d40 474c4942 4358585f 332e3400 cmm@GLIBCXX_3.4.
+  0x00005200 5f5a4e4b 53733137 66696e64 5f666972 _ZNKSs17find_fir
+  0x00005210 73745f6e 6f745f6f 6645504b 636d6d40 st_not_ofEPKcmm@
+  0x00005220 474c4942 4358585f 332e3400 50794279 GLIBCXX_3.4.PyBy
+  0x00005230 74654172 7261795f 53697a65 005f5a4e teArray_Size._ZN
+  0x00005240 32617438 696e6465 78696e67 31315465 2at8indexing11Te
+  0x00005250 6e736f72 496e6465 78443145 76005f5a nsorIndexD1Ev._Z
+  0x00005260 646c5076 40474c49 42435858 5f332e34 dlPv@GLIBCXX_3.4
+  0x00005270 005f5a4e 4b336331 30346375 64613469 ._ZNK3c104cuda4i
+  0x00005280 6d706c31 33435544 41477561 7264496d mpl13CUDAGuardIm
+  0x00005290 706c3233 67657453 74726561 6d46726f pl23getStreamFro
+  0x000052a0 6d476c6f 62616c50 6f6f6c45 4e535f36 mGlobalPoolENS_6
+  0x000052b0 44657669 63654562 005f5a4e 4b336331 DeviceEb._ZNK3c1
+  0x000052c0 3034696d 706c3136 56697274 75616c47 04impl16VirtualG
+  0x000052d0 75617264 496d706c 31326765 744e6577 uardImpl12getNew
+  0x000052e0 53747265 616d454e 535f3644 65766963 StreamENS_6Devic
+  0x000052f0 65456900 5f5a4e53 73433145 504b636d eEi._ZNSsC1EPKcm
+  0x00005300 524b5361 49634540 474c4942 4358585f RKSaIcE@GLIBCXX_
+  0x00005310 332e3400 5f5a4e33 63313031 3153796d 3.4._ZN3c1011Sym
+  0x00005320 4e6f6465 496d706c 31326d61 7962655f NodeImpl12maybe_
+  0x00005330 61735f69 6e744576 005f5a4e 33633130 as_intEv._ZN3c10
+  0x00005340 31344f70 65726174 6f724b65 726e656c 14OperatorKernel
+  0x00005350 44304576 00507943 61707375 6c655f47 D0Ev.PyCapsule_G
+  0x00005360 6574436f 6e746578 74005f5a 4e4b3261 etContext._ZNK2a
+  0x00005370 74313054 656e736f 72426173 6532315f t10TensorBase21_
+  0x00005380 5f646973 70617463 685f636f 6e746967 _dispatch_contig
+  0x00005390 756f7573 454e3363 31303132 4d656d6f uousEN3c1012Memo
+  0x000053a0 7279466f 726d6174 45005f5a 4e336331 ryFormatE._ZN3c1
+  0x000053b0 30313153 796d4e6f 6465496d 706c3562 011SymNodeImpl5b
+  0x000053c0 6f6f6c5f 4576005f 5a4e4b33 63313034 ool_Ev._ZNK3c104
+  0x000053d0 696d706c 31365669 72747561 6c477561 impl16VirtualGua
+  0x000053e0 7264496d 706c3137 73796e63 68726f6e rdImpl17synchron
+  0x000053f0 697a6553 74726561 6d45524b 4e535f36 izeStreamERKNS_6
+  0x00005400 53747265 616d4500 5f5a4e32 6174345f StreamE._ZN2at4_
+  0x00005410 6f707331 39656d70 74795f6d 656d6f72 ops19empty_memor
+  0x00005420 795f666f 726d6174 3463616c 6c454e33 y_format4callEN3
+  0x00005430 63313038 41727261 79526566 494e5332 c108ArrayRefINS2
+  0x00005440 5f365379 6d496e74 45454553 74386f70 _6SymIntEEESt8op
+  0x00005450 74696f6e 616c494e 53325f31 30536361 tionalINS2_10Sca
+  0x00005460 6c617254 79706545 4553365f 494e5332 larTypeEES6_INS2
+  0x00005470 5f364c61 796f7574 45455336 5f494e53 _6LayoutEES6_INS
+  0x00005480 325f3644 65766963 65454553 365f4962 2_6DeviceEES6_Ib
+  0x00005490 4553365f 494e5332 5f31324d 656d6f72 ES6_INS2_12Memor
+  0x000054a0 79466f72 6d617445 45005f5a 4e336331 yFormatEE._ZN3c1
+  0x000054b0 30313153 796d4e6f 6465496d 706c3563 011SymNodeImpl5c
+  0x000054c0 6c6f6e65 4576005f 5a54494e 33633130 loneEv._ZTIN3c10
+  0x000054d0 31344f70 65726174 6f724b65 726e656c 14OperatorKernel
+  0x000054e0 45005f5a 4e537336 61707065 6e644550 E._ZNSs6appendEP
+  0x000054f0 4b636d40 474c4942 4358585f 332e3400 Kcm@GLIBCXX_3.4.
+  0x00005500 5f5a4e33 63313032 30696e74 72757369 _ZN3c1020intrusi
+  0x00005510 76655f70 74725f74 61726765 74443045 ve_ptr_targetD0E
+  0x00005520 76005f5a 4e537334 73776170 45525373 v._ZNSs4swapERSs
+  0x00005530 40474c49 42435858 5f332e34 005f5a54 @GLIBCXX_3.4._ZT
+  0x00005540 564e3363 31303135 56617269 61626c65 VN3c1015Variable
+  0x00005550 56657273 696f6e31 34566572 73696f6e Version14Version
+  0x00005560 436f756e 74657245 005f5079 54797065 CounterE._PyType
+  0x00005570 5f4c6f6f 6b757000 50795468 72656164 _Lookup.PyThread
+  0x00005580 53746174 655f436c 65617200 50794572 State_Clear.PyEr
+  0x00005590 725f436c 65617200 5f5a4e53 74367665 r_Clear._ZNSt6ve
+  0x000055a0 63746f72 49625361 49624545 31345f4d ctorIbSaIbEE14_M
+  0x000055b0 5f66696c 6c5f696e 73657274 45537431 _fill_insertESt1
+  0x000055c0 335f4269 745f6974 65726174 6f726d62 3_Bit_iteratormb
+  0x000055d0 005f5f63 78615f74 68726f77 40435858 .__cxa_throw@CXX
+  0x000055e0 4142495f 312e3300 63756461 53747265 ABI_1.3.cudaStre
+  0x000055f0 616d5379 6e636872 6f6e697a 65406c69 amSynchronize@li
+  0x00005600 62637564 6172742e 736f2e31 32005f5a bcudart.so.12._Z
+  0x00005610 5453464e 32617436 54656e73 6f724552 TSFN2at6TensorER
+  0x00005620 4b53305f 53325f64 45005f5a 4e37746f KS0_S2_dE._ZN7to
+  0x00005630 72636861 6f34335f 474c4f42 414c5f5f rchao43_GLOBAL__
+  0x00005640 4e5f5f35 62326539 3235395f 365f6e6d N__5b2e9259_6_nm
+  0x00005650 735f6375 5f343364 31306539 345f3231 s_cu_43d10e94_21
+  0x00005660 39333135 6e6d735f 6b65726e 656c5f69 9315nms_kernel_i
+  0x00005670 6d706c49 66454576 6964504b 545f5079 mplIfEEvidPKT_Py
+  0x00005680 00507943 61707375 6c655f4e 65770050 .PyCapsule_New.P
+  0x00005690 794d656d 5f43616c 6c6f6300 5f5a4e33 yMem_Calloc._ZN3
+  0x000056a0 63313034 696d706c 36646574 61696c33 c104impl6detail3
+  0x000056b0 31577261 7046756e 6374696f 6e496e74 1WrapFunctionInt
+  0x000056c0 6f52756e 74696d65 46756e63 746f725f oRuntimeFunctor_
+  0x000056d0 4950464e 32617436 54656e73 6f724553 IPFN2at6TensorES
+  0x000056e0 345f5334 5f455334 5f4e535f 34677574 4_S4_ES4_NS_4gut
+  0x000056f0 73387479 70656c69 73743874 7970656c s8typelist8typel
+  0x00005700 69737449 4a53345f 53345f45 45454544 istIJS4_S4_EEEED
+  0x00005710 31457600 5f5a4e33 63313036 64657461 1Ev._ZN3c106deta
+  0x00005720 696c3132 5f737472 5f777261 70706572 il12_str_wrapper
+  0x00005730 494a504b 63524b6c 45453463 616c6c45 IJPKcRKlEE4callE
+  0x00005740 524b5333 5f53355f 005f5a4e 32617434 RKS3_S5_._ZN2at4
+  0x00005750 5f6f7073 3131736f 72745f73 7461626c _ops11sort_stabl
+  0x00005760 65346361 6c6c4552 4b4e535f 3654656e e4callERKNS_6Ten
+  0x00005770 736f7245 5374386f 7074696f 6e616c49 sorESt8optionalI
+  0x00005780 62456c62 005f5a53 7432305f 5f746872 bElb._ZSt20__thr
+  0x00005790 6f775f6c 656e6774 685f6572 726f7250 ow_length_errorP
+  0x000057a0 4b634047 4c494243 58585f33 2e34005f Kc@GLIBCXX_3.4._
+  0x000057b0 5a4e3574 6f726368 374c6962 72617279 ZN5torch7Library
+  0x000057c0 4331454e 53305f34 4b696e64 45537353 C1ENS0_4KindESsS
+  0x000057d0 74386f70 74696f6e 616c494e 33633130 t8optionalIN3c10
+  0x000057e0 31314469 73706174 63684b65 79454550 11DispatchKeyEEP
+  0x000057f0 4b636a00 5f556e77 696e645f 52657375 Kcj._Unwind_Resu
+  0x00005800 6d654047 43435f33 2e30005f 5a4e4b33 me@GCC_3.0._ZNK3
+  0x00005810 63313034 63756461 34696d70 6c313343 c104cuda4impl13C
+  0x00005820 55444147 75617264 496d706c 31317175 UDAGuardImpl11qu
+  0x00005830 65727953 74726561 6d45524b 4e535f36 eryStreamERKNS_6
+  0x00005840 53747265 616d4500 50794279 7465735f StreamE.PyBytes_
+  0x00005850 53697a65 005f5a54 534e3363 31303469 Size._ZTSN3c104i
+  0x00005860 6d706c36 64657461 696c3331 57726170 mpl6detail31Wrap
+  0x00005870 46756e63 74696f6e 496e746f 52756e74 FunctionIntoRunt
+  0x00005880 696d6546 756e6374 6f725f49 50464e32 imeFunctor_IPFN2
+  0x00005890 61743654 656e736f 72455334 5f53345f at6TensorES4_S4_
+  0x000058a0 4553345f 4e535f34 67757473 38747970 ES4_NS_4guts8typ
+  0x000058b0 656c6973 74387479 70656c69 7374494a elist8typelistIJ
+  0x000058c0 53345f53 345f4545 45454500 5f5a4e33 S4_S4_EEEEE._ZN3
+  0x000058d0 63313031 3153796d 4e6f6465 496d706c c1011SymNodeImpl
+  0x000058e0 31366e65 73746564 5f696e74 5f636f65 16nested_int_coe
+  0x000058f0 66664576 005f5a4e 4b336331 30346375 ffEv._ZNK3c104cu
+  0x00005900 64613469 6d706c31 33435544 41477561 da4impl13CUDAGua
+  0x00005910 7264496d 706c3136 73796e63 68726f6e rdImpl16synchron
+  0x00005920 697a6545 76656e74 45507600 5f5a4e33 izeEventEPv._ZN3
+  0x00005930 63313034 63756461 31326465 76696365 c104cuda12device
+  0x00005940 5f636f75 6e744576 005f5a4e 4b336331 _countEv._ZNK3c1
+  0x00005950 30346375 64613469 6d706c31 33435544 04cuda4impl13CUD
+  0x00005960 41477561 7264496d 706c3967 65744465 AGuardImpl9getDe
+  0x00005970 76696365 4576005f 5a323042 6974496e viceEv._Z20BitIn
+  0x00005980 7465726c 65617669 6e675f32 62697450 terleaving_2bitP
+  0x00005990 68005f5a 4e37746f 72636861 6f323577 h._ZN7torchao25w
+  0x000059a0 65696768 745f6d61 74726978 5f646571 eight_matrix_deq
+  0x000059b0 75616e74 5f637075 454e3261 74365465 uant_cpuEN2at6Te
+  0x000059c0 6e736f72 4553315f 0076736e 7072696e nsorES1_.vsnprin
+  0x000059d0 74664047 4c494243 5f322e32 2e35005f tf@GLIBC_2.2.5._
+  0x000059e0 5a4e3363 31303469 6d706c32 38777261 ZN3c104impl28wra
+  0x000059f0 705f6b65 726e656c 5f66756e 63746f72 p_kernel_functor
+  0x00005a00 5f756e62 6f786564 5f494e53 305f3664 _unboxed_INS0_6d
+  0x00005a10 65746169 6c333157 72617046 756e6374 etail31WrapFunct
+  0x00005a20 696f6e49 6e746f52 756e7469 6d654675 ionIntoRuntimeFu
+  0x00005a30 6e63746f 725f4950 464e3261 74365465 nctor_IPFN2at6Te
+  0x00005a40 6e736f72 4553355f 4553355f 4e535f34 nsorES5_ES5_NS_4
+  0x00005a50 67757473 38747970 656c6973 74387479 guts8typelist8ty
+  0x00005a60 70656c69 7374494a 53355f45 45454545 pelistIJS5_EEEEE
+  0x00005a70 53365f45 3463616c 6c45504e 535f3134 S6_E4callEPNS_14
+  0x00005a80 4f706572 61746f72 4b65726e 656c454e OperatorKernelEN
+  0x00005a90 535f3134 44697370 61746368 4b657953 S_14DispatchKeyS
+  0x00005aa0 65744553 355f005f 5a4e3363 31303135 etES5_._ZN3c1015
+  0x00005ab0 56617269 61626c65 56657273 696f6e31 VariableVersion1
+  0x00005ac0 34566572 73696f6e 436f756e 74657244 4VersionCounterD
+  0x00005ad0 30457600 5f5a4e33 63313031 3153796d 0Ev._ZN3c1011Sym
+  0x00005ae0 4e6f6465 496d706c 3773796d 5f6d6178 NodeImpl7sym_max
+  0x00005af0 45524b4e 535f3133 696e7472 75736976 ERKNS_13intrusiv
+  0x00005b00 655f7074 72495330 5f4e535f 36646574 e_ptrIS0_NS_6det
+  0x00005b10 61696c33 34696e74 72757369 76655f74 ail34intrusive_t
+  0x00005b20 61726765 745f6465 6661756c 745f6e75 arget_default_nu
+  0x00005b30 6c6c5f74 79706549 53305f45 45454500 ll_typeIS0_EEEE.
+  0x00005b40 5f5a5449 464e3261 74365465 6e736f72 _ZTIFN2at6Tensor
+  0x00005b50 4553305f 53305f53 305f6c45 00507945 ES0_S0_S0_lE.PyE
+  0x00005b60 78635f54 79706545 72726f72 005f5a4e xc_TypeError._ZN
+  0x00005b70 33633130 31315379 6d4e6f64 65496d70 3c1011SymNodeImp
+  0x00005b80 6c35666c 6f6f7245 76005f5a 54494e33 l5floorEv._ZTIN3
+  0x00005b90 63313034 63756461 34696d70 6c313343 c104cuda4impl13C
+  0x00005ba0 55444147 75617264 496d706c 45005f5a UDAGuardImplE._Z
+  0x00005bb0 4e4b3363 31303469 6d706c31 36566972 NK3c104impl16Vir
+  0x00005bc0 7475616c 47756172 64496d70 6c313875 tualGuardImpl18u
+  0x00005bd0 6e636865 636b6564 53657444 65766963 ncheckedSetDevic
+  0x00005be0 65454e53 5f364465 76696365 45005f5a eENS_6DeviceE._Z
+  0x00005bf0 4e4b3363 31303463 75646134 696d706c NK3c104cuda4impl
+  0x00005c00 31334355 44414775 61726449 6d706c39 13CUDAGuardImpl9
+  0x00005c10 73657444 65766963 65454e53 5f364465 setDeviceENS_6De
+  0x00005c20 76696365 45005f5a 54564e33 63313031 viceE._ZTVN3c101
+  0x00005c30 3153796d 4e6f6465 496d706c 45005f5a 1SymNodeImplE._Z
+  0x00005c40 54494e33 63313031 3056616c 75654572 TIN3c1010ValueEr
+  0x00005c50 726f7245 005f5a54 564e3363 31303469 rorE._ZTVN3c104i
+  0x00005c60 6d706c36 64657461 696c3331 57726170 mpl6detail31Wrap
+  0x00005c70 46756e63 74696f6e 496e746f 52756e74 FunctionIntoRunt
+  0x00005c80 696d6546 756e6374 6f725f49 50464e32 imeFunctor_IPFN2
+  0x00005c90 61743654 656e736f 72455334 5f455334 at6TensorES4_ES4
+  0x00005ca0 5f4e535f 34677574 73387479 70656c69 _NS_4guts8typeli
+  0x00005cb0 73743874 7970656c 69737449 4a53345f st8typelistIJS4_
+  0x00005cc0 45454545 45005079 54797065 5f526561 EEEEE.PyType_Rea
+  0x00005cd0 6479005f 5a544953 74313962 61645f6f dy._ZTISt19bad_o
+  0x00005ce0 7074696f 6e616c5f 61636365 7373005f ptional_access._
+  0x00005cf0 5a54534e 33633130 34696d70 6c366465 ZTSN3c104impl6de
+  0x00005d00 7461696c 33315772 61704675 6e637469 tail31WrapFuncti
+  0x00005d10 6f6e496e 746f5275 6e74696d 6546756e onIntoRuntimeFun
+  0x00005d20 63746f72 5f495046 4e326174 3654656e ctor_IPFN2at6Ten
+  0x00005d30 736f7245 53345f45 53345f4e 535f3467 sorES4_ES4_NS_4g
+  0x00005d40 75747338 74797065 6c697374 38747970 uts8typelist8typ
+  0x00005d50 656c6973 74494a53 345f4545 45454500 elistIJS4_EEEEE.
+  0x00005d60 5f5a4e33 63313031 3153796d 4e6f6465 _ZN3c1011SymNode
+  0x00005d70 496d706c 32676545 524b4e53 5f313369 Impl2geERKNS_13i
+  0x00005d80 6e747275 73697665 5f707472 4953305f ntrusive_ptrIS0_
+  0x00005d90 4e535f36 64657461 696c3334 696e7472 NS_6detail34intr
+  0x00005da0 75736976 655f7461 72676574 5f646566 usive_target_def
+  0x00005db0 61756c74 5f6e756c 6c5f7479 70654953 ault_null_typeIS
+  0x00005dc0 305f4545 4545005f 5a4e3363 31303545 0_EEEE._ZN3c105E
+  0x00005dd0 72726f72 4332454e 535f3134 536f7572 rrorC2ENS_14Sour
+  0x00005de0 63654c6f 63617469 6f6e4553 73005f5a ceLocationESs._Z
+  0x00005df0 4e37746f 72636861 6f34335f 474c4f42 N7torchao43_GLOB
+  0x00005e00 414c5f5f 4e5f5f35 62326539 3235395f AL__N__5b2e9259_
+  0x00005e10 365f6e6d 735f6375 5f343364 31306539 6_nms_cu_43d10e9
+  0x00005e20 345f3231 39333135 6e6d735f 6b65726e 4_219315nms_kern
+  0x00005e30 656c5f69 6d706c49 64454576 6964504b el_implIdEEvidPK
+  0x00005e40 545f5079 005f5a54 494e3363 31303131 T_Py._ZTIN3c1011
+  0x00005e50 53796d4e 6f646549 6d706c45 005f5a53 SymNodeImplE._ZS
+  0x00005e60 7432345f 5f746872 6f775f6f 75745f6f t24__throw_out_o
+  0x00005e70 665f7261 6e67655f 666d7450 4b637a00 f_range_fmtPKcz.
+  0x00005e80 5f5a3137 5155414e 545f4745 4d4d5f4b _Z17QUANT_GEMM_K
+  0x00005e90 65726e65 6c493132 54696c69 6e67436f ernelI12TilingCo
+  0x00005ea0 6e666967 494c6934 454c6931 454c6931 nfigILi4ELi1ELi1
+  0x00005eb0 45456645 76504b35 75696e74 34504b36 EEfEvPK5uint4PK6
+  0x00005ec0 5f5f6861 6c665337 5f505430 5f6d6d6d __halfS7_PT0_mmm
+  0x00005ed0 69005f5a 4e336331 3034696d 706c3664 i._ZN3c104impl6d
+  0x00005ee0 65746169 6c333157 72617046 756e6374 etail31WrapFunct
+  0x00005ef0 696f6e49 6e746f52 756e7469 6d654675 ionIntoRuntimeFu
+  0x00005f00 6e63746f 725f4950 464e3261 74365465 nctor_IPFN2at6Te
+  0x00005f10 6e736f72 4553345f 53345f53 345f6c45 nsorES4_S4_S4_lE
+  0x00005f20 53345f4e 535f3467 75747338 74797065 S4_NS_4guts8type
+  0x00005f30 6c697374 38747970 656c6973 74494a53 list8typelistIJS
+  0x00005f40 345f5334 5f53345f 6c454545 45443045 4_S4_S4_lEEEED0E
+  0x00005f50 76005f5a 4e336331 30313153 796d4e6f v._ZN3c1011SymNo
+  0x00005f60 6465496d 706c3133 69735f63 6f6e7469 deImpl13is_conti
+  0x00005f70 67756f75 73454e53 5f384172 72617952 guousENS_8ArrayR
+  0x00005f80 6566494e 535f3133 696e7472 75736976 efINS_13intrusiv
+  0x00005f90 655f7074 72495330 5f4e535f 36646574 e_ptrIS0_NS_6det
+  0x00005fa0 61696c33 34696e74 72757369 76655f74 ail34intrusive_t
+  0x00005fb0 61726765 745f6465 6661756c 745f6e75 arget_default_nu
+  0x00005fc0 6c6c5f74 79706549 53305f45 45454545 ll_typeIS0_EEEEE
+  0x00005fd0 4553375f 005f5a4e 33633130 31315379 ES7_._ZN3c1011Sy
+  0x00005fe0 6d4e6f64 65496d70 6c443045 76005f5a mNodeImplD0Ev._Z
+  0x00005ff0 4e537336 61737369 676e4552 4b537340 NSs6assignERKSs@
+  0x00006000 474c4942 4358585f 332e3400 5f5a4e53 GLIBCXX_3.4._ZNS
+  0x00006010 73366173 7369676e 45504b63 6d40474c s6assignEPKcm@GL
+  0x00006020 49424358 585f332e 34005f5a 4e336331 IBCXX_3.4._ZN3c1
+  0x00006030 30313153 796d4e6f 6465496d 706c3673 011SymNodeImpl6s
+  0x00006040 796d5f6f 7245524b 4e535f31 33696e74 ym_orERKNS_13int
+  0x00006050 72757369 76655f70 74724953 305f4e53 rusive_ptrIS0_NS
+  0x00006060 5f366465 7461696c 3334696e 74727573 _6detail34intrus
+  0x00006070 6976655f 74617267 65745f64 65666175 ive_target_defau
+  0x00006080 6c745f6e 756c6c5f 74797065 4953305f lt_null_typeIS0_
+  0x00006090 45454545 005f5a4e 33633130 31315379 EEEE._ZN3c1011Sy
+  0x000060a0 6d4e6f64 65496d70 6c33706f 7745524b mNodeImpl3powERK
+  0x000060b0 4e535f31 33696e74 72757369 76655f70 NS_13intrusive_p
+  0x000060c0 74724953 305f4e53 5f366465 7461696c trIS0_NS_6detail
+  0x000060d0 3334696e 74727573 6976655f 74617267 34intrusive_targ
+  0x000060e0 65745f64 65666175 6c745f6e 756c6c5f et_default_null_
+  0x000060f0 74797065 4953305f 45454545 005f5a4e typeIS0_EEEE._ZN
+  0x00006100 33633130 36646574 61696c32 33746f72 3c106detail23tor
+  0x00006110 6368496e 7465726e 616c4173 73657274 chInternalAssert
+  0x00006120 4661696c 45504b63 53325f6a 53325f52 FailEPKcS2_jS2_R
+  0x00006130 4b537300 5079496e 69745f5f 43005f5a KSs.PyInit__C._Z
+  0x00006140 4e537336 61707065 6e644552 4b537340 NSs6appendERKSs@
+  0x00006150 474c4942 4358585f 332e3400 5f5a5453 GLIBCXX_3.4._ZTS
+  0x00006160 464e3261 74365465 6e736f72 4553305f FN2at6TensorES0_
+  0x00006170 53305f45 00507954 75706c65 5f476574 S0_E.PyTuple_Get
+  0x00006180 4974656d 005f5a4e 53743135 5f5f6578 Item._ZNSt15__ex
+  0x00006190 63657074 696f6e5f 7074726e 6545524b ception_ptrneERK
+  0x000061a0 4e535f31 33657863 65707469 6f6e5f70 NS_13exception_p
+  0x000061b0 74724553 325f4043 58584142 495f312e trES2_@CXXABI_1.
+  0x000061c0 332e3300 5f5a4e37 746f7263 68616f32 3.3._ZN7torchao2
+  0x000061d0 38776569 6768745f 6d617472 69785f70 8weight_matrix_p
+  0x000061e0 72657061 636b696e 675f6370 75454e32 repacking_cpuEN2
+  0x000061f0 61743654 656e736f 7245005f 50794f62 at6TensorE._PyOb
+  0x00006200 6a656374 5f476574 44696374 50747200 ject_GetDictPtr.
+  0x00006210 5f5a4e4b 32617436 54656e73 6f723569 _ZNK2at6Tensor5i
+  0x00006220 6e646578 45537431 36696e69 7469616c ndexESt16initial
+  0x00006230 697a6572 5f6c6973 74494e53 5f38696e izer_listINS_8in
+  0x00006240 64657869 6e673131 54656e73 6f72496e dexing11TensorIn
+  0x00006250 64657845 45005f5f 6378615f 61746578 dexEE.__cxa_atex
+  0x00006260 69744047 4c494243 5f322e32 2e35005f it@GLIBC_2.2.5._
+  0x00006270 5a54564e 33633130 31344f70 65726174 ZTVN3c1014Operat
+  0x00006280 6f724b65 726e656c 45005f5a 4e4b3261 orKernelE._ZNK2a
+  0x00006290 74313054 656e736f 72426173 65386461 t10TensorBase8da
+  0x000062a0 74615f70 7472496c 45455054 5f760050 ta_ptrIlEEPT_v.P
+  0x000062b0 79547570 6c655f53 65744974 656d005f yTuple_SetItem._
+  0x000062c0 5a313751 55414e54 5f47454d 4d5f4b65 Z17QUANT_GEMM_Ke
+  0x000062d0 726e656c 49313254 696c696e 67436f6e rnelI12TilingCon
+  0x000062e0 66696749 4c693445 4c693145 4c693845 figILi4ELi1ELi8E
+  0x000062f0 45664576 504b3575 696e7434 504b365f EfEvPK5uint4PK6_
+  0x00006300 5f68616c 6653375f 5054305f 6d6d6d69 _halfS7_PT0_mmmi
+  0x00006310 00507954 68726561 645f7473 735f6765 .PyThread_tss_ge
+  0x00006320 74005079 4572725f 52657374 6f726500 t.PyErr_Restore.
+  0x00006330 5f5a3239 77656967 68745f70 72657061 _Z29weight_prepa
+  0x00006340 636b696e 675f6670 31365f74 6f5f6670 cking_fp16_to_fp
+  0x00006350 36507450 686d6d00 5f5a4e35 746f7263 6PtPhmm._ZN5torc
+  0x00006360 6835656d 70747945 4e336331 30384172 h5emptyEN3c108Ar
+  0x00006370 72617952 6566496c 45454e53 305f3133 rayRefIlEENS0_13
+  0x00006380 54656e73 6f724f70 74696f6e 73455374 TensorOptionsESt
+  0x00006390 386f7074 696f6e61 6c494e53 305f3132 8optionalINS0_12
+  0x000063a0 4d656d6f 7279466f 726d6174 4545005f MemoryFormatEE._
+  0x000063b0 5a4e3574 6f726368 374c6962 72617279 ZN5torch7Library
+  0x000063c0 44314576 005f5a4e 33633130 34637564 D1Ev._ZN3c104cud
+  0x000063d0 6134696d 706c3133 43554441 47756172 a4impl13CUDAGuar
+  0x000063e0 64496d70 6c443145 76005f5f 6378615f dImplD1Ev.__cxa_
+  0x000063f0 70757265 5f766972 7475616c 40435858 pure_virtual@CXX
+  0x00006400 4142495f 312e3300 5f5f7074 68726561 ABI_1.3.__pthrea
+  0x00006410 645f6b65 795f6372 65617465 40474c49 d_key_create@GLI
+  0x00006420 42435f32 2e322e35 005f5a4e 53743135 BC_2.2.5._ZNSt15
+  0x00006430 5f5f6578 63657074 696f6e5f 70747231 __exception_ptr1
+  0x00006440 33657863 65707469 6f6e5f70 74723473 3exception_ptr4s
+  0x00006450 77617045 5253305f 40435858 4142495f wapERS0_@CXXABI_
+  0x00006460 312e332e 33005f5a 4e336331 30313153 1.3.3._ZN3c1011S
+  0x00006470 796d4e6f 6465496d 706c3130 77726170 ymNodeImpl10wrap
+  0x00006480 5f666c6f 61744564 005f5a4e 4b336331 _floatEd._ZNK3c1
+  0x00006490 30346375 64613469 6d706c31 33435544 04cuda4impl13CUD
+  0x000064a0 41477561 7264496d 706c3672 65636f72 AGuardImpl6recor
+  0x000064b0 64455050 76524b4e 535f3653 74726561 dEPPvRKNS_6Strea
+  0x000064c0 6d45614e 535f3945 76656e74 466c6167 mEaNS_9EventFlag
+  0x000064d0 45005f5a 4e523574 6f726368 374c6962 E._ZNR5torch7Lib
+  0x000064e0 72617279 355f696d 706c4550 4b634f4e rary5_implEPKcON
+  0x000064f0 535f3131 43707046 756e6374 696f6e45 S_11CppFunctionE
+  0x00006500 4e535f31 375f5265 67697374 65724f72 NS_17_RegisterOr
+  0x00006510 56657269 66794500 5f5a5374 706c4963 VerifyE._ZStplIc
+  0x00006520 53743131 63686172 5f747261 69747349 St11char_traitsI
+  0x00006530 63455361 49634545 53624954 5f54305f cESaIcEESbIT_T0_
+  0x00006540 54315f45 504b5333 5f524b53 365f005f T1_EPKS3_RKS6_._
+  0x00006550 5a4e5373 43314552 4b536149 63454047 ZNSsC1ERKSaIcE@G
+  0x00006560 4c494243 58585f33 2e34005f 5a4e3363 LIBCXX_3.4._ZN3c
+  0x00006570 31303463 75646139 47657444 65766963 104cuda9GetDevic
+  0x00006580 65455061 005f5a4e 33633130 31346765 eEPa._ZN3c1014ge
+  0x00006590 74547970 65507472 436f7079 494e3261 tTypePtrCopyIN2a
+  0x000065a0 74365465 6e736f72 4545454e 535f3454 t6TensorEEENS_4T
+  0x000065b0 79706532 3453696e 676c6574 6f6e4f72 ype24SingletonOr
+  0x000065c0 53686172 65645479 70655074 72495333 SharedTypePtrIS3
+  0x000065d0 5f454576 005f5a4e 5373345f 52657031 _EEv._ZNSs4_Rep1
+  0x000065e0 305f4d5f 64657374 726f7945 524b5361 0_M_destroyERKSa
+  0x000065f0 49634540 474c4942 4358585f 332e3400 IcE@GLIBCXX_3.4.
+  0x00006600 5f5a4e53 7431355f 5f657863 65707469 _ZNSt15__excepti
+  0x00006610 6f6e5f70 74723133 65786365 7074696f on_ptr13exceptio
+  0x00006620 6e5f7074 72443145 76404358 58414249 n_ptrD1Ev@CXXABI
+  0x00006630 5f312e33 2e33005f 5a4e3261 74345f6f _1.3.3._ZN2at4_o
+  0x00006640 70733132 696e6465 785f7365 6c656374 ps12index_select
+  0x00006650 3463616c 6c45524b 4e535f36 54656e73 4callERKNS_6Tens
+  0x00006660 6f72456c 53345f00 50795468 72656164 orElS4_.PyThread
+  0x00006670 5f747373 5f616c6c 6f63005f 5a544953 _tss_alloc._ZTIS
+  0x00006680 7431366e 65737465 645f6578 63657074 t16nested_except
+  0x00006690 696f6e40 43585841 42495f31 2e332e35 ion@CXXABI_1.3.5
+  0x000066a0 005f5a4e 33633130 31315379 6d4e6f64 ._ZN3c1011SymNod
+  0x000066b0 65496d70 6c326c65 45524b4e 535f3133 eImpl2leERKNS_13
+  0x000066c0 696e7472 75736976 655f7074 72495330 intrusive_ptrIS0
+  0x000066d0 5f4e535f 36646574 61696c33 34696e74 _NS_6detail34int
+  0x000066e0 72757369 76655f74 61726765 745f6465 rusive_target_de
+  0x000066f0 6661756c 745f6e75 6c6c5f74 79706549 fault_null_typeI
+  0x00006700 53305f45 45454500 5f5a4e4b 33633130 S0_EEEE._ZNK3c10
+  0x00006710 34696d70 6c313656 69727475 616c4775 4impl16VirtualGu
+  0x00006720 61726449 6d706c31 34657863 68616e67 ardImpl14exchang
+  0x00006730 65446576 69636545 4e535f36 44657669 eDeviceENS_6Devi
+  0x00006740 63654500 5f5a4e4b 33633130 34696d70 ceE._ZNK3c104imp
+  0x00006750 6c313656 69727475 616c4775 61726449 l16VirtualGuardI
+  0x00006760 6d706c31 36676574 44656661 756c7453 mpl16getDefaultS
+  0x00006770 74726561 6d454e53 5f364465 76696365 treamENS_6Device
+  0x00006780 45005f5a 4e366361 66666532 38547970 E._ZN6caffe28Typ
+  0x00006790 654d6574 61323665 72726f72 5f756e73 eMeta26error_uns
+  0x000067a0 7570706f 72746564 5f747970 656d6574 upported_typemet
+  0x000067b0 61455330 5f005f5a 4e336331 30313153 aES0_._ZN3c1011S
+  0x000067c0 796d4e6f 6465496d 706c3769 735f626f ymNodeImpl7is_bo
+  0x000067d0 6f6c4576 005f5a54 49537431 3372756e olEv._ZTISt13run
+  0x000067e0 74696d65 5f657272 6f724047 4c494243 time_error@GLIBC
+  0x000067f0 58585f33 2e34005f 5a4e3363 31303134 XX_3.4._ZN3c1014
+  0x00006800 4f706572 61746f72 4b65726e 656c4431 OperatorKernelD1
+  0x00006810 45760063 75646147 65744572 726f7253 Ev.cudaGetErrorS
+  0x00006820 7472696e 67406c69 62637564 6172742e tring@libcudart.
+  0x00006830 736f2e31 32005f5a 4e537431 3372756e so.12._ZNSt13run
+  0x00006840 74696d65 5f657272 6f724331 45524b53 time_errorC1ERKS
+  0x00006850 7340474c 49424358 585f332e 34005f5a s@GLIBCXX_3.4._Z
+  0x00006860 4e326174 345f6f70 73366e61 72726f77 N2at4_ops6narrow
+  0x00006870 3463616c 6c45524b 4e535f36 54656e73 4callERKNS_6Tens
+  0x00006880 6f72456c 4e336331 30365379 6d496e74 orElN3c106SymInt
+  0x00006890 4553365f 005f5a4e 33633130 31315379 ES6_._ZN3c1011Sy
+  0x000068a0 6d4e6f64 65496d70 6c326e65 45524b4e mNodeImpl2neERKN
+  0x000068b0 535f3133 696e7472 75736976 655f7074 S_13intrusive_pt
+  0x000068c0 72495330 5f4e535f 36646574 61696c33 rIS0_NS_6detail3
+  0x000068d0 34696e74 72757369 76655f74 61726765 4intrusive_targe
+  0x000068e0 745f6465 6661756c 745f6e75 6c6c5f74 t_default_null_t
+  0x000068f0 79706549 53305f45 45454500 5f5a4e35 ypeIS0_EEEE._ZN5
+  0x00006900 746f7263 68386175 746f6772 61643133 torch8autograd13
+  0x00006910 6d616b65 5f766172 6961626c 65454e32 make_variableEN2
+  0x00006920 61743654 656e736f 72456262 005f5a4e at6TensorEbb._ZN
+  0x00006930 53743135 62617369 635f7374 72696e67 St15basic_string
+  0x00006940 62756649 63537431 31636861 725f7472 bufIcSt11char_tr
+  0x00006950 61697473 49634553 61496345 45443045 aitsIcESaIcEED0E
+  0x00006960 76005f5a 4e336331 30313556 61726961 v._ZN3c1015Varia
+  0x00006970 626c6556 65727369 6f6e3134 56657273 bleVersion14Vers
+  0x00006980 696f6e43 6f756e74 65724431 4576005f ionCounterD1Ev._
+  0x00006990 5a4e3363 31303130 56616c75 65457272 ZN3c1010ValueErr
+  0x000069a0 6f724431 4576005f 5a4e3363 31303131 orD1Ev._ZN3c1011
+  0x000069b0 53796d4e 6f646549 6d706c31 31677561 SymNodeImpl11gua
+  0x000069c0 72645f66 6c6f6174 45504b63 6c005f5a rd_floatEPKcl._Z
+  0x000069d0 5374706c 49635374 31316368 61725f74 StplIcSt11char_t
+  0x000069e0 72616974 73496345 53614963 45455362 raitsIcESaIcEESb
+  0x000069f0 49545f54 305f5431 5f454f53 365f5337 IT_T0_T1_EOS6_S7
+  0x00006a00 5f005f5a 54534e33 63313031 3153796d _._ZTSN3c1011Sym
+  0x00006a10 4e6f6465 496d706c 45005f5a 53743136 NodeImplE._ZSt16
+  0x00006a20 5f5f6f73 74726561 6d5f696e 73657274 __ostream_insert
+  0x00006a30 49635374 31316368 61725f74 72616974 IcSt11char_trait
+  0x00006a40 73496345 45525374 31336261 7369635f sIcEERSt13basic_
+  0x00006a50 6f737472 65616d49 545f5430 5f455336 ostreamIT_T0_ES6
+  0x00006a60 5f504b53 335f6c40 474c4942 4358585f _PKS3_l@GLIBCXX_
+  0x00006a70 332e342e 39005f49 544d5f72 65676973 3.4.9._ITM_regis
+  0x00006a80 74657254 4d436c6f 6e655461 626c6500 terTMCloneTable.
+  0x00006a90 50794346 756e6374 696f6e5f 54797065 PyCFunction_Type
+  0x00006aa0 005f5a4e 33633130 34696d70 6c366465 ._ZN3c104impl6de
+  0x00006ab0 7461696c 33315772 61704675 6e637469 tail31WrapFuncti
+  0x00006ac0 6f6e496e 746f5275 6e74696d 6546756e onIntoRuntimeFun
+  0x00006ad0 63746f72 5f495046 4e326174 3654656e ctor_IPFN2at6Ten
+  0x00006ae0 736f7245 53345f53 345f5334 5f6c4553 sorES4_S4_S4_lES
+  0x00006af0 345f4e53 5f346775 74733874 7970656c 4_NS_4guts8typel
+  0x00006b00 69737438 74797065 6c697374 494a5334 ist8typelistIJS4
+  0x00006b10 5f53345f 53345f6c 45454545 44324576 _S4_S4_lEEEED2Ev
+  0x00006b20 005f5a4e 53734331 45524b53 736d6d40 ._ZNSsC1ERKSsmm@
+  0x00006b30 474c4942 4358585f 332e3400 50794749 GLIBCXX_3.4.PyGI
+  0x00006b40 4c537461 74655f47 65745468 69735468 LState_GetThisTh
+  0x00006b50 72656164 53746174 65005079 42797465 readState.PyByte
+  0x00006b60 735f4173 53747269 6e67416e 6453697a s_AsStringAndSiz
+  0x00006b70 65006d65 6d636d70 40474c49 42435f32 e.memcmp@GLIBC_2
+  0x00006b80 2e322e35 005f5a4e 33633130 3133696e .2.5._ZN3c1013in
+  0x00006b90 74727573 6976655f 70747249 4e535f31 trusive_ptrINS_1
+  0x00006ba0 35566172 6961626c 65566572 73696f6e 5VariableVersion
+  0x00006bb0 31345665 7273696f 6e436f75 6e746572 14VersionCounter
+  0x00006bc0 454e535f 36646574 61696c33 34696e74 ENS_6detail34int
+  0x00006bd0 72757369 76655f74 61726765 745f6465 rusive_target_de
+  0x00006be0 6661756c 745f6e75 6c6c5f74 79706549 fault_null_typeI
+  0x00006bf0 53325f45 45453672 65736574 5f457600 S2_EEE6reset_Ev.
+  0x00006c00 5079556e 69636f64 655f4173 456e636f PyUnicode_AsEnco
+  0x00006c10 64656453 7472696e 67005f5a 4e4b5373 dedString._ZNKSs
+  0x00006c20 37636f6d 70617265 45504b63 40474c49 7compareEPKc@GLI
+  0x00006c30 42435858 5f332e34 005f5a4e 4b326174 BCXX_3.4._ZNK2at
+  0x00006c40 31305465 6e736f72 42617365 38646174 10TensorBase8dat
+  0x00006c50 615f7074 72494e33 63313034 48616c66 a_ptrIN3c104Half
+  0x00006c60 45454550 545f7600 5f5a4e33 63313031 EEEPT_v._ZN3c101
+  0x00006c70 3153796d 4e6f6465 496d706c 44324576 1SymNodeImplD2Ev
+  0x00006c80 005f5a4e 33633130 31315379 6d4e6f64 ._ZN3c1011SymNod
+  0x00006c90 65496d70 6c386861 735f6869 6e744576 eImpl8has_hintEv
+  0x00006ca0 00507954 75706c65 5f4e6577 005f5a31 .PyTuple_New._Z1
+  0x00006cb0 37515541 4e545f47 454d4d5f 4b65726e 7QUANT_GEMM_Kern
+  0x00006cc0 656c4931 3254696c 696e6743 6f6e6669 elI12TilingConfi
+  0x00006cd0 67494c69 34454c69 31454c69 32454536 gILi4ELi1ELi2EE6
+  0x00006ce0 5f5f6861 6c664576 504b3575 696e7434 __halfEvPK5uint4
+  0x00006cf0 504b5332 5f53375f 5054305f 6d6d6d69 PKS2_S7_PT0_mmmi
+  0x00006d00 005f5a4e 35746f72 63683664 65746169 ._ZN5torch6detai
+  0x00006d10 6c313654 6f726368 4c696272 61727949 l16TorchLibraryI
+  0x00006d20 6e697444 31457600 50794f62 6a656374 nitD1Ev.PyObject
+  0x00006d30 5f43616c 6c46756e 6374696f 6e4f626a _CallFunctionObj
+  0x00006d40 41726773 005f5a4e 33633130 34696d70 Args._ZN3c104imp
+  0x00006d50 6c323345 78636c75 64654469 73706174 l23ExcludeDispat
+  0x00006d60 63684b65 79477561 72644331 454e535f chKeyGuardC1ENS_
+  0x00006d70 31344469 73706174 63684b65 79536574 14DispatchKeySet
+  0x00006d80 45005f5a 4e4b3261 74313054 656e736f E._ZNK2at10Tenso
+  0x00006d90 72426173 65386461 74615f70 74724968 rBase8data_ptrIh
+  0x00006da0 45455054 5f76005f 5a4e4b53 74313962 EEPT_v._ZNKSt19b
+  0x00006db0 61645f6f 7074696f 6e616c5f 61636365 ad_optional_acce
+  0x00006dc0 73733477 68617445 76005f5a 54495374 ss4whatEv._ZTISt
+  0x00006dd0 31365f53 705f636f 756e7465 645f6261 16_Sp_counted_ba
+  0x00006de0 7365494c 4e395f5f 676e755f 63787831 seILN9__gnu_cxx1
+  0x00006df0 325f4c6f 636b5f70 6f6c6963 79453245 2_Lock_policyE2E
+  0x00006e00 45006375 64614576 656e7453 796e6368 E.cudaEventSynch
+  0x00006e10 726f6e69 7a65406c 69626375 64617274 ronize@libcudart
+  0x00006e20 2e736f2e 3132005f 5a4e3363 31303463 .so.12._ZN3c104c
+  0x00006e30 75646132 30676574 44656661 756c7443 uda20getDefaultC
+  0x00006e40 55444153 74726561 6d456100 5f5a3234 UDAStreamEa._Z24
+  0x00006e50 77656967 68745f6d 61747269 785f7072 weight_matrix_pr
+  0x00006e60 65706163 6b696e67 5069535f 6d6d005f epackingPiS_mm._
+  0x00006e70 5a4e4b33 63313031 3054656e 736f7249 ZNK3c1010TensorI
+  0x00006e80 6d706c36 64657669 63654576 005f5a4e mpl6deviceEv._ZN
+  0x00006e90 53743676 6563746f 72496253 61496245 St6vectorIbSaIbE
+  0x00006ea0 4531335f 4d5f696e 73657274 5f617578 E13_M_insert_aux
+  0x00006eb0 45537431 335f4269 745f6974 65726174 ESt13_Bit_iterat
+  0x00006ec0 6f726200 5f5a4e33 6331306c 73455253 orb._ZN3c10lsERS
+  0x00006ed0 6f4e535f 31304465 76696365 54797065 oNS_10DeviceType
+  0x00006ee0 45005f5a 54545374 31396261 7369635f E._ZTTSt19basic_
+  0x00006ef0 6f737472 696e6773 74726561 6d496353 ostringstreamIcS
+  0x00006f00 74313163 6861725f 74726169 74734963 t11char_traitsIc
+  0x00006f10 45536149 63454540 474c4942 4358585f ESaIcEE@GLIBCXX_
+  0x00006f20 332e3400 5f5a4e4b 33633130 34637564 3.4._ZNK3c104cud
+  0x00006f30 6134696d 706c3133 43554441 47756172 a4impl13CUDAGuar
+  0x00006f40 64496d70 6c313465 78636861 6e676544 dImpl14exchangeD
+  0x00006f50 65766963 65454e53 5f364465 76696365 eviceENS_6Device
+  0x00006f60 45005f5a 4e336331 30323069 6e747275 E._ZN3c1020intru
+  0x00006f70 73697665 5f707472 5f746172 67657431 sive_ptr_target1
+  0x00006f80 3772656c 65617365 5f726573 6f757263 7release_resourc
+  0x00006f90 65734576 005f5a4e 53743130 5f486173 esEv._ZNSt10_Has
+  0x00006fa0 68746162 6c654953 73537434 70616972 htableISsSt4pair
+  0x00006fb0 494b5373 50764553 61495333 5f454e53 IKSsPvESaIS3_ENS
+  0x00006fc0 74385f5f 64657461 696c3130 5f53656c t8__detail10_Sel
+  0x00006fd0 65637431 73744553 74386571 75616c5f ect1stESt8equal_
+  0x00006fe0 746f4953 73455374 34686173 68495373 toISsESt4hashISs
+  0x00006ff0 454e5335 5f31385f 4d6f645f 72616e67 ENS5_18_Mod_rang
+  0x00007000 655f6861 7368696e 67454e53 355f3230 e_hashingENS5_20
+  0x00007010 5f446566 61756c74 5f72616e 6765645f _Default_ranged_
+  0x00007020 68617368 454e5335 5f32305f 5072696d hashENS5_20_Prim
+  0x00007030 655f7265 68617368 5f706f6c 69637945 e_rehash_policyE
+  0x00007040 4e53355f 31375f48 61736874 61626c65 NS5_17_Hashtable
+  0x00007050 5f747261 69747349 4c623145 4c623045 _traitsILb1ELb0E
+  0x00007060 4c623145 45454539 5f4d5f72 65686173 Lb1EEEE9_M_rehas
+  0x00007070 68456d52 4b6d0050 79457863 5f496d70 hEmRKm.PyExc_Imp
+  0x00007080 6f727445 72726f72 005f5a4e 33633130 ortError._ZN3c10
+  0x00007090 31315379 6d4e6f64 65496d70 6c326c74 11SymNodeImpl2lt
+  0x000070a0 45524b4e 535f3133 696e7472 75736976 ERKNS_13intrusiv
+  0x000070b0 655f7074 72495330 5f4e535f 36646574 e_ptrIS0_NS_6det
+  0x000070c0 61696c33 34696e74 72757369 76655f74 ail34intrusive_t
+  0x000070d0 61726765 745f6465 6661756c 745f6e75 arget_default_nu
+  0x000070e0 6c6c5f74 79706549 53305f45 45454500 ll_typeIS0_EEEE.
+  0x000070f0 5f5a4e4b 33633130 31315379 6d4e6f64 _ZNK3c1011SymNod
+  0x00007100 65496d70 6c313369 735f6e65 73746564 eImpl13is_nested
+  0x00007110 5f696e74 4576005f 5a4e5374 31396261 _intEv._ZNSt19ba
+  0x00007120 7369635f 6f737472 696e6773 74726561 sic_ostringstrea
+  0x00007130 6d496353 74313163 6861725f 74726169 mIcSt11char_trai
+  0x00007140 74734963 45536149 63454543 31457600 tsIcESaIcEEC1Ev.
+  0x00007150 5f5a5449 4e336331 3034696d 706c3664 _ZTIN3c104impl6d
+  0x00007160 65746169 6c333157 72617046 756e6374 etail31WrapFunct
+  0x00007170 696f6e49 6e746f52 756e7469 6d654675 ionIntoRuntimeFu
+  0x00007180 6e63746f 725f4950 464e3261 74365465 nctor_IPFN2at6Te
+  0x00007190 6e736f72 4553345f 4553345f 4e535f34 nsorES4_ES4_NS_4
+  0x000071a0 67757473 38747970 656c6973 74387479 guts8typelist8ty
+  0x000071b0 70656c69 7374494a 53345f45 45454545 pelistIJS4_EEEEE
+  0x000071c0 00507945 72725f4f 63637572 72656400 .PyErr_Occurred.
+  0x000071d0 50795468 72656164 53746174 655f4465 PyThreadState_De
+  0x000071e0 6c657465 43757272 656e7400 5f5a4e33 leteCurrent._ZN3
+  0x000071f0 63313031 33696e74 72757369 76655f70 c1013intrusive_p
+  0x00007200 7472494e 535f3131 53796d4e 6f646549 trINS_11SymNodeI
+  0x00007210 6d706c45 4e535f36 64657461 696c3334 mplENS_6detail34
+  0x00007220 696e7472 75736976 655f7461 72676574 intrusive_target
+  0x00007230 5f646566 61756c74 5f6e756c 6c5f7479 _default_null_ty
+  0x00007240 70654953 315f4545 45367265 7365745f peIS1_EEE6reset_
+  0x00007250 4576005f 5a4e4b32 61743130 54656e73 Ev._ZNK2at10Tens
+  0x00007260 6f724261 73653864 6174615f 70747249 orBase8data_ptrI
+  0x00007270 69454550 545f7600 5f5a3137 5155414e iEEPT_v._Z17QUAN
+  0x00007280 545f4745 4d4d5f4b 65726e65 6c493132 T_GEMM_KernelI12
+  0x00007290 54696c69 6e67436f 6e666967 494c6934 TilingConfigILi4
+  0x000072a0 454c6931 454c6934 4545365f 5f68616c ELi1ELi4EE6__hal
+  0x000072b0 66457650 4b357569 6e743450 4b53325f fEvPK5uint4PKS2_
+  0x000072c0 53375f50 54305f6d 6d6d6900 5f5a5449 S7_PT0_mmmi._ZTI
+  0x000072d0 464e3261 74365465 6e736f72 4553305f FN2at6TensorES0_
+  0x000072e0 45006375 64614576 656e7452 65636f72 E.cudaEventRecor
+  0x000072f0 64406c69 62637564 6172742e 736f2e31 d@libcudart.so.1
+  0x00007300 32005f5a 4e336331 3034696d 706c3664 2._ZN3c104impl6d
+  0x00007310 65746169 6c333157 72617046 756e6374 etail31WrapFunct
+  0x00007320 696f6e49 6e746f52 756e7469 6d654675 ionIntoRuntimeFu
+  0x00007330 6e63746f 725f4950 464e3261 74365465 nctor_IPFN2at6Te
+  0x00007340 6e736f72 4553345f 53345f45 53345f4e nsorES4_S4_ES4_N
+  0x00007350 535f3467 75747338 74797065 6c697374 S_4guts8typelist
+  0x00007360 38747970 656c6973 74494a53 345f5334 8typelistIJS4_S4
+  0x00007370 5f454545 45443045 76005079 5765616b _EEEED0Ev.PyWeak
+  0x00007380 7265665f 4e657752 6566005f 5a4e5374 ref_NewRef._ZNSt
+  0x00007390 385f5f64 65746169 6c395f4d 61705f62 8__detail9_Map_b
+  0x000073a0 61736549 53735374 34706169 72494b53 aseISsSt4pairIKS
+  0x000073b0 73507645 53614953 345f454e 535f3130 sPvESaIS4_ENS_10
+  0x000073c0 5f53656c 65637431 73744553 74386571 _Select1stESt8eq
+  0x000073d0 75616c5f 746f4953 73455374 34686173 ual_toISsESt4has
+  0x000073e0 68495373 454e535f 31385f4d 6f645f72 hISsENS_18_Mod_r
+  0x000073f0 616e6765 5f686173 68696e67 454e535f ange_hashingENS_
+  0x00007400 32305f44 65666175 6c745f72 616e6765 20_Default_range
+  0x00007410 645f6861 7368454e 535f3230 5f507269 d_hashENS_20_Pri
+  0x00007420 6d655f72 65686173 685f706f 6c696379 me_rehash_policy
+  0x00007430 454e535f 31375f48 61736874 61626c65 ENS_17_Hashtable
+  0x00007440 5f747261 69747349 4c623145 4c623045 _traitsILb1ELb0E
+  0x00007450 4c623145 45454c62 31454569 78454f53 Lb1EEELb1EEixEOS
+  0x00007460 73005f5a 4e4b3363 31303545 72726f72 s._ZNK3c105Error
+  0x00007470 34776861 74457600 5f5a4e53 73433145 4whatEv._ZNSsC1E
+  0x00007480 504b6352 4b536149 63454047 4c494243 PKcRKSaIcE@GLIBC
+  0x00007490 58585f33 2e34005f 5a4e4b33 63313034 XX_3.4._ZNK3c104
+  0x000074a0 63756461 34696d70 6c313343 55444147 cuda4impl13CUDAG
+  0x000074b0 75617264 496d706c 31346578 6368616e uardImpl14exchan
+  0x000074c0 67655374 7265616d 454e535f 36537472 geStreamENS_6Str
+  0x000074d0 65616d45 005f5a4e 53733772 65736572 eamE._ZNSs7reser
+  0x000074e0 7665456d 40474c49 42435858 5f332e34 veEm@GLIBCXX_3.4
+  0x000074f0 00637564 6146756e 63536574 41747472 .cudaFuncSetAttr
+  0x00007500 69627574 65406c69 62637564 6172742e ibute@libcudart.
+  0x00007510 736f2e31 32005f5a 4e336331 3034696d so.12._ZN3c104im
+  0x00007520 706c3664 65746169 6c333157 72617046 pl6detail31WrapF
+  0x00007530 756e6374 696f6e49 6e746f52 756e7469 unctionIntoRunti
+  0x00007540 6d654675 6e63746f 725f4950 464e3261 meFunctor_IPFN2a
+  0x00007550 74365465 6e736f72 4553345f 4553345f t6TensorES4_ES4_
+  0x00007560 4e535f34 67757473 38747970 656c6973 NS_4guts8typelis
+  0x00007570 74387479 70656c69 7374494a 53345f45 t8typelistIJS4_E
+  0x00007580 45454544 30457600 5079556e 69636f64 EEED0Ev.PyUnicod
+  0x00007590 655f4173 55544638 53747269 6e670050 e_AsUTF8String.P
+  0x000075a0 79457661 6c5f4765 74427569 6c74696e yEval_GetBuiltin
+  0x000075b0 73005f5a 4e4b3363 31303463 75646134 s._ZNK3c104cuda4
+  0x000075c0 696d706c 31334355 44414775 61726449 impl13CUDAGuardI
+  0x000075d0 6d706c31 32646573 74726f79 4576656e mpl12destroyEven
+  0x000075e0 74455076 61005f5a 54495374 31346f76 tEPva._ZTISt14ov
+  0x000075f0 6572666c 6f775f65 72726f72 40474c49 erflow_error@GLI
+  0x00007600 42435858 5f332e34 00507945 78635f56 BCXX_3.4.PyExc_V
+  0x00007610 616c7565 4572726f 72005f5a 4e537337 alueError._ZNSs7
+  0x00007620 7265706c 61636545 6d6d504b 636d4047 replaceEmmPKcm@G
+  0x00007630 4c494243 58585f33 2e34005f 5a4e5374 LIBCXX_3.4._ZNSt
+  0x00007640 31337275 6e74696d 655f6572 726f7243 13runtime_errorC
+  0x00007650 3245524b 53734047 4c494243 58585f33 2ERKSs@GLIBCXX_3
+  0x00007660 2e34005f 5a4e3574 6f726368 336a6974 .4._ZN5torch3jit
+  0x00007670 31317061 72736553 6368656d 6145524b 11parseSchemaERK
+  0x00007680 5373005f 5a4e3363 31303477 61726e45 Ss._ZN3c104warnE
+  0x00007690 524b4e53 5f375761 726e696e 6745005f RKNS_7WarningE._
+  0x000076a0 5a4e5373 43314552 4b537340 474c4942 ZNSsC1ERKSs@GLIB
+  0x000076b0 4358585f 332e3400 6d656d63 70794047 CXX_3.4.memcpy@G
+  0x000076c0 4c494243 5f322e31 34006375 64614576 LIBC_2.14.cudaEv
+  0x000076d0 656e7443 72656174 65576974 68466c61 entCreateWithFla
+  0x000076e0 6773406c 69626375 64617274 2e736f2e gs@libcudart.so.
+  0x000076f0 3132005f 5a54494e 31305f5f 63787861 12._ZTIN10__cxxa
+  0x00007700 62697631 31355f5f 666f7263 65645f75 biv115__forced_u
+  0x00007710 6e77696e 64454043 58584142 495f312e nwindE@CXXABI_1.
+  0x00007720 332e3200 5f5a4e53 74396261 645f616c 3.2._ZNSt9bad_al
+  0x00007730 6c6f6344 31457640 474c4942 4358585f locD1Ev@GLIBCXX_
+  0x00007740 332e3400 5f5a4e33 63313034 696d706c 3.4._ZN3c104impl
+  0x00007750 36646574 61696c33 31577261 7046756e 6detail31WrapFun
+  0x00007760 6374696f 6e496e74 6f52756e 74696d65 ctionIntoRuntime
+  0x00007770 46756e63 746f725f 4950464e 32617436 Functor_IPFN2at6
+  0x00007780 54656e73 6f724552 4b53345f 53365f64 TensorERKS4_S6_d
+  0x00007790 4553345f 4e535f34 67757473 38747970 ES4_NS_4guts8typ
+  0x000077a0 656c6973 74387479 70656c69 7374494a elist8typelistIJ
+  0x000077b0 53365f53 365f6445 45454544 31457600 S6_S6_dEEEED1Ev.
+  0x000077c0 5f5a4e53 73366170 70656e64 456d6340 _ZNSs6appendEmc@
+  0x000077d0 474c4942 4358585f 332e3400 50794361 GLIBCXX_3.4.PyCa
+  0x000077e0 7073756c 655f4765 744e616d 65005f5a psule_GetName._Z
+  0x000077f0 31375155 414e545f 47454d4d 5f4b6572 17QUANT_GEMM_Ker
+  0x00007800 6e656c49 31325469 6c696e67 436f6e66 nelI12TilingConf
+  0x00007810 6967494c 6934454c 6931454c 69324545 igILi4ELi1ELi2EE
+  0x00007820 66457650 4b357569 6e743450 4b365f5f fEvPK5uint4PK6__
+  0x00007830 68616c66 53375f50 54305f6d 6d6d6900 halfS7_PT0_mmmi.
+  0x00007840 5f5a4e53 73366170 70656e64 45524b53 _ZNSs6appendERKS
+  0x00007850 736d6d40 474c4942 4358585f 332e3400 smm@GLIBCXX_3.4.
+  0x00007860 5f5a5374 31375f5f 7468726f 775f6261 _ZSt17__throw_ba
+  0x00007870 645f616c 6c6f6376 40474c49 42435858 d_allocv@GLIBCXX
+  0x00007880 5f332e34 005f5a6e 776d4047 4c494243 _3.4._Znwm@GLIBC
+  0x00007890 58585f33 2e340050 79457863 5f4f7665 XX_3.4.PyExc_Ove
+  0x000078a0 72666c6f 77457272 6f72005f 5a4e4b33 rflowError._ZNK3
+  0x000078b0 63313034 696d706c 31365669 72747561 c104impl16Virtua
+  0x000078c0 6c477561 7264496d 706c3131 656c6170 lGuardImpl11elap
+  0x000078d0 73656454 696d6545 50765332 5f61005f sedTimeEPvS2_a._
+  0x000078e0 5a4e3363 31303469 6d706c31 36566972 ZN3c104impl16Vir
+  0x000078f0 7475616c 47756172 64496d70 6c443045 tualGuardImplD0E
+  0x00007900 76005f5a 4e336331 30313153 796d4e6f v._ZN3c1011SymNo
+  0x00007910 6465496d 706c3469 6e745f45 76005f49 deImpl4int_Ev._I
+  0x00007920 544d5f64 65726567 69737465 72544d43 TM_deregisterTMC
+  0x00007930 6c6f6e65 5461626c 65005f5a 4e336331 loneTable._ZN3c1
+  0x00007940 30313446 756e6374 696f6e53 6368656d 014FunctionSchem
+  0x00007950 61443245 76005f5a 5374706c 49635374 aD2Ev._ZStplIcSt
+  0x00007960 31316368 61725f74 72616974 73496345 11char_traitsIcE
+  0x00007970 53614963 45455362 49545f54 305f5431 SaIcEESbIT_T0_T1
+  0x00007980 5f454f53 365f504b 53335f00 66726565 _EOS6_PKS3_.free
+  0x00007990 40474c49 42435f32 2e322e35 005f5a4e @GLIBC_2.2.5._ZN
+  0x000079a0 4b336331 30346375 64613469 6d706c31 K3c104cuda4impl1
+  0x000079b0 33435544 41477561 7264496d 706c3967 3CUDAGuardImpl9g
+  0x000079c0 65745374 7265616d 454e535f 36446576 etStreamENS_6Dev
+  0x000079d0 69636545 005f5a4e 33633130 31305661 iceE._ZN3c1010Va
+  0x000079e0 6c756545 72726f72 44324576 005f5a4e lueErrorD2Ev._ZN
+  0x000079f0 53743139 62617369 635f6f73 7472696e St19basic_ostrin
+  0x00007a00 67737472 65616d49 63537431 31636861 gstreamIcSt11cha
+  0x00007a10 725f7472 61697473 49634553 61496345 r_traitsIcESaIcE
+  0x00007a20 45443145 7640474c 49424358 585f332e ED1Ev@GLIBCXX_3.
+  0x00007a30 34005f5a 54565374 31356261 7369635f 4._ZTVSt15basic_
+  0x00007a40 73747269 6e676275 66496353 74313163 stringbufIcSt11c
+  0x00007a50 6861725f 74726169 74734963 45536149 har_traitsIcESaI
+  0x00007a60 63454540 474c4942 4358585f 332e3400 cEE@GLIBCXX_3.4.
+  0x00007a70 5f5f6378 615f6669 6e616c69 7a654047 __cxa_finalize@G
+  0x00007a80 4c494243 5f322e32 2e35005f 5a54534e LIBC_2.2.5._ZTSN
+  0x00007a90 33633130 34696d70 6c366465 7461696c 3c104impl6detail
+  0x00007aa0 33315772 61704675 6e637469 6f6e496e 31WrapFunctionIn
+  0x00007ab0 746f5275 6e74696d 6546756e 63746f72 toRuntimeFunctor
+  0x00007ac0 5f495046 4e326174 3654656e 736f7245 _IPFN2at6TensorE
+  0x00007ad0 524b5334 5f53365f 64455334 5f4e535f RKS4_S6_dES4_NS_
+  0x00007ae0 34677574 73387479 70656c69 73743874 4guts8typelist8t
+  0x00007af0 7970656c 69737449 4a53365f 53365f64 ypelistIJS6_S6_d
+  0x00007b00 45454545 45005f5a 4e4b3363 31303469 EEEEE._ZNK3c104i
+  0x00007b10 6d706c31 36566972 7475616c 47756172 mpl16VirtualGuar
+  0x00007b20 64496d70 6c313071 75657279 4576656e dImpl10queryEven
+  0x00007b30 74455076 00507944 6963745f 54797065 tEPv.PyDict_Type
+  0x00007b40 005f5a54 53537431 39626164 5f6f7074 ._ZTSSt19bad_opt
+  0x00007b50 696f6e61 6c5f6163 63657373 005f5a54 ional_access._ZT
+  0x00007b60 49537431 32646f6d 61696e5f 6572726f ISt12domain_erro
+  0x00007b70 7240474c 49424358 585f332e 34005f5a r@GLIBCXX_3.4._Z
+  0x00007b80 4e336331 30366465 7461696c 31325f73 N3c106detail12_s
+  0x00007b90 74725f77 72617070 6572494a 504b6352 tr_wrapperIJPKcR
+  0x00007ba0 4b694545 3463616c 6c45524b 53335f53 KiEE4callERKS3_S
+  0x00007bb0 355f005f 5a4e3363 31303664 65746169 5_._ZN3c106detai
+  0x00007bc0 6c31325f 7374725f 77726170 70657249 l12_str_wrapperI
+  0x00007bd0 4a504b63 524b6a45 45346361 6c6c4552 JPKcRKjEE4callER
+  0x00007be0 4b53335f 53355f00 5f5a4e33 63313031 KS3_S5_._ZN3c101
+  0x00007bf0 34446973 70617463 684b6579 53657443 4DispatchKeySetC
+  0x00007c00 32454e53 5f313144 69737061 7463684b 2ENS_11DispatchK
+  0x00007c10 65794500 5f5a4e33 63313034 696d706c eyE._ZN3c104impl
+  0x00007c20 36646574 61696c33 31577261 7046756e 6detail31WrapFun
+  0x00007c30 6374696f 6e496e74 6f52756e 74696d65 ctionIntoRuntime
+  0x00007c40 46756e63 746f725f 4950464e 32617436 Functor_IPFN2at6
+  0x00007c50 54656e73 6f724552 4b53345f 53365f64 TensorERKS4_S6_d
+  0x00007c60 4553345f 4e535f34 67757473 38747970 ES4_NS_4guts8typ
+  0x00007c70 656c6973 74387479 70656c69 7374494a elist8typelistIJ
+  0x00007c80 53365f53 365f6445 45454544 32457600 S6_S6_dEEEED2Ev.
+  0x00007c90 5079434d 6574686f 645f4e65 77006375 PyCMethod_New.cu
+  0x00007ca0 64614765 744c6173 74457272 6f72406c daGetLastError@l
+  0x00007cb0 69626375 64617274 2e736f2e 3132005f ibcudart.so.12._
+  0x00007cc0 5a54564e 33633130 34696d70 6c366465 ZTVN3c104impl6de
+  0x00007cd0 7461696c 33315772 61704675 6e637469 tail31WrapFuncti
+  0x00007ce0 6f6e496e 746f5275 6e74696d 6546756e onIntoRuntimeFun
+  0x00007cf0 63746f72 5f495046 4e326174 3654656e ctor_IPFN2at6Ten
+  0x00007d00 736f7245 53345f53 345f5334 5f6c4553 sorES4_S4_S4_lES
+  0x00007d10 345f4e53 5f346775 74733874 7970656c 4_NS_4guts8typel
+  0x00007d20 69737438 74797065 6c697374 494a5334 ist8typelistIJS4
+  0x00007d30 5f53345f 53345f6c 45454545 45005f5a _S4_S4_lEEEEE._Z
+  0x00007d40 4e4b3363 31303137 53796d62 6f6c6963 NK3c1017Symbolic
+  0x00007d50 53686170 654d6574 61313869 6e69745f ShapeMeta18init_
+  0x00007d60 69735f63 6f6e7469 67756f75 73457600 is_contiguousEv.
+  0x00007d70 5f5a4e33 63313031 3153796d 4e6f6465 _ZN3c1011SymNode
+  0x00007d80 496d706c 32306775 6172645f 73697a65 Impl20guard_size
+  0x00007d90 5f6f626c 6976696f 75734550 4b636c00 _obliviousEPKcl.
+  0x00007da0 5f5a4e4b 53743133 72756e74 696d655f _ZNKSt13runtime_
+  0x00007db0 6572726f 72347768 61744576 40474c49 error4whatEv@GLI
+  0x00007dc0 42435858 5f332e34 005f5f62 73735f73 BCXX_3.4.__bss_s
+  0x00007dd0 74617274 005f5a31 3653706c 69744b5f tart._Z16SplitK_
+  0x00007de0 52656475 6374696f 6e50365f 5f68616c ReductionP6__hal
+  0x00007df0 6650666d 6d690050 79457863 65707469 fPfmmi.PyExcepti
+  0x00007e00 6f6e5f53 6574436f 6e746578 74005f5a on_SetContext._Z
+  0x00007e10 4e4b3363 31303469 6d706c31 36566972 NK3c104impl16Vir
+  0x00007e20 7475616c 47756172 64496d70 6c313673 tualGuardImpl16s
+  0x00007e30 796e6368 726f6e69 7a654576 656e7445 ynchronizeEventE
+  0x00007e40 5076005f 5a4e5374 36766563 746f7249 Pv._ZNSt6vectorI
+  0x00007e50 4e336331 30384172 67756d65 6e744553 N3c108ArgumentES
+  0x00007e60 61495331 5f454544 32457600 5f5a4e33 aIS1_EED2Ev._ZN3
+  0x00007e70 63313031 3153796d 4e6f6465 496d706c c1011SymNodeImpl
+  0x00007e80 37747275 65646976 45524b4e 535f3133 7truedivERKNS_13
+  0x00007e90 696e7472 75736976 655f7074 72495330 intrusive_ptrIS0
+  0x00007ea0 5f4e535f 36646574 61696c33 34696e74 _NS_6detail34int
+  0x00007eb0 72757369 76655f74 61726765 745f6465 rusive_target_de
+  0x00007ec0 6661756c 745f6e75 6c6c5f74 79706549 fault_null_typeI
+  0x00007ed0 53305f45 45454500 5f5a5449 4e336331 S0_EEEE._ZTIN3c1
+  0x00007ee0 3034696d 706c3664 65746169 6c333157 04impl6detail31W
+  0x00007ef0 72617046 756e6374 696f6e49 6e746f52 rapFunctionIntoR
+  0x00007f00 756e7469 6d654675 6e63746f 725f4950 untimeFunctor_IP
+  0x00007f10 464e3261 74365465 6e736f72 4553345f FN2at6TensorES4_
+  0x00007f20 53345f53 345f6c45 53345f4e 535f3467 S4_S4_lES4_NS_4g
+  0x00007f30 75747338 74797065 6c697374 38747970 uts8typelist8typ
+  0x00007f40 656c6973 74494a53 345f5334 5f53345f elistIJS4_S4_S4_
+  0x00007f50 6c454545 45450050 7947494c 53746174 lEEEEE.PyGILStat
+  0x00007f60 655f456e 73757265 00507945 76616c5f e_Ensure.PyEval_
+  0x00007f70 41637175 69726554 68726561 64005079 AcquireThread.Py
+  0x00007f80 4572725f 53657453 7472696e 67005079 Err_SetString.Py
+  0x00007f90 4f626a65 63745f43 616c6c4f 626a6563 Object_CallObjec
+  0x00007fa0 74005079 54687265 61645f74 73735f73 t.PyThread_tss_s
+  0x00007fb0 6574005f 5f637861 5f64656d 616e676c et.__cxa_demangl
+  0x00007fc0 65404358 58414249 5f312e33 005f5a4e e@CXXABI_1.3._ZN
+  0x00007fd0 33633130 34637564 6134696d 706c3133 3c104cuda4impl13
+  0x00007fe0 43554441 47756172 64496d70 6c443045 CUDAGuardImplD0E
+  0x00007ff0 76005f5a 4e35746f 72636831 31437070 v._ZN5torch11Cpp
+  0x00008000 46756e63 74696f6e 44314576 005f5a4e FunctionD1Ev._ZN
+  0x00008010 32617434 5f6f7073 3135746f 5f647479 2at4_ops15to_dty
+  0x00008020 70655f6c 61796f75 74346361 6c6c4552 pe_layout4callER
+  0x00008030 4b4e535f 3654656e 736f7245 5374386f KNS_6TensorESt8o
+  0x00008040 7074696f 6e616c49 4e336331 30313053 ptionalIN3c1010S
+  0x00008050 63616c61 72547970 65454553 355f494e calarTypeEES5_IN
+  0x00008060 53365f36 4c61796f 75744545 53355f49 S6_6LayoutEES5_I
+  0x00008070 4e53365f 36446576 69636545 4553355f NS6_6DeviceEES5_
+  0x00008080 49624562 6253355f 494e5336 5f31324d IbEbbS5_INS6_12M
+  0x00008090 656d6f72 79466f72 6d617445 45005f5a emoryFormatEE._Z
+  0x000080a0 4e536f6c 73456940 474c4942 4358585f NSolsEi@GLIBCXX_
+  0x000080b0 332e3400 5f5a4e52 35746f72 6368374c 3.4._ZNR5torch7L
+  0x000080c0 69627261 7279345f 64656645 4f4e3363 ibrary4_defEON3c
+  0x000080d0 31303134 46756e63 74696f6e 53636865 1014FunctionSche
+  0x000080e0 6d614550 4e53315f 31324f70 65726174 maEPNS1_12Operat
+  0x000080f0 6f724e61 6d654552 4b537436 76656374 orNameERKSt6vect
+  0x00008100 6f72494e 32617433 54616745 53614953 orIN2at3TagESaIS
+  0x00008110 385f4545 4e535f31 375f5265 67697374 8_EENS_17_Regist
+  0x00008120 65724f72 56657269 66794500 63756461 erOrVerifyE.cuda
+  0x00008130 53747265 616d5761 69744576 656e7440 StreamWaitEvent@
+  0x00008140 6c696263 75646172 742e736f 2e313200 libcudart.so.12.
+  0x00008150 5f5a4e33 63313034 63756461 32304355 _ZN3c104cuda20CU
+  0x00008160 44414361 6368696e 67416c6c 6f636174 DACachingAllocat
+  0x00008170 6f723961 6c6c6f63 61746f72 45005f5f or9allocatorE.__
+  0x00008180 6378615f 67756172 645f6163 71756972 cxa_guard_acquir
+  0x00008190 65404358 58414249 5f312e33 005f5a54 e@CXXABI_1.3._ZT
+  0x000081a0 564e3363 31303469 6d706c36 64657461 VN3c104impl6deta
+  0x000081b0 696c3331 57726170 46756e63 74696f6e il31WrapFunction
+  0x000081c0 496e746f 52756e74 696d6546 756e6374 IntoRuntimeFunct
+  0x000081d0 6f725f49 50464e32 61743654 656e736f or_IPFN2at6Tenso
+  0x000081e0 7245524b 53345f53 365f6445 53345f4e rERKS4_S6_dES4_N
+  0x000081f0 535f3467 75747338 74797065 6c697374 S_4guts8typelist
+  0x00008200 38747970 656c6973 74494a53 365f5336 8typelistIJS6_S6
+  0x00008210 5f644545 45454500 5f5a4e33 63313034 _dEEEEE._ZN3c104
+  0x00008220 63756461 31376765 74537472 65616d46 cuda17getStreamF
+  0x00008230 726f6d50 6f6f6c45 6961005f 5a4e5374 romPoolEia._ZNSt
+  0x00008240 3136696e 76616c69 645f6172 67756d65 16invalid_argume
+  0x00008250 6e744331 45504b63 0050794f 626a6563 ntC1EPKc.PyObjec
+  0x00008260 745f4973 496e7374 616e6365 005f5a4e t_IsInstance._ZN
+  0x00008270 4b336331 30346375 64613469 6d706c31 K3c104cuda4impl1
+  0x00008280 33435544 41477561 7264496d 706c3474 3CUDAGuardImpl4t
+  0x00008290 79706545 76005f5a 4e537431 36696e76 ypeEv._ZNSt16inv
+  0x000082a0 616c6964 5f617267 756d656e 74443145 alid_argumentD1E
+  0x000082b0 7640474c 49424358 585f332e 34005f5a v@GLIBCXX_3.4._Z
+  0x000082c0 54495374 3136696e 76616c69 645f6172 TISt16invalid_ar
+  0x000082d0 67756d65 6e744047 4c494243 58585f33 gument@GLIBCXX_3
+  0x000082e0 2e34005f 5f676d6f 6e5f7374 6172745f .4.__gmon_start_
+  0x000082f0 5f005f5a 4e336331 30323141 75746f67 _._ZN3c1021Autog
+  0x00008300 7261644d 65746149 6e746572 66616365 radMetaInterface
+  0x00008310 44324576 0050794d 656d5f46 72656500 D2Ev.PyMem_Free.
+  0x00008320 50795468 72656164 53746174 655f4765 PyThreadState_Ge
+  0x00008330 74005f5a 53743137 63757272 656e745f t._ZSt17current_
+  0x00008340 65786365 7074696f 6e764043 58584142 exceptionv@CXXAB
+  0x00008350 495f312e 332e3300 5f5a4e53 6f395f4d I_1.3.3._ZNSo9_M
+  0x00008360 5f696e73 65727449 6c454552 536f545f _insertIlEERSoT_
+  0x00008370 40474c49 42435858 5f332e34 2e39005f @GLIBCXX_3.4.9._
+  0x00008380 5f637861 5f616c6c 6f636174 655f6578 _cxa_allocate_ex
+  0x00008390 63657074 696f6e40 43585841 42495f31 ception@CXXABI_1
+  0x000083a0 2e33005f 5a4e4b33 63313034 63756461 .3._ZNK3c104cuda
+  0x000083b0 34696d70 6c313343 55444147 75617264 4impl13CUDAGuard
+  0x000083c0 496d706c 31377379 6e636872 6f6e697a Impl17synchroniz
+  0x000083d0 65537472 65616d45 524b4e53 5f365374 eStreamERKNS_6St
+  0x000083e0 7265616d 45005f5a 5453464e 32617436 reamE._ZTSFN2at6
+  0x000083f0 54656e73 6f724553 305f4500 5f5a4e33 TensorES0_E._ZN3
+  0x00008400 63313036 64657461 696c3330 696e6665 c106detail30infe
+  0x00008410 7246756e 6374696f 6e536368 656d6146 rFunctionSchemaF
+  0x00008420 726f6d46 756e6374 6f724950 464e3261 romFunctorIPFN2a
+  0x00008430 74365465 6e736f72 45524b53 335f5335 t6TensorERKS3_S5
+  0x00008440 5f644545 45537431 30756e69 7175655f _dEEESt10unique_
+  0x00008450 70747249 4e535f31 3446756e 6374696f ptrINS_14Functio
+  0x00008460 6e536368 656d6145 53743134 64656661 nSchemaESt14defa
+  0x00008470 756c745f 64656c65 74654953 395f4545 ult_deleteIS9_EE
+  0x00008480 76005079 54797065 5f547970 65005f5a v.PyType_Type._Z
+  0x00008490 4e4b3363 31303469 6d706c31 36566972 NK3c104impl16Vir
+  0x000084a0 7475616c 47756172 64496d70 6c397365 tualGuardImpl9se
+  0x000084b0 74446576 69636545 4e535f36 44657669 tDeviceENS_6Devi
+  0x000084c0 63654500 5f5a4e4b 33633130 34696d70 ceE._ZNK3c104imp
+  0x000084d0 6c313656 69727475 616c4775 61726449 l16VirtualGuardI
+  0x000084e0 6d706c32 33676574 53747265 616d4672 mpl23getStreamFr
+  0x000084f0 6f6d476c 6f62616c 506f6f6c 454e535f omGlobalPoolENS_
+  0x00008500 36446576 69636545 62005f5a 4e336331 6DeviceEb._ZN3c1
+  0x00008510 30313153 796d4e6f 6465496d 706c3669 011SymNodeImpl6i
+  0x00008520 735f696e 74457600 5f5a4e33 63313031 s_intEv._ZN3c101
+  0x00008530 3153796d 4e6f6465 496d706c 336d756c 1SymNodeImpl3mul
+  0x00008540 45524b4e 535f3133 696e7472 75736976 ERKNS_13intrusiv
+  0x00008550 655f7074 72495330 5f4e535f 36646574 e_ptrIS0_NS_6det
+  0x00008560 61696c33 34696e74 72757369 76655f74 ail34intrusive_t
+  0x00008570 61726765 745f6465 6661756c 745f6e75 arget_default_nu
+  0x00008580 6c6c5f74 79706549 53305f45 45454500 ll_typeIS0_EEEE.
+  0x00008590 5f5a4e39 5f5f676e 755f6378 7831325f _ZN9__gnu_cxx12_
+  0x000085a0 5f746f5f 78737472 696e6749 53736345 _to_xstringISscE
+  0x000085b0 45545f50 46695054 305f6d50 4b53325f ET_PFiPT0_mPKS2_
+  0x000085c0 5031335f 5f76615f 6c697374 5f746167 P13__va_list_tag
+  0x000085d0 456d5335 5f7a005f 5a4e3363 31303664 EmS5_z._ZN3c106d
+  0x000085e0 65746169 6c31325f 7374725f 77726170 etail12_str_wrap
+  0x000085f0 70657249 4a524b63 524b5053 325f5334 perIJRKcRKPS2_S4
+  0x00008600 5f53365f 53345f45 45346361 6c6c4553 _S6_S4_EE4callES
+  0x00008610 335f5336 5f53365f 53365f53 365f0050 3_S6_S6_S6_S6_.P
+  0x00008620 79546872 65616453 74617465 5f4e6577 yThreadState_New
+  0x00008630 005f5a4e 4b336331 30346375 64613469 ._ZNK3c104cuda4i
+  0x00008640 6d706c31 33435544 41477561 7264496d mpl13CUDAGuardIm
+  0x00008650 706c3562 6c6f636b 45507652 4b4e535f pl5blockEPvRKNS_
+  0x00008660 36537472 65616d45 005f5a4e 4b336331 6StreamE._ZNK3c1
+  0x00008670 3034696d 706c3136 56697274 75616c47 04impl16VirtualG
+  0x00008680 75617264 496d706c 32317265 636f7264 uardImpl21record
+  0x00008690 44617461 5074724f 6e537472 65616d45 DataPtrOnStreamE
+  0x000086a0 524b4e53 5f374461 74615074 7245524b RKNS_7DataPtrERK
+  0x000086b0 4e535f36 53747265 616d4500 5f5a5456 NS_6StreamE._ZTV
+  0x000086c0 4e35746f 72636838 6175746f 67726164 N5torch8autograd
+  0x000086d0 31324175 746f6772 61644d65 74614500 12AutogradMetaE.
+  0x000086e0 5f5a4e33 63313031 3153796d 4e6f6465 _ZN3c1011SymNode
+  0x000086f0 496d706c 3133636f 6e737461 6e745f62 Impl13constant_b
+  0x00008700 6f6f6c45 76005f5a 54494e33 63313034 oolEv._ZTIN3c104
+  0x00008710 696d706c 32344465 76696365 47756172 impl24DeviceGuar
+  0x00008720 64496d70 6c496e74 65726661 63654500 dImplInterfaceE.
+  0x00008730 5f5a5456 4e336331 30323069 6e747275 _ZTVN3c1020intru
+  0x00008740 73697665 5f707472 5f746172 67657445 sive_ptr_targetE
+  0x00008750 0050794f 626a6563 745f5265 7072005f .PyObject_Repr._
+  0x00008760 5a4e3363 31303131 53796d4e 6f646549 ZN3c1011SymNodeI
+  0x00008770 6d706c31 306e6573 7465645f 696e7445 mpl10nested_intE
+  0x00008780 76005079 50726f70 65727479 5f547970 v.PyProperty_Typ
+  0x00008790 65005f5a 4e537431 39626164 5f6f7074 e._ZNSt19bad_opt
+  0x000087a0 696f6e61 6c5f6163 63657373 44314576 ional_accessD1Ev
+  0x000087b0 00507946 72616d65 5f476574 4c696e65 .PyFrame_GetLine
+  0x000087c0 4e756d62 65720073 74726368 7240474c Number.strchr@GL
+  0x000087d0 4942435f 322e322e 35005f5a 646c5076 IBC_2.2.5._ZdlPv
+  0x000087e0 6d005079 4572725f 4e6f726d 616c697a m.PyErr_Normaliz
+  0x000087f0 65457863 65707469 6f6e0050 794f626a eException.PyObj
+  0x00008800 6563745f 436c6561 72576561 6b526566 ect_ClearWeakRef
+  0x00008810 73005079 44696374 5f4e6578 74005f5a s.PyDict_Next._Z
+  0x00008820 4e537439 62617369 635f696f 73496353 NSt9basic_iosIcS
+  0x00008830 74313163 6861725f 74726169 74734963 t11char_traitsIc
+  0x00008840 45453469 6e697445 50537431 35626173 EE4initEPSt15bas
+  0x00008850 69635f73 74726561 6d627566 49635331 ic_streambufIcS1
+  0x00008860 5f454047 4c494243 58585f33 2e34005f _E@GLIBCXX_3.4._
+  0x00008870 5a4e3363 31303133 696e7472 75736976 ZN3c1013intrusiv
+  0x00008880 655f7074 72494e53 5f313556 61726961 e_ptrINS_15Varia
+  0x00008890 626c6556 65727369 6f6e3134 56657273 bleVersion14Vers
+  0x000088a0 696f6e43 6f756e74 6572454e 535f3664 ionCounterENS_6d
+  0x000088b0 65746169 6c333469 6e747275 73697665 etail34intrusive
+  0x000088c0 5f746172 6765745f 64656661 756c745f _target_default_
+  0x000088d0 6e756c6c 5f747970 65495332 5f454545 null_typeIS2_EEE
+  0x000088e0 43324550 53325f00 5f5a5449 53743962 C2EPS2_._ZTISt9b
+  0x000088f0 61645f61 6c6c6f63 40474c49 42435858 ad_alloc@GLIBCXX
+  0x00008900 5f332e34 005f5a54 494e3363 31303135 _3.4._ZTIN3c1015
+  0x00008910 56617269 61626c65 56657273 696f6e31 VariableVersion1
+  0x00008920 34566572 73696f6e 436f756e 74657245 4VersionCounterE
+  0x00008930 005f5a4e 4b537431 35626173 69635f73 ._ZNKSt15basic_s
+  0x00008940 7472696e 67627566 49635374 31316368 tringbufIcSt11ch
+  0x00008950 61725f74 72616974 73496345 53614963 ar_traitsIcESaIc
+  0x00008960 45453373 74724576 40474c49 42435858 EE3strEv@GLIBCXX
+  0x00008970 5f332e34 005f5a54 49537431 315f4d75 _3.4._ZTISt11_Mu
+  0x00008980 7465785f 62617365 494c4e39 5f5f676e tex_baseILN9__gn
+  0x00008990 755f6378 7831325f 4c6f636b 5f706f6c u_cxx12_Lock_pol
+  0x000089a0 69637945 32454500 5f5a4e53 73395f4d icyE2EE._ZNSs9_M
+  0x000089b0 5f6d7574 61746545 6d6d6d40 474c4942 _mutateEmmm@GLIB
+  0x000089c0 4358585f 332e3400 50794361 7073756c CXX_3.4.PyCapsul
   0x000089d0 655f4765 74506f69 6e746572 005f5a4e e_GetPointer._ZN
   0x000089e0 33633130 31305465 6e736f72 496d706c 3c1010TensorImpl
   0x000089f0 31377365 745f6175 746f6772 61645f6d 17set_autograd_m
   0x00008a00 65746145 53743130 756e6971 75655f70 etaESt10unique_p
   0x00008a10 7472494e 535f3231 4175746f 67726164 trINS_21Autograd
   0x00008a20 4d657461 496e7465 72666163 65455374 MetaInterfaceESt
   0x00008a30 31346465 6661756c 745f6465 6c657465 14default_delete
```

## Comparing `torchao_nightly-2024.5.19.dist-info/LICENSE` & `torchao_nightly-2024.5.22.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `torchao_nightly-2024.5.19.dist-info/METADATA` & `torchao_nightly-2024.5.22.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchao-nightly
-Version: 2024.5.19
+Version: 2024.5.22
 Summary: Package for applying ao techniques to GPU models
 Home-page: https://github.com/pytorch-labs/ao
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: numpy
 Requires-Dist: sentencepiece
```

## Comparing `torchao_nightly-2024.5.19.dist-info/RECORD` & `torchao_nightly-2024.5.22.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-torchao/_C.cpython-39-x86_64-linux-gnu.so,sha256=L_UuK-P0Tnsq-5hEr8kR-E9yerF5spKVRFqP2eFgmiY,810656
+torchao/_C.cpython-39-x86_64-linux-gnu.so,sha256=KfLyR1XxyIROsXvE3ae-e0UVUdDlexp3qhInu-B5tCw,810656
 torchao/__init__.py,sha256=cV6Ke6Rr9WsMlnQGs6znd-25GrJewfDgfpHUtbvvGEs,426
 torchao/ops.py,sha256=xFX9XhUPDhdvc4u2wbfX-s4Li4mjAShnPMTRvX0R6ek,4792
+torchao/utils.py,sha256=d_pvMlkW6uyLO3RmMKJns2KL3s9Q2m6G0CEB6N5vZcg,860
 torchao/csrc/init.cpp,sha256=yH3sqHPiMO4t2b7lqJb4GU3zJtQtt_OrjvNm1qRSELs,74
 torchao/csrc/nms.cpp,sha256=xXR6X-w9AkhKwFuZhge3dp-cX5YI80FcUVigbzExWa4,251
 torchao/csrc/cuda/nms.cu,sha256=IhBuR-PhH1WFBtbGDSG7k5OE2lZAgKXQLtJkaNHKoUo,5554
 torchao/csrc/cuda/fp6_llm/fp6_linear.cu,sha256=qOzQyFNT2v3Z1HjtSt7LXEf0bn6hqFZ3t36Li01cTF0,9437
 torchao/csrc/cuda/fp6_llm/weight_quant.cu,sha256=UiUmoPfEY63DusvYNNIiF8fpnIaBcuo5fGnXUlHQvBs,9472
 torchao/csrc/fp6_llm/fp6_llm.cpp,sha256=8AnxiaMMeHAOer6K-hcj0SN8_3v3SNwVTCMBvnGp4NQ,479
 torchao/csrc/fp6_llm/weight_prepacking.cpp,sha256=-lyFTytvmrN__OLPDBfSUMkXnx5XnnBJPp7HRqWfclQ,9210
@@ -72,12 +73,12 @@
 torchao/sparsity/prototype/scheduler/cubic_scheduler.py,sha256=fXirWwTeIixjh4Vpvzt-4fgjyPb7awM_ixQjQhTC-2c,3873
 torchao/sparsity/prototype/scheduler/lambda_scheduler.py,sha256=fRoa4OTZuuhxwwd9VLtUti5s6e7RHfwfDyy3UB3QjbU,2018
 torchao/sparsity/prototype/sparsifier/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torchao/sparsity/prototype/sparsifier/base_sparsifier.py,sha256=JVlL80Zwjv13u802EzD3yThnnkH4L2hM8hbI6cXqplg,13762
 torchao/sparsity/prototype/sparsifier/nearly_diagonal_sparsifier.py,sha256=tAI5EFoh6JZfolesoyfDuCzSxkjqhhtISXVvWjdMEw8,2189
 torchao/sparsity/prototype/sparsifier/utils.py,sha256=tFKke04D87JFiXX0AAgvWzAAfoj0TxC03HqgZzDG0N0,4786
 torchao/sparsity/prototype/sparsifier/weight_norm_sparsifier.py,sha256=xPLtL3wyQuBShVcL1yqpJeCRPiyO9EKop4O6KMxzX9I,8853
-torchao_nightly-2024.5.19.dist-info/LICENSE,sha256=ZK-8briIL4OZEMv4DgmmN3My6-Lhe3rFAaPDzKH693s,1453
-torchao_nightly-2024.5.19.dist-info/METADATA,sha256=5Aa7OlySJUjymCbIww7dzeenkZVMtGjU2IzOeBZibQM,7128
-torchao_nightly-2024.5.19.dist-info/WHEEL,sha256=FNUt4eBsrBVn_Yc5KG3aXtKE40X3uNZrbGLNCbVxyFw,148
-torchao_nightly-2024.5.19.dist-info/top_level.txt,sha256=gGr5oEJ1W-T-QL0cRUf7RhX8HXPkJVi8DDnRwMMDZyY,8
-torchao_nightly-2024.5.19.dist-info/RECORD,,
+torchao_nightly-2024.5.22.dist-info/LICENSE,sha256=ZK-8briIL4OZEMv4DgmmN3My6-Lhe3rFAaPDzKH693s,1453
+torchao_nightly-2024.5.22.dist-info/METADATA,sha256=dgXtGi80S69tAEcO7vCHqhwyt812Oyeq_Eb2PIvFrYo,7128
+torchao_nightly-2024.5.22.dist-info/WHEEL,sha256=FNUt4eBsrBVn_Yc5KG3aXtKE40X3uNZrbGLNCbVxyFw,148
+torchao_nightly-2024.5.22.dist-info/top_level.txt,sha256=gGr5oEJ1W-T-QL0cRUf7RhX8HXPkJVi8DDnRwMMDZyY,8
+torchao_nightly-2024.5.22.dist-info/RECORD,,
```

