# Comparing `tmp/testwizard.commands-video-3.8.1b4749.tar.gz` & `tmp/testwizard.commands-video-3.8.1b4810.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testwizard.commands-video-3.8.1b4749.tar", last modified: Tue Mar 19 15:01:43 2024, max compression
+gzip compressed data, was "testwizard.commands-video-3.8.1b4810.tar", last modified: Wed Mar 27 12:56:30 2024, max compression
```

## Comparing `testwizard.commands-video-3.8.1b4749.tar` & `testwizard.commands-video-3.8.1b4810.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:43.398747 testwizard.commands-video-3.8.1b4749/
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/LICENSE.txt
--rw-rw-rw-   0        0        0      541 2024-03-19 15:01:43.398747 testwizard.commands-video-3.8.1b4749/PKG-INFO
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/README.md
--rw-rw-rw-   0        0        0       42 2024-03-19 15:01:43.398747 testwizard.commands-video-3.8.1b4749/setup.cfg
--rw-rw-rw-   0        0        0      819 2024-03-19 15:01:43.000000 testwizard.commands-video-3.8.1b4749/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:43.367602 testwizard.commands-video-3.8.1b4749/testwizard/
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:43.398747 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/
--rw-rw-rw-   0        0        0      511 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/CaptureReferenceBitmapCommand.py
--rw-rw-rw-   0        0        0      583 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/ClearOnScreenDisplayCommand.py
--rw-rw-rw-   0        0        0      524 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/CompareCommand.py
--rw-rw-rw-   0        0        0      549 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/CompareResult.py
--rw-rw-rw-   0        0        0      576 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/CountLastPatternMatchesCommand.py
--rw-rw-rw-   0        0        0      572 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/CountLastPatternMatchesResult.py
--rw-rw-rw-   0        0        0      499 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/DeleteAllRecordingsCommand.py
--rw-rw-rw-   0        0        0      509 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/DeleteAllSnapshotsCommand.py
--rw-rw-rw-   0        0        0     1251 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/DetectMotionCommand.py
--rw-rw-rw-   0        0        0      784 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/DetectMotionResult.py
--rw-rw-rw-   0        0        0     1259 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/DetectNoMotionCommand.py
--rw-rw-rw-   0        0        0      497 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/FilterBlackWhiteCommand.py
--rw-rw-rw-   0        0        0      511 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/FilterCBICommand.py
--rw-rw-rw-   0        0        0      529 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/FilterColorBlackWhiteCommand.py
--rw-rw-rw-   0        0        0      485 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/FilterGrayscaleCommand.py
--rw-rw-rw-   0        0        0      459 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/FilterInvertCommand.py
--rw-rw-rw-   0        0        0      463 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/FilterResult.py
--rw-rw-rw-   0        0        0      608 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/FindAllPatternLocationsCommand.py
--rw-rw-rw-   0        0        0      654 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/FindAllPatternLocationsExCommand.py
--rw-rw-rw-   0        0        0      600 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/FindAllPatternLocationsResult.py
--rw-rw-rw-   0        0        0      511 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/FindPatternCommand.py
--rw-rw-rw-   0        0        0      546 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/FindPatternExCommand.py
--rw-rw-rw-   0        0        0      592 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/FindPatternResult.py
--rw-rw-rw-   0        0        0      519 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/GetVideoResolutionCommand.py
--rw-rw-rw-   0        0        0      382 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/GetVideoResolutionResult.py
--rw-rw-rw-   0        0        0      529 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/LoadReferenceBitmapCommand.py
--rw-rw-rw-   0        0        0      716 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/SaveFileResult.py
--rw-rw-rw-   0        0        0      511 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/SaveReferenceBitmapCommand.py
--rw-rw-rw-   0        0        0      475 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/SaveRegionCommand.py
--rw-rw-rw-   0        0        0     1079 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/SetAttributeOnScreenDisplayCommand.py
--rw-rw-rw-   0        0        0      487 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/SetRegionCommand.py
--rw-rw-rw-   0        0        0     1023 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/SetTextOnScreenDisplayCommand.py
--rw-rw-rw-   0        0        0      479 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/SnapShotBMPCommand.py
--rw-rw-rw-   0        0        0      596 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/SnapShotCommand.py
--rw-rw-rw-   0        0        0      569 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/SnapShotJPGCommand.py
--rw-rw-rw-   0        0        0      553 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/StartBackgroundCaptureCommand.py
--rw-rw-rw-   0        0        0      491 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/StartRecordingCommand.py
--rw-rw-rw-   0        0        0      499 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/StopBackgroundCaptureCommand.py
--rw-rw-rw-   0        0        0      475 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/StopRecordingCommand.py
--rw-rw-rw-   0        0        0      464 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/TextOCRCommand.py
--rw-rw-rw-   0        0        0      502 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/TextOCRResult.py
--rw-rw-rw-   0        0        0      630 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/WaitForColorCommand.py
--rw-rw-rw-   0        0        0      658 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/WaitForColorNoMatchCommand.py
--rw-rw-rw-   0        0        0      971 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/WaitForColorResult.py
--rw-rw-rw-   0        0        0      611 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/WaitForPatternCommand.py
--rw-rw-rw-   0        0        0      662 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/WaitForPatternNoMatchCommand.py
--rw-rw-rw-   0        0        0      629 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/WaitForPatternResult.py
--rw-rw-rw-   0        0        0      865 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/WaitForSampleCommand.py
--rw-rw-rw-   0        0        0      893 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/WaitForSampleNoMatchCommand.py
--rw-rw-rw-   0        0        0      642 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/WaitForSampleResult.py
--rw-rw-rw-   0        0        0     2358 2024-03-19 15:00:53.000000 testwizard.commands-video-3.8.1b4749/testwizard/commands_video/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:43.367602 testwizard.commands-video-3.8.1b4749/testwizard.commands_video.egg-info/
--rw-rw-rw-   0        0        0      541 2024-03-19 15:01:43.000000 testwizard.commands-video-3.8.1b4749/testwizard.commands_video.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2914 2024-03-19 15:01:43.000000 testwizard.commands-video-3.8.1b4749/testwizard.commands_video.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 15:01:43.000000 testwizard.commands-video-3.8.1b4749/testwizard.commands_video.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-03-19 15:01:43.000000 testwizard.commands-video-3.8.1b4749/testwizard.commands_video.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-19 15:01:43.000000 testwizard.commands-video-3.8.1b4749/testwizard.commands_video.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:30.506344 testwizard.commands-video-3.8.1b4810/
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/LICENSE.txt
+-rw-rw-rw-   0        0        0      541 2024-03-27 12:56:30.506344 testwizard.commands-video-3.8.1b4810/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-27 12:56:30.506344 testwizard.commands-video-3.8.1b4810/setup.cfg
+-rw-rw-rw-   0        0        0      819 2024-03-27 12:56:30.000000 testwizard.commands-video-3.8.1b4810/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:30.475093 testwizard.commands-video-3.8.1b4810/testwizard/
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:30.506344 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/
+-rw-rw-rw-   0        0        0      511 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/CaptureReferenceBitmapCommand.py
+-rw-rw-rw-   0        0        0      583 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/ClearOnScreenDisplayCommand.py
+-rw-rw-rw-   0        0        0      524 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/CompareCommand.py
+-rw-rw-rw-   0        0        0      549 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/CompareResult.py
+-rw-rw-rw-   0        0        0      576 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/CountLastPatternMatchesCommand.py
+-rw-rw-rw-   0        0        0      572 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/CountLastPatternMatchesResult.py
+-rw-rw-rw-   0        0        0      499 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/DeleteAllRecordingsCommand.py
+-rw-rw-rw-   0        0        0      509 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/DeleteAllSnapshotsCommand.py
+-rw-rw-rw-   0        0        0     1251 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/DetectMotionCommand.py
+-rw-rw-rw-   0        0        0      784 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/DetectMotionResult.py
+-rw-rw-rw-   0        0        0     1259 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/DetectNoMotionCommand.py
+-rw-rw-rw-   0        0        0      497 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/FilterBlackWhiteCommand.py
+-rw-rw-rw-   0        0        0      511 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/FilterCBICommand.py
+-rw-rw-rw-   0        0        0      529 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/FilterColorBlackWhiteCommand.py
+-rw-rw-rw-   0        0        0      485 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/FilterGrayscaleCommand.py
+-rw-rw-rw-   0        0        0      459 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/FilterInvertCommand.py
+-rw-rw-rw-   0        0        0      463 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/FilterResult.py
+-rw-rw-rw-   0        0        0      608 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/FindAllPatternLocationsCommand.py
+-rw-rw-rw-   0        0        0      654 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/FindAllPatternLocationsExCommand.py
+-rw-rw-rw-   0        0        0      600 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/FindAllPatternLocationsResult.py
+-rw-rw-rw-   0        0        0      511 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/FindPatternCommand.py
+-rw-rw-rw-   0        0        0      546 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/FindPatternExCommand.py
+-rw-rw-rw-   0        0        0      592 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/FindPatternResult.py
+-rw-rw-rw-   0        0        0      519 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/GetVideoResolutionCommand.py
+-rw-rw-rw-   0        0        0      382 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/GetVideoResolutionResult.py
+-rw-rw-rw-   0        0        0      529 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/LoadReferenceBitmapCommand.py
+-rw-rw-rw-   0        0        0      716 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/SaveFileResult.py
+-rw-rw-rw-   0        0        0      511 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/SaveReferenceBitmapCommand.py
+-rw-rw-rw-   0        0        0      475 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/SaveRegionCommand.py
+-rw-rw-rw-   0        0        0     1079 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/SetAttributeOnScreenDisplayCommand.py
+-rw-rw-rw-   0        0        0      487 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/SetRegionCommand.py
+-rw-rw-rw-   0        0        0     1023 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/SetTextOnScreenDisplayCommand.py
+-rw-rw-rw-   0        0        0      479 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/SnapShotBMPCommand.py
+-rw-rw-rw-   0        0        0      596 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/SnapShotCommand.py
+-rw-rw-rw-   0        0        0      569 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/SnapShotJPGCommand.py
+-rw-rw-rw-   0        0        0      553 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/StartBackgroundCaptureCommand.py
+-rw-rw-rw-   0        0        0      491 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/StartRecordingCommand.py
+-rw-rw-rw-   0        0        0      499 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/StopBackgroundCaptureCommand.py
+-rw-rw-rw-   0        0        0      475 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/StopRecordingCommand.py
+-rw-rw-rw-   0        0        0      464 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/TextOCRCommand.py
+-rw-rw-rw-   0        0        0      502 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/TextOCRResult.py
+-rw-rw-rw-   0        0        0      630 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/WaitForColorCommand.py
+-rw-rw-rw-   0        0        0      658 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/WaitForColorNoMatchCommand.py
+-rw-rw-rw-   0        0        0      971 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/WaitForColorResult.py
+-rw-rw-rw-   0        0        0      611 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/WaitForPatternCommand.py
+-rw-rw-rw-   0        0        0      662 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/WaitForPatternNoMatchCommand.py
+-rw-rw-rw-   0        0        0      629 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/WaitForPatternResult.py
+-rw-rw-rw-   0        0        0      865 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/WaitForSampleCommand.py
+-rw-rw-rw-   0        0        0      893 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/WaitForSampleNoMatchCommand.py
+-rw-rw-rw-   0        0        0      642 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/WaitForSampleResult.py
+-rw-rw-rw-   0        0        0     2358 2024-03-27 12:55:37.000000 testwizard.commands-video-3.8.1b4810/testwizard/commands_video/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:30.475093 testwizard.commands-video-3.8.1b4810/testwizard.commands_video.egg-info/
+-rw-rw-rw-   0        0        0      541 2024-03-27 12:56:30.000000 testwizard.commands-video-3.8.1b4810/testwizard.commands_video.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2914 2024-03-27 12:56:30.000000 testwizard.commands-video-3.8.1b4810/testwizard.commands_video.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-27 12:56:30.000000 testwizard.commands-video-3.8.1b4810/testwizard.commands_video.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-03-27 12:56:30.000000 testwizard.commands-video-3.8.1b4810/testwizard.commands_video.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-03-27 12:56:30.000000 testwizard.commands-video-3.8.1b4810/testwizard.commands_video.egg-info/top_level.txt
```

### Comparing `testwizard.commands-video-3.8.1b4749/PKG-INFO` & `testwizard.commands-video-3.8.1b4810/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.commands-video
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard Video commands
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

