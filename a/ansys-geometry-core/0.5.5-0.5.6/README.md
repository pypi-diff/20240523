# Comparing `tmp/ansys_geometry_core-0.5.5.tar.gz` & `tmp/ansys_geometry_core-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_geometry_core-0.5.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_geometry_core-0.5.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_geometry_core-0.5.5.tar` & `ansys_geometry_core-0.5.6.tar`

### file list

```diff
@@ -1,113 +1,114 @@
--rw-r--r--   0        0        0     1098 2024-05-21 11:20:22.139464 ansys_geometry_core-0.5.5/LICENSE
--rw-r--r--   0        0        0     4966 2024-05-21 11:20:22.139464 ansys_geometry_core-0.5.5/README.rst
--rw-r--r--   0        0        0     4467 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     2762 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/__init__.py
--rw-r--r--   0        0        0     2477 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/connection/__init__.py
--rw-r--r--   0        0        0     1618 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/connection/backend.py
--rw-r--r--   0        0        0    12306 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/connection/client.py
--rw-r--r--   0        0        0    18876 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/connection/conversions.py
--rw-r--r--   0        0        0     2483 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/connection/defaults.py
--rw-r--r--   0        0        0    13911 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/connection/docker_instance.py
--rw-r--r--   0        0        0    30050 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/connection/launcher.py
--rw-r--r--   0        0        0      167 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/connection/pim_configuration.json
--rw-r--r--   0        0        0    16343 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/connection/product_instance.py
--rw-r--r--   0        0        0     1776 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/connection/validate.py
--rw-r--r--   0        0        0     1782 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/designer/__init__.py
--rw-r--r--   0        0        0     7898 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/designer/beam.py
--rw-r--r--   0        0        0    46126 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/designer/body.py
--rw-r--r--   0        0        0    52507 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/designer/component.py
--rw-r--r--   0        0        0     6034 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/designer/coordinate_system.py
--rw-r--r--   0        0        0    40126 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/designer/design.py
--rw-r--r--   0        0        0     3697 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/designer/designpoint.py
--rw-r--r--   0        0        0     7750 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/designer/edge.py
--rw-r--r--   0        0        0    15145 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/designer/face.py
--rw-r--r--   0        0        0     5468 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/designer/part.py
--rw-r--r--   0        0        0     4686 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/designer/selection.py
--rw-r--r--   0        0        0     4101 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/errors.py
--rw-r--r--   0        0        0    22524 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/logger.py
--rw-r--r--   0        0        0     1349 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/materials/__init__.py
--rw-r--r--   0        0        0     3268 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/materials/material.py
--rw-r--r--   0        0        0     4107 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/materials/property.py
--rw-r--r--   0        0        0     1883 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/math/__init__.py
--rw-r--r--   0        0        0     6819 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/math/bbox.py
--rw-r--r--   0        0        0     3259 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/math/constants.py
--rw-r--r--   0        0        0     7035 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/math/frame.py
--rw-r--r--   0        0        0     4823 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/math/matrix.py
--rw-r--r--   0        0        0     4240 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/math/plane.py
--rw-r--r--   0        0        0    12120 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/math/point.py
--rw-r--r--   0        0        0    18024 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/math/vector.py
--rw-r--r--   0        0        0     2085 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/misc/__init__.py
--rw-r--r--   0        0        0     8033 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/misc/accuracy.py
--rw-r--r--   0        0        0     5215 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/misc/auxiliary.py
--rw-r--r--   0        0        0    12751 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/misc/checks.py
--rw-r--r--   0        0        0     8253 2024-05-21 11:20:22.147464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/misc/measurements.py
--rw-r--r--   0        0        0     2291 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/misc/options.py
--rw-r--r--   0        0        0     3684 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/misc/units.py
--rw-r--r--   0        0        0    17075 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/modeler.py
--rw-r--r--   0        0        0     1417 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/__init__.py
--rw-r--r--   0        0        0    22163 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/plotter.py
--rw-r--r--   0        0        0    15007 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/plotter_helper.py
--rw-r--r--   0        0        0     5826 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/plotting_types.py
--rw-r--r--   0        0        0     4213 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/trame_gui.py
--rw-r--r--   0        0        0     1710 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/__init__.py
--rw-r--r--   0        0        0      499 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/_images/+xy.png
--rw-r--r--   0        0        0      487 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/_images/+xz.png
--rw-r--r--   0        0        0      497 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/_images/+yz.png
--rw-r--r--   0        0        0      496 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/_images/-xy.png
--rw-r--r--   0        0        0      484 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/_images/-xz.png
--rw-r--r--   0        0        0      495 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/_images/-yz.png
--rw-r--r--   0        0        0      569 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/_images/designpoint.png
--rw-r--r--   0        0        0      526 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/_images/downarrow.png
--rw-r--r--   0        0        0      725 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/_images/isometric.png
--rw-r--r--   0        0        0      339 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/_images/measurement.png
--rw-r--r--   0        0        0      341 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/_images/ruler.png
--rw-r--r--   0        0        0      451 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/_images/upxarrow.png
--rw-r--r--   0        0        0      442 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/_images/upyarrow.png
--rw-r--r--   0        0        0      428 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/_images/upzarrow.png
--rw-r--r--   0        0        0     3058 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/button.py
--rw-r--r--   0        0        0     4239 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/displace_arrows.py
--rw-r--r--   0        0        0     3626 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/measure.py
--rw-r--r--   0        0        0     3700 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/ruler.py
--rw-r--r--   0        0        0     3480 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/show_design_point.py
--rw-r--r--   0        0        0     3348 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/view_button.py
--rw-r--r--   0        0        0     2305 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/widget.py
--rw-r--r--   0        0        0     2176 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/__init__.py
--rw-r--r--   0        0        0     5634 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/box_uv.py
--rw-r--r--   0        0        0     1580 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/curves/__init__.py
--rw-r--r--   0        0        0    11617 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/curves/circle.py
--rw-r--r--   0        0        0     3539 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/curves/curve.py
--rw-r--r--   0        0        0     2767 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/curves/curve_evaluation.py
--rw-r--r--   0        0        0    14319 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/curves/ellipse.py
--rw-r--r--   0        0        0     8893 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/curves/line.py
--rw-r--r--   0        0        0     7428 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/curves/trimmed_curve.py
--rw-r--r--   0        0        0    13001 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/parameterization.py
--rw-r--r--   0        0        0     1746 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/surfaces/__init__.py
--rw-r--r--   0        0        0    14274 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/surfaces/cone.py
--rw-r--r--   0        0        0    14748 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/surfaces/cylinder.py
--rw-r--r--   0        0        0     8067 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/surfaces/plane.py
--rw-r--r--   0        0        0    13257 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/surfaces/sphere.py
--rw-r--r--   0        0        0     3467 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/surfaces/surface.py
--rw-r--r--   0        0        0     4281 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/surfaces/surface_evaluation.py
--rw-r--r--   0        0        0    16027 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/surfaces/torus.py
--rw-r--r--   0        0        0     5694 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/surfaces/trimmed_surface.py
--rw-r--r--   0        0        0     1909 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/__init__.py
--rw-r--r--   0        0        0    11643 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/arc.py
--rw-r--r--   0        0        0     6690 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/box.py
--rw-r--r--   0        0        0     5139 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/circle.py
--rw-r--r--   0        0        0     2991 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/edge.py
--rw-r--r--   0        0        0     7734 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/ellipse.py
--rw-r--r--   0        0        0     3018 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/face.py
--rw-r--r--   0        0        0    19590 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/gears.py
--rw-r--r--   0        0        0     6063 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/polygon.py
--rw-r--r--   0        0        0     6076 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/segment.py
--rw-r--r--   0        0        0    31342 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/sketch.py
--rw-r--r--   0        0        0     6878 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/slot.py
--rw-r--r--   0        0        0     8286 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/trapezoid.py
--rw-r--r--   0        0        0     3847 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/triangle.py
--rw-r--r--   0        0        0     1550 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/tools/__init__.py
--rw-r--r--   0        0        0     3856 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/tools/measurement_tools.py
--rw-r--r--   0        0        0    14367 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/tools/problem_areas.py
--rw-r--r--   0        0        0     2429 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/tools/repair_tool_message.py
--rw-r--r--   0        0        0    10524 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/tools/repair_tools.py
--rw-r--r--   0        0        0     1670 2024-05-21 11:20:22.151464 ansys_geometry_core-0.5.5/src/ansys/geometry/core/typing.py
--rw-r--r--   0        0        0     9186 1970-01-01 00:00:00.000000 ansys_geometry_core-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-05-23 16:09:17.386957 ansys_geometry_core-0.5.6/LICENSE
+-rw-r--r--   0        0        0     4966 2024-05-23 16:09:17.386957 ansys_geometry_core-0.5.6/README.rst
+-rw-r--r--   0        0        0     4464 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     2762 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/__init__.py
+-rw-r--r--   0        0        0     2477 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/connection/__init__.py
+-rw-r--r--   0        0        0     1618 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/connection/backend.py
+-rw-r--r--   0        0        0    12306 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/connection/client.py
+-rw-r--r--   0        0        0    18876 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/connection/conversions.py
+-rw-r--r--   0        0        0     2483 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/connection/defaults.py
+-rw-r--r--   0        0        0    13911 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/connection/docker_instance.py
+-rw-r--r--   0        0        0    30050 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/connection/launcher.py
+-rw-r--r--   0        0        0      167 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/connection/pim_configuration.json
+-rw-r--r--   0        0        0    16336 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/connection/product_instance.py
+-rw-r--r--   0        0        0     1776 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/connection/validate.py
+-rw-r--r--   0        0        0     1782 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/designer/__init__.py
+-rw-r--r--   0        0        0     7898 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/designer/beam.py
+-rw-r--r--   0        0        0    46126 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/designer/body.py
+-rw-r--r--   0        0        0    52507 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/designer/component.py
+-rw-r--r--   0        0        0     6034 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/designer/coordinate_system.py
+-rw-r--r--   0        0        0    40126 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/designer/design.py
+-rw-r--r--   0        0        0     3697 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/designer/designpoint.py
+-rw-r--r--   0        0        0     7750 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/designer/edge.py
+-rw-r--r--   0        0        0    15145 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/designer/face.py
+-rw-r--r--   0        0        0     5468 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/designer/part.py
+-rw-r--r--   0        0        0     4686 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/designer/selection.py
+-rw-r--r--   0        0        0     4101 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/errors.py
+-rw-r--r--   0        0        0    22524 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/logger.py
+-rw-r--r--   0        0        0     1349 2024-05-23 16:09:17.394956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/materials/__init__.py
+-rw-r--r--   0        0        0     3268 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/materials/material.py
+-rw-r--r--   0        0        0     4107 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/materials/property.py
+-rw-r--r--   0        0        0     1954 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/math/__init__.py
+-rw-r--r--   0        0        0     6819 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/math/bbox.py
+-rw-r--r--   0        0        0     3259 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/math/constants.py
+-rw-r--r--   0        0        0     7035 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/math/frame.py
+-rw-r--r--   0        0        0     4823 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/math/matrix.py
+-rw-r--r--   0        0        0     3309 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/math/misc.py
+-rw-r--r--   0        0        0     4240 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/math/plane.py
+-rw-r--r--   0        0        0    12120 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/math/point.py
+-rw-r--r--   0        0        0    18024 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/math/vector.py
+-rw-r--r--   0        0        0     2085 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/misc/__init__.py
+-rw-r--r--   0        0        0     8033 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/misc/accuracy.py
+-rw-r--r--   0        0        0     5215 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/misc/auxiliary.py
+-rw-r--r--   0        0        0    12751 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/misc/checks.py
+-rw-r--r--   0        0        0     8253 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/misc/measurements.py
+-rw-r--r--   0        0        0     2291 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/misc/options.py
+-rw-r--r--   0        0        0     3684 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/misc/units.py
+-rw-r--r--   0        0        0    17075 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/modeler.py
+-rw-r--r--   0        0        0     1417 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/__init__.py
+-rw-r--r--   0        0        0    22163 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/plotter.py
+-rw-r--r--   0        0        0    15007 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/plotter_helper.py
+-rw-r--r--   0        0        0     5826 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/plotting_types.py
+-rw-r--r--   0        0        0     4213 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/trame_gui.py
+-rw-r--r--   0        0        0     1710 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/__init__.py
+-rw-r--r--   0        0        0      499 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/_images/+xy.png
+-rw-r--r--   0        0        0      487 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/_images/+xz.png
+-rw-r--r--   0        0        0      497 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/_images/+yz.png
+-rw-r--r--   0        0        0      496 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/_images/-xy.png
+-rw-r--r--   0        0        0      484 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/_images/-xz.png
+-rw-r--r--   0        0        0      495 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/_images/-yz.png
+-rw-r--r--   0        0        0      569 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/_images/designpoint.png
+-rw-r--r--   0        0        0      526 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/_images/downarrow.png
+-rw-r--r--   0        0        0      725 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/_images/isometric.png
+-rw-r--r--   0        0        0      339 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/_images/measurement.png
+-rw-r--r--   0        0        0      341 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/_images/ruler.png
+-rw-r--r--   0        0        0      451 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/_images/upxarrow.png
+-rw-r--r--   0        0        0      442 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/_images/upyarrow.png
+-rw-r--r--   0        0        0      428 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/_images/upzarrow.png
+-rw-r--r--   0        0        0     3058 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/button.py
+-rw-r--r--   0        0        0     4239 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/displace_arrows.py
+-rw-r--r--   0        0        0     3626 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/measure.py
+-rw-r--r--   0        0        0     3700 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/ruler.py
+-rw-r--r--   0        0        0     3480 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/show_design_point.py
+-rw-r--r--   0        0        0     3348 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/view_button.py
+-rw-r--r--   0        0        0     2305 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/widget.py
+-rw-r--r--   0        0        0     2176 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/__init__.py
+-rw-r--r--   0        0        0     5634 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/box_uv.py
+-rw-r--r--   0        0        0     1580 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/curves/__init__.py
+-rw-r--r--   0        0        0    11617 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/curves/circle.py
+-rw-r--r--   0        0        0     3539 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/curves/curve.py
+-rw-r--r--   0        0        0     2767 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/curves/curve_evaluation.py
+-rw-r--r--   0        0        0    14319 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/curves/ellipse.py
+-rw-r--r--   0        0        0     8893 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/curves/line.py
+-rw-r--r--   0        0        0     7428 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/curves/trimmed_curve.py
+-rw-r--r--   0        0        0    13001 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/parameterization.py
+-rw-r--r--   0        0        0     1746 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/surfaces/__init__.py
+-rw-r--r--   0        0        0    14274 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/surfaces/cone.py
+-rw-r--r--   0        0        0    14748 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/surfaces/cylinder.py
+-rw-r--r--   0        0        0     8067 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/surfaces/plane.py
+-rw-r--r--   0        0        0    13257 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/surfaces/sphere.py
+-rw-r--r--   0        0        0     3467 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/surfaces/surface.py
+-rw-r--r--   0        0        0     4281 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/surfaces/surface_evaluation.py
+-rw-r--r--   0        0        0    16002 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/surfaces/torus.py
+-rw-r--r--   0        0        0     5694 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/surfaces/trimmed_surface.py
+-rw-r--r--   0        0        0     1909 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/__init__.py
+-rw-r--r--   0        0        0    15941 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/arc.py
+-rw-r--r--   0        0        0     6690 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/box.py
+-rw-r--r--   0        0        0     5139 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/circle.py
+-rw-r--r--   0        0        0     2991 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/edge.py
+-rw-r--r--   0        0        0     7734 2024-05-23 16:09:17.398956 ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/ellipse.py
+-rw-r--r--   0        0        0     3018 2024-05-23 16:09:17.402957 ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/face.py
+-rw-r--r--   0        0        0    19590 2024-05-23 16:09:17.402957 ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/gears.py
+-rw-r--r--   0        0        0     6063 2024-05-23 16:09:17.402957 ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/polygon.py
+-rw-r--r--   0        0        0     6076 2024-05-23 16:09:17.402957 ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/segment.py
+-rw-r--r--   0        0        0    34089 2024-05-23 16:09:17.402957 ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/sketch.py
+-rw-r--r--   0        0        0     6878 2024-05-23 16:09:17.402957 ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/slot.py
+-rw-r--r--   0        0        0     8286 2024-05-23 16:09:17.402957 ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/trapezoid.py
+-rw-r--r--   0        0        0     3847 2024-05-23 16:09:17.402957 ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/triangle.py
+-rw-r--r--   0        0        0     1550 2024-05-23 16:09:17.402957 ansys_geometry_core-0.5.6/src/ansys/geometry/core/tools/__init__.py
+-rw-r--r--   0        0        0     3856 2024-05-23 16:09:17.402957 ansys_geometry_core-0.5.6/src/ansys/geometry/core/tools/measurement_tools.py
+-rw-r--r--   0        0        0    14367 2024-05-23 16:09:17.402957 ansys_geometry_core-0.5.6/src/ansys/geometry/core/tools/problem_areas.py
+-rw-r--r--   0        0        0     2429 2024-05-23 16:09:17.402957 ansys_geometry_core-0.5.6/src/ansys/geometry/core/tools/repair_tool_message.py
+-rw-r--r--   0        0        0    10524 2024-05-23 16:09:17.402957 ansys_geometry_core-0.5.6/src/ansys/geometry/core/tools/repair_tools.py
+-rw-r--r--   0        0        0     1670 2024-05-23 16:09:17.402957 ansys_geometry_core-0.5.6/src/ansys/geometry/core/typing.py
+-rw-r--r--   0        0        0     9183 1970-01-01 00:00:00.000000 ansys_geometry_core-0.5.6/PKG-INFO
```

