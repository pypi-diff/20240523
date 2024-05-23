# Comparing `tmp/testwizard.commands-web-3.8.1b4749.tar.gz` & `tmp/testwizard.commands-web-3.8.1b4810.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testwizard.commands-web-3.8.1b4749.tar", last modified: Tue Mar 19 15:01:44 2024, max compression
+gzip compressed data, was "testwizard.commands-web-3.8.1b4810.tar", last modified: Wed Mar 27 12:56:31 2024, max compression
```

## Comparing `testwizard.commands-web-3.8.1b4749.tar` & `testwizard.commands-web-3.8.1b4810.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:44.414905 testwizard.commands-web-3.8.1b4749/
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/LICENSE.txt
--rw-rw-rw-   0        0        0      537 2024-03-19 15:01:44.414905 testwizard.commands-web-3.8.1b4749/PKG-INFO
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/README.md
--rw-rw-rw-   0        0        0       42 2024-03-19 15:01:44.414905 testwizard.commands-web-3.8.1b4749/setup.cfg
--rw-rw-rw-   0        0        0      813 2024-03-19 15:01:44.000000 testwizard.commands-web-3.8.1b4749/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:44.368033 testwizard.commands-web-3.8.1b4749/testwizard/
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:44.414905 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/
--rw-rw-rw-   0        0        0      526 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/AcceptAlertCommand.py
--rw-rw-rw-   0        0        0      506 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/AddArgumentCommand.py
--rw-rw-rw-   0        0        0      518 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/AddCapabilityCommand.py
--rw-rw-rw-   0        0        0      527 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/AddChromeExtensionCommand.py
--rw-rw-rw-   0        0        0      592 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/AuthenticateUrlCommand.py
--rw-rw-rw-   0        0        0      520 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/ClearCommand.py
--rw-rw-rw-   0        0        0      520 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/ClickCommand.py
--rw-rw-rw-   0        0        0      603 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/CloseWindowCommand.py
--rw-rw-rw-   0        0        0      546 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/DeleteAllCookiesCommand.py
--rw-rw-rw-   0        0        0      530 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/DismissAlertCommand.py
--rw-rw-rw-   0        0        0      580 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/DragNDropCommand.py
--rw-rw-rw-   0        0        0      518 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/ExitFullScreenCommand.py
--rw-rw-rw-   0        0        0      490 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/GetChildrenCommand.py
--rw-rw-rw-   0        0        0      603 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/GetChildrenResult.py
--rw-rw-rw-   0        0        0      549 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/GetCurrentWindowHandleCommand.py
--rw-rw-rw-   0        0        0      554 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/GetCurrentWindowHandleResult.py
--rw-rw-rw-   0        0        0      558 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/GetElementAttributeCommand.py
--rw-rw-rw-   0        0        0      545 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/GetElementAttributeResult.py
--rw-rw-rw-   0        0        0      483 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/GetElementCommand.py
--rw-rw-rw-   0        0        0      717 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/GetElementResult.py
--rw-rw-rw-   0        0        0      437 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/GetUrlCommand.py
--rw-rw-rw-   0        0        0      528 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/GetUrlResult.py
--rw-rw-rw-   0        0        0      507 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/GetWindowHandlesCommand.py
--rw-rw-rw-   0        0        0      606 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/GetWindowHandlesResult.py
--rw-rw-rw-   0        0        0      518 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/GoToUrlCommand.py
--rw-rw-rw-   0        0        0      538 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/IsDriverLoadedCommand.py
--rw-rw-rw-   0        0        0      538 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MaximizeWindowCommand.py
--rw-rw-rw-   0        0        0      591 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_ClickAndHoldCommand.py
--rw-rw-rw-   0        0        0      568 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_ClickCommand.py
--rw-rw-rw-   0        0        0      596 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_ContextClickCommand.py
--rw-rw-rw-   0        0        0      592 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_DoubleClickCommand.py
--rw-rw-rw-   0        0        0      636 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_DragAndDropCommand.py
--rw-rw-rw-   0        0        0      696 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_DragAndDropToOffsetCommand.py
--rw-rw-rw-   0        0        0      600 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_MoveToElementCommand.py
--rw-rw-rw-   0        0        0      660 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_MoveToElementOffsetCommand.py
--rw-rw-rw-   0        0        0      542 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_NewCommand.py
--rw-rw-rw-   0        0        0      558 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_PerformCommand.py
--rw-rw-rw-   0        0        0      654 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_ReleaseCommand.py
--rw-rw-rw-   0        0        0      680 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_SendKeysCommand.py
--rw-rw-rw-   0        0        0      652 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_keyDownCommand.py
--rw-rw-rw-   0        0        0      644 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_keyUpCommand.py
--rw-rw-rw-   0        0        0      548 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/OpenInNewTabCommand.py
--rw-rw-rw-   0        0        0      491 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/OpenInNewWindowCommand.py
--rw-rw-rw-   0        0        0      516 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/OpenInNewWindowResult.py
--rw-rw-rw-   0        0        0      522 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/QuitDriverCommand.py
--rw-rw-rw-   0        0        0      495 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/ScreenshotBMPCommand.py
--rw-rw-rw-   0        0        0      602 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/ScreenshotJPGCommand.py
--rw-rw-rw-   0        0        0      522 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/ScreenshotResult.py
--rw-rw-rw-   0        0        0      524 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/ScrollByCommand.py
--rw-rw-rw-   0        0        0      592 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SendKeyboardShortcutCommand.py
--rw-rw-rw-   0        0        0      544 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SendKeysAlertCommand.py
--rw-rw-rw-   0        0        0      544 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SendKeysCommand.py
--rw-rw-rw-   0        0        0      672 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/StartWebDriverCommand.py
--rw-rw-rw-   0        0        0      569 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/StartWebDriverResult.py
--rw-rw-rw-   0        0        0      524 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SubmitCommand.py
--rw-rw-rw-   0        0        0      550 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SwitchToDefaultContentCommand.py
--rw-rw-rw-   0        0        0      538 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SwitchToFirstWindowCommand.py
--rw-rw-rw-   0        0        0      559 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SwitchToFrameCommand.py
--rw-rw-rw-   0        0        0      648 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SwitchToFullScreenCommand.py
--rw-rw-rw-   0        0        0      534 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SwitchToLastWindowCommand.py
--rw-rw-rw-   0        0        0      642 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SwitchToNewWindowCommand.py
--rw-rw-rw-   0        0        0      534 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SwitchToNextWindowCommand.py
--rw-rw-rw-   0        0        0      565 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SwitchToParentFrameCommand.py
--rw-rw-rw-   0        0        0      550 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SwitchToPreviousWindowCommand.py
--rw-rw-rw-   0        0        0      560 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SwitchToWindowCommand.py
--rw-rw-rw-   0        0        0      574 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/WaitForControlCommand.py
--rw-rw-rw-   0        0        0        0 2024-03-19 15:00:53.000000 testwizard.commands-web-3.8.1b4749/testwizard/commands_web/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:44.383655 testwizard.commands-web-3.8.1b4749/testwizard.commands_web.egg-info/
--rw-rw-rw-   0        0        0      537 2024-03-19 15:01:44.000000 testwizard.commands-web-3.8.1b4749/testwizard.commands_web.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3616 2024-03-19 15:01:44.000000 testwizard.commands-web-3.8.1b4749/testwizard.commands_web.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 15:01:44.000000 testwizard.commands-web-3.8.1b4749/testwizard.commands_web.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-03-19 15:01:44.000000 testwizard.commands-web-3.8.1b4749/testwizard.commands_web.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-19 15:01:44.000000 testwizard.commands-web-3.8.1b4749/testwizard.commands_web.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:31.506721 testwizard.commands-web-3.8.1b4810/
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/LICENSE.txt
+-rw-rw-rw-   0        0        0      537 2024-03-27 12:56:31.506721 testwizard.commands-web-3.8.1b4810/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-27 12:56:31.506721 testwizard.commands-web-3.8.1b4810/setup.cfg
+-rw-rw-rw-   0        0        0      813 2024-03-27 12:56:31.000000 testwizard.commands-web-3.8.1b4810/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:31.459847 testwizard.commands-web-3.8.1b4810/testwizard/
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:31.506721 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/
+-rw-rw-rw-   0        0        0      526 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/AcceptAlertCommand.py
+-rw-rw-rw-   0        0        0      506 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/AddArgumentCommand.py
+-rw-rw-rw-   0        0        0      518 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/AddCapabilityCommand.py
+-rw-rw-rw-   0        0        0      527 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/AddChromeExtensionCommand.py
+-rw-rw-rw-   0        0        0      592 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/AuthenticateUrlCommand.py
+-rw-rw-rw-   0        0        0      520 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/ClearCommand.py
+-rw-rw-rw-   0        0        0      520 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/ClickCommand.py
+-rw-rw-rw-   0        0        0      603 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/CloseWindowCommand.py
+-rw-rw-rw-   0        0        0      546 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/DeleteAllCookiesCommand.py
+-rw-rw-rw-   0        0        0      530 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/DismissAlertCommand.py
+-rw-rw-rw-   0        0        0      580 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/DragNDropCommand.py
+-rw-rw-rw-   0        0        0      518 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/ExitFullScreenCommand.py
+-rw-rw-rw-   0        0        0      490 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/GetChildrenCommand.py
+-rw-rw-rw-   0        0        0      603 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/GetChildrenResult.py
+-rw-rw-rw-   0        0        0      549 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/GetCurrentWindowHandleCommand.py
+-rw-rw-rw-   0        0        0      554 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/GetCurrentWindowHandleResult.py
+-rw-rw-rw-   0        0        0      558 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/GetElementAttributeCommand.py
+-rw-rw-rw-   0        0        0      545 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/GetElementAttributeResult.py
+-rw-rw-rw-   0        0        0      483 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/GetElementCommand.py
+-rw-rw-rw-   0        0        0      717 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/GetElementResult.py
+-rw-rw-rw-   0        0        0      437 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/GetUrlCommand.py
+-rw-rw-rw-   0        0        0      528 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/GetUrlResult.py
+-rw-rw-rw-   0        0        0      507 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/GetWindowHandlesCommand.py
+-rw-rw-rw-   0        0        0      606 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/GetWindowHandlesResult.py
+-rw-rw-rw-   0        0        0      518 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/GoToUrlCommand.py
+-rw-rw-rw-   0        0        0      538 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/IsDriverLoadedCommand.py
+-rw-rw-rw-   0        0        0      538 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MaximizeWindowCommand.py
+-rw-rw-rw-   0        0        0      591 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_ClickAndHoldCommand.py
+-rw-rw-rw-   0        0        0      568 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_ClickCommand.py
+-rw-rw-rw-   0        0        0      596 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_ContextClickCommand.py
+-rw-rw-rw-   0        0        0      592 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_DoubleClickCommand.py
+-rw-rw-rw-   0        0        0      636 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_DragAndDropCommand.py
+-rw-rw-rw-   0        0        0      696 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_DragAndDropToOffsetCommand.py
+-rw-rw-rw-   0        0        0      600 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_MoveToElementCommand.py
+-rw-rw-rw-   0        0        0      660 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_MoveToElementOffsetCommand.py
+-rw-rw-rw-   0        0        0      542 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_NewCommand.py
+-rw-rw-rw-   0        0        0      558 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_PerformCommand.py
+-rw-rw-rw-   0        0        0      654 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_ReleaseCommand.py
+-rw-rw-rw-   0        0        0      680 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_SendKeysCommand.py
+-rw-rw-rw-   0        0        0      652 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_keyDownCommand.py
+-rw-rw-rw-   0        0        0      644 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_keyUpCommand.py
+-rw-rw-rw-   0        0        0      548 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/OpenInNewTabCommand.py
+-rw-rw-rw-   0        0        0      491 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/OpenInNewWindowCommand.py
+-rw-rw-rw-   0        0        0      516 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/OpenInNewWindowResult.py
+-rw-rw-rw-   0        0        0      522 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/QuitDriverCommand.py
+-rw-rw-rw-   0        0        0      495 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/ScreenshotBMPCommand.py
+-rw-rw-rw-   0        0        0      602 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/ScreenshotJPGCommand.py
+-rw-rw-rw-   0        0        0      522 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/ScreenshotResult.py
+-rw-rw-rw-   0        0        0      524 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/ScrollByCommand.py
+-rw-rw-rw-   0        0        0      592 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SendKeyboardShortcutCommand.py
+-rw-rw-rw-   0        0        0      544 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SendKeysAlertCommand.py
+-rw-rw-rw-   0        0        0      544 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SendKeysCommand.py
+-rw-rw-rw-   0        0        0      672 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/StartWebDriverCommand.py
+-rw-rw-rw-   0        0        0      569 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/StartWebDriverResult.py
+-rw-rw-rw-   0        0        0      524 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SubmitCommand.py
+-rw-rw-rw-   0        0        0      550 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SwitchToDefaultContentCommand.py
+-rw-rw-rw-   0        0        0      538 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SwitchToFirstWindowCommand.py
+-rw-rw-rw-   0        0        0      559 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SwitchToFrameCommand.py
+-rw-rw-rw-   0        0        0      648 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SwitchToFullScreenCommand.py
+-rw-rw-rw-   0        0        0      534 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SwitchToLastWindowCommand.py
+-rw-rw-rw-   0        0        0      642 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SwitchToNewWindowCommand.py
+-rw-rw-rw-   0        0        0      534 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SwitchToNextWindowCommand.py
+-rw-rw-rw-   0        0        0      565 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SwitchToParentFrameCommand.py
+-rw-rw-rw-   0        0        0      550 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SwitchToPreviousWindowCommand.py
+-rw-rw-rw-   0        0        0      560 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SwitchToWindowCommand.py
+-rw-rw-rw-   0        0        0      574 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/WaitForControlCommand.py
+-rw-rw-rw-   0        0        0        0 2024-03-27 12:55:37.000000 testwizard.commands-web-3.8.1b4810/testwizard/commands_web/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:31.475469 testwizard.commands-web-3.8.1b4810/testwizard.commands_web.egg-info/
+-rw-rw-rw-   0        0        0      537 2024-03-27 12:56:31.000000 testwizard.commands-web-3.8.1b4810/testwizard.commands_web.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3616 2024-03-27 12:56:31.000000 testwizard.commands-web-3.8.1b4810/testwizard.commands_web.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-27 12:56:31.000000 testwizard.commands-web-3.8.1b4810/testwizard.commands_web.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-03-27 12:56:31.000000 testwizard.commands-web-3.8.1b4810/testwizard.commands_web.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-03-27 12:56:31.000000 testwizard.commands-web-3.8.1b4810/testwizard.commands_web.egg-info/top_level.txt
```

### Comparing `testwizard.commands-web-3.8.1b4749/PKG-INFO` & `testwizard.commands-web-3.8.1b4810/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.commands-web
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard Web commands
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

