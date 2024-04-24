# Comparing `tmp/robot_descriptions-1.8.1.tar.gz` & `tmp/robot_descriptions-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robot_descriptions-1.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "robot_descriptions-1.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `robot_descriptions-1.8.1.tar` & `robot_descriptions-1.9.0.tar`

### file list

```diff
@@ -1,127 +1,136 @@
--rw-r--r--   0        0        0      488 2024-01-04 10:27:09.712963 robot_descriptions-1.8.1/.github/workflows/changelog.yml
--rw-r--r--   0        0        0     2477 2024-01-04 10:27:09.712963 robot_descriptions-1.8.1/.github/workflows/test.yml
--rw-r--r--   0        0        0       42 2023-08-10 08:23:16.568791 robot_descriptions-1.8.1/.gitignore
--rw-r--r--   0        0        0     7344 2024-01-29 15:00:49.626541 robot_descriptions-1.8.1/CHANGELOG.md
--rw-r--r--   0        0        0     2037 2023-12-08 10:41:14.213830 robot_descriptions-1.8.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-08-10 08:23:16.568791 robot_descriptions-1.8.1/LICENSE
--rw-r--r--   0        0        0    16125 2024-01-29 14:51:48.920463 robot_descriptions-1.8.1/README.md
--rw-r--r--   0        0        0     2397 2024-01-08 10:28:42.493391 robot_descriptions-1.8.1/examples/display_urdf_frames.py
--rw-r--r--   0        0        0      790 2024-01-08 10:28:42.493391 robot_descriptions-1.8.1/examples/load_in_idyntree.py
--rw-r--r--   0        0        0      772 2024-01-08 10:28:42.493391 robot_descriptions-1.8.1/examples/load_in_mujoco.py
--rw-r--r--   0        0        0      767 2024-01-08 10:28:42.493391 robot_descriptions-1.8.1/examples/load_in_pinocchio.py
--rw-r--r--   0        0        0      862 2024-01-08 10:28:42.493391 robot_descriptions-1.8.1/examples/load_in_pybullet.py
--rw-r--r--   0        0        0      772 2024-01-08 10:28:42.493391 robot_descriptions-1.8.1/examples/load_in_robomeshcat.py
--rw-r--r--   0        0        0      772 2024-01-08 10:28:42.493391 robot_descriptions-1.8.1/examples/load_in_yourdfpy.py
--rw-r--r--   0        0        0     1134 2024-01-08 10:28:42.493391 robot_descriptions-1.8.1/examples/show_in_meshcat.py
--rw-r--r--   0        0        0     1208 2024-01-08 10:28:42.493391 robot_descriptions-1.8.1/examples/show_in_mujoco.py
--rw-r--r--   0        0        0      997 2024-01-08 10:28:42.493391 robot_descriptions-1.8.1/examples/show_in_pybullet.py
--rw-r--r--   0        0        0     1157 2024-01-08 10:28:42.493391 robot_descriptions-1.8.1/examples/show_in_robomeshcat.py
--rw-r--r--   0        0        0     1071 2024-01-08 10:28:42.493391 robot_descriptions-1.8.1/examples/show_in_yourdfpy.py
--rw-r--r--   0        0        0     1861 2024-01-29 14:51:48.920463 robot_descriptions-1.8.1/pyproject.toml
--rw-r--r--   0        0        0      206 2024-01-29 15:00:49.626541 robot_descriptions-1.8.1/robot_descriptions/__init__.py
--rw-r--r--   0        0        0     3877 2024-01-08 10:28:42.493391 robot_descriptions-1.8.1/robot_descriptions/_cache.py
--rw-r--r--   0        0        0     5096 2024-01-08 10:28:42.493391 robot_descriptions-1.8.1/robot_descriptions/_command_line.py
--rw-r--r--   0        0        0     5066 2024-01-29 14:51:48.920463 robot_descriptions-1.8.1/robot_descriptions/_descriptions.py
--rw-r--r--   0        0        0      166 2024-01-08 10:28:42.493391 robot_descriptions-1.8.1/robot_descriptions/_empty_description.py
--rw-r--r--   0        0        0      606 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/_package_dirs.py
--rw-r--r--   0        0        0     9869 2024-01-29 14:51:48.920463 robot_descriptions-1.8.1/robot_descriptions/_repositories.py
--rw-r--r--   0        0        0      516 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/a1_description.py
--rw-r--r--   0        0        0      570 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/a1_mj_description.py
--rw-r--r--   0        0        0      585 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/aliengo_description.py
--rw-r--r--   0        0        0      817 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/allegro_hand_description.py
--rw-r--r--   0        0        0      514 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/anymal_b_description.py
--rw-r--r--   0        0        0      523 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/anymal_b_mj_description.py
--rw-r--r--   0        0        0      514 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/anymal_c_description.py
--rw-r--r--   0        0        0      523 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/anymal_c_mj_description.py
--rw-r--r--   0        0        0      663 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/atlas_drc_description.py
--rw-r--r--   0        0        0      873 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/atlas_v4_description.py
--rw-r--r--   0        0        0      517 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/b1_description.py
--rw-r--r--   0        0        0      508 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/barrett_hand_description.py
--rw-r--r--   0        0        0      520 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/baxter_description.py
--rw-r--r--   0        0        0      531 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/bolt_description.py
--rw-r--r--   0        0        0      504 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/cassie_description.py
--rw-r--r--   0        0        0      515 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/cassie_mj_description.py
--rw-r--r--   0        0        0      540 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/cf2_description.py
--rw-r--r--   0        0        0      796 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/double_pendulum_description.py
--rw-r--r--   0        0        0      503 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/draco3_description.py
--rw-r--r--   0        0        0      489 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/edo_description.py
--rw-r--r--   0        0        0      534 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/ergocub_description.py
--rw-r--r--   0        0        0      526 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/eve_r3_description.py
--rw-r--r--   0        0        0      518 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/fanuc_m710ic_description.py
--rw-r--r--   0        0        0      552 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/fetch_description.py
--rw-r--r--   0        0        0      557 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/finger_edu_description.py
--rw-r--r--   0        0        0      547 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/gen2_description.py
--rw-r--r--   0        0        0      566 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/gen3_description.py
--rw-r--r--   0        0        0      524 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/gen3_mj_description.py
--rw-r--r--   0        0        0      499 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/ginger_description.py
--rw-r--r--   0        0        0      519 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/go1_description.py
--rw-r--r--   0        0        0      574 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/go1_mj_description.py
--rw-r--r--   0        0        0      531 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/go2_description.py
--rw-r--r--   0        0        0      506 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/go2_mj_description.py
--rw-r--r--   0        0        0      517 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/h1_description.py
--rw-r--r--   0        0        0      523 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/h1_mj_description.py
--rw-r--r--   0        0        0      539 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/hyq_description.py
--rw-r--r--   0        0        0      527 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/icub_description.py
--rw-r--r--   0        0        0      919 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/iiwa_description.py
--rw-r--r--   0        0        0      505 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/jaxon_description.py
--rw-r--r--   0        0        0      500 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/jvrc_description.py
--rw-r--r--   0        0        0      506 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/jvrc_mj_description.py
--rw-r--r--   0        0        0      585 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/laikago_description.py
--rw-r--r--   0        0        0      175 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/loaders/__init__.py
--rw-r--r--   0        0        0     2079 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/loaders/idyntree.py
--rw-r--r--   0        0        0     1006 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/loaders/mujoco.py
--rw-r--r--   0        0        0     1665 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/loaders/pinocchio.py
--rw-r--r--   0        0        0     1649 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/loaders/pybullet.py
--rw-r--r--   0        0        0     1104 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/loaders/robomeshcat.py
--rw-r--r--   0        0        0     1224 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/loaders/yourdfpy.py
--rw-r--r--   0        0        0      514 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/mini_cheetah_description.py
--rw-r--r--   0        0        0      509 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/minitaur_description.py
--rw-r--r--   0        0        0      528 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/nextage_description.py
--rw-r--r--   0        0        0      532 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/panda_description.py
--rw-r--r--   0        0        0      517 2024-01-08 10:28:42.497391 robot_descriptions-1.8.1/robot_descriptions/panda_mj_description.py
--rw-r--r--   0        0        0      503 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/pepper_description.py
--rw-r--r--   0        0        0      524 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/poppy_ergo_jr_description.py
--rw-r--r--   0        0        0      518 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/poppy_torso_description.py
--rw-r--r--   0        0        0      509 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/pr2_description.py
--rw-r--r--   0        0        0     2240 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/r2_description.py
--rw-r--r--   0        0        0      495 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/reachy_description.py
--rw-r--r--   0        0        0      497 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/rhea_description.py
--rw-r--r--   0        0        0      544 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/robotiq_2f85_description.py
--rw-r--r--   0        0        0      518 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/robotiq_2f85_mj_description.py
--rw-r--r--   0        0        0      545 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/romeo_description.py
--rw-r--r--   0        0        0      682 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/shadow_hand_mj_description.py
--rw-r--r--   0        0        0      491 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/sigmaban_description.py
--rw-r--r--   0        0        0      631 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/simple_humanoid_description.py
--rw-r--r--   0        0        0      507 2024-01-29 14:51:48.920463 robot_descriptions-1.8.1/robot_descriptions/skydio_x2_description.py
--rw-r--r--   0        0        0      504 2024-01-29 14:51:48.920463 robot_descriptions-1.8.1/robot_descriptions/skydio_x2_mj_description.py
--rw-r--r--   0        0        0      533 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/solo_description.py
--rw-r--r--   0        0        0      527 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/spryped_description.py
--rw-r--r--   0        0        0      500 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/stretch_description.py
--rw-r--r--   0        0        0      778 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/talos_description.py
--rw-r--r--   0        0        0      730 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/tiago_description.py
--rw-r--r--   0        0        0      570 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/trifinger_edu_description.py
--rw-r--r--   0        0        0      500 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/upkie_description.py
--rw-r--r--   0        0        0      667 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/ur10_description.py
--rw-r--r--   0        0        0      521 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/ur10e_mj_description.py
--rw-r--r--   0        0        0      743 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/ur3_description.py
--rw-r--r--   0        0        0      743 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/ur5_description.py
--rw-r--r--   0        0        0      518 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/ur5e_mj_description.py
--rw-r--r--   0        0        0      842 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/valkyrie_description.py
--rw-r--r--   0        0        0      512 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/yumi_description.py
--rw-r--r--   0        0        0      517 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/z1_description.py
--rw-r--r--   0        0        0      503 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/robot_descriptions/z1_mj_description.py
--rw-r--r--   0        0        0      494 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/tests/__init__.py
--rw-r--r--   0        0        0       59 2023-08-10 08:23:16.572791 robot_descriptions-1.8.1/tests/loaders/__init__.py
--rw-r--r--   0        0        0     1023 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/tests/loaders/test_idyntree.py
--rw-r--r--   0        0        0      971 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/tests/loaders/test_mujoco.py
--rw-r--r--   0        0        0     1029 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/tests/loaders/test_pinocchio.py
--rw-r--r--   0        0        0     1468 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/tests/loaders/test_pybullet.py
--rw-r--r--   0        0        0     1039 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/tests/loaders/test_robomeshcat.py
--rw-r--r--   0        0        0      981 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/tests/loaders/test_yourdfpy.py
--rw-r--r--   0        0        0     2293 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/tests/test_clone_to_cache.py
--rw-r--r--   0        0        0     3076 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/tests/test_clone_to_directory.py
--rw-r--r--   0        0        0     1865 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/tests/test_descriptions.py
--rw-r--r--   0        0        0     2075 2024-01-29 14:45:37.144537 robot_descriptions-1.8.1/tests/test_loaders.py
--rw-r--r--   0        0        0      478 2024-01-08 10:28:42.501391 robot_descriptions-1.8.1/tests/test_progress_bar.py
--rw-r--r--   0        0        0     2240 2024-01-29 14:51:48.920463 robot_descriptions-1.8.1/tox.ini
--rw-r--r--   0        0        0    17591 1970-01-01 00:00:00.000000 robot_descriptions-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0      488 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0     2477 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0       42 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/.gitignore
+-rw-r--r--   0        0        0     8378 2024-03-27 17:47:50.009033 robot_descriptions-1.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0      786 2024-03-27 17:47:50.009033 robot_descriptions-1.9.0/CITATION.cff
+-rw-r--r--   0        0        0     2037 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/LICENSE
+-rw-r--r--   0        0        0    17720 2024-03-27 17:47:50.009033 robot_descriptions-1.9.0/README.md
+-rw-r--r--   0        0        0     2397 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/examples/display_urdf_frames.py
+-rw-r--r--   0        0        0      790 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/examples/load_in_idyntree.py
+-rw-r--r--   0        0        0      772 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/examples/load_in_mujoco.py
+-rw-r--r--   0        0        0      767 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/examples/load_in_pinocchio.py
+-rw-r--r--   0        0        0      862 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/examples/load_in_pybullet.py
+-rw-r--r--   0        0        0      772 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/examples/load_in_robomeshcat.py
+-rw-r--r--   0        0        0      772 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/examples/load_in_yourdfpy.py
+-rw-r--r--   0        0        0     1134 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/examples/show_in_meshcat.py
+-rw-r--r--   0        0        0     1208 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/examples/show_in_mujoco.py
+-rw-r--r--   0        0        0      997 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/examples/show_in_pybullet.py
+-rw-r--r--   0        0        0     1157 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/examples/show_in_robomeshcat.py
+-rw-r--r--   0        0        0     1071 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/examples/show_in_yourdfpy.py
+-rw-r--r--   0        0        0     1861 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0      206 2024-03-27 17:47:50.009033 robot_descriptions-1.9.0/robot_descriptions/__init__.py
+-rw-r--r--   0        0        0     4429 2024-03-27 17:28:20.246727 robot_descriptions-1.9.0/robot_descriptions/_cache.py
+-rw-r--r--   0        0        0     5096 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/robot_descriptions/_command_line.py
+-rw-r--r--   0        0        0     5503 2024-03-27 16:02:27.678696 robot_descriptions-1.9.0/robot_descriptions/_descriptions.py
+-rw-r--r--   0        0        0      166 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/robot_descriptions/_empty_description.py
+-rw-r--r--   0        0        0      606 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/robot_descriptions/_package_dirs.py
+-rw-r--r--   0        0        0     9862 2024-03-27 17:28:20.246727 robot_descriptions-1.9.0/robot_descriptions/_repositories.py
+-rw-r--r--   0        0        0      516 2024-03-27 16:55:30.608804 robot_descriptions-1.9.0/robot_descriptions/a1_description.py
+-rw-r--r--   0        0        0      570 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/a1_mj_description.py
+-rw-r--r--   0        0        0      585 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/aliengo_description.py
+-rw-r--r--   0        0        0      817 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/allegro_hand_description.py
+-rw-r--r--   0        0        0      588 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/allegro_hand_mj_description.py
+-rw-r--r--   0        0        0      473 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/aloha_mj_description.py
+-rw-r--r--   0        0        0      514 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/anymal_b_description.py
+-rw-r--r--   0        0        0      523 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/anymal_b_mj_description.py
+-rw-r--r--   0        0        0      514 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/anymal_c_description.py
+-rw-r--r--   0        0        0      523 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/anymal_c_mj_description.py
+-rw-r--r--   0        0        0      663 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/atlas_drc_description.py
+-rw-r--r--   0        0        0      873 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/atlas_v4_description.py
+-rw-r--r--   0        0        0      517 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/b1_description.py
+-rw-r--r--   0        0        0      508 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/barrett_hand_description.py
+-rw-r--r--   0        0        0      520 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/baxter_description.py
+-rw-r--r--   0        0        0      531 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/bolt_description.py
+-rw-r--r--   0        0        0      504 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/cassie_description.py
+-rw-r--r--   0        0        0      515 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/cassie_mj_description.py
+-rw-r--r--   0        0        0      540 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/cf2_description.py
+-rw-r--r--   0        0        0      492 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/cf2_mj_description.py
+-rw-r--r--   0        0        0      796 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/double_pendulum_description.py
+-rw-r--r--   0        0        0      503 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/draco3_description.py
+-rw-r--r--   0        0        0      489 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/edo_description.py
+-rw-r--r--   0        0        0      534 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/ergocub_description.py
+-rw-r--r--   0        0        0      526 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/eve_r3_description.py
+-rw-r--r--   0        0        0      518 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/fanuc_m710ic_description.py
+-rw-r--r--   0        0        0      552 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/fetch_description.py
+-rw-r--r--   0        0        0      557 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/finger_edu_description.py
+-rw-r--r--   0        0        0      547 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/gen2_description.py
+-rw-r--r--   0        0        0      566 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/gen3_description.py
+-rw-r--r--   0        0        0      524 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/gen3_mj_description.py
+-rw-r--r--   0        0        0      499 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/ginger_description.py
+-rw-r--r--   0        0        0      519 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/go1_description.py
+-rw-r--r--   0        0        0      514 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/go1_mj_description.py
+-rw-r--r--   0        0        0      531 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/go2_description.py
+-rw-r--r--   0        0        0      514 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/go2_mj_description.py
+-rw-r--r--   0        0        0      517 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/h1_description.py
+-rw-r--r--   0        0        0      511 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/h1_mj_description.py
+-rw-r--r--   0        0        0      539 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/hyq_description.py
+-rw-r--r--   0        0        0      527 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/icub_description.py
+-rw-r--r--   0        0        0      919 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/iiwa_description.py
+-rw-r--r--   0        0        0      485 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/iiwa_mj_description.py
+-rw-r--r--   0        0        0      505 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/jaxon_description.py
+-rw-r--r--   0        0        0      500 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/jvrc_description.py
+-rw-r--r--   0        0        0      506 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/jvrc_mj_description.py
+-rw-r--r--   0        0        0      585 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/laikago_description.py
+-rw-r--r--   0        0        0      175 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/robot_descriptions/loaders/__init__.py
+-rw-r--r--   0        0        0     2190 2024-03-27 17:28:20.246727 robot_descriptions-1.9.0/robot_descriptions/loaders/idyntree.py
+-rw-r--r--   0        0        0     1117 2024-03-27 17:28:20.246727 robot_descriptions-1.9.0/robot_descriptions/loaders/mujoco.py
+-rw-r--r--   0        0        0     1776 2024-03-27 17:28:20.246727 robot_descriptions-1.9.0/robot_descriptions/loaders/pinocchio.py
+-rw-r--r--   0        0        0     1760 2024-03-27 17:28:20.246727 robot_descriptions-1.9.0/robot_descriptions/loaders/pybullet.py
+-rw-r--r--   0        0        0     1215 2024-03-27 17:28:20.246727 robot_descriptions-1.9.0/robot_descriptions/loaders/robomeshcat.py
+-rw-r--r--   0        0        0     1335 2024-03-27 17:28:20.246727 robot_descriptions-1.9.0/robot_descriptions/loaders/yourdfpy.py
+-rw-r--r--   0        0        0      514 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/mini_cheetah_description.py
+-rw-r--r--   0        0        0      509 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/minitaur_description.py
+-rw-r--r--   0        0        0      528 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/nextage_description.py
+-rw-r--r--   0        0        0      476 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/op3_mj_description.py
+-rw-r--r--   0        0        0      532 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/panda_description.py
+-rw-r--r--   0        0        0      517 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/panda_mj_description.py
+-rw-r--r--   0        0        0      503 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/pepper_description.py
+-rw-r--r--   0        0        0      524 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/poppy_ergo_jr_description.py
+-rw-r--r--   0        0        0      518 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/poppy_torso_description.py
+-rw-r--r--   0        0        0      509 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/pr2_description.py
+-rw-r--r--   0        0        0     2240 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/r2_description.py
+-rw-r--r--   0        0        0      495 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/reachy_description.py
+-rw-r--r--   0        0        0      497 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/rhea_description.py
+-rw-r--r--   0        0        0      544 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/robotiq_2f85_description.py
+-rw-r--r--   0        0        0      518 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/robotiq_2f85_mj_description.py
+-rw-r--r--   0        0        0      545 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/romeo_description.py
+-rw-r--r--   0        0        0      508 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/sawyer_mj_description.py
+-rw-r--r--   0        0        0      682 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/shadow_hand_mj_description.py
+-rw-r--r--   0        0        0      491 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/sigmaban_description.py
+-rw-r--r--   0        0        0      631 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/simple_humanoid_description.py
+-rw-r--r--   0        0        0      507 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/skydio_x2_description.py
+-rw-r--r--   0        0        0      504 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/skydio_x2_mj_description.py
+-rw-r--r--   0        0        0      533 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/solo_description.py
+-rw-r--r--   0        0        0      527 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/spryped_description.py
+-rw-r--r--   0        0        0      500 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/stretch_description.py
+-rw-r--r--   0        0        0      486 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/stretch_mj_description.py
+-rw-r--r--   0        0        0      778 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/talos_description.py
+-rw-r--r--   0        0        0      730 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/tiago_description.py
+-rw-r--r--   0        0        0      570 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/trifinger_edu_description.py
+-rw-r--r--   0        0        0      500 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/upkie_description.py
+-rw-r--r--   0        0        0      667 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/ur10_description.py
+-rw-r--r--   0        0        0      521 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/ur10e_mj_description.py
+-rw-r--r--   0        0        0      743 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/ur3_description.py
+-rw-r--r--   0        0        0      743 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/ur5_description.py
+-rw-r--r--   0        0        0      518 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/ur5e_mj_description.py
+-rw-r--r--   0        0        0      842 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/valkyrie_description.py
+-rw-r--r--   0        0        0      524 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/viper_mj_description.py
+-rw-r--r--   0        0        0      512 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/yumi_description.py
+-rw-r--r--   0        0        0      517 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/z1_description.py
+-rw-r--r--   0        0        0      503 2024-03-27 16:51:30.133507 robot_descriptions-1.9.0/robot_descriptions/z1_mj_description.py
+-rw-r--r--   0        0        0      494 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/tests/__init__.py
+-rw-r--r--   0        0        0       59 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/tests/loaders/__init__.py
+-rw-r--r--   0        0        0     1023 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/tests/loaders/test_idyntree.py
+-rw-r--r--   0        0        0      971 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/tests/loaders/test_mujoco.py
+-rw-r--r--   0        0        0     1029 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/tests/loaders/test_pinocchio.py
+-rw-r--r--   0        0        0     1468 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/tests/loaders/test_pybullet.py
+-rw-r--r--   0        0        0     1039 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/tests/loaders/test_robomeshcat.py
+-rw-r--r--   0        0        0      981 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/tests/loaders/test_yourdfpy.py
+-rw-r--r--   0        0        0     2542 2024-03-27 17:28:20.246727 robot_descriptions-1.9.0/tests/test_clone_to_cache.py
+-rw-r--r--   0        0        0     3076 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/tests/test_clone_to_directory.py
+-rw-r--r--   0        0        0     1865 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/tests/test_descriptions.py
+-rw-r--r--   0        0        0     2636 2024-03-27 17:28:20.246727 robot_descriptions-1.9.0/tests/test_loaders.py
+-rw-r--r--   0        0        0      478 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/tests/test_progress_bar.py
+-rw-r--r--   0        0        0     2240 2024-03-06 17:11:28.551395 robot_descriptions-1.9.0/tox.ini
+-rw-r--r--   0        0        0    19186 1970-01-01 00:00:00.000000 robot_descriptions-1.9.0/PKG-INFO
```

