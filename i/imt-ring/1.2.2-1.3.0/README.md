# Comparing `tmp/imt_ring-1.2.2.tar.gz` & `tmp/imt_ring-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imt_ring-1.2.2.tar", last modified: Wed Apr 24 11:18:10 2024, max compression
+gzip compressed data, was "imt_ring-1.3.0.tar", last modified: Wed Apr 24 11:18:18 2024, max compression
```

## Comparing `imt_ring-1.2.2.tar` & `imt_ring-1.3.0.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.932594 imt_ring-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-24 11:18:10.932594 imt_ring-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-24 11:18:06.000000 imt_ring-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-24 11:18:06.000000 imt_ring-1.2.2/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-24 11:18:10.932594 imt_ring-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.896594 imt_ring-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.928594 imt_ring-1.2.2/src/imt_ring.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-24 11:18:10.000000 imt_ring-1.2.2/src/imt_ring.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-24 11:18:10.000000 imt_ring-1.2.2/src/imt_ring.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:18:10.000000 imt_ring-1.2.2/src/imt_ring.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-24 11:18:10.000000 imt_ring-1.2.2/src/imt_ring.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 11:18:10.000000 imt_ring-1.2.2/src/imt_ring.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.900594 imt_ring-1.2.2/src/ring/
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algebra.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.900594 imt_ring-1.2.2/src/ring/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13340 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/_random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.904594 imt_ring-1.2.2/src/ring/algorithms/custom_joints/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/custom_joints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/custom_joints/rr_imp_joint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/custom_joints/rr_joint.py
--rw-r--r--   0 runner    (1001) docker     (127)    13680 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/custom_joints/suntay.py
--rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/dynamics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.904594 imt_ring-1.2.2/src/ring/algorithms/generator/
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14952 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/generator/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/generator/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/generator/motion_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/generator/pd_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/generator/randomize.py
--rw-r--r--   0 runner    (1001) docker     (127)    12782 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/generator/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/generator/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    25270 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/jcalc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)    18005 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)    33566 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.904594 imt_ring-1.2.2/src/ring/io/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.908594 imt_ring-1.2.2/src/ring/io/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/branched.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.908594 imt_ring-1.2.2/src/ring/io/examples/exclude/
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/exclude/knee_trans_dof.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/exclude/standard_sys.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/exclude/standard_sys_rr_imp.xml
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/inv_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/knee_flexible_imus.xml
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/spherical_stiff.xml
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/symmetric.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/test_all_1.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/test_all_2.xml
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/test_ang0_pos0.xml
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/test_control.xml
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/test_double_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/test_free.xml
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/test_kinematics.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.908594 imt_ring-1.2.2/src/ring/io/examples/test_morph_system/
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/test_morph_system/four_seg_seg1.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/test_morph_system/four_seg_seg3.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/test_randomize_position.xml
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/test_sensors.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/test_three_seg_seg2.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/test_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.908594 imt_ring-1.2.2/src/ring/io/xml/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/xml/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/xml/from_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/xml/test_from_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/xml/test_to_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/xml/to_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)    12193 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/maths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.912594 imt_ring-1.2.2/src/ring/ml/
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/ml/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13109 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/ml/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/ml/ml_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/ml/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.912594 imt_ring-1.2.2/src/ring/ml/params/
--rw-r--r--   0 runner    (1001) docker     (127)  9355838 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/ml/params/0x13e3518065c21cd8.pickle
--rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/ml/ringnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/ml/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/ml/training_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.924594 imt_ring-1.2.2/src/ring/rendering/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/rendering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/rendering/base_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/rendering/mujoco_render.py
--rw-r--r--   0 runner    (1001) docker     (127)    10260 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/rendering/vispy_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/rendering/vispy_visuals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.924594 imt_ring-1.2.2/src/ring/sim2real/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/sim2real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/sim2real/sim2real.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/spatial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.924594 imt_ring-1.2.2/src/ring/sys_composer/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/sys_composer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/sys_composer/delete_sys.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/sys_composer/inject_sys.py
--rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/sys_composer/morph_sys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.924594 imt_ring-1.2.2/src/ring/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/utils/batchsize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/utils/colab.py
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/utils/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/utils/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.928594 imt_ring-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_custom_joints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_jcalc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_jit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_maths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_ml_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_motion_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_pd_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_randomize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_rcmg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_sim2real.py
--rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_sys_composer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_train.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.610648 imt_ring-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-24 11:18:18.610648 imt_ring-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-24 11:18:07.000000 imt_ring-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-24 11:18:07.000000 imt_ring-1.3.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-24 11:18:18.610648 imt_ring-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.578647 imt_ring-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.610648 imt_ring-1.3.0/src/imt_ring.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-24 11:18:18.000000 imt_ring-1.3.0/src/imt_ring.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-24 11:18:18.000000 imt_ring-1.3.0/src/imt_ring.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:18:18.000000 imt_ring-1.3.0/src/imt_ring.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-24 11:18:18.000000 imt_ring-1.3.0/src/imt_ring.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 11:18:18.000000 imt_ring-1.3.0/src/imt_ring.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.582647 imt_ring-1.3.0/src/ring/
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algebra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.582647 imt_ring-1.3.0/src/ring/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13340 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/_random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.586647 imt_ring-1.3.0/src/ring/algorithms/custom_joints/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/custom_joints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/custom_joints/rr_imp_joint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/custom_joints/rr_joint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13680 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/custom_joints/suntay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/dynamics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.586647 imt_ring-1.3.0/src/ring/algorithms/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14952 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/generator/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/generator/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/generator/motion_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/generator/pd_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/generator/randomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12782 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/generator/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/generator/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28213 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/jcalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18005 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/algorithms/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33566 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.586647 imt_ring-1.3.0/src/ring/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.590648 imt_ring-1.3.0/src/ring/io/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/branched.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.590648 imt_ring-1.3.0/src/ring/io/examples/exclude/
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/exclude/knee_trans_dof.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/exclude/standard_sys.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/exclude/standard_sys_rr_imp.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/inv_pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/knee_flexible_imus.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/spherical_stiff.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/symmetric.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/test_all_1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/test_all_2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/test_ang0_pos0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/test_control.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/test_double_pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/test_free.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/test_kinematics.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.590648 imt_ring-1.3.0/src/ring/io/examples/test_morph_system/
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/test_morph_system/four_seg_seg1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/test_morph_system/four_seg_seg3.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/test_randomize_position.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/test_sensors.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples/test_three_seg_seg2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.590648 imt_ring-1.3.0/src/ring/io/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/xml/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/xml/from_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/xml/test_from_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/xml/test_to_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/io/xml/to_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12193 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/maths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.590648 imt_ring-1.3.0/src/ring/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/ml/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/ml/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/ml/ml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/ml/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.590648 imt_ring-1.3.0/src/ring/ml/params/
+-rw-r--r--   0 runner    (1001) docker     (127)  9355838 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/ml/params/0x13e3518065c21cd8.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/ml/ringnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/ml/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/ml/training_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.602648 imt_ring-1.3.0/src/ring/rendering/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/rendering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/rendering/base_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/rendering/mujoco_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10260 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/rendering/vispy_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/rendering/vispy_visuals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.606648 imt_ring-1.3.0/src/ring/sim2real/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/sim2real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/sim2real/sim2real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/spatial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.606648 imt_ring-1.3.0/src/ring/sys_composer/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/sys_composer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/sys_composer/delete_sys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/sys_composer/inject_sys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/sys_composer/morph_sys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.606648 imt_ring-1.3.0/src/ring/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/utils/batchsize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/utils/colab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/utils/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/utils/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-24 11:18:07.000000 imt_ring-1.3.0/src/ring/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:18.610648 imt_ring-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_custom_joints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_jcalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_jit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_maths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_ml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_motion_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_pd_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_randomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_rcmg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_sim2real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_sys_composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-24 11:18:07.000000 imt_ring-1.3.0/tests/test_utils.py
```

### Comparing `imt_ring-1.2.2/PKG-INFO` & `imt_ring-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imt-ring
-Version: 1.2.2
+Version: 1.3.0
 Summary: RING: Recurrent Inertial Graph-based Estimator
 Author-email: Simon Bachhuber <simon.bachhuber@fau.de>
 Project-URL: Homepage, https://github.com/SimiPixel/ring
 Project-URL: Issues, https://github.com/SimiPixel/ring/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `imt_ring-1.2.2/pyproject.toml` & `imt_ring-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "imt-ring"
