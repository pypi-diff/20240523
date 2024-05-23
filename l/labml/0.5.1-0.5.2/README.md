# Comparing `tmp/labml-0.5.1.tar.gz` & `tmp/labml-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labml-0.5.1.tar", last modified: Thu Mar 21 07:36:29 2024, max compression
+gzip compressed data, was "labml-0.5.2.tar", last modified: Thu May 23 20:28:39 2024, max compression
```

## Comparing `labml-0.5.1.tar` & `labml-0.5.2.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.612863 labml-0.5.1/
--rw-r--r--   0 varuna     (501) staff       (20)       19 2020-06-05 09:45:19.000000 labml-0.5.1/MANIFEST.in
--rw-r--r--   0 varuna     (501) staff       (20)     7042 2024-03-21 07:36:29.612734 labml-0.5.1/PKG-INFO
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.588369 labml-0.5.1/labml/
--rw-r--r--   0 varuna     (501) staff       (20)       22 2024-03-21 07:28:47.000000 labml-0.5.1/labml/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.590085 labml-0.5.1/labml/analytics/
--rw-r--r--   0 varuna     (501) staff       (20)    18149 2023-12-22 06:27:55.000000 labml-0.5.1/labml/analytics/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)      662 2020-06-05 09:45:19.000000 labml-0.5.1/labml/analytics/matplotlib.py
--rw-r--r--   0 varuna     (501) staff       (20)     7487 2024-03-11 09:31:18.000000 labml-0.5.1/labml/cli.py
--rw-r--r--   0 varuna     (501) staff       (20)     6360 2023-12-22 06:27:55.000000 labml-0.5.1/labml/configs.py
--rw-r--r--   0 varuna     (501) staff       (20)     9431 2023-12-22 06:27:55.000000 labml-0.5.1/labml/experiment.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.590333 labml-0.5.1/labml/internal/
--rw-r--r--   0 varuna     (501) staff       (20)        0 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.591414 labml-0.5.1/labml/internal/analytics/
--rw-r--r--   0 varuna     (501) staff       (20)        0 2020-06-05 09:45:19.000000 labml-0.5.1/labml/internal/analytics/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.594041 labml-0.5.1/labml/internal/analytics/altair/
--rw-r--r--   0 varuna     (501) staff       (20)        0 2020-06-05 09:45:19.000000 labml-0.5.1/labml/internal/analytics/altair/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     3847 2023-09-04 03:26:19.000000 labml-0.5.1/labml/internal/analytics/altair/binned_heatmap.py
--rw-r--r--   0 varuna     (501) staff       (20)     4151 2023-09-04 03:32:40.000000 labml-0.5.1/labml/internal/analytics/altair/density.py
--rw-r--r--   0 varuna     (501) staff       (20)     5071 2023-09-04 03:26:19.000000 labml-0.5.1/labml/internal/analytics/altair/density_multi.py
--rw-r--r--   0 varuna     (501) staff       (20)     1277 2021-06-23 08:39:50.000000 labml-0.5.1/labml/internal/analytics/altair/histogram.py
--rw-r--r--   0 varuna     (501) staff       (20)     4413 2023-09-04 03:26:19.000000 labml-0.5.1/labml/internal/analytics/altair/scatter.py
--rw-r--r--   0 varuna     (501) staff       (20)      250 2020-06-05 09:45:19.000000 labml-0.5.1/labml/internal/analytics/altair/utils.py
--rw-r--r--   0 varuna     (501) staff       (20)     1098 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/analytics/analytics.py
--rw-r--r--   0 varuna     (501) staff       (20)     1533 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/analytics/cache.py
--rw-r--r--   0 varuna     (501) staff       (20)     5671 2022-06-09 09:03:36.000000 labml-0.5.1/labml/internal/analytics/indicators.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.594452 labml-0.5.1/labml/internal/analytics/matplotlib/
--rw-r--r--   0 varuna     (501) staff       (20)      667 2020-06-05 09:45:19.000000 labml-0.5.1/labml/internal/analytics/matplotlib/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     2628 2020-06-05 09:45:19.000000 labml-0.5.1/labml/internal/analytics/matplotlib/tb.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.594602 labml-0.5.1/labml/internal/analytics/models/
--rw-r--r--   0 varuna     (501) staff       (20)     6152 2022-05-30 08:05:49.000000 labml-0.5.1/labml/internal/analytics/models/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.594875 labml-0.5.1/labml/internal/analytics/viz/
--rw-r--r--   0 varuna     (501) staff       (20)     1610 2022-01-18 11:05:00.000000 labml-0.5.1/labml/internal/analytics/viz/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.595976 labml-0.5.1/labml/internal/app/
--rw-r--r--   0 varuna     (501) staff       (20)     7903 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/app/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)      378 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/app/configs.py
--rw-r--r--   0 varuna     (501) staff       (20)      122 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/app/dynamic.py
--rw-r--r--   0 varuna     (501) staff       (20)     3792 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/app/experiment.py
--rw-r--r--   0 varuna     (501) staff       (20)     3928 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/app/logs.py
--rw-r--r--   0 varuna     (501) staff       (20)      689 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/app/url.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.597038 labml-0.5.1/labml/internal/computer/
--rw-r--r--   0 varuna     (501) staff       (20)        1 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/computer/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     4160 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/computer/configs.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.597699 labml-0.5.1/labml/internal/computer/monitor/
--rw-r--r--   0 varuna     (501) staff       (20)      919 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/computer/monitor/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     6099 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/computer/monitor/process.py
--rw-r--r--   0 varuna     (501) staff       (20)     7288 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/computer/monitor/scanner.py
--rw-r--r--   0 varuna     (501) staff       (20)     2164 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/computer/monitoring_process.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.598893 labml-0.5.1/labml/internal/computer/projects/
--rw-r--r--   0 varuna     (501) staff       (20)     2152 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/computer/projects/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     2498 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/computer/projects/app.py
--rw-r--r--   0 varuna     (501) staff       (20)      763 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/computer/projects/methods.py
--rw-r--r--   0 varuna     (501) staff       (20)     1645 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/computer/projects/polling.py
--rw-r--r--   0 varuna     (501) staff       (20)     2645 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/computer/projects/run_summary.py
--rw-r--r--   0 varuna     (501) staff       (20)     2129 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/computer/projects/sync.py
--rw-r--r--   0 varuna     (501) staff       (20)     2583 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/computer/service.py
--rw-r--r--   0 varuna     (501) staff       (20)     3435 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/computer/writer.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.601699 labml-0.5.1/labml/internal/configs/
--rw-r--r--   0 varuna     (501) staff       (20)        0 2020-06-05 09:45:19.000000 labml-0.5.1/labml/internal/configs/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)    20151 2023-11-05 09:27:57.000000 labml-0.5.1/labml/internal/configs/base.py
--rw-r--r--   0 varuna     (501) staff       (20)     4910 2020-11-14 04:46:19.000000 labml-0.5.1/labml/internal/configs/config_function.py
--rw-r--r--   0 varuna     (501) staff       (20)      834 2020-09-29 11:33:48.000000 labml-0.5.1/labml/internal/configs/config_item.py
--rw-r--r--   0 varuna     (501) staff       (20)     3121 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/configs/dynamic_hyperparam.py
--rw-r--r--   0 varuna     (501) staff       (20)      223 2020-11-14 04:46:19.000000 labml-0.5.1/labml/internal/configs/eval_function.py
--rw-r--r--   0 varuna     (501) staff       (20)     3905 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/configs/processor.py
--rw-r--r--   0 varuna     (501) staff       (20)     4804 2021-03-22 12:21:18.000000 labml-0.5.1/labml/internal/configs/utils.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.602812 labml-0.5.1/labml/internal/experiment/
--rw-r--r--   0 varuna     (501) staff       (20)    12855 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/experiment/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     9760 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/experiment/experiment_run.py
--rw-r--r--   0 varuna     (501) staff       (20)      489 2020-11-07 04:56:54.000000 labml-0.5.1/labml/internal/experiment/watcher.py
--rw-r--r--   0 varuna     (501) staff       (20)     7347 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/lab.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.603188 labml-0.5.1/labml/internal/logger/
--rw-r--r--   0 varuna     (501) staff       (20)      911 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/logger/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.604167 labml-0.5.1/labml/internal/logger/destinations/
--rw-r--r--   0 varuna     (501) staff       (20)      294 2020-11-27 03:09:18.000000 labml-0.5.1/labml/internal/logger/destinations/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     1642 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/logger/destinations/console.py
--rw-r--r--   0 varuna     (501) staff       (20)      707 2020-12-22 02:49:21.000000 labml-0.5.1/labml/internal/logger/destinations/factory.py
--rw-r--r--   0 varuna     (501) staff       (20)     3230 2020-12-22 03:14:00.000000 labml-0.5.1/labml/internal/logger/destinations/ipynb.py
--rw-r--r--   0 varuna     (501) staff       (20)     2546 2020-12-22 03:15:47.000000 labml-0.5.1/labml/internal/logger/destinations/ipynb_pycharm.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.604332 labml-0.5.1/labml/internal/logger/inspect/
--rw-r--r--   0 varuna     (501) staff       (20)    11460 2022-09-15 09:44:21.000000 labml-0.5.1/labml/internal/logger/inspect/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)      147 2020-11-06 14:29:30.000000 labml-0.5.1/labml/internal/logger/types.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.604796 labml-0.5.1/labml/internal/manage/
--rw-r--r--   0 varuna     (501) staff       (20)        0 2020-11-07 07:42:56.000000 labml-0.5.1/labml/internal/manage/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     2799 2020-11-07 07:59:10.000000 labml-0.5.1/labml/internal/manage/process.py
--rw-r--r--   0 varuna     (501) staff       (20)     2739 2022-06-09 09:03:36.000000 labml-0.5.1/labml/internal/manage/runs.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.606339 labml-0.5.1/labml/internal/monitor/
--rw-r--r--   0 varuna     (501) staff       (20)     9200 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/monitor/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     2843 2022-06-03 03:04:55.000000 labml-0.5.1/labml/internal/monitor/iterator.py
--rw-r--r--   0 varuna     (501) staff       (20)     4477 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/monitor/loop.py
--rw-r--r--   0 varuna     (501) staff       (20)     3907 2022-07-05 13:44:45.000000 labml-0.5.1/labml/internal/monitor/mix.py
--rw-r--r--   0 varuna     (501) staff       (20)     8905 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/monitor/sections.py
--rw-r--r--   0 varuna     (501) staff       (20)     2108 2023-06-13 15:11:05.000000 labml-0.5.1/labml/internal/monitor/time_recorder.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.606801 labml-0.5.1/labml/internal/tracker/
--rw-r--r--   0 varuna     (501) staff       (20)     7235 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/tracker/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.607249 labml-0.5.1/labml/internal/tracker/indicators/
--rw-r--r--   0 varuna     (501) staff       (20)      938 2022-04-08 07:11:33.000000 labml-0.5.1/labml/internal/tracker/indicators/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     1317 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/tracker/indicators/factory.py
--rw-r--r--   0 varuna     (501) staff       (20)     1878 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/tracker/indicators/numeric.py
--rw-r--r--   0 varuna     (501) staff       (20)      429 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/tracker/namespace.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.608031 labml-0.5.1/labml/internal/tracker/writers/
--rw-r--r--   0 varuna     (501) staff       (20)      412 2023-08-04 09:33:36.000000 labml-0.5.1/labml/internal/tracker/writers/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     3908 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/tracker/writers/app.py
--rw-r--r--   0 varuna     (501) staff       (20)     2968 2023-08-04 09:53:23.000000 labml-0.5.1/labml/internal/tracker/writers/file.py
--rw-r--r--   0 varuna     (501) staff       (20)     2531 2023-12-22 06:27:55.000000 labml-0.5.1/labml/internal/tracker/writers/screen.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.608601 labml-0.5.1/labml/internal/util/
--rw-r--r--   0 varuna     (501) staff       (20)     1563 2021-04-30 07:55:34.000000 labml-0.5.1/labml/internal/util/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     3427 2020-11-01 09:14:27.000000 labml-0.5.1/labml/internal/util/colors.py
--rw-r--r--   0 varuna     (501) staff       (20)      990 2023-07-10 03:59:50.000000 labml-0.5.1/labml/internal/util/strings.py
--rw-r--r--   0 varuna     (501) staff       (20)     1147 2023-07-18 08:26:21.000000 labml-0.5.1/labml/internal/util/values.py
--rw-r--r--   0 varuna     (501) staff       (20)      956 2023-12-22 06:27:55.000000 labml-0.5.1/labml/lab.py
--rw-r--r--   0 varuna     (501) staff       (20)     4808 2022-03-08 03:44:09.000000 labml-0.5.1/labml/logger.py
--rw-r--r--   0 varuna     (501) staff       (20)     1357 2021-07-30 10:48:22.000000 labml-0.5.1/labml/manage.py
--rw-r--r--   0 varuna     (501) staff       (20)    12092 2023-12-22 06:27:55.000000 labml-0.5.1/labml/monit.py
--rw-r--r--   0 varuna     (501) staff       (20)     5733 2023-12-22 06:27:55.000000 labml-0.5.1/labml/tracker.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.610659 labml-0.5.1/labml/utils/
--rw-r--r--   0 varuna     (501) staff       (20)      966 2023-11-19 19:42:16.000000 labml-0.5.1/labml/utils/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     3139 2021-07-30 13:13:45.000000 labml-0.5.1/labml/utils/cache.py
--rw-r--r--   0 varuna     (501) staff       (20)     1186 2021-07-30 13:16:01.000000 labml-0.5.1/labml/utils/delayed_keyboard_interrupt.py
--rw-r--r--   0 varuna     (501) staff       (20)     1691 2021-07-30 13:17:43.000000 labml-0.5.1/labml/utils/download.py
--rw-r--r--   0 varuna     (501) staff       (20)       43 2020-06-05 09:45:19.000000 labml-0.5.1/labml/utils/errors.py
--rw-r--r--   0 varuna     (501) staff       (20)     1407 2022-08-15 03:10:28.000000 labml-0.5.1/labml/utils/fastai.py
--rw-r--r--   0 varuna     (501) staff       (20)      968 2023-12-22 06:27:55.000000 labml-0.5.1/labml/utils/git_info.py
--rw-r--r--   0 varuna     (501) staff       (20)     1319 2021-07-30 11:12:56.000000 labml-0.5.1/labml/utils/keras.py
--rw-r--r--   0 varuna     (501) staff       (20)     1621 2021-07-30 11:10:34.000000 labml-0.5.1/labml/utils/lightning.py
--rw-r--r--   0 varuna     (501) staff       (20)     1080 2022-07-18 12:49:33.000000 labml-0.5.1/labml/utils/notice.py
--rw-r--r--   0 varuna     (501) staff       (20)     3699 2021-07-30 13:22:26.000000 labml-0.5.1/labml/utils/pytorch.py
--rw-r--r--   0 varuna     (501) staff       (20)      245 2022-08-15 02:57:03.000000 labml-0.5.1/labml/utils/validators.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.589568 labml-0.5.1/labml.egg-info/
--rw-r--r--   0 varuna     (501) staff       (20)     7042 2024-03-21 07:36:29.000000 labml-0.5.1/labml.egg-info/PKG-INFO
--rw-r--r--   0 varuna     (501) staff       (20)     3871 2024-03-21 07:36:29.000000 labml-0.5.1/labml.egg-info/SOURCES.txt
--rw-r--r--   0 varuna     (501) staff       (20)        1 2024-03-21 07:36:29.000000 labml-0.5.1/labml.egg-info/dependency_links.txt
--rw-r--r--   0 varuna     (501) staff       (20)       41 2024-03-21 07:36:29.000000 labml-0.5.1/labml.egg-info/entry_points.txt
--rw-r--r--   0 varuna     (501) staff       (20)       23 2024-03-21 07:36:29.000000 labml-0.5.1/labml.egg-info/requires.txt
--rw-r--r--   0 varuna     (501) staff       (20)        6 2024-03-21 07:36:29.000000 labml-0.5.1/labml.egg-info/top_level.txt
--rw-r--r--   0 varuna     (501) staff       (20)       38 2024-03-21 07:36:29.612907 labml-0.5.1/setup.cfg
--rw-r--r--   0 varuna     (501) staff       (20)     1552 2023-12-22 06:27:55.000000 labml-0.5.1/setup.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-03-21 07:36:29.612404 labml-0.5.1/test/
--rw-r--r--   0 varuna     (501) staff       (20)      361 2023-12-22 06:27:55.000000 labml-0.5.1/test/test_app.py
--rw-r--r--   0 varuna     (501) staff       (20)      300 2021-01-02 08:08:13.000000 labml-0.5.1/test/test_experiment.py
--rw-r--r--   0 varuna     (501) staff       (20)      569 2022-01-11 08:31:20.000000 labml-0.5.1/test/test_inspect.py
--rw-r--r--   0 varuna     (501) staff       (20)     1097 2022-01-11 10:00:29.000000 labml-0.5.1/test/test_model_probe.py
--rw-r--r--   0 varuna     (501) staff       (20)      404 2022-11-23 04:26:01.000000 labml-0.5.1/test/test_monit.py
--rw-r--r--   0 varuna     (501) staff       (20)      531 2020-12-08 08:14:23.000000 labml-0.5.1/test/test_tracker.py
--rw-r--r--   0 varuna     (501) staff       (20)      383 2023-08-10 14:00:12.000000 labml-0.5.1/test/test_tracker_file_write.py
--rw-r--r--   0 varuna     (501) staff       (20)      556 2020-08-31 08:27:27.000000 labml-0.5.1/test/test_watcher.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.702924 labml-0.5.2/
+-rw-r--r--   0 varuna     (501) staff       (20)       19 2020-06-05 09:45:19.000000 labml-0.5.2/MANIFEST.in
+-rw-r--r--   0 varuna     (501) staff       (20)     7032 2024-05-23 20:28:39.702768 labml-0.5.2/PKG-INFO
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.680055 labml-0.5.2/labml/
+-rw-r--r--   0 varuna     (501) staff       (20)       22 2024-05-23 20:28:18.000000 labml-0.5.2/labml/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.681678 labml-0.5.2/labml/analytics/
+-rw-r--r--   0 varuna     (501) staff       (20)    18149 2023-12-22 06:27:55.000000 labml-0.5.2/labml/analytics/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)      662 2020-06-05 09:45:19.000000 labml-0.5.2/labml/analytics/matplotlib.py
+-rw-r--r--   0 varuna     (501) staff       (20)     7487 2024-03-11 09:31:18.000000 labml-0.5.2/labml/cli.py
+-rw-r--r--   0 varuna     (501) staff       (20)     6360 2023-12-22 06:27:55.000000 labml-0.5.2/labml/configs.py
+-rw-r--r--   0 varuna     (501) staff       (20)     9431 2023-12-22 06:27:55.000000 labml-0.5.2/labml/experiment.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.681918 labml-0.5.2/labml/internal/
+-rw-r--r--   0 varuna     (501) staff       (20)        0 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.682902 labml-0.5.2/labml/internal/analytics/
+-rw-r--r--   0 varuna     (501) staff       (20)        0 2020-06-05 09:45:19.000000 labml-0.5.2/labml/internal/analytics/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.685536 labml-0.5.2/labml/internal/analytics/altair/
+-rw-r--r--   0 varuna     (501) staff       (20)        0 2020-06-05 09:45:19.000000 labml-0.5.2/labml/internal/analytics/altair/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3847 2023-09-04 03:26:19.000000 labml-0.5.2/labml/internal/analytics/altair/binned_heatmap.py
+-rw-r--r--   0 varuna     (501) staff       (20)     4151 2023-09-04 03:32:40.000000 labml-0.5.2/labml/internal/analytics/altair/density.py
+-rw-r--r--   0 varuna     (501) staff       (20)     5071 2023-09-04 03:26:19.000000 labml-0.5.2/labml/internal/analytics/altair/density_multi.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1277 2021-06-23 08:39:50.000000 labml-0.5.2/labml/internal/analytics/altair/histogram.py
+-rw-r--r--   0 varuna     (501) staff       (20)     4413 2023-09-04 03:26:19.000000 labml-0.5.2/labml/internal/analytics/altair/scatter.py
+-rw-r--r--   0 varuna     (501) staff       (20)      250 2020-06-05 09:45:19.000000 labml-0.5.2/labml/internal/analytics/altair/utils.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1098 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/analytics/analytics.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1533 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/analytics/cache.py
+-rw-r--r--   0 varuna     (501) staff       (20)     5671 2022-06-09 09:03:36.000000 labml-0.5.2/labml/internal/analytics/indicators.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.685999 labml-0.5.2/labml/internal/analytics/matplotlib/
+-rw-r--r--   0 varuna     (501) staff       (20)      667 2020-06-05 09:45:19.000000 labml-0.5.2/labml/internal/analytics/matplotlib/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2628 2020-06-05 09:45:19.000000 labml-0.5.2/labml/internal/analytics/matplotlib/tb.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.686151 labml-0.5.2/labml/internal/analytics/models/
+-rw-r--r--   0 varuna     (501) staff       (20)     6152 2022-05-30 08:05:49.000000 labml-0.5.2/labml/internal/analytics/models/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.686349 labml-0.5.2/labml/internal/analytics/viz/
+-rw-r--r--   0 varuna     (501) staff       (20)     1610 2022-01-18 11:05:00.000000 labml-0.5.2/labml/internal/analytics/viz/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.687330 labml-0.5.2/labml/internal/app/
+-rw-r--r--   0 varuna     (501) staff       (20)     7903 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/app/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)      378 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/app/configs.py
+-rw-r--r--   0 varuna     (501) staff       (20)      122 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/app/dynamic.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3792 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/app/experiment.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3928 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/app/logs.py
+-rw-r--r--   0 varuna     (501) staff       (20)      689 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/app/url.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.688190 labml-0.5.2/labml/internal/computer/
+-rw-r--r--   0 varuna     (501) staff       (20)        1 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/computer/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     4160 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/computer/configs.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.688675 labml-0.5.2/labml/internal/computer/monitor/
+-rw-r--r--   0 varuna     (501) staff       (20)      919 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/computer/monitor/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     6099 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/computer/monitor/process.py
+-rw-r--r--   0 varuna     (501) staff       (20)     7288 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/computer/monitor/scanner.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2164 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/computer/monitoring_process.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.689575 labml-0.5.2/labml/internal/computer/projects/
+-rw-r--r--   0 varuna     (501) staff       (20)     2152 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/computer/projects/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2498 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/computer/projects/app.py
+-rw-r--r--   0 varuna     (501) staff       (20)      763 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/computer/projects/methods.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1645 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/computer/projects/polling.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2645 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/computer/projects/run_summary.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2129 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/computer/projects/sync.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2583 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/computer/service.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3435 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/computer/writer.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.691726 labml-0.5.2/labml/internal/configs/
+-rw-r--r--   0 varuna     (501) staff       (20)        0 2020-06-05 09:45:19.000000 labml-0.5.2/labml/internal/configs/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)    20151 2023-11-05 09:27:57.000000 labml-0.5.2/labml/internal/configs/base.py
+-rw-r--r--   0 varuna     (501) staff       (20)     4910 2020-11-14 04:46:19.000000 labml-0.5.2/labml/internal/configs/config_function.py
+-rw-r--r--   0 varuna     (501) staff       (20)      834 2020-09-29 11:33:48.000000 labml-0.5.2/labml/internal/configs/config_item.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3121 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/configs/dynamic_hyperparam.py
+-rw-r--r--   0 varuna     (501) staff       (20)      223 2020-11-14 04:46:19.000000 labml-0.5.2/labml/internal/configs/eval_function.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3905 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/configs/processor.py
+-rw-r--r--   0 varuna     (501) staff       (20)     4804 2021-03-22 12:21:18.000000 labml-0.5.2/labml/internal/configs/utils.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.692874 labml-0.5.2/labml/internal/experiment/
+-rw-r--r--   0 varuna     (501) staff       (20)    12855 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/experiment/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     9760 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/experiment/experiment_run.py
+-rw-r--r--   0 varuna     (501) staff       (20)      489 2020-11-07 04:56:54.000000 labml-0.5.2/labml/internal/experiment/watcher.py
+-rw-r--r--   0 varuna     (501) staff       (20)     7347 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/lab.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.693215 labml-0.5.2/labml/internal/logger/
+-rw-r--r--   0 varuna     (501) staff       (20)      911 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/logger/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.694597 labml-0.5.2/labml/internal/logger/destinations/
+-rw-r--r--   0 varuna     (501) staff       (20)      294 2020-11-27 03:09:18.000000 labml-0.5.2/labml/internal/logger/destinations/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1642 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/logger/destinations/console.py
+-rw-r--r--   0 varuna     (501) staff       (20)      707 2020-12-22 02:49:21.000000 labml-0.5.2/labml/internal/logger/destinations/factory.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3485 2024-05-23 20:28:18.000000 labml-0.5.2/labml/internal/logger/destinations/ipynb.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2546 2020-12-22 03:15:47.000000 labml-0.5.2/labml/internal/logger/destinations/ipynb_pycharm.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.694824 labml-0.5.2/labml/internal/logger/inspect/
+-rw-r--r--   0 varuna     (501) staff       (20)    11460 2022-09-15 09:44:21.000000 labml-0.5.2/labml/internal/logger/inspect/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)      147 2020-11-06 14:29:30.000000 labml-0.5.2/labml/internal/logger/types.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.695412 labml-0.5.2/labml/internal/manage/
+-rw-r--r--   0 varuna     (501) staff       (20)        0 2020-11-07 07:42:56.000000 labml-0.5.2/labml/internal/manage/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2799 2020-11-07 07:59:10.000000 labml-0.5.2/labml/internal/manage/process.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2739 2022-06-09 09:03:36.000000 labml-0.5.2/labml/internal/manage/runs.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.696763 labml-0.5.2/labml/internal/monitor/
+-rw-r--r--   0 varuna     (501) staff       (20)     9200 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/monitor/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2843 2022-06-03 03:04:55.000000 labml-0.5.2/labml/internal/monitor/iterator.py
+-rw-r--r--   0 varuna     (501) staff       (20)     4477 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/monitor/loop.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3907 2022-07-05 13:44:45.000000 labml-0.5.2/labml/internal/monitor/mix.py
+-rw-r--r--   0 varuna     (501) staff       (20)     8905 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/monitor/sections.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2108 2023-06-13 15:11:05.000000 labml-0.5.2/labml/internal/monitor/time_recorder.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.697115 labml-0.5.2/labml/internal/tracker/
+-rw-r--r--   0 varuna     (501) staff       (20)     7235 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/tracker/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.697569 labml-0.5.2/labml/internal/tracker/indicators/
+-rw-r--r--   0 varuna     (501) staff       (20)      938 2022-04-08 07:11:33.000000 labml-0.5.2/labml/internal/tracker/indicators/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1317 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/tracker/indicators/factory.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1878 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/tracker/indicators/numeric.py
+-rw-r--r--   0 varuna     (501) staff       (20)      429 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/tracker/namespace.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.698277 labml-0.5.2/labml/internal/tracker/writers/
+-rw-r--r--   0 varuna     (501) staff       (20)      412 2023-08-04 09:33:36.000000 labml-0.5.2/labml/internal/tracker/writers/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3908 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/tracker/writers/app.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2968 2023-08-04 09:53:23.000000 labml-0.5.2/labml/internal/tracker/writers/file.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2531 2023-12-22 06:27:55.000000 labml-0.5.2/labml/internal/tracker/writers/screen.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.698829 labml-0.5.2/labml/internal/util/
+-rw-r--r--   0 varuna     (501) staff       (20)     1563 2021-04-30 07:55:34.000000 labml-0.5.2/labml/internal/util/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3427 2020-11-01 09:14:27.000000 labml-0.5.2/labml/internal/util/colors.py
+-rw-r--r--   0 varuna     (501) staff       (20)      990 2023-07-10 03:59:50.000000 labml-0.5.2/labml/internal/util/strings.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1147 2023-07-18 08:26:21.000000 labml-0.5.2/labml/internal/util/values.py
+-rw-r--r--   0 varuna     (501) staff       (20)      956 2023-12-22 06:27:55.000000 labml-0.5.2/labml/lab.py
+-rw-r--r--   0 varuna     (501) staff       (20)     4808 2022-03-08 03:44:09.000000 labml-0.5.2/labml/logger.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1357 2021-07-30 10:48:22.000000 labml-0.5.2/labml/manage.py
+-rw-r--r--   0 varuna     (501) staff       (20)    12092 2023-12-22 06:27:55.000000 labml-0.5.2/labml/monit.py
+-rw-r--r--   0 varuna     (501) staff       (20)     5733 2023-12-22 06:27:55.000000 labml-0.5.2/labml/tracker.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.700797 labml-0.5.2/labml/utils/
+-rw-r--r--   0 varuna     (501) staff       (20)      966 2023-11-19 19:42:16.000000 labml-0.5.2/labml/utils/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3139 2021-07-30 13:13:45.000000 labml-0.5.2/labml/utils/cache.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1186 2021-07-30 13:16:01.000000 labml-0.5.2/labml/utils/delayed_keyboard_interrupt.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1691 2021-07-30 13:17:43.000000 labml-0.5.2/labml/utils/download.py
+-rw-r--r--   0 varuna     (501) staff       (20)       43 2020-06-05 09:45:19.000000 labml-0.5.2/labml/utils/errors.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1407 2022-08-15 03:10:28.000000 labml-0.5.2/labml/utils/fastai.py
+-rw-r--r--   0 varuna     (501) staff       (20)      968 2023-12-22 06:27:55.000000 labml-0.5.2/labml/utils/git_info.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1319 2021-07-30 11:12:56.000000 labml-0.5.2/labml/utils/keras.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1621 2021-07-30 11:10:34.000000 labml-0.5.2/labml/utils/lightning.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1080 2022-07-18 12:49:33.000000 labml-0.5.2/labml/utils/notice.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3699 2021-07-30 13:22:26.000000 labml-0.5.2/labml/utils/pytorch.py
+-rw-r--r--   0 varuna     (501) staff       (20)      245 2022-08-15 02:57:03.000000 labml-0.5.2/labml/utils/validators.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.681006 labml-0.5.2/labml.egg-info/
+-rw-r--r--   0 varuna     (501) staff       (20)     7032 2024-05-23 20:28:39.000000 labml-0.5.2/labml.egg-info/PKG-INFO
+-rw-r--r--   0 varuna     (501) staff       (20)     3871 2024-05-23 20:28:39.000000 labml-0.5.2/labml.egg-info/SOURCES.txt
+-rw-r--r--   0 varuna     (501) staff       (20)        1 2024-05-23 20:28:39.000000 labml-0.5.2/labml.egg-info/dependency_links.txt
+-rw-r--r--   0 varuna     (501) staff       (20)       41 2024-05-23 20:28:39.000000 labml-0.5.2/labml.egg-info/entry_points.txt
+-rw-r--r--   0 varuna     (501) staff       (20)       23 2024-05-23 20:28:39.000000 labml-0.5.2/labml.egg-info/requires.txt
+-rw-r--r--   0 varuna     (501) staff       (20)        6 2024-05-23 20:28:39.000000 labml-0.5.2/labml.egg-info/top_level.txt
+-rw-r--r--   0 varuna     (501) staff       (20)       38 2024-05-23 20:28:39.702968 labml-0.5.2/setup.cfg
+-rw-r--r--   0 varuna     (501) staff       (20)     1552 2023-12-22 06:27:55.000000 labml-0.5.2/setup.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2024-05-23 20:28:39.702523 labml-0.5.2/test/
+-rw-r--r--   0 varuna     (501) staff       (20)      361 2023-12-22 06:27:55.000000 labml-0.5.2/test/test_app.py
+-rw-r--r--   0 varuna     (501) staff       (20)      300 2021-01-02 08:08:13.000000 labml-0.5.2/test/test_experiment.py
+-rw-r--r--   0 varuna     (501) staff       (20)      569 2022-01-11 08:31:20.000000 labml-0.5.2/test/test_inspect.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1097 2022-01-11 10:00:29.000000 labml-0.5.2/test/test_model_probe.py
+-rw-r--r--   0 varuna     (501) staff       (20)      404 2022-11-23 04:26:01.000000 labml-0.5.2/test/test_monit.py
+-rw-r--r--   0 varuna     (501) staff       (20)      531 2020-12-08 08:14:23.000000 labml-0.5.2/test/test_tracker.py
+-rw-r--r--   0 varuna     (501) staff       (20)      383 2023-08-10 14:00:12.000000 labml-0.5.2/test/test_tracker_file_write.py
+-rw-r--r--   0 varuna     (501) staff       (20)      556 2020-08-31 08:27:27.000000 labml-0.5.2/test/test_watcher.py
```

### Comparing `labml-0.5.1/PKG-INFO` & `labml-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labml
-Version: 0.5.1
+Version: 0.5.2
 Summary: Organize Machine Learning Experiments
 Home-page: https://github.com/labmlai/labml
 Author: Varuna Jayasiri, Nipun Wijerathne
 Author-email: vpjayasiri@gmail.com, hnipun@gmail.com
 Project-URL: Documentation, https://docs.labml.ai/
 Keywords: machine learning
 Classifier: Programming Language :: Python :: 3
