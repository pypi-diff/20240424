# Comparing `tmp/imt-ring-1.2.1.tar.gz` & `tmp/imt_ring-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imt-ring-1.2.1.tar", last modified: Fri Mar 29 10:59:02 2024, max compression
+gzip compressed data, was "imt_ring-1.2.2.tar", last modified: Wed Apr 24 11:18:10 2024, max compression
```

## Comparing `imt-ring-1.2.1.tar` & `imt_ring-1.2.2.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:59:02.067829 imt-ring-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-03-29 10:59:02.067829 imt-ring-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-03-29 10:58:58.000000 imt-ring-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-03-29 10:58:58.000000 imt-ring-1.2.1/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-29 10:59:02.067829 imt-ring-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:59:02.035829 imt-ring-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:59:02.067829 imt-ring-1.2.1/src/imt_ring.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-03-29 10:59:02.000000 imt-ring-1.2.1/src/imt_ring.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-03-29 10:59:02.000000 imt-ring-1.2.1/src/imt_ring.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 10:59:02.000000 imt-ring-1.2.1/src/imt_ring.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-29 10:59:02.000000 imt-ring-1.2.1/src/imt_ring.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-29 10:59:02.000000 imt-ring-1.2.1/src/imt_ring.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:59:02.039829 imt-ring-1.2.1/src/ring/
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/algebra.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:59:02.039829 imt-ring-1.2.1/src/ring/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13340 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/algorithms/_random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:59:02.043829 imt-ring-1.2.1/src/ring/algorithms/custom_joints/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/algorithms/custom_joints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/algorithms/custom_joints/rr_imp_joint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/algorithms/custom_joints/rr_joint.py
--rw-r--r--   0 runner    (1001) docker     (127)    13139 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/algorithms/custom_joints/suntay.py
--rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/algorithms/dynamics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:59:02.043829 imt-ring-1.2.1/src/ring/algorithms/generator/
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/algorithms/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14952 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/algorithms/generator/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/algorithms/generator/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/algorithms/generator/motion_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/algorithms/generator/pd_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/algorithms/generator/randomize.py
--rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/algorithms/generator/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/algorithms/generator/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    25270 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/algorithms/jcalc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/algorithms/kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)    18005 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/algorithms/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)    33566 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:59:02.043829 imt-ring-1.2.1/src/ring/io/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:59:02.047829 imt-ring-1.2.1/src/ring/io/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/examples/branched.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:59:02.047829 imt-ring-1.2.1/src/ring/io/examples/exclude/
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/examples/exclude/knee_trans_dof.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/examples/exclude/standard_sys.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/examples/exclude/standard_sys_rr_imp.xml
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/examples/inv_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/examples/knee_flexible_imus.xml
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/examples/spherical_stiff.xml
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/examples/symmetric.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/examples/test_all_1.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/examples/test_all_2.xml
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/examples/test_ang0_pos0.xml
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/examples/test_control.xml
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/examples/test_double_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/examples/test_free.xml
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/examples/test_kinematics.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:59:02.047829 imt-ring-1.2.1/src/ring/io/examples/test_morph_system/
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/examples/test_morph_system/four_seg_seg1.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/examples/test_morph_system/four_seg_seg3.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/examples/test_randomize_position.xml
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/examples/test_sensors.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/examples/test_three_seg_seg2.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/test_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:59:02.047829 imt-ring-1.2.1/src/ring/io/xml/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/xml/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/xml/from_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/xml/test_from_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/xml/test_to_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/io/xml/to_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)    12193 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/maths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:59:02.047829 imt-ring-1.2.1/src/ring/ml/
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/ml/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13108 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/ml/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/ml/ml_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/ml/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:59:02.047829 imt-ring-1.2.1/src/ring/ml/params/
--rw-r--r--   0 runner    (1001) docker     (127)  9355838 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/ml/params/0x13e3518065c21cd8.pickle
--rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/ml/ringnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/ml/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/ml/training_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:59:02.063829 imt-ring-1.2.1/src/ring/rendering/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/rendering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/rendering/base_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/rendering/mujoco_render.py
--rw-r--r--   0 runner    (1001) docker     (127)    10260 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/rendering/vispy_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/rendering/vispy_visuals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:59:02.063829 imt-ring-1.2.1/src/ring/sim2real/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/sim2real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/sim2real/sim2real.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/spatial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:59:02.063829 imt-ring-1.2.1/src/ring/sys_composer/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/sys_composer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/sys_composer/delete_sys.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/sys_composer/inject_sys.py
--rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/sys_composer/morph_sys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:59:02.063829 imt-ring-1.2.1/src/ring/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/utils/batchsize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/utils/colab.py
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/utils/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/utils/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-03-29 10:58:58.000000 imt-ring-1.2.1/src/ring/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:59:02.067829 imt-ring-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-03-29 10:58:58.000000 imt-ring-1.2.1/tests/test_algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-03-29 10:58:58.000000 imt-ring-1.2.1/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-03-29 10:58:58.000000 imt-ring-1.2.1/tests/test_custom_joints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-03-29 10:58:58.000000 imt-ring-1.2.1/tests/test_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-03-29 10:58:58.000000 imt-ring-1.2.1/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-03-29 10:58:58.000000 imt-ring-1.2.1/tests/test_jcalc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-03-29 10:58:58.000000 imt-ring-1.2.1/tests/test_jit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-03-29 10:58:58.000000 imt-ring-1.2.1/tests/test_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-03-29 10:58:58.000000 imt-ring-1.2.1/tests/test_maths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-03-29 10:58:58.000000 imt-ring-1.2.1/tests/test_ml_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-03-29 10:58:58.000000 imt-ring-1.2.1/tests/test_motion_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-03-29 10:58:58.000000 imt-ring-1.2.1/tests/test_pd_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-03-29 10:58:58.000000 imt-ring-1.2.1/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-03-29 10:58:58.000000 imt-ring-1.2.1/tests/test_randomize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-03-29 10:58:58.000000 imt-ring-1.2.1/tests/test_rcmg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-03-29 10:58:58.000000 imt-ring-1.2.1/tests/test_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-03-29 10:58:58.000000 imt-ring-1.2.1/tests/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-03-29 10:58:58.000000 imt-ring-1.2.1/tests/test_sim2real.py
--rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-03-29 10:58:58.000000 imt-ring-1.2.1/tests/test_sys_composer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-03-29 10:58:58.000000 imt-ring-1.2.1/tests/test_train.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-29 10:58:58.000000 imt-ring-1.2.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.932594 imt_ring-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-24 11:18:10.932594 imt_ring-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-24 11:18:06.000000 imt_ring-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-24 11:18:06.000000 imt_ring-1.2.2/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-24 11:18:10.932594 imt_ring-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.896594 imt_ring-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.928594 imt_ring-1.2.2/src/imt_ring.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-24 11:18:10.000000 imt_ring-1.2.2/src/imt_ring.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-24 11:18:10.000000 imt_ring-1.2.2/src/imt_ring.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:18:10.000000 imt_ring-1.2.2/src/imt_ring.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-24 11:18:10.000000 imt_ring-1.2.2/src/imt_ring.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 11:18:10.000000 imt_ring-1.2.2/src/imt_ring.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.900594 imt_ring-1.2.2/src/ring/
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algebra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.900594 imt_ring-1.2.2/src/ring/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13340 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/_random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.904594 imt_ring-1.2.2/src/ring/algorithms/custom_joints/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/custom_joints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/custom_joints/rr_imp_joint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/custom_joints/rr_joint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13680 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/custom_joints/suntay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/dynamics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.904594 imt_ring-1.2.2/src/ring/algorithms/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14952 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/generator/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/generator/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/generator/motion_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/generator/pd_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/generator/randomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12782 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/generator/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/generator/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25270 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/jcalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18005 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/algorithms/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33566 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.904594 imt_ring-1.2.2/src/ring/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.908594 imt_ring-1.2.2/src/ring/io/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/branched.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.908594 imt_ring-1.2.2/src/ring/io/examples/exclude/
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/exclude/knee_trans_dof.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/exclude/standard_sys.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/exclude/standard_sys_rr_imp.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/inv_pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/knee_flexible_imus.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/spherical_stiff.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/symmetric.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/test_all_1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/test_all_2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/test_ang0_pos0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/test_control.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/test_double_pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/test_free.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/test_kinematics.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.908594 imt_ring-1.2.2/src/ring/io/examples/test_morph_system/
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/test_morph_system/four_seg_seg1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/test_morph_system/four_seg_seg3.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/test_randomize_position.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/test_sensors.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples/test_three_seg_seg2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.908594 imt_ring-1.2.2/src/ring/io/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/xml/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/xml/from_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/xml/test_from_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/xml/test_to_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/io/xml/to_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12193 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/maths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.912594 imt_ring-1.2.2/src/ring/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/ml/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13109 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/ml/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/ml/ml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/ml/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.912594 imt_ring-1.2.2/src/ring/ml/params/
+-rw-r--r--   0 runner    (1001) docker     (127)  9355838 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/ml/params/0x13e3518065c21cd8.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/ml/ringnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/ml/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/ml/training_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.924594 imt_ring-1.2.2/src/ring/rendering/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/rendering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/rendering/base_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/rendering/mujoco_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10260 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/rendering/vispy_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/rendering/vispy_visuals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.924594 imt_ring-1.2.2/src/ring/sim2real/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/sim2real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/sim2real/sim2real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/spatial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.924594 imt_ring-1.2.2/src/ring/sys_composer/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/sys_composer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/sys_composer/delete_sys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/sys_composer/inject_sys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/sys_composer/morph_sys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.924594 imt_ring-1.2.2/src/ring/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/utils/batchsize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/utils/colab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/utils/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/utils/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-24 11:18:06.000000 imt_ring-1.2.2/src/ring/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:18:10.928594 imt_ring-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_custom_joints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_jcalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_jit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_maths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_ml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_motion_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_pd_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_randomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_rcmg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_sim2real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_sys_composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-24 11:18:06.000000 imt_ring-1.2.2/tests/test_utils.py
```

### Comparing `imt-ring-1.2.1/PKG-INFO` & `imt_ring-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imt-ring
-Version: 1.2.1
+Version: 1.2.2
 Summary: RING: Recurrent Inertial Graph-based Estimator
 Author-email: Simon Bachhuber <simon.bachhuber@fau.de>
 Project-URL: Homepage, https://github.com/SimiPixel/ring
 Project-URL: Issues, https://github.com/SimiPixel/ring/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `imt-ring-1.2.1/pyproject.toml` & `imt_ring-1.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "imt-ring"
