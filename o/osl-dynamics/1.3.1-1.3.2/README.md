# Comparing `tmp/osl-dynamics-1.3.1.tar.gz` & `tmp/osl_dynamics-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osl-dynamics-1.3.1.tar", last modified: Fri Mar 29 13:39:09 2024, max compression
+gzip compressed data, was "osl_dynamics-1.3.2.tar", last modified: Thu May 23 07:57:49 2024, max compression
```

## Comparing `osl-dynamics-1.3.1.tar` & `osl_dynamics-1.3.2.tar`

### file list

```diff
@@ -1,194 +1,195 @@
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-03-29 13:39:09.660111 osl-dynamics-1.3.1/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5993 2024-03-29 13:39:09.659827 osl-dynamics-1.3.1/PKG-INFO
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5219 2024-03-18 16:01:33.000000 osl-dynamics-1.3.1/README.rst
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-03-29 13:39:07.045064 osl-dynamics-1.3.1/osl_dynamics/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      643 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/__init__.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-03-29 13:39:07.228065 osl-dynamics-1.3.1/osl_dynamics/analysis/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      250 2023-05-09 14:36:05.000000 osl-dynamics-1.3.1/osl_dynamics/analysis/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    31871 2024-01-25 10:42:57.000000 osl-dynamics-1.3.1/osl_dynamics/analysis/connectivity.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7178 2024-01-25 10:42:57.000000 osl-dynamics-1.3.1/osl_dynamics/analysis/fisher_kernel.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6742 2023-07-10 17:29:58.000000 osl-dynamics-1.3.1/osl_dynamics/analysis/gmm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    25231 2024-01-25 10:42:57.000000 osl-dynamics-1.3.1/osl_dynamics/analysis/modes.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    24843 2024-03-18 16:01:37.000000 osl-dynamics-1.3.1/osl_dynamics/analysis/power.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2823 2023-10-10 08:06:22.000000 osl-dynamics-1.3.1/osl_dynamics/analysis/regression.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    61220 2024-03-02 10:57:19.000000 osl-dynamics-1.3.1/osl_dynamics/analysis/spectral.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7123 2024-01-25 10:42:57.000000 osl-dynamics-1.3.1/osl_dynamics/analysis/static.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    12084 2024-02-27 08:45:34.000000 osl-dynamics-1.3.1/osl_dynamics/analysis/statistics.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    30797 2024-01-25 10:42:57.000000 osl-dynamics-1.3.1/osl_dynamics/analysis/tinda.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6502 2024-03-18 16:01:37.000000 osl-dynamics-1.3.1/osl_dynamics/analysis/workbench.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     9834 2024-01-25 10:42:57.000000 osl-dynamics-1.3.1/osl_dynamics/array_ops.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-03-29 13:39:07.235077 osl-dynamics-1.3.1/osl_dynamics/config_api/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     1979 2023-07-11 08:14:28.000000 osl-dynamics-1.3.1/osl_dynamics/config_api/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5215 2023-07-10 17:29:58.000000 osl-dynamics-1.3.1/osl_dynamics/config_api/pipeline.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    75055 2024-03-26 20:34:36.000000 osl-dynamics-1.3.1/osl_dynamics/config_api/wrappers.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-03-29 13:39:07.264362 osl-dynamics-1.3.1/osl_dynamics/data/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      501 2024-03-27 21:20:03.000000 osl-dynamics-1.3.1/osl_dynamics/data/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    54474 2024-03-27 21:20:03.000000 osl-dynamics-1.3.1/osl_dynamics/data/base.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     4839 2023-07-10 17:29:58.000000 osl-dynamics-1.3.1/osl_dynamics/data/processing.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     8842 2024-03-27 21:20:03.000000 osl-dynamics-1.3.1/osl_dynamics/data/rw.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2499 2023-07-10 17:29:58.000000 osl-dynamics-1.3.1/osl_dynamics/data/task.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    13807 2024-03-27 21:20:03.000000 osl-dynamics-1.3.1/osl_dynamics/data/tf.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-03-29 13:39:07.265649 osl-dynamics-1.3.1/osl_dynamics/files/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     1264 2024-01-04 19:06:53.000000 osl-dynamics-1.3.1/osl_dynamics/files/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      758 2023-07-11 08:14:28.000000 osl-dynamics-1.3.1/osl_dynamics/files/functions.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-03-29 13:39:07.491047 osl-dynamics-1.3.1/osl_dynamics/files/mask/
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)  3219212 2023-11-01 10:40:05.000000 osl-dynamics-1.3.1/osl_dynamics/files/mask/MNI152_T1_1mm_brain.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   414185 2023-11-01 10:40:05.000000 osl-dynamics-1.3.1/osl_dynamics/files/mask/MNI152_T1_2mm_brain.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     7241 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/mask/MNI152_T1_8mm_brain.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   724726 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/mask/ParcellationPilot.L.inflated.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   723434 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/mask/ParcellationPilot.L.midthickness.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   723505 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/mask/ParcellationPilot.L.very_inflated.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   713031 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/mask/ParcellationPilot.R.inflated.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   710727 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/mask/ParcellationPilot.R.midthickness.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   712178 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/mask/ParcellationPilot.R.very_inflated.32k_fs_LR.surf.gii
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     1707 2023-11-01 10:40:05.000000 osl-dynamics-1.3.1/osl_dynamics/files/mask/__init__.py
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)      971 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/mask/ft_8mm_brain_mask.nii.gz
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-03-29 13:39:07.598254 osl-dynamics-1.3.1/osl_dynamics/files/parcellation/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    41373 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/parcellation/Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     9131 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/parcellation/Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     1031 2024-01-04 19:06:53.000000 osl-dynamics-1.3.1/osl_dynamics/files/parcellation/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    36166 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/parcellation/aal_cortical_merged_8mm_stacked.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    23705 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/parcellation/fMRI_parcellation_ds8mm.nii.gz
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    24111 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm.nii.gz
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    33885 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm_adj.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    23705 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    63185 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    63835 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     5233 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/parcellation/giles_39_binary.nii.gz
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-03-29 13:39:07.624991 osl-dynamics-1.3.1/osl_dynamics/files/scanner/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      268 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5568 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/ctf275_channel_names.npy
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-03-29 13:39:08.564681 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6679 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/4D148.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11272 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/4D248.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    22296 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/4D248_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    42102 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/4D248_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7077 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/CTF151.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    13813 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/CTF151_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    46654 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/CTF151_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    12927 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/CTF275.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    25461 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/CTF275_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    46654 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/CTF275_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    15330 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/EEG1005.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3827 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/EEG1010.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      985 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/EEG1020.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7134 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5164 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5813 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5697 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/biosemi128.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      770 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/biosemi16.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7128 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/biosemi160.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11414 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/biosemi256.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     1470 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/biosemi32.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2860 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/biosemi64.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5110 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6161 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6696 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM1.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM1.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5581 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM10.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM10.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5833 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM11.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6367 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM11.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11302 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM14.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM14.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11794 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM15.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM15.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7800 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM16.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6362 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM16.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2643 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM17.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM17.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6873 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM20.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM20.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2547 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM22.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM22.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2985 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM23.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM23.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3165 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM24.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM24.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2016 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM25.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM25.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2906 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM3.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM3.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2989 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM7.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM7.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    15330 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/elec1005.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3827 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/elec1010.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      985 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/elec1020.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5269 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6161 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6127 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/natmeg_customized_eeg1005.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3249 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag122cmb.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5961 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag122planar.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    14973 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag306all.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2643 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5489 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag306cmb.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6873 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     4979 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag306mag.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2547 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     9969 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag306planar.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2985 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5691 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/quickcap64.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6366 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/quickcap64.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    20670 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/yokogawa440.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    19775 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/yokogawa440_old.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    14079 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/yokogawa440ag.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    20655 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/yokogawa440all.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6565 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/yokogawa440pg.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     8696 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scanner/neuromag306_channel_names.npy
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-03-29 13:39:08.566252 osl-dynamics-1.3.1/osl_dynamics/files/scene/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)       82 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scene/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)  1511998 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/files/scene/mode_scene.scene
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-03-29 13:39:08.793567 osl-dynamics-1.3.1/osl_dynamics/inference/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      160 2023-05-09 14:22:26.000000 osl-dynamics-1.3.1/osl_dynamics/inference/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     8875 2023-11-01 10:40:05.000000 osl-dynamics-1.3.1/osl_dynamics/inference/callbacks.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     8097 2023-11-01 10:40:05.000000 osl-dynamics-1.3.1/osl_dynamics/inference/initializers.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    64591 2024-03-26 20:34:36.000000 osl-dynamics-1.3.1/osl_dynamics/inference/layers.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11615 2024-01-25 10:42:57.000000 osl-dynamics-1.3.1/osl_dynamics/inference/metrics.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    23818 2024-01-25 10:42:57.000000 osl-dynamics-1.3.1/osl_dynamics/inference/modes.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2900 2024-01-04 16:19:32.000000 osl-dynamics-1.3.1/osl_dynamics/inference/optimizers.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6434 2023-07-10 17:29:58.000000 osl-dynamics-1.3.1/osl_dynamics/inference/regularizers.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     1868 2023-07-10 17:29:58.000000 osl-dynamics-1.3.1/osl_dynamics/inference/tf_ops.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-03-29 13:39:09.576473 osl-dynamics-1.3.1/osl_dynamics/models/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     1453 2024-02-01 16:47:05.000000 osl-dynamics-1.3.1/osl_dynamics/models/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    34659 2024-03-26 20:34:36.000000 osl-dynamics-1.3.1/osl_dynamics/models/dive.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    26978 2024-03-26 20:34:37.000000 osl-dynamics-1.3.1/osl_dynamics/models/dynemo.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    35658 2024-03-26 20:34:37.000000 osl-dynamics-1.3.1/osl_dynamics/models/hive.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    57840 2024-03-27 21:20:03.000000 osl-dynamics-1.3.1/osl_dynamics/models/hmm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    49953 2024-02-01 16:47:05.000000 osl-dynamics-1.3.1/osl_dynamics/models/hmm_poi.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    52035 2024-03-27 21:20:03.000000 osl-dynamics-1.3.1/osl_dynamics/models/inf_mod_base.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    28353 2024-01-25 10:42:57.000000 osl-dynamics-1.3.1/osl_dynamics/models/mage.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    25278 2024-03-02 10:56:54.000000 osl-dynamics-1.3.1/osl_dynamics/models/mdynemo.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    21245 2024-03-27 21:20:03.000000 osl-dynamics-1.3.1/osl_dynamics/models/mod_base.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    25278 2024-03-26 20:34:37.000000 osl-dynamics-1.3.1/osl_dynamics/models/obs_mod.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    22372 2024-01-25 10:42:57.000000 osl-dynamics-1.3.1/osl_dynamics/models/sage.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    14048 2023-09-16 14:06:03.000000 osl-dynamics-1.3.1/osl_dynamics/models/state_dynemo.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-03-29 13:39:09.604415 osl-dynamics-1.3.1/osl_dynamics/simulation/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      514 2024-01-25 10:42:57.000000 osl-dynamics-1.3.1/osl_dynamics/simulation/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      975 2023-07-10 17:29:58.000000 osl-dynamics-1.3.1/osl_dynamics/simulation/base.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    29087 2024-03-26 20:34:37.000000 osl-dynamics-1.3.1/osl_dynamics/simulation/hmm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    12415 2024-03-26 20:34:37.000000 osl-dynamics-1.3.1/osl_dynamics/simulation/hsmm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2969 2024-03-26 20:34:37.000000 osl-dynamics-1.3.1/osl_dynamics/simulation/mar.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    30268 2024-03-26 20:34:37.000000 osl-dynamics-1.3.1/osl_dynamics/simulation/mvn.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2362 2024-03-26 20:34:37.000000 osl-dynamics-1.3.1/osl_dynamics/simulation/poi.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    10619 2024-03-26 20:34:37.000000 osl-dynamics-1.3.1/osl_dynamics/simulation/sm.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-03-29 13:39:09.641567 osl-dynamics-1.3.1/osl_dynamics/utils/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      298 2024-03-26 20:34:37.000000 osl-dynamics-1.3.1/osl_dynamics/utils/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11314 2024-03-27 21:20:03.000000 osl-dynamics-1.3.1/osl_dynamics/utils/misc.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6700 2023-07-10 17:29:58.000000 osl-dynamics-1.3.1/osl_dynamics/utils/model.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2501 2023-07-10 17:29:58.000000 osl-dynamics-1.3.1/osl_dynamics/utils/parcellation.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    67789 2024-02-29 13:51:14.000000 osl-dynamics-1.3.1/osl_dynamics/utils/plotting.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     9146 2024-02-01 16:47:05.000000 osl-dynamics-1.3.1/osl_dynamics/utils/topoplots.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-03-29 13:39:07.144375 osl-dynamics-1.3.1/osl_dynamics.egg-info/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5993 2024-03-29 13:39:07.142609 osl-dynamics-1.3.1/osl_dynamics.egg-info/PKG-INFO
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     8316 2024-03-29 13:39:07.142966 osl-dynamics-1.3.1/osl_dynamics.egg-info/SOURCES.txt
--rw-r--r--   0 wlo995   (37469) woolrich (37107)        1 2024-03-29 13:39:07.143389 osl-dynamics-1.3.1/osl_dynamics.egg-info/dependency_links.txt
--rw-r--r--   0 wlo995   (37469) woolrich (37107)       83 2024-03-29 13:39:07.143696 osl-dynamics-1.3.1/osl_dynamics.egg-info/entry_points.txt
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      233 2024-03-29 13:39:07.144078 osl-dynamics-1.3.1/osl_dynamics.egg-info/requires.txt
--rw-r--r--   0 wlo995   (37469) woolrich (37107)       13 2024-03-29 13:39:07.144480 osl-dynamics-1.3.1/osl_dynamics.egg-info/top_level.txt
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     1264 2024-03-29 13:39:09.660970 osl-dynamics-1.3.1/setup.cfg
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)      234 2024-02-14 13:02:44.000000 osl-dynamics-1.3.1/setup.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-05-23 07:57:49.685967 osl_dynamics-1.3.2/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5591 2024-05-23 07:57:49.685752 osl_dynamics-1.3.2/PKG-INFO
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4785 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/README.rst
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-05-23 07:57:48.317359 osl_dynamics-1.3.2/osl_dynamics/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      643 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/__init__.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-05-23 07:57:48.390966 osl_dynamics-1.3.2/osl_dynamics/analysis/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      250 2023-05-09 14:36:05.000000 osl_dynamics-1.3.2/osl_dynamics/analysis/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    33403 2024-05-23 07:53:42.000000 osl_dynamics-1.3.2/osl_dynamics/analysis/connectivity.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7178 2024-01-25 10:42:57.000000 osl_dynamics-1.3.2/osl_dynamics/analysis/fisher_kernel.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6742 2023-07-10 17:29:58.000000 osl_dynamics-1.3.2/osl_dynamics/analysis/gmm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    28528 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/analysis/modes.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    26570 2024-05-23 07:53:42.000000 osl_dynamics-1.3.2/osl_dynamics/analysis/power.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2823 2023-10-10 08:06:22.000000 osl_dynamics-1.3.2/osl_dynamics/analysis/regression.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    61306 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/analysis/spectral.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7123 2024-01-25 10:42:57.000000 osl_dynamics-1.3.2/osl_dynamics/analysis/static.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    12084 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/analysis/statistics.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    30797 2024-01-25 10:42:57.000000 osl_dynamics-1.3.2/osl_dynamics/analysis/tinda.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6502 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/analysis/workbench.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     9834 2024-01-25 10:42:57.000000 osl_dynamics-1.3.2/osl_dynamics/array_ops.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-05-23 07:57:48.412584 osl_dynamics-1.3.2/osl_dynamics/config_api/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     1979 2023-07-11 08:14:28.000000 osl_dynamics-1.3.2/osl_dynamics/config_api/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5215 2023-07-10 17:29:58.000000 osl_dynamics-1.3.2/osl_dynamics/config_api/pipeline.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    75055 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/config_api/wrappers.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-05-23 07:57:48.467288 osl_dynamics-1.3.2/osl_dynamics/data/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      501 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/data/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    55105 2024-05-23 07:53:42.000000 osl_dynamics-1.3.2/osl_dynamics/data/base.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4839 2023-07-10 17:29:58.000000 osl_dynamics-1.3.2/osl_dynamics/data/processing.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     8842 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/data/rw.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2499 2023-07-10 17:29:58.000000 osl_dynamics-1.3.2/osl_dynamics/data/task.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    13807 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/data/tf.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-05-23 07:57:48.475900 osl_dynamics-1.3.2/osl_dynamics/files/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     1264 2024-01-04 19:06:53.000000 osl_dynamics-1.3.2/osl_dynamics/files/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      758 2023-07-11 08:14:28.000000 osl_dynamics-1.3.2/osl_dynamics/files/functions.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-05-23 07:57:48.650825 osl_dynamics-1.3.2/osl_dynamics/files/mask/
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)  3219212 2023-11-01 10:40:05.000000 osl_dynamics-1.3.2/osl_dynamics/files/mask/MNI152_T1_1mm_brain.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   414185 2023-11-01 10:40:05.000000 osl_dynamics-1.3.2/osl_dynamics/files/mask/MNI152_T1_2mm_brain.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     7241 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/mask/MNI152_T1_8mm_brain.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   724726 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/mask/ParcellationPilot.L.inflated.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   723434 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/mask/ParcellationPilot.L.midthickness.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   723505 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/mask/ParcellationPilot.L.very_inflated.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   713031 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/mask/ParcellationPilot.R.inflated.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   710727 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/mask/ParcellationPilot.R.midthickness.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   712178 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/mask/ParcellationPilot.R.very_inflated.32k_fs_LR.surf.gii
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     1707 2023-11-01 10:40:05.000000 osl_dynamics-1.3.2/osl_dynamics/files/mask/__init__.py
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)      971 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/mask/ft_8mm_brain_mask.nii.gz
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-05-23 07:57:48.715107 osl_dynamics-1.3.2/osl_dynamics/files/parcellation/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    41373 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/parcellation/Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     9131 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/parcellation/Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     1031 2024-01-04 19:06:53.000000 osl_dynamics-1.3.2/osl_dynamics/files/parcellation/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    36166 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/parcellation/aal_cortical_merged_8mm_stacked.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    23705 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/parcellation/fMRI_parcellation_ds8mm.nii.gz
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    24111 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm.nii.gz
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    33885 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm_adj.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    23705 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    63185 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    63835 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     5233 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/parcellation/giles_39_binary.nii.gz
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-05-23 07:57:48.727019 osl_dynamics-1.3.2/osl_dynamics/files/scanner/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      268 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5568 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/ctf275_channel_names.npy
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-05-23 07:57:49.302407 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6679 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/4D148.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11272 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/4D248.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    22296 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/4D248_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    42102 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/4D248_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7077 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/CTF151.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    13813 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/CTF151_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    46654 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/CTF151_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    12927 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/CTF275.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    25461 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/CTF275_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    46654 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/CTF275_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    15330 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/EEG1005.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3827 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/EEG1010.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      985 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/EEG1020.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7134 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5164 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5813 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5697 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/biosemi128.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      770 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/biosemi16.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7128 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/biosemi160.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11414 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/biosemi256.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     1470 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/biosemi32.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2860 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/biosemi64.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5110 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6161 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6696 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM1.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM1.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5581 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM10.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM10.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5833 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM11.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6367 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM11.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11302 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM14.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM14.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11794 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM15.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM15.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7800 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM16.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6362 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM16.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2643 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM17.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM17.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6873 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM20.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM20.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2547 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM22.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM22.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2985 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM23.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM23.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3165 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM24.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM24.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2016 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM25.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM25.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2906 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM3.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM3.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2989 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM7.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM7.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    15330 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/elec1005.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3827 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/elec1010.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      985 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/elec1020.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5269 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6161 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6127 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/natmeg_customized_eeg1005.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3249 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag122cmb.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5961 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag122planar.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    14973 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag306all.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2643 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5489 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag306cmb.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6873 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4979 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag306mag.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2547 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     9969 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag306planar.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2985 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5691 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/quickcap64.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6366 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/quickcap64.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    20670 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/yokogawa440.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    19775 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/yokogawa440_old.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    14079 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/yokogawa440ag.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    20655 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/yokogawa440all.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6565 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/yokogawa440pg.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     8696 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scanner/neuromag306_channel_names.npy
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-05-23 07:57:49.311337 osl_dynamics-1.3.2/osl_dynamics/files/scene/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)       82 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scene/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)  1511998 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/files/scene/mode_scene.scene
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-05-23 07:57:49.438464 osl_dynamics-1.3.2/osl_dynamics/inference/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      160 2023-05-09 14:22:26.000000 osl_dynamics-1.3.2/osl_dynamics/inference/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     8875 2023-11-01 10:40:05.000000 osl_dynamics-1.3.2/osl_dynamics/inference/callbacks.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     8097 2023-11-01 10:40:05.000000 osl_dynamics-1.3.2/osl_dynamics/inference/initializers.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    66185 2024-05-21 07:41:21.000000 osl_dynamics-1.3.2/osl_dynamics/inference/layers.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11615 2024-01-25 10:42:57.000000 osl_dynamics-1.3.2/osl_dynamics/inference/metrics.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    27123 2024-05-23 07:53:42.000000 osl_dynamics-1.3.2/osl_dynamics/inference/modes.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2900 2024-01-04 16:19:32.000000 osl_dynamics-1.3.2/osl_dynamics/inference/optimizers.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6434 2023-07-10 17:29:58.000000 osl_dynamics-1.3.2/osl_dynamics/inference/regularizers.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     1868 2023-07-10 17:29:58.000000 osl_dynamics-1.3.2/osl_dynamics/inference/tf_ops.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-05-23 07:57:49.587982 osl_dynamics-1.3.2/osl_dynamics/models/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     1519 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/models/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    34300 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/models/dive.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    26796 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/models/dynemo.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    35688 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/models/hive.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    58582 2024-05-23 07:53:42.000000 osl_dynamics-1.3.2/osl_dynamics/models/hmm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    17550 2024-05-21 07:09:57.000000 osl_dynamics-1.3.2/osl_dynamics/models/hmm_poi.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    58666 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/models/inf_mod_base.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    28353 2024-01-25 10:42:57.000000 osl_dynamics-1.3.2/osl_dynamics/models/mage.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    25359 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/models/mdynemo.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    21245 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/models/mod_base.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    25537 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/models/obs_mod.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    22372 2024-01-25 10:42:57.000000 osl_dynamics-1.3.2/osl_dynamics/models/sage.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     8352 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/models/simplified_dynemo.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7411 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/models/state_dynemo.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-05-23 07:57:49.623821 osl_dynamics-1.3.2/osl_dynamics/simulation/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      514 2024-01-25 10:42:57.000000 osl_dynamics-1.3.2/osl_dynamics/simulation/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      975 2023-07-10 17:29:58.000000 osl_dynamics-1.3.2/osl_dynamics/simulation/base.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    29350 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/simulation/hmm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    12415 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/simulation/hsmm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2969 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/simulation/mar.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    31188 2024-05-21 07:10:14.000000 osl_dynamics-1.3.2/osl_dynamics/simulation/mvn.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2362 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/simulation/poi.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    10619 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/simulation/sm.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-05-23 07:57:49.668886 osl_dynamics-1.3.2/osl_dynamics/utils/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      298 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/utils/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11314 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/osl_dynamics/utils/misc.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6700 2023-07-10 17:29:58.000000 osl_dynamics-1.3.2/osl_dynamics/utils/model.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2501 2023-07-10 17:29:58.000000 osl_dynamics-1.3.2/osl_dynamics/utils/parcellation.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    69779 2024-05-23 07:53:42.000000 osl_dynamics-1.3.2/osl_dynamics/utils/plotting.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     9146 2024-04-19 14:17:24.000000 osl_dynamics-1.3.2/osl_dynamics/utils/topoplots.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2024-05-23 07:57:48.334661 osl_dynamics-1.3.2/osl_dynamics.egg-info/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5591 2024-05-23 07:57:48.332743 osl_dynamics-1.3.2/osl_dynamics.egg-info/PKG-INFO
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     8357 2024-05-23 07:57:48.333124 osl_dynamics-1.3.2/osl_dynamics.egg-info/SOURCES.txt
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)        1 2024-05-23 07:57:48.333577 osl_dynamics-1.3.2/osl_dynamics.egg-info/dependency_links.txt
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)       83 2024-05-23 07:57:48.333908 osl_dynamics-1.3.2/osl_dynamics.egg-info/entry_points.txt
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      250 2024-05-23 07:57:48.334340 osl_dynamics-1.3.2/osl_dynamics.egg-info/requires.txt
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)       13 2024-05-23 07:57:48.334760 osl_dynamics-1.3.2/osl_dynamics.egg-info/top_level.txt
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     1282 2024-05-23 07:57:49.686641 osl_dynamics-1.3.2/setup.cfg
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)      234 2024-05-21 07:08:28.000000 osl_dynamics-1.3.2/setup.py
```

### Comparing `osl-dynamics-1.3.1/PKG-INFO` & `osl_dynamics-1.3.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: osl-dynamics
-Version: 1.3.1
+Version: 1.3.2
 Summary: Models for infering dynamics in neuroimaging data
 Home-page: https://github.com/OHBA-analysis/osl-dynamics
 License: MIT
 Project-URL: Documentation, https://osl-dynamics.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 Requires-Dist: glmtools~=0.2.1
 Requires-Dist: mat73~=0.62
 Requires-Dist: matplotlib~=3.7.1
 Requires-Dist: mne~=1.3.1
 Requires-Dist: nibabel~=5.1.0
 Requires-Dist: nilearn~=0.10.2
 Requires-Dist: numba==0.58
 Requires-Dist: numpy~=1.23.5
+Requires-Dist: osfclient~=0.0.5
 Requires-Dist: pandas~=1.5.3
 Requires-Dist: pyyaml~=6.0.1
 Requires-Dist: pqdm~=0.2.0
 Requires-Dist: scipy~=1.10.1
 Requires-Dist: scikit-learn~=1.3.1
 Requires-Dist: seaborn~=0.13.0
 Requires-Dist: tabulate~=0.9.0
@@ -40,38 +41,36 @@
 ============
 
 Conda
 -----
 
 We recommend installing osl-dynamics within a virtual environment. You can do this with `Anaconda <https://docs.anaconda.com/free/anaconda/install/index.html>`_ (or `miniconda <https://docs.conda.io/projects/miniconda/en/latest/miniconda-install.html>`_).
 
+Below we describe how to install osl-dynamics from source. We recommend using the conda environment files in ``/envs``.
+
 Linux
 -----
 
-Here, we describe how to install osl-dynamics from source. We recommend using the conda environment files in ``/envs``. For a generic linux machine, osl-dynamics can be installed in editable mode with:
-
 .. code-block:: shell
 
     git clone https://github.com/OHBA-analysis/osl-dynamics.git
     cd osl-dynamics
     conda env create -f envs/linux.yml
     conda activate osld
     pip install -e .
 
-Note, if you have a Mac you may want to use the ``envs/mac.yml`` environment file instead.
+Mac
+---
+
+For a Mac, the installation of TensorFlow is slightly different to a Linux computer. We recommend using the lines above replacing the Linux environment file ``envs/linux.yml`` with the Mac environment file ``envs/mac.yml``.
 
 Windows
 -------
 
-If you are using a Windows computer, we recommend first installing linux (Ubuntu) as a Windows Subsystem by following the instructions `here <https://ubuntu.com/wsl>`_. Then following the instructions above in the Ubuntu terminal.
-
-Oxford specific computers
--------------------------
-
-If you're installing on the Oxford BMRC server, use ``envs/bmrc.yml``. If you're installing on the OHBA workstation, use ``envs/hbaws.yml``. Note, the ``hbaws.yml`` environment will automatically install spyder and jupyter notebooks.
+If you are using a Windows computer, we recommend first installing Linux (Ubuntu) as a Windows Subsystem by following the instructions `here <https://ubuntu.com/wsl>`_. Then following the instructions above in the Ubuntu terminal.
 
 Within an osl environment
 -------------------------
 
 If you have already installed `OSL <https://github.com/OHBA-analysis/osl>`_ you can install osl-dynamics in the ``osl`` environment with:
 
 .. code-block:: shell
@@ -80,23 +79,23 @@
     cd osl-dynamics
     pip install tensorflow==2.9.1
     pip install tensorflow-probability==0.17
     pip install -e .
 
 Note, if you're using a Mac computer you need to install TensorFlow with ``pip install tensorflow-macos==2.9.1`` instead of ``tensorflow==2.9.1``.
 
-Developers
-----------
+Removing osl-dynamics
+---------------------
 
-Developers might want to clone the repo using SSH instead of HTTPS:
+Simply delete the conda environment and repository:
 
 .. code-block:: shell
 
-    git clone git@github.com:OHBA-analysis/osl-dynamics.git
-
+    conda env remove -n osld
+    rm -rf osl-dynamics
 
 Documentation
 =============
 
 The read the docs page should be automatically updated whenever there's a new commit on the ``main`` branch.
 
 The documentation is included as docstrings in the source code. Please write docstrings to any classes or functions you add following the `numpy style <https://numpydoc.readthedocs.io/en/latest/format.html>`_. The API reference documentation will only be automatically generated if the docstrings are written correctly. The documentation directory ``/doc`` also contains ``.rst`` files that provide additional info regarding installation, development, the models, etc.
@@ -115,16 +114,14 @@
     python setup.py build_sphinx
 
 The local build of the documentation webpage can be found in ``build/sphinx/html/index.html``.
 
 Releases
 ========
 
-The process of packaging a python project is described here: `https://packaging.python.org/en/latest/tutorials/packaging-projects <https://packaging.python.org/en/latest/tutorials/packaging-projects>`_.
-
 A couple packages are needed to build and upload a project to PyPI, these can be installed in your conda environment with:
 
 .. code-block:: shell
 
     pip install build twine
 
 The following steps can be used to release a new version:
```

### Comparing `osl-dynamics-1.3.1/README.rst` & `osl_dynamics-1.3.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -15,38 +15,36 @@
 ============
 
 Conda
 -----
 
 We recommend installing osl-dynamics within a virtual environment. You can do this with `Anaconda <https://docs.anaconda.com/free/anaconda/install/index.html>`_ (or `miniconda <https://docs.conda.io/projects/miniconda/en/latest/miniconda-install.html>`_).
 
+Below we describe how to install osl-dynamics from source. We recommend using the conda environment files in ``/envs``.
+
 Linux
 -----
 
-Here, we describe how to install osl-dynamics from source. We recommend using the conda environment files in ``/envs``. For a generic linux machine, osl-dynamics can be installed in editable mode with:
-
 .. code-block:: shell
 
     git clone https://github.com/OHBA-analysis/osl-dynamics.git
     cd osl-dynamics
     conda env create -f envs/linux.yml
     conda activate osld
     pip install -e .
 
-Note, if you have a Mac you may want to use the ``envs/mac.yml`` environment file instead.
+Mac
+---
+
+For a Mac, the installation of TensorFlow is slightly different to a Linux computer. We recommend using the lines above replacing the Linux environment file ``envs/linux.yml`` with the Mac environment file ``envs/mac.yml``.
 
 Windows
 -------
 
-If you are using a Windows computer, we recommend first installing linux (Ubuntu) as a Windows Subsystem by following the instructions `here <https://ubuntu.com/wsl>`_. Then following the instructions above in the Ubuntu terminal.
-
-Oxford specific computers
--------------------------
-
-If you're installing on the Oxford BMRC server, use ``envs/bmrc.yml``. If you're installing on the OHBA workstation, use ``envs/hbaws.yml``. Note, the ``hbaws.yml`` environment will automatically install spyder and jupyter notebooks.
+If you are using a Windows computer, we recommend first installing Linux (Ubuntu) as a Windows Subsystem by following the instructions `here <https://ubuntu.com/wsl>`_. Then following the instructions above in the Ubuntu terminal.
 
 Within an osl environment
 -------------------------
 
 If you have already installed `OSL <https://github.com/OHBA-analysis/osl>`_ you can install osl-dynamics in the ``osl`` environment with:
 
 .. code-block:: shell
@@ -55,23 +53,23 @@
     cd osl-dynamics
     pip install tensorflow==2.9.1
     pip install tensorflow-probability==0.17
     pip install -e .
 
 Note, if you're using a Mac computer you need to install TensorFlow with ``pip install tensorflow-macos==2.9.1`` instead of ``tensorflow==2.9.1``.
 
-Developers
-----------
+Removing osl-dynamics
+---------------------
 
-Developers might want to clone the repo using SSH instead of HTTPS:
+Simply delete the conda environment and repository:
 
 .. code-block:: shell
 
-    git clone git@github.com:OHBA-analysis/osl-dynamics.git
-
+    conda env remove -n osld
+    rm -rf osl-dynamics
 
 Documentation
 =============
 
 The read the docs page should be automatically updated whenever there's a new commit on the ``main`` branch.
 
 The documentation is included as docstrings in the source code. Please write docstrings to any classes or functions you add following the `numpy style <https://numpydoc.readthedocs.io/en/latest/format.html>`_. The API reference documentation will only be automatically generated if the docstrings are written correctly. The documentation directory ``/doc`` also contains ``.rst`` files that provide additional info regarding installation, development, the models, etc.
@@ -90,16 +88,14 @@
     python setup.py build_sphinx
 
 The local build of the documentation webpage can be found in ``build/sphinx/html/index.html``.
 
 Releases
 ========
 
-The process of packaging a python project is described here: `https://packaging.python.org/en/latest/tutorials/packaging-projects <https://packaging.python.org/en/latest/tutorials/packaging-projects>`_.
-
 A couple packages are needed to build and upload a project to PyPI, these can be installed in your conda environment with:
 
 .. code-block:: shell
 
     pip install build twine
 
 The following steps can be used to release a new version:
