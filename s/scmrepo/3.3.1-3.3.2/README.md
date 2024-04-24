# Comparing `tmp/scmrepo-3.3.1.tar.gz` & `tmp/scmrepo-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scmrepo-3.3.1.tar", last modified: Fri Mar 22 01:40:25 2024, max compression
+gzip compressed data, was "scmrepo-3.3.2.tar", last modified: Wed Apr 24 16:18:41 2024, max compression
```

## Comparing `scmrepo-3.3.1.tar` & `scmrepo-3.3.2.tar`

### file list

```diff
@@ -1,84 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:40:25.644775 scmrepo-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-22 01:40:03.000000 scmrepo-3.3.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-22 01:40:03.000000 scmrepo-3.3.1/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-22 01:40:03.000000 scmrepo-3.3.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:40:25.632775 scmrepo-3.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-22 01:40:03.000000 scmrepo-3.3.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:40:25.632775 scmrepo-3.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-22 01:40:03.000000 scmrepo-3.3.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-03-22 01:40:03.000000 scmrepo-3.3.1/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-22 01:40:03.000000 scmrepo-3.3.1/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-03-22 01:40:03.000000 scmrepo-3.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-22 01:40:03.000000 scmrepo-3.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-03-22 01:40:03.000000 scmrepo-3.3.1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-03-22 01:40:03.000000 scmrepo-3.3.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-03-22 01:40:03.000000 scmrepo-3.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-03-22 01:40:25.644775 scmrepo-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-03-22 01:40:03.000000 scmrepo-3.3.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-03-22 01:40:03.000000 scmrepo-3.3.1/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-03-22 01:40:03.000000 scmrepo-3.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 01:40:25.644775 scmrepo-3.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:40:25.628775 scmrepo-3.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:40:25.632775 scmrepo-3.3.1/src/scmrepo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:40:25.636775 scmrepo-3.3.1/src/scmrepo/git/
--rw-r--r--   0 runner    (1001) docker     (127)    17189 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/git/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:40:25.636775 scmrepo-3.3.1/src/scmrepo/git/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/git/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13560 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/git/backend/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:40:25.636775 scmrepo-3.3.1/src/scmrepo/git/backend/dulwich/
--rw-r--r--   0 runner    (1001) docker     (127)    34820 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/git/backend/dulwich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11562 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/git/backend/dulwich/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    25350 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/git/backend/gitpython.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:40:25.636775 scmrepo-3.3.1/src/scmrepo/git/backend/pygit2/
--rw-r--r--   0 runner    (1001) docker     (127)    37035 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/git/backend/pygit2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/git/backend/pygit2/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/git/backend/pygit2/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/git/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    20944 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/git/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:40:25.636775 scmrepo-3.3.1/src/scmrepo/git/lfs/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/git/lfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/git/lfs/client.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/git/lfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/git/lfs/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/git/lfs/object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/git/lfs/pointer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/git/lfs/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/git/lfs/smudge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/git/lfs/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/git/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/git/stash.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/noscm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-22 01:40:03.000000 scmrepo-3.3.1/src/scmrepo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:40:25.640775 scmrepo-3.3.1/src/scmrepo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-03-22 01:40:25.000000 scmrepo-3.3.1/src/scmrepo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-22 01:40:25.000000 scmrepo-3.3.1/src/scmrepo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 01:40:25.000000 scmrepo-3.3.1/src/scmrepo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-22 01:40:25.000000 scmrepo-3.3.1/src/scmrepo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-22 01:40:25.000000 scmrepo-3.3.1/src/scmrepo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:40:25.640775 scmrepo-3.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 01:40:03.000000 scmrepo-3.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-03-22 01:40:03.000000 scmrepo-3.3.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-22 01:40:03.000000 scmrepo-3.3.1/tests/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:40:25.640775 scmrepo-3.3.1/tests/git-init/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-22 01:40:03.000000 scmrepo-3.3.1/tests/git-init/git.sh
--rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-03-22 01:40:03.000000 scmrepo-3.3.1/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-03-22 01:40:03.000000 scmrepo-3.3.1/tests/test_dulwich.py
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-03-22 01:40:03.000000 scmrepo-3.3.1/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)    36426 2024-03-22 01:40:03.000000 scmrepo-3.3.1/tests/test_git.py
--rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-03-22 01:40:03.000000 scmrepo-3.3.1/tests/test_lfs.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-22 01:40:03.000000 scmrepo-3.3.1/tests/test_noscm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-03-22 01:40:03.000000 scmrepo-3.3.1/tests/test_pygit2.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-22 01:40:03.000000 scmrepo-3.3.1/tests/test_scmrepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-03-22 01:40:03.000000 scmrepo-3.3.1/tests/test_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-22 01:40:03.000000 scmrepo-3.3.1/tests/test_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-22 01:40:03.000000 scmrepo-3.3.1/tests/user.key
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-22 01:40:03.000000 scmrepo-3.3.1/tests/user.key.pub
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.733954 scmrepo-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 16:18:22.000000 scmrepo-3.3.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-24 16:18:22.000000 scmrepo-3.3.2/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-24 16:18:22.000000 scmrepo-3.3.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.721954 scmrepo-3.3.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-24 16:18:22.000000 scmrepo-3.3.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.721954 scmrepo-3.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-24 16:18:22.000000 scmrepo-3.3.2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-24 16:18:22.000000 scmrepo-3.3.2/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-24 16:18:22.000000 scmrepo-3.3.2/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-24 16:18:22.000000 scmrepo-3.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-24 16:18:22.000000 scmrepo-3.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-24 16:18:22.000000 scmrepo-3.3.2/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-24 16:18:22.000000 scmrepo-3.3.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-24 16:18:22.000000 scmrepo-3.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-24 16:18:41.733954 scmrepo-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-24 16:18:22.000000 scmrepo-3.3.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-24 16:18:22.000000 scmrepo-3.3.2/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-04-24 16:18:22.000000 scmrepo-3.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 16:18:41.733954 scmrepo-3.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.717954 scmrepo-3.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.721954 scmrepo-3.3.2/src/scmrepo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.725954 scmrepo-3.3.2/src/scmrepo/git/
+-rw-r--r--   0 runner    (1001) docker     (127)    17189 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.725954 scmrepo-3.3.2/src/scmrepo/git/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13560 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/backend/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.725954 scmrepo-3.3.2/src/scmrepo/git/backend/dulwich/
+-rw-r--r--   0 runner    (1001) docker     (127)    34820 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/backend/dulwich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11562 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/backend/dulwich/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25350 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/backend/gitpython.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.725954 scmrepo-3.3.2/src/scmrepo/git/backend/pygit2/
+-rw-r--r--   0 runner    (1001) docker     (127)    37035 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/backend/pygit2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/backend/pygit2/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/backend/pygit2/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20944 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.729954 scmrepo-3.3.2/src/scmrepo/git/lfs/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/lfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/lfs/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/lfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/lfs/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/lfs/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/lfs/pointer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/lfs/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/lfs/smudge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/lfs/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/git/stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/noscm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-24 16:18:22.000000 scmrepo-3.3.2/src/scmrepo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.733954 scmrepo-3.3.2/src/scmrepo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-24 16:18:41.000000 scmrepo-3.3.2/src/scmrepo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-24 16:18:41.000000 scmrepo-3.3.2/src/scmrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:18:41.000000 scmrepo-3.3.2/src/scmrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-24 16:18:41.000000 scmrepo-3.3.2/src/scmrepo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 16:18:41.000000 scmrepo-3.3.2/src/scmrepo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.729954 scmrepo-3.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.729954 scmrepo-3.3.2/tests/git-init/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/git-init/git.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/test_dulwich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36426 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/test_lfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/test_noscm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/test_pygit2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/test_scmrepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/test_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/user.key
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/user.key.pub
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:41.729954 scmrepo-3.3.2/tests/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/vendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-24 16:18:22.000000 scmrepo-3.3.2/tests/vendor/test_paramiko_vendor.py
```

### Comparing `scmrepo-3.3.1/.cruft.json` & `scmrepo-3.3.2/.cruft.json`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/.github/workflows/release.yaml` & `scmrepo-3.3.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/.github/workflows/tests.yaml` & `scmrepo-3.3.2/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/.gitignore` & `scmrepo-3.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/.pre-commit-config.yaml` & `scmrepo-3.3.2/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
       - id: check-yaml
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: ['--fix=lf']
       - id: sort-simple-yaml
       - id: trailing-whitespace
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: 'v0.3.3'
+    rev: 'v0.3.5'
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
       - id: ruff-format
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
     hooks:
```

