# Comparing `tmp/spai-2024.5.23.tar.gz` & `tmp/spai-2024.5.23.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spai-2024.5.23.tar", max compression
+gzip compressed data, was "spai-2024.5.23.post3.tar", max compression
```

## Comparing `spai-2024.5.23.tar` & `spai-2024.5.23.post3.tar`

### file list

```diff
@@ -1,133 +1,132 @@
--rw-r--r--   0        0        0       57 2024-04-29 10:40:31.981993 spai-2024.5.23/README.md
--rw-r--r--   0        0        0      525 2024-05-23 09:41:42.320981 spai-2024.5.23/pyproject.toml
--rw-r--r--   0        0        0       27 2024-05-23 09:41:42.324981 spai-2024.5.23/spai/__init__.py
--rw-r--r--   0        0        0        1 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/analytics/__init__.py
--rw-r--r--   0        0        0     5030 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/analytics/forest_monitoring.py
--rw-r--r--   0        0        0      110 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/analytics/utils.py
--rw-r--r--   0        0        0    13235 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/analytics/water_quality.py
--rw-r--r--   0        0        0      151 2024-05-13 10:34:36.432830 spai-2024.5.23/spai/auth/__init__.py
--rw-r--r--   0        0        0     1210 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/auth/auth.py
--rw-r--r--   0        0        0       99 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/auth/is_logged.py
--rw-r--r--   0        0        0      161 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/auth/logout.py
--rw-r--r--   0        0        0      423 2024-05-13 10:34:36.432830 spai-2024.5.23/spai/auth/retrieve_credentials.py
--rw-r--r--   0        0        0     7202 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/cli.py
--rw-r--r--   0        0        0        0 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/commands/__init__.py
--rw-r--r--   0        0        0     1531 2024-05-13 10:34:36.432830 spai-2024.5.23/spai/commands/auth.py
--rw-r--r--   0        0        0     1160 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/commands/list.py
--rw-r--r--   0        0        0       86 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/config/__init__.py
--rw-r--r--   0        0        0     3777 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/config/validate.py
--rw-r--r--   0        0        0     1324 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/config/vars.py
--rw-r--r--   0        0        0        0 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/__init__.py
--rw-r--r--   0        0        0       49 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/indices/__init__.py
--rw-r--r--   0        0        0       54 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/indices/fwi/__init__.py
--rw-r--r--   0        0        0     3234 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/indices/fwi/fwi_nasa.py
--rw-r--r--   0        0        0      608 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/__init__.py
--rw-r--r--   0        0        0     3941 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/download.py
--rw-r--r--   0        0        0     6332 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/download_stac.py
--rw-r--r--   0        0        0      647 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/explore.py
--rw-r--r--   0        0        0      725 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/sentinelhub/SHCloudMaskDownloader.py
--rw-r--r--   0        0        0      758 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/sentinelhub/SHDEM30Downloader 2.py
--rw-r--r--   0        0        0      758 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/sentinelhub/SHDEM30Downloader 3.py
--rw-r--r--   0        0        0      758 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/sentinelhub/SHDEM30Downloader.py
--rw-r--r--   0        0        0     3587 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/sentinelhub/SHDownloader.py
--rw-r--r--   0        0        0     2584 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/sentinelhub/SHExplorer.py
--rw-r--r--   0        0        0      854 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/sentinelhub/SHS1Downloader.py
--rw-r--r--   0        0        0     1264 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/sentinelhub/SHS2Downloader.py
--rw-r--r--   0        0        0      275 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
--rw-r--r--   0        0        0      276 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
--rw-r--r--   0        0        0      282 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/sentinelhub/__init__.py
--rw-r--r--   0        0        0     2222 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/stac/STACDownloader.py
--rw-r--r--   0        0        0      208 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/stac/__init__.py
--rw-r--r--   0        0        0      461 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/stac/aws/AWSDEM30Downloader.py
--rw-r--r--   0        0        0      461 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/stac/aws/AWSDEM90Downloader.py
--rw-r--r--   0        0        0      876 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/stac/aws/AWSDEMDownloader.py
--rw-r--r--   0        0        0      392 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/stac/aws/AWSDownloader.py
--rw-r--r--   0        0        0     1951 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/stac/aws/AWSS2L2ADownloader.py
--rw-r--r--   0        0        0      233 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/stac/aws/__init__.py
--rw-r--r--   0        0        0      456 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/stac/decorators.py
--rw-r--r--   0        0        0      716 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/stac/pc/PCDownloader.py
--rw-r--r--   0        0        0      802 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/stac/pc/PCS1GRDDownloader.py
--rw-r--r--   0        0        0      120 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/stac/pc/__init__.py
--rw-r--r--   0        0        0     8905 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/satellite/utils.py
--rw-r--r--   0        0        0       84 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/vector/__init__.py
--rw-r--r--   0        0        0     5533 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/data/vector/openstreetmap.py
--rw-r--r--   0        0        0       71 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/errors/__init__.py
--rw-r--r--   0        0        0      308 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/errors/auth.py
--rw-r--r--   0        0        0      156 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/errors/mails.py
--rw-r--r--   0        0        0       29 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/image/__init__.py
--rw-r--r--   0        0        0     1350 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/image/utils.py
--rw-r--r--   0        0        0       95 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/image/xyz/__init__.py
--rw-r--r--   0        0        0     2026 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/image/xyz/cache.py
--rw-r--r--   0        0        0      575 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/image/xyz/errors.py
--rw-r--r--   0        0        0     6924 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/image/xyz/get_image_tile.py
--rw-r--r--   0        0        0     1828 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/image/xyz/image_utils.py
--rw-r--r--   0        0        0       28 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/mails/__init__.py
--rw-r--r--   0        0        0     1334 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/mails/mimetypes.py
--rw-r--r--   0        0        0     2932 2024-04-29 10:40:32.077990 spai-2024.5.23/spai/mails/send.py
--rw-r--r--   0        0        0     4444 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/models/Config.py
--rw-r--r--   0        0        0      984 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/models/StorageConfig.py
--rw-r--r--   0        0        0       27 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/models/__init__.py
--rw-r--r--   0        0        0      391 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/processing/__init__.py
--rw-r--r--   0        0        0      669 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/processing/autocategorize1D.py
--rw-r--r--   0        0        0      477 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/processing/colorize_raster.py
--rw-r--r--   0        0        0      932 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/processing/convert_array_to_vector.py
--rw-r--r--   0        0        0      291 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/processing/mask_raster.py
--rw-r--r--   0        0        0      682 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/processing/normalised_difference.py
--rw-r--r--   0        0        0     1239 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/processing/px_count.py
--rw-r--r--   0        0        0      107 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/processing/rasterio_mask.py
--rw-r--r--   0        0        0      266 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/processing/read_raster.py
--rw-r--r--   0        0        0     1109 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/processing/save_table.py
--rw-r--r--   0        0        0      496 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/processing/utils.py
--rw-r--r--   0        0        0      475 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/__init__.py
--rw-r--r--   0        0        0      466 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/bck/GetLogs.py
--rw-r--r--   0        0        0     1018 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/bck/InstallReqs 2.py
--rw-r--r--   0        0        0     1018 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/bck/InstallReqs 3.py
--rw-r--r--   0        0        0      482 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/bck/RunService.py
--rw-r--r--   0        0        0      492 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/bck/ScheduleService.py
--rw-r--r--   0        0        0      510 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/bck/StopService.py
--rw-r--r--   0        0        0     1578 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/bck/main.py
--rw-r--r--   0        0        0      337 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/delete_project.py
--rw-r--r--   0        0        0     2030 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/deploy_folder.py
--rw-r--r--   0        0        0      407 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/deploy_template.py
--rw-r--r--   0        0        0     1203 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/download_template.py
--rw-r--r--   0        0        0      455 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/get_logs.py
--rw-r--r--   0        0        0      242 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/get_project_by_name.py
--rw-r--r--   0        0        0      172 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/get_projects.py
--rw-r--r--   0        0        0      344 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/get_service_by_name_type_project.py
--rw-r--r--   0        0        0     1616 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/get_services.py
--rw-r--r--   0        0        0      525 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/init_project.py
--rw-r--r--   0        0        0      726 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/install_requirements.py
--rw-r--r--   0        0        0     5472 2024-05-14 09:34:31.684960 spai-2024.5.23/spai/project/project-template/README.md
--rw-r--r--   0        0        0      867 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/project-template/apis/analytics/main.py
--rw-r--r--   0        0        0       36 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/project-template/apis/analytics/requirements.txt
--rw-r--r--   0        0        0     1800 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/project-template/apis/xyz/main.py
--rw-r--r--   0        0        0       88 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/project-template/apis/xyz/requirements.txt
--rw-r--r--   0        0        0   748531 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/project-template/notebooks/analytics/main.ipynb
--rw-r--r--   0        0        0       39 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/project-template/notebooks/analytics/requirements.txt
--rw-r--r--   0        0        0     1602 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/project-template/scripts/analytics/main.py
--rw-r--r--   0        0        0       30 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/project-template/scripts/analytics/requirements.txt
--rw-r--r--   0        0        0     1076 2024-04-29 10:40:32.081990 spai-2024.5.23/spai/project/project-template/scripts/downloader/main.py
--rw-r--r--   0        0        0       85 2024-04-29 10:40:32.085990 spai-2024.5.23/spai/project/project-template/scripts/downloader/requirements.txt
--rw-r--r--   0        0        0      618 2024-04-29 10:40:32.085990 spai-2024.5.23/spai/project/project-template/spai.config.yaml
--rw-r--r--   0        0        0     1523 2024-04-29 10:40:32.085990 spai-2024.5.23/spai/project/project-template/uis/map/main.py
--rw-r--r--   0        0        0       23 2024-04-29 10:40:32.085990 spai-2024.5.23/spai/project/project-template/uis/map/requirements.txt
--rw-r--r--   0        0        0     5209 2024-05-23 08:20:39.330088 spai-2024.5.23/spai/project/run_local.py
--rw-r--r--   0        0        0      813 2024-04-29 10:40:32.085990 spai-2024.5.23/spai/project/stop_service.py
--rw-r--r--   0        0        0       38 2024-04-29 10:40:32.085990 spai-2024.5.23/spai/reports/__init__.py
--rw-r--r--   0        0        0     1328 2024-04-29 10:40:32.085990 spai-2024.5.23/spai/reports/generate.py
--rw-r--r--   0        0        0     4998 2024-05-13 10:34:36.432830 spai-2024.5.23/spai/repos/APIRepo.py
--rw-r--r--   0        0        0      997 2024-04-29 10:40:32.085990 spai-2024.5.23/spai/repos/AuthRepo.py
--rw-r--r--   0        0        0      188 2024-04-29 10:40:32.085990 spai-2024.5.23/spai/repos/MailsRepo.py
--rw-r--r--   0        0        0      200 2024-04-29 10:40:32.085990 spai-2024.5.23/spai/repos/ReportsRepo.py
--rw-r--r--   0        0        0       60 2024-04-29 10:40:32.085990 spai-2024.5.23/spai/repos/__init__.py
--rw-r--r--   0        0        0     2426 2024-04-29 10:40:32.085990 spai-2024.5.23/spai/storage/BaseStorage.py
--rw-r--r--   0        0        0     3716 2024-04-29 10:40:32.085990 spai-2024.5.23/spai/storage/CloudStorage.py
--rw-r--r--   0        0        0     5306 2024-05-23 09:41:14.793397 spai-2024.5.23/spai/storage/LocalStorage.py
--rw-r--r--   0        0        0     8548 2024-05-14 10:13:06.562198 spai-2024.5.23/spai/storage/S3Storage.py
--rw-r--r--   0        0        0     1407 2024-04-29 10:40:32.085990 spai-2024.5.23/spai/storage/Storage.py
--rw-r--r--   0        0        0     6077 2024-04-29 10:40:32.085990 spai-2024.5.23/spai/storage/_S3Storage.py
--rw-r--r--   0        0        0      120 2024-04-29 10:40:32.085990 spai-2024.5.23/spai/storage/__init__.py
--rw-r--r--   0        0        0      409 2024-04-29 10:40:32.085990 spai-2024.5.23/spai/storage/create_s3.py
--rw-r--r--   0        0        0     1559 2024-04-29 10:40:32.085990 spai-2024.5.23/spai/storage/decorators.py
--rw-r--r--   0        0        0      583 2024-04-29 10:40:32.085990 spai-2024.5.23/spai/storage/minio.py
--rw-r--r--   0        0        0      888 1970-01-01 00:00:00.000000 spai-2024.5.23/PKG-INFO
+-rw-r--r--   0        0        0       57 2024-04-29 10:40:31.981993 spai-2024.5.23.post3/README.md
+-rw-r--r--   0        0        0      527 2024-05-23 12:12:57.739210 spai-2024.5.23.post3/pyproject.toml
+-rw-r--r--   0        0        0       29 2024-05-23 12:12:57.743210 spai-2024.5.23.post3/spai/__init__.py
+-rw-r--r--   0        0        0        1 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/analytics/__init__.py
+-rw-r--r--   0        0        0     5030 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/analytics/forest_monitoring.py
+-rw-r--r--   0        0        0      110 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/analytics/utils.py
+-rw-r--r--   0        0        0    13235 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/analytics/water_quality.py
+-rw-r--r--   0        0        0      151 2024-05-13 10:34:36.432830 spai-2024.5.23.post3/spai/auth/__init__.py
+-rw-r--r--   0        0        0     1210 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/auth/auth.py
+-rw-r--r--   0        0        0       99 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/auth/is_logged.py
+-rw-r--r--   0        0        0      161 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/auth/logout.py
+-rw-r--r--   0        0        0      423 2024-05-13 10:34:36.432830 spai-2024.5.23.post3/spai/auth/retrieve_credentials.py
+-rw-r--r--   0        0        0     7202 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/cli.py
+-rw-r--r--   0        0        0        0 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/commands/__init__.py
+-rw-r--r--   0        0        0     1531 2024-05-13 10:34:36.432830 spai-2024.5.23.post3/spai/commands/auth.py
+-rw-r--r--   0        0        0     1160 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/commands/list.py
+-rw-r--r--   0        0        0       86 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/config/__init__.py
+-rw-r--r--   0        0        0     3777 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/config/validate.py
+-rw-r--r--   0        0        0     1324 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/config/vars.py
+-rw-r--r--   0        0        0        0 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/__init__.py
+-rw-r--r--   0        0        0       49 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/indices/__init__.py
+-rw-r--r--   0        0        0       54 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/indices/fwi/__init__.py
+-rw-r--r--   0        0        0     3234 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/indices/fwi/fwi_nasa.py
+-rw-r--r--   0        0        0      608 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/__init__.py
+-rw-r--r--   0        0        0     3941 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/download.py
+-rw-r--r--   0        0        0     6332 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/download_stac.py
+-rw-r--r--   0        0        0      647 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/explore.py
+-rw-r--r--   0        0        0      725 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/sentinelhub/SHCloudMaskDownloader.py
+-rw-r--r--   0        0        0      758 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/sentinelhub/SHDEM30Downloader 2.py
+-rw-r--r--   0        0        0      758 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/sentinelhub/SHDEM30Downloader 3.py
+-rw-r--r--   0        0        0      758 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/sentinelhub/SHDEM30Downloader.py
+-rw-r--r--   0        0        0     3587 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/sentinelhub/SHDownloader.py
+-rw-r--r--   0        0        0     2584 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/sentinelhub/SHExplorer.py
+-rw-r--r--   0        0        0      854 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/sentinelhub/SHS1Downloader.py
+-rw-r--r--   0        0        0     1264 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/sentinelhub/SHS2Downloader.py
+-rw-r--r--   0        0        0      275 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
+-rw-r--r--   0        0        0      276 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
+-rw-r--r--   0        0        0      282 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/sentinelhub/__init__.py
+-rw-r--r--   0        0        0     2222 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/stac/STACDownloader.py
+-rw-r--r--   0        0        0      208 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/stac/__init__.py
+-rw-r--r--   0        0        0      461 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/stac/aws/AWSDEM30Downloader.py
+-rw-r--r--   0        0        0      461 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/stac/aws/AWSDEM90Downloader.py
+-rw-r--r--   0        0        0      876 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/stac/aws/AWSDEMDownloader.py
+-rw-r--r--   0        0        0      392 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/stac/aws/AWSDownloader.py
+-rw-r--r--   0        0        0     1951 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/stac/aws/AWSS2L2ADownloader.py
+-rw-r--r--   0        0        0      233 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/stac/aws/__init__.py
+-rw-r--r--   0        0        0      456 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/stac/decorators.py
+-rw-r--r--   0        0        0      716 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/stac/pc/PCDownloader.py
+-rw-r--r--   0        0        0      802 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/stac/pc/PCS1GRDDownloader.py
+-rw-r--r--   0        0        0      120 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/stac/pc/__init__.py
+-rw-r--r--   0        0        0     8905 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/satellite/utils.py
+-rw-r--r--   0        0        0       84 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/vector/__init__.py
+-rw-r--r--   0        0        0     5533 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/data/vector/openstreetmap.py
+-rw-r--r--   0        0        0       71 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/errors/__init__.py
+-rw-r--r--   0        0        0      308 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/errors/auth.py
+-rw-r--r--   0        0        0      156 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/errors/mails.py
+-rw-r--r--   0        0        0       29 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/image/__init__.py
+-rw-r--r--   0        0        0     1350 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/image/utils.py
+-rw-r--r--   0        0        0       95 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/image/xyz/__init__.py
+-rw-r--r--   0        0        0     2026 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/image/xyz/cache.py
+-rw-r--r--   0        0        0      575 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/image/xyz/errors.py
+-rw-r--r--   0        0        0     6924 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/image/xyz/get_image_tile.py
+-rw-r--r--   0        0        0     1828 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/image/xyz/image_utils.py
+-rw-r--r--   0        0        0       28 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/mails/__init__.py
+-rw-r--r--   0        0        0     1334 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/mails/mimetypes.py
+-rw-r--r--   0        0        0     2932 2024-04-29 10:40:32.077990 spai-2024.5.23.post3/spai/mails/send.py
+-rw-r--r--   0        0        0     4444 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/models/Config.py
+-rw-r--r--   0        0        0      984 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/models/StorageConfig.py
+-rw-r--r--   0        0        0       27 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/models/__init__.py
+-rw-r--r--   0        0        0      391 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/processing/__init__.py
+-rw-r--r--   0        0        0      669 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/processing/autocategorize1D.py
+-rw-r--r--   0        0        0      477 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/processing/colorize_raster.py
+-rw-r--r--   0        0        0      932 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/processing/convert_array_to_vector.py
+-rw-r--r--   0        0        0      291 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/processing/mask_raster.py
+-rw-r--r--   0        0        0      682 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/processing/normalised_difference.py
+-rw-r--r--   0        0        0     1239 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/processing/px_count.py
+-rw-r--r--   0        0        0      107 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/processing/rasterio_mask.py
+-rw-r--r--   0        0        0      266 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/processing/read_raster.py
+-rw-r--r--   0        0        0     1109 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/processing/save_table.py
+-rw-r--r--   0        0        0      496 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/processing/utils.py
+-rw-r--r--   0        0        0      475 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/__init__.py
+-rw-r--r--   0        0        0      466 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/bck/GetLogs.py
+-rw-r--r--   0        0        0     1018 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/bck/InstallReqs 2.py
+-rw-r--r--   0        0        0     1018 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/bck/InstallReqs 3.py
+-rw-r--r--   0        0        0      482 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/bck/RunService.py
+-rw-r--r--   0        0        0      492 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/bck/ScheduleService.py
+-rw-r--r--   0        0        0      510 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/bck/StopService.py
+-rw-r--r--   0        0        0     1578 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/bck/main.py
+-rw-r--r--   0        0        0      337 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/delete_project.py
+-rw-r--r--   0        0        0     2030 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/deploy_folder.py
+-rw-r--r--   0        0        0      407 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/deploy_template.py
+-rw-r--r--   0        0        0     1203 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/download_template.py
+-rw-r--r--   0        0        0      455 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/get_logs.py
+-rw-r--r--   0        0        0      242 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/get_project_by_name.py
+-rw-r--r--   0        0        0      172 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/get_projects.py
+-rw-r--r--   0        0        0      344 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/get_service_by_name_type_project.py
+-rw-r--r--   0        0        0     1616 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/get_services.py
+-rw-r--r--   0        0        0      525 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/init_project.py
+-rw-r--r--   0        0        0      726 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/install_requirements.py
+-rw-r--r--   0        0        0     5472 2024-05-14 09:34:31.684960 spai-2024.5.23.post3/spai/project/project-template/README.md
+-rw-r--r--   0        0        0      867 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/project-template/apis/analytics/main.py
+-rw-r--r--   0        0        0       36 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/project-template/apis/analytics/requirements.txt
+-rw-r--r--   0        0        0     1800 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/project-template/apis/xyz/main.py
+-rw-r--r--   0        0        0       88 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/project-template/apis/xyz/requirements.txt
+-rw-r--r--   0        0        0   748531 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/project-template/notebooks/analytics/main.ipynb
+-rw-r--r--   0        0        0       39 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/project-template/notebooks/analytics/requirements.txt
+-rw-r--r--   0        0        0     1602 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/project-template/scripts/analytics/main.py
+-rw-r--r--   0        0        0       30 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/project-template/scripts/analytics/requirements.txt
+-rw-r--r--   0        0        0     1076 2024-04-29 10:40:32.081990 spai-2024.5.23.post3/spai/project/project-template/scripts/downloader/main.py
+-rw-r--r--   0        0        0       85 2024-04-29 10:40:32.085990 spai-2024.5.23.post3/spai/project/project-template/scripts/downloader/requirements.txt
+-rw-r--r--   0        0        0      618 2024-04-29 10:40:32.085990 spai-2024.5.23.post3/spai/project/project-template/spai.config.yaml
+-rw-r--r--   0        0        0     1523 2024-04-29 10:40:32.085990 spai-2024.5.23.post3/spai/project/project-template/uis/map/main.py
+-rw-r--r--   0        0        0       23 2024-04-29 10:40:32.085990 spai-2024.5.23.post3/spai/project/project-template/uis/map/requirements.txt
+-rw-r--r--   0        0        0     5209 2024-05-23 08:20:39.330088 spai-2024.5.23.post3/spai/project/run_local.py
+-rw-r--r--   0        0        0      813 2024-04-29 10:40:32.085990 spai-2024.5.23.post3/spai/project/stop_service.py
+-rw-r--r--   0        0        0       38 2024-04-29 10:40:32.085990 spai-2024.5.23.post3/spai/reports/__init__.py
+-rw-r--r--   0        0        0     1328 2024-04-29 10:40:32.085990 spai-2024.5.23.post3/spai/reports/generate.py
+-rw-r--r--   0        0        0     4998 2024-05-13 10:34:36.432830 spai-2024.5.23.post3/spai/repos/APIRepo.py
+-rw-r--r--   0        0        0      997 2024-04-29 10:40:32.085990 spai-2024.5.23.post3/spai/repos/AuthRepo.py
+-rw-r--r--   0        0        0      188 2024-04-29 10:40:32.085990 spai-2024.5.23.post3/spai/repos/MailsRepo.py
+-rw-r--r--   0        0        0      200 2024-04-29 10:40:32.085990 spai-2024.5.23.post3/spai/repos/ReportsRepo.py
+-rw-r--r--   0        0        0       60 2024-04-29 10:40:32.085990 spai-2024.5.23.post3/spai/repos/__init__.py
+-rw-r--r--   0        0        0     2643 2024-05-23 12:06:49.012871 spai-2024.5.23.post3/spai/storage/BaseStorage.py
+-rw-r--r--   0        0        0     3716 2024-04-29 10:40:32.085990 spai-2024.5.23.post3/spai/storage/CloudStorage.py
+-rw-r--r--   0        0        0     5131 2024-05-23 12:06:53.000809 spai-2024.5.23.post3/spai/storage/LocalStorage.py
+-rw-r--r--   0        0        0     8770 2024-05-23 12:10:02.037903 spai-2024.5.23.post3/spai/storage/S3Storage.py
+-rw-r--r--   0        0        0     1407 2024-04-29 10:40:32.085990 spai-2024.5.23.post3/spai/storage/Storage.py
+-rw-r--r--   0        0        0      120 2024-04-29 10:40:32.085990 spai-2024.5.23.post3/spai/storage/__init__.py
+-rw-r--r--   0        0        0      409 2024-04-29 10:40:32.085990 spai-2024.5.23.post3/spai/storage/create_s3.py
+-rw-r--r--   0        0        0     1559 2024-04-29 10:40:32.085990 spai-2024.5.23.post3/spai/storage/decorators.py
+-rw-r--r--   0        0        0      583 2024-04-29 10:40:32.085990 spai-2024.5.23.post3/spai/storage/minio.py
+-rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 spai-2024.5.23.post3/PKG-INFO
```

### Comparing `spai-2024.5.23/pyproject.toml` & `spai-2024.5.23.post3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spai"
-version = "2024.05.23"
+version = "2024.05.23-3"
 description = ""
 authors = ["Juan Sensio <it@earthpulse.es>"]
 readme = "README.md"
 packages = [{include = "spai"}]
 
 [tool.poetry.scripts]
 spai = "spai.cli:app"
