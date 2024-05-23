# Comparing `tmp/krillscan-0.3.0.tar.gz` & `tmp/krillscan-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krillscan-0.3.0.tar", last modified: Wed May 22 13:47:35 2024, max compression
+gzip compressed data, was "krillscan-0.3.1.tar", last modified: Thu May 23 14:32:49 2024, max compression
```

## Comparing `krillscan-0.3.0.tar` & `krillscan-0.3.1.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 13:47:35.145266 krillscan-0.3.0/
--rw-rw-rw-   0        0        0    11918 2024-05-22 13:47:35.145266 krillscan-0.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-22 13:47:33.967634 krillscan-0.3.0/echolab2/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.014510 krillscan-0.3.0/echolab2/instruments/
--rw-rw-rw-   0        0        0   159358 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/EK60.py
--rw-rw-rw-   0        0        0   193943 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/EK80.py
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/__init__.py
--rw-rw-rw-   0        0        0     3283 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/echosounder.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.186418 krillscan-0.3.0/echolab2/instruments/util/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/__init__.py
--rw-rw-rw-   0        0        0     5456 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/annotation_data.py
--rw-rw-rw-   0        0        0     8274 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/bottom_data.py
--rw-rw-rw-   0        0        0     6783 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/date_conversion.py
--rw-rw-rw-   0        0        0     3698 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/ek80_datagram_example.py
--rw-rw-rw-   0        0        0     8616 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/motion_data.py
--rw-rw-rw-   0        0        0    24904 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/nmea_data.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.285883 krillscan-0.3.0/echolab2/instruments/util/pynmea2/
--rw-rw-rw-   0        0        0      410 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/__init__.py
--rw-rw-rw-   0        0        0       23 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/_version.py
--rw-rw-rw-   0        0        0     7181 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/nmea.py
--rw-rw-rw-   0        0        0     2014 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/nmea_file.py
--rw-rw-rw-   0        0        0     3415 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/nmea_utils.py
--rw-rw-rw-   0        0        0      902 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/seatalk_utils.py
--rw-rw-rw-   0        0        0     2050 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/stream.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.332761 krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/
--rw-rw-rw-   0        0        0       85 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.457760 krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/
--rw-rw-rw-   0        0        0      127 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/__init__.py
--rw-rw-rw-   0        0        0     3937 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/ash.py
--rw-rw-rw-   0        0        0     1382 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/grm.py
--rw-rw-rw-   0        0        0      634 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/rdi.py
--rw-rw-rw-   0        0        0     1196 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/srf.py
--rw-rw-rw-   0        0        0     3675 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/sxn.py
--rw-rw-rw-   0        0        0     3404 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/tnl.py
--rw-rw-rw-   0        0        0     2099 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/ubx.py
--rw-rw-rw-   0        0        0    34150 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/talker.py
--rw-rw-rw-   0        0        0     1141 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/read_idx_example.py
--rw-rw-rw-   0        0        0    26010 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/simrad_calibration.py
--rw-rw-rw-   0        0        0    78275 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/simrad_parsers.py
--rw-rw-rw-   0        0        0    21140 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/simrad_raw_file.py
--rw-rw-rw-   0        0        0    11377 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/simrad_signal_proc.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.473438 krillscan-0.3.0/echolab2/instruments/util/vincenty/
--rw-rw-rw-   0        0        0     3179 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/instruments/util/vincenty/__init__.py
--rw-rw-rw-   0        0        0    67919 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/ping_data.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.473438 krillscan-0.3.0/echolab2/plotting/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.504636 krillscan-0.3.0/echolab2/plotting/matplotlib/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/matplotlib/__init__.py
--rw-rw-rw-   0        0        0    16178 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/matplotlib/echogram.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.504636 krillscan-0.3.0/echolab2/plotting/qt/
-drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.754638 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/
--rw-rw-rw-   0        0        0    26210 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QEchogramViewer.py
--rw-rw-rw-   0        0        0    19146 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QEnhancedImage.py
--rw-rw-rw-   0        0        0    20595 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QEnhancedImage_threaded.py
--rw-rw-rw-   0        0        0    20668 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVDimensionLine.py
--rw-rw-rw-   0        0        0    15704 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVGrid.py
--rw-rw-rw-   0        0        0     6629 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVHudText.py
--rw-rw-rw-   0        0        0     7732 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVLine.py
--rw-rw-rw-   0        0        0    17957 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVMarker.py
--rw-rw-rw-   0        0        0     7030 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVMarkerText.py
--rw-rw-rw-   0        0        0    13085 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVPolygon.py
--rw-rw-rw-   0        0        0    12899 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVPolygonItem.py
--rw-rw-rw-   0        0        0    12600 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVRubberBandLine.py
--rw-rw-rw-   0        0        0    12009 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QImageViewer.py
--rw-rw-rw-   0        0        0    12665 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QImageViewer_threaded.py
--rw-rw-rw-   0        0        0    61143 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QViewerBase.py
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/__init__.py
--rw-rw-rw-   0        0        0     8890 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/imageAdjustmentsDlg.py
--rw-rw-rw-   0        0        0     7787 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/imageAdjustmentsDlg_simple.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.817138 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/ui/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/ui/__init__.py
--rw-rw-rw-   0        0        0    17722 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/ui/ui_imageAdjustmentsDlg.py
--rw-rw-rw-   0        0        0    14034 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/ui/ui_imageAdjustmentsDlg_simple.py
--rw-rw-rw-   0        0        0     1615 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/ui/ui_simple.py
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.832764 krillscan-0.3.0/echolab2/plotting/qt/ui/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/ui/__init__.py
--rw-rw-rw-   0        0        0     2379 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/plotting/qt/ui/ui_echogram_viewer.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:47:34.926514 krillscan-0.3.0/echolab2/processing/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/processing/__init__.py
--rw-rw-rw-   0        0        0    10904 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/processing/afsc_bot_detector.py
--rw-rw-rw-   0        0        0     3347 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/processing/batch_utils.py
--rw-rw-rw-   0        0        0     9669 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/processing/grid.py
--rw-rw-rw-   0        0        0    21422 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/processing/line.py
--rw-rw-rw-   0        0        0    22367 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/processing/mask.py
--rw-rw-rw-   0        0        0    75289 2023-04-21 13:42:55.000000 krillscan-0.3.0/echolab2/processing/processed_data.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:47:35.098391 krillscan-0.3.0/echopy/
--rw-rw-rw-   0        0        0      758 2023-04-21 13:50:02.000000 krillscan-0.3.0/echopy/__init__.py
--rw-rw-rw-   0        0        0     1515 2023-04-21 13:42:55.000000 krillscan-0.3.0/echopy/cmaps.py
--rw-rw-rw-   0        0        0      267 2023-04-21 13:42:55.000000 krillscan-0.3.0/echopy/correct_absorption.py
--rw-rw-rw-   0        0        0      248 2023-04-21 13:42:55.000000 krillscan-0.3.0/echopy/correct_es60triangle.py
--rw-rw-rw-   0        0        0      250 2023-04-21 13:42:55.000000 krillscan-0.3.0/echopy/correct_soundspeed.py
--rw-rw-rw-   0        0        0     3372 2023-04-21 13:50:19.000000 krillscan-0.3.0/echopy/get_background.py
--rw-rw-rw-   0        0        0     5966 2023-04-21 13:50:51.000000 krillscan-0.3.0/echopy/mask_attenuated.py
--rw-rw-rw-   0        0        0     7763 2023-04-21 13:51:06.000000 krillscan-0.3.0/echopy/mask_impulse.py
--rw-rw-rw-   0        0        0     1358 2023-04-21 13:42:55.000000 krillscan-0.3.0/echopy/mask_multifrequency.py
--rw-rw-rw-   0        0        0     2609 2023-04-21 13:42:55.000000 krillscan-0.3.0/echopy/mask_range.py
--rw-rw-rw-   0        0        0    21355 2023-04-21 13:51:18.000000 krillscan-0.3.0/echopy/mask_seabed.py
--rw-rw-rw-   0        0        0    10771 2023-04-21 13:42:55.000000 krillscan-0.3.0/echopy/mask_shoals.py
--rw-rw-rw-   0        0        0     2511 2023-04-21 13:51:29.000000 krillscan-0.3.0/echopy/mask_signal2noise.py
--rw-rw-rw-   0        0        0      873 2023-04-21 13:42:55.000000 krillscan-0.3.0/echopy/mask_stationary.py
--rw-rw-rw-   0        0        0     7131 2023-04-21 13:51:37.000000 krillscan-0.3.0/echopy/mask_transient.py
--rw-rw-rw-   0        0        0    13405 2023-04-21 13:42:55.000000 krillscan-0.3.0/echopy/read_calibration.py
--rw-rw-rw-   0        0        0    17793 2023-04-21 13:50:29.000000 krillscan-0.3.0/echopy/resample.py
--rw-rw-rw-   0        0        0     5841 2023-04-21 13:50:38.000000 krillscan-0.3.0/echopy/transform.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:47:35.145266 krillscan-0.3.0/krillscan/
--rw-rw-rw-   0        0        0      123 2023-04-27 09:16:18.000000 krillscan-0.3.0/krillscan/__init__.py
--rw-rw-rw-   0        0        0    37891 2024-04-24 08:37:15.000000 krillscan-0.3.0/krillscan/inspect.py
--rw-rw-rw-   0        0        0    67697 2024-05-13 12:02:29.000000 krillscan-0.3.0/krillscan/process.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:47:35.145266 krillscan-0.3.0/krillscan.egg-info/
--rw-rw-rw-   0        0        0    11918 2024-05-22 13:47:33.000000 krillscan-0.3.0/krillscan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3950 2024-05-22 13:47:33.000000 krillscan-0.3.0/krillscan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 13:47:33.000000 krillscan-0.3.0/krillscan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2024-05-22 13:47:33.000000 krillscan-0.3.0/krillscan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-22 13:47:33.000000 krillscan-0.3.0/krillscan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 13:47:35.145266 krillscan-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      906 2024-05-22 13:45:47.000000 krillscan-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:49.425206 krillscan-0.3.1/
+-rw-rw-rw-   0        0        0    11918 2024-05-23 14:32:49.422705 krillscan-0.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:49.125281 krillscan-0.3.1/krillscan/
+-rw-rw-rw-   0        0        0      123 2023-04-27 09:16:18.000000 krillscan-0.3.1/krillscan/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:49.152712 krillscan-0.3.1/krillscan/echolab2/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:49.165207 krillscan-0.3.1/krillscan/echolab2/instruments/
+-rw-rw-rw-   0        0        0   159358 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/EK60.py
+-rw-rw-rw-   0        0        0   193943 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/EK80.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/__init__.py
+-rw-rw-rw-   0        0        0     3283 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/echosounder.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:49.197705 krillscan-0.3.1/krillscan/echolab2/instruments/util/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/__init__.py
+-rw-rw-rw-   0        0        0     5456 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/annotation_data.py
+-rw-rw-rw-   0        0        0     8274 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/bottom_data.py
+-rw-rw-rw-   0        0        0     6783 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/date_conversion.py
+-rw-rw-rw-   0        0        0     3698 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/ek80_datagram_example.py
+-rw-rw-rw-   0        0        0     8616 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/motion_data.py
+-rw-rw-rw-   0        0        0    24904 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/nmea_data.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:49.230212 krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/
+-rw-rw-rw-   0        0        0      410 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/_version.py
+-rw-rw-rw-   0        0        0     7181 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/nmea.py
+-rw-rw-rw-   0        0        0     2014 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/nmea_file.py
+-rw-rw-rw-   0        0        0     3415 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/nmea_utils.py
+-rw-rw-rw-   0        0        0      902 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/seatalk_utils.py
+-rw-rw-rw-   0        0        0     2050 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/stream.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:49.240211 krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/types/
+-rw-rw-rw-   0        0        0       85 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/types/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:49.262704 krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/
+-rw-rw-rw-   0        0        0      127 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/__init__.py
+-rw-rw-rw-   0        0        0     3937 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/ash.py
+-rw-rw-rw-   0        0        0     1382 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/grm.py
+-rw-rw-rw-   0        0        0      634 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/rdi.py
+-rw-rw-rw-   0        0        0     1196 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/srf.py
+-rw-rw-rw-   0        0        0     3675 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/sxn.py
+-rw-rw-rw-   0        0        0     3404 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/tnl.py
+-rw-rw-rw-   0        0        0     2099 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/ubx.py
+-rw-rw-rw-   0        0        0    34150 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/types/talker.py
+-rw-rw-rw-   0        0        0     1141 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/read_idx_example.py
+-rw-rw-rw-   0        0        0    26010 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/simrad_calibration.py
+-rw-rw-rw-   0        0        0    78275 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/simrad_parsers.py
+-rw-rw-rw-   0        0        0    21140 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/simrad_raw_file.py
+-rw-rw-rw-   0        0        0    11377 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/simrad_signal_proc.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:49.265204 krillscan-0.3.1/krillscan/echolab2/instruments/util/vincenty/
+-rw-rw-rw-   0        0        0     3179 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/instruments/util/vincenty/__init__.py
+-rw-rw-rw-   0        0        0    67919 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/ping_data.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:49.265204 krillscan-0.3.1/krillscan/echolab2/plotting/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:49.267703 krillscan-0.3.1/krillscan/echolab2/plotting/matplotlib/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/matplotlib/__init__.py
+-rw-rw-rw-   0        0        0    16178 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/matplotlib/echogram.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:49.270207 krillscan-0.3.1/krillscan/echolab2/plotting/qt/
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:49.320210 krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/
+-rw-rw-rw-   0        0        0    26210 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QEchogramViewer.py
+-rw-rw-rw-   0        0        0    19146 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QEnhancedImage.py
+-rw-rw-rw-   0        0        0    20595 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QEnhancedImage_threaded.py
+-rw-rw-rw-   0        0        0    20668 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QIVDimensionLine.py
+-rw-rw-rw-   0        0        0    15704 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QIVGrid.py
+-rw-rw-rw-   0        0        0     6629 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QIVHudText.py
+-rw-rw-rw-   0        0        0     7732 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QIVLine.py
+-rw-rw-rw-   0        0        0    17957 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QIVMarker.py
+-rw-rw-rw-   0        0        0     7030 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QIVMarkerText.py
+-rw-rw-rw-   0        0        0    13085 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QIVPolygon.py
+-rw-rw-rw-   0        0        0    12899 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QIVPolygonItem.py
+-rw-rw-rw-   0        0        0    12600 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QIVRubberBandLine.py
+-rw-rw-rw-   0        0        0    12009 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QImageViewer.py
+-rw-rw-rw-   0        0        0    12665 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QImageViewer_threaded.py
+-rw-rw-rw-   0        0        0    61143 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QViewerBase.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/__init__.py
+-rw-rw-rw-   0        0        0     8890 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/imageAdjustmentsDlg.py
+-rw-rw-rw-   0        0        0     7787 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/imageAdjustmentsDlg_simple.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:49.340206 krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/ui/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/ui/__init__.py
+-rw-rw-rw-   0        0        0    17722 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/ui/ui_imageAdjustmentsDlg.py
+-rw-rw-rw-   0        0        0    14034 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/ui/ui_imageAdjustmentsDlg_simple.py
+-rw-rw-rw-   0        0        0     1615 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/ui/ui_simple.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:49.345211 krillscan-0.3.1/krillscan/echolab2/plotting/qt/ui/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/ui/__init__.py
+-rw-rw-rw-   0        0        0     2379 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/plotting/qt/ui/ui_echogram_viewer.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:49.362706 krillscan-0.3.1/krillscan/echolab2/processing/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/processing/__init__.py
+-rw-rw-rw-   0        0        0    10904 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/processing/afsc_bot_detector.py
+-rw-rw-rw-   0        0        0     3347 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/processing/batch_utils.py
+-rw-rw-rw-   0        0        0     9669 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/processing/grid.py
+-rw-rw-rw-   0        0        0    21422 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/processing/line.py
+-rw-rw-rw-   0        0        0    22367 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/processing/mask.py
+-rw-rw-rw-   0        0        0    75289 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echolab2/processing/processed_data.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:49.420209 krillscan-0.3.1/krillscan/echopy/
+-rw-rw-rw-   0        0        0      758 2023-04-21 13:50:02.000000 krillscan-0.3.1/krillscan/echopy/__init__.py
+-rw-rw-rw-   0        0        0     1515 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echopy/cmaps.py
+-rw-rw-rw-   0        0        0      267 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echopy/correct_absorption.py
+-rw-rw-rw-   0        0        0      248 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echopy/correct_es60triangle.py
+-rw-rw-rw-   0        0        0      250 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echopy/correct_soundspeed.py
+-rw-rw-rw-   0        0        0     3372 2023-04-21 13:50:19.000000 krillscan-0.3.1/krillscan/echopy/get_background.py
+-rw-rw-rw-   0        0        0     5966 2023-04-21 13:50:51.000000 krillscan-0.3.1/krillscan/echopy/mask_attenuated.py
+-rw-rw-rw-   0        0        0     7763 2023-04-21 13:51:06.000000 krillscan-0.3.1/krillscan/echopy/mask_impulse.py
+-rw-rw-rw-   0        0        0     1358 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echopy/mask_multifrequency.py
+-rw-rw-rw-   0        0        0     2609 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echopy/mask_range.py
+-rw-rw-rw-   0        0        0    21355 2023-04-21 13:51:18.000000 krillscan-0.3.1/krillscan/echopy/mask_seabed.py
+-rw-rw-rw-   0        0        0    10771 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echopy/mask_shoals.py
+-rw-rw-rw-   0        0        0     2511 2023-04-21 13:51:29.000000 krillscan-0.3.1/krillscan/echopy/mask_signal2noise.py
+-rw-rw-rw-   0        0        0      873 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echopy/mask_stationary.py
+-rw-rw-rw-   0        0        0     7131 2023-04-21 13:51:37.000000 krillscan-0.3.1/krillscan/echopy/mask_transient.py
+-rw-rw-rw-   0        0        0    13405 2023-04-21 13:42:55.000000 krillscan-0.3.1/krillscan/echopy/read_calibration.py
+-rw-rw-rw-   0        0        0    17793 2023-04-21 13:50:29.000000 krillscan-0.3.1/krillscan/echopy/resample.py
+-rw-rw-rw-   0        0        0     5841 2023-04-21 13:50:38.000000 krillscan-0.3.1/krillscan/echopy/transform.py
+-rw-rw-rw-   0        0        0    37891 2024-04-24 08:37:15.000000 krillscan-0.3.1/krillscan/inspect.py
+-rw-rw-rw-   0        0        0    67697 2024-05-13 12:02:29.000000 krillscan-0.3.1/krillscan/process.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:49.140789 krillscan-0.3.1/krillscan.egg-info/
+-rw-rw-rw-   0        0        0    11918 2024-05-23 14:32:48.000000 krillscan-0.3.1/krillscan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4840 2024-05-23 14:32:48.000000 krillscan-0.3.1/krillscan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 14:32:48.000000 krillscan-0.3.1/krillscan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2024-05-23 14:32:48.000000 krillscan-0.3.1/krillscan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 14:32:48.000000 krillscan-0.3.1/krillscan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 14:32:49.427706 krillscan-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      906 2024-05-23 14:32:32.000000 krillscan-0.3.1/setup.py
```

### Comparing `krillscan-0.3.0/PKG-INFO` & `krillscan-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krillscan
-Version: 0.3.0
+Version: 0.3.1
 Summary: A python module for automatic analysis of backscatter data from vessels of opportunity
 Home-page: 
 Author: Sebastian Menze
 Author-email: sebastian.menze@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Requires-Dist: lxml
