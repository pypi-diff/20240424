# Comparing `tmp/rlberry-0.7.2.tar.gz` & `tmp/rlberry-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlberry-0.7.2.tar", max compression
+gzip compressed data, was "rlberry-0.7.3.tar", max compression
```

## Comparing `rlberry-0.7.2.tar` & `rlberry-0.7.3.tar`

### file list

```diff
@@ -1,131 +1,128 @@
--rw-r--r--   0        0        0     1067 2024-03-06 13:20:21.183589 rlberry-0.7.2/LICENSE
--rw-r--r--   0        0        0     4053 2024-03-06 13:20:21.183589 rlberry-0.7.2/README.md
--rw-r--r--   0        0        0     3272 2024-03-06 13:20:38.939307 rlberry-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      376 2024-03-06 13:20:21.215588 rlberry-0.7.2/rlberry/__init__.py
--rw-r--r--   0        0        0      109 2024-03-06 13:20:21.215588 rlberry-0.7.2/rlberry/agents/__init__.py
--rw-r--r--   0        0        0    28030 2024-03-06 13:20:21.215588 rlberry-0.7.2/rlberry/agents/agent.py
--rw-r--r--   0        0        0       51 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/agents/stable_baselines/__init__.py
--rw-r--r--   0        0        0     9619 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/agents/stable_baselines/stable_baselines.py
--rw-r--r--   0        0        0        0 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/agents/tests/__init__.py
--rw-r--r--   0        0        0     6106 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/agents/tests/test_replay.py
--rw-r--r--   0        0        0     1058 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/agents/tests/test_stable_baselines.py
--rw-r--r--   0        0        0        0 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/agents/utils/__init__.py
--rw-r--r--   0        0        0    14321 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/agents/utils/replay.py
--rw-r--r--   0        0        0     5290 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/agents/utils/replay_utils.py
--rw-r--r--   0        0        0      478 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/check_packages.py
--rw-r--r--   0        0        0      173 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/envs/__init__.py
--rw-r--r--   0        0        0     4626 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/envs/basewrapper.py
--rw-r--r--   0        0        0     5728 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/envs/finite_mdp.py
--rw-r--r--   0        0        0     5278 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/envs/gym_make.py
--rw-r--r--   0        0        0       25 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/envs/interface/__init__.py
--rw-r--r--   0        0        0     4826 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/envs/interface/model.py
--rw-r--r--   0        0        0     1227 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/envs/pipeline.py
--rw-r--r--   0        0        0        0 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/envs/tests/__init__.py
--rw-r--r--   0        0        0     2661 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/envs/tests/test_env_seeding.py
--rw-r--r--   0        0        0     2365 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/envs/tests/test_gym_env_seeding.py
--rw-r--r--   0        0        0     4788 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/envs/tests/test_gym_make.py
--rw-r--r--   0        0        0      849 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/envs/utils.py
--rw-r--r--   0        0        0      142 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/experiment/__init__.py
--rw-r--r--   0        0        0     1855 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/experiment/generator.py
--rw-r--r--   0        0        0     3760 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/experiment/load_results.py
--rw-r--r--   0        0        0      375 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/experiment/tests/params_experiment.yaml
--rw-r--r--   0        0        0      144 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/experiment/tests/room.yaml
--rw-r--r--   0        0        0      269 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/experiment/tests/rsucbvi.yaml
--rw-r--r--   0        0        0      106 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/experiment/tests/rsucbvi_alternative.yaml
--rw-r--r--   0        0        0     1772 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/experiment/tests/test_experiment_generator.py
--rw-r--r--   0        0        0      818 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/experiment/tests/test_load_results.py
--rw-r--r--   0        0        0     6150 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/experiment/yaml_utils.py
--rw-r--r--   0        0        0      463 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/manager/__init__.py
--rw-r--r--   0        0        0    15413 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/manager/comparison.py
--rw-r--r--   0        0        0    12163 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/manager/evaluation.py
--rw-r--r--   0        0        0    51801 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/manager/experiment_manager.py
--rw-r--r--   0        0        0     3027 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/manager/multiple_managers.py
--rw-r--r--   0        0        0    25666 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/manager/plotting.py
--rw-r--r--   0        0        0        0 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/manager/tests/__init__.py
--rw-r--r--   0        0        0     3861 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/manager/tests/test_comparisons.py
--rw-r--r--   0        0        0    16792 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/manager/tests/test_experiment_manager.py
--rw-r--r--   0        0        0     2764 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/manager/tests/test_experiment_manager_seeding.py
--rw-r--r--   0        0        0     6056 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/manager/tests/test_hyperparam_optim.py
--rw-r--r--   0        0        0     8145 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/manager/tests/test_plot.py
--rw-r--r--   0        0        0     1259 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/manager/tests/test_shared_data.py
--rw-r--r--   0        0        0      391 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/manager/utils.py
--rw-r--r--   0        0        0     1947 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/metadata_utils.py
--rw-r--r--   0        0        0      138 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/rendering/__init__.py
--rw-r--r--   0        0        0     1001 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/rendering/common_shapes.py
--rw-r--r--   0        0        0     1265 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/rendering/core.py
--rw-r--r--   0        0        0     7709 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/rendering/opengl_render2d.py
--rw-r--r--   0        0        0     5931 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/rendering/pygame_render2d.py
--rw-r--r--   0        0        0     4604 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/rendering/render_interface.py
--rw-r--r--   0        0        0        0 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/rendering/tests/__init__.py
--rw-r--r--   0        0        0     7807 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/rendering/tests/test_rendering_interface.py
--rw-r--r--   0        0        0     2616 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/rendering/utils.py
--rw-r--r--   0        0        0       99 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/seeding/__init__.py
--rw-r--r--   0        0        0     3973 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/seeding/seeder.py
--rw-r--r--   0        0        0     2234 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/seeding/seeding.py
--rw-r--r--   0        0        0        0 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/seeding/tests/__init__.py
--rw-r--r--   0        0        0     1728 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/seeding/tests/test_seeding.py
--rw-r--r--   0        0        0      874 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/seeding/tests/test_threads.py
--rw-r--r--   0        0        0     1072 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/seeding/tests/test_threads_torch.py
--rw-r--r--   0        0        0      180 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/spaces/__init__.py
--rw-r--r--   0        0        0     3022 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/spaces/box.py
--rw-r--r--   0        0        0      826 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/spaces/dict.py
--rw-r--r--   0        0        0     1572 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/spaces/discrete.py
--rw-r--r--   0        0        0     1471 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/spaces/from_gym.py
--rw-r--r--   0        0        0     1280 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/spaces/multi_binary.py
--rw-r--r--   0        0        0     1366 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/spaces/multi_discrete.py
--rw-r--r--   0        0        0        0 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/spaces/tests/__init__.py
--rw-r--r--   0        0        0     4874 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/spaces/tests/test_from_gym.py
--rw-r--r--   0        0        0     3611 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/spaces/tests/test_spaces.py
--rw-r--r--   0        0        0      782 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/spaces/tuple.py
--rw-r--r--   0        0        0        0 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/tests/__init__.py
--rw-r--r--   0        0        0     2819 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/tests/test_agent_extra.py
--rw-r--r--   0        0        0     2036 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/tests/test_agents_base.py
--rw-r--r--   0        0        0      823 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/tests/test_envs.py
--rw-r--r--   0        0        0      321 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/tests/test_imports.py
--rw-r--r--   0        0        0     3610 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/tests/test_rlberry_main_agents_and_env.py
--rw-r--r--   0        0        0      302 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/types.py
--rw-r--r--   0        0        0      182 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/utils/__init__.py
--rw-r--r--   0        0        0     1177 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/utils/binsearch.py
--rw-r--r--   0        0        0    24546 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/utils/check_agent.py
--rw-r--r--   0        0        0     1490 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/utils/check_env.py
--rw-r--r--   0        0        0    11348 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/utils/check_gym_env.py
--rw-r--r--   0        0        0      199 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/utils/factory.py
--rw-r--r--   0        0        0      395 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/utils/jit_setup.py
--rw-r--r--   0        0        0     3466 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/utils/logging.py
--rw-r--r--   0        0        0      699 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/utils/metrics.py
--rw-r--r--   0        0        0     2206 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/utils/space_discretizer.py
--rw-r--r--   0        0        0        0 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/utils/tests/__init__.py
--rw-r--r--   0        0        0     1061 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/utils/tests/test_binsearch.py
--rw-r--r--   0        0        0     3236 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/utils/tests/test_check.py
--rw-r--r--   0        0        0      483 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/utils/tests/test_metrics.py
--rw-r--r--   0        0        0     1985 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/utils/tests/test_writer.py
--rw-r--r--   0        0        0     2517 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/utils/torch.py
--rw-r--r--   0        0        0    17459 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/utils/writers.py
--rw-r--r--   0        0        0      195 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/__init__.py
--rw-r--r--   0        0        0     1017 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/autoreset.py
--rw-r--r--   0        0        0     1059 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/discrete2onehot.py
--rw-r--r--   0        0        0     3455 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/discretize_state.py
--rw-r--r--   0        0        0     1956 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/gym_utils.py
--rw-r--r--   0        0        0     2154 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/rescale_reward.py
--rw-r--r--   0        0        0      243 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/tests/__init__.py
--rw-r--r--   0        0        0      411 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/tests/old_env/__init__.py
--rw-r--r--   0        0        0    12214 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/tests/old_env/old_acrobot.py
--rw-r--r--   0        0        0     5552 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/tests/old_env/old_apple_gold.py
--rw-r--r--   0        0        0     6337 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/tests/old_env/old_ball2d.py
--rw-r--r--   0        0        0     5806 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/tests/old_env/old_finite_mdp.py
--rw-r--r--   0        0        0     4065 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/tests/old_env/old_four_room.py
--rw-r--r--   0        0        0    16455 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/tests/old_env/old_gridworld.py
--rw-r--r--   0        0        0     6159 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/tests/old_env/old_mountain_car.py
--rw-r--r--   0        0        0    10752 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/tests/old_env/old_nroom.py
--rw-r--r--   0        0        0    14902 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/tests/old_env/old_pball.py
--rw-r--r--   0        0        0     3865 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/tests/old_env/old_pendulum.py
--rw-r--r--   0        0        0     4487 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/tests/old_env/old_six_room.py
--rw-r--r--   0        0        0     5670 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/tests/old_env/old_twinrooms.py
--rw-r--r--   0        0        0      798 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/tests/test_basewrapper.py
--rw-r--r--   0        0        0     7979 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/tests/test_common_wrappers.py
--rw-r--r--   0        0        0     3001 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/tests/test_gym_space_conversion.py
--rw-r--r--   0        0        0     4039 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/tests/test_wrapper_seeding.py
--rw-r--r--   0        0        0     1132 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/tests/test_writer_utils.py
--rw-r--r--   0        0        0     3636 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/uncertainty_estimator_wrapper.py
--rw-r--r--   0        0        0     1465 2024-03-06 13:20:21.219588 rlberry-0.7.2/rlberry/wrappers/writer_utils.py
--rw-r--r--   0        0        0     6476 1970-01-01 00:00:00.000000 rlberry-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-24 14:15:13.443367 rlberry-0.7.3/LICENSE
+-rw-r--r--   0        0        0     4063 2024-04-24 14:15:13.443367 rlberry-0.7.3/README.md
+-rw-r--r--   0        0        0     3136 2024-04-24 14:19:10.918577 rlberry-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0      376 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/__init__.py
+-rw-r--r--   0        0        0      109 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/agents/__init__.py
+-rw-r--r--   0        0        0    28030 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/agents/agent.py
+-rw-r--r--   0        0        0       51 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/agents/stable_baselines/__init__.py
+-rw-r--r--   0        0        0     9619 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/agents/stable_baselines/stable_baselines.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/agents/tests/__init__.py
+-rw-r--r--   0        0        0     6106 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/agents/tests/test_replay.py
+-rw-r--r--   0        0        0     1058 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/agents/tests/test_stable_baselines.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/agents/utils/__init__.py
+-rw-r--r--   0        0        0    14321 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/agents/utils/replay.py
+-rw-r--r--   0        0        0     5290 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/agents/utils/replay_utils.py
+-rw-r--r--   0        0        0      336 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/check_packages.py
+-rw-r--r--   0        0        0      173 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/envs/__init__.py
+-rw-r--r--   0        0        0     4626 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/envs/basewrapper.py
+-rw-r--r--   0        0        0     5728 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/envs/finite_mdp.py
+-rw-r--r--   0        0        0     5278 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/envs/gym_make.py
+-rw-r--r--   0        0        0       25 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/envs/interface/__init__.py
+-rw-r--r--   0        0        0     4826 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/envs/interface/model.py
+-rw-r--r--   0        0        0     1227 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/envs/pipeline.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/envs/tests/__init__.py
+-rw-r--r--   0        0        0     2655 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/envs/tests/test_env_seeding.py
+-rw-r--r--   0        0        0     2365 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/envs/tests/test_gym_env_seeding.py
+-rw-r--r--   0        0        0     4788 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/envs/tests/test_gym_make.py
+-rw-r--r--   0        0        0      849 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/envs/utils.py
+-rw-r--r--   0        0        0      142 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/experiment/__init__.py
+-rw-r--r--   0        0        0     1855 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/experiment/generator.py
+-rw-r--r--   0        0        0     3760 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/experiment/load_results.py
+-rw-r--r--   0        0        0      375 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/experiment/tests/params_experiment.yaml
+-rw-r--r--   0        0        0      144 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/experiment/tests/room.yaml
+-rw-r--r--   0        0        0      269 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/experiment/tests/rsucbvi.yaml
+-rw-r--r--   0        0        0      106 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/experiment/tests/rsucbvi_alternative.yaml
+-rw-r--r--   0        0        0     1772 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/experiment/tests/test_experiment_generator.py
+-rw-r--r--   0        0        0      818 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/experiment/tests/test_load_results.py
+-rw-r--r--   0        0        0     6150 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/experiment/yaml_utils.py
+-rw-r--r--   0        0        0      463 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/manager/__init__.py
+-rw-r--r--   0        0        0    16104 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/manager/comparison.py
+-rw-r--r--   0        0        0    12270 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/manager/evaluation.py
+-rw-r--r--   0        0        0    51603 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/manager/experiment_manager.py
+-rw-r--r--   0        0        0     3027 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/manager/multiple_managers.py
+-rw-r--r--   0        0        0    25666 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/manager/plotting.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/manager/tests/__init__.py
+-rw-r--r--   0        0        0     3892 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/manager/tests/test_comparisons.py
+-rw-r--r--   0        0        0    16792 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/manager/tests/test_experiment_manager.py
+-rw-r--r--   0        0        0     2764 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/manager/tests/test_experiment_manager_seeding.py
+-rw-r--r--   0        0        0     6056 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/manager/tests/test_hyperparam_optim.py
+-rw-r--r--   0        0        0     8142 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/manager/tests/test_plot.py
+-rw-r--r--   0        0        0     1259 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/manager/tests/test_shared_data.py
+-rw-r--r--   0        0        0      391 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/manager/utils.py
+-rw-r--r--   0        0        0     1947 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/metadata_utils.py
+-rw-r--r--   0        0        0      138 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/rendering/__init__.py
+-rw-r--r--   0        0        0     1001 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/rendering/common_shapes.py
+-rw-r--r--   0        0        0     1265 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/rendering/core.py
+-rw-r--r--   0        0        0     7709 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/rendering/opengl_render2d.py
+-rw-r--r--   0        0        0     5931 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/rendering/pygame_render2d.py
+-rw-r--r--   0        0        0     4604 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/rendering/render_interface.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/rendering/tests/__init__.py
+-rw-r--r--   0        0        0     7667 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/rendering/tests/test_rendering_interface.py
+-rw-r--r--   0        0        0     2616 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/rendering/utils.py
+-rw-r--r--   0        0        0       99 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/seeding/__init__.py
+-rw-r--r--   0        0        0     3973 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/seeding/seeder.py
+-rw-r--r--   0        0        0     2234 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/seeding/seeding.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/seeding/tests/__init__.py
+-rw-r--r--   0        0        0     1728 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/seeding/tests/test_seeding.py
+-rw-r--r--   0        0        0      874 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/seeding/tests/test_threads.py
+-rw-r--r--   0        0        0     1072 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/seeding/tests/test_threads_torch.py
+-rw-r--r--   0        0        0      180 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/spaces/__init__.py
+-rw-r--r--   0        0        0     3022 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/spaces/box.py
+-rw-r--r--   0        0        0      826 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/spaces/dict.py
+-rw-r--r--   0        0        0     1572 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/spaces/discrete.py
+-rw-r--r--   0        0        0     1471 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/spaces/from_gym.py
+-rw-r--r--   0        0        0     1280 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/spaces/multi_binary.py
+-rw-r--r--   0        0        0     1366 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/spaces/multi_discrete.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/spaces/tests/__init__.py
+-rw-r--r--   0        0        0     4874 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/spaces/tests/test_from_gym.py
+-rw-r--r--   0        0        0     3611 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/spaces/tests/test_spaces.py
+-rw-r--r--   0        0        0      782 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/spaces/tuple.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/tests/__init__.py
+-rw-r--r--   0        0        0     2819 2024-04-24 14:15:13.471367 rlberry-0.7.3/rlberry/tests/test_agent_extra.py
+-rw-r--r--   0        0        0     2033 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/tests/test_agents_base.py
+-rw-r--r--   0        0        0      820 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/tests/test_envs.py
+-rw-r--r--   0        0        0      321 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/tests/test_imports.py
+-rw-r--r--   0        0        0     3610 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/tests/test_rlberry_main_agents_and_env.py
+-rw-r--r--   0        0        0      302 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/types.py
+-rw-r--r--   0        0        0      182 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/utils/__init__.py
+-rw-r--r--   0        0        0     1177 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/utils/binsearch.py
+-rw-r--r--   0        0        0    24546 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/utils/check_agent.py
+-rw-r--r--   0        0        0     1490 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/utils/check_env.py
+-rw-r--r--   0        0        0    11348 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/utils/check_gym_env.py
+-rw-r--r--   0        0        0      199 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/utils/factory.py
+-rw-r--r--   0        0        0     3377 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/utils/logging.py
+-rw-r--r--   0        0        0     2206 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/utils/space_discretizer.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/utils/tests/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/utils/tests/test_binsearch.py
+-rw-r--r--   0        0        0     3233 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/utils/tests/test_check.py
+-rw-r--r--   0        0        0     1985 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/utils/tests/test_writer.py
+-rw-r--r--   0        0        0     2517 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/utils/torch.py
+-rw-r--r--   0        0        0    17459 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/utils/writers.py
+-rw-r--r--   0        0        0      195 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/__init__.py
+-rw-r--r--   0        0        0     1017 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/autoreset.py
+-rw-r--r--   0        0        0     1059 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/discrete2onehot.py
+-rw-r--r--   0        0        0     3455 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/discretize_state.py
+-rw-r--r--   0        0        0     1956 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/gym_utils.py
+-rw-r--r--   0        0        0     2154 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/rescale_reward.py
+-rw-r--r--   0        0        0      243 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/tests/__init__.py
+-rw-r--r--   0        0        0      411 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/tests/old_env/__init__.py
+-rw-r--r--   0        0        0    12214 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/tests/old_env/old_acrobot.py
+-rw-r--r--   0        0        0     5552 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/tests/old_env/old_apple_gold.py
+-rw-r--r--   0        0        0     6337 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/tests/old_env/old_ball2d.py
+-rw-r--r--   0        0        0     5806 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/tests/old_env/old_finite_mdp.py
+-rw-r--r--   0        0        0     4065 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/tests/old_env/old_four_room.py
+-rw-r--r--   0        0        0    16455 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/tests/old_env/old_gridworld.py
+-rw-r--r--   0        0        0     6159 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/tests/old_env/old_mountain_car.py
+-rw-r--r--   0        0        0    10752 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/tests/old_env/old_nroom.py
+-rw-r--r--   0        0        0    14902 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/tests/old_env/old_pball.py
+-rw-r--r--   0        0        0     3865 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/tests/old_env/old_pendulum.py
+-rw-r--r--   0        0        0     4487 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/tests/old_env/old_six_room.py
+-rw-r--r--   0        0        0     5670 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/tests/old_env/old_twinrooms.py
+-rw-r--r--   0        0        0      798 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/tests/test_basewrapper.py
+-rw-r--r--   0        0        0     7979 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/tests/test_common_wrappers.py
+-rw-r--r--   0        0        0     3001 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/tests/test_gym_space_conversion.py
+-rw-r--r--   0        0        0     4033 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/tests/test_wrapper_seeding.py
+-rw-r--r--   0        0        0     1126 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/tests/test_writer_utils.py
+-rw-r--r--   0        0        0     3636 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/uncertainty_estimator_wrapper.py
+-rw-r--r--   0        0        0     1465 2024-04-24 14:15:13.475367 rlberry-0.7.3/rlberry/wrappers/writer_utils.py
+-rw-r--r--   0        0        0     6378 1970-01-01 00:00:00.000000 rlberry-0.7.3/PKG-INFO
```

### Comparing `rlberry-0.7.2/LICENSE` & `rlberry-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/README.md` & `rlberry-0.7.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 that you can spend most of your time developing agents.
 `rlberry` also provides implementations of several RL agents, benchmark environments and many other useful tools.
 
 We provide you a number of tools to help you achieve **reproducibility**, **statistically comparisons** of RL agents, and **nice visualization**.
 
 ## Installation
 