-version = "1.2.1"
+version = "1.2.2"
 authors = [
   { name="Simon Bachhuber", email="simon.bachhuber@fau.de" },
 ]
 description = "RING: Recurrent Inertial Graph-based Estimator"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `imt-ring-1.2.1/readme.md` & `imt_ring-1.2.2/readme.md`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/imt_ring.egg-info/PKG-INFO` & `imt_ring-1.2.2/src/imt_ring.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imt-ring
-Version: 1.2.1
+Version: 1.2.2
 Summary: RING: Recurrent Inertial Graph-based Estimator
 Author-email: Simon Bachhuber <simon.bachhuber@fau.de>
 Project-URL: Homepage, https://github.com/SimiPixel/ring
 Project-URL: Issues, https://github.com/SimiPixel/ring/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `imt-ring-1.2.1/src/imt_ring.egg-info/SOURCES.txt` & `imt_ring-1.2.2/src/imt_ring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/__init__.py` & `imt_ring-1.2.2/src/ring/__init__.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/algebra.py` & `imt_ring-1.2.2/src/ring/algebra.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/algorithms/__init__.py` & `imt_ring-1.2.2/src/ring/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/algorithms/_random.py` & `imt_ring-1.2.2/src/ring/algorithms/_random.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/algorithms/custom_joints/rr_imp_joint.py` & `imt_ring-1.2.2/src/ring/algorithms/custom_joints/rr_imp_joint.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/algorithms/custom_joints/rr_joint.py` & `imt_ring-1.2.2/src/ring/algorithms/custom_joints/rr_joint.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/algorithms/custom_joints/suntay.py` & `imt_ring-1.2.2/src/ring/algorithms/custom_joints/suntay.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import haiku as hk
 import jax
 import jax.numpy as jnp
 from tree_utils import PyTree
 
 import ring
 from ring import maths
