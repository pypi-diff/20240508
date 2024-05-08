# Comparing `tmp/craft_application-2.6.3.tar.gz` & `tmp/craft_application-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft_application-2.6.3.tar", last modified: Tue Apr 30 18:43:07 2024, max compression
+gzip compressed data, was "craft_application-2.7.0.tar", last modified: Wed May  8 18:41:26 2024, max compression
```

## Comparing `craft_application-2.6.3.tar` & `craft_application-2.7.0.tar`

### file list

```diff
@@ -1,217 +1,214 @@
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.111186 craft_application-2.6.3/
--rw-rw-r--   0 developer  (1000) developer  (1000)      723 2023-10-21 00:19:20.000000 craft_application-2.6.3/.editorconfig
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.091186 craft_application-2.6.3/.github/
--rw-rw-r--   0 developer  (1000) developer  (1000)      518 2024-02-13 19:35:41.000000 craft_application-2.6.3/.github/.jira_sync_config.yaml
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.091186 craft_application-2.6.3/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 developer  (1000) developer  (1000)     1386 2023-10-21 00:19:20.000000 craft_application-2.6.3/.github/ISSUE_TEMPLATE/bug.yaml
--rw-rw-r--   0 developer  (1000) developer  (1000)      389 2023-10-21 00:19:20.000000 craft_application-2.6.3/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 developer  (1000) developer  (1000)      788 2023-10-21 00:19:20.000000 craft_application-2.6.3/.github/ISSUE_TEMPLATE/task.yaml
--rw-rw-r--   0 developer  (1000) developer  (1000)      179 2023-10-21 00:19:20.000000 craft_application-2.6.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-rw-r--   0 developer  (1000) developer  (1000)      506 2023-10-21 00:19:20.000000 craft_application-2.6.3/.github/release-drafter.yaml
--rw-rw-r--   0 developer  (1000) developer  (1000)      506 2023-10-21 00:19:20.000000 craft_application-2.6.3/.github/release-drafter.yml
--rw-rw-r--   0 developer  (1000) developer  (1000)     4699 2024-03-26 14:14:40.000000 craft_application-2.6.3/.github/renovate.json5
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.091186 craft_application-2.6.3/.github/workflows/
--rw-rw-r--   0 developer  (1000) developer  (1000)      179 2023-10-21 00:19:20.000000 craft_application-2.6.3/.github/workflows/cla-check.yaml
--rw-rw-r--   0 developer  (1000) developer  (1000)      919 2024-01-26 19:28:17.000000 craft_application-2.6.3/.github/workflows/docs.yaml
--rw-rw-r--   0 developer  (1000) developer  (1000)      346 2024-02-09 15:30:38.000000 craft_application-2.6.3/.github/workflows/release-drafter.yaml
--rw-rw-r--   0 developer  (1000) developer  (1000)     4541 2024-02-22 14:28:03.000000 craft_application-2.6.3/.github/workflows/tests.yaml
--rw-rw-r--   0 developer  (1000) developer  (1000)     1949 2023-10-21 00:19:20.000000 craft_application-2.6.3/.gitignore
--rw-rw-r--   0 developer  (1000) developer  (1000)      921 2023-10-21 00:19:20.000000 craft_application-2.6.3/.pre-commit-config.yaml
--rw-rw-r--   0 developer  (1000) developer  (1000)      395 2023-11-02 19:27:48.000000 craft_application-2.6.3/.readthedocs.yaml
--rw-rw-r--   0 developer  (1000) developer  (1000)      188 2023-10-21 00:19:20.000000 craft_application-2.6.3/.yamllint.yaml
--rw-rw-r--   0 developer  (1000) developer  (1000)     4393 2024-03-11 15:45:17.000000 craft_application-2.6.3/HACKING.rst
--rw-rw-r--   0 developer  (1000) developer  (1000)     7652 2023-10-21 00:19:20.000000 craft_application-2.6.3/LICENSE
--rw-r--r--   0 developer  (1000) developer  (1000)     3310 2024-04-30 18:43:07.111186 craft_application-2.6.3/PKG-INFO
--rw-rw-r--   0 developer  (1000) developer  (1000)      552 2023-10-21 00:19:20.000000 craft_application-2.6.3/README.rst
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.091186 craft_application-2.6.3/craft_application/
--rw-rw-r--   0 developer  (1000) developer  (1000)     1522 2024-03-28 14:15:19.000000 craft_application-2.6.3/craft_application/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)      411 2024-04-30 18:43:06.000000 craft_application-2.6.3/craft_application/_version.py
--rw-rw-r--   0 developer  (1000) developer  (1000)    29819 2024-04-30 18:41:52.000000 craft_application-2.6.3/craft_application/application.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.091186 craft_application-2.6.3/craft_application/commands/
--rw-rw-r--   0 developer  (1000) developer  (1000)     1163 2023-11-28 20:45:58.000000 craft_application-2.6.3/craft_application/commands/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     7234 2024-03-26 14:14:40.000000 craft_application-2.6.3/craft_application/commands/base.py
--rw-rw-r--   0 developer  (1000) developer  (1000)    12723 2024-03-26 14:14:40.000000 craft_application-2.6.3/craft_application/commands/lifecycle.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1608 2023-10-21 00:19:20.000000 craft_application-2.6.3/craft_application/commands/other.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     7040 2024-04-29 20:16:59.000000 craft_application-2.6.3/craft_application/errors.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     4504 2024-04-30 13:24:23.000000 craft_application-2.6.3/craft_application/grammar.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.095186 craft_application-2.6.3/craft_application/launchpad/
--rw-rw-r--   0 developer  (1000) developer  (1000)     1135 2024-02-09 15:30:38.000000 craft_application-2.6.3/craft_application/launchpad/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1000 2024-02-09 15:30:38.000000 craft_application-2.6.3/craft_application/launchpad/errors.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     8564 2024-03-05 01:56:17.000000 craft_application-2.6.3/craft_application/launchpad/launchpad.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.095186 craft_application-2.6.3/craft_application/launchpad/models/
--rw-rw-r--   0 developer  (1000) developer  (1000)      621 2024-02-26 13:30:19.000000 craft_application-2.6.3/craft_application/launchpad/models/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     6820 2024-02-26 13:30:19.000000 craft_application-2.6.3/craft_application/launchpad/models/base.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     4927 2024-02-26 13:30:19.000000 craft_application-2.6.3/craft_application/launchpad/models/build.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     5292 2024-02-22 14:28:03.000000 craft_application-2.6.3/craft_application/launchpad/models/code.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     2236 2024-02-26 13:30:19.000000 craft_application-2.6.3/craft_application/launchpad/models/distro.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     3496 2024-04-09 13:20:54.000000 craft_application-2.6.3/craft_application/launchpad/models/project.py
--rw-rw-r--   0 developer  (1000) developer  (1000)    16303 2024-03-26 14:14:40.000000 craft_application-2.6.3/craft_application/launchpad/models/recipe.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     6039 2024-02-22 14:28:03.000000 craft_application-2.6.3/craft_application/launchpad/util.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.095186 craft_application-2.6.3/craft_application/misc/
--rw-rw-r--   0 developer  (1000) developer  (1000)     1637 2024-01-26 19:28:17.000000 craft_application-2.6.3/craft_application/misc/instance_bashrc
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.095186 craft_application-2.6.3/craft_application/models/
--rw-rw-r--   0 developer  (1000) developer  (1000)     1506 2024-04-30 13:24:23.000000 craft_application-2.6.3/craft_application/models/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     3725 2024-02-09 15:30:38.000000 craft_application-2.6.3/craft_application/models/base.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     2935 2024-03-26 14:14:40.000000 craft_application-2.6.3/craft_application/models/constraints.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     3823 2024-04-30 13:24:23.000000 craft_application-2.6.3/craft_application/models/grammar.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1175 2023-10-21 00:19:20.000000 craft_application-2.6.3/craft_application/models/metadata.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     4752 2024-04-29 20:16:59.000000 craft_application-2.6.3/craft_application/models/project.py
--rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-10-21 00:19:20.000000 craft_application-2.6.3/craft_application/py.typed
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.095186 craft_application-2.6.3/craft_application/remote/
--rw-rw-r--   0 developer  (1000) developer  (1000)     1337 2024-03-11 15:45:17.000000 craft_application-2.6.3/craft_application/remote/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     2329 2024-02-22 14:28:03.000000 craft_application-2.6.3/craft_application/remote/errors.py
--rw-rw-r--   0 developer  (1000) developer  (1000)    11974 2024-04-09 13:20:54.000000 craft_application-2.6.3/craft_application/remote/git.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     4206 2024-04-29 20:16:59.000000 craft_application-2.6.3/craft_application/remote/utils.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     2070 2024-02-09 15:30:38.000000 craft_application-2.6.3/craft_application/remote/worktree.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     6731 2024-02-22 14:28:03.000000 craft_application-2.6.3/craft_application/secrets.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.095186 craft_application-2.6.3/craft_application/services/
--rw-rw-r--   0 developer  (1000) developer  (1000)     1444 2024-02-09 15:30:38.000000 craft_application-2.6.3/craft_application/services/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     2106 2024-02-09 15:30:38.000000 craft_application-2.6.3/craft_application/services/base.py
--rw-rw-r--   0 developer  (1000) developer  (1000)    16505 2024-04-30 18:41:52.000000 craft_application-2.6.3/craft_application/services/lifecycle.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     3128 2024-03-26 14:14:40.000000 craft_application-2.6.3/craft_application/services/package.py
--rw-rw-r--   0 developer  (1000) developer  (1000)    12545 2024-04-29 20:16:59.000000 craft_application-2.6.3/craft_application/services/provider.py
--rw-rw-r--   0 developer  (1000) developer  (1000)    14846 2024-04-17 14:51:43.000000 craft_application-2.6.3/craft_application/services/remotebuild.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     4323 2024-02-09 15:30:38.000000 craft_application-2.6.3/craft_application/services/request.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     4273 2024-02-09 15:30:38.000000 craft_application-2.6.3/craft_application/services/service_factory.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.099186 craft_application-2.6.3/craft_application/util/
--rw-rw-r--   0 developer  (1000) developer  (1000)     1701 2024-04-24 12:55:03.000000 craft_application-2.6.3/craft_application/util/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     2465 2024-04-24 12:55:03.000000 craft_application-2.6.3/craft_application/util/callbacks.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     4170 2024-02-22 14:28:03.000000 craft_application-2.6.3/craft_application/util/error_formatting.py
--rw-rw-r--   0 developer  (1000) developer  (1000)      950 2023-11-28 20:45:58.000000 craft_application-2.6.3/craft_application/util/logging.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1470 2024-02-09 15:30:38.000000 craft_application-2.6.3/craft_application/util/paths.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     2494 2024-04-25 23:19:47.000000 craft_application-2.6.3/craft_application/util/platforms.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     2507 2024-04-29 12:34:28.000000 craft_application-2.6.3/craft_application/util/repositories.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     4110 2024-02-26 22:34:16.000000 craft_application-2.6.3/craft_application/util/snap_config.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     2241 2024-03-11 15:45:17.000000 craft_application-2.6.3/craft_application/util/string.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     4930 2024-03-26 14:14:40.000000 craft_application-2.6.3/craft_application/util/yaml.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.107186 craft_application-2.6.3/craft_application.egg-info/
--rw-r--r--   0 developer  (1000) developer  (1000)     3310 2024-04-30 18:43:07.000000 craft_application-2.6.3/craft_application.egg-info/PKG-INFO
--rw-rw-r--   0 developer  (1000) developer  (1000)     6060 2024-04-30 18:43:07.000000 craft_application-2.6.3/craft_application.egg-info/SOURCES.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)        1 2024-04-30 18:43:07.000000 craft_application-2.6.3/craft_application.egg-info/dependency_links.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)      871 2024-04-30 18:43:07.000000 craft_application-2.6.3/craft_application.egg-info/requires.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)       18 2024-04-30 18:43:07.000000 craft_application-2.6.3/craft_application.egg-info/top_level.txt
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.099186 craft_application-2.6.3/docs/
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.083186 craft_application-2.6.3/docs/_static/
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.099186 craft_application-2.6.3/docs/_static/css/
--rw-rw-r--   0 developer  (1000) developer  (1000)      481 2024-04-29 20:16:59.000000 craft_application-2.6.3/docs/_static/css/custom.css
--rw-rw-r--   0 developer  (1000) developer  (1000)     1684 2024-04-29 20:16:59.000000 craft_application-2.6.3/docs/conf.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.099186 craft_application-2.6.3/docs/explanation/
--rw-rw-r--   0 developer  (1000) developer  (1000)       72 2023-10-21 00:19:20.000000 craft_application-2.6.3/docs/explanation/index.rst
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.099186 craft_application-2.6.3/docs/howto/
--rw-rw-r--   0 developer  (1000) developer  (1000)       70 2023-10-21 00:19:20.000000 craft_application-2.6.3/docs/howto/index.rst
--rw-rw-r--   0 developer  (1000) developer  (1000)     1201 2023-10-21 00:19:20.000000 craft_application-2.6.3/docs/index.rst
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.099186 craft_application-2.6.3/docs/reference/
--rw-rw-r--   0 developer  (1000) developer  (1000)      142 2023-10-21 00:19:20.000000 craft_application-2.6.3/docs/reference/index.rst
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.099186 craft_application-2.6.3/docs/tutorials/
--rw-rw-r--   0 developer  (1000) developer  (1000)      238 2023-10-21 00:19:20.000000 craft_application-2.6.3/docs/tutorials/index.rst
--rw-rw-r--   0 developer  (1000) developer  (1000)    10638 2024-04-29 20:16:59.000000 craft_application-2.6.3/pyproject.toml
--rw-rw-r--   0 developer  (1000) developer  (1000)       38 2024-04-30 18:43:07.111186 craft_application-2.6.3/setup.cfg
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.099186 craft_application-2.6.3/tests/
--rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-10-21 00:19:20.000000 craft_application-2.6.3/tests/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     9416 2024-04-30 14:46:33.000000 craft_application-2.6.3/tests/conftest.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.099186 craft_application-2.6.3/tests/integration/
--rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-10-21 00:19:20.000000 craft_application-2.6.3/tests/integration/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     3149 2024-04-09 13:20:54.000000 craft_application-2.6.3/tests/integration/conftest.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.087185 craft_application-2.6.3/tests/integration/data/
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.099186 craft_application-2.6.3/tests/integration/data/build-secrets/
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.099186 craft_application-2.6.3/tests/integration/data/build-secrets/secret-source-folder/
--rw-rw-r--   0 developer  (1000) developer  (1000)       14 2023-11-02 19:27:48.000000 craft_application-2.6.3/tests/integration/data/build-secrets/secret-source-folder/source-file.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)      442 2024-04-29 20:16:59.000000 craft_application-2.6.3/tests/integration/data/build-secrets/testcraft.yaml
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.087185 craft_application-2.6.3/tests/integration/data/invalid_projects/
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.099186 craft_application-2.6.3/tests/integration/data/invalid_projects/build-error/
--rw-rw-r--   0 developer  (1000) developer  (1000)      177 2024-04-29 20:16:59.000000 craft_application-2.6.3/tests/integration/data/invalid_projects/build-error/testcraft.yaml
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.087185 craft_application-2.6.3/tests/integration/data/valid_projects/
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.099186 craft_application-2.6.3/tests/integration/data/valid_projects/adoption/
--rw-rw-r--   0 developer  (1000) developer  (1000)       26 2024-04-30 14:30:12.000000 craft_application-2.6.3/tests/integration/data/valid_projects/adoption/stderr
--rw-rw-r--   0 developer  (1000) developer  (1000)      209 2024-04-30 14:30:12.000000 craft_application-2.6.3/tests/integration/data/valid_projects/adoption/testcraft.yaml
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.099186 craft_application-2.6.3/tests/integration/data/valid_projects/basic/
--rw-rw-r--   0 developer  (1000) developer  (1000)       26 2024-04-30 14:30:07.000000 craft_application-2.6.3/tests/integration/data/valid_projects/basic/stderr
--rw-rw-r--   0 developer  (1000) developer  (1000)      114 2024-04-30 14:30:07.000000 craft_application-2.6.3/tests/integration/data/valid_projects/basic/testcraft.yaml
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.099186 craft_application-2.6.3/tests/integration/data/valid_projects/environment/
--rw-rw-r--   0 developer  (1000) developer  (1000)       26 2024-02-26 19:18:49.000000 craft_application-2.6.3/tests/integration/data/valid_projects/environment/stderr
--rw-rw-r--   0 developer  (1000) developer  (1000)      887 2024-04-30 18:41:52.000000 craft_application-2.6.3/tests/integration/data/valid_projects/environment/testcraft.yaml
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.099186 craft_application-2.6.3/tests/integration/data/valid_projects/grammar/
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.087185 craft_application-2.6.3/tests/integration/data/valid_projects/grammar/src/
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.099186 craft_application-2.6.3/tests/integration/data/valid_projects/grammar/src/on-amd64-to-amd64/
--rw-rw-r--   0 developer  (1000) developer  (1000)       18 2024-04-30 14:29:58.000000 craft_application-2.6.3/tests/integration/data/valid_projects/grammar/src/on-amd64-to-amd64/hello.txt
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.099186 craft_application-2.6.3/tests/integration/data/valid_projects/grammar/src/on-amd64-to-arm64/
--rw-rw-r--   0 developer  (1000) developer  (1000)       18 2024-04-30 14:29:58.000000 craft_application-2.6.3/tests/integration/data/valid_projects/grammar/src/on-amd64-to-arm64/hello.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)       26 2024-04-30 14:29:58.000000 craft_application-2.6.3/tests/integration/data/valid_projects/grammar/stderr
--rw-rw-r--   0 developer  (1000) developer  (1000)      521 2024-04-30 14:29:58.000000 craft_application-2.6.3/tests/integration/data/valid_projects/grammar/testcraft.yaml
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.099186 craft_application-2.6.3/tests/integration/launchpad/
--rw-rw-r--   0 developer  (1000) developer  (1000)        0 2024-02-09 15:30:38.000000 craft_application-2.6.3/tests/integration/launchpad/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1021 2024-02-22 14:28:03.000000 craft_application-2.6.3/tests/integration/launchpad/conftest.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1709 2024-04-23 21:07:18.000000 craft_application-2.6.3/tests/integration/launchpad/test_anonymous_access.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.099186 craft_application-2.6.3/tests/integration/services/
--rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-10-21 00:19:20.000000 craft_application-2.6.3/tests/integration/services/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     5475 2024-03-05 01:55:10.000000 craft_application-2.6.3/tests/integration/services/test_lifecycle.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     4287 2024-03-26 14:14:40.000000 craft_application-2.6.3/tests/integration/services/test_provider.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1886 2024-04-09 13:20:54.000000 craft_application-2.6.3/tests/integration/services/test_remotebuild.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     3445 2024-02-09 15:30:38.000000 craft_application-2.6.3/tests/integration/services/test_request.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1909 2024-03-05 01:55:10.000000 craft_application-2.6.3/tests/integration/services/test_service_factory.py
--rw-rw-r--   0 developer  (1000) developer  (1000)    14516 2024-04-30 18:41:52.000000 craft_application-2.6.3/tests/integration/test_application.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     2201 2023-10-21 00:19:20.000000 craft_application-2.6.3/tests/integration/test_version.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.103186 craft_application-2.6.3/tests/unit/
--rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-10-21 00:19:20.000000 craft_application-2.6.3/tests/unit/__init__.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.103186 craft_application-2.6.3/tests/unit/commands/
--rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-10-21 00:19:20.000000 craft_application-2.6.3/tests/unit/commands/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     6705 2024-04-29 20:07:13.000000 craft_application-2.6.3/tests/unit/commands/test_base.py
--rw-rw-r--   0 developer  (1000) developer  (1000)    17375 2024-03-26 14:14:40.000000 craft_application-2.6.3/tests/unit/commands/test_lifecycle.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1363 2023-10-21 00:19:20.000000 craft_application-2.6.3/tests/unit/commands/test_other.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1673 2024-04-23 21:58:47.000000 craft_application-2.6.3/tests/unit/conftest.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.103186 craft_application-2.6.3/tests/unit/launchpad/
--rw-rw-r--   0 developer  (1000) developer  (1000)        0 2024-02-09 15:30:38.000000 craft_application-2.6.3/tests/unit/launchpad/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1194 2024-02-22 14:28:03.000000 craft_application-2.6.3/tests/unit/launchpad/conftest.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.103186 craft_application-2.6.3/tests/unit/launchpad/models/
--rw-rw-r--   0 developer  (1000) developer  (1000)        0 2024-02-09 15:30:38.000000 craft_application-2.6.3/tests/unit/launchpad/models/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     5159 2024-02-22 14:28:03.000000 craft_application-2.6.3/tests/unit/launchpad/models/test_base.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     2562 2024-02-22 14:28:03.000000 craft_application-2.6.3/tests/unit/launchpad/models/test_code.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     9305 2024-03-26 14:14:40.000000 craft_application-2.6.3/tests/unit/launchpad/test_launchpad.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     3500 2024-03-11 15:45:17.000000 craft_application-2.6.3/tests/unit/launchpad/test_util.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.103186 craft_application-2.6.3/tests/unit/models/
--rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-10-21 00:19:20.000000 craft_application-2.6.3/tests/unit/models/__init__.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.103186 craft_application-2.6.3/tests/unit/models/project_models/
--rw-rw-r--   0 developer  (1000) developer  (1000)       68 2023-10-21 00:19:20.000000 craft_application-2.6.3/tests/unit/models/project_models/basic_project.yaml
--rw-rw-r--   0 developer  (1000) developer  (1000)      436 2024-04-29 20:16:59.000000 craft_application-2.6.3/tests/unit/models/project_models/full_project.yaml
--rw-rw-r--   0 developer  (1000) developer  (1000)       24 2023-10-21 00:19:20.000000 craft_application-2.6.3/tests/unit/models/project_models/invalid_project.yaml
--rw-rw-r--   0 developer  (1000) developer  (1000)     4489 2024-02-22 14:28:03.000000 craft_application-2.6.3/tests/unit/models/test_constraints.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1673 2024-04-30 13:24:23.000000 craft_application-2.6.3/tests/unit/models/test_grammar.py
--rw-rw-r--   0 developer  (1000) developer  (1000)    10302 2024-04-29 20:16:59.000000 craft_application-2.6.3/tests/unit/models/test_project.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.103186 craft_application-2.6.3/tests/unit/remote/
--rw-rw-r--   0 developer  (1000) developer  (1000)        0 2024-02-09 15:30:38.000000 craft_application-2.6.3/tests/unit/remote/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)      855 2024-02-09 15:30:38.000000 craft_application-2.6.3/tests/unit/remote/conftest.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     2116 2024-02-09 15:30:38.000000 craft_application-2.6.3/tests/unit/remote/test_errors.py
--rw-rw-r--   0 developer  (1000) developer  (1000)    18388 2024-03-26 14:14:40.000000 craft_application-2.6.3/tests/unit/remote/test_git.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     5855 2024-03-11 15:45:17.000000 craft_application-2.6.3/tests/unit/remote/test_utils.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     3034 2024-02-09 15:30:38.000000 craft_application-2.6.3/tests/unit/remote/test_worktree.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.107186 craft_application-2.6.3/tests/unit/services/
--rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-10-21 00:19:20.000000 craft_application-2.6.3/tests/unit/services/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     3946 2024-04-09 13:20:54.000000 craft_application-2.6.3/tests/unit/services/conftest.py
--rw-rw-r--   0 developer  (1000) developer  (1000)    21815 2024-04-30 18:41:52.000000 craft_application-2.6.3/tests/unit/services/test_lifecycle.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     3413 2024-03-11 15:45:17.000000 craft_application-2.6.3/tests/unit/services/test_package.py
--rw-rw-r--   0 developer  (1000) developer  (1000)    19346 2024-04-18 18:37:15.000000 craft_application-2.6.3/tests/unit/services/test_provider.py
--rw-rw-r--   0 developer  (1000) developer  (1000)    11829 2024-04-17 14:51:43.000000 craft_application-2.6.3/tests/unit/services/test_remotebuild.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     3867 2024-04-29 12:34:28.000000 craft_application-2.6.3/tests/unit/services/test_repositories.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     4000 2024-02-09 15:30:38.000000 craft_application-2.6.3/tests/unit/services/test_request.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     5005 2024-04-29 20:16:59.000000 craft_application-2.6.3/tests/unit/services/test_service_factory.py
--rw-rw-r--   0 developer  (1000) developer  (1000)    56026 2024-04-30 18:41:52.000000 craft_application-2.6.3/tests/unit/test_application.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     2968 2024-02-09 15:30:38.000000 craft_application-2.6.3/tests/unit/test_errors.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     7670 2024-02-22 14:28:03.000000 craft_application-2.6.3/tests/unit/test_grammar.py
--rw-rw-r--   0 developer  (1000) developer  (1000)       57 2023-10-21 00:19:20.000000 craft_application-2.6.3/tests/unit/test_nothing.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     5444 2023-11-02 19:27:48.000000 craft_application-2.6.3/tests/unit/test_secrets.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.107186 craft_application-2.6.3/tests/unit/util/
--rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-10-21 00:19:20.000000 craft_application-2.6.3/tests/unit/util/__init__.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.107186 craft_application-2.6.3/tests/unit/util/invalid_yaml/
--rw-rw-r--   0 developer  (1000) developer  (1000)      156 2023-10-21 00:19:20.000000 craft_application-2.6.3/tests/unit/util/invalid_yaml/_README
--rw-rw-r--   0 developer  (1000) developer  (1000)       46 2023-10-21 00:19:20.000000 craft_application-2.6.3/tests/unit/util/invalid_yaml/duplicate_second_level.yaml-invalid
--rw-rw-r--   0 developer  (1000) developer  (1000)       40 2023-10-21 00:19:20.000000 craft_application-2.6.3/tests/unit/util/invalid_yaml/duplicate_top_level.yaml-invalid
--rw-rw-r--   0 developer  (1000) developer  (1000)       30 2024-04-29 20:16:59.000000 craft_application-2.6.3/tests/unit/util/invalid_yaml/unhashable.yaml-invalid
--rw-rw-r--   0 developer  (1000) developer  (1000)     3189 2024-01-26 19:28:17.000000 craft_application-2.6.3/tests/unit/util/test_error_formatting.py
--rw-rw-r--   0 developer  (1000) developer  (1000)      603 2023-11-28 20:45:58.000000 craft_application-2.6.3/tests/unit/util/test_logging.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1573 2024-02-09 15:30:38.000000 craft_application-2.6.3/tests/unit/util/test_paths.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     5221 2024-02-26 19:18:49.000000 craft_application-2.6.3/tests/unit/util/test_snap_config.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     3383 2024-03-11 15:45:17.000000 craft_application-2.6.3/tests/unit/util/test_string.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     2992 2024-03-26 14:14:40.000000 craft_application-2.6.3/tests/unit/util/test_yaml.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-04-30 18:43:07.107186 craft_application-2.6.3/tests/unit/util/valid_yaml/
--rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-10-21 00:19:20.000000 craft_application-2.6.3/tests/unit/util/valid_yaml/empty.yaml
--rw-rw-r--   0 developer  (1000) developer  (1000)     4900 2024-04-29 20:16:59.000000 craft_application-2.6.3/tox.ini
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.223203 craft_application-2.7.0/
+-rw-rw-r--   0 developer  (1000) developer  (1000)      723 2023-10-21 00:19:20.000000 craft_application-2.7.0/.editorconfig
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.203203 craft_application-2.7.0/.github/
+-rw-rw-r--   0 developer  (1000) developer  (1000)      518 2024-02-13 19:35:41.000000 craft_application-2.7.0/.github/.jira_sync_config.yaml
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.203203 craft_application-2.7.0/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1386 2023-10-21 00:19:20.000000 craft_application-2.7.0/.github/ISSUE_TEMPLATE/bug.yaml
+-rw-rw-r--   0 developer  (1000) developer  (1000)      389 2023-10-21 00:19:20.000000 craft_application-2.7.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 developer  (1000) developer  (1000)      788 2023-10-21 00:19:20.000000 craft_application-2.7.0/.github/ISSUE_TEMPLATE/task.yaml
+-rw-rw-r--   0 developer  (1000) developer  (1000)      179 2023-10-21 00:19:20.000000 craft_application-2.7.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-rw-r--   0 developer  (1000) developer  (1000)      506 2023-10-21 00:19:20.000000 craft_application-2.7.0/.github/release-drafter.yaml
+-rw-rw-r--   0 developer  (1000) developer  (1000)      506 2023-10-21 00:19:20.000000 craft_application-2.7.0/.github/release-drafter.yml
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4699 2024-03-26 14:14:40.000000 craft_application-2.7.0/.github/renovate.json5
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.203203 craft_application-2.7.0/.github/workflows/
+-rw-rw-r--   0 developer  (1000) developer  (1000)      179 2023-10-21 00:19:20.000000 craft_application-2.7.0/.github/workflows/cla-check.yaml
+-rw-rw-r--   0 developer  (1000) developer  (1000)      919 2024-01-26 19:28:17.000000 craft_application-2.7.0/.github/workflows/docs.yaml
+-rw-rw-r--   0 developer  (1000) developer  (1000)      346 2024-02-09 15:30:38.000000 craft_application-2.7.0/.github/workflows/release-drafter.yaml
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4541 2024-02-22 14:28:03.000000 craft_application-2.7.0/.github/workflows/tests.yaml
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1949 2023-10-21 00:19:20.000000 craft_application-2.7.0/.gitignore
+-rw-rw-r--   0 developer  (1000) developer  (1000)      921 2023-10-21 00:19:20.000000 craft_application-2.7.0/.pre-commit-config.yaml
+-rw-rw-r--   0 developer  (1000) developer  (1000)      395 2023-11-02 19:27:48.000000 craft_application-2.7.0/.readthedocs.yaml
+-rw-rw-r--   0 developer  (1000) developer  (1000)      188 2023-10-21 00:19:20.000000 craft_application-2.7.0/.yamllint.yaml
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4393 2024-03-11 15:45:17.000000 craft_application-2.7.0/HACKING.rst
+-rw-rw-r--   0 developer  (1000) developer  (1000)     7652 2023-10-21 00:19:20.000000 craft_application-2.7.0/LICENSE
+-rw-r--r--   0 developer  (1000) developer  (1000)     3046 2024-05-08 18:41:26.223203 craft_application-2.7.0/PKG-INFO
+-rw-rw-r--   0 developer  (1000) developer  (1000)      552 2023-10-21 00:19:20.000000 craft_application-2.7.0/README.rst
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.203203 craft_application-2.7.0/craft_application/
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1522 2024-03-28 14:15:19.000000 craft_application-2.7.0/craft_application/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)      411 2024-05-08 18:41:26.000000 craft_application-2.7.0/craft_application/_version.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)    29839 2024-05-08 18:34:14.000000 craft_application-2.7.0/craft_application/application.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.207203 craft_application-2.7.0/craft_application/commands/
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1218 2024-05-08 18:34:14.000000 craft_application-2.7.0/craft_application/commands/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     7734 2024-05-08 18:34:14.000000 craft_application-2.7.0/craft_application/commands/base.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)    14182 2024-05-08 18:34:14.000000 craft_application-2.7.0/craft_application/commands/lifecycle.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1608 2023-10-21 00:19:20.000000 craft_application-2.7.0/craft_application/commands/other.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     7040 2024-05-07 21:06:46.000000 craft_application-2.7.0/craft_application/errors.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4504 2024-04-30 19:53:17.000000 craft_application-2.7.0/craft_application/grammar.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.207203 craft_application-2.7.0/craft_application/launchpad/
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1135 2024-02-09 15:30:38.000000 craft_application-2.7.0/craft_application/launchpad/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1000 2024-02-09 15:30:38.000000 craft_application-2.7.0/craft_application/launchpad/errors.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     8564 2024-05-01 17:00:00.000000 craft_application-2.7.0/craft_application/launchpad/launchpad.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.207203 craft_application-2.7.0/craft_application/launchpad/models/
+-rw-rw-r--   0 developer  (1000) developer  (1000)      621 2024-02-26 13:30:19.000000 craft_application-2.7.0/craft_application/launchpad/models/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     6820 2024-02-26 13:30:19.000000 craft_application-2.7.0/craft_application/launchpad/models/base.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4927 2024-02-26 13:30:19.000000 craft_application-2.7.0/craft_application/launchpad/models/build.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     5292 2024-02-22 14:28:03.000000 craft_application-2.7.0/craft_application/launchpad/models/code.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     2236 2024-02-26 13:30:19.000000 craft_application-2.7.0/craft_application/launchpad/models/distro.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     3496 2024-04-09 13:20:54.000000 craft_application-2.7.0/craft_application/launchpad/models/project.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)    16303 2024-03-26 14:14:40.000000 craft_application-2.7.0/craft_application/launchpad/models/recipe.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     6039 2024-02-22 14:28:03.000000 craft_application-2.7.0/craft_application/launchpad/util.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.207203 craft_application-2.7.0/craft_application/misc/
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1637 2024-01-26 19:28:17.000000 craft_application-2.7.0/craft_application/misc/instance_bashrc
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.207203 craft_application-2.7.0/craft_application/models/
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1624 2024-04-30 19:53:17.000000 craft_application-2.7.0/craft_application/models/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     3725 2024-02-09 15:30:38.000000 craft_application-2.7.0/craft_application/models/base.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     2935 2024-03-26 14:14:40.000000 craft_application-2.7.0/craft_application/models/constraints.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     3823 2024-04-30 19:53:17.000000 craft_application-2.7.0/craft_application/models/grammar.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1175 2023-10-21 00:19:20.000000 craft_application-2.7.0/craft_application/models/metadata.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     7862 2024-04-30 18:45:16.000000 craft_application-2.7.0/craft_application/models/project.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-10-21 00:19:20.000000 craft_application-2.7.0/craft_application/py.typed
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.207203 craft_application-2.7.0/craft_application/remote/
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1337 2024-03-11 15:45:17.000000 craft_application-2.7.0/craft_application/remote/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     2329 2024-02-22 14:28:03.000000 craft_application-2.7.0/craft_application/remote/errors.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)    11974 2024-04-09 13:20:54.000000 craft_application-2.7.0/craft_application/remote/git.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4207 2024-04-30 18:45:16.000000 craft_application-2.7.0/craft_application/remote/utils.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     2070 2024-02-09 15:30:38.000000 craft_application-2.7.0/craft_application/remote/worktree.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     6731 2024-02-22 14:28:03.000000 craft_application-2.7.0/craft_application/secrets.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.207203 craft_application-2.7.0/craft_application/services/
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1444 2024-02-09 15:30:38.000000 craft_application-2.7.0/craft_application/services/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     2106 2024-02-09 15:30:38.000000 craft_application-2.7.0/craft_application/services/base.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)    16505 2024-05-07 20:58:17.000000 craft_application-2.7.0/craft_application/services/lifecycle.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     3128 2024-03-26 14:14:40.000000 craft_application-2.7.0/craft_application/services/package.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)    12521 2024-04-30 18:45:16.000000 craft_application-2.7.0/craft_application/services/provider.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)    14846 2024-05-01 16:59:44.000000 craft_application-2.7.0/craft_application/services/remotebuild.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4323 2024-02-09 15:30:38.000000 craft_application-2.7.0/craft_application/services/request.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4273 2024-02-09 15:30:38.000000 craft_application-2.7.0/craft_application/services/service_factory.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.211203 craft_application-2.7.0/craft_application/util/
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1701 2024-04-24 12:55:03.000000 craft_application-2.7.0/craft_application/util/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     2465 2024-04-24 12:55:03.000000 craft_application-2.7.0/craft_application/util/callbacks.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4170 2024-02-22 14:28:03.000000 craft_application-2.7.0/craft_application/util/error_formatting.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)      950 2023-11-28 20:45:58.000000 craft_application-2.7.0/craft_application/util/logging.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1470 2024-02-09 15:30:38.000000 craft_application-2.7.0/craft_application/util/paths.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     2494 2024-04-25 23:19:47.000000 craft_application-2.7.0/craft_application/util/platforms.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     2507 2024-04-29 12:34:28.000000 craft_application-2.7.0/craft_application/util/repositories.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4110 2024-02-26 22:34:16.000000 craft_application-2.7.0/craft_application/util/snap_config.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     2241 2024-03-11 15:45:17.000000 craft_application-2.7.0/craft_application/util/string.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4930 2024-03-26 14:14:40.000000 craft_application-2.7.0/craft_application/util/yaml.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.223203 craft_application-2.7.0/craft_application.egg-info/
+-rw-r--r--   0 developer  (1000) developer  (1000)     3046 2024-05-08 18:41:26.000000 craft_application-2.7.0/craft_application.egg-info/PKG-INFO
+-rw-rw-r--   0 developer  (1000) developer  (1000)     6032 2024-05-08 18:41:26.000000 craft_application-2.7.0/craft_application.egg-info/SOURCES.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)        1 2024-05-08 18:41:26.000000 craft_application-2.7.0/craft_application.egg-info/dependency_links.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)      767 2024-05-08 18:41:26.000000 craft_application-2.7.0/craft_application.egg-info/requires.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)       18 2024-05-08 18:41:26.000000 craft_application-2.7.0/craft_application.egg-info/top_level.txt
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.211203 craft_application-2.7.0/docs/
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1330 2024-04-30 18:45:16.000000 craft_application-2.7.0/docs/conf.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.211203 craft_application-2.7.0/docs/explanation/
+-rw-rw-r--   0 developer  (1000) developer  (1000)       72 2023-10-21 00:19:20.000000 craft_application-2.7.0/docs/explanation/index.rst
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.211203 craft_application-2.7.0/docs/howto/
+-rw-rw-r--   0 developer  (1000) developer  (1000)       70 2023-10-21 00:19:20.000000 craft_application-2.7.0/docs/howto/index.rst
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1201 2023-10-21 00:19:20.000000 craft_application-2.7.0/docs/index.rst
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.211203 craft_application-2.7.0/docs/reference/
+-rw-rw-r--   0 developer  (1000) developer  (1000)      142 2023-10-21 00:19:20.000000 craft_application-2.7.0/docs/reference/index.rst
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.211203 craft_application-2.7.0/docs/tutorials/
+-rw-rw-r--   0 developer  (1000) developer  (1000)      238 2023-10-21 00:19:20.000000 craft_application-2.7.0/docs/tutorials/index.rst
+-rw-rw-r--   0 developer  (1000) developer  (1000)    10499 2024-04-30 18:45:16.000000 craft_application-2.7.0/pyproject.toml
+-rw-rw-r--   0 developer  (1000) developer  (1000)       38 2024-05-08 18:41:26.223203 craft_application-2.7.0/setup.cfg
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.211203 craft_application-2.7.0/tests/
+-rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-10-21 00:19:20.000000 craft_application-2.7.0/tests/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     9427 2024-04-30 18:45:16.000000 craft_application-2.7.0/tests/conftest.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.211203 craft_application-2.7.0/tests/integration/
+-rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-10-21 00:19:20.000000 craft_application-2.7.0/tests/integration/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     3149 2024-04-09 13:20:54.000000 craft_application-2.7.0/tests/integration/conftest.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.199203 craft_application-2.7.0/tests/integration/data/
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.211203 craft_application-2.7.0/tests/integration/data/build-secrets/
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.211203 craft_application-2.7.0/tests/integration/data/build-secrets/secret-source-folder/
+-rw-rw-r--   0 developer  (1000) developer  (1000)       14 2023-11-02 19:27:48.000000 craft_application-2.7.0/tests/integration/data/build-secrets/secret-source-folder/source-file.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)      437 2024-04-30 18:45:16.000000 craft_application-2.7.0/tests/integration/data/build-secrets/testcraft.yaml
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.199203 craft_application-2.7.0/tests/integration/data/invalid_projects/
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.211203 craft_application-2.7.0/tests/integration/data/invalid_projects/build-error/
+-rw-rw-r--   0 developer  (1000) developer  (1000)      172 2024-04-30 18:45:16.000000 craft_application-2.7.0/tests/integration/data/invalid_projects/build-error/testcraft.yaml
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.199203 craft_application-2.7.0/tests/integration/data/valid_projects/
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.211203 craft_application-2.7.0/tests/integration/data/valid_projects/adoption/
+-rw-rw-r--   0 developer  (1000) developer  (1000)       26 2024-04-30 14:30:12.000000 craft_application-2.7.0/tests/integration/data/valid_projects/adoption/stderr
+-rw-rw-r--   0 developer  (1000) developer  (1000)      204 2024-04-30 18:45:16.000000 craft_application-2.7.0/tests/integration/data/valid_projects/adoption/testcraft.yaml
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.211203 craft_application-2.7.0/tests/integration/data/valid_projects/basic/
+-rw-rw-r--   0 developer  (1000) developer  (1000)       26 2024-04-30 14:30:07.000000 craft_application-2.7.0/tests/integration/data/valid_projects/basic/stderr
+-rw-rw-r--   0 developer  (1000) developer  (1000)      109 2024-04-30 18:45:16.000000 craft_application-2.7.0/tests/integration/data/valid_projects/basic/testcraft.yaml
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.211203 craft_application-2.7.0/tests/integration/data/valid_projects/environment/
+-rw-rw-r--   0 developer  (1000) developer  (1000)       26 2024-02-26 19:18:49.000000 craft_application-2.7.0/tests/integration/data/valid_projects/environment/stderr
+-rw-rw-r--   0 developer  (1000) developer  (1000)      882 2024-05-07 21:06:46.000000 craft_application-2.7.0/tests/integration/data/valid_projects/environment/testcraft.yaml
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.211203 craft_application-2.7.0/tests/integration/data/valid_projects/grammar/
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.199203 craft_application-2.7.0/tests/integration/data/valid_projects/grammar/src/
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.215203 craft_application-2.7.0/tests/integration/data/valid_projects/grammar/src/on-amd64-to-amd64/
+-rw-rw-r--   0 developer  (1000) developer  (1000)       18 2024-04-30 14:29:58.000000 craft_application-2.7.0/tests/integration/data/valid_projects/grammar/src/on-amd64-to-amd64/hello.txt
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.215203 craft_application-2.7.0/tests/integration/data/valid_projects/grammar/src/on-amd64-to-arm64/
+-rw-rw-r--   0 developer  (1000) developer  (1000)       18 2024-04-30 14:29:58.000000 craft_application-2.7.0/tests/integration/data/valid_projects/grammar/src/on-amd64-to-arm64/hello.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)       26 2024-04-30 14:29:58.000000 craft_application-2.7.0/tests/integration/data/valid_projects/grammar/stderr
+-rw-rw-r--   0 developer  (1000) developer  (1000)      516 2024-04-30 19:53:17.000000 craft_application-2.7.0/tests/integration/data/valid_projects/grammar/testcraft.yaml
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.215203 craft_application-2.7.0/tests/integration/launchpad/
+-rw-rw-r--   0 developer  (1000) developer  (1000)        0 2024-02-09 15:30:38.000000 craft_application-2.7.0/tests/integration/launchpad/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1021 2024-02-22 14:28:03.000000 craft_application-2.7.0/tests/integration/launchpad/conftest.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1709 2024-04-23 21:07:18.000000 craft_application-2.7.0/tests/integration/launchpad/test_anonymous_access.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.215203 craft_application-2.7.0/tests/integration/services/
+-rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-10-21 00:19:20.000000 craft_application-2.7.0/tests/integration/services/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     5475 2024-03-05 01:55:10.000000 craft_application-2.7.0/tests/integration/services/test_lifecycle.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4287 2024-03-26 14:14:40.000000 craft_application-2.7.0/tests/integration/services/test_provider.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1886 2024-04-09 13:20:54.000000 craft_application-2.7.0/tests/integration/services/test_remotebuild.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     3445 2024-02-09 15:30:38.000000 craft_application-2.7.0/tests/integration/services/test_request.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1909 2024-03-05 01:55:10.000000 craft_application-2.7.0/tests/integration/services/test_service_factory.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)    14516 2024-05-07 21:06:46.000000 craft_application-2.7.0/tests/integration/test_application.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     2201 2023-10-21 00:19:20.000000 craft_application-2.7.0/tests/integration/test_version.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.215203 craft_application-2.7.0/tests/unit/
+-rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-10-21 00:19:20.000000 craft_application-2.7.0/tests/unit/__init__.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.215203 craft_application-2.7.0/tests/unit/commands/
+-rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-10-21 00:19:20.000000 craft_application-2.7.0/tests/unit/commands/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     7035 2024-05-08 18:34:14.000000 craft_application-2.7.0/tests/unit/commands/test_base.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)    17640 2024-05-08 18:34:14.000000 craft_application-2.7.0/tests/unit/commands/test_lifecycle.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1363 2023-10-21 00:19:20.000000 craft_application-2.7.0/tests/unit/commands/test_other.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1673 2024-04-23 21:58:47.000000 craft_application-2.7.0/tests/unit/conftest.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.215203 craft_application-2.7.0/tests/unit/launchpad/
+-rw-rw-r--   0 developer  (1000) developer  (1000)        0 2024-02-09 15:30:38.000000 craft_application-2.7.0/tests/unit/launchpad/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1194 2024-02-22 14:28:03.000000 craft_application-2.7.0/tests/unit/launchpad/conftest.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.219203 craft_application-2.7.0/tests/unit/launchpad/models/
+-rw-rw-r--   0 developer  (1000) developer  (1000)        0 2024-02-09 15:30:38.000000 craft_application-2.7.0/tests/unit/launchpad/models/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     5159 2024-02-22 14:28:03.000000 craft_application-2.7.0/tests/unit/launchpad/models/test_base.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     2562 2024-02-22 14:28:03.000000 craft_application-2.7.0/tests/unit/launchpad/models/test_code.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     9305 2024-03-26 14:14:40.000000 craft_application-2.7.0/tests/unit/launchpad/test_launchpad.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     3500 2024-03-11 15:45:17.000000 craft_application-2.7.0/tests/unit/launchpad/test_util.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.219203 craft_application-2.7.0/tests/unit/models/
+-rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-10-21 00:19:20.000000 craft_application-2.7.0/tests/unit/models/__init__.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.219203 craft_application-2.7.0/tests/unit/models/project_models/
+-rw-rw-r--   0 developer  (1000) developer  (1000)       68 2023-10-21 00:19:20.000000 craft_application-2.7.0/tests/unit/models/project_models/basic_project.yaml
+-rw-rw-r--   0 developer  (1000) developer  (1000)      442 2024-04-30 18:45:16.000000 craft_application-2.7.0/tests/unit/models/project_models/full_project.yaml
+-rw-rw-r--   0 developer  (1000) developer  (1000)       24 2023-10-21 00:19:20.000000 craft_application-2.7.0/tests/unit/models/project_models/invalid_project.yaml
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4489 2024-02-22 14:28:03.000000 craft_application-2.7.0/tests/unit/models/test_constraints.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1673 2024-04-30 19:53:17.000000 craft_application-2.7.0/tests/unit/models/test_grammar.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)    13503 2024-04-30 18:45:16.000000 craft_application-2.7.0/tests/unit/models/test_project.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.219203 craft_application-2.7.0/tests/unit/remote/
+-rw-rw-r--   0 developer  (1000) developer  (1000)        0 2024-02-09 15:30:38.000000 craft_application-2.7.0/tests/unit/remote/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)      855 2024-02-09 15:30:38.000000 craft_application-2.7.0/tests/unit/remote/conftest.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     2116 2024-02-09 15:30:38.000000 craft_application-2.7.0/tests/unit/remote/test_errors.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)    18388 2024-03-26 14:14:40.000000 craft_application-2.7.0/tests/unit/remote/test_git.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     5855 2024-03-11 15:45:17.000000 craft_application-2.7.0/tests/unit/remote/test_utils.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     3034 2024-02-09 15:30:38.000000 craft_application-2.7.0/tests/unit/remote/test_worktree.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.219203 craft_application-2.7.0/tests/unit/services/
+-rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-10-21 00:19:20.000000 craft_application-2.7.0/tests/unit/services/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     3946 2024-04-09 13:20:54.000000 craft_application-2.7.0/tests/unit/services/conftest.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)    21821 2024-04-30 19:53:17.000000 craft_application-2.7.0/tests/unit/services/test_lifecycle.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     3413 2024-03-11 15:45:17.000000 craft_application-2.7.0/tests/unit/services/test_package.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)    19346 2024-04-18 18:37:15.000000 craft_application-2.7.0/tests/unit/services/test_provider.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)    11829 2024-04-17 14:51:43.000000 craft_application-2.7.0/tests/unit/services/test_remotebuild.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     3867 2024-04-29 12:34:28.000000 craft_application-2.7.0/tests/unit/services/test_repositories.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4000 2024-02-09 15:30:38.000000 craft_application-2.7.0/tests/unit/services/test_request.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     5010 2024-04-30 18:45:16.000000 craft_application-2.7.0/tests/unit/services/test_service_factory.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)    56141 2024-05-07 21:06:46.000000 craft_application-2.7.0/tests/unit/test_application.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     2968 2024-02-09 15:30:38.000000 craft_application-2.7.0/tests/unit/test_errors.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     7670 2024-02-22 14:28:03.000000 craft_application-2.7.0/tests/unit/test_grammar.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)       57 2023-10-21 00:19:20.000000 craft_application-2.7.0/tests/unit/test_nothing.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     5444 2023-11-02 19:27:48.000000 craft_application-2.7.0/tests/unit/test_secrets.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.219203 craft_application-2.7.0/tests/unit/util/
+-rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-10-21 00:19:20.000000 craft_application-2.7.0/tests/unit/util/__init__.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.223203 craft_application-2.7.0/tests/unit/util/invalid_yaml/
+-rw-rw-r--   0 developer  (1000) developer  (1000)      156 2023-10-21 00:19:20.000000 craft_application-2.7.0/tests/unit/util/invalid_yaml/_README
+-rw-rw-r--   0 developer  (1000) developer  (1000)       46 2023-10-21 00:19:20.000000 craft_application-2.7.0/tests/unit/util/invalid_yaml/duplicate_second_level.yaml-invalid
+-rw-rw-r--   0 developer  (1000) developer  (1000)       40 2023-10-21 00:19:20.000000 craft_application-2.7.0/tests/unit/util/invalid_yaml/duplicate_top_level.yaml-invalid
+-rw-rw-r--   0 developer  (1000) developer  (1000)       38 2024-04-30 18:45:16.000000 craft_application-2.7.0/tests/unit/util/invalid_yaml/unhashable.yaml-invalid
+-rw-rw-r--   0 developer  (1000) developer  (1000)     3189 2024-01-26 19:28:17.000000 craft_application-2.7.0/tests/unit/util/test_error_formatting.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)      603 2023-11-28 20:45:58.000000 craft_application-2.7.0/tests/unit/util/test_logging.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1573 2024-02-09 15:30:38.000000 craft_application-2.7.0/tests/unit/util/test_paths.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     5221 2024-02-26 19:18:49.000000 craft_application-2.7.0/tests/unit/util/test_snap_config.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     3383 2024-03-11 15:45:17.000000 craft_application-2.7.0/tests/unit/util/test_string.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     2992 2024-03-26 14:14:40.000000 craft_application-2.7.0/tests/unit/util/test_yaml.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2024-05-08 18:41:26.223203 craft_application-2.7.0/tests/unit/util/valid_yaml/
+-rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-10-21 00:19:20.000000 craft_application-2.7.0/tests/unit/util/valid_yaml/empty.yaml
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4895 2024-04-30 18:45:16.000000 craft_application-2.7.0/tox.ini
```

### Comparing `craft_application-2.6.3/.editorconfig` & `craft_application-2.7.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/.github/.jira_sync_config.yaml` & `craft_application-2.7.0/.github/.jira_sync_config.yaml`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/.github/ISSUE_TEMPLATE/bug.yaml` & `craft_application-2.7.0/.github/ISSUE_TEMPLATE/bug.yaml`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/.github/ISSUE_TEMPLATE/task.yaml` & `craft_application-2.7.0/.github/ISSUE_TEMPLATE/task.yaml`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/.github/renovate.json5` & `craft_application-2.7.0/.github/renovate.json5`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/.github/workflows/docs.yaml` & `craft_application-2.7.0/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/.github/workflows/tests.yaml` & `craft_application-2.7.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/.gitignore` & `craft_application-2.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/.pre-commit-config.yaml` & `craft_application-2.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/HACKING.rst` & `craft_application-2.7.0/HACKING.rst`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/LICENSE` & `craft_application-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/PKG-INFO` & `craft_application-2.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-application
-Version: 2.6.3
+Version: 2.7.0
 Summary: A framework for *craft applications.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.10
@@ -43,25 +43,20 @@
 Requires-Dist: craft-application[remote]; extra == "dev"
 Provides-Extra: lint
 Requires-Dist: black~=24.0; extra == "lint"
 Requires-Dist: codespell[toml]==2.2.6; extra == "lint"
 Requires-Dist: yamllint==1.35.1; extra == "lint"
 Provides-Extra: types
 Requires-Dist: mypy[reports]==1.9.0; extra == "types"
-Requires-Dist: pyright==1.1.358; extra == "types"
+Requires-Dist: pyright==1.1.359; extra == "types"
 Requires-Dist: types-requests; extra == "types"
 Requires-Dist: types-urllib3; extra == "types"
 Provides-Extra: docs
-Requires-Dist: furo==2024.1.29; extra == "docs"
-Requires-Dist: sphinx<7.3,>=7.2.6; extra == "docs"
+Requires-Dist: canonical-sphinx~=0.1; extra == "docs"
 Requires-Dist: sphinx-autobuild==2024.2.4; extra == "docs"
-Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
-Requires-Dist: sphinx-design==0.5.0; extra == "docs"
-Requires-Dist: sphinx-pydantic==0.1.1; extra == "docs"
-Requires-Dist: sphinx-toolbox==3.5.0; extra == "docs"
 Requires-Dist: sphinx-lint==0.9.1; extra == "docs"
 Provides-Extra: apt
 Requires-Dist: python-apt>=2.4.0; sys_platform == "linux" and extra == "apt"
 
 *****************
 craft-application
 *****************
```

