# Comparing `tmp/ansys_geometry_core-0.5.0.tar.gz` & `tmp/ansys_geometry_core-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_geometry_core-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_geometry_core-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_geometry_core-0.5.0.tar` & `ansys_geometry_core-0.5.1.tar`

### file list

```diff
@@ -1,113 +1,113 @@
--rw-r--r--   0        0        0     1089 2024-04-17 07:07:51.897322 ansys_geometry_core-0.5.0/LICENSE
--rw-r--r--   0        0        0     5051 2024-04-17 07:07:51.897322 ansys_geometry_core-0.5.0/README.rst
--rw-r--r--   0        0        0     4395 2024-04-17 07:07:51.901322 ansys_geometry_core-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2762 2024-04-17 07:07:51.901322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/__init__.py
--rw-r--r--   0        0        0     2477 2024-04-17 07:07:51.901322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/__init__.py
--rw-r--r--   0        0        0     1618 2024-04-17 07:07:51.901322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/backend.py
--rw-r--r--   0        0        0    12286 2024-04-17 07:07:51.901322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/client.py
--rw-r--r--   0        0        0    18876 2024-04-17 07:07:51.901322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/conversions.py
--rw-r--r--   0        0        0     2483 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/defaults.py
--rw-r--r--   0        0        0    13911 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/docker_instance.py
--rw-r--r--   0        0        0    28218 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/launcher.py
--rw-r--r--   0        0        0      167 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/pim_configuration.json
--rw-r--r--   0        0        0    16343 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/product_instance.py
--rw-r--r--   0        0        0     1776 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/validate.py
--rw-r--r--   0        0        0     1782 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/__init__.py
--rw-r--r--   0        0        0     7898 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/beam.py
--rw-r--r--   0        0        0    46126 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/body.py
--rw-r--r--   0        0        0    52507 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/component.py
--rw-r--r--   0        0        0     6034 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/coordinate_system.py
--rw-r--r--   0        0        0    33930 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/design.py
--rw-r--r--   0        0        0     3697 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/designpoint.py
--rw-r--r--   0        0        0     6069 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/edge.py
--rw-r--r--   0        0        0    13956 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/face.py
--rw-r--r--   0        0        0     5468 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/part.py
--rw-r--r--   0        0        0     4686 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/selection.py
--rw-r--r--   0        0        0     4101 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/errors.py
--rw-r--r--   0        0        0    22524 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/logger.py
--rw-r--r--   0        0        0     1349 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/materials/__init__.py
--rw-r--r--   0        0        0     3268 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/materials/material.py
--rw-r--r--   0        0        0     4107 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/materials/property.py
--rw-r--r--   0        0        0     1883 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/__init__.py
--rw-r--r--   0        0        0     6819 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/bbox.py
--rw-r--r--   0        0        0     3259 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/constants.py
--rw-r--r--   0        0        0     7035 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/frame.py
--rw-r--r--   0        0        0     4823 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/matrix.py
--rw-r--r--   0        0        0     4240 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/plane.py
--rw-r--r--   0        0        0    12120 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/point.py
--rw-r--r--   0        0        0    18024 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/vector.py
--rw-r--r--   0        0        0     2085 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/__init__.py
--rw-r--r--   0        0        0     8033 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/accuracy.py
--rw-r--r--   0        0        0     5215 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/auxiliary.py
--rw-r--r--   0        0        0    12180 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/checks.py
--rw-r--r--   0        0        0     8253 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/measurements.py
--rw-r--r--   0        0        0     2291 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/options.py
--rw-r--r--   0        0        0     3684 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/units.py
--rw-r--r--   0        0        0    17075 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/modeler.py
--rw-r--r--   0        0        0     1417 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/__init__.py
--rw-r--r--   0        0        0    22179 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/plotter.py
--rw-r--r--   0        0        0    14013 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/plotter_helper.py
--rw-r--r--   0        0        0     5826 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/plotting_types.py
--rw-r--r--   0        0        0     2816 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/trame_gui.py
--rw-r--r--   0        0        0     1710 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/__init__.py
--rw-r--r--   0        0        0      499 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/+xy.png
--rw-r--r--   0        0        0      487 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/+xz.png
--rw-r--r--   0        0        0      497 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/+yz.png
--rw-r--r--   0        0        0      496 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/-xy.png
--rw-r--r--   0        0        0      484 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/-xz.png
--rw-r--r--   0        0        0      495 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/-yz.png
--rw-r--r--   0        0        0      569 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/designpoint.png
--rw-r--r--   0        0        0      526 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/downarrow.png
--rw-r--r--   0        0        0      725 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/isometric.png
--rw-r--r--   0        0        0      339 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/measurement.png
--rw-r--r--   0        0        0      341 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/ruler.png
--rw-r--r--   0        0        0      451 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/upxarrow.png
--rw-r--r--   0        0        0      442 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/upyarrow.png
--rw-r--r--   0        0        0      428 2024-04-17 07:07:51.905322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/upzarrow.png
--rw-r--r--   0        0        0     3058 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/button.py
--rw-r--r--   0        0        0     4239 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/displace_arrows.py
--rw-r--r--   0        0        0     3626 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/measure.py
--rw-r--r--   0        0        0     3700 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/ruler.py
--rw-r--r--   0        0        0     3480 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/show_design_point.py
--rw-r--r--   0        0        0     3348 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/view_button.py
--rw-r--r--   0        0        0     2305 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/widget.py
--rw-r--r--   0        0        0     2176 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/__init__.py
--rw-r--r--   0        0        0     5634 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/box_uv.py
--rw-r--r--   0        0        0     1580 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/__init__.py
--rw-r--r--   0        0        0    11617 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/circle.py
--rw-r--r--   0        0        0     3539 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/curve.py
--rw-r--r--   0        0        0     2767 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/curve_evaluation.py
--rw-r--r--   0        0        0    14319 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/ellipse.py
--rw-r--r--   0        0        0     8893 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/line.py
--rw-r--r--   0        0        0     7428 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/trimmed_curve.py
--rw-r--r--   0        0        0    13001 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/parameterization.py
--rw-r--r--   0        0        0     1746 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/__init__.py
--rw-r--r--   0        0        0    14274 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/cone.py
--rw-r--r--   0        0        0    14748 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/cylinder.py
--rw-r--r--   0        0        0     8067 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/plane.py
--rw-r--r--   0        0        0    13257 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/sphere.py
--rw-r--r--   0        0        0     3467 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/surface.py
--rw-r--r--   0        0        0     4281 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/surface_evaluation.py
--rw-r--r--   0        0        0    16027 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/torus.py
--rw-r--r--   0        0        0     5694 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/trimmed_surface.py
--rw-r--r--   0        0        0     1909 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/__init__.py
--rw-r--r--   0        0        0    11643 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/arc.py
--rw-r--r--   0        0        0     6690 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/box.py
--rw-r--r--   0        0        0     5139 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/circle.py
--rw-r--r--   0        0        0     2991 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/edge.py
--rw-r--r--   0        0        0     7734 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/ellipse.py
--rw-r--r--   0        0        0     3018 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/face.py
--rw-r--r--   0        0        0    19590 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/gears.py
--rw-r--r--   0        0        0     6063 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/polygon.py
--rw-r--r--   0        0        0     6076 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/segment.py
--rw-r--r--   0        0        0    31342 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/sketch.py
--rw-r--r--   0        0        0     6878 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/slot.py
--rw-r--r--   0        0        0     8286 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/trapezoid.py
--rw-r--r--   0        0        0     3847 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/triangle.py
--rw-r--r--   0        0        0     1550 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/tools/__init__.py
--rw-r--r--   0        0        0     3856 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/tools/measurement_tools.py
--rw-r--r--   0        0        0    14367 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/tools/problem_areas.py
--rw-r--r--   0        0        0     2429 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/tools/repair_tool_message.py
--rw-r--r--   0        0        0    10524 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/tools/repair_tools.py
--rw-r--r--   0        0        0     1670 2024-04-17 07:07:51.909322 ansys_geometry_core-0.5.0/src/ansys/geometry/core/typing.py
--rw-r--r--   0        0        0     9057 1970-01-01 00:00:00.000000 ansys_geometry_core-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-24 15:03:14.635642 ansys_geometry_core-0.5.1/LICENSE
+-rw-r--r--   0        0        0     5051 2024-04-24 15:03:14.635642 ansys_geometry_core-0.5.1/README.rst
+-rw-r--r--   0        0        0     4373 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2762 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/__init__.py
+-rw-r--r--   0        0        0     2477 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/__init__.py
+-rw-r--r--   0        0        0     1618 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/backend.py
+-rw-r--r--   0        0        0    12286 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/client.py
+-rw-r--r--   0        0        0    18876 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/conversions.py
+-rw-r--r--   0        0        0     2483 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/defaults.py
+-rw-r--r--   0        0        0    13911 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/docker_instance.py
+-rw-r--r--   0        0        0    28217 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/launcher.py
+-rw-r--r--   0        0        0      167 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/pim_configuration.json
+-rw-r--r--   0        0        0    16343 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/product_instance.py
+-rw-r--r--   0        0        0     1776 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/validate.py
+-rw-r--r--   0        0        0     1782 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/__init__.py
+-rw-r--r--   0        0        0     7898 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/beam.py
+-rw-r--r--   0        0        0    46126 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/body.py
+-rw-r--r--   0        0        0    52507 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/component.py
+-rw-r--r--   0        0        0     6034 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/coordinate_system.py
+-rw-r--r--   0        0        0    40126 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/design.py
+-rw-r--r--   0        0        0     3697 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/designpoint.py
+-rw-r--r--   0        0        0     6069 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/edge.py
+-rw-r--r--   0        0        0    13956 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/face.py
+-rw-r--r--   0        0        0     5468 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/part.py
+-rw-r--r--   0        0        0     4686 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/selection.py
+-rw-r--r--   0        0        0     4101 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/errors.py
+-rw-r--r--   0        0        0    22524 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/logger.py
+-rw-r--r--   0        0        0     1349 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/materials/__init__.py
+-rw-r--r--   0        0        0     3268 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/materials/material.py
+-rw-r--r--   0        0        0     4107 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/materials/property.py
+-rw-r--r--   0        0        0     1883 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/__init__.py
+-rw-r--r--   0        0        0     6819 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/bbox.py
+-rw-r--r--   0        0        0     3259 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/constants.py
+-rw-r--r--   0        0        0     7035 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/frame.py
+-rw-r--r--   0        0        0     4823 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/matrix.py
+-rw-r--r--   0        0        0     4240 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/plane.py
+-rw-r--r--   0        0        0    12120 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/point.py
+-rw-r--r--   0        0        0    18024 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/vector.py
+-rw-r--r--   0        0        0     2085 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/__init__.py
+-rw-r--r--   0        0        0     8033 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/accuracy.py
+-rw-r--r--   0        0        0     5215 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/auxiliary.py
+-rw-r--r--   0        0        0    12745 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/checks.py
+-rw-r--r--   0        0        0     8253 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/measurements.py
+-rw-r--r--   0        0        0     2291 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/options.py
+-rw-r--r--   0        0        0     3684 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/units.py
+-rw-r--r--   0        0        0    17075 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/modeler.py
+-rw-r--r--   0        0        0     1417 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/__init__.py
+-rw-r--r--   0        0        0    22177 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/plotter.py
+-rw-r--r--   0        0        0    15007 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/plotter_helper.py
+-rw-r--r--   0        0        0     5826 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/plotting_types.py
+-rw-r--r--   0        0        0     4213 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/trame_gui.py
+-rw-r--r--   0        0        0     1710 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/__init__.py
+-rw-r--r--   0        0        0      499 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/+xy.png
+-rw-r--r--   0        0        0      487 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/+xz.png
+-rw-r--r--   0        0        0      497 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/+yz.png
+-rw-r--r--   0        0        0      496 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/-xy.png
+-rw-r--r--   0        0        0      484 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/-xz.png
+-rw-r--r--   0        0        0      495 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/-yz.png
+-rw-r--r--   0        0        0      569 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/designpoint.png
+-rw-r--r--   0        0        0      526 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/downarrow.png
+-rw-r--r--   0        0        0      725 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/isometric.png
+-rw-r--r--   0        0        0      339 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/measurement.png
+-rw-r--r--   0        0        0      341 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/ruler.png
+-rw-r--r--   0        0        0      451 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/upxarrow.png
+-rw-r--r--   0        0        0      442 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/upyarrow.png
+-rw-r--r--   0        0        0      428 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/upzarrow.png
+-rw-r--r--   0        0        0     3058 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/button.py
+-rw-r--r--   0        0        0     4239 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/displace_arrows.py
+-rw-r--r--   0        0        0     3626 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/measure.py
+-rw-r--r--   0        0        0     3700 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/ruler.py
+-rw-r--r--   0        0        0     3480 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/show_design_point.py
+-rw-r--r--   0        0        0     3348 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/view_button.py
+-rw-r--r--   0        0        0     2305 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/widget.py
+-rw-r--r--   0        0        0     2176 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/__init__.py
+-rw-r--r--   0        0        0     5634 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/box_uv.py
+-rw-r--r--   0        0        0     1580 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/__init__.py
+-rw-r--r--   0        0        0    11617 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/circle.py
+-rw-r--r--   0        0        0     3539 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/curve.py
+-rw-r--r--   0        0        0     2767 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/curve_evaluation.py
+-rw-r--r--   0        0        0    14319 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/ellipse.py
+-rw-r--r--   0        0        0     8893 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/line.py
+-rw-r--r--   0        0        0     7428 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/trimmed_curve.py
+-rw-r--r--   0        0        0    13001 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/parameterization.py
+-rw-r--r--   0        0        0     1746 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/__init__.py
+-rw-r--r--   0        0        0    14274 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/cone.py
+-rw-r--r--   0        0        0    14748 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/cylinder.py
+-rw-r--r--   0        0        0     8067 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/plane.py
+-rw-r--r--   0        0        0    13257 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/sphere.py
+-rw-r--r--   0        0        0     3467 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/surface.py
+-rw-r--r--   0        0        0     4281 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/surface_evaluation.py
+-rw-r--r--   0        0        0    16027 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/torus.py
+-rw-r--r--   0        0        0     5694 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/trimmed_surface.py
+-rw-r--r--   0        0        0     1909 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/__init__.py
+-rw-r--r--   0        0        0    11643 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/arc.py
+-rw-r--r--   0        0        0     6690 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/box.py
+-rw-r--r--   0        0        0     5139 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/circle.py
+-rw-r--r--   0        0        0     2991 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/edge.py
+-rw-r--r--   0        0        0     7734 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/ellipse.py
+-rw-r--r--   0        0        0     3018 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/face.py
+-rw-r--r--   0        0        0    19590 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/gears.py
+-rw-r--r--   0        0        0     6063 2024-04-24 15:03:14.651642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/polygon.py
+-rw-r--r--   0        0        0     6076 2024-04-24 15:03:14.651642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/segment.py
+-rw-r--r--   0        0        0    31342 2024-04-24 15:03:14.651642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/sketch.py
+-rw-r--r--   0        0        0     6878 2024-04-24 15:03:14.651642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/slot.py
+-rw-r--r--   0        0        0     8286 2024-04-24 15:03:14.651642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/trapezoid.py
+-rw-r--r--   0        0        0     3847 2024-04-24 15:03:14.651642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/triangle.py
+-rw-r--r--   0        0        0     1550 2024-04-24 15:03:14.651642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/tools/__init__.py
+-rw-r--r--   0        0        0     3856 2024-04-24 15:03:14.651642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/tools/measurement_tools.py
+-rw-r--r--   0        0        0    14367 2024-04-24 15:03:14.651642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/tools/problem_areas.py
+-rw-r--r--   0        0        0     2429 2024-04-24 15:03:14.651642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/tools/repair_tool_message.py
+-rw-r--r--   0        0        0    10524 2024-04-24 15:03:14.651642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/tools/repair_tools.py
+-rw-r--r--   0        0        0     1670 2024-04-24 15:03:14.651642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/typing.py
+-rw-r--r--   0        0        0     9167 1970-01-01 00:00:00.000000 ansys_geometry_core-0.5.1/PKG-INFO
```