### Comparing `scmrepo-3.3.1/CODE_OF_CONDUCT.rst` & `scmrepo-3.3.2/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/CONTRIBUTING.rst` & `scmrepo-3.3.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/LICENSE` & `scmrepo-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/PKG-INFO` & `scmrepo-3.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmrepo
-Version: 3.3.1
+Version: 3.3.2
 Summary: scmrepo
 Author-email: Iterative <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/scmrepo/issues
 Project-URL: Source, https://github.com/iterative/scmrepo
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: gitpython>3
-Requires-Dist: dulwich>=0.21.6
+Requires-Dist: dulwich>=0.22.1
 Requires-Dist: pygit2>=1.14.0
 Requires-Dist: pygtrie>=2.3.2
 Requires-Dist: fsspec[tqdm]>=2024.2.0
 Requires-Dist: pathspec>=0.9.0
 Requires-Dist: asyncssh<3,>=2.13.1
 Requires-Dist: funcy>=1.14
 Requires-Dist: aiohttp-retry>=2.5.0
```

### Comparing `scmrepo-3.3.1/README.rst` & `scmrepo-3.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/noxfile.py` & `scmrepo-3.3.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/pyproject.toml` & `scmrepo-3.3.2/pyproject.toml`

 * *Files identical despite different names*

```diff
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: 3.12",
     "Development Status :: 4 - Beta",
 ]
 requires-python = ">=3.9"
 dynamic = ["version"]
 dependencies = [
     "gitpython>3",
-    "dulwich>=0.21.6",
+    "dulwich>=0.22.1",
     "pygit2>=1.14.0",
     "pygtrie>=2.3.2",
     "fsspec[tqdm]>=2024.2.0",
     "pathspec>=0.9.0",
     "asyncssh>=2.13.1,<3",
     "funcy>=1.14",
     "aiohttp-retry>=2.5.0",
```

### Comparing `scmrepo-3.3.1/src/scmrepo/asyn.py` & `scmrepo-3.3.2/src/scmrepo/asyn.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/base.py` & `scmrepo-3.3.2/src/scmrepo/base.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/exceptions.py` & `scmrepo-3.3.2/src/scmrepo/exceptions.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/fs.py` & `scmrepo-3.3.2/src/scmrepo/fs.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/git/__init__.py` & `scmrepo-3.3.2/src/scmrepo/git/__init__.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/git/backend/base.py` & `scmrepo-3.3.2/src/scmrepo/git/backend/base.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/git/backend/dulwich/__init__.py` & `scmrepo-3.3.2/src/scmrepo/git/backend/dulwich/__init__.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py` & `scmrepo-3.3.2/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/git/backend/dulwich/client.py` & `scmrepo-3.3.2/src/scmrepo/git/backend/dulwich/client.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/git/backend/gitpython.py` & `scmrepo-3.3.2/src/scmrepo/git/backend/gitpython.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/git/backend/pygit2/__init__.py` & `scmrepo-3.3.2/src/scmrepo/git/backend/pygit2/__init__.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/git/backend/pygit2/callbacks.py` & `scmrepo-3.3.2/src/scmrepo/git/backend/pygit2/callbacks.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/git/backend/pygit2/filter.py` & `scmrepo-3.3.2/src/scmrepo/git/backend/pygit2/filter.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/git/config.py` & `scmrepo-3.3.2/src/scmrepo/git/config.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/git/credentials.py` & `scmrepo-3.3.2/src/scmrepo/git/credentials.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/git/lfs/client.py` & `scmrepo-3.3.2/src/scmrepo/git/lfs/client.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/git/lfs/fetch.py` & `scmrepo-3.3.2/src/scmrepo/git/lfs/fetch.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/git/lfs/pointer.py` & `scmrepo-3.3.2/src/scmrepo/git/lfs/pointer.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/git/lfs/progress.py` & `scmrepo-3.3.2/src/scmrepo/git/lfs/progress.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/git/lfs/smudge.py` & `scmrepo-3.3.2/src/scmrepo/git/lfs/smudge.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/git/lfs/storage.py` & `scmrepo-3.3.2/src/scmrepo/git/lfs/storage.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/git/objects.py` & `scmrepo-3.3.2/src/scmrepo/git/objects.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/git/stash.py` & `scmrepo-3.3.2/src/scmrepo/git/stash.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/progress.py` & `scmrepo-3.3.2/src/scmrepo/progress.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/urls.py` & `scmrepo-3.3.2/src/scmrepo/urls.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo/utils.py` & `scmrepo-3.3.2/src/scmrepo/utils.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/src/scmrepo.egg-info/PKG-INFO` & `scmrepo-3.3.2/src/scmrepo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmrepo
-Version: 3.3.1
+Version: 3.3.2
 Summary: scmrepo
 Author-email: Iterative <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/scmrepo/issues
 Project-URL: Source, https://github.com/iterative/scmrepo
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: gitpython>3
-Requires-Dist: dulwich>=0.21.6
+Requires-Dist: dulwich>=0.22.1
 Requires-Dist: pygit2>=1.14.0
 Requires-Dist: pygtrie>=2.3.2
 Requires-Dist: fsspec[tqdm]>=2024.2.0
 Requires-Dist: pathspec>=0.9.0
 Requires-Dist: asyncssh<3,>=2.13.1
 Requires-Dist: funcy>=1.14
 Requires-Dist: aiohttp-retry>=2.5.0
```

### Comparing `scmrepo-3.3.1/src/scmrepo.egg-info/SOURCES.txt` & `scmrepo-3.3.2/src/scmrepo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -62,8 +62,10 @@
 tests/test_noscm.py
 tests/test_pygit2.py
 tests/test_scmrepo.py
 tests/test_stash.py
 tests/test_urls.py
 tests/user.key
 tests/user.key.pub
-tests/git-init/git.sh
+tests/git-init/git.sh
+tests/vendor/__init__.py
+tests/vendor/test_paramiko_vendor.py
```

### Comparing `scmrepo-3.3.1/tests/conftest.py` & `scmrepo-3.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/tests/test_credentials.py` & `scmrepo-3.3.2/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/tests/test_dulwich.py` & `scmrepo-3.3.2/tests/test_dulwich.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,26 @@
 from io import StringIO
 from typing import Any
 from unittest.mock import AsyncMock
 
 import asyncssh
 import paramiko
 import pytest
-from dulwich.contrib.test_paramiko_vendor import CLIENT_KEY, PASSWORD, USER, Server
 from pytest_mock import MockerFixture
 from pytest_test_utils.waiters import wait_until
 
 from scmrepo.git.backend.dulwich.asyncssh_vendor import AsyncSSHVendor
 
+from .vendor.test_paramiko_vendor import (
+    CLIENT_KEY,
+    PASSWORD,
+    USER,
+    Server,
+)
+
 # pylint: disable=redefined-outer-name
 
 
 @pytest.fixture
 def ssh_conn(request: pytest.FixtureRequest) -> dict[str, Any]:
     server = Server([])
```

### Comparing `scmrepo-3.3.1/tests/test_fs.py` & `scmrepo-3.3.2/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/tests/test_git.py` & `scmrepo-3.3.2/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/tests/test_lfs.py` & `scmrepo-3.3.2/tests/test_lfs.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/tests/test_noscm.py` & `scmrepo-3.3.2/tests/test_noscm.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/tests/test_pygit2.py` & `scmrepo-3.3.2/tests/test_pygit2.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/tests/test_scmrepo.py` & `scmrepo-3.3.2/tests/test_scmrepo.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/tests/test_stash.py` & `scmrepo-3.3.2/tests/test_stash.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/tests/test_urls.py` & `scmrepo-3.3.2/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `scmrepo-3.3.1/tests/user.key` & `scmrepo-3.3.2/tests/user.key`

 * *Files identical despite different names*

