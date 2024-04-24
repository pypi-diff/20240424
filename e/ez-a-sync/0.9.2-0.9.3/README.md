# Comparing `tmp/ez-a-sync-0.9.2.tar.gz` & `tmp/ez-a-sync-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez-a-sync-0.9.2.tar", last modified: Thu Oct  5 16:55:42 2023, max compression
+gzip compressed data, was "ez-a-sync-0.9.3.tar", last modified: Fri Oct  6 22:49:14 2023, max compression
```

## Comparing `ez-a-sync-0.9.2.tar` & `ez-a-sync-0.9.3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 16:55:42.665477 ez-a-sync-0.9.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 16:55:42.649476 ez-a-sync-0.9.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 16:55:42.653476 ez-a-sync-0.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      575 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-10-05 16:55:42.665477 ez-a-sync-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6139 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/TODO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 16:55:42.657476 ez-a-sync-0.9.2/a_sync/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/ENVIRONMENT_VARIABLES.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4982 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/_bound.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6133 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    24596 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/future.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/modified.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 16:55:42.657476 ez-a-sync-0.9.2/a_sync/modifiers/
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/modifiers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 16:55:42.657476 ez-a-sync-0.9.2/a_sync/modifiers/cache/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/modifiers/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/modifiers/cache/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/modifiers/limiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/modifiers/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/modifiers/semaphores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 16:55:42.661476 ez-a-sync-0.9.2/a_sync/primitives/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/primitives/_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/primitives/_loggable.py
--rw-r--r--   0 runner    (1001) docker     (127)     8732 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/primitives/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 16:55:42.661476 ez-a-sync-0.9.2/a_sync/primitives/locks/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/primitives/locks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/primitives/locks/counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/primitives/locks/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     8172 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/primitives/locks/prio_semaphore.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/primitives/locks/semaphore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/primitives/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/property.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      407 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 16:55:42.661476 ez-a-sync-0.9.2/a_sync/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      681 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/a_sync/utils/iterators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 16:55:42.661476 ez-a-sync-0.9.2/ez_a_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-10-05 16:55:42.000000 ez-a-sync-0.9.2/ez_a_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2023-10-05 16:55:42.000000 ez-a-sync-0.9.2/ez_a_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 16:55:42.000000 ez-a-sync-0.9.2/ez_a_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-10-05 16:55:42.000000 ez-a-sync-0.9.2/ez_a_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-05 16:55:42.000000 ez-a-sync-0.9.2/ez_a_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-05 16:55:42.665477 ez-a-sync-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      807 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 16:55:42.665477 ez-a-sync-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/tests/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5116 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/tests/test_future.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/tests/test_limiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2023-10-05 16:55:31.000000 ez-a-sync-0.9.2/tests/test_semaphore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 22:49:14.208183 ez-a-sync-0.9.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 22:49:14.192187 ez-a-sync-0.9.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 22:49:14.196186 ez-a-sync-0.9.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2023-10-06 22:49:14.208183 ez-a-sync-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6139 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/TODO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 22:49:14.200185 ez-a-sync-0.9.3/a_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/ENVIRONMENT_VARIABLES.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/_bound.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6133 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24596 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/future.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/modified.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 22:49:14.200185 ez-a-sync-0.9.3/a_sync/modifiers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/modifiers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 22:49:14.200185 ez-a-sync-0.9.3/a_sync/modifiers/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/modifiers/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/modifiers/cache/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/modifiers/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/modifiers/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/modifiers/semaphores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 22:49:14.200185 ez-a-sync-0.9.3/a_sync/primitives/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/primitives/_debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/primitives/_loggable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8732 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/primitives/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 22:49:14.204184 ez-a-sync-0.9.3/a_sync/primitives/locks/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/primitives/locks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/primitives/locks/counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/primitives/locks/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/primitives/locks/prio_semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/primitives/locks/semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/primitives/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 22:49:14.204184 ez-a-sync-0.9.3/a_sync/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/a_sync/utils/iterators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 22:49:14.204184 ez-a-sync-0.9.3/ez_a_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2023-10-06 22:49:14.000000 ez-a-sync-0.9.3/ez_a_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2023-10-06 22:49:14.000000 ez-a-sync-0.9.3/ez_a_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 22:49:14.000000 ez-a-sync-0.9.3/ez_a_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2023-10-06 22:49:14.000000 ez-a-sync-0.9.3/ez_a_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-06 22:49:14.000000 ez-a-sync-0.9.3/ez_a_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-06 22:49:14.208183 ez-a-sync-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 22:49:14.208183 ez-a-sync-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/tests/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5116 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/tests/test_future.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/tests/test_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2023-10-06 22:49:04.000000 ez-a-sync-0.9.3/tests/test_semaphore.py
```

### Comparing `ez-a-sync-0.9.2/.github/workflows/codeql.yaml` & `ez-a-sync-0.9.3/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/.github/workflows/mypy.yaml` & `ez-a-sync-0.9.3/.github/workflows/mypy.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/.github/workflows/pytest.yaml` & `ez-a-sync-0.9.3/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/.github/workflows/release.yaml` & `ez-a-sync-0.9.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/LICENSE.txt` & `ez-a-sync-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/README.md` & `ez-a-sync-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/__init__.py` & `ez-a-sync-0.9.3/a_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/_bound.py` & `ez-a-sync-0.9.3/a_sync/_bound.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/_flags.py` & `ez-a-sync-0.9.3/a_sync/_flags.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/_helpers.py` & `ez-a-sync-0.9.3/a_sync/_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             raise RuntimeError(f"{fn} must not have any arguments with the following names: {_flags.VIABLE_FLAGS}")
 
 def _await(awaitable: Awaitable[T]) -> T:
     try:
         return get_event_loop().run_until_complete(awaitable)
     except RuntimeError as e:
         if str(e) == "This event loop is already running":