### Comparing `ansys_geometry_core-0.5.0/LICENSE` & `ansys_geometry_core-0.5.1/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 MIT License
 
-Copyright (c) 2022 ANSYS, Inc. All rights reserved.
+Copyright (c) 2023 - 2024 ANSYS, Inc. and/or its affiliates.
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+of the Software, and to permit persons to whom the Software is furnished to do
+so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
```

### Comparing `ansys_geometry_core-0.5.0/README.rst` & `ansys_geometry_core-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/pyproject.toml` & `ansys_geometry_core-0.5.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-geometry-core"
-version = "0.5.0"
+version = "0.5.1"
 description = "A python wrapper for Ansys Geometry service"
 readme = "README.rst"
 requires-python = ">=3.9,<4"
 license = { file = "LICENSE" }
 authors = [{ name = "ANSYS, Inc.", email = "pyansys.core@ansys.com" }]
 maintainers = [{ name = "ANSYS, Inc.", email = "pyansys.core@ansys.com" }]
 classifiers = [
@@ -23,76 +23,80 @@
     "Programming Language :: Python :: 3.12",
 ]
 
 dependencies = [
     "ansys-api-geometry==0.4.1",
     "ansys-tools-path>=0.3,<1",
     "beartype>=0.11.0,<0.19",
-    "google-api-python-client>=1.7.11,<3",
-    "googleapis-common-protos>=1.52.0,<2",
     "grpcio>=1.35.0,<2",
     "grpcio-health-checking>=1.45.0,<2",
     "numpy>=1.20.3,<2",
     "Pint>=0.18,<1",
-    "protobuf>=3.20.2,<5",
+    "protobuf>=3.20.2,<6",
     "pyvista>=0.37.0,<1",
+    "requests>=2,<3",
     "scipy>=1.7.3,<2",
+    "semver>=3,<4",
     "six>=1.16.0,<2",
     "vtk>=9,<10",
-    "semver>=3,<4",
 ]
 
 [project.optional-dependencies]
 all = [
     "ansys-platform-instancemanagement>=1.0.3,<2",
     "docker>=6.0.1,<8",
-    "pyvista[jupyter]>=0.38.1,<0.42",
+    "pyvista[jupyter]>=0.38.1,<1",
 ]
 tests = [
     "ansys-platform-instancemanagement==1.1.2",
-    "ansys-tools-path==0.5.1",
-    "beartype==0.18.2",
+    "ansys-tools-path==0.5.2",
+    "beartype==0.18.5",
     "docker==7.0.0",
-    "google-api-python-client==2.122.0",
-    "googleapis-common-protos==1.63.0",
-    "grpcio==1.62.1",
+    "grpcio==1.62.2",
     "grpcio-health-checking==1.60.0",
     "numpy==1.26.4",
     "Pint==0.23",
-    "protobuf==4.25.1",
+    "protobuf==5.26.1",
     "pytest==8.1.1",
     "pytest-cov==5.0.0",
     "pytest-pyvista==0.1.9",
     "pytest-xvfb==3.0.0",
     "pyvista[jupyter]==0.43.5",
     "requests==2.31.0",
     "scipy==1.13.0",
     "semver==3.0.2",
     "six==1.16.0",
     "vtk==9.3.0",
 ]