@@ -78,15 +78,15 @@
 ### Monitor Experiments
 
 #### Installation
 
 1. Install the package using pip.
 
 ```bash
-pip install labml labml-app
+pip install labml
 ```
 
 2. Create a file named `.labml.yaml` at the top level of your project folder, and add the following line to the file:
 
 ```yaml
 app_url: http://localhost:{port}/api/v1/default
```

### Comparing `labml-0.5.1/labml/analytics/__init__.py` & `labml-0.5.2/labml/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/analytics/matplotlib.py` & `labml-0.5.2/labml/analytics/matplotlib.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/cli.py` & `labml-0.5.2/labml/cli.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/configs.py` & `labml-0.5.2/labml/configs.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/experiment.py` & `labml-0.5.2/labml/experiment.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/analytics/altair/binned_heatmap.py` & `labml-0.5.2/labml/internal/analytics/altair/binned_heatmap.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/analytics/altair/density.py` & `labml-0.5.2/labml/internal/analytics/altair/density.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/analytics/altair/density_multi.py` & `labml-0.5.2/labml/internal/analytics/altair/density_multi.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/analytics/altair/histogram.py` & `labml-0.5.2/labml/internal/analytics/altair/histogram.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/analytics/altair/scatter.py` & `labml-0.5.2/labml/internal/analytics/altair/scatter.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/analytics/analytics.py` & `labml-0.5.2/labml/internal/analytics/analytics.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/analytics/cache.py` & `labml-0.5.2/labml/internal/analytics/cache.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/analytics/indicators.py` & `labml-0.5.2/labml/internal/analytics/indicators.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/analytics/matplotlib/__init__.py` & `labml-0.5.2/labml/internal/analytics/matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/analytics/matplotlib/tb.py` & `labml-0.5.2/labml/internal/analytics/matplotlib/tb.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/analytics/models/__init__.py` & `labml-0.5.2/labml/internal/analytics/models/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/analytics/viz/__init__.py` & `labml-0.5.2/labml/internal/analytics/viz/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/app/__init__.py` & `labml-0.5.2/labml/internal/app/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/app/experiment.py` & `labml-0.5.2/labml/internal/app/experiment.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/app/logs.py` & `labml-0.5.2/labml/internal/app/logs.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/app/url.py` & `labml-0.5.2/labml/internal/app/url.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/computer/configs.py` & `labml-0.5.2/labml/internal/computer/configs.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/computer/monitor/__init__.py` & `labml-0.5.2/labml/internal/computer/monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/computer/monitor/process.py` & `labml-0.5.2/labml/internal/computer/monitor/process.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/computer/monitor/scanner.py` & `labml-0.5.2/labml/internal/computer/monitor/scanner.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/computer/monitoring_process.py` & `labml-0.5.2/labml/internal/computer/monitoring_process.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/computer/projects/__init__.py` & `labml-0.5.2/labml/internal/computer/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/computer/projects/app.py` & `labml-0.5.2/labml/internal/computer/projects/app.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/computer/projects/methods.py` & `labml-0.5.2/labml/internal/computer/projects/methods.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/computer/projects/polling.py` & `labml-0.5.2/labml/internal/computer/projects/polling.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/computer/projects/run_summary.py` & `labml-0.5.2/labml/internal/computer/projects/run_summary.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/computer/projects/sync.py` & `labml-0.5.2/labml/internal/computer/projects/sync.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/computer/service.py` & `labml-0.5.2/labml/internal/computer/service.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/computer/writer.py` & `labml-0.5.2/labml/internal/computer/writer.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/configs/base.py` & `labml-0.5.2/labml/internal/configs/base.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/configs/config_function.py` & `labml-0.5.2/labml/internal/configs/config_function.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/configs/config_item.py` & `labml-0.5.2/labml/internal/configs/config_item.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/configs/dynamic_hyperparam.py` & `labml-0.5.2/labml/internal/configs/dynamic_hyperparam.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/configs/processor.py` & `labml-0.5.2/labml/internal/configs/processor.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/configs/utils.py` & `labml-0.5.2/labml/internal/configs/utils.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/experiment/__init__.py` & `labml-0.5.2/labml/internal/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/experiment/experiment_run.py` & `labml-0.5.2/labml/internal/experiment/experiment_run.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/lab.py` & `labml-0.5.2/labml/internal/lab.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/logger/__init__.py` & `labml-0.5.2/labml/internal/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/logger/destinations/console.py` & `labml-0.5.2/labml/internal/logger/destinations/console.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/logger/destinations/factory.py` & `labml-0.5.2/labml/internal/logger/destinations/factory.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/logger/destinations/ipynb.py` & `labml-0.5.2/labml/internal/logger/destinations/ipynb.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,22 +30,31 @@
         self.__cell_count = cells
         self.__cell_lines = []
         self.__last_handle = None
 
         return False
 
     @staticmethod
