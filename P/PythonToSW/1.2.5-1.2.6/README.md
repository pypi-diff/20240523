# Comparing `tmp/PythonToSW-1.2.5.tar.gz` & `tmp/PythonToSW-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonToSW-1.2.5.tar", last modified: Sun May 19 10:58:28 2024, max compression
+gzip compressed data, was "PythonToSW-1.2.6.tar", last modified: Thu May 23 14:49:40 2024, max compression
```

## Comparing `PythonToSW-1.2.5.tar` & `PythonToSW-1.2.6.tar`

### file list

```diff
@@ -1,108 +1,107 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 10:58:28.137231 PythonToSW-1.2.5/
--rw-rw-rw-   0        0        0    11558 2024-01-17 15:06:42.000000 PythonToSW-1.2.5/LICENSE
--rw-rw-rw-   0        0        0       92 2024-05-15 22:14:52.000000 PythonToSW-1.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1865 2024-05-19 10:58:28.135735 PythonToSW-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     1242 2024-05-16 22:19:42.000000 PythonToSW-1.2.5/README.md
--rw-rw-rw-   0        0        0        5 2024-05-19 10:57:13.000000 PythonToSW-1.2.5/VERSION
--rw-rw-rw-   0        0        0       62 2024-05-16 22:06:47.000000 PythonToSW-1.2.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 10:58:28.137231 PythonToSW-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0     2072 2024-05-19 10:58:18.000000 PythonToSW-1.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:58:27.996763 PythonToSW-1.2.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-19 10:58:28.008403 PythonToSW-1.2.5/src/PythonToSW/
--rw-rw-rw-   0        0        0     6348 2024-05-17 09:46:54.000000 PythonToSW-1.2.5/src/PythonToSW/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:58:28.036634 PythonToSW-1.2.5/src/PythonToSW/addon/
--rw-rw-rw-   0        0        0      315 2024-05-16 03:46:54.000000 PythonToSW-1.2.5/src/PythonToSW/addon/playlist.xml
--rw-rw-rw-   0        0        0   161117 2024-05-16 21:57:12.000000 PythonToSW-1.2.5/src/PythonToSW/addon/script.lua
--rw-rw-rw-   0        0        0    21012 2024-05-17 07:34:55.000000 PythonToSW-1.2.5/src/PythonToSW/addon.py
--rw-rw-rw-   0        0        0     3176 2024-05-17 07:31:58.000000 PythonToSW-1.2.5/src/PythonToSW/event.py
--rw-rw-rw-   0        0        0     1247 2024-05-17 03:19:53.000000 PythonToSW-1.2.5/src/PythonToSW/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:58:28.133464 PythonToSW-1.2.5/src/PythonToSW/executions/
--rw-rw-rw-   0        0        0     2809 2024-05-14 23:36:22.000000 PythonToSW-1.2.5/src/PythonToSW/executions/__createExecution.py
--rw-rw-rw-   0        0        0     1732 2024-05-17 09:47:00.000000 PythonToSW-1.2.5/src/PythonToSW/executions/__generateImportCode.py
--rw-rw-rw-   0        0        0     3893 2024-05-17 09:47:29.000000 PythonToSW-1.2.5/src/PythonToSW/executions/__init__.py
--rw-rw-rw-   0        0        0     1059 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/addAdmin.py
--rw-rw-rw-   0        0        0     1056 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/addAuth.py
--rw-rw-rw-   0        0        0     1216 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/addMapLabel.py
--rw-rw-rw-   0        0        0     1220 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/addMapLine.py
--rw-rw-rw-   0        0        0     1582 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/addMapObject.py
--rw-rw-rw-   0        0        0     1107 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/announce.py
--rw-rw-rw-   0        0        0     1027 2024-05-14 23:48:22.000000 PythonToSW-1.2.5/src/PythonToSW/executions/cancelGerstner.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/clearOilSpills.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/clearRadiation.py
--rw-rw-rw-   0        0        0     1025 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/clearVehicles.py
--rw-rw-rw-   0        0        0     1106 2024-05-14 23:49:23.000000 PythonToSW-1.2.5/src/PythonToSW/executions/despawnObject.py
--rw-rw-rw-   0        0        0     1111 2024-05-14 23:49:25.000000 PythonToSW-1.2.5/src/PythonToSW/executions/despawnVehicle.py
--rw-rw-rw-   0        0        0     1123 2024-05-14 23:49:26.000000 PythonToSW-1.2.5/src/PythonToSW/executions/despawnVehicleGroup.py
--rw-rw-rw-   0        0        0     1025 2024-05-16 04:08:52.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getAddonIndex.py
--rw-rw-rw-   0        0        0     1105 2024-05-14 18:26:42.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getCharacterItem.py
--rw-rw-rw-   0        0        0     1018 2024-05-15 22:28:57.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getCurrency.py
--rw-rw-rw-   0        0        0     1031 2024-05-16 22:21:02.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getGameSettings.py
--rw-rw-rw-   0        0        0     1079 2024-05-14 18:24:19.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getObjectData.py
--rw-rw-rw-   0        0        0     1092 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getPlayerCharacter.py
--rw-rw-rw-   0        0        0     1103 2024-05-16 00:01:47.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getPlayerLookDirection.py
--rw-rw-rw-   0        0        0     1075 2024-05-16 00:01:47.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getPlayerName.py
--rw-rw-rw-   0        0        0     1072 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getPlayerPos.py
--rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getPlayers.py
--rw-rw-rw-   0        0        0     1035 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getSeasonalEvent.py
--rw-rw-rw-   0        0        0     1017 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getUniqueID.py
--rw-rw-rw-   0        0        0     1138 2024-05-14 23:44:48.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleBatteryByName.py
--rw-rw-rw-   0        0        0     1172 2024-05-14 23:44:45.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleBatteryByVoxel.py
--rw-rw-rw-   0        0        0     1102 2024-05-14 18:30:01.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleComponents.py
--rw-rw-rw-   0        0        0     1084 2024-05-14 18:29:46.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleData.py
--rw-rw-rw-   0        0        0     1083 2024-05-15 22:28:49.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleGroup.py
--rw-rw-rw-   0        0        0     1162 2024-05-15 22:08:55.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getVehiclePos.py
--rw-rw-rw-   0        0        0     1123 2024-05-14 23:44:59.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleTankByName.py
--rw-rw-rw-   0        0        0     1163 2024-05-14 23:45:28.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleTankByVoxel.py
--rw-rw-rw-   0        0        0     1012 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/isAridDLC.py
--rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/isSpaceDLC.py
--rw-rw-rw-   0        0        0     1021 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/isWeaponsDLC.py
--rw-rw-rw-   0        0        0     1080 2024-05-16 00:01:47.000000 PythonToSW-1.2.5/src/PythonToSW/executions/moveGroup.py
--rw-rw-rw-   0        0        0     1093 2024-05-16 00:01:47.000000 PythonToSW-1.2.5/src/PythonToSW/executions/moveGroupSafe.py
--rw-rw-rw-   0        0        0     1090 2024-05-16 00:01:47.000000 PythonToSW-1.2.5/src/PythonToSW/executions/moveVehicle.py
--rw-rw-rw-   0        0        0     1103 2024-05-16 00:02:01.000000 PythonToSW-1.2.5/src/PythonToSW/executions/moveVehicleSafe.py
--rw-rw-rw-   0        0        0     1135 2024-05-14 23:47:34.000000 PythonToSW-1.2.5/src/PythonToSW/executions/notify.py
--rw-rw-rw-   0        0        0     1068 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/removeAdmin.py
--rw-rw-rw-   0        0        0     1065 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/removeAuth.py
--rw-rw-rw-   0        0        0     1097 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/removeMapLabel.py
--rw-rw-rw-   0        0        0     1094 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/removeMapLine.py
--rw-rw-rw-   0        0        0     1100 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/removeMapObject.py
--rw-rw-rw-   0        0        0     1087 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/removePopup.py
--rw-rw-rw-   0        0        0     1171 2024-05-14 18:25:00.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setCharacterData.py
--rw-rw-rw-   0        0        0     1222 2024-05-14 18:26:10.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setCharacterItem.py
--rw-rw-rw-   0        0        0     1120 2024-05-14 18:25:27.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setCharacterTooltip.py
--rw-rw-rw-   0        0        0     1115 2024-05-14 23:49:29.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setCreatureMoveTarget.py
--rw-rw-rw-   0        0        0     1115 2024-05-15 22:28:48.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setCurrency.py
--rw-rw-rw-   0        0        0     1120 2024-05-16 22:20:48.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setGameSetting.py
--rw-rw-rw-   0        0        0     1100 2024-05-16 00:01:49.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setGroupPosSafe.py
--rw-rw-rw-   0        0        0     1089 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setOilSpill.py
--rw-rw-rw-   0        0        0     1088 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setPlayerPos.py
--rw-rw-rw-   0        0        0     1299 2024-05-14 18:18:44.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setPopup.py
--rw-rw-rw-   0        0        0     1161 2024-05-14 23:43:28.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleBatteryByName.py
--rw-rw-rw-   0        0        0     1194 2024-05-14 23:42:27.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleBatteryByVoxel.py
--rw-rw-rw-   0        0        0     1126 2024-05-14 23:39:49.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleEditable.py
--rw-rw-rw-   0        0        0     1146 2024-05-14 23:39:47.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleInvulnerable.py
--rw-rw-rw-   0        0        0     1097 2024-05-15 22:08:43.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setVehiclePos.py
--rw-rw-rw-   0        0        0     1110 2024-05-16 00:01:47.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setVehiclePosSafe.py
--rw-rw-rw-   0        0        0     1123 2024-05-14 23:39:52.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleShowOnMap.py
--rw-rw-rw-   0        0        0     1146 2024-05-14 23:43:54.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleTankByName.py
--rw-rw-rw-   0        0        0     1186 2024-05-14 23:44:14.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleTankByVoxel.py
--rw-rw-rw-   0        0        0     1122 2024-05-16 04:03:12.000000 PythonToSW-1.2.5/src/PythonToSW/executions/spawnAddonVehicle.py
--rw-rw-rw-   0        0        0     1095 2024-05-14 23:46:38.000000 PythonToSW-1.2.5/src/PythonToSW/executions/spawnCharacter.py
--rw-rw-rw-   0        0        0     1143 2024-05-14 23:47:06.000000 PythonToSW-1.2.5/src/PythonToSW/executions/spawnCreature.py
--rw-rw-rw-   0        0        0     1157 2024-05-16 04:03:12.000000 PythonToSW-1.2.5/src/PythonToSW/executions/spawnEquipment.py
--rw-rw-rw-   0        0        0     1099 2024-05-14 23:47:30.000000 PythonToSW-1.2.5/src/PythonToSW/executions/spawnExplosion.py
--rw-rw-rw-   0        0        0     1128 2024-05-14 23:46:36.000000 PythonToSW-1.2.5/src/PythonToSW/executions/spawnMeteor.py
--rw-rw-rw-   0        0        0     1147 2024-05-14 23:45:56.000000 PythonToSW-1.2.5/src/PythonToSW/executions/spawnMeteorShower.py
--rw-rw-rw-   0        0        0     1090 2024-05-16 04:03:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/spawnObject.py
--rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:58.000000 PythonToSW-1.2.5/src/PythonToSW/executions/spawnTsunami.py
--rw-rw-rw-   0        0        0     1089 2024-05-16 04:03:12.000000 PythonToSW-1.2.5/src/PythonToSW/executions/spawnVehicle.py
--rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:54.000000 PythonToSW-1.2.5/src/PythonToSW/executions/spawnVolcano.py
--rw-rw-rw-   0        0        0     1099 2024-05-14 23:45:59.000000 PythonToSW-1.2.5/src/PythonToSW/executions/spawnWhirlpool.py
--rw-rw-rw-   0        0        0     2688 2024-05-17 07:20:38.000000 PythonToSW-1.2.5/src/PythonToSW/helpers.py
--rw-rw-rw-   0        0        0     2157 2024-05-17 07:25:51.000000 PythonToSW-1.2.5/src/PythonToSW/matrix.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:58:28.134240 PythonToSW-1.2.5/src/PythonToSW.egg-info/
--rw-rw-rw-   0        0        0     1865 2024-05-19 10:58:27.000000 PythonToSW-1.2.5/src/PythonToSW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4065 2024-05-19 10:58:27.000000 PythonToSW-1.2.5/src/PythonToSW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 10:58:27.000000 PythonToSW-1.2.5/src/PythonToSW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-05-19 10:58:27.000000 PythonToSW-1.2.5/src/PythonToSW.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-19 10:58:27.000000 PythonToSW-1.2.5/src/PythonToSW.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 14:49:40.085612 PythonToSW-1.2.6/
+-rw-rw-rw-   0        0        0    11558 2024-01-17 15:06:42.000000 PythonToSW-1.2.6/LICENSE
+-rw-rw-rw-   0        0        0       92 2024-05-15 22:14:52.000000 PythonToSW-1.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1865 2024-05-23 14:49:40.084117 PythonToSW-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1242 2024-05-16 22:19:42.000000 PythonToSW-1.2.6/README.md
+-rw-rw-rw-   0        0        0        5 2024-05-23 14:49:06.000000 PythonToSW-1.2.6/VERSION
+-rw-rw-rw-   0        0        0       62 2024-05-16 22:06:47.000000 PythonToSW-1.2.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 14:49:40.086359 PythonToSW-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     2072 2024-05-19 10:58:18.000000 PythonToSW-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:49:39.879594 PythonToSW-1.2.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 14:49:39.894243 PythonToSW-1.2.6/src/PythonToSW/
+-rw-rw-rw-   0        0        0     6314 2024-05-23 14:47:30.000000 PythonToSW-1.2.6/src/PythonToSW/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:49:39.941706 PythonToSW-1.2.6/src/PythonToSW/addon/
+-rw-rw-rw-   0        0        0      315 2024-05-16 03:46:54.000000 PythonToSW-1.2.6/src/PythonToSW/addon/playlist.xml
+-rw-rw-rw-   0        0        0   161117 2024-05-16 21:57:12.000000 PythonToSW-1.2.6/src/PythonToSW/addon/script.lua
+-rw-rw-rw-   0        0        0    24588 2024-05-23 14:48:55.000000 PythonToSW-1.2.6/src/PythonToSW/addon.py
+-rw-rw-rw-   0        0        0     3176 2024-05-17 07:31:58.000000 PythonToSW-1.2.6/src/PythonToSW/event.py
+-rw-rw-rw-   0        0        0     1247 2024-05-17 03:19:53.000000 PythonToSW-1.2.6/src/PythonToSW/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:49:40.080704 PythonToSW-1.2.6/src/PythonToSW/executions/
+-rw-rw-rw-   0        0        0     2818 2024-05-23 14:37:19.000000 PythonToSW-1.2.6/src/PythonToSW/executions/__createExecution.py
+-rw-rw-rw-   0        0        0     1732 2024-05-17 09:47:00.000000 PythonToSW-1.2.6/src/PythonToSW/executions/__generateImportCode.py
+-rw-rw-rw-   0        0        0     1068 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/addAdmin.py
+-rw-rw-rw-   0        0        0     1065 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/addAuth.py
+-rw-rw-rw-   0        0        0     1225 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/addMapLabel.py
+-rw-rw-rw-   0        0        0     1229 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/addMapLine.py
+-rw-rw-rw-   0        0        0     1591 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/addMapObject.py
+-rw-rw-rw-   0        0        0     1116 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/announce.py
+-rw-rw-rw-   0        0        0     1036 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/cancelGerstner.py
+-rw-rw-rw-   0        0        0     1037 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/clearOilSpills.py
+-rw-rw-rw-   0        0        0     1037 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/clearRadiation.py
+-rw-rw-rw-   0        0        0     1034 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/clearVehicles.py
+-rw-rw-rw-   0        0        0     1115 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/despawnObject.py
+-rw-rw-rw-   0        0        0     1120 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/despawnVehicle.py
+-rw-rw-rw-   0        0        0     1132 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/despawnVehicleGroup.py
+-rw-rw-rw-   0        0        0     1034 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/getAddonIndex.py
+-rw-rw-rw-   0        0        0     1114 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/getCharacterItem.py
+-rw-rw-rw-   0        0        0     1027 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/getCurrency.py
+-rw-rw-rw-   0        0        0     1040 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/getGameSettings.py
+-rw-rw-rw-   0        0        0     1088 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/getObjectData.py
+-rw-rw-rw-   0        0        0     1101 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/getPlayerCharacter.py
+-rw-rw-rw-   0        0        0     1112 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/getPlayerLookDirection.py
+-rw-rw-rw-   0        0        0     1084 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/getPlayerName.py
+-rw-rw-rw-   0        0        0     1081 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/getPlayerPos.py
+-rw-rw-rw-   0        0        0     1024 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/getPlayers.py
+-rw-rw-rw-   0        0        0     1044 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/getSeasonalEvent.py
+-rw-rw-rw-   0        0        0     1026 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/getUniqueID.py
+-rw-rw-rw-   0        0        0     1147 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/getVehicleBatteryByName.py
+-rw-rw-rw-   0        0        0     1181 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/getVehicleBatteryByVoxel.py
+-rw-rw-rw-   0        0        0     1111 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/getVehicleComponents.py
+-rw-rw-rw-   0        0        0     1093 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/getVehicleData.py
+-rw-rw-rw-   0        0        0     1092 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/getVehicleGroup.py
+-rw-rw-rw-   0        0        0     1171 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/getVehiclePos.py
+-rw-rw-rw-   0        0        0     1132 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/getVehicleTankByName.py
+-rw-rw-rw-   0        0        0     1172 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/getVehicleTankByVoxel.py
+-rw-rw-rw-   0        0        0     1021 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/isAridDLC.py
+-rw-rw-rw-   0        0        0     1024 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/isSpaceDLC.py
+-rw-rw-rw-   0        0        0     1030 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/isWeaponsDLC.py
+-rw-rw-rw-   0        0        0     1089 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/moveGroup.py
+-rw-rw-rw-   0        0        0     1102 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/moveGroupSafe.py
+-rw-rw-rw-   0        0        0     1099 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/moveVehicle.py
+-rw-rw-rw-   0        0        0     1112 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/moveVehicleSafe.py
+-rw-rw-rw-   0        0        0     1144 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/notify.py
+-rw-rw-rw-   0        0        0     1077 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/removeAdmin.py
+-rw-rw-rw-   0        0        0     1074 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/removeAuth.py
+-rw-rw-rw-   0        0        0     1106 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/removeMapLabel.py
+-rw-rw-rw-   0        0        0     1103 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/removeMapLine.py
+-rw-rw-rw-   0        0        0     1109 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/removeMapObject.py
+-rw-rw-rw-   0        0        0     1096 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/removePopup.py
+-rw-rw-rw-   0        0        0     1180 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/setCharacterData.py
+-rw-rw-rw-   0        0        0     1231 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/setCharacterItem.py
+-rw-rw-rw-   0        0        0     1129 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/setCharacterTooltip.py
+-rw-rw-rw-   0        0        0     1124 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/setCreatureMoveTarget.py
+-rw-rw-rw-   0        0        0     1124 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/setCurrency.py
+-rw-rw-rw-   0        0        0     1129 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/setGameSetting.py
+-rw-rw-rw-   0        0        0     1109 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/setGroupPosSafe.py
+-rw-rw-rw-   0        0        0     1098 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/setOilSpill.py
+-rw-rw-rw-   0        0        0     1097 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/setPlayerPos.py
+-rw-rw-rw-   0        0        0     1308 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/setPopup.py
+-rw-rw-rw-   0        0        0     1170 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/setVehicleBatteryByName.py
+-rw-rw-rw-   0        0        0     1203 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/setVehicleBatteryByVoxel.py
+-rw-rw-rw-   0        0        0     1135 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/setVehicleEditable.py
+-rw-rw-rw-   0        0        0     1155 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/setVehicleInvulnerable.py
+-rw-rw-rw-   0        0        0     1106 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/setVehiclePos.py
+-rw-rw-rw-   0        0        0     1119 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/setVehiclePosSafe.py
+-rw-rw-rw-   0        0        0     1132 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/setVehicleShowOnMap.py
+-rw-rw-rw-   0        0        0     1155 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/setVehicleTankByName.py
+-rw-rw-rw-   0        0        0     1195 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/setVehicleTankByVoxel.py
+-rw-rw-rw-   0        0        0     1131 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/spawnAddonVehicle.py
+-rw-rw-rw-   0        0        0     1104 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/spawnCharacter.py
+-rw-rw-rw-   0        0        0     1152 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/spawnCreature.py
+-rw-rw-rw-   0        0        0     1166 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/spawnEquipment.py
+-rw-rw-rw-   0        0        0     1108 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/spawnExplosion.py
+-rw-rw-rw-   0        0        0     1137 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/spawnMeteor.py
+-rw-rw-rw-   0        0        0     1156 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/spawnMeteorShower.py
+-rw-rw-rw-   0        0        0     1099 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/spawnObject.py
+-rw-rw-rw-   0        0        0     1102 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/spawnTsunami.py
+-rw-rw-rw-   0        0        0     1098 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/spawnVehicle.py
+-rw-rw-rw-   0        0        0     1102 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/spawnVolcano.py
+-rw-rw-rw-   0        0        0     1108 2024-05-23 14:21:46.000000 PythonToSW-1.2.6/src/PythonToSW/executions/spawnWhirlpool.py
+-rw-rw-rw-   0        0        0     2688 2024-05-17 07:20:38.000000 PythonToSW-1.2.6/src/PythonToSW/helpers.py
+-rw-rw-rw-   0        0        0     2157 2024-05-17 07:25:51.000000 PythonToSW-1.2.6/src/PythonToSW/matrix.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:49:40.082454 PythonToSW-1.2.6/src/PythonToSW.egg-info/
+-rw-rw-rw-   0        0        0     1865 2024-05-23 14:49:39.000000 PythonToSW-1.2.6/src/PythonToSW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4027 2024-05-23 14:49:39.000000 PythonToSW-1.2.6/src/PythonToSW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 14:49:39.000000 PythonToSW-1.2.6/src/PythonToSW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-23 14:49:39.000000 PythonToSW-1.2.6/src/PythonToSW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-23 14:49:39.000000 PythonToSW-1.2.6/src/PythonToSW.egg-info/top_level.txt
```

### Comparing `PythonToSW-1.2.5/LICENSE` & `PythonToSW-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.5/PKG-INFO` & `PythonToSW-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToSW
-Version: 1.2.5
+Version: 1.2.6
 Summary: A package that allows you to create addons in Stormworks with Python, handled through HTTP.
 Author: Cuh4
 License: Apache License 2.0
 Project-URL: Source code, https://github.com/cuh4/PythonToSW
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
```

### Comparing `PythonToSW-1.2.5/README.md` & `PythonToSW-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.5/setup.py` & `PythonToSW-1.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.5/src/PythonToSW/__init__.py` & `PythonToSW-1.2.6/src/PythonToSW/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,21 +23,20 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
 # Main
 from PythonToSW.event import Event