### Comparing `ansys_geometry_core-0.5.5/LICENSE` & `ansys_geometry_core-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/README.rst` & `ansys_geometry_core-0.5.6/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/pyproject.toml` & `ansys_geometry_core-0.5.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-geometry-core"
-version = "0.5.5"
+version = "0.5.6"
 description = "A python wrapper for Ansys Geometry service"
 readme = "README.rst"
 requires-python = ">=3.9,<4"
 license = { file = "LICENSE" }
 authors = [{ name = "ANSYS, Inc.", email = "pyansys.core@ansys.com" }]
 maintainers = [{ name = "ANSYS, Inc.", email = "pyansys.core@ansys.com" }]
 classifiers = [
@@ -29,15 +29,15 @@
     "beartype>=0.11.0,<0.19",
     "grpcio>=1.35.0,<2",
     "grpcio-health-checking>=1.45.0,<2",
     "numpy>=1.20.3,<2",
     "Pint>=0.18,<1",
     "protobuf>=3.20.2,<6",
     "pyvista>=0.37.0,<1",
-    "requests>=2,<2.32",
+    "requests>=2,<3",
     "scipy>=1.7.3,<2",
     "semver>=3,<4",
     "six>=1.16.0,<2",
     "vtk>=9,<10",
 ]
 
 [project.optional-dependencies]
