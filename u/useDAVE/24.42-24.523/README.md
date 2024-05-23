# Comparing `tmp/usedave-24.42.tar.gz` & `tmp/usedave-24.523.tar.gz`

## Comparing `usedave-24.42.tar` & `usedave-24.523.tar`

### file list

```diff
@@ -1,114 +1,114 @@
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/100x30x8_barge.dave
--rw-r--r--   0        0        0  1494035 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/17919_Seal_baby_happy_V1.obj
--rw-r--r--   0        0        0   600596 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/CWB_generic_800t.obj
--rw-r--r--   0        0        0   398197 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/Crosby_anchor_shackle_generic200t.obj
--rw-r--r--   0        0        0 10007952 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/GPWB_generic.blend
--rw-r--r--   0        0        0 10007952 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/GPWB_generic.blend1
--rw-r--r--   0        0        0    88646 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/GPWB_generic.obj
--rw-r--r--   0        0        0    16349 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/Scene_barge_at_yard.dave
--rw-r--r--   0        0        0     7730 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/Snake15.dave
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/barge with linear hydrostatics.dave
--rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/barge.obj
--rw-r--r--   0        0        0   113974 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/barge_100_30_4.dhyd
--rw-r--r--   0        0        0    76967 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/barge_100x30x4_ofx.hyd
--rw-r--r--   0        0        0   983816 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/base ocean.blend
--rw-r--r--   0        0        0   975776 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/base ocean.blend1
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/billy.dave
--rw-r--r--   0        0        0    15178 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/buoyancy husky.obj
--rw-r--r--   0        0        0   142032 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/buoyancy octopus.obj
--rw-r--r--   0        0        0   112773 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/buoyancy turtle.obj
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah with crane and 4p block.dave
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah with crane.dave
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah.dave
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/client_scene.dave
--rw-r--r--   0        0        0    26529 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cog.obj
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cone chopped.obj
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cone d1.obj
--rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/crane block 2p.dave
--rw-r--r--   0        0        0     7287 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/crane block 4p.dave
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cube.obj
--rw-r--r--   0        0        0    15161 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cube_with_bevel.obj
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cylinder 1x1x1 lowres.obj
--rw-r--r--   0        0        0     5483 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cylinder 1x1x1.obj
--rw-r--r--   0        0        0  1289891 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/day.hdr
--rw-r--r--   0        0        0   853652 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/default.blend
--rw-r--r--   0        0        0  8294465 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/default.hdr
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/default_component.dave
--rw-r--r--   0        0        0    42891 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/floater.obj
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/foundation.dave
--rw-r--r--   0        0        0   237901 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/foundation.obj
--rw-r--r--   0        0        0    86516 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/grid10.dave
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/grid_1m.obj
--rw-r--r--   0        0        0    55444 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/hook2p.obj
--rw-r--r--   0        0        0    74145 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/hook4p.obj
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/husky.dave
--rw-r--r--   0        0        0   113844 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/husky.dhyd
--rw-r--r--   0        0        0    19208 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/lower_block.obj
--rw-r--r--   0        0        0  4264572 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/magic.hdr
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/mast crane.dave
--rw-r--r--   0        0        0    50059 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/node_prop_info.csv
--rw-r--r--   0        0        0     6070 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/octopus.dave
--rw-r--r--   0        0        0    44823 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/padeye.obj
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/pendulum.dave
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/plane.obj
--rw-r--r--   0        0        0   240184 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/plane_curved.stl
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/pyramid.obj
--rw-r--r--   0        0        0   260595 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/shackle_gp800.obj
--rw-r--r--   0        0        0   681748 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/shackle_gp800_wb.obj
--rw-r--r--   0        0        0    23772 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/sphere d1.obj
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/spreaderbar.dave
--rw-r--r--   0        0        0    48484 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/suzanne.stl
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/tower.dave
--rw-r--r--   0        0        0    67478 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/trunnion_800.obj
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/turbine blade.dave
--rw-r--r--   0        0        0    18010 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/turbine blade.obj
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/turbine nacelle.dave
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/turtle.dave
--rw-r--r--   0        0        0     5936 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/uc_colorbar_smaller.png
--rw-r--r--   0        0        0    29815 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/upper_block.obj
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/upsea turbine.dave
--rw-r--r--   0        0        0   316808 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/virtualSea.jpg
--rw-r--r--   0        0        0    50228 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/visual a-frame.obj
--rw-r--r--   0        0        0   473943 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/visual crane mast and boomrest.obj
--rw-r--r--   0        0        0     8412 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/visual crane-boom.obj
--rw-r--r--   0        0        0  4803793 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/visual vessel husky.obj
--rw-r--r--   0        0        0   635361 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/visual vessel octopus.obj
--rw-r--r--   0        0        0  3040554 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/visual vessel turtle.obj
--rw-r--r--   0        0        0   189848 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/waveplane.jpg
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/white.png
--rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/wirecube.obj
--rw-r--r--   0        0        0   863643 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/worker.obj
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/yard.dave
--rw-r--r--   0        0        0   194047 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/buoyancy cheetah.obj
--rw-r--r--   0        0        0   114215 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/cheetah.dhyd
--rw-r--r--   0        0        0   771159 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/visual vessel cheetah.obj
--rw-r--r--   0        0        0    23284 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/tanks/c10.stl
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/tanks/c7.stl
--rw-r--r--   0        0        0     6984 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/tanks/c8.stl
--rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/tanks/c9.stl
--rw-r--r--   0        0        0     8684 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/tanks/ps1.stl
--rw-r--r--   0        0        0     8484 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/tanks/ps10.stl
--rw-r--r--   0        0        0     9684 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/tanks/ps2.stl
--rw-r--r--   0        0        0     9484 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/tanks/ps3.stl
--rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/tanks/ps4.stl
--rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/tanks/ps5.stl
--rw-r--r--   0        0        0     8784 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/tanks/ps6.stl
--rw-r--r--   0        0        0     9784 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/tanks/ps7.stl
--rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/tanks/ps8.stl
--rw-r--r--   0        0        0    11084 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/tanks/ps9.stl
--rw-r--r--   0        0        0     7484 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/tanks/sb1.stl
--rw-r--r--   0        0        0     8784 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/tanks/sb10.stl
--rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/tanks/sb2.stl
--rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/tanks/sb3.stl
--rw-r--r--   0        0        0    10384 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/tanks/sb4.stl
--rw-r--r--   0        0        0    10384 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/tanks/sb5.stl
--rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/tanks/sb6.stl
--rw-r--r--   0        0        0     9384 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/tanks/sb7.stl
--rw-r--r--   0        0        0     9784 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/tanks/sb8.stl
--rw-r--r--   0        0        0    11284 2020-02-02 00:00:00.000000 usedave-24.42/src/DAVE/resources/cheetah/tanks/sb9.stl
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 usedave-24.42/.gitignore
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 usedave-24.42/AUTHORS.rst
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 usedave-24.42/LICENSE
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 usedave-24.42/README.md
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 usedave-24.42/pyproject.toml
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 usedave-24.42/PKG-INFO
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/100x30x8_barge.dave
+-rw-r--r--   0        0        0  1494035 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/17919_Seal_baby_happy_V1.obj
+-rw-r--r--   0        0        0   600596 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/CWB_generic_800t.obj
+-rw-r--r--   0        0        0   398197 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/Crosby_anchor_shackle_generic200t.obj
+-rw-r--r--   0        0        0 10007952 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/GPWB_generic.blend
+-rw-r--r--   0        0        0 10007952 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/GPWB_generic.blend1
+-rw-r--r--   0        0        0    88646 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/GPWB_generic.obj
+-rw-r--r--   0        0        0    16349 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/Scene_barge_at_yard.dave
+-rw-r--r--   0        0        0     7730 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/Snake15.dave
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/barge with linear hydrostatics.dave
+-rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/barge.obj
+-rw-r--r--   0        0        0   113974 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/barge_100_30_4.dhyd
+-rw-r--r--   0        0        0    76967 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/barge_100x30x4_ofx.hyd
+-rw-r--r--   0        0        0   983816 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/base ocean.blend
+-rw-r--r--   0        0        0   975776 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/base ocean.blend1
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/billy.dave
+-rw-r--r--   0        0        0    15178 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/buoyancy husky.obj
+-rw-r--r--   0        0        0   142032 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/buoyancy octopus.obj
+-rw-r--r--   0        0        0   112773 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/buoyancy turtle.obj
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah with crane and 4p block.dave
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah with crane.dave
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah.dave
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/client_scene.dave
+-rw-r--r--   0        0        0    26529 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cog.obj
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cone chopped.obj
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cone d1.obj
+-rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/crane block 2p.dave
+-rw-r--r--   0        0        0     7287 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/crane block 4p.dave
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cube.obj
+-rw-r--r--   0        0        0    15161 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cube_with_bevel.obj
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cylinder 1x1x1 lowres.obj
+-rw-r--r--   0        0        0     5483 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cylinder 1x1x1.obj
+-rw-r--r--   0        0        0  1289891 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/day.hdr
+-rw-r--r--   0        0        0   853652 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/default.blend
+-rw-r--r--   0        0        0  8294465 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/default.hdr
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/default_component.dave
+-rw-r--r--   0        0        0    42891 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/floater.obj
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/foundation.dave
+-rw-r--r--   0        0        0   237901 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/foundation.obj
+-rw-r--r--   0        0        0    86516 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/grid10.dave
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/grid_1m.obj
+-rw-r--r--   0        0        0    55444 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/hook2p.obj
+-rw-r--r--   0        0        0    74145 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/hook4p.obj
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/husky.dave
+-rw-r--r--   0        0        0   113844 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/husky.dhyd
+-rw-r--r--   0        0        0    19208 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/lower_block.obj
+-rw-r--r--   0        0        0  4264572 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/magic.hdr
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/mast crane.dave
+-rw-r--r--   0        0        0    50059 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/node_prop_info.csv
+-rw-r--r--   0        0        0     6070 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/octopus.dave
+-rw-r--r--   0        0        0    44823 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/padeye.obj
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/pendulum.dave
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/plane.obj
+-rw-r--r--   0        0        0   240184 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/plane_curved.stl
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/pyramid.obj
+-rw-r--r--   0        0        0   260595 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/shackle_gp800.obj
+-rw-r--r--   0        0        0   681748 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/shackle_gp800_wb.obj
+-rw-r--r--   0        0        0    23772 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/sphere d1.obj
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/spreaderbar.dave
+-rw-r--r--   0        0        0    48484 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/suzanne.stl
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/tower.dave
+-rw-r--r--   0        0        0    67478 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/trunnion_800.obj
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/turbine blade.dave
+-rw-r--r--   0        0        0    18010 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/turbine blade.obj
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/turbine nacelle.dave
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/turtle.dave
+-rw-r--r--   0        0        0     5936 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/uc_colorbar_smaller.png
+-rw-r--r--   0        0        0    29815 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/upper_block.obj
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/upsea turbine.dave
+-rw-r--r--   0        0        0   316808 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/virtualSea.jpg
+-rw-r--r--   0        0        0    50228 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/visual a-frame.obj
+-rw-r--r--   0        0        0   473943 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/visual crane mast and boomrest.obj
+-rw-r--r--   0        0        0     8412 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/visual crane-boom.obj
+-rw-r--r--   0        0        0  4803793 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/visual vessel husky.obj
+-rw-r--r--   0        0        0   635361 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/visual vessel octopus.obj
+-rw-r--r--   0        0        0  3040554 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/visual vessel turtle.obj
+-rw-r--r--   0        0        0   189848 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/waveplane.jpg
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/white.png
+-rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/wirecube.obj
+-rw-r--r--   0        0        0   863643 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/worker.obj
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/yard.dave
+-rw-r--r--   0        0        0   194047 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/buoyancy cheetah.obj
+-rw-r--r--   0        0        0   114215 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/cheetah.dhyd
+-rw-r--r--   0        0        0   771159 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/visual vessel cheetah.obj
+-rw-r--r--   0        0        0    23284 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/tanks/c10.stl
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/tanks/c7.stl
+-rw-r--r--   0        0        0     6984 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/tanks/c8.stl
+-rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/tanks/c9.stl
+-rw-r--r--   0        0        0     8684 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/tanks/ps1.stl
+-rw-r--r--   0        0        0     8484 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/tanks/ps10.stl
+-rw-r--r--   0        0        0     9684 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/tanks/ps2.stl
+-rw-r--r--   0        0        0     9484 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/tanks/ps3.stl
+-rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/tanks/ps4.stl
+-rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/tanks/ps5.stl
+-rw-r--r--   0        0        0     8784 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/tanks/ps6.stl
+-rw-r--r--   0        0        0     9784 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/tanks/ps7.stl
+-rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/tanks/ps8.stl
+-rw-r--r--   0        0        0    11084 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/tanks/ps9.stl
+-rw-r--r--   0        0        0     7484 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/tanks/sb1.stl
+-rw-r--r--   0        0        0     8784 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/tanks/sb10.stl
+-rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/tanks/sb2.stl
+-rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/tanks/sb3.stl
+-rw-r--r--   0        0        0    10384 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/tanks/sb4.stl
+-rw-r--r--   0        0        0    10384 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/tanks/sb5.stl
+-rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/tanks/sb6.stl
+-rw-r--r--   0        0        0     9384 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/tanks/sb7.stl
+-rw-r--r--   0        0        0     9784 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/tanks/sb8.stl
+-rw-r--r--   0        0        0    11284 2020-02-02 00:00:00.000000 usedave-24.523/src/DAVE/resources/cheetah/tanks/sb9.stl
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 usedave-24.523/.gitignore
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 usedave-24.523/AUTHORS.rst
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 usedave-24.523/LICENSE
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 usedave-24.523/README.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 usedave-24.523/pyproject.toml
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 usedave-24.523/PKG-INFO
```

