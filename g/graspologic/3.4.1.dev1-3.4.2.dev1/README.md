# Comparing `tmp/graspologic-3.4.1.dev1.tar.gz` & `tmp/graspologic-3.4.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graspologic-3.4.1.dev1.tar", max compression
+gzip compressed data, was "graspologic-3.4.2.dev1.tar", max compression
```

## Comparing `graspologic-3.4.1.dev1.tar` & `graspologic-3.4.2.dev1.tar`

### file list

```diff
@@ -1,163 +1,163 @@
--rw-r--r--   0        0        0     1074 2024-05-22 22:35:49.067155 graspologic-3.4.1.dev1/LICENSE.txt
--rw-r--r--   0        0        0     4240 2024-05-22 22:35:49.067155 graspologic-3.4.1.dev1/README.md
--rw-r--r--   0        0        0      605 2024-05-22 22:35:49.083155 graspologic-3.4.1.dev1/graspologic/__init__.py
--rw-r--r--   0        0        0      304 2024-05-22 22:35:49.083155 graspologic-3.4.1.dev1/graspologic/align/__init__.py
--rw-r--r--   0        0        0     4615 2024-05-22 22:35:49.083155 graspologic-3.4.1.dev1/graspologic/align/base.py
--rw-r--r--   0        0        0     4197 2024-05-22 22:35:49.083155 graspologic-3.4.1.dev1/graspologic/align/orthogonal_procrustes.py
--rw-r--r--   0        0        0    17718 2024-05-22 22:35:49.083155 graspologic-3.4.1.dev1/graspologic/align/seedless_procrustes.py
--rw-r--r--   0        0        0     3733 2024-05-22 22:35:49.083155 graspologic-3.4.1.dev1/graspologic/align/sign_flips.py
--rw-r--r--   0        0        0      328 2024-05-22 22:35:49.083155 graspologic-3.4.1.dev1/graspologic/cluster/__init__.py
--rw-r--r--   0        0        0    30149 2024-05-22 22:35:49.083155 graspologic-3.4.1.dev1/graspologic/cluster/autogmm.py
--rw-r--r--   0        0        0     2576 2024-05-22 22:35:49.087155 graspologic-3.4.1.dev1/graspologic/cluster/base.py
--rw-r--r--   0        0        0    16926 2024-05-22 22:35:49.087155 graspologic-3.4.1.dev1/graspologic/cluster/divisive_cluster.py
--rw-r--r--   0        0        0    11062 2024-05-22 22:35:49.087155 graspologic-3.4.1.dev1/graspologic/cluster/gclust.py
--rw-r--r--   0        0        0     4178 2024-05-22 22:35:49.087155 graspologic-3.4.1.dev1/graspologic/cluster/kclust.py
--rw-r--r--   0        0        0      238 2024-05-22 22:35:49.087155 graspologic-3.4.1.dev1/graspologic/datasets/__init__.py
--rw-r--r--   0        0        0     6898 2024-05-22 22:35:49.087155 graspologic-3.4.1.dev1/graspologic/datasets/base.py
--rw-r--r--   0        0        0    87769 2024-05-22 22:35:49.087155 graspologic-3.4.1.dev1/graspologic/datasets/drosophila/left_adjacency.csv
--rw-r--r--   0        0        0      418 2024-05-22 22:35:49.087155 graspologic-3.4.1.dev1/graspologic/datasets/drosophila/left_cell_labels.csv
--rw-r--r--   0        0        0    91164 2024-05-22 22:35:49.087155 graspologic-3.4.1.dev1/graspologic/datasets/drosophila/right_adjacency.csv
--rw-r--r--   0        0        0      426 2024-05-22 22:35:49.087155 graspologic-3.4.1.dev1/graspologic/datasets/drosophila/right_cell_labels.csv
--rw-r--r--   0        0        0    19847 2024-05-22 22:35:49.087155 graspologic-3.4.1.dev1/graspologic/datasets/mice/atlas.csv
--rw-r--r--   0        0        0      297 2024-05-22 22:35:49.087155 graspologic-3.4.1.dev1/graspologic/datasets/mice/blocks.csv
--rw-r--r--   0        0        0   465335 2024-05-22 22:35:49.087155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54776_ses-1_dti.edgelist
--rw-r--r--   0        0        0   417268 2024-05-22 22:35:49.091155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54777_ses-1_dti.edgelist
--rw-r--r--   0        0        0   481030 2024-05-22 22:35:49.091155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54779_ses-1_dti.edgelist
--rw-r--r--   0        0        0   513067 2024-05-22 22:35:49.095155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54781_ses-1_dti.edgelist
--rw-r--r--   0        0        0   486685 2024-05-22 22:35:49.095155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54790_ses-1_dti.edgelist
--rw-r--r--   0        0        0   502512 2024-05-22 22:35:49.099155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54793_ses-1_dti.edgelist
--rw-r--r--   0        0        0   501644 2024-05-22 22:35:49.099155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54794_ses-1_dti.edgelist
--rw-r--r--   0        0        0   490182 2024-05-22 22:35:49.103155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54797_ses-1_dti.edgelist
--rw-r--r--   0        0        0   423952 2024-05-22 22:35:49.103155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54811_ses-1_dti.edgelist
--rw-r--r--   0        0        0   410522 2024-05-22 22:35:49.107155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54813_ses-1_dti.edgelist
--rw-r--r--   0        0        0   418663 2024-05-22 22:35:49.107155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54815_ses-1_dti.edgelist
--rw-r--r--   0        0        0   426113 2024-05-22 22:35:49.111155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54817_ses-1_dti.edgelist
--rw-r--r--   0        0        0   459110 2024-05-22 22:35:49.111155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54821_ses-1_dti.edgelist
--rw-r--r--   0        0        0   456778 2024-05-22 22:35:49.115155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54823_ses-1_dti.edgelist
--rw-r--r--   0        0        0   500977 2024-05-22 22:35:49.115155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54829_ses-1_dti.edgelist
--rw-r--r--   0        0        0   429240 2024-05-22 22:35:49.115155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54831_ses-1_dti.edgelist
--rw-r--r--   0        0        0   412281 2024-05-22 22:35:49.119155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54833_ses-1_dti.edgelist
--rw-r--r--   0        0        0   486497 2024-05-22 22:35:49.119155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54835_ses-1_dti.edgelist
--rw-r--r--   0        0        0   466098 2024-05-22 22:35:49.123155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54842_ses-1_dti.edgelist
--rw-r--r--   0        0        0   469626 2024-05-22 22:35:49.123155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54847_ses-1_dti.edgelist
--rw-r--r--   0        0        0   431457 2024-05-22 22:35:49.127155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54849_ses-1_dti.edgelist
--rw-r--r--   0        0        0   408031 2024-05-22 22:35:49.127155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54851_ses-1_dti.edgelist
--rw-r--r--   0        0        0   450727 2024-05-22 22:35:49.131155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54853_ses-1_dti.edgelist
--rw-r--r--   0        0        0   343162 2024-05-22 22:35:49.131155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54855_ses-1_dti.edgelist
--rw-r--r--   0        0        0   451278 2024-05-22 22:35:49.131155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54864_ses-1_dti.edgelist
--rw-r--r--   0        0        0   496115 2024-05-22 22:35:49.135155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54866_ses-1_dti.edgelist
--rw-r--r--   0        0        0   493788 2024-05-22 22:35:49.135155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54868_ses-1_dti.edgelist
--rw-r--r--   0        0        0   481678 2024-05-22 22:35:49.139155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54870_ses-1_dti.edgelist
--rw-r--r--   0        0        0   479782 2024-05-22 22:35:49.139155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54883_ses-1_dti.edgelist
--rw-r--r--   0        0        0   416610 2024-05-22 22:35:49.143155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54885_ses-1_dti.edgelist
--rw-r--r--   0        0        0   363031 2024-05-22 22:35:49.143155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54887_ses-1_dti.edgelist
--rw-r--r--   0        0        0   474339 2024-05-22 22:35:49.147155 graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54890_ses-1_dti.edgelist
--rwxr-xr-x   0        0        0    33536 2024-05-22 22:35:49.147155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54776.csv
--rwxr-xr-x   0        0        0    33530 2024-05-22 22:35:49.147155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54777.csv
--rwxr-xr-x   0        0        0    33537 2024-05-22 22:35:49.147155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54779.csv
--rwxr-xr-x   0        0        0    33535 2024-05-22 22:35:49.147155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54781.csv
--rwxr-xr-x   0        0        0    33544 2024-05-22 22:35:49.147155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54790.csv
--rwxr-xr-x   0        0        0    33551 2024-05-22 22:35:49.147155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54793.csv
--rwxr-xr-x   0        0        0    33549 2024-05-22 22:35:49.147155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54794.csv
--rwxr-xr-x   0        0        0    33555 2024-05-22 22:35:49.147155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54797.csv
--rwxr-xr-x   0        0        0    33519 2024-05-22 22:35:49.147155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54811.csv
--rwxr-xr-x   0        0        0    33525 2024-05-22 22:35:49.147155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54813.csv
--rwxr-xr-x   0        0        0    33530 2024-05-22 22:35:49.147155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54815.csv
--rwxr-xr-x   0        0        0    33528 2024-05-22 22:35:49.147155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54817.csv
--rwxr-xr-x   0        0        0    33501 2024-05-22 22:35:49.147155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54821.csv
--rwxr-xr-x   0        0        0    33510 2024-05-22 22:35:49.147155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54823.csv
--rwxr-xr-x   0        0        0    33536 2024-05-22 22:35:49.147155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54829.csv
--rwxr-xr-x   0        0        0    33538 2024-05-22 22:35:49.147155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54831.csv
--rwxr-xr-x   0        0        0    33530 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54833.csv
--rwxr-xr-x   0        0        0    33535 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54835.csv
--rwxr-xr-x   0        0        0    33505 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54842.csv
--rwxr-xr-x   0        0        0    33508 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54847.csv
--rwxr-xr-x   0        0        0    33520 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54849.csv
--rwxr-xr-x   0        0        0    33520 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54851.csv
--rwxr-xr-x   0        0        0    33525 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54853.csv
--rwxr-xr-x   0        0        0    33527 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54855.csv
--rwxr-xr-x   0        0        0    33551 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54864.csv
--rwxr-xr-x   0        0        0    33551 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54866.csv
--rwxr-xr-x   0        0        0    33551 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54868.csv
--rwxr-xr-x   0        0        0    33552 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54870.csv
--rwxr-xr-x   0        0        0    33508 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54883.csv
--rwxr-xr-x   0        0        0    33514 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54885.csv
--rwxr-xr-x   0        0        0    33509 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54887.csv
--rwxr-xr-x   0        0        0    33496 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54890.csv
--rw-r--r--   0        0        0      684 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/datasets/mice/participants.csv
--rw-r--r--   0        0        0      699 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/embed/__init__.py
--rw-r--r--   0        0        0     6965 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/embed/ase.py
--rw-r--r--   0        0        0    17726 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/embed/base.py
--rw-r--r--   0        0        0     8276 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/embed/case.py
--rw-r--r--   0        0        0     7502 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/embed/lse.py
--rw-r--r--   0        0        0    10447 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/embed/mase.py
--rw-r--r--   0        0        0     8317 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/embed/mds.py
--rw-r--r--   0        0        0     6972 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/embed/mug2vec.py
--rw-r--r--   0        0        0    19443 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/embed/n2v.py
--rw-r--r--   0        0        0    11479 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/embed/omni.py
--rw-r--r--   0        0        0    11834 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/embed/svd.py
--rw-r--r--   0        0        0      429 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/inference/__init__.py
--rw-r--r--   0        0        0     2880 2024-05-22 22:35:49.151155 graspologic-3.4.1.dev1/graspologic/inference/binomial.py
--rw-r--r--   0        0        0     4564 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/inference/density_test.py
--rw-r--r--   0        0        0    20564 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/inference/group_connection_test.py
--rw-r--r--   0        0        0    20135 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/inference/latent_distribution_test.py
--rw-r--r--   0        0        0     9837 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/inference/latent_position_test.py
--rw-r--r--   0        0        0     2392 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/inference/utils.py
--rw-r--r--   0        0        0      428 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/layouts/__init__.py
--rw-r--r--   0        0        0    10697 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/layouts/__main__.py
--rw-r--r--   0        0        0    16074 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/layouts/auto.py
--rw-r--r--   0        0        0      345 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/layouts/classes.py
--rw-r--r--   0        0        0     6025 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/layouts/colors.py
--rw-r--r--   0        0        0    28486 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/layouts/include/colors-100.json
--rw-r--r--   0        0        0      174 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/layouts/nooverlap/__init__.py
--rw-r--r--   0        0        0     7029 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/layouts/nooverlap/_grid.py
--rw-r--r--   0        0        0      860 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/layouts/nooverlap/_node.py
--rw-r--r--   0        0        0    42453 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/layouts/nooverlap/_quad_node.py
--rw-r--r--   0        0        0     2171 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/layouts/nooverlap/_quad_tree.py
--rw-r--r--   0        0        0      964 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/layouts/nooverlap/nooverlap.py
--rw-r--r--   0        0        0    10077 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/layouts/render.py
--rw-r--r--   0        0        0      152 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/match/__init__.py
--rw-r--r--   0        0        0    26991 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/match/solver.py
--rw-r--r--   0        0        0      840 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/match/types.py
--rw-r--r--   0        0        0    14080 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/match/wrappers.py
--rw-r--r--   0        0        0      459 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/models/__init__.py
--rw-r--r--   0        0        0     7322 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/models/base.py
--rw-r--r--   0        0        0     7136 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/models/edge_swaps.py
--rw-r--r--   0        0        0     5488 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/models/er.py
--rw-r--r--   0        0        0     5906 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/models/rdpg.py
--rw-r--r--   0        0        0    19673 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/models/sbm_estimators.py
--rw-r--r--   0        0        0    16934 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/nominate/VNviaSGM.py
--rw-r--r--   0        0        0      234 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/nominate/__init__.py
--rw-r--r--   0        0        0    10972 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/nominate/spectralVN.py
--rw-r--r--   0        0        0      419 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/partition/__init__.py
--rw-r--r--   0        0        0    25165 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/partition/leiden.py
--rw-r--r--   0        0        0     5311 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/partition/modularity.py
--rw-r--r--   0        0        0     1091 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/pipeline/__init__.py
--rw-r--r--   0        0        0      744 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/pipeline/embed/__init__.py
--rw-r--r--   0        0        0     2318 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/pipeline/embed/_elbow.py
--rw-r--r--   0        0        0       91 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/pipeline/embed/_types.py
--rw-r--r--   0        0        0     9212 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/pipeline/embed/adjacency_spectral_embedding.py
--rw-r--r--   0        0        0     4269 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/pipeline/embed/embeddings.py
--rw-r--r--   0        0        0     9918 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/pipeline/embed/laplacian_spectral_embedding.py
--rw-r--r--   0        0        0    12796 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/pipeline/embed/omnibus_embedding.py
--rw-r--r--   0        0        0     4045 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/pipeline/graph_builder.py
--rw-r--r--   0        0        0      528 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/plot/__init__.py
--rw-r--r--   0        0        0    64195 2024-05-22 22:35:49.155155 graspologic-3.4.1.dev1/graspologic/plot/plot.py
--rw-r--r--   0        0        0    34806 2024-05-22 22:35:49.159155 graspologic-3.4.1.dev1/graspologic/plot/plot_matrix.py
--rw-r--r--   0        0        0     3456 2024-05-22 22:35:49.159155 graspologic-3.4.1.dev1/graspologic/preconditions.py
--rw-r--r--   0        0        0      604 2024-05-22 22:35:49.159155 graspologic-3.4.1.dev1/graspologic/preprocessing/__init__.py
--rw-r--r--   0        0        0    16315 2024-05-22 22:35:49.159155 graspologic-3.4.1.dev1/graspologic/preprocessing/graph_cuts.py
--rw-r--r--   0        0        0        0 2024-05-22 22:35:49.159155 graspologic-3.4.1.dev1/graspologic/py.typed
--rw-r--r--   0        0        0      482 2024-05-22 22:35:49.159155 graspologic-3.4.1.dev1/graspologic/simulations/__init__.py
--rw-r--r--   0        0        0     4904 2024-05-22 22:35:49.159155 graspologic-3.4.1.dev1/graspologic/simulations/rdpg_corr.py
--rw-r--r--   0        0        0    38533 2024-05-22 22:35:49.159155 graspologic-3.4.1.dev1/graspologic/simulations/simulations.py
--rw-r--r--   0        0        0    10269 2024-05-22 22:35:49.159155 graspologic-3.4.1.dev1/graspologic/simulations/simulations_corr.py
--rw-r--r--   0        0        0      153 2024-05-22 22:35:49.159155 graspologic-3.4.1.dev1/graspologic/subgraph/__init__.py
--rw-r--r--   0        0        0     8470 2024-05-22 22:35:49.159155 graspologic-3.4.1.dev1/graspologic/subgraph/sg.py
--rw-r--r--   0        0        0     1781 2024-05-22 22:35:49.159155 graspologic-3.4.1.dev1/graspologic/types.py
--rw-r--r--   0        0        0     1195 2024-05-22 22:35:49.159155 graspologic-3.4.1.dev1/graspologic/utils/__init__.py
--rw-r--r--   0        0        0     4201 2024-05-22 22:35:49.159155 graspologic-3.4.1.dev1/graspologic/utils/ptr.py
--rw-r--r--   0        0        0    40441 2024-05-22 22:35:49.159155 graspologic-3.4.1.dev1/graspologic/utils/utils.py
--rw-r--r--   0        0        0      168 2024-05-22 22:36:17.807145 graspologic-3.4.1.dev1/graspologic/version.py
--rw-r--r--   0        0        0     4668 2024-05-22 22:36:17.803146 graspologic-3.4.1.dev1/pyproject.toml
--rw-r--r--   0        0        0     5779 1970-01-01 00:00:00.000000 graspologic-3.4.1.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-22 23:52:43.786774 graspologic-3.4.2.dev1/LICENSE.txt
+-rw-r--r--   0        0        0     4240 2024-05-22 23:52:43.786774 graspologic-3.4.2.dev1/README.md
+-rw-r--r--   0        0        0      605 2024-05-22 23:52:43.806774 graspologic-3.4.2.dev1/graspologic/__init__.py
+-rw-r--r--   0        0        0      304 2024-05-22 23:52:43.806774 graspologic-3.4.2.dev1/graspologic/align/__init__.py
+-rw-r--r--   0        0        0     4615 2024-05-22 23:52:43.806774 graspologic-3.4.2.dev1/graspologic/align/base.py
+-rw-r--r--   0        0        0     4197 2024-05-22 23:52:43.806774 graspologic-3.4.2.dev1/graspologic/align/orthogonal_procrustes.py
+-rw-r--r--   0        0        0    17718 2024-05-22 23:52:43.806774 graspologic-3.4.2.dev1/graspologic/align/seedless_procrustes.py
+-rw-r--r--   0        0        0     3733 2024-05-22 23:52:43.806774 graspologic-3.4.2.dev1/graspologic/align/sign_flips.py
+-rw-r--r--   0        0        0      328 2024-05-22 23:52:43.806774 graspologic-3.4.2.dev1/graspologic/cluster/__init__.py
+-rw-r--r--   0        0        0    30149 2024-05-22 23:52:43.806774 graspologic-3.4.2.dev1/graspologic/cluster/autogmm.py
+-rw-r--r--   0        0        0     2576 2024-05-22 23:52:43.806774 graspologic-3.4.2.dev1/graspologic/cluster/base.py
+-rw-r--r--   0        0        0    16926 2024-05-22 23:52:43.806774 graspologic-3.4.2.dev1/graspologic/cluster/divisive_cluster.py
+-rw-r--r--   0        0        0    11062 2024-05-22 23:52:43.806774 graspologic-3.4.2.dev1/graspologic/cluster/gclust.py
+-rw-r--r--   0        0        0     4178 2024-05-22 23:52:43.806774 graspologic-3.4.2.dev1/graspologic/cluster/kclust.py
+-rw-r--r--   0        0        0      238 2024-05-22 23:52:43.806774 graspologic-3.4.2.dev1/graspologic/datasets/__init__.py
+-rw-r--r--   0        0        0     6898 2024-05-22 23:52:43.806774 graspologic-3.4.2.dev1/graspologic/datasets/base.py
+-rw-r--r--   0        0        0    87769 2024-05-22 23:52:43.806774 graspologic-3.4.2.dev1/graspologic/datasets/drosophila/left_adjacency.csv
+-rw-r--r--   0        0        0      418 2024-05-22 23:52:43.806774 graspologic-3.4.2.dev1/graspologic/datasets/drosophila/left_cell_labels.csv
+-rw-r--r--   0        0        0    91164 2024-05-22 23:52:43.806774 graspologic-3.4.2.dev1/graspologic/datasets/drosophila/right_adjacency.csv
+-rw-r--r--   0        0        0      426 2024-05-22 23:52:43.806774 graspologic-3.4.2.dev1/graspologic/datasets/drosophila/right_cell_labels.csv
+-rw-r--r--   0        0        0    19847 2024-05-22 23:52:43.806774 graspologic-3.4.2.dev1/graspologic/datasets/mice/atlas.csv
+-rw-r--r--   0        0        0      297 2024-05-22 23:52:43.806774 graspologic-3.4.2.dev1/graspologic/datasets/mice/blocks.csv
+-rw-r--r--   0        0        0   465335 2024-05-22 23:52:43.806774 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54776_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   417268 2024-05-22 23:52:43.810774 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54777_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   481030 2024-05-22 23:52:43.810774 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54779_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   513067 2024-05-22 23:52:43.814774 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54781_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   486685 2024-05-22 23:52:43.814774 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54790_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   502512 2024-05-22 23:52:43.818775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54793_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   501644 2024-05-22 23:52:43.818775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54794_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   490182 2024-05-22 23:52:43.822775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54797_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   423952 2024-05-22 23:52:43.822775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54811_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   410522 2024-05-22 23:52:43.826774 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54813_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   418663 2024-05-22 23:52:43.826774 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54815_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   426113 2024-05-22 23:52:43.830775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54817_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   459110 2024-05-22 23:52:43.830775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54821_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   456778 2024-05-22 23:52:43.834775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54823_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   500977 2024-05-22 23:52:43.834775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54829_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   429240 2024-05-22 23:52:43.838775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54831_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   412281 2024-05-22 23:52:43.838775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54833_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   486497 2024-05-22 23:52:43.838775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54835_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   466098 2024-05-22 23:52:43.842775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54842_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   469626 2024-05-22 23:52:43.842775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54847_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   431457 2024-05-22 23:52:43.846775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54849_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   408031 2024-05-22 23:52:43.846775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54851_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   450727 2024-05-22 23:52:43.850775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54853_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   343162 2024-05-22 23:52:43.850775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54855_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   451278 2024-05-22 23:52:43.854775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54864_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   496115 2024-05-22 23:52:43.854775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54866_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   493788 2024-05-22 23:52:43.858775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54868_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   481678 2024-05-22 23:52:43.858775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54870_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   479782 2024-05-22 23:52:43.858775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54883_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   416610 2024-05-22 23:52:43.862775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54885_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   363031 2024-05-22 23:52:43.862775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54887_ses-1_dti.edgelist
+-rw-r--r--   0        0        0   474339 2024-05-22 23:52:43.866775 graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54890_ses-1_dti.edgelist
+-rwxr-xr-x   0        0        0    33536 2024-05-22 23:52:43.866775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54776.csv
+-rwxr-xr-x   0        0        0    33530 2024-05-22 23:52:43.866775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54777.csv
+-rwxr-xr-x   0        0        0    33537 2024-05-22 23:52:43.866775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54779.csv
+-rwxr-xr-x   0        0        0    33535 2024-05-22 23:52:43.866775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54781.csv
+-rwxr-xr-x   0        0        0    33544 2024-05-22 23:52:43.866775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54790.csv
+-rwxr-xr-x   0        0        0    33551 2024-05-22 23:52:43.866775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54793.csv
+-rwxr-xr-x   0        0        0    33549 2024-05-22 23:52:43.866775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54794.csv
+-rwxr-xr-x   0        0        0    33555 2024-05-22 23:52:43.866775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54797.csv
+-rwxr-xr-x   0        0        0    33519 2024-05-22 23:52:43.866775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54811.csv
+-rwxr-xr-x   0        0        0    33525 2024-05-22 23:52:43.866775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54813.csv
+-rwxr-xr-x   0        0        0    33530 2024-05-22 23:52:43.866775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54815.csv
+-rwxr-xr-x   0        0        0    33528 2024-05-22 23:52:43.866775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54817.csv
+-rwxr-xr-x   0        0        0    33501 2024-05-22 23:52:43.866775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54821.csv
+-rwxr-xr-x   0        0        0    33510 2024-05-22 23:52:43.866775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54823.csv
+-rwxr-xr-x   0        0        0    33536 2024-05-22 23:52:43.866775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54829.csv
+-rwxr-xr-x   0        0        0    33538 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54831.csv
+-rwxr-xr-x   0        0        0    33530 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54833.csv
+-rwxr-xr-x   0        0        0    33535 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54835.csv
+-rwxr-xr-x   0        0        0    33505 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54842.csv
+-rwxr-xr-x   0        0        0    33508 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54847.csv
+-rwxr-xr-x   0        0        0    33520 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54849.csv
+-rwxr-xr-x   0        0        0    33520 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54851.csv
+-rwxr-xr-x   0        0        0    33525 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54853.csv
+-rwxr-xr-x   0        0        0    33527 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54855.csv
+-rwxr-xr-x   0        0        0    33551 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54864.csv
+-rwxr-xr-x   0        0        0    33551 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54866.csv
+-rwxr-xr-x   0        0        0    33551 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54868.csv
+-rwxr-xr-x   0        0        0    33552 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54870.csv
+-rwxr-xr-x   0        0        0    33508 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54883.csv
+-rwxr-xr-x   0        0        0    33514 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54885.csv
+-rwxr-xr-x   0        0        0    33509 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54887.csv
+-rwxr-xr-x   0        0        0    33496 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54890.csv
+-rw-r--r--   0        0        0      684 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/datasets/mice/participants.csv
+-rw-r--r--   0        0        0      699 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/embed/__init__.py
+-rw-r--r--   0        0        0     6965 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/embed/ase.py
+-rw-r--r--   0        0        0    17726 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/embed/base.py
+-rw-r--r--   0        0        0     8276 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/embed/case.py
+-rw-r--r--   0        0        0     7502 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/embed/lse.py
+-rw-r--r--   0        0        0    10447 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/embed/mase.py
+-rw-r--r--   0        0        0     8317 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/embed/mds.py
+-rw-r--r--   0        0        0     6972 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/embed/mug2vec.py
+-rw-r--r--   0        0        0    19443 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/embed/n2v.py
+-rw-r--r--   0        0        0    11479 2024-05-22 23:52:43.870775 graspologic-3.4.2.dev1/graspologic/embed/omni.py
+-rw-r--r--   0        0        0    11834 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/embed/svd.py
+-rw-r--r--   0        0        0      429 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/inference/__init__.py
+-rw-r--r--   0        0        0     2880 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/inference/binomial.py
+-rw-r--r--   0        0        0     4564 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/inference/density_test.py
+-rw-r--r--   0        0        0    20564 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/inference/group_connection_test.py
+-rw-r--r--   0        0        0    20135 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/inference/latent_distribution_test.py
+-rw-r--r--   0        0        0     9837 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/inference/latent_position_test.py
+-rw-r--r--   0        0        0     2392 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/inference/utils.py
+-rw-r--r--   0        0        0      428 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/layouts/__init__.py
+-rw-r--r--   0        0        0    10697 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/layouts/__main__.py
+-rw-r--r--   0        0        0    16074 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/layouts/auto.py
+-rw-r--r--   0        0        0      345 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/layouts/classes.py
+-rw-r--r--   0        0        0     6025 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/layouts/colors.py
+-rw-r--r--   0        0        0    28486 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/layouts/include/colors-100.json
+-rw-r--r--   0        0        0      174 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/layouts/nooverlap/__init__.py
+-rw-r--r--   0        0        0     7029 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/layouts/nooverlap/_grid.py
+-rw-r--r--   0        0        0      860 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/layouts/nooverlap/_node.py
+-rw-r--r--   0        0        0    42453 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/layouts/nooverlap/_quad_node.py
+-rw-r--r--   0        0        0     2171 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/layouts/nooverlap/_quad_tree.py
+-rw-r--r--   0        0        0      964 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/layouts/nooverlap/nooverlap.py
+-rw-r--r--   0        0        0    10077 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/layouts/render.py
+-rw-r--r--   0        0        0      152 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/match/__init__.py
+-rw-r--r--   0        0        0    26991 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/match/solver.py
+-rw-r--r--   0        0        0      840 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/match/types.py
+-rw-r--r--   0        0        0    14080 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/match/wrappers.py
+-rw-r--r--   0        0        0      459 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/models/__init__.py
+-rw-r--r--   0        0        0     7322 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/models/base.py
+-rw-r--r--   0        0        0     7136 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/models/edge_swaps.py
+-rw-r--r--   0        0        0     5488 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/models/er.py
+-rw-r--r--   0        0        0     5906 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/models/rdpg.py
+-rw-r--r--   0        0        0    19673 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/models/sbm_estimators.py
+-rw-r--r--   0        0        0    16934 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/nominate/VNviaSGM.py
+-rw-r--r--   0        0        0      234 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/nominate/__init__.py
+-rw-r--r--   0        0        0    10972 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/nominate/spectralVN.py
+-rw-r--r--   0        0        0      419 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/partition/__init__.py
+-rw-r--r--   0        0        0    25165 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/partition/leiden.py
+-rw-r--r--   0        0        0     5311 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/partition/modularity.py
+-rw-r--r--   0        0        0     1091 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/pipeline/__init__.py
+-rw-r--r--   0        0        0      744 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/pipeline/embed/__init__.py
+-rw-r--r--   0        0        0     2318 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/pipeline/embed/_elbow.py
+-rw-r--r--   0        0        0       91 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/pipeline/embed/_types.py
+-rw-r--r--   0        0        0     9212 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/pipeline/embed/adjacency_spectral_embedding.py
+-rw-r--r--   0        0        0     4269 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/pipeline/embed/embeddings.py
+-rw-r--r--   0        0        0     9918 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/pipeline/embed/laplacian_spectral_embedding.py
+-rw-r--r--   0        0        0    12796 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/pipeline/embed/omnibus_embedding.py
+-rw-r--r--   0        0        0     4045 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/pipeline/graph_builder.py
+-rw-r--r--   0        0        0      528 2024-05-22 23:52:43.874775 graspologic-3.4.2.dev1/graspologic/plot/__init__.py
+-rw-r--r--   0        0        0    64195 2024-05-22 23:52:43.878775 graspologic-3.4.2.dev1/graspologic/plot/plot.py
+-rw-r--r--   0        0        0    34806 2024-05-22 23:52:43.878775 graspologic-3.4.2.dev1/graspologic/plot/plot_matrix.py
+-rw-r--r--   0        0        0     3456 2024-05-22 23:52:43.878775 graspologic-3.4.2.dev1/graspologic/preconditions.py
+-rw-r--r--   0        0        0      604 2024-05-22 23:52:43.878775 graspologic-3.4.2.dev1/graspologic/preprocessing/__init__.py
+-rw-r--r--   0        0        0    16315 2024-05-22 23:52:43.878775 graspologic-3.4.2.dev1/graspologic/preprocessing/graph_cuts.py
+-rw-r--r--   0        0        0        0 2024-05-22 23:52:43.878775 graspologic-3.4.2.dev1/graspologic/py.typed
+-rw-r--r--   0        0        0      482 2024-05-22 23:52:43.878775 graspologic-3.4.2.dev1/graspologic/simulations/__init__.py
+-rw-r--r--   0        0        0     4904 2024-05-22 23:52:43.878775 graspologic-3.4.2.dev1/graspologic/simulations/rdpg_corr.py
+-rw-r--r--   0        0        0    38533 2024-05-22 23:52:43.878775 graspologic-3.4.2.dev1/graspologic/simulations/simulations.py
+-rw-r--r--   0        0        0    10269 2024-05-22 23:52:43.878775 graspologic-3.4.2.dev1/graspologic/simulations/simulations_corr.py
+-rw-r--r--   0        0        0      153 2024-05-22 23:52:43.878775 graspologic-3.4.2.dev1/graspologic/subgraph/__init__.py
+-rw-r--r--   0        0        0     8470 2024-05-22 23:52:43.878775 graspologic-3.4.2.dev1/graspologic/subgraph/sg.py
+-rw-r--r--   0        0        0     1781 2024-05-22 23:52:43.878775 graspologic-3.4.2.dev1/graspologic/types.py
+-rw-r--r--   0        0        0     1195 2024-05-22 23:52:43.878775 graspologic-3.4.2.dev1/graspologic/utils/__init__.py
+-rw-r--r--   0        0        0     4201 2024-05-22 23:52:43.878775 graspologic-3.4.2.dev1/graspologic/utils/ptr.py
+-rw-r--r--   0        0        0    40441 2024-05-22 23:52:43.878775 graspologic-3.4.2.dev1/graspologic/utils/utils.py
+-rw-r--r--   0        0        0      168 2024-05-22 23:53:14.163151 graspologic-3.4.2.dev1/graspologic/version.py
+-rw-r--r--   0        0        0     4668 2024-05-22 23:53:14.163151 graspologic-3.4.2.dev1/pyproject.toml
+-rw-r--r--   0        0        0     5779 1970-01-01 00:00:00.000000 graspologic-3.4.2.dev1/PKG-INFO
```

### Comparing `graspologic-3.4.1.dev1/LICENSE.txt` & `graspologic-3.4.2.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/README.md` & `graspologic-3.4.2.dev1/README.md`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/__init__.py` & `graspologic-3.4.2.dev1/graspologic/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/align/base.py` & `graspologic-3.4.2.dev1/graspologic/align/base.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/align/orthogonal_procrustes.py` & `graspologic-3.4.2.dev1/graspologic/align/orthogonal_procrustes.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/align/seedless_procrustes.py` & `graspologic-3.4.2.dev1/graspologic/align/seedless_procrustes.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/align/sign_flips.py` & `graspologic-3.4.2.dev1/graspologic/align/sign_flips.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/cluster/autogmm.py` & `graspologic-3.4.2.dev1/graspologic/cluster/autogmm.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/cluster/base.py` & `graspologic-3.4.2.dev1/graspologic/cluster/base.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/cluster/divisive_cluster.py` & `graspologic-3.4.2.dev1/graspologic/cluster/divisive_cluster.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/cluster/gclust.py` & `graspologic-3.4.2.dev1/graspologic/cluster/gclust.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/cluster/kclust.py` & `graspologic-3.4.2.dev1/graspologic/cluster/kclust.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/base.py` & `graspologic-3.4.2.dev1/graspologic/datasets/base.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/drosophila/left_adjacency.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/drosophila/left_adjacency.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/drosophila/right_adjacency.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/drosophila/right_adjacency.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/atlas.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/atlas.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54776_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54776_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54777_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54777_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54779_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54779_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54781_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54781_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54790_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54790_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54793_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54793_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54794_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54794_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54797_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54797_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54811_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54811_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54813_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54813_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54815_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54815_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54817_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54817_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54821_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54821_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54823_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54823_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54829_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54829_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54831_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54831_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54833_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54833_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54835_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54835_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54842_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54842_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54847_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54847_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54849_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54849_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54851_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54851_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54853_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54853_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54855_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54855_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54864_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54864_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54866_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54866_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54868_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54868_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54870_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54870_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54883_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54883_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54885_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54885_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54887_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54887_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/edgelists/sub-54890_ses-1_dti.edgelist` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/edgelists/sub-54890_ses-1_dti.edgelist`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54776.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54776.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54777.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54777.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54779.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54779.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54781.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54781.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54790.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54790.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54793.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54793.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54794.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54794.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54797.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54797.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54811.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54811.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54813.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54813.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54815.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54815.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54817.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54817.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54821.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54821.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54823.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54823.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54829.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54829.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54831.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54831.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54833.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54833.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54835.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54835.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54842.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54842.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54847.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54847.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54849.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54849.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54851.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54851.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54853.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54853.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54855.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54855.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54864.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54864.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54866.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54866.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54868.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54868.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54870.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54870.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54883.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54883.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54885.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54885.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54887.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54887.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/features/54890.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/features/54890.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/datasets/mice/participants.csv` & `graspologic-3.4.2.dev1/graspologic/datasets/mice/participants.csv`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/embed/__init__.py` & `graspologic-3.4.2.dev1/graspologic/embed/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/embed/ase.py` & `graspologic-3.4.2.dev1/graspologic/embed/ase.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/embed/base.py` & `graspologic-3.4.2.dev1/graspologic/embed/base.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/embed/case.py` & `graspologic-3.4.2.dev1/graspologic/embed/case.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/embed/lse.py` & `graspologic-3.4.2.dev1/graspologic/embed/lse.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/embed/mase.py` & `graspologic-3.4.2.dev1/graspologic/embed/mase.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/embed/mds.py` & `graspologic-3.4.2.dev1/graspologic/embed/mds.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/embed/mug2vec.py` & `graspologic-3.4.2.dev1/graspologic/embed/mug2vec.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/embed/n2v.py` & `graspologic-3.4.2.dev1/graspologic/embed/n2v.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/embed/omni.py` & `graspologic-3.4.2.dev1/graspologic/embed/omni.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/embed/svd.py` & `graspologic-3.4.2.dev1/graspologic/embed/svd.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/inference/binomial.py` & `graspologic-3.4.2.dev1/graspologic/inference/binomial.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/inference/density_test.py` & `graspologic-3.4.2.dev1/graspologic/inference/density_test.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/inference/group_connection_test.py` & `graspologic-3.4.2.dev1/graspologic/inference/group_connection_test.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/inference/latent_distribution_test.py` & `graspologic-3.4.2.dev1/graspologic/inference/latent_distribution_test.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/inference/latent_position_test.py` & `graspologic-3.4.2.dev1/graspologic/inference/latent_position_test.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/inference/utils.py` & `graspologic-3.4.2.dev1/graspologic/inference/utils.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/layouts/__main__.py` & `graspologic-3.4.2.dev1/graspologic/layouts/__main__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/layouts/auto.py` & `graspologic-3.4.2.dev1/graspologic/layouts/auto.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/layouts/colors.py` & `graspologic-3.4.2.dev1/graspologic/layouts/colors.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/layouts/include/colors-100.json` & `graspologic-3.4.2.dev1/graspologic/layouts/include/colors-100.json`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/layouts/nooverlap/_grid.py` & `graspologic-3.4.2.dev1/graspologic/layouts/nooverlap/_grid.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/layouts/nooverlap/_node.py` & `graspologic-3.4.2.dev1/graspologic/layouts/nooverlap/_node.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/layouts/nooverlap/_quad_node.py` & `graspologic-3.4.2.dev1/graspologic/layouts/nooverlap/_quad_node.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/layouts/nooverlap/_quad_tree.py` & `graspologic-3.4.2.dev1/graspologic/layouts/nooverlap/_quad_tree.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/layouts/nooverlap/nooverlap.py` & `graspologic-3.4.2.dev1/graspologic/layouts/nooverlap/nooverlap.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/layouts/render.py` & `graspologic-3.4.2.dev1/graspologic/layouts/render.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/match/solver.py` & `graspologic-3.4.2.dev1/graspologic/match/solver.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/match/types.py` & `graspologic-3.4.2.dev1/graspologic/match/types.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/match/wrappers.py` & `graspologic-3.4.2.dev1/graspologic/match/wrappers.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/models/base.py` & `graspologic-3.4.2.dev1/graspologic/models/base.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/models/edge_swaps.py` & `graspologic-3.4.2.dev1/graspologic/models/edge_swaps.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/models/er.py` & `graspologic-3.4.2.dev1/graspologic/models/er.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/models/rdpg.py` & `graspologic-3.4.2.dev1/graspologic/models/rdpg.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/models/sbm_estimators.py` & `graspologic-3.4.2.dev1/graspologic/models/sbm_estimators.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/nominate/VNviaSGM.py` & `graspologic-3.4.2.dev1/graspologic/nominate/VNviaSGM.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/nominate/spectralVN.py` & `graspologic-3.4.2.dev1/graspologic/nominate/spectralVN.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/partition/leiden.py` & `graspologic-3.4.2.dev1/graspologic/partition/leiden.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/partition/modularity.py` & `graspologic-3.4.2.dev1/graspologic/partition/modularity.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/pipeline/__init__.py` & `graspologic-3.4.2.dev1/graspologic/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/pipeline/embed/__init__.py` & `graspologic-3.4.2.dev1/graspologic/pipeline/embed/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/pipeline/embed/_elbow.py` & `graspologic-3.4.2.dev1/graspologic/pipeline/embed/_elbow.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/pipeline/embed/adjacency_spectral_embedding.py` & `graspologic-3.4.2.dev1/graspologic/pipeline/embed/adjacency_spectral_embedding.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/pipeline/embed/embeddings.py` & `graspologic-3.4.2.dev1/graspologic/pipeline/embed/embeddings.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/pipeline/embed/laplacian_spectral_embedding.py` & `graspologic-3.4.2.dev1/graspologic/pipeline/embed/laplacian_spectral_embedding.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/pipeline/embed/omnibus_embedding.py` & `graspologic-3.4.2.dev1/graspologic/pipeline/embed/omnibus_embedding.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/pipeline/graph_builder.py` & `graspologic-3.4.2.dev1/graspologic/pipeline/graph_builder.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/plot/__init__.py` & `graspologic-3.4.2.dev1/graspologic/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/plot/plot.py` & `graspologic-3.4.2.dev1/graspologic/plot/plot.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/plot/plot_matrix.py` & `graspologic-3.4.2.dev1/graspologic/plot/plot_matrix.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/preconditions.py` & `graspologic-3.4.2.dev1/graspologic/preconditions.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/preprocessing/__init__.py` & `graspologic-3.4.2.dev1/graspologic/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/preprocessing/graph_cuts.py` & `graspologic-3.4.2.dev1/graspologic/preprocessing/graph_cuts.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/simulations/rdpg_corr.py` & `graspologic-3.4.2.dev1/graspologic/simulations/rdpg_corr.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/simulations/simulations.py` & `graspologic-3.4.2.dev1/graspologic/simulations/simulations.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/simulations/simulations_corr.py` & `graspologic-3.4.2.dev1/graspologic/simulations/simulations_corr.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/subgraph/sg.py` & `graspologic-3.4.2.dev1/graspologic/subgraph/sg.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/types.py` & `graspologic-3.4.2.dev1/graspologic/types.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/utils/__init__.py` & `graspologic-3.4.2.dev1/graspologic/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/utils/ptr.py` & `graspologic-3.4.2.dev1/graspologic/utils/ptr.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/graspologic/utils/utils.py` & `graspologic-3.4.2.dev1/graspologic/utils/utils.py`

 * *Files identical despite different names*

### Comparing `graspologic-3.4.1.dev1/pyproject.toml` & `graspologic-3.4.2.dev1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graspologic"
-version = "3.4.1.dev1"
+version = "3.4.2.dev1"
 description = "A set of Python modules for graph statistics"
 repository = "https://github.com/graspologic-org/graspologic"
 authors = [
     "Eric Bridgeford", 
     "Jaewon Chung <j1c@jhu.edu>", 
     "Benjamin Pedigo", 
     "Bijan Varjavand",
```

### Comparing `graspologic-3.4.1.dev1/PKG-INFO` & `graspologic-3.4.2.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graspologic
-Version: 3.4.1.dev1
+Version: 3.4.2.dev1
 Summary: A set of Python modules for graph statistics
 Home-page: https://github.com/graspologic-org/graspologic
 License: MIT
 Author: Eric Bridgeford
 Maintainer: Dax Pryce
 Maintainer-email: daxpryce@microsoft.com
 Requires-Python: >=3.9,<3.13
```