@@ -46,52 +46,52 @@
     "docker>=6.0.1,<8",
     "pyvista[jupyter]>=0.38.1,<1",
 ]
 tests = [
     "ansys-platform-instancemanagement==1.1.2",
     "ansys-tools-path==0.5.2",
     "beartype==0.18.5",
-    "docker==7.0.0",
+    "docker==7.1.0",
     "grpcio==1.64.0",
     "grpcio-health-checking==1.60.0",
     "numpy==1.26.4",
     "Pint==0.23",
     "protobuf==5.26.1",
     "pytest==8.2.1",
     "pytest-cov==5.0.0",
     "pytest-pyvista==0.1.9",
     "pytest-xvfb==3.0.0",
     "pyvista[jupyter]==0.43.8",
-    "requests==2.31.0",
-    "scipy==1.13.0",
+    "requests==2.32.2",
+    "scipy==1.13.1",
     "semver==3.0.2",
     "six==1.16.0",
     "vtk==9.3.0",
 ]
 tests-minimal = [
     "pytest==8.2.1",
     "pytest-cov==5.0.0",
     "pytest-pyvista==0.1.9",
     "pytest-xvfb==3.0.0",
 ]
 doc = [
-    "ansys-sphinx-theme[autoapi]==0.16.0",
+    "ansys-sphinx-theme[autoapi]==0.16.2",
     "beartype==0.18.5",
-    "docker==7.0.0",
+    "docker==7.1.0",
     "ipyvtklink==0.2.3",
     "jupyter_sphinx==0.5.3",
     "jupytext==1.16.2",
     "myst-parser==3.0.1",
     "nbconvert==7.16.4",
     "nbsphinx==0.9.4",
     "notebook==7.2.0",
     "numpydoc==1.7.0",
     "panel==1.4.2",
     "pyvista[jupyter]==0.43.8",
-    "requests==2.31.0",
+    "requests==2.32.2",
     "sphinx==7.3.7",
     "sphinx-autodoc-typehints==1.24.0",
     "sphinx-copybutton==0.5.2",
     "sphinx-jinja==2.0.2",
     "trame-vtk==2.8.8",
     "vtk==9.3.0",
 ]