-version = "1.2.2"
+version = "1.3.0"
 authors = [
   { name="Simon Bachhuber", email="simon.bachhuber@fau.de" },
 ]
 description = "RING: Recurrent Inertial Graph-based Estimator"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `imt_ring-1.2.2/readme.md` & `imt_ring-1.3.0/readme.md`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/imt_ring.egg-info/PKG-INFO` & `imt_ring-1.3.0/src/imt_ring.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imt-ring
-Version: 1.2.2
+Version: 1.3.0
 Summary: RING: Recurrent Inertial Graph-based Estimator
 Author-email: Simon Bachhuber <simon.bachhuber@fau.de>
 Project-URL: Homepage, https://github.com/SimiPixel/ring
 Project-URL: Issues, https://github.com/SimiPixel/ring/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `imt_ring-1.2.2/src/imt_ring.egg-info/SOURCES.txt` & `imt_ring-1.3.0/src/imt_ring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/__init__.py` & `imt_ring-1.3.0/src/ring/__init__.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/algebra.py` & `imt_ring-1.3.0/src/ring/algebra.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/algorithms/__init__.py` & `imt_ring-1.3.0/src/ring/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/algorithms/_random.py` & `imt_ring-1.3.0/src/ring/algorithms/_random.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/algorithms/custom_joints/rr_imp_joint.py` & `imt_ring-1.3.0/src/ring/algorithms/custom_joints/rr_imp_joint.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/algorithms/custom_joints/rr_joint.py` & `imt_ring-1.3.0/src/ring/algorithms/custom_joints/rr_joint.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/algorithms/custom_joints/suntay.py` & `imt_ring-1.3.0/src/ring/algorithms/custom_joints/suntay.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/algorithms/dynamics.py` & `imt_ring-1.3.0/src/ring/algorithms/dynamics.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/algorithms/generator/__init__.py` & `imt_ring-1.3.0/src/ring/algorithms/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/algorithms/generator/base.py` & `imt_ring-1.3.0/src/ring/algorithms/generator/base.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/algorithms/generator/batch.py` & `imt_ring-1.3.0/src/ring/algorithms/generator/batch.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/algorithms/generator/motion_artifacts.py` & `imt_ring-1.3.0/src/ring/algorithms/generator/motion_artifacts.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/algorithms/generator/pd_control.py` & `imt_ring-1.3.0/src/ring/algorithms/generator/pd_control.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/algorithms/generator/randomize.py` & `imt_ring-1.3.0/src/ring/algorithms/generator/randomize.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/algorithms/generator/transforms.py` & `imt_ring-1.3.0/src/ring/algorithms/generator/transforms.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/algorithms/generator/types.py` & `imt_ring-1.3.0/src/ring/algorithms/generator/types.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/algorithms/jcalc.py` & `imt_ring-1.3.0/src/ring/algorithms/jcalc.py`

 * *Files 7% similar despite different names*

```diff
@@ -84,14 +84,126 @@
             "dpos_max",
         ]:
             kwargs[key] = 0.0
         nomotion_config = MotionConfig(**kwargs)
         assert nomotion_config.is_feasible()
         return nomotion_config
 
+    @staticmethod
+    def from_register(name: str) -> "MotionConfig":
+        return _registered_motion_configs[name]
+
+
+_registered_motion_configs = {
+    "hinUndHer": MotionConfig(
+        t_min=0.3,
+        t_max=1.5,
+        dang_max=3.0,
+        delta_ang_min=0.5,
+        pos_min=-1.5,
+        pos_max=1.5,
+        randomized_interpolation_angle=True,
+        cor=True,
+    ),
+    "langsam": MotionConfig(
+        t_min=0.2,
+        t_max=1.25,
+        dang_max=2.0,
+        randomized_interpolation_angle=True,
+        dang_max_free_spherical=2.0,
+        cdf_bins_min=1,
+        cdf_bins_max=3,
+        pos_min=-1.5,
+        pos_max=1.5,
+        cor=True,
+    ),
+    "standard": MotionConfig(
+        randomized_interpolation_angle=True,
+        cdf_bins_min=1,
+        cdf_bins_max=5,
+        cor=True,
+    ),
+    "expFast": MotionConfig(
+        t_min=0.4,
+        t_max=1.1,
+        dang_max=jnp.deg2rad(180),
+        delta_ang_min=jnp.deg2rad(60),
+        delta_ang_max=jnp.deg2rad(110),
+        pos_min=-1.5,
+        pos_max=1.5,
+        range_of_motion_hinge_method="sigmoid",
+        randomized_interpolation_angle=True,
+        cdf_bins_min=1,
+        cdf_bins_max=3,
+        cor=True,
+    ),
+    "expSlow": MotionConfig(
+        t_min=0.75,
+        t_max=3.0,
+        dang_min=0.1,
+        dang_max=1.0,
+        dang_min_free_spherical=0.1,
+        delta_ang_min=0.4,
+        dang_max_free_spherical=1.0,
+        delta_ang_max_free_spherical=1.0,
+        dpos_max=0.3,
+        cor_dpos_max=0.3,
+        range_of_motion_hinge_method="sigmoid",
+        randomized_interpolation_angle=True,
+        cdf_bins_min=1,
+        cdf_bins_max=5,
+        cor=True,
+    ),
+    "expFastNoSig": MotionConfig(
+        t_min=0.4,
+        t_max=1.1,
+        dang_max=jnp.deg2rad(180),
+        delta_ang_min=jnp.deg2rad(60),
+        delta_ang_max=jnp.deg2rad(110),
+        pos_min=-1.5,
+        pos_max=1.5,
+        randomized_interpolation_angle=True,
+        cdf_bins_min=1,
+        cdf_bins_max=3,
+        cor=True,
+    ),
+    "expSlowNoSig": MotionConfig(
+        t_min=0.75,
+        t_max=3.0,
+        dang_min=0.1,
+        dang_max=1.0,
+        dang_min_free_spherical=0.1,
+        delta_ang_min=0.4,
+        dang_max_free_spherical=1.0,
+        delta_ang_max_free_spherical=1.0,
+        dpos_max=0.3,
+        cor_dpos_max=0.3,
+        randomized_interpolation_angle=True,
+        cdf_bins_min=1,
+        cdf_bins_max=3,
+        cor=True,
+    ),
+    "verySlow": MotionConfig(
+        t_min=1.5,
+        t_max=5.0,
+        dang_min=jnp.deg2rad(1),
+        dang_max=jnp.deg2rad(30),
+        delta_ang_min=jnp.deg2rad(20),
+        dang_min_free_spherical=jnp.deg2rad(1),
+        dang_max_free_spherical=jnp.deg2rad(10),
+        delta_ang_min_free_spherical=jnp.deg2rad(5),
+        dpos_max=0.3,
+        cor_dpos_max=0.3,
+        randomized_interpolation_angle=True,
+        cdf_bins_min=1,
+        cdf_bins_max=3,
+        cor=True,
+    ),
+}
+
 
 def _is_feasible_config1(c: MotionConfig) -> bool:
     t_min, t_max = c.t_min, _to_float(c.t_max, 0.0)
 
     def dx_deltax_check(dx_min, dx_max, deltax_min, deltax_max) -> bool:
         dx_min, dx_max, deltax_min, deltax_max = map(
             (lambda v: _to_float(v, 0.0)), (dx_min, dx_max, deltax_min, deltax_max)
```

### Comparing `imt_ring-1.2.2/src/ring/algorithms/kinematics.py` & `imt_ring-1.3.0/src/ring/algorithms/kinematics.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/algorithms/sensors.py` & `imt_ring-1.3.0/src/ring/algorithms/sensors.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/base.py` & `imt_ring-1.3.0/src/ring/base.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/io/examples/branched.xml` & `imt_ring-1.3.0/src/ring/io/examples/branched.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/io/examples/exclude/knee_trans_dof.xml` & `imt_ring-1.3.0/src/ring/io/examples/exclude/knee_trans_dof.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/io/examples/exclude/standard_sys.xml` & `imt_ring-1.3.0/src/ring/io/examples/exclude/standard_sys.xml`

 * *Files 0% similar despite different names*

