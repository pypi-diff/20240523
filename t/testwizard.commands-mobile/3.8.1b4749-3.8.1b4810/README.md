# Comparing `tmp/testwizard.commands-mobile-3.8.1b4749.tar.gz` & `tmp/testwizard.commands-mobile-3.8.1b4810.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testwizard.commands-mobile-3.8.1b4749.tar", last modified: Tue Mar 19 15:01:40 2024, max compression
+gzip compressed data, was "testwizard.commands-mobile-3.8.1b4810.tar", last modified: Wed Mar 27 12:56:27 2024, max compression
```

## Comparing `testwizard.commands-mobile-3.8.1b4749.tar` & `testwizard.commands-mobile-3.8.1b4810.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:40.631676 testwizard.commands-mobile-3.8.1b4749/
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/LICENSE.txt
--rw-rw-rw-   0        0        0      543 2024-03-19 15:01:40.616048 testwizard.commands-mobile-3.8.1b4749/PKG-INFO
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/README.md
--rw-rw-rw-   0        0        0       42 2024-03-19 15:01:40.631676 testwizard.commands-mobile-3.8.1b4749/setup.cfg
--rw-rw-rw-   0        0        0      908 2024-03-19 15:01:40.000000 testwizard.commands-mobile-3.8.1b4749/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:40.584802 testwizard.commands-mobile-3.8.1b4749/testwizard/
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:40.616048 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/
--rw-rw-rw-   0        0        0      584 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/ActivateAppCommand.py
--rw-rw-rw-   0        0        0      518 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/AddCapabilityCommand.py
--rw-rw-rw-   0        0        0      534 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/Android_SendKeyCodeCommand.py
--rw-rw-rw-   0        0        0      508 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/ClearElementCommand.py
--rw-rw-rw-   0        0        0      508 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/ClickElementCommand.py
--rw-rw-rw-   0        0        0      504 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/ClickPositionCommand.py
--rw-rw-rw-   0        0        0      572 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/CloseAppCommand.py
--rw-rw-rw-   0        0        0      500 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/FindElementCommand.py
--rw-rw-rw-   0        0        0      519 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/GetAppiumSettingsCommand.py
--rw-rw-rw-   0        0        0      369 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/GetAppiumSettingsResult.py
--rw-rw-rw-   0        0        0      573 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/GetElementAttributeCommand.py
--rw-rw-rw-   0        0        0      353 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/GetElementAttributeResult.py
--rw-rw-rw-   0        0        0      488 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/GetElementCommand.py
--rw-rw-rw-   0        0        0      574 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/GetElementLocationCommand.py
--rw-rw-rw-   0        0        0      392 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/GetElementLocationResult.py
--rw-rw-rw-   0        0        0      321 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/GetElementResult.py
--rw-rw-rw-   0        0        0      495 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/GetElementSizeCommand.py
--rw-rw-rw-   0        0        0      495 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/GetElementsCommand.py
--rw-rw-rw-   0        0        0      411 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/GetElementsResult.py
--rw-rw-rw-   0        0        0      498 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/GetOrientationCommand.py
--rw-rw-rw-   0        0        0      362 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/GetOrientationResult.py
--rw-rw-rw-   0        0        0      473 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/GetScreenSizeCommand.py
--rw-rw-rw-   0        0        0      381 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/GetSizeResult.py
--rw-rw-rw-   0        0        0      466 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/GetSourceCommand.py
--rw-rw-rw-   0        0        0      363 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/GetSourceResult.py
--rw-rw-rw-   0        0        0      585 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/HideKeyboardCommand.py
--rw-rw-rw-   0        0        0      586 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/InitDriverCommand.py
--rw-rw-rw-   0        0        0      508 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/InputTextCommand.py
--rw-rw-rw-   0        0        0      500 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/InstallAppCommand.py
--rw-rw-rw-   0        0        0      596 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/IsAppInstalledCommand.py
--rw-rw-rw-   0        0        0      329 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/IsAppInstalledResult.py
--rw-rw-rw-   0        0        0      576 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/LaunchAppCommand.py
--rw-rw-rw-   0        0        0      524 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/MultiTouch_AddCommand.py
--rw-rw-rw-   0        0        0      522 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/MultiTouch_NewCommand.py
--rw-rw-rw-   0        0        0      514 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/MultiTouch_PerformCommand.py
--rw-rw-rw-   0        0        0      532 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/PinchCoordinatesCommand.py
--rw-rw-rw-   0        0        0      508 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/PinchElementCommand.py
--rw-rw-rw-   0        0        0      589 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/QueryAppStateCommand.py
--rw-rw-rw-   0        0        0      326 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/QueryAppStateResult.py
--rw-rw-rw-   0        0        0      482 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/QuitDriverCommand.py
--rw-rw-rw-   0        0        0      490 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/RemoveAppCommand.py
--rw-rw-rw-   0        0        0      570 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/ResetAppCommand.py
--rw-rw-rw-   0        0        0      607 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/RunAppInBackgroundCommand.py
--rw-rw-rw-   0        0        0      588 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/ScreenShotJPGCommand.py
--rw-rw-rw-   0        0        0      500 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/ScreenshotBMPCommand.py
--rw-rw-rw-   0        0        0      447 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/ScreenshotResult.py
--rw-rw-rw-   0        0        0      540 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/SetAppiumSettingsCommand.py
--rw-rw-rw-   0        0        0      522 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/SetOrientationCommand.py
--rw-rw-rw-   0        0        0      572 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/StartDeviceLoggingCommand.py
--rw-rw-rw-   0        0        0      510 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/StopDeviceLoggingCommand.py
--rw-rw-rw-   0        0        0      582 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/SwipeArcCommand.py
--rw-rw-rw-   0        0        0      536 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/SwipeCommand.py
--rw-rw-rw-   0        0        0      524 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/TouchAction_MoveToCommand.py
--rw-rw-rw-   0        0        0      574 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/TouchAction_MoveToElementCommand.py
--rw-rw-rw-   0        0        0      527 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/TouchAction_NewCommand.py
--rw-rw-rw-   0        0        0      518 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/TouchAction_PerformCommand.py
--rw-rw-rw-   0        0        0      520 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/TouchAction_PressCommand.py
--rw-rw-rw-   0        0        0      570 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/TouchAction_PressElementCommand.py
--rw-rw-rw-   0        0        0      518 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/TouchAction_ReleaseCommand.py
--rw-rw-rw-   0        0        0      512 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/TouchAction_TapCommand.py
--rw-rw-rw-   0        0        0      524 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/TouchAction_WaitCommand.py
--rw-rw-rw-   0        0        0      536 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/WaitForElementCommand.py
--rw-rw-rw-   0        0        0      366 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/WaitForElementResult.py
--rw-rw-rw-   0        0        0      528 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/ZoomCoordinatesCommand.py
--rw-rw-rw-   0        0        0      504 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/ZoomElementCommand.py
--rw-rw-rw-   0        0        0     3056 2024-03-19 15:00:53.000000 testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:40.584802 testwizard.commands-mobile-3.8.1b4749/testwizard.commands_mobile.egg-info/
--rw-rw-rw-   0        0        0      543 2024-03-19 15:01:40.000000 testwizard.commands-mobile-3.8.1b4749/testwizard.commands_mobile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3665 2024-03-19 15:01:40.000000 testwizard.commands-mobile-3.8.1b4749/testwizard.commands_mobile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 15:01:40.000000 testwizard.commands-mobile-3.8.1b4749/testwizard.commands_mobile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-03-19 15:01:40.000000 testwizard.commands-mobile-3.8.1b4749/testwizard.commands_mobile.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-19 15:01:40.000000 testwizard.commands-mobile-3.8.1b4749/testwizard.commands_mobile.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:27.270910 testwizard.commands-mobile-3.8.1b4810/
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/LICENSE.txt
+-rw-rw-rw-   0        0        0      543 2024-03-27 12:56:27.270910 testwizard.commands-mobile-3.8.1b4810/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-27 12:56:27.270910 testwizard.commands-mobile-3.8.1b4810/setup.cfg
+-rw-rw-rw-   0        0        0      908 2024-03-27 12:56:26.000000 testwizard.commands-mobile-3.8.1b4810/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:27.239722 testwizard.commands-mobile-3.8.1b4810/testwizard/
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:27.270910 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/
+-rw-rw-rw-   0        0        0      584 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/ActivateAppCommand.py
+-rw-rw-rw-   0        0        0      518 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/AddCapabilityCommand.py
+-rw-rw-rw-   0        0        0      534 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/Android_SendKeyCodeCommand.py
+-rw-rw-rw-   0        0        0      508 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/ClearElementCommand.py
+-rw-rw-rw-   0        0        0      508 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/ClickElementCommand.py
+-rw-rw-rw-   0        0        0      504 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/ClickPositionCommand.py
+-rw-rw-rw-   0        0        0      563 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/CloseAppCommand.py
+-rw-rw-rw-   0        0        0      500 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/FindElementCommand.py
+-rw-rw-rw-   0        0        0      519 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/GetAppiumSettingsCommand.py
+-rw-rw-rw-   0        0        0      369 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/GetAppiumSettingsResult.py
+-rw-rw-rw-   0        0        0      573 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/GetElementAttributeCommand.py
+-rw-rw-rw-   0        0        0      353 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/GetElementAttributeResult.py
+-rw-rw-rw-   0        0        0      488 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/GetElementCommand.py
+-rw-rw-rw-   0        0        0      574 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/GetElementLocationCommand.py
+-rw-rw-rw-   0        0        0      392 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/GetElementLocationResult.py
+-rw-rw-rw-   0        0        0      321 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/GetElementResult.py
+-rw-rw-rw-   0        0        0      495 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/GetElementSizeCommand.py
+-rw-rw-rw-   0        0        0      495 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/GetElementsCommand.py
+-rw-rw-rw-   0        0        0      411 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/GetElementsResult.py
+-rw-rw-rw-   0        0        0      498 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/GetOrientationCommand.py
+-rw-rw-rw-   0        0        0      362 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/GetOrientationResult.py
+-rw-rw-rw-   0        0        0      473 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/GetScreenSizeCommand.py
+-rw-rw-rw-   0        0        0      381 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/GetSizeResult.py
+-rw-rw-rw-   0        0        0      466 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/GetSourceCommand.py
+-rw-rw-rw-   0        0        0      363 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/GetSourceResult.py
+-rw-rw-rw-   0        0        0      585 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/HideKeyboardCommand.py
+-rw-rw-rw-   0        0        0      586 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/InitDriverCommand.py
+-rw-rw-rw-   0        0        0      508 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/InputTextCommand.py
+-rw-rw-rw-   0        0        0      500 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/InstallAppCommand.py
+-rw-rw-rw-   0        0        0      596 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/IsAppInstalledCommand.py
+-rw-rw-rw-   0        0        0      329 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/IsAppInstalledResult.py
+-rw-rw-rw-   0        0        0      697 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/LaunchAppCommand.py
+-rw-rw-rw-   0        0        0      524 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/MultiTouch_AddCommand.py
+-rw-rw-rw-   0        0        0      522 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/MultiTouch_NewCommand.py
+-rw-rw-rw-   0        0        0      514 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/MultiTouch_PerformCommand.py
+-rw-rw-rw-   0        0        0      532 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/PinchCoordinatesCommand.py
+-rw-rw-rw-   0        0        0      508 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/PinchElementCommand.py
+-rw-rw-rw-   0        0        0      589 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/QueryAppStateCommand.py
+-rw-rw-rw-   0        0        0      326 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/QueryAppStateResult.py
+-rw-rw-rw-   0        0        0      482 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/QuitDriverCommand.py
+-rw-rw-rw-   0        0        0      490 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/RemoveAppCommand.py
+-rw-rw-rw-   0        0        0      474 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/ResetAppCommand.py
+-rw-rw-rw-   0        0        0      607 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/RunAppInBackgroundCommand.py
+-rw-rw-rw-   0        0        0      588 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/ScreenShotJPGCommand.py
+-rw-rw-rw-   0        0        0      500 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/ScreenshotBMPCommand.py
+-rw-rw-rw-   0        0        0      447 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/ScreenshotResult.py
+-rw-rw-rw-   0        0        0      540 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/SetAppiumSettingsCommand.py
+-rw-rw-rw-   0        0        0      522 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/SetOrientationCommand.py
+-rw-rw-rw-   0        0        0      572 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/StartDeviceLoggingCommand.py
+-rw-rw-rw-   0        0        0      510 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/StopDeviceLoggingCommand.py
+-rw-rw-rw-   0        0        0      582 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/SwipeArcCommand.py
+-rw-rw-rw-   0        0        0      536 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/SwipeCommand.py
+-rw-rw-rw-   0        0        0      524 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/TouchAction_MoveToCommand.py
+-rw-rw-rw-   0        0        0      574 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/TouchAction_MoveToElementCommand.py
+-rw-rw-rw-   0        0        0      527 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/TouchAction_NewCommand.py
+-rw-rw-rw-   0        0        0      518 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/TouchAction_PerformCommand.py
+-rw-rw-rw-   0        0        0      520 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/TouchAction_PressCommand.py
+-rw-rw-rw-   0        0        0      570 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/TouchAction_PressElementCommand.py
+-rw-rw-rw-   0        0        0      518 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/TouchAction_ReleaseCommand.py
+-rw-rw-rw-   0        0        0      512 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/TouchAction_TapCommand.py
+-rw-rw-rw-   0        0        0      524 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/TouchAction_WaitCommand.py
+-rw-rw-rw-   0        0        0      536 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/WaitForElementCommand.py
+-rw-rw-rw-   0        0        0      366 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/WaitForElementResult.py
+-rw-rw-rw-   0        0        0      528 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/ZoomCoordinatesCommand.py
+-rw-rw-rw-   0        0        0      504 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/ZoomElementCommand.py
+-rw-rw-rw-   0        0        0     3056 2024-03-27 12:55:37.000000 testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:27.239722 testwizard.commands-mobile-3.8.1b4810/testwizard.commands_mobile.egg-info/
+-rw-rw-rw-   0        0        0      543 2024-03-27 12:56:27.000000 testwizard.commands-mobile-3.8.1b4810/testwizard.commands_mobile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3665 2024-03-27 12:56:27.000000 testwizard.commands-mobile-3.8.1b4810/testwizard.commands_mobile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-27 12:56:27.000000 testwizard.commands-mobile-3.8.1b4810/testwizard.commands_mobile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-03-27 12:56:27.000000 testwizard.commands-mobile-3.8.1b4810/testwizard.commands_mobile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-03-27 12:56:27.000000 testwizard.commands-mobile-3.8.1b4810/testwizard.commands_mobile.egg-info/top_level.txt
```

### Comparing `testwizard.commands-mobile-3.8.1b4749/PKG-INFO` & `testwizard.commands-mobile-3.8.1b4810/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.commands-mobile
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard Mobile commands
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