```

### Comparing `osl-dynamics-1.3.1/osl_dynamics/__init__.py` & `osl_dynamics-1.3.2/osl_dynamics/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/analysis/connectivity.py` & `osl_dynamics-1.3.2/osl_dynamics/analysis/connectivity.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,22 @@
   /tutorials_build/sliding_window_analysis.html>`_.
 - `HMM Coherence Analysis <https://osl-dynamics.readthedocs.io/en/latest\
   /tutorials_build/hmm_coherence_analysis.html>`_.
 - `DyNeMo Plotting Networks <https://osl-dynamics.readthedocs.io/en/latest\
   /tutorials_build/dynemo_plotting_networks.html>`_.
 """
 
+import os
 from pathlib import Path
 
 import numpy as np
 from nilearn import plotting
 from scipy import stats
 from tqdm.auto import trange
+import matplotlib.pyplot as plt
 
 from osl_dynamics import array_ops
 from osl_dynamics.analysis import gmm
 from osl_dynamics.analysis.spectral import get_frequency_args_range
 from osl_dynamics.utils.misc import override_dict_defaults
 from osl_dynamics.utils.parcellation import Parcellation
 
@@ -755,14 +757,18 @@
 def save(
     connectivity_map,
     parcellation_file,
     filename=None,
     component=None,
     threshold=0,
     plot_kwargs=None,
+    axes=None,
+    combined=False,
+    titles=None,
+    n_rows=1,
 ):
     """Save connectivity maps as image files.
 
     This function is a wrapper for `nilearn.plotting.plot_connectome \
     <https://nilearn.github.io/stable/modules/generated/nilearn\
     .plotting.plot_connectome.html>`_.
 
@@ -783,14 +789,25 @@
     threshold : float or np.ndarray, optional
         Threshold to determine which connectivity to show. Should be between 0
         and 1. If a :code:`float` is passed the same threshold is used for all
         modes. Otherwise, threshold should be a numpy array of shape
         (n_modes,).
     plot_kwargs : dict, optional
         Keyword arguments to pass to the nilearn plotting function.
+    axes : list, optional
+        List of matplotlib axes to plot the connectivity maps on.
+    combined : bool, optional
+        Should the connectivity maps be combined on the same figure?
+        The combined image is always shown on screen (for Juptyer notebooks).
+        Note if :code:`True` is passed, the individual images will be deleted.
+    titles : list, optional
+        List of titles for each connectivity map. Only used if
+        :code:`combined=True`.
+    n_rows : int, optional
+        Number of rows in the combined image. Only used if :code:`combined=True`.
 
     Examples
     --------
     Change colormap and views::
 
         connectivity.save(
             ...,
@@ -834,14 +851,16 @@
         np.fill_diagonal(c, 0)
 
     # Default plotting settings
     default_plot_kwargs = {"node_size": 10, "node_color": "black"}
 
     # Loop through each connectivity map
     n_modes = conn_map.shape[0]
+    axes = axes or [None] * n_modes
+    output_files = []
     for i in trange(n_modes, desc="Saving images"):
         # Overwrite keyword arguments if passed
         kwargs = override_dict_defaults(default_plot_kwargs, plot_kwargs)
 
         # Output filename
         if filename is None:
             output_file = None
@@ -857,16 +876,38 @@
 
         # Plot maps
         plotting.plot_connectome(
             conn_map[i],
             parcellation.roi_centers(),
             edge_threshold=f"{threshold[i] * 100}%",
             output_file=output_file,
+            axes=axes[i],
             **kwargs,
         )
+        output_files.append(output_file)
+
+    if combined:
+        # Combine the images
+        if filename is None:
+            raise ValueError("filename must be passed to save the combined image.")
+
+        n_columns = -(n_modes // -n_rows)
+        titles = titles or [None] * n_modes
+        fig, axes = plt.subplots(n_rows, n_columns, figsize=(n_columns * 5, n_rows * 5))
+        for i, ax in enumerate(axes.flatten()):
+            ax.axis("off")
+            if i < n_modes:
+                ax.imshow(plt.imread(output_files[i]))
+                ax.set_title(titles[i], fontsize=20)
+        fig.tight_layout()
+        fig.savefig(filename)
+
+        # Remove the individual images
+        for output_file in output_files:
+            os.remove(output_file)
 
 
 def save_interactive(
     connectivity_map,
     parcellation_file,
     filename=None,
     component=None,
```

### Comparing `osl-dynamics-1.3.1/osl_dynamics/analysis/fisher_kernel.py` & `osl_dynamics-1.3.2/osl_dynamics/analysis/fisher_kernel.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/analysis/gmm.py` & `osl_dynamics-1.3.2/osl_dynamics/analysis/gmm.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/analysis/modes.py` & `osl_dynamics-1.3.2/osl_dynamics/analysis/modes.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 """
 
 import itertools
 import logging
 
 import numpy as np
 from scipy import signal
+from pqdm.threads import pqdm
+from tqdm.auto import trange
 
 from osl_dynamics import array_ops
 
 _logger = logging.getLogger("osl-dynamics")
 
 
 def autocorr_from_tde_cov(
@@ -773,7 +775,110 @@
         # Variance normalise state/mode time courses
         a_normed = a / np.std(a, axis=0, keepdims=True)
 
         # Do multiple regression of alpha onto data
         pcovs.append(np.linalg.pinv(a_normed) @ X)
 
     return np.squeeze(pcovs)
+
+
+def hmm_dual_estimation(data, alpha, zero_mean=False, eps=1e-5, n_jobs=1):
+    """HMM dual estiation of observation model parameters.
+
+    Parameters
+    ----------
+    data : np.ndarray or list of np.ndarray
+        Time series data. Shape must be (n_samples, n_channels)
+        or (n_subjects, n_samples, n_channels).
+    alpha : np.ndarray or list of np.ndarray
+        State probabilities. Shape must be (n_samples, n_states)
+        or (n_subjects, n_samples, n_states).
+    zero_mean : bool, optional
+        Should we force the state means to be zero?
+    eps : float, optional
+        Small value to add to the diagonal of each state covariance.
+    n_jobs : int, optional
+        Number of jobs to run in parallel.
+
+    Returns
+    -------
+    means : np.ndarray or list of np.ndarray
+        State means. Shape is (n_states, n_channels) or
+        (n_subjects, n_states, n_channels).
+    covariances : np.ndarray or list of np.ndarray
+        State covariances. Shape is (n_states, n_channels, n_channels)
+        or (n_subjects, n_states, n_channels, n_channels).
+    """
+
+    # Validation
+    if (isinstance(data, list) != isinstance(alpha, list)) or (
+        isinstance(data, np.ndarray) != isinstance(alpha, np.ndarray)
+    ):
+        raise ValueError(
+            f"data is type {type(data)} and alpha is type "
+            f"{type(alpha)}. They must both be lists or numpy arrays."
+        )
+
+    if isinstance(data, np.ndarray):
+        if alpha.shape[0] != data.shape[0]:
+            raise ValueError("data and alpha must have the same number of samples.")
+
+        if data.ndim == 2:
+            data = [data]
+            alpha = [alpha]
+
+    if len(data) != len(alpha):
+        raise ValueError(
+            "A different number of arrays has been passed for "
+            f"data and alpha: len(data)={len(data)}, "
+            f"len(alpha)={len(alpha)}."
+        )
+
+    # Check the number of samples in data and alpha
+    for i in range(len(alpha)):
+        if alpha[i].shape[0] != data[i].shape[0]:
+            raise ValueError(
+                "items in data and alpha must have the same number of samples."
+            )
+
+    n_states = alpha[0].shape[1]
+    n_channels = data[0].shape[1]
+
+    # Helper function
+    def _calc(a, x):
+        sum_a = np.sum(a, axis=0)
+
+        m = np.zeros([n_states, n_channels])
+        if not zero_mean:
+            for i in range(n_states):
+                m[i] = np.sum(x * a[:, i, None], axis=0) / sum_a[i]
+
+        c = np.zeros([n_states, n_channels, n_channels])
+        for i in range(n_states):
+            d = x - m[i]
+            c[i] = (
+                np.sum(d[:, :, None] * d[:, None, :] * a[:, i, None, None], axis=0)
+                / sum_a[i]
+            )
+            c[i] += eps * np.eye(n_channels)
+
+        return m, c
+
+    # Calculate in parallel
+    results = pqdm(
+        array=zip(alpha, data),
+        function=_calc,
+        n_jobs=n_jobs,
+        desc="Dual estimation",
+        argument_type="args",
+        total=len(data),
+    )
+
+    # Unpack results
+    means = []
+    covariances = []
+    for result in results:
+        m, c = result
+        means.append(m)
+        covariances.append(c)
+
+    return np.squeeze(means), np.squeeze(covariances)
```

### Comparing `osl-dynamics-1.3.1/osl_dynamics/analysis/power.py` & `osl_dynamics-1.3.2/osl_dynamics/analysis/power.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import logging
 from pathlib import Path
 
 import numpy as np
 import nibabel as nib
 from nilearn import plotting
 from tqdm.auto import trange
+import matplotlib.pyplot as plt
 
 from osl_dynamics import array_ops, files
 from osl_dynamics.analysis.spectral import get_frequency_args_range
 
 _logger = logging.getLogger("osl-dynamics")
 
 
@@ -242,14 +243,17 @@
 
     Returns
     -------
     voxel_grid : np.ndarray
         Value at each voxel. Shape is (x, y, z), where :code:`x`,
         :code:`y` and :code:`z` correspond to 3D voxel locations.
     """
+    # Suppress INFO messages from nibabel
+    logging.getLogger("nibabel.global").setLevel(logging.ERROR)
+
     # Validation
     mask_file = files.check_exists(mask_file, files.mask.directory)
     parcellation_file = files.check_exists(
         parcellation_file, files.parcellation.directory
     )
 
     # Load the mask
@@ -296,14 +300,18 @@
     mask_file,
     parcellation_file,
     filename=None,
     component=0,
     subtract_mean=False,
     mean_weights=None,
     plot_kwargs=None,
+    show_plots=True,
+    combined=False,
+    titles=None,
+    n_rows=1,
 ):
     """Saves power maps.
 
     This function is a wrapper for `nilearn.plotting.plot_img_on_surf
     <https://nilearn.github.io/stable/modules/generated/nilearn.plotting\
     .plot_img_on_surf.html>`_.
 
@@ -330,14 +338,24 @@
     mean_weights: np.ndarray, optional
         Numpy array with weightings for each mode to use to calculate the mean.
         Default is equal weighting.
     plot_kwargs : dict, optional
         Keyword arguments to pass to `nilearn.plotting.plot_img_on_surf
         <https://nilearn.github.io/stable/modules/generated/nilearn.plotting\
         .plot_img_on_surf.html>`_.
+    show_plots : bool, optional
+        Should the individual plots be shown on screen (for Juptyer notebooks)?
+    combined : bool, optional
+        Should the individual plots be combined into a single image?
+        The combined image is always shown on screen (for Juptyer notebooks).
+        Note if :code:`True` is passed, the individual images will be deleted.
+    titles : list, optional
+        List of titles for each power plot. Only used if :code:`combined=True`.
+    n_rows : int, optional
+        Number of rows in the combined image. Only used if :code:`combined=True`.
 
     Returns
     -------
     figures : list of plt.figure
         List of Matplotlib figure object. Only returned if
         :code:`filename=None`.
     axes : list of plt.axis
@@ -435,28 +453,53 @@
         if ".nii" in filename:
             _logger.info(f"Saving {filename}")
             nii = nib.Nifti1Image(power_map, mask.affine, mask.header)
             nib.save(nii, filename)
 
         else:
             # Save each map as an image
+            output_files = []
             for i in trange(n_modes, desc="Saving images"):
                 nii = nib.Nifti1Image(
                     power_map[:, :, :, i],
                     mask.affine,
                     mask.header,
                 )
                 fig, ax = plotting.plot_img_on_surf(
                     nii, output_file=None, **plot_kwargs
                 )
                 output_file = "{fn.parent}/{fn.stem}{i:0{w}d}{fn.suffix}".format(
                     fn=Path(filename), i=i, w=len(str(n_modes))
                 )
+                output_files.append(output_file)
                 fig.savefig(output_file)
 
+                if not show_plots:
+                    plt.close(fig)
+
+            if combined:
+                n_columns = -(n_modes // -n_rows)
+
+                titles = titles or [None] * n_modes
+                # Combine images into a single image
+                fig, axes = plt.subplots(
+                    n_rows, n_columns, figsize=(n_columns * 5, n_rows * 5)
+                )
+                for i, ax in enumerate(axes.flatten()):
+                    ax.axis("off")
+                    if i < n_modes:
+                        ax.imshow(plt.imread(output_files[i]))
+                        ax.set_title(titles[i], fontsize=20)
+                fig.tight_layout()
+                fig.savefig(filename)
+
+                # Remove the individual images
+                for output_file in output_files:
+                    os.remove(output_file)
+
 
 def multi_save(
     group_power_map,
     session_power_map,
     mask_file,
     parcellation_file,
     filename=None,
```

### Comparing `osl-dynamics-1.3.1/osl_dynamics/analysis/regression.py` & `osl_dynamics-1.3.2/osl_dynamics/analysis/regression.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/analysis/spectral.py` & `osl_dynamics-1.3.2/osl_dynamics/analysis/spectral.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,23 +193,23 @@
                     f"len(alpha)={len(alpha)}."
                 )
 
             # Check the number of samples in data and alpha
             for i in range(len(alpha)):
                 if alpha[i].shape[0] != data[i].shape[0]:
                     raise ValueError(
-                        "items in data and alpha must have the same shape."
+                        "items in data and alpha must have the number of samples."
                     )
 
     elif isinstance(data, list):
         alpha = np.array([None] * len(data))
 
     if isinstance(data, np.ndarray):
         if alpha is not None and alpha.shape[0] != data.shape[0]:
-            raise ValueError("data and alpha must have the same shape.")
+            raise ValueError("data and alpha must have the number of samples.")
 
         if data.ndim == 2:
             data = [data]
             alpha = [alpha]
 
     if window_length is None:
         window_length = 2 * sampling_frequency
@@ -383,23 +383,23 @@
                     f"len(alpha)={len(alpha)}."
                 )
 
             # Check the number of samples in data and alpha
             for i in range(len(alpha)):
                 if alpha[i].shape[0] != data[i].shape[0]:
                     raise ValueError(
-                        "items in data and alpha must have the same shape."
+                        "items in data and alpha must have the same number of samples."
                     )
 
     elif isinstance(data, list):
         alpha = np.array([None] * len(data))
 
     if isinstance(data, np.ndarray):
         if alpha is not None and alpha.shape[0] != data.shape[0]:
-            raise ValueError("data and alpha must have the same shape.")
+            raise ValueError("data and alpha must have the number of samples.")
 
         if data.ndim == 2:
             data = [data]
             alpha = [alpha]
 
     if window_length is None:
         window_length = 2 * sampling_frequency
@@ -585,19 +585,21 @@
                 f"data and alpha: len(data)={len(data)}, "
                 f"len(alpha)={len(alpha)}."
             )
 
         # Check the number of samples in data and alpha
         for i in range(len(alpha)):
             if alpha[i].shape[0] != data[i].shape[0]:
-                raise ValueError("items in data and alpha must have the same shape.")
+                raise ValueError(
+                    "items in data and alpha must have the number of samples."
+                )
 
     if isinstance(data, np.ndarray):
         if alpha.shape[0] != data.shape[0]:
-            raise ValueError("data and alpha must have the same shape.")
+            raise ValueError("data and alpha must have the number of samples.")
 
         if data.ndim == 2:
             data = [data]
             alpha = [alpha]
 
     # Ensure data and alpha are float32
     data = [d.astype(np.float32) for d in data]
@@ -1733,15 +1735,15 @@
     # each state was active
     fo = np.sum(stc, axis=0) / stc.shape[0]
     for i, (psd_, fo_) in enumerate(zip(psd, fo)):
         psd_ /= fo_
         if np.isnan(psd_).any():
             psd[i] = np.nan_to_num(psd_)  # zero out nan values
             _logger.warn(
-                "PSD contains NaN values. This may indicate a potentially"
+                "PSD contains NaN values. This may indicate a potentially "
                 "poor HMM fit. You should consider running the model again "
                 "or selecting the model run with the lowest free energy after "
                 "training multiple times."
             )
 
     if not keepdims:
         # Squeeze any axes of length 1
```

### Comparing `osl-dynamics-1.3.1/osl_dynamics/analysis/static.py` & `osl_dynamics-1.3.2/osl_dynamics/analysis/static.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/analysis/statistics.py` & `osl_dynamics-1.3.2/osl_dynamics/analysis/statistics.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/analysis/tinda.py` & `osl_dynamics-1.3.2/osl_dynamics/analysis/tinda.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/analysis/workbench.py` & `osl_dynamics-1.3.2/osl_dynamics/analysis/workbench.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/array_ops.py` & `osl_dynamics-1.3.2/osl_dynamics/array_ops.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/config_api/__init__.py` & `osl_dynamics-1.3.2/osl_dynamics/config_api/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/config_api/pipeline.py` & `osl_dynamics-1.3.2/osl_dynamics/config_api/pipeline.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/config_api/wrappers.py` & `osl_dynamics-1.3.2/osl_dynamics/config_api/wrappers.py`

 * *Files 0% similar despite different names*

```diff
@@ -471,15 +471,15 @@
         # Save inferred parameters
         save(f"{inf_params_dir}/alp.pkl", alpha)
         save(f"{inf_params_dir}/means.npy", means)
         save(f"{inf_params_dir}/covs.npy", covs)
         save(f"{inf_params_dir}/session_means.npy", session_means)
         save(f"{inf_params_dir}/session_covs.npy", session_covs)
         save(f"{inf_params_dir}/summed_embeddings.npy", summed_embeddings)
-        save(f"{inf_params_dir}/embedding_weights.npy", embedding_weights)
+        save(f"{inf_params_dir}/embedding_weights.pkl", embedding_weights)
 
 
 def get_inf_params(data, output_dir, observation_model_only=False):
     """Get inferred alphas.
 
     This function expects a model has already been trained and the following
     directory to exist:
```

### Comparing `osl-dynamics-1.3.1/osl_dynamics/data/base.py` & `osl_dynamics-1.3.2/osl_dynamics/data/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -325,23 +325,25 @@
 
     def validate_data(self):
         """Validate data files."""
         n_channels = [array.shape[-1] for array in self.raw_data_arrays]
         if not np.equal(n_channels, n_channels[0]).all():
             raise ValueError("All inputs should have the same number of channels.")
 
-    def select(self, channels=None, use_raw=False):
+    def select(self, channels=None, sessions=None, use_raw=False):
         """Select channels.
 
         This is an in-place operation.
 
         Parameters
         ----------
         channels : int or list of int, optional
             Channel indices to keep. If None, all channels are retained.
+        sessions : int or list of int, optional
+            Session indices to keep. If None, all sessions are retained.
         use_raw : bool, optional
             Should we select channel from the original 'raw' data that
             we loaded?
 
         Returns
         -------
         data : osl_dynamics.data.Data
@@ -351,29 +353,46 @@
             # Keep all channels
             if use_raw:
                 n_channels = self.raw_data_arrays[0].shape[-1]
             else:
                 n_channels = self.arrays[0].shape[-1]
             channels = range(n_channels)
 
+        if sessions is None:
+            # Keep all sessions
+            if use_raw:
+                n_sessions = len(self.raw_data_arrays)
+            else:
+                n_sessions = len(self.arrays)
+            sessions = range(n_sessions)
+
         if isinstance(channels, int):
             channels = [channels]
 
+        if isinstance(sessions, int):
+            sessions = [sessions]
+
         if isinstance(channels, range):
             channels = list(channels)
 
+        if isinstance(sessions, range):
+            sessions = list(sessions)
+
         if not isinstance(channels, list):
             raise ValueError("channels must be an int or list of int.")
 
+        if not isinstance(sessions, list):
+            raise ValueError("sessions must be an int or list of int.")
+
         # What data should we use?
         arrays = self.raw_data_arrays if use_raw else self.arrays
 
         # Select channels
         new_arrays = []
-        for i in tqdm(range(self.n_sessions), desc="Selecting channels"):
+        for i in tqdm(sessions, desc="Selecting channels/sessions"):
             array = arrays[i][:, channels]
             if self.load_memmaps:
                 array = misc.array_to_memmap(self.prepared_data_filenames[i], array)
             new_arrays.append(array)
         self.arrays = new_arrays
 
         return self
@@ -965,15 +984,15 @@
             if hasattr(self, "n_window"):
                 n_remove += self.n_window // 2
         else:
             n_remove += n_window // 2
         if verbose:
             _logger.info(
                 f"Removing {n_remove} data points from the start and end"
-                + " of each array due to time embedding/sliding window."
+                " of each array due to time embedding/sliding window."
             )
 
         # What data should we trim?
         if prepared:
             arrays = self.arrays
         else:
             arrays = self.raw_data_arrays
@@ -986,16 +1005,16 @@
 
             # Remove data points lost to separating into sequences
             if sequence_length is not None:
                 n_sequences = array.shape[0] // sequence_length
                 n_keep = n_sequences * sequence_length
                 if verbose:
                     _logger.info(
-                        f"Removing {array.shape[0] - n_keep} data points"
-                        + f" from the end of array {i} due to sequencing."
+                        f"Removing {array.shape[0] - n_keep} data points "
+                        f"from the end of array {i} due to sequencing."
                     )
                 array = array[:n_keep]
 
             trimmed_time_series.append(array)
 
         if concatenate or len(trimmed_time_series) == 1:
             trimmed_time_series = np.concatenate(trimmed_time_series)
@@ -1152,16 +1171,16 @@
                 training_dataset_size = round((1.0 - validation_split) * dataset_size)
 
                 # Split the full dataset into a training and validation dataset
                 training_dataset = full_dataset.take(training_dataset_size)
                 validation_dataset = full_dataset.skip(training_dataset_size)
                 _logger.info(
                     f"{len(training_dataset)} batches in training dataset, "
-                    + f"{len(validation_dataset)} batches in the validation "
-                    + "dataset."
+                    f"{len(validation_dataset)} batches in the validation "
+                    "dataset."
                 )
 
                 return training_dataset.prefetch(
                     tf.data.AUTOTUNE
                 ), validation_dataset.prefetch(tf.data.AUTOTUNE)
 
         # Otherwise create a dataset for each array separately
@@ -1205,17 +1224,17 @@
                     validation_datasets.append(
                         full_datasets[i]
                         .skip(training_dataset_size)
                         .prefetch(tf.data.AUTOTUNE)
                     )
                     _logger.info(
                         f"Session {i}: "
-                        + f"{len(training_datasets[i])} batches in training dataset, "
-                        + f"{len(validation_datasets[i])} batches in the validation "
-                        + "dataset."
+                        f"{len(training_datasets[i])} batches in training dataset, "
+                        f"{len(validation_datasets[i])} batches in the validation "
+                        "dataset."
                     )
                 return training_datasets, validation_datasets
 
     def save_tfrecord_dataset(
         self,
         tfrecord_dir,
         sequence_length,
```

### Comparing `osl-dynamics-1.3.1/osl_dynamics/data/processing.py` & `osl_dynamics-1.3.2/osl_dynamics/data/processing.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/data/rw.py` & `osl_dynamics-1.3.2/osl_dynamics/data/rw.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/data/task.py` & `osl_dynamics-1.3.2/osl_dynamics/data/task.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/data/tf.py` & `osl_dynamics-1.3.2/osl_dynamics/data/tf.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/__init__.py` & `osl_dynamics-1.3.2/osl_dynamics/files/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/functions.py` & `osl_dynamics-1.3.2/osl_dynamics/files/functions.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/mask/MNI152_T1_1mm_brain.nii.gz` & `osl_dynamics-1.3.2/osl_dynamics/files/mask/MNI152_T1_1mm_brain.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/mask/MNI152_T1_2mm_brain.nii.gz` & `osl_dynamics-1.3.2/osl_dynamics/files/mask/MNI152_T1_2mm_brain.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/mask/MNI152_T1_8mm_brain.nii.gz` & `osl_dynamics-1.3.2/osl_dynamics/files/mask/MNI152_T1_8mm_brain.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/mask/ParcellationPilot.L.inflated.32k_fs_LR.surf.gii` & `osl_dynamics-1.3.2/osl_dynamics/files/mask/ParcellationPilot.L.inflated.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/mask/ParcellationPilot.L.midthickness.32k_fs_LR.surf.gii` & `osl_dynamics-1.3.2/osl_dynamics/files/mask/ParcellationPilot.L.midthickness.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/mask/ParcellationPilot.L.very_inflated.32k_fs_LR.surf.gii` & `osl_dynamics-1.3.2/osl_dynamics/files/mask/ParcellationPilot.L.very_inflated.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/mask/ParcellationPilot.R.inflated.32k_fs_LR.surf.gii` & `osl_dynamics-1.3.2/osl_dynamics/files/mask/ParcellationPilot.R.inflated.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/mask/ParcellationPilot.R.midthickness.32k_fs_LR.surf.gii` & `osl_dynamics-1.3.2/osl_dynamics/files/mask/ParcellationPilot.R.midthickness.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/mask/ParcellationPilot.R.very_inflated.32k_fs_LR.surf.gii` & `osl_dynamics-1.3.2/osl_dynamics/files/mask/ParcellationPilot.R.very_inflated.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/mask/__init__.py` & `osl_dynamics-1.3.2/osl_dynamics/files/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/mask/ft_8mm_brain_mask.nii.gz` & `osl_dynamics-1.3.2/osl_dynamics/files/mask/ft_8mm_brain_mask.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/parcellation/Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz` & `osl_dynamics-1.3.2/osl_dynamics/files/parcellation/Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/parcellation/Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz` & `osl_dynamics-1.3.2/osl_dynamics/files/parcellation/Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/parcellation/__init__.py` & `osl_dynamics-1.3.2/osl_dynamics/files/parcellation/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/parcellation/aal_cortical_merged_8mm_stacked.nii.gz` & `osl_dynamics-1.3.2/osl_dynamics/files/parcellation/aal_cortical_merged_8mm_stacked.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/parcellation/fMRI_parcellation_ds8mm.nii.gz` & `osl_dynamics-1.3.2/osl_dynamics/files/parcellation/fMRI_parcellation_ds8mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm.nii.gz` & `osl_dynamics-1.3.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm_adj.nii.gz` & `osl_dynamics-1.3.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm_adj.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz` & `osl_dynamics-1.3.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz` & `osl_dynamics-1.3.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz` & `osl_dynamics-1.3.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/parcellation/giles_39_binary.nii.gz` & `osl_dynamics-1.3.2/osl_dynamics/files/parcellation/giles_39_binary.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/ctf275_channel_names.npy` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/ctf275_channel_names.npy`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/4D148.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/4D148.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/4D248.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/4D248.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/4D248_helmet.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/4D248_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/4D248_helmet.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/4D248_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/CTF151.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/CTF151.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/CTF151_helmet.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/CTF151_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/CTF151_helmet.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/CTF151_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/CTF275.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/CTF275.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/CTF275_helmet.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/CTF275_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/CTF275_helmet.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/CTF275_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/EEG1005.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/EEG1005.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/EEG1010.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/EEG1010.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/EEG1020.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/EEG1020.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/biosemi128.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/biosemi128.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/biosemi16.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/biosemi16.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/biosemi160.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/biosemi160.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/biosemi256.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/biosemi256.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/biosemi32.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/biosemi32.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/biosemi64.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/biosemi64.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM1.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM1.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM1.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM1.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM10.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM10.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM10.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM10.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM11.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM11.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM11.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM11.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM14.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM14.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM14.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM14.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM15.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM15.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM15.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM15.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM16.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM16.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM16.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM16.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM17.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM17.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM17.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM17.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM20.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM20.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM20.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM20.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM22.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM22.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM22.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM22.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM23.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM23.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM23.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM23.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM24.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM24.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM24.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM24.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM25.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM25.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM25.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM25.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM3.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM3.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM3.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM3.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM7.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM7.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/easycapM7.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/easycapM7.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/elec1005.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/elec1005.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/elec1010.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/elec1010.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/elec1020.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/elec1020.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/natmeg_customized_eeg1005.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/natmeg_customized_eeg1005.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag122cmb.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag122cmb.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag122planar.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag122planar.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag306all.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag306all.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag306cmb.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag306cmb.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag306mag.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag306mag.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag306planar.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag306planar.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/quickcap64.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/quickcap64.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/quickcap64.outline` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/quickcap64.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/yokogawa440.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/yokogawa440.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/yokogawa440_old.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/yokogawa440_old.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/yokogawa440ag.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/yokogawa440ag.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/yokogawa440all.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/yokogawa440all.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/layouts/yokogawa440pg.lay` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/layouts/yokogawa440pg.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scanner/neuromag306_channel_names.npy` & `osl_dynamics-1.3.2/osl_dynamics/files/scanner/neuromag306_channel_names.npy`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/files/scene/mode_scene.scene` & `osl_dynamics-1.3.2/osl_dynamics/files/scene/mode_scene.scene`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/inference/callbacks.py` & `osl_dynamics-1.3.2/osl_dynamics/inference/callbacks.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/inference/initializers.py` & `osl_dynamics-1.3.2/osl_dynamics/inference/initializers.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/inference/layers.py` & `osl_dynamics-1.3.2/osl_dynamics/inference/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,22 +266,27 @@
         if do_annealing:
             self.annealing_factor = tf.Variable(0.0, trainable=False)
         else:
             self.annealing_factor = tf.Variable(1.0, trainable=False)
 
     def call(self, inputs, training=None, **kwargs):
         """This method accepts the shape and rate and outputs the samples."""
-        alpha, beta = inputs
-        # alpha.shape = (None, n_states, 1)
-        # beta.shape = (None, n_states, 1)
+        alpha, beta, session_id = inputs
+        # alpha.shape = (n_sessions, n_states, 1)
+        # beta.shape = (n_sessions, n_states, 1)
+        # session_id.shape = (None, sequence_length)
 
         # output.shape = (None, n_states, 1)
 
         alpha = add_epsilon(alpha, self.epsilon)
         beta = add_epsilon(beta, self.epsilon)
+        session_id = session_id[:, 0]
+
+        alpha = tf.gather(alpha, session_id, axis=0)  # shape = (None, n_states, 1)
+        beta = tf.gather(beta, session_id, axis=0)  # shape = (None, n_states, 1)
         if training:
             output = alpha / beta
             if self.annealing_factor > 0:
                 N = tfp.distributions.Gamma(
                     concentration=alpha,
                     rate=beta,
                     allow_nan_stats=False,
@@ -1445,56 +1450,56 @@
         ) + 0 * tf.expand_dims(tf.expand_dims(place_holder, axis=-1), axis=-1)
 
         concat_embeddings = tf.concat([embeddings, spatial_embeddings], axis=-1)
 
         return concat_embeddings
 
 
-class SessionMapLayer(layers.Layer):
-    """Layer for getting the array specific maps.
+class SessionParamLayer(layers.Layer):
+    """Layer for getting the array specific parameters.
 
-    This layer adds deviations to the group spatial maps.
+    This layer adds deviations to the group spatial parameters.
 
     Parameters
     ----------
-    which_map : str
-        Which spatial map are we using? Must be :code:`'means'` or
+    param : str
+        Which parameter are we using? Must be :code:`'means'` or
         :code:`'covariances'`.
     epsilon : float
         Error added to the diagonal of covariances for numerical stability.
     kwargs : keyword arguments, optional
         Keyword arguments to pass to the base class.
     """
 
-    def __init__(self, which_map, epsilon, **kwargs):
+    def __init__(self, param, epsilon, **kwargs):
         super().__init__(**kwargs)
-        self.which_map = which_map
+        self.param = param
         self.epsilon = epsilon
-        if which_map == "covariances":
+        if param == "covariances":
             self.bijector = tfb.Chain(
                 [tfb.CholeskyOuterProduct(), tfb.FillScaleTriL()],
             )
-        elif which_map == "means":
+        elif param == "means":
             self.bijector = tfb.Identity()
         else:
-            raise ValueError("which_map must be one of 'means' and 'covariances'.")
+            raise ValueError("param must be one of 'means' and 'covariances'.")
 
     def call(self, inputs):
-        group_map, dev = inputs
-        group_map = self.bijector.inverse(group_map)
+        group_param, dev = inputs
+        group_param = self.bijector.inverse(group_param)
 
         # Match dimensions for addition
-        group_map = tf.expand_dims(group_map, axis=0)
-        session_map = tf.add(group_map, dev)
-        session_map = self.bijector(session_map)
+        group_param = tf.expand_dims(group_param, axis=0)
+        session_param = tf.add(group_param, dev)
+        session_param = self.bijector(session_param)
 
-        if self.which_map == "covariances":
-            session_map = add_epsilon(session_map, self.epsilon, diag=True)
+        if self.param == "covariances":
+            session_param = add_epsilon(session_param, self.epsilon, diag=True)
 
-        return session_map
+        return session_param
 
 
 class MixSessionSpecificParametersLayer(layers.Layer):
     r"""Class for mixing means and covariances.
 
     The mixture is calculated as
 
@@ -1537,18 +1542,18 @@
         Keyword arguments to pass to the base class.
     """
 
     def __init__(self, epsilon, **kwargs):
         super().__init__(**kwargs)
         self.epsilon = epsilon
 
-    def call(self, inputs, **kwargs):
-        # inference_alpha.shape = (None, n_states, 1)
-        # inference_beta.shape  = (None, n_states, 1)
-        # model_beta.shape      = (None, n_states, 1)
+    def call(self, inputs, static_loss_scaling_factor=1, **kwargs):
+        # inference_alpha.shape = (n_sessions, n_states, 1)
+        # inference_beta.shape  = (n_sessions, n_states, 1)
+        # model_beta.shape      = (n_sessions, n_states, 1)
 
         inference_alpha, inference_beta, model_beta = inputs
 
         # Add a small error for numerical stability
         inference_alpha = add_epsilon(inference_alpha, self.epsilon)
         inference_beta = add_epsilon(inference_beta, self.epsilon)
         model_beta = add_epsilon(model_beta, self.epsilon)
@@ -1557,18 +1562,17 @@
         prior = tfp.distributions.Exponential(rate=model_beta)
         posterior = tfp.distributions.Gamma(
             concentration=inference_alpha, rate=inference_beta
         )
         kl_loss = tfp.distributions.kl_divergence(
             posterior, prior, allow_nan_stats=False
         )
-        kl_loss = tf.reduce_mean(kl_loss, axis=0)
         kl_loss = tf.reduce_sum(kl_loss)
 
-        return kl_loss
+        return kl_loss * static_loss_scaling_factor
 
 
 class MultiLayerPerceptronLayer(layers.Layer):
     """Multi-Layer Perceptron layer.
 
     Parameters
     ----------
@@ -1966,35 +1970,81 @@
     def call(self, inputs, **kwargs):
         out = inputs[0]
         for tensor in inputs[1:]:
             out = tf.add(out, tensor)
         return out
 
 
-class ConstrainedEmbeddingLayer(layers.Layer):
-    """Layer for unit norm constrained embeddings.
+class EmbeddingLayer(layers.Layer):
+    """Layer for embeddings.
 
     Parameters
     ----------
     input_dim : int
         Input dimension.
     output_dim : int
         Output dimension.
+    unit_norm : bool, optional
+        Should the embeddings be unit norm?
     """
 
-    def __init__(self, input_dim, output_dim, **kwargs):
+    def __init__(self, input_dim, output_dim, unit_norm, **kwargs):
         super().__init__(**kwargs)
+        if unit_norm:
+            output_dim = output_dim - 1
+
         self.embedding_layer = layers.Embedding(
             input_dim=input_dim,
             output_dim=output_dim,
         )
-        self.constrain_layer = constraints.UnitNorm(axis=1)
         self.layers = [self.embedding_layer]
+        self.unit_norm = unit_norm
 
     def call(self, inputs, **kwargs):
         output = self.embedding_layer(inputs)
-        output = self.constrain_layer(output)
+
+        # Add the last element to ensure the embeddings are unit norm
+        if self.unit_norm:
+            norm_sq = tf.reduce_sum(tf.square(output), axis=-1, keepdims=True)
+            output = tf.concat([2 * output, norm_sq - 1], axis=-1) / (norm_sq + 1)
         return output
 
     @property
     def embeddings(self):
-        return self.constrain_layer(self.embedding_layer.embeddings)
+        output = self.embedding_layer.embeddings
+        if self.unit_norm:
+            norm_sq = tf.reduce_sum(tf.square(output), axis=-1, keepdims=True)
+            output = tf.concat([2 * output, norm_sq - 1], axis=-1) / (norm_sq + 1)
+        return output
+
+
+class ShiftForForecastingLayer(layers.Layer):
+    """Clip two tensors to ensure they align for causal forecasting.
+
+    Parameters
+    ----------
+    clip : int
+        Number of elements to clip.
+    """
+
+    def __init__(self, clip, **kwargs):
+        super().__init__(**kwargs)
+        self.clip = clip
+
+    def call(self, inputs, **kwargs):
+        A, B = inputs
+        A = A[:, : -self.clip]
+        B = B[:, self.clip :]
+        return A, B
+
+
+class TFConstantLayer(layers.Layer):
+    """Wrapper for `tf.constant \
+        <https://www.tensorflow.org/api_docs/python/tf/constant>`_.
+    """
+
+    def __init__(self, values, **kwargs):
+        super().__init__(**kwargs)
+        self.values = values
+
+    def call(self, inputs, **kwargs):
+        return tf.constant(self.values)
```

### Comparing `osl-dynamics-1.3.1/osl_dynamics/inference/metrics.py` & `osl_dynamics-1.3.2/osl_dynamics/inference/metrics.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/inference/modes.py` & `osl_dynamics-1.3.2/osl_dynamics/inference/modes.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 
 from pathlib import Path
 
 import mne
 import numpy as np
 import matplotlib.pyplot as plt
 from tqdm.auto import trange
-from scipy.optimize import linear_sum_assignment
-from scipy.cluster import hierarchy
+from scipy import cluster, spatial, optimize
 from sklearn.cluster import AgglomerativeClustering
 
 from osl_dynamics import analysis, array_ops
 from osl_dynamics.inference import metrics
 from osl_dynamics.utils import plotting
 from osl_dynamics.utils.misc import override_dict_defaults
 
@@ -290,26 +289,95 @@
                     F[j, k] = -np.corrcoef(
                         covariances[i][k].flatten(), covariances[0][j].flatten()
                     )[0, 1]
                 else:
                     F[j, k] = -metrics.pairwise_rv_coefficient(
                         np.array([covariances[i][k], covariances[0][j]])
                     )[0, 1]
-        order = linear_sum_assignment(F)[1]
+        order = optimize.linear_sum_assignment(F)[1]
 
         # Add the ordered matrix to the list
         matched_covariances.append(covariances[i][order])
         orders.append(order)
 
     if return_order:
         return orders
     else:
         return tuple(matched_covariances)
 
 
+def match_vectors(*vectors, comparison="correlation", return_order=False):
+    """Matches vectors.
+
+    Parameters
+    ----------
+    vectors : tuple of np.ndarray
+        Sets of vectors to match.
+        Each variable must be shape (n_vectors, n_channels).
+    comparison : str, optional
+        Must be :code:`'correlation' or :code:`'cosine_similarity'`.
+    return_order : bool, optional
+        Should we return the order instead of the matched vectors?
+
+    Returns
+    -------
+    matched_vectors : tuple of np.ndarray
+        Set of matched vectors of shape (n_vectors, n_channels)
+        or order if :code:`return_order=True`.
+
+    Examples
+    --------
+    Reorder the vectors directly:
+
+    >>> v1, v2 = match_vectors(v1, v2, comparison="correlation")
+
+    Just get the reordering:
+
+    >>> orders = match_vectors(v1, v2, comparison="correlation", return_order=True)
+    >>> print(orders[0])  # order for v1 (always unchanged)
+    >>> print(orders[1])  # order for v2
+    """
+    # Validation
+    for vector in vectors[1:]:
+        if vector.shape != vectors[0].shape:
+            raise ValueError("Vectors must have the same shape.")
+
+    if comparison not in ["correlation", "cosine_similarity"]:
+        raise ValueError("Comparison must be 'correlation' or 'cosine_similarity'.")
+
+    # Number of arguments and number of vectors in each argument passed
+    n_args = len(vectors)
+    n_vectors = vectors[0].shape[0]
+
+    # Calculate the similarity between vectors
+    F = np.empty([n_vectors, n_vectors])
+    matched_vectors = [vectors[0]]
+    orders = [np.arange(vectors[0].shape[0])]
+    for i in range(1, n_args):
+        for j in range(n_vectors):
+            # Find the vector that is most similar to vector j
+            for k in range(n_vectors):
+                if comparison == "correlation":
+                    F[j, k] = -np.corrcoef(vectors[i][k], vectors[0][j])[0, 1]
+                elif comparison == "cosine_similarity":
+                    F[j, k] = -(
+                        1 - spatial.distance.cosine(vectors[i][k], vectors[0][j])
+                    )
+        order = optimize.linear_sum_assignment(F)[1]
+
+        # Add the ordered vector to the list
+        matched_vectors.append(vectors[i][order])
+        orders.append(order)
+
+    if return_order:
+        return orders
+    else:
+        return tuple(matched_vectors)
+
+
 def match_modes(*mode_time_courses, return_order=False):
     """Find correlated modes between mode time courses.
 
     Given N mode time courses and using the first given mode time course as a
     basis, find the best matches for modes between all of the mode time courses.
     Once found, the mode time courses are returned with the modes reordered so
     that the modes match.
@@ -352,15 +420,15 @@
     for mode_time_course in mode_time_courses[1:]:
         correlation = correlate_modes(
             mode_time_courses[0][:n_samples], mode_time_course[:n_samples]
         )
         correlation = np.nan_to_num(
             np.nan_to_num(correlation, nan=np.nanmin(correlation) - 1)
         )
-        matches = linear_sum_assignment(-correlation)
+        matches = optimize.linear_sum_assignment(-correlation)
         matched_mode_time_courses.append(mode_time_course[:n_samples, matches[1]])
         orders.append(matches[1])
 
     if return_order:
         return orders
     else:
         return matched_mode_time_courses
@@ -561,28 +629,54 @@
         Mode covariances. Shape must be (n_modes, n_channels, n_channels).
 
     Returns
     -------
     reweighted_alpha : list of np.ndarray or np.ndarray
         Re-weighted mixing coefficients. Shape is the same as :code:`alpha`.
     """
-    if isinstance(alpha, np.ndarray):
-        alpha = [alpha]
+    return reweight_mtc(alpha, covs, "covariance")
 
-    # Calculate normalised alphas
-    traces = np.trace(covs, axis1=1, axis2=2)
-    reweighted_alpha = [a * traces[np.newaxis, :] for a in alpha]
-    reweighted_alpha = [
-        na / np.sum(na, axis=1, keepdims=True) for na in reweighted_alpha
-    ]
 
-    if len(reweighted_alpha) == 1:
-        reweighted_alpha = reweighted_alpha[0]
+def reweight_mtc(mtc, params, params_type):
+    """Re-weight mixing coefficients to account for the magnitude of
+    observation model parameters.
+
+    Parameters
+    ----------
+    mtc : List[np.ndarray] or np.ndarray
+        Raw mixing coefficients. Shape must be (n_sessions, n_samples, n_modes)
+        or (n_samples, n_modes).
+    params : np.ndarray
+        Observation model parameters. Shape must be (n_modes, n_channels, n_channels).
+    params_type : str
+        Observation model parameters type. Either 'covariance' or 'correlation'.
+
+    Returns
+    -------
+    reweighted_mtc : List[np.ndarray]
+        Re-weighted mixing coefficients. Shape is the same as :code:`mtc`.
+    """
+    if isinstance(mtc, np.ndarray):
+        mtc = [mtc]
+
+    if params_type == "covariance":
+        weights = np.trace(params, axis1=1, axis2=2)
+    elif params_type == "correlation":
+        m, n = np.tril_indices(params.shape[-1], -1)
+        weights = np.sum(np.abs(params[:, m, n]), axis=-1)
+    else:
+        raise ValueError("params_type must be 'covariance' or 'correlation'.")
+
+    reweighted_mtc = [x * weights[np.newaxis, :] for x in mtc]
+    reweighted_mtc = [x / np.sum(x, axis=1, keepdims=True) for x in reweighted_mtc]
+
+    if len(reweighted_mtc) == 1:
+        reweighted_mtc = reweighted_mtc[0]
 
-    return reweighted_alpha
+    return reweighted_mtc
 
 
 def average_runs(alpha, n_clusters=None, return_cluster_info=False):
     """Average the state probabilities from different runs using hierarchical clustering.
 
     Parameters
     ----------
@@ -653,15 +747,15 @@
     average_alpha = np.array(average_alpha, dtype=np.float32).T
 
     # Split average alphas back into session-specific time courses
     average_alpha = np.split(average_alpha, np.cumsum(n_session_samples[:-1]))
 
     if return_cluster_info:
         # Create a dictionary containing the clustering info
-        linkage = hierarchy.linkage(dissimilarity, method="ward")
+        linkage = cluster.hierarchy.linkage(dissimilarity, method="ward")
         cluster_info = {
             "correlation": corr,
             "dissimilarity": dissimilarity,
             "ids": cluster_ids,
             "linkage": linkage,
         }
         return average_alpha, cluster_info
```

### Comparing `osl-dynamics-1.3.1/osl_dynamics/inference/optimizers.py` & `osl_dynamics-1.3.2/osl_dynamics/inference/optimizers.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/inference/regularizers.py` & `osl_dynamics-1.3.2/osl_dynamics/inference/regularizers.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/inference/tf_ops.py` & `osl_dynamics-1.3.2/osl_dynamics/inference/tf_ops.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/models/__init__.py` & `osl_dynamics-1.3.2/osl_dynamics/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 
 """
 
 import yaml
 
 from osl_dynamics.models import (
     dynemo,
+    simplified_dynemo,
     mage,
     sage,
     mdynemo,
     state_dynemo,
     hmm,
     hmm_poi,
     hive,
     dive,
 )
-from osl_dynamics.utils.misc import NumpyLoader
+from osl_dynamics.utils import misc
 
 models = {
     "DyNeMo": dynemo.Model,
+    "Simplified-DyNeMo": simplified_dynemo.Model,
     "MAGE": mage.Model,
     "SAGE": sage.Model,
     "M-DyNeMo": mdynemo.Model,
     "State-DyNeMo": state_dynemo.Model,
     "HMM": hmm.Model,
     "HMM-Poisson": hmm_poi.Model,
     "HIVE": hive.Model,
@@ -42,15 +44,15 @@
 
     Returns
     -------
     model : DyNeMo model
         Model object.
     """
     with open(f"{dirname}/config.yml", "r") as file:
-        config_dict = yaml.load(file, NumpyLoader)
+        config_dict = yaml.load(file, misc.NumpyLoader)
 
     if "model_name" not in config_dict:
         raise ValueError(
             "Either use a specific `Model.load` method or "
             + "provide a `model_name` field in config"
         )
```

### Comparing `osl-dynamics-1.3.1/osl_dynamics/models/dive.py` & `osl_dynamics-1.3.2/osl_dynamics/models/dive.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from dataclasses import dataclass
 
 import numpy as np
 import tensorflow as tf
 import tensorflow_probability as tfp
 from tensorflow.keras import layers
 
-import osl_dynamics.data.tf as dtf
 from osl_dynamics.models import obs_mod
 from osl_dynamics.models.mod_base import BaseModelConfig
 from osl_dynamics.models.inf_mod_base import (
     VariationalInferenceModelConfig,
     VariationalInferenceModelBase,
 )
 import osl_dynamics.inference.initializers as osld_initializers
@@ -27,33 +26,33 @@
     NormalizationLayer,
     KLDivergenceLayer,
     KLLossLayer,
     SampleNormalDistributionLayer,
     SampleGammaDistributionLayer,
     SoftmaxLayer,
     ConcatEmbeddingsLayer,
-    SessionMapLayer,
+    SessionParamLayer,
     MixSessionSpecificParametersLayer,
     ZeroLayer,
     InverseCholeskyLayer,
     GammaExponentialKLDivergenceLayer,
     MultiLayerPerceptronLayer,
     LearnableTensorLayer,
     StaticLossScalingFactorLayer,
     BatchSizeLayer,
-    TFGatherLayer,
     AddLayer,
-    ConstrainedEmbeddingLayer,
+    TFConstantLayer,
+    EmbeddingLayer,
 )
 from osl_dynamics.data import SessionLabels
 
 
 @dataclass
 class Config(BaseModelConfig, VariationalInferenceModelConfig):