#### Comparing `imt_ring-1.2.2/src/ring/io/examples/exclude/standard_sys.xml` & `imt_ring-1.3.0/src/ring/io/examples/exclude/standard_sys.xml`

```diff
@@ -1,106 +1,106 @@
 <?xml version="1.0" encoding="utf-8"?>
 <x_xy model="arm_1Seg">
   <options dt="0.01" gravity="0.0 0.0 9.81"/>
   <worldbody>
-    <body joint="free" name="seg2_1Seg" pos="0.4 0.0 0.0" pos_min="0.2 -0.05 -0.05" pos_max="0.55 0.05 0.05" damping="5.0 5.0 5.0 25.0 25.0 25.0">
+    <body joint="free" name="seg3_1Seg" pos="0.4 0.0 0.0" pos_min="0.2 -0.05 -0.05" pos_max="0.55 0.05 0.05" damping="5.0 5.0 5.0 25.0 25.0 25.0">
       <geom pos="0.1 0.0 0.0" mass="1.0" color="dustin_exp_blue" edge_color="black" type="box" dim="0.2 0.05 0.05"/>
       <geom pos="0.05 0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
       <geom pos="0.15 -0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
-      <omc pos="0.0 0.0 -0.02" name="seg2" pos_marker="1"/>
-      <body joint="frozen" name="imu2_1Seg" pos="0.099999994 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.15 0.05 0.05">
+      <omc pos="0.0 0.0 -0.02" name="seg3" pos_marker="1"/>
+      <body joint="frozen" name="imu3_1Seg" pos="0.099999994 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.15 0.05 0.05">
         <geom mass="0.1" color="dustin_exp_orange" edge_color="black" type="box" dim="0.05 0.03 0.02"/>
-        <omc pos="0.1 0.0 0.015" name="seg2" pos_marker="1"/>
+        <omc pos="0.1 0.0 0.015" name="seg3" pos_marker="1"/>
       </body>
     </body>
-    <body joint="free" name="seg2_2Seg" pos="0.4 0.0 0.0" pos_min="0.2 -0.05 -0.05" pos_max="0.55 0.05 0.05" damping="5.0 5.0 5.0 25.0 25.0 25.0">
+    <body joint="free" name="seg3_2Seg" pos="0.4 0.0 0.0" pos_min="0.2 -0.05 -0.05" pos_max="0.55 0.05 0.05" damping="5.0 5.0 5.0 25.0 25.0 25.0">
       <geom pos="0.1 0.0 0.0" mass="1.0" color="dustin_exp_blue" edge_color="black" type="box" dim="0.2 0.05 0.05"/>
       <geom pos="0.05 0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
       <geom pos="0.15 -0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
-      <omc pos="0.0 0.0 -0.02" name="seg2" pos_marker="1"/>
-      <body joint="frozen" name="imu2_2Seg" pos="0.099999994 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.15 0.05 0.05">
+      <omc pos="0.0 0.0 -0.02" name="seg3" pos_marker="1"/>
+      <body joint="frozen" name="imu3_2Seg" pos="0.099999994 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.15 0.05 0.05">
         <geom mass="0.1" color="dustin_exp_orange" edge_color="black" type="box" dim="0.05 0.03 0.02"/>
-        <omc pos="0.1 0.0 0.015" name="seg2" pos_marker="1"/>
+        <omc pos="0.1 0.0 0.015" name="seg3" pos_marker="1"/>
       </body>
-      <body joint="ry" name="seg3_2Seg" pos="0.20000002 0.0 0.0" pos_min="0.0 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3.0">
+      <body joint="ry" name="seg4_2Seg" pos="0.20000002 0.0 0.0" pos_min="0.0 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3.0">
         <geom pos="0.1 0.0 0.0" mass="1.0" color="dustin_exp_white" edge_color="black" type="box" dim="0.2 0.05 0.05"/>
         <geom pos="0.1 0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
         <geom pos="0.15 -0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
-        <omc pos="0.0 0.0 -0.02" name="seg3" pos_marker="2"/>
-        <body joint="frozen" name="imu3_2Seg" pos="0.100000024 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.14999998 0.05 0.05">
+        <omc pos="0.0 0.0 -0.02" name="seg4" pos_marker="2"/>
+        <body joint="frozen" name="imu4_2Seg" pos="0.100000024 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.14999998 0.05 0.05">
           <geom mass="0.1" color="dustin_exp_orange" edge_color="black" type="box" dim="0.05 0.03 0.02"/>
-          <omc pos="0.1 0.0 0.015" name="seg3" pos_marker="2"/>
+          <omc pos="0.1 0.0 0.015" name="seg4" pos_marker="2"/>
         </body>
       </body>
     </body>
-    <body joint="free" name="seg2_3Seg" pos="0.4 0.0 0.0" pos_min="0.2 -0.05 -0.05" pos_max="0.55 0.05 0.05" damping="5.0 5.0 5.0 25.0 25.0 25.0">
+    <body joint="free" name="seg3_3Seg" pos="0.4 0.0 0.0" pos_min="0.2 -0.05 -0.05" pos_max="0.55 0.05 0.05" damping="5.0 5.0 5.0 25.0 25.0 25.0">
       <geom pos="0.1 0.0 0.0" mass="1.0" color="dustin_exp_blue" edge_color="black" type="box" dim="0.2 0.05 0.05"/>
       <geom pos="0.05 0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
       <geom pos="0.15 -0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
-      <omc pos="0.0 0.0 -0.02" name="seg2" pos_marker="1"/>
-      <body joint="frozen" name="imu2_3Seg" pos="0.099999994 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.15 0.05 0.05">
+      <omc pos="0.0 0.0 -0.02" name="seg3" pos_marker="1"/>
+      <body joint="frozen" name="imu3_3Seg" pos="0.099999994 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.15 0.05 0.05">
         <geom mass="0.1" color="dustin_exp_orange" edge_color="black" type="box" dim="0.05 0.03 0.02"/>
-        <omc pos="0.1 0.0 0.015" name="seg2" pos_marker="1"/>
+        <omc pos="0.1 0.0 0.015" name="seg3" pos_marker="1"/>
       </body>
-      <body joint="ry" name="seg3_3Seg" pos="0.20000002 0.0 0.0" pos_min="0.0 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3.0">
+      <body joint="ry" name="seg4_3Seg" pos="0.20000002 0.0 0.0" pos_min="0.0 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3.0">
         <geom pos="0.1 0.0 0.0" mass="1.0" color="dustin_exp_white" edge_color="black" type="box" dim="0.2 0.05 0.05"/>
         <geom pos="0.1 0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
         <geom pos="0.15 -0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
-        <omc pos="0.0 0.0 -0.02" name="seg3" pos_marker="2"/>
-        <body joint="frozen" name="imu3_3Seg" pos="0.100000024 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.14999998 0.05 0.05">
+        <omc pos="0.0 0.0 -0.02" name="seg4" pos_marker="2"/>
+        <body joint="frozen" name="imu4_3Seg" pos="0.100000024 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.14999998 0.05 0.05">
           <geom mass="0.1" color="dustin_exp_orange" edge_color="black" type="box" dim="0.05 0.03 0.02"/>
-          <omc pos="0.1 0.0 0.015" name="seg3" pos_marker="2"/>
+          <omc pos="0.1 0.0 0.015" name="seg4" pos_marker="2"/>
         </body>
-        <body joint="rz" name="seg4_3Seg" pos="0.19999999 0.0 0.0" pos_min="0.0 -0.05 -0.05" pos_max="0.35000002 0.05 0.05" damping="3.0">
+        <body joint="rz" name="seg5_3Seg" pos="0.19999999 0.0 0.0" pos_min="0.0 -0.05 -0.05" pos_max="0.35000002 0.05 0.05" damping="3.0">
           <geom pos="0.1 0.0 0.0" mass="1.0" color="dustin_exp_white" edge_color="black" type="box" dim="0.2 0.05 0.05"/>
           <geom pos="0.03 -0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
           <geom pos="0.17 -0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
-          <omc pos="0.0 0.0 -0.02" name="seg4" pos_marker="4"/>
-          <body joint="frozen" name="imu4_3Seg" pos="0.100000024 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.15000004 0.05 0.05">
+          <omc pos="0.0 0.0 -0.02" name="seg5" pos_marker="4"/>
+          <body joint="frozen" name="imu5_3Seg" pos="0.100000024 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.15000004 0.05 0.05">
             <geom mass="0.1" color="dustin_exp_orange" edge_color="black" type="box" dim="0.05 0.03 0.02"/>
-            <omc pos="0.1 0.0 0.015" name="seg4" pos_marker="4"/>
+            <omc pos="0.1 0.0 0.015" name="seg5" pos_marker="4"/>
           </body>
         </body>
       </body>
     </body>
-    <body joint="free" name="seg5_4Seg" pos="0.2 0.0 0.0" pos_min="0.15 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="5.0 5.0 5.0 25.0 25.0 25.0">
+    <body joint="free" name="seg2_4Seg" pos="0.2 0.0 0.0" pos_min="0.15 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="5.0 5.0 5.0 25.0 25.0 25.0">
       <geom pos="0.1 0.0 0.0" mass="1.0" color="dustin_exp_white" edge_color="black" type="box" dim="0.2 0.05 0.05"/>
       <geom pos="0.03 -0.05 0.0" mass="0.1" color="dustin_exp_white" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
       <geom pos="0.17 -0.05 0.0" mass="0.1" color="dustin_exp_white" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
-      <omc pos="0.0 0.0 -0.02" name="seg5" pos_marker="2"/>
-      <body joint="frozen" name="imu5_4Seg" pos="0.10000001 0.0 0.035" pos_min="0.049999997 -0.05 -0.05" pos_max="0.15000002 0.05 0.05">
+      <omc pos="0.0 0.0 -0.02" name="seg2" pos_marker="2"/>
+      <body joint="frozen" name="imu2_4Seg" pos="0.10000001 0.0 0.035" pos_min="0.049999997 -0.05 -0.05" pos_max="0.15000002 0.05 0.05">
         <geom mass="0.1" color="dustin_exp_orange" edge_color="black" type="box" dim="0.05 0.03 0.02"/>
-        <omc pos="0.1 0.0 0.015" name="seg5" pos_marker="2"/>
+        <omc pos="0.1 0.0 0.015" name="seg2" pos_marker="2"/>
       </body>
-      <body joint="rx" name="seg2_4Seg" pos="0.2 0.0 0.0" pos_min="0.0 -0.05 -0.05" pos_max="0.35000002 0.05 0.05" damping="3.0">
+      <body joint="rx" name="seg3_4Seg" pos="0.2 0.0 0.0" pos_min="0.0 -0.05 -0.05" pos_max="0.35000002 0.05 0.05" damping="3.0">
         <geom pos="0.1 0.0 0.0" mass="1.0" color="dustin_exp_blue" edge_color="black" type="box" dim="0.2 0.05 0.05"/>
         <geom pos="0.05 0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
         <geom pos="0.15 -0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
-        <omc pos="0.0 0.0 -0.02" name="seg2" pos_marker="1"/>
-        <body joint="frozen" name="imu2_4Seg" pos="0.099999994 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.15 0.05 0.05">
+        <omc pos="0.0 0.0 -0.02" name="seg3" pos_marker="1"/>
+        <body joint="frozen" name="imu3_4Seg" pos="0.099999994 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.15 0.05 0.05">
           <geom mass="0.1" color="dustin_exp_orange" edge_color="black" type="box" dim="0.05 0.03 0.02"/>
-          <omc pos="0.1 0.0 0.015" name="seg2" pos_marker="1"/>
+          <omc pos="0.1 0.0 0.015" name="seg3" pos_marker="1"/>
         </body>
-        <body joint="ry" name="seg3_4Seg" pos="0.20000002 0.0 0.0" pos_min="0.0 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3.0">
+        <body joint="ry" name="seg4_4Seg" pos="0.20000002 0.0 0.0" pos_min="0.0 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3.0">
           <geom pos="0.1 0.0 0.0" mass="1.0" color="dustin_exp_white" edge_color="black" type="box" dim="0.2 0.05 0.05"/>
           <geom pos="0.1 0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
           <geom pos="0.15 -0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
-          <omc pos="0.0 0.0 -0.02" name="seg3" pos_marker="2"/>
-          <body joint="frozen" name="imu3_4Seg" pos="0.100000024 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.14999998 0.05 0.05">
+          <omc pos="0.0 0.0 -0.02" name="seg4" pos_marker="2"/>
+          <body joint="frozen" name="imu4_4Seg" pos="0.100000024 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.14999998 0.05 0.05">
             <geom mass="0.1" color="dustin_exp_orange" edge_color="black" type="box" dim="0.05 0.03 0.02"/>
-            <omc pos="0.1 0.0 0.015" name="seg3" pos_marker="2"/>
+            <omc pos="0.1 0.0 0.015" name="seg4" pos_marker="2"/>
           </body>
-          <body joint="rz" name="seg4_4Seg" pos="0.19999999 0.0 0.0" pos_min="0.0 -0.05 -0.05" pos_max="0.35000002 0.05 0.05" damping="3.0">
+          <body joint="rz" name="seg5_4Seg" pos="0.19999999 0.0 0.0" pos_min="0.0 -0.05 -0.05" pos_max="0.35000002 0.05 0.05" damping="3.0">
             <geom pos="0.1 0.0 0.0" mass="1.0" color="dustin_exp_white" edge_color="black" type="box" dim="0.2 0.05 0.05"/>
             <geom pos="0.03 -0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
             <geom pos="0.17 -0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
-            <omc pos="0.0 0.0 -0.02" name="seg4" pos_marker="4"/>
-            <body joint="frozen" name="imu4_4Seg" pos="0.100000024 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.15000004 0.05 0.05">
+            <omc pos="0.0 0.0 -0.02" name="seg5" pos_marker="4"/>
+            <body joint="frozen" name="imu5_4Seg" pos="0.100000024 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.15000004 0.05 0.05">
               <geom mass="0.1" color="dustin_exp_orange" edge_color="black" type="box" dim="0.05 0.03 0.02"/>
-              <omc pos="0.1 0.0 0.015" name="seg4" pos_marker="4"/>
+              <omc pos="0.1 0.0 0.015" name="seg5" pos_marker="4"/>
             </body>
           </body>
         </body>
       </body>
     </body>
   </worldbody>
 </x_xy>
```