+tests-minimal = [
+    "pytest==8.1.1",
+    "pytest-cov==5.0.0",
+    "pytest-pyvista==0.1.9",
+    "pytest-xvfb==3.0.0",
+]
 doc = [
     "ansys-sphinx-theme[autoapi]==0.15.2",
-    "beartype==0.18.2",
+    "beartype==0.18.5",
     "docker==7.0.0",
     "ipyvtklink==0.2.3",
     "jupyter_sphinx==0.5.3",
     "jupytext==1.16.1",
     "myst-parser==2.0.0",
     "nbconvert==7.16.3",
     "nbsphinx==0.9.3",
-    "notebook==7.1.2",
+    "notebook==7.1.3",
     "numpydoc==1.7.0",
     "panel==1.4.1",
     "pyvista[jupyter]==0.43.5",
     "requests==2.31.0",
     "sphinx==7.2.6",
     "sphinx-autodoc-typehints==1.24.0",
     "sphinx-copybutton==0.5.2",
     "sphinx-jinja==2.0.2",
+    "trame-vtk==2.8.6",
     "vtk==9.3.0",
 ]
 
 [project.urls]
 Source = "https://github.com/ansys/pyansys-geometry"
 Issues = "https://github.com/ansys/pyansys-geometry/issues"
 Discussions = "https://github.com/ansys/pyansys-geometry/discussions"