```

### Comparing `spai-2024.5.23/spai/analytics/forest_monitoring.py` & `spai-2024.5.23.post3/spai/analytics/forest_monitoring.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/analytics/water_quality.py` & `spai-2024.5.23.post3/spai/analytics/water_quality.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/auth/auth.py` & `spai-2024.5.23.post3/spai/auth/auth.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/cli.py` & `spai-2024.5.23.post3/spai/cli.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/commands/auth.py` & `spai-2024.5.23.post3/spai/commands/auth.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/commands/list.py` & `spai-2024.5.23.post3/spai/commands/list.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/config/validate.py` & `spai-2024.5.23.post3/spai/config/validate.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/config/vars.py` & `spai-2024.5.23.post3/spai/config/vars.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/data/indices/fwi/fwi_nasa.py` & `spai-2024.5.23.post3/spai/data/indices/fwi/fwi_nasa.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/data/satellite/__init__.py` & `spai-2024.5.23.post3/spai/data/satellite/__init__.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/data/satellite/download.py` & `spai-2024.5.23.post3/spai/data/satellite/download.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/data/satellite/download_stac.py` & `spai-2024.5.23.post3/spai/data/satellite/download_stac.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/data/satellite/explore.py` & `spai-2024.5.23.post3/spai/data/satellite/explore.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/data/satellite/sentinelhub/SHCloudMaskDownloader.py` & `spai-2024.5.23.post3/spai/data/satellite/sentinelhub/SHCloudMaskDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/data/satellite/sentinelhub/SHDEM30Downloader 2.py` & `spai-2024.5.23.post3/spai/data/satellite/sentinelhub/SHDEM30Downloader 2.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/data/satellite/sentinelhub/SHDEM30Downloader 3.py` & `spai-2024.5.23.post3/spai/data/satellite/sentinelhub/SHDEM30Downloader 3.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/data/satellite/sentinelhub/SHDEM30Downloader.py` & `spai-2024.5.23.post3/spai/data/satellite/sentinelhub/SHDEM30Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/data/satellite/sentinelhub/SHDownloader.py` & `spai-2024.5.23.post3/spai/data/satellite/sentinelhub/SHDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/data/satellite/sentinelhub/SHExplorer.py` & `spai-2024.5.23.post3/spai/data/satellite/sentinelhub/SHExplorer.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/data/satellite/sentinelhub/SHS1Downloader.py` & `spai-2024.5.23.post3/spai/data/satellite/sentinelhub/SHS1Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/data/satellite/sentinelhub/SHS2Downloader.py` & `spai-2024.5.23.post3/spai/data/satellite/sentinelhub/SHS2Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/data/satellite/stac/STACDownloader.py` & `spai-2024.5.23.post3/spai/data/satellite/stac/STACDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/data/satellite/stac/aws/AWSDEMDownloader.py` & `spai-2024.5.23.post3/spai/data/satellite/stac/aws/AWSDEMDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/data/satellite/stac/aws/AWSS2L2ADownloader.py` & `spai-2024.5.23.post3/spai/data/satellite/stac/aws/AWSS2L2ADownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/data/satellite/stac/pc/PCDownloader.py` & `spai-2024.5.23.post3/spai/data/satellite/stac/pc/PCDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/data/satellite/stac/pc/PCS1GRDDownloader.py` & `spai-2024.5.23.post3/spai/data/satellite/stac/pc/PCS1GRDDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/data/satellite/utils.py` & `spai-2024.5.23.post3/spai/data/satellite/utils.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/data/vector/openstreetmap.py` & `spai-2024.5.23.post3/spai/data/vector/openstreetmap.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/image/utils.py` & `spai-2024.5.23.post3/spai/image/utils.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/image/xyz/cache.py` & `spai-2024.5.23.post3/spai/image/xyz/cache.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/image/xyz/errors.py` & `spai-2024.5.23.post3/spai/image/xyz/errors.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/image/xyz/get_image_tile.py` & `spai-2024.5.23.post3/spai/image/xyz/get_image_tile.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/image/xyz/image_utils.py` & `spai-2024.5.23.post3/spai/image/xyz/image_utils.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/mails/mimetypes.py` & `spai-2024.5.23.post3/spai/mails/mimetypes.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/mails/send.py` & `spai-2024.5.23.post3/spai/mails/send.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/models/Config.py` & `spai-2024.5.23.post3/spai/models/Config.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/models/StorageConfig.py` & `spai-2024.5.23.post3/spai/models/StorageConfig.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/processing/autocategorize1D.py` & `spai-2024.5.23.post3/spai/processing/autocategorize1D.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/processing/convert_array_to_vector.py` & `spai-2024.5.23.post3/spai/processing/convert_array_to_vector.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/processing/normalised_difference.py` & `spai-2024.5.23.post3/spai/processing/normalised_difference.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/processing/px_count.py` & `spai-2024.5.23.post3/spai/processing/px_count.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/processing/save_table.py` & `spai-2024.5.23.post3/spai/processing/save_table.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/project/bck/InstallReqs 2.py` & `spai-2024.5.23.post3/spai/project/bck/InstallReqs 2.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/project/bck/InstallReqs 3.py` & `spai-2024.5.23.post3/spai/project/bck/InstallReqs 3.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/project/bck/main.py` & `spai-2024.5.23.post3/spai/project/bck/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/project/deploy_folder.py` & `spai-2024.5.23.post3/spai/project/deploy_folder.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/project/download_template.py` & `spai-2024.5.23.post3/spai/project/download_template.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/project/get_services.py` & `spai-2024.5.23.post3/spai/project/get_services.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/project/init_project.py` & `spai-2024.5.23.post3/spai/project/init_project.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/project/install_requirements.py` & `spai-2024.5.23.post3/spai/project/install_requirements.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/project/project-template/README.md` & `spai-2024.5.23.post3/spai/project/project-template/README.md`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/project/project-template/apis/analytics/main.py` & `spai-2024.5.23.post3/spai/project/project-template/apis/analytics/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/project/project-template/apis/xyz/main.py` & `spai-2024.5.23.post3/spai/project/project-template/apis/xyz/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/project/project-template/notebooks/analytics/main.ipynb` & `spai-2024.5.23.post3/spai/project/project-template/notebooks/analytics/main.ipynb`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/project/project-template/scripts/analytics/main.py` & `spai-2024.5.23.post3/spai/project/project-template/scripts/analytics/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/project/project-template/scripts/downloader/main.py` & `spai-2024.5.23.post3/spai/project/project-template/scripts/downloader/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/project/project-template/spai.config.yaml` & `spai-2024.5.23.post3/spai/project/project-template/spai.config.yaml`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/project/project-template/uis/map/main.py` & `spai-2024.5.23.post3/spai/project/project-template/uis/map/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/project/run_local.py` & `spai-2024.5.23.post3/spai/project/run_local.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/project/stop_service.py` & `spai-2024.5.23.post3/spai/project/stop_service.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/reports/generate.py` & `spai-2024.5.23.post3/spai/reports/generate.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/repos/APIRepo.py` & `spai-2024.5.23.post3/spai/repos/APIRepo.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/repos/AuthRepo.py` & `spai-2024.5.23.post3/spai/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/storage/BaseStorage.py` & `spai-2024.5.23.post3/spai/storage/BaseStorage.py`

 * *Files 22% similar despite different names*