### Comparing `testwizard.commands-mobile-3.8.1b4749/setup.py` & `testwizard.commands-mobile-3.8.1b4810/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="testwizard.commands-mobile",
-    version="3.8.1b4749",
+    version="3.8.1b4810",
     author="Resillion",
     author_email="testwizard-support@resillion.com",
     description="Testwizard Mobile commands",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.resillion.com/services/software-testing/testing-tools/testwizard/",
     packages=['testwizard.commands_mobile'],
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

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/ActivateAppCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/ActivateAppCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/AddCapabilityCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/AddCapabilityCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/Android_SendKeyCodeCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/Android_SendKeyCodeCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/CloseAppCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/InitDriverCommand.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-00000000: 0d0a 696d 706f 7274 2073 7973 0d0a 696d  ..import sys..im
-00000010: 706f 7274 206a 736f 6e0d 0a0d 0a66 726f  port json....fro
-00000020: 6d20 7465 7374 7769 7a61 7264 2e63 6f6d  m testwizard.com
-00000030: 6d61 6e64 735f 636f 7265 2069 6d70 6f72  mands_core impor
-00000040: 7420 436f 6d6d 616e 6442 6173 650d 0a66  t CommandBase..f
-00000050: 726f 6d20 7465 7374 7769 7a61 7264 2e63  rom testwizard.c
-00000060: 6f6d 6d61 6e64 735f 636f 7265 2e53 696d  ommands_core.Sim
-00000070: 706c 6552 6573 756c 7420 696d 706f 7274  pleResult import
-00000080: 2053 696d 706c 6552 6573 756c 740d 0a0d   SimpleResult...
-00000090: 0a0d 0a63 6c61 7373 2043 6c6f 7365 4170  ...class CloseAp
-000000a0: 7043 6f6d 6d61 6e64 2843 6f6d 6d61 6e64  pCommand(Command
-000000b0: 4261 7365 293a 0d0a 2020 2020 6465 6620  Base):..    def 
-000000c0: 5f5f 696e 6974 5f5f 2873 656c 662c 2074  __init__(self, t
-000000d0: 6573 744f 626a 6563 7429 3a0d 0a20 2020  estObject):..   
-000000e0: 2020 2020 2043 6f6d 6d61 6e64 4261 7365       CommandBase
-000000f0: 2e5f 5f69 6e69 745f 5f28 7365 6c66 2c20  .__init__(self, 
-00000100: 7465 7374 4f62 6a65 6374 2c20 224d 6f62  testObject, "Mob
-00000110: 696c 652e 436c 6f73 6541 7070 2229 0d0a  ile.CloseApp")..
-00000120: 0d0a 2020 2020 6465 6620 6578 6563 7574  ..    def execut
-00000130: 6528 7365 6c66 2c20 6275 6e64 6c65 4964  e(self, bundleId
-00000140: 293a 0d0a 2020 2020 2020 2020 6966 2062  ):..        if b
-00000150: 756e 646c 6549 6420 6973 204e 6f6e 653a  undleId is None:
-00000160: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00000170: 7175 6573 744f 626a 203d 205b 5d0d 0a20  questObj = [].. 
-00000180: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00000190: 2020 2020 2020 2020 2020 7265 7175 6573            reques
-000001a0: 744f 626a 203d 205b 6275 6e64 6c65 4964  tObj = [bundleId
-000001b0: 5d0d 0a0d 0a20 2020 2020 2020 2072 6573  ]....        res
-000001c0: 756c 7420 3d20 7365 6c66 2e65 7865 6375  ult = self.execu
-000001d0: 7465 436f 6d6d 616e 6428 7265 7175 6573  teCommand(reques
-000001e0: 744f 626a 290d 0a0d 0a20 2020 2020 2020  tObj)....       
-000001f0: 2072 6574 7572 6e20 5369 6d70 6c65 5265   return SimpleRe
-00000200: 7375 6c74 2872 6573 756c 742c 2022 436c  sult(result, "Cl
-00000210: 6f73 6541 7070 2077 6173 2073 7563 6365  oseApp was succe
-00000220: 7373 6675 6c22 2c20 2243 6c6f 7365 4170  ssful", "CloseAp
-00000230: 7020 6661 696c 6564 2229 0d0a            p failed")..
+00000000: 696d 706f 7274 2073 7973 0d0a 0d0a 6672  import sys....fr
+00000010: 6f6d 2074 6573 7477 697a 6172 642e 636f  om testwizard.co
+00000020: 6d6d 616e 6473 5f63 6f72 6520 696d 706f  mmands_core impo
+00000030: 7274 2043 6f6d 6d61 6e64 4261 7365 0d0a  rt CommandBase..
+00000040: 6672 6f6d 2074 6573 7477 697a 6172 642e  from testwizard.
+00000050: 636f 6d6d 616e 6473 5f63 6f72 652e 5369  commands_core.Si
+00000060: 6d70 6c65 5265 7375 6c74 2069 6d70 6f72  mpleResult impor
+00000070: 7420 5369 6d70 6c65 5265 7375 6c74 0d0a  t SimpleResult..
+00000080: 0d0a 696d 706f 7274 206a 736f 6e0d 0a63  ..import json..c
+00000090: 6c61 7373 2049 6e69 7444 7269 7665 7243  lass InitDriverC
+000000a0: 6f6d 6d61 6e64 2843 6f6d 6d61 6e64 4261  ommand(CommandBa
+000000b0: 7365 293a 0d0a 2020 2020 6465 6620 5f5f  se):..    def __
+000000c0: 696e 6974 5f5f 2873 656c 662c 2074 6573  init__(self, tes
+000000d0: 744f 626a 6563 7429 3a0d 0a20 2020 2020  tObject):..     
+000000e0: 2020 2043 6f6d 6d61 6e64 4261 7365 2e5f     CommandBase._
+000000f0: 5f69 6e69 745f 5f28 7365 6c66 2c20 7465  _init__(self, te
+00000100: 7374 4f62 6a65 6374 2c20 224d 6f62 696c  stObject, "Mobil
+00000110: 652e 496e 6974 4472 6976 6572 2229 0d0a  e.InitDriver")..
+00000120: 2020 2020 0d0a 2020 2020 6465 6620 6578      ..    def ex
+00000130: 6563 7574 6528 7365 6c66 2c20 6170 7050  ecute(self, appP
+00000140: 6174 6829 3a0d 0a20 2020 2020 2020 2069  ath):..        i
+00000150: 6620 6170 7050 6174 6820 6973 204e 6f6e  f appPath is Non
+00000160: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00000170: 7265 7175 6573 744f 626a 203d 205b 5d0d  requestObj = [].
+00000180: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
+00000190: 2020 2020 2020 2020 2020 2020 7265 7175              requ
+000001a0: 6573 744f 626a 203d 205b 6170 7050 6174  estObj = [appPat
+000001b0: 685d 0d0a 0d0a 2020 2020 2020 2020 7265  h]....        re
+000001c0: 7375 6c74 203d 2073 656c 662e 6578 6563  sult = self.exec
+000001d0: 7574 6543 6f6d 6d61 6e64 2872 6571 7565  uteCommand(reque
+000001e0: 7374 4f62 6a29 0d0a 2020 2020 2020 2020  stObj)..        
+000001f0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00000200: 2053 696d 706c 6552 6573 756c 7428 7265   SimpleResult(re
+00000210: 7375 6c74 2c20 2249 6e69 7444 7269 7665  sult, "InitDrive
+00000220: 7220 7761 7320 7375 6363 6573 7366 756c  r was successful
+00000230: 222c 2022 496e 6974 4472 6976 6572 2066  ", "InitDriver f
+00000240: 6169 6c65 6422 2920 2020                 ailed")
```

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/GetAppiumSettingsCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/GetAppiumSettingsCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/GetElementAttributeCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/GetElementAttributeCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/GetElementLocationCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/GetElementLocationCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/HideKeyboardCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/HideKeyboardCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/InitDriverCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/TouchAction_MoveToElementCommand.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import sys
+import json
 
 from testwizard.commands_core import CommandBase
 from testwizard.commands_core.SimpleResult import SimpleResult
 
-import json
-class InitDriverCommand(CommandBase):
+
+class TouchAction_MoveToElementCommand(CommandBase):
     def __init__(self, testObject):
-        CommandBase.__init__(self, testObject, "Mobile.InitDriver")
-    
-    def execute(self, appPath):
-        if appPath is None:
-            requestObj = []
-        else:
-            requestObj = [appPath]
+        CommandBase.__init__(
+            self, testObject, "Mobile.TouchAction_MoveToElement")
+
+    def execute(self, selector):
+        requestObj = [selector]
 
         result = self.executeCommand(requestObj)
-        
-        return SimpleResult(result, "InitDriver was successful", "InitDriver failed")   
+
+        return SimpleResult(result, "TouchAction_MoveToElement was successful", "TouchAction_MoveToElement failed")
```

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/IsAppInstalledCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/IsAppInstalledCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/MultiTouch_AddCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/MultiTouch_AddCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/MultiTouch_NewCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/MultiTouch_NewCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/MultiTouch_PerformCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/MultiTouch_PerformCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/PinchCoordinatesCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/PinchCoordinatesCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/QueryAppStateCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/QueryAppStateCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/ResetAppCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/LaunchAppCommand.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,25 @@
+
 import sys
 import json
 
 from testwizard.commands_core import CommandBase
 from testwizard.commands_core.SimpleResult import SimpleResult
 
 
-class ResetAppCommand(CommandBase):
+class LaunchAppCommand(CommandBase):
     def __init__(self, testObject):
-        CommandBase.__init__(self, testObject, "Mobile.ResetApp")
+        CommandBase.__init__(self, testObject, "Mobile.LaunchApp")
 
-    def execute(self, bundleId):
-        if bundleId is None:
-            requestObj = []
+    def execute(self, appId, activityId):
+        requestObj = []
+        if appId is None:
+            requestObj.append(None)
         else:
-            requestObj = [bundleId]
+            requestObj.append(appId)
+
+        if activityId is not None:
+            requestObj.append(activityId)
 
         result = self.executeCommand(requestObj)
 
-        return SimpleResult(result, "ResetApp was successful", "ResetApp failed")
+        return SimpleResult(result, "LaunchApp was successful", "LaunchApp failed")
```

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/RunAppInBackgroundCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/RunAppInBackgroundCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/ScreenShotJPGCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/ScreenShotJPGCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/SetAppiumSettingsCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/SetAppiumSettingsCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/SetOrientationCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/SetOrientationCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/StartDeviceLoggingCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/StartDeviceLoggingCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/SwipeArcCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/SwipeArcCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/SwipeCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/SwipeCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/TouchAction_MoveToCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/TouchAction_MoveToCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/TouchAction_MoveToElementCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/TouchAction_PressElementCommand.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import sys
 import json
 
 from testwizard.commands_core import CommandBase
 from testwizard.commands_core.SimpleResult import SimpleResult
 
 
-class TouchAction_MoveToElementCommand(CommandBase):
+class TouchAction_PressElementCommand(CommandBase):
     def __init__(self, testObject):
         CommandBase.__init__(
-            self, testObject, "Mobile.TouchAction_MoveToElement")
+            self, testObject, "Mobile.TouchAction_PressElement")
 
     def execute(self, selector):
         requestObj = [selector]
 
         result = self.executeCommand(requestObj)
 
-        return SimpleResult(result, "TouchAction_MoveToElement was successful", "TouchAction_MoveToElement failed")
+        return SimpleResult(result, "TouchAction_PressElement was successful", "TouchAction_PressElement failed")
```

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/TouchAction_NewCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/TouchAction_NewCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/TouchAction_PerformCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/TouchAction_PerformCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/TouchAction_PressCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/TouchAction_PressCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/TouchAction_PressElementCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/TouchAction_TapCommand.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import sys
 import json
 
 from testwizard.commands_core import CommandBase
 from testwizard.commands_core.SimpleResult import SimpleResult
 
 
-class TouchAction_PressElementCommand(CommandBase):
+class TouchAction_TapCommand(CommandBase):
     def __init__(self, testObject):
-        CommandBase.__init__(
-            self, testObject, "Mobile.TouchAction_PressElement")
+        CommandBase.__init__(self, testObject, "Mobile.TouchAction_Tap")
 
-    def execute(self, selector):
-        requestObj = [selector]
+    def execute(self, x, y):
+        requestObj = [x, y]
 
         result = self.executeCommand(requestObj)
 
-        return SimpleResult(result, "TouchAction_PressElement was successful", "TouchAction_PressElement failed")
+        return SimpleResult(result, "TouchAction_Tap was successful", "TouchAction_Tap failed")
```

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/TouchAction_ReleaseCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/TouchAction_ReleaseCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/TouchAction_WaitCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/TouchAction_WaitCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/WaitForElementCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/WaitForElementCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/ZoomCoordinatesCommand.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/ZoomCoordinatesCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard/commands_mobile/__init__.py` & `testwizard.commands-mobile-3.8.1b4810/testwizard/commands_mobile/__init__.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard.commands_mobile.egg-info/PKG-INFO` & `testwizard.commands-mobile-3.8.1b4810/testwizard.commands_mobile.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.commands-mobile
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard Mobile commands
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

### Comparing `testwizard.commands-mobile-3.8.1b4749/testwizard.commands_mobile.egg-info/SOURCES.txt` & `testwizard.commands-mobile-3.8.1b4810/testwizard.commands_mobile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

