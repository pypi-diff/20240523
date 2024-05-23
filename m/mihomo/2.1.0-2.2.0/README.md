# Comparing `tmp/mihomo-2.1.0.tar.gz` & `tmp/mihomo-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mihomo-2.1.0.tar", max compression
+gzip compressed data, was "mihomo-2.2.0.tar", max compression
```

## Comparing `mihomo-2.1.0.tar` & `mihomo-2.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1090 2023-06-01 05:14:24.496130 mihomo-2.1.0/LICENSE
--rw-r--r--   0        0        0       90 2023-06-07 08:41:32.652372 mihomo-2.1.0/mihomo/__init__.py
--rw-r--r--   0        0        0    11152 2024-02-07 11:37:57.477471 mihomo-2.1.0/mihomo/api.py
--rw-r--r--   0        0        0     2594 2024-02-07 11:24:38.190032 mihomo-2.1.0/mihomo/model.py
--rw-r--r--   0        0        0      479 2024-02-07 11:40:39.590450 mihomo-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      366 2024-02-06 13:37:45.700640 mihomo-2.1.0/README.md
--rw-r--r--   0        0        0     1166 1970-01-01 00:00:00.000000 mihomo-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-06-01 05:14:24.496130 mihomo-2.2.0/LICENSE
+-rw-r--r--   0        0        0       90 2023-06-07 08:41:32.652372 mihomo-2.2.0/mihomo/__init__.py
+-rw-r--r--   0        0        0    11229 2024-05-23 12:35:29.351454 mihomo-2.2.0/mihomo/api.py
+-rw-r--r--   0        0        0     2722 2024-05-23 12:35:33.779456 mihomo-2.2.0/mihomo/model.py
+-rw-r--r--   0        0        0      479 2024-05-23 12:41:33.511016 mihomo-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      366 2024-02-06 13:37:45.700640 mihomo-2.2.0/README.md
+-rw-r--r--   0        0        0     1166 1970-01-01 00:00:00.000000 mihomo-2.2.0/PKG-INFO
```

### Comparing `mihomo-2.1.0/LICENSE` & `mihomo-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mihomo-2.1.0/mihomo/api.py` & `mihomo-2.2.0/mihomo/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,17 +250,18 @@
             is_display=api_data.detailInfo.isDisplayAvatar,
         )
         if api_data.detailInfo.recordInfo:
             space_info = api_data.detailInfo.recordInfo
             if space_info:
                 if space_info.challengeInfo:
                     memory_info = MemoryInfo(
-                        level=space_info.challengeInfo.scheduleMaxLevel,
+                        level=space_info.challengeInfo.noneScheduleMaxLevel,
                         chaos_id=space_info.challengeInfo.scheduleGroupId,
-                        chaos_level=space_info.challengeInfo.noneScheduleMaxLevel,
+                        chaos_level=space_info.challengeInfo.abyssLevel,
+                        chaos_star_count=space_info.challengeInfo.abyssStarCount,
                     )
                 else:
                     memory_info = None
                 player_info.space_info = SpaceInfo(
                     memory_data=memory_info,
                     universe_level=space_info.maxRogueChallengeScore,
                     light_cone_count=space_info.equipmentCount,
```

### Comparing `mihomo-2.1.0/mihomo/model.py` & `mihomo-2.2.0/mihomo/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,25 +18,29 @@
     PT = "pt"
     RU = "ru"
     TH = "th"
     VI = "vi"
 
 
 class SpaceChallengeData(Struct):
-    scheduleMaxLevel: int = 0
     scheduleGroupId: Optional[int] = None
-    noneScheduleMaxLevel: Optional[int] = None
+    abyssLevel: int = 0
+    abyssStarCount: int = 0
+    noneScheduleMaxLevel: int = 0
 
 
 class SpaceData(Struct):
     challengeInfo: Optional[SpaceChallengeData] = None
     maxRogueChallengeScore: int = 0
-    equipmentCount: int = 0
     avatarCount: int = 0
+    equipmentCount: int = 0
+    relicCount: int = 0
     achievementCount: int = 0
+    bookCount: int = 0
+    musicCount: int = 0
 
 
 class EquipmentData(Struct):
     tid: Optional[int] = None
     rank: int = 1
     level: int = 1
     promotion: int = 0
@@ -91,14 +95,15 @@
     detailInfo: Optional[PlayerData] = None
 
 
 class MemoryInfo(Struct):
     level: int = 0
     chaos_id: Optional[int] = None
     chaos_level: Optional[int] = None
+    chaos_star_count: Optional[int] = None
 
 
 class SpaceInfo(Struct):
     memory_data: Optional[MemoryInfo] = None
     universe_level: int = 0
     light_cone_count: int = 0
     avatar_count: int = 0
```

### Comparing `mihomo-2.1.0/PKG-INFO` & `mihomo-2.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mihomo
-Version: 2.1.0
+Version: 2.2.0
 Summary: Library for API wrapper data from mihomo
 Home-page: https://github.com/Mar-7th/mihomo.py
 License: MIT
 Author: mobyw
 Author-email: mobyw66@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