### Comparing `imt_ring-1.2.2/src/ring/io/examples/exclude/standard_sys_rr_imp.xml` & `imt_ring-1.3.0/src/ring/io/examples/exclude/standard_sys_rr_imp.xml`

 * *Files 0% similar despite different names*

#### Comparing `imt_ring-1.2.2/src/ring/io/examples/exclude/standard_sys_rr_imp.xml` & `imt_ring-1.3.0/src/ring/io/examples/exclude/standard_sys_rr_imp.xml`

```diff
@@ -1,106 +1,106 @@
 <?xml version="1.0" encoding="utf-8"?>
 <x_xy model="arm_1Seg">
   <options dt="0.01" gravity="0.0 0.0 9.81"/>
   <worldbody>
-    <body joint="free" name="seg2_1Seg" pos="0.4 0.0 0.0" pos_min="0.2 -0.05 -0.05" pos_max="0.55 0.05 0.05" damping="5.0 5.0 5.0 25.0 25.0 25.0">
+    <body joint="free" name="seg3_1Seg" pos="0.4 0.0 0.0" pos_min="0.2 -0.05 -0.05" pos_max="0.55 0.05 0.05" damping="5.0 5.0 5.0 25.0 25.0 25.0">
       <geom pos="0.1 0.0 0.0" mass="1.0" color="dustin_exp_blue" edge_color="black" type="box" dim="0.2 0.05 0.05"/>
       <geom pos="0.05 0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
       <geom pos="0.15 -0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
-      <omc pos="0.0 0.0 -0.02" name="seg2" pos_marker="1"/>
-      <body joint="frozen" name="imu2_1Seg" pos="0.099999994 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.15 0.05 0.05">
+      <omc pos="0.0 0.0 -0.02" name="seg3" pos_marker="1"/>
+      <body joint="frozen" name="imu3_1Seg" pos="0.099999994 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.15 0.05 0.05">
         <geom mass="0.1" color="dustin_exp_orange" edge_color="black" type="box" dim="0.05 0.03 0.02"/>
-        <omc pos="0.1 0.0 0.015" name="seg2" pos_marker="1"/>
+        <omc pos="0.1 0.0 0.015" name="seg3" pos_marker="1"/>
       </body>
     </body>
-    <body joint="free" name="seg2_2Seg" pos="0.4 0.0 0.0" pos_min="0.2 -0.05 -0.05" pos_max="0.55 0.05 0.05" damping="5.0 5.0 5.0 25.0 25.0 25.0">
+    <body joint="free" name="seg3_2Seg" pos="0.4 0.0 0.0" pos_min="0.2 -0.05 -0.05" pos_max="0.55 0.05 0.05" damping="5.0 5.0 5.0 25.0 25.0 25.0">
       <geom pos="0.1 0.0 0.0" mass="1.0" color="dustin_exp_blue" edge_color="black" type="box" dim="0.2 0.05 0.05"/>
       <geom pos="0.05 0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
       <geom pos="0.15 -0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
-      <omc pos="0.0 0.0 -0.02" name="seg2" pos_marker="1"/>
-      <body joint="frozen" name="imu2_2Seg" pos="0.099999994 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.15 0.05 0.05">
+      <omc pos="0.0 0.0 -0.02" name="seg3" pos_marker="1"/>
+      <body joint="frozen" name="imu3_2Seg" pos="0.099999994 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.15 0.05 0.05">
         <geom mass="0.1" color="dustin_exp_orange" edge_color="black" type="box" dim="0.05 0.03 0.02"/>
-        <omc pos="0.1 0.0 0.015" name="seg2" pos_marker="1"/>
+        <omc pos="0.1 0.0 0.015" name="seg3" pos_marker="1"/>
       </body>
-      <body joint="rr_imp" name="seg3_2Seg" pos="0.20000002 0.0 0.0" pos_min="0.0 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3.0 3.0">
+      <body joint="rr_imp" name="seg4_2Seg" pos="0.20000002 0.0 0.0" pos_min="0.0 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3.0 3.0">
         <geom pos="0.1 0.0 0.0" mass="1.0" color="dustin_exp_white" edge_color="black" type="box" dim="0.2 0.05 0.05"/>
         <geom pos="0.1 0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
         <geom pos="0.15 -0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
-        <omc pos="0.0 0.0 -0.02" name="seg3" pos_marker="2"/>
-        <body joint="frozen" name="imu3_2Seg" pos="0.100000024 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.14999998 0.05 0.05">
+        <omc pos="0.0 0.0 -0.02" name="seg4" pos_marker="2"/>
+        <body joint="frozen" name="imu4_2Seg" pos="0.100000024 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.14999998 0.05 0.05">
           <geom mass="0.1" color="dustin_exp_orange" edge_color="black" type="box" dim="0.05 0.03 0.02"/>
-          <omc pos="0.1 0.0 0.015" name="seg3" pos_marker="2"/>
+          <omc pos="0.1 0.0 0.015" name="seg4" pos_marker="2"/>
         </body>
       </body>
     </body>
-    <body joint="free" name="seg2_3Seg" pos="0.4 0.0 0.0" pos_min="0.2 -0.05 -0.05" pos_max="0.55 0.05 0.05" damping="5.0 5.0 5.0 25.0 25.0 25.0">
+    <body joint="free" name="seg3_3Seg" pos="0.4 0.0 0.0" pos_min="0.2 -0.05 -0.05" pos_max="0.55 0.05 0.05" damping="5.0 5.0 5.0 25.0 25.0 25.0">
       <geom pos="0.1 0.0 0.0" mass="1.0" color="dustin_exp_blue" edge_color="black" type="box" dim="0.2 0.05 0.05"/>
       <geom pos="0.05 0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
       <geom pos="0.15 -0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
-      <omc pos="0.0 0.0 -0.02" name="seg2" pos_marker="1"/>
-      <body joint="frozen" name="imu2_3Seg" pos="0.099999994 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.15 0.05 0.05">
+      <omc pos="0.0 0.0 -0.02" name="seg3" pos_marker="1"/>
+      <body joint="frozen" name="imu3_3Seg" pos="0.099999994 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.15 0.05 0.05">
         <geom mass="0.1" color="dustin_exp_orange" edge_color="black" type="box" dim="0.05 0.03 0.02"/>
-        <omc pos="0.1 0.0 0.015" name="seg2" pos_marker="1"/>
+        <omc pos="0.1 0.0 0.015" name="seg3" pos_marker="1"/>
       </body>
-      <body joint="rr_imp" name="seg3_3Seg" pos="0.20000002 0.0 0.0" pos_min="0.0 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3.0 3.0">
+      <body joint="rr_imp" name="seg4_3Seg" pos="0.20000002 0.0 0.0" pos_min="0.0 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3.0 3.0">
         <geom pos="0.1 0.0 0.0" mass="1.0" color="dustin_exp_white" edge_color="black" type="box" dim="0.2 0.05 0.05"/>
         <geom pos="0.1 0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
         <geom pos="0.15 -0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
-        <omc pos="0.0 0.0 -0.02" name="seg3" pos_marker="2"/>
-        <body joint="frozen" name="imu3_3Seg" pos="0.100000024 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.14999998 0.05 0.05">
+        <omc pos="0.0 0.0 -0.02" name="seg4" pos_marker="2"/>
+        <body joint="frozen" name="imu4_3Seg" pos="0.100000024 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.14999998 0.05 0.05">
           <geom mass="0.1" color="dustin_exp_orange" edge_color="black" type="box" dim="0.05 0.03 0.02"/>
-          <omc pos="0.1 0.0 0.015" name="seg3" pos_marker="2"/>
+          <omc pos="0.1 0.0 0.015" name="seg4" pos_marker="2"/>
         </body>
-        <body joint="rr_imp" name="seg4_3Seg" pos="0.19999999 0.0 0.0" pos_min="0.0 -0.05 -0.05" pos_max="0.35000002 0.05 0.05" damping="3.0 3.0">
+        <body joint="rr_imp" name="seg5_3Seg" pos="0.19999999 0.0 0.0" pos_min="0.0 -0.05 -0.05" pos_max="0.35000002 0.05 0.05" damping="3.0 3.0">
           <geom pos="0.1 0.0 0.0" mass="1.0" color="dustin_exp_white" edge_color="black" type="box" dim="0.2 0.05 0.05"/>
           <geom pos="0.03 -0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
           <geom pos="0.17 -0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
-          <omc pos="0.0 0.0 -0.02" name="seg4" pos_marker="4"/>
-          <body joint="frozen" name="imu4_3Seg" pos="0.100000024 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.15000004 0.05 0.05">
+          <omc pos="0.0 0.0 -0.02" name="seg5" pos_marker="4"/>
+          <body joint="frozen" name="imu5_3Seg" pos="0.100000024 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.15000004 0.05 0.05">
             <geom mass="0.1" color="dustin_exp_orange" edge_color="black" type="box" dim="0.05 0.03 0.02"/>
-            <omc pos="0.1 0.0 0.015" name="seg4" pos_marker="4"/>
+            <omc pos="0.1 0.0 0.015" name="seg5" pos_marker="4"/>
           </body>
         </body>
       </body>
     </body>
-    <body joint="free" name="seg5_4Seg" pos="0.2 0.0 0.0" pos_min="0.15 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="5.0 5.0 5.0 25.0 25.0 25.0">
+    <body joint="free" name="seg2_4Seg" pos="0.2 0.0 0.0" pos_min="0.15 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="5.0 5.0 5.0 25.0 25.0 25.0">
       <geom pos="0.1 0.0 0.0" mass="1.0" color="dustin_exp_white" edge_color="black" type="box" dim="0.2 0.05 0.05"/>
       <geom pos="0.03 -0.05 0.0" mass="0.1" color="dustin_exp_white" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
       <geom pos="0.17 -0.05 0.0" mass="0.1" color="dustin_exp_white" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
-      <omc pos="0.0 0.0 -0.02" name="seg5" pos_marker="2"/>
-      <body joint="frozen" name="imu5_4Seg" pos="0.10000001 0.0 0.035" pos_min="0.049999997 -0.05 -0.05" pos_max="0.15000002 0.05 0.05">
+      <omc pos="0.0 0.0 -0.02" name="seg2" pos_marker="2"/>
+      <body joint="frozen" name="imu2_4Seg" pos="0.10000001 0.0 0.035" pos_min="0.049999997 -0.05 -0.05" pos_max="0.15000002 0.05 0.05">
         <geom mass="0.1" color="dustin_exp_orange" edge_color="black" type="box" dim="0.05 0.03 0.02"/>
-        <omc pos="0.1 0.0 0.015" name="seg5" pos_marker="2"/>
+        <omc pos="0.1 0.0 0.015" name="seg2" pos_marker="2"/>
       </body>
-      <body joint="rr_imp" name="seg2_4Seg" pos="0.2 0.0 0.0" pos_min="0.0 -0.05 -0.05" pos_max="0.35000002 0.05 0.05" damping="3.0 3.0">
+      <body joint="rr_imp" name="seg3_4Seg" pos="0.2 0.0 0.0" pos_min="0.0 -0.05 -0.05" pos_max="0.35000002 0.05 0.05" damping="3.0 3.0">
         <geom pos="0.1 0.0 0.0" mass="1.0" color="dustin_exp_blue" edge_color="black" type="box" dim="0.2 0.05 0.05"/>
         <geom pos="0.05 0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
         <geom pos="0.15 -0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
-        <omc pos="0.0 0.0 -0.02" name="seg2" pos_marker="1"/>
-        <body joint="frozen" name="imu2_4Seg" pos="0.099999994 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.15 0.05 0.05">
+        <omc pos="0.0 0.0 -0.02" name="seg3" pos_marker="1"/>
+        <body joint="frozen" name="imu3_4Seg" pos="0.099999994 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.15 0.05 0.05">
           <geom mass="0.1" color="dustin_exp_orange" edge_color="black" type="box" dim="0.05 0.03 0.02"/>
-          <omc pos="0.1 0.0 0.015" name="seg2" pos_marker="1"/>
+          <omc pos="0.1 0.0 0.015" name="seg3" pos_marker="1"/>
         </body>
-        <body joint="rr_imp" name="seg3_4Seg" pos="0.20000002 0.0 0.0" pos_min="0.0 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3.0 3.0">
+        <body joint="rr_imp" name="seg4_4Seg" pos="0.20000002 0.0 0.0" pos_min="0.0 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3.0 3.0">
           <geom pos="0.1 0.0 0.0" mass="1.0" color="dustin_exp_white" edge_color="black" type="box" dim="0.2 0.05 0.05"/>
           <geom pos="0.1 0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
           <geom pos="0.15 -0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
-          <omc pos="0.0 0.0 -0.02" name="seg3" pos_marker="2"/>
-          <body joint="frozen" name="imu3_4Seg" pos="0.100000024 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.14999998 0.05 0.05">
+          <omc pos="0.0 0.0 -0.02" name="seg4" pos_marker="2"/>
+          <body joint="frozen" name="imu4_4Seg" pos="0.100000024 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.14999998 0.05 0.05">
             <geom mass="0.1" color="dustin_exp_orange" edge_color="black" type="box" dim="0.05 0.03 0.02"/>
-            <omc pos="0.1 0.0 0.015" name="seg3" pos_marker="2"/>
+            <omc pos="0.1 0.0 0.015" name="seg4" pos_marker="2"/>
           </body>
-          <body joint="rr_imp" name="seg4_4Seg" pos="0.19999999 0.0 0.0" pos_min="0.0 -0.05 -0.05" pos_max="0.35000002 0.05 0.05" damping="3.0 3.0">
+          <body joint="rr_imp" name="seg5_4Seg" pos="0.19999999 0.0 0.0" pos_min="0.0 -0.05 -0.05" pos_max="0.35000002 0.05 0.05" damping="3.0 3.0">
             <geom pos="0.1 0.0 0.0" mass="1.0" color="dustin_exp_white" edge_color="black" type="box" dim="0.2 0.05 0.05"/>
             <geom pos="0.03 -0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
             <geom pos="0.17 -0.05 0.0" mass="0.1" color="black" edge_color="black" type="box" dim="0.01 0.1 0.01"/>
-            <omc pos="0.0 0.0 -0.02" name="seg4" pos_marker="4"/>
-            <body joint="frozen" name="imu4_4Seg" pos="0.100000024 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.15000004 0.05 0.05">
+            <omc pos="0.0 0.0 -0.02" name="seg5" pos_marker="4"/>
+            <body joint="frozen" name="imu5_4Seg" pos="0.100000024 0.0 0.035" pos_min="0.050000012 -0.05 -0.05" pos_max="0.15000004 0.05 0.05">
               <geom mass="0.1" color="dustin_exp_orange" edge_color="black" type="box" dim="0.05 0.03 0.02"/>
-              <omc pos="0.1 0.0 0.015" name="seg4" pos_marker="4"/>
+              <omc pos="0.1 0.0 0.015" name="seg5" pos_marker="4"/>
             </body>
           </body>
         </body>
       </body>
     </body>
   </worldbody>
 </x_xy>
```