@@ -127,20 +131,19 @@
 [tool.pytest.ini_options]
 minversion = "7.1"
 addopts = "-ra --cov=ansys.geometry --cov-report html:.cov/html --cov-report xml:.cov/xml --cov-report term -vv --image_cache_dir tests/integration/image_cache --add_missing_images"
 testpaths = ["tests"]
 
 [tool.towncrier]
 directory = "doc/changelog.d"
-filename = "CHANGELOG.md"
-start_string = "<!-- towncrier release notes start -->\n"
-underlines = ["", "", ""]
+filename = "doc/source/changelog.rst"
 template = "doc/changelog.d/changelog_template.jinja"
-title_format = "## [{version}](https://github.com/ansys/pyansys-geometry/releases/tag/v{version}) - {project_date}"
-issue_format = "[#{issue}](https://github.com/ansys/pyansys-geometry/pull/{issue})"
+start_string = ".. towncrier release notes start\n"
+title_format = "`{version} <https://github.com/ansys/pyansys-geometry/releases/tag/v{version}>`_ - {project_date}"
+issue_format = "`#{issue} <https://github.com/ansys/pyansys-geometry/pull/{issue}>`_"
 
 [[tool.towncrier.type]]
 directory = "added"
 name = "Added"
 showcontent = true
 
 [[tool.towncrier.type]]
