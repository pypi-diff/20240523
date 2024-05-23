# Comparing `tmp/brickbundles-0.8.1-py3-none-any.whl.zip` & `tmp/brickbundles-0.8.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 114892 bytes, number of entries: 286
+Zip file size: 115283 bytes, number of entries: 287
 -rw-r--r--  2.0 unx      106 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Actuator.brick
 -rw-r--r--  2.0 unx     1363 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/CombustionEngine.brick
 -rw-r--r--  2.0 unx      742 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Differential.brick
 -rw-r--r--  2.0 unx     3717 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/EmpiricalTorqueConverter.brick
 -rw-r--r--  2.0 unx      133 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Gear.brick
 -rw-r--r--  2.0 unx       77 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/HingeActuator.brick
 -rw-r--r--  2.0 unx      246 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/PrismaticActuator.brick
@@ -270,19 +270,20 @@
 -rw-r--r--  2.0 unx      545 b- defN 80-Jan-01 00:00 brickbundles/Vehicles/Tracks/RigidCylindricalRoller.brick
 -rw-r--r--  2.0 unx      551 b- defN 80-Jan-01 00:00 brickbundles/Vehicles/Tracks/RigidCylindricalSprocket.brick
 -rw-r--r--  2.0 unx      376 b- defN 80-Jan-01 00:00 brickbundles/Vehicles/Tracks/RoadWheel.brick
 -rw-r--r--  2.0 unx      313 b- defN 80-Jan-01 00:00 brickbundles/Vehicles/Tracks/SinusoidalVariation.brick
 -rw-r--r--  2.0 unx      810 b- defN 80-Jan-01 00:00 brickbundles/Vehicles/Tracks/System.brick
 -rw-r--r--  2.0 unx      124 b- defN 80-Jan-01 00:00 brickbundles/Vehicles/config.brick
 -rw-r--r--  2.0 unx       39 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/Box.brick
+-rw-r--r--  2.0 unx      339 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/ConvexMesh.brick
 -rw-r--r--  2.0 unx      131 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/Cylinder.brick
 -rw-r--r--  2.0 unx      234 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/ExternalTriMeshGeometry.brick
 -rw-r--r--  2.0 unx       90 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/Geometry.brick
 -rw-r--r--  2.0 unx       39 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/Sphere.brick
 -rw-r--r--  2.0 unx       96 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/TriMeshGeometry.brick
 -rw-r--r--  2.0 unx       10 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Materials/Material.brick
 -rw-r--r--  2.0 unx       72 b- defN 80-Jan-01 00:00 brickbundles/Visuals/config.brick
 -rw-r--r--  2.0 unx     1346 b- defN 80-Jan-01 00:00 brickbundles/__init__.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 brickbundles-0.8.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 brickbundles-0.8.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx    31948 b- defN 16-Jan-01 00:00 brickbundles-0.8.1.dist-info/RECORD
-286 files, 139341 bytes uncompressed, 61086 bytes compressed:  56.2%
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 brickbundles-0.8.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 brickbundles-0.8.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx    32052 b- defN 16-Jan-01 00:00 brickbundles-0.8.2.dist-info/RECORD
+287 files, 139784 bytes uncompressed, 61305 bytes compressed:  56.1%
```

## zipnote {}

```diff
@@ -819,14 +819,17 @@
 
 Filename: brickbundles/Vehicles/config.brick
 Comment: 
 
 Filename: brickbundles/Visuals/Geometries/Box.brick
 Comment: 
 
+Filename: brickbundles/Visuals/Geometries/ConvexMesh.brick
+Comment: 
+
 Filename: brickbundles/Visuals/Geometries/Cylinder.brick
 Comment: 
 
 Filename: brickbundles/Visuals/Geometries/ExternalTriMeshGeometry.brick
 Comment: 
 
 Filename: brickbundles/Visuals/Geometries/Geometry.brick
@@ -843,17 +846,17 @@
 
 Filename: brickbundles/Visuals/config.brick
 Comment: 
 
 Filename: brickbundles/__init__.py
 Comment: 
 
-Filename: brickbundles-0.8.1.dist-info/METADATA
+Filename: brickbundles-0.8.2.dist-info/METADATA
 Comment: 
 