-Install the latest version for a stable release.
+Install the latest (minimal) version for a stable release.
 
 ```bash
 pip install rlberry
 ```
 
 The documentation includes more [installation instructions](https://rlberry-py.github.io/rlberry/installation.html).
```

#### html2text {}

```diff
@@ -8,16 +8,16 @@
 in parallel, average and plot results, optimize hyperparameters, compare to
 baselines, create tricky environments etc etc! `rlberry` **is a Python library
 that makes your life easier** by doing all these things with a few lines of
 code, so that you can spend most of your time developing agents. `rlberry` also
 provides implementations of several RL agents, benchmark environments and many
 other useful tools. We provide you a number of tools to help you achieve
 **reproducibility**, **statistically comparisons** of RL agents, and **nice
-visualization**. ## Installation Install the latest version for a stable
-release. ```bash pip install rlberry ``` The documentation includes more
+visualization**. ## Installation Install the latest (minimal) version for a
+stable release. ```bash pip install rlberry ``` The documentation includes more
 [installation instructions](https://rlberry-py.github.io/rlberry/
 installation.html). ## Getting started In our [dev documentation](https://
 rlberry-py.github.io/rlberry/), you will find [quick starts](https://rlberry-
 py.github.io/rlberry/basics/quick_start_rl/quickstart.html#quick-start) to the
 library and a [user guide](https://rlberry-py.github.io/rlberry/
 user_guide.html) with a few tutorials on using rlberry, and some [examples]
 (https://rlberry-py.github.io/rlberry/auto_examples/index.html). See also the
```

### Comparing `rlberry-0.7.2/pyproject.toml` & `rlberry-0.7.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rlberry"
-version = "v0.7.2"
+version = "v0.7.3"
 description = "An easy-to-use reinforcement learning library for research and education"
 authors = ["Omar Darwiche Domingues, Yannis Flet-Berliac, Edouard Leurent, Pierre Menard, Xuedong Shang"]
 homepage = "https://github.com/rlberry-py"
 repository = "https://github.com/rlberry-py"
 readme = "README.md"
 license="LICENSE"
 classifiers=[
@@ -29,55 +29,53 @@
 pyyaml = "*"
 tqdm = "*"
 adastop = "*"
 moviepy = "*"
 pyopengl = "*"
 optuna ={version="*", optional=true}
 ffmpeg-python = {version="*", optional=true}
-pyvirtualdisplay = {version="*", optional=true}
 opencv-python = {version="*", optional=true}
 ale-py = {version="*", optional=true}
 stable-baselines3 = {version="*", optional=true}
 tensorboard = {version="*", optional=true}
 torch = {version=">=2.0.0, !=2.0.1, !=2.1.0", optional=true}
 pandas = "*"
-numba = "^0.58.1"
 scikit-fda = {version="^0.9", optional=true}
-scikit-learn = {version="1.2.2", optional=true}
 sphinx = {version="6.2.1", optional=true}
 sphinx-gallery = { version= "^0.14.0", optional=true}
 sphinx-math-dollar = {version="^1.2.1", optional=true}
+sphinxcontrib-video = {version="0.2.0", optional=true}
 numpydoc = {version="^1.6.0", optional=true}
 myst-parser = {version="^2.0.0", optional=true}
 
 
 ########### hack : some dependencies are not compatible #############
 # dependency of scikit-fda :
 fdasrsf = {version="2.5.2", optional=true}   # new version (2.5.8) : crash all our CI  (21-02-2024)
 multimethod = {version="1.10", optional=true}     # new version 1.11 : crash our tests in "rlberry/manager/tests/test_plot.py"  (21-02-2024)
 ###############################################################
 
 
 [tool.poetry.extras]
 torch = ["opencv-python", "ale-py", "stable-baselines3", "tensorboard", "torch"]
-extras = ["optuna", "numba", "ffmpeg-python", "pyvirtualdisplay", "scikit-fda", "scikit-learn"]
+extras = ["optuna", "ffmpeg-python", "scikit-fda"]
 doc = ["sphinx", "sphinx-gallery", "sphinx-math-dollar", "numpydoc", "myst-parser", "sphinxcontrib-video", "matplotlib"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 pytest-xprocess = "^0.23.0"
 codecov = "^2.1.13"
 black = "23.9.1"
 pre-commit = "^3.5.0"
 rlberry-research = {git = "https://github.com/rlberry-py/rlberry-research.git"}
 rlberry-scool = {git = "https://github.com/rlberry-py/rlberry-scool.git"}
-sphinxcontrib-video = {git = "https://github.com/sphinx-contrib/video", optional=true}
+sphinxcontrib-video = {version="0.2.0", optional=true}
 sphinx = {version="6.2.1", optional=true}
 sphinx-gallery = { version= "^0.14.0", optional=true}
 sphinx-math-dollar = {version="^1.2.1", optional=true}
 numpydoc = {version="^1.6.0", optional=true}
 myst-parser = {version="^2.0.0", optional=true}
```

### Comparing `rlberry-0.7.2/rlberry/agents/agent.py` & `rlberry-0.7.3/rlberry/agents/agent.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/agents/stable_baselines/stable_baselines.py` & `rlberry-0.7.3/rlberry/agents/stable_baselines/stable_baselines.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/agents/tests/test_replay.py` & `rlberry-0.7.3/rlberry/agents/tests/test_replay.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/agents/tests/test_stable_baselines.py` & `rlberry-0.7.3/rlberry/agents/tests/test_stable_baselines.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/agents/utils/replay.py` & `rlberry-0.7.3/rlberry/agents/utils/replay.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/agents/utils/replay_utils.py` & `rlberry-0.7.3/rlberry/agents/utils/replay_utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/envs/basewrapper.py` & `rlberry-0.7.3/rlberry/envs/basewrapper.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/envs/finite_mdp.py` & `rlberry-0.7.3/rlberry/envs/finite_mdp.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/envs/gym_make.py` & `rlberry-0.7.3/rlberry/envs/gym_make.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/envs/interface/model.py` & `rlberry-0.7.3/rlberry/envs/interface/model.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/envs/pipeline.py` & `rlberry-0.7.3/rlberry/envs/pipeline.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/envs/tests/test_env_seeding.py` & `rlberry-0.7.3/rlberry/envs/tests/test_env_seeding.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import pytest
 import rlberry.seeding as seeding
 
 from copy import deepcopy
 from rlberry_research.envs.classic_control import MountainCar, Acrobot, Pendulum
-from rlberry_research.envs.finite import Chain
-from rlberry_research.envs.finite import GridWorld
+from rlberry_scool.envs.finite import Chain
+from rlberry_scool.envs.finite import GridWorld
 from rlberry_research.envs.benchmarks.grid_exploration.four_room import FourRoom
 from rlberry_research.envs.benchmarks.grid_exploration.six_room import SixRoom
 from rlberry_research.envs.benchmarks.grid_exploration.apple_gold import AppleGold
 from rlberry_research.envs.benchmarks.ball_exploration import PBall2D, SimplePBallND
 
 classes = [
     MountainCar,
```

### Comparing `rlberry-0.7.2/rlberry/envs/tests/test_gym_env_seeding.py` & `rlberry-0.7.3/rlberry/envs/tests/test_gym_env_seeding.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/envs/tests/test_gym_make.py` & `rlberry-0.7.3/rlberry/envs/tests/test_gym_make.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/envs/utils.py` & `rlberry-0.7.3/rlberry/envs/utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/experiment/generator.py` & `rlberry-0.7.3/rlberry/experiment/generator.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/experiment/load_results.py` & `rlberry-0.7.3/rlberry/experiment/load_results.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/experiment/tests/test_experiment_generator.py` & `rlberry-0.7.3/rlberry/experiment/tests/test_experiment_generator.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/experiment/tests/test_load_results.py` & `rlberry-0.7.3/rlberry/experiment/tests/test_load_results.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/experiment/yaml_utils.py` & `rlberry-0.7.3/rlberry/experiment/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/manager/comparison.py` & `rlberry-0.7.3/rlberry/manager/comparison.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,14 +101,36 @@
             if self.is_finished:
                 break
 
         logger.info("Test finished")
         logger.info("Results are ")
         print(self.get_results())
 
+    def print_results(self):
+        """
+        Print the results of the test.
+        """
+        print("Number of scores used for each agent:")
+        for key in self.n_iters:
+            print(key + ":" + str(self.n_iters[key]))
+
+        print("")
+        print("Mean of scores of each agent:")
+        for key in self.eval_values:
+            print(key + ":" + str(np.mean(self.eval_values[key])))
+
+        print("")
+        print("Decision for each comparison:")
+        for c in self.comparisons:
+            print(
+                "{0} vs {1}".format(self.agent_names[c[0]], self.agent_names[c[1]])
+                + ":"
+                + str(self.decisions[str(c)])
+            )
+
     def _fit_evaluate(self, managers, eval_values, seeders):
         """
         fit rlberry agents.
         """
         if isinstance(self.n, int):
             self.n = np.array([self.n] * len(managers))
```

### Comparing `rlberry-0.7.2/rlberry/manager/evaluation.py` & `rlberry-0.7.3/rlberry/manager/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,15 +310,18 @@
 
 def _load_data(agent_folder, dir_name, id_agent):
     writer_data = {}
 
     agent_dir = Path(dir_name) / agent_folder
     # list all the fits of this experiment
     exp_files = (agent_dir / Path("agent_handlers")).iterdir()
-    nfit = len(list(exp_files))
+    nfit = len(
+        [1 for a_ in [str(e).split(".") for e in exp_files] if a_[-1] == "pickle"]
+    )
+    # nfit = len(list(exp_files))
     if nfit == 0:
         raise ValueError("Folders do not contain pickle files")
 
     if id_agent is not None:
         id_fits = [id_agent]
     else:
         id_fits = range(nfit)
```

### Comparing `rlberry-0.7.2/rlberry/manager/experiment_manager.py` & `rlberry-0.7.3/rlberry/manager/experiment_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -589,14 +589,15 @@
         >>> # evaluation_results will return 5 values (n_simulations=5) where each value is the Monte-Carlo
         >>> # evaluation over 10 simulations ((eval_kwargs["n_simulation"]))
         >>> evaluation_results = agent_manager.eval_agents(n_simulations=5, verbose=True)
         """
         eval_kwargs = eval_kwargs or self.eval_kwargs
         if not n_simulations:
             n_simulations = 2 * self.n_fit
+        logger.info(f"Computing {n_simulations} evaluations.")
         values = []
 
         if verbose:
             if logger.getEffectiveLevel() > 10:
                 previous_handlers = logger.handlers
                 ch = logging.StreamHandler()
                 ch.terminator = ""
@@ -616,19 +617,14 @@
                 logger.error(
                     "Calling eval() in an ExperimentManager instance contaning an empty AgentHandler."
                     " Returning []."
                 )
                 return []
             # Update eval_kwargs with n_simulations parameter
             eval_kwargs_with_n_simulations = eval_kwargs.copy()
-            if "n_simulations" in eval_kwargs:
-                # Issue a warning that n_simulations is overwritten
-                logger.info(
-                    "Warning: n_simulations parameter in eval_kwargs is being overwritten with 1."
-                )
             eval_kwargs_with_n_simulations["n_simulations"] = 1
             values.append(agent.eval(**eval_kwargs_with_n_simulations))
             if verbose:
                 if logger.getEffectiveLevel() <= 10:  # If debug
                     logger.debug(f"[eval]... simulation {ii + 1}/{n_simulations}")
                 else:
                     logger.info(".")
```

### Comparing `rlberry-0.7.2/rlberry/manager/multiple_managers.py` & `rlberry-0.7.3/rlberry/manager/multiple_managers.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/manager/plotting.py` & `rlberry-0.7.3/rlberry/manager/plotting.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/manager/tests/test_comparisons.py` & `rlberry-0.7.3/rlberry/manager/tests/test_comparisons.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,9 +135,10 @@
             "fit_budget": 5,
             "init_kwargs": {"eval_val": 10},
         },
     ]
 
     comparator = AdastopComparator(seed=42)
     comparator.compare(managers)
+    comparator.print_results()
     assert comparator.is_finished
     assert not ("equal" in comparator.decisions.values())
```

### Comparing `rlberry-0.7.2/rlberry/manager/tests/test_experiment_manager.py` & `rlberry-0.7.3/rlberry/manager/tests/test_experiment_manager.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/manager/tests/test_experiment_manager_seeding.py` & `rlberry-0.7.3/rlberry/manager/tests/test_experiment_manager_seeding.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/manager/tests/test_hyperparam_optim.py` & `rlberry-0.7.3/rlberry/manager/tests/test_hyperparam_optim.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/manager/tests/test_plot.py` & `rlberry-0.7.3/rlberry/manager/tests/test_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 from pathlib import Path
 import pandas as pd
 import sys
 import matplotlib.pyplot as plt
 
 from rlberry.wrappers import WriterWrapper
-from rlberry_research.envs import Chain
+from rlberry_scool.envs import Chain
 from rlberry.manager import plot_writer_data, ExperimentManager, read_writer_data
 from rlberry.manager.plotting import plot_smoothed_curves, plot_synchronized_curves
 from rlberry.agents import AgentWithSimplePolicy
 
 # np.random.seed(42)
```

### Comparing `rlberry-0.7.2/rlberry/manager/tests/test_shared_data.py` & `rlberry-0.7.3/rlberry/manager/tests/test_shared_data.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/metadata_utils.py` & `rlberry-0.7.3/rlberry/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/rendering/common_shapes.py` & `rlberry-0.7.3/rlberry/rendering/common_shapes.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/rendering/core.py` & `rlberry-0.7.3/rlberry/rendering/core.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/rendering/opengl_render2d.py` & `rlberry-0.7.3/rlberry/rendering/opengl_render2d.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/rendering/pygame_render2d.py` & `rlberry-0.7.3/rlberry/rendering/pygame_render2d.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/rendering/render_interface.py` & `rlberry-0.7.3/rlberry/rendering/render_interface.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/rendering/tests/test_rendering_interface.py` & `rlberry-0.7.3/rlberry/rendering/tests/test_rendering_interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import pytest
 import sys
 
-from pyvirtualdisplay import Display
 from rlberry_research.envs.classic_control import MountainCar
 from rlberry_research.envs.classic_control import Acrobot
 from rlberry_research.envs.classic_control import Pendulum
 from rlberry_scool.envs.finite import Chain
 from rlberry_scool.envs.finite import GridWorld
 from rlberry_scool.agents.dynprog import ValueIterationAgent
 from rlberry_research.envs.benchmarks.grid_exploration.four_room import FourRoom
@@ -16,19 +15,14 @@
 from rlberry_research.envs.benchmarks.generalization.twinrooms import TwinRooms
 from rlberry.rendering import RenderInterface
 from rlberry.rendering import RenderInterface2D
 from rlberry.envs import Wrapper
 
 import tempfile
 
-try:
-    display = Display(visible=0, size=(1400, 900))
-    display.start()
-except Exception:
-    pass
 
 classes = [
     Acrobot,
     Pendulum,
     MountainCar,
     GridWorld,
     Chain,
```

### Comparing `rlberry-0.7.2/rlberry/rendering/utils.py` & `rlberry-0.7.3/rlberry/rendering/utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/seeding/seeder.py` & `rlberry-0.7.3/rlberry/seeding/seeder.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/seeding/seeding.py` & `rlberry-0.7.3/rlberry/seeding/seeding.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/seeding/tests/test_seeding.py` & `rlberry-0.7.3/rlberry/seeding/tests/test_seeding.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/seeding/tests/test_threads.py` & `rlberry-0.7.3/rlberry/seeding/tests/test_threads.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/seeding/tests/test_threads_torch.py` & `rlberry-0.7.3/rlberry/seeding/tests/test_threads_torch.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/spaces/box.py` & `rlberry-0.7.3/rlberry/spaces/box.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/spaces/dict.py` & `rlberry-0.7.3/rlberry/spaces/dict.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/spaces/discrete.py` & `rlberry-0.7.3/rlberry/spaces/discrete.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/spaces/from_gym.py` & `rlberry-0.7.3/rlberry/spaces/from_gym.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/spaces/multi_binary.py` & `rlberry-0.7.3/rlberry/spaces/multi_binary.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/spaces/multi_discrete.py` & `rlberry-0.7.3/rlberry/spaces/multi_discrete.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/spaces/tests/test_from_gym.py` & `rlberry-0.7.3/rlberry/spaces/tests/test_from_gym.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/spaces/tests/test_spaces.py` & `rlberry-0.7.3/rlberry/spaces/tests/test_spaces.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/spaces/tuple.py` & `rlberry-0.7.3/rlberry/spaces/tuple.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/tests/test_agent_extra.py` & `rlberry-0.7.3/rlberry/tests/test_agent_extra.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/tests/test_agents_base.py` & `rlberry-0.7.3/rlberry/tests/test_agents_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 
 FINITE_MDP_AGENTS = [
     agents_scool.QLAgent,
     agents_scool.SARSAAgent,
     agents_scool.ValueIterationAgent,
     agents_scool.MBQVIAgent,
-    agents_research.UCBVIAgent,
+    agents_scool.UCBVIAgent,
     agents_research.OptQLAgent,
     agents_research.PSRLAgent,
     agents_research.RLSVIAgent,
     OneHotLSVI,
 ]
```

### Comparing `rlberry-0.7.2/rlberry/tests/test_envs.py` & `rlberry-0.7.3/rlberry/tests/test_envs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from rlberry.utils.check_env import check_env, check_rlberry_env
 from rlberry_research.envs import Acrobot
 from rlberry_research.envs.benchmarks.ball_exploration import PBall2D
 from rlberry_research.envs.benchmarks.generalization.twinrooms import TwinRooms
 from rlberry_research.envs.benchmarks.grid_exploration.apple_gold import AppleGold
 from rlberry_research.envs.benchmarks.grid_exploration.nroom import NRoom
 from rlberry_research.envs.classic_control import MountainCar, SpringCartPole
-from rlberry_research.envs.finite import Chain, GridWorld
+from rlberry_scool.envs.finite import Chain, GridWorld
 import pytest
 
 ALL_ENVS = [
     Acrobot,
     PBall2D,
     TwinRooms,
     AppleGold,
```

### Comparing `rlberry-0.7.2/rlberry/tests/test_rlberry_main_agents_and_env.py` & `rlberry-0.7.3/rlberry/tests/test_rlberry_main_agents_and_env.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/utils/binsearch.py` & `rlberry-0.7.3/rlberry/utils/binsearch.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/utils/check_agent.py` & `rlberry-0.7.3/rlberry/utils/check_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     ):  # If env param is a str, we use the corresponding "by default" env, and return it as tuple
         if env == "continuous_state":
             from rlberry_research.envs.benchmarks.ball_exploration import PBall2D
 
             env_ctor = PBall2D
             env_kwargs = {}
         elif env == "discrete_state":
-            from rlberry_research.envs import Chain
+            from rlberry_scool.envs import Chain
 
             env_ctor = Chain
             env_kwargs = {}
         elif env == "vectorized_env_continuous":
             env_ctor = gym_make
             env_kwargs = dict(id="CartPole-v1")
         elif env == "continuous_action":
@@ -498,15 +498,15 @@
         if tuple, env is the constructor and keywords of the env on which to test.
         if str in {"continuous_state", "discrete_state"}, we use a default Benchmark environment.
     init_kwargs : dict
         Arguments required by the agent's constructor.
 
     Examples
     --------
-    >>> from rlberry_research.agents import UCBVIAgent
+    >>> from rlberry_scool.agents import UCBVIAgent
     >>> from rlberry.utils import check_rl_agent
     >>> check_rl_agent(UCBVIAgent) # which does not return an error.
     """
     check_experiment_manager(
         agent, env, init_kwargs=init_kwargs
     )  # check manager compatible.
     check_agent_base(agent, env, init_kwargs=init_kwargs)  # check without manager
@@ -534,15 +534,15 @@
         if tuple, env is the constructor and keywords of the env on which to test.
         if str in {"continuous_state", "discrete_state"}, we use a default Benchmark environment.
     init_kwargs : dict
         Arguments required by the agent's constructor.
 
     Examples
     --------
-    >>> from rlberry.agents import UCBVIAgent
+    >>> from rlberry_scool.agents import UCBVIAgent
     >>> from rlberry.utils import check_rl_agent
     >>> check_rl_agent(UCBVIAgent) #
     """
     manager = _fit_experiment_manager(
         agent, env, init_kwargs=init_kwargs
     ).agent_handlers[0]
     try:
```

### Comparing `rlberry-0.7.2/rlberry/utils/check_env.py` & `rlberry-0.7.3/rlberry/utils/check_env.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/utils/check_gym_env.py` & `rlberry-0.7.3/rlberry/utils/check_gym_env.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/utils/logging.py` & `rlberry-0.7.3/rlberry/utils/logging.py`

 * *Files 8% similar despite different names*

```diff
@@ -106,9 +106,7 @@
         }
         config["loggers"]["rlberry_logger"]["handlers"].append(file_path.name)
 
     logging.config.dictConfig(config)
     gym.logger.set_level(
         logging.getLevelName(level) + 10
     )  # If info -> go to warning gym level. If debug, go to info.
-    numba_logger = logging.getLogger("numba")
-    numba_logger.setLevel(logging.WARNING)
```

### Comparing `rlberry-0.7.2/rlberry/utils/space_discretizer.py` & `rlberry-0.7.3/rlberry/utils/space_discretizer.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/utils/tests/test_binsearch.py` & `rlberry-0.7.3/rlberry/utils/tests/test_binsearch.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/utils/tests/test_check.py` & `rlberry-0.7.3/rlberry/utils/tests/test_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     check_rl_agent,
     _fit_experiment_manager,
     check_agents_almost_equal,
 )
 from rlberry.spaces import Box, Dict, Discrete
 import gymnasium as gym
 from rlberry_scool.agents import ValueIterationAgent
-from rlberry_research.agents import UCBVIAgent
+from rlberry_scool.agents import UCBVIAgent
 
 
 class ActionDictTestEnv(gym.Env):
     action_space = Dict({"position": Discrete(1), "velocity": Discrete(1)})
     observation_space = Box(low=-1.0, high=2.0, shape=(3,), dtype=np.float32)
 
     def step(self, action):
```

### Comparing `rlberry-0.7.2/rlberry/utils/tests/test_writer.py` & `rlberry-0.7.3/rlberry/utils/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/utils/torch.py` & `rlberry-0.7.3/rlberry/utils/torch.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/utils/writers.py` & `rlberry-0.7.3/rlberry/utils/writers.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/wrappers/autoreset.py` & `rlberry-0.7.3/rlberry/wrappers/autoreset.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/wrappers/discrete2onehot.py` & `rlberry-0.7.3/rlberry/wrappers/discrete2onehot.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/wrappers/discretize_state.py` & `rlberry-0.7.3/rlberry/wrappers/discretize_state.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/wrappers/gym_utils.py` & `rlberry-0.7.3/rlberry/wrappers/gym_utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/wrappers/rescale_reward.py` & `rlberry-0.7.3/rlberry/wrappers/rescale_reward.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/wrappers/tests/old_env/old_acrobot.py` & `rlberry-0.7.3/rlberry/wrappers/tests/old_env/old_acrobot.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/wrappers/tests/old_env/old_apple_gold.py` & `rlberry-0.7.3/rlberry/wrappers/tests/old_env/old_apple_gold.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/wrappers/tests/old_env/old_ball2d.py` & `rlberry-0.7.3/rlberry/wrappers/tests/old_env/old_ball2d.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/wrappers/tests/old_env/old_finite_mdp.py` & `rlberry-0.7.3/rlberry/wrappers/tests/old_env/old_finite_mdp.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/wrappers/tests/old_env/old_four_room.py` & `rlberry-0.7.3/rlberry/wrappers/tests/old_env/old_four_room.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/wrappers/tests/old_env/old_gridworld.py` & `rlberry-0.7.3/rlberry/wrappers/tests/old_env/old_gridworld.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/wrappers/tests/old_env/old_mountain_car.py` & `rlberry-0.7.3/rlberry/wrappers/tests/old_env/old_mountain_car.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/wrappers/tests/old_env/old_nroom.py` & `rlberry-0.7.3/rlberry/wrappers/tests/old_env/old_nroom.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/wrappers/tests/old_env/old_pball.py` & `rlberry-0.7.3/rlberry/wrappers/tests/old_env/old_pball.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/wrappers/tests/old_env/old_pendulum.py` & `rlberry-0.7.3/rlberry/wrappers/tests/old_env/old_pendulum.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/wrappers/tests/old_env/old_six_room.py` & `rlberry-0.7.3/rlberry/wrappers/tests/old_env/old_six_room.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/wrappers/tests/old_env/old_twinrooms.py` & `rlberry-0.7.3/rlberry/wrappers/tests/old_env/old_twinrooms.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/wrappers/tests/test_basewrapper.py` & `rlberry-0.7.3/rlberry/wrappers/tests/test_basewrapper.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/wrappers/tests/test_common_wrappers.py` & `rlberry-0.7.3/rlberry/wrappers/tests/test_common_wrappers.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/wrappers/tests/test_gym_space_conversion.py` & `rlberry-0.7.3/rlberry/wrappers/tests/test_gym_space_conversion.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/wrappers/tests/test_wrapper_seeding.py` & `rlberry-0.7.3/rlberry/wrappers/tests/test_wrapper_seeding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import pytest
 from rlberry.seeding import Seeder
 
 from copy import deepcopy
 from rlberry_research.envs.classic_control import MountainCar, Acrobot
-from rlberry_research.envs.finite import Chain
-from rlberry_research.envs.finite import GridWorld
+from rlberry_scool.envs.finite import Chain
+from rlberry_scool.envs.finite import GridWorld
 from rlberry_research.envs.benchmarks.ball_exploration import PBall2D, SimplePBallND
 from rlberry.envs import Wrapper
 from rlberry.wrappers import RescaleRewardWrapper
 
 _GYM_INSTALLED = True
 try:
     import gymnasium as gym
```

### Comparing `rlberry-0.7.2/rlberry/wrappers/tests/test_writer_utils.py` & `rlberry-0.7.3/rlberry/wrappers/tests/test_writer_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 
 from rlberry.wrappers import WriterWrapper
-from rlberry_research.envs import GridWorld
+from rlberry_scool.envs import GridWorld
 
-from rlberry_research.agents import UCBVIAgent
+from rlberry_scool.agents import UCBVIAgent
 
 
 @pytest.mark.parametrize("write_scalar", ["action", "reward", "action_and_reward"])
 def test_wrapper(write_scalar):
     """Test that the wrapper record data"""
 
     class MyAgent(UCBVIAgent):
```

### Comparing `rlberry-0.7.2/rlberry/wrappers/uncertainty_estimator_wrapper.py` & `rlberry-0.7.3/rlberry/wrappers/uncertainty_estimator_wrapper.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/rlberry/wrappers/writer_utils.py` & `rlberry-0.7.3/rlberry/wrappers/writer_utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.7.2/PKG-INFO` & `rlberry-0.7.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlberry
-Version: 0.7.2
+Version: 0.7.3
 Summary: An easy-to-use reinforcement learning library for research and education
 Home-page: https://github.com/rlberry-py
 License: LICENSE
 Author: Omar Darwiche Domingues, Yannis Flet-Berliac, Edouard Leurent, Pierre Menard, Xuedong Shang
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -29,29 +29,27 @@
 Requires-Dist: fdasrsf (==2.5.2)
 Requires-Dist: ffmpeg-python ; extra == "extras"
 Requires-Dist: gymnasium[accept-rom-license,atari] (>=0.29.1,<0.30.0)
 Requires-Dist: matplotlib ; extra == "doc"
 Requires-Dist: moviepy
 Requires-Dist: multimethod (==1.10)
 Requires-Dist: myst-parser (>=2.0.0,<3.0.0) ; extra == "doc"
-Requires-Dist: numba (>=0.58.1,<0.59.0) ; extra == "extras"
 Requires-Dist: numpydoc (>=1.6.0,<2.0.0) ; extra == "doc"
 Requires-Dist: opencv-python ; extra == "torch"
 Requires-Dist: optuna ; extra == "extras"
 Requires-Dist: pandas
 Requires-Dist: pygame-ce
 Requires-Dist: pyopengl
-Requires-Dist: pyvirtualdisplay ; extra == "extras"
 Requires-Dist: pyyaml
 Requires-Dist: scikit-fda (>=0.9,<0.10) ; extra == "extras"
-Requires-Dist: scikit-learn (==1.2.2) ; extra == "extras"
 Requires-Dist: scipy
 Requires-Dist: sphinx (==6.2.1) ; extra == "doc"
 Requires-Dist: sphinx-gallery (>=0.14.0,<0.15.0) ; extra == "doc"
 Requires-Dist: sphinx-math-dollar (>=1.2.1,<2.0.0) ; extra == "doc"
+Requires-Dist: sphinxcontrib-video (==0.2.0) ; extra == "doc"
 Requires-Dist: stable-baselines3 ; extra == "torch"
 Requires-Dist: tensorboard ; extra == "torch"
 Requires-Dist: torch (>=2.0.0,!=2.0.1,!=2.1.0) ; extra == "torch"
 Requires-Dist: tqdm
 Project-URL: Repository, https://github.com/rlberry-py
 Description-Content-Type: text/markdown
 
@@ -95,15 +93,15 @@
 that you can spend most of your time developing agents.
 `rlberry` also provides implementations of several RL agents, benchmark environments and many other useful tools.
 
 We provide you a number of tools to help you achieve **reproducibility**, **statistically comparisons** of RL agents, and **nice visualization**.
 
 ## Installation
 
-Install the latest version for a stable release.
+Install the latest (minimal) version for a stable release.
 
 ```bash
 pip install rlberry
 ```
 
 The documentation includes more [installation instructions](https://rlberry-py.github.io/rlberry/installation.html).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rlberry Version: 0.7.2 Summary: An easy-to-use
+Metadata-Version: 2.1 Name: rlberry Version: 0.7.3 Summary: An easy-to-use
 reinforcement learning library for research and education Home-page: https://
 github.com/rlberry-py License: LICENSE Author: Omar Darwiche Domingues, Yannis
 Flet-Berliac, Edouard Leurent, Pierre Menard, Xuedong Shang Requires-Python:
 >=3.9,<3.13 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Education Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License Classifier: License ::
 Other/Proprietary License Classifier: Operating System :: OS Independent
@@ -13,44 +13,42 @@
 Only Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Provides-Extra: doc Provides-Extra: extras Provides-Extra: torch Requires-Dist:
 adastop Requires-Dist: ale-py ; extra == "torch" Requires-Dist: dill Requires-
 Dist: docopt Requires-Dist: fdasrsf (==2.5.2) Requires-Dist: ffmpeg-python ;
 extra == "extras" Requires-Dist: gymnasium[accept-rom-license,atari]
 (>=0.29.1,<0.30.0) Requires-Dist: matplotlib ; extra == "doc" Requires-Dist:
 moviepy Requires-Dist: multimethod (==1.10) Requires-Dist: myst-parser
-(>=2.0.0,<3.0.0) ; extra == "doc" Requires-Dist: numba (>=0.58.1,<0.59.0) ;
-extra == "extras" Requires-Dist: numpydoc (>=1.6.0,<2.0.0) ; extra == "doc"
-Requires-Dist: opencv-python ; extra == "torch" Requires-Dist: optuna ; extra
-== "extras" Requires-Dist: pandas Requires-Dist: pygame-ce Requires-Dist:
-pyopengl Requires-Dist: pyvirtualdisplay ; extra == "extras" Requires-Dist:
-pyyaml Requires-Dist: scikit-fda (>=0.9,<0.10) ; extra == "extras" Requires-
-Dist: scikit-learn (==1.2.2) ; extra == "extras" Requires-Dist: scipy Requires-
-Dist: sphinx (==6.2.1) ; extra == "doc" Requires-Dist: sphinx-gallery
-(>=0.14.0,<0.15.0) ; extra == "doc" Requires-Dist: sphinx-math-dollar
-(>=1.2.1,<2.0.0) ; extra == "doc" Requires-Dist: stable-baselines3 ; extra ==
-"torch" Requires-Dist: tensorboard ; extra == "torch" Requires-Dist: torch
-(>=2.0.0,!=2.0.1,!=2.1.0) ; extra == "torch" Requires-Dist: tqdm Project-URL:
-Repository, https://github.com/rlberry-py Description-Content-Type: text/
-markdown
+(>=2.0.0,<3.0.0) ; extra == "doc" Requires-Dist: numpydoc (>=1.6.0,<2.0.0) ;
+extra == "doc" Requires-Dist: opencv-python ; extra == "torch" Requires-Dist:
+optuna ; extra == "extras" Requires-Dist: pandas Requires-Dist: pygame-ce
+Requires-Dist: pyopengl Requires-Dist: pyyaml Requires-Dist: scikit-fda
+(>=0.9,<0.10) ; extra == "extras" Requires-Dist: scipy Requires-Dist: sphinx
+(==6.2.1) ; extra == "doc" Requires-Dist: sphinx-gallery (>=0.14.0,<0.15.0) ;
+extra == "doc" Requires-Dist: sphinx-math-dollar (>=1.2.1,<2.0.0) ; extra ==
+"doc" Requires-Dist: sphinxcontrib-video (==0.2.0) ; extra == "doc" Requires-
+Dist: stable-baselines3 ; extra == "torch" Requires-Dist: tensorboard ; extra
+== "torch" Requires-Dist: torch (>=2.0.0,!=2.0.1,!=2.1.0) ; extra == "torch"
+Requires-Dist: tqdm Project-URL: Repository, https://github.com/rlberry-py
+Description-Content-Type: text/markdown
       [https://raw.githubusercontent.com/rlberry-py/rlberry/main/assets/
                                 logo_wide.svg]
           A Reinforcement Learning Library for Research and Education
                     _[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_c_o_n_t_r_i_b_u_t_o_r_s_]_[_c_o_d_e_c_o_v_]
 ===============================================================================
 ## What is `rlberry`? **Writing reinforcement learning algorithms is fun!**
 *But after the fun, we have lots of boring things to implement*: run our agents
 in parallel, average and plot results, optimize hyperparameters, compare to
 baselines, create tricky environments etc etc! `rlberry` **is a Python library
 that makes your life easier** by doing all these things with a few lines of
 code, so that you can spend most of your time developing agents. `rlberry` also
 provides implementations of several RL agents, benchmark environments and many
 other useful tools. We provide you a number of tools to help you achieve
 **reproducibility**, **statistically comparisons** of RL agents, and **nice
-visualization**. ## Installation Install the latest version for a stable
-release. ```bash pip install rlberry ``` The documentation includes more
+visualization**. ## Installation Install the latest (minimal) version for a
+stable release. ```bash pip install rlberry ``` The documentation includes more
 [installation instructions](https://rlberry-py.github.io/rlberry/
 installation.html). ## Getting started In our [dev documentation](https://
 rlberry-py.github.io/rlberry/), you will find [quick starts](https://rlberry-
 py.github.io/rlberry/basics/quick_start_rl/quickstart.html#quick-start) to the
 library and a [user guide](https://rlberry-py.github.io/rlberry/
 user_guide.html) with a few tutorials on using rlberry, and some [examples]
 (https://rlberry-py.github.io/rlberry/auto_examples/index.html). See also the
```