-            raise SyncModeInAsyncContextError from None
+            raise SyncModeInAsyncContextError from e
         raise ASyncRuntimeError(e) from e
 
 def _asyncify(func: SyncFn[P, T], executor: Executor) -> CoroFn[P, T]:  # type: ignore [misc]
     @functools.wraps(func)
     async def _asyncify_wrap(*args: P.args, **kwargs: P.kwargs) -> T:
         return await asyncio.futures.wrap_future(
             executor.submit(func, *args, **kwargs),
```

### Comparing `ez-a-sync-0.9.2/a_sync/_kwargs.py` & `ez-a-sync-0.9.3/a_sync/_kwargs.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/_meta.py` & `ez-a-sync-0.9.3/a_sync/_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/_typing.py` & `ez-a-sync-0.9.3/a_sync/_typing.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/abstract.py` & `ez-a-sync-0.9.3/a_sync/abstract.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/base.py` & `ez-a-sync-0.9.3/a_sync/base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/config.py` & `ez-a-sync-0.9.3/a_sync/config.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/decorator.py` & `ez-a-sync-0.9.3/a_sync/decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/exceptions.py` & `ez-a-sync-0.9.3/a_sync/exceptions.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/future.py` & `ez-a-sync-0.9.3/a_sync/future.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/iter.py` & `ez-a-sync-0.9.3/a_sync/iter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/modified.py` & `ez-a-sync-0.9.3/a_sync/modified.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/modifiers/__init__.py` & `ez-a-sync-0.9.3/a_sync/modifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/modifiers/cache/__init__.py` & `ez-a-sync-0.9.3/a_sync/modifiers/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/modifiers/cache/memory.py` & `ez-a-sync-0.9.3/a_sync/modifiers/cache/memory.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/modifiers/limiter.py` & `ez-a-sync-0.9.3/a_sync/modifiers/limiter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/modifiers/manager.py` & `ez-a-sync-0.9.3/a_sync/modifiers/manager.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/modifiers/semaphores.py` & `ez-a-sync-0.9.3/a_sync/modifiers/semaphores.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/primitives/__init__.py` & `ez-a-sync-0.9.3/a_sync/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/primitives/_debug.py` & `ez-a-sync-0.9.3/a_sync/primitives/_debug.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/primitives/executor.py` & `ez-a-sync-0.9.3/a_sync/primitives/executor.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/primitives/locks/counter.py` & `ez-a-sync-0.9.3/a_sync/primitives/locks/counter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 from collections import defaultdict
+from time import time
 from typing import Iterable, Optional
 
 from a_sync.primitives._debug import _DebugDaemonMixin
 from a_sync.primitives.locks.event import Event
 
 
 class CounterLock(_DebugDaemonMixin):
@@ -45,17 +46,19 @@
             self._value = value
             ready = [self._events.pop(key) for key in list(self._events.keys()) if key <= self._value]
             for event in ready:
                 event.set()
         elif value < self._value:
             raise ValueError("You cannot decrease the value.")
     
-    def _debug_daemon(self) -> None:
+    async def _debug_daemon(self) -> None:
+        start = time()
         while self._events:
-            self.logger.debug(self)
+            self.logger.debug("%s is still locked after %sm", self, round(time() - start / 60, 2))
+            await asyncio.sleep(300)
 
 class CounterLockCluster:
     """
     An asyncio primitive that represents 2 or more CounterLock objects.
     
     `wait_for(i)` will block until the value of all CounterLock objects is >= i.
     """
```

### Comparing `ez-a-sync-0.9.2/a_sync/primitives/locks/event.py` & `ez-a-sync-0.9.3/a_sync/primitives/locks/event.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/primitives/locks/prio_semaphore.py` & `ez-a-sync-0.9.3/a_sync/primitives/locks/prio_semaphore.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             any(
                 cm._waiters and any(not w.cancelled() for w in cm._waiters) 
                 for cm in (self._context_managers.values() or ())
             )
         )
     
     def _count_waiters(self) -> Dict[PT, int]:
-        return {manager._priority: len(manager._waiters) for manager in sorted(self._waiters, key=lambda m: m._priority)}
+        return {manager._priority: len(manager.waiters) for manager in sorted(self._waiters, key=lambda m: m._priority)}
     
     def _wake_up_next(self) -> None:
         while self._waiters:
             manager = heapq.heappop(self._waiters)
             if len(manager) == 0:
                 # There are no more waiters, get rid of the empty manager
                 logger.debug("manager %s has no more waiters, popping from %s", manager._repr_no_parent_(), self)
```

### Comparing `ez-a-sync-0.9.2/a_sync/primitives/locks/semaphore.py` & `ez-a-sync-0.9.3/a_sync/primitives/locks/semaphore.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/primitives/queue.py` & `ez-a-sync-0.9.3/a_sync/primitives/queue.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/property.py` & `ez-a-sync-0.9.3/a_sync/property.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/utils/__init__.py` & `ez-a-sync-0.9.3/a_sync/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/a_sync/utils/iterators.py` & `ez-a-sync-0.9.3/a_sync/utils/iterators.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/ez_a_sync.egg-info/SOURCES.txt` & `ez-a-sync-0.9.3/ez_a_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/setup.py` & `ez-a-sync-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/tests/fixtures.py` & `ez-a-sync-0.9.3/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/tests/test_base.py` & `ez-a-sync-0.9.3/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/tests/test_cache.py` & `ez-a-sync-0.9.3/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/tests/test_decorator.py` & `ez-a-sync-0.9.3/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/tests/test_executor.py` & `ez-a-sync-0.9.3/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/tests/test_future.py` & `ez-a-sync-0.9.3/tests/test_future.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/tests/test_limiter.py` & `ez-a-sync-0.9.3/tests/test_limiter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/tests/test_meta.py` & `ez-a-sync-0.9.3/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.9.2/tests/test_semaphore.py` & `ez-a-sync-0.9.3/tests/test_semaphore.py`

 * *Files identical despite different names*