### Comparing `robot_descriptions-1.8.1/.github/workflows/test.yml` & `robot_descriptions-1.9.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/CHANGELOG.md` & `robot_descriptions-1.9.0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,40 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 ## [Unreleased]
 
+## [1.9.0] - 2024-03-27
+
+### Added
+
+- Citation file and BibTeX section in the readme
+- Description: Allegro Hand V3 (MJCF) (thanks to @kevinzakka)
+- Description: ALOHA 2 (MJCF) (thanks to @kevinzakka)
+- Description: Bitcraze Crazyflie 2.0 (MJCF) (thanks to @kevinzakka)
+- Description: KUKA iiwa 14 (MJCF) (thanks to @kevinzakka)
+- Description: Robotics OP3 (MJCF) (thanks to @kevinzakka)
+- Description: Saywer (MJCF) (thanks to @kevinzakka)
+- Description: Stretch 2 (MJCF) (thanks to @kevinzakka)
+- Description: ViperX 300 6DOF (MJCF) (thanks to @kevinzakka)
+
+### Changed
+
+- Go1: Switch repository to MuJoCo Menagerie
+- Go2: Switch repository to MuJoCo Menagerie
+- H1: Switch repository to MuJoCo Menagerie
+- JVRC-1: Update repository to maintained one at jrl-umi3218
+- Upkie: Update repository to v1.5.0
+
+### Fixed
+
+- Bug when cloning a non-pinned description after a commit-pinned one
+- Package name resolution when pinning a description to a specific commit
+
 ## [1.8.1] - 2024-01-29
 
 ### Changed
 
 - Update example-robot-data to version 4.0.9 (thanks to @htadashi)
 
 ## [1.8.0] - 2024-01-24