```diff
@@ -66,7 +66,15 @@
         pass
 
     def delete(self):
         pass
 
     def list(self, pattern="*"):
         pass
+
+    def exists(self, name):
+        pass
+
+    def create_dir(self, path):
+        # create directory if not exists
+        if not os.path.exists(os.path.dirname(path)):
+            os.makedirs(os.path.dirname(path))
```

### Comparing `spai-2024.5.23/spai/storage/CloudStorage.py` & `spai-2024.5.23.post3/spai/storage/CloudStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/storage/LocalStorage.py` & `spai-2024.5.23.post3/spai/storage/LocalStorage.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,19 +22,14 @@
 
     def exists(self, name):
         return os.path.exists(self.get_path(name))
 
     def get_path(self, name):
         return os.path.join(self.path, name)
 
-    def create_dir(self, path):
-        # create directory if not exists
-        if not os.path.exists(os.path.dirname(path)):
-            os.makedirs(os.path.dirname(path))
-
     def create_from_path(self, data, name):
         dst_path = self.get_path(name)
         shutil.move(data, dst_path)  # porque se hace un move en vez de un copy?
         return dst_path
 
     def create_from_dict(self, data, name):
         if name.endswith(".json") or name.endswith(".geojson"):
```

### Comparing `spai-2024.5.23/spai/storage/S3Storage.py` & `spai-2024.5.23.post3/spai/storage/S3Storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import pandas as pd
 import json
 import io
 from minio import Minio
 import fnmatch
 from io import BytesIO
 import numpy as np