-from PythonToSW.addon import Addon
+from PythonToSW.addon import Addon, BaseExecution
 from PythonToSW import exceptions
 from PythonToSW import helpers
 from PythonToSW import matrix
 
 # Executions
-from PythonToSW.executions import BaseExecution
 from PythonToSW.executions.addAdmin import AddAdmin
 from PythonToSW.executions.addAuth import AddAuth
 from PythonToSW.executions.addMapLabel import AddMapLabel
 from PythonToSW.executions.addMapLine import AddMapLine
 from PythonToSW.executions.addMapObject import AddMapObject
 from PythonToSW.executions.announce import Announce
 from PythonToSW.executions.cancelGerstner import CancelGerstner
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/addon/script.lua` & `PythonToSW-1.2.6/src/PythonToSW/addon/script.lua`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.5/src/PythonToSW/addon.py` & `PythonToSW-1.2.6/src/PythonToSW/addon.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,35 +20,38 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
+from __future__ import annotations
 import os
 import flask
 import flask.cli
 import json
 import threading
 import logging
 import werkzeug
 import werkzeug.utils
 import colorama
 from datetime import datetime
+from uuid import uuid4
+import time
 
-from . import helpers
-from . import exceptions
-from . import executions
-from . import Event
+from PythonToSW import helpers
+from PythonToSW import exceptions
+from PythonToSW import Event
 
 # ---- // Main
 colorama.init()
 
 class Addon():
-    """
+    # raw string to prevent "SyntaxWarning: invalid escape sequence '\S'" from %appdata% part
+    r"""
     A class that represents a Stormworks addon.
     
     >>> import PythonToSW as PTS
     >>> addon = PTS.Addon("MyAddon", port = 3000)
     >>>
     >>> def main():
     >>>     addon.execute(PTS.Announce("Server", "Hello World", -1))
@@ -71,15 +74,15 @@
         self.addonName = addonName
         self.port = port
         self.app = flask.Flask(__name__)
         self.running = False
         self.allowLogging = allowLogging
         self.addonPath = os.path.join(os.path.dirname(__file__), "addon")
         self.destinationAddonPath = destinationAddonPath
-        self.pendingExecutions: dict[str, executions.BaseExecution] = {}
+        self.pendingExecutions: dict[str, BaseExecution] = {}
         self.callbacks: dict[str, Event] = {}
         
         self.playlistEncoded = self._parsePlaylist()
         self.script = self._parseScript()
         self.vehicles: list[str] = []
         
         # check if paths exist
@@ -146,28 +149,28 @@
         # send startup message
         self.log(f"{self.addonName} (addon) has started, listening on port {self.port}. Create a save with your addon enabled in Stormworks and keep this running.")
         
         # start server
         threading.Thread(target = target).start()
         self.app.run(host = "127.0.0.1", port = self.port, threaded = True)
         
-    def execute(self, execution: executions.BaseExecution):
+    def execute(self, execution: BaseExecution):
         """
         Sends an execution to the in-game addon.
         
         >>> import PythonToSW as PTS
         >>> addon = PTS.Addon("MyAddon", port = 3000)
         >>>
         >>> def main():
         >>>     addon.execute(PTS.Announce("Server", "Hello World", -1)) # Sends a message to everyone
         >>>
         >>> addon.start(target = main)
         
         Args:
-            execution: (executions.BaseExecution) The execution to send.
+            execution: (BaseExecution) The execution to send.
             
         Raises:
             exceptions.FailedExecutionAttempt: Raised if the addon is not running, or if an execution with the same ID already exists.
         """
 
         # check if addon is running
         if not self.running:
@@ -190,33 +193,33 @@
         
         # remove execution now that its complete
         self.removePendingExecution(execution.ID)
         
         # return
         return returnValues
     
-    def getPendingExecution(self, executionID: str) -> executions.BaseExecution|None:
+    def getPendingExecution(self, executionID: str) -> BaseExecution|None:
         """
         Returns the pending execution with the given ID.
         
         Args:
             executionID: (str) The ID of the execution to return.
             
         Returns:
-            (executions.BaseExecution|None) The pending execution with the given ID, or None if it doesn't exist.
+            (BaseExecution|None) The pending execution with the given ID, or None if it doesn't exist.
         """
 
         return self.getPendingExecutions().get(executionID)
         
-    def getPendingExecutions(self) -> dict[str, executions.BaseExecution]:
+    def getPendingExecutions(self) -> dict[str, BaseExecution]:
         """
         Returns the pending executions.
         
         Returns:
-            (dict[str, executions.BaseExecution]) The pending executions, with the keys being the execution IDs.
+            (dict[str, BaseExecution]) The pending executions, with the keys being the execution IDs.
         """
 
         return self.pendingExecutions.copy()
     
     def removePendingExecution(self, executionID: str):
         """
         Removes the pending execution with the given ID.
@@ -559,8 +562,121 @@
         helpers.quickWrite(os.path.join(destinationPath, "script.lua"), self.script)
         
         # add vehicles to addon directory
         for vehicle in self.vehicles:
             vehicleID = vehicle["vehicleID"]
             content = helpers.quickRead(vehicle["path"])
             
-            helpers.quickWrite(os.path.join(destinationPath, f"vehicle_{vehicleID}"), content)
+            helpers.quickWrite(os.path.join(destinationPath, f"vehicle_{vehicleID}"), content)
+            
+class BaseExecution():
+    """
+    Represents an execution that can be sent to the in-game addon.
+
+    You never really need to use this directly. If there is an in-game
+    function that doesn't have an execution, create an execution that
+    inherits from this. Example:
+    
+    >>> class MoveGroup(BaseExecution):
+    >>>     def __init__(self, group_id: int, pos: list):
+    >>>         super().__init__(
+    >>>             functionName = "moveGroup",
+    >>>             arguments = [group_id, pos]
+    >>>         )
+    
+    Args:
+        functionName: (str) The name of the in-game function to call
+        arguments: (list) The arguments to pass to the in-game function
+    """
+
+    def __init__(self, functionName: str, arguments: list = []):
+        self.ID = str(uuid4())
+        self.functionName = functionName
+        self.arguments = arguments
+        
+        self.handled = False
+        self.returnValues = []
+        self.isWaiting = False
+        
+    def __str__(self):
+        return f"Execution-{self.ID} ({self.functionName})"
+    
+    def execute(self, addon: Addon) -> list:
+        """
+        Send this execution to the in-game addon.
+        Equivalent to: addon.execute(self)
+        
+        Args:
+            addon: (Addon) The addon to send this execution to.
+            
+        Returns:
+            (list) The return values from the in-game function call.
+
+        Raises:
+            exceptions.FailedExecutionAttempt: Raised if the addon is not running, or if an execution with the same ID already exists.
+        """
+
+        return addon.execute(self)
+        
+    def _toDict(self):
+        """
+        Converts this execution into a dictionary that can be sent to the addon
+        
+        Returns:
+            (dict) The dictionary representation of this execution
+        """
+
+        return {
+            "ID" : self.ID,
+            "functionName": self.functionName,
+            "arguments": self.arguments,
+            "handled": self.handled
+        }
+        
+    def _return(self, returnValues: list):
+        """
+        Marks this execution as handled and saves return values.
+        
+        Args:
+            returnValues: (list) The return values from the in-game function.
+            
+        Raises:
+            exceptions.InternalError: Raised if this method is called when the execution is already handled.
+        """
+
+        if self.handled:
+            raise exceptions.InternalError("Tried to return after already returning")
+        
+        self.handled = True
+        self.returnValues = returnValues
+    
+    def _halt(self):
+        """
+        Stops waiting on this execution via _wait() method.
+        """
+
+        self.isWaiting = False
+        
+    def _obsolete(self):
+        """
+        Returns whether this execution has been handled.
+        
+        Returns:
+            (bool) Whether this execution has been handled.
+        """
+
+        return not self.isWaiting
+        
+    def _wait(self) -> list:
+        """
+        Waits until this execution has been handled and returns the return values.
+        
+        Returns:
+            (list) The return values from the in-game function call.
+        """
+
+        self.isWaiting = True
+        
+        while not self.handled and self.isWaiting:
+            time.sleep(0.01)
+            
+        return self.returnValues
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/event.py` & `PythonToSW-1.2.6/src/PythonToSW/event.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.5/src/PythonToSW/exceptions.py` & `PythonToSW-1.2.6/src/PythonToSW/exceptions.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/__createExecution.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/__createExecution.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,13 +75,13 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 \"\"\"
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
 {generated}"""
 
     file.write(main)
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/__generateImportCode.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/__generateImportCode.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/addAdmin.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/addAuth.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Add Admin
+# [PythonToSW] Add Auth
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class AddAdmin(BaseExecution):
+class AddAuth(BaseExecution):
     def __init__(self, peer_id: int):
         super().__init__(
-            functionName = "addAdmin",
+            functionName = "addAuth",
             arguments = [peer_id]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/addAuth.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/removeAuth.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Add Auth
+# [PythonToSW] Remove Auth
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class AddAuth(BaseExecution):
+class RemoveAuth(BaseExecution):
     def __init__(self, peer_id: int):
         super().__init__(
-            functionName = "addAuth",
+            functionName = "removeAuth",
             arguments = [peer_id]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/addMapLabel.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/addMapLabel.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 from .. import matrix
 
 # ---- // Main
 class AddMapLabel(BaseExecution):
     def __init__(self, peer_id: int, ui_id: int, label_type: int, label: str, pos: list):
         x, _, z = matrix.getXYZ(pos)
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/addMapLine.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/addMapLine.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
 class AddMapLine(BaseExecution):
     def __init__(self, peer_id: int, ui_id: int, startPos: list, endPos: list, width: int, r: int = 255, g: int = 255, b: int = 255, a: int = 255):
         super().__init__(
             functionName = "addMapLine",
             arguments = [peer_id, ui_id, startPos, endPos, width, r, g, b, a]
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/addMapObject.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/addMapObject.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 from .. import matrix
 
 # ---- // Main
 class AddMapObject(BaseExecution):
     def __init__(self, peer_id: int, ui_id: int, label: str, hoverLabel: str, radius: int|float, positionType: int, markerType: int, pos: list, relativePos: list = matrix.new(0, 0, 0), vehicle_id: int = 0, object_id: int = 0, r: int = 255, g: int = 255, b: int = 255, a: int = 255):
         globalX, _, globalZ = matrix.getXYZ(pos)
         localX, _, localZ = matrix.getXYZ(relativePos)
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/announce.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/getPlayerPos.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Announce
+# [PythonToSW] Get Player Pos
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class Announce(BaseExecution):
-    def __init__(self, author: str, message: str, peer_id: int = -1):
+class GetPlayerPos(BaseExecution):
+    def __init__(self, peer_id: int):
         super().__init__(
-            functionName = "announce",
-            arguments = [author, message, peer_id]
+            functionName = "getPlayerPos",
+            arguments = [peer_id]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/cancelGerstner.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/cancelGerstner.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
 class CancelGerstner(BaseExecution):
     def __init__(self):
         super().__init__(
             functionName = "cancelGerstner"
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/clearOilSpills.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/isWeaponsDLC.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Clear Oil Spills
+# [PythonToSW] Is Weapons DLC
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,15 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class ClearOilSpills(BaseExecution):
+class IsWeaponsDLC(BaseExecution):
     def __init__(self):
         super().__init__(
-            functionName = "clearOilSpill",
+            functionName = "dlcWeapons",
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/clearRadiation.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/clearRadiation.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
 class ClearRadiation(BaseExecution):
     def __init__(self):
         super().__init__(
             functionName = "clearRadiation",
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/clearVehicles.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/clearVehicles.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
 class ClearVehicles(BaseExecution):
     def __init__(self):
         super().__init__(
             functionName = "cleanVehicles",
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/despawnObject.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/despawnObject.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
 class DespawnObject(BaseExecution):
     def __init__(self, object_id: int, isInstant: bool):
         super().__init__(
             functionName = "despawnObject",
             arguments = [object_id, isInstant]
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/despawnVehicle.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/despawnVehicleGroup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Despawn Vehicle
+# [PythonToSW] Despawn Vehicle Group
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class DespawnVehicle(BaseExecution):
-    def __init__(self, vehicle_id: int, isInstant: bool):
+class DespawnVehicleGroup(BaseExecution):
+    def __init__(self, group_id: int, isInstant: bool):
         super().__init__(
-            functionName = "despawnVehicle",
-            arguments = [vehicle_id, isInstant]
+            functionName = "despawnVehicleGroup",
+            arguments = [group_id, isInstant]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/despawnVehicleGroup.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/despawnVehicle.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Despawn Vehicle Group
+# [PythonToSW] Despawn Vehicle
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class DespawnVehicleGroup(BaseExecution):
-    def __init__(self, group_id: int, isInstant: bool):
+class DespawnVehicle(BaseExecution):
+    def __init__(self, vehicle_id: int, isInstant: bool):
         super().__init__(
-            functionName = "despawnVehicleGroup",
-            arguments = [group_id, isInstant]
+            functionName = "despawnVehicle",
+            arguments = [vehicle_id, isInstant]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/getAddonIndex.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/getUniqueID.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Get Addon Index
+# [PythonToSW] Get Unique ID
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,15 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class GetAddonIndex(BaseExecution):
+class GetUniqueID(BaseExecution):
     def __init__(self):
         super().__init__(
-            functionName = "getAddonIndex"
+            functionName = "getMapID",
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/getCharacterItem.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/getObjectData.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Get Character Item
+# [PythonToSW] Get Object Data
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class GetCharacterItem(BaseExecution):
-    def __init__(self, object_id: int, slot: int):
+class GetObjectData(BaseExecution):
+    def __init__(self, object_id: int):
         super().__init__(
-            functionName = "getCharacterItem",
-            arguments = [object_id, slot]
+            functionName = "getObjectData",
+            arguments = [object_id]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/getCurrency.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/getPlayerName.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Get Currency
+# [PythonToSW] Get Player Name
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,15 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class GetCurrency(BaseExecution):
-    def __init__(self):
+class GetPlayerName(BaseExecution):
+    def __init__(self, peer_id: int):
         super().__init__(
-            functionName = "getCurrency"
+            functionName = "getPlayerName",
+            arguments = [peer_id]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/getGameSettings.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/setVehiclePos.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Get Game Settings
+# [PythonToSW] Set Vehicle Pos
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,15 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class GetGameSettings(BaseExecution):
-    def __init__(self):
+class SetVehiclePos(BaseExecution):
+    def __init__(self, vehicle_id: int, pos: list):
         super().__init__(
-            functionName = "getGameSettings"
+            functionName = "setVehiclePos",
+            arguments = [vehicle_id, pos]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/getObjectData.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/moveVehicleSafe.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Get Object Data
+# [PythonToSW] Move Vehicle Safe
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class GetObjectData(BaseExecution):
-    def __init__(self, object_id: int):
+class MoveVehicleSafe(BaseExecution):
+    def __init__(self, vehicle_id: int, pos: list):
         super().__init__(
-            functionName = "getObjectData",
-            arguments = [object_id]
+            functionName = "moveVehicleSafe",
+            arguments = [vehicle_id, pos]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/getPlayerCharacter.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/setPlayerPos.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Get Player Character
+# [PythonToSW] Set Player Pos
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class GetPlayerCharacter(BaseExecution):
-    def __init__(self, peer_id: int):
+class SetPlayerPos(BaseExecution):
+    def __init__(self, peer_id: int, pos: list):
         super().__init__(
-            functionName = "getPlayerCharacterID",
-            arguments = [peer_id]
+            functionName = "setPlayerPos",
+            arguments = [peer_id, pos]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/getPlayerLookDirection.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/getPlayers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Get Player Look Direction
+# [PythonToSW] Get Players
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class GetPlayerLookDirection(BaseExecution):
-    def __init__(self, peer_id: int):
+class GetPlayers(BaseExecution):
+    def __init__(self):
         super().__init__(
-            functionName = "getPlayerLookDirection",
-            arguments = [peer_id]
+            functionName = "getPlayers"
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/getPlayerName.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/setVehicleBatteryByVoxel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Get Player Name
+# [PythonToSW] Set Vehicle Battery By Voxel
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class GetPlayerName(BaseExecution):
-    def __init__(self, peer_id: int):
+class SetVehicleBatteryByName(BaseExecution):
+    def __init__(self, vehicle_id: int, voxelX: int, voxelY: int, voxelZ: int, amount: float):
         super().__init__(
-            functionName = "getPlayerName",
-            arguments = [peer_id]
+            functionName = "setVehicleBattery",
+            arguments = [vehicle_id, voxelX, voxelY, voxelZ, amount]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/getPlayerPos.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/spawnMeteor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Get Player Pos
+# [PythonToSW] Spawn Meteor
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class GetPlayerPos(BaseExecution):
-    def __init__(self, peer_id: int):
+class SpawnMeteor(BaseExecution):
+    def __init__(self, pos: list, magnitude: float, isSpawnTsunami: bool):
         super().__init__(
-            functionName = "getPlayerPos",
-            arguments = [peer_id]
+            functionName = "spawnMeteor",
+            arguments = [pos, magnitude, isSpawnTsunami]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/getPlayers.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/spawnMeteorShower.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Get Players
+# [PythonToSW] Spawn Meteor Shower
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,15 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class GetPlayers(BaseExecution):
-    def __init__(self):
+class SpawnMeteorShower(BaseExecution):
+    def __init__(self, pos: list, magnitude: float, isSpawnTsunami: bool):
         super().__init__(
-            functionName = "getPlayers"
+            functionName = "spawnMeteorShower",
+            arguments = [pos, magnitude, isSpawnTsunami]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/getSeasonalEvent.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/setOilSpill.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Get Seasonal Event
+# [PythonToSW] Set Oil Spill
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,15 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class GetSeasonalEvent(BaseExecution):
-    def __init__(self):
+class SetOilSpill(BaseExecution):
+    def __init__(self, pos: list, amount: int|float):
         super().__init__(
-            functionName = "getSeasonalEvent",
+            functionName = "setOilSpill",
+            arguments = [pos, amount]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/getUniqueID.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/setVehiclePosSafe.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Get Unique ID
+# [PythonToSW] Set Vehicle Pos Safe
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,15 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class GetUniqueID(BaseExecution):
-    def __init__(self):
+class SetVehiclePosSafe(BaseExecution):
+    def __init__(self, vehicle_id: int, pos: list):
         super().__init__(
-            functionName = "getMapID",
+            functionName = "setVehiclePosSafe",
+            arguments = [vehicle_id, pos]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleBatteryByName.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/getVehicleTankByName.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Get Vehicle Battery By Name
+# [PythonToSW] Get Vehicle Tank By Name
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class GetVehicleBatteryByName(BaseExecution):
-    def __init__(self, vehicle_id: int, batteryName: str):
+class GetVehicleTankByName(BaseExecution):
+    def __init__(self, vehicle_id: int, tankName: str):
         super().__init__(
-            functionName = "getVehicleBattery",
-            arguments = [vehicle_id, batteryName]
+            functionName = "getVehicleTank",
+            arguments = [vehicle_id, tankName]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleBatteryByVoxel.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/getVehicleBatteryByVoxel.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
 class GetVehicleBatteryByVoxel(BaseExecution):
     def __init__(self, vehicle_id: int, voxelX: int, voxelY: int, voxelZ: int):
         super().__init__(
             functionName = "getVehicleBattery",
             arguments = [vehicle_id, voxelX, voxelY, voxelZ]
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleComponents.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/getVehicleComponents.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
 class GetVehicleComponents(BaseExecution):
     def __init__(self, vehicle_id: int):
         super().__init__(
             functionName = "getVehicleComponents",
             arguments = [vehicle_id]
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleData.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/spawnCharacter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Get Vehicle Data
+# [PythonToSW] Spawn Character
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class GetVehicleData(BaseExecution):
-    def __init__(self, vehicle_id: int):
+class SpawnCharacter(BaseExecution):
+    def __init__(self, pos: list, outfitID: int):
         super().__init__(
-            functionName = "getVehicleData",
-            arguments = [vehicle_id]
+            functionName = "spawnCharacter",
+            arguments = [pos, outfitID]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleGroup.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/getGameSettings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Get Vehicle Group
+# [PythonToSW] Get Game Settings
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class GetVehicleGroup(BaseExecution):
-    def __init__(self, group_id: int):
+class GetGameSettings(BaseExecution):
+    def __init__(self):
         super().__init__(
-            functionName = "getVehicleGroup",
-            arguments = [group_id]
+            functionName = "getGameSettings"
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/getVehiclePos.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/getVehicleData.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Get Vehicle Pos
+# [PythonToSW] Get Vehicle Data
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class GetVehiclePos(BaseExecution):
-    def __init__(self, vehicle_id: int, voxel_x: int = 0, voxel_y: int = 0, voxel_z: int = 0):
+class GetVehicleData(BaseExecution):
+    def __init__(self, vehicle_id: int):
         super().__init__(
-            functionName = "getVehiclePos",
-            arguments = [vehicle_id, voxel_x, voxel_y, voxel_z]
+            functionName = "getVehicleData",
+            arguments = [vehicle_id]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleTankByName.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/getVehicleTankByVoxel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Get Vehicle Tank By Name
+# [PythonToSW] Get Vehicle Tank By Voxel
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class GetVehicleTankByName(BaseExecution):
-    def __init__(self, vehicle_id: int, tankName: str):
+class GetVehicleTankByVoxel(BaseExecution):
+    def __init__(self, vehicle_id: int, voxelX: int, voxelY: int, voxelZ: int):
         super().__init__(
             functionName = "getVehicleTank",
-            arguments = [vehicle_id, tankName]
+            arguments = [vehicle_id, voxelX, voxelY, voxelZ]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleTankByVoxel.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/setVehicleTankByVoxel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Get Vehicle Tank By Voxel
+# [PythonToSW] Set Vehicle Tank By Voxel
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class GetVehicleTankByVoxel(BaseExecution):
-    def __init__(self, vehicle_id: int, voxelX: int, voxelY: int, voxelZ: int):
+class SetVehicleTankByVoxel(BaseExecution):
+    def __init__(self, vehicle_id: int, voxelX: int, voxelY: int, voxelZ: int, amount: float):
         super().__init__(
-            functionName = "getVehicleTank",
-            arguments = [vehicle_id, voxelX, voxelY, voxelZ]
+            functionName = "setVehicleTank",
+            arguments = [vehicle_id, voxelX, voxelY, voxelZ, amount]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/isAridDLC.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/isAridDLC.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
 class IsAridDLC(BaseExecution):
     def __init__(self):
         super().__init__(
             functionName = "dlcArid",
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/isSpaceDLC.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/isSpaceDLC.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
 class IsSpaceDLC(BaseExecution):
     def __init__(self):
         super().__init__(
             functionName = "dlcSpace",
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/isWeaponsDLC.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/moveGroup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Is Weapons DLC
+# [PythonToSW] Move Group
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,15 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class IsWeaponsDLC(BaseExecution):
-    def __init__(self):
+class MoveGroup(BaseExecution):
+    def __init__(self, group_id: int, pos: list):
         super().__init__(
-            functionName = "dlcWeapons",
+            functionName = "moveGroup",
+            arguments = [group_id, pos]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/moveGroup.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/moveGroupSafe.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Move Group
+# [PythonToSW] Move Group Safe
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class MoveGroup(BaseExecution):
+class MoveGroupSafe(BaseExecution):
     def __init__(self, group_id: int, pos: list):
         super().__init__(
-            functionName = "moveGroup",
+            functionName = "moveGroupSafe",
             arguments = [group_id, pos]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/moveGroupSafe.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/clearOilSpills.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Move Group Safe
+# [PythonToSW] Clear Oil Spills
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class MoveGroupSafe(BaseExecution):
-    def __init__(self, group_id: int, pos: list):
+class ClearOilSpills(BaseExecution):
+    def __init__(self):
         super().__init__(
-            functionName = "moveGroupSafe",
-            arguments = [group_id, pos]
+            functionName = "clearOilSpill",
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/moveVehicle.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/spawnVehicle.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Move Vehicle
+# [PythonToSW] Spawn Vehicle
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class MoveVehicle(BaseExecution):
-    def __init__(self, vehicle_id: int, pos: list):
+class SpawnVehicle(BaseExecution):
+    def __init__(self, pos: list, saveName: str):
         super().__init__(
-            functionName = "moveVehicle",
-            arguments = [vehicle_id, pos]
+            functionName = "spawnVehicle",
+            arguments = [pos, saveName]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/moveVehicleSafe.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/setVehicleTankByName.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Move Vehicle Safe
+# [PythonToSW] Set Vehicle Tank By Name
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class MoveVehicleSafe(BaseExecution):
-    def __init__(self, vehicle_id: int, pos: list):
+class SetVehicleTankByName(BaseExecution):
+    def __init__(self, vehicle_id: int, tankName: str, amount: float):
         super().__init__(
-            functionName = "moveVehicleSafe",
-            arguments = [vehicle_id, pos]
+            functionName = "setVehicleTank",
+            arguments = [vehicle_id, tankName, amount]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/notify.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/notify.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
 class Notify(BaseExecution):
     def __init__(self, peer_id: int, title: str, message: str, notificationType: int):
         super().__init__(
             functionName = "notify",
             arguments = [peer_id, title, message, notificationType]
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/removeAdmin.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/getAddonIndex.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Remove Admin
+# [PythonToSW] Get Addon Index
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class RemoveAdmin(BaseExecution):
-    def __init__(self, peer_id: int):
+class GetAddonIndex(BaseExecution):
+    def __init__(self):
         super().__init__(
-            functionName = "removeAdmin",
-            arguments = [peer_id]
+            functionName = "getAddonIndex"
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/removeAuth.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/removeMapLine.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Remove Auth
+# [PythonToSW] Remove Map Line
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class RemoveAuth(BaseExecution):
-    def __init__(self, peer_id: int):
+class RemoveMapLine(BaseExecution):
+    def __init__(self, peer_id: int, ui_id: int):
         super().__init__(
-            functionName = "removeAuth",
-            arguments = [peer_id]
+            functionName = "removeMapLine",
+            arguments = [peer_id, ui_id]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/removeMapLabel.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/removeMapObject.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Remove Map Label
+# [PythonToSW] Remove Map Object
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class RemoveMapLabel(BaseExecution):
+class RemoveMapObject(BaseExecution):
     def __init__(self, peer_id: int, ui_id: int):
         super().__init__(
-            functionName = "removeMapLabel",
+            functionName = "removeMapObject",
             arguments = [peer_id, ui_id]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/removeMapLine.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/removePopup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Remove Map Line
+# [PythonToSW] Remove Popup
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class RemoveMapLine(BaseExecution):
+class RemovePopup(BaseExecution):
     def __init__(self, peer_id: int, ui_id: int):
         super().__init__(
-            functionName = "removeMapLine",
+            functionName = "removePopup",
             arguments = [peer_id, ui_id]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/removeMapObject.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/spawnObject.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Remove Map Object
+# [PythonToSW] Spawn Object
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class RemoveMapObject(BaseExecution):
-    def __init__(self, peer_id: int, ui_id: int):
+class SpawnObject(BaseExecution):
+    def __init__(self, pos: list, objectType: int):
         super().__init__(
-            functionName = "removeMapObject",
-            arguments = [peer_id, ui_id]
+            functionName = "spawnObject",
+            arguments = [pos, objectType]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/removePopup.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/getSeasonalEvent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Remove Popup
+# [PythonToSW] Get Seasonal Event
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class RemovePopup(BaseExecution):
-    def __init__(self, peer_id: int, ui_id: int):
+class GetSeasonalEvent(BaseExecution):
+    def __init__(self):
         super().__init__(
-            functionName = "removePopup",
-            arguments = [peer_id, ui_id]
+            functionName = "getSeasonalEvent",
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/setCharacterData.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/setCharacterData.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
 class SetCharacterData(BaseExecution):
     def __init__(self, object_id: int, health: int|float, isInteractable: bool, isAI: bool):
         super().__init__(
             functionName = "setCharacterData",
             arguments = [object_id, health, isInteractable, isAI]
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/setCharacterItem.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/setCharacterItem.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
 class SetCharacterItem(BaseExecution):
     def __init__(self, object_id: int, slot: int, equipmentID: int, active: bool, intValue: int = 0, floatValue: float = 0):
         super().__init__(
             functionName = "setCharacterItem",
             arguments = [object_id, slot, equipmentID, active, intValue, floatValue]
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/setCharacterTooltip.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/setCurrency.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Set Character Tooltip
+# [PythonToSW] Set Currency
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class SetCharacterTooltip(BaseExecution):
-    def __init__(self, object_id: int, tooltip: str):
+class SetCurrency(BaseExecution):
+    def __init__(self, money: int|float, research_points: int|float):
         super().__init__(
-            functionName = "setCharacterTooltip",
-            arguments = [object_id, tooltip]
+            functionName = "setCurrency",
+            arguments = [money, research_points]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/setCreatureMoveTarget.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/setCreatureMoveTarget.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
 class SetCreatureMoveTarget(BaseExecution):
     def __init__(self, object_id, pos: list):
         super().__init__(
             functionName = "setCreatureMoveTarget",
             arguments = [object_id, pos]
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/setCurrency.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/spawnExplosion.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Set Currency
+# [PythonToSW] Spawn Explosion
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class SetCurrency(BaseExecution):
-    def __init__(self, money: int|float, research_points: int|float):
+class SpawnExplosion(BaseExecution):
+    def __init__(self, pos: list, magnitude: float):
         super().__init__(
-            functionName = "setCurrency",
-            arguments = [money, research_points]
+            functionName = "spawnExplosion",
+            arguments = [pos, magnitude]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/setGameSetting.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/setGameSetting.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
 class SetGameSetting(BaseExecution):
     def __init__(self, gameSetting: str, value: str|bool|int|float):
         super().__init__(
             functionName = "setGameSetting",
             arguments = [gameSetting, value]
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/setGroupPosSafe.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/setGroupPosSafe.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
 class SetGroupPosSafe(BaseExecution):
     def __init__(self, group_id: int, pos: list):
         super().__init__(
             functionName = "setGroupPosSafe",
             arguments = [group_id, pos]
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/setOilSpill.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/spawnTsunami.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Set Oil Spill
+# [PythonToSW] Spawn Tsunami
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class SetOilSpill(BaseExecution):
-    def __init__(self, pos: list, amount: int|float):
+class SpawnTsunami(BaseExecution):
+    def __init__(self, pos: list, magnitude: float):
         super().__init__(
-            functionName = "setOilSpill",
-            arguments = [pos, amount]
+            functionName = "spawnTsunami",
+            arguments = [pos, magnitude]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/setPlayerPos.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/setPopup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Set Player Pos
+# [PythonToSW] Set Popup
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,17 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
+from .. import matrix
 
 # ---- // Main
-class SetPlayerPos(BaseExecution):
-    def __init__(self, peer_id: int, pos: list):
+class SetPopup(BaseExecution):
+    def __init__(self, peer_id: int, ui_id: int, visible: bool, text: str, pos: list, renderDistance: int, vehicleParentID: int = 0, objectParentID: int = 0):
         super().__init__(
-            functionName = "setPlayerPos",
-            arguments = [peer_id, pos]
+            functionName = "setPopup",
+            arguments = [peer_id, ui_id, "", visible, text, *matrix.getXYZ(pos), renderDistance, vehicleParentID, objectParentID]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/setPopup.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/setVehicleInvulnerable.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Set Popup
+# [PythonToSW] Set Vehicle Invulnerable
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,17 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
-from .. import matrix
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class SetPopup(BaseExecution):
-    def __init__(self, peer_id: int, ui_id: int, visible: bool, text: str, pos: list, renderDistance: int, vehicleParentID: int = 0, objectParentID: int = 0):
+class SetVehicleInvulnerable(BaseExecution):
+    def __init__(self, vehicle_id: int, isInvulnerable: bool):
         super().__init__(
-            functionName = "setPopup",
-            arguments = [peer_id, ui_id, "", visible, text, *matrix.getXYZ(pos), renderDistance, vehicleParentID, objectParentID]
+            functionName = "setVehicleInvulnerable",
+            arguments = [vehicle_id, isInvulnerable]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleBatteryByName.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/setVehicleBatteryByName.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
 class SetVehicleBatteryByName(BaseExecution):
     def __init__(self, vehicle_id: int, batteryName: str, amount: float):
         super().__init__(
             functionName = "setVehicleBattery",
             arguments = [vehicle_id, batteryName, amount]
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleBatteryByVoxel.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/setCharacterTooltip.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Set Vehicle Battery By Voxel
+# [PythonToSW] Set Character Tooltip
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class SetVehicleBatteryByName(BaseExecution):
-    def __init__(self, vehicle_id: int, voxelX: int, voxelY: int, voxelZ: int, amount: float):
+class SetCharacterTooltip(BaseExecution):
+    def __init__(self, object_id: int, tooltip: str):
         super().__init__(
-            functionName = "setVehicleBattery",
-            arguments = [vehicle_id, voxelX, voxelY, voxelZ, amount]
+            functionName = "setCharacterTooltip",
+            arguments = [object_id, tooltip]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleEditable.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/setVehicleEditable.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
 class SetVehicleEditable(BaseExecution):
     def __init__(self, vehicle_id: int, isEditable: bool):
         super().__init__(
             functionName = "setVehicleEditable",
             arguments = [vehicle_id, isEditable]
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleInvulnerable.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/spawnCreature.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Set Vehicle Invulnerable
+# [PythonToSW] Spawn Creature
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class SetVehicleInvulnerable(BaseExecution):
-    def __init__(self, vehicle_id: int, isInvulnerable: bool):
+class SpawnCreature(BaseExecution):
+    def __init__(self, pos: list, creatureType: int, sizeMultiplier: int|float):
         super().__init__(
-            functionName = "setVehicleInvulnerable",
-            arguments = [vehicle_id, isInvulnerable]
+            functionName = "spawnCreature",
+            arguments = [pos, creatureType, sizeMultiplier]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/setVehiclePos.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/spawnWhirlpool.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Set Vehicle Pos
+# [PythonToSW] Spawn Whirlpool
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class SetVehiclePos(BaseExecution):
-    def __init__(self, vehicle_id: int, pos: list):
+class SpawnWhirlpool(BaseExecution):
+    def __init__(self, pos: list, magnitude: float):
         super().__init__(
-            functionName = "setVehiclePos",
-            arguments = [vehicle_id, pos]
+            functionName = "spawnWhirlpool",
+            arguments = [pos, magnitude]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/setVehiclePosSafe.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/moveVehicle.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Set Vehicle Pos Safe
+# [PythonToSW] Move Vehicle
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class SetVehiclePosSafe(BaseExecution):
+class MoveVehicle(BaseExecution):
     def __init__(self, vehicle_id: int, pos: list):
         super().__init__(
-            functionName = "setVehiclePosSafe",
+            functionName = "moveVehicle",
             arguments = [vehicle_id, pos]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleShowOnMap.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/setVehicleShowOnMap.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
 class SetVehicleShowOnMap(BaseExecution):
     def __init__(self, vehicle_id: int, isShow: bool):
         super().__init__(
             functionName = "setVehicleShowOnMap",
             arguments = [vehicle_id, isShow]
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleTankByName.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/spawnVolcano.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Set Vehicle Tank By Name
+# [PythonToSW] Spawn Volcano
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class SetVehicleTankByName(BaseExecution):
-    def __init__(self, vehicle_id: int, tankName: str, amount: float):
+class SpawnVolcano(BaseExecution):
+    def __init__(self, pos: list, magnitude: float):
         super().__init__(
-            functionName = "setVehicleTank",
-            arguments = [vehicle_id, tankName, amount]
+            functionName = "spawnVolcano",
+            arguments = [pos, magnitude]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleTankByVoxel.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/getCurrency.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Set Vehicle Tank By Voxel
+# [PythonToSW] Get Currency
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class SetVehicleTankByVoxel(BaseExecution):
-    def __init__(self, vehicle_id: int, voxelX: int, voxelY: int, voxelZ: int, amount: float):
+class GetCurrency(BaseExecution):
+    def __init__(self):
         super().__init__(
-            functionName = "setVehicleTank",
-            arguments = [vehicle_id, voxelX, voxelY, voxelZ, amount]
+            functionName = "getCurrency"
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/spawnAddonVehicle.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/spawnAddonVehicle.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
 class SpawnAddonVehicle(BaseExecution):
     def __init__(self, pos: list, addonIndex: int, id: int):
         super().__init__(
             functionName = "spawnAddonVehicle",
             arguments = [pos, addonIndex, id]
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/spawnCharacter.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/getCharacterItem.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Spawn Character
+# [PythonToSW] Get Character Item
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class SpawnCharacter(BaseExecution):
-    def __init__(self, pos: list, outfitID: int):
+class GetCharacterItem(BaseExecution):
+    def __init__(self, object_id: int, slot: int):
         super().__init__(
-            functionName = "spawnCharacter",
-            arguments = [pos, outfitID]
+            functionName = "getCharacterItem",
+            arguments = [object_id, slot]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/spawnEquipment.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/spawnEquipment.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
 class SpawnEquipment(BaseExecution):
     def __init__(self, pos: list, equipmentID: int, intValue: int, floatValue: float):
         super().__init__(
             functionName = "spawnEquipment",
             arguments = [pos, equipmentID, intValue, floatValue]
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/spawnMeteorShower.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/getVehicleBatteryByName.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Spawn Meteor Shower
+# [PythonToSW] Get Vehicle Battery By Name
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class SpawnMeteorShower(BaseExecution):
-    def __init__(self, pos: list, magnitude: float, isSpawnTsunami: bool):
+class GetVehicleBatteryByName(BaseExecution):
+    def __init__(self, vehicle_id: int, batteryName: str):
         super().__init__(
-            functionName = "spawnMeteorShower",
-            arguments = [pos, magnitude, isSpawnTsunami]
+            functionName = "getVehicleBattery",
+            arguments = [vehicle_id, batteryName]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/spawnObject.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/announce.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Spawn Object
+# [PythonToSW] Announce
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class SpawnObject(BaseExecution):
-    def __init__(self, pos: list, objectType: int):
+class Announce(BaseExecution):
+    def __init__(self, author: str, message: str, peer_id: int = -1):
         super().__init__(
-            functionName = "spawnObject",
-            arguments = [pos, objectType]
+            functionName = "announce",
+            arguments = [author, message, peer_id]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/executions/spawnWhirlpool.py` & `PythonToSW-1.2.6/src/PythonToSW/executions/getVehicleGroup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Spawn Whirlpool
+# [PythonToSW] Get Vehicle Group
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -18,16 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from . import BaseExecution
+from PythonToSW import BaseExecution
 
 # ---- // Main
-class SpawnWhirlpool(BaseExecution):
-    def __init__(self, pos: list, magnitude: float):
+class GetVehicleGroup(BaseExecution):
+    def __init__(self, group_id: int):
         super().__init__(
-            functionName = "spawnWhirlpool",
-            arguments = [pos, magnitude]
+            functionName = "getVehicleGroup",
+            arguments = [group_id]
         )
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW/helpers.py` & `PythonToSW-1.2.6/src/PythonToSW/helpers.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.5/src/PythonToSW/matrix.py` & `PythonToSW-1.2.6/src/PythonToSW/matrix.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.5/src/PythonToSW.egg-info/PKG-INFO` & `PythonToSW-1.2.6/src/PythonToSW.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToSW
-Version: 1.2.5
+Version: 1.2.6
 Summary: A package that allows you to create addons in Stormworks with Python, handled through HTTP.
 Author: Cuh4
 License: Apache License 2.0
 Project-URL: Source code, https://github.com/cuh4/PythonToSW
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
```

### Comparing `PythonToSW-1.2.5/src/PythonToSW.egg-info/SOURCES.txt` & `PythonToSW-1.2.6/src/PythonToSW.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 src/PythonToSW.egg-info/dependency_links.txt
 src/PythonToSW.egg-info/requires.txt
 src/PythonToSW.egg-info/top_level.txt
 src/PythonToSW/addon/playlist.xml
 src/PythonToSW/addon/script.lua
 src/PythonToSW/executions/__createExecution.py
 src/PythonToSW/executions/__generateImportCode.py
-src/PythonToSW/executions/__init__.py
 src/PythonToSW/executions/addAdmin.py
 src/PythonToSW/executions/addAuth.py
 src/PythonToSW/executions/addMapLabel.py
 src/PythonToSW/executions/addMapLine.py
 src/PythonToSW/executions/addMapObject.py
 src/PythonToSW/executions/announce.py
 src/PythonToSW/executions/cancelGerstner.py
```