```

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/__init__.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/connection/__init__.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/connection/backend.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/connection/backend.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/connection/client.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/connection/client.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/connection/conversions.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/connection/conversions.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/connection/defaults.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/connection/defaults.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/connection/docker_instance.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/connection/docker_instance.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/connection/launcher.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/connection/launcher.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/connection/product_instance.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/connection/product_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,15 +359,15 @@
                 time.sleep(5)
 
     raise ConnectionError("Timeout while waiting for backend to be ready.")
 
 
 def _is_port_available(port: int, host: str = "localhost") -> bool:
     """
-    Check whether the argument port is available or not.
+    Check whether the argument port is available.
 
     The optional argument is the ip address where to check port availability.
     Its default is ``localhost``.
     """
     if port != 0:
         with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
             try:
```

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/connection/validate.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/connection/validate.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/designer/__init__.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/designer/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/designer/beam.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/designer/beam.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/designer/body.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/designer/body.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/designer/component.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/designer/component.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/designer/coordinate_system.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/designer/coordinate_system.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/designer/design.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/designer/design.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/designer/designpoint.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/designer/designpoint.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/designer/edge.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/designer/edge.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/designer/face.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/designer/face.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/designer/part.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/designer/part.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/designer/selection.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/designer/selection.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/errors.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/errors.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/logger.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/materials/__init__.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/materials/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/materials/material.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/materials/material.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/materials/property.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/materials/property.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/math/__init__.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/math/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,10 +35,11 @@
     ZERO_POINT2D,
     ZERO_POINT3D,
     ZERO_VECTOR2D,
     ZERO_VECTOR3D,
 )
 from ansys.geometry.core.math.frame import Frame
 from ansys.geometry.core.math.matrix import Matrix, Matrix33, Matrix44