+from ring.algorithms import jcalc
 from ring.algorithms._random import random_angle_over_time
 
 Params = PyTree
 
 
 class DrawnFnPair(NamedTuple):
     # (key) -> tree
@@ -254,47 +255,62 @@
             mconfig.randomized_interpolation_angle,
             mconfig.range_of_motion_hinge,
             mconfig.range_of_motion_hinge_method,
             mconfig.cdf_bins_min,
             mconfig.cdf_bins_max,
             mconfig.interpolation_method,
         )
+        return _apply_rom(qs_flexion)
+
+    def _apply_rom(qs_flexion):
         return restrict(
             qs_flexion,
             sconfig.flexion_rot_min,
             sconfig.flexion_rot_max,
             -jnp.pi,
             jnp.pi,
             method=sconfig.flexion_rot_restrict_method,
         )
 
+    def coordinate_vector_to_q_suntay(q_flexion):
+        q_flexion = ring.maths.wrap_to_pi(q_flexion)
+        return _apply_rom(q_flexion)
+
     joint_model = ring.JointModel(
         transform=_transform_suntay,
+        motion=[jcalc.mrx],
         rcmg_draw_fn=_draw_flexion_angle,
+        p_control_term=jcalc._p_control_term_rxyz,
+        qd_from_q=jcalc._qd_from_q_cartesian,
+        coordinate_vector_to_q=coordinate_vector_to_q_suntay,
+        inv_kin=None,
         init_joint_params=_init_joint_params_suntay,
         utilities=dict(
             Q_S_H_alpha_beta_gamma=_utils_Q_S_H_alpha_beta_gamma,
             find_suntay_joint=_utils_find_suntay_joint,
+            sconfig=sconfig,
         ),
     )