```

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/__init__.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/__init__.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/backend.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/backend.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/client.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/client.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/conversions.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/conversions.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/defaults.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/defaults.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/docker_instance.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/docker_instance.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/launcher.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/launcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -497,15 +497,15 @@
     hidden: bool = False,
 ):
     """
     Start Ansys Discovery locally using the ``ProductInstance`` class.
 
     .. note::
 
-       Support for Ansys Discovery is restricted to Ansys 24.1 onwards.
+       Support for Ansys Discovery is restricted to Ansys 24.1 onward.
 
     When calling this method, a standalone Discovery session is started.
     By default, if an endpoint is specified (by defining `host` and `port` parameters)
     but the endpoint is not available, the startup will fail. Otherwise, it will try to
     launch its own service.
 
     Parameters
```

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/product_instance.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/product_instance.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/connection/validate.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/validate.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/__init__.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/beam.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/beam.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/body.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/body.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/component.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/component.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/coordinate_system.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/coordinate_system.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/design.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/design.py`

 * *Files 18% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 from ansys.api.geometry.v0.parts_pb2_grpc import PartsStub
 from beartype import beartype as check_input_types
 from beartype.typing import Dict, List, Optional, Union
 from google.protobuf.empty_pb2 import Empty
 import numpy as np
 from pint import Quantity, UndefinedUnitError
 
+from ansys.geometry.core.connection.backend import BackendType
 from ansys.geometry.core.connection.conversions import (
     grpc_frame_to_frame,
     grpc_matrix_to_matrix,
     plane_to_grpc_plane,
     point3d_to_grpc_point,
 )
 from ansys.geometry.core.designer.beam import Beam, BeamCircularProfile, BeamProfile
@@ -249,21 +250,21 @@
         ----------
         file_location : Union[~pathlib.Path, str]
             Location on disk to save the file to.
         format :DesignFileFormat, default: DesignFileFormat.SCDOCX
             Format for the file to save to.
         """
         # Sanity checks on inputs
-        if isinstance(file_location, Path):
-            file_location = str(file_location)
+        if isinstance(file_location, str):
+            file_location = Path(file_location)
 
         # Check if the folder for the file location exists
-        if not Path(file_location).parent.exists():
+        if not file_location.parent.exists():
             # Create the parent directory
-            Path(file_location).parent.mkdir(parents=True, exist_ok=True)
+            file_location.parent.mkdir(parents=True, exist_ok=True)
 
         # Process response
         self._grpc_client.log.debug(f"Requesting design download in {format.value[0]} format.")
         received_bytes = bytes()
         if format is DesignFileFormat.SCDOCX:
             response = self._commands_stub.DownloadFile(Empty())
             received_bytes += response.data
@@ -288,14 +289,207 @@
         downloaded_file.write(received_bytes)
         downloaded_file.close()
 
         self._grpc_client.log.debug(
             f"Design is successfully downloaded at location {file_location}."
         )
 
+    def __build_export_file_location(self, location: Union[Path, str, None], ext: str) -> Path:
+        """
+        Build the file location for export functions.
+
+        Parameters
+        ----------
+        location : Union[~pathlib.Path, str, None]
+            Location on disk to save the file to. If None, the file will be saved
+            in the current working directory.
+        ext : str
+            Extension to use for the file.
+
+        Returns
+        -------
+        ~pathlib.Path
+            The file location for the export function.
+        """
+        return (Path(location) if location else Path.cwd()) / f"{self.name}.{ext}"
+
+    def export_to_scdocx(self, location: Union[Path, str] = None) -> str:
+        """
+        Export the design to an scdocx file.
+
+        Parameters
+        ----------
+        location : Union[~pathlib.Path, str], optional
+            Location on disk to save the file to. If None, the file will be saved
+            in the current working directory.
+
+        Returns
+        -------
+        str
+            The path to the saved file.
+        """
+        # Define the file location
+        file_location = self.__build_export_file_location(location, "scdocx")
+
+        # Export the design to an scdocx file
+        self.download(file_location, DesignFileFormat.SCDOCX)
+
+        # Return the file location
+        return file_location
+
+    def export_to_parasolid_text(self, location: Union[Path, str] = None) -> str:
+        """
+        Export the design to a Parasolid text file.
+
+        Parameters
+        ----------
+        location : Union[~pathlib.Path, str], optional
+            Location on disk to save the file to. If None, the file will be saved
+            in the current working directory.
+
+        Returns
+        -------
+        str
+            The path to the saved file.
+        """
+        # Determine the extension based on the backend type
+        ext = "x_t" if self._grpc_client.backend_type == BackendType.LINUX_SERVICE else "xmt_txt"
+
+        # Define the file location
+        file_location = self.__build_export_file_location(location, ext)
+
+        # Export the design to a Parasolid text file
+        self.download(file_location, DesignFileFormat.PARASOLID_TEXT)
+
+        # Return the file location
+        return file_location
+
+    def export_to_parasolid_bin(self, location: Union[Path, str] = None) -> str:
+        """
+        Export the design to a Parasolid binary file.
+
+        Parameters
+        ----------
+        location : Union[~pathlib.Path, str], optional
+            Location on disk to save the file to. If None, the file will be saved
+            in the current working directory.
+
+        Returns
+        -------
+        str
+            The path to the saved file.
+        """
+        # Determine the extension based on the backend type
+        ext = "x_b" if self._grpc_client.backend_type == BackendType.LINUX_SERVICE else "xmt_bin"
+
+        # Define the file location
+        file_location = self.__build_export_file_location(location, ext)
+
+        # Export the design to a Parasolid binary file
+        self.download(file_location, DesignFileFormat.PARASOLID_BIN)
+
+        # Return the file location
+        return file_location
+
+    def export_to_fmd(self, location: Union[Path, str] = None) -> str:
+        """
+        Export the design to an FMD file.
+
+        Parameters
+        ----------
+        location : Union[~pathlib.Path, str], optional
+            Location on disk to save the file to. If None, the file will be saved
+            in the current working directory.
+
+        Returns
+        -------
+        str
+            The path to the saved file.
+        """
+        # Define the file location
+        file_location = self.__build_export_file_location(location, "fmd")
+
+        # Export the design to an FMD file
+        self.download(file_location, DesignFileFormat.FMD)
+
+        # Return the file location
+        return file_location
+
+    def export_to_step(self, location: Union[Path, str] = None) -> str:
+        """
+        Export the design to a STEP file.
+
+        Parameters
+        ----------
+        location : Union[~pathlib.Path, str], optional
+            Location on disk to save the file to. If None, the file will be saved
+            in the current working directory.
+
+        Returns
+        -------
+        str
+            The path to the saved file.
+        """
+        # Define the file location
+        file_location = self.__build_export_file_location(location, "stp")
+
+        # Export the design to a STEP file
+        self.download(file_location, DesignFileFormat.STEP)
+
+        # Return the file location
+        return file_location
+
+    def export_to_iges(self, location: Union[Path, str] = None) -> str:
+        """
+        Export the design to an IGES file.
+
+        Parameters
+        ----------
+        location : Union[~pathlib.Path, str], optional
+            Location on disk to save the file to. If None, the file will be saved
+            in the current working directory.
+
+        Returns
+        -------
+        str
+            The path to the saved file.
+        """
+        # Define the file location
+        file_location = self.__build_export_file_location(location, "igs")
+
+        # Export the design to an IGES file
+        self.download(file_location, DesignFileFormat.IGES)
+
+        # Return the file location
+        return file_location
+
+    def export_to_pmdb(self, location: Union[Path, str] = None) -> str:
+        """
+        Export the design to a PMDB file.
+
+        Parameters
+        ----------
+        location : Union[~pathlib.Path, str], optional
+            Location on disk to save the file to. If None, the file will be saved
+            in the current working directory.
+
+        Returns
+        -------
+        str
+            The path to the saved file.
+        """
+        # Define the file location
+        file_location = self.__build_export_file_location(location, "pmdb")
+
+        # Export the design to a PMDB file
+        self.download(file_location, DesignFileFormat.PMDB)
+
+        # Return the file location
+        return file_location
+
     @check_input_types
     @ensure_design_is_active
     def create_named_selection(
         self,
         name: str,
         bodies: Optional[List[Body]] = None,
         faces: Optional[List[Face]] = None,
@@ -690,15 +884,15 @@
             self._design_id = design.id
             self._id = design.main_part.id
             self._activate(called_after_design_creation=True)
             # Here we may take the design's name instead of the main part's name.
             # Since they're the same in the backend.
             self._name = design.name
 
-        response = self._commands_stub.GetAssembly(EntityIdentifier(id=""))
+        response = self._commands_stub.GetAssembly(EntityIdentifier(id=self._design_id))
 
         # Store created objects
         created_parts = {p.id: Part(p.id, p.name, [], []) for p in response.parts}
         created_tps = {}
         created_components = {design.main_part.id: self}
         created_bodies = {}
```

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/designpoint.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/designpoint.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/edge.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/edge.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/face.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/face.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/part.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/part.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/designer/selection.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/selection.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/errors.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/errors.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/logger.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/materials/__init__.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/materials/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/materials/material.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/materials/material.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/materials/property.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/materials/property.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/__init__.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/bbox.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/bbox.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/constants.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/constants.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/frame.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/frame.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/matrix.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/matrix.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/plane.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/plane.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/point.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/point.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/math/vector.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/vector.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/__init__.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/accuracy.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/accuracy.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/auxiliary.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/auxiliary.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/checks.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/checks.py`

 * *Files 7% similar despite different names*

```diff
@@ -337,19 +337,27 @@
                     raise GeometryRuntimeError(
                         "The client is not available. You must initialize the client first."
                     )
                 elif self._grpc_client.backend_version is not None:
                     comp = semver.compare(method_version, self._grpc_client.backend_version)
                     # if comp is 1, method version is higher than backend version.
                     if comp == 1:
-                        raise GeometryRuntimeError(
-                            f"The method '{method.__name__}' requires a minimum backend version of "
-                            + f"{method_version}, and the current backend version is "
-                            + f"{self._grpc_client.backend_version}."
-                        )
+
+                        # Check if the version is "0.0.0" (i.e., the version is not available)
+                        if self._grpc_client.backend_version == "0.0.0":
+                            raise GeometryRuntimeError(
+                                f"The method '{method.__name__}' requires a minimum Ansys release version of "  # noqa: E501
+                                + f"{method_version}, but the current version used is 24.1.0 or lower."  # noqa: E501
+                            )
+                        else:
+                            raise GeometryRuntimeError(
+                                f"The method '{method.__name__}' requires a minimum Ansys release version of "  # noqa: E501
+                                + f"{method_version}, but the current version used is "
+                                + f"{self._grpc_client.backend_version}."
+                            )
                     else:
                         return method(self, *args, **kwargs)
             else:
                 logger.warning("This object does not have a connection with the backend.")
 
         return wrapper
```

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/measurements.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/measurements.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/options.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/options.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/misc/units.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/units.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/modeler.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/modeler.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/__init__.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/plotter.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/plotter.py`

 * *Files 0% similar despite different names*

```diff
@@ -548,15 +548,15 @@
         # Conditionally set the Jupyter backend as not all users will be within
         # a notebook environment to avoid a pyvista warning
         if self.scene.notebook and jupyter_backend is None:
             jupyter_backend = "trame"
 
         # Override jupyter backend in case we are building docs
         if DOCUMENTATION_BUILD:
-            jupyter_backend = "static"
+            jupyter_backend = "html"
 
         # Enabling anti-aliasing by default on scene
         self.scene.enable_anti_aliasing("ssaa")
 
         self.scene.show(jupyter_backend=jupyter_backend, **kwargs)
 
     def __set_add_mesh_defaults(self, plotting_options: Optional[Dict]) -> None:
```

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/plotter_helper.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/plotter_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -248,24 +248,46 @@
             callback=self.picker_callback, use_actor=True, show=False, show_message=False
         )
 
     def disable_picking(self):
         """Disable picking capabilities in the plotter."""
         self._pl.scene.disable_picking()
 