+    def _escape_html(text: str) -> str:
+        text = text.replace('&', '&amp;')
+        text = text.replace('<', '&lt;')
+        text = text.replace('>', '&gt;')
+        return text
+
+    @staticmethod
     def html_code(text: str, color: List[StyleCode] or StyleCode or None):
         """
         ### Add ansi color codes
         """
         if text == '\n':
             assert color is None
             return text
 
+        text = IpynbDestination._escape_html(text)
+
         if color is None:
             return text
         elif isinstance(color, list):
             open_tags = ''.join([c.html_open(text) for c in color])
             close_tags = ''.join([c.html_close(text) for c in reversed(color)])
         else:
             open_tags = color.html_open(text)
```

### Comparing `labml-0.5.1/labml/internal/logger/destinations/ipynb_pycharm.py` & `labml-0.5.2/labml/internal/logger/destinations/ipynb_pycharm.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/logger/inspect/__init__.py` & `labml-0.5.2/labml/internal/logger/inspect/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/manage/process.py` & `labml-0.5.2/labml/internal/manage/process.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/manage/runs.py` & `labml-0.5.2/labml/internal/manage/runs.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/monitor/__init__.py` & `labml-0.5.2/labml/internal/monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/monitor/iterator.py` & `labml-0.5.2/labml/internal/monitor/iterator.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/monitor/loop.py` & `labml-0.5.2/labml/internal/monitor/loop.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/monitor/mix.py` & `labml-0.5.2/labml/internal/monitor/mix.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/monitor/sections.py` & `labml-0.5.2/labml/internal/monitor/sections.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/monitor/time_recorder.py` & `labml-0.5.2/labml/internal/monitor/time_recorder.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/tracker/__init__.py` & `labml-0.5.2/labml/internal/tracker/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/tracker/indicators/__init__.py` & `labml-0.5.2/labml/internal/tracker/indicators/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/tracker/indicators/factory.py` & `labml-0.5.2/labml/internal/tracker/indicators/factory.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/tracker/indicators/numeric.py` & `labml-0.5.2/labml/internal/tracker/indicators/numeric.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/tracker/writers/app.py` & `labml-0.5.2/labml/internal/tracker/writers/app.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/tracker/writers/file.py` & `labml-0.5.2/labml/internal/tracker/writers/file.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/tracker/writers/screen.py` & `labml-0.5.2/labml/internal/tracker/writers/screen.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/util/__init__.py` & `labml-0.5.2/labml/internal/util/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/util/colors.py` & `labml-0.5.2/labml/internal/util/colors.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/util/strings.py` & `labml-0.5.2/labml/internal/util/strings.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/internal/util/values.py` & `labml-0.5.2/labml/internal/util/values.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/lab.py` & `labml-0.5.2/labml/lab.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/logger.py` & `labml-0.5.2/labml/logger.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/manage.py` & `labml-0.5.2/labml/manage.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/monit.py` & `labml-0.5.2/labml/monit.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/tracker.py` & `labml-0.5.2/labml/tracker.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/utils/__init__.py` & `labml-0.5.2/labml/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/utils/cache.py` & `labml-0.5.2/labml/utils/cache.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/utils/delayed_keyboard_interrupt.py` & `labml-0.5.2/labml/utils/delayed_keyboard_interrupt.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/utils/download.py` & `labml-0.5.2/labml/utils/download.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/utils/fastai.py` & `labml-0.5.2/labml/utils/fastai.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/utils/git_info.py` & `labml-0.5.2/labml/utils/git_info.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/utils/keras.py` & `labml-0.5.2/labml/utils/keras.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/utils/lightning.py` & `labml-0.5.2/labml/utils/lightning.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/utils/notice.py` & `labml-0.5.2/labml/utils/notice.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml/utils/pytorch.py` & `labml-0.5.2/labml/utils/pytorch.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/labml.egg-info/PKG-INFO` & `labml-0.5.2/labml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labml
-Version: 0.5.1
+Version: 0.5.2
 Summary: Organize Machine Learning Experiments
 Home-page: https://github.com/labmlai/labml
 Author: Varuna Jayasiri, Nipun Wijerathne
 Author-email: vpjayasiri@gmail.com, hnipun@gmail.com
 Project-URL: Documentation, https://docs.labml.ai/
 Keywords: machine learning
 Classifier: Programming Language :: Python :: 3
@@ -78,15 +78,15 @@
 ### Monitor Experiments
 
 #### Installation
 
 1. Install the package using pip.
 
 ```bash
-pip install labml labml-app
+pip install labml
 ```
 
 2. Create a file named `.labml.yaml` at the top level of your project folder, and add the following line to the file:
 
 ```yaml
 app_url: http://localhost:{port}/api/v1/default
```

### Comparing `labml-0.5.1/labml.egg-info/SOURCES.txt` & `labml-0.5.2/labml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/setup.py` & `labml-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/test/test_inspect.py` & `labml-0.5.2/test/test_inspect.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/test/test_model_probe.py` & `labml-0.5.2/test/test_model_probe.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/test/test_tracker.py` & `labml-0.5.2/test/test_tracker.py`

 * *Files identical despite different names*

### Comparing `labml-0.5.1/test/test_watcher.py` & `labml-0.5.2/test/test_watcher.py`

 * *Files identical despite different names*