+from ansys.geometry.core.math.misc import get_two_circle_intersections
 from ansys.geometry.core.math.plane import Plane
 from ansys.geometry.core.math.point import Point2D, Point3D
 from ansys.geometry.core.math.vector import UnitVector2D, UnitVector3D, Vector2D, Vector3D
```

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/math/bbox.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/math/bbox.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/math/constants.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/math/constants.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/math/frame.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/math/frame.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/math/matrix.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/math/matrix.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/math/plane.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/math/plane.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/math/point.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/math/point.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/math/vector.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/math/vector.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/misc/__init__.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/misc/accuracy.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/misc/accuracy.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/misc/auxiliary.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/misc/auxiliary.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/misc/checks.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/misc/checks.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/misc/measurements.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/misc/measurements.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/misc/options.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/misc/options.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/misc/units.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/misc/units.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/modeler.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/modeler.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/__init__.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/plotter.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/plotter.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/plotter_helper.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/plotter_helper.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/plotting_types.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/plotting_types.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/trame_gui.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/trame_gui.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/__init__.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/_images/designpoint.png` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/_images/designpoint.png`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/_images/downarrow.png` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/_images/downarrow.png`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/_images/isometric.png` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/_images/isometric.png`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/button.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/button.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/displace_arrows.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/displace_arrows.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/measure.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/measure.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/ruler.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/ruler.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/show_design_point.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/show_design_point.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/view_button.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/view_button.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/plotting/widgets/widget.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/plotting/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/__init__.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/box_uv.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/box_uv.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/curves/__init__.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/curves/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/curves/circle.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/curves/circle.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/curves/curve.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/curves/curve.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/curves/curve_evaluation.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/curves/curve_evaluation.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/curves/ellipse.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/curves/ellipse.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/curves/line.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/curves/line.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/curves/trimmed_curve.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/curves/trimmed_curve.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/parameterization.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/parameterization.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/surfaces/__init__.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/surfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/surfaces/cone.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/surfaces/cone.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/surfaces/cylinder.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/surfaces/cylinder.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/surfaces/plane.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/surfaces/plane.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/surfaces/sphere.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/surfaces/sphere.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/surfaces/surface.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/surfaces/surface.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/surfaces/surface_evaluation.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/surfaces/surface_evaluation.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/surfaces/torus.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/surfaces/torus.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Provides for creating and managing a torus."""
 
 from functools import cached_property
-from typing import Tuple
 
 from beartype import beartype as check_input_types
 from beartype.typing import Tuple, Union
 import numpy as np
 from pint import Quantity
 
 from ansys.geometry.core.math.constants import UNITVECTOR3D_X, UNITVECTOR3D_Z
```

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/shapes/surfaces/trimmed_surface.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/shapes/surfaces/trimmed_surface.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/__init__.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/arc.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/arc.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,24 +18,26 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Provides for creating and managing an arc."""
 
 from beartype import beartype as check_input_types
-from beartype.typing import Optional
+from beartype.typing import Optional, Union
 import numpy as np
 from pint import Quantity
 import pyvista as pv
 
+from ansys.geometry.core.math.matrix import Matrix
 from ansys.geometry.core.math.point import Point2D
 from ansys.geometry.core.math.vector import Vector2D
-from ansys.geometry.core.misc.measurements import DEFAULT_UNITS
+from ansys.geometry.core.misc.measurements import DEFAULT_UNITS, Angle, Distance
 from ansys.geometry.core.misc.units import UNITS
 from ansys.geometry.core.sketch.edge import SketchEdge
+from ansys.geometry.core.typing import Real
 
 
 class Arc(SketchEdge):
     """
     Provides for modeling an arc.
 
     Parameters