### Comparing `craft_application-2.6.3/README.rst` & `craft_application-2.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/__init__.py` & `craft_application-2.7.0/craft_application/__init__.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/application.py` & `craft_application-2.7.0/craft_application/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -500,15 +500,15 @@
 
             craft_cli.emit.debug(
                 f"Build plan: platform={platform}, build_for={build_for}"
             )
             self._pre_run(dispatcher)
 
             managed_mode = command.run_managed(dispatcher.parsed_args())
-            if managed_mode or command.always_load_project:
+            if managed_mode or command.needs_project(dispatcher.parsed_args()):
                 self.services.project = self.get_project(
                     platform=platform, build_for=build_for
                 )
 
             self._configure_services(provider_name)
 
             if not managed_mode:
```

### Comparing `craft_application-2.6.3/craft_application/commands/__init__.py` & `craft_application-2.7.0/craft_application/commands/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,17 +13,21 @@
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Command classes for a craft application."""
 
 from craft_application.commands.base import AppCommand, ExtensibleCommand
 from craft_application.commands import lifecycle
-from craft_application.commands.lifecycle import get_lifecycle_command_group
+from craft_application.commands.lifecycle import (
+    get_lifecycle_command_group,
+    LifecycleCommand,
+)
 from craft_application.commands.other import get_other_command_group
 
 __all__ = [
     "AppCommand",
     "ExtensibleCommand",
     "lifecycle",
+    "LifecycleCommand",
     "get_lifecycle_command_group",
     "get_other_command_group",
 ]
```

### Comparing `craft_application-2.6.3/craft_application/commands/base.py` & `craft_application-2.7.0/craft_application/commands/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,28 @@
             return
 
         super().__init__(config)
 
         self._app: application.AppMetadata = config["app"]
         self._services: service_factory.ServiceFactory = config["services"]
 
+    def needs_project(
+        self,
+        parsed_args: argparse.Namespace,  # noqa: ARG002 (unused argument is for subclasses)
+    ) -> bool:
+        """Property to determine if the command needs a project loaded.
+
+        Defaults to `self.always_load_project`. Subclasses can override this property
+
+        :param parsed_args: Parsed arguments for the command.
+
+        :returns: True if the command needs a project loaded, False otherwise.
+        """
+        return self.always_load_project
+
     def run_managed(
         self,
         parsed_args: argparse.Namespace,  # noqa: ARG002 (the unused argument is for subclasses)
     ) -> bool:
         """Whether this command should run in managed mode.
 
         By default returns `False`. Subclasses can override this method to change this,