### Comparing `testwizard.commands-web-3.8.1b4749/setup.py` & `testwizard.commands-web-3.8.1b4810/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="testwizard.commands-web",
-    version="3.8.1b4749",
+    version="3.8.1b4810",
     author="Resillion",
     author_email="testwizard-support@resillion.com",
     description="Testwizard Web commands",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.resillion.com/services/software-testing/testing-tools/testwizard/",
     packages=['testwizard.commands_web'],
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

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/AcceptAlertCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/AcceptAlertCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/AddCapabilityCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/AddCapabilityCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/AddChromeExtensionCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/AddChromeExtensionCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/AuthenticateUrlCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/AuthenticateUrlCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/ClearCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/ClearCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/ClickCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/ClickCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/CloseWindowCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/CloseWindowCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/DeleteAllCookiesCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/DeleteAllCookiesCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/DismissAlertCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/DismissAlertCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/DragNDropCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/DragNDropCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/ExitFullScreenCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/ExitFullScreenCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/GetChildrenResult.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/GetChildrenResult.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/GetCurrentWindowHandleCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/GetCurrentWindowHandleCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/GetCurrentWindowHandleResult.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/GetCurrentWindowHandleResult.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/GetElementAttributeCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/GetElementAttributeCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/GetElementAttributeResult.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/GetElementAttributeResult.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/GetElementResult.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/GetElementResult.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/GetUrlResult.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/GetUrlResult.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/GetWindowHandlesResult.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/GetWindowHandlesResult.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/GoToUrlCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/GoToUrlCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/IsDriverLoadedCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/IsDriverLoadedCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MaximizeWindowCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MaximizeWindowCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_ClickAndHoldCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_ClickAndHoldCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_ClickCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_ClickCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_ContextClickCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_ContextClickCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_DoubleClickCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_DoubleClickCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_DragAndDropCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_DragAndDropCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_DragAndDropToOffsetCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_DragAndDropToOffsetCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_MoveToElementCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_MoveToElementCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_MoveToElementOffsetCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_MoveToElementOffsetCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_NewCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_NewCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_PerformCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_PerformCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_ReleaseCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_ReleaseCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_SendKeysCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_SendKeysCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_keyDownCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_keyDownCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/MultiAction_keyUpCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/MultiAction_keyUpCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/OpenInNewTabCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/OpenInNewTabCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/OpenInNewWindowResult.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/OpenInNewWindowResult.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/QuitDriverCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/QuitDriverCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/ScreenshotJPGCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/ScreenshotJPGCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/ScreenshotResult.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/ScreenshotResult.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/ScrollByCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/ScrollByCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SendKeyboardShortcutCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SendKeyboardShortcutCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SendKeysAlertCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SendKeysAlertCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SendKeysCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SendKeysCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/StartWebDriverCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/StartWebDriverCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/StartWebDriverResult.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/StartWebDriverResult.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SubmitCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SubmitCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SwitchToDefaultContentCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SwitchToDefaultContentCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SwitchToFirstWindowCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SwitchToFirstWindowCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SwitchToFrameCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SwitchToFrameCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SwitchToFullScreenCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SwitchToFullScreenCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SwitchToLastWindowCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SwitchToLastWindowCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SwitchToNewWindowCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SwitchToNewWindowCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SwitchToNextWindowCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SwitchToNextWindowCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SwitchToParentFrameCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SwitchToParentFrameCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SwitchToPreviousWindowCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SwitchToPreviousWindowCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/SwitchToWindowCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/SwitchToWindowCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard/commands_web/WaitForControlCommand.py` & `testwizard.commands-web-3.8.1b4810/testwizard/commands_web/WaitForControlCommand.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard.commands_web.egg-info/PKG-INFO` & `testwizard.commands-web-3.8.1b4810/testwizard.commands_web.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.commands-web
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard Web commands
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

### Comparing `testwizard.commands-web-3.8.1b4749/testwizard.commands_web.egg-info/SOURCES.txt` & `testwizard.commands-web-3.8.1b4810/testwizard.commands_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