@@ -266,14 +268,15 @@
             end_point,
             center_point,
         )
 
         return arc_sub1 + arc_sub2
 
     @classmethod
+    @check_input_types
     def from_three_points(cls, start: Point2D, inter: Point2D, end: Point2D):
         """
         Create an arc from three given points.
 
         Parameters
         ----------
         start : Point2D
@@ -338,7 +341,126 @@
         angle_s_i = Vector2D.get_angle_between(center_start, center_inter)
         angle_s_e = Vector2D.get_angle_between(center_start, center_end)
 
         is_clockwise = False if angle_s_i < angle_s_e else True
 
         # Finally... you can create the arc
         return Arc(start=start, end=end, center=center, clockwise=is_clockwise)
+
+    @classmethod
+    @check_input_types
+    def from_start_end_and_radius(
+        cls,
+        start: Point2D,
+        end: Point2D,
+        radius: Union[Quantity, Distance, Real],
+        convex_arc: Optional[bool] = False,
+        clockwise: Optional[bool] = False,
+    ):
+        """
+        Create an arc from a starting point, an ending point, and a radius.
+
+        Parameters
+        ----------
+        start : Point2D
+            Starting point of the arc.
+        end : Point2D
+            Ending point of the arc.
+        radius : Union[Quantity, Distance, Real]
+            Radius of the arc.
+        convex_arc : bool, default: False
+            Whether the arc is convex. The default is ``False``.
+            When ``False``, the arc is concave. When ``True``, the arc is convex.
+        clockwise : bool, default: False
+            Whether the arc spans the clockwise angle between the start and end points.
+            When ``False``, the arc spans the counter-clockwise angle.
+            When ``True``, the arc spands the clockwise angle.
+
+        Returns
+        -------
+        Arc
+            Arc generated from the three points.
+        """
+        # Compute the potential centers of the circle
+        # that could generate the arc
+        from ansys.geometry.core.math.misc import get_two_circle_intersections
+
+        # Sanitize the radius
+        radius = radius if isinstance(radius, Distance) else Distance(radius)
+        if radius.value <= 0:
+            raise ValueError("Radius must be a real positive value.")
+
+        # Unpack the points into its coordinates (in DEFAULT_UNITS.LENGTH)
+        x_s, y_s = start.tolist()
+        x_e, y_e = end.tolist()
+        r0 = r1 = radius.value.m_as(DEFAULT_UNITS.LENGTH)
+
+        # Compute the potential centers of the circle
+        centers = get_two_circle_intersections(x0=x_s, y0=y_s, r0=r0, x1=x_e, y1=y_e, r1=r1)
+        if centers is None:
+            raise ValueError("The provided points and radius do not yield a valid arc.")
+
+        # Choose the center depending on if the arc is convex
+        center = Point2D(centers[1] if convex_arc else centers[0])
+
+        # Create the arc
+        return Arc(start=start, end=end, center=center, clockwise=clockwise)
+
+    @classmethod
+    @check_input_types
+    def from_start_center_and_angle(
+        cls,
+        start: Point2D,
+        center: Point2D,
+        angle: Union[Angle, Quantity, Real],
+        clockwise: Optional[bool] = False,
+    ):
+        """
+        Create an arc from a starting point, a center point, and an angle.
+
+        Parameters
+        ----------
+        start : Point2D
+            Starting point of the arc.
+        center : Point2D
+            Center point of the arc.
+        angle : Union[Angle, Quantity, Real]
+            Angle of the arc.
+        clockwise : bool, default: False
+            Whether the provided angle should be considered clockwise.
+            When ``False``, the angle is considered counter-clockwise.
+            When ``True``, the angle is considered clockwise.
+
+        Returns
+        -------
+        Arc
+            Arc generated from the three points.
+        """
+        # Define a 2D vector from the center to the start point
+        to_start_vector = Vector2D.from_points(center, start)
+
+        # Perform sanity check for the angle
+        angle = angle if isinstance(angle, Angle) else Angle(angle)
+        rad_angle = angle.value.m_as(UNITS.radian)
+        cang = np.cos(rad_angle)
+        sang = np.sin(rad_angle)
+
+        # Rotate the vector by the angle
+        if clockwise:
+            rot_matrix = Matrix([[cang, sang], [-sang, cang]])
+        else:
+            rot_matrix = Matrix([[cang, -sang], [sang, cang]])
+
+        # Compute the end vector
+        to_end_vector = rot_matrix @ to_start_vector
+
+        # Define the end point
+        end = Point2D(
+            [
+                to_end_vector[0] + center.x.to_base_units().m,
+                to_end_vector[1] + center.y.to_base_units().m,
+            ],
+            center.base_unit,
+        )
+
+        # Create the arc
+        return Arc(start=start, end=end, center=center, clockwise=clockwise)
```

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/box.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/box.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/circle.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/circle.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/edge.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/edge.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/ellipse.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/ellipse.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/face.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/face.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/gears.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/gears.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/polygon.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/polygon.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/segment.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/segment.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/sketch.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/sketch.py`

 * *Files 8% similar despite different names*

```diff
@@ -481,14 +481,97 @@
         -------
         Sketch
             Revised sketch state ready for further sketch actions.
         """
         arc = Arc.from_three_points(start, inter, end)
         return self.edge(arc, tag)
 