```

### Comparing `craft_application-2.6.3/craft_application/commands/lifecycle.py` & `craft_application-2.7.0/craft_application/commands/lifecycle.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 if TYPE_CHECKING:  # pragma: no cover
     import argparse
 
 
 def get_lifecycle_command_group() -> CommandGroup:
     """Return the lifecycle related command group."""
-    commands: list[type[_LifecycleCommand]] = [
+    commands: list[type[_BaseLifecycleCommand]] = [
         CleanCommand,
         PullCommand,
         OverlayCommand,
         BuildCommand,
         StageCommand,
         PrimeCommand,
         PackCommand,
@@ -46,38 +46,29 @@
 
     return CommandGroup(
         "Lifecycle",
         commands,  # type: ignore[arg-type] # https://github.com/canonical/craft-cli/pull/157
     )
 
 
-class _LifecycleCommand(base.ExtensibleCommand):
-    """Lifecycle-related commands."""
+class _BaseLifecycleCommand(base.ExtensibleCommand):
+    """Base class for lifecycle-related commands.
+
+    All lifecycle commands must know where to execute (locally or in a build
+    environment) but do not have to provide shell access into the environment.
+    """
 
     @override
     def _run(self, parsed_args: argparse.Namespace, **kwargs: Any) -> None:
         emit.trace(f"lifecycle command: {self.name!r}, arguments: {parsed_args!r}")
 
-
-class LifecyclePartsCommand(_LifecycleCommand):
-    """A lifecycle command that uses parts."""
-
-    # All lifecycle-related commands need a project to work
-    always_load_project = True
-
     @override
     def _fill_parser(self, parser: argparse.ArgumentParser) -> None:
         super()._fill_parser(parser)  # type: ignore[arg-type]
-        parser.add_argument(
-            "parts",
-            metavar="part-name",
-            type=str,
-            nargs="*",
-            help="Optional list of parts to process",
-        )
+
         group = parser.add_mutually_exclusive_group()
         group.add_argument(
             "--destructive-mode",
             action="store_true",
             help="Build in the current host",
         )
         group.add_argument(
@@ -117,16 +108,20 @@
                 f"Not running managed mode because CRAFT_BUILD_ENVIRONMENT={build_env}"
             )
             return False
 
         return True
 
 
-class LifecycleStepCommand(LifecyclePartsCommand):
-    """An actual lifecycle step."""
+class LifecycleCommand(_BaseLifecycleCommand):
+    """A command that will run the lifecycle and can shell into the environment.
+
+    LifecycleCommands do not require a part. For example 'pack' will run
+    the lifecycle but cannot be run on a specific part.
+    """
 
     @override
     def _fill_parser(self, parser: argparse.ArgumentParser) -> None:
         super()._fill_parser(parser)
 
         if self._should_add_shell_args():
             group = parser.add_mutually_exclusive_group()
@@ -198,87 +193,120 @@
 
         if shell:
             previous_step = self._services.lifecycle.previous_step_name(step_name)
             step_name = previous_step
             shell_after = True
 
         try:
-            self._services.lifecycle.run(
-                step_name=step_name,
-                part_names=parsed_args.parts,
-            )
+            self._run_lifecycle(parsed_args, step_name)
         except Exception as err:
             if debug:
                 emit.progress(str(err), permanent=True)
                 _launch_shell()
             raise
 
         if shell_after:
             _launch_shell()
 
+    def _run_lifecycle(
+        self,
+        parsed_args: argparse.Namespace,  # noqa: ARG002 (unused argument is for subclasses)
+        step_name: str | None = None,
+    ) -> None:
+        """Run the lifecycle."""
+        self._services.lifecycle.run(step_name=step_name)
+
     @staticmethod
     def _should_add_shell_args() -> bool:
         return True
 
 
-class PullCommand(LifecycleStepCommand):
+class LifecyclePartsCommand(LifecycleCommand):
+    """A command that can run the lifecycle for a particular part."""
+
+    # All lifecycle-related commands need a project to work
+    always_load_project = True
+
+    @override
+    def _fill_parser(self, parser: argparse.ArgumentParser) -> None:
+        super()._fill_parser(parser)  # type: ignore[arg-type]
+        parser.add_argument(
+            "parts",
+            metavar="part-name",
+            type=str,
+            nargs="*",
+            help="Optional list of parts to process",
+        )
+
+    @override
+    def _run_lifecycle(
+        self, parsed_args: argparse.Namespace, step_name: str | None = None
+    ) -> None:
+        """Run the lifecycle, optionally for a part or list of parts."""
+        self._services.lifecycle.run(
+            step_name=step_name,
+            part_names=parsed_args.parts,
+        )
+
+
+class PullCommand(LifecyclePartsCommand):
     """Command to pull parts."""
 
     name = "pull"
     help_msg = "Download or retrieve artifacts defined for a part"
     overview = textwrap.dedent(
         """
         Download or retrieve artifacts defined for a part. If part names
         are specified only those parts will be pulled, otherwise all parts
         will be pulled.
         """
     )
 
 
-class OverlayCommand(LifecycleStepCommand):
+class OverlayCommand(LifecyclePartsCommand):
     """Command to overlay parts."""
 
     name = "overlay"
     help_msg = "Create part layers over the base filesystem."
     overview = textwrap.dedent(
         """
         Execute operations defined for each part on a layer over the base
         filesystem, potentially modifying its contents.
         """
     )
 
 
-class BuildCommand(LifecycleStepCommand):
+class BuildCommand(LifecyclePartsCommand):
     """Command to build parts."""
 
     name = "build"
     help_msg = "Build artifacts defined for a part"
     overview = textwrap.dedent(
         """
         Build artifacts defined for a part. If part names are specified only
         those parts will be built, otherwise all parts will be built.
         """
     )
 
 
-class StageCommand(LifecycleStepCommand):
+class StageCommand(LifecyclePartsCommand):
     """Command to stage parts."""
 
     name = "stage"
     help_msg = "Stage built artifacts into a common staging area"
     overview = textwrap.dedent(
         """
         Stage built artifacts into a common staging area. If part names are
         specified only those parts will be staged. The default is to stage
         all parts.
         """
     )
 
 
-class PrimeCommand(LifecycleStepCommand):
+class PrimeCommand(LifecyclePartsCommand):
     """Command to prime parts."""
 
     name = "prime"
     help_msg = "Prime artifacts defined for a part"
     overview = textwrap.dedent(
         """
         Prepare the final payload to be packed, performing additional
@@ -351,28 +379,44 @@
 
     @staticmethod
     @override
     def _should_add_shell_args() -> bool:
         return False
 
 
-class CleanCommand(LifecyclePartsCommand):
+class CleanCommand(_BaseLifecycleCommand):
     """Command to remove part assets."""
 
+    always_load_project = True
     name = "clean"
     help_msg = "Remove a part's assets"
     overview = textwrap.dedent(
         """
         Clean up artifacts belonging to parts. If no parts are specified,
         remove the packing environment.
         """
     )
 
     @override
-    def _run(self, parsed_args: argparse.Namespace, **kwargs: Any) -> None:
+    def _fill_parser(self, parser: argparse.ArgumentParser) -> None:
+        super()._fill_parser(parser)  # type: ignore[arg-type]
+        parser.add_argument(
+            "parts",
+            metavar="part-name",
+            type=str,
+            nargs="*",
+            help="Optional list of parts to process",
+        )
+
+    @override
+    def _run(
+        self,
+        parsed_args: argparse.Namespace,
+        **kwargs: Any,
+    ) -> None:
         """Run the clean command.
 
         The project's work directory will be cleaned if:
         - the `--destructive-mode` flag is provided OR
         - `CRAFT_BUILD_ENVIRONMENT` is set to `host` OR
         - no list of specific parts to clean is provided
```

### Comparing `craft_application-2.6.3/craft_application/commands/other.py` & `craft_application-2.7.0/craft_application/commands/other.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/errors.py` & `craft_application-2.7.0/craft_application/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 
 
 class MultipleBuildsError(CraftError):
     """The build plan contains multiple possible builds."""
 
     def __init__(self) -> None:
         message = "Multiple builds match the current platform."
-        resolution = 'Check the "--platform" and "--bulld-for" parameters.'
+        resolution = 'Check the "--platform" and "--build-for" parameters.'
 
         super().__init__(message=message, resolution=resolution)
 
 
 class IncompatibleBaseError(CraftError):
     """The build plan's base is incompatible with the host environment."""
```

### Comparing `craft_application-2.6.3/craft_application/grammar.py` & `craft_application-2.7.0/craft_application/grammar.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/launchpad/__init__.py` & `craft_application-2.7.0/craft_application/launchpad/__init__.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/launchpad/errors.py` & `craft_application-2.7.0/craft_application/launchpad/errors.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/launchpad/launchpad.py` & `craft_application-2.7.0/craft_application/launchpad/launchpad.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/launchpad/models/__init__.py` & `craft_application-2.7.0/craft_application/launchpad/models/__init__.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/launchpad/models/base.py` & `craft_application-2.7.0/craft_application/launchpad/models/base.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/launchpad/models/build.py` & `craft_application-2.7.0/craft_application/launchpad/models/build.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/launchpad/models/code.py` & `craft_application-2.7.0/craft_application/launchpad/models/code.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/launchpad/models/distro.py` & `craft_application-2.7.0/craft_application/launchpad/models/distro.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/launchpad/models/project.py` & `craft_application-2.7.0/craft_application/launchpad/models/project.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/launchpad/models/recipe.py` & `craft_application-2.7.0/craft_application/launchpad/models/recipe.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/launchpad/util.py` & `craft_application-2.7.0/craft_application/launchpad/util.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/misc/instance_bashrc` & `craft_application-2.7.0/craft_application/misc/instance_bashrc`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/models/__init__.py` & `craft_application-2.7.0/craft_application/models/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of craft_application.
 #
-# Copyright 2023 Canonical Ltd.
+# Copyright 2023-2024 Canonical Ltd.
 #
 # This program is free software: you can redistribute it and/or modify it
 # under the terms of the GNU Lesser General Public License version 3, as
 # published by the Free Software Foundation.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranties of MERCHANTABILITY,
@@ -24,20 +24,28 @@
     VersionStr,
 )
 from craft_application.models.grammar import (
     GrammarAwareProject,
     get_grammar_aware_part_keywords,
 )
 from craft_application.models.metadata import BaseMetadata
-from craft_application.models.project import BuildInfo, BuildPlanner, Project
+from craft_application.models.project import (
+    DEVEL_BASE_INFOS,
+    DEVEL_BASE_WARNING,
+    BuildInfo,
+    BuildPlanner,
+    Project,
+)
 
 
 __all__ = [
     "BaseMetadata",
     "BuildInfo",
+    "DEVEL_BASE_INFOS",
+    "DEVEL_BASE_WARNING",
     "CraftBaseConfig",
     "CraftBaseModel",
     "get_grammar_aware_part_keywords",
     "GrammarAwareProject",
     "Project",
     "BuildPlanner",
     "ProjectName",
```

### Comparing `craft_application-2.6.3/craft_application/models/base.py` & `craft_application-2.7.0/craft_application/models/base.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/models/constraints.py` & `craft_application-2.7.0/craft_application/models/constraints.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/models/grammar.py` & `craft_application-2.7.0/craft_application/models/grammar.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/models/metadata.py` & `craft_application-2.7.0/craft_application/models/metadata.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/remote/__init__.py` & `craft_application-2.7.0/craft_application/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/remote/errors.py` & `craft_application-2.7.0/craft_application/remote/errors.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/remote/git.py` & `craft_application-2.7.0/craft_application/remote/git.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/remote/utils.py` & `craft_application-2.7.0/craft_application/remote/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         )
     if not directory.is_dir():
         raise FileNotFoundError(
             f"Could not compute hash because {str(directory.absolute())} is not "
             "a directory."
         )
 
-    files = sorted([file for file in Path().glob("**/*") if file.is_file()])
+    files = sorted(file for file in directory.glob("**/*") if file.is_file())
     hashes: list[str] = []
 
     for file_path in files:
         md5_hash = md5()  # noqa: S324 (insecure-hash-function)
         with file_path.open("rb") as file:
             # read files in chunks in case they are large
             for block in iter(partial(file.read, 4096), b""):
```

### Comparing `craft_application-2.6.3/craft_application/remote/worktree.py` & `craft_application-2.7.0/craft_application/remote/worktree.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/secrets.py` & `craft_application-2.7.0/craft_application/secrets.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/services/__init__.py` & `craft_application-2.7.0/craft_application/services/__init__.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/services/base.py` & `craft_application-2.7.0/craft_application/services/base.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/services/lifecycle.py` & `craft_application-2.7.0/craft_application/services/lifecycle.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/services/package.py` & `craft_application-2.7.0/craft_application/services/package.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/services/provider.py` & `craft_application-2.7.0/craft_application/services/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         *,
         work_dir: pathlib.Path,
         allow_unstable: bool = True,
         **kwargs: bool | str | None,
     ) -> Generator[craft_providers.Executor, None, None]:
         """Context manager for getting a provider instance.
 
-        :param base_name: A craft_providers capable base name (tuple of name, version)
+        :param build_info: Build information for the instance.
         :param work_dir: Local path to mount inside the provider instance.
         :param allow_unstable: Whether to allow the use of unstable images.
         :returns: a context manager of the provider instance.
         """
         instance_name = self._get_instance_name(work_dir, build_info)
         emit.debug(f"Preparing managed instance {instance_name!r}")
         base_name = build_info.base
```

### Comparing `craft_application-2.6.3/craft_application/services/remotebuild.py` & `craft_application-2.7.0/craft_application/services/remotebuild.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/services/request.py` & `craft_application-2.7.0/craft_application/services/request.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/services/service_factory.py` & `craft_application-2.7.0/craft_application/services/service_factory.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/util/__init__.py` & `craft_application-2.7.0/craft_application/util/__init__.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/util/callbacks.py` & `craft_application-2.7.0/craft_application/util/callbacks.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/util/error_formatting.py` & `craft_application-2.7.0/craft_application/util/error_formatting.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/util/logging.py` & `craft_application-2.7.0/craft_application/util/logging.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/util/paths.py` & `craft_application-2.7.0/craft_application/util/paths.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/util/platforms.py` & `craft_application-2.7.0/craft_application/util/platforms.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/util/repositories.py` & `craft_application-2.7.0/craft_application/util/repositories.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/util/snap_config.py` & `craft_application-2.7.0/craft_application/util/snap_config.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/util/string.py` & `craft_application-2.7.0/craft_application/util/string.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application/util/yaml.py` & `craft_application-2.7.0/craft_application/util/yaml.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/craft_application.egg-info/PKG-INFO` & `craft_application-2.7.0/craft_application.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-application
-Version: 2.6.3
+Version: 2.7.0
 Summary: A framework for *craft applications.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.10
@@ -43,25 +43,20 @@
 Requires-Dist: craft-application[remote]; extra == "dev"
 Provides-Extra: lint
 Requires-Dist: black~=24.0; extra == "lint"
 Requires-Dist: codespell[toml]==2.2.6; extra == "lint"
 Requires-Dist: yamllint==1.35.1; extra == "lint"
 Provides-Extra: types
 Requires-Dist: mypy[reports]==1.9.0; extra == "types"
-Requires-Dist: pyright==1.1.358; extra == "types"
+Requires-Dist: pyright==1.1.359; extra == "types"
 Requires-Dist: types-requests; extra == "types"
 Requires-Dist: types-urllib3; extra == "types"
 Provides-Extra: docs
-Requires-Dist: furo==2024.1.29; extra == "docs"
-Requires-Dist: sphinx<7.3,>=7.2.6; extra == "docs"
+Requires-Dist: canonical-sphinx~=0.1; extra == "docs"
 Requires-Dist: sphinx-autobuild==2024.2.4; extra == "docs"
-Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
-Requires-Dist: sphinx-design==0.5.0; extra == "docs"
-Requires-Dist: sphinx-pydantic==0.1.1; extra == "docs"
-Requires-Dist: sphinx-toolbox==3.5.0; extra == "docs"
 Requires-Dist: sphinx-lint==0.9.1; extra == "docs"
 Provides-Extra: apt
 Requires-Dist: python-apt>=2.4.0; sys_platform == "linux" and extra == "apt"
 
 *****************
 craft-application
 *****************
```

### Comparing `craft_application-2.6.3/craft_application.egg-info/SOURCES.txt` & `craft_application-2.7.0/craft_application.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,14 @@
 craft_application/util/platforms.py
 craft_application/util/repositories.py
 craft_application/util/snap_config.py
 craft_application/util/string.py
 craft_application/util/yaml.py
 docs/conf.py
 docs/index.rst
-docs/_static/css/custom.css
 docs/explanation/index.rst
 docs/howto/index.rst
 docs/reference/index.rst
 docs/tutorials/index.rst
 tests/__init__.py
 tests/conftest.py
 tests/integration/__init__.py
```

### Comparing `craft_application-2.6.3/docs/index.rst` & `craft_application-2.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/pyproject.toml` & `craft_application-2.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -60,35 +60,30 @@
 lint = [
     "black~=24.0",
     "codespell[toml]==2.2.6",
     "yamllint==1.35.1"
 ]
 types = [
     "mypy[reports]==1.9.0",
-    "pyright==1.1.358",
+    "pyright==1.1.359",
     "types-requests",
     "types-urllib3",
 ]
 docs = [
-    "furo==2024.1.29",
-    "sphinx>=7.2.6,<7.3",
+    "canonical-sphinx~=0.1",
     "sphinx-autobuild==2024.2.4",
-    "sphinx-copybutton==0.5.2",
-    "sphinx-design==0.5.0",
-    "sphinx-pydantic==0.1.1",
-    "sphinx-toolbox==3.5.0",
     "sphinx-lint==0.9.1",
 ]
 apt = [
     "python-apt>=2.4.0;sys_platform=='linux'"
 ]
 
 [build-system]
 requires = [
-    "setuptools==69.4.0",
+    "setuptools==69.5.1",
     "setuptools_scm[toml]>=7.1"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.dynamic]
 readme = {file = "README.rst"}
```

### Comparing `craft_application-2.6.3/tests/conftest.py` & `craft_application-2.7.0/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of craft_application.
 #
-# Copyright 2023 Canonical Ltd.
+# Copyright 2023-2024 Canonical Ltd.
 #
 # This program is free software: you can redistribute it and/or modify it
 # under the terms of the GNU Lesser General Public License version 3, as
 # published by the Free Software Foundation.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranties of MERCHANTABILITY,
@@ -99,15 +99,15 @@
 
 @pytest.fixture()
 def fake_project() -> models.Project:
     arch = util.get_host_architecture()
     return models.Project(
         name="full-project",  # pyright: ignore[reportArgumentType]
         title="A fully-defined project",  # pyright: ignore[reportArgumentType]
-        base="core24",
+        base="ubuntu@24.04",
         version="1.0.0.post64+git12345678",  # pyright: ignore[reportArgumentType]
         contact="author@project.org",
         issues="https://github.com/canonical/craft-application/issues",
         source_code="https://github.com/canonical/craft-application",  # pyright: ignore[reportArgumentType]
         summary="A fully-defined craft-application project.",  # pyright: ignore[reportArgumentType]
         description="A fully-defined craft-application project. (description)",
         license="LGPLv3",
```

### Comparing `craft_application-2.6.3/tests/integration/conftest.py` & `craft_application-2.7.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/integration/data/valid_projects/environment/testcraft.yaml` & `craft_application-2.7.0/tests/integration/data/valid_projects/environment/testcraft.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 name: environment-project
 summary: A project with environment variables
 version: 1.0
-base: ["ubuntu", "22.04"]
+base: "ubuntu@22.04"
 
 parts:
   my-part:
     plugin: nil
     override-build: |
         target_file=${CRAFT_PART_INSTALL}/variables.yaml
         touch $target_file
```

### Comparing `craft_application-2.6.3/tests/integration/data/valid_projects/grammar/testcraft.yaml` & `craft_application-2.7.0/tests/integration/data/valid_projects/grammar/testcraft.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 name: empty
 title: A most basic project
 version: 1.0
-base: ["ubuntu", "22.04"]
+base: "ubuntu@22.04"
 
 parts:
   hello-world:
     plugin: dump
     source:
       - on amd64 to amd64: src/on-amd64-to-amd64
       - on amd64 to arm64: src/on-amd64-to-arm64
```

### Comparing `craft_application-2.6.3/tests/integration/launchpad/conftest.py` & `craft_application-2.7.0/tests/integration/launchpad/conftest.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/integration/launchpad/test_anonymous_access.py` & `craft_application-2.7.0/tests/integration/launchpad/test_anonymous_access.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/integration/services/test_lifecycle.py` & `craft_application-2.7.0/tests/integration/services/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/integration/services/test_provider.py` & `craft_application-2.7.0/tests/integration/services/test_provider.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/integration/services/test_remotebuild.py` & `craft_application-2.7.0/tests/integration/services/test_remotebuild.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/integration/services/test_request.py` & `craft_application-2.7.0/tests/integration/services/test_request.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/integration/services/test_service_factory.py` & `craft_application-2.7.0/tests/integration/services/test_service_factory.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/integration/test_application.py` & `craft_application-2.7.0/tests/integration/test_application.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/integration/test_version.py` & `craft_application-2.7.0/tests/integration/test_version.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/commands/test_base.py` & `craft_application-2.7.0/tests/unit/commands/test_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,14 +74,22 @@
     command = base.AppCommand(None)
 
     emitter.assert_trace("Not completing command configuration")
     assert not hasattr(command, "_app")
     assert not hasattr(command, "_services")
 
 
+@pytest.mark.parametrize("always_load_project", [True, False])
+def test_needs_project(fake_command, always_load_project):
+    """`needs_project()` defaults to `always_load_project`."""
+    fake_command.always_load_project = always_load_project
+
+    assert fake_command.needs_project(argparse.Namespace()) is always_load_project
+
+
 # region Tests for ExtensibleCommand
 @pytest.fixture()
 def fake_extensible_cls():
     class FakeExtensibleCommand(base.ExtensibleCommand):
         name = "fake"
         help_msg = "A fake command"
         overview = "A fake extensible command for testing."
```

### Comparing `craft_application-2.6.3/tests/unit/commands/test_lifecycle.py` & `craft_application-2.7.0/tests/unit/commands/test_lifecycle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of craft-application.
 #
-# Copyright 2023 Canonical Ltd.
+# Copyright 2023-2024 Canonical Ltd.
 #
 # This program is free software: you can redistribute it and/or modify it
 # under the terms of the GNU Lesser General Public License version 3, as
 # published by the Free Software Foundation.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranties of MERCHANTABILITY,
@@ -19,16 +19,16 @@
 import subprocess
 
 import craft_parts
 import pytest
 from craft_application.commands.lifecycle import (
     BuildCommand,
     CleanCommand,
+    LifecycleCommand,
     LifecyclePartsCommand,
-    LifecycleStepCommand,
     OverlayCommand,
     PackCommand,
     PrimeCommand,
     PullCommand,
     StageCommand,
     get_lifecycle_command_group,
 )
@@ -103,30 +103,41 @@
 
     assert set(actual.commands) == commands
 
     Features.reset()
 
 
 @pytest.mark.parametrize(("build_env_dict", "build_env_args"), BUILD_ENV_COMMANDS)
-@pytest.mark.parametrize("parts_args", PARTS_LISTS)
-def test_parts_command_fill_parser(
+@pytest.mark.parametrize(("debug_dict", "debug_args"), DEBUG_PARAMS)
+@pytest.mark.parametrize(("shell_dict", "shell_args"), SHELL_PARAMS)
+def test_lifecycle_command_fill_parser(
     app_metadata,
     fake_services,
     build_env_dict,
     build_env_args,
-    parts_args,
+    debug_dict,
+    debug_args,
+    shell_dict,
+    shell_args,
 ):
-    cls = get_fake_command_class(LifecyclePartsCommand, managed=True)
+    cls = get_fake_command_class(LifecycleCommand, managed=True)
     parser = argparse.ArgumentParser("parts_command")
     command = cls({"app": app_metadata, "services": fake_services})
+    expected = {
+        "platform": None,
+        "build_for": None,
+        **shell_dict,
+        **debug_dict,
+        **build_env_dict,
+    }
 
     command.fill_parser(parser)
 
-    args_dict = vars(parser.parse_args([*parts_args, *build_env_args]))
-    assert args_dict == {"parts": parts_args, **build_env_dict}
+    args_dict = vars(parser.parse_args([*build_env_args, *debug_args, *shell_args]))
+    assert args_dict == expected
 
 
 @pytest.mark.parametrize("parts", PARTS_LISTS)
 def test_parts_command_get_managed_cmd(
     app_metadata, fake_services, parts, emitter_verbosity
 ):
     cls = get_fake_command_class(LifecyclePartsCommand, managed=True)
@@ -188,15 +199,15 @@
     build_env_dict,
     build_env_args,
     debug_dict,
     debug_args,
     shell_args,
     shell_dict,
 ):
-    cls = get_fake_command_class(LifecycleStepCommand, managed=True)
+    cls = get_fake_command_class(LifecyclePartsCommand, managed=True)
     parser = argparse.ArgumentParser("step_command")
     expected = {
         "parts": parts_args,
         "platform": None,
         "build_for": None,
         **shell_dict,
         **debug_dict,
@@ -213,15 +224,15 @@
 
 
 @pytest.mark.parametrize(("shell_params", "shell_opts"), SHELL_PARAMS)
 @pytest.mark.parametrize("parts", PARTS_LISTS)
 def test_step_command_get_managed_cmd(
     app_metadata, fake_services, parts, emitter_verbosity, shell_params, shell_opts
 ):
-    cls = get_fake_command_class(LifecycleStepCommand, managed=True)
+    cls = get_fake_command_class(LifecyclePartsCommand, managed=True)
 
     expected = [
         app_metadata.name,
         f"--verbosity={emitter_verbosity.name.lower()}",
         "fake",
         *parts,
         *shell_opts,
@@ -235,15 +246,15 @@
 
     assert actual == expected
 
 
 @pytest.mark.parametrize("step_name", STEP_NAMES)
 @pytest.mark.parametrize("parts", PARTS_LISTS)
 def test_step_command_run_explicit_step(app_metadata, mock_services, parts, step_name):
-    cls = get_fake_command_class(LifecycleStepCommand, managed=True)
+    cls = get_fake_command_class(LifecyclePartsCommand, managed=True)
 
     parsed_args = argparse.Namespace(parts=parts)
     command = cls({"app": app_metadata, "services": mock_services})
 
     command.run(parsed_args=parsed_args, step_name=step_name)
 
     mock_services.lifecycle.run.assert_called_once_with(
```

### Comparing `craft_application-2.6.3/tests/unit/commands/test_other.py` & `craft_application-2.7.0/tests/unit/commands/test_other.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/conftest.py` & `craft_application-2.7.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/launchpad/conftest.py` & `craft_application-2.7.0/tests/unit/launchpad/conftest.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/launchpad/models/test_base.py` & `craft_application-2.7.0/tests/unit/launchpad/models/test_base.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/launchpad/models/test_code.py` & `craft_application-2.7.0/tests/unit/launchpad/models/test_code.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/launchpad/test_launchpad.py` & `craft_application-2.7.0/tests/unit/launchpad/test_launchpad.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/launchpad/test_util.py` & `craft_application-2.7.0/tests/unit/launchpad/test_util.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/models/test_constraints.py` & `craft_application-2.7.0/tests/unit/models/test_constraints.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/models/test_grammar.py` & `craft_application-2.7.0/tests/unit/models/test_grammar.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/remote/conftest.py` & `craft_application-2.7.0/tests/unit/remote/conftest.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/remote/test_errors.py` & `craft_application-2.7.0/tests/unit/remote/test_errors.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/remote/test_git.py` & `craft_application-2.7.0/tests/unit/remote/test_git.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/remote/test_utils.py` & `craft_application-2.7.0/tests/unit/remote/test_utils.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/remote/test_worktree.py` & `craft_application-2.7.0/tests/unit/remote/test_worktree.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/services/conftest.py` & `craft_application-2.7.0/tests/unit/services/conftest.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/services/test_lifecycle.py` & `craft_application-2.7.0/tests/unit/services/test_lifecycle.py`

 * *Files 1% similar despite different names*

```diff
@@ -679,15 +679,15 @@
 
     class LocalProject(models.Project):
         color: str | None
 
     fake_project = LocalProject.unmarshal(
         {
             "name": "project",
-            "base": "core24",
+            "base": "ubuntu@24.04",
             "version": "1.0.0.post64+git12345678",
             "parts": {"my-part": {"plugin": "nil"}},
             "adopt-info": "my-part",
         }
     )
     work_dir = tmp_path / "work"
     app_metadata = dataclasses.replace(
```

### Comparing `craft_application-2.6.3/tests/unit/services/test_package.py` & `craft_application-2.7.0/tests/unit/services/test_package.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/services/test_provider.py` & `craft_application-2.7.0/tests/unit/services/test_provider.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/services/test_remotebuild.py` & `craft_application-2.7.0/tests/unit/services/test_remotebuild.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/services/test_repositories.py` & `craft_application-2.7.0/tests/unit/services/test_repositories.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/services/test_request.py` & `craft_application-2.7.0/tests/unit/services/test_request.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/services/test_service_factory.py` & `craft_application-2.7.0/tests/unit/services/test_service_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 Canonical Ltd.
+# Copyright 2023-2024 Canonical Ltd.
 #
 # This program is free software: you can redistribute it and/or modify it
 # under the terms of the GNU Lesser General Public License version 3, as
 # published by the Free Software Foundation.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranties of MERCHANTABILITY,
```

### Comparing `craft_application-2.6.3/tests/unit/test_application.py` & `craft_application-2.7.0/tests/unit/test_application.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,41 +302,56 @@
 
 
 def test_app_metadata_version_attribute(tmp_path, monkeypatch):
     """Set the AppMetadata version from the main app package."""
     monkeypatch.syspath_prepend(tmp_path)
     (tmp_path / "dummycraft_version.py").write_text("__version__ = '1.2.3'")
 
-    app = application.AppMetadata(name="dummycraft_version", summary="dummy craft")
+    app = application.AppMetadata(
+        name="dummycraft_version",
+        summary="dummy craft",
+    )
     assert app.version == "1.2.3"
 
 
 def test_app_metadata_importlib(tmp_path, monkeypatch, mocker):
     """Set the AppMetadata version via importlib."""
     monkeypatch.syspath_prepend(tmp_path)
     (tmp_path / "dummycraft_importlib.py").write_text("print('hi')")
 
     mocker.patch.object(importlib.metadata, "version", return_value="4.5.6")
 
-    app = application.AppMetadata(name="dummycraft_importlib", summary="dummy craft")
+    app = application.AppMetadata(
+        name="dummycraft_importlib",
+        summary="dummy craft",
+    )
     assert app.version == "4.5.6"
 
 
 def test_app_metadata_dev():
-    app = application.AppMetadata(name="dummycraft_dev", summary="dummy craft")
+    app = application.AppMetadata(
+        name="dummycraft_dev",
+        summary="dummy craft",
+    )
     assert app.version == "dev"
 
 
 def test_app_metadata_default_project_variables():
-    app = application.AppMetadata(name="dummycraft_dev", summary="dummy craft")
+    app = application.AppMetadata(
+        name="dummycraft_dev",
+        summary="dummy craft",
+    )
     assert app.project_variables == ["version"]
 
 
 def test_app_metadata_default_mandatory_adoptable_fields():
-    app = application.AppMetadata(name="dummycraft_dev", summary="dummy craft")
+    app = application.AppMetadata(
+        name="dummycraft_dev",
+        summary="dummy craft",
+    )
     assert app.mandatory_adoptable_fields == ["version"]
 
 
 class FakeApplication(application.Application):
     """An application class explicitly for testing. Adds some convenient test hooks."""
 
     platform: str = "unknown-platform"
```

### Comparing `craft_application-2.6.3/tests/unit/test_errors.py` & `craft_application-2.7.0/tests/unit/test_errors.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/test_grammar.py` & `craft_application-2.7.0/tests/unit/test_grammar.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/test_secrets.py` & `craft_application-2.7.0/tests/unit/test_secrets.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/util/test_error_formatting.py` & `craft_application-2.7.0/tests/unit/util/test_error_formatting.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/util/test_logging.py` & `craft_application-2.7.0/tests/unit/util/test_logging.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/util/test_paths.py` & `craft_application-2.7.0/tests/unit/util/test_paths.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/util/test_snap_config.py` & `craft_application-2.7.0/tests/unit/util/test_snap_config.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/util/test_string.py` & `craft_application-2.7.0/tests/unit/util/test_string.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tests/unit/util/test_yaml.py` & `craft_application-2.7.0/tests/unit/util/test_yaml.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.6.3/tox.ini` & `craft_application-2.7.0/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
 [testenv:build-docs]
 description = Build sphinx documentation
 base = docs
 allowlist_externals = bash
 commands_pre = bash -c 'if [[ ! -e docs ]];then echo "No docs directory. Run `tox run -e sphinx-quickstart` to create one.;";return 1;fi'
 # "-W" is to treat warnings as errors
-commands = sphinx-build {posargs:-b html} -W {tox_root}/docs {tox_root}/docs/_build/html
+commands = sphinx-build {posargs:-b html} -W {tox_root}/docs {tox_root}/docs/_build
 
 [testenv:autobuild-docs]
 description = Build documentation with an autoupdating server
 base = docs
 commands = sphinx-autobuild {posargs:-b html --open-browser --port 8080} -W --watch {tox_root}/craft_application {tox_root}/docs {tox_root}/docs/_build/html
 
 [testenv:lint-docs]
```