### Comparing `imt_ring-1.2.2/src/ring/io/examples/inv_pendulum.xml` & `imt_ring-1.3.0/src/ring/io/examples/inv_pendulum.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/io/examples/knee_flexible_imus.xml` & `imt_ring-1.3.0/src/ring/io/examples/knee_flexible_imus.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/io/examples/test_all_1.xml` & `imt_ring-1.3.0/src/ring/io/examples/test_all_1.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/io/examples/test_all_2.xml` & `imt_ring-1.3.0/src/ring/io/examples/test_all_2.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/io/examples/test_control.xml` & `imt_ring-1.3.0/src/ring/io/examples/test_control.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/io/examples/test_double_pendulum.xml` & `imt_ring-1.3.0/src/ring/io/examples/test_double_pendulum.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/io/examples/test_kinematics.xml` & `imt_ring-1.3.0/src/ring/io/examples/test_kinematics.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/io/examples/test_morph_system/four_seg_seg1.xml` & `imt_ring-1.3.0/src/ring/io/examples/test_morph_system/four_seg_seg1.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/io/examples/test_morph_system/four_seg_seg3.xml` & `imt_ring-1.3.0/src/ring/io/examples/test_morph_system/four_seg_seg3.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/io/examples/test_randomize_position.xml` & `imt_ring-1.3.0/src/ring/io/examples/test_randomize_position.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/io/examples/test_three_seg_seg2.xml` & `imt_ring-1.3.0/src/ring/io/examples/test_three_seg_seg2.xml`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/io/examples.py` & `imt_ring-1.3.0/src/ring/io/examples.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/io/xml/abstract.py` & `imt_ring-1.3.0/src/ring/io/xml/abstract.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/io/xml/from_xml.py` & `imt_ring-1.3.0/src/ring/io/xml/from_xml.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/io/xml/test_from_xml.py` & `imt_ring-1.3.0/src/ring/io/xml/test_from_xml.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/io/xml/test_to_xml.py` & `imt_ring-1.3.0/src/ring/io/xml/test_to_xml.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/io/xml/to_xml.py` & `imt_ring-1.3.0/src/ring/io/xml/to_xml.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/maths.py` & `imt_ring-1.3.0/src/ring/maths.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/ml/base.py` & `imt_ring-1.3.0/src/ring/ml/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,17 @@
             )
         )
 
     @abstractmethod
     def _apply_batched(self, X, params, state, y, lam):
         pass
 