+    def arc_from_start_end_and_radius(
+        self,
+        start: Point2D,
+        end: Point2D,
+        radius: Union[Quantity, Distance, Real],
+        convex_arc: Optional[bool] = False,
+        clockwise: Optional[bool] = False,
+        tag: Optional[str] = None,
+    ) -> "Sketch":
+        """
+        Add an arc to the sketch plane from the start and end points and a given radius.
+
+        Parameters
+        ----------
+        start : Point2D
+            Starting point of the arc.
+        end : Point2D
+            Ending point of the arc.
+        radius : Union[~pint.Quantity, Distance, Real]
+            Radius of the arc.
+        convex_arc : bool, default: False
+            Whether the arc is convex. The default is ``False``.
+            When ``False`` , the arc spans the concave version of the arc.
+            When ``True``, the arc spans the convex version of the arc.
+        clockwise : bool, default: False
+            Whether the arc spans the angle clockwise between the start
+            and end points. When ``False``, the arc spans the angle
+            counter-clockwise. When ``True``, the arc spans the angle
+            clockwise.
+        tag : str, default: None
+            User-defined label for identifying the edge.
+
+        Returns
+        -------
+        Sketch
+            Revised sketch state ready for further sketch actions.
+        """
+        arc = Arc.from_start_end_and_radius(
+            start,
+            end,
+            radius,
+            convex_arc=convex_arc,
+            clockwise=clockwise,
+        )
+        return self.edge(arc, tag)
+
+    def arc_from_start_center_and_angle(
+        self,
+        start: Point2D,
+        center: Point2D,
+        angle: Union[Quantity, Angle, Real],
+        clockwise: Optional[bool] = False,
+        tag: Optional[str] = None,
+    ) -> "Sketch":
+        """
+        Add an arc to the sketch plane from the start, center point, and angle.
+
+        Parameters
+        ----------
+        start : Point2D
+            Starting point of the arc.
+        center : Point2D
+            Center point of the arc.
+        angle : Union[~pint.Quantity, Angle, Real]
+            Angle of the arc.
+        clockwise : bool, default: False
+            Whether the arc spans the angle clockwise. The default is ``False``.
+            When ``False`` , the arc spans the angle counter-clockwise.
+            When ``True``, the arc spans the angle clockwise.
+
+        Returns
+        -------
+        Sketch
+            Revised sketch state ready for further sketch actions.
+        """
+        arc = Arc.from_start_center_and_angle(
+            start,
+            center,
+            angle,
+            clockwise=clockwise,
+        )
+        return self.edge(arc, tag)
+
     def triangle(
         self,
         point1: Point2D,
         point2: Point2D,
         point3: Point2D,
         tag: Optional[str] = None,
     ) -> "Sketch":