@@ -300,15 +327,16 @@
 ### Added
 
 - Caching of git repositories
 - Command line to show or animate robot descriptions
 - Contributing instructions
 - This changelog
 
-[unreleased]: https://github.com/qpsolvers/qpsolvers/compare/v1.8.1...HEAD
+[unreleased]: https://github.com/qpsolvers/qpsolvers/compare/v1.9.0...HEAD
+[1.9.0]: https://github.com/qpsolvers/qpsolvers/compare/v1.8.1...v1.9.0
 [1.8.1]: https://github.com/qpsolvers/qpsolvers/compare/v1.8.0...v1.8.1
 [1.8.0]: https://github.com/qpsolvers/qpsolvers/compare/v1.7.0...v1.8.0
 [1.7.0]: https://github.com/qpsolvers/qpsolvers/compare/v1.6.0...v1.7.0
 [1.6.0]: https://github.com/qpsolvers/qpsolvers/compare/v1.5.0...v1.6.0
 [1.5.0]: https://github.com/qpsolvers/qpsolvers/compare/v1.4.1...v1.5.0
 [1.4.1]: https://github.com/qpsolvers/qpsolvers/compare/v1.4.0...v1.4.1
 [1.4.0]: https://github.com/qpsolvers/qpsolvers/compare/v1.3.1...v1.4.0