-    @abstractmethod
     def init(self, bs, X, lam, seed: int):
-        pass
+        params = state = None
+        return params, state
 
     def apply(self, X, params=None, state=None, y=None, lam=None):
         "X.shape = (B, T, N, F) or (T, N, F)"
         assert X.ndim in [3, 4]
         if X.ndim == 4:
             return self._apply_batched(X, params, state, y, lam)
         else:
@@ -282,11 +282,11 @@
         else:
             T, N, F = X.shape
             X = X.reshape((T, 1, N * F))
             yhat, state = super().apply(X, params, state, y, (-1,))
             yhat = yhat.reshape((T, N, -1))
 
         if self._quat_normalize:
-            assert yhat.shape[-1] == 4
+            assert yhat.shape[-1] == 4, f"yhat.shape={yhat.shape}"
             yhat = ring.maths.safe_normalize(yhat)
 
         return yhat, state
```

### Comparing `imt_ring-1.2.2/src/ring/ml/callbacks.py` & `imt_ring-1.3.0/src/ring/ml/callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,18 @@
     ):
         if self.eval_every == -1:
             return
 
         if (i_episode % self.eval_every) == 0:
             point_estimates = self.eval_fn(params)
             self.last_metrices = {self.metric_identifier: point_estimates}
+
+        assert (
+            self.metric_identifier not in metrices
+        ), f"`{self.metric_identifier}` is already in `{metrices.keys()}`"
         metrices.update(self.last_metrices)
 
 
 class AverageMetricesTLCB(training_loop.TrainingLoopCallback):
     def __init__(self, metrices_names: list[list[str]], name: str):
         self.zoom_ins = metrices_names
         self.name = name