-    ring.register_new_joint_type(name, joint_model, 1, qd_width=0, overwrite=True)
+    ring.register_new_joint_type(name, joint_model, 1, overwrite=True)
 
 
 def MLP_DrawnFnPair(
     center: bool = False, flexion_center: Optional[float] = None
 ) -> DrawnFnPairFactory:
 
     def factory(xs, mn, mx):
         nonlocal flexion_center
 
         flexion_mn = jnp.min(xs)
         flexion_mx = jnp.max(xs)
 
         if flexion_center is None:
             flexion_center = (flexion_mn + flexion_mx) / 2
+        else:
+            flexion_center = jnp.array(flexion_center)
 
         @hk.without_apply_rng
         @hk.transform
         def mlp(x):
             # normalize the x input; [0, 1]
             x = _shift(x, flexion_mn, flexion_mx)
             # center the x input; [-0.5, 0.5]
```

### Comparing `imt-ring-1.2.1/src/ring/algorithms/dynamics.py` & `imt_ring-1.2.2/src/ring/algorithms/dynamics.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/algorithms/generator/__init__.py` & `imt_ring-1.2.2/src/ring/algorithms/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/algorithms/generator/base.py` & `imt_ring-1.2.2/src/ring/algorithms/generator/base.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/algorithms/generator/batch.py` & `imt_ring-1.2.2/src/ring/algorithms/generator/batch.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/algorithms/generator/motion_artifacts.py` & `imt_ring-1.2.2/src/ring/algorithms/generator/motion_artifacts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,81 @@
 import warnings
 
 import jax
 import jax.numpy as jnp
+import tree_utils
+
 from ring import base
 from ring import io
-import tree_utils
 
 
 def imu_reference_link_name(imu_link_name: str) -> str:
     return "_" + imu_link_name
 
 
 def unactuated_subsystem(sys) -> list[str]:
     return [imu_reference_link_name(name) for name in sys.findall_imus()]
 
 
-def _subsystem_factory(imu_name: str, pos_min_max: float) -> base.System:
+def _subsystem_factory(
+    imu_name: str,
+    pos_min_max: float,
+    translational_stif: float,
+    translational_damp: float,
+) -> base.System:
     assert pos_min_max >= 0
     pos = f'pos_min="-{pos_min_max} -{pos_min_max} -{pos_min_max}" pos_max="{pos_min_max} {pos_min_max} {pos_min_max}"'  # noqa: E501