```

### Comparing `robot_descriptions-1.8.1/CONTRIBUTING.md` & `robot_descriptions-1.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/LICENSE` & `robot_descriptions-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/README.md` & `robot_descriptions-1.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,21 +8,25 @@
 
 Import open source robot descriptions as Python modules.
 
 Importing a description for the first time automatically downloads and caches files for future imports. Most [Awesome Robot Descriptions](https://github.com/robot-descriptions/awesome-robot-descriptions) are available. All of them load successfully in respectively MuJoCo (MJCF) or Pinocchio, iDynTree, PyBullet and yourdfpy (URDF).
 
 ## Installation
 
-### Install from pip
+### PyPI
+
+[![PyPI version](https://img.shields.io/pypi/v/robot_descriptions)](https://pypi.org/project/robot_descriptions/)
 
 ```console
 pip install robot_descriptions
 ```
 
-### Install from conda
+### Conda
+
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/robot_descriptions.svg)](https://anaconda.org/conda-forge/robot_descriptions)
 
 ```console
 conda install -c conda-forge robot_descriptions
 ```
 
 ## Usage
 
@@ -107,44 +111,47 @@
 robot_descriptions show solo_description
 ```
 
 ## Descriptions
 
 Available robot descriptions ([gallery](https://github.com/robot-descriptions/awesome-robot-descriptions#gallery)) are listed in the following categories:
 
-* [Arms](#arms)
-* [Bipeds](#bipeds)
-* [Dual arms](#dual-arms)
-* [Drones](#drones)
-* [Educational](#educational)
-* [End effectors](#end-effectors)
-* [Mobile manipulators](#mobile-manipulators)
-* [Humanoids](#humanoids)
-* [Quadrupeds](#quadrupeds)
+- [Arms](#arms)
+- [Bipeds](#bipeds)
+- [Dual arms](#dual-arms)
+- [Drones](#drones)
+- [Educational](#educational)
+- [End effectors](#end-effectors)
+- [Humanoids](#humanoids)
+- [Mobile manipulators](#mobile-manipulators)
+- [Quadrupeds](#quadrupeds)
 
 The DOF column denotes the number of actuated degrees of freedom.
 
 ### Arms
 
 | Name                          | Robot                 | Maker                    | DOF | Format     |
 |-------------------------------|-----------------------|--------------------------|-----|------------|
 | `edo_description`             | e.DO                  | Comau                    | 6   | URDF       |
 | `fanuc_m710ic_description`    | M-710iC               | Fanuc                    | 6   | URDF       |
 | `gen2_description`            | Gen2 (Jaco)           | Kinova                   | 6   | URDF       |
 | `gen3_description`            | Gen3 (Jaco)           | Kinova                   | 6   | URDF       |
 | `gen3_mj_description`         | Gen3 (Jaco)           | Kinova                   | 7   | MJCF       |
 | `iiwa_description`            | iiwa                  | KUKA                     | 7   | URDF       |
+| `iiwa_mj_description`         | iiwa14                | KUKA                     | 7   | MJCF       |
 | `panda_description`           | Panda                 | Franka Emika             | 8   | URDF       |
 | `panda_mj_description`        | Panda                 | Franka Emika             | 8   | MJCF       |
 | `poppy_ergo_jr_description`   | Poppy Ergo Jr         | Poppy Project            | 6   | URDF       |
+| `sawyer_mj_description`       | Sawyer                | Rethink Robotics         | 7   | MJCF       |
 | `ur10_description`            | UR10                  | Universal Robots         | 6   | URDF       |
 | `ur10e_mj_description`        | UR10e                 | Universal Robots         | 6   | MJCF       |
 | `ur3_description`             | UR3                   | Universal Robots         | 6   | URDF       |
 | `ur5_description`             | UR5                   | Universal Robots         | 6   | URDF       |
 | `ur5e_mj_description`         | UR5e                  | Universal Robots         | 6   | MJCF       |
+| `viper_mj_description`        | Viper                 | Trossen Robotics         | 7   | MJCF       |
 | `z1_description`              | Z1                    | UNITREE Robotics         | 6   | URDF       |
 
 ### Bipeds
 
 | Name                          | Robot                 | Maker                    | DOF | Format     |
 |-------------------------------|-----------------------|--------------------------|-----|------------|
 | `bolt_description`            | Bolt                  | ODRI                     | 6   | URDF       |
@@ -154,24 +161,26 @@
 | `spryped_description`         | Spryped               | Benjamin Bokser          | 8   | URDF       |
 | `upkie_description`           | Upkie                 | Tast's Robots            | 6   | URDF       |
 
 ### Dual arms
 
 | Name                          | Robot                 | Maker                    | DOF | Format     |
 |-------------------------------|-----------------------|--------------------------|-----|------------|
+| `aloha_mj_description`        | Aloha 2               | Trossen Robotics         | 14  | MJCF       |
 | `baxter_description`          | Baxter                | Rethink Robotics         | 15  | URDF       |
 | `nextage_description`         | NEXTAGE               | Kawada Robotics          | 15  | URDF       |
 | `poppy_torso_description`     | Poppy Torso           | Poppy Project            | 13  | URDF       |
 | `yumi_description`            | YuMi                  | ABB                      | 16  | URDF       |
 
 ### Drones
 
 | Name                          | Robot                 | Maker                    | DOF | Format     |
 |-------------------------------|-----------------------|--------------------------|-----|------------|
 | `cf2_description`             | Crazyflie 2.0         | Bitcraze                 | 0   | URDF       |
+| `cf2_mj_description`          | Crazyflie 2.0         | Bitcraze                 | 6   | MJCF       |
 | `skydio_x2_description`       | Skydio X2             | Skydio                   | 6   | URDF       |
 | `skydio_x2_mj_description`    | Skydio X2             | Skydio                   | 6   | MJCF       |
 
 ### Educational
 
 | Name                          | Robot                 | DOF | Format     |
 |-------------------------------|-----------------------|-----|------------|
@@ -181,14 +190,15 @@
 | `trifinger_edu_description`   | TriFingerEdu          | 9   | URDF       |
 
 ### End effectors
 
 | Name                          | Robot                 | Maker                    | DOF | Format     |
 |-------------------------------|-----------------------|--------------------------|-----|------------|
 | `allegro_hand_description`    | Allegro Hand          | Wonik Robotics           | 16  | URDF       |
+| `allegro_hand_mj_description` | Allegro Hand          | Wonik Robotics           | 16  | MJCF       |
 | `barrett_hand_description`    | BarrettHand           | Barrett Technology       | 8   | URDF       |
 | `robotiq_2f85_description`    | Robotiq 2F-85         | Robotiq                  | 1   | URDF       |
 | `robotiq_2f85_mj_description` | Robotiq 2F-85         | Robotiq                  | 1   | MJCF       |
 | `shadow_hand_mj_description`  | Shadow Hand           | The Shadow Robot Company | 24  | MJCF       |
 
 ### Humanoids
 
@@ -200,14 +210,15 @@
 | `ergocub_description`         | ergoCub               | IIT                      | 57  | URDF       |
 | `h1_description`              | H1                    | UNITREE Robotics         | 25  | URDF       |
 | `h1_mj_description`           | H1                    | UNITREE Robotics         | 25  | MJCF       |
 | `icub_description`            | iCub                  | IIT                      | 32  | URDF       |
 | `jaxon_description`           | JAXON                 | JSK                      | 38  | URDF       |
 | `jvrc_description`            | JVRC-1                | AIST                     | 34  | URDF       |
 | `jvrc_mj_description`         | JVRC-1                | AIST                     | 34  | MJCF       |
+| `op3_mj_description`          | OP3                   | ROBOTIS                  | 20  | MJCF       |
 | `r2_description`              | Robonaut 2            | NASA JSC Robotics        | 56  | URDF       |
 | `romeo_description`           | Romeo                 | Aldebaran Robotics       | 37  | URDF       |
 | `sigmaban_description`        | SigmaBan              | Rhoban                   | 20  | URDF       |
 | `talos_description`           | TALOS                 | PAL Robotics             | 32  | URDF       |
 | `valkyrie_description`        | Valkyrie              | NASA JSC Robotics        | 59  | URDF       |
 
 ### Mobile manipulators
@@ -217,14 +228,15 @@
 | `eve_r3_description`          | Eve R3                | Halodi                   | 23  | URDF       |
 | `fetch_description`           | Fetch                 | Fetch Robotics           | 14  | URDF       |
 | `ginger_description`          | Ginger                | Paaila Technology        | 49  | URDF       |
 | `pepper_description`          | Pepper                | SoftBank Robotics        | 17  | URDF       |
 | `pr2_description`             | PR2                   | Willow Garage            | 32  | URDF       |
 | `reachy_description`          | Reachy                | Pollen Robotics          | 21  | URDF       |
 | `stretch_description`         | Stretch RE1           | Hello Robot              | 14  | URDF       |
+| `sretch_mj_description`       | Stretch 2             | Hello Robot              | 14  | MJCF       |
 | `tiago_description`           | TIAGo                 | PAL Robotics             | 48  | URDF       |
 
 ### Quadrupeds
 
 | Name                          | Robot                 | Maker                    | DOF | Format     |
 |-------------------------------|-----------------------|--------------------------|-----|------------|
 | `a1_mj_description`           | A1                    | UNITREE Robotics         | 12  | MJCF       |
@@ -249,13 +261,29 @@
 
 New robot descriptions are welcome! Check out the [guidelines](https://github.com/robot-descriptions/robot_descriptions.py/tree/main/CONTRIBUTING.md) then open a PR.
 
 ## Thanks
 
 Thanks to the maintainers of all the git repositories that made these robot descriptions available.
 
+## Citation
+
+If you use `robot_descriptions.py` in your scientific works, please cite it *e.g.* as follows:
+
+```bibtex
+@software{robot_descriptions_py2024,
+  author = {Caron, Stéphane and Romualdi, Giulio and Kozlov, Lev and Ordonez, Daniel and Tadashi Kussaba, Hugo and Bang, Seung Hyeon and Zakka, Kevin},
+  license = {Apache-2.0},
+  month = mar,
+  title = {{robot_descriptions.py: Robot descriptions in Python}},
+  url = {https://github.com/robot-descriptions/robot_descriptions.py},
+  version = {1.9.0},
+  year = {2024}
+}
+```
+
 ## See also
 
 Robot descriptions in other languages:
 
 | ![C++](https://img.shields.io/badge/C%2B%2B-00599C?logo=c%2B%2B&logoColor=white) | [robot\_descriptions.cpp](https://github.com/mayataka/robot_descriptions.cpp) |
 |--|--|
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `robot_descriptions-1.8.1/examples/display_urdf_frames.py` & `robot_descriptions-1.9.0/examples/display_urdf_frames.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/examples/load_in_idyntree.py` & `robot_descriptions-1.9.0/examples/load_in_idyntree.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/examples/load_in_mujoco.py` & `robot_descriptions-1.9.0/examples/load_in_mujoco.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/examples/load_in_pinocchio.py` & `robot_descriptions-1.9.0/examples/load_in_pinocchio.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/examples/load_in_pybullet.py` & `robot_descriptions-1.9.0/examples/load_in_pybullet.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/examples/load_in_robomeshcat.py` & `robot_descriptions-1.9.0/examples/load_in_robomeshcat.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/examples/load_in_yourdfpy.py` & `robot_descriptions-1.9.0/examples/load_in_yourdfpy.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/examples/show_in_meshcat.py` & `robot_descriptions-1.9.0/examples/show_in_meshcat.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/examples/show_in_mujoco.py` & `robot_descriptions-1.9.0/examples/show_in_mujoco.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/examples/show_in_pybullet.py` & `robot_descriptions-1.9.0/examples/show_in_pybullet.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/examples/show_in_robomeshcat.py` & `robot_descriptions-1.9.0/examples/show_in_robomeshcat.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/examples/show_in_yourdfpy.py` & `robot_descriptions-1.9.0/examples/show_in_yourdfpy.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/pyproject.toml` & `robot_descriptions-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/_cache.py` & `robot_descriptions-1.9.0/robot_descriptions/_cache.py`

 * *Files 11% similar despite different names*

```diff
@@ -126,15 +126,29 @@
             "ROBOT_DESCRIPTIONS_CACHE",
             "~/.cache/robot_descriptions",
         )
     )
 
     cache_path = repository.cache_path
     if commit is not None:
-        cache_path += f"-{commit}"
+        # Requirement: the last directory in the cache path is named after the
+        # cache path (more precisely the package name) so that package:// URIs
+        # work in frameworks that resolve them via directories
+        cache_path = f"{cache_path}-{commit}/{cache_path}"
     target_dir = os.path.join(cache_dir, cache_path)
     clone = clone_to_directory(
         repository.url,
         target_dir,
         commit=repository.commit if commit is None else commit,
     )
     return str(clone.working_dir)
+
+
+def clear_cache() -> None:
+    """Clears the local cache where robot descriptions are stored."""
+    cache_dir = os.path.expanduser(
+        os.environ.get(
+            "ROBOT_DESCRIPTIONS_CACHE",
+            "~/.cache/robot_descriptions",
+        )
+    )
+    shutil.rmtree(cache_dir, ignore_errors=True)
```

### Comparing `robot_descriptions-1.8.1/robot_descriptions/_command_line.py` & `robot_descriptions-1.9.0/robot_descriptions/_command_line.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/_descriptions.py` & `robot_descriptions-1.9.0/robot_descriptions/_descriptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,28 +47,31 @@
         return Format.URDF in self.formats
 
 
 DESCRIPTIONS: Dict[str, Description] = {
     "a1_description": Description(Format.URDF),
     "a1_mj_description": Description(Format.MJCF),
     "aliengo_description": Description(Format.MJCF),
+    "aloha_mj_description": Description(Format.MJCF),
     "allegro_hand_description": Description(Format.URDF),
+    "allegro_hand_mj_description": Description(Format.MJCF),
     "anymal_b_description": Description(Format.URDF),
     "anymal_b_mj_description": Description(Format.MJCF),
     "anymal_c_description": Description(Format.URDF),
     "anymal_c_mj_description": Description(Format.MJCF),
     "atlas_drc_description": Description(Format.URDF),
     "atlas_v4_description": Description(Format.URDF),
     "b1_description": Description(Format.URDF),
     "barrett_hand_description": Description(Format.URDF),
     "baxter_description": Description(Format.URDF),
     "bolt_description": Description(Format.URDF),
     "cassie_description": Description(Format.URDF),
     "cassie_mj_description": Description(Format.MJCF),
     "cf2_description": Description(Format.URDF),
+    "cf2_mj_description": Description(Format.MJCF),
     "double_pendulum_description": Description(Format.URDF),
     "draco3_description": Description(Format.URDF),
     "edo_description": Description(Format.URDF),
     "ergocub_description": Description(Format.URDF),
     "eve_r3_description": Description(Format.URDF),
     "fanuc_m710ic_description": Description(Format.URDF),
     "fetch_description": Description(Format.URDF),
@@ -80,47 +83,52 @@
     "go1_description": Description(Format.URDF),
     "go1_mj_description": Description(Format.MJCF),
     "h1_description": Description(Format.URDF),
     "h1_mj_description": Description(Format.MJCF),
     "hyq_description": Description(Format.URDF),
     "icub_description": Description(Format.URDF),
     "iiwa_description": Description(Format.URDF),
+    "iiwa_mj_description": Description(Format.MJCF),
     "jaxon_description": Description(Format.URDF),
     "jvrc_description": Description(Format.URDF),
     "jvrc_mj_description": Description(Format.MJCF),
     "laikago_description": Description(Format.URDF),
     "mini_cheetah_description": Description(Format.URDF),
     "minitaur_description": Description(Format.URDF),
     "nextage_description": Description(Format.URDF),
+    "op3_mj_description": Description(Format.MJCF),
     "panda_description": Description(Format.URDF),
     "panda_mj_description": Description(Format.MJCF),
     "pepper_description": Description(Format.URDF),
     "poppy_ergo_jr_description": Description(Format.URDF),
     "poppy_torso_description": Description(Format.URDF),
     "pr2_description": Description(Format.URDF),
     "r2_description": Description(Format.URDF),
     "reachy_description": Description(Format.URDF),
     "rhea_description": Description(Format.URDF),
     "robotiq_2f85_description": Description(Format.URDF),
     "robotiq_2f85_mj_description": Description(Format.MJCF),
     "romeo_description": Description(Format.URDF),
+    "sawyer_mj_description": Description(Format.MJCF),
     "shadow_hand_mj_description": Description(Format.MJCF),
     "simple_humanoid_description": Description(Format.URDF),
     "skydio_x2_description": Description(Format.URDF),
     "skydio_x2_mj_description": Description(Format.MJCF),
     "solo_description": Description(Format.URDF),
     "spryped_description": Description(Format.URDF),
     "stretch_description": Description(Format.URDF),
+    "stretch_mj_description": Description(Format.MJCF),
     "talos_description": Description(Format.URDF),
     "tiago_description": Description(Format.URDF),
     "trifinger_edu_description": Description(Format.URDF),
     "upkie_description": Description(Format.URDF),
     "ur10_description": Description(Format.URDF),
     "ur10e_mj_description": Description(Format.MJCF),
     "ur3_description": Description(Format.URDF),
     "ur5_description": Description(Format.URDF),
     "ur5e_mj_description": Description(Format.MJCF),
     "valkyrie_description": Description(Format.URDF),
+    "viper_mj_description": Description(Format.MJCF),
     "yumi_description": Description(Format.URDF),
     "z1_description": Description(Format.URDF),
     "z1_mj_description": Description(Format.MJCF),
 }
```

### Comparing `robot_descriptions-1.8.1/robot_descriptions/_package_dirs.py` & `robot_descriptions-1.9.0/robot_descriptions/_package_dirs.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/_repositories.py` & `robot_descriptions-1.9.0/robot_descriptions/_repositories.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,16 +119,16 @@
     ),
     "jaxon_description": Repository(
         url="https://github.com/robot-descriptions/jaxon_description.git",
         commit="4a0cb7a4a737864312f8d6e3f89823a741539bfc",
         cache_path="jaxon_description",
     ),
     "jvrc_description": Repository(
-        url="https://github.com/robot-descriptions/jvrc_description.git",
-        commit="b788e1a7c874b3447fc027e175f216c6192e9e96",
+        url="https://github.com/jrl-umi3218/jvrc_description.git",
+        commit="9ff8efbc7043459a8f0892662bd030d8020fb682",
         cache_path="jvrc_description",
     ),
     "jvrc_mj_description": Repository(
         url="https://github.com/isri-aist/jvrc_mj_description.git",
         commit="0f0ce7daefdd66c54e0909a6bf2c22154844f5f3",
         cache_path="jvrc_mj_description",
     ),