```

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/slot.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/slot.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/trapezoid.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/trapezoid.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/sketch/triangle.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/sketch/triangle.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/tools/__init__.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/tools/measurement_tools.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/tools/measurement_tools.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/tools/problem_areas.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/tools/problem_areas.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/tools/repair_tool_message.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/tools/repair_tool_message.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/tools/repair_tools.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/tools/repair_tools.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/src/ansys/geometry/core/typing.py` & `ansys_geometry_core-0.5.6/src/ansys/geometry/core/typing.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.5/PKG-INFO` & `ansys_geometry_core-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-geometry-core
-Version: 0.5.5
+Version: 0.5.6
 Summary: A python wrapper for Ansys Geometry service
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -20,58 +20,58 @@
 Requires-Dist: beartype>=0.11.0,<0.19
 Requires-Dist: grpcio>=1.35.0,<2
 Requires-Dist: grpcio-health-checking>=1.45.0,<2
 Requires-Dist: numpy>=1.20.3,<2
 Requires-Dist: Pint>=0.18,<1
 Requires-Dist: protobuf>=3.20.2,<6
 Requires-Dist: pyvista>=0.37.0,<1
-Requires-Dist: requests>=2,<2.32
+Requires-Dist: requests>=2,<3
 Requires-Dist: scipy>=1.7.3,<2
 Requires-Dist: semver>=3,<4
 Requires-Dist: six>=1.16.0,<2
 Requires-Dist: vtk>=9,<10
 Requires-Dist: ansys-platform-instancemanagement>=1.0.3,<2 ; extra == "all"
 Requires-Dist: docker>=6.0.1,<8 ; extra == "all"
 Requires-Dist: pyvista[jupyter]>=0.38.1,<1 ; extra == "all"
-Requires-Dist: ansys-sphinx-theme[autoapi]==0.16.0 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme[autoapi]==0.16.2 ; extra == "doc"
 Requires-Dist: beartype==0.18.5 ; extra == "doc"
-Requires-Dist: docker==7.0.0 ; extra == "doc"
+Requires-Dist: docker==7.1.0 ; extra == "doc"
 Requires-Dist: ipyvtklink==0.2.3 ; extra == "doc"
 Requires-Dist: jupyter_sphinx==0.5.3 ; extra == "doc"
 Requires-Dist: jupytext==1.16.2 ; extra == "doc"
 Requires-Dist: myst-parser==3.0.1 ; extra == "doc"
 Requires-Dist: nbconvert==7.16.4 ; extra == "doc"
 Requires-Dist: nbsphinx==0.9.4 ; extra == "doc"
 Requires-Dist: notebook==7.2.0 ; extra == "doc"
 Requires-Dist: numpydoc==1.7.0 ; extra == "doc"
 Requires-Dist: panel==1.4.2 ; extra == "doc"
 Requires-Dist: pyvista[jupyter]==0.43.8 ; extra == "doc"
-Requires-Dist: requests==2.31.0 ; extra == "doc"
+Requires-Dist: requests==2.32.2 ; extra == "doc"
 Requires-Dist: sphinx==7.3.7 ; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints==1.24.0 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx-jinja==2.0.2 ; extra == "doc"
 Requires-Dist: trame-vtk==2.8.8 ; extra == "doc"
 Requires-Dist: vtk==9.3.0 ; extra == "doc"
 Requires-Dist: ansys-platform-instancemanagement==1.1.2 ; extra == "tests"
 Requires-Dist: ansys-tools-path==0.5.2 ; extra == "tests"
 Requires-Dist: beartype==0.18.5 ; extra == "tests"
-Requires-Dist: docker==7.0.0 ; extra == "tests"
+Requires-Dist: docker==7.1.0 ; extra == "tests"
 Requires-Dist: grpcio==1.64.0 ; extra == "tests"
 Requires-Dist: grpcio-health-checking==1.60.0 ; extra == "tests"
 Requires-Dist: numpy==1.26.4 ; extra == "tests"
 Requires-Dist: Pint==0.23 ; extra == "tests"
 Requires-Dist: protobuf==5.26.1 ; extra == "tests"
 Requires-Dist: pytest==8.2.1 ; extra == "tests"
 Requires-Dist: pytest-cov==5.0.0 ; extra == "tests"
 Requires-Dist: pytest-pyvista==0.1.9 ; extra == "tests"
 Requires-Dist: pytest-xvfb==3.0.0 ; extra == "tests"
 Requires-Dist: pyvista[jupyter]==0.43.8 ; extra == "tests"
-Requires-Dist: requests==2.31.0 ; extra == "tests"
-Requires-Dist: scipy==1.13.0 ; extra == "tests"
+Requires-Dist: requests==2.32.2 ; extra == "tests"
+Requires-Dist: scipy==1.13.1 ; extra == "tests"
 Requires-Dist: semver==3.0.2 ; extra == "tests"
 Requires-Dist: six==1.16.0 ; extra == "tests"
 Requires-Dist: vtk==9.3.0 ; extra == "tests"
 Requires-Dist: pytest==8.2.1 ; extra == "tests-minimal"
 Requires-Dist: pytest-cov==5.0.0 ; extra == "tests-minimal"
 Requires-Dist: pytest-pyvista==0.1.9 ; extra == "tests-minimal"
 Requires-Dist: pytest-xvfb==3.0.0 ; extra == "tests-minimal"
```