-from os import remove
+import shutil
+import os
 
 from .BaseStorage import BaseStorage
 from .decorators import with_rio, with_geopandas, with_rioxarray
 
 
 # Ver funciones en CloudStorage si las de aquí no acaban de funcionar...
 
@@ -45,14 +46,21 @@
 
     def get_path(self, name):
         return self.get_url(name)
 
     def get_url(self, name):
         return self.client.presigned_get_object(self.bucket, name)
 
+    def exists(self, name):
+        try:
+            self.client.stat_object(self.bucket, name)
+            return True
+        except:
+            return False
+
     def list(self, pattern="*"):
         return fnmatch.filter(
             [
                 obj.object_name
                 for obj in self.client.list_objects(self.bucket, recursive=True)
             ],
             pattern,
@@ -107,22 +115,23 @@
         return self.get_url(name)
 
     @with_rioxarray
     def create_from_xarray(self, rxr, data, name):
         # TODO don't save to disk
         content_type = "image/tiff"
         tmp_path = f"/tmp/{name}"
+        self.create_dir(tmp_path)
         data.rio.to_raster(tmp_path)
         self.client.fput_object(
             self.bucket,
             name,
             tmp_path,
             content_type=content_type,
         )
-        remove(tmp_path)
+        shutil.rmtree(os.path.dirname(tmp_path))
         return self.get_url(name)
 
     def create_from_array(self, data, name):
         array_bytes = BytesIO()
         np.save(array_bytes, data)
         array_bytes.seek(0)
         self.client.put_object(
```

### Comparing `spai-2024.5.23/spai/storage/Storage.py` & `spai-2024.5.23.post3/spai/storage/Storage.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/storage/decorators.py` & `spai-2024.5.23.post3/spai/storage/decorators.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/spai/storage/minio.py` & `spai-2024.5.23.post3/spai/storage/minio.py`

 * *Files identical despite different names*

### Comparing `spai-2024.5.23/PKG-INFO` & `spai-2024.5.23.post3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spai
-Version: 2024.5.23
+Version: 2024.5.23.post3
 Summary: 
 Author: Juan Sensio
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```