### Comparing `testwizard.commands-video-3.8.1b4749/setup.py` & `testwizard.commands-video-3.8.1b4810/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="testwizard.commands-video",
-    version="3.8.1b4749",
+    version="3.8.1b4810",
     author="Resillion",
     author_email="testwizard-support@resillion.com",
     description="Testwizard Video commands",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.resillion.com/services/software-testing/testing-tools/testwizard/",
     packages=['testwizard.commands_video'],
     install_requires=[
-        'testwizard.commands-core==3.8.1b4749'
+        'testwizard.commands-core==3.8.1b4810'
     ],
     classifiers=[
         "Programming Language :: Python :: 3.3",
         "Development Status :: 5 - Production/Stable",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/ClearOnScreenDisplayCommand.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/ClearOnScreenDisplayCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/CompareCommand.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/CompareCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/CompareResult.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/CompareResult.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/CountLastPatternMatchesCommand.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/CountLastPatternMatchesCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/CountLastPatternMatchesResult.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/CountLastPatternMatchesResult.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/DetectMotionCommand.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/DetectMotionCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/DetectMotionResult.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/DetectMotionResult.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/DetectNoMotionCommand.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/DetectNoMotionCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/FilterColorBlackWhiteCommand.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/FilterColorBlackWhiteCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/FindAllPatternLocationsCommand.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/FindAllPatternLocationsCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/FindAllPatternLocationsExCommand.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/FindAllPatternLocationsExCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/FindAllPatternLocationsResult.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/FindAllPatternLocationsResult.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/FindPatternExCommand.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/FindPatternExCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/FindPatternResult.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/FindPatternResult.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/GetVideoResolutionCommand.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/GetVideoResolutionCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/LoadReferenceBitmapCommand.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/LoadReferenceBitmapCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/SaveFileResult.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/SaveFileResult.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/SetAttributeOnScreenDisplayCommand.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/SetAttributeOnScreenDisplayCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/SetTextOnScreenDisplayCommand.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/SetTextOnScreenDisplayCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/SnapShotCommand.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/SnapShotCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/SnapShotJPGCommand.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/SnapShotJPGCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/StartBackgroundCaptureCommand.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/StartBackgroundCaptureCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/WaitForColorCommand.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/WaitForColorCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/WaitForColorNoMatchCommand.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/WaitForColorNoMatchCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/WaitForColorResult.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/WaitForColorResult.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/WaitForPatternCommand.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/WaitForPatternCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/WaitForPatternNoMatchCommand.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/WaitForPatternNoMatchCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/WaitForPatternResult.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/WaitForPatternResult.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/WaitForSampleCommand.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/WaitForSampleCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/WaitForSampleNoMatchCommand.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/WaitForSampleNoMatchCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/WaitForSampleResult.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/WaitForSampleResult.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard/commands_video/__init__.py` & `testwizard.commands-video-3.8.1b4810/testwizard/commands_video/__init__.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard.commands_video.egg-info/PKG-INFO` & `testwizard.commands-video-3.8.1b4810/testwizard.commands_video.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.commands-video
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard Video commands
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

### Comparing `testwizard.commands-video-3.8.1b4749/testwizard.commands_video.egg-info/SOURCES.txt` & `testwizard.commands-video-3.8.1b4810/testwizard.commands_video.egg-info/SOURCES.txt`

 * *Files identical despite different names*