```

### Comparing `krillscan-0.3.0/echolab2/instruments/EK60.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/EK60.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/EK80.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/EK80.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/echosounder.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/echosounder.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/annotation_data.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/annotation_data.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/bottom_data.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/bottom_data.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/date_conversion.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/date_conversion.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/ek80_datagram_example.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/ek80_datagram_example.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/motion_data.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/motion_data.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/nmea_data.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/nmea_data.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/pynmea2/nmea.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/nmea.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/pynmea2/nmea_file.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/nmea_file.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/pynmea2/nmea_utils.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/nmea_utils.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/pynmea2/seatalk_utils.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/seatalk_utils.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/pynmea2/stream.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/stream.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/ash.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/ash.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/grm.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/grm.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/rdi.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/rdi.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/srf.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/srf.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/sxn.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/sxn.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/tnl.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/tnl.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/proprietary/ubx.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/types/proprietary/ubx.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/pynmea2/types/talker.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/pynmea2/types/talker.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/read_idx_example.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/read_idx_example.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/simrad_calibration.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/simrad_calibration.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/simrad_parsers.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/simrad_parsers.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/simrad_raw_file.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/simrad_raw_file.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/simrad_signal_proc.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/simrad_signal_proc.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/instruments/util/vincenty/__init__.py` & `krillscan-0.3.1/krillscan/echolab2/instruments/util/vincenty/__init__.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/ping_data.py` & `krillscan-0.3.1/krillscan/echolab2/ping_data.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/plotting/matplotlib/echogram.py` & `krillscan-0.3.1/krillscan/echolab2/plotting/matplotlib/echogram.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QEchogramViewer.py` & `krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QEchogramViewer.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QEnhancedImage.py` & `krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QEnhancedImage.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QEnhancedImage_threaded.py` & `krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QEnhancedImage_threaded.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVDimensionLine.py` & `krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QIVDimensionLine.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVGrid.py` & `krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QIVGrid.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVHudText.py` & `krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QIVHudText.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVLine.py` & `krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QIVLine.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVMarker.py` & `krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QIVMarker.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVMarkerText.py` & `krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QIVMarkerText.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVPolygon.py` & `krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QIVPolygon.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVPolygonItem.py` & `krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QIVPolygonItem.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QIVRubberBandLine.py` & `krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QIVRubberBandLine.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QImageViewer.py` & `krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QImageViewer.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QImageViewer_threaded.py` & `krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QImageViewer_threaded.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/QViewerBase.py` & `krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/QViewerBase.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/imageAdjustmentsDlg.py` & `krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/imageAdjustmentsDlg.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/imageAdjustmentsDlg_simple.py` & `krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/imageAdjustmentsDlg_simple.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/ui/ui_imageAdjustmentsDlg.py` & `krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/ui/ui_imageAdjustmentsDlg.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/ui/ui_imageAdjustmentsDlg_simple.py` & `krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/ui/ui_imageAdjustmentsDlg_simple.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/plotting/qt/QImageViewer/ui/ui_simple.py` & `krillscan-0.3.1/krillscan/echolab2/plotting/qt/QImageViewer/ui/ui_simple.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/plotting/qt/ui/ui_echogram_viewer.py` & `krillscan-0.3.1/krillscan/echolab2/plotting/qt/ui/ui_echogram_viewer.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/processing/afsc_bot_detector.py` & `krillscan-0.3.1/krillscan/echolab2/processing/afsc_bot_detector.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/processing/batch_utils.py` & `krillscan-0.3.1/krillscan/echolab2/processing/batch_utils.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/processing/grid.py` & `krillscan-0.3.1/krillscan/echolab2/processing/grid.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/processing/line.py` & `krillscan-0.3.1/krillscan/echolab2/processing/line.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/processing/mask.py` & `krillscan-0.3.1/krillscan/echolab2/processing/mask.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echolab2/processing/processed_data.py` & `krillscan-0.3.1/krillscan/echolab2/processing/processed_data.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echopy/__init__.py` & `krillscan-0.3.1/krillscan/echopy/__init__.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echopy/cmaps.py` & `krillscan-0.3.1/krillscan/echopy/cmaps.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echopy/get_background.py` & `krillscan-0.3.1/krillscan/echopy/get_background.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echopy/mask_attenuated.py` & `krillscan-0.3.1/krillscan/echopy/mask_attenuated.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echopy/mask_impulse.py` & `krillscan-0.3.1/krillscan/echopy/mask_impulse.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echopy/mask_multifrequency.py` & `krillscan-0.3.1/krillscan/echopy/mask_multifrequency.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echopy/mask_range.py` & `krillscan-0.3.1/krillscan/echopy/mask_range.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echopy/mask_seabed.py` & `krillscan-0.3.1/krillscan/echopy/mask_seabed.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echopy/mask_shoals.py` & `krillscan-0.3.1/krillscan/echopy/mask_shoals.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echopy/mask_signal2noise.py` & `krillscan-0.3.1/krillscan/echopy/mask_signal2noise.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echopy/mask_stationary.py` & `krillscan-0.3.1/krillscan/echopy/mask_stationary.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echopy/mask_transient.py` & `krillscan-0.3.1/krillscan/echopy/mask_transient.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echopy/read_calibration.py` & `krillscan-0.3.1/krillscan/echopy/read_calibration.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echopy/resample.py` & `krillscan-0.3.1/krillscan/echopy/resample.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/echopy/transform.py` & `krillscan-0.3.1/krillscan/echopy/transform.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/krillscan/inspect.py` & `krillscan-0.3.1/krillscan/inspect.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/krillscan/process.py` & `krillscan-0.3.1/krillscan/process.py`

 * *Files identical despite different names*

### Comparing `krillscan-0.3.0/krillscan.egg-info/PKG-INFO` & `krillscan-0.3.1/krillscan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krillscan
-Version: 0.3.0
+Version: 0.3.1
 Summary: A python module for automatic analysis of backscatter data from vessels of opportunity
 Home-page: 
 Author: Sebastian Menze
 Author-email: sebastian.menze@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Requires-Dist: lxml
```

### Comparing `krillscan-0.3.0/setup.py` & `krillscan-0.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "readme.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="krillscan",
-    version="0.3.0",
+    version="0.3.1",
     description="A python module for automatic analysis of backscatter data from vessels of opportunity",
     long_description=README,
     long_description_content_type="text/markdown",
     url="",
     author="Sebastian Menze",
     author_email="sebastian.menze@gmail.com",
     classifiers=[
```