-    """Settings for SE-DyNeMo.
+    """Settings for DIVE.
 
     Parameters
     ----------
     model_name : str
         Model name.
 
     n_modes : int
@@ -151,14 +150,16 @@
 
     n_sessions : int
         Number of sessions whose observation model parameters can vary.
     embeddings_dim : int
         Number of dimensions for the embedding vectors.
     spatial_embeddings_dim : int
         Number of dimensions for the spatial embeddings.
+    unit_norm_embeddings : bool
+        Should we normalize the embeddings to have unit norm?
 
     dev_n_layers : int
         Number of layers for the MLP for deviations.
     dev_n_units : int
         Number of units for the MLP for deviations.
     dev_normalization : str
         Type of normalization for the MLP for deviations.
@@ -207,14 +208,15 @@
     means_regularizer: tf.keras.regularizers.Regularizer = None
     covariances_regularizer: tf.keras.regularizers.Regularizer = None
 
     # Parameters specific to embedding model
     n_sessions: int = None
     embeddings_dim: int = None
     spatial_embeddings_dim: int = None
+    unit_norm_embeddings: bool = False
 
     dev_n_layers: int = 0
     dev_n_units: int = None
     dev_normalization: str = None
     dev_activation: str = None
     dev_dropout: float = 0.0
     dev_regularizer: str = None
@@ -363,19 +365,15 @@
         Returns
         -------
         summed_embeddings : np.ndarray
             Summed embeddings. Shape is (n_sessions, embeddings_dim).
         """
         return obs_mod.get_summed_embeddings(self.model, self.config.session_labels)
 
-    def get_session_means_covariances(
-        self,
-        embeddings=None,
-        n_neighbours=2,
-    ):
+    def get_session_means_covariances(self):
         """Get the means and covariances for each session.
 
         Returns
         -------
         session_means : np.ndarray
             Mode means for each session.
             Shape is (n_sessions, n_modes, n_channels).
@@ -519,15 +517,15 @@
         self.set_group_means_covariances(
             group_observation_model_parameters[0],
             group_observation_model_parameters[1],
             update_initializer=update_initializer,
         )
 
     def random_subject_initialization(self, **kwargs):
-        """random subject initialisation not compatible with SE-DyNeMo."""
+        """random subject initialisation not compatible with DIVE."""
         raise AttributeError(
             " 'Model' object has no attribute 'random_subject_initialization'."
         )
 
 
 def _model_structure(config):
     # Inputs
@@ -541,59 +539,51 @@
 
     # Static loss scaling factor
     static_loss_scaling_factor_layer = StaticLossScalingFactorLayer(
         name="static_loss_scaling_factor"
     )
     static_loss_scaling_factor = static_loss_scaling_factor_layer(data)
 
-    # Session labels input
-    session_labels = []
+    session_id = layers.Input(
+        shape=(config.sequence_length,),
+        dtype=tf.int32,
+        name="session_id",
+    )
+    session_label_layers = dict()
+    session_labels = dict()
+    label_embeddings_layers = dict()
+    label_embeddings = []
     for session_label in config.session_labels:
-        session_labels.append(
-            layers.Input(
-                shape=(config.sequence_length,),
-                dtype=(
-                    tf.int32
-                    if session_label.label_type == "categorical"
-                    else tf.float32
-                ),
-                name=session_label.name,
+        session_label_layers[session_label.name] = TFConstantLayer(
+            values=session_label.values,
+            name=f"{session_label.name}_constant",
+        )
+        session_labels[session_label.name] = session_label_layers[session_label.name](
+            data
+        )
+        label_embeddings_layers[session_label.name] = (
+            EmbeddingLayer(
+                session_label.n_classes,
+                config.embeddings_dim,
+                config.unit_norm_embeddings,
+                name=f"{session_label.name}_embeddings",
             )
-        )
-
-    session_label_embeddings_layers = []
-    for session_label in config.session_labels:
-        if session_label.label_type == "categorical":
-            session_label_embeddings_layers.append(
-                ConstrainedEmbeddingLayer(
-                    session_label.n_classes,
-                    config.embeddings_dim,
-                    name=f"{session_label.name}_embeddings",
-                )
+            if session_label.label_type == "categorical"
+            else layers.Dense(
+                config.embeddings_dim, name=f"{session_label.name}_embeddings"
             )
-        else:
-            session_label_embeddings_layers.append(
-                layers.Dense(
-                    config.embeddings_dim, name=f"{session_label.name}_embeddings"
-                ),
+        )
+        label_embeddings.append(
+            label_embeddings_layers[session_label.name](
+                session_labels[session_label.name]
             )
-
-    tf_gather_0_layer = TFGatherLayer(axis=0)
-    tf_gather_1_layer = TFGatherLayer(axis=1)
-    session_label_embeddings = []
-    # session_label_embeddings[0].shape = (None, embeddings_dim)
-    for session_label, session_label_embeddings_layer in zip(
-        session_labels, session_label_embeddings_layers
-    ):
-        session_label_embeddings.append(
-            session_label_embeddings_layer(tf_gather_1_layer([session_label, 0]))
         )
 
     embeddings_layer = AddLayer(name="embeddings")
-    embeddings = embeddings_layer(session_label_embeddings)
+    embeddings = embeddings_layer(label_embeddings)
 
     # Inference RNN:
     # Layer definitions
     inference_input_dropout_layer = layers.Dropout(
         config.inference_dropout, name="data_drop"
     )
     inference_output_layer = InferenceRNNLayer(
@@ -673,15 +663,14 @@
         means_spatial_embeddings_layer = layers.Dense(
             config.spatial_embeddings_dim,
             name="means_spatial_embeddings",
         )
         means_concat_embeddings_layer = ConcatEmbeddingsLayer(
             name="means_concat_embeddings",
         )
-
         means_dev_decoder_layer = MultiLayerPerceptronLayer(
             config.dev_n_layers,
             config.dev_n_units,
             config.dev_normalization,
             config.dev_activation,
             config.dev_dropout,
             config.dev_regularizer,
@@ -720,48 +709,50 @@
         )
         means_dev_mag_layer = SampleGammaDistributionLayer(
             config.covariances_epsilon, config.do_kl_annealing, name="means_dev_mag"
         )
 
         means_dev_layer = layers.Multiply(name="means_dev")
 
-        # Data flow to get the means deviations
+        # Data flow to get mean deviations
 
         # Get the concatenated embeddings
         means_spatial_embeddings = means_spatial_embeddings_layer(group_mu)
         means_concat_embeddings = means_concat_embeddings_layer(
             [embeddings, means_spatial_embeddings]
-        )  # shape = (None, n_modes, embeddings_dim + spatial_embeddings_dim)
+        )  # shape = (n_sessions, n_modes, embeddings_dim + spatial_embeddings_dim)
 
         # Get the mean deviation maps (no global magnitude information)
         means_dev_decoder = means_dev_decoder_layer(
             means_concat_embeddings,
             static_loss_scaling_factor=static_loss_scaling_factor,
         )
         means_dev_map = means_dev_map_layer(means_dev_decoder)
-        norm_means_dev_map = norm_means_dev_map_layer(means_dev_map)
-        # norm_means_dev_map.shape = (None, n_modes, n_channels)
+        norm_means_dev_map = tf.gather(
+            norm_means_dev_map_layer(means_dev_map),
+            session_id[:, 0],
+            axis=0,
+        )
+        # shape = (None, n_modes, n_channels)
 
         # Get the deviation magnitudes (scale deviation maps globally)
         means_dev_mag_inf_alpha_input = means_dev_mag_inf_alpha_input_layer(data)
-        means_dev_mag_inf_alpha_input = tf_gather_0_layer(
-            [means_dev_mag_inf_alpha_input, tf_gather_1_layer([session_labels[0], 0])]
-        )
         means_dev_mag_inf_alpha = means_dev_mag_inf_alpha_layer(
             means_dev_mag_inf_alpha_input
         )
         means_dev_mag_inf_beta_input = means_dev_mag_inf_beta_input_layer(data)
-        means_dev_mag_inf_beta_input = tf_gather_0_layer(
-            [means_dev_mag_inf_beta_input, tf_gather_1_layer([session_labels[0], 0])]
-        )
         means_dev_mag_inf_beta = means_dev_mag_inf_beta_layer(
             means_dev_mag_inf_beta_input
         )
         means_dev_mag = means_dev_mag_layer(
-            [means_dev_mag_inf_alpha, means_dev_mag_inf_beta]
+            [
+                means_dev_mag_inf_alpha,
+                means_dev_mag_inf_beta,
+                session_id,
+            ]
         )
         means_dev = means_dev_layer([means_dev_mag, norm_means_dev_map])
     else:
         means_dev_layer = ZeroLayer(
             shape=(config.n_modes, config.n_channels),
             name="means_dev",
         )
@@ -840,31 +831,34 @@
 
         # Get the covariance deviation maps (no global magnitude information)
         covs_dev_decoder = covs_dev_decoder_layer(
             covs_concat_embeddings,
             static_loss_scaling_factor=static_loss_scaling_factor,
         )
         covs_dev_map = covs_dev_map_layer(covs_dev_decoder)
-        norm_covs_dev_map = norm_covs_dev_map_layer(covs_dev_map)
+        norm_covs_dev_map = tf.gather(
+            norm_covs_dev_map_layer(covs_dev_map),
+            session_id[:, 0],
+            axis=0,
+        )
 
         # Get the deviation magnitudes (scale deviation maps globally)
         covs_dev_mag_inf_alpha_input = covs_dev_mag_inf_alpha_input_layer(data)
-        covs_dev_mag_inf_alpha_input = tf_gather_0_layer(
-            [covs_dev_mag_inf_alpha_input, tf_gather_1_layer([session_labels[0], 0])]
-        )
         covs_dev_mag_inf_alpha = covs_dev_mag_inf_alpha_layer(
             covs_dev_mag_inf_alpha_input
         )
         covs_dev_mag_inf_beta_input = covs_dev_mag_inf_beta_input_layer(data)
-        covs_dev_mag_inf_beta_input = tf_gather_0_layer(
-            [covs_dev_mag_inf_beta_input, tf_gather_1_layer([session_labels[0], 0])]
-        )
         covs_dev_mag_inf_beta = covs_dev_mag_inf_beta_layer(covs_dev_mag_inf_beta_input)
+
         covs_dev_mag = covs_dev_mag_layer(
-            [covs_dev_mag_inf_alpha, covs_dev_mag_inf_beta]
+            [
+                covs_dev_mag_inf_alpha,
+                covs_dev_mag_inf_beta,
+                session_id,
+            ]
         )
         # covs_dev_mag.shape = (None, n_modes, 1)
         covs_dev = covs_dev_layer([covs_dev_mag, norm_covs_dev_map])
         # covs_dev.shape = (None, n_modes, n_channels * (n_channels + 1) // 2)
     else:
         covs_dev_layer = ZeroLayer(
             shape=(
@@ -882,24 +876,28 @@
             ),
         )
 
     # ----------------------------------------
     # Add deviations to group level parameters
 
     # Layer definitions
-    session_means_layer = SessionMapLayer(
+    session_means_layer = SessionParamLayer(
         "means", config.covariances_epsilon, name="session_means"
     )
-    session_covs_layer = SessionMapLayer(
+    session_covs_layer = SessionParamLayer(
         "covariances", config.covariances_epsilon, name="session_covs"
     )
 
     # Data flow
-    mu = session_means_layer([group_mu, means_dev])
-    D = session_covs_layer([group_D, covs_dev])
+    mu = session_means_layer(
+        [group_mu, means_dev]
+    )  # shape = (None, n_modes, n_channels)
+    D = session_covs_layer(
+        [group_D, covs_dev]
+    )  # shape = (None, n_modes, n_channels, n_channels)
 
     # -----------------------------------
     # Mix the session specific paraemters
     # and get the conditional likelihood
 
     # Layer definitions
     mix_session_means_covs_layer = MixSessionSpecificParametersLayer(
@@ -962,14 +960,15 @@
         means_dev_mag_mod_beta = means_dev_mag_mod_beta_layer(means_dev_decoder)
         means_dev_mag_kl_loss = means_dev_mag_kl_loss_layer(
             [
                 means_dev_mag_inf_alpha,
                 means_dev_mag_inf_beta,
                 means_dev_mag_mod_beta,
             ],
+            static_loss_scaling_factor=static_loss_scaling_factor,
         )
     else:
         means_dev_mag_kl_loss_layer = ZeroLayer(
             (),
             name="means_dev_mag_kl_loss",
         )
         means_dev_mag_kl_loss = means_dev_mag_kl_loss_layer(data)
@@ -992,14 +991,15 @@
         )
         covs_dev_mag_kl_loss = covs_dev_mag_kl_loss_layer(
             [
                 covs_dev_mag_inf_alpha,
                 covs_dev_mag_inf_beta,
                 covs_dev_mag_mod_beta,
             ],
+            static_loss_scaling_factor=static_loss_scaling_factor,
         )
     else:
         covs_dev_mag_kl_loss_layer = ZeroLayer((), name="covs_dev_mag_kl_loss")
         covs_dev_mag_kl_loss = covs_dev_mag_kl_loss_layer(data)
 
     # Total KL loss
     # Layer definitions
@@ -1007,11 +1007,11 @@
 
     # Data flow
     kl_loss = kl_loss_layer(
         [kl_div, means_dev_mag_kl_loss, covs_dev_mag_kl_loss],
     )
 
     return tf.keras.Model(
-        inputs=[data] + session_labels,
+        inputs=[data, session_id],
         outputs=[ll_loss, kl_loss, theta_norm],
         name="DIVE",
     )
```

### Comparing `osl-dynamics-1.3.1/osl_dynamics/models/dynemo.py` & `osl_dynamics-1.3.2/osl_dynamics/models/dynemo.py`

 * *Files 2% similar despite different names*

```diff
@@ -618,35 +618,30 @@
 
         return np.array(means), np.array(covariances)
 
     def _select_covariance_layer(self):
         """Select the covariance layer based on the config."""
         config = self.config
         if config.diagonal_covariances:
-            return DiagonalMatricesLayer(
-                config.n_modes,
-                config.n_channels,
-                config.learn_covariances,
-                config.initial_covariances,
-                config.covariances_epsilon,
-                config.covariances_regularizer,
-                name="covs",
-            )
-        return CovarianceMatricesLayer(
-            config.n_modes,
+            CovsLayer = DiagonalMatricesLayer
+        else:
+            CovsLayer = CovarianceMatricesLayer
+        return CovsLayer(
+            config.n_modes or config.n_states,
             config.n_channels,
             config.learn_covariances,
             config.initial_covariances,
             config.covariances_epsilon,
             config.covariances_regularizer,
             name="covs",
         )
 
     def _model_structure(self):
         """Build the model structure."""
+
         config = self.config
 
         # Layer for input
         inputs = layers.Input(
             shape=(config.sequence_length, config.n_channels), name="data"
         )
 
@@ -766,9 +761,11 @@
         mod_rnn = mod_rnn_layer(theta_norm_drop)
         mod_mu = mod_mu_layer(mod_rnn)
         mod_sigma = mod_sigma_layer(mod_rnn)
         kl_div = kl_div_layer([inf_mu, inf_sigma, mod_mu, mod_sigma])
         kl_loss = kl_loss_layer(kl_div)
 
         return tf.keras.Model(
-            inputs=inputs, outputs=[ll_loss, kl_loss, theta_norm], name="DyNeMo"
+            inputs=inputs,
+            outputs=[ll_loss, kl_loss, theta_norm],
+            name=config.model_name,
         )
```

### Comparing `osl-dynamics-1.3.1/osl_dynamics/models/hive.py` & `osl_dynamics-1.3.2/osl_dynamics/models/hive.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 import tensorflow_probability as tfp
 from tensorflow.keras import layers
 
 from osl_dynamics.inference.layers import (
     VectorsLayer,
     CovarianceMatricesLayer,
     ConcatEmbeddingsLayer,
-    SessionMapLayer,
+    SessionParamLayer,
     ZeroLayer,
     InverseCholeskyLayer,
     SampleGammaDistributionLayer,
     GammaExponentialKLDivergenceLayer,
     KLLossLayer,
     MultiLayerPerceptronLayer,
     StaticLossScalingFactorLayer,
     HiddenMarkovStateInferenceLayer,
     SeparateLogLikelihoodLayer,
     SumLogLikelihoodLossLayer,
     LearnableTensorLayer,
     BatchSizeLayer,
-    TFGatherLayer,
     AddLayer,
-    ConstrainedEmbeddingLayer,
+    TFConstantLayer,
+    EmbeddingLayer,
 )
 from osl_dynamics.models import obs_mod
 from osl_dynamics.models.mod_base import BaseModelConfig
 from osl_dynamics.inference import callbacks
 from osl_dynamics.inference import initializers as osld_initializers
 from osl_dynamics.models.inf_mod_base import (
     MarkovStateInferenceModelConfig,
@@ -74,14 +74,16 @@
 
     n_sessions : int
         Number of sessions whose observation model parameters can vary.
     embeddings_dim : int
         Number of dimensions for embeddings dimension.
     spatial_embeddings_dim : int
         Number of dimensions for spatial embeddings.
+    unit_norm_embeddings : bool
+        Should we normalize the embeddings to have unit norm?
 
     dev_n_layers : int
         Number of layers for the MLP for deviations.
     dev_n_units : int
         Number of units for the MLP for deviations.
     dev_normalization : str
         Type of normalization for the MLP for deviations.
@@ -148,14 +150,15 @@
 
     model_name: str = "HIVE"
 
     # Parameters specific to embedding model
     n_sessions: int = None
     embeddings_dim: int = None
     spatial_embeddings_dim: int = None
+    unit_norm_embeddings: bool = False
 
     # Observation model parameters
     learn_means: bool = None
     learn_covariances: bool = None
     initial_means: np.ndarray = None
     initial_covariances: np.ndarray = None
     covariances_epsilon: float = None
@@ -329,14 +332,22 @@
 
     def reset_kl_annealing_factor(self):
         """Reset the KL annealing factor."""
         if self.config.do_kl_annealing:
             kl_loss_layer = self.model.get_layer("kl_loss")
             kl_loss_layer.annealing_factor.assign(0.0)
 
+            if "means_dev_mag" in self.model.layers:
+                means_dev_mag_layer = self.model.get_layer("means_dev_mag")
+                means_dev_mag_layer.annealing_factor.assign(0.0)
+
+            if "covs_dev_mag" in self.model.layers:
+                covs_dev_mag_layer = self.model.get_layer("covs_dev_mag")
+                covs_dev_mag_layer.annealing_factor.assign(0.0)
+
     def get_group_means(self):
         """Get the group level state means.
 
         Returns
         -------
         means : np.ndarray
             Group means. Shape is (n_states, n_channels).
@@ -613,60 +624,52 @@
 
     # Static loss scaling factor
     static_loss_scaling_factor_layer = StaticLossScalingFactorLayer(
         name="static_loss_scaling_factor"
     )
     static_loss_scaling_factor = static_loss_scaling_factor_layer(data)
 
-    # Session labels input
-    session_labels = []
+    session_id = layers.Input(
+        shape=(config.sequence_length,),
+        dtype=tf.int32,
+        name="session_id",
+    )
+    session_label_layers = dict()
+    session_labels = dict()
+    label_embeddings_layers = dict()
+    label_embeddings = []
     for session_label in config.session_labels:
-        session_labels.append(
-            layers.Input(
-                shape=(config.sequence_length,),
-                dtype=(
-                    tf.int32
-                    if session_label.label_type == "categorical"
-                    else tf.float32
-                ),
-                name=session_label.name,
+        session_label_layers[session_label.name] = TFConstantLayer(
+            values=session_label.values,
+            name=f"{session_label.name}_constant",
+        )
+        session_labels[session_label.name] = session_label_layers[session_label.name](
+            data
+        )
+        label_embeddings_layers[session_label.name] = (
+            EmbeddingLayer(
+                session_label.n_classes,
+                config.embeddings_dim,
+                config.unit_norm_embeddings,
+                name=f"{session_label.name}_embeddings",
             )
-        )
-
-    session_label_embeddings_layers = []
-    for session_label in config.session_labels:
-        if session_label.label_type == "categorical":
-            session_label_embeddings_layers.append(
-                ConstrainedEmbeddingLayer(
-                    session_label.n_classes,
-                    config.embeddings_dim,
-                    name=f"{session_label.name}_embeddings",
-                )
+            if session_label.label_type == "categorical"
+            else layers.Dense(
+                config.embeddings_dim, name=f"{session_label.name}_embeddings"
             )
-        else:
-            session_label_embeddings_layers.append(
-                layers.Dense(
-                    config.embeddings_dim, name=f"{session_label.name}_embeddings"
-                ),
+        )
+        label_embeddings.append(
+            label_embeddings_layers[session_label.name](
+                session_labels[session_label.name]
             )
-
-    tf_gather_0_layer = TFGatherLayer(axis=0)
-    tf_gather_1_layer = TFGatherLayer(axis=1)
-    session_label_embeddings = []
-    # session_label_embeddings[0].shape = (None, embeddings_dim)
-    for session_label, session_label_embeddings_layer in zip(
-        session_labels, session_label_embeddings_layers
-    ):
-        session_label_embeddings.append(
-            session_label_embeddings_layer(tf_gather_1_layer([session_label, 0]))
         )
 
     embeddings_layer = AddLayer(name="embeddings")
-    embeddings = embeddings_layer(session_label_embeddings)
-    # embeddings.shape = (None, embeddings_dim)
+    embeddings = embeddings_layer(label_embeddings)
+    # embeddings.shape = (n_sessions, embeddings_dim)
 
     # Group level observation model parameters
     group_means_layer = VectorsLayer(
         config.n_states,
         config.n_channels,
         config.learn_means,
         config.initial_means,
@@ -750,42 +753,44 @@
 
         # Data flow to get mean deviations
 
         # Get the concatenated embeddings
         means_spatial_embeddings = means_spatial_embeddings_layer(group_mu)
         means_concat_embeddings = means_concat_embeddings_layer(
             [embeddings, means_spatial_embeddings]
-        )  # shape = (None, n_states, embeddings_dim + spatial_embeddings_dim)
+        )  # shape = (n_sessions, n_states, embeddings_dim + spatial_embeddings_dim)
 
         # Get the mean deviation maps (no global magnitude information)
         means_dev_decoder = means_dev_decoder_layer(
             means_concat_embeddings,
             static_loss_scaling_factor=static_loss_scaling_factor,
         )
         means_dev_map = means_dev_map_layer(means_dev_decoder)
-        norm_means_dev_map = norm_means_dev_map_layer(means_dev_map)
-        # norm_means_dev_map.shape = (None, n_states, n_channels)
+        norm_means_dev_map = tf.gather(
+            norm_means_dev_map_layer(means_dev_map),
+            session_id[:, 0],
+            axis=0,
+        )
+        # shape = (None, n_states, n_channels)
 
         # Get the deviation magnitudes (scale deviation maps globally)
         means_dev_mag_inf_alpha_input = means_dev_mag_inf_alpha_input_layer(data)
-        means_dev_mag_inf_alpha_input = tf_gather_0_layer(
-            [means_dev_mag_inf_alpha_input, tf_gather_1_layer([session_labels[0], 0])]
-        )
         means_dev_mag_inf_alpha = means_dev_mag_inf_alpha_layer(
             means_dev_mag_inf_alpha_input
         )
         means_dev_mag_inf_beta_input = means_dev_mag_inf_beta_input_layer(data)
-        means_dev_mag_inf_beta_input = tf_gather_0_layer(
-            [means_dev_mag_inf_beta_input, tf_gather_1_layer([session_labels[0], 0])]
-        )
         means_dev_mag_inf_beta = means_dev_mag_inf_beta_layer(
             means_dev_mag_inf_beta_input
         )
         means_dev_mag = means_dev_mag_layer(
-            [means_dev_mag_inf_alpha, means_dev_mag_inf_beta]
+            [
+                means_dev_mag_inf_alpha,
+                means_dev_mag_inf_beta,
+                session_id,
+            ]
         )
         means_dev = means_dev_layer([means_dev_mag, norm_means_dev_map])
     else:
         means_dev_layer = ZeroLayer(
             shape=(config.n_states, config.n_channels),
             name="means_dev",
         )
@@ -864,31 +869,34 @@
 
         # Get the covariance deviation maps (no global magnitude information)
         covs_dev_decoder = covs_dev_decoder_layer(
             covs_concat_embeddings,
             static_loss_scaling_factor=static_loss_scaling_factor,
         )
         covs_dev_map = covs_dev_map_layer(covs_dev_decoder)
-        norm_covs_dev_map = norm_covs_dev_map_layer(covs_dev_map)
+        norm_covs_dev_map = tf.gather(
+            norm_covs_dev_map_layer(covs_dev_map),
+            session_id[:, 0],
+            axis=0,
+        )
 
         # Get the deviation magnitudes (scale deviation maps globally)
         covs_dev_mag_inf_alpha_input = covs_dev_mag_inf_alpha_input_layer(data)
-        covs_dev_mag_inf_alpha_input = tf_gather_0_layer(
-            [covs_dev_mag_inf_alpha_input, tf_gather_1_layer([session_labels[0], 0])]
-        )
         covs_dev_mag_inf_alpha = covs_dev_mag_inf_alpha_layer(
             covs_dev_mag_inf_alpha_input
         )
         covs_dev_mag_inf_beta_input = covs_dev_mag_inf_beta_input_layer(data)
-        covs_dev_mag_inf_beta_input = tf_gather_0_layer(
-            [covs_dev_mag_inf_beta_input, tf_gather_1_layer([session_labels[0], 0])]
-        )
         covs_dev_mag_inf_beta = covs_dev_mag_inf_beta_layer(covs_dev_mag_inf_beta_input)
+
         covs_dev_mag = covs_dev_mag_layer(
-            [covs_dev_mag_inf_alpha, covs_dev_mag_inf_beta]
+            [
+                covs_dev_mag_inf_alpha,
+                covs_dev_mag_inf_beta,
+                session_id,
+            ]
         )
         # covs_dev_mag.shape = (None, n_states, 1)
         covs_dev = covs_dev_layer([covs_dev_mag, norm_covs_dev_map])
         # covs_dev.shape = (None, n_states, n_channels * (n_channels + 1) // 2)
     else:
         covs_dev_layer = ZeroLayer(
             shape=(
@@ -906,18 +914,18 @@
             ),
         )
 
     # ----------------------------------------
     # Add deviations to group level parameters
 
     # Layer definitions
-    session_means_layer = SessionMapLayer(
+    session_means_layer = SessionParamLayer(
         "means", config.covariances_epsilon, name="session_means"
     )
-    session_covs_layer = SessionMapLayer(
+    session_covs_layer = SessionParamLayer(
         "covariances", config.covariances_epsilon, name="session_covs"
     )
 
     # Data flow
     mu = session_means_layer(
         [group_mu, means_dev]
     )  # shape = (None, n_states, n_channels)
@@ -970,14 +978,15 @@
         means_dev_mag_mod_beta = means_dev_mag_mod_beta_layer(means_dev_decoder)
         means_dev_mag_kl_loss = means_dev_mag_kl_loss_layer(
             [
                 means_dev_mag_inf_alpha,
                 means_dev_mag_inf_beta,
                 means_dev_mag_mod_beta,
             ],
+            static_loss_scaling_factor=static_loss_scaling_factor,
         )
     else:
         means_dev_mag_kl_loss_layer = ZeroLayer(
             (),
             name="means_dev_mag_kl_loss",
         )
         means_dev_mag_kl_loss = means_dev_mag_kl_loss_layer(data)
@@ -1000,24 +1009,25 @@
         )
         covs_dev_mag_kl_loss = covs_dev_mag_kl_loss_layer(
             [
                 covs_dev_mag_inf_alpha,
                 covs_dev_mag_inf_beta,
                 covs_dev_mag_mod_beta,
             ],
+            static_loss_scaling_factor=static_loss_scaling_factor,
         )
     else:
         covs_dev_mag_kl_loss_layer = ZeroLayer((), name="covs_dev_mag_kl_loss")
         covs_dev_mag_kl_loss = covs_dev_mag_kl_loss_layer(data)
 
     # Total KL loss
     # Layer definitions
     kl_loss_layer = KLLossLayer(do_annealing=config.do_kl_annealing, name="kl_loss")
 
     # Data flow
     kl_loss = kl_loss_layer([means_dev_mag_kl_loss, covs_dev_mag_kl_loss])
 
     return tf.keras.Model(
-        inputs=[data] + session_labels,
+        inputs=[data, session_id],
         outputs=[ll_loss, kl_loss, gamma, xi],
         name="HIVE",
     )
```

### Comparing `osl-dynamics-1.3.1/osl_dynamics/models/hmm.py` & `osl_dynamics-1.3.2/osl_dynamics/models/hmm.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 from osl_dynamics.models.mod_base import BaseModelConfig, ModelBase
 from osl_dynamics.simulation import HMM
 from osl_dynamics.utils.misc import set_logging_level
 
 _logger = logging.getLogger("osl-dynamics")
 
 warnings.filterwarnings("ignore", category=NumbaWarning)
+logging.getLogger("numba.core.transforms").setLevel(logging.ERROR)
 
 EPS = sys.float_info.epsilon
 
 
 @dataclass
 class Config(BaseModelConfig):
     """Settings for HMM.
@@ -178,15 +179,15 @@
     config : osl_dynamics.models.hmm.Config
     """
 
     config_type = Config
 
     def build_model(self):
         """Builds a keras model."""
-        self.model = _model_structure(self.config)
+        self.model = self._model_structure()
 
         self.rho = 1
         self.set_trans_prob(self.config.initial_trans_prob)
         self.set_state_probs_t0(self.config.state_probs_t0)
 
     def fit(self, dataset, epochs=None, use_tqdm=False, verbose=1, **kwargs):
         """Fit model to a dataset.
@@ -300,16 +301,18 @@
         :code:`"static_loss_scaling_factor"` layer.
 
         Parameters
         ----------
         dataset : tf.data.Dataset
             TensorFlow dataset.
         """
-        n_batches = dtf.get_n_batches(dataset)
-        self.model.get_layer("static_loss_scaling_factor").n_batches = n_batches
+        layer_names = [layer.name for layer in self.model.layers]
+        if "static_loss_scaling_factor" in layer_names:
+            n_batches = dtf.get_n_batches(dataset)
+            self.model.get_layer("static_loss_scaling_factor").n_batches = n_batches
 
     def random_subset_initialization(
         self, training_data, n_epochs, n_init, take, **kwargs
     ):
         """Random subset initialization.
 
         The model is trained for a few epochs with different random subsets
@@ -734,15 +737,15 @@
                 np.expand_dims(self.trans_prob, 0),
             )
         )
 
         return first_term + remaining_terms
 
     def get_log_likelihood(self, data):
-        """Get the log-likelihood of data, :math:`\log p(x_t | s_t)`.
+        r"""Get the log-likelihood of data, :math:`\log p(x_t | s_t)`.
 
         Parameters
         ----------
         data : np.ndarray
             Data. Shape is (batch_size, ..., n_channels).
 
         Returns
@@ -926,16 +929,15 @@
         """
 
         if state_probs_t0 is None:
             state_probs_t0 = np.ones((self.config.n_states,)) / self.config.n_states
         self.state_probs_t0 = state_probs_t0
 
     def set_random_state_time_course_initialization(self, training_dataset):
-        """Sets the initial means/covariances based on a random state time
-        course.
+        """Sets the initial means/covariances based on a random state time course.
 
         Parameters
         ----------
         training_dataset : tf.data.Dataset
             Training data.
         """
         _logger.info("Setting random means and covariances")
@@ -950,27 +952,33 @@
         )
 
         n_batches = 0
         for batch in training_dataset:
             # Concatenate all the sequences in this batch
             data = np.concatenate(batch["data"])
 
+            if data.shape[0] < 2 * self.config.n_channels:
+                raise ValueError(
+                    "Not enough time points in batch, "
+                    "increase batch_size or sequence_length"
+                )
+
             # Sample a state time course using the initial transition
             # probability matrix
             stc = self.sample_state_time_course(data.shape[0])
 
             # Make sure each state activates
-            non_active_states = np.sum(stc, axis=0) == 0
+            non_active_states = np.sum(stc, axis=0) < 2 * self.config.n_channels
             while np.any(non_active_states):
                 new_stc = self.sample_state_time_course(data.shape[0])
                 new_active_states = np.sum(new_stc, axis=0) != 0
                 for j in range(self.config.n_states):
                     if non_active_states[j] and new_active_states[j]:
                         stc[:, j] = new_stc[:, j]
-                non_active_states = np.sum(stc, axis=0) == 0
+                non_active_states = np.sum(stc, axis=0) < 2 * self.config.n_channels
 
             # Calculate the mean/covariance for each state for this batch
             m = []
             C = []
             for j in range(self.config.n_states):
                 x = data[stc[:, j] == 1]
                 mu = np.mean(x, axis=0)
@@ -1570,65 +1578,68 @@
         self.set_trans_prob(trans_prob)
 
     def reset_weights(self):
         """Resets trainable variables in the model to their initial value."""
         initializers.reinitialize_model_weights(self.model)
         self.set_trans_prob(self.config.initial_trans_prob)
 
+    def _model_structure(self):
+        """Build the model structure."""
 
-def _model_structure(config):
-    # Inputs
-    inputs = layers.Input(
-        shape=(config.sequence_length, config.n_channels + config.n_states),
-        name="inputs",
-    )
-    data, gamma = tf.split(inputs, [config.n_channels, config.n_states], axis=2)
-
-    # Static loss scaling factor
-    static_loss_scaling_factor_layer = StaticLossScalingFactorLayer(
-        name="static_loss_scaling_factor"
-    )
-    static_loss_scaling_factor = static_loss_scaling_factor_layer(data)
-
-    # Definition of layers
-    means_layer = VectorsLayer(
-        config.n_states,
-        config.n_channels,
-        config.learn_means,
-        config.initial_means,
-        config.means_regularizer,
-        name="means",
-    )
-    if config.diagonal_covariances:
-        covs_layer = DiagonalMatricesLayer(
-            config.n_states,
-            config.n_channels,
-            config.learn_covariances,
-            config.initial_covariances,
-            config.covariances_epsilon,
-            config.covariances_regularizer,
-            name="covs",
+        config = self.config
+
+        # Inputs
+        inputs = layers.Input(
+            shape=(config.sequence_length, config.n_channels + config.n_states),
+            name="inputs",
+        )
+        data, gamma = tf.split(inputs, [config.n_channels, config.n_states], axis=2)
+
+        # Static loss scaling factor
+        static_loss_scaling_factor_layer = StaticLossScalingFactorLayer(
+            name="static_loss_scaling_factor"
         )
-    else:
-        covs_layer = CovarianceMatricesLayer(
+        static_loss_scaling_factor = static_loss_scaling_factor_layer(data)
+
+        # Definition of layers
+        means_layer = VectorsLayer(
             config.n_states,
             config.n_channels,
-            config.learn_covariances,
-            config.initial_covariances,
-            config.covariances_epsilon,
-            config.covariances_regularizer,
-            name="covs",
+            config.learn_means,
+            config.initial_means,
+            config.means_regularizer,
+            name="means",
         )
-    ll_loss_layer = CategoricalLogLikelihoodLossLayer(
-        config.n_states, config.covariances_epsilon, name="ll_loss"
-    )
-
-    # Data flow
-    mu = means_layer(
-        data, static_loss_scaling_factor=static_loss_scaling_factor
-    )  # data not used
-    D = covs_layer(
-        data, static_loss_scaling_factor=static_loss_scaling_factor
-    )  # data not used
-    ll_loss = ll_loss_layer([data, mu, D, gamma, None])
+        if config.diagonal_covariances:
+            covs_layer = DiagonalMatricesLayer(
+                config.n_states,
+                config.n_channels,
+                config.learn_covariances,
+                config.initial_covariances,
+                config.covariances_epsilon,
+                config.covariances_regularizer,
+                name="covs",
+            )
+        else:
+            covs_layer = CovarianceMatricesLayer(
+                config.n_states,
+                config.n_channels,
+                config.learn_covariances,
+                config.initial_covariances,
+                config.covariances_epsilon,
+                config.covariances_regularizer,
+                name="covs",
+            )
+        ll_loss_layer = CategoricalLogLikelihoodLossLayer(
+            config.n_states, config.covariances_epsilon, name="ll_loss"
+        )
+
+        # Data flow
+        mu = means_layer(
+            data, static_loss_scaling_factor=static_loss_scaling_factor
+        )  # data not used
+        D = covs_layer(
+            data, static_loss_scaling_factor=static_loss_scaling_factor
+        )  # data not used
+        ll_loss = ll_loss_layer([data, mu, D, gamma, None])
 
-    return tf.keras.Model(inputs=inputs, outputs=[ll_loss], name="HMM")
+        return tf.keras.Model(inputs=inputs, outputs=[ll_loss], name="HMM")
```

### Comparing `osl-dynamics-1.3.1/osl_dynamics/models/hmm_poi.py` & `osl_dynamics-1.3.2/osl_dynamics/models/inf_mod_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,267 +1,169 @@
-"""Hidden Markov Model (HMM) with a Possion observation model.
+"""Base classes inference models.
 
 """
 
 import logging
-import os
-import os.path as op
-import sys
-import warnings
 from dataclasses import dataclass
-from pathlib import Path
+from typing import Literal
 
-import numba
 import numpy as np
 import tensorflow as tf
-import tensorflow_probability as tfp
-from tensorflow.keras import backend, layers, utils
-from numba.core.errors import NumbaWarning
-from scipy.special import logsumexp, xlogy
+from tensorflow.keras import utils
+from scipy.special import xlogy, logsumexp
 from tqdm.auto import trange
-from pqdm.threads import pqdm
 
 import osl_dynamics.data.tf as dtf
-from osl_dynamics.inference import initializers
-from osl_dynamics.inference.layers import (
-    CategoricalPoissonLogLikelihoodLossLayer,
-    VectorsLayer,
-    StaticLossScalingFactorLayer,
-)
-from osl_dynamics.models import obs_mod
-from osl_dynamics.models.mod_base import BaseModelConfig, ModelBase
 from osl_dynamics.simulation import HMM
-from osl_dynamics.utils.misc import set_logging_level
+from osl_dynamics.inference import callbacks, optimizers
+from osl_dynamics.inference.initializers import WeightInitializer
+from osl_dynamics.models.mod_base import ModelBase
+from osl_dynamics.utils.misc import replace_argument
 
 _logger = logging.getLogger("osl-dynamics")
 
-warnings.filterwarnings("ignore", category=NumbaWarning)
-
-EPS = sys.float_info.epsilon
-
 
 @dataclass
-class Config(BaseModelConfig):
-    """Settings for HMM.
-
-    Parameters
-    ----------
-    model_name : str
-        Model name.
-    n_states : int
-        Number of states.
-    n_channels : int
-        Number of channels.
-    sequence_length : int
-        Length of sequence passed to the inference network and generative model.
-
-    learn_log_rates : bool
-        Should we make :code:`log_rate` for each state trainable?
-    initial_log_rates : np.ndarray
-        Initialisation for state :code:`log_rates`.
-
-    initial_trans_prob : np.ndarray
-        Initialisation for the transition probability matrix.
-    learn_trans_prob : bool
-        Should we make the transition probability matrix trainable?
-    state_probs_t0: np.ndarray
-        State probabilities at :code:`time=0`. Not trainable.
-    observation_update_decay : float
-        Decay rate for the learning rate of the observation model.
-        We update the learning rate (:code:`lr`) as
-        :code:`lr = config.learning_rate * exp(-observation_update_decay *
-        epoch)`.
-
-    batch_size : int
-        Mini-batch size.
-    learning_rate : float
-        Learning rate.
-    trans_prob_update_delay : float
-        We update the transition probability matrix as
-        :code:`trans_prob = (1-rho) * trans_prob + rho * trans_prob_update`,
-        where :code:`rho = (100 * epoch / n_epochs + 1 +
-        trans_prob_update_delay) ** -trans_prob_update_forget`.
-        This is the delay parameter.
-    trans_prob_update_forget : float
-        We update the transition probability matrix as
-        :code:`trans_prob = (1-rho) * trans_prob + rho * trans_prob_update`,
-        where :code:`rho = (100 * epoch / n_epochs + 1 +
-        trans_prob_update_delay) ** -trans_prob_update_forget`.
-        This is the forget parameter.
-    n_epochs : int
-        Number of training epochs.
-    optimizer : str or tf.keras.optimizers.Optimizer
-        Optimizer to use.
-    multi_gpu : bool
-        Should be use multiple GPUs for training?
-    strategy : str
-        Strategy for distributed learning.
-    """
-
-    model_name: str = "HMM-Poisson"
-
-    # Observation model parameters
-    learn_log_rates: bool = None
-    initial_log_rates: np.ndarray = None
-
-    initial_trans_prob: np.ndarray = None
-    learn_trans_prob: bool = True
-    state_probs_t0: np.ndarray = None
-
-    # Learning rate schedule parameters
-    trans_prob_update_delay: float = 5  # alpha
-    trans_prob_update_forget: float = 0.7  # beta
-    observation_update_decay: float = 0.1
-
-    def __post_init__(self):
-        self.validate_observation_model_parameters()
-        self.validate_trans_prob_parameters()
-        self.validate_dimension_parameters()
-        self.validate_training_parameters()
-
-    def validate_observation_model_parameters(self):
-        if self.learn_log_rates is None:
-            raise ValueError("learn_log_rates must be passed.")
-
-    def validate_trans_prob_parameters(self):
-        if self.initial_trans_prob is not None:
-            if (
-                not isinstance(self.initial_trans_prob, np.ndarray)
-                or self.initial_trans_prob.ndim != 2
-            ):
-                raise ValueError("initial_trans_prob must be a 2D numpy array.")
-
-            if not all(np.isclose(np.sum(self.initial_trans_prob, axis=1), 1)):
-                raise ValueError("rows of initial_trans_prob must sum to one.")
+class VariationalInferenceModelConfig:
+    """Settings needed for the inference model."""
 
+    # Alpha parameters
+    theta_normalization: Literal[None, "batch", "layer"] = None
+    learn_alpha_temperature: bool = None
+    initial_alpha_temperature: float = None
+    theta_std_epsilon: float = 1e-6
+
+    # KL annealing parameters
+    do_kl_annealing: bool = False
+    kl_annealing_curve: Literal["linear", "tanh"] = None
+    kl_annealing_sharpness: float = None
+    n_kl_annealing_epochs: int = None
+
+    def validate_alpha_parameters(self):
+        if self.initial_alpha_temperature is None:
+            self.initial_alpha_temperature = 1.0
+
+        if self.initial_alpha_temperature <= 0:
+            raise ValueError("initial_alpha_temperature must be greater than zero.")
+
+    def validate_kl_annealing_parameters(self):
+        if self.do_kl_annealing:
+            if self.kl_annealing_curve is None:
+                raise ValueError(
+                    "If we are performing KL annealing, "
+                    "kl_annealing_curve must be passed."
+                )
 
-class Model(ModelBase):
-    """HMM class.
+            if self.kl_annealing_curve not in ["linear", "tanh"]:
+                raise ValueError("KL annealing curve must be 'linear' or 'tanh'.")
 
-    Parameters
-    ----------
-    config : osl_dynamics.models.hmm.Config
-    """
+            if self.kl_annealing_curve == "tanh":
+                if self.kl_annealing_sharpness is None:
+                    raise ValueError(
+                        "kl_annealing_sharpness must be passed if "
+                        "kl_annealing_curve='tanh'."
+                    )
 
-    config_type = Config
+                if self.kl_annealing_sharpness < 0:
+                    raise ValueError("KL annealing sharpness must be positive.")
 
-    def build_model(self):
-        """Builds a keras model."""
-        self.model = _model_structure(self.config)
+            if self.n_kl_annealing_epochs is None:
+                raise ValueError(
+                    "If we are performing KL annealing, "
+                    "n_kl_annealing_epochs must be passed."
+                )
 
-        self.rho = 1
-        self.set_trans_prob(self.config.initial_trans_prob)
-        self.set_state_probs_t0(self.config.state_probs_t0)
+            if self.n_kl_annealing_epochs < 1:
+                raise ValueError(
+                    "Number of KL annealing epochs must be greater than zero."
+                )
 
-    def fit(self, dataset, epochs=None, use_tqdm=False, verbose=1, **kwargs):
-        """Fit model to a dataset.
 
-        Iterates between:
+class VariationalInferenceModelBase(ModelBase):
+    """Base class for a variational inference model."""
 
-        - Baum-Welch updates of latent variable time courses and transition
-          probability matrix.
-        - TensorFlow updates of observation model parameters.
+    def fit(self, *args, kl_annealing_callback=None, lr_decay=None, **kwargs):
+        """Wrapper for the standard keras fit method.
 
         Parameters
         ----------
-        dataset : tf.data.Dataset or osl_dynamics.data.Data
-            Training dataset.
-        epochs : int, optional
-            Number of epochs.
-        use_tqdm : bool, optional
-            Should we use :code:`tqdm` to display a progress bar?
-        verbose : int, optional
-            Verbosity level. :code:`0=silent`.
-        kwargs : keyword arguments, optional
-            Keyword arguments for the TensorFlow observation model training.
-            These keywords arguments will be passed to :code:`self.model.fit()`.
+        *args : arguments
+            Arguments for :code:`ModelBase.fit()`.
+        kl_annealing_callback : bool, optional
+            Should we update the KL annealing factor during training?
+        lr_decay : float, optional
+            Learning rate decay after KL annealing period.
+        **kwargs : keyword arguments, optional
+            Keyword arguments for :code:`ModelBase.fit()`.
 
         Returns
         -------
-        history : dict
-            Dictionary with history of the loss and learning rates (:code:`lr`
-            and :code:`rho`).
+        history : history
+            The training history.
         """
-        if epochs is None:
-            epochs = self.config.n_epochs
-
-        # Make a TensorFlow Dataset
-        dataset = self.make_dataset(dataset, shuffle=True, concatenate=True)
+        # Validation
+        if lr_decay is None:
+            lr_decay = self.config.lr_decay
 
-        # Training curves
-        history = {"loss": [], "rho": [], "lr": []}
+        if kl_annealing_callback is None:
+            kl_annealing_callback = self.config.do_kl_annealing
 
-        # Loop through epochs
-        if use_tqdm:
-            _range = trange(epochs)
+        # Learning rate decay
+        if kl_annealing_callback:
+            decay_start_epoch = self.config.n_kl_annealing_epochs
         else:
-            _range = range(epochs)
-        for n in _range:
-            # Setup a progress bar for this epoch
-            if verbose > 0 and not use_tqdm:
-                print("Epoch {}/{}".format(n + 1, epochs))
-                pb_i = utils.Progbar(dtf.get_n_batches(dataset))
-
-            # Update rho
-            self._update_rho(n)
-
-            # Set learning rate for the observation model
-            lr = self.config.learning_rate * np.exp(
-                -self.config.observation_update_decay * n
-            )
-            backend.set_value(self.model.optimizer.lr, lr)
-
-            # Loop over batches
-            loss = []
-            for data in dataset:
-                x = data["data"]
-
-                # Update state probabilities
-                gamma, xi = self.get_posterior(x)
-
-                # Update transition probability matrix
-                if self.config.learn_trans_prob:
-                    self.update_trans_prob(gamma, xi)
-
-                # Reshape gamma: (batch_size*sequence_length, n_states)
-                # -> (batch_size, sequence_length, n_states)
-                gamma = gamma.reshape(x.shape[0], x.shape[1], -1)
-
-                # Update observation model
-                x_and_gamma = np.concatenate([x, gamma], axis=2)
-                h = self.model.fit(x_and_gamma, epochs=1, verbose=0, **kwargs)
-
-                # Get new loss
-                l = h.history["loss"][0]
-                if np.isnan(l):
-                    _logger.error("Training failed!")
-                    return
-                loss.append(l)
-
-                if verbose > 0:
-                    # Update progress bar
-                    if use_tqdm:
-                        _range.set_postfix(rho=self.rho, lr=lr, loss=l)
-                    else:
-                        pb_i.add(
-                            1,
-                            values=[("rho", self.rho), ("lr", lr), ("loss", l)],
-                        )
-
-            history["loss"].append(np.mean(loss))
-            history["rho"].append(self.rho)
-            history["lr"].append(lr)
+            decay_start_epoch = 0
+        learning_rate = self.config.learning_rate
 
-        if use_tqdm:
-            _range.close()
+        def lr_scheduler(epoch, lr):
+            if epoch < decay_start_epoch:
+                return learning_rate
+            else:
+                return learning_rate * np.exp(
+                    -lr_decay * (epoch - decay_start_epoch + 1)
+                )
 
-        return history
+        lr_callback = tf.keras.callbacks.LearningRateScheduler(lr_scheduler)
+        args, kwargs = replace_argument(
+            self.model.fit,
+            "callbacks",
+            [lr_callback],
+            args,
+            kwargs,
+            append=True,
+        )
+
+        # KL annealing
+        if kl_annealing_callback:
+            kl_annealing_callback = callbacks.KLAnnealingCallback(
+                curve=self.config.kl_annealing_curve,
+                annealing_sharpness=self.config.kl_annealing_sharpness,
+                n_annealing_epochs=self.config.n_kl_annealing_epochs,
+            )
+
+            # Update arguments to pass to the fit method
+            args, kwargs = replace_argument(
+                self.model.fit,
+                "callbacks",
+                [kl_annealing_callback],
+                args,
+                kwargs,
+                append=True,
+            )
+
+        return super().fit(*args, **kwargs)
 
     def random_subset_initialization(
-        self, training_data, n_epochs, n_init, take, **kwargs
+        self,
+        training_data,
+        n_epochs,
+        n_init,
+        take,
+        n_kl_annealing_epochs=None,
+        **kwargs,
     ):
         """Random subset initialization.
 
         The model is trained for a few epochs with different random subsets
         of the training dataset. The model with the best free energy is kept.
 
         Parameters
@@ -270,76 +172,220 @@
             Dataset to use for training.
         n_epochs : int
             Number of epochs to train the model.
         n_init : int
             Number of initializations.
         take : float
             Fraction of total batches to take.
+        n_kl_annealing_epochs : int, optional
+            Number of KL annealing epochs.
         kwargs : keyword arguments, optional
             Keyword arguments for the fit method.
 
         Returns
         -------
         history : history
             The training history of the best initialization.
         """
         if n_init is None or n_init == 0:
-            _logger.info(
+            _logger.warning(
                 "Number of initializations was set to zero. "
                 + "Skipping initialization."
             )
             return
 
         _logger.info("Random subset initialization")
 
-        # Get the buffer size
-        buffer_size = getattr(training_data, "buffer_size", 100000)
+        # Original number of KL annealing epochs
+        original_n_kl_annealing_epochs = self.config.n_kl_annealing_epochs
+
+        # Use n_kl_annealing_epochs if passed
+        self.config.n_kl_annealing_epochs = (
+            n_kl_annealing_epochs or original_n_kl_annealing_epochs
+        )
 
         # Make a TensorFlow Dataset
         training_dataset = self.make_dataset(
-            training_data, shuffle=True, concatenate=True
+            training_data,
+            shuffle=True,
+            concatenate=True,
+            drop_last_batch=True,
         )
 
         # Calculate the number of batches to use
-        n_total_batches = dtf.get_n_batches(training_dataset)
-        n_batches = max(round(n_total_batches * take), 1)
-        _logger.info(f"Using {n_batches} out of {n_total_batches} batches")
+        if take < 1:
+            n_total_batches = dtf.get_n_batches(training_dataset)
+            n_batches = max(round(n_total_batches * take), 1)
+            _logger.info(f"Using {n_batches} out of {n_total_batches} batches")
 
         # Pick the initialization with the lowest free energy
         best_loss = np.Inf
         for n in range(n_init):
             _logger.info(f"Initialization {n}")
             self.reset()
+            if take < 1:
+                training_data_subset = training_dataset.take(n_batches)
+            else:
+                training_data_subset = training_dataset
 
-            training_dataset = self.make_dataset(
-                training_data, shuffle=True, concatenate=True
-            )
-            training_data_subset = training_dataset.shuffle(buffer_size).take(n_batches)
-
-            history = self.fit(training_data_subset, epochs=n_epochs, **kwargs)
-            if history is None:
+            try:
+                history = self.fit(
+                    training_data_subset,
+                    epochs=n_epochs,
+                    **kwargs,
+                )
+            except tf.errors.InvalidArgumentError as e:
+                _logger.warning(e)
+                _logger.warning(
+                    "Training failed! Could be due to instability of the KL "
+                    + "term. Skipping initialization."
+                )
                 continue
+
             loss = history["loss"][-1]
             if loss < best_loss:
                 best_initialization = n
                 best_loss = loss
                 best_history = history
-                best_weights, best_trans_prob = self.get_weights()
+                best_weights = self.get_weights()
 
         if best_loss == np.Inf:
-            _logger.error("Initialization failed")
-            return
+            raise ValueError("No valid initializations were found.")
 
         _logger.info(f"Using initialization {best_initialization}")
-        self.set_weights(best_weights, best_trans_prob)
+        self.set_weights(best_weights)
+        self.reset_kl_annealing_factor()
+
+        # Reset the number of KL annealing epochs
+        self.config.n_kl_annealing_epochs = original_n_kl_annealing_epochs
 
         return best_history
 
+    def single_subject_initialization(
+        self,
+        training_data,
+        n_epochs,
+        n_init,
+        n_kl_annealing_epochs=None,
+        **kwargs,
+    ):
+        """Initialization for the mode means/covariances.
+
+        Pick a subject at random, train a model, repeat a few times. Use
+        the means/covariances from the best model (judged using the final loss).
+
+        Parameters
+        ----------
+        training_data : list of tf.data.Dataset or osl_dynamics.data.Data
+            Datasets for each subject.
+        n_epochs : int
+            Number of epochs to train.
+        n_init : int
+            How many subjects should we train on?
+        n_kl_annealing_epochs : int, optional
+            Number of KL annealing epochs to use during initialization. If
+            :code:`None` then the KL annealing epochs in the :code:`config`
+            is used.
+        kwargs : keyword arguments, optional
+            Keyword arguments for the fit method.
+        """
+        if n_init is None or n_init == 0:
+            _logger.warning(
+                "Number of initializations was set to zero. Skipping initialization."
+            )
+            return
+
+        _logger.info("Single subject initialization")
+
+        # Original number of KL annealing epochs
+        original_n_kl_annealing_epochs = self.config.n_kl_annealing_epochs
+
+        # Use n_kl_annealing_epochs if passed
+        self.config.n_kl_annealing_epochs = (
+            n_kl_annealing_epochs or original_n_kl_annealing_epochs
+        )
+
+        # Make a list of tensorflow Datasets if the data
+        training_data = self.make_dataset(
+            training_data, shuffle=True, drop_last_batch=True
+        )
+
+        if not isinstance(training_data, list):
+            raise ValueError(
+                "training_data must be a list of Datasets or a Data object."
+            )
+
+        # Pick n_init subjects at random
+        n_all_subjects = len(training_data)
+        subjects_to_use = np.random.choice(
+            range(n_all_subjects),
+            n_init,
+            replace=False,
+        )
+
+        # Train the model a few times and keep the best one
+        best_loss = np.Inf
+        losses = []
+        for subject in subjects_to_use:
+            _logger.info(f"Using subject {subject}")
+
+            # Get the dataset for this subject
+            subject_dataset = training_data[subject]
+
+            # Reset the model weights and train
+            self.reset()
+            history = self.fit(subject_dataset, epochs=n_epochs, **kwargs)
+            loss = history["loss"][-1]
+            losses.append(loss)
+            _logger.info(f"Subject {subject} loss: {loss}")
+
+            # Record the loss of this subject's data
+            if loss < best_loss:
+                best_loss = loss
+                subject_chosen = subject
+                best_weights = self.get_weights()
+
+        _logger.info(f"Using means and covariances from subject {subject_chosen}")
+
+        # Use the weights from the best initialisation for the full training
+        self.set_weights(best_weights)
+        self.reset_kl_annealing_factor()
+
+        # Reset the number of KL annealing epochs
+        self.config.n_kl_annealing_epochs = original_n_kl_annealing_epochs
+
+    def multistart_initialization(
+        self,
+        training_data,
+        n_epochs,
+        n_init,
+        n_kl_annealing_epochs=None,
+        **kwargs,
+    ):
+        """Multi-start initialization.
+
+        Wrapper for :code:`random_subset_initialization` with :code:`take=1`.
+
+        Returns
+        -------
+        history : history
+            The training history of the best initialization.
+        """
+
+        return self.random_subset_initialization(
+            training_data,
+            n_epochs,
+            n_init,
+            take=1,
+            n_kl_annealing_epochs=n_kl_annealing_epochs,
+            **kwargs,
+        )
+
     def random_state_time_course_initialization(
-        self, training_data, n_epochs, n_init, take=1, **kwargs
+        self, training_data, n_epochs, n_init, take=1, stay_prob=0.9, **kwargs
     ):
         """Random state time course initialization.
 
         The model is trained for a few epochs with a sampled state time course
         initialization. The model with the best free energy is kept.
 
         Parameters
@@ -348,14 +394,17 @@
             Dataset to use for training.
         n_epochs : int
             Number of epochs to train the model.
         n_init : int
             Number of initializations.
         take : float, optional
             Fraction of total batches to take.
+        stay_prob : float, optional
+            Stay probability (diagonal for the transition probability
+            matrix). Other states have uniform probability.
         kwargs : keyword arguments, optional
             Keyword arguments for the fit method.
 
         Returns
         -------
         history : history
             The training history of the best initialization.
@@ -365,540 +414,1070 @@
                 "Number of initializations was set to zero. "
                 + "Skipping initialization."
             )
             return
 
         _logger.info("Random state time course initialization")
 
-        # Get the buffer size
-        buffer_size = getattr(training_data, "buffer_size", 100000)
-
         # Make a TensorFlow Dataset
         training_dataset = self.make_dataset(
-            training_data, shuffle=True, concatenate=True
+            training_data, shuffle=True, concatenate=True, drop_last_batch=True
         )
 
         # Calculate the number of batches to use
-        n_total_batches = dtf.get_n_batches(training_dataset)
-        n_batches = max(round(n_total_batches * take), 1)
-        _logger.info(f"Using {n_batches} out of {n_total_batches} batches")
+        if take < 1:
+            n_total_batches = dtf.get_n_batches(training_dataset)
+            n_batches = max(round(n_total_batches * take), 1)
+            _logger.info(f"Using {n_batches} out of {n_total_batches} batches")
 
         # Pick the initialization with the lowest free energy
         best_loss = np.Inf
         for n in range(n_init):
             _logger.info(f"Initialization {n}")
             self.reset()
-            training_data_subset = training_dataset.shuffle(buffer_size).take(n_batches)
+            if take < 1:
+                training_data_subset = training_dataset.take(n_batches)
+            else:
+                training_data_subset = training_dataset
 
-            self.set_random_state_time_course_initialization(training_data_subset)
-            history = self.fit(training_data_subset, epochs=n_epochs, **kwargs)
-            if history is None:
+            self.set_random_state_time_course_initialization(
+                training_data_subset, stay_prob
+            )
+
+            try:
+                history = self.fit(training_data_subset, epochs=n_epochs, **kwargs)
+            except tf.errors.InvalidArgumentError as e:
+                _logger.warning(e)
+                _logger.warning("Training failed! Skipping initialization.")
                 continue
+
             loss = history["loss"][-1]
             if loss < best_loss:
                 best_initialization = n
                 best_loss = loss
                 best_history = history
-                best_weights, best_trans_prob = self.get_weights()
+                best_weights = self.get_weights()
 
         if best_loss == np.Inf:
-            _logger.error("Initialization failed")
-            return
+            raise ValueError("No valid initializations were found.")
 
         _logger.info(f"Using initialization {best_initialization}")
-        self.set_weights(best_weights, best_trans_prob)
+        self.set_weights(best_weights)
+        self.reset_kl_annealing_factor()
 
         return best_history
 
-    def get_posterior(self, x):
-        """Get marginal and joint posterior.
+    def set_random_state_time_course_initialization(
+        self, training_dataset, stay_prob=0.9
+    ):
+        """Sets the initial means/covariances based on a random state time course.
 
         Parameters
         ----------
-        x : np.ndarray
-            Observed data. Shape is (batch_size, sequence_length, n_channels).
+        training_dataset : tf.data.Dataset
+            Training data.
+        stay_prob : float, optional
+            Stay probability (diagonal for the transition probability
+            matrix). Other states have uniform probability.
+        """
+        _logger.info("Setting random means and covariances")
+
+        # HMM simulation to sample from
+        sim = HMM(
+            trans_prob="uniform",
+            stay_prob=stay_prob,
+            n_states=self.config.n_states or self.config.n_modes,
+        )
+
+        # Mean and covariance for each state
+        means = np.zeros(
+            [self.config.n_states or self.config.n_modes, self.config.n_channels],
+            dtype=np.float32,
+        )
+        covariances = np.zeros(
+            [
+                self.config.n_states or self.config.n_modes,
+                self.config.n_channels,
+                self.config.n_channels,
+            ],
+            dtype=np.float32,
+        )
+
+        n_batches = 0
+        for batch in training_dataset:
+            # Concatenate all the sequences in this batch
+            data = np.concatenate(batch["data"])
+
+            if data.shape[0] < 2 * self.config.n_channels:
+                raise ValueError(
+                    "Not enough time points in batch, "
+                    "increase batch_size or sequence_length"
+                )
+
+            # Sample a state time course using the initial transition
+            # probability matrix
+            stc = sim.generate_states(data.shape[0])
+
+            # Make sure each state activates
+            non_active_states = np.sum(stc, axis=0) < 2 * self.config.n_channels
+            while np.any(non_active_states):
+                new_stc = sim.generate_states(data.shape[0])
+                new_active_states = np.sum(new_stc, axis=0) != 0
+                for j in range(self.config.n_states or self.config.n_modes):
+                    if non_active_states[j] and new_active_states[j]:
+                        stc[:, j] = new_stc[:, j]
+                non_active_states = np.sum(stc, axis=0) < 2 * self.config.n_channels
+
+            # Calculate the mean/covariance for each state for this batch
+            m = []
+            C = []
+            for j in range(self.config.n_states or self.config.n_modes):
+                x = data[stc[:, j] == 1]
+                mu = np.mean(x, axis=0)
+                sigma = np.cov(x, rowvar=False)
+                m.append(mu)
+                C.append(sigma)
+            means += m
+            covariances += C
+            n_batches += 1
+
+        # Calculate the average from the running total
+        means /= n_batches
+        covariances /= n_batches
+
+        if self.config.learn_means:
+            # Set initial means
+            self.set_means(means, update_initializer=True)
+
+        if self.config.learn_covariances:
+            # Set initial covariances
+            self.set_covariances(covariances, update_initializer=True)
+
+    def reset_kl_annealing_factor(self):
+        """Sets the KL annealing factor to zero.
+
+        This method assumes there is a keras layer named :code:`'kl_loss'`
+        in the model.
+        """
+        if self.config.do_kl_annealing:
+            kl_loss_layer = self.model.get_layer("kl_loss")
+            kl_loss_layer.annealing_factor.assign(0.0)
+
+    def reset_weights(self, keep=None):
+        """Reset the model as if you've built a new model.
+
+        Parameters
+        ----------
+        keep : list of str, optional
+            Layer names to NOT reset.
+        """
+        super().reset_weights(keep=keep)
+        self.reset_kl_annealing_factor()
+
+    def predict(self, *args, **kwargs):
+        """Wrapper for the standard keras predict method.
 
         Returns
         -------
-        gamma : np.ndarray
-            Marginal posterior distribution of hidden states given the data,
-            :math:`q(s_t)`. Shape is (batch_size*sequence_length, n_states).
-        xi : np.ndarray
-            Joint posterior distribution of hidden states at two consecutive
-            time points, :math:`q(s_t, s_{t+1})`. Shape is
-            (batch_size*sequence_length-1, n_states*n_states).
+        predictions : dict
+            Dictionary with labels for each prediction.
         """
-        B = self.get_likelihood(x)
-        Pi_0 = self.state_probs_t0
-        P = self.trans_prob
-        return self.baum_welch(B, Pi_0, P)
+        predictions = self.model.predict(*args, **kwargs)
+        if not self.config.multiple_dynamics:
+            return_names = ["ll_loss", "kl_loss", "theta"]
+        else:
+            return_names = ["ll_loss", "kl_loss", "power_theta", "fc_theta"]
+        predictions_dict = dict(zip(return_names, predictions))
 
-    @numba.jit
-    def baum_welch(self, B, Pi_0, P):
-        """Hidden state inference using the Baum-Welch algorithm.
+        return predictions_dict
+
+    def get_theta(
+        self, dataset, concatenate=False, remove_edge_effects=False, **kwargs
+    ):
+        """Mode mixing logits, :code:`theta`.
 
         Parameters
         ----------
-        B : np.ndarray
-            Probability of array data points, under observation model for
-            each state. Shape is (n_states, n_samples).
-        Pi_0 : np.ndarray
-            Initial state probabilities. Shape is (n_states,).
-        P : np.ndarray
-            State transition probabilities. Shape is (n_states, n_states).
+        dataset : tf.data.Dataset or osl_dynamics.data.Data
+            Prediction dataset. This can be a list of datasets, one for each
+            session.
+        concatenate : bool, optional
+            Should we concatenate theta for each session?
+        remove_edge_effects : bool, optional
+            Edge effects can arise due to separating the data into sequences.
+            We can remove these by predicting overlapping :code:`theta` and
+            disregarding the :code:`theta` near the ends. Passing :code:`True`
+            does this by using sequences with 50% overlap and throwing away the
+            first and last 25% of predictions.
 
         Returns
         -------
-        gamma : np.ndarray
-            Marginal posterior distribution of hidden states given the data,
-            :math:`q(s_t)`. Shape is (n_samples, n_states).
-        xi : np.ndarray
-            Joint posterior distribution of hidden states at two consecutive
-            time points, :math:`q(s_t, s_{t+1})`. Shape is (n_samples-1,
-            n_states*n_states).
+        theta : list or np.ndarray
+            Mode mixing logits with shape (n_sessions, n_samples, n_modes)
+            or (n_samples, n_modes).
+        fc_theta : list or np.ndarray
+            Mode mixing logits for FC.
+            Only returned if :code:`self.config.multiple_dynamics=True`.
         """
-        n_samples = B.shape[1]
-        n_states = B.shape[0]
+        if self.is_multi_gpu:
+            raise ValueError(
+                "MirroredStrategy is not supported for this method. "
+                + "Please load a new model with "
+                + "osl_dynamics.models.load(..., single_gpu=True)."
+            )
 
-        # Memory allocation
-        alpha = np.empty((n_samples, n_states))
-        beta = np.empty((n_samples, n_states))
-        scale = np.empty(n_samples)
+        if self.config.multiple_dynamics:
+            return self.get_mode_logits(
+                dataset,
+                concatenate,
+                remove_edge_effects,
+            )
 
-        # Forward pass
-        alpha[0] = Pi_0 * B[:, 0]
-        scale[0] = np.sum(alpha[0])
-        alpha[0] /= scale[0] + EPS
-        for i in range(1, n_samples):
-            alpha[i] = (alpha[i - 1] @ P) * B[:, i]
-            scale[i] = np.sum(alpha[i])
-            alpha[i] /= scale[i] + EPS
+        if remove_edge_effects:
+            step_size = self.config.sequence_length // 2  # 50% overlap
+        else:
+            step_size = None
 
-        # Backward pass
-        beta[-1] = 1.0 / (scale[-1] + EPS)
-        for i in range(2, n_samples + 1):
-            beta[-i] = (beta[-i + 1] * B[:, -i + 1]) @ P.T
-            beta[-i] /= scale[-i] + EPS
+        dataset = self.make_dataset(dataset, step_size=step_size)
 
-        # Marginal probabilities
-        gamma = alpha * beta
-        gamma /= np.sum(gamma, axis=1, keepdims=True)
+        n_datasets = len(dataset)
+        if len(dataset) > 1:
+            iterator = trange(n_datasets, desc="Getting theta")
+            kwargs["verbose"] = 0
+        else:
+            iterator = range(n_datasets)
+            _logger.info("Getting theta")
 
-        # Joint probabilities
-        b = beta[1:] * B[:, 1:].T
-        t = P * np.expand_dims(alpha[:-1], axis=2) * np.expand_dims(b, axis=1)
-        xi = t.reshape(n_samples - 1, -1, order="F")
-        xi /= np.expand_dims(np.sum(xi, axis=1), axis=1) + EPS
+        theta = []
+        for i in iterator:
+            predictions = self.predict(dataset[i], **kwargs)
+            theta_ = predictions["theta"]
+            if remove_edge_effects:
+                trim = step_size // 2  # throw away 25%
+                theta_ = (
+                    [theta_[0, :-trim]]
+                    + list(theta_[1:-1, trim:-trim])
+                    + [theta_[-1, trim:]]
+                )
+            theta.append(np.concatenate(theta_))
+
+        if concatenate or len(theta) == 1:
+            theta = np.concatenate(theta)
 
-        return gamma, xi
+        return theta
 
-    def get_likelihood(self, x):
-        """Get the likelihood, :math:`p(x_t | s_t)`.
+    def get_mode_logits(
+        self, dataset, concatenate=False, remove_edge_effects=False, **kwargs
+    ):
+        """Get logits (:code:`theta`) for a multi-time-scale model.
 
         Parameters
         ----------
-        x : np.ndarray
-            Observed data. Shape is (batch_size, sequence_length, n_channels).
+        dataset : tf.data.Dataset or osl_dynamics.data.Data
+            Prediction dataset. This can be a list of datasets, one for each
+            session.
+        concatenate : bool, optional
+            Should we concatenate theta for each session?
+        remove_edge_effects : bool, optional
+            Edge effects can arise due to separating the data into sequences.
+            We can remove these by predicting overlapping :code:`theta` and
+            disregarding the :code:`theta` near the ends. Passing :code:`True`
+            does this by using sequences with 50% overlap and throwing away the
+            first and last 25% of predictions.
 
         Returns
         -------
-        likelihood : np.ndarray
-            Likelihood. Shape is (n_states, batch_size*sequence_length).
+        power_theta : list or np.ndarray
+            Mode mixing logits for power with shape (n_sessions, n_samples,
+            n_modes) or (n_samples, n_modes).
+        fc_theta : list or np.ndarray
+            Mode mixing logits for FC with shape (n_sessions, n_samples,
+            n_modes) or (n_samples, n_modes).
         """
-        # Get the current observation model parameters
-        log_rates = self.get_log_rates()
-        n_states = log_rates.shape[0]
+        if self.is_multi_gpu:
+            raise ValueError(
+                "MirroredStrategy is not supported for this method. "
+                + "Please load a new model with "
+                + "osl_dynamics.models.load(..., single_gpu=True)."
+            )
+
+        if not self.config.multiple_dynamics:
+            raise ValueError("Please use get_theta for a single time scale model.")
 
-        batch_size = x.shape[0]
-        sequence_length = x.shape[1]
+        if remove_edge_effects:
+            step_size = self.config.sequence_length // 2  # 50% overlap
+        else:
+            step_size = None
+
+        dataset = self.make_dataset(dataset, step_size=step_size)
+
+        n_datasets = len(dataset)
+        if len(dataset) > 1:
+            iterator = trange(n_datasets, desc="Getting mode logits")
+            kwargs["verbose"] = 0
+        else:
+            iterator = range(n_datasets)
+            _logger.info("Getting mode logits")
 
-        # Calculate the log-likelihood for each state to have generated the
-        # observed data
-        log_likelihood = np.empty([n_states, batch_size, sequence_length])
-        for state in range(n_states):
-            poi = tf.stop_gradient(
-                tfp.distributions.Poisson(
-                    log_rate=tf.gather(log_rates, state, axis=-2),
-                    allow_nan_stats=False,
+        power_theta = []
+        fc_theta = []
+        for i in iterator:
+            predictions = self.predict(dataset[i], **kwargs)
+            power_theta_ = predictions["power_theta"]
+            fc_theta_ = predictions["fc_theta"]
+            if remove_edge_effects:
+                trim = step_size // 2  # throw away 25%
+                power_theta_ = (
+                    [power_theta_[0, :-trim]]
+                    + list(power_theta_[1:-1, trim:-trim])
+                    + [power_theta_[-1, trim:]]
                 )
+                fc_theta_ = (
+                    [fc_theta_[0, :-trim]]
+                    + list(fc_theta_[1:-1, trim:-trim])
+                    + [fc_theta_[-1, trim:]]
+                )
+            power_theta.append(np.concatenate(power_theta_))
+            fc_theta.append(np.concatenate(fc_theta_))
+
+        if concatenate or len(power_theta) == 1:
+            power_theta = np.concatenate(power_theta)
+            fc_theta = np.concatenate(fc_theta)
+
+        return power_theta, fc_theta
+
+    def get_alpha(
+        self, dataset, concatenate=False, remove_edge_effects=False, **kwargs
+    ):
+        """Get mode mixing coefficients, :code:`alpha`.
+
+        Parameters
+        ----------
+        dataset : tf.data.Dataset or osl_dynamics.data.Data
+            Prediction dataset. This can be a list of datasets, one for each
+            session.
+        concatenate : bool, optional
+            Should we concatenate alpha for each session?
+        remove_edge_effects : bool, optional
+            Edge effects can arise due to separating the data into sequences.
+            We can remove these by predicting overlapping :code:`alpha` and
+            disregarding the :code:`alpha` near the ends. Passing :code:`True`
+            does this by using sequences with 50% overlap and throwing away the
+            first and last 25% of predictions.
+
+        Returns
+        -------
+        alpha : list or np.ndarray
+            Mode mixing coefficients with shape (n_sessions, n_samples,
+            n_modes) or (n_samples, n_modes).
+        """
+        if self.is_multi_gpu:
+            raise ValueError(
+                "MirroredStrategy is not supported for this method. "
+                + "Please load a new model with "
+                + "osl_dynamics.models.load(..., single_gpu=True)."
             )
-            log_likelihood[state] = tf.reduce_sum(poi.log_prob(x), axis=-1)
-        log_likelihood = log_likelihood.reshape(n_states, batch_size * sequence_length)
 
-        # We add a constant to the log-likelihood for time points where all
-        # states have a negative log-likelihood. This is critical for numerical
-        # stability.
-        time_points_with_all_states_negative = np.all(log_likelihood < 0, axis=0)
-        if np.any(time_points_with_all_states_negative):
-            log_likelihood[:, time_points_with_all_states_negative] -= np.max(
-                log_likelihood[:, time_points_with_all_states_negative], axis=0
-            )
-
-        # Return the likelihood
-        return np.exp(log_likelihood)
-
-    def update_trans_prob(self, gamma, xi):
-        """Update transition probability matrix.
-
-        Parameters
-        ----------
-        gamma : np.ndarray
-            Marginal posterior distribution of hidden states given the data,
-            :math:`q(s_t)`. Shape is (batch_size*sequence_length, n_states).
-        xi : np.ndarray
-            Joint posterior distribution of hidden states at two consecutive
-            time points, :math:`q(s_t, s_{t+1})`. Shape is
-            (batch_size*sequence_length-1, n_states*n_states).
-        """
-        # Calculate the new transition probability matrix using the posterior
-        # from the Baum-Welch algorithm:
-        #
-        # p(s_t+1 | s_t) = E{q(s_t, s_t+1)} / E{q(s_t)}
-        #                = sum^{T-1}_{t=1} xi(t, t+1) / sum^{T-1}_{t=1} gamma(t)
-        #
-        # where E{.} denotes the expectation.
-        phi_interim = np.sum(xi, axis=0).reshape(
-            self.config.n_states, self.config.n_states
-        ).T / np.sum(gamma[:-1], axis=0).reshape(self.config.n_states, 1)
-
-        # We use stochastic updates on trans_prob as per Eqs. (1) and (2) in the
-        # paper:
-        # https://www.sciencedirect.com/science/article/pii/S1053811917305487
-        self.trans_prob = (1 - self.rho) * self.trans_prob + self.rho * phi_interim
-
-    def _update_rho(self, ind):
-        """Update rho.
-
-        Parameters
-        ---------
-        ind : int
-            Index of iteration.
-        """
-        # Calculate new value, using modified version of Eq. (2) to account for
-        # total number of iterations:
-        # https://www.sciencedirect.com/science/article/pii/S1053811917305487
-        self.rho = np.power(
-            100 * ind / self.config.n_epochs + 1 + self.config.trans_prob_update_delay,
-            -self.config.trans_prob_update_forget,
-        )
+        if self.config.multiple_dynamics:
+            return self.get_mode_time_courses(
+                dataset,
+                concatenate,
+                remove_edge_effects,
+            )
 
-    def get_posterior_entropy(self, gamma, xi):
-        """Posterior entropy.
+        if remove_edge_effects:
+            step_size = self.config.sequence_length // 2  # 50% overlap
+        else:
+            step_size = None
 
-        Calculate the entropy of the posterior distribution:
+        dataset = self.make_dataset(dataset, step_size=step_size)
+        alpha_layer = self.model.get_layer("alpha")
 
-        .. math::
-            E &= \int q(s_{1:T}) \log q(s_{1:T}) ds_{1:T}
+        n_datasets = len(dataset)
+        if len(dataset) > 1:
+            iterator = trange(n_datasets, desc="Getting alpha")
+            kwargs["verbose"] = 0
+        else:
+            iterator = range(n_datasets)
+            _logger.info("Getting alpha")
 
-              &= \displaystyle\sum_{t=1}^{T-1} \int q(s_t, s_{t+1}) \
-                 \log q(s_t, s_{t+1}) ds_t ds_{t+1} - \
-                 \displaystyle\sum_{t=2}^{T-1} \
-                 \int q(s_t) \log q(s_t) ds_t
+        alpha = []
+        for i in iterator:
+            predictions = self.predict(dataset[i], **kwargs)
+            theta = predictions["theta"]
+            alpha_ = alpha_layer(theta)
+            if remove_edge_effects:
+                trim = step_size // 2  # throw away 25%
+                alpha_ = (
+                    [alpha_[0, :-trim]]
+                    + list(alpha_[1:-1, trim:-trim])
+                    + [alpha_[-1, trim:]]
+                )
+            alpha.append(np.concatenate(alpha_))
+
+        if concatenate or len(alpha) == 1:
+            alpha = np.concatenate(alpha)
+
+        return alpha
+
+    def get_mode_time_courses(
+        self, dataset, concatenate=False, remove_edge_effects=False, **kwargs
+    ):
+        """Get mode time courses (:code:`alpha`) for a multi-time-scale model.
 
         Parameters
         ----------
-        gamma : np.ndarray
-            Marginal posterior distribution of hidden states given the data,
-            :math:`q(s_t)`. Shape is (batch_size*sequence_length, n_states).
-        xi : np.ndarray
-            Joint posterior distribution of hidden states at two consecutive
-            time points, :math:`q(s_t, s_{t+1})`. Shape is
-            (batch_size*sequence_length-1, n_states*n_states).
+        dataset : tf.data.Dataset or osl_dynamics.data.Data
+            Prediction data. This can be a list of datasets, one for each
+            session.
+        concatenate : bool, optional
+            Should we concatenate alpha/beta for each session?
+        remove_edge_effects : bool, optional
+            Edge effects can arise due to separating the data into sequences.
+            We can remove these by predicting overlapping :code:`alpha`/
+            :code:`beta` and disregarding the :code:`alpha`/:code:`beta` near
+            the ends. Passing :code:`True` does this by using sequences with 50%
+            overlap and throwing away the first and last 25% of predictions.
 
         Returns
         -------
-        entropy : float
-            Entropy.
+        alpha : list or np.ndarray
+            Alpha time course with shape (n_sessions, n_samples, n_modes) or
+            (n_samples, n_modes).
+        beta : list or np.ndarray
+            Beta time course with shape (n_sessions, n_samples, n_modes) or
+            (n_samples, n_modes).
         """
-        # first_term = sum^{T-1}_t=1 int q(s_t, s_t+1)
-        # log(q(s_t, s_t+1)) ds_t ds_t+1
-        first_term = np.sum(xlogy(xi, xi))
+        if self.is_multi_gpu:
+            raise ValueError(
+                "MirroredStrategy is not supported for this method. "
+                + "Please load a new model with "
+                + "osl_dynamics.models.load(..., single_gpu=True)."
+            )
 
-        # second_term = sum^{T-1}_t=2 int q(s_t) log q(s_t) ds_t
-        second_term = np.sum(xlogy(gamma, gamma)[1:-1])
+        if not self.config.multiple_dynamics:
+            raise ValueError("Please use get_alpha for a single time scale model.")
 
-        return first_term - second_term
+        if remove_edge_effects:
+            step_size = self.config.sequence_length // 2  # 50% overlap
+        else:
+            step_size = None
 
-    def get_posterior_expected_log_likelihood(self, x, gamma):
-        """Expected log-likelihood.
+        dataset = self.make_dataset(dataset, step_size=step_size)
+        alpha_layer = self.model.get_layer("alpha")
+        beta_layer = self.model.get_layer("beta")
 
-        Calculates the expected log-likelihood with respect to the posterior
-        distribution of the states:
+        n_datasets = len(dataset)
+        if len(dataset) > 1:
+            iterator = trange(n_datasets, desc="Getting mode time courses")
+            kwargs["verbose"] = 0
+        else:
+            iterator = range(n_datasets)
+            _logger.info("Getting mode time courses")
 
-        .. math::
-            LL &= \int q(s_{1:T}) \log \prod_{t=1}^T p(x_t | s_t) ds_{1:T}
+        alpha = []
+        beta = []
+        for i in iterator:
+            predictions = self.predict(dataset[i], **kwargs)
+            power_theta = predictions["power_theta"]
+            fc_theta = predictions["fc_theta"]
+            alpha_ = alpha_layer(power_theta)
+            beta_ = beta_layer(fc_theta)
+            if remove_edge_effects:
+                trim = step_size // 2  # throw away 25%
+                alpha_ = (
+                    [alpha_[0, :-trim]]
+                    + list(alpha_[1:-1, trim:-trim])
+                    + [alpha_[-1, trim:]]
+                )
+                beta_ = (
+                    [beta_[0, :-trim]]
+                    + list(beta_[1:-1, trim:-trim])
+                    + [beta_[-1, trim:]]
+                )
+            alpha.append(np.concatenate(alpha_))
+            beta.append(np.concatenate(beta_))
+
+        if concatenate or len(alpha) == 1:
+            alpha = np.concatenate(alpha)
+            beta = np.concatenate(beta)
 
-               &= \sum_{t=1}^T \int q(s_t) \log p(x_t | s_t) ds_t
+        return alpha, beta
+
+    def losses(self, dataset, **kwargs):
+        """Calculates the log-likelihood and KL loss for a dataset.
 
         Parameters
         ----------
-        x : np.ndarray
-            Data. Shape is (batch_size, sequence_length, n_channels).
-        gamma : np.ndarray
-            Marginal posterior distribution of hidden states given the data,
-            :math:`q(s_t)`. Shape is (batch_size*sequence_length, n_states).
+        dataset : tf.data.Dataset or osl_dynamics.data.Data
+            Dataset to calculate losses for.
 
         Returns
         -------
-        log_likelihood : float
-            Posterior expected log-likelihood.
+        ll_loss : float
+            Negative log-likelihood loss.
+        kl_loss : float
+            KL divergence loss.
         """
-        gamma = np.reshape(gamma, (x.shape[0], x.shape[1], -1))
-        log_likelihood = self.get_log_likelihood(x)
-        return tf.stop_gradient(tf.reduce_sum(log_likelihood * gamma))
+        if self.is_multi_gpu:
+            raise ValueError(
+                "MirroredStrategy is not supported for this method. "
+                + "Please load a new model with "
+                + "osl_dynamics.models.load(..., single_gpu=True)."
+            )
 
-    def get_posterior_expected_prior(self, gamma, xi):
-        """Posterior expected prior.
+        dataset = self.make_dataset(dataset, concatenate=True)
+        _logger.info("Getting losses")
+        predictions = self.predict(dataset, **kwargs)
+        ll_loss = np.mean(predictions["ll_loss"])
+        kl_loss = np.mean(predictions["kl_loss"])
+        return ll_loss, kl_loss
 
-        Calculates the expected prior probability of states with respect to the
-        posterior distribution of the states:
+    def free_energy(self, dataset, **kwargs):
+        """Calculates the variational free energy of a dataset.
 
-        .. math::
-            P &= \int q(s_{1:T}) \log p(s_{1:T}) ds
-
-              &= \int q(s_1) \log p(s_1) ds_1 + \displaystyle\sum_{t=1}^{T-1} \
-                 \int q(s_t, s_{t+1}) \log p(s_{t+1} | s_t) ds_t ds_{t+1}
+        Note, this method returns a free energy which may have a significantly
+        smaller KL loss. This is because during training we sample from the
+        posterior, however, when we're evaluating the model, we take the maximum
+        a posteriori estimate (posterior mean). This has the effect of giving a
+        lower KL loss for a given dataset.
 
         Parameters
         ----------
-        gamma : np.ndarray
-            Marginal posterior distribution of hidden states given the data,
-            :math:`q(s_t)`. Shape is (batch_size*sequence_length, n_states).
-        xi : np.ndarray
-            Joint posterior distribution of hidden states at two consecutive
-            time points, :math:`q(s_t, s_{t+1})`. Shape is
-            (batch_size*sequence_length-1, n_states*n_states).
+        dataset : tf.data.Dataset or osl_dynamics.data.Data.
+            Dataset to calculate the variational free energy for.
 
         Returns
         -------
-        prior : float
-            Posterior expected prior probability.
+        free_energy : float
+            Variational free energy for the dataset.
         """
-        n_samples, n_states = gamma.shape
+        dataset = self.make_dataset(dataset, concatenate=True)
+        ll_loss, kl_loss = self.losses(dataset, **kwargs)
+        free_energy = ll_loss + kl_loss
+        return free_energy
+
+    def bayesian_information_criterion(self, dataset):
+        """Calculate the Bayesian Information Criterion (BIC) of the model
+        for a given dataset.
 
-        # first_term = int q(s_1) log p(s_1) ds_1
-        first_term = np.sum(xlogy(gamma[0], self.state_probs_t0))
+        Note this method uses free energy as an approximate to the negative
+        log-likelihood.
 
-        # remaining_terms =
-        # sum^{T-1}_t=1 int q(s_t, s_t+1) log p(s_t+1 | s_t}) ds_t ds_t+1
-        remaining_terms = np.sum(
-            xlogy(
-                xi.reshape(n_samples - 1, n_states, n_states, order="F"),
-                np.expand_dims(self.trans_prob, 0),
-            )
+        Parameters
+        ----------
+        dataset : osl_dynamics.data.Data
+            Dataset to calculate the BIC for.
+
+        Returns
+        -------
+        bic : float
+            Bayesian Information Criterion for the model (for each sequence).
+        """
+        loss = self.free_energy(dataset)
+        n_params = self.get_n_params_generative_model()
+        n_sequences = dtf.n_batches(
+            dataset.time_series(concatenate=True), self.config.sequence_length
         )
 
-        return first_term + remaining_terms
+        bic = (
+            2 * loss
+            + (np.log(self.config.sequence_length) + np.log(n_sequences))
+            * n_params
+            / n_sequences
+        )
+        return bic
+
+
+@dataclass
+class MarkovStateInferenceModelConfig:
+    """Settings needed for inferring a Markov chain for hidden states."""
+
+    # Transition probability matrix
+    initial_trans_prob: np.ndarray = None
+    learn_trans_prob: bool = True
+    trans_prob_update_delay: float = 5  # alpha
+    trans_prob_update_forget: float = 0.7  # beta
+
+    def validate_trans_prob_parameters(self):
+        if self.initial_trans_prob is not None:
+            if (
+                not isinstance(self.initial_trans_prob, np.ndarray)
+                or self.initial_trans_prob.ndim != 2
+            ):
+                raise ValueError("initial_trans_prob must be a 2D numpy array.")
+
+            if not all(np.isclose(np.sum(self.initial_trans_prob, axis=1), 1)):
+                raise ValueError("rows of initial_trans_prob must sum to one.")
+
+
+class MarkovStateInferenceModelBase(ModelBase):
+    """Base class for a Markov chain hidden state inference model."""
 
-    def get_log_likelihood(self, data):
-        """Get the log-likelihood of data, :math:`\log p(x_t | s_t)`.
+    def fit(self, *args, lr_decay=None, **kwargs):
+        """Wrapper for the standard keras fit method.
 
         Parameters
         ----------
-        data : np.ndarray
-            Data. Shape is (batch_size, ..., n_channels).
+        *args : arguments
+            Arguments for :code:`ModelBase.fit()`.
+        lr_decay : float, optional
+            Learning rate decay.
+        **kwargs : keyword arguments, optional
+            Keyword arguments for :code:`ModelBase.fit()`.
 
         Returns
         -------
-        log_likelihood : np.ndarray
-            Log-likelihood. Shape is (batch_size, ..., n_states)
+        history : history
+            The training history.
         """
-        log_rates = self.get_log_rates()
-        poi = tf.stop_gradient(
-            tfp.distributions.Poisson(
-                log_rate=log_rates,
-                allow_nan_stats=False,
-            )
+        # Callback for a learning rate decay
+        if lr_decay is None:
+            lr_decay = self.config.lr_decay
+
+        def lr_scheduler(epoch, lr):
+            return self.config.learning_rate * np.exp(-lr_decay * epoch)
+
+        lr_callback = tf.keras.callbacks.LearningRateScheduler(lr_scheduler)
+
+        # Callback for updating the the decay rate used in the
+        # EMA update of the transition probability matrix
+        trans_prob_decay_callback = callbacks.EMADecayCallback(
+            delay=self.config.trans_prob_update_delay,
+            forget=self.config.trans_prob_update_forget,
+            n_epochs=self.config.n_epochs,
+        )
+
+        # Update arguments to pass to the fit method
+        args, kwargs = replace_argument(
+            self.model.fit,
+            "callbacks",
+            [lr_callback, trans_prob_decay_callback],
+            args,
+            kwargs,
+            append=True,
+        )
+
+        return super().fit(*args, **kwargs)
+
+    def compile(self, optimizer=None):
+        """Compile the model.
+
+        Parameters
+        ----------
+        optimizer : str or tf.keras.optimizers.Optimizer
+            Optimizer to use when compiling.
+        """
+
+        # Moving average optimizer for the transition probability matrix
+        decay = (
+            1 + self.config.trans_prob_update_delay
+        ) ** -self.config.trans_prob_update_forget
+        ema_optimizer = optimizers.ExponentialMovingAverage(decay)
+
+        # Optimizer for all other trainable parameters
+        base_optimizer = tf.keras.optimizers.get(
+            {
+                "class_name": self.config.optimizer.lower(),
+                "config": {
+                    "learning_rate": self.config.learning_rate,
+                },
+            }
         )
-        log_likelihood = tf.reduce_sum(
-            poi.log_prob(tf.expand_dims(data, axis=-2)), axis=-1
+
+        # Combine into a single optimizer for the model
+        optimizer = optimizers.MarkovStateModelOptimizer(
+            ema_optimizer,
+            base_optimizer,
+            learning_rate=self.config.learning_rate,
         )
-        return log_likelihood.numpy()
 
-    def get_stationary_distribution(self):
-        """Get the stationary distribution of the Markov chain.
+        # Compile
+        self.model.compile(optimizer)
 
-        This is the left eigenvector of the transition probability matrix
-        corresponding to eigenvalue = 1.
+    def predict(self, *args, **kwargs):
+        """Wrapper for the standard keras predict method.
 
         Returns
         -------
-        stationary_distribution : np.ndarray
-            Stationary distribution of the Markov chain. Shape is (n_states,).
+        predictions : dict
+            Dictionary with labels for each prediction.
         """
-        eigval, eigvec = np.linalg.eig(self.trans_prob.T)
-        stationary_distribution = np.squeeze(eigvec[:, np.isclose(eigval, 1)]).real
-        stationary_distribution /= np.sum(stationary_distribution)
-        return stationary_distribution
+        predictions = self.model.predict(*args, **kwargs)
+        if self.config.model_name == "HIVE":
+            names = ["ll_loss", "kl_loss", "gamma", "xi"]
+        else:
+            names = ["ll_loss", "gamma", "xi"]
+        return dict(zip(names, predictions))
 
-    def sample_state_time_course(self, n_samples):
-        """Sample a state time course.
+    def get_alpha(
+        self, dataset, concatenate=False, remove_edge_effects=False, **kwargs
+    ):
+        """Get state probabilities.
 
         Parameters
         ----------
-        n_samples : int
-            Number of samples.
+        dataset : tf.data.Dataset or osl_dynamics.data.Data
+            Prediction dataset. This can be a list of datasets, one for
+            each session.
+        concatenate : bool, optional
+            Should we concatenate alpha for each session?
+        remove_edge_effects : bool, optional
+            Edge effects can arise due to separating the data into sequences.
+            We can remove these by predicting overlapping :code:`alpha` and
+            disregarding the :code:`alpha` near the ends. Passing :code:`True`
+            does this by using sequences with 50% overlap and throwing away the
+            first and last 25% of predictions.
 
         Returns
         -------
-        stc : np.ndarray
-            State time course with shape (n_samples, n_states).
+        alpha : list or np.ndarray
+            State probabilities with shape (n_sessions, n_samples, n_states)
+            or (n_samples, n_states).
         """
-        sim = HMM(self.trans_prob)
-        stc = sim.generate_states(n_samples)
-        return stc
+        if self.is_multi_gpu:
+            raise ValueError(
+                "MirroredStrategy is not supported for this method. "
+                + "Please load a new model with "
+                + "osl_dynamics.models.load(..., single_gpu=True)."
+            )
+
+        if remove_edge_effects:
+            step_size = self.config.sequence_length // 2  # 50% overlap
+        else:
+            step_size = None
+
+        dataset = self.make_dataset(dataset, step_size=step_size)
+
+        n_datasets = len(dataset)
+        if len(dataset) > 1:
+            iterator = trange(n_datasets, desc="Getting alpha")
+            kwargs["verbose"] = 0
+        else:
+            iterator = range(n_datasets)
+            _logger.info("Getting alpha")
+
+        alpha = []
+        for i in iterator:
+            predictions = self.predict(dataset[i], **kwargs)
+            alpha_ = predictions["gamma"]
+            if remove_edge_effects:
+                trim = step_size // 2  # throw away 25%
+                alpha_ = (
+                    [alpha_[0, :-trim]]
+                    + list(alpha_[1:-1, trim:-trim])
+                    + [alpha_[-1, trim:]]
+                )
+            alpha.append(np.concatenate(alpha_))
+
+        if concatenate or len(alpha) == 1:
+            alpha = np.concatenate(alpha)
+
+        return alpha
 
     def get_trans_prob(self):
         """Get the transition probability matrix.
 
         Returns
         -------
         trans_prob : np.ndarray
             Transition probability matrix. Shape is (n_states, n_states).
         """
-        return self.trans_prob
+        hidden_state_inference_layer = self.model.get_layer("hid_state_inf")
+        return hidden_state_inference_layer.get_trans_prob().numpy()
 
-    def get_log_rates(self):
-        """Get the state :code:`log_rates`.
+    def get_initial_distribution(self):
+        """Get the initial distribution.
 
         Returns
         -------
-        log_rates : np.ndarray
-            State :code:`log_rates`. Shape is (n_states, n_channels).
+        initial_distribution : np.ndarray
+            Initial distribution. Shape is (n_states,).
         """
-        return obs_mod.get_observation_model_parameter(self.model, "log_rates")
+        hidden_state_inference_layer = self.model.get_layer("hid_state_inf")
+        return hidden_state_inference_layer.initial_state_probs
 
-    def get_rates(self):
-        """Get the state rates.
+    def set_trans_prob(self, trans_prob, update_initializer=True):
+        """Set the transition probability matrix.
 
-        Returns
-        -------
-        rates : np.ndarray
-            State rates. Shape is (n_states, n_channels).
+        Parameters
+        ----------
+        trans_prob : np.ndarray
+            Transition probability matrix. Shape must be (n_states, n_states).
+            Rows (axis=1) must sum to one.
         """
-        return np.exp(self.get_log_rates())
+        # Validation
+        if not isinstance(trans_prob, np.ndarray) or trans_prob.ndim != 2:
+            raise ValueError("trans_prob must be a 2D numpy array.")
+
+        if not all(np.isclose(np.sum(trans_prob, axis=1), 1)):
+            raise ValueError("rows of trans_prob must sum to one.")
 
-    def get_observation_model_parameters(self):
-        """Wrapper for :code:`get_log_rates`."""
-        return self.get_log_rates()
+        hidden_state_inference_layer = self.model.get_layer("hid_state_inf")
+        learnable_tensor_layer = hidden_state_inference_layer.layers[0]
+        learnable_tensor_layer.tensor.assign(trans_prob.astype(np.float32))
+
+        if update_initializer:
+            learnable_tensor_layer.tensor_initializer = WeightInitializer(
+                trans_prob.astype(np.float32)
+            )
 
-    def set_log_rates(self, log_rates, update_initializer=True):
-        """Set the state :code:`log_rates`.
+    def random_subset_initialization(
+        self, training_data, n_epochs, n_init, take, **kwargs
+    ):
+        """Random subset initialization.
+
+        The model is trained for a few epochs with different random subsets
+        of the training dataset. The model with the best free energy is kept.
 
         Parameters
         ----------
-        log_rates : np.ndarray
-            State :code:`log_rates`. Shape is (n_states, n_channels).
-        update_initializer : bool, optional
-            Do we want to use the passed :code:`log_rates` when we
-            re-initialize the model?
+        training_data : tf.data.Dataset or osl_dynamics.data.Data
+            Dataset to use for training.
+        n_epochs : int
+            Number of epochs to train the model.
+        n_init : int
+            Number of initializations.
+        take : float
+            Fraction of total batches to take.
+        kwargs : keyword arguments, optional
+            Keyword arguments for the fit method.
+
+        Returns
+        -------
+        history : history
+            The training history of the best initialization.
         """
-        obs_mod.set_observation_model_parameter(
-            self.model,
-            log_rates,
-            layer_name="log_rates",
-            update_initializer=update_initializer,
+        if n_init is None or n_init == 0:
+            _logger.info(
+                "Number of initializations was set to zero. "
+                + "Skipping initialization."
+            )
+            return
+
+        _logger.info("Random subset initialization")
+
+        # Make a TensorFlow Dataset
+        training_dataset = self.make_dataset(
+            training_data, shuffle=True, concatenate=True, drop_last_batch=True
         )
 
-    def set_rates(self, log_rates, epsilon=1e-6, update_initializer=True):
-        """Set the state rates.
+        # Calculate the number of batches to use
+        if take < 1:
+            n_total_batches = dtf.get_n_batches(training_dataset)
+            n_batches = max(round(n_total_batches * take), 1)
+            _logger.info(f"Using {n_batches} out of {n_total_batches} batches")
 
-        Parameters
-        ----------
-        rates : np.ndarray
-            State rates. Shape is (n_states, n_channels).
-        update_initializer : bool, optional
-            Do we want to use the passed :code:`log_rates` when we
-            re-initialize the model?
-        """
-        log_rates = np.log(log_rates + epsilon)
-        self.set_log_rates(log_rates, update_initializer=update_initializer)
+        # Pick the initialization with the lowest free energy
+        best_loss = np.Inf
+        for n in range(n_init):
+            _logger.info(f"Initialization {n}")
+            self.reset()
+            if take < 1:
+                training_data_subset = training_dataset.take(n_batches)
+            else:
+                training_data_subset = training_dataset
+
+            try:
+                history = self.fit(
+                    training_data_subset,
+                    epochs=n_epochs,
+                    **kwargs,
+                )
+            except tf.errors.InvalidArgumentError as e:
+                _logger.warning(e)
+                _logger.warning("Training failed! Skipping initialization.")
+                continue
 
-    def set_observation_model_parameters(
-        self, observation_model_parameters, update_initializer=True
+            loss = history["loss"][-1]
+            if loss < best_loss:
+                best_initialization = n
+                best_loss = loss
+                best_history = history
+                best_weights = self.get_weights()
+
+        if best_loss == np.Inf:
+            raise ValueError("No valid initializations were found.")
+
+        _logger.info(f"Using initialization {best_initialization}")
+        self.set_weights(best_weights)
+        self.reset_kl_annealing_factor()
+
+        return best_history
+
+    def random_state_time_course_initialization(
+        self, training_data, n_epochs, n_init, take=1, **kwargs
     ):
-        """Wrapper for :code:`set_log_rates`."""
-        self.set_log_rates(
-            observation_model_parameters,
-            update_initializer=update_initializer,
-        )
+        """Random state time course initialization.
 
-    def set_trans_prob(self, trans_prob):
-        """Sets the transition probability matrix.
+        The model is trained for a few epochs with a sampled state time course
+        initialization. The model with the best free energy is kept.
 
         Parameters
         ----------
-        trans_prob : np.ndarray
-            State transition probabilities. Shape must be (n_states, n_states).
+        training_data : tf.data.Dataset or osl_dynamics.data.Data
+            Dataset to use for training.
+        n_epochs : int
+            Number of epochs to train the model.
+        n_init : int
+            Number of initializations.
+        take : float, optional
+            Fraction of total batches to take.
+        kwargs : keyword arguments, optional
+            Keyword arguments for the fit method.
+
+        Returns
+        -------
+        history : history
+            The training history of the best initialization.
         """
-        if trans_prob is None:
-            trans_prob = (
-                np.ones((self.config.n_states, self.config.n_states))
-                * 0.1
-                / (self.config.n_states - 1)
+        if n_init is None or n_init == 0:
+            _logger.info(
+                "Number of initializations was set to zero. "
+                + "Skipping initialization."
             )
-            np.fill_diagonal(trans_prob, 0.9)
-        self.trans_prob = trans_prob
+            return
 
-    def set_state_probs_t0(self, state_probs_t0):
-        """Set the initial state probabilities.
+        _logger.info("Random state time course initialization")
 
-        Parameters
-        ----------
-        state_probs_t0 : np.ndarray
-            Initial state probabilities. Shape is (n_states,).
-        """
+        # Make a TensorFlow Dataset
+        training_dataset = self.make_dataset(
+            training_data, shuffle=True, concatenate=True, drop_last_batch=True
+        )
+
+        # Calculate the number of batches to use
+        if take < 1:
+            n_total_batches = dtf.get_n_batches(training_dataset)
+            n_batches = max(round(n_total_batches * take), 1)
+            _logger.info(f"Using {n_batches} out of {n_total_batches} batches")
+
+        # Pick the initialization with the lowest free energy
+        best_loss = np.Inf
+        for n in range(n_init):
+            _logger.info(f"Initialization {n}")
+            self.reset()
+            if take < 1:
+                training_data_subset = training_dataset.take(n_batches)
+            else:
+                training_data_subset = training_dataset
+
+            self.set_random_state_time_course_initialization(training_data_subset)
+
+            try:
+                history = self.fit(training_data_subset, epochs=n_epochs, **kwargs)
+            except tf.errors.InvalidArgumentError as e:
+                _logger.warning(e)
+                _logger.warning("Training failed! Skipping initialization.")
+                continue
+
+            loss = history["loss"][-1]
+            if loss < best_loss:
+                best_initialization = n
+                best_loss = loss
+                best_history = history
+                best_weights = self.get_weights()
+
+        if best_loss == np.Inf:
+            raise ValueError("No valid initializations were found.")
 
-        if state_probs_t0 is None:
-            state_probs_t0 = np.ones((self.config.n_states,)) / self.config.n_states
-        self.state_probs_t0 = state_probs_t0
+        _logger.info(f"Using initialization {best_initialization}")
+        self.set_weights(best_weights)
+        self.reset_kl_annealing_factor()
 
-    def set_random_state_time_course_initialization(self, training_data):
-        """Sets the initial :code:`log_rates` based on a random state time course.
+        return best_history
+
+    def set_random_state_time_course_initialization(self, training_dataset):
+        """Sets the initial means/covariances based on a random state time course.
 
         Parameters
         ----------
-        training_data : tf.data.Dataset or osl_dynamics.data.Data
+        training_dataset : tf.data.Dataset
             Training data.
         """
-        _logger.info("Setting random log_rates")
+        _logger.info("Setting random means and covariances")
 
-        # Make a TensorFlow Dataset
-        training_dataset = self.make_dataset(training_data, concatenate=True)
-
-        # Log_rate for each state
-        rates = np.zeros(
+        # Mean and covariance for each state
+        means = np.zeros(
             [self.config.n_states, self.config.n_channels], dtype=np.float32
         )
+        covariances = np.zeros(
+            [self.config.n_states, self.config.n_channels, self.config.n_channels],
+            dtype=np.float32,
+        )
+
+        n_batches = 0
         for batch in training_dataset:
             # Concatenate all the sequences in this batch
             data = np.concatenate(batch["data"])
 
+            if data.shape[0] < 2 * self.config.n_channels:
+                raise ValueError(
+                    "Not enough time points in batch, "
+                    "increase batch_size or sequence_length"
+                )
+
             # Sample a state time course using the initial transition
             # probability matrix
             stc = self.sample_state_time_course(data.shape[0])
 
-            # Calculate the mean for each state for this batch as log_rate
+            # Make sure each state activates
+            non_active_states = np.sum(stc, axis=0) < 2 * self.config.n_channels
+            while np.any(non_active_states):
+                new_stc = self.sample_state_time_course(data.shape[0])
+                new_active_states = np.sum(new_stc, axis=0) != 0
+                for j in range(self.config.n_states):
+                    if non_active_states[j] and new_active_states[j]:
+                        stc[:, j] = new_stc[:, j]
+                non_active_states = np.sum(stc, axis=0) < 2 * self.config.n_channels
+
+            # Calculate the mean/covariance for each state for this batch
             m = []
+            C = []
             for j in range(self.config.n_states):
                 x = data[stc[:, j] == 1]
-                mu_j = np.mean(x, axis=0)
-                m.append(mu_j)
-            rates += m
+                mu = np.mean(x, axis=0)
+                sigma = np.cov(x, rowvar=False)
+                m.append(mu)
+                C.append(sigma)
+            means += m
+            covariances += C
+            n_batches += 1
 
         # Calculate the average from the running total
-        n_batches = dtf.get_n_batches(training_dataset)
-        rates /= n_batches
+        means /= n_batches
+        covariances /= n_batches
+
+        if self.config.learn_means:
+            # Set initial means
+            self.set_means(means, update_initializer=True)
+
+        if self.config.learn_covariances:
+            # Set initial covariances
+            self.set_covariances(covariances, update_initializer=True)
+
+    def sample_state_time_course(self, n_samples):
+        """Sample a state time course.
+
+        Parameters
+        ----------
+        n_samples : int
+            Number of samples.
 
-        if self.config.learn_log_rates:
-            # Set initial log_rates
-            self.set_rates(rates, update_initializer=True)
+        Returns
+        -------
+        stc : np.ndarray
+            State time course with shape (n_samples, n_states).
+        """
+        trans_prob = self.get_trans_prob()
+        sim = HMM(trans_prob)
+        stc = sim.generate_states(n_samples)
+        return stc
 
-    def free_energy(self, dataset):
-        """Get the variational free energy.
+    def free_energy(self, dataset, **kwargs):
+        """Get the variational free energy of HMM-based models.
 
         This calculates:
 
         .. math::
             \mathcal{F} = \int q(s_{1:T}) \log \left[ \
                           \\frac{q(s_{1:T})}{p(x_{1:T}, s_{1:T})} \\right] \
                           ds_{1:T}
@@ -909,45 +1488,77 @@
             Dataset to evaluate the free energy for.
 
         Returns
         -------
         free_energy : float
             Variational free energy.
         """
-        _logger.info("Getting free energy")
 
-        # Convert to a TensorFlow dataset if not already
-        dataset = self.make_dataset(dataset, concatenate=True)
+        # Helper functions
+        def _get_posterior_entropy(gamma, xi):
+            # E = int q(s_1:T) log q(s_1:T) ds_1:T
+            #   = sum_{t=1}^{T-1} int q(s_t,s_{t+1}) log q(s_t,s_{t+1}) ds_t ds_{t+1}
+            #     - sum_{t=2}^{T-1} int q(s_t) log q(s_t) ds_t
+
+            # first_term = sum^{T-1}_t=1 int q(s_t, s_t+1)
+            # log(q(s_t, s_t+1)) ds_t ds_t+1
+            first_term = xlogy(xi, xi)
+            first_term = np.sum(first_term, axis=(1, 2))
+            first_term = np.mean(first_term)
+
+            # second_term = sum^{T-1}_t=2 int q(s_t) log q(s_t) ds_t
+            second_term = xlogy(gamma, gamma)[:, 1:-1, :]
+            second_term = np.sum(second_term, axis=(1, 2))
+            second_term = np.mean(second_term)
+            return first_term - second_term
+
+        def _get_posterior_expected_prior(gamma, xi):
+            # P = int q(s_1:T) log p(s_1:T) ds
+            #   = int q(s_1) log p(s_1) ds_1
+            #     + sum_{t=1}^{T-1} int q(s_t,s_{t+1}) log p(s_{t+1}|s_t) ds_t ds_{t+1}
+
+            initial_distribution = self.get_initial_distribution()
+            trans_prob = self.get_trans_prob()
+
+            # first_term = int q(s_1) log p(s_1) ds_1
+            first_term = xlogy(gamma[:, 0, :], initial_distribution[None, ...])
+            first_term = np.sum(first_term, axis=1)
+            first_term = np.mean(first_term)
+
+            # remaining_terms =
+            # sum^{T-1}_t=1 int q(s_t, s_t+1) log p(s_t+1 | s_t}) ds_t ds_t+1
+            remaining_terms = xlogy(xi, trans_prob[None, None, ...])
+            remaining_terms = np.sum(remaining_terms, axis=(1, 2, 3))
+            remaining_terms = np.mean(remaining_terms)
 
-        # Calculate variational free energy for each batch
-        free_energy = []
-        for data in dataset:
-            x = data["data"]
-            batch_size = x.shape[0]
+            return first_term + remaining_terms
 
-            # Get the marginal and join posterior to calculate the free energy
-            gamma, xi = self.get_posterior(x)
+        if self.is_multi_gpu:
+            raise ValueError(
+                "MirroredStrategy is not supported for this method. "
+                + "Please load a new model with "
+                + "osl_dynamics.models.load(..., single_gpu=True)."
+            )
 
-            # Calculate the free energy:
-            #
-            # F = int q(s) log[q(s) / p(x, s)] ds
-            #   = int q(s) log[q(s) / p(x | s) p(s)] ds
-            #   = - int q(s) log p(x | s) ds    [log_likelihood]
-            #     + int q(s) log q(s) ds        [entropy]
-            #     - int q(s) log p(s) ds        [prior]
-
-            log_likelihood = self.get_posterior_expected_log_likelihood(x, gamma)
-            entropy = self.get_posterior_entropy(gamma, xi)
-            prior = self.get_posterior_expected_prior(gamma, xi)
-
-            # Average free energy for a sequence in this batch
-            seq_fe = (-log_likelihood + entropy - prior) / batch_size
-            free_energy.append(seq_fe)
+        dataset = self.make_dataset(dataset, concatenate=False)
+        _logger.info("Getting free energy")
+        free_energy = []
+        for ds in dataset:
+            predictions = self.predict(ds, **kwargs)
+            ll_loss = np.mean(predictions["ll_loss"])
+            entropy = _get_posterior_entropy(predictions["gamma"], predictions["xi"])
+            prior = _get_posterior_expected_prior(
+                predictions["gamma"], predictions["xi"]
+            )
+            fe = ll_loss + entropy - prior
+            if self.config.model_name == "HIVE":
+                kl_loss = np.mean(predictions["kl_loss"])
+                fe += kl_loss
+            free_energy.append(fe)
 
-        # Return average over batches
         return np.mean(free_energy)
 
     def evidence(self, dataset):
         """Calculate the model evidence, :math:`p(x)`, of HMM on a dataset.
 
         Parameters
         ----------
@@ -958,75 +1569,48 @@
         -------
         evidence : float
             Model evidence.
         """
 
         # Helper functions
         def _evidence_predict_step(log_smoothing_distribution=None):
-            """Predict step for calculating the evidence.
-
-            .. math::
-                p(s_t=j | x_{1:t-1}) = \displaystyle\sum_i p(s_t = j | s_{t-1} = i)\
-                                                        p(s_{t-1} = i | x_{1:t-1})
-
-            Parameters
-            ----------
-            log_smoothing_distribution : np.ndarray
-                :math:`\log p(s_{t-1} | x_{1:t-1})`.
-                Shape is (batch_size, n_states).
-
-            Returns
-            -------
-            log_prediction_distribution : np.ndarray
-                :math:`\log p(s_t | x_{1:t-1})`. Shape is (batch_size, n_states).
-            """
+            # Predict step for calculating the evidence
+            # p(s_t=j|x_{1:t-1}) = sum_i p(s_t=j|s_{t-1}=i) p(s_{t-1}=i|x_{1:t-1})
+            # log_smoothing_distribution.shape = (batch_size, n_states)
             if log_smoothing_distribution is None:
-                initial_distribution = self.get_stationary_distribution()
+                initial_distribution = self.get_initial_distribution()
                 log_prediction_distribution = np.broadcast_to(
                     np.expand_dims(initial_distribution, axis=0),
                     (batch_size, self.config.n_states),
                 )
             else:
-                log_trans_prob = np.expand_dims(np.log(self.trans_prob), 0)
+                log_trans_prob = np.expand_dims(np.log(self.get_trans_prob()), axis=0)
                 log_smoothing_distribution = np.expand_dims(
                     log_smoothing_distribution,
                     axis=-1,
                 )
                 log_prediction_distribution = logsumexp(
-                    log_trans_prob + log_smoothing_distribution, -2
+                    log_trans_prob + log_smoothing_distribution, axis=-2
                 )
             return log_prediction_distribution
 
         def _evidence_update_step(data, log_prediction_distribution):
-            """Update step for calculating the evidence.
+            # Update step for calculating the evidence
+            # p(s_t=j|x_{1:t}) = p(x_t|s_t=j) p(s_t=j|x_{1:t-1}) / p(x_t|x_{1:t-1})
+            # p(x_t|x_{1:t-1}) = sum_i p(x_t|s_t=i) p(s_t=i|x_{1:t-1})
+            # data.shape = (batch_size, n_channels)
+            # log_prediction_distribution.shape = (batch_size, n_states)
+
+            # Get the log-likelihood
+            means, covs = self.get_means_covariances()
+            ll_layer = self.model.get_layer("ll")
+            log_likelihood = ll_layer([data, means, covs])
 
-            .. math::
-                p(s_t = j | x_{1:t}) &= \displaystyle\\frac{p(x_t | s_t = j) \
-                                        p(s_t = j | x_{1:t-1})}{p(x_t | x_{1:t-1})}
-
-                p(x_t | x_{1:t-1}) &= \displaystyle\sum_i p(x_t | s_t = j) \
-                                                        p(s_t = i | x_{1:t-1})
-
-            Parameters
-            ----------
-            data : np.ndarray
-                Data for the update step. Shape is (batch_size, n_channels).
-            log_prediction_distribution : np.ndarray
-                :math:`\log p(s_t | x_{1:t-1})`. Shape is (batch_size, n_states).
-
-            Returns
-            -------
-            log_smoothing_distribution : np.ndarray
-                :math:`\log p(s_t | x_{1:t})`. Shape is (batch_size, n_states).
-            predictive_log_likelihood : np.ndarray
-                :math:`\log p(x_t | x_{1:t-1})`. Shape is (batch_size,).
-            """
-            log_likelihood = self.get_log_likelihood(data)
             log_smoothing_distribution = log_likelihood + log_prediction_distribution
-            predictive_log_likelihood = logsumexp(log_smoothing_distribution, -1)
+            predictive_log_likelihood = logsumexp(log_smoothing_distribution, axis=-1)
 
             # Normalise the log smoothing distribution
             log_smoothing_distribution -= np.expand_dims(
                 predictive_log_likelihood,
                 axis=-1,
             )
             return log_smoothing_distribution, predictive_log_likelihood
@@ -1037,15 +1621,15 @@
 
         evidence = 0
         for n, data in enumerate(dataset):
             x = data["data"]
             print("Batch {}/{}".format(n + 1, n_batches))
             pb_i = utils.Progbar(self.config.sequence_length)
             batch_size = tf.shape(x)[0]
-            batch_evidence = np.zeros((batch_size))
+            batch_evidence = np.zeros(batch_size, dtype=np.float32)
             log_smoothing_distribution = None
             for t in range(self.config.sequence_length):
                 # Prediction step
                 log_prediction_distribution = _evidence_predict_step(
                     log_smoothing_distribution
                 )
 
@@ -1057,379 +1641,7 @@
 
                 # Update the batch evidence
                 batch_evidence += predictive_log_likelihood
                 pb_i.add(1)
             evidence += np.mean(batch_evidence)
 
         return evidence / n_batches
-
-    def get_alpha(self, dataset, concatenate=False, remove_edge_effects=False):
-        """Get state probabilities.
-
-        Parameters
-        ----------
-        dataset : tf.data.Dataset or osl_dynamics.data.Data
-            Prediction dataset. This can be a list of datasets, one for
-            each session.
-        concatenate : bool, optional
-            Should we concatenate alpha for each session?
-        remove_edge_effects : bool, optional
-            Edge effects can arise due to separating the data into sequences.
-            We can remove these by predicting overlapping :code:`alpha` and
-            disregarding the :code:`alpha` near the ends. Passing :code:`True`
-            does this by using sequences with 50% overlap and throwing away the
-            first and last 25% of predictions.
-
-        Returns
-        -------
-        alpha : list or np.ndarray
-            State probabilities with shape (n_sessions, n_samples, n_states)
-            or (n_samples, n_states).
-        """
-        if remove_edge_effects:
-            step_size = self.config.sequence_length // 2  # 50% overlap
-            trim = step_size // 2  # throw away 25%
-        else:
-            step_size = None
-
-        dataset = self.make_dataset(dataset, step_size=step_size)
-
-        n_datasets = len(dataset)
-        if len(dataset) > 1:
-            iterator = trange(n_datasets, desc="Getting alpha")
-        else:
-            iterator = range(n_datasets)
-            _logger.info("Getting alpha")
-
-        alpha = []
-        for i in iterator:
-            gamma = []
-            for j, data in enumerate(dataset[i]):
-                n_batches = dtf.get_n_batches(dataset[i])
-                x = data["data"]
-                g, _ = self.get_posterior(x)
-                if remove_edge_effects:
-                    batch_size, sequence_length, _ = x.shape
-                    n_states = g.shape[-1]
-                    g = g.reshape(batch_size, sequence_length, n_states)
-                    if j == 0:
-                        g = [
-                            g[0, :-trim],
-                            g[1:, trim:-trim].reshape(-1, n_states),
-                        ]
-                    elif j == n_batches - 1:
-                        g = [
-                            g[:-1, trim:-trim].reshape(-1, n_states),
-                            g[-1, trim:],
-                        ]
-                    else:
-                        g = [g[:, trim:-trim].reshape(-1, n_states)]
-                    g = np.concatenate(g).reshape(-1, n_states)
-                gamma.append(g)
-            alpha.append(np.concatenate(gamma).astype(np.float32))
-
-        if concatenate or len(alpha) == 1:
-            alpha = np.concatenate(alpha)
-
-        return alpha
-
-    def get_n_params_generative_model(self):
-        """Get the number of trainable parameters in the generative model.
-
-        This includes the transition probabiltity matrix, state :code:`log_rates`.
-
-        Returns
-        -------
-        n_params : int
-            Number of parameters in the generative model.
-        """
-        n_params = 0
-        if self.config.learn_trans_prob:
-            n_params += self.config.n_states * (self.config.n_states - 1)
-
-        for var in self.trainable_weights:
-            var_name = var.name
-            if "log_rates" in var_name:
-                n_params += np.prod(var.shape)
-
-        return int(n_params)
-
-    def bayesian_information_criterion(self, dataset, loss_type="free_energy"):
-        """Calculate the Bayesian Information Criterion (BIC) for the model.
-
-        Parameters
-        ----------
-        dataset : osl_dynamics.data.Data
-            Dataset to calculate the BIC for.
-        loss_type : str, optional
-            Which loss to use for the BIC. Can be :code:`"free_energy"`
-            or :code:`"evidence"`.
-
-        Returns
-        -------
-        bic : float
-            Bayesian Information Criterion for the model (for each sequence).
-        """
-        if loss_type == "free_energy":
-            loss = self.free_energy(dataset)
-        elif loss_type == "evidence":
-            loss = -self.evidence(dataset)
-        else:
-            raise ValueError("loss_type must be 'free_energy' or 'evidence'")
-
-        n_params = self.get_n_params_generative_model()
-        n_sequences = dtf.n_batches(
-            dataset.time_series(concatenate=True), self.config.sequence_length
-        )
-
-        bic = (
-            2 * loss
-            + (np.log(self.config.sequence_length) + np.log(n_sequences))
-            * n_params
-            / n_sequences
-        )
-        return bic
-
-    def fine_tuning(
-        self, training_data, n_epochs=None, learning_rate=None, store_dir="tmp"
-    ):
-        """Fine tuning the model for each session.
-
-        Here, we estimate the posterior distribution (state probabilities)
-        and observation model using the data from a single session with the
-        group-level transition probability matrix held fixed.
-
-        Parameters
-        ----------
-        training_data : osl_dynamics.data.Data
-            Training dataset.
-        n_epochs : int, optional
-            Number of epochs to train for. Defaults to the value in the
-            :code:`config` used to create the model.
-        learning_rate : float, optional
-            Learning rate. Defaults to the value in the :code:`config` used
-            to create the model.
-        store_dir : str, optional
-            Directory to temporarily store the model in.
-
-        Returns
-        -------
-        alpha : list of np.ndarray
-            Session-specific mixing coefficients.
-            Each element has shape (n_samples, n_states).
-        log_rates : np.ndarray
-            Session-specific :code:`log_rates`.
-            Shape is (n_sessions, n_states, n_channels).
-        """
-        # Save group-level model parameters
-        os.makedirs(store_dir, exist_ok=True)
-        self.save_weights(f"{store_dir}/weights.h5")
-
-        # Temporarily change hyperparameters
-        original_n_epochs = self.config.n_epochs
-        original_learning_rate = self.config.learning_rate
-        original_learn_trans_prob = self.config.learn_trans_prob
-        self.config.n_epochs = n_epochs or self.config.n_epochs
-        self.config.learning_rate = learning_rate or self.config.learning_rate
-        self.config.learn_trans_prob = False
-
-        # Reset the optimiser
-        self.compile()
-
-        # Fine tune the model for each session
-        alpha = []
-        log_rates = []
-        with set_logging_level(_logger, logging.WARNING):
-            for i in trange(training_data.n_sessions, desc="Fine tuning"):
-                # Train on this session
-                with training_data.set_keep(i):
-                    self.fit(training_data, verbose=0)
-                    a = self.get_alpha(training_data, concatenate=True)
-
-                # Get the inferred parameters
-                m = self.get_log_rates()
-                alpha.append(a)
-                log_rates.append(m)
-
-                # Reset back to group-level model parameters
-                self.load_weights(f"{store_dir}/weights.h5")
-                self.compile()
-
-        # Reset hyperparameters
-        self.config.n_epochs = original_n_epochs
-        self.config.learning_rate = original_learning_rate
-        self.config.learn_trans_prob = original_learn_trans_prob
-
-        return alpha, np.array(log_rates)
-
-    def dual_estimation(self, training_data, alpha=None, n_jobs=1):
-        """Dual estimation to get session-specific observation model parameters.
-
-        Here, we estimate the state :code:`log_rates` for sessions
-        with the posterior distribution of the states held fixed.
-
-        Parameters
-        ----------
-        training_data : osl_dynamics.data.Data
-            Prepared training data object.
-        alpha : list of np.ndarray, optional
-            Posterior distribution of the states. Shape is
-            (n_sessions, n_samples, n_states).
-        n_jobs : int, optional
-            Number of jobs to run in parallel.
-
-        Returns
-        -------
-        log_rates : np.ndarray
-            Session-specific :code:`log_rates`.
-            Shape is (n_sessions, n_states, n_channels).
-        """
-        if alpha is None:
-            # Get the posterior
-            alpha = self.get_alpha(training_data, concatenate=False)
-
-        # Validation
-        if isinstance(alpha, np.ndarray):
-            alpha = [alpha]
-
-        # Get the session-specific data
-        data = training_data.time_series(prepared=True, concatenate=False)
-
-        if len(alpha) != len(data):
-            raise ValueError(
-                "len(alpha) and training_data.n_sessions must be the same."
-            )
-
-        # Make sure the data and alpha have the same number of samples
-        data = [d[: a.shape[0]] for d, a in zip(data, alpha)]
-
-        n_states = self.config.n_states
-        n_channels = self.config.n_channels
-
-        # Helper function for dual estimation for a single session
-        def _single_dual_estimation(a, x):
-            sum_a = np.sum(a, axis=0)
-            if self.config.learn_log_rates:
-                session_log_rates = np.empty((n_states, n_channels))
-                for state in range(n_states):
-                    session_log_rates[state] = (
-                        np.sum(x * a[:, state, None], axis=0) / sum_a[state]
-                    )
-            else:
-                session_log_rates = self.get_log_rates()
-
-            return session_log_rates
-
-        # Setup keyword arguments to pass to the helper function
-        kwargs = []
-        for a, x in zip(alpha, data):
-            kwargs.append({"a": a, "x": x})
-
-        if len(data) == 1:
-            _logger.info("Dual estimation")
-            results = [_single_dual_estimation(**kwargs[0])]
-
-        elif n_jobs == 1:
-            results = []
-            for i in trange(len(data), desc="Dual estimation"):
-                results.append(_single_dual_estimation(**kwargs[i]))
-
-        else:
-            _logger.info("Dual estimation")
-            results = pqdm(
-                kwargs,
-                _single_dual_estimation,
-                argument_type="kwargs",
-                n_jobs=n_jobs,
-            )
-
-        # Unpack the results
-        log_rates = []
-        for result in results:
-            m = result
-            log_rates.append(m)
-
-        return np.squeeze(log_rates)
-
-    def save_weights(self, filepath):
-        """Save all model weights.
-
-        Parameters
-        ----------
-        filepath : str
-            Location to save model weights to.
-        """
-        self.model.save_weights(filepath)
-        np.save(
-            op.join(str(Path(filepath).parent), "trans_prob.npy"),
-            self.trans_prob,
-        )
-
-    def load_weights(self, filepath):
-        """Load all model parameters.
-
-        Parameters
-        ----------
-        filepath : str
-            Location to load model weights from.
-        """
-        self.trans_prob = np.load(
-            op.join(str(Path(filepath).parent), "trans_prob.npy"),
-        )
-        return self.model.load_weights(filepath)
-
-    def get_weights(self):
-        """Get model parameter weights.
-
-        Returns
-        -------
-        weights : tensorflow weights
-            TensorFlow weights for the observation model.
-        trans_prob : np.ndarray
-            Transition probability matrix.
-        """
-        return self.model.get_weights(), self.trans_prob
-
-    def set_weights(self, weights, trans_prob):
-        """Set model parameter weights.
-
-        Parameters
-        ----------
-        weights : tensorflow weights
-            TensorFlow weights for the observation model.
-        trans_prob : np.ndarray
-            Transition probability matrix.
-        """
-        self.model.set_weights(weights)
-        self.set_trans_prob(trans_prob)
-
-    def reset_weights(self):
-        """Resets trainable variables in the model to their initial value."""
-        initializers.reinitialize_model_weights(self.model)
-        self.set_trans_prob(self.config.initial_trans_prob)
-
-
-def _model_structure(config):
-    # Inputs
-    inputs = layers.Input(
-        shape=(config.sequence_length, config.n_channels + config.n_states),
-        name="inputs",
-    )
-    data, gamma = tf.split(inputs, [config.n_channels, config.n_states], axis=2)
-
-    # Definition of layers
-    log_rates_layer = VectorsLayer(
-        config.n_states,
-        config.n_channels,
-        config.learn_log_rates,
-        config.initial_log_rates,
-        name="log_rates",
-    )
-    ll_loss_layer = CategoricalPoissonLogLikelihoodLossLayer(
-        config.n_states, name="ll_loss"
-    )
-
-    # Data flow
-    mu = log_rates_layer(data)  # data not used
-    ll_loss = ll_loss_layer([data, mu, gamma, None])
-
-    return tf.keras.Model(inputs=inputs, outputs=[ll_loss], name="HMM-Poisson")
```

### Comparing `osl-dynamics-1.3.1/osl_dynamics/models/mage.py` & `osl_dynamics-1.3.2/osl_dynamics/models/mage.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/models/mdynemo.py` & `osl_dynamics-1.3.2/osl_dynamics/models/mdynemo.py`

 * *Files 13% similar despite different names*

```diff
@@ -48,17 +48,17 @@
     """Settings for M-DyNeMo.
 
     Parameters
     ----------
     model_name : str
         Model name.
     n_modes : int
-        Number of modes for both power.
-    n_fc_modes : int
-        Number of modes for functional connectivity.
+        Number of modes.
+    n_corr_modes : int
+        Number of modes for correlation.
         If :code:`None`, then set to :code:`n_modes`.
     n_channels : int
         Number of channels.
     sequence_length : int
         Length of sequence passed to the inference network and generative model.
 
     inference_rnn : str
@@ -101,31 +101,31 @@
         The same parameter is used for the :code:`gamma` time course.
 
 
     learn_means : bool
         Should we make the mean for each mode trainable?
     learn_stds : bool
         Should we make the standard deviation for each mode trainable?
-    learn_fcs : bool
-        Should we make the functional connectivity for each mode trainable?
+    learn_corrs : bool
+        Should we make the correlation for each mode trainable?
     initial_means : np.ndarray
         Initialisation for the mode means.
     initial_stds : np.ndarray
         Initialisation for mode standard deviations.
-    initial_fcs : np.ndarray
-        Initialisation for mode functional connectivity matrices.
+    initial_corrs : np.ndarray
+        Initialisation for mode correlation matrices.
     stds_epsilon : float
         Error added to mode stds for numerical stability.
-    fcs_epsilon : float
-        Error added to mode fcs for numerical stability.
+    corrs_epsilon : float
+        Error added to mode corrs for numerical stability.
     means_regularizer : tf.keras.regularizers.Regularizer
         Regularizer for the mean vectors.
     stds_regularizer : tf.keras.regularizers.Regularizer
         Regularizer for the standard deviation vectors.
-    fcs_regularizer : tf.keras.regularizers.Regularizer
+    corrs_regularizer : tf.keras.regularizers.Regularizer
         Regularizer for the correlation matrices.
 
     do_kl_annealing : bool
         Should we use KL annealing during training?
     kl_annealing_curve : str
         Type of KL annealing curve. Either :code:`'linear'` or :code:`'tanh'`.
     kl_annealing_sharpness : float
@@ -171,26 +171,26 @@
     model_n_units: int = None
     model_normalization: str = None
     model_activation: str = None
     model_dropout: float = 0.0
     model_regularizer: str = None
 
     # Observation model parameters
-    n_fc_modes: int = None
+    n_corr_modes: int = None
     learn_means: bool = None
     learn_stds: bool = None
-    learn_fcs: bool = None
+    learn_corrs: bool = None
     initial_means: np.ndarray = None
     initial_stds: np.ndarray = None
-    initial_fcs: np.ndarray = None
+    initial_corrs: np.ndarray = None
     stds_epsilon: float = None
-    fcs_epsilon: float = None
+    corrs_epsilon: float = None
     means_regularizer: tf.keras.regularizers.Regularizer = None
     stds_regularizer: tf.keras.regularizers.Regularizer = None
-    fcs_regularizer: tf.keras.regularizers.Regularizer = None
+    corrs_regularizer: tf.keras.regularizers.Regularizer = None
     multiple_dynamics: bool = True
 
     pca_components: np.ndarray = None
 
     def __post_init__(self):
         self.validate_rnn_parameters()
         self.validate_observation_model_parameters()
@@ -206,39 +206,39 @@
         if self.model_n_units is None:
             raise ValueError("Please pass model_n_units.")
 
     def validate_observation_model_parameters(self):
         if (
             self.learn_means is None
             or self.learn_stds is None
-            or self.learn_fcs is None
+            or self.learn_corrs is None
         ):
-            raise ValueError("learn_means, learn_stds and learn_fcs must be passed.")
+            raise ValueError("learn_means, learn_stds and learn_corrs must be passed.")
 
         if self.stds_epsilon is None:
             if self.learn_stds:
                 self.stds_epsilon = 1e-6
             else:
                 self.stds_epsilon = 0.0
 
-        if self.fcs_epsilon is None:
-            if self.learn_fcs:
-                self.fcs_epsilon = 1e-6
+        if self.corrs_epsilon is None:
+            if self.learn_corrs:
+                self.corrs_epsilon = 1e-6
             else:
-                self.fcs_epsilon = 0.0
+                self.corrs_epsilon = 0.0
 
         if self.pca_components is None:
             self.pca_components = np.eye(self.n_channels)
         self.pca_components = self.pca_components.astype(np.float32)
 
     def validate_dimension_parameters(self):
         super().validate_dimension_parameters()
-        if self.n_fc_modes is None:
-            self.n_fc_modes = self.n_modes
-            _logger.warning("n_fc_modes is None, set to n_modes.")
+        if self.n_corr_modes is None:
+            self.n_corr_modes = self.n_modes
+            _logger.warning("n_corr_modes is None, set to n_modes.")
 
 
 class Model(VariationalInferenceModelBase):
     """M-DyNeMo model class.
 
     Parameters
     ----------
@@ -267,47 +267,47 @@
         Returns
         -------
         stds : np.ndarray
             Mode standard deviations. Shape (n_modes, n_channels, n_channels).
         """
         return obs_mod.get_observation_model_parameter(self.model, "stds")
 
-    def get_fcs(self):
-        """Get the mode functional connectivities.
+    def get_corrs(self):
+        """Get the mode correlations.
 
         Returns
         -------
-        fcs : np.ndarray
-            Mode functional connectivities.
+        corrs : np.ndarray
+            Mode correlations.
             Shape (n_modes, n_channels, n_channels).
         """
-        return obs_mod.get_observation_model_parameter(self.model, "fcs")
+        return obs_mod.get_observation_model_parameter(self.model, "corrs")
 
-    def get_means_stds_fcs(self):
-        """Get the mode means, standard deviations, functional connectivities.
+    def get_means_stds_corrs(self):
+        """Get the mode means, standard deviations, correlations.
 
         This is a wrapper for :code:`get_means`, :code:`get_stds`,
-        :code:`get_fcs`.
+        :code:`get_corrs`.
 
         Returns
         -------
         means : np.ndarray
             Mode means. Shape is (n_modes, n_channels).
         stds : np.ndarray
             Mode standard deviations.
             Shape is (n_modes, n_channels, n_channels).
-        fcs : np.ndarray
-            Mode functional connectivities.
+        corrs : np.ndarray
+            Mode correlations.
             Shape is (n_modes, n_channels, n_channels).
         """
-        return self.get_means(), self.get_stds(), self.get_fcs()
+        return self.get_means(), self.get_stds(), self.get_corrs()
 
     def get_observation_model_parameters(self):
-        """Wrapper for :code:`get_means_stds_fcs`."""
-        return self.get_means_stds_fcs()
+        """Wrapper for :code:`get_means_stds_corrs`."""
+        return self.get_means_stds_corrs()
 
     def set_means(self, means, update_initializer=True):
         """Set the mode means.
 
         Parameters
         ----------
         means : np.ndarray
@@ -338,52 +338,52 @@
         obs_mod.set_observation_model_parameter(
             self.model,
             stds,
             layer_name="stds",
             update_initializer=update_initializer,
         )
 
-    def set_fcs(self, fcs, update_initializer=True):
-        """Set the mode functional connectivities.
+    def set_corrs(self, corrs, update_initializer=True):
+        """Set the mode correlations.
 
         Parameters
         ----------
-        fcs : np.ndarray
-            Mode functional connectivities.
+        corrs : np.ndarray
+            Mode correlations.
             Shape is (n_modes, n_channels, n_channels).
         update_initializer : bool
             Do we want to use the passed parameters when we re-initialize
             the model?
         """
         obs_mod.set_observation_model_parameter(
             self.model,
-            fcs,
-            layer_name="fcs",
+            corrs,
+            layer_name="corrs",
             update_initializer=update_initializer,
         )
 
-    def set_means_stds_fcs(self, means, stds, fcs, update_initializer=True):
-        """This is a wrapper for set_means, set_stds, set_fcs."""
+    def set_means_stds_corrs(self, means, stds, corrs, update_initializer=True):
+        """This is a wrapper for set_means, set_stds, set_corrs."""
         self.set_means(means, update_initializer=update_initializer)
         self.set_stds(stds, update_initializer=update_initializer)
-        self.set_fcs(fcs, update_initializer=update_initializer)
+        self.set_corrs(corrs, update_initializer=update_initializer)
 
     def set_observation_model_parameters(
         self, observation_model_parameters, update_initializer=True
     ):
-        """Wrapper for set_means_stds_fcs."""
-        self.set_means_stds_fcs(
+        """Wrapper for set_means_stds_corrs."""
+        self.set_means_stds_corrs(
             observation_model_parameters[0],
             observation_model_parameters[1],
             observation_model_parameters[2],
             update_initializer=update_initializer,
         )
 
     def set_regularizers(self, training_dataset):
-        """Set the regularizers of means, stds and fcs based on the training
+        """Set the regularizers of means, stds and corrs based on the training
         data.
 
         A multivariate normal prior is applied to the mean vectors with
         :code:`mu=0`, :code:`sigma=diag((range/2)**2)`, a log normal prior is
         applied to the standard deviations with :code:`mu=0`,
         :code:`sigma=sqrt(log(2*range))` and a marginal inverse Wishart prior
         is applied to the functional connectivity matrices with
@@ -400,126 +400,128 @@
             obs_mod.set_means_regularizer(self.model, training_dataset)
 
         if self.config.learn_stds:
             obs_mod.set_stds_regularizer(
                 self.model, training_dataset, self.config.stds_epsilon
             )
 
-        if self.config.learn_fcs:
-            obs_mod.set_fcs_regularizer(
-                self.model, training_dataset, self.config.fcs_epsilon
+        if self.config.learn_corrs:
+            obs_mod.set_corrs_regularizer(
+                self.model, training_dataset, self.config.corrs_epsilon
             )
 
-    def sample_time_courses(self, n_samples: int):
+    def sample_time_courses(self, n_samples):
         """Uses the model RNN to sample mode mixing factors,
-        :code:`alpha` and :code:`gamma`.
+        :code:`alpha` and :code:`beta`.
 
         Parameters
         ----------
         n_samples : int
             Number of samples to take.
 
         Returns
         -------
         alpha : np.ndarray
             Sampled :code:`alpha`.
-        gamma : np.ndarray
-            Sampled :code:`gamma`.
+        beta : np.ndarray
+            Sampled :code:`beta`.
         """
         # Get layers
         model_rnn_layer = self.model.get_layer("mod_rnn")
-        mean_mod_mu_layer = self.model.get_layer("mean_mod_mu")
-        mean_mod_sigma_layer = self.model.get_layer("mean_mod_sigma")
-        mean_theta_norm_layer = self.model.get_layer("mean_theta_norm")
+        power_mod_mu_layer = self.model.get_layer("power_mod_mu")
+        power_mod_sigma_layer = self.model.get_layer("power_mod_sigma")
+        power_theta_norm_layer = self.model.get_layer("power_theta_norm")
         alpha_layer = self.model.get_layer("alpha")
         fc_mod_mu_layer = self.model.get_layer("fc_mod_mu")
         fc_mod_sigma_layer = self.model.get_layer("fc_mod_sigma")
         fc_theta_norm_layer = self.model.get_layer("fc_theta_norm")
-        gamma_layer = self.model.get_layer("gamma")
+        beta_layer = self.model.get_layer("beta")
         concatenate_layer = self.model.get_layer("theta_norm")
 
         # Normally distributed random numbers used to sample the logits theta
-        mean_epsilon = np.random.normal(
+        power_epsilon = np.random.normal(
             0, 1, [n_samples + 1, self.config.n_modes]
         ).astype(np.float32)
         fc_epsilon = np.random.normal(
-            0, 1, [n_samples + 1, self.config.n_fc_modes]
+            0, 1, [n_samples + 1, self.config.n_corr_modes]
         ).astype(np.float32)
 
         # Initialise sequence of underlying logits theta
-        mean_theta_norm = np.zeros(
+        power_theta_norm = np.zeros(
             [self.config.sequence_length, self.config.n_modes],
             dtype=np.float32,
         )
-        mean_theta_norm[-1] = np.random.normal(size=self.config.n_modes)
+        power_theta_norm[-1] = np.random.normal(size=self.config.n_modes)
         fc_theta_norm = np.zeros(
-            [self.config.sequence_length, self.config.n_fc_modes],
+            [self.config.sequence_length, self.config.n_corr_modes],
             dtype=np.float32,
         )
-        fc_theta_norm[-1] = np.random.normal(size=self.config.n_fc_modes)
+        fc_theta_norm[-1] = np.random.normal(size=self.config.n_corr_modes)
 
         # Sample the mode time courses
         alpha = np.empty([n_samples, self.config.n_modes])
-        gamma = np.empty([n_samples, self.config.n_fc_modes])
+        beta = np.empty([n_samples, self.config.n_corr_modes])
         for i in trange(n_samples, desc="Sampling mode time courses"):
             # If there are leading zeros we trim theta so that we don't pass
             # the zeros
-            trimmed_mean_theta = mean_theta_norm[~np.all(mean_theta_norm == 0, axis=1)][
-                np.newaxis, :, :
-            ]
+            trimmed_power_theta = power_theta_norm[
+                ~np.all(power_theta_norm == 0, axis=1)
+            ][np.newaxis, :, :]
             trimmed_fc_theta = fc_theta_norm[~np.all(fc_theta_norm == 0, axis=1)][
                 np.newaxis, :, :
             ]
-            trimmed_theta = concatenate_layer([trimmed_mean_theta, trimmed_fc_theta])
+            trimmed_theta = concatenate_layer([trimmed_power_theta, trimmed_fc_theta])
             # p(theta|theta_<t) ~ N(mod_mu, sigma_theta_jt)
             model_rnn = model_rnn_layer(trimmed_theta)
-            mean_mod_mu = mean_mod_mu_layer(model_rnn)[0, -1]
-            mean_mod_sigma = mean_mod_sigma_layer(model_rnn)[0, -1]
+            power_mod_mu = power_mod_mu_layer(model_rnn)[0, -1]
+            power_mod_sigma = power_mod_sigma_layer(model_rnn)[0, -1]
             fc_mod_mu = fc_mod_mu_layer(model_rnn)[0, -1]
             fc_mod_sigma = fc_mod_sigma_layer(model_rnn)[0, -1]
 
             # Shift theta one time step to the left
-            mean_theta_norm = np.roll(mean_theta_norm, -1, axis=0)
+            power_theta_norm = np.roll(power_theta_norm, -1, axis=0)
             fc_theta_norm = np.roll(fc_theta_norm, -1, axis=0)
 
             # Sample from the probability distribution function
-            mean_theta = mean_mod_mu + mean_mod_sigma * mean_epsilon[i]
-            mean_theta_norm[-1] = mean_theta_norm_layer(
-                mean_theta[np.newaxis, np.newaxis, :]
+            power_theta = power_mod_mu + power_mod_sigma * power_epsilon[i]
+            power_theta_norm[-1] = power_theta_norm_layer(
+                power_theta[np.newaxis, np.newaxis, :]
             )
             fc_theta = fc_mod_mu + fc_mod_sigma * fc_epsilon[i]
             fc_theta_norm[-1] = fc_theta_norm_layer(fc_theta[np.newaxis, np.newaxis, :])
 
-            alpha[i] = alpha_layer(mean_theta_norm[-1][np.newaxis, np.newaxis, :])[0, 0]
-            gamma[i] = gamma_layer(fc_theta_norm[-1][np.newaxis, np.newaxis, :])[0, 0]
+            alpha[i] = alpha_layer(power_theta_norm[-1][np.newaxis, np.newaxis, :])[
+                0, 0
+            ]
+            beta[i] = beta_layer(fc_theta_norm[-1][np.newaxis, np.newaxis, :])[0, 0]
 
-        return alpha, gamma
+        return alpha, beta
 
     def get_n_params_generative_model(self):
         """Get the number of trainable parameters in the generative model.
 
         This includes the model RNN weights and biases, mixing coefficients,
-        mode means and covariances.
+        mode means, standard deviations and correlations.
 
         Returns
         -------
         n_params : int
             Number of parameters in the generative model.
         """
         n_params = 0
 
         for var in self.trainable_weights:
             var_name = var.name
             if (
                 "mod_" in var_name
                 or "alpha" in var_name
-                or "gamma" in var_name
+                or "beta" in var_name
                 or "means" in var_name
                 or "stds" in var_name
-                or "fcs" in var_name
+                or "corrs" in var_name
             ):
                 n_params += np.prod(var.shape)
 
             return int(n_params)
 
 
 def _model_structure(config):
@@ -552,68 +554,68 @@
     )
 
     # Data flow
     data_drop = data_drop_layer(inputs)
     inf_rnn = inf_rnn_layer(data_drop)
 
     #
-    # Mode time course for the mean and standard deviation
+    # Mode time course for Power
     #
 
     # Layers
-    mean_inf_mu_layer = layers.Dense(config.n_modes, name="mean_inf_mu")
-    mean_inf_sigma_layer = layers.Dense(
-        config.n_modes, activation="softplus", name="mean_inf_sigma"
+    power_inf_mu_layer = layers.Dense(config.n_modes, name="power_inf_mu")
+    power_inf_sigma_layer = layers.Dense(
+        config.n_modes, activation="softplus", name="power_inf_sigma"
     )
-    mean_theta_layer = SampleNormalDistributionLayer(
-        config.theta_std_epsilon, name="mean_theta"
+    power_theta_layer = SampleNormalDistributionLayer(
+        config.theta_std_epsilon, name="power_theta"
     )
-    mean_theta_norm_layer = NormalizationLayer(
-        config.theta_normalization, name="mean_theta_norm"
+    power_theta_norm_layer = NormalizationLayer(
+        config.theta_normalization, name="power_theta_norm"
     )
     alpha_layer = SoftmaxLayer(
         initial_temperature=1.0,
         learn_temperature=False,
         name="alpha",
     )
 
     # Data flow
-    mean_inf_mu = mean_inf_mu_layer(inf_rnn)
-    mean_inf_sigma = mean_inf_sigma_layer(inf_rnn)
-    mean_theta = mean_theta_layer([mean_inf_mu, mean_inf_sigma])
-    mean_theta_norm = mean_theta_norm_layer(mean_theta)
-    alpha = alpha_layer(mean_theta_norm)
+    power_inf_mu = power_inf_mu_layer(inf_rnn)
+    power_inf_sigma = power_inf_sigma_layer(inf_rnn)
+    power_theta = power_theta_layer([power_inf_mu, power_inf_sigma])
+    power_theta_norm = power_theta_norm_layer(power_theta)
+    alpha = alpha_layer(power_theta_norm)
 
     #
     # Mode time course for the FCs
     #
 
     # Layers
-    fc_inf_mu_layer = layers.Dense(config.n_fc_modes, name="fc_inf_mu")
+    fc_inf_mu_layer = layers.Dense(config.n_corr_modes, name="fc_inf_mu")
     fc_inf_sigma_layer = layers.Dense(
-        config.n_fc_modes, activation="softplus", name="fc_inf_sigma"
+        config.n_corr_modes, activation="softplus", name="fc_inf_sigma"
     )
     fc_theta_layer = SampleNormalDistributionLayer(
         config.theta_std_epsilon, name="fc_theta"
     )
     fc_theta_norm_layer = NormalizationLayer(
         config.theta_normalization, name="fc_theta_norm"
     )
-    gamma_layer = SoftmaxLayer(
+    beta_layer = SoftmaxLayer(
         initial_temperature=1.0,
         learn_temperature=False,
-        name="gamma",
+        name="beta",
     )
 
     # Data flow
     fc_inf_mu = fc_inf_mu_layer(inf_rnn)
     fc_inf_sigma = fc_inf_sigma_layer(inf_rnn)
     fc_theta = fc_theta_layer([fc_inf_mu, fc_inf_sigma])
     fc_theta_norm = fc_theta_norm_layer(fc_theta)
-    gamma = gamma_layer(fc_theta_norm)
+    beta = beta_layer(fc_theta_norm)
 
     #
     # Observation model
     #
 
     # Layers
     means_layer = VectorsLayer(
@@ -629,42 +631,42 @@
         config.n_channels,
         config.learn_stds,
         config.initial_stds,
         config.stds_epsilon,
         config.stds_regularizer,
         name="stds",
     )
-    fcs_layer = CorrelationMatricesLayer(
-        config.n_fc_modes,
+    corrs_layer = CorrelationMatricesLayer(
+        config.n_corr_modes,
         config.n_channels,
-        config.learn_fcs,
-        config.initial_fcs,
-        config.fcs_epsilon,
-        config.fcs_regularizer,
-        name="fcs",
+        config.learn_corrs,
+        config.initial_corrs,
+        config.corrs_epsilon,
+        config.corrs_regularizer,
+        name="corrs",
     )
     mix_means_layer = MixVectorsLayer(name="mix_means")
     mix_stds_layer = MixMatricesLayer(name="mix_stds")
-    mix_fcs_layer = MixMatricesLayer(name="mix_fcs")
+    mix_corrs_layer = MixMatricesLayer(name="mix_corrs")
     matmul_layer = MatMulLayer(name="cov")
     pca_means_layer = MatMulLayer(name="pca_means")
     pca_stds_layer = MatMulLayer(name="pca_stds")
-    pca_fcs_layer = MatMulLayer(name="pca_fcs")
+    pca_corrs_layer = MatMulLayer(name="pca_corrs")
     ll_loss_layer = LogLikelihoodLossLayer(
-        np.maximum(config.stds_epsilon, config.fcs_epsilon), name="ll_loss"
+        np.maximum(config.stds_epsilon, config.corrs_epsilon), name="ll_loss"
     )
 
     # Data flow
     mu = means_layer(
         inputs, static_loss_scaling_factor=static_loss_scaling_factor
     )  # inputs not used
     E = stds_layer(
         inputs, static_loss_scaling_factor=static_loss_scaling_factor
     )  # inputs not used
-    D = fcs_layer(
+    R = corrs_layer(
         inputs, static_loss_scaling_factor=static_loss_scaling_factor
     )  # inputs not used
 
     # multiply with pca components
     pca_mu = tf.squeeze(
         pca_means_layer(
             [
@@ -676,25 +678,25 @@
     pca_E = pca_stds_layer(
         [
             tf.expand_dims(tf.transpose(config.pca_components), 0),
             E,
             tf.expand_dims(config.pca_components, 0),
         ]
     )
-    pca_D = pca_fcs_layer(
+    pca_R = pca_corrs_layer(
         [
             tf.expand_dims(tf.transpose(config.pca_components), 0),
-            D,
+            R,
             tf.expand_dims(config.pca_components, 0),
         ]
     )
 
     m = mix_means_layer([alpha, pca_mu])
     G = mix_stds_layer([alpha, pca_E])
-    F = mix_fcs_layer([gamma, pca_D])
+    F = mix_corrs_layer([beta, pca_R])
     C = matmul_layer([G, F, G])
 
     ll_loss = ll_loss_layer([inputs, m, C])
 
     #
     # Model RNN
     #
@@ -713,47 +715,47 @@
         config.model_n_units,
         config.model_dropout,
         config.model_regularizer,
         name="mod_rnn",
     )
 
     # Data flow
-    theta_norm = concatenate_layer([mean_theta_norm, fc_theta_norm])
+    theta_norm = concatenate_layer([power_theta_norm, fc_theta_norm])
     theta_norm_drop = theta_norm_drop_layer(theta_norm)
     mod_rnn = mod_rnn_layer(theta_norm_drop)
 
     #
     # Mode time course for the mean
     #
 
     # Layers
-    mean_mod_mu_layer = layers.Dense(config.n_modes, name="mean_mod_mu")
-    mean_mod_sigma_layer = layers.Dense(
-        config.n_modes, activation="softplus", name="mean_mod_sigma"
+    power_mod_mu_layer = layers.Dense(config.n_modes, name="power_mod_mu")
+    power_mod_sigma_layer = layers.Dense(
+        config.n_modes, activation="softplus", name="power_mod_sigma"
     )
-    kl_div_layer_mean = KLDivergenceLayer(
+    kl_div_layer_power = KLDivergenceLayer(
         config.theta_std_epsilon,
-        name="mean_kl_div",
+        name="power_kl_div",
     )
 
     # Data flow
-    mean_mod_mu = mean_mod_mu_layer(mod_rnn)
-    mean_mod_sigma = mean_mod_sigma_layer(mod_rnn)
-    mean_kl_div = kl_div_layer_mean(
-        [mean_inf_mu, mean_inf_sigma, mean_mod_mu, mean_mod_sigma]
+    power_mod_mu = power_mod_mu_layer(mod_rnn)
+    power_mod_sigma = power_mod_sigma_layer(mod_rnn)
+    power_kl_div = kl_div_layer_power(
+        [power_inf_mu, power_inf_sigma, power_mod_mu, power_mod_sigma]
     )
 
     #
     # Mode time course for the functional connectivity
     #
 
     # Layers
-    fc_mod_mu_layer = layers.Dense(config.n_fc_modes, name="fc_mod_mu")
+    fc_mod_mu_layer = layers.Dense(config.n_corr_modes, name="fc_mod_mu")
     fc_mod_sigma_layer = layers.Dense(
-        config.n_fc_modes, activation="softplus", name="fc_mod_sigma"
+        config.n_corr_modes, activation="softplus", name="fc_mod_sigma"
     )
     fc_kl_div_layer = KLDivergenceLayer(
         config.theta_std_epsilon,
         name="fc_kl_div",
     )
 
     # Data flow
@@ -763,14 +765,14 @@
         [fc_inf_mu, fc_inf_sigma, fc_mod_mu, fc_mod_sigma],
     )
 
     #
     # Total KL loss
     #
     kl_loss_layer = KLLossLayer(config.do_kl_annealing, name="kl_loss")
-    kl_loss = kl_loss_layer([mean_kl_div, fc_kl_div])
+    kl_loss = kl_loss_layer([power_kl_div, fc_kl_div])
 
     return tf.keras.Model(
         inputs=inputs,
-        outputs=[ll_loss, kl_loss, mean_theta_norm, fc_theta_norm],
+        outputs=[ll_loss, kl_loss, power_theta_norm, fc_theta_norm],
         name="M-DyNeMo",
     )
```

### Comparing `osl-dynamics-1.3.1/osl_dynamics/models/mod_base.py` & `osl_dynamics-1.3.2/osl_dynamics/models/mod_base.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/models/obs_mod.py` & `osl_dynamics-1.3.2/osl_dynamics/models/obs_mod.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     obs_parameter : np.ndarray
         The observation model parameter.
     """
     available_layers = [
         "means",
         "covs",
         "stds",
-        "fcs",
+        "corrs",
         "group_means",
         "group_covs",
         "log_rates",
     ]
     if layer_name not in available_layers:
         raise ValueError(
             f"Layer name {layer_name} not in available layers {available_layers}."
@@ -71,15 +71,15 @@
         Whether the covariances are diagonal.
         Ignored if :code:`layer_name` is not :code:`"covs"`.
     """
     available_layers = [
         "means",
         "covs",
         "stds",
-        "fcs",
+        "corrs",
         "group_means",
         "group_covs",
         "log_rates",
     ]
     if layer_name not in available_layers:
         raise ValueError(
             f"Layer name {layer_name} not in available layers {available_layers}."
@@ -178,24 +178,25 @@
     """Set the embeddings initializer.
 
     Parameters
     ----------
     model : osl_dynamics.models.*.Model.model
         The model. * must be :code:`hive` or :code:`dive`.
     initial_embeddings : dict
-        The initial_embeddings dictionary. {name: initial_embeddings}
+        The initial_embeddings dictionary. {name: value}
     """
 
-    def _set_embeddings_initializer(layer_name, initial_embeddings):
+    # Helper function to set a single layer's initializer
+    def _set_embeddings_initializer(layer_name, value):
         embedding_layer = model.get_layer(layer_name)
         embedding_layer.embedding_layer.embeddings_initializer = WeightInitializer(
-            initial_embeddings
+            value
         )
 
-    for k, v in config.items():
+    for k, v in initial_embeddings.items():
         _set_embeddings_initializer(f"{k}_embeddings", v)
 
 
 def set_means_regularizer(model, training_dataset, layer_name="means"):
     """Set the means regularizer based on training data.
 
     A multivariate normal prior is applied to the mean vectors with
@@ -303,35 +304,35 @@
     learnable_tensor_layer.regularizer = regularizers.LogNormal(
         mu,
         sigma,
         epsilon,
     )
 
 
-def set_fcs_regularizer(model, training_dataset, epsilon):
-    """Set the FCS regularizer based on training data.
+def set_corrs_regularizer(model, training_dataset, epsilon):
+    """Set the correlations regularizer based on training data.
 
-    A marginal inverse Wishart prior is applied to the functional connectivities
+    A marginal inverse Wishart prior is applied to the correlations
     with :code:`nu=n_channels-1+0.1`.
 
     Parameters
     ----------
     model : osl_dynamics.models.*.Model.model
         The model.
     training_dataset : osl_dynamics.data.Data
         The training dataset.
     epsilon : float
-        Error added to the functional connectivities.
+        Error added to the correlations.
     """
     n_channels = dtf.get_n_channels(training_dataset)
 
     nu = n_channels - 1 + 0.1
 
-    fcs_layer = model.get_layer("fcs")
-    learnable_tensor_layer = fcs_layer.layers[0]
+    corrs_layer = model.get_layer("corrs")
+    learnable_tensor_layer = corrs_layer.layers[0]
     learnable_tensor_layer.regularizer = regularizers.MarginalInverseWishart(
         nu,
         epsilon,
         n_channels,
     )
 
 
@@ -451,52 +452,52 @@
     covs_spatial_embeddings_layer = model.get_layer("covs_spatial_embeddings")
     covs_spatial_embeddings = covs_spatial_embeddings_layer(
         cholesky_bijector.inverse(group_covs)
     )
     return covs_spatial_embeddings.numpy()
 
 
-def get_spatial_embeddings(model, map):
+def get_spatial_embeddings(model, param):
     """Wrapper for getting the spatial embeddings for the means and covariances."""
-    if map == "means":
+    if param == "means":
         return get_means_spatial_embeddings(model)
-    elif map == "covs":
+    elif param == "covs":
         return get_covs_spatial_embeddings(model)
     else:
-        raise ValueError("map must be either 'means' or 'covs'")
+        raise ValueError("param must be either 'means' or 'covs'")
 
 
-def get_concatenated_embeddings(model, map, session_labels):
+def get_concatenated_embeddings(model, param, session_labels):
     """Get the concatenated embeddings.
 
     Parameters
     ----------
     model : osl_dynamics.models.*.Model.model
         The model. * must be :code:`hive` or :code:`dive`.
-    map : str
-        The map to use. Either :code:`"means"` or :code:`"covs"`.
+    param : str
+        The param to use. Either :code:`"means"` or :code:`"covs"`.
     embeddings : np.ndarray, optional
         Input embeddings. If :code:`None`, they are retrieved from
         the model. Shape is (n_sessions, embeddings_dim).
 
     Returns
     -------
     concat_embeddings : np.ndarray
         The concatenated embeddings. Shape is (n_sessions, n_states,
         embeddings_dim + spatial_embeddings_dim).
     """
     embeddings = get_summed_embeddings(model, session_labels)
-    if map == "means":
+    if param == "means":
         spatial_embeddings = get_means_spatial_embeddings(model)
         concat_embeddings_layer = model.get_layer("means_concat_embeddings")
-    elif map == "covs":
+    elif param == "covs":
         spatial_embeddings = get_covs_spatial_embeddings(model)
         concat_embeddings_layer = model.get_layer("covs_concat_embeddings")
     else:
-        raise ValueError("map must be either 'means' or 'covs'")
+        raise ValueError("param must be either 'means' or 'covs'")
     concat_embeddings = concat_embeddings_layer([embeddings, spatial_embeddings])
     return concat_embeddings.numpy()
 
 
 def get_means_dev_mag_parameters(model):
     """Get the means deviation magnitude parameters.
 
@@ -557,84 +558,86 @@
     covs_dev_mag_inf_alpha = covs_dev_mag_inf_alpha_layer(covs_dev_mag_inf_alpha_input)
 
     covs_dev_mag_inf_beta_input = covs_dev_mag_inf_beta_input_layer(1)
     covs_dev_mag_inf_beta = covs_dev_mag_inf_beta_layer(covs_dev_mag_inf_beta_input)
     return covs_dev_mag_inf_alpha.numpy(), covs_dev_mag_inf_beta.numpy()
 
 
-def get_dev_mag_parameters(model, map):
+def get_dev_mag_parameters(model, param):
     """Wrapper for getting the deviance magnitude parameters for the means
     and covariances."""
-    if map == "means":
+    if param == "means":
         return get_means_dev_mag_parameters(model)
-    elif map == "covs":
+    elif param == "covs":
         return get_covs_dev_mag_parameters(model)
     else:
-        raise ValueError("map must be either 'means' or 'covs'")
+        raise ValueError("param must be either 'means' or 'covs'")
 
 
-def get_dev_mag(model, map):
+def get_dev_mag(model, param):
     """Getting the deviance magnitude.
 
     Parameters
     ----------
     model : osl_dynamics.models.*.Model.model
         The model. * must be :code:`hive` or :code:`dive`.
-    map : str
-        The map. Must be either :code:`'means'` or :code:`'covs'`.
+    param : str
+        The param. Must be either :code:`'means'` or :code:`'covs'`.
 
     Returns
     -------
     dev_mag : np.ndarray
         The deviance magnitude. Shape is (n_sessions, n_states, 1).
     """
-    if map == "means":
+    if param == "means":
         alpha, beta = get_means_dev_mag_parameters(model)
         dev_mag_layer = model.get_layer("means_dev_mag")
-    elif map == "covs":
+    elif param == "covs":
         alpha, beta = get_covs_dev_mag_parameters(model)
         dev_mag_layer = model.get_layer("covs_dev_mag")
     else:
-        raise ValueError("map must be either 'means' or 'covs'")
-    dev_mag = dev_mag_layer([alpha, beta])
+        raise ValueError("param must be either 'means' or 'covs'")
+
+    n_sessions = alpha.shape[0]
+    dev_mag = dev_mag_layer([alpha, beta, np.arange(n_sessions)[..., None]])
     return dev_mag.numpy()
 
 
-def get_dev_map(model, map, session_labels):
+def get_dev_map(model, param, session_labels):
     """Get the deviance map.
 
     Parameters
     ----------
     model : osl_dynamics.models.*.Model.model
         The model. * must be :code:`hive` or :code:`dive`.
-    map : str
-        The map to use. Either :code:`"means"` or :code:`"covs"`.
+    param : str
+        The param to use. Either :code:`"means"` or :code:`"covs"`.
     embeddings : np.ndarray, optional
         Input embeddings. If :code:`None`, they are retrieved from
         the model. Shape is (n_sessions, embeddings_dim).
 
     Returns
     -------
     dev_map : np.ndarray
         The deviance map.
-        If :code:`map="means"`, shape is (n_sessions, n_states, n_channels).
-        If :code:`map="covs"`, shape is (n_sessions, n_states,
+        If :code:`param="means"`, shape is (n_sessions, n_states, n_channels).
+        If :code:`param="covs"`, shape is (n_sessions, n_states,
         n_channels * (n_channels + 1) // 2).
     """
-    concat_embeddings = get_concatenated_embeddings(model, map, session_labels)
-    if map == "means":
+    concat_embeddings = get_concatenated_embeddings(model, param, session_labels)
+    if param == "means":
         dev_decoder_layer = model.get_layer("means_dev_decoder")
         dev_map_layer = model.get_layer("means_dev_map")
         norm_dev_map_layer = model.get_layer("norm_means_dev_map")
-    elif map == "covs":
+    elif param == "covs":
         dev_decoder_layer = model.get_layer("covs_dev_decoder")
         dev_map_layer = model.get_layer("covs_dev_map")
         norm_dev_map_layer = model.get_layer("norm_covs_dev_map")
     else:
-        raise ValueError("map must be either 'means' or 'covs'")
+        raise ValueError("param must be either 'means' or 'covs'")
     dev_decoder = dev_decoder_layer(concat_embeddings)
     dev_map = dev_map_layer(dev_decoder)
     norm_dev_map = norm_dev_map_layer(dev_map)
     return norm_dev_map.numpy()
 
 
 def get_session_dev(
@@ -649,20 +652,16 @@
     ----------
     model : osl_dynamics.models.*.Model.model
         The model. * must be :code:`hive` or :code:`dive`.
     learn_means : bool
         Whether the mean is learnt.
     learn_covariances : bool
         Whether the covariances are learnt.
-    embeddings : np.ndarray, optional
-        Input embeddings. Shape is (n_sessions, embeddings_dim).
-        If :code:`None`, then the embeddings are retrieved from the model.
-    n_neighbours : int, optional
-        The number of nearest neighbours if :code:`embedding` is not
-        :code:`None`.
+    session_labels : List[osl_dynamics.data.SessionLabel]
+        List of session labels.
 
     Returns
     -------
     means_dev : np.ndarray
         The means deviation. Shape is (n_sessions, n_states, n_channels).
     covs_dev : np.ndarray
         The covariances deviation.
@@ -700,14 +699,16 @@
     ----------
     model : osl_dynamics.models.*.Model.model
         The model. * must be :code:`hive` or :code:`dive`.
     learn_means : bool
         Whether the mean is learnt.
     learn_covariances : bool
         Whether the covariances are learnt.
+    session_labels : List[osl_dynamics.data.SessionLabel]
+        List of session labels.
 
     Returns
     -------
     mu : np.ndarray
         The session means. Shape is (n_sessions, n_states, n_channels).
     D : np.ndarray
         The session covariances.
@@ -723,35 +724,41 @@
     session_covs_layer = model.get_layer("session_covs")
 
     mu = session_means_layer([group_means, means_dev])
     D = session_covs_layer([group_covs, covs_dev])
     return mu.numpy(), D.numpy()
 
 
-def get_nearest_neighbours(model, embeddings, n_neighbours):
-    """Get the indices of the nearest neighours in the embedding space.
+def generate_covariances(model, session_labels):
+    """Generate covariances from the generative model.
 
     Parameters
     ----------
     model : osl_dynamics.models.*.Model.model
         The model. * must be :code:`hive` or :code:`dive`.
-    embeddings : np.ndarray
-        Input embeddings. Shape is (n_sessions, embeddings_dim).
-    n_neighbours : int
-        The number of nearest neighbours.
+    session_labels : List[osl_dynamics.data.SessionLabel]
+        List of session labels.
 
     Returns
     -------
-    nearest_neighbours : np.ndarray
-        The indices of the nearest neighbours.
-        Shape is (n_sessions, n_neighbours).
+    covs : np.ndarray
+        The covariances. Shape is (n_sessions, n_states, n_channels, n_channels)
+        or (n_states, n_channels, n_channels).
     """
-    model_embeddings = get_embeddings(model)
-    distances = np.linalg.norm(
-        np.expand_dims(embeddings, axis=1) - np.expand_dims(model_embeddings, axis=0),
-        axis=-1,
-    )
 
-    # Sort distances and get indices of nearest neighbours
-    sorted_distances = np.argsort(distances, axis=1)
-    nearest_neighbours = sorted_distances[:, :n_neighbours]
-    return nearest_neighbours
+    dev_map = get_dev_map(model, "covs", session_labels)
+    concat_embeddings = get_concatenated_embeddings(model, "covs", session_labels)
+
+    covs_dev_decoder_layer = model.get_layer("covs_dev_decoder")
+    dev_mag_mod_layer = model.get_layer("covs_dev_mag_mod_beta")
+    dev_mag_mod = 1 / dev_mag_mod_layer(covs_dev_decoder_layer(concat_embeddings))
+
+    # Generate deviations
+    dev_layer = model.get_layer("covs_dev")
+    dev = dev_layer([dev_mag_mod, dev_map])
+
+    # Generate covariances
+    group_covs = get_observation_model_parameter(model, "group_covs")
+    covs_layer = model.get_layer("session_covs")
+    covs = np.squeeze(covs_layer([group_covs, dev]).numpy())
+
+    return covs
```

### Comparing `osl-dynamics-1.3.1/osl_dynamics/models/sage.py` & `osl_dynamics-1.3.2/osl_dynamics/models/sage.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/simulation/__init__.py` & `osl_dynamics-1.3.2/osl_dynamics/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/simulation/base.py` & `osl_dynamics-1.3.2/osl_dynamics/simulation/base.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/simulation/hmm.py` & `osl_dynamics-1.3.2/osl_dynamics/simulation/hmm.py`

 * *Files 2% similar despite different names*

```diff
@@ -384,28 +384,28 @@
         # HMM objects for sampling state time courses
         # N.b. we use a different random seed to the observation model
         self.alpha_hmm = HMM(
             trans_prob=trans_prob,
             stay_prob=stay_prob,
             n_states=self.n_states,
         )
-        self.gamma_hmm = HMM(
+        self.beta_hmm = HMM(
             trans_prob=trans_prob,
             stay_prob=stay_prob,
             n_states=self.n_states,
         )
 
         # Initialise base class
         super().__init__(n_samples=n_samples)
 
         # Simulate state time courses
         alpha = self.alpha_hmm.generate_states(self.n_samples)
-        gamma = self.gamma_hmm.generate_states(self.n_samples)
+        beta = self.beta_hmm.generate_states(self.n_samples)
 
-        self.state_time_course = np.array([alpha, gamma])
+        self.state_time_course = np.array([alpha, beta])
 
         # Simulate data
         self.time_series = self.obs_mod.simulate_data(self.state_time_course)
 
     @property
     def n_modes(self):
         return self.n_states
@@ -416,16 +416,17 @@
 
     def __getattr__(self, attr):
         if attr in dir(self.obs_mod):
             return getattr(self.obs_mod, attr)
         else:
             raise AttributeError(f"No attribute called {attr}.")
 
+    def get_instantaneous_covariances(self):
         """Get the ground truth covariances at each time point.
-        
+
         Returns
         -------
         inst_covs : np.ndarray
             Instantaneous covariances.
             Shape is (n_samples, n_channels, n_channels).
         """
         return self.obs_mod.get_instantaneous_covariances(self.state_time_course)
@@ -533,14 +534,17 @@
         instead.
     n_modes : int, optional
         Number of modes.
     n_channels : int, optional
         Number of channels.
     n_covariances_act : int, optional
         Number of iterations to add activations to covariance matrices.
+    embedding_vectors : np.ndarray, optional
+        Embedding vectors for each state, shape should be
+        (n_states, embeddings_dim).
     n_sessions : int, optional
         Number of sessions.
     embeddings_dim : int
         Dimension of the embedding vectors.
     spatial_embeddings_dim : int
         Dimension of the spatial embedding vectors.
     embeddings_scale : float
@@ -565,63 +569,65 @@
         trans_prob,
         session_means,
         session_covariances,
         n_states=None,
         n_modes=None,
         n_channels=None,
         n_covariances_act=1,
+        embedding_vectors=None,
         n_sessions=None,
         embeddings_dim=None,
         spatial_embeddings_dim=None,
         embeddings_scale=None,
         n_groups=None,
         between_group_scale=None,
         tc_std=0.0,
         stay_prob=None,
         observation_error=0.0,
     ):
         if n_states is None:
             n_states = n_modes
 
-        # Construct trans_prob for each session
-        if isinstance(trans_prob, str) or trans_prob is None:
-            trans_prob = [trans_prob] * n_sessions
-
         # Observation model
         self.obs_mod = MSess_MVN(
             session_means=session_means,
             session_covariances=session_covariances,
             n_modes=n_states,
             n_channels=n_channels,
             n_covariances_act=n_covariances_act,
+            embedding_vectors=embedding_vectors,
             n_sessions=n_sessions,
             embeddings_dim=embeddings_dim,
             spatial_embeddings_dim=spatial_embeddings_dim,
             embeddings_scale=embeddings_scale,
             n_groups=n_groups,
             between_group_scale=between_group_scale,
             observation_error=observation_error,
         )
 
         self.n_states = self.obs_mod.n_modes
         self.n_channels = self.obs_mod.n_channels
         self.n_sessions = self.obs_mod.n_sessions
 
+        # Construct trans_prob for each session
+        if isinstance(trans_prob, str) or trans_prob is None:
+            trans_prob = [trans_prob] * self.n_sessions
+
         # Vary the stay probability for each session
         if stay_prob is not None:
             session_stay_prob = np.random.normal(
                 loc=stay_prob,
                 scale=tc_std,
                 size=self.n_sessions,
             )
             # truncate stay_prob at 0 and 1
             session_stay_prob = np.minimum(session_stay_prob, 1)
             session_stay_prob = np.maximum(session_stay_prob, 0)
         else:
-            session_stay_prob = [stay_prob] * n_sessions
+            session_stay_prob = [stay_prob] * self.n_sessions
 
         # Initialise base class
         super().__init__(n_samples=n_samples)
 
         # Simulate state time courses for all sessions
         self.state_time_course = []
         self.hmm = []
```

### Comparing `osl-dynamics-1.3.1/osl_dynamics/simulation/hsmm.py` & `osl_dynamics-1.3.2/osl_dynamics/simulation/hsmm.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/simulation/mar.py` & `osl_dynamics-1.3.2/osl_dynamics/simulation/mar.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/simulation/mvn.py` & `osl_dynamics-1.3.2/osl_dynamics/simulation/mvn.py`

 * *Files 3% similar despite different names*

```diff
@@ -247,17 +247,17 @@
             covariances=covariances,
             n_modes=n_modes,
             n_channels=n_channels,
             n_covariances_act=n_covariances_act,
             observation_error=observation_error,
         )
 
-        # Get the std and FC from self.covariance
+        # Get the stds and corrs from self.covariance
         self.stds = array_ops.cov2std(self.covariances)
-        self.fcs = array_ops.cov2corr(self.covariances)
+        self.corrs = array_ops.cov2corr(self.covariances)
 
     def simulate_data(self, state_time_courses):
         """Simulates data.
 
         Parameters
         ----------
         state_time_courses : np.ndarray
@@ -280,22 +280,22 @@
         # Initialise array to hold data
         data = np.zeros([n_samples, self.n_channels])
 
         # Loop through all unique combinations of states
         for time_courses in np.unique(state_time_courses, axis=0):
             # Extract the different time courses
             alpha = time_courses[:, 0]
-            gamma = time_courses[:, 1]
+            beta = time_courses[:, 1]
 
-            # Mean, standard deviation, FC for this combination of time courses
+            # Mean, standard deviation, corr for this combination of time courses
             mu = np.sum(self.means * alpha[:, np.newaxis], axis=0)
             G = np.diag(np.sum(self.stds * alpha[:, np.newaxis], axis=0))
-            F = np.sum(self.fcs * gamma[:, np.newaxis, np.newaxis], axis=0)
+            F = np.sum(self.corrs * beta[:, np.newaxis, np.newaxis], axis=0)
 
-            # Calculate covariance matrix from the standard deviation and FC
+            # Calculate covariance matrix from the standard deviation and corr
             sigma = G @ F @ G
 
             # Generate data for the time points that this combination of states
             # is active
             data[np.all(state_time_courses == time_courses, axis=(1, 2))] = (
                 np.random.multivariate_normal(
                     mu,
@@ -337,21 +337,21 @@
         # Initialise an array to hold data
         inst_covs = np.empty([n_samples, self.n_channels, self.n_channels])
 
         # Loop through all unique combinations of states
         for time_courses in np.unique(state_time_courses, axis=0):
             # Extract the different time courses
             alpha = time_courses[:, 0]
-            gamma = time_courses[:, 1]
+            beta = time_courses[:, 1]
 
-            # Mean, standard deviation, FC for this combination of time courses
+            # Mean, standard deviation, corr for this combination of time courses
             G = np.diag(np.sum(self.stds * alpha[:, np.newaxis], axis=0))
-            F = np.sum(self.fcs * gamma[:, np.newaxis, np.newaxis], axis=0)
+            F = np.sum(self.corrs * beta[:, np.newaxis, np.newaxis], axis=0)
 
-            # Calculate covariance matrix from the standard deviation and FC
+            # Calculate covariance matrix from the standard deviation and corr
             sigma = G @ F @ G
 
             inst_covs[np.all(state_time_courses == time_courses, axis=(1, 2))] = sigma
 
         return inst_covs.astype(np.float32)
 
 
@@ -371,14 +371,17 @@
         array or :code:`'random'`.
     n_modes : int, optional
         Number of modes.
     n_channels : int, optional
         Number of channels.
     n_covariances_act : int, optional
         Number of iterations to add activations to covariance matrices.
+    embedding_vectors : np.ndarray, optional
+        Embedding vectors for each session, shape should be
+        (n_sessions, embeddings_dim).
     n_sessions : int, optional
         Number of sessions.
     embeddings_dim : int, optional
         Dimension of embeddings.
     spatial_embeddings_dim : int, optional
         Dimension of spatial embeddings.
     embeddings_scale : float, optional
@@ -396,14 +399,15 @@
     def __init__(
         self,
         session_means,
         session_covariances,
         n_modes=None,
         n_channels=None,
         n_covariances_act=1,
+        embedding_vectors=None,
         n_sessions=None,
         embeddings_dim=None,
         spatial_embeddings_dim=None,
         embeddings_scale=None,
         n_groups=None,
         between_group_scale=None,
         observation_error=0.0,
@@ -412,14 +416,20 @@
         self.observation_error = observation_error
         self.embeddings_dim = embeddings_dim
         self.spatial_embeddings_dim = spatial_embeddings_dim
         self.embeddings_scale = embeddings_scale
         self.n_groups = n_groups
         self.between_group_scale = between_group_scale
 
+        if embedding_vectors is not None:
+            n_sessions = embedding_vectors.shape[0]
+            self.n_sessions = n_sessions
+            embeddings_dim = embedding_vectors.shape[1]
+            self.embeddings_dim = embeddings_dim
+
         # Both the session means and covariances were passed as numpy arrays
         if isinstance(session_means, np.ndarray) and isinstance(
             session_covariances, np.ndarray
         ):
             if session_means.ndim != 3:
                 raise ValueError(
                     "session_means must have shape (n_sessions, n_modes, n_channels)."
@@ -464,16 +474,16 @@
         elif isinstance(session_means, np.ndarray) and not isinstance(
             session_covariances, np.ndarray
         ):
             self.n_sessions = session_means.shape[0]
             self.n_modes = session_means.shape[1]
             self.n_channels = session_means.shape[2]
 
-            self.validate_embedding_parameters()
-            self.create_embeddings()
+            self.validate_embedding_parameters(embedding_vectors)
+            self.create_embeddings(embedding_vectors)
 
             self.group_means = None
             self.session_means = session_means
 
             self.group_covariances = super().create_covariances(session_covariances)
             self.session_covariances = self.create_session_covariances()
 
@@ -481,16 +491,17 @@
         elif not isinstance(session_means, np.ndarray) and isinstance(
             session_covariances, np.ndarray
         ):
             self.n_sessions = session_covariances.shape[0]
             self.n_modes = session_covariances.shape[1]
             self.n_channels = session_covariances.shape[2]
 
-            self.validate_embedding_parameters()
-            self.create_embeddings()
+            if not session_means == "zero":
+                self.validate_embedding_parameters(embedding_vectors)
+                self.create_embeddings(embedding_vectors)
 
             self.group_means = super().create_means(session_means)
             self.session_means = self.create_session_means(session_means)
 
             self.group_covariances = None
             self.session_covariances = session_covariances
 
@@ -504,68 +515,72 @@
                     "n_sessions, n_modes, n_channels must be passed."
                 )
 
             self.n_sessions = n_sessions
             self.n_modes = n_modes
             self.n_channels = n_channels
 
-            self.validate_embedding_parameters()
-            self.create_embeddings()
+            self.validate_embedding_parameters(embedding_vectors)
+            self.create_embeddings(embedding_vectors)
 
             self.group_means = super().create_means(session_means)
             self.session_means = self.create_session_means(session_means)
 
             self.group_covariances = super().create_covariances(session_covariances)
             self.session_covariances = self.create_session_covariances()
 
-    def validate_embedding_parameters(self):
-        if self.embeddings_dim is None:
-            raise ValueError(
-                "Session means or covariances not passed, please pass "
-                "'embeddings_dim'."
-            )
-        if self.spatial_embeddings_dim is None:
-            raise ValueError(
-                "Session means or covariances not passed, please pass "
-                "'spatial_embeddings_dim'."
-            )
-        if self.embeddings_scale is None:
-            raise ValueError(
-                "Session means or covariances not passed, please pass "
-                "'embeddings_scale'."
-            )
-        if self.n_groups is None:
-            raise ValueError(
-                "Session means or covariances not passed, please pass 'n_groups'."
-            )
-        if self.between_group_scale is None:
-            raise ValueError(
-                "Session means or covariances not passed, please pass "
-                "'between_group_scale'."
-            )
-
-    def create_embeddings(self):
-        # Assign groups to sessions
-        assigned_groups = np.random.choice(self.n_groups, self.n_sessions)
-        self.group_centroids = np.random.normal(
-            scale=self.between_group_scale,
-            size=[self.n_groups, self.embeddings_dim],
-        )
+    def validate_embedding_parameters(self, embedding_vectors):
+        if embedding_vectors is None:
+            if self.embeddings_dim is None:
+                raise ValueError(
+                    "Session means or covariances not passed, please pass "
+                    "'embeddings_dim'."
+                )
+            if self.spatial_embeddings_dim is None:
+                raise ValueError(
+                    "Session means or covariances not passed, please pass "
+                    "'spatial_embeddings_dim'."
+                )
+            if self.embeddings_scale is None:
+                raise ValueError(
+                    "Session means or covariances not passed, please pass "
+                    "'embeddings_scale'."
+                )
+            if self.n_groups is None:
+                raise ValueError(
+                    "Session means or covariances not passed, please pass 'n_groups'."
+                )
+            if self.between_group_scale is None:
+                raise ValueError(
+                    "Session means or covariances not passed, please pass "
+                    "'between_group_scale'."
+                )
 
-        embeddings = np.zeros([self.n_sessions, self.embeddings_dim])
-        for i in range(self.n_groups):
-            group_mask = assigned_groups == i
-            embeddings[group_mask] = np.random.multivariate_normal(
-                mean=self.group_centroids[i],
-                cov=self.embeddings_scale * np.eye(self.embeddings_dim),
-                size=[np.sum(group_mask)],
+    def create_embeddings(self, embedding_vectors):
+        if embedding_vectors is None:
+            # Assign groups to sessions
+            assigned_groups = np.random.choice(self.n_groups, self.n_sessions)
+            self.group_centroids = np.random.normal(
+                scale=self.between_group_scale,
+                size=[self.n_groups, self.embeddings_dim],
             )
 
-        self.assigned_groups = assigned_groups
-        self.embeddings = embeddings
+            embeddings = np.zeros([self.n_sessions, self.embeddings_dim])
+            for i in range(self.n_groups):
+                group_mask = assigned_groups == i
+                embeddings[group_mask] = np.random.multivariate_normal(
+                    mean=self.group_centroids[i],
+                    cov=self.embeddings_scale * np.eye(self.embeddings_dim),
+                    size=[np.sum(group_mask)],
+                )
+
+            self.assigned_groups = assigned_groups
+            self.embeddings = embeddings
+        else:
+            self.embeddings = embedding_vectors
 
     def create_linear_transform(self, input_dim, output_dim, scale=0.1):
         linear_transform = np.random.normal(
             scale=scale,
             size=(output_dim, input_dim),
         )
         return linear_transform / np.sqrt(
```

### Comparing `osl-dynamics-1.3.1/osl_dynamics/simulation/poi.py` & `osl_dynamics-1.3.2/osl_dynamics/simulation/poi.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/simulation/sm.py` & `osl_dynamics-1.3.2/osl_dynamics/simulation/sm.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/utils/misc.py` & `osl_dynamics-1.3.2/osl_dynamics/utils/misc.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/utils/model.py` & `osl_dynamics-1.3.2/osl_dynamics/utils/model.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/utils/parcellation.py` & `osl_dynamics-1.3.2/osl_dynamics/utils/parcellation.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics/utils/plotting.py` & `osl_dynamics-1.3.2/osl_dynamics/utils/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 from osl_dynamics.utils.misc import override_dict_defaults
 from osl_dynamics.utils.topoplots import Topology
 from osl_dynamics.utils.parcellation import Parcellation
 
 
 _logger = logging.getLogger("osl-dynamics")
 
+# Suppress matplotlib warnings
+logging.getLogger("matplotlib.category").setLevel(logging.ERROR)
+
 
 def set_style(params):
     """Sets matplotlib's style.
 
     Wrapper for `plt.rcParams.update
     <https://matplotlib.org/stable/tutorials/introductory/customizing.html>`_.
     List of parameters can be found `here
@@ -912,15 +915,15 @@
     create_fig = ax is None
     if create_fig:
         fig, ax = create_figure(**fig_kwargs)
 
     # Plot violins
     x = np.concatenate([[x_] * len(y) for x_, y in zip(x, data)])
     y = data.flatten()
-    ax = sns.violinplot(x=x, y=y, ax=ax, **sns_kwargs)
+    ax = sns.violinplot(x=x, y=y, hue=x, ax=ax, legend=False, **sns_kwargs)
 
     # Set title and axis labels
     ax.set_title(title)
     ax.set_xlabel(x_label)
     ax.set_ylabel(y_label)
 
     # Save the figure if a filename has been pass
@@ -1255,19 +1258,17 @@
         Should we show the elements on a log scale?
     filename: str, optional
         Output filename.
 
     Returns
     -------
     fig : plt.figure
-        Matplotlib figure object. Only returned if :code:`ax=None` and
-        :code:`filename=None`.
+        Matplotlib figure object. Only returned if :code:`filename=None`.
     ax : plt.axes
-        Matplotlib axis object(s). Only returned if :code:`ax=None` and
-        :code:`filename=None`.
+        Matplotlib axis object(s). Only returned if :code:`filename=None`.
     """
     matrix = np.array(matrix)
     if matrix.ndim == 2:
         matrix = matrix[None, :]
     if matrix.ndim != 3:
         raise ValueError("Must be a 3D array.")
     short, long, empty = rough_square_axes(len(matrix))
@@ -2010,14 +2011,98 @@
     # Save
     if filename is not None:
         save(fig, filename)
     else:
         return fig, ax
 
 
+def plot_hmm_summary_stats(
+    fo,
+    lt,
+    intv,
+    sr,
+    filename,
+    cmap="tab10",
+    fig_kwargs=None,
+    sns_kwargs=None,
+):
+    """Plot summary statistics (FO, LT, INTV, SR).
+
+    Parameters
+    ----------
+    fo : np.ndarray
+        Fractional occupancies. Shape must be (n_subjects, n_states).
+    lt : np.ndarray
+        Mean lifetimes in seconds. Shape must be (n_subjects, n_states).
+    intv : np.ndarray
+        Mean intervals in seconds. Shape must be (n_subjects, n_states).
+    sr : np.ndarray
+        Switching rates in Hz. Shape must be (n_subjects, n_states).
+    filename : str
+        Output filename.
+    cmap : str, optional
+        Matplotlib colormap.
+    fig_kwargs : dict, optional
+        Arguments to pass to :code:`plt.subplots()`.
+    sns_kwargs : dict, optional
+        Arguments to pass to :code:`sns.violinplot()`.
+    """
+    if fig_kwargs is None:
+        fig_kwargs = {}
+
+    if sns_kwargs is None:
+        sns_kwargs = {}
+
+    n_states = fo.shape[1]
+    x = range(1, n_states + 1)
+
+    sns_kwargs.update(
+        {
+            "inner": "quart",
+            "cut": 0,
+            "palette": cmap,
+        }
+    )
+
+    fig, ax = create_figure(nrows=1, ncols=4, figsize=(15, 3))
+    plot_violin(
+        fo.T,
+        x=x,
+        x_label="State",
+        y_label="Fractional Occupancy",
+        ax=ax[0],
+        sns_kwargs=sns_kwargs,
+    )
+    plot_violin(
+        lt.T,
+        x=x,
+        x_label="State",
+        y_label="Mean Lifetime (s)",
+        ax=ax[1],
+        sns_kwargs=sns_kwargs,
+    )
+    plot_violin(
+        intv.T,
+        x=x,
+        x_label="State",
+        y_label="Mean Interval (s)",
+        ax=ax[2],
+        sns_kwargs=sns_kwargs,
+    )
+    plot_violin(
+        sr.T,
+        x=x,
+        x_label="State",
+        y_label="Switching rate (Hz)",
+        ax=ax[3],
+        sns_kwargs=sns_kwargs,
+    )
+    save(fig, filename=filename, tight_layout=True)
+
+
 def plot_summary_stats_group_diff(
     name,
     summary_stats,
     pvalues,
     assignments,
     fig_kwargs=None,
     ax=None,
```

### Comparing `osl-dynamics-1.3.1/osl_dynamics/utils/topoplots.py` & `osl_dynamics-1.3.2/osl_dynamics/utils/topoplots.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.3.1/osl_dynamics.egg-info/PKG-INFO` & `osl_dynamics-1.3.2/osl_dynamics.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: osl-dynamics
-Version: 1.3.1
+Version: 1.3.2
 Summary: Models for infering dynamics in neuroimaging data
 Home-page: https://github.com/OHBA-analysis/osl-dynamics
 License: MIT
 Project-URL: Documentation, https://osl-dynamics.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 Requires-Dist: glmtools~=0.2.1
 Requires-Dist: mat73~=0.62
 Requires-Dist: matplotlib~=3.7.1
 Requires-Dist: mne~=1.3.1
 Requires-Dist: nibabel~=5.1.0
 Requires-Dist: nilearn~=0.10.2
 Requires-Dist: numba==0.58
 Requires-Dist: numpy~=1.23.5
+Requires-Dist: osfclient~=0.0.5
 Requires-Dist: pandas~=1.5.3
 Requires-Dist: pyyaml~=6.0.1
 Requires-Dist: pqdm~=0.2.0
 Requires-Dist: scipy~=1.10.1
 Requires-Dist: scikit-learn~=1.3.1
 Requires-Dist: seaborn~=0.13.0
 Requires-Dist: tabulate~=0.9.0
@@ -40,38 +41,36 @@
 ============
 
 Conda
 -----
 
 We recommend installing osl-dynamics within a virtual environment. You can do this with `Anaconda <https://docs.anaconda.com/free/anaconda/install/index.html>`_ (or `miniconda <https://docs.conda.io/projects/miniconda/en/latest/miniconda-install.html>`_).
 
+Below we describe how to install osl-dynamics from source. We recommend using the conda environment files in ``/envs``.
+
 Linux
 -----
 
-Here, we describe how to install osl-dynamics from source. We recommend using the conda environment files in ``/envs``. For a generic linux machine, osl-dynamics can be installed in editable mode with:
-
 .. code-block:: shell
 
     git clone https://github.com/OHBA-analysis/osl-dynamics.git
     cd osl-dynamics
     conda env create -f envs/linux.yml
     conda activate osld
     pip install -e .
 
-Note, if you have a Mac you may want to use the ``envs/mac.yml`` environment file instead.
+Mac
+---
+
+For a Mac, the installation of TensorFlow is slightly different to a Linux computer. We recommend using the lines above replacing the Linux environment file ``envs/linux.yml`` with the Mac environment file ``envs/mac.yml``.
 
 Windows
 -------
 
-If you are using a Windows computer, we recommend first installing linux (Ubuntu) as a Windows Subsystem by following the instructions `here <https://ubuntu.com/wsl>`_. Then following the instructions above in the Ubuntu terminal.
-
-Oxford specific computers
--------------------------
-
-If you're installing on the Oxford BMRC server, use ``envs/bmrc.yml``. If you're installing on the OHBA workstation, use ``envs/hbaws.yml``. Note, the ``hbaws.yml`` environment will automatically install spyder and jupyter notebooks.
+If you are using a Windows computer, we recommend first installing Linux (Ubuntu) as a Windows Subsystem by following the instructions `here <https://ubuntu.com/wsl>`_. Then following the instructions above in the Ubuntu terminal.
 
 Within an osl environment
 -------------------------
 
 If you have already installed `OSL <https://github.com/OHBA-analysis/osl>`_ you can install osl-dynamics in the ``osl`` environment with:
 
 .. code-block:: shell
@@ -80,23 +79,23 @@
     cd osl-dynamics
     pip install tensorflow==2.9.1
     pip install tensorflow-probability==0.17
     pip install -e .
 
 Note, if you're using a Mac computer you need to install TensorFlow with ``pip install tensorflow-macos==2.9.1`` instead of ``tensorflow==2.9.1``.
 
-Developers
-----------
+Removing osl-dynamics
+---------------------
 
-Developers might want to clone the repo using SSH instead of HTTPS:
+Simply delete the conda environment and repository:
 
 .. code-block:: shell
 
-    git clone git@github.com:OHBA-analysis/osl-dynamics.git
-
+    conda env remove -n osld
+    rm -rf osl-dynamics
 
 Documentation
 =============
 
 The read the docs page should be automatically updated whenever there's a new commit on the ``main`` branch.
 
 The documentation is included as docstrings in the source code. Please write docstrings to any classes or functions you add following the `numpy style <https://numpydoc.readthedocs.io/en/latest/format.html>`_. The API reference documentation will only be automatically generated if the docstrings are written correctly. The documentation directory ``/doc`` also contains ``.rst`` files that provide additional info regarding installation, development, the models, etc.
@@ -115,16 +114,14 @@
     python setup.py build_sphinx
 
 The local build of the documentation webpage can be found in ``build/sphinx/html/index.html``.
 
 Releases
 ========
 
-The process of packaging a python project is described here: `https://packaging.python.org/en/latest/tutorials/packaging-projects <https://packaging.python.org/en/latest/tutorials/packaging-projects>`_.
-
 A couple packages are needed to build and upload a project to PyPI, these can be installed in your conda environment with:
 
 .. code-block:: shell
 
     pip install build twine
 
 The following steps can be used to release a new version:
```

### Comparing `osl-dynamics-1.3.1/osl_dynamics.egg-info/SOURCES.txt` & `osl_dynamics-1.3.2/osl_dynamics.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -156,14 +156,15 @@
 osl_dynamics/models/hmm_poi.py
 osl_dynamics/models/inf_mod_base.py
 osl_dynamics/models/mage.py
 osl_dynamics/models/mdynemo.py
 osl_dynamics/models/mod_base.py
 osl_dynamics/models/obs_mod.py
 osl_dynamics/models/sage.py
+osl_dynamics/models/simplified_dynemo.py
 osl_dynamics/models/state_dynemo.py
 osl_dynamics/simulation/__init__.py
 osl_dynamics/simulation/base.py
 osl_dynamics/simulation/hmm.py
 osl_dynamics/simulation/hsmm.py
 osl_dynamics/simulation/mar.py
 osl_dynamics/simulation/mvn.py
```

### Comparing `osl-dynamics-1.3.1/setup.cfg` & `osl_dynamics-1.3.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = osl-dynamics
-version = 1.3.1
+version = 1.3.2
 description = Models for infering dynamics in neuroimaging data
 license = MIT
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/OHBA-analysis/osl-dynamics
 project_urls = 
 	Documentation = https://osl-dynamics.readthedocs.io/en/latest/
@@ -15,14 +15,15 @@
 	mat73~=0.62
 	matplotlib~=3.7.1
 	mne~=1.3.1
 	nibabel~=5.1.0
 	nilearn~=0.10.2
 	numba==0.58
 	numpy~=1.23.5
+	osfclient~=0.0.5
 	pandas~=1.5.3
 	pyyaml~=6.0.1
 	pqdm~=0.2.0
 	scipy~=1.10.1
 	scikit-learn~=1.3.1
 	seaborn~=0.13.0
 	tabulate~=0.9.0
```