@@ -140,15 +140,15 @@
     "mini_cheetah_urdf": Repository(
         url="https://github.com/Derek-TH-Wang/mini_cheetah_urdf.git",
         commit="1988bceb26e81f28594a16e7d5e6abe5cbb27ace",
         cache_path="mini_cheetah_urdf",
     ),
     "mujoco_menagerie": Repository(
         url="https://github.com/deepmind/mujoco_menagerie.git",
-        commit="a099b54b539416bff0db4d35fc2271c35c10f37a",
+        commit="915d92c60858c3649e04af2ae93ac2c51fe18c24",
         cache_path="mujoco_menagerie",
     ),
     "nao_robot": Repository(
         url="https://github.com/ros-naoqi/nao_robot.git",
         commit="67476469a1371b00b17538eb6ea336367ece7d44",
         cache_path="nao_robot",
     ),
@@ -240,15 +240,15 @@
     "unitree_ros": Repository(
         url="https://github.com/unitreerobotics/unitree_ros.git",
         commit="e197ae10d301c41f17f61fe3a741925a033db1e8",
         cache_path="unitree_ros",
     ),
     "upkie_description": Repository(
         url="https://github.com/upkie/upkie_description.git",
-        commit="3bc5251b7255641d275de8c6b949e13bf1a608ea",
+        commit="44445f66b3a40af06a8d2e277436f53377bb8ebd",
         cache_path="upkie_description",
     ),
     "skydio_x2_description": Repository(
         url="https://github.com/lvjonok/skydio_x2_description.git",
         commit="9a6a057a055babaf47119fac42c361fffc189128",
         cache_path="skydio_x2_description",
     ),
```

### Comparing `robot_descriptions-1.8.1/robot_descriptions/a1_description.py` & `robot_descriptions-1.9.0/robot_descriptions/a1_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/a1_mj_description.py` & `robot_descriptions-1.9.0/robot_descriptions/a1_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/aliengo_description.py` & `robot_descriptions-1.9.0/robot_descriptions/aliengo_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/allegro_hand_description.py` & `robot_descriptions-1.9.0/robot_descriptions/allegro_hand_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/anymal_b_description.py` & `robot_descriptions-1.9.0/robot_descriptions/anymal_b_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/anymal_b_mj_description.py` & `robot_descriptions-1.9.0/robot_descriptions/anymal_b_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/anymal_c_description.py` & `robot_descriptions-1.9.0/robot_descriptions/anymal_c_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/anymal_c_mj_description.py` & `robot_descriptions-1.9.0/robot_descriptions/anymal_c_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/atlas_drc_description.py` & `robot_descriptions-1.9.0/robot_descriptions/atlas_drc_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/atlas_v4_description.py` & `robot_descriptions-1.9.0/robot_descriptions/atlas_v4_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/b1_description.py` & `robot_descriptions-1.9.0/robot_descriptions/b1_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/baxter_description.py` & `robot_descriptions-1.9.0/robot_descriptions/baxter_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/bolt_description.py` & `robot_descriptions-1.9.0/robot_descriptions/bolt_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/cassie_mj_description.py` & `robot_descriptions-1.9.0/robot_descriptions/cassie_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/cf2_description.py` & `robot_descriptions-1.9.0/robot_descriptions/cf2_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/double_pendulum_description.py` & `robot_descriptions-1.9.0/robot_descriptions/double_pendulum_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/ergocub_description.py` & `robot_descriptions-1.9.0/robot_descriptions/ergocub_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/eve_r3_description.py` & `robot_descriptions-1.9.0/robot_descriptions/eve_r3_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/fanuc_m710ic_description.py` & `robot_descriptions-1.9.0/robot_descriptions/fanuc_m710ic_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/fetch_description.py` & `robot_descriptions-1.9.0/robot_descriptions/fetch_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/finger_edu_description.py` & `robot_descriptions-1.9.0/robot_descriptions/finger_edu_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/gen2_description.py` & `robot_descriptions-1.9.0/robot_descriptions/gen2_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/gen3_description.py` & `robot_descriptions-1.9.0/robot_descriptions/gen3_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/gen3_mj_description.py` & `robot_descriptions-1.9.0/robot_descriptions/gen3_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/go1_description.py` & `robot_descriptions-1.9.0/robot_descriptions/go1_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/go1_mj_description.py` & `robot_descriptions-1.9.0/robot_descriptions/go2_description.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Stéphane Caron
 