-    def add(self, object: Any, **plotting_options):
+    def add(
+        self,
+        object: Any,
+        merge_bodies: bool = False,
+        merge_component: bool = False,
+        filter: str = None,
+        **plotting_options,
+    ):
         """
         Add a ``pyansys-geometry`` or ``PyVista`` object to the plotter.
 
         Parameters
         ----------
         object : Any
-            Object you want to show.
+            Object or list of objects you want to show.
+        merge_bodies : bool, default: False
+            Whether to merge each body into a single dataset. When ``True``,
+            all the faces of each individual body are effectively combined
+            into a single dataset without separating faces.
+        merge_component : bool, default: False
+            Whether to merge this component into a single dataset. When ``True``,
+            all the individual bodies are effectively combined into a single
+            dataset without any hierarchy.
+        **plotting_options : dict, default: None
+            Keyword arguments. For allowable keyword arguments, see the
+            :meth:`Plotter.add_mesh <pyvista.Plotter.add_mesh>` method.
         """
-        self._pl.add(object=object, **plotting_options)
+        if isinstance(object, List) and not isinstance(object[0], pv.PolyData):
+            logger.debug("Plotting objects in list...")
+            self._pl.add_list(object, merge_bodies, merge_component, filter, **plotting_options)
+        else:
+            self._pl.add(object, merge_bodies, merge_component, filter, **plotting_options)
 
     def plot(
         self,
         object: Any = None,
         screenshot: Optional[str] = None,
         merge_bodies: bool = False,
         merge_component: bool = False,
@@ -302,19 +324,22 @@
             :meth:`Plotter.add_mesh <pyvista.Plotter.add_mesh>` method.
 
         Returns
         -------
         List[Any]
             List with the picked bodies in the picked order.
         """
-        if isinstance(object, List) and not isinstance(object[0], pv.PolyData):
-            logger.debug("Plotting objects in list...")
-            self._pl.add_list(object, merge_bodies, merge_component, filter, **plotting_options)
-        else:
-            self._pl.add(object, merge_bodies, merge_component, filter, **plotting_options)
+        self.add(
+            object=object,
+            merge_bodies=merge_bodies,
+            merge_component=merge_component,
+            filter=filter,
+            **plotting_options,
+        )
+
         if self._pl.geom_object_actors_map:
             self._geom_object_actors_map = self._pl.geom_object_actors_map
         else:
             logger.warning("No actors added to the plotter.")
 
         self.compute_edge_object_map()
         # Compute mapping between the objects and its edges.
```

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/plotting_types.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/plotting_types.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/__init__.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/designpoint.png` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/designpoint.png`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/downarrow.png` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/downarrow.png`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/_images/isometric.png` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/isometric.png`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/button.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/button.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/displace_arrows.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/displace_arrows.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/measure.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/measure.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/ruler.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/ruler.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/show_design_point.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/show_design_point.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/view_button.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/view_button.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/plotting/widgets/widget.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/__init__.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/box_uv.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/box_uv.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/__init__.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/circle.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/circle.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/curve.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/curve.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/curve_evaluation.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/curve_evaluation.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/ellipse.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/ellipse.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/line.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/line.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/curves/trimmed_curve.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/trimmed_curve.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/parameterization.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/parameterization.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/__init__.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/cone.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/cone.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/cylinder.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/cylinder.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/plane.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/plane.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/sphere.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/sphere.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/surface.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/surface.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/surface_evaluation.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/surface_evaluation.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/torus.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/torus.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/shapes/surfaces/trimmed_surface.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/trimmed_surface.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/__init__.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/arc.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/arc.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/box.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/box.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/circle.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/circle.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/edge.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/edge.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/ellipse.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/ellipse.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/face.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/face.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/gears.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/gears.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/polygon.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/polygon.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/segment.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/segment.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/sketch.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/sketch.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/slot.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/slot.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/trapezoid.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/trapezoid.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/sketch/triangle.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/triangle.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/tools/__init__.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/tools/measurement_tools.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/tools/measurement_tools.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/tools/problem_areas.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/tools/problem_areas.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/tools/repair_tool_message.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/tools/repair_tool_message.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/tools/repair_tools.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/tools/repair_tools.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/src/ansys/geometry/core/typing.py` & `ansys_geometry_core-0.5.1/src/ansys/geometry/core/typing.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.0/PKG-INFO` & `ansys_geometry_core-0.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-geometry-core
-Version: 0.5.0
+Version: 0.5.1
 Summary: A python wrapper for Ansys Geometry service
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -14,77 +14,80 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ansys-api-geometry==0.4.1
 Requires-Dist: ansys-tools-path>=0.3,<1
 Requires-Dist: beartype>=0.11.0,<0.19
-Requires-Dist: google-api-python-client>=1.7.11,<3
-Requires-Dist: googleapis-common-protos>=1.52.0,<2
 Requires-Dist: grpcio>=1.35.0,<2
 Requires-Dist: grpcio-health-checking>=1.45.0,<2
 Requires-Dist: numpy>=1.20.3,<2
 Requires-Dist: Pint>=0.18,<1
-Requires-Dist: protobuf>=3.20.2,<5
+Requires-Dist: protobuf>=3.20.2,<6
 Requires-Dist: pyvista>=0.37.0,<1
+Requires-Dist: requests>=2,<3
 Requires-Dist: scipy>=1.7.3,<2
+Requires-Dist: semver>=3,<4
 Requires-Dist: six>=1.16.0,<2
 Requires-Dist: vtk>=9,<10
-Requires-Dist: semver>=3,<4
 Requires-Dist: ansys-platform-instancemanagement>=1.0.3,<2 ; extra == "all"
 Requires-Dist: docker>=6.0.1,<8 ; extra == "all"
-Requires-Dist: pyvista[jupyter]>=0.38.1,<0.42 ; extra == "all"
+Requires-Dist: pyvista[jupyter]>=0.38.1,<1 ; extra == "all"
 Requires-Dist: ansys-sphinx-theme[autoapi]==0.15.2 ; extra == "doc"
-Requires-Dist: beartype==0.18.2 ; extra == "doc"
+Requires-Dist: beartype==0.18.5 ; extra == "doc"
 Requires-Dist: docker==7.0.0 ; extra == "doc"
 Requires-Dist: ipyvtklink==0.2.3 ; extra == "doc"
 Requires-Dist: jupyter_sphinx==0.5.3 ; extra == "doc"
 Requires-Dist: jupytext==1.16.1 ; extra == "doc"
 Requires-Dist: myst-parser==2.0.0 ; extra == "doc"
 Requires-Dist: nbconvert==7.16.3 ; extra == "doc"
 Requires-Dist: nbsphinx==0.9.3 ; extra == "doc"
-Requires-Dist: notebook==7.1.2 ; extra == "doc"
+Requires-Dist: notebook==7.1.3 ; extra == "doc"
 Requires-Dist: numpydoc==1.7.0 ; extra == "doc"
 Requires-Dist: panel==1.4.1 ; extra == "doc"
 Requires-Dist: pyvista[jupyter]==0.43.5 ; extra == "doc"
 Requires-Dist: requests==2.31.0 ; extra == "doc"
 Requires-Dist: sphinx==7.2.6 ; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints==1.24.0 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx-jinja==2.0.2 ; extra == "doc"
+Requires-Dist: trame-vtk==2.8.6 ; extra == "doc"
 Requires-Dist: vtk==9.3.0 ; extra == "doc"
 Requires-Dist: ansys-platform-instancemanagement==1.1.2 ; extra == "tests"
-Requires-Dist: ansys-tools-path==0.5.1 ; extra == "tests"
-Requires-Dist: beartype==0.18.2 ; extra == "tests"
+Requires-Dist: ansys-tools-path==0.5.2 ; extra == "tests"
+Requires-Dist: beartype==0.18.5 ; extra == "tests"
 Requires-Dist: docker==7.0.0 ; extra == "tests"
-Requires-Dist: google-api-python-client==2.122.0 ; extra == "tests"
-Requires-Dist: googleapis-common-protos==1.63.0 ; extra == "tests"
-Requires-Dist: grpcio==1.62.1 ; extra == "tests"
+Requires-Dist: grpcio==1.62.2 ; extra == "tests"
 Requires-Dist: grpcio-health-checking==1.60.0 ; extra == "tests"
 Requires-Dist: numpy==1.26.4 ; extra == "tests"
 Requires-Dist: Pint==0.23 ; extra == "tests"
-Requires-Dist: protobuf==4.25.1 ; extra == "tests"
+Requires-Dist: protobuf==5.26.1 ; extra == "tests"
 Requires-Dist: pytest==8.1.1 ; extra == "tests"
 Requires-Dist: pytest-cov==5.0.0 ; extra == "tests"
 Requires-Dist: pytest-pyvista==0.1.9 ; extra == "tests"
 Requires-Dist: pytest-xvfb==3.0.0 ; extra == "tests"
 Requires-Dist: pyvista[jupyter]==0.43.5 ; extra == "tests"
 Requires-Dist: requests==2.31.0 ; extra == "tests"
 Requires-Dist: scipy==1.13.0 ; extra == "tests"
 Requires-Dist: semver==3.0.2 ; extra == "tests"
 Requires-Dist: six==1.16.0 ; extra == "tests"
 Requires-Dist: vtk==9.3.0 ; extra == "tests"
+Requires-Dist: pytest==8.1.1 ; extra == "tests-minimal"
+Requires-Dist: pytest-cov==5.0.0 ; extra == "tests-minimal"
+Requires-Dist: pytest-pyvista==0.1.9 ; extra == "tests-minimal"
+Requires-Dist: pytest-xvfb==3.0.0 ; extra == "tests-minimal"
 Project-URL: Discussions, https://github.com/ansys/pyansys-geometry/discussions
 Project-URL: Documentation, https://geometry.docs.pyansys.com
 Project-URL: Issues, https://github.com/ansys/pyansys-geometry/issues
 Project-URL: Releases, https://github.com/ansys/pyansys-geometry/releases
 Project-URL: Source, https://github.com/ansys/pyansys-geometry
 Provides-Extra: all
 Provides-Extra: doc
 Provides-Extra: tests
+Provides-Extra: tests-minimal
 
 PyAnsys Geometry
 ================
 |pyansys| |python| |pypi| |downloads| |GH-CI| |codecov| |MIT| |black| |pre-commit|
 
 .. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
    :target: https://docs.pyansys.com/
```