-Filename: brickbundles-0.8.1.dist-info/WHEEL
+Filename: brickbundles-0.8.2.dist-info/WHEEL
 Comment: 
 
-Filename: brickbundles-0.8.1.dist-info/RECORD
+Filename: brickbundles-0.8.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `brickbundles-0.8.1.dist-info/METADATA` & `brickbundles-0.8.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BrickBundles
-Version: 0.8.1
+Version: 0.8.2
 Summary: Brick Bundles package, i.e. all Brick sourcefiles and convenience access method in a package
 License: Apache 2.0
 Author: Algoryx
 Author-email: algoryx@algoryx.com
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `brickbundles-0.8.1.dist-info/RECORD` & `brickbundles-0.8.2.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -269,18 +269,19 @@
 brickbundles/Vehicles/Tracks/RigidCylindricalRoller.brick,sha256=WmGHUNh7MKWQB4t13Tzpu9P1opCh5ZmT7bCZDWnuonY,545
 brickbundles/Vehicles/Tracks/RigidCylindricalSprocket.brick,sha256=myJgqvkK1rFJsXAcRinV3gNfktppzyC8jOJ2hc2VvbM,551
 brickbundles/Vehicles/Tracks/RoadWheel.brick,sha256=eiwDqc6HlzkvBbyDt5CtGeuGnr3G6bgpDmSqi-M-h00,376
 brickbundles/Vehicles/Tracks/SinusoidalVariation.brick,sha256=E8aDJJyS8cwI2c1o8Q7mgrPzC7bhkLJAzLSOVPfyZQ0,313
 brickbundles/Vehicles/Tracks/System.brick,sha256=h7OX92DGMkmzXI3-Ogllc3n2MoHPmqnA6Bn4LGSraDs,810
 brickbundles/Vehicles/config.brick,sha256=7soYoDFChCnplGjfKYIUA7tcFhYuzWsKN_pCSyd4b6M,124
 brickbundles/Visuals/Geometries/Box.brick,sha256=4xh_I1x2iZ9JwD0HTD0ScbXlUBosGbkVWymp8MZCWNY,39
+brickbundles/Visuals/Geometries/ConvexMesh.brick,sha256=WsuH8RplIA9q7FW4CyKJG9F3QSqmPfG_ComIfzpp3tU,339
 brickbundles/Visuals/Geometries/Cylinder.brick,sha256=EoVwnqE9fMtHjbU1oG5VTPQXJPG-9ylPBseUyrQM4uQ,131
 brickbundles/Visuals/Geometries/ExternalTriMeshGeometry.brick,sha256=0cEEaVuE72vhJvAv6J1guVo6yZVOCf7Q4gFP9KvElGQ,234
 brickbundles/Visuals/Geometries/Geometry.brick,sha256=-tiwTgsHtKnrPvaPO6kj5LG_gfF0csLAxdJUXJJzywg,90
 brickbundles/Visuals/Geometries/Sphere.brick,sha256=K3DerE_AE6EnHc_2GmT1e9sYrCMUosmUlTXIcqYapBg,39
 brickbundles/Visuals/Geometries/TriMeshGeometry.brick,sha256=qctdVQYflyKPuuX6HK8QvTgRbKNYlI5JAB82UNmKTZs,96
 brickbundles/Visuals/Materials/Material.brick,sha256=hVvFGaQhcFJblZ1R0SLDhWjIY6lSKC84i9hBwmA3sq8,10
 brickbundles/Visuals/config.brick,sha256=Z7y-m-8BN9N4V0OvqKp8BKivcspo8_-IpA2xA5xvf80,72
 brickbundles/__init__.py,sha256=VC7H2Q-oD1kqfe06eBZdgPlW8tC1kzBRQXWHkOIYk24,1346
-brickbundles-0.8.1.dist-info/METADATA,sha256=Lrx1nagt1b-UWWLGdFG0Yw2oT_0ZyD9ouzcR_lqmtAg,1066
-brickbundles-0.8.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-brickbundles-0.8.1.dist-info/RECORD,,
+brickbundles-0.8.2.dist-info/METADATA,sha256=qDIafX6XpHay92zG8pT9ijUF1jDphC3jO2QmnWSB0U0,1066
+brickbundles-0.8.2.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+brickbundles-0.8.2.dist-info/RECORD,,
```