-    stiff = 'spring_stiff="50 50 50"'
-    damping = 'damping="5 5 5"'
+    stiff = (
+        f'spring_stiff="{translational_stif} {translational_stif} {translational_stif}"'
+    )
+    translational_damp = translational_stif * translational_damp
+    damping = (
+        f'damping="{translational_damp} {translational_damp} {translational_damp}"'
+    )
     return io.load_sys_from_str(
         f"""
         <x_xy>
         <worldbody>
         <body name="{imu_name}" joint="p3d" {pos if pos_min_max != 0.0 else ""} {stiff} {damping}/>
         </worldbody>
         </x_xy>
         """  # noqa: E501
     )
 
 
 def inject_subsystems(
     sys: base.System,
     pos_min_max: float = 0.0,
+    rotational_stif: float = 0.3,
+    rotational_damp: float = 0.1,
+    translational_stif: float = 50.0,
+    translational_damp: float = 0.1,
     **kwargs,
 ) -> base.System:
     imu_idx_to_name_map = {sys.name_to_idx(imu): imu for imu in sys.findall_imus()}
 
-    default_spher_stif = jnp.ones((3,)) * 0.3
-    default_spher_damp = default_spher_stif * 0.1
+    default_spher_stif = jnp.ones((3,)) * rotational_stif
+    default_spher_damp = default_spher_stif * rotational_damp
     for imu in sys.findall_imus():
         sys = sys.unfreeze(imu, "spherical")
         # set default stiffness and damping of spherical joint
         # this won't override anything because the frozen joint can not have any values
         qd_slice = sys.idx_map("d")[imu]
         stiffne = sys.link_spring_stiffness.at[qd_slice].set(default_spher_stif)
         damping = sys.link_damping.at[qd_slice].set(default_spher_damp)
         sys = sys.replace(link_spring_stiffness=stiffne, link_damping=damping)
 
         _imu = imu_reference_link_name(imu)
         sys = sys.change_link_name(imu, _imu)
-        sys = sys.inject_system(_subsystem_factory(imu, pos_min_max), _imu)
+        sys = sys.inject_system(
+            _subsystem_factory(
+                imu, pos_min_max, translational_stif, translational_damp
+            ),
+            _imu,
+        )
 
     # attach geoms to newly injected link
     new_geoms = []
 
     for geom in sys.geoms:
         if geom.link_idx in imu_idx_to_name_map:
             imu_name = imu_idx_to_name_map[geom.link_idx]
```

### Comparing `imt-ring-1.2.1/src/ring/algorithms/generator/pd_control.py` & `imt_ring-1.2.2/src/ring/algorithms/generator/pd_control.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/algorithms/generator/randomize.py` & `imt_ring-1.2.2/src/ring/algorithms/generator/randomize.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/algorithms/generator/transforms.py` & `imt_ring-1.2.2/src/ring/algorithms/generator/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,14 +273,15 @@
     # primary, residual
     "rr_imp": jnp.array([P_rot, P_rot]),
     "cor": jnp.array(3 * [P_rot] + 6 * [P_pos]),
     "spherical": jnp.array(3 * [P_rot]),
     "p3d": jnp.array(3 * [P_pos]),
     "saddle": jnp.array([P_rot, P_rot]),
     "frozen": jnp.array([]),