```

### Comparing `imt_ring-1.2.2/src/ring/ml/ml_utils.py` & `imt_ring-1.3.0/src/ring/ml/ml_utils.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/ml/optimizer.py` & `imt_ring-1.3.0/src/ring/ml/optimizer.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/ml/params/0x13e3518065c21cd8.pickle` & `imt_ring-1.3.0/src/ring/ml/params/0x13e3518065c21cd8.pickle`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/ml/ringnet.py` & `imt_ring-1.3.0/src/ring/ml/ringnet.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/ml/train.py` & `imt_ring-1.3.0/src/ring/ml/train.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/ml/training_loop.py` & `imt_ring-1.3.0/src/ring/ml/training_loop.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/rendering/base_render.py` & `imt_ring-1.3.0/src/ring/rendering/base_render.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,15 @@
 
     return geom.replace(color=new_color)
 
 
 def _xyz_to_three_capsules(xyz: base.XYZ) -> list[base.Geometry]:
     capsules = []
     length = xyz.size
-    radius = length / 6
+    radius = length / 7
     colors = ["red", "green", "blue"]
     rot_axis = [1, 0, 2]
 
     for i, (color, axis) in enumerate(zip(colors, rot_axis)):
         pos = maths.unit_vectors(i) * length / 2
         rot = maths.quat_rot_axis(maths.unit_vectors(axis), jnp.pi / 2)
         t = algebra.transform_mul(base.Transform(pos, rot), xyz.transform)
```

### Comparing `imt_ring-1.2.2/src/ring/rendering/mujoco_render.py` & `imt_ring-1.3.0/src/ring/rendering/mujoco_render.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/rendering/vispy_render.py` & `imt_ring-1.3.0/src/ring/rendering/vispy_render.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/rendering/vispy_visuals.py` & `imt_ring-1.3.0/src/ring/rendering/vispy_visuals.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/sim2real/sim2real.py` & `imt_ring-1.3.0/src/ring/sim2real/sim2real.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/spatial.py` & `imt_ring-1.3.0/src/ring/spatial.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/sys_composer/delete_sys.py` & `imt_ring-1.3.0/src/ring/sys_composer/delete_sys.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/sys_composer/inject_sys.py` & `imt_ring-1.3.0/src/ring/sys_composer/inject_sys.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/sys_composer/morph_sys.py` & `imt_ring-1.3.0/src/ring/sys_composer/morph_sys.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/utils/__init__.py` & `imt_ring-1.3.0/src/ring/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/utils/batchsize.py` & `imt_ring-1.3.0/src/ring/utils/batchsize.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/utils/colab.py` & `imt_ring-1.3.0/src/ring/utils/colab.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/utils/hdf5.py` & `imt_ring-1.3.0/src/ring/utils/hdf5.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/utils/normalizer.py` & `imt_ring-1.3.0/src/ring/utils/normalizer.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/utils/path.py` & `imt_ring-1.3.0/src/ring/utils/path.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/src/ring/utils/utils.py` & `imt_ring-1.3.0/src/ring/utils/utils.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/tests/test_algebra.py` & `imt_ring-1.3.0/tests/test_algebra.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/tests/test_base.py` & `imt_ring-1.3.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/tests/test_custom_joints.py` & `imt_ring-1.3.0/tests/test_custom_joints.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/tests/test_dynamics.py` & `imt_ring-1.3.0/tests/test_dynamics.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/tests/test_generator.py` & `imt_ring-1.3.0/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/tests/test_jcalc.py` & `imt_ring-1.3.0/tests/test_jcalc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from _compat import unbatch_gen
 import jax
 import jax.numpy as jnp
 import numpy as np
 import pytest
+
 import ring
 from ring.algorithms.jcalc import _find_interval
 
 
 @pytest.mark.parametrize("T,seed", [(10.0, 0), (20.0, 0), (10.0, 1), (20.0, 1)])
 def test_join_motionconfigs(T, seed):
     motion_config = ring.MotionConfig()
@@ -55,7 +56,11 @@
         ring.join_motionconfigs([motion_config, motion_config_disagree], [T])
 
 
 def test_find_interval():
     assert _find_interval(1.5, jnp.array([0.0, 1.0, 2.0])) == 2
     assert _find_interval(0.5, jnp.array([0.0])) == 1
     assert _find_interval(-0.5, jnp.array([0.0])) == 0
+
+
+def test_motion_config_register():
+    ring.MotionConfig.from_register("expSlow")
```

### Comparing `imt_ring-1.2.2/tests/test_jit.py` & `imt_ring-1.3.0/tests/test_jit.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/tests/test_kinematics.py` & `imt_ring-1.3.0/tests/test_kinematics.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/tests/test_maths.py` & `imt_ring-1.3.0/tests/test_maths.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/tests/test_ml_utils.py` & `imt_ring-1.3.0/tests/test_ml_utils.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/tests/test_motion_artifacts.py` & `imt_ring-1.3.0/tests/test_motion_artifacts.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/tests/test_pd_control.py` & `imt_ring-1.3.0/tests/test_pd_control.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/tests/test_random.py` & `imt_ring-1.3.0/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/tests/test_randomize.py` & `imt_ring-1.3.0/tests/test_randomize.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,29 +7,29 @@
     anchor_1Seg=None,
     anchor_2Seg=None,
     anchor_3Seg=None,
     anchor_4Seg=None,
 ):
     """
     4Seg:
-        Four anchors : ["seg5", "seg2", "seg3", "seg4"]
-        Two anchors  : ["seg5", "seg4"]
+        Four anchors : ["seg2", "seg3", "seg4", "seg5"]
+        Two anchors  : ["seg2", "seg5"]
     3Seg:
-        Three anchors: ["seg2", "seg3", "seg4"]
-        Two anchors  : ["seg2", "seg4"]
+        Three anchors: ["seg3", "seg4", "seg5"]
+        Two anchors  : ["seg3", "seg5"]
     2Seg:
-        Two anchors: ["seg2", "seg3"]
+        Two anchors: ["seg3", "seg4"]
     1Seg:
         Single anchor: Any of the five segments.
     """
     delete_4Seg = ["seg1"]
