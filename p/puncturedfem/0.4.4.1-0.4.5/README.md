# Comparing `tmp/puncturedfem-0.4.4.1.tar.gz` & `tmp/puncturedfem-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puncturedfem-0.4.4.1.tar", max compression
+gzip compressed data, was "puncturedfem-0.4.5.tar", max compression
```

## Comparing `puncturedfem-0.4.4.1.tar` & `puncturedfem-0.4.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0    35149 2024-02-14 06:15:58.603112 puncturedfem-0.4.4.1/LICENSE
--rw-r--r--   0        0        0     6703 2024-04-08 17:56:44.261359 puncturedfem-0.4.4.1/README.md
--rw-r--r--   0        0        0     2909 2024-04-07 23:56:28.564817 puncturedfem-0.4.4.1/puncturedfem/__init__.py
--rw-r--r--   0        0        0      647 2024-03-19 20:35:01.952304 puncturedfem-0.4.4.1/puncturedfem/locfun/__init__.py
--rw-r--r--   0        0        0      271 2024-02-14 06:15:58.623114 puncturedfem-0.4.4.1/puncturedfem/locfun/antilap/__init__.py
--rw-r--r--   0        0        0     5181 2024-02-28 23:45:15.504147 puncturedfem-0.4.4.1/puncturedfem/locfun/antilap/antilap.py
--rw-r--r--   0        0        0     2572 2024-03-19 20:35:01.952304 puncturedfem-0.4.4.1/puncturedfem/locfun/antilap/log_antilap.py
--rw-r--r--   0        0        0      439 2024-02-28 23:45:15.508147 puncturedfem-0.4.4.1/puncturedfem/locfun/d2n/__init__.py
--rw-r--r--   0        0        0     1322 2024-02-14 06:15:58.623114 puncturedfem-0.4.4.1/puncturedfem/locfun/d2n/fft_deriv.py
--rw-r--r--   0        0        0     3515 2024-03-19 20:35:01.952304 puncturedfem-0.4.4.1/puncturedfem/locfun/d2n/log_terms.py
--rw-r--r--   0        0        0     1463 2024-02-14 06:15:58.623114 puncturedfem-0.4.4.1/puncturedfem/locfun/d2n/trace2tangential.py
--rw-r--r--   0        0        0    10769 2024-03-19 20:35:01.952304 puncturedfem-0.4.4.1/puncturedfem/locfun/edge_space.py
--rw-r--r--   0        0        0    23954 2024-03-19 20:35:01.952304 puncturedfem-0.4.4.1/puncturedfem/locfun/locfun.py
--rw-r--r--   0        0        0     8564 2024-03-19 20:35:01.952304 puncturedfem-0.4.4.1/puncturedfem/locfun/locfunsp.py
--rw-r--r--   0        0        0    22086 2024-03-19 20:35:01.952304 puncturedfem-0.4.4.1/puncturedfem/locfun/nystrom.py
--rw-r--r--   0        0        0      671 2024-02-28 23:45:15.508147 puncturedfem-0.4.4.1/puncturedfem/locfun/poly/__init__.py
--rw-r--r--   0        0        0     3341 2024-03-19 20:35:01.952304 puncturedfem-0.4.4.1/puncturedfem/locfun/poly/barycentric.py
--rw-r--r--   0        0        0      926 2024-02-20 23:42:26.935693 puncturedfem-0.4.4.1/puncturedfem/locfun/poly/integrate_poly.py
--rw-r--r--   0        0        0     2839 2024-02-14 06:15:58.623114 puncturedfem-0.4.4.1/puncturedfem/locfun/poly/legendre.py
--rw-r--r--   0        0        0     6524 2024-03-19 20:35:01.952304 puncturedfem-0.4.4.1/puncturedfem/locfun/poly/monomial.py
--rw-r--r--   0        0        0     2880 2024-02-14 06:15:58.623114 puncturedfem-0.4.4.1/puncturedfem/locfun/poly/multi_index.py
--rw-r--r--   0        0        0     3405 2024-03-19 20:35:01.952304 puncturedfem-0.4.4.1/puncturedfem/locfun/poly/piecewise_poly.py
--rw-r--r--   0        0        0    13244 2024-03-19 20:35:01.952304 puncturedfem-0.4.4.1/puncturedfem/locfun/poly/poly.py
--rw-r--r--   0        0        0     1081 2024-03-19 20:35:01.956304 puncturedfem-0.4.4.1/puncturedfem/locfun/poly/poly_eval.py
--rw-r--r--   0        0        0     1075 2024-02-14 06:15:58.623114 puncturedfem-0.4.4.1/puncturedfem/locfun/poly/poly_exceptions.py
--rw-r--r--   0        0        0    12236 2024-03-19 20:35:01.956304 puncturedfem-0.4.4.1/puncturedfem/locfun/trace.py
--rw-r--r--   0        0        0      918 2024-02-14 06:15:58.623114 puncturedfem-0.4.4.1/puncturedfem/mesh/__init__.py
--rw-r--r--   0        0        0     1090 2024-02-14 06:15:58.623114 puncturedfem-0.4.4.1/puncturedfem/mesh/bounding_box.py
--rw-r--r--   0        0        0    20320 2024-03-19 20:35:01.956304 puncturedfem-0.4.4.1/puncturedfem/mesh/cell.py
--rw-r--r--   0        0        0    12861 2024-03-19 20:35:01.956304 puncturedfem-0.4.4.1/puncturedfem/mesh/closed_contour.py
--rw-r--r--   0        0        0    21278 2024-03-19 20:35:01.956304 puncturedfem-0.4.4.1/puncturedfem/mesh/edge.py
--rw-r--r--   0        0        0      771 2024-02-14 06:15:58.623114 puncturedfem-0.4.4.1/puncturedfem/mesh/edgelib/bean.py
--rw-r--r--   0        0        0     1336 2024-02-14 06:15:58.623114 puncturedfem-0.4.4.1/puncturedfem/mesh/edgelib/cartioid.py
--rw-r--r--   0        0        0      947 2024-02-14 06:15:58.623114 puncturedfem-0.4.4.1/puncturedfem/mesh/edgelib/circle.py
--rw-r--r--   0        0        0     1394 2024-02-14 06:15:58.623114 puncturedfem-0.4.4.1/puncturedfem/mesh/edgelib/circular_arc.py
--rw-r--r--   0        0        0     1295 2024-02-14 06:15:58.627115 puncturedfem-0.4.4.1/puncturedfem/mesh/edgelib/circular_arc_deg.py
--rw-r--r--   0        0        0      762 2024-02-14 06:15:58.627115 puncturedfem-0.4.4.1/puncturedfem/mesh/edgelib/ellipse.py
--rw-r--r--   0        0        0      605 2024-02-14 06:15:58.627115 puncturedfem-0.4.4.1/puncturedfem/mesh/edgelib/line.py
--rw-r--r--   0        0        0     1408 2024-02-14 06:15:58.627115 puncturedfem-0.4.4.1/puncturedfem/mesh/edgelib/sine_wave.py
--rw-r--r--   0        0        0     1595 2024-02-28 23:45:15.512147 puncturedfem-0.4.4.1/puncturedfem/mesh/edgelib/spline.py
--rw-r--r--   0        0        0     1102 2024-02-14 06:15:58.627115 puncturedfem-0.4.4.1/puncturedfem/mesh/edgelib/teardrop.py
--rw-r--r--   0        0        0     1164 2024-02-14 06:15:58.627115 puncturedfem-0.4.4.1/puncturedfem/mesh/mesh_exceptions.py
--rw-r--r--   0        0        0     1344 2024-02-14 06:15:58.627115 puncturedfem-0.4.4.1/puncturedfem/mesh/meshlib/__builder__.py
--rw-r--r--   0        0        0      448 2024-02-14 06:15:58.627115 puncturedfem-0.4.4.1/puncturedfem/mesh/meshlib/__init__.py
--rw-r--r--   0        0        0     6022 2024-02-14 06:15:58.627115 puncturedfem-0.4.4.1/puncturedfem/mesh/meshlib/pacman.py
--rw-r--r--   0        0        0     6509 2024-02-14 06:15:58.627115 puncturedfem-0.4.4.1/puncturedfem/mesh/meshlib/pacman_subdiv.py
--rw-r--r--   0        0        0     1508 2024-02-14 06:15:58.627115 puncturedfem-0.4.4.1/puncturedfem/mesh/meshlib/square_circular_hole.py
--rw-r--r--   0        0        0     8245 2024-02-14 06:15:58.627115 puncturedfem-0.4.4.1/puncturedfem/mesh/planar_mesh.py
--rw-r--r--   0        0        0     4388 2024-03-19 20:35:01.956304 puncturedfem-0.4.4.1/puncturedfem/mesh/quad.py
--rw-r--r--   0        0        0     4012 2024-04-08 00:34:56.332232 puncturedfem-0.4.4.1/puncturedfem/mesh/split_edge.py
--rw-r--r--   0        0        0     2868 2024-02-28 23:45:15.512147 puncturedfem-0.4.4.1/puncturedfem/mesh/transform.py
--rw-r--r--   0        0        0     4804 2024-02-28 23:45:15.512147 puncturedfem-0.4.4.1/puncturedfem/mesh/vert.py
--rw-r--r--   0        0        0      344 2024-02-28 23:45:15.512147 puncturedfem-0.4.4.1/puncturedfem/plot/__init__.py
--rw-r--r--   0        0        0     7290 2024-02-28 23:45:15.516147 puncturedfem-0.4.4.1/puncturedfem/plot/globfun_plot.py
--rw-r--r--   0        0        0     4352 2024-02-28 23:45:15.516147 puncturedfem-0.4.4.1/puncturedfem/plot/locfun_plot.py
--rw-r--r--   0        0        0     3846 2024-02-28 23:45:15.516147 puncturedfem-0.4.4.1/puncturedfem/plot/mesh_plot.py
--rw-r--r--   0        0        0     1891 2024-02-28 23:45:15.516147 puncturedfem-0.4.4.1/puncturedfem/plot/plot_util.py
--rw-r--r--   0        0        0    11087 2024-03-19 20:35:01.956304 puncturedfem-0.4.4.1/puncturedfem/plot/trace_plot.py
--rw-r--r--   0        0        0      289 2024-02-14 06:15:58.627115 puncturedfem-0.4.4.1/puncturedfem/solver/__init__.py
--rw-r--r--   0        0        0     3756 2024-04-05 19:41:53.569850 puncturedfem-0.4.4.1/puncturedfem/solver/bilinear_form.py
--rw-r--r--   0        0        0     7793 2024-02-28 23:45:15.516147 puncturedfem-0.4.4.1/puncturedfem/solver/globfunsp.py
--rw-r--r--   0        0        0     3369 2024-02-14 06:15:58.627115 puncturedfem-0.4.4.1/puncturedfem/solver/globkey.py
--rw-r--r--   0        0        0    11301 2024-02-28 23:45:15.516147 puncturedfem-0.4.4.1/puncturedfem/solver/solver.py
--rw-r--r--   0        0        0      136 2024-02-14 06:15:58.627115 puncturedfem-0.4.4.1/puncturedfem/util/__init__.py
--rw-r--r--   0        0        0      590 2024-02-14 06:15:58.627115 puncturedfem-0.4.4.1/puncturedfem/util/print_color.py
--rw-r--r--   0        0        0      912 2024-03-19 20:35:01.956304 puncturedfem-0.4.4.1/puncturedfem/util/types.py
--rw-r--r--   0        0        0     1868 2024-04-08 18:04:53.789158 puncturedfem-0.4.4.1/pyproject.toml
--rw-r--r--   0        0        0     7412 1970-01-01 00:00:00.000000 puncturedfem-0.4.4.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-14 06:15:58.603112 puncturedfem-0.4.5/LICENSE
+-rw-r--r--   0        0        0     6707 2024-04-24 18:46:20.176432 puncturedfem-0.4.5/README.md
+-rw-r--r--   0        0        0     2906 2024-04-24 18:46:20.176432 puncturedfem-0.4.5/puncturedfem/__init__.py
+-rw-r--r--   0        0        0      647 2024-03-19 20:35:01.952304 puncturedfem-0.4.5/puncturedfem/locfun/__init__.py
+-rw-r--r--   0        0        0      271 2024-02-14 06:15:58.623114 puncturedfem-0.4.5/puncturedfem/locfun/antilap/__init__.py
+-rw-r--r--   0        0        0     5181 2024-02-28 23:45:15.504147 puncturedfem-0.4.5/puncturedfem/locfun/antilap/antilap.py
+-rw-r--r--   0        0        0     2572 2024-04-24 17:00:19.280461 puncturedfem-0.4.5/puncturedfem/locfun/antilap/log_antilap.py
+-rw-r--r--   0        0        0      439 2024-02-28 23:45:15.508147 puncturedfem-0.4.5/puncturedfem/locfun/d2n/__init__.py
+-rw-r--r--   0        0        0     1322 2024-02-14 06:15:58.623114 puncturedfem-0.4.5/puncturedfem/locfun/d2n/fft_deriv.py
+-rw-r--r--   0        0        0     3515 2024-03-19 20:35:01.952304 puncturedfem-0.4.5/puncturedfem/locfun/d2n/log_terms.py
+-rw-r--r--   0        0        0     1463 2024-02-14 06:15:58.623114 puncturedfem-0.4.5/puncturedfem/locfun/d2n/trace2tangential.py
+-rw-r--r--   0        0        0    10769 2024-03-19 20:35:01.952304 puncturedfem-0.4.5/puncturedfem/locfun/edge_space.py
+-rw-r--r--   0        0        0    23954 2024-04-24 17:00:19.280461 puncturedfem-0.4.5/puncturedfem/locfun/locfun.py
+-rw-r--r--   0        0        0     8564 2024-03-19 20:35:01.952304 puncturedfem-0.4.5/puncturedfem/locfun/locfunsp.py
+-rw-r--r--   0        0        0    22075 2024-04-24 18:46:20.176432 puncturedfem-0.4.5/puncturedfem/locfun/nystrom.py
+-rw-r--r--   0        0        0      671 2024-02-28 23:45:15.508147 puncturedfem-0.4.5/puncturedfem/locfun/poly/__init__.py
+-rw-r--r--   0        0        0     3341 2024-03-19 20:35:01.952304 puncturedfem-0.4.5/puncturedfem/locfun/poly/barycentric.py
+-rw-r--r--   0        0        0      926 2024-02-20 23:42:26.935693 puncturedfem-0.4.5/puncturedfem/locfun/poly/integrate_poly.py
+-rw-r--r--   0        0        0     2839 2024-02-14 06:15:58.623114 puncturedfem-0.4.5/puncturedfem/locfun/poly/legendre.py
+-rw-r--r--   0        0        0     6524 2024-03-19 20:35:01.952304 puncturedfem-0.4.5/puncturedfem/locfun/poly/monomial.py
+-rw-r--r--   0        0        0     2880 2024-02-14 06:15:58.623114 puncturedfem-0.4.5/puncturedfem/locfun/poly/multi_index.py
+-rw-r--r--   0        0        0     3405 2024-04-24 17:00:19.280461 puncturedfem-0.4.5/puncturedfem/locfun/poly/piecewise_poly.py
+-rw-r--r--   0        0        0    13244 2024-04-24 17:00:19.284462 puncturedfem-0.4.5/puncturedfem/locfun/poly/poly.py
+-rw-r--r--   0        0        0     1081 2024-03-19 20:35:01.956304 puncturedfem-0.4.5/puncturedfem/locfun/poly/poly_eval.py
+-rw-r--r--   0        0        0     1075 2024-02-14 06:15:58.623114 puncturedfem-0.4.5/puncturedfem/locfun/poly/poly_exceptions.py
+-rw-r--r--   0        0        0    12236 2024-04-24 17:00:19.284462 puncturedfem-0.4.5/puncturedfem/locfun/trace.py
+-rw-r--r--   0        0        0      918 2024-02-14 06:15:58.623114 puncturedfem-0.4.5/puncturedfem/mesh/__init__.py
+-rw-r--r--   0        0        0     1090 2024-02-14 06:15:58.623114 puncturedfem-0.4.5/puncturedfem/mesh/bounding_box.py
+-rw-r--r--   0        0        0    20320 2024-04-24 18:17:00.673329 puncturedfem-0.4.5/puncturedfem/mesh/cell.py
+-rw-r--r--   0        0        0    12859 2024-04-24 18:46:20.176432 puncturedfem-0.4.5/puncturedfem/mesh/closed_contour.py
+-rw-r--r--   0        0        0    21278 2024-04-24 18:17:00.773326 puncturedfem-0.4.5/puncturedfem/mesh/edge.py
+-rw-r--r--   0        0        0      771 2024-02-14 06:15:58.623114 puncturedfem-0.4.5/puncturedfem/mesh/edgelib/bean.py
+-rw-r--r--   0        0        0     1336 2024-02-14 06:15:58.623114 puncturedfem-0.4.5/puncturedfem/mesh/edgelib/cartioid.py
+-rw-r--r--   0        0        0      947 2024-02-14 06:15:58.623114 puncturedfem-0.4.5/puncturedfem/mesh/edgelib/circle.py
+-rw-r--r--   0        0        0     1394 2024-02-14 06:15:58.623114 puncturedfem-0.4.5/puncturedfem/mesh/edgelib/circular_arc.py
+-rw-r--r--   0        0        0     1295 2024-02-14 06:15:58.627115 puncturedfem-0.4.5/puncturedfem/mesh/edgelib/circular_arc_deg.py
+-rw-r--r--   0        0        0      762 2024-02-14 06:15:58.627115 puncturedfem-0.4.5/puncturedfem/mesh/edgelib/ellipse.py
+-rw-r--r--   0        0        0      605 2024-02-14 06:15:58.627115 puncturedfem-0.4.5/puncturedfem/mesh/edgelib/line.py
+-rw-r--r--   0        0        0     1408 2024-02-14 06:15:58.627115 puncturedfem-0.4.5/puncturedfem/mesh/edgelib/sine_wave.py
+-rw-r--r--   0        0        0     1595 2024-02-28 23:45:15.512147 puncturedfem-0.4.5/puncturedfem/mesh/edgelib/spline.py
+-rw-r--r--   0        0        0     1102 2024-02-14 06:15:58.627115 puncturedfem-0.4.5/puncturedfem/mesh/edgelib/teardrop.py
+-rw-r--r--   0        0        0     1164 2024-02-14 06:15:58.627115 puncturedfem-0.4.5/puncturedfem/mesh/mesh_exceptions.py
+-rw-r--r--   0        0        0     1344 2024-04-24 17:00:19.284462 puncturedfem-0.4.5/puncturedfem/mesh/meshlib/__builder__.py
+-rw-r--r--   0        0        0      448 2024-02-14 06:15:58.627115 puncturedfem-0.4.5/puncturedfem/mesh/meshlib/__init__.py
+-rw-r--r--   0        0        0     6022 2024-02-14 06:15:58.627115 puncturedfem-0.4.5/puncturedfem/mesh/meshlib/pacman.py
+-rw-r--r--   0        0        0     6509 2024-02-14 06:15:58.627115 puncturedfem-0.4.5/puncturedfem/mesh/meshlib/pacman_subdiv.py
+-rw-r--r--   0        0        0     1508 2024-02-14 06:15:58.627115 puncturedfem-0.4.5/puncturedfem/mesh/meshlib/square_circular_hole.py
+-rw-r--r--   0        0        0     8245 2024-04-24 17:00:19.284462 puncturedfem-0.4.5/puncturedfem/mesh/planar_mesh.py
+-rw-r--r--   0        0        0     4412 2024-04-24 18:46:20.176432 puncturedfem-0.4.5/puncturedfem/mesh/quad.py
+-rw-r--r--   0        0        0     4038 2024-04-24 18:46:20.176432 puncturedfem-0.4.5/puncturedfem/mesh/split_edge.py
+-rw-r--r--   0        0        0     2868 2024-02-28 23:45:15.512147 puncturedfem-0.4.5/puncturedfem/mesh/transform.py
+-rw-r--r--   0        0        0     4804 2024-02-28 23:45:15.512147 puncturedfem-0.4.5/puncturedfem/mesh/vert.py
+-rw-r--r--   0        0        0      344 2024-02-28 23:45:15.512147 puncturedfem-0.4.5/puncturedfem/plot/__init__.py
+-rw-r--r--   0        0        0     7290 2024-02-28 23:45:15.516147 puncturedfem-0.4.5/puncturedfem/plot/globfun_plot.py
+-rw-r--r--   0        0        0     4352 2024-02-28 23:45:15.516147 puncturedfem-0.4.5/puncturedfem/plot/locfun_plot.py
+-rw-r--r--   0        0        0     3846 2024-02-28 23:45:15.516147 puncturedfem-0.4.5/puncturedfem/plot/mesh_plot.py
+-rw-r--r--   0        0        0     1891 2024-02-28 23:45:15.516147 puncturedfem-0.4.5/puncturedfem/plot/plot_util.py
+-rw-r--r--   0        0        0    11131 2024-04-24 18:46:20.180433 puncturedfem-0.4.5/puncturedfem/plot/trace_plot.py
+-rw-r--r--   0        0        0      289 2024-02-14 06:15:58.627115 puncturedfem-0.4.5/puncturedfem/solver/__init__.py
+-rw-r--r--   0        0        0     3756 2024-04-05 19:41:53.569850 puncturedfem-0.4.5/puncturedfem/solver/bilinear_form.py
+-rw-r--r--   0        0        0     7793 2024-02-28 23:45:15.516147 puncturedfem-0.4.5/puncturedfem/solver/globfunsp.py
+-rw-r--r--   0        0        0     3369 2024-02-14 06:15:58.627115 puncturedfem-0.4.5/puncturedfem/solver/globkey.py
+-rw-r--r--   0        0        0    11333 2024-04-24 18:46:20.180433 puncturedfem-0.4.5/puncturedfem/solver/solver.py
+-rw-r--r--   0        0        0      136 2024-02-14 06:15:58.627115 puncturedfem-0.4.5/puncturedfem/util/__init__.py
+-rw-r--r--   0        0        0      590 2024-02-14 06:15:58.627115 puncturedfem-0.4.5/puncturedfem/util/print_color.py
+-rw-r--r--   0        0        0      912 2024-04-24 17:00:19.284462 puncturedfem-0.4.5/puncturedfem/util/types.py
+-rw-r--r--   0        0        0     1888 2024-04-24 18:46:20.180433 puncturedfem-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     7558 1970-01-01 00:00:00.000000 puncturedfem-0.4.5/PKG-INFO
```

### Comparing `puncturedfem-0.4.4.1/LICENSE` & `puncturedfem-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/README.md` & `puncturedfem-0.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 ## Installation
 This package is available on [PyPI](https://pypi.org/project/puncturedfem/), and can be installed with pip:
 ```bash
 pip install puncturedfem
 ```
 
 ### Dependencies
-This project is written in Python 3.11 and uses the following packages:
+This project requires Python 3.9 or higher and uses the following packages:
 - [matplotlib](https://matplotlib.org/) (plotting)
 - [numba](https://numba.pydata.org/) (just-in-time compilation)
 - [numpy](https://numpy.org/) (arrays, FFT)
 - [scipy](https://www.scipy.org/) (sparse matrices, GMRES)
 - [tqdm](https://tqdm.github.io/) (progress bars)
 
 Furthermore, this repo contains examples presented with [Jupyter notebooks](https://jupyter.org/).
```

### Comparing `puncturedfem-0.4.4.1/puncturedfem/__init__.py` & `puncturedfem-0.4.5/puncturedfem/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,27 +80,24 @@
     "Quad",
     "QuadDict",
     "Vert",
     "get_quad_dict",
     "meshlib",
     "mesh_builder",
     "split_edge",
-
     # locfun
     "DirichletTrace",
     "EdgeSpace",
     "LocalFunction",
     "LocalFunctionSpace",
     "NystromSolver",
     "Polynomial",
     "PiecewisePolynomial",
     "barycentric_coordinates",
     "barycentric_coordinates_edge",
-
     # solver
     "GlobalFunctionSpace",
     "BilinearForm",
     "Solver",
-
     # plot
     "plot",
 ]
```

### Comparing `puncturedfem-0.4.4.1/puncturedfem/locfun/__init__.py` & `puncturedfem-0.4.5/puncturedfem/locfun/__init__.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/locfun/antilap/antilap.py` & `puncturedfem-0.4.5/puncturedfem/locfun/antilap/antilap.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/locfun/antilap/log_antilap.py` & `puncturedfem-0.4.5/puncturedfem/locfun/antilap/log_antilap.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/locfun/d2n/fft_deriv.py` & `puncturedfem-0.4.5/puncturedfem/locfun/d2n/fft_deriv.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/locfun/d2n/log_terms.py` & `puncturedfem-0.4.5/puncturedfem/locfun/d2n/log_terms.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/locfun/d2n/trace2tangential.py` & `puncturedfem-0.4.5/puncturedfem/locfun/d2n/trace2tangential.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/locfun/edge_space.py` & `puncturedfem-0.4.5/puncturedfem/locfun/edge_space.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/locfun/locfun.py` & `puncturedfem-0.4.5/puncturedfem/locfun/locfun.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/locfun/locfunsp.py` & `puncturedfem-0.4.5/puncturedfem/locfun/locfunsp.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/locfun/nystrom.py` & `puncturedfem-0.4.5/puncturedfem/locfun/nystrom.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         a = x[N:]
 
         return psi_hat, a
 
     def _gmres_solve(
         self, A: LinearOperator, b: np.ndarray, M: LinearOperator
     ) -> np.ndarray:
-        x, flag = gmres(A=A, b=b, M=M, atol=1e-12, tol=1e-12)
+        x, flag = gmres(A=A, b=b, M=M, atol=1e-12, rtol=1e-12)
         if flag > 0:
             r = b - A @ x
             print(
                 "warn-NystromSolver: "
                 + f"GMRES failed to converge after {flag} iterations"
                 + f", residual norm = {np.linalg.norm(r):.2e}"
             )
@@ -353,17 +353,17 @@
         self.single_layer_mat = np.zeros((self.K.num_pts, self.K.num_pts))
         for i in range(self.K.num_holes + 1):
             ii1 = self.K.component_start_idx[i]
             ii2 = self.K.component_start_idx[i + 1]
             for j in range(self.K.num_holes + 1):
                 jj1 = self.K.component_start_idx[j]
                 jj2 = self.K.component_start_idx[j + 1]
-                self.single_layer_mat[ii1:ii2, jj1:jj2] = (
-                    self.single_layer_component_block(i, j)
-                )
+                self.single_layer_mat[
+                    ii1:ii2, jj1:jj2
+                ] = self.single_layer_component_block(i, j)
 
     def single_layer_component_block(self, i: int, j: int) -> np.ndarray:
         """
         Block of the single layer operator matrix corresponding to the i-th
         and j-th components of the boundary of K.
         """
         B_comp = np.zeros(
@@ -466,18 +466,18 @@
         self.double_layer_mat = np.zeros((self.K.num_pts, self.K.num_pts))
         for i in range(self.K.num_holes + 1):
             ii1 = self.K.component_start_idx[i]
             ii2 = self.K.component_start_idx[i + 1]
             for j in range(self.K.num_holes + 1):
                 jj1 = self.K.component_start_idx[j]
                 jj2 = self.K.component_start_idx[j + 1]
-                self.double_layer_mat[ii1:ii2, jj1:jj2] = (
-                    self.double_layer_component_block(
-                        self.K.components[i], self.K.components[j]
-                    )
+                self.double_layer_mat[
+                    ii1:ii2, jj1:jj2
+                ] = self.double_layer_component_block(
+                    self.K.components[i], self.K.components[j]
                 )
 
     def double_layer_component_block(
         self, ci: ClosedContour, cj: ClosedContour
     ) -> np.ndarray:
         """
         Block of the double layer operator matrix corresponding to the i-th
```

### Comparing `puncturedfem-0.4.4.1/puncturedfem/locfun/poly/__init__.py` & `puncturedfem-0.4.5/puncturedfem/locfun/poly/__init__.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/locfun/poly/barycentric.py` & `puncturedfem-0.4.5/puncturedfem/locfun/poly/barycentric.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/locfun/poly/integrate_poly.py` & `puncturedfem-0.4.5/puncturedfem/locfun/poly/integrate_poly.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/locfun/poly/legendre.py` & `puncturedfem-0.4.5/puncturedfem/locfun/poly/legendre.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/locfun/poly/monomial.py` & `puncturedfem-0.4.5/puncturedfem/locfun/poly/monomial.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/locfun/poly/multi_index.py` & `puncturedfem-0.4.5/puncturedfem/locfun/poly/multi_index.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/locfun/poly/piecewise_poly.py` & `puncturedfem-0.4.5/puncturedfem/locfun/poly/piecewise_poly.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/locfun/poly/poly.py` & `puncturedfem-0.4.5/puncturedfem/locfun/poly/poly.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/locfun/poly/poly_eval.py` & `puncturedfem-0.4.5/puncturedfem/locfun/poly/poly_eval.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/locfun/poly/poly_exceptions.py` & `puncturedfem-0.4.5/puncturedfem/locfun/poly/poly_exceptions.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/locfun/trace.py` & `puncturedfem-0.4.5/puncturedfem/locfun/trace.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/__init__.py` & `puncturedfem-0.4.5/puncturedfem/mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/bounding_box.py` & `puncturedfem-0.4.5/puncturedfem/mesh/bounding_box.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/cell.py` & `puncturedfem-0.4.5/puncturedfem/mesh/cell.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/closed_contour.py` & `puncturedfem-0.4.5/puncturedfem/mesh/closed_contour.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,17 +150,17 @@
             mid_idx[i] = self.vert_idx[i] + n
 
         # on first half of an Edge, the closest vertex is the starting
         # point on that Edge; on the second half of an Edge, the closest vertex
         # is the starting point of the next Edge
         self.closest_vert_idx = np.zeros((self.num_pts,), dtype=int)
         for i in range(self.num_edges):
-            self.closest_vert_idx[self.vert_idx[i] : mid_idx[i]] = (
-                self.vert_idx[i]
-            )
+            self.closest_vert_idx[
+                self.vert_idx[i] : mid_idx[i]
+            ] = self.vert_idx[i]
             self.closest_vert_idx[mid_idx[i] : self.vert_idx[i + 1]] = (
                 self.vert_idx[i + 1] % self.num_pts
             )
 
     # INTERIOR POINTS ########################################################
     def get_distance_to_boundary(self, x: float, y: float) -> float:
         """Minimum distance from (x,y) to a point on the boundary"""
```

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/edge.py` & `puncturedfem-0.4.5/puncturedfem/mesh/edge.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/edgelib/bean.py` & `puncturedfem-0.4.5/puncturedfem/mesh/edgelib/bean.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/edgelib/cartioid.py` & `puncturedfem-0.4.5/puncturedfem/mesh/edgelib/cartioid.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/edgelib/circle.py` & `puncturedfem-0.4.5/puncturedfem/mesh/edgelib/circle.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/edgelib/circular_arc.py` & `puncturedfem-0.4.5/puncturedfem/mesh/edgelib/circular_arc.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/edgelib/circular_arc_deg.py` & `puncturedfem-0.4.5/puncturedfem/mesh/edgelib/circular_arc_deg.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/edgelib/ellipse.py` & `puncturedfem-0.4.5/puncturedfem/mesh/edgelib/ellipse.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/edgelib/line.py` & `puncturedfem-0.4.5/puncturedfem/mesh/edgelib/line.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/edgelib/sine_wave.py` & `puncturedfem-0.4.5/puncturedfem/mesh/edgelib/sine_wave.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/edgelib/spline.py` & `puncturedfem-0.4.5/puncturedfem/mesh/edgelib/spline.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/edgelib/teardrop.py` & `puncturedfem-0.4.5/puncturedfem/mesh/edgelib/teardrop.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/mesh_exceptions.py` & `puncturedfem-0.4.5/puncturedfem/mesh/mesh_exceptions.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/meshlib/__builder__.py` & `puncturedfem-0.4.5/puncturedfem/mesh/meshlib/__builder__.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/meshlib/pacman.py` & `puncturedfem-0.4.5/puncturedfem/mesh/meshlib/pacman.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/meshlib/pacman_subdiv.py` & `puncturedfem-0.4.5/puncturedfem/mesh/meshlib/pacman_subdiv.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/meshlib/square_circular_hole.py` & `puncturedfem-0.4.5/puncturedfem/mesh/meshlib/square_circular_hole.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/planar_mesh.py` & `puncturedfem-0.4.5/puncturedfem/mesh/planar_mesh.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/quad.py` & `puncturedfem-0.4.5/puncturedfem/mesh/quad.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,17 @@
         s = self.t / np.pi - 1
         s2 = s * s
         c = (0.5 - 1 / p) * s * s2 + s / p + 0.5
         cp = c**p
         denom = cp + (1 - c) ** p
 
         self.t = (2 * np.pi) * cp / denom
-        self.wgt = (3 * (p - 2) * s2 + 2) * (c * (1 - c)) ** (p - 1) / denom**2
+        self.wgt = (
+            (3 * (p - 2) * s2 + 2) * (c * (1 - c)) ** (p - 1) / denom**2
+        )
 
     def martensen(self) -> None:
         """
         Martensen Quadrature
 
         E. Martensen, Über eine M
         ethode zum räumlichen Neumannschen Problem
```

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/split_edge.py` & `puncturedfem-0.4.5/puncturedfem/mesh/split_edge.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,19 @@
 from . import transform
 from .edge import Edge
 from .vert import Vert
 
 
 def split_edge(
     e: Edge,
-    t_split: Optional[Union[int, float, list[int | float], np.ndarray]] = None,
+    t_split: Optional[
+        Union[int, float, list[Union[int, float]], np.ndarray]
+    ] = None,
     num_edges: Optional[int] = None,
-) -> list[Edge] | tuple[Edge, Edge]:
+) -> Union[list[Edge], tuple[Edge, Edge]]:
     """
     Splits the edge e at the parameter t_split and returns the resulting edges.
     If t_split is a list of parameters, the edge is split at each parameter in
     the list. If num_edges is provided, the edge is split into num_edges equal
     parts.
 
     Parameters
```

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/transform.py` & `puncturedfem-0.4.5/puncturedfem/mesh/transform.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/mesh/vert.py` & `puncturedfem-0.4.5/puncturedfem/mesh/vert.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/plot/globfun_plot.py` & `puncturedfem-0.4.5/puncturedfem/plot/globfun_plot.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/plot/locfun_plot.py` & `puncturedfem-0.4.5/puncturedfem/plot/locfun_plot.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/plot/mesh_plot.py` & `puncturedfem-0.4.5/puncturedfem/plot/mesh_plot.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/plot/plot_util.py` & `puncturedfem-0.4.5/puncturedfem/plot/plot_util.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/plot/trace_plot.py` & `puncturedfem-0.4.5/puncturedfem/plot/trace_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,26 +28,26 @@
 
     fig_handle: plt.Figure
     t: np.ndarray
     traces: list[np.ndarray]
     x_ticks: np.ndarray
     x_labels: list[str]
     num_pts: int
-    fmt: str | list[str]
+    fmt: Union[str, list[str]]
     legend: tuple
     title: str
     log_scale: bool
     show_grid: bool
 
     def __init__(
         self,
         traces: Union[TraceLike, list[TraceLike]],
         K: MeshCell,
         quad_dict: dict[str, Quad],
-        fmt: str | list[str] = "k-",
+        fmt: Union[str, list[str]] = "k-",
         legend: tuple = (),
         title: str = "",
         log_scale: bool = False,
         show_grid: bool = True,
         max_num_ticks: int = 9,
     ) -> None:
         """
@@ -138,15 +138,15 @@
             if len(f) != self.num_pts:
                 raise ValueError(
                     "Each trace must be a numpy array of the same length as "
                     "the number of sampled boundary points of the MeshCell"
                 )
             self.traces.append(f)
 
-    def set_format(self, fmt: str | list[str]) -> None:
+    def set_format(self, fmt: Union[str, list[str]]) -> None:
         """
         Sets the format string(s) used to plot the traces.
         """
         self._validate_format(fmt)
         self.fmt = fmt
 
     def set_legend(self, legend: tuple) -> None:
@@ -189,27 +189,29 @@
         if legend:
             if len(legend) != len(self.traces):
                 raise ValueError(
                     "legend must be a tuple of strings of the same length as "
                     "traces"
                 )
 
-    def _validate_format(self, fmt: str | list[str]) -> None:
+    def _validate_format(self, fmt: Union[str, list[str]]) -> None:
         if isinstance(fmt, str):
             pass
         elif isinstance(fmt, list):
             if len(fmt) != len(self.traces):
                 raise ValueError(
                     "fmt must either be a string or a list of the same length "
                     "as traces"
                 )
         else:
             raise TypeError("fmt must be a string or a list of strings")
 
-    def _validate_traces(self, traces: np.ndarray | list[np.ndarray]) -> None:
+    def _validate_traces(
+        self, traces: Union[np.ndarray, list[np.ndarray]]
+    ) -> None:
         if isinstance(traces, np.ndarray):
             if len(traces) != self.num_pts:
                 raise ValueError(
                     "traces must be a numpy array of the same length as the "
                     "trace parameter"
                 )
         elif isinstance(traces, list):
```

### Comparing `puncturedfem-0.4.4.1/puncturedfem/solver/bilinear_form.py` & `puncturedfem-0.4.5/puncturedfem/solver/bilinear_form.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/solver/globfunsp.py` & `puncturedfem-0.4.5/puncturedfem/solver/globfunsp.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/solver/globkey.py` & `puncturedfem-0.4.5/puncturedfem/solver/globkey.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/solver/solver.py` & `puncturedfem-0.4.5/puncturedfem/solver/solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 solver.py
 =========
 
 Module containing the Solver class, which is a convenience class for solving
 the global linear system.
 """
 
+from typing import Union
+
 from numpy import ndarray, shape, zeros
 from scipy.sparse import csr_matrix
 from scipy.sparse.linalg import spsolve
 from tqdm import tqdm
 
 from ..util.print_color import Color, print_color
 from .bilinear_form import BilinearForm
@@ -211,15 +213,15 @@
 
             if verbose:
                 print("Evaluating bilinear form and right-hand side...")
 
             # loop over local functions
             loc_basis = V_K.get_basis()
 
-            range_num_funs: range | tqdm[int]
+            range_num_funs: Union[range, tqdm[int]]
             if verbose:
                 range_num_funs = tqdm(range(V_K.num_funs))
             else:
                 range_num_funs = range(V_K.num_funs)
 
             for i in range_num_funs:
                 v = loc_basis[i]
```

### Comparing `puncturedfem-0.4.4.1/puncturedfem/util/print_color.py` & `puncturedfem-0.4.5/puncturedfem/util/print_color.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/puncturedfem/util/types.py` & `puncturedfem-0.4.5/puncturedfem/util/types.py`

 * *Files identical despite different names*

### Comparing `puncturedfem-0.4.4.1/pyproject.toml` & `puncturedfem-0.4.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "puncturedfem"
-version = "0.4.4.1"
+version = "0.4.5"
 authors = ["Sam Reynolds <sreyn@proton.me>"]
 description = "A finite element method on meshes with curvilinear and multiply connected cells."
 readme = "README.md"
 license = "GNU General Public License v3.0"
 packages = [{include = "puncturedfem"}]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.9"
+deprecated = "^1.2.14"
 matplotlib = "^3.8.0"
 numba = "^0.59.1"
 numpy = "^1.26.0"
-scipy = "^1.11.2"
+scipy = "^1.12.0"
 tqdm = "^4.66.1"
 
 [project]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
```

### Comparing `puncturedfem-0.4.4.1/PKG-INFO` & `puncturedfem-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: puncturedfem
-Version: 0.4.4.1
+Version: 0.4.5
 Summary: A finite element method on meshes with curvilinear and multiply connected cells.
 License: GNU General Public License v3.0
 Author: Sam Reynolds
 Author-email: sreyn@proton.me
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: deprecated (>=1.2.14,<2.0.0)
 Requires-Dist: matplotlib (>=3.8.0,<4.0.0)
 Requires-Dist: numba (>=0.59.1,<0.60.0)
 Requires-Dist: numpy (>=1.26.0,<2.0.0)
-Requires-Dist: scipy (>=1.11.2,<2.0.0)
+Requires-Dist: scipy (>=1.12.0,<2.0.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Punctured FEM
 
 https://github.com/samreynoldsmath/PuncturedFEM
 
@@ -66,15 +69,15 @@
 ## Installation
 This package is available on [PyPI](https://pypi.org/project/puncturedfem/), and can be installed with pip:
 ```bash
 pip install puncturedfem
 ```
 
 ### Dependencies
-This project is written in Python 3.11 and uses the following packages:
+This project requires Python 3.9 or higher and uses the following packages:
 - [matplotlib](https://matplotlib.org/) (plotting)
 - [numba](https://numba.pydata.org/) (just-in-time compilation)
 - [numpy](https://numpy.org/) (arrays, FFT)
 - [scipy](https://www.scipy.org/) (sparse matrices, GMRES)
 - [tqdm](https://tqdm.github.io/) (progress bars)
 
 Furthermore, this repo contains examples presented with [Jupyter notebooks](https://jupyter.org/).
```