-"""Go1 MJCF description."""
+"""Go2 description."""
 
 from os import getenv as _getenv
 from os import path as _path
 
 from ._cache import clone_to_cache as _clone_to_cache
 
 REPOSITORY_PATH: str = _clone_to_cache(
-    "unitree_mujoco",
+    "unitree_ros",
     commit=_getenv("ROBOT_DESCRIPTION_COMMIT", None),
 )
 
-PACKAGE_PATH: str = _path.join(REPOSITORY_PATH, "data", "go1")
+PACKAGE_PATH: str = _path.join(REPOSITORY_PATH, "robots", "go2_description")
 
-MJCF_PATH: str = _path.join(PACKAGE_PATH, "xml", "go1.xml")
-
-URDF_PATH: str = _path.join(PACKAGE_PATH, "urdf", "go1.urdf")
+URDF_PATH: str = _path.join(PACKAGE_PATH, "urdf", "go2_description.urdf")
```

### Comparing `robot_descriptions-1.8.1/robot_descriptions/go2_description.py` & `robot_descriptions-1.9.0/robot_descriptions/robotiq_2f85_description.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Stéphane Caron
 
-"""Go2 description."""
+"""Robotiq 2F-85 description."""
 
 from os import getenv as _getenv
 from os import path as _path
 
 from ._cache import clone_to_cache as _clone_to_cache
 
 REPOSITORY_PATH: str = _clone_to_cache(
-    "unitree_ros",
+    "robotiq_arg85_description",
     commit=_getenv("ROBOT_DESCRIPTION_COMMIT", None),
 )
 
-PACKAGE_PATH: str = _path.join(REPOSITORY_PATH, "robots", "go2_description")
+PACKAGE_PATH: str = _path.join(REPOSITORY_PATH)
 
-URDF_PATH: str = _path.join(PACKAGE_PATH, "urdf", "go2_description.urdf")
+URDF_PATH: str = _path.join(
+    PACKAGE_PATH, "robots", "robotiq_arg85_description.URDF"
+)
```

### Comparing `robot_descriptions-1.8.1/robot_descriptions/h1_description.py` & `robot_descriptions-1.9.0/robot_descriptions/h1_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/h1_mj_description.py` & `robot_descriptions-1.9.0/robot_descriptions/panda_mj_description.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,14 @@
 
 from os import getenv as _getenv
 from os import path as _path
 
 from ._cache import clone_to_cache as _clone_to_cache
 
 REPOSITORY_PATH: str = _clone_to_cache(
-    "unitree_ros",
+    "mujoco_menagerie",
     commit=_getenv("ROBOT_DESCRIPTION_COMMIT", None),
 )
 
-PACKAGE_PATH: str = _path.join(REPOSITORY_PATH, "robots", "h1_description")
+PACKAGE_PATH: str = _path.join(REPOSITORY_PATH, "franka_emika_panda")
 
-MJCF_PATH: str = _path.join(PACKAGE_PATH, "mjcf", "h1.xml")
+MJCF_PATH: str = _path.join(PACKAGE_PATH, "panda.xml")
```

### Comparing `robot_descriptions-1.8.1/robot_descriptions/hyq_description.py` & `robot_descriptions-1.9.0/robot_descriptions/hyq_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/icub_description.py` & `robot_descriptions-1.9.0/robot_descriptions/icub_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/iiwa_description.py` & `robot_descriptions-1.9.0/robot_descriptions/iiwa_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/laikago_description.py` & `robot_descriptions-1.9.0/robot_descriptions/laikago_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/loaders/idyntree.py` & `robot_descriptions-1.9.0/robot_descriptions/loaders/idyntree.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,17 +35,19 @@
     Returns:
         Identifier of the robot in iDynTree.
 
     Raises:
         ValueError:
             If the description is not URDF, or iDynTree is unable to load it.
     """
-    if commit is not None:
+    if commit is not None:  # technical debt, see #31
         os.environ["ROBOT_DESCRIPTION_COMMIT"] = commit
     module = import_module(f"robot_descriptions.{description_name}")
+    if commit is not None:
+        os.environ.pop("ROBOT_DESCRIPTION_COMMIT", None)
     if not hasattr(module, "URDF_PATH"):
         raise ValueError(f"{description_name} is not a URDF description")
 
     model_loader = idyn.ModelLoader()
 
     if joints_list is None:
         if not model_loader.loadModelFromFile(
```

### Comparing `robot_descriptions-1.8.1/robot_descriptions/loaders/mujoco.py` & `robot_descriptions-1.9.0/robot_descriptions/loaders/mujoco.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,16 @@
         description_name: Name of the robot description.
         commit: If specified, check out that commit from the cloned robot
             description repository.
 
     Returns:
         Robot model for MuJoCo.
     """
-    if commit is not None:
+    if commit is not None:  # technical debt, see #31
         os.environ["ROBOT_DESCRIPTION_COMMIT"] = commit
     module = import_module(f"robot_descriptions.{description_name}")
+    if commit is not None:
+        os.environ.pop("ROBOT_DESCRIPTION_COMMIT", None)
     if not hasattr(module, "MJCF_PATH"):
         raise ValueError(f"{description_name} is not an MJCF description")
 
     return mujoco.MjModel.from_xml_path(module.MJCF_PATH)
```

### Comparing `robot_descriptions-1.8.1/robot_descriptions/loaders/pinocchio.py` & `robot_descriptions-1.9.0/robot_descriptions/loaders/pinocchio.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,16 +44,18 @@
             inertial frame. Defaults to no joint, i.e., a fixed base.
         commit: If specified, check out that commit from the cloned robot
             description repository.
 
     Returns:
         Robot model for Pinocchio.
     """
-    if commit is not None:
+    if commit is not None:  # technical debt, see #31
         os.environ["ROBOT_DESCRIPTION_COMMIT"] = commit
     module = import_module(f"robot_descriptions.{description_name}")
+    if commit is not None:
+        os.environ.pop("ROBOT_DESCRIPTION_COMMIT", None)
     robot = pin.RobotWrapper.BuildFromURDF(
         filename=module.URDF_PATH,
         package_dirs=get_package_dirs(module),
         root_joint=root_joint,
     )
     return robot
```

### Comparing `robot_descriptions-1.8.1/robot_descriptions/loaders/pybullet.py` & `robot_descriptions-1.9.0/robot_descriptions/loaders/pybullet.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,16 +34,18 @@
             useFixedBase: boolean indicating use a fix joint between world and
                 robot base.
             physicsClientId: int indicating the pybullet client id.
 
     Returns:
         Integer identifier of the robot in PyBullet.
     """
-    if commit is not None:
+    if commit is not None:  # technical debt, see #31
         os.environ["ROBOT_DESCRIPTION_COMMIT"] = commit
     module = import_module(f"robot_descriptions.{description_name}")
+    if commit is not None:
+        os.environ.pop("ROBOT_DESCRIPTION_COMMIT", None)
     if not hasattr(module, "URDF_PATH"):
         raise ValueError(f"{description_name} is not a URDF description")
 
     pybullet.setAdditionalSearchPath(module.PACKAGE_PATH)
     robot = pybullet.loadURDF(module.URDF_PATH, **kwargs)
     return robot
```

### Comparing `robot_descriptions-1.8.1/robot_descriptions/loaders/robomeshcat.py` & `robot_descriptions-1.9.0/robot_descriptions/loaders/robomeshcat.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,17 @@
         description_name: Name of the robot description.
         commit: If specified, check out that commit from the cloned robot
             description repository.
 
     Returns:
         Robot model for RoboMeshCat.
     """
-    if commit is not None:
+    if commit is not None:  # technical debt, see #31
         os.environ["ROBOT_DESCRIPTION_COMMIT"] = commit
     module = import_module(f"robot_descriptions.{description_name}")
+    if commit is not None:
+        os.environ.pop("ROBOT_DESCRIPTION_COMMIT", None)
     robot = robomeshcat.Robot(
         urdf_path=module.URDF_PATH,
         mesh_folder_path=get_package_dirs(module),
     )
     return robot
```

### Comparing `robot_descriptions-1.8.1/robot_descriptions/loaders/yourdfpy.py` & `robot_descriptions-1.9.0/robot_descriptions/loaders/yourdfpy.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,14 +30,16 @@
         description_name: Name of the robot description.
         commit: If specified, check out that commit from the cloned robot
             description repository.
 
     Returns:
         Robot model for yourdfpy.
     """
-    if commit is not None:
+    if commit is not None:  # technical debt, see #31
         os.environ["ROBOT_DESCRIPTION_COMMIT"] = commit
     module = import_module(f"robot_descriptions.{description_name}")
+    if commit is not None:
+        os.environ.pop("ROBOT_DESCRIPTION_COMMIT", None)
     if not hasattr(module, "URDF_PATH"):
         raise ValueError(f"{description_name} is not a URDF description")
 
     return yourdfpy.URDF.load(module.URDF_PATH, mesh_dir=module.PACKAGE_PATH)
```

### Comparing `robot_descriptions-1.8.1/robot_descriptions/mini_cheetah_description.py` & `robot_descriptions-1.9.0/robot_descriptions/mini_cheetah_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/nextage_description.py` & `robot_descriptions-1.9.0/robot_descriptions/nextage_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/panda_description.py` & `robot_descriptions-1.9.0/robot_descriptions/panda_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/panda_mj_description.py` & `robot_descriptions-1.9.0/robot_descriptions/ur5e_mj_description.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Stéphane Caron
 
-"""Panda MJCF description."""
+"""UR5e MJCF description."""
 
 from os import getenv as _getenv
 from os import path as _path
 
 from ._cache import clone_to_cache as _clone_to_cache
 
 REPOSITORY_PATH: str = _clone_to_cache(
     "mujoco_menagerie",
     commit=_getenv("ROBOT_DESCRIPTION_COMMIT", None),
 )
 