-    delete_3Seg = ["seg5"]
-    delete_2Seg = ["seg5", "seg4"]
+    delete_3Seg = ["seg2"]
+    delete_2Seg = ["seg2", "seg5"]
     delete_1Seg = list(
-        set(["seg1", "seg5", "seg2", "seg3", "seg4"]) - set([anchor_1Seg])
+        set(["seg1", "seg2", "seg3", "seg4", "seg5"]) - set([anchor_1Seg])
     )
 
     assert not (
         anchor_3Seg is None
         and anchor_4Seg is None
         and anchor_2Seg is None
         and anchor_1Seg is None
@@ -86,20 +86,20 @@
 
 def _new_load_standard_system():
     "Generates the system `standard_sys.xml` and `standard_sys_rr_imp.xml"
     sys_4Seg: ring.System = (
         _load_sys(
             1,
         )
-        .morph_system(new_anchor="seg5")
+        .morph_system(new_anchor="seg2")
         .delete_system("seg1")
     )
-    sys_3Seg = sys_4Seg.morph_system(new_anchor="seg2").delete_system("seg5")
-    sys_2Seg = sys_3Seg.delete_system("seg4")
-    sys_1Seg = sys_2Seg.delete_system("seg3")
+    sys_3Seg = sys_4Seg.morph_system(new_anchor="seg3").delete_system("seg2")
+    sys_2Seg = sys_3Seg.delete_system("seg5")
+    sys_1Seg = sys_2Seg.delete_system("seg4")
 
     def add_suffix(sys, suffix):
         return sys.change_model_name(suffix=suffix).add_prefix_suffix(suffix=suffix)
 
     sys = add_suffix(sys_1Seg, "_1Seg")
     for _sys, suffix in zip(
         [sys_2Seg, sys_3Seg, sys_4Seg], ["_2Seg", "_3Seg", "_4Seg"]
@@ -111,63 +111,63 @@
 def test_new_load_standard_system():
     "Test the new way of loading the 10 body standard system."
 
     sys = _new_load_standard_system()
     assert ring.utils.sys_compare(
         sys,
         _load_1Seg2Seg3Seg4Seg_system(
+            "seg3",
+            "seg3",
+            "seg3",
             "seg2",
-            "seg2",
-            "seg2",
-            "seg5",
         ),
     )
 
     assert ring.utils.sys_compare(sys, ring.io.load_example("exclude/standard_sys"))
 
 
 def SKIP_test_randomize_anchors_long():
-    anchors_2Seg = ["seg2", "seg3"]
-    anchors_3Seg = ["seg2", "seg4"]
-    anchors_4Seg = ["seg5", "seg2", "seg3", "seg4"]
+    anchors_2Seg = ["seg3", "seg4"]
+    anchors_3Seg = ["seg3", "seg5"]
+    anchors_4Seg = ["seg2", "seg3", "seg4", "seg5"]
 
     sys_data = []
     for a2S in anchors_2Seg:
         for a3S in anchors_3Seg:
             for a4S in anchors_4Seg:
-                sys_data.append(_load_1Seg2Seg3Seg4Seg_system("seg2", a2S, a3S, a4S))
+                sys_data.append(_load_1Seg2Seg3Seg4Seg_system("seg3", a2S, a3S, a4S))
     anchors = [
-        "seg2_2Seg",
         "seg3_2Seg",
-        "seg2_3Seg",
-        "seg4_3Seg",
-        "seg5_4Seg",
+        "seg4_2Seg",
+        "seg3_3Seg",
+        "seg5_3Seg",
         "seg2_4Seg",
         "seg3_4Seg",
         "seg4_4Seg",
+        "seg5_4Seg",
     ]
     sys_data_new = ring.algorithms.generator.randomize_anchors(
         ring.io.load_example("exclude/standard_sys"), anchors
     )
 
     for sys_old, sys_new in zip(sys_data, sys_data_new):
         assert ring.utils.sys_compare(sys_old, sys_new)
 
 
 def test_randomize_anchors():
-    anchors_2Seg = ["seg2", "seg3"]
-    anchors_3Seg = ["seg2", "seg4"]
+    anchors_2Seg = ["seg3", "seg4"]
+    anchors_3Seg = ["seg3", "seg5"]
 
     sys_data = []
     for a2S in anchors_2Seg:
         for a3S in anchors_3Seg:
             sys_data.append(_load_1Seg2Seg3Seg4Seg_system(None, a2S, a3S, None))
     anchors = [
-        "seg2_2Seg",
         "seg3_2Seg",
-        "seg2_3Seg",
-        "seg4_3Seg",
+        "seg4_2Seg",
+        "seg3_3Seg",
+        "seg5_3Seg",
     ]
     sys_data_new = ring.algorithms.generator.randomize_anchors(sys_data[0], anchors)
 
     for sys_old, sys_new in zip(sys_data, sys_data_new):
         assert ring.utils.sys_compare(sys_old, sys_new)
```

### Comparing `imt_ring-1.2.2/tests/test_rcmg.py` & `imt_ring-1.3.0/tests/test_rcmg.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/tests/test_render.py` & `imt_ring-1.3.0/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/tests/test_sensors.py` & `imt_ring-1.3.0/tests/test_sensors.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/tests/test_sim2real.py` & `imt_ring-1.3.0/tests/test_sim2real.py`

 * *Files identical despite different names*

### Comparing `imt_ring-1.2.2/tests/test_sys_composer.py` & `imt_ring-1.3.0/tests/test_sys_composer.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,17 +73,17 @@
         ["seg3", "seg2", "seg1", -1, "seg3"],
     )
 
     assert sys_compare(
         delete_subsystem(sys, ["seg1", "seg2"]), delete_subsystem(sys, ["seg2"])
     )
 
-    sys = _compat._load_sys(1).morph_system(new_anchor="seg3")
+    sys = _compat._load_sys(1).morph_system(new_anchor="seg4")
     assert sys_compare(
-        delete_subsystem(sys, ["seg5", "seg2"]), delete_subsystem(sys, ["seg2"])
+        delete_subsystem(sys, ["seg2", "seg3"]), delete_subsystem(sys, ["seg3"])
     )
 
 
 def test_tree_equal():
     sys = ring.io.load_example("test_three_seg_seg2")
     sys_mod_nofield = sys.replace(link_parents=[i + 1 for i in sys.link_parents])
     sys_mod_field = sys.replace(link_damping=sys.link_damping + 1.0)
@@ -204,21 +204,21 @@
 
 def test_morph_new_anchor():
     sys = _compat._load_sys(1)
     sys_compare(
         morph_system(
             sys,
             new_parents=[
-                "seg5",
+                "seg2",
                 "seg1",
+                "seg3",
                 "seg2",
-                "seg5",
                 -1,
-                "seg2",
-                "seg2",
                 "seg3",
                 "seg3",
                 "seg4",
+                "seg4",
+                "seg5",
             ],
         ),
-        morph_system(sys, new_anchor="seg2"),
+        morph_system(sys, new_anchor="seg3"),
     )
```

### Comparing `imt_ring-1.2.2/tests/test_train.py` & `imt_ring-1.3.0/tests/test_train.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,64 @@
+from pathlib import Path
+
 import numpy as np
 import optax
+import tree_utils
+
 import ring
 from ring import ml
 from ring import utils
-import tree_utils
 
 
-def test_ring():
+def _load_gen_lam():
     example = "test_three_seg_seg2"
     sys = ring.io.load_example(example)
     sys_noimu = sys.make_sys_noimu()[0]
     gen = ring.RCMG(
         sys,
         ring.MotionConfig(T=10.0),
         add_X_imus=1,
         add_y_relpose=1,
         add_y_rootincl=1,
         use_link_number_in_Xy=1,
     ).to_lazy_gen()
     gen = ring.algorithms.GeneratorTrafoExpandFlatten(gen)
+    lam = sys_noimu.link_parents
+    return gen, lam
+
+
+def test_rnno():
+    gen, lam = _load_gen_lam()
+
+    N = len(lam)
+    ml.train_fn(
+        gen,
+        5,
+        ml.RNNO(N * 4, return_quats=True, eval=False, hidden_state_dim=20),
+    )
+
+
+def test_ring():
+    gen, lam = _load_gen_lam()
 
     ml.train_fn(
         gen,
         5,
-        ml.RING(hidden_state_dim=20, message_dim=10, lam=sys_noimu.link_parents),
+        ml.RING(hidden_state_dim=20, message_dim=10, lam=lam),
     )
 
 
+def _remove_file_if_exists(path: str) -> None:
+    Path(path).expanduser().unlink(missing_ok=True)
+
+
 def test_checkpointing():
+    _remove_file_if_exists("~/params/test_checkpointing_nopause.pickle")
+    _remove_file_if_exists("~/params/test_checkpointing_pause.pickle")
+
     optimizer = optax.adam(0.1)
 
     ring.setup(unique_id="test_checkpointing_nopause")
     example = "test_three_seg_seg2"
     sys = ring.io.load_example(example)
     sys_noimu, _ = sys.make_sys_noimu()
     gen = ring.RCMG(
```

### Comparing `imt_ring-1.2.2/tests/test_utils.py` & `imt_ring-1.3.0/tests/test_utils.py`

 * *Files identical despite different names*