### Comparing `usedave-24.42/src/DAVE/resources/100x30x8_barge.dave` & `usedave-24.523/src/DAVE/resources/100x30x8_barge.dave`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/17919_Seal_baby_happy_V1.obj` & `usedave-24.523/src/DAVE/resources/17919_Seal_baby_happy_V1.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/CWB_generic_800t.obj` & `usedave-24.523/src/DAVE/resources/CWB_generic_800t.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/Crosby_anchor_shackle_generic200t.obj` & `usedave-24.523/src/DAVE/resources/Crosby_anchor_shackle_generic200t.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/GPWB_generic.blend` & `usedave-24.523/src/DAVE/resources/GPWB_generic.blend`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/GPWB_generic.blend1` & `usedave-24.523/src/DAVE/resources/GPWB_generic.blend1`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/GPWB_generic.obj` & `usedave-24.523/src/DAVE/resources/GPWB_generic.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/Scene_barge_at_yard.dave` & `usedave-24.523/src/DAVE/resources/Scene_barge_at_yard.dave`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/Snake15.dave` & `usedave-24.523/src/DAVE/resources/Snake15.dave`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/barge with linear hydrostatics.dave` & `usedave-24.523/src/DAVE/resources/barge with linear hydrostatics.dave`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/barge.obj` & `usedave-24.523/src/DAVE/resources/barge.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/barge_100_30_4.dhyd` & `usedave-24.523/src/DAVE/resources/barge_100_30_4.dhyd`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/barge_100x30x4_ofx.hyd` & `usedave-24.523/src/DAVE/resources/barge_100x30x4_ofx.hyd`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/base ocean.blend` & `usedave-24.523/src/DAVE/resources/base ocean.blend`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/base ocean.blend1` & `usedave-24.523/src/DAVE/resources/base ocean.blend1`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/billy.dave` & `usedave-24.523/src/DAVE/resources/billy.dave`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/buoyancy husky.obj` & `usedave-24.523/src/DAVE/resources/buoyancy husky.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/buoyancy octopus.obj` & `usedave-24.523/src/DAVE/resources/buoyancy octopus.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/buoyancy turtle.obj` & `usedave-24.523/src/DAVE/resources/buoyancy turtle.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah with crane and 4p block.dave` & `usedave-24.523/src/DAVE/resources/cheetah with crane and 4p block.dave`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah.dave` & `usedave-24.523/src/DAVE/resources/cheetah.dave`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cog.obj` & `usedave-24.523/src/DAVE/resources/cog.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cone chopped.obj` & `usedave-24.523/src/DAVE/resources/cone chopped.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cone d1.obj` & `usedave-24.523/src/DAVE/resources/cone d1.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/crane block 2p.dave` & `usedave-24.523/src/DAVE/resources/crane block 2p.dave`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/crane block 4p.dave` & `usedave-24.523/src/DAVE/resources/crane block 4p.dave`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cube.obj` & `usedave-24.523/src/DAVE/resources/cube.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cube_with_bevel.obj` & `usedave-24.523/src/DAVE/resources/cube_with_bevel.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cylinder 1x1x1 lowres.obj` & `usedave-24.523/src/DAVE/resources/cylinder 1x1x1 lowres.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cylinder 1x1x1.obj` & `usedave-24.523/src/DAVE/resources/cylinder 1x1x1.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/day.hdr` & `usedave-24.523/src/DAVE/resources/day.hdr`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/default.blend` & `usedave-24.523/src/DAVE/resources/default.blend`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/default.hdr` & `usedave-24.523/src/DAVE/resources/default.hdr`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/floater.obj` & `usedave-24.523/src/DAVE/resources/floater.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/foundation.dave` & `usedave-24.523/src/DAVE/resources/foundation.dave`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/foundation.obj` & `usedave-24.523/src/DAVE/resources/foundation.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/grid10.dave` & `usedave-24.523/src/DAVE/resources/grid10.dave`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/grid_1m.obj` & `usedave-24.523/src/DAVE/resources/grid_1m.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/hook2p.obj` & `usedave-24.523/src/DAVE/resources/hook2p.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/hook4p.obj` & `usedave-24.523/src/DAVE/resources/hook4p.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/husky.dave` & `usedave-24.523/src/DAVE/resources/husky.dave`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/husky.dhyd` & `usedave-24.523/src/DAVE/resources/husky.dhyd`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/lower_block.obj` & `usedave-24.523/src/DAVE/resources/lower_block.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/magic.hdr` & `usedave-24.523/src/DAVE/resources/magic.hdr`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/mast crane.dave` & `usedave-24.523/src/DAVE/resources/mast crane.dave`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/node_prop_info.csv` & `usedave-24.523/src/DAVE/resources/node_prop_info.csv`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/octopus.dave` & `usedave-24.523/src/DAVE/resources/octopus.dave`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/padeye.obj` & `usedave-24.523/src/DAVE/resources/padeye.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/pendulum.dave` & `usedave-24.523/src/DAVE/resources/pendulum.dave`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/plane.obj` & `usedave-24.523/src/DAVE/resources/plane.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/plane_curved.stl` & `usedave-24.523/src/DAVE/resources/plane_curved.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/pyramid.obj` & `usedave-24.523/src/DAVE/resources/pyramid.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/shackle_gp800.obj` & `usedave-24.523/src/DAVE/resources/shackle_gp800.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/shackle_gp800_wb.obj` & `usedave-24.523/src/DAVE/resources/shackle_gp800_wb.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/sphere d1.obj` & `usedave-24.523/src/DAVE/resources/sphere d1.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/spreaderbar.dave` & `usedave-24.523/src/DAVE/resources/spreaderbar.dave`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/suzanne.stl` & `usedave-24.523/src/DAVE/resources/suzanne.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/tower.dave` & `usedave-24.523/src/DAVE/resources/tower.dave`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/trunnion_800.obj` & `usedave-24.523/src/DAVE/resources/trunnion_800.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/turbine blade.dave` & `usedave-24.523/src/DAVE/resources/turbine blade.dave`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/turbine blade.obj` & `usedave-24.523/src/DAVE/resources/turbine blade.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/turbine nacelle.dave` & `usedave-24.523/src/DAVE/resources/turbine nacelle.dave`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/turtle.dave` & `usedave-24.523/src/DAVE/resources/turtle.dave`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/uc_colorbar_smaller.png` & `usedave-24.523/src/DAVE/resources/uc_colorbar_smaller.png`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/upper_block.obj` & `usedave-24.523/src/DAVE/resources/upper_block.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/upsea turbine.dave` & `usedave-24.523/src/DAVE/resources/upsea turbine.dave`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/virtualSea.jpg` & `usedave-24.523/src/DAVE/resources/virtualSea.jpg`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/visual a-frame.obj` & `usedave-24.523/src/DAVE/resources/visual a-frame.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/visual crane mast and boomrest.obj` & `usedave-24.523/src/DAVE/resources/visual crane mast and boomrest.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/visual crane-boom.obj` & `usedave-24.523/src/DAVE/resources/visual crane-boom.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/visual vessel husky.obj` & `usedave-24.523/src/DAVE/resources/visual vessel husky.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/visual vessel octopus.obj` & `usedave-24.523/src/DAVE/resources/visual vessel octopus.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/visual vessel turtle.obj` & `usedave-24.523/src/DAVE/resources/visual vessel turtle.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/waveplane.jpg` & `usedave-24.523/src/DAVE/resources/waveplane.jpg`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/wirecube.obj` & `usedave-24.523/src/DAVE/resources/wirecube.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/worker.obj` & `usedave-24.523/src/DAVE/resources/worker.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/yard.dave` & `usedave-24.523/src/DAVE/resources/yard.dave`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/buoyancy cheetah.obj` & `usedave-24.523/src/DAVE/resources/cheetah/buoyancy cheetah.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/cheetah.dhyd` & `usedave-24.523/src/DAVE/resources/cheetah/cheetah.dhyd`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/visual vessel cheetah.obj` & `usedave-24.523/src/DAVE/resources/cheetah/visual vessel cheetah.obj`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/tanks/c10.stl` & `usedave-24.523/src/DAVE/resources/cheetah/tanks/c10.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/tanks/c7.stl` & `usedave-24.523/src/DAVE/resources/cheetah/tanks/c7.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/tanks/c8.stl` & `usedave-24.523/src/DAVE/resources/cheetah/tanks/c8.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/tanks/c9.stl` & `usedave-24.523/src/DAVE/resources/cheetah/tanks/c9.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/tanks/ps1.stl` & `usedave-24.523/src/DAVE/resources/cheetah/tanks/ps1.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/tanks/ps10.stl` & `usedave-24.523/src/DAVE/resources/cheetah/tanks/ps10.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/tanks/ps2.stl` & `usedave-24.523/src/DAVE/resources/cheetah/tanks/ps2.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/tanks/ps3.stl` & `usedave-24.523/src/DAVE/resources/cheetah/tanks/ps3.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/tanks/ps4.stl` & `usedave-24.523/src/DAVE/resources/cheetah/tanks/ps4.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/tanks/ps5.stl` & `usedave-24.523/src/DAVE/resources/cheetah/tanks/ps5.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/tanks/ps6.stl` & `usedave-24.523/src/DAVE/resources/cheetah/tanks/ps6.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/tanks/ps7.stl` & `usedave-24.523/src/DAVE/resources/cheetah/tanks/ps7.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/tanks/ps8.stl` & `usedave-24.523/src/DAVE/resources/cheetah/tanks/ps8.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/tanks/ps9.stl` & `usedave-24.523/src/DAVE/resources/cheetah/tanks/ps9.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/tanks/sb1.stl` & `usedave-24.523/src/DAVE/resources/cheetah/tanks/sb1.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/tanks/sb10.stl` & `usedave-24.523/src/DAVE/resources/cheetah/tanks/sb10.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/tanks/sb2.stl` & `usedave-24.523/src/DAVE/resources/cheetah/tanks/sb2.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/tanks/sb3.stl` & `usedave-24.523/src/DAVE/resources/cheetah/tanks/sb3.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/tanks/sb4.stl` & `usedave-24.523/src/DAVE/resources/cheetah/tanks/sb4.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/tanks/sb5.stl` & `usedave-24.523/src/DAVE/resources/cheetah/tanks/sb5.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/tanks/sb6.stl` & `usedave-24.523/src/DAVE/resources/cheetah/tanks/sb6.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/tanks/sb7.stl` & `usedave-24.523/src/DAVE/resources/cheetah/tanks/sb7.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/tanks/sb8.stl` & `usedave-24.523/src/DAVE/resources/cheetah/tanks/sb8.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/src/DAVE/resources/cheetah/tanks/sb9.stl` & `usedave-24.523/src/DAVE/resources/cheetah/tanks/sb9.stl`

 * *Files identical despite different names*

### Comparing `usedave-24.42/.gitignore` & `usedave-24.523/.gitignore`

 * *Files identical despite different names*

### Comparing `usedave-24.42/LICENSE` & `usedave-24.523/LICENSE`

 * *Files identical despite different names*

### Comparing `usedave-24.42/README.md` & `usedave-24.523/README.md`

 * *Files identical despite different names*

### Comparing `usedave-24.42/pyproject.toml` & `usedave-24.523/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/DAVE"]
 
 
 [project]
 name = "useDAVE"
-version = "24.42"
+version = "24.0523"
 authors = [
   { name="Ruben de Bruin", email="info@rdbr.nl" },
 ]
 description = "Design Analysis Visualization Engineering (or Difficult Analysis Very Easy)!"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `usedave-24.42/PKG-INFO` & `usedave-24.523/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: useDAVE
-Version: 24.42
+Version: 24.523
 Summary: Design Analysis Visualization Engineering (or Difficult Analysis Very Easy)!
 Project-URL: Homepage, https://usedave.nl
 Project-URL: Issues, https://github.com/RubendeBruin/DAVE
 Author-email: Ruben de Bruin <info@rdbr.nl>
 License-File: AUTHORS.rst
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