+    "suntay": jnp.array([P_rot]),
 }
 
 
 class GeneratorTrafoDynamicalSimulation(types.GeneratorTrafo):
     def __init__(
         self,
         custom_P_gains: dict[str, jax.Array] = dict(),
```

### Comparing `imt-ring-1.2.1/src/ring/algorithms/generator/types.py` & `imt_ring-1.2.2/src/ring/algorithms/generator/types.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/algorithms/jcalc.py` & `imt_ring-1.2.2/src/ring/algorithms/jcalc.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/algorithms/kinematics.py` & `imt_ring-1.2.2/src/ring/algorithms/kinematics.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/algorithms/sensors.py` & `imt_ring-1.2.2/src/ring/algorithms/sensors.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/base.py` & `imt_ring-1.2.2/src/ring/base.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/io/examples/branched.xml` & `imt_ring-1.2.2/src/ring/io/examples/branched.xml`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/io/examples/exclude/knee_trans_dof.xml` & `imt_ring-1.2.2/src/ring/io/examples/exclude/knee_trans_dof.xml`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/io/examples/exclude/standard_sys.xml` & `imt_ring-1.2.2/src/ring/io/examples/exclude/standard_sys.xml`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/io/examples/exclude/standard_sys_rr_imp.xml` & `imt_ring-1.2.2/src/ring/io/examples/exclude/standard_sys_rr_imp.xml`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/io/examples/inv_pendulum.xml` & `imt_ring-1.2.2/src/ring/io/examples/inv_pendulum.xml`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/io/examples/knee_flexible_imus.xml` & `imt_ring-1.2.2/src/ring/io/examples/knee_flexible_imus.xml`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/io/examples/test_all_1.xml` & `imt_ring-1.2.2/src/ring/io/examples/test_all_1.xml`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/io/examples/test_all_2.xml` & `imt_ring-1.2.2/src/ring/io/examples/test_all_2.xml`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/io/examples/test_control.xml` & `imt_ring-1.2.2/src/ring/io/examples/test_control.xml`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/io/examples/test_double_pendulum.xml` & `imt_ring-1.2.2/src/ring/io/examples/test_double_pendulum.xml`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/io/examples/test_kinematics.xml` & `imt_ring-1.2.2/src/ring/io/examples/test_kinematics.xml`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/io/examples/test_morph_system/four_seg_seg1.xml` & `imt_ring-1.2.2/src/ring/io/examples/test_morph_system/four_seg_seg1.xml`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/io/examples/test_morph_system/four_seg_seg3.xml` & `imt_ring-1.2.2/src/ring/io/examples/test_morph_system/four_seg_seg3.xml`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/io/examples/test_randomize_position.xml` & `imt_ring-1.2.2/src/ring/io/examples/test_randomize_position.xml`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/io/examples/test_three_seg_seg2.xml` & `imt_ring-1.2.2/src/ring/io/examples/test_three_seg_seg2.xml`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/io/examples.py` & `imt_ring-1.2.2/src/ring/io/examples.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/io/xml/abstract.py` & `imt_ring-1.2.2/src/ring/io/xml/abstract.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/io/xml/from_xml.py` & `imt_ring-1.2.2/src/ring/io/xml/from_xml.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/io/xml/test_from_xml.py` & `imt_ring-1.2.2/src/ring/io/xml/test_from_xml.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/io/xml/test_to_xml.py` & `imt_ring-1.2.2/src/ring/io/xml/test_to_xml.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/io/xml/to_xml.py` & `imt_ring-1.2.2/src/ring/io/xml/to_xml.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/maths.py` & `imt_ring-1.2.2/src/ring/maths.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/ml/__init__.py` & `imt_ring-1.2.2/src/ring/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/ml/base.py` & `imt_ring-1.2.2/src/ring/ml/base.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/ml/callbacks.py` & `imt_ring-1.2.2/src/ring/ml/callbacks.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
             else:
                 value = "{:.2f}".format(ele.value).replace(".", ",")
                 filename = parse_path(
                     self.path_to_file + f"_episode={ele.episode}_value={value}",
                     extension="pickle",
                 )
 
-            pickle_save(ele.params, filename, overwrite=True)
+            pickle_save(ele.params, filename, overwrite=False)
             if self.upload:
                 success = False
                 for logger in self._loggers:
                     try:
                         logger.log_params(filename)
                         success = True
                     except NotImplementedError:
```

### Comparing `imt-ring-1.2.1/src/ring/ml/ml_utils.py` & `imt_ring-1.2.2/src/ring/ml/ml_utils.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/ml/optimizer.py` & `imt_ring-1.2.2/src/ring/ml/optimizer.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/ml/params/0x13e3518065c21cd8.pickle` & `imt_ring-1.2.2/src/ring/ml/params/0x13e3518065c21cd8.pickle`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/ml/ringnet.py` & `imt_ring-1.2.2/src/ring/ml/ringnet.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/ml/train.py` & `imt_ring-1.2.2/src/ring/ml/train.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/ml/training_loop.py` & `imt_ring-1.2.2/src/ring/ml/training_loop.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/rendering/base_render.py` & `imt_ring-1.2.2/src/ring/rendering/base_render.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/rendering/mujoco_render.py` & `imt_ring-1.2.2/src/ring/rendering/mujoco_render.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/rendering/vispy_render.py` & `imt_ring-1.2.2/src/ring/rendering/vispy_render.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/rendering/vispy_visuals.py` & `imt_ring-1.2.2/src/ring/rendering/vispy_visuals.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/sim2real/sim2real.py` & `imt_ring-1.2.2/src/ring/sim2real/sim2real.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/spatial.py` & `imt_ring-1.2.2/src/ring/spatial.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/sys_composer/delete_sys.py` & `imt_ring-1.2.2/src/ring/sys_composer/delete_sys.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/sys_composer/inject_sys.py` & `imt_ring-1.2.2/src/ring/sys_composer/inject_sys.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/sys_composer/morph_sys.py` & `imt_ring-1.2.2/src/ring/sys_composer/morph_sys.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/utils/__init__.py` & `imt_ring-1.2.2/src/ring/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/utils/batchsize.py` & `imt_ring-1.2.2/src/ring/utils/batchsize.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/utils/colab.py` & `imt_ring-1.2.2/src/ring/utils/colab.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/utils/hdf5.py` & `imt_ring-1.2.2/src/ring/utils/hdf5.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/utils/normalizer.py` & `imt_ring-1.2.2/src/ring/utils/normalizer.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/utils/path.py` & `imt_ring-1.2.2/src/ring/utils/path.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/src/ring/utils/utils.py` & `imt_ring-1.2.2/src/ring/utils/utils.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/tests/test_algebra.py` & `imt_ring-1.2.2/tests/test_algebra.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/tests/test_base.py` & `imt_ring-1.2.2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/tests/test_custom_joints.py` & `imt_ring-1.2.2/tests/test_custom_joints.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/tests/test_dynamics.py` & `imt_ring-1.2.2/tests/test_dynamics.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/tests/test_generator.py` & `imt_ring-1.2.2/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/tests/test_jcalc.py` & `imt_ring-1.2.2/tests/test_jcalc.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/tests/test_jit.py` & `imt_ring-1.2.2/tests/test_jit.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/tests/test_kinematics.py` & `imt_ring-1.2.2/tests/test_kinematics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import jax
 import jax.numpy as jnp
+import jaxopt
 import numpy as np
+import tree_utils as tu
+
 import ring
 from ring import base
 from ring import maths
 from ring.algorithms import jcalc
 from ring.algorithms import kinematics
 from ring.sim2real.sim2real import _checks_time_series_of_xs
-import tree_utils as tu
 
 
 def test_forward_kinematics_transforms():
     sys = ring.io.load_example("test_kinematics")
     q = [
         jnp.array([1, 0, 0, 0, 1, 1, 1.0]),
         jnp.pi / 2,
@@ -76,17 +78,17 @@
 
             q0 = jax.random.normal(c2, (sys.q_size(),))
             _, value, _ = kinematics.inverse_kinematics_endeffector(
                 sys,
                 "endeffector",
                 endeffector_x,
                 q0=q0,
-                # jaxopt_solver=jaxopt.GradientDescent,
-                # maxiter=5000,
-                # maxls=5,
+                jaxopt_solver=jaxopt.GradientDescent,
+                maxiter=5000,
+                maxls=3,
             )
             return value
 
         for trial in range(20):
             print(sys.model_name, trial)
             key, consume = jax.random.split(key)
             assert solve(consume) < 1e-3
```

### Comparing `imt-ring-1.2.1/tests/test_maths.py` & `imt_ring-1.2.2/tests/test_maths.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/tests/test_ml_utils.py` & `imt_ring-1.2.2/tests/test_ml_utils.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/tests/test_motion_artifacts.py` & `imt_ring-1.2.2/tests/test_motion_artifacts.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/tests/test_pd_control.py` & `imt_ring-1.2.2/tests/test_pd_control.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/tests/test_random.py` & `imt_ring-1.2.2/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/tests/test_randomize.py` & `imt_ring-1.2.2/tests/test_randomize.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/tests/test_rcmg.py` & `imt_ring-1.2.2/tests/test_rcmg.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/tests/test_render.py` & `imt_ring-1.2.2/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/tests/test_sensors.py` & `imt_ring-1.2.2/tests/test_sensors.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/tests/test_sim2real.py` & `imt_ring-1.2.2/tests/test_sim2real.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/tests/test_sys_composer.py` & `imt_ring-1.2.2/tests/test_sys_composer.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/tests/test_train.py` & `imt_ring-1.2.2/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `imt-ring-1.2.1/tests/test_utils.py` & `imt_ring-1.2.2/tests/test_utils.py`

 * *Files identical despite different names*