-PACKAGE_PATH: str = _path.join(REPOSITORY_PATH, "franka_emika_panda")
+PACKAGE_PATH: str = _path.join(REPOSITORY_PATH, "universal_robots_ur5e")
 
-MJCF_PATH: str = _path.join(PACKAGE_PATH, "panda.xml")
+MJCF_PATH: str = _path.join(PACKAGE_PATH, "ur5e.xml")
```

### Comparing `robot_descriptions-1.8.1/robot_descriptions/poppy_ergo_jr_description.py` & `robot_descriptions-1.9.0/robot_descriptions/poppy_ergo_jr_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/poppy_torso_description.py` & `robot_descriptions-1.9.0/robot_descriptions/poppy_torso_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/r2_description.py` & `robot_descriptions-1.9.0/robot_descriptions/r2_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/robotiq_2f85_description.py` & `robot_descriptions-1.9.0/robot_descriptions/romeo_description.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Stéphane Caron
 
-"""Robotiq 2F-85 description."""
+"""Romeo description."""
 
 from os import getenv as _getenv
 from os import path as _path
 
 from ._cache import clone_to_cache as _clone_to_cache
 
 REPOSITORY_PATH: str = _clone_to_cache(
-    "robotiq_arg85_description",
+    "romeo_robot",
     commit=_getenv("ROBOT_DESCRIPTION_COMMIT", None),
 )
 
-PACKAGE_PATH: str = _path.join(REPOSITORY_PATH)
+PACKAGE_PATH: str = _path.join(REPOSITORY_PATH, "romeo_description")
 
 URDF_PATH: str = _path.join(
-    PACKAGE_PATH, "robots", "robotiq_arg85_description.URDF"
+    PACKAGE_PATH, "urdf", "romeo_generated_urdf", "romeo.urdf"
 )
```

### Comparing `robot_descriptions-1.8.1/robot_descriptions/robotiq_2f85_mj_description.py` & `robot_descriptions-1.9.0/robot_descriptions/robotiq_2f85_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/romeo_description.py` & `robot_descriptions-1.9.0/robot_descriptions/go1_mj_description.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Stéphane Caron
 
-"""Romeo description."""
+"""Unitree Go1 MJCF description."""
 
 from os import getenv as _getenv
 from os import path as _path
 
 from ._cache import clone_to_cache as _clone_to_cache
 
 REPOSITORY_PATH: str = _clone_to_cache(
-    "romeo_robot",
+    "mujoco_menagerie",
     commit=_getenv("ROBOT_DESCRIPTION_COMMIT", None),
 )
 
-PACKAGE_PATH: str = _path.join(REPOSITORY_PATH, "romeo_description")
+PACKAGE_PATH: str = _path.join(REPOSITORY_PATH, "unitree_go1")
 
-URDF_PATH: str = _path.join(
-    PACKAGE_PATH, "urdf", "romeo_generated_urdf", "romeo.urdf"
-)
+MJCF_PATH: str = _path.join(PACKAGE_PATH, "go1.xml")
```

### Comparing `robot_descriptions-1.8.1/robot_descriptions/shadow_hand_mj_description.py` & `robot_descriptions-1.9.0/robot_descriptions/shadow_hand_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/simple_humanoid_description.py` & `robot_descriptions-1.9.0/robot_descriptions/simple_humanoid_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/solo_description.py` & `robot_descriptions-1.9.0/robot_descriptions/solo_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/spryped_description.py` & `robot_descriptions-1.9.0/robot_descriptions/spryped_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/talos_description.py` & `robot_descriptions-1.9.0/robot_descriptions/talos_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/tiago_description.py` & `robot_descriptions-1.9.0/robot_descriptions/tiago_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/trifinger_edu_description.py` & `robot_descriptions-1.9.0/robot_descriptions/trifinger_edu_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/ur10_description.py` & `robot_descriptions-1.9.0/robot_descriptions/ur10_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/ur10e_mj_description.py` & `robot_descriptions-1.9.0/robot_descriptions/ur10e_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/ur3_description.py` & `robot_descriptions-1.9.0/robot_descriptions/ur3_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/ur5_description.py` & `robot_descriptions-1.9.0/robot_descriptions/ur5_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/ur5e_mj_description.py` & `robot_descriptions-1.9.0/robot_descriptions/go2_mj_description.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Stéphane Caron
 
-"""UR5e MJCF description."""
+"""Unitree Go2 MJCF description."""
 
 from os import getenv as _getenv
 from os import path as _path
 
 from ._cache import clone_to_cache as _clone_to_cache
 
 REPOSITORY_PATH: str = _clone_to_cache(
     "mujoco_menagerie",
     commit=_getenv("ROBOT_DESCRIPTION_COMMIT", None),
 )
 
-PACKAGE_PATH: str = _path.join(REPOSITORY_PATH, "universal_robots_ur5e")
+PACKAGE_PATH: str = _path.join(REPOSITORY_PATH, "unitree_go2")
 
-MJCF_PATH: str = _path.join(PACKAGE_PATH, "ur5e.xml")
+MJCF_PATH: str = _path.join(PACKAGE_PATH, "go2.xml")
```

### Comparing `robot_descriptions-1.8.1/robot_descriptions/valkyrie_description.py` & `robot_descriptions-1.9.0/robot_descriptions/valkyrie_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/yumi_description.py` & `robot_descriptions-1.9.0/robot_descriptions/yumi_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/robot_descriptions/z1_description.py` & `robot_descriptions-1.9.0/robot_descriptions/z1_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/tests/loaders/test_idyntree.py` & `robot_descriptions-1.9.0/tests/loaders/test_idyntree.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/tests/loaders/test_mujoco.py` & `robot_descriptions-1.9.0/tests/loaders/test_mujoco.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/tests/loaders/test_pinocchio.py` & `robot_descriptions-1.9.0/tests/loaders/test_pinocchio.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/tests/loaders/test_pybullet.py` & `robot_descriptions-1.9.0/tests/loaders/test_pybullet.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/tests/loaders/test_robomeshcat.py` & `robot_descriptions-1.9.0/tests/loaders/test_robomeshcat.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/tests/loaders/test_yourdfpy.py` & `robot_descriptions-1.9.0/tests/loaders/test_yourdfpy.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/tests/test_clone_to_cache.py` & `robot_descriptions-1.9.0/tests/test_clone_to_cache.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import os
 import tempfile
 import unittest
 
 import git
 
-from robot_descriptions._cache import clone_to_cache
+from robot_descriptions._cache import clone_to_cache, clear_cache
 from robot_descriptions._repositories import REPOSITORIES
 
 
 class TestCloneToCache(unittest.TestCase):
     def test_clone_to_cache_found(self):
         """
         Test clone_to_cache on a valid repository.
@@ -59,8 +59,16 @@
         with self.assertRaises(git.exc.GitCommandError):
             clone_to_cache("simple_humanoid_description", commit="foobar")
 
     def test_clone_valid_commit(self):
         description_name = "simple_humanoid_description"
         commit = "0e488ee4708155a71b2a92d05305a9186b543593"
         repository_path = clone_to_cache(description_name, commit)
-        self.assertTrue(repository_path.endswith(f"-{commit}"))
+        self.assertTrue(commit in repository_path)
+
+    def test_clone_with_commit_then_without(self):
+        clear_cache()
+        clone_to_cache(
+            "upkie_description",
+            commit="a2c820054a7572603875def478f21376165c125e",
+        )
+        clone_to_cache("draco3_description")
```

### Comparing `robot_descriptions-1.8.1/tests/test_clone_to_directory.py` & `robot_descriptions-1.9.0/tests/test_clone_to_directory.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/tests/test_descriptions.py` & `robot_descriptions-1.9.0/tests/test_descriptions.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/tests/test_loaders.py` & `robot_descriptions-1.9.0/tests/test_loaders.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 )
 from robot_descriptions.loaders.yourdfpy import (
     load_robot_description as load_yourdfpy,
 )
 
 
 class TestLoaders(unittest.TestCase):
-
     """
     Test loaders.
     """
 
     upkie_description_commit = "98502d5b175c3d6b60b3cf475b7eeef9fd290c43"
 
     def test_mujoco(self):
@@ -76,7 +75,22 @@
     def test_idyntree(self):
         self.assertIsNotNone(
             load_idyntree(
                 "upkie_description",
                 commit=self.upkie_description_commit,
             )
         )
+
+    def test_cache_path_package_name(self):
+        """Check a description with package:// URIs and a custom commit ID."""
+        load_pinocchio(
+            "draco3_description",
+            commit="5afd19733d7b3e9f1135ba93e0aad90ed1a24cc7",
+        )
+
+    def test_load_with_commit_then_without(self):
+        # https://github.com/robot-descriptions/robot_descriptions.py/issues/67
+        load_pinocchio(
+            "draco3_description",
+            commit="5afd19733d7b3e9f1135ba93e0aad90ed1a24cc7",
+        )
+        load_pinocchio("baxter_description")
```

### Comparing `robot_descriptions-1.8.1/tox.ini` & `robot_descriptions-1.9.0/tox.ini`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.8.1/PKG-INFO` & `robot_descriptions-1.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robot_descriptions
-Version: 1.8.1
+Version: 1.9.0
 Summary: Import open source robot description as Python modules.
 Keywords: robot,description,urdf,mjcf
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
@@ -39,21 +39,25 @@
 
 Import open source robot descriptions as Python modules.
 
 Importing a description for the first time automatically downloads and caches files for future imports. Most [Awesome Robot Descriptions](https://github.com/robot-descriptions/awesome-robot-descriptions) are available. All of them load successfully in respectively MuJoCo (MJCF) or Pinocchio, iDynTree, PyBullet and yourdfpy (URDF).
 
 ## Installation
 
-### Install from pip
+### PyPI
+
+[![PyPI version](https://img.shields.io/pypi/v/robot_descriptions)](https://pypi.org/project/robot_descriptions/)
 
 ```console
 pip install robot_descriptions
 ```
 
-### Install from conda
+### Conda
+
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/robot_descriptions.svg)](https://anaconda.org/conda-forge/robot_descriptions)
 
 ```console
 conda install -c conda-forge robot_descriptions
 ```
 
 ## Usage
 
@@ -138,44 +142,47 @@
 robot_descriptions show solo_description
 ```
 
 ## Descriptions
 
 Available robot descriptions ([gallery](https://github.com/robot-descriptions/awesome-robot-descriptions#gallery)) are listed in the following categories:
 
-* [Arms](#arms)
-* [Bipeds](#bipeds)
-* [Dual arms](#dual-arms)
-* [Drones](#drones)
-* [Educational](#educational)
-* [End effectors](#end-effectors)
-* [Mobile manipulators](#mobile-manipulators)
-* [Humanoids](#humanoids)
-* [Quadrupeds](#quadrupeds)
+- [Arms](#arms)
+- [Bipeds](#bipeds)
+- [Dual arms](#dual-arms)
+- [Drones](#drones)
+- [Educational](#educational)
+- [End effectors](#end-effectors)
+- [Humanoids](#humanoids)
+- [Mobile manipulators](#mobile-manipulators)
+- [Quadrupeds](#quadrupeds)
 
 The DOF column denotes the number of actuated degrees of freedom.
 
 ### Arms
 
 | Name                          | Robot                 | Maker                    | DOF | Format     |
 |-------------------------------|-----------------------|--------------------------|-----|------------|
 | `edo_description`             | e.DO                  | Comau                    | 6   | URDF       |
 | `fanuc_m710ic_description`    | M-710iC               | Fanuc                    | 6   | URDF       |
 | `gen2_description`            | Gen2 (Jaco)           | Kinova                   | 6   | URDF       |
 | `gen3_description`            | Gen3 (Jaco)           | Kinova                   | 6   | URDF       |
 | `gen3_mj_description`         | Gen3 (Jaco)           | Kinova                   | 7   | MJCF       |
 | `iiwa_description`            | iiwa                  | KUKA                     | 7   | URDF       |
+| `iiwa_mj_description`         | iiwa14                | KUKA                     | 7   | MJCF       |
 | `panda_description`           | Panda                 | Franka Emika             | 8   | URDF       |
 | `panda_mj_description`        | Panda                 | Franka Emika             | 8   | MJCF       |
 | `poppy_ergo_jr_description`   | Poppy Ergo Jr         | Poppy Project            | 6   | URDF       |
+| `sawyer_mj_description`       | Sawyer                | Rethink Robotics         | 7   | MJCF       |
 | `ur10_description`            | UR10                  | Universal Robots         | 6   | URDF       |
 | `ur10e_mj_description`        | UR10e                 | Universal Robots         | 6   | MJCF       |
 | `ur3_description`             | UR3                   | Universal Robots         | 6   | URDF       |
 | `ur5_description`             | UR5                   | Universal Robots         | 6   | URDF       |
 | `ur5e_mj_description`         | UR5e                  | Universal Robots         | 6   | MJCF       |
+| `viper_mj_description`        | Viper                 | Trossen Robotics         | 7   | MJCF       |
 | `z1_description`              | Z1                    | UNITREE Robotics         | 6   | URDF       |
 
 ### Bipeds
 
 | Name                          | Robot                 | Maker                    | DOF | Format     |
 |-------------------------------|-----------------------|--------------------------|-----|------------|
 | `bolt_description`            | Bolt                  | ODRI                     | 6   | URDF       |
@@ -185,24 +192,26 @@
 | `spryped_description`         | Spryped               | Benjamin Bokser          | 8   | URDF       |
 | `upkie_description`           | Upkie                 | Tast's Robots            | 6   | URDF       |
 
 ### Dual arms
 
 | Name                          | Robot                 | Maker                    | DOF | Format     |
 |-------------------------------|-----------------------|--------------------------|-----|------------|
+| `aloha_mj_description`        | Aloha 2               | Trossen Robotics         | 14  | MJCF       |
 | `baxter_description`          | Baxter                | Rethink Robotics         | 15  | URDF       |
 | `nextage_description`         | NEXTAGE               | Kawada Robotics          | 15  | URDF       |
 | `poppy_torso_description`     | Poppy Torso           | Poppy Project            | 13  | URDF       |
 | `yumi_description`            | YuMi                  | ABB                      | 16  | URDF       |
 
 ### Drones
 
 | Name                          | Robot                 | Maker                    | DOF | Format     |
 |-------------------------------|-----------------------|--------------------------|-----|------------|
 | `cf2_description`             | Crazyflie 2.0         | Bitcraze                 | 0   | URDF       |
+| `cf2_mj_description`          | Crazyflie 2.0         | Bitcraze                 | 6   | MJCF       |
 | `skydio_x2_description`       | Skydio X2             | Skydio                   | 6   | URDF       |
 | `skydio_x2_mj_description`    | Skydio X2             | Skydio                   | 6   | MJCF       |
 
 ### Educational
 
 | Name                          | Robot                 | DOF | Format     |
 |-------------------------------|-----------------------|-----|------------|
@@ -212,14 +221,15 @@
 | `trifinger_edu_description`   | TriFingerEdu          | 9   | URDF       |
 
 ### End effectors
 
 | Name                          | Robot                 | Maker                    | DOF | Format     |
 |-------------------------------|-----------------------|--------------------------|-----|------------|
 | `allegro_hand_description`    | Allegro Hand          | Wonik Robotics           | 16  | URDF       |
+| `allegro_hand_mj_description` | Allegro Hand          | Wonik Robotics           | 16  | MJCF       |
 | `barrett_hand_description`    | BarrettHand           | Barrett Technology       | 8   | URDF       |
 | `robotiq_2f85_description`    | Robotiq 2F-85         | Robotiq                  | 1   | URDF       |
 | `robotiq_2f85_mj_description` | Robotiq 2F-85         | Robotiq                  | 1   | MJCF       |
 | `shadow_hand_mj_description`  | Shadow Hand           | The Shadow Robot Company | 24  | MJCF       |
 
 ### Humanoids
 
@@ -231,14 +241,15 @@
 | `ergocub_description`         | ergoCub               | IIT                      | 57  | URDF       |
 | `h1_description`              | H1                    | UNITREE Robotics         | 25  | URDF       |
 | `h1_mj_description`           | H1                    | UNITREE Robotics         | 25  | MJCF       |
 | `icub_description`            | iCub                  | IIT                      | 32  | URDF       |
 | `jaxon_description`           | JAXON                 | JSK                      | 38  | URDF       |
 | `jvrc_description`            | JVRC-1                | AIST                     | 34  | URDF       |
 | `jvrc_mj_description`         | JVRC-1                | AIST                     | 34  | MJCF       |
+| `op3_mj_description`          | OP3                   | ROBOTIS                  | 20  | MJCF       |
 | `r2_description`              | Robonaut 2            | NASA JSC Robotics        | 56  | URDF       |
 | `romeo_description`           | Romeo                 | Aldebaran Robotics       | 37  | URDF       |
 | `sigmaban_description`        | SigmaBan              | Rhoban                   | 20  | URDF       |
 | `talos_description`           | TALOS                 | PAL Robotics             | 32  | URDF       |
 | `valkyrie_description`        | Valkyrie              | NASA JSC Robotics        | 59  | URDF       |
 
 ### Mobile manipulators
@@ -248,14 +259,15 @@
 | `eve_r3_description`          | Eve R3                | Halodi                   | 23  | URDF       |
 | `fetch_description`           | Fetch                 | Fetch Robotics           | 14  | URDF       |
 | `ginger_description`          | Ginger                | Paaila Technology        | 49  | URDF       |
 | `pepper_description`          | Pepper                | SoftBank Robotics        | 17  | URDF       |
 | `pr2_description`             | PR2                   | Willow Garage            | 32  | URDF       |
 | `reachy_description`          | Reachy                | Pollen Robotics          | 21  | URDF       |
 | `stretch_description`         | Stretch RE1           | Hello Robot              | 14  | URDF       |
+| `sretch_mj_description`       | Stretch 2             | Hello Robot              | 14  | MJCF       |
 | `tiago_description`           | TIAGo                 | PAL Robotics             | 48  | URDF       |
 
 ### Quadrupeds
 
 | Name                          | Robot                 | Maker                    | DOF | Format     |
 |-------------------------------|-----------------------|--------------------------|-----|------------|
 | `a1_mj_description`           | A1                    | UNITREE Robotics         | 12  | MJCF       |
@@ -280,14 +292,30 @@
 
 New robot descriptions are welcome! Check out the [guidelines](https://github.com/robot-descriptions/robot_descriptions.py/tree/main/CONTRIBUTING.md) then open a PR.
 
 ## Thanks
 
 Thanks to the maintainers of all the git repositories that made these robot descriptions available.
 
+## Citation
+
+If you use `robot_descriptions.py` in your scientific works, please cite it *e.g.* as follows:
+
+```bibtex
+@software{robot_descriptions_py2024,
+  author = {Caron, Stéphane and Romualdi, Giulio and Kozlov, Lev and Ordonez, Daniel and Tadashi Kussaba, Hugo and Bang, Seung Hyeon and Zakka, Kevin},
+  license = {Apache-2.0},
+  month = mar,
+  title = {{robot_descriptions.py: Robot descriptions in Python}},
+  url = {https://github.com/robot-descriptions/robot_descriptions.py},
+  version = {1.9.0},
+  year = {2024}
+}
+```
+
 ## See also
 
 Robot descriptions in other languages:
 
 | ![C++](https://img.shields.io/badge/C%2B%2B-00599C?logo=c%2B%2B&logoColor=white) | [robot\_descriptions.cpp](https://github.com/mayataka/robot_descriptions.cpp) |
 |--|--|
```

