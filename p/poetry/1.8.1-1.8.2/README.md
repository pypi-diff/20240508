# Comparing `tmp/poetry-1.8.1.tar.gz` & `tmp/poetry-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry-1.8.1.tar", max compression
+gzip compressed data, was "poetry-1.8.2.tar", max compression
```

## Comparing `poetry-1.8.1.tar` & `poetry-1.8.2.tar`

### file list

```diff
@@ -1,771 +1,771 @@
--rw-r--r--   0        0        0     1070 2024-02-26 16:12:32.214543 poetry-1.8.1/LICENSE
--rw-r--r--   0        0        0     4662 2024-02-26 16:12:32.214543 poetry-1.8.1/README.md
--rw-r--r--   0        0        0     5197 2024-02-26 16:12:32.226544 poetry-1.8.1/pyproject.toml
--rw-r--r--   0        0        0      146 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/__main__.py
--rw-r--r--   0        0        0      342 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/__version__.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/config/__init__.py
--rw-r--r--   0        0        0    11113 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/config/config.py
--rw-r--r--   0        0        0      261 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/config/config_source.py
--rw-r--r--   0        0        0     1018 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/config/dict_config_source.py
--rw-r--r--   0        0        0     2339 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/config/file_config_source.py
--rw-r--r--   0        0        0     1348 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/config/source.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/__init__.py
--rw-r--r--   0        0        0    12831 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/application.py
--rw-r--r--   0        0        0      615 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/command_loader.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/__init__.py
--rw-r--r--   0        0        0      915 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/about.py
--rw-r--r--   0        0        0    10616 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/add.py
--rw-r--r--   0        0        0     2093 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/build.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/cache/__init__.py
--rw-r--r--   0        0        0     2411 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/cache/clear.py
--rw-r--r--   0        0        0      634 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/cache/list.py
--rw-r--r--   0        0        0     6351 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/check.py
--rw-r--r--   0        0        0     1118 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/command.py
--rw-r--r--   0        0        0    11385 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/config.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/debug/__init__.py
--rw-r--r--   0        0        0      764 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/debug/info.py
--rw-r--r--   0        0        0     4484 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/debug/resolve.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/env/__init__.py
--rw-r--r--   0        0        0     2590 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/env/info.py
--rw-r--r--   0        0        0      822 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/env/list.py
--rw-r--r--   0        0        0     1807 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/env/remove.py
--rw-r--r--   0        0        0      706 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/env/use.py
--rw-r--r--   0        0        0      544 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/env_command.py
--rw-r--r--   0        0        0      962 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/export.py
--rw-r--r--   0        0        0     4370 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/group_command.py
--rw-r--r--   0        0        0    17434 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/init.py
--rw-r--r--   0        0        0     7522 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/install.py
--rw-r--r--   0        0        0      907 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/installer_command.py
--rw-r--r--   0        0        0     1766 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/lock.py
--rw-r--r--   0        0        0     3000 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/new.py
--rw-r--r--   0        0        0     3223 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/publish.py
--rw-r--r--   0        0        0     5087 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/remove.py
--rw-r--r--   0        0        0     3261 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/run.py
--rw-r--r--   0        0        0      786 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/search.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/self/__init__.py
--rw-r--r--   0        0        0     1261 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/self/add.py
--rw-r--r--   0        0        0      973 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/self/install.py
--rw-r--r--   0        0        0      642 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/self/lock.py
--rw-r--r--   0        0        0      607 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/self/remove.py
--rw-r--r--   0        0        0     4503 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/self/self_command.py
--rw-r--r--   0        0        0     1209 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/self/show/__init__.py
--rw-r--r--   0        0        0     4034 2024-02-26 16:12:32.226544 poetry-1.8.1/src/poetry/console/commands/self/show/plugins.py
--rw-r--r--   0        0        0     1766 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/console/commands/self/update.py
--rw-r--r--   0        0        0     1527 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/console/commands/shell.py
--rw-r--r--   0        0        0    20329 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/console/commands/show.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/console/commands/source/__init__.py
--rw-r--r--   0        0        0     5687 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/console/commands/source/add.py
--rw-r--r--   0        0        0     1181 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/console/commands/source/remove.py
--rw-r--r--   0        0        0     1614 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/console/commands/source/show.py
--rw-r--r--   0        0        0     1718 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/console/commands/update.py
--rw-r--r--   0        0        0     3994 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/console/commands/version.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/console/events/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/console/events/console_events.py
--rw-r--r--   0        0        0      174 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/console/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/console/io/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/console/io/inputs/__init__.py
--rw-r--r--   0        0        0     2516 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/console/io/inputs/run_argv_input.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/console/logging/__init__.py
--rw-r--r--   0        0        0       99 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/console/logging/filters.py
--rw-r--r--   0        0        0      336 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/console/logging/formatters/__init__.py
--rw-r--r--   0        0        0      788 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/console/logging/formatters/builder_formatter.py
--rw-r--r--   0        0        0      132 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/console/logging/formatters/formatter.py
--rw-r--r--   0        0        0     2126 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/console/logging/io_formatter.py
--rw-r--r--   0        0        0      702 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/console/logging/io_handler.py
--rw-r--r--   0        0        0      134 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/exceptions.py
--rw-r--r--   0        0        0    13132 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/factory.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/inspection/__init__.py
--rw-r--r--   0        0        0    22076 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/inspection/info.py
--rw-r--r--   0        0        0    27586 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/inspection/lazy_wheel.py
--rw-r--r--   0        0        0      114 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/installation/__init__.py
--rw-r--r--   0        0        0     6798 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/installation/chef.py
--rw-r--r--   0        0        0     7508 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/installation/chooser.py
--rw-r--r--   0        0        0    36156 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/installation/executor.py
--rw-r--r--   0        0        0    14951 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/installation/installer.py
--rw-r--r--   0        0        0      262 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/installation/operations/__init__.py
--rw-r--r--   0        0        0      906 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/installation/operations/install.py
--rw-r--r--   0        0        0     1303 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/installation/operations/operation.py
--rw-r--r--   0        0        0      953 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/installation/operations/uninstall.py
--rw-r--r--   0        0        0     1540 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/installation/operations/update.py
--rw-r--r--   0        0        0     4002 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/installation/wheel_installer.py
--rw-r--r--   0        0        0     1067 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/json/__init__.py
--rw-r--r--   0        0        0     2127 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/json/schemas/poetry.json
--rw-r--r--   0        0        0      310 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/layouts/__init__.py
--rw-r--r--   0        0        0     5983 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/layouts/layout.py
--rw-r--r--   0        0        0      202 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/layouts/src.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/layouts/standard.py
--rw-r--r--   0        0        0     1625 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/locations.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/masonry/__init__.py
--rw-r--r--   0        0        0      497 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/masonry/api.py
--rw-r--r--   0        0        0      374 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/masonry/builders/__init__.py
--rw-r--r--   0        0        0     9774 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/masonry/builders/editable.py
--rw-r--r--   0        0        0      467 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/mixology/__init__.py
--rw-r--r--   0        0        0     1555 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/mixology/assignment.py
--rw-r--r--   0        0        0    10074 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/mixology/failure.py
--rw-r--r--   0        0        0    15275 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/mixology/incompatibility.py
--rw-r--r--   0        0        0     1903 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/mixology/incompatibility_cause.py
--rw-r--r--   0        0        0     7080 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/mixology/partial_solution.py
--rw-r--r--   0        0        0      676 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/mixology/result.py
--rw-r--r--   0        0        0      211 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/mixology/set_relation.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/mixology/solutions/__init__.py
--rw-r--r--   0        0        0      214 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/mixology/solutions/providers/__init__.py
--rw-r--r--   0        0        0     1059 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/mixology/solutions/providers/python_requirement_solution_provider.py
--rw-r--r--   0        0        0      189 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/mixology/solutions/solutions/__init__.py
--rw-r--r--   0        0        0     2253 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/mixology/solutions/solutions/python_requirement_solution.py
--rw-r--r--   0        0        0     6904 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/mixology/term.py
--rw-r--r--   0        0        0    23682 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/mixology/version_solver.py
--rw-r--r--   0        0        0      273 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/packages/__init__.py
--rw-r--r--   0        0        0     1297 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/packages/dependency_package.py
--rw-r--r--   0        0        0     3146 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/packages/direct_origin.py
--rw-r--r--   0        0        0    18253 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/packages/locker.py
--rw-r--r--   0        0        0      921 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/packages/package_collection.py
--rw-r--r--   0        0        0      185 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/plugins/__init__.py
--rw-r--r--   0        0        0      687 2024-02-26 16:12:32.230543 poetry-1.8.1/src/poetry/plugins/application_plugin.py
--rw-r--r--   0        0        0      435 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/plugins/base_plugin.py
--rw-r--r--   0        0        0      484 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/plugins/plugin.py
--rw-r--r--   0        0        0     2537 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/plugins/plugin_manager.py
--rw-r--r--   0        0        0     2491 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/poetry.py
--rw-r--r--   0        0        0      112 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/publishing/__init__.py
--rw-r--r--   0        0        0     2933 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/publishing/publisher.py
--rw-r--r--   0        0        0    12295 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/publishing/uploader.py
--rw-r--r--   0        0        0       99 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/puzzle/__init__.py
--rw-r--r--   0        0        0      768 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/puzzle/exceptions.py
--rw-r--r--   0        0        0    37680 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/puzzle/provider.py
--rw-r--r--   0        0        0    11114 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/puzzle/solver.py
--rw-r--r--   0        0        0     5167 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/puzzle/transaction.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/py.typed
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/pyproject/__init__.py
--rw-r--r--   0        0        0     1740 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/pyproject/toml.py
--rw-r--r--   0        0        0      198 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/repositories/__init__.py
--rw-r--r--   0        0        0      809 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/repositories/abstract_repository.py
--rw-r--r--   0        0        0     2545 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/repositories/cached_repository.py
--rw-r--r--   0        0        0      173 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/repositories/exceptions.py
--rw-r--r--   0        0        0    16821 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/repositories/http_repository.py
--rw-r--r--   0        0        0    10243 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/repositories/installed_repository.py
--rw-r--r--   0        0        0     4572 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/repositories/legacy_repository.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/repositories/link_sources/__init__.py
--rw-r--r--   0        0        0     3873 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/repositories/link_sources/base.py
--rw-r--r--   0        0        0     2611 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/repositories/link_sources/html.py
--rw-r--r--   0        0        0     1850 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/repositories/link_sources/json.py
--rw-r--r--   0        0        0      841 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/repositories/lockfile_repository.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/repositories/parsers/__init__.py
--rw-r--r--   0        0        0      596 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/repositories/parsers/html_page_parser.py
--rw-r--r--   0        0        0     2480 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/repositories/parsers/pypi_search_parser.py
--rw-r--r--   0        0        0     7466 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/repositories/pypi_repository.py
--rw-r--r--   0        0        0     3970 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/repositories/repository.py
--rw-r--r--   0        0        0     7457 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/repositories/repository_pool.py
--rw-r--r--   0        0        0      753 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/repositories/single_page_repository.py
--rw-r--r--   0        0        0      157 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/toml/__init__.py
--rw-r--r--   0        0        0      198 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/toml/exceptions.py
--rw-r--r--   0        0        0     1324 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/toml/file.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/__init__.py
--rw-r--r--   0        0        0     1369 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/_compat.py
--rw-r--r--   0        0        0    16311 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/authenticator.py
--rw-r--r--   0        0        0    10192 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/cache.py
--rw-r--r--   0        0        0      302 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/constants.py
--rw-r--r--   0        0        0     7648 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/dependency_specification.py
--rw-r--r--   0        0        0     4164 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/env/__init__.py
--rw-r--r--   0        0        0    12374 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/env/base_env.py
--rw-r--r--   0        0        0    26519 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/env/env_manager.py
--rw-r--r--   0        0        0     2113 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/env/exceptions.py
--rw-r--r--   0        0        0     3196 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/env/generic_env.py
--rw-r--r--   0        0        0     2377 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/env/mock_env.py
--rw-r--r--   0        0        0     1348 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/env/null_env.py
--rw-r--r--   0        0        0     3280 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/env/script_strings.py
--rw-r--r--   0        0        0     7425 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/env/site_packages.py
--rw-r--r--   0        0        0     2597 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/env/system_env.py
--rw-r--r--   0        0        0     4550 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/env/virtual_env.py
--rw-r--r--   0        0        0     1857 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/extras.py
--rw-r--r--   0        0        0    10479 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/helpers.py
--rw-r--r--   0        0        0     7956 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/password_manager.py
--rw-r--r--   0        0        0      406 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/patterns.py
--rw-r--r--   0        0        0     1446 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/pip.py
--rw-r--r--   0        0        0    12402 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/setup_reader.py
--rw-r--r--   0        0        0     5211 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/shell.py
--rw-r--r--   0        0        0      446 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/source.py
--rw-r--r--   0        0        0     1361 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/utils/wheel.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/vcs/__init__.py
--rw-r--r--   0        0        0       95 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/vcs/git/__init__.py
--rw-r--r--   0        0        0    17357 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/vcs/git/backend.py
--rw-r--r--   0        0        0     1520 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/vcs/git/system.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/version/__init__.py
--rw-r--r--   0        0        0     1573 2024-02-26 16:12:32.234543 poetry-1.8.1/src/poetry/version/version_selector.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.234543 poetry-1.8.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.234543 poetry-1.8.1/tests/config/__init__.py
--rw-r--r--   0        0        0     3365 2024-02-26 16:12:32.234543 poetry-1.8.1/tests/config/test_config.py
--rw-r--r--   0        0        0    14767 2024-02-26 16:12:32.234543 poetry-1.8.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.234543 poetry-1.8.1/tests/console/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/cache/__init__.py
--rw-r--r--   0        0        0     1334 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/cache/conftest.py
--rw-r--r--   0        0        0     2324 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/cache/test_clear.py
--rw-r--r--   0        0        0      832 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/cache/test_list.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/debug/__init__.py
--rw-r--r--   0        0        0     1807 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/debug/test_resolve.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/env/__init__.py
--rw-r--r--   0        0        0     2349 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/env/conftest.py
--rw-r--r--   0        0        0     1417 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/env/helpers.py
--rw-r--r--   0        0        0     1590 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/env/test_info.py
--rw-r--r--   0        0        0     2039 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/env/test_list.py
--rw-r--r--   0        0        0     4061 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/env/test_remove.py
--rw-r--r--   0        0        0     4701 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/env/test_use.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/self/__init__.py
--rw-r--r--   0        0        0     2244 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/self/conftest.py
--rw-r--r--   0        0        0       65 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/self/fixtures/poetry-1.0.5-darwin.sha256sum
--rw-r--r--   0        0        0     1041 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/self/fixtures/poetry-1.0.5-darwin.tar.gz
--rw-r--r--   0        0        0     7561 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/self/test_add_plugins.py
--rw-r--r--   0        0        0     3028 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/self/test_remove_plugins.py
--rw-r--r--   0        0        0     1596 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/self/test_self_command.py
--rw-r--r--   0        0        0     5879 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/self/test_show_plugins.py
--rw-r--r--   0        0        0     2147 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/self/test_update.py
--rw-r--r--   0        0        0     1167 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/self/utils.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/source/__init__.py
--rw-r--r--   0        0        0     4105 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/source/conftest.py
--rw-r--r--   0        0        0    10757 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/source/test_add.py
--rw-r--r--   0        0        0     2902 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/source/test_remove.py
--rw-r--r--   0        0        0     4943 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/source/test_show.py
--rw-r--r--   0        0        0      835 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/test_about.py
--rw-r--r--   0        0        0    42863 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/test_add.py
--rw-r--r--   0        0        0     4061 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/test_build.py
--rw-r--r--   0        0        0     6542 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/test_check.py
--rw-r--r--   0        0        0    17315 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/test_config.py
--rw-r--r--   0        0        0      820 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/test_export.py
--rw-r--r--   0        0        0    30078 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/test_init.py
--rw-r--r--   0        0        0    16288 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/test_install.py
--rw-r--r--   0        0        0    10591 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/test_lock.py
--rw-r--r--   0        0        0     6085 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/test_new.py
--rw-r--r--   0        0        0     7038 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/test_publish.py
--rw-r--r--   0        0        0    10936 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/test_remove.py
--rw-r--r--   0        0        0     6649 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/test_run.py
--rw-r--r--   0        0        0     2568 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/test_search.py
--rw-r--r--   0        0        0     2568 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/test_shell.py
--rw-r--r--   0        0        0    70996 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/test_show.py
--rw-r--r--   0        0        0     3020 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/test_update.py
--rw-r--r--   0        0        0     4392 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/commands/test_version.py
--rw-r--r--   0        0        0     4627 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/conftest.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/logging/__init__.py
--rw-r--r--   0        0        0     2780 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/logging/test_io_formatter.py
--rw-r--r--   0        0        0     3336 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/console/test_application.py
--rw-r--r--   0        0        0       22 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/fixtures/bad_scripts_project/no_colon/README.rst
--rw-r--r--   0        0        0      729 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/fixtures/bad_scripts_project/no_colon/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/fixtures/bad_scripts_project/no_colon/simple_project/__init__.py
--rw-r--r--   0        0        0       22 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/fixtures/bad_scripts_project/too_many_colon/README.rst
--rw-r--r--   0        0        0      727 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/fixtures/bad_scripts_project/too_many_colon/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/fixtures/bad_scripts_project/too_many_colon/simple_project/__init__.py
--rw-r--r--   0        0        0       22 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/fixtures/build_system_requires_not_available/README.rst
--rw-r--r--   0        0        0      676 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/fixtures/build_system_requires_not_available/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/fixtures/build_system_requires_not_available/simple_project/__init__.py
--rw-r--r--   0        0        0     1168 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/fixtures/complete.toml
--rw-r--r--   0        0        0      406 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/fixtures/deleted_directory_dependency/poetry.lock
--rw-r--r--   0        0        0      234 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/fixtures/deleted_directory_dependency/pyproject.toml
--rw-r--r--   0        0        0      428 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/fixtures/deleted_file_dependency/poetry.lock
--rw-r--r--   0        0        0      234 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/fixtures/deleted_file_dependency/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/fixtures/directory/project_with_transitive_directory_dependencies/project_with_transitive_directory_dependencies/__init__.py
--rw-r--r--   0        0        0      418 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/fixtures/directory/project_with_transitive_directory_dependencies/pyproject.toml
--rw-r--r--   0        0        0      574 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/fixtures/directory/project_with_transitive_directory_dependencies/setup.py
--rw-r--r--   0        0        0      234 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/fixtures/directory/project_with_transitive_file_dependencies/inner-directory-project/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/fixtures/directory/project_with_transitive_file_dependencies/project_with_transitive_file_dependencies/__init__.py
--rw-r--r--   0        0        0      385 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/fixtures/directory/project_with_transitive_file_dependencies/pyproject.toml
--rw-r--r--   0        0        0     1116 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1003 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/fixtures/distributions/demo-0.1.0.tar.gz
--rw-r--r--   0        0        0     1552 2024-02-26 16:12:32.238544 poetry-1.8.1/tests/fixtures/distributions/demo-0.1.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1169 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/distributions/demo_invalid_record-0.1.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1307 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/distributions/demo_invalid_record2-0.1.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0      310 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/distributions/demo_missing_dist_info-0.1.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0      594 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/distributions/demo_no_pkg_info-0.1.0.tar.gz
--rw-r--r--   0        0        0       22 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/excluded_subpackage/README.rst
--rw-r--r--   0        0        0       59 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/excluded_subpackage/example/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/excluded_subpackage/example/test/__init__.py
--rw-r--r--   0        0        0      159 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/excluded_subpackage/example/test/excluded.py
--rw-r--r--   0        0        0      329 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/excluded_subpackage/pyproject.toml
--rw-r--r--   0        0        0       22 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/extended_project/README.rst
--rw-r--r--   0        0        0      362 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/extended_project/build.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/extended_project/extended_project/__init__.py
--rw-r--r--   0        0        0      652 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/extended_project/pyproject.toml
--rw-r--r--   0        0        0       22 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/extended_project_without_setup/README.rst
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/extended_project_without_setup/build.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/extended_project_without_setup/extended_project/__init__.py
--rw-r--r--   0        0        0      756 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/extended_project_without_setup/pyproject.toml
--rw-r--r--   0        0        0       18 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/extended_with_no_setup/README.md
--rw-r--r--   0        0        0      859 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/extended_with_no_setup/build.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/extended_with_no_setup/extended/__init__.py
--rw-r--r--   0        0        0      888 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/extended_with_no_setup/extended/extended.c
--rw-r--r--   0        0        0      581 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/extended_with_no_setup/pyproject.toml
--rw-r--r--   0        0        0       59 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/demo/demo/__init__.py
--rw-r--r--   0        0        0      226 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/demo/demo.egg-info/PKG-INFO
--rw-r--r--   0        0        0      164 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/demo/demo.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/demo/demo.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       43 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/demo/demo.egg-info/requires.txt
--rw-r--r--   0        0        0        5 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/demo/demo.egg-info/top_level.txt
--rw-r--r--   0        0        0      429 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/demo/setup.py
--rw-r--r--   0        0        0       93 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/namespace-package-one/namespace_package/__init__.py
--rw-r--r--   0        0        0       50 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/namespace-package-one/namespace_package/one/__init__.py
--rw-r--r--   0        0        0      402 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/namespace-package-one/setup.py
--rw-r--r--   0        0        0       59 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/no-dependencies/demo/__init__.py
--rw-r--r--   0        0        0      214 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/no-dependencies/demo.egg-info/PKG-INFO
--rw-r--r--   0        0        0      137 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/no-dependencies/demo.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/no-dependencies/demo.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        5 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/no-dependencies/demo.egg-info/top_level.txt
--rw-r--r--   0        0        0      329 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/no-dependencies/setup.py
--rw-r--r--   0        0        0       59 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/no-version/demo/__init__.py
--rw-r--r--   0        0        0      696 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/no-version/setup.py
--rw-r--r--   0        0        0      254 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/PKG-INFO
--rw-r--r--   0        0        0      164 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       43 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/requires.txt
--rw-r--r--   0        0        0        5 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/top_level.txt
--rw-r--r--   0        0        0       59 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/non-canonical-name/demo/__init__.py
--rw-r--r--   0        0        0      429 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/non-canonical-name/setup.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/poetry-plugin/poetry_plugin/__init__.py
--rw-r--r--   0        0        0      349 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/poetry-plugin/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/poetry-plugin2/subdir/poetry_plugin/__init__.py
--rw-r--r--   0        0        0      349 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/poetry-plugin2/subdir/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/prerelease/prerelease/__init__.py
--rw-r--r--   0        0        0      268 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/prerelease/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/pyproject-demo/demo/__init__.py
--rw-r--r--   0        0        0      275 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/pyproject-demo/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/subdirectories/one/one/__init__.py
--rw-r--r--   0        0        0      244 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/subdirectories/one/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/subdirectories/one-copy/one/__init__.py
--rw-r--r--   0        0        0      244 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/subdirectories/one-copy/pyproject.toml
--rw-r--r--   0        0        0      252 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/subdirectories/two/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/git/github.com/demo/subdirectories/two/two/__init__.py
--rw-r--r--   0        0        0       34 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/incompatible_lock/poetry.lock
--rw-r--r--   0        0        0      320 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/incompatible_lock/pyproject.toml
--rw-r--r--   0        0        0      378 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/inspection/demo/pyproject.toml
--rw-r--r--   0        0        0      225 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/inspection/demo_no_setup_pkg_info_no_deps/PKG-INFO
--rw-r--r--   0        0        0      461 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/inspection/demo_no_setup_pkg_info_no_deps/pyproject.toml
--rw-r--r--   0        0        0      225 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/inspection/demo_only_requires_txt.egg-info/PKG-INFO
--rw-r--r--   0        0        0       64 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/inspection/demo_only_requires_txt.egg-info/requires.txt
--rw-r--r--   0        0        0      300 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/inspection/demo_poetry_package/pyproject.toml
--rw-r--r--   0        0        0      225 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/inspection/demo_with_obsolete_egg_info/demo-0.1.0.egg-info/PKG-INFO
--rw-r--r--   0        0        0       64 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/inspection/demo_with_obsolete_egg_info/demo-0.1.0.egg-info/requires.txt
--rw-r--r--   0        0        0      378 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/inspection/demo_with_obsolete_egg_info/pyproject.toml
--rw-r--r--   0        0        0       26 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/invalid_lock/poetry.lock
--rw-r--r--   0        0        0      320 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/invalid_lock/pyproject.toml
--rw-r--r--   0        0        0      717 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/invalid_pyproject/pyproject.toml
--rw-r--r--   0        0        0      406 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/missing_directory_dependency/poetry.lock
--rw-r--r--   0        0        0      299 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/missing_directory_dependency/pyproject.toml
--rw-r--r--   0        0        0      467 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/missing_extra_directory_dependency/poetry.lock
--rw-r--r--   0        0        0      341 2024-02-26 16:12:32.242544 poetry-1.8.1/tests/fixtures/missing_extra_directory_dependency/pyproject.toml
--rw-r--r--   0        0        0      428 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/missing_file_dependency/poetry.lock
--rw-r--r--   0        0        0      324 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/missing_file_dependency/pyproject.toml
--rw-r--r--   0        0        0      147 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/nameless_pyproject/pyproject.toml
--rw-r--r--   0        0        0       32 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/no_name_project/README.rst
--rw-r--r--   0        0        0      306 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/no_name_project/pyproject.toml
--rw-r--r--   0        0        0      174 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/non_package_mode/pyproject.toml
--rw-r--r--   0        0        0      762 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/old_lock/poetry.lock
--rw-r--r--   0        0        0      320 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/old_lock/pyproject.toml
--rw-r--r--   0        0        0      430 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/old_lock_path_dependency/poetry.lock
--rw-r--r--   0        0        0      336 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/old_lock_path_dependency/pyproject.toml
--rw-r--r--   0        0        0      247 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/old_lock_path_dependency/quix/pyproject.toml
--rw-r--r--   0        0        0     6512 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/outdated_lock/poetry.lock
--rw-r--r--   0        0        0      311 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/outdated_lock/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/private_pyproject/README.md
--rw-r--r--   0        0        0      309 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/private_pyproject/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/project_with_extras/project_with_extras/__init__.py
--rw-r--r--   0        0        0      402 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/project_with_extras/pyproject.toml
--rw-r--r--   0        0        0      881 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/project_with_git_dev_dependency/pyproject.toml
--rw-r--r--   0        0        0      893 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/project_with_local_dependencies/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/project_with_multi_constraints_dependency/project/__init__.py
--rw-r--r--   0        0        0      394 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/project_with_multi_constraints_dependency/pyproject.toml
--rw-r--r--   0        0        0      264 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/project_with_nested_local/bar/pyproject.toml
--rw-r--r--   0        0        0      262 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/project_with_nested_local/foo/pyproject.toml
--rw-r--r--   0        0        0      324 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/project_with_nested_local/pyproject.toml
--rw-r--r--   0        0        0      221 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/project_with_nested_local/quix/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/project_with_setup/my_package/__init__.py
--rw-r--r--   0        0        0      239 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/PKG-INFO
--rw-r--r--   0        0        0      201 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       38 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/requires.txt
--rw-r--r--   0        0        0       11 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/top_level.txt
--rw-r--r--   0        0        0      416 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/project_with_setup/setup.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/project_with_setup_calls_script/my_package/__init__.py
--rw-r--r--   0        0        0      105 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/project_with_setup_calls_script/pyproject.toml
--rw-r--r--   0        0        0      532 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/project_with_setup_calls_script/setup.py
--rw-r--r--   0        0        0       22 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/sample_project/README.rst
--rw-r--r--   0        0        0     1501 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/sample_project/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/scripts/README.md
--rw-r--r--   0        0        0      400 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/scripts/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/scripts/scripts/__init__.py
--rw-r--r--   0        0        0      557 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/scripts/scripts/check_argv0.py
--rw-r--r--   0        0        0      122 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/scripts/scripts/exit_code.py
--rw-r--r--   0        0        0      128 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/scripts/scripts/return_code.py
--rw-r--r--   0        0        0       22 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/simple_project/README.rst
--rw-r--r--   0        0        0     1320 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1106 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/simple_project/dist/simple_project-1.2.3.tar.gz
--rw-r--r--   0        0        0      775 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/simple_project/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/simple_project/simple_project/__init__.py
--rw-r--r--   0        0        0     6404 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/up_to_date_lock/poetry.lock
--rw-r--r--   0        0        0      313 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/up_to_date_lock/pyproject.toml
--rw-r--r--   0        0        0     1722 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/wheel_with_no_requires_dist/demo-0.1.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1062 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with-include/LICENSE
--rw-r--r--   0        0        0       22 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with-include/README.rst
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with-include/extra_dir/README.md
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with-include/extra_dir/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with-include/extra_dir/sub_pkg/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with-include/extra_dir/sub_pkg/vcs_excluded.txt
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with-include/extra_dir/vcs_excluded.txt
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with-include/for_wheel_only/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with-include/my_module.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with-include/notes.txt
--rw-r--r--   0        0        0       59 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with-include/package_with_include/__init__.py
--rw-r--r--   0        0        0     1259 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with-include/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with-include/src/src_package/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with-include/tests/__init__.py
--rw-r--r--   0        0        0      153 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with_conditional_path_deps/demo_one/pyproject.toml
--rw-r--r--   0        0        0      153 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with_conditional_path_deps/demo_two/pyproject.toml
--rw-r--r--   0        0        0      257 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with_conditional_path_deps/pyproject.toml
--rw-r--r--   0        0        0       22 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with_default_source/README.rst
--rw-r--r--   0        0        0     1428 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with_default_source/pyproject.toml
--rw-r--r--   0        0        0       22 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with_default_source_and_pypi/README.rst
--rw-r--r--   0        0        0     1467 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with_default_source_and_pypi/pyproject.toml
--rw-r--r--   0        0        0       22 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with_default_source_legacy/README.rst
--rw-r--r--   0        0        0     1426 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with_default_source_legacy/pyproject.toml
--rw-r--r--   0        0        0       22 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with_default_source_pypi/README.rst
--rw-r--r--   0        0        0     1393 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with_default_source_pypi/pyproject.toml
--rw-r--r--   0        0        0      370 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with_explicit_pypi_and_other/pyproject.toml
--rw-r--r--   0        0        0      402 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with_explicit_pypi_and_other_explicit/pyproject.toml
--rw-r--r--   0        0        0      301 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with_explicit_pypi_no_other/pyproject.toml
--rw-r--r--   0        0        0      352 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with_explicit_source/pyproject.toml
--rw-r--r--   0        0        0       22 2024-02-26 16:12:32.246544 poetry-1.8.1/tests/fixtures/with_local_config/README.rst
--rw-r--r--   0        0        0       48 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_local_config/poetry.toml
--rw-r--r--   0        0        0     1331 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_local_config/pyproject.toml
--rw-r--r--   0        0        0       22 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_multiple_dist_dir/README.rst
--rw-r--r--   0        0        0     1320 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_multiple_dist_dir/dist/simple_project-1.2.3-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1106 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_multiple_dist_dir/dist/simple_project-1.2.3.tar.gz
--rw-r--r--   0        0        0     1320 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_multiple_dist_dir/other_dist/dist/simple_project-1.2.3-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1106 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_multiple_dist_dir/other_dist/dist/simple_project-1.2.3.tar.gz
--rw-r--r--   0        0        0      775 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_multiple_dist_dir/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_multiple_dist_dir/simple_project/__init__.py
--rw-r--r--   0        0        0       28 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_multiple_readme_files/README-1.rst
--rw-r--r--   0        0        0       20 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_multiple_readme_files/README-2.rst
--rw-r--r--   0        0        0       79 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_multiple_readme_files/my_package/__init__.py
--rw-r--r--   0        0        0      286 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_multiple_readme_files/pyproject.toml
--rw-r--r--   0        0        0      425 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_non_default_multiple_secondary_sources/pyproject.toml
--rw-r--r--   0        0        0      413 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_non_default_multiple_secondary_sources_legacy/pyproject.toml
--rw-r--r--   0        0        0      402 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_non_default_multiple_sources/pyproject.toml
--rw-r--r--   0        0        0      396 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_non_default_multiple_sources_legacy/pyproject.toml
--rw-r--r--   0        0        0      509 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_non_default_multiple_sources_pypi/pyproject.toml
--rw-r--r--   0        0        0      333 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_non_default_secondary_source/pyproject.toml
--rw-r--r--   0        0        0      327 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_non_default_secondary_source_legacy/pyproject.toml
--rw-r--r--   0        0        0      331 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_non_default_source_explicit/pyproject.toml
--rw-r--r--   0        0        0      310 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_non_default_source_implicit/pyproject.toml
--rw-r--r--   0        0        0      214 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_path_dependency/bazz/setup.py
--rw-r--r--   0        0        0     3370 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_path_dependency/poetry.lock
--rw-r--r--   0        0        0      305 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_path_dependency/pyproject.toml
--rw-r--r--   0        0        0      364 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_supplemental_source/pyproject.toml
--rw-r--r--   0        0        0       22 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_two_default_sources/README.rst
--rw-r--r--   0        0        0     1518 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_two_default_sources/pyproject.toml
--rw-r--r--   0        0        0       22 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_two_default_sources_legacy/README.rst
--rw-r--r--   0        0        0     1520 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/fixtures/with_two_default_sources_legacy/pyproject.toml
--rw-r--r--   0        0        0     9022 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/helpers.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/inspection/__init__.py
--rw-r--r--   0        0        0    10681 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/inspection/test_info.py
--rw-r--r--   0        0        0    11409 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/inspection/test_lazy_wheel.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/__init__.py
--rw-r--r--   0        0        0     1180 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/conftest.py
--rw-r--r--   0        0        0      564 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/extras-with-dependencies.test
--rw-r--r--   0        0        0      530 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/extras.test
--rw-r--r--   0        0        0      402 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/install-no-dev.test
--rw-r--r--   0        0        0       95 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/no-dependencies.test
--rw-r--r--   0        0        0     4081 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/old-lock.test
--rw-r--r--   0        0        0      188 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/remove.test
--rw-r--r--   0        0        0      188 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/update-with-lock.test
--rw-r--r--   0        0        0      698 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/update-with-locked-extras.test
--rw-r--r--   0        0        0      410 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/with-conditional-dependency.test
--rw-r--r--   0        0        0      509 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/with-dependencies-extras.test
--rw-r--r--   0        0        0      631 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/with-dependencies-nested-extras.test
--rw-r--r--   0        0        0      295 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/with-dependencies.test
--rw-r--r--   0        0        0     2168 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/with-directory-dependency-poetry-transitive.test
--rw-r--r--   0        0        0      598 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/with-directory-dependency-poetry.test
--rw-r--r--   0        0        0      641 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/with-directory-dependency-setuptools.test
--rw-r--r--   0        0        0      471 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/with-duplicate-dependencies-update.test
--rw-r--r--   0        0        0      853 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/with-duplicate-dependencies.test
--rw-r--r--   0        0        0     1379 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/with-file-dependency-transitive.test
--rw-r--r--   0        0        0      676 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/with-file-dependency.test
--rw-r--r--   0        0        0      764 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/with-multiple-updates.test
--rw-r--r--   0        0        0      469 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/with-optional-dependencies.test
--rw-r--r--   0        0        0      565 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/with-platform-dependencies.test
--rw-r--r--   0        0        0      297 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/with-prereleases.test
--rw-r--r--   0        0        0     5109 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/with-pypi-repository.test
--rw-r--r--   0        0        0      424 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/with-python-versions.test
--rw-r--r--   0        0        0     1146 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/with-same-version-url-dependencies.test
--rw-r--r--   0        0        0      579 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/with-sub-dependencies.test
--rw-r--r--   0        0        0      686 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/with-url-dependency.test
--rw-r--r--   0        0        0      708 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/with-vcs-dependency-with-extras.test
--rw-r--r--   0        0        0      491 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/with-vcs-dependency-without-ref.test
--rw-r--r--   0        0        0      478 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/fixtures/with-wheel-dependency-no-requires-dist.test
--rw-r--r--   0        0        0     6612 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/test_chef.py
--rw-r--r--   0        0        0    11815 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/test_chooser.py
--rw-r--r--   0        0        0    49339 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/test_executor.py
--rw-r--r--   0        0        0    84595 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/test_installer.py
--rw-r--r--   0        0        0     2706 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/installation/test_wheel_installer.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/integration/__init__.py
--rw-r--r--   0        0        0    13137 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/integration/test_utils_vcs_git.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/json/__init__.py
--rw-r--r--   0        0        0      338 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/json/fixtures/source/complete_invalid_priority.toml
--rw-r--r--   0        0        0      352 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/json/fixtures/source/complete_invalid_priority_legacy_and_new.toml
--rw-r--r--   0        0        0      282 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/json/fixtures/source/complete_invalid_url.toml
--rw-r--r--   0        0        0      337 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/json/fixtures/source/complete_valid.toml
--rw-r--r--   0        0        0      349 2024-02-26 16:12:32.250543 poetry-1.8.1/tests/json/fixtures/source/complete_valid_legacy.toml
--rw-r--r--   0        0        0     1497 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/json/test_schema_sources.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/masonry/builders/__init__.py
--rw-r--r--   0        0        0       22 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/masonry/builders/fixtures/excluded_subpackage/README.rst
--rw-r--r--   0        0        0       59 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/masonry/builders/fixtures/excluded_subpackage/example/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/masonry/builders/fixtures/excluded_subpackage/example/test/__init__.py
--rw-r--r--   0        0        0      176 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/masonry/builders/fixtures/excluded_subpackage/example/test/excluded.py
--rw-r--r--   0        0        0      329 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/masonry/builders/fixtures/excluded_subpackage/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/masonry/builders/fixtures/pep_561_stub_only/pkg-stubs/__init__.pyi
--rw-r--r--   0        0        0       83 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/masonry/builders/fixtures/pep_561_stub_only/pkg-stubs/module.pyi
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/masonry/builders/fixtures/pep_561_stub_only/pkg-stubs/subpkg/__init__.pyi
--rw-r--r--   0        0        0      261 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/masonry/builders/fixtures/pep_561_stub_only/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/__init__.pyi
--rw-r--r--   0        0        0       83 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/module.pyi
--rw-r--r--   0        0        0        8 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/py.typed
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/subpkg/__init__.pyi
--rw-r--r--   0        0        0      291 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pyproject.toml
--rw-r--r--   0        0        0      294 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/masonry/builders/fixtures/pep_561_stub_only_src/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/masonry/builders/fixtures/pep_561_stub_only_src/src/pkg-stubs/__init__.pyi
--rw-r--r--   0        0        0       83 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/masonry/builders/fixtures/pep_561_stub_only_src/src/pkg-stubs/module.pyi
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/masonry/builders/fixtures/pep_561_stub_only_src/src/pkg-stubs/subpkg/__init__.pyi
--rw-r--r--   0        0        0    11777 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/masonry/builders/test_editable_builder.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/mixology/__init__.py
--rw-r--r--   0        0        0     2188 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/mixology/helpers.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/mixology/solutions/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/mixology/solutions/providers/__init__.py
--rw-r--r--   0        0        0     1449 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/mixology/solutions/providers/test_python_requirement_solution_provider.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/mixology/solutions/solutions/__init__.py
--rw-r--r--   0        0        0     1442 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/mixology/solutions/solutions/test_python_requirement_solution.py
--rw-r--r--   0        0        0     1572 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/mixology/test_incompatibility.py
--rw-r--r--   0        0        0      109 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/mixology/version_solver/__init__.py
--rw-r--r--   0        0        0     1066 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/mixology/version_solver/conftest.py
--rw-r--r--   0        0        0     7406 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/mixology/version_solver/test_backtracking.py
--rw-r--r--   0        0        0     4326 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/mixology/version_solver/test_basic_graph.py
--rw-r--r--   0        0        0     7554 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/mixology/version_solver/test_dependency_cache.py
--rw-r--r--   0        0        0     1157 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/mixology/version_solver/test_python_constraint.py
--rw-r--r--   0        0        0     5493 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/mixology/version_solver/test_unsolvable.py
--rw-r--r--   0        0        0     7700 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/mixology/version_solver/test_with_lock.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/packages/__init__.py
--rw-r--r--   0        0        0     1935 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/packages/test_direct_origin.py
--rw-r--r--   0        0        0    30734 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/packages/test_locker.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/plugins/__init__.py
--rw-r--r--   0        0        0     3299 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/plugins/test_plugin_manager.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/publishing/__init__.py
--rw-r--r--   0        0        0     6438 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/publishing/test_publisher.py
--rw-r--r--   0        0        0     4720 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/publishing/test_uploader.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/puzzle/__init__.py
--rw-r--r--   0        0        0      528 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/puzzle/conftest.py
--rw-r--r--   0        0        0    30314 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/puzzle/test_provider.py
--rw-r--r--   0        0        0   148037 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/puzzle/test_solver.py
--rw-r--r--   0        0        0     5634 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/puzzle/test_transaction.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/pyproject/__init__.py
--rw-r--r--   0        0        0      813 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/pyproject/conftest.py
--rw-r--r--   0        0        0     1379 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/pyproject/test_pyproject_toml.py
--rw-r--r--   0        0        0      755 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/pyproject/test_pyproject_toml_file.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/repositories/__init__.py
--rw-r--r--   0        0        0     1474 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/repositories/conftest.py
--rw-r--r--   0        0        0    16009 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/cleo-0.7.6.dist-info/METADATA
--rw-r--r--   0        0        0      110 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/directory_pep_610-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0       81 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/directory_pep_610-1.2.3.dist-info/direct_url.json
--rw-r--r--   0        0        0      719 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-2.3.4.dist-info/METADATA
--rw-r--r--   0        0        0      731 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-with-import-2.3.4.dist-info/METADATA
--rw-r--r--   0        0        0       10 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-with-import.pth
--rw-r--r--   0        0        0       18 2024-02-26 16:12:32.254544 poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable.pth
--rw-r--r--   0        0        0      119 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable_directory_pep_610-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0      105 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable_directory_pep_610-1.2.3.dist-info/direct_url.json
--rw-r--r--   0        0        0      105 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/file_pep_610-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0      182 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/file_pep_610-1.2.3.dist-info/direct_url.json
--rw-r--r--   0        0        0     1306 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/foo-0.1.0-py3.8.egg
--rw-r--r--   0        0        0      104 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0      159 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610-1.2.3.dist-info/direct_url.json
--rw-r--r--   0        0        0      125 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610_no_requested_version-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0      141 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610_no_requested_version-1.2.3.dist-info/direct_url.json
--rw-r--r--   0        0        0      117 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610_subdirectory-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0      200 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610_subdirectory-1.2.3.dist-info/direct_url.json
--rw-r--r--   0        0        0      719 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/standard-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0        9 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/standard.pth
--rw-r--r--   0        0        0      104 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/url_pep_610-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0      102 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/url_pep_610-1.2.3.dist-info/direct_url.json
--rw-r--r--   0        0        0      717 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/bender-2.0.5.dist-info/METADATA
--rw-r--r--   0        0        0       20 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/bender.pth
--rw-r--r--   0        0        0      710 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/lib64-2.3.4.dist-info/METADATA
--rw-r--r--   0        0        0      717 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/installed/src/bender/bender.egg-info/PKG-INFO
--rw-r--r--   0        0        0     8866 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/installed/src/pendulum/pendulum.egg-info/PKG-INFO
--rw-r--r--   0        0        0       87 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/installed/src/pendulum/pendulum.egg-info/requires.txt
--rw-r--r--   0        0        0     9020 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/installed/vendor/py3.7/attrs-19.3.0.dist-info/METADATA
--rw-r--r--   0        0        0      731 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/legacy/absolute.html
--rw-r--r--   0        0        0      790 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/legacy/black.html
--rw-r--r--   0        0        0     1455 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/legacy/clikit.html
--rw-r--r--   0        0        0      260 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/legacy/demo.html
--rw-r--r--   0        0        0      746 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/legacy/discord-py.html
--rw-r--r--   0        0        0      759 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/legacy/futures-partial-yank.html
--rw-r--r--   0        0        0      747 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/legacy/futures.html
--rw-r--r--   0        0        0      625 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/legacy/invalid-version.html
--rw-r--r--   0        0        0     1433 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/legacy/ipython.html
--rw-r--r--   0        0        0      470 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/legacy/isort-metadata.html
--rw-r--r--   0        0        0      917 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/legacy/isort.html
--rw-r--r--   0        0        0      333 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/legacy/jupyter.html
--rw-r--r--   0        0        0      348 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/legacy/missing-version.html
--rw-r--r--   0        0        0      401 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/legacy/pastel.html
--rw-r--r--   0        0        0      534 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/legacy/poetry-test-py2-py3-metadata-merge.html
--rw-r--r--   0        0        0     1727 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/legacy/pytest-with-extra-packages.html
--rw-r--r--   0        0        0      802 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/legacy/pytest.html
--rw-r--r--   0        0        0      467 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/legacy/python-language-server.html
--rw-r--r--   0        0        0      941 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/legacy/pyyaml.html
--rw-r--r--   0        0        0      687 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/legacy/relative.html
--rw-r--r--   0        0        0      473 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/legacy/tomlkit.html
--rw-r--r--   0        0        0     1223 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/metadata/isort-metadata-4.3.4-py2-none-any.whl.metadata
--rw-r--r--   0        0        0     1223 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/metadata/isort-metadata-4.3.4-py3-none-any.whl.metadata
--rw-r--r--   0        0        0    18499 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/SQLAlchemy-1.2.12.tar.gz
--rw-r--r--   0        0        0     9634 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/Twisted-18.9.0.tar.bz2
--rw-r--r--   0        0        0     1940 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/black-19.10b0-py36-none-any.whl
--rw-r--r--   0        0        0    14949 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/black-21.11b0-py3-none-any.whl
--rw-r--r--   0        0        0    78701 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/cleo-1.0.0a5-py3-none-any.whl
--rw-r--r--   0        0        0     2329 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/clikit-0.2.4-py2.py3-none-any.whl
--rw-r--r--   0        0        0     2290 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/discord.py-2.0.0-py3-none-any.whl
--rw-r--r--   0        0        0    15847 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0-py2-none-any.whl
--rw-r--r--   0        0        0    18359 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0.tar.gz
--rw-r--r--   0        0        0    31809 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/importlib_metadata-1.7.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0    23473 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py2-none-any.whl
--rw-r--r--   0        0        0    23475 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py3-none-any.whl
--rw-r--r--   0        0        0    15795 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0.tar.gz
--rw-r--r--   0        0        0    22352 2024-02-26 16:12:32.258544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/ipython-7.5.0-py3-none-any.whl
--rw-r--r--   0        0        0    45393 2024-02-26 16:12:32.262544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py2-none-any.whl
--rw-r--r--   0        0        0    45352 2024-02-26 16:12:32.262544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py3-none-any.whl
--rw-r--r--   0        0        0    56070 2024-02-26 16:12:32.262544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4.tar.gz
--rw-r--r--   0        0        0     2736 2024-02-26 16:12:32.262544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0    12916 2024-02-26 16:12:32.262544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0.tar.gz
--rw-r--r--   0        0        0     4490 2024-02-26 16:12:32.262544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/pastel-0.1.0.tar.gz
--rw-r--r--   0        0        0   464992 2024-02-26 16:12:32.262544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/poetry_core-1.5.0-py3-none-any.whl
--rw-r--r--   0        0        0     1213 2024-02-26 16:12:32.262544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py2-none-any.whl
--rw-r--r--   0        0        0     1218 2024-02-26 16:12:32.262544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py3-none-any.whl
--rw-r--r--   0        0        0     3691 2024-02-26 16:12:32.262544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/pytest-3.5.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0     3708 2024-02-26 16:12:32.262544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/pytest-3.5.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0    54076 2024-02-26 16:12:32.262544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/python-language-server-0.21.2.tar.gz
--rw-r--r--   0        0        0    29813 2024-02-26 16:12:32.262544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.2.tar.gz
--rw-r--r--   0        0        0    29864 2024-02-26 16:12:32.262544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.3.tar.gz
--rw-r--r--   0        0        0     5700 2024-02-26 16:12:32.262544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/zipp-3.5.0-py3-none-any.whl
--rw-r--r--   0        0        0     3421 2024-02-26 16:12:32.262544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/attrs/17.4.0.json
--rw-r--r--   0        0        0      856 2024-02-26 16:12:32.262544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/attrs.json
--rw-r--r--   0        0        0    62683 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/black/19.10b0.json
--rw-r--r--   0        0        0     5924 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/black/21.11b0.json
--rw-r--r--   0        0        0     1709 2024-02-26 16:12:32.262544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/black.json
--rw-r--r--   0        0        0     2298 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/cachecontrol/0.12.5.json
--rw-r--r--   0        0        0     2425 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/cachecontrol.json
--rw-r--r--   0        0        0     3035 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/cleo/1.0.0a5.json
--rw-r--r--   0        0        0     3745 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/clikit/0.2.4.json
--rw-r--r--   0        0        0      997 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/clikit.json
--rw-r--r--   0        0        0     2922 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/colorama/0.3.9.json
--rw-r--r--   0        0        0      867 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/colorama.json
--rw-r--r--   0        0        0     4035 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/discord-py/2.0.0.json
--rw-r--r--   0        0        0     2944 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/funcsigs/1.0.2.json
--rw-r--r--   0        0        0      867 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/funcsigs.json
--rw-r--r--   0        0        0     3838 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/hbmqtt/0.9.6.json
--rw-r--r--   0        0        0    14437 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/hbmqtt.json
--rw-r--r--   0        0        0     5331 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/importlib-metadata/1.7.0.json
--rw-r--r--   0        0        0     1065 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/importlib-metadata.json
--rw-r--r--   0        0        0     5984 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/ipython/4.1.0rc1.json
--rw-r--r--   0        0        0    21476 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/isort/4.3.4.json
--rw-r--r--   0        0        0    21476 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/isort-metadata/4.3.4.json
--rw-r--r--   0        0        0     1342 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/isort-metadata.json
--rw-r--r--   0        0        0     1221 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/isort.json
--rw-r--r--   0        0        0     3969 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/jupyter/1.0.0.json
--rw-r--r--   0        0        0     1217 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/jupyter.json
--rw-r--r--   0        0        0     2931 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/lockfile/0.12.2.json
--rw-r--r--   0        0        0      871 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/lockfile.json
--rw-r--r--   0        0        0     3552 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/more-itertools/4.1.0.json
--rw-r--r--   0        0        0     1284 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/more-itertools.json
--rw-r--r--   0        0        0     2328 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/pluggy/0.6.0.json
--rw-r--r--   0        0        0      470 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/pluggy.json
--rw-r--r--   0        0        0     3180 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/poetry/0.12.4.json
--rw-r--r--   0        0        0     3555 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/poetry-core/1.5.0.json
--rw-r--r--   0        0        0      897 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/poetry-core.json
--rw-r--r--   0        0        0     4561 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/poetry.json
--rw-r--r--   0        0        0     3095 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/py/1.5.3.json
--rw-r--r--   0        0        0      837 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/py.json
--rw-r--r--   0        0        0      931 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/pygame-music-grid.json
--rw-r--r--   0        0        0     4469 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/pylev/1.3.0.json
--rw-r--r--   0        0        0      495 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/pylev.json
--rw-r--r--   0        0        0     6933 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/pytest/3.5.0.json
--rw-r--r--   0        0        0     7555 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/pytest/3.5.1.json
--rw-r--r--   0        0        0      857 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/pytest.json
--rw-r--r--   0        0        0    14143 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/pyyaml/3.13.0.json
--rw-r--r--   0        0        0     7805 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/pyyaml.json
--rw-r--r--   0        0        0     3142 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/requests/2.18.4.json
--rw-r--r--   0        0        0    67409 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/requests.json
--rw-r--r--   0        0        0     5315 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/setuptools/39.2.0.json
--rw-r--r--   0        0        0     8423 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/setuptools/67.6.1.json
--rw-r--r--   0        0        0     1843 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/setuptools.json
--rw-r--r--   0        0        0     2387 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/six/1.11.0.json
--rw-r--r--   0        0        0      846 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/six.json
--rw-r--r--   0        0        0     8870 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/sqlalchemy/1.2.12.json
--rw-r--r--   0        0        0      484 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/sqlalchemy.json
--rw-r--r--   0        0        0     6109 2024-02-26 16:12:32.266544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/toga.json
--rw-r--r--   0        0        0    11126 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/tomlkit/0.5.3.json
--rw-r--r--   0        0        0     1892 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/tomlkit.json
--rw-r--r--   0        0        0     3184 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/trackpy/0.4.1.json
--rw-r--r--   0        0        0      838 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/trackpy.json
--rw-r--r--   0        0        0    11606 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/twisted/18.9.0.json
--rw-r--r--   0        0        0      477 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/twisted.json
--rw-r--r--   0        0        0     4483 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/wheel/0.40.0.json
--rw-r--r--   0        0        0     1041 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/wheel.json
--rw-r--r--   0        0        0     5188 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/zipp/3.5.0.json
--rw-r--r--   0        0        0      907 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/zipp.json
--rw-r--r--   0        0        0   224197 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/fixtures/pypi.org/search/search.html
--rw-r--r--   0        0        0     3407 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/fixtures/single-page/jax_releases.html
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/link_sources/__init__.py
--rw-r--r--   0        0        0     3108 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/link_sources/test_base.py
--rw-r--r--   0        0        0     5532 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/link_sources/test_html.py
--rw-r--r--   0        0        0     2522 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/link_sources/test_json.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/parsers/__init__.py
--rw-r--r--   0        0        0     2219 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/parsers/test_html_page_parser.py
--rw-r--r--   0        0        0     4176 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/parsers/test_pypi_search_parser.py
--rw-r--r--   0        0        0     5910 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/test_http_repository.py
--rw-r--r--   0        0        0    12293 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/test_installed_repository.py
--rw-r--r--   0        0        0    19821 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/test_legacy_repository.py
--rw-r--r--   0        0        0     1746 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/test_lockfile_repository.py
--rw-r--r--   0        0        0    12350 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/test_pypi_repository.py
--rw-r--r--   0        0        0     2321 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/test_repository.py
--rw-r--r--   0        0        0    13022 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/test_repository_pool.py
--rw-r--r--   0        0        0     2084 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/repositories/test_single_page_repository.py
--rw-r--r--   0        0        0    21940 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/test_factory.py
--rw-r--r--   0        0        0      399 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/test_helpers.py
--rw-r--r--   0        0        0     1873 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/types.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/__init__.py
--rw-r--r--   0        0        0      384 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/conftest.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/env/__init__.py
--rw-r--r--   0        0        0      541 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/env/conftest.py
--rw-r--r--   0        0        0    18529 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/env/test_env.py
--rw-r--r--   0        0        0    37640 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/env/test_env_manager.py
--rw-r--r--   0        0        0     1562 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/env/test_env_site_packages.py
--rw-r--r--   0        0        0      604 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/fixtures/pyproject.toml
--rw-r--r--   0        0        0      371 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/fixtures/setups/ansible/requirements.txt
--rw-r--r--   0        0        0    10765 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/fixtures/setups/ansible/setup.py
--rw-r--r--   0        0        0      271 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/fixtures/setups/extras_require_with_vars/setup.py
--rw-r--r--   0        0        0     2581 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/fixtures/setups/flask/setup.py
--rw-r--r--   0        0        0       75 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/fixtures/setups/minimal/setup.py
--rw-r--r--   0        0        0     1353 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/fixtures/setups/pendulum/setup.py
--rw-r--r--   0        0        0    11825 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/fixtures/setups/pyyaml/setup.py
--rw-r--r--   0        0        0     3366 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/fixtures/setups/requests/setup.py
--rw-r--r--   0        0        0      290 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/fixtures/setups/setuptools_setup/setup.py
--rw-r--r--   0        0        0     6272 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/fixtures/setups/sqlalchemy/setup.py
--rw-r--r--   0        0        0      339 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/fixtures/setups/with-setup-cfg/setup.cfg
--rw-r--r--   0        0        0       75 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/fixtures/setups/with-setup-cfg/setup.py
--rw-r--r--   0        0        0      339 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/fixtures/setups/with-setup-cfg-attr/setup.cfg
--rw-r--r--   0        0        0       75 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/fixtures/setups/with-setup-cfg-attr/setup.py
--rw-r--r--   0        0        0        0 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/fixtures/setups/with-setup-cfg-minimal/setup.cfg
--rw-r--r--   0        0        0       75 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/fixtures/setups/with-setup-cfg-minimal/setup.py
--rw-r--r--   0        0        0    22054 2024-02-26 16:12:32.270544 poetry-1.8.1/tests/utils/test_authenticator.py
--rw-r--r--   0        0        0    10896 2024-02-26 16:12:32.274544 poetry-1.8.1/tests/utils/test_cache.py
--rw-r--r--   0        0        0     6069 2024-02-26 16:12:32.274544 poetry-1.8.1/tests/utils/test_dependency_specification.py
--rw-r--r--   0        0        0     2374 2024-02-26 16:12:32.274544 poetry-1.8.1/tests/utils/test_extras.py
--rw-r--r--   0        0        0     6830 2024-02-26 16:12:32.274544 poetry-1.8.1/tests/utils/test_helpers.py
--rw-r--r--   0        0        0    11278 2024-02-26 16:12:32.274544 poetry-1.8.1/tests/utils/test_password_manager.py
--rw-r--r--   0        0        0     1114 2024-02-26 16:12:32.274544 poetry-1.8.1/tests/utils/test_patterns.py
--rw-r--r--   0        0        0     1092 2024-02-26 16:12:32.274544 poetry-1.8.1/tests/utils/test_pip.py
--rw-r--r--   0        0        0     9111 2024-02-26 16:12:32.274544 poetry-1.8.1/tests/utils/test_setup_reader.py
--rw-r--r--   0        0        0     2182 2024-02-26 16:12:32.274544 poetry-1.8.1/tests/utils/test_source.py
--rw-r--r--   0        0        0      607 2024-02-26 16:12:32.274544 poetry-1.8.1/tests/vcs/git/test_backend.py
--rw-r--r--   0        0        0     2588 2024-02-26 16:12:32.274544 poetry-1.8.1/tests/vcs/git/test_system.py
--rw-r--r--   0        0        0     6839 1970-01-01 00:00:00.000000 poetry-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-02 15:26:20.011978 poetry-1.8.2/LICENSE
+-rw-r--r--   0        0        0     4662 2024-03-02 15:26:20.011978 poetry-1.8.2/README.md
+-rw-r--r--   0        0        0     5197 2024-03-02 15:26:20.023979 poetry-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0      146 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/__main__.py
+-rw-r--r--   0        0        0      342 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/__version__.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/config/__init__.py
+-rw-r--r--   0        0        0    11113 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/config/config.py
+-rw-r--r--   0        0        0      261 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/config/config_source.py
+-rw-r--r--   0        0        0     1018 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/config/dict_config_source.py
+-rw-r--r--   0        0        0     2339 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/config/file_config_source.py
+-rw-r--r--   0        0        0     1348 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/config/source.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/__init__.py
+-rw-r--r--   0        0        0    12831 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/application.py
+-rw-r--r--   0        0        0      615 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/command_loader.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/__init__.py
+-rw-r--r--   0        0        0      915 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/about.py
+-rw-r--r--   0        0        0    10672 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/add.py
+-rw-r--r--   0        0        0     2093 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/build.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/cache/__init__.py
+-rw-r--r--   0        0        0     2411 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/cache/clear.py
+-rw-r--r--   0        0        0      634 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/cache/list.py
+-rw-r--r--   0        0        0     6351 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/check.py
+-rw-r--r--   0        0        0     1118 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/command.py
+-rw-r--r--   0        0        0    11385 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/config.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/debug/__init__.py
+-rw-r--r--   0        0        0      764 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/debug/info.py
+-rw-r--r--   0        0        0     4484 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/debug/resolve.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/env/__init__.py
+-rw-r--r--   0        0        0     2590 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/env/info.py
+-rw-r--r--   0        0        0      822 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/env/list.py
+-rw-r--r--   0        0        0     1807 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/env/remove.py
+-rw-r--r--   0        0        0      706 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/env/use.py
+-rw-r--r--   0        0        0      544 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/env_command.py
+-rw-r--r--   0        0        0      962 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/export.py
+-rw-r--r--   0        0        0     4370 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/group_command.py
+-rw-r--r--   0        0        0    17434 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/init.py
+-rw-r--r--   0        0        0     7542 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/install.py
+-rw-r--r--   0        0        0      907 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/installer_command.py
+-rw-r--r--   0        0        0     1766 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/lock.py
+-rw-r--r--   0        0        0     3000 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/new.py
+-rw-r--r--   0        0        0     3223 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/publish.py
+-rw-r--r--   0        0        0     5087 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/remove.py
+-rw-r--r--   0        0        0     3261 2024-03-02 15:26:20.023979 poetry-1.8.2/src/poetry/console/commands/run.py
+-rw-r--r--   0        0        0      786 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/commands/search.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/commands/self/__init__.py
+-rw-r--r--   0        0        0     1261 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/commands/self/add.py
+-rw-r--r--   0        0        0      973 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/commands/self/install.py
+-rw-r--r--   0        0        0      642 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/commands/self/lock.py
+-rw-r--r--   0        0        0      607 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/commands/self/remove.py
+-rw-r--r--   0        0        0     4503 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/commands/self/self_command.py
+-rw-r--r--   0        0        0     1209 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/commands/self/show/__init__.py
+-rw-r--r--   0        0        0     4034 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/commands/self/show/plugins.py
+-rw-r--r--   0        0        0     1766 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/commands/self/update.py
+-rw-r--r--   0        0        0     1527 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/commands/shell.py
+-rw-r--r--   0        0        0    20329 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/commands/show.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/commands/source/__init__.py
+-rw-r--r--   0        0        0     5687 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/commands/source/add.py
+-rw-r--r--   0        0        0     1181 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/commands/source/remove.py
+-rw-r--r--   0        0        0     1614 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/commands/source/show.py
+-rw-r--r--   0        0        0     1718 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/commands/update.py
+-rw-r--r--   0        0        0     3994 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/commands/version.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/events/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/events/console_events.py
+-rw-r--r--   0        0        0      174 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/io/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/io/inputs/__init__.py
+-rw-r--r--   0        0        0     2516 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/io/inputs/run_argv_input.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/logging/__init__.py
+-rw-r--r--   0        0        0       99 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/logging/filters.py
+-rw-r--r--   0        0        0      336 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/logging/formatters/__init__.py
+-rw-r--r--   0        0        0      788 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/logging/formatters/builder_formatter.py
+-rw-r--r--   0        0        0      132 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/logging/formatters/formatter.py
+-rw-r--r--   0        0        0     2126 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/logging/io_formatter.py
+-rw-r--r--   0        0        0      702 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/console/logging/io_handler.py
+-rw-r--r--   0        0        0      134 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/exceptions.py
+-rw-r--r--   0        0        0    13132 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/factory.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/inspection/__init__.py
+-rw-r--r--   0        0        0    22076 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/inspection/info.py
+-rw-r--r--   0        0        0    29321 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/inspection/lazy_wheel.py
+-rw-r--r--   0        0        0      114 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/installation/__init__.py
+-rw-r--r--   0        0        0     6798 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/installation/chef.py
+-rw-r--r--   0        0        0     7508 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/installation/chooser.py
+-rw-r--r--   0        0        0    36156 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/installation/executor.py
+-rw-r--r--   0        0        0    14951 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/installation/installer.py
+-rw-r--r--   0        0        0      262 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/installation/operations/__init__.py
+-rw-r--r--   0        0        0      906 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/installation/operations/install.py
+-rw-r--r--   0        0        0     1303 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/installation/operations/operation.py
+-rw-r--r--   0        0        0      953 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/installation/operations/uninstall.py
+-rw-r--r--   0        0        0     1540 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/installation/operations/update.py
+-rw-r--r--   0        0        0     4002 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/installation/wheel_installer.py
+-rw-r--r--   0        0        0     1067 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/json/__init__.py
+-rw-r--r--   0        0        0     2127 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/json/schemas/poetry.json
+-rw-r--r--   0        0        0      310 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/layouts/__init__.py
+-rw-r--r--   0        0        0     5983 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/layouts/layout.py
+-rw-r--r--   0        0        0      202 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/layouts/src.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/layouts/standard.py
+-rw-r--r--   0        0        0     1625 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/locations.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/masonry/__init__.py
+-rw-r--r--   0        0        0      497 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/masonry/api.py
+-rw-r--r--   0        0        0      374 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/masonry/builders/__init__.py
+-rw-r--r--   0        0        0     9774 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/masonry/builders/editable.py
+-rw-r--r--   0        0        0      467 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/mixology/__init__.py
+-rw-r--r--   0        0        0     1555 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/mixology/assignment.py
+-rw-r--r--   0        0        0    10074 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/mixology/failure.py
+-rw-r--r--   0        0        0    15275 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/mixology/incompatibility.py
+-rw-r--r--   0        0        0     1903 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/mixology/incompatibility_cause.py
+-rw-r--r--   0        0        0     7080 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/mixology/partial_solution.py
+-rw-r--r--   0        0        0      676 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/mixology/result.py
+-rw-r--r--   0        0        0      211 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/mixology/set_relation.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/mixology/solutions/__init__.py
+-rw-r--r--   0        0        0      214 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/mixology/solutions/providers/__init__.py
+-rw-r--r--   0        0        0     1059 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/mixology/solutions/providers/python_requirement_solution_provider.py
+-rw-r--r--   0        0        0      189 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/mixology/solutions/solutions/__init__.py
+-rw-r--r--   0        0        0     2253 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/mixology/solutions/solutions/python_requirement_solution.py
+-rw-r--r--   0        0        0     6904 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/mixology/term.py
+-rw-r--r--   0        0        0    23682 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/mixology/version_solver.py
+-rw-r--r--   0        0        0      273 2024-03-02 15:26:20.027979 poetry-1.8.2/src/poetry/packages/__init__.py
+-rw-r--r--   0        0        0     1297 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/packages/dependency_package.py
+-rw-r--r--   0        0        0     3146 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/packages/direct_origin.py
+-rw-r--r--   0        0        0    18253 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/packages/locker.py
+-rw-r--r--   0        0        0      921 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/packages/package_collection.py
+-rw-r--r--   0        0        0      185 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/plugins/__init__.py
+-rw-r--r--   0        0        0      687 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/plugins/application_plugin.py
+-rw-r--r--   0        0        0      435 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/plugins/base_plugin.py
+-rw-r--r--   0        0        0      484 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/plugins/plugin.py
+-rw-r--r--   0        0        0     2537 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/plugins/plugin_manager.py
+-rw-r--r--   0        0        0     2491 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/poetry.py
+-rw-r--r--   0        0        0      112 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/publishing/__init__.py
+-rw-r--r--   0        0        0     2933 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/publishing/publisher.py
+-rw-r--r--   0        0        0    12295 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/publishing/uploader.py
+-rw-r--r--   0        0        0       99 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/puzzle/__init__.py
+-rw-r--r--   0        0        0      768 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/puzzle/exceptions.py
+-rw-r--r--   0        0        0    37680 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/puzzle/provider.py
+-rw-r--r--   0        0        0    11114 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/puzzle/solver.py
+-rw-r--r--   0        0        0     5167 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/puzzle/transaction.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/py.typed
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/pyproject/__init__.py
+-rw-r--r--   0        0        0     1740 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/pyproject/toml.py
+-rw-r--r--   0        0        0      198 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/repositories/__init__.py
+-rw-r--r--   0        0        0      809 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/repositories/abstract_repository.py
+-rw-r--r--   0        0        0     2545 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/repositories/cached_repository.py
+-rw-r--r--   0        0        0      173 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/repositories/exceptions.py
+-rw-r--r--   0        0        0    16967 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/repositories/http_repository.py
+-rw-r--r--   0        0        0    10243 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/repositories/installed_repository.py
+-rw-r--r--   0        0        0     4572 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/repositories/legacy_repository.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/repositories/link_sources/__init__.py
+-rw-r--r--   0        0        0     3873 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/repositories/link_sources/base.py
+-rw-r--r--   0        0        0     2611 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/repositories/link_sources/html.py
+-rw-r--r--   0        0        0     1850 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/repositories/link_sources/json.py
+-rw-r--r--   0        0        0      841 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/repositories/lockfile_repository.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/repositories/parsers/__init__.py
+-rw-r--r--   0        0        0      596 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/repositories/parsers/html_page_parser.py
+-rw-r--r--   0        0        0     2480 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/repositories/parsers/pypi_search_parser.py
+-rw-r--r--   0        0        0     7466 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/repositories/pypi_repository.py
+-rw-r--r--   0        0        0     3970 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/repositories/repository.py
+-rw-r--r--   0        0        0     7457 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/repositories/repository_pool.py
+-rw-r--r--   0        0        0      753 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/repositories/single_page_repository.py
+-rw-r--r--   0        0        0      157 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/toml/__init__.py
+-rw-r--r--   0        0        0      198 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/toml/exceptions.py
+-rw-r--r--   0        0        0     1324 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/toml/file.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/__init__.py
+-rw-r--r--   0        0        0     1369 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/_compat.py
+-rw-r--r--   0        0        0    16311 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/authenticator.py
+-rw-r--r--   0        0        0    10192 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/cache.py
+-rw-r--r--   0        0        0      302 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/constants.py
+-rw-r--r--   0        0        0     7648 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/dependency_specification.py
+-rw-r--r--   0        0        0     4164 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/env/__init__.py
+-rw-r--r--   0        0        0    12374 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/env/base_env.py
+-rw-r--r--   0        0        0    26519 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/env/env_manager.py
+-rw-r--r--   0        0        0     2113 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/env/exceptions.py
+-rw-r--r--   0        0        0     3196 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/env/generic_env.py
+-rw-r--r--   0        0        0     2377 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/env/mock_env.py
+-rw-r--r--   0        0        0     1348 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/env/null_env.py
+-rw-r--r--   0        0        0     3280 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/env/script_strings.py
+-rw-r--r--   0        0        0     7425 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/env/site_packages.py
+-rw-r--r--   0        0        0     2597 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/env/system_env.py
+-rw-r--r--   0        0        0     4550 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/env/virtual_env.py
+-rw-r--r--   0        0        0     1857 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/extras.py
+-rw-r--r--   0        0        0    10479 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/helpers.py
+-rw-r--r--   0        0        0     7956 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/password_manager.py
+-rw-r--r--   0        0        0      406 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/patterns.py
+-rw-r--r--   0        0        0     1446 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/pip.py
+-rw-r--r--   0        0        0    12402 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/setup_reader.py
+-rw-r--r--   0        0        0     5211 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/shell.py
+-rw-r--r--   0        0        0      446 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/source.py
+-rw-r--r--   0        0        0     1361 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/utils/wheel.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/vcs/__init__.py
+-rw-r--r--   0        0        0       95 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/vcs/git/__init__.py
+-rw-r--r--   0        0        0    17357 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/vcs/git/backend.py
+-rw-r--r--   0        0        0     1520 2024-03-02 15:26:20.031978 poetry-1.8.2/src/poetry/vcs/git/system.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.035978 poetry-1.8.2/src/poetry/version/__init__.py
+-rw-r--r--   0        0        0     1573 2024-03-02 15:26:20.035978 poetry-1.8.2/src/poetry/version/version_selector.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/config/__init__.py
+-rw-r--r--   0        0        0     3365 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/config/test_config.py
+-rw-r--r--   0        0        0    15253 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/cache/__init__.py
+-rw-r--r--   0        0        0     1334 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/cache/conftest.py
+-rw-r--r--   0        0        0     2324 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/cache/test_clear.py
+-rw-r--r--   0        0        0      832 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/cache/test_list.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/debug/__init__.py
+-rw-r--r--   0        0        0     1807 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/debug/test_resolve.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/env/__init__.py
+-rw-r--r--   0        0        0     2349 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/env/conftest.py
+-rw-r--r--   0        0        0     1417 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/env/helpers.py
+-rw-r--r--   0        0        0     1590 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/env/test_info.py
+-rw-r--r--   0        0        0     2039 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/env/test_list.py
+-rw-r--r--   0        0        0     4061 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/env/test_remove.py
+-rw-r--r--   0        0        0     4701 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/env/test_use.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/self/__init__.py
+-rw-r--r--   0        0        0     2244 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/self/conftest.py
+-rw-r--r--   0        0        0       65 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/self/fixtures/poetry-1.0.5-darwin.sha256sum
+-rw-r--r--   0        0        0     1041 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/self/fixtures/poetry-1.0.5-darwin.tar.gz
+-rw-r--r--   0        0        0     7561 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/self/test_add_plugins.py
+-rw-r--r--   0        0        0     3028 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/self/test_remove_plugins.py
+-rw-r--r--   0        0        0     1596 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/self/test_self_command.py
+-rw-r--r--   0        0        0     5879 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/self/test_show_plugins.py
+-rw-r--r--   0        0        0     2147 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/self/test_update.py
+-rw-r--r--   0        0        0     1167 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/self/utils.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/source/__init__.py
+-rw-r--r--   0        0        0     4105 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/source/conftest.py
+-rw-r--r--   0        0        0    10757 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/source/test_add.py
+-rw-r--r--   0        0        0     2902 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/source/test_remove.py
+-rw-r--r--   0        0        0     4943 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/source/test_show.py
+-rw-r--r--   0        0        0      835 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/test_about.py
+-rw-r--r--   0        0        0    43608 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/test_add.py
+-rw-r--r--   0        0        0     4061 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/test_build.py
+-rw-r--r--   0        0        0     6542 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/test_check.py
+-rw-r--r--   0        0        0    17315 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/test_config.py
+-rw-r--r--   0        0        0      820 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/test_export.py
+-rw-r--r--   0        0        0    30078 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/test_init.py
+-rw-r--r--   0        0        0    16288 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/test_install.py
+-rw-r--r--   0        0        0    10591 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/test_lock.py
+-rw-r--r--   0        0        0     6085 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/test_new.py
+-rw-r--r--   0        0        0     7038 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/test_publish.py
+-rw-r--r--   0        0        0    10936 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/test_remove.py
+-rw-r--r--   0        0        0     6649 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/test_run.py
+-rw-r--r--   0        0        0     2568 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/test_search.py
+-rw-r--r--   0        0        0     2568 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/test_shell.py
+-rw-r--r--   0        0        0    70996 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/test_show.py
+-rw-r--r--   0        0        0     3020 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/test_update.py
+-rw-r--r--   0        0        0     4392 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/commands/test_version.py
+-rw-r--r--   0        0        0     4627 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/logging/__init__.py
+-rw-r--r--   0        0        0     2780 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/logging/test_io_formatter.py
+-rw-r--r--   0        0        0     3336 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/console/test_application.py
+-rw-r--r--   0        0        0       22 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/fixtures/bad_scripts_project/no_colon/README.rst
+-rw-r--r--   0        0        0      729 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/fixtures/bad_scripts_project/no_colon/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/fixtures/bad_scripts_project/no_colon/simple_project/__init__.py
+-rw-r--r--   0        0        0       22 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/fixtures/bad_scripts_project/too_many_colon/README.rst
+-rw-r--r--   0        0        0      727 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/fixtures/bad_scripts_project/too_many_colon/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/fixtures/bad_scripts_project/too_many_colon/simple_project/__init__.py
+-rw-r--r--   0        0        0       22 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/fixtures/build_system_requires_not_available/README.rst
+-rw-r--r--   0        0        0      676 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/fixtures/build_system_requires_not_available/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/fixtures/build_system_requires_not_available/simple_project/__init__.py
+-rw-r--r--   0        0        0     1168 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/fixtures/complete.toml
+-rw-r--r--   0        0        0      406 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/fixtures/deleted_directory_dependency/poetry.lock
+-rw-r--r--   0        0        0      234 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/fixtures/deleted_directory_dependency/pyproject.toml
+-rw-r--r--   0        0        0      428 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/fixtures/deleted_file_dependency/poetry.lock
+-rw-r--r--   0        0        0      234 2024-03-02 15:26:20.035978 poetry-1.8.2/tests/fixtures/deleted_file_dependency/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/directory/project_with_transitive_directory_dependencies/project_with_transitive_directory_dependencies/__init__.py
+-rw-r--r--   0        0        0      418 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/directory/project_with_transitive_directory_dependencies/pyproject.toml
+-rw-r--r--   0        0        0      574 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/directory/project_with_transitive_directory_dependencies/setup.py
+-rw-r--r--   0        0        0      234 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/directory/project_with_transitive_file_dependencies/inner-directory-project/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/directory/project_with_transitive_file_dependencies/project_with_transitive_file_dependencies/__init__.py
+-rw-r--r--   0        0        0      385 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/directory/project_with_transitive_file_dependencies/pyproject.toml
+-rw-r--r--   0        0        0     1116 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1003 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/distributions/demo-0.1.0.tar.gz
+-rw-r--r--   0        0        0     1552 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/distributions/demo-0.1.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1169 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/distributions/demo_invalid_record-0.1.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1307 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/distributions/demo_invalid_record2-0.1.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0      310 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/distributions/demo_missing_dist_info-0.1.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0      594 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/distributions/demo_no_pkg_info-0.1.0.tar.gz
+-rw-r--r--   0        0        0       22 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/excluded_subpackage/README.rst
+-rw-r--r--   0        0        0       59 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/excluded_subpackage/example/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/excluded_subpackage/example/test/__init__.py
+-rw-r--r--   0        0        0      159 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/excluded_subpackage/example/test/excluded.py
+-rw-r--r--   0        0        0      329 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/excluded_subpackage/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/extended_project/README.rst
+-rw-r--r--   0        0        0      362 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/extended_project/build.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/extended_project/extended_project/__init__.py
+-rw-r--r--   0        0        0      652 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/extended_project/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/extended_project_without_setup/README.rst
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/extended_project_without_setup/build.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/extended_project_without_setup/extended_project/__init__.py
+-rw-r--r--   0        0        0      756 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/extended_project_without_setup/pyproject.toml
+-rw-r--r--   0        0        0       18 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/extended_with_no_setup/README.md
+-rw-r--r--   0        0        0      859 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/extended_with_no_setup/build.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/extended_with_no_setup/extended/__init__.py
+-rw-r--r--   0        0        0      888 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/extended_with_no_setup/extended/extended.c
+-rw-r--r--   0        0        0      581 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/extended_with_no_setup/pyproject.toml
+-rw-r--r--   0        0        0       59 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/demo/demo/__init__.py
+-rw-r--r--   0        0        0      226 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/demo/demo.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      164 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/demo/demo.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/demo/demo.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       43 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/demo/demo.egg-info/requires.txt
+-rw-r--r--   0        0        0        5 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/demo/demo.egg-info/top_level.txt
+-rw-r--r--   0        0        0      429 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/demo/setup.py
+-rw-r--r--   0        0        0       93 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/namespace-package-one/namespace_package/__init__.py
+-rw-r--r--   0        0        0       50 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/namespace-package-one/namespace_package/one/__init__.py
+-rw-r--r--   0        0        0      402 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/namespace-package-one/setup.py
+-rw-r--r--   0        0        0       59 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/no-dependencies/demo/__init__.py
+-rw-r--r--   0        0        0      214 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/no-dependencies/demo.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      137 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/no-dependencies/demo.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/no-dependencies/demo.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        5 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/no-dependencies/demo.egg-info/top_level.txt
+-rw-r--r--   0        0        0      329 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/no-dependencies/setup.py
+-rw-r--r--   0        0        0       59 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/no-version/demo/__init__.py
+-rw-r--r--   0        0        0      696 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/no-version/setup.py
+-rw-r--r--   0        0        0      254 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      164 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       43 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/requires.txt
+-rw-r--r--   0        0        0        5 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/top_level.txt
+-rw-r--r--   0        0        0       59 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/non-canonical-name/demo/__init__.py
+-rw-r--r--   0        0        0      429 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/non-canonical-name/setup.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/poetry-plugin/poetry_plugin/__init__.py
+-rw-r--r--   0        0        0      349 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/poetry-plugin/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/poetry-plugin2/subdir/poetry_plugin/__init__.py
+-rw-r--r--   0        0        0      349 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/poetry-plugin2/subdir/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/prerelease/prerelease/__init__.py
+-rw-r--r--   0        0        0      268 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/prerelease/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/pyproject-demo/demo/__init__.py
+-rw-r--r--   0        0        0      275 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/pyproject-demo/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/subdirectories/one/one/__init__.py
+-rw-r--r--   0        0        0      244 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/subdirectories/one/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/subdirectories/one-copy/one/__init__.py
+-rw-r--r--   0        0        0      244 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/subdirectories/one-copy/pyproject.toml
+-rw-r--r--   0        0        0      252 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/subdirectories/two/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/git/github.com/demo/subdirectories/two/two/__init__.py
+-rw-r--r--   0        0        0       34 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/incompatible_lock/poetry.lock
+-rw-r--r--   0        0        0      320 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/incompatible_lock/pyproject.toml
+-rw-r--r--   0        0        0      378 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/inspection/demo/pyproject.toml
+-rw-r--r--   0        0        0      225 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/inspection/demo_no_setup_pkg_info_no_deps/PKG-INFO
+-rw-r--r--   0        0        0      461 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/inspection/demo_no_setup_pkg_info_no_deps/pyproject.toml
+-rw-r--r--   0        0        0      225 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/inspection/demo_only_requires_txt.egg-info/PKG-INFO
+-rw-r--r--   0        0        0       64 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/inspection/demo_only_requires_txt.egg-info/requires.txt
+-rw-r--r--   0        0        0      300 2024-03-02 15:26:20.039979 poetry-1.8.2/tests/fixtures/inspection/demo_poetry_package/pyproject.toml
+-rw-r--r--   0        0        0      225 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/inspection/demo_with_obsolete_egg_info/demo-0.1.0.egg-info/PKG-INFO
+-rw-r--r--   0        0        0       64 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/inspection/demo_with_obsolete_egg_info/demo-0.1.0.egg-info/requires.txt
+-rw-r--r--   0        0        0      378 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/inspection/demo_with_obsolete_egg_info/pyproject.toml
+-rw-r--r--   0        0        0       26 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/invalid_lock/poetry.lock
+-rw-r--r--   0        0        0      320 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/invalid_lock/pyproject.toml
+-rw-r--r--   0        0        0      717 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/invalid_pyproject/pyproject.toml
+-rw-r--r--   0        0        0      406 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/missing_directory_dependency/poetry.lock
+-rw-r--r--   0        0        0      299 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/missing_directory_dependency/pyproject.toml
+-rw-r--r--   0        0        0      467 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/missing_extra_directory_dependency/poetry.lock
+-rw-r--r--   0        0        0      341 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/missing_extra_directory_dependency/pyproject.toml
+-rw-r--r--   0        0        0      428 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/missing_file_dependency/poetry.lock
+-rw-r--r--   0        0        0      324 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/missing_file_dependency/pyproject.toml
+-rw-r--r--   0        0        0      147 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/nameless_pyproject/pyproject.toml
+-rw-r--r--   0        0        0       32 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/no_name_project/README.rst
+-rw-r--r--   0        0        0      306 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/no_name_project/pyproject.toml
+-rw-r--r--   0        0        0      174 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/non_package_mode/pyproject.toml
+-rw-r--r--   0        0        0      762 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/old_lock/poetry.lock
+-rw-r--r--   0        0        0      320 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/old_lock/pyproject.toml
+-rw-r--r--   0        0        0      430 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/old_lock_path_dependency/poetry.lock
+-rw-r--r--   0        0        0      336 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/old_lock_path_dependency/pyproject.toml
+-rw-r--r--   0        0        0      247 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/old_lock_path_dependency/quix/pyproject.toml
+-rw-r--r--   0        0        0     6512 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/outdated_lock/poetry.lock
+-rw-r--r--   0        0        0      311 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/outdated_lock/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/private_pyproject/README.md
+-rw-r--r--   0        0        0      309 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/private_pyproject/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/project_with_extras/project_with_extras/__init__.py
+-rw-r--r--   0        0        0      402 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/project_with_extras/pyproject.toml
+-rw-r--r--   0        0        0      881 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/project_with_git_dev_dependency/pyproject.toml
+-rw-r--r--   0        0        0      893 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/project_with_local_dependencies/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/project_with_multi_constraints_dependency/project/__init__.py
+-rw-r--r--   0        0        0      394 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/project_with_multi_constraints_dependency/pyproject.toml
+-rw-r--r--   0        0        0      264 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/project_with_nested_local/bar/pyproject.toml
+-rw-r--r--   0        0        0      262 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/project_with_nested_local/foo/pyproject.toml
+-rw-r--r--   0        0        0      324 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/project_with_nested_local/pyproject.toml
+-rw-r--r--   0        0        0      221 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/project_with_nested_local/quix/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/project_with_setup/my_package/__init__.py
+-rw-r--r--   0        0        0      239 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/project_with_setup/project_with_setup.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      201 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/project_with_setup/project_with_setup.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/project_with_setup/project_with_setup.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       38 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/project_with_setup/project_with_setup.egg-info/requires.txt
+-rw-r--r--   0        0        0       11 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/project_with_setup/project_with_setup.egg-info/top_level.txt
+-rw-r--r--   0        0        0      416 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/project_with_setup/setup.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/project_with_setup_calls_script/my_package/__init__.py
+-rw-r--r--   0        0        0      105 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/project_with_setup_calls_script/pyproject.toml
+-rw-r--r--   0        0        0      532 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/project_with_setup_calls_script/setup.py
+-rw-r--r--   0        0        0       22 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/sample_project/README.rst
+-rw-r--r--   0        0        0     1501 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/sample_project/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/scripts/README.md
+-rw-r--r--   0        0        0      400 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/scripts/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/scripts/scripts/__init__.py
+-rw-r--r--   0        0        0      557 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/scripts/scripts/check_argv0.py
+-rw-r--r--   0        0        0      122 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/scripts/scripts/exit_code.py
+-rw-r--r--   0        0        0      128 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/scripts/scripts/return_code.py
+-rw-r--r--   0        0        0       22 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/simple_project/README.rst
+-rw-r--r--   0        0        0     1320 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1106 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/simple_project/dist/simple_project-1.2.3.tar.gz
+-rw-r--r--   0        0        0      775 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/simple_project/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/simple_project/simple_project/__init__.py
+-rw-r--r--   0        0        0     6404 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/up_to_date_lock/poetry.lock
+-rw-r--r--   0        0        0      313 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/up_to_date_lock/pyproject.toml
+-rw-r--r--   0        0        0     1722 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/wheel_with_no_requires_dist/demo-0.1.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1062 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/with-include/LICENSE
+-rw-r--r--   0        0        0       22 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/with-include/README.rst
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/with-include/extra_dir/README.md
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/with-include/extra_dir/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/with-include/extra_dir/sub_pkg/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/with-include/extra_dir/sub_pkg/vcs_excluded.txt
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/with-include/extra_dir/vcs_excluded.txt
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/with-include/for_wheel_only/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/with-include/my_module.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/with-include/notes.txt
+-rw-r--r--   0        0        0       59 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/with-include/package_with_include/__init__.py
+-rw-r--r--   0        0        0     1259 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/with-include/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/with-include/src/src_package/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/with-include/tests/__init__.py
+-rw-r--r--   0        0        0      153 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/with_conditional_path_deps/demo_one/pyproject.toml
+-rw-r--r--   0        0        0      153 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/with_conditional_path_deps/demo_two/pyproject.toml
+-rw-r--r--   0        0        0      257 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/with_conditional_path_deps/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/with_default_source/README.rst
+-rw-r--r--   0        0        0     1428 2024-03-02 15:26:20.043979 poetry-1.8.2/tests/fixtures/with_default_source/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_default_source_and_pypi/README.rst
+-rw-r--r--   0        0        0     1467 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_default_source_and_pypi/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_default_source_legacy/README.rst
+-rw-r--r--   0        0        0     1426 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_default_source_legacy/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_default_source_pypi/README.rst
+-rw-r--r--   0        0        0     1393 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_default_source_pypi/pyproject.toml
+-rw-r--r--   0        0        0      370 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_explicit_pypi_and_other/pyproject.toml
+-rw-r--r--   0        0        0      402 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_explicit_pypi_and_other_explicit/pyproject.toml
+-rw-r--r--   0        0        0      301 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_explicit_pypi_no_other/pyproject.toml
+-rw-r--r--   0        0        0      352 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_explicit_source/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_local_config/README.rst
+-rw-r--r--   0        0        0       48 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_local_config/poetry.toml
+-rw-r--r--   0        0        0     1331 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_local_config/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_multiple_dist_dir/README.rst
+-rw-r--r--   0        0        0     1320 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_multiple_dist_dir/dist/simple_project-1.2.3-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1106 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_multiple_dist_dir/dist/simple_project-1.2.3.tar.gz
+-rw-r--r--   0        0        0     1320 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_multiple_dist_dir/other_dist/dist/simple_project-1.2.3-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1106 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_multiple_dist_dir/other_dist/dist/simple_project-1.2.3.tar.gz
+-rw-r--r--   0        0        0      775 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_multiple_dist_dir/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_multiple_dist_dir/simple_project/__init__.py
+-rw-r--r--   0        0        0       28 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_multiple_readme_files/README-1.rst
+-rw-r--r--   0        0        0       20 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_multiple_readme_files/README-2.rst
+-rw-r--r--   0        0        0       79 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_multiple_readme_files/my_package/__init__.py
+-rw-r--r--   0        0        0      286 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_multiple_readme_files/pyproject.toml
+-rw-r--r--   0        0        0      425 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_non_default_multiple_secondary_sources/pyproject.toml
+-rw-r--r--   0        0        0      413 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_non_default_multiple_secondary_sources_legacy/pyproject.toml
+-rw-r--r--   0        0        0      402 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_non_default_multiple_sources/pyproject.toml
+-rw-r--r--   0        0        0      396 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_non_default_multiple_sources_legacy/pyproject.toml
+-rw-r--r--   0        0        0      509 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_non_default_multiple_sources_pypi/pyproject.toml
+-rw-r--r--   0        0        0      333 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_non_default_secondary_source/pyproject.toml
+-rw-r--r--   0        0        0      327 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_non_default_secondary_source_legacy/pyproject.toml
+-rw-r--r--   0        0        0      331 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_non_default_source_explicit/pyproject.toml
+-rw-r--r--   0        0        0      310 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_non_default_source_implicit/pyproject.toml
+-rw-r--r--   0        0        0      214 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_path_dependency/bazz/setup.py
+-rw-r--r--   0        0        0     3370 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_path_dependency/poetry.lock
+-rw-r--r--   0        0        0      305 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_path_dependency/pyproject.toml
+-rw-r--r--   0        0        0      364 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_supplemental_source/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_two_default_sources/README.rst
+-rw-r--r--   0        0        0     1518 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_two_default_sources/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_two_default_sources_legacy/README.rst
+-rw-r--r--   0        0        0     1520 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/fixtures/with_two_default_sources_legacy/pyproject.toml
+-rw-r--r--   0        0        0     9928 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/helpers.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/inspection/__init__.py
+-rw-r--r--   0        0        0    10681 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/inspection/test_info.py
+-rw-r--r--   0        0        0    17215 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/inspection/test_lazy_wheel.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/__init__.py
+-rw-r--r--   0        0        0     1180 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/conftest.py
+-rw-r--r--   0        0        0      564 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/extras-with-dependencies.test
+-rw-r--r--   0        0        0      530 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/extras.test
+-rw-r--r--   0        0        0      402 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/install-no-dev.test
+-rw-r--r--   0        0        0       95 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/no-dependencies.test
+-rw-r--r--   0        0        0     4081 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/old-lock.test
+-rw-r--r--   0        0        0      188 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/remove.test
+-rw-r--r--   0        0        0      188 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/update-with-lock.test
+-rw-r--r--   0        0        0      698 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/update-with-locked-extras.test
+-rw-r--r--   0        0        0      410 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/with-conditional-dependency.test
+-rw-r--r--   0        0        0      509 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/with-dependencies-extras.test
+-rw-r--r--   0        0        0      631 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/with-dependencies-nested-extras.test
+-rw-r--r--   0        0        0      295 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/with-dependencies.test
+-rw-r--r--   0        0        0     2168 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/with-directory-dependency-poetry-transitive.test
+-rw-r--r--   0        0        0      598 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/with-directory-dependency-poetry.test
+-rw-r--r--   0        0        0      641 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/with-directory-dependency-setuptools.test
+-rw-r--r--   0        0        0      471 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/with-duplicate-dependencies-update.test
+-rw-r--r--   0        0        0      853 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/with-duplicate-dependencies.test
+-rw-r--r--   0        0        0     1379 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/with-file-dependency-transitive.test
+-rw-r--r--   0        0        0      676 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/with-file-dependency.test
+-rw-r--r--   0        0        0      764 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/with-multiple-updates.test
+-rw-r--r--   0        0        0      469 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/with-optional-dependencies.test
+-rw-r--r--   0        0        0      565 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/with-platform-dependencies.test
+-rw-r--r--   0        0        0      297 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/with-prereleases.test
+-rw-r--r--   0        0        0     5109 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/with-pypi-repository.test
+-rw-r--r--   0        0        0      424 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/with-python-versions.test
+-rw-r--r--   0        0        0     1146 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/with-same-version-url-dependencies.test
+-rw-r--r--   0        0        0      579 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/with-sub-dependencies.test
+-rw-r--r--   0        0        0      686 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/with-url-dependency.test
+-rw-r--r--   0        0        0      708 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/with-vcs-dependency-with-extras.test
+-rw-r--r--   0        0        0      491 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/with-vcs-dependency-without-ref.test
+-rw-r--r--   0        0        0      478 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/fixtures/with-wheel-dependency-no-requires-dist.test
+-rw-r--r--   0        0        0     6612 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/test_chef.py
+-rw-r--r--   0        0        0    11815 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/test_chooser.py
+-rw-r--r--   0        0        0    49339 2024-03-02 15:26:20.047978 poetry-1.8.2/tests/installation/test_executor.py
+-rw-r--r--   0        0        0    84595 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/installation/test_installer.py
+-rw-r--r--   0        0        0     2706 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/installation/test_wheel_installer.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/integration/__init__.py
+-rw-r--r--   0        0        0    13137 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/integration/test_utils_vcs_git.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/json/__init__.py
+-rw-r--r--   0        0        0      338 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/json/fixtures/source/complete_invalid_priority.toml
+-rw-r--r--   0        0        0      352 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/json/fixtures/source/complete_invalid_priority_legacy_and_new.toml
+-rw-r--r--   0        0        0      282 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/json/fixtures/source/complete_invalid_url.toml
+-rw-r--r--   0        0        0      337 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/json/fixtures/source/complete_valid.toml
+-rw-r--r--   0        0        0      349 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/json/fixtures/source/complete_valid_legacy.toml
+-rw-r--r--   0        0        0     1497 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/json/test_schema_sources.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/masonry/builders/__init__.py
+-rw-r--r--   0        0        0       22 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/masonry/builders/fixtures/excluded_subpackage/README.rst
+-rw-r--r--   0        0        0       59 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/masonry/builders/fixtures/excluded_subpackage/example/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/masonry/builders/fixtures/excluded_subpackage/example/test/__init__.py
+-rw-r--r--   0        0        0      176 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/masonry/builders/fixtures/excluded_subpackage/example/test/excluded.py
+-rw-r--r--   0        0        0      329 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/masonry/builders/fixtures/excluded_subpackage/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/masonry/builders/fixtures/pep_561_stub_only/pkg-stubs/__init__.pyi
+-rw-r--r--   0        0        0       83 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/masonry/builders/fixtures/pep_561_stub_only/pkg-stubs/module.pyi
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/masonry/builders/fixtures/pep_561_stub_only/pkg-stubs/subpkg/__init__.pyi
+-rw-r--r--   0        0        0      261 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/masonry/builders/fixtures/pep_561_stub_only/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/__init__.pyi
+-rw-r--r--   0        0        0       83 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/module.pyi
+-rw-r--r--   0        0        0        8 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/py.typed
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/subpkg/__init__.pyi
+-rw-r--r--   0        0        0      291 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pyproject.toml
+-rw-r--r--   0        0        0      294 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/masonry/builders/fixtures/pep_561_stub_only_src/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/masonry/builders/fixtures/pep_561_stub_only_src/src/pkg-stubs/__init__.pyi
+-rw-r--r--   0        0        0       83 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/masonry/builders/fixtures/pep_561_stub_only_src/src/pkg-stubs/module.pyi
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/masonry/builders/fixtures/pep_561_stub_only_src/src/pkg-stubs/subpkg/__init__.pyi
+-rw-r--r--   0        0        0    11777 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/masonry/builders/test_editable_builder.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/mixology/__init__.py
+-rw-r--r--   0        0        0     2188 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/mixology/helpers.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/mixology/solutions/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/mixology/solutions/providers/__init__.py
+-rw-r--r--   0        0        0     1449 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/mixology/solutions/providers/test_python_requirement_solution_provider.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/mixology/solutions/solutions/__init__.py
+-rw-r--r--   0        0        0     1442 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/mixology/solutions/solutions/test_python_requirement_solution.py
+-rw-r--r--   0        0        0     1572 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/mixology/test_incompatibility.py
+-rw-r--r--   0        0        0      109 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/mixology/version_solver/__init__.py
+-rw-r--r--   0        0        0     1066 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/mixology/version_solver/conftest.py
+-rw-r--r--   0        0        0     7406 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/mixology/version_solver/test_backtracking.py
+-rw-r--r--   0        0        0     4326 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/mixology/version_solver/test_basic_graph.py
+-rw-r--r--   0        0        0     7554 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/mixology/version_solver/test_dependency_cache.py
+-rw-r--r--   0        0        0     1157 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/mixology/version_solver/test_python_constraint.py
+-rw-r--r--   0        0        0     5493 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/mixology/version_solver/test_unsolvable.py
+-rw-r--r--   0        0        0     7700 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/mixology/version_solver/test_with_lock.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/packages/__init__.py
+-rw-r--r--   0        0        0     1935 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/packages/test_direct_origin.py
+-rw-r--r--   0        0        0    30734 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/packages/test_locker.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/plugins/__init__.py
+-rw-r--r--   0        0        0     3299 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/plugins/test_plugin_manager.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/publishing/__init__.py
+-rw-r--r--   0        0        0     6438 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/publishing/test_publisher.py
+-rw-r--r--   0        0        0     4720 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/publishing/test_uploader.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/puzzle/__init__.py
+-rw-r--r--   0        0        0      528 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/puzzle/conftest.py
+-rw-r--r--   0        0        0    30314 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/puzzle/test_provider.py
+-rw-r--r--   0        0        0   148037 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/puzzle/test_solver.py
+-rw-r--r--   0        0        0     5634 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/puzzle/test_transaction.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/pyproject/__init__.py
+-rw-r--r--   0        0        0      813 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/pyproject/conftest.py
+-rw-r--r--   0        0        0     1379 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/pyproject/test_pyproject_toml.py
+-rw-r--r--   0        0        0      755 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/pyproject/test_pyproject_toml_file.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.051978 poetry-1.8.2/tests/repositories/__init__.py
+-rw-r--r--   0        0        0     1474 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/conftest.py
+-rw-r--r--   0        0        0    16009 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/cleo-0.7.6.dist-info/METADATA
+-rw-r--r--   0        0        0      110 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/directory_pep_610-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0       81 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/directory_pep_610-1.2.3.dist-info/direct_url.json
+-rw-r--r--   0        0        0      719 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-2.3.4.dist-info/METADATA
+-rw-r--r--   0        0        0      731 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-with-import-2.3.4.dist-info/METADATA
+-rw-r--r--   0        0        0       10 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-with-import.pth
+-rw-r--r--   0        0        0       18 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable.pth
+-rw-r--r--   0        0        0      119 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable_directory_pep_610-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0      105 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable_directory_pep_610-1.2.3.dist-info/direct_url.json
+-rw-r--r--   0        0        0      105 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/file_pep_610-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0      182 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/file_pep_610-1.2.3.dist-info/direct_url.json
+-rw-r--r--   0        0        0     1306 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/foo-0.1.0-py3.8.egg
+-rw-r--r--   0        0        0      104 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0      159 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610-1.2.3.dist-info/direct_url.json
+-rw-r--r--   0        0        0      125 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610_no_requested_version-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0      141 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610_no_requested_version-1.2.3.dist-info/direct_url.json
+-rw-r--r--   0        0        0      117 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610_subdirectory-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0      200 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610_subdirectory-1.2.3.dist-info/direct_url.json
+-rw-r--r--   0        0        0      719 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/standard-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0        9 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/standard.pth
+-rw-r--r--   0        0        0      104 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/url_pep_610-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0      102 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/url_pep_610-1.2.3.dist-info/direct_url.json
+-rw-r--r--   0        0        0      717 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/bender-2.0.5.dist-info/METADATA
+-rw-r--r--   0        0        0       20 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/bender.pth
+-rw-r--r--   0        0        0      710 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/lib64-2.3.4.dist-info/METADATA
+-rw-r--r--   0        0        0      717 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/src/bender/bender.egg-info/PKG-INFO
+-rw-r--r--   0        0        0     8866 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/src/pendulum/pendulum.egg-info/PKG-INFO
+-rw-r--r--   0        0        0       87 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/src/pendulum/pendulum.egg-info/requires.txt
+-rw-r--r--   0        0        0     9020 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/installed/vendor/py3.7/attrs-19.3.0.dist-info/METADATA
+-rw-r--r--   0        0        0      731 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/legacy/absolute.html
+-rw-r--r--   0        0        0      790 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/legacy/black.html
+-rw-r--r--   0        0        0     1455 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/legacy/clikit.html
+-rw-r--r--   0        0        0      260 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/legacy/demo.html
+-rw-r--r--   0        0        0      746 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/legacy/discord-py.html
+-rw-r--r--   0        0        0      759 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/legacy/futures-partial-yank.html
+-rw-r--r--   0        0        0      747 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/legacy/futures.html
+-rw-r--r--   0        0        0      625 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/legacy/invalid-version.html
+-rw-r--r--   0        0        0     1433 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/legacy/ipython.html
+-rw-r--r--   0        0        0      470 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/legacy/isort-metadata.html
+-rw-r--r--   0        0        0      917 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/legacy/isort.html
+-rw-r--r--   0        0        0      333 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/legacy/jupyter.html
+-rw-r--r--   0        0        0      348 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/legacy/missing-version.html
+-rw-r--r--   0        0        0      401 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/legacy/pastel.html
+-rw-r--r--   0        0        0      534 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/legacy/poetry-test-py2-py3-metadata-merge.html
+-rw-r--r--   0        0        0     1727 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/legacy/pytest-with-extra-packages.html
+-rw-r--r--   0        0        0      802 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/legacy/pytest.html
+-rw-r--r--   0        0        0      467 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/legacy/python-language-server.html
+-rw-r--r--   0        0        0      941 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/legacy/pyyaml.html
+-rw-r--r--   0        0        0      687 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/legacy/relative.html
+-rw-r--r--   0        0        0      473 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/legacy/tomlkit.html
+-rw-r--r--   0        0        0     1223 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/metadata/isort-metadata-4.3.4-py2-none-any.whl.metadata
+-rw-r--r--   0        0        0     1223 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/metadata/isort-metadata-4.3.4-py3-none-any.whl.metadata
+-rw-r--r--   0        0        0    18499 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/SQLAlchemy-1.2.12.tar.gz
+-rw-r--r--   0        0        0     9634 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/Twisted-18.9.0.tar.bz2
+-rw-r--r--   0        0        0     1940 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/black-19.10b0-py36-none-any.whl
+-rw-r--r--   0        0        0    14949 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/black-21.11b0-py3-none-any.whl
+-rw-r--r--   0        0        0    78701 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/cleo-1.0.0a5-py3-none-any.whl
+-rw-r--r--   0        0        0     2329 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/clikit-0.2.4-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     2290 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/discord.py-2.0.0-py3-none-any.whl
+-rw-r--r--   0        0        0    15847 2024-03-02 15:26:20.055978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0-py2-none-any.whl
+-rw-r--r--   0        0        0    18359 2024-03-02 15:26:20.059979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0.tar.gz
+-rw-r--r--   0        0        0    31809 2024-03-02 15:26:20.059979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/importlib_metadata-1.7.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    23473 2024-03-02 15:26:20.059979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py2-none-any.whl
+-rw-r--r--   0        0        0    23475 2024-03-02 15:26:20.059979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py3-none-any.whl
+-rw-r--r--   0        0        0    15795 2024-03-02 15:26:20.059979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0.tar.gz
+-rw-r--r--   0        0        0    22352 2024-03-02 15:26:20.059979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/ipython-7.5.0-py3-none-any.whl
+-rw-r--r--   0        0        0    45393 2024-03-02 15:26:20.059979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py2-none-any.whl
+-rw-r--r--   0        0        0    45352 2024-03-02 15:26:20.059979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py3-none-any.whl
+-rw-r--r--   0        0        0    56070 2024-03-02 15:26:20.059979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4.tar.gz
+-rw-r--r--   0        0        0     2736 2024-03-02 15:26:20.059979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    12916 2024-03-02 15:26:20.059979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0.tar.gz
+-rw-r--r--   0        0        0     4490 2024-03-02 15:26:20.059979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/pastel-0.1.0.tar.gz
+-rw-r--r--   0        0        0   464992 2024-03-02 15:26:20.059979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/poetry_core-1.5.0-py3-none-any.whl
+-rw-r--r--   0        0        0     1213 2024-03-02 15:26:20.059979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py2-none-any.whl
+-rw-r--r--   0        0        0     1218 2024-03-02 15:26:20.059979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0     3691 2024-03-02 15:26:20.059979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/pytest-3.5.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     3708 2024-03-02 15:26:20.059979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/pytest-3.5.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    54076 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/python-language-server-0.21.2.tar.gz
+-rw-r--r--   0        0        0    29813 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.2.tar.gz
+-rw-r--r--   0        0        0    29864 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.3.tar.gz
+-rw-r--r--   0        0        0     5700 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/zipp-3.5.0-py3-none-any.whl
+-rw-r--r--   0        0        0     3421 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/attrs/17.4.0.json
+-rw-r--r--   0        0        0      856 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/attrs.json
+-rw-r--r--   0        0        0    62683 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/black/19.10b0.json
+-rw-r--r--   0        0        0     5924 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/black/21.11b0.json
+-rw-r--r--   0        0        0     1709 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/black.json
+-rw-r--r--   0        0        0     2298 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/cachecontrol/0.12.5.json
+-rw-r--r--   0        0        0     2425 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/cachecontrol.json
+-rw-r--r--   0        0        0     3035 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/cleo/1.0.0a5.json
+-rw-r--r--   0        0        0     3745 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/clikit/0.2.4.json
+-rw-r--r--   0        0        0      997 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/clikit.json
+-rw-r--r--   0        0        0     2922 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/colorama/0.3.9.json
+-rw-r--r--   0        0        0      867 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/colorama.json
+-rw-r--r--   0        0        0     4035 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/discord-py/2.0.0.json
+-rw-r--r--   0        0        0     2944 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/funcsigs/1.0.2.json
+-rw-r--r--   0        0        0      867 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/funcsigs.json
+-rw-r--r--   0        0        0     3838 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/hbmqtt/0.9.6.json
+-rw-r--r--   0        0        0    14437 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/hbmqtt.json
+-rw-r--r--   0        0        0     5331 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/importlib-metadata/1.7.0.json
+-rw-r--r--   0        0        0     1065 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/importlib-metadata.json
+-rw-r--r--   0        0        0     5984 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/ipython/4.1.0rc1.json
+-rw-r--r--   0        0        0    21476 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/isort/4.3.4.json
+-rw-r--r--   0        0        0    21476 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/isort-metadata/4.3.4.json
+-rw-r--r--   0        0        0     1342 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/isort-metadata.json
+-rw-r--r--   0        0        0     1221 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/isort.json
+-rw-r--r--   0        0        0     3969 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/jupyter/1.0.0.json
+-rw-r--r--   0        0        0     1217 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/jupyter.json
+-rw-r--r--   0        0        0     2931 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/lockfile/0.12.2.json
+-rw-r--r--   0        0        0      871 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/lockfile.json
+-rw-r--r--   0        0        0     3552 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/more-itertools/4.1.0.json
+-rw-r--r--   0        0        0     1284 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/more-itertools.json
+-rw-r--r--   0        0        0     2328 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/pluggy/0.6.0.json
+-rw-r--r--   0        0        0      470 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/pluggy.json
+-rw-r--r--   0        0        0     3180 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/poetry/0.12.4.json
+-rw-r--r--   0        0        0     3555 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/poetry-core/1.5.0.json
+-rw-r--r--   0        0        0      897 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/poetry-core.json
+-rw-r--r--   0        0        0     4561 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/poetry.json
+-rw-r--r--   0        0        0     3095 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/py/1.5.3.json
+-rw-r--r--   0        0        0      837 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/py.json
+-rw-r--r--   0        0        0      931 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/pygame-music-grid.json
+-rw-r--r--   0        0        0     4469 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/pylev/1.3.0.json
+-rw-r--r--   0        0        0      495 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/pylev.json
+-rw-r--r--   0        0        0     6933 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/pytest/3.5.0.json
+-rw-r--r--   0        0        0     7555 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/pytest/3.5.1.json
+-rw-r--r--   0        0        0      857 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/pytest.json
+-rw-r--r--   0        0        0    14143 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/pyyaml/3.13.0.json
+-rw-r--r--   0        0        0     7805 2024-03-02 15:26:20.063979 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/pyyaml.json
+-rw-r--r--   0        0        0     3142 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/requests/2.18.4.json
+-rw-r--r--   0        0        0    67409 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/requests.json
+-rw-r--r--   0        0        0     5315 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/setuptools/39.2.0.json
+-rw-r--r--   0        0        0     8423 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/setuptools/67.6.1.json
+-rw-r--r--   0        0        0     1843 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/setuptools.json
+-rw-r--r--   0        0        0     2387 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/six/1.11.0.json
+-rw-r--r--   0        0        0      846 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/six.json
+-rw-r--r--   0        0        0     8870 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/sqlalchemy/1.2.12.json
+-rw-r--r--   0        0        0      484 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/sqlalchemy.json
+-rw-r--r--   0        0        0     6109 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/toga.json
+-rw-r--r--   0        0        0    11126 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/tomlkit/0.5.3.json
+-rw-r--r--   0        0        0     1892 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/tomlkit.json
+-rw-r--r--   0        0        0     3184 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/trackpy/0.4.1.json
+-rw-r--r--   0        0        0      838 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/trackpy.json
+-rw-r--r--   0        0        0    11606 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/twisted/18.9.0.json
+-rw-r--r--   0        0        0      477 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/twisted.json
+-rw-r--r--   0        0        0     4483 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/wheel/0.40.0.json
+-rw-r--r--   0        0        0     1041 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/wheel.json
+-rw-r--r--   0        0        0     5188 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/zipp/3.5.0.json
+-rw-r--r--   0        0        0      907 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/zipp.json
+-rw-r--r--   0        0        0   224197 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/fixtures/pypi.org/search/search.html
+-rw-r--r--   0        0        0     3407 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/fixtures/single-page/jax_releases.html
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/link_sources/__init__.py
+-rw-r--r--   0        0        0     3108 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/link_sources/test_base.py
+-rw-r--r--   0        0        0     5532 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/link_sources/test_html.py
+-rw-r--r--   0        0        0     2522 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/link_sources/test_json.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/parsers/__init__.py
+-rw-r--r--   0        0        0     2219 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/parsers/test_html_page_parser.py
+-rw-r--r--   0        0        0     4176 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/parsers/test_pypi_search_parser.py
+-rw-r--r--   0        0        0     5910 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/test_http_repository.py
+-rw-r--r--   0        0        0    12293 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/test_installed_repository.py
+-rw-r--r--   0        0        0    19821 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/test_legacy_repository.py
+-rw-r--r--   0        0        0     1746 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/test_lockfile_repository.py
+-rw-r--r--   0        0        0    12350 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/test_pypi_repository.py
+-rw-r--r--   0        0        0     2321 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/test_repository.py
+-rw-r--r--   0        0        0    13022 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/test_repository_pool.py
+-rw-r--r--   0        0        0     2084 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/repositories/test_single_page_repository.py
+-rw-r--r--   0        0        0    21940 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/test_factory.py
+-rw-r--r--   0        0        0      399 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/test_helpers.py
+-rw-r--r--   0        0        0     2338 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/types.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/utils/__init__.py
+-rw-r--r--   0        0        0      384 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/utils/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/utils/env/__init__.py
+-rw-r--r--   0        0        0      541 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/utils/env/conftest.py
+-rw-r--r--   0        0        0    18529 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/utils/env/test_env.py
+-rw-r--r--   0        0        0    37640 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/utils/env/test_env_manager.py
+-rw-r--r--   0        0        0     1562 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/utils/env/test_env_site_packages.py
+-rw-r--r--   0        0        0      604 2024-03-02 15:26:20.067978 poetry-1.8.2/tests/utils/fixtures/pyproject.toml
+-rw-r--r--   0        0        0      371 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/fixtures/setups/ansible/requirements.txt
+-rw-r--r--   0        0        0    10765 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/fixtures/setups/ansible/setup.py
+-rw-r--r--   0        0        0      271 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/fixtures/setups/extras_require_with_vars/setup.py
+-rw-r--r--   0        0        0     2581 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/fixtures/setups/flask/setup.py
+-rw-r--r--   0        0        0       75 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/fixtures/setups/minimal/setup.py
+-rw-r--r--   0        0        0     1353 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/fixtures/setups/pendulum/setup.py
+-rw-r--r--   0        0        0    11825 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/fixtures/setups/pyyaml/setup.py
+-rw-r--r--   0        0        0     3366 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/fixtures/setups/requests/setup.py
+-rw-r--r--   0        0        0      290 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/fixtures/setups/setuptools_setup/setup.py
+-rw-r--r--   0        0        0     6272 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/fixtures/setups/sqlalchemy/setup.py
+-rw-r--r--   0        0        0      339 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/fixtures/setups/with-setup-cfg/setup.cfg
+-rw-r--r--   0        0        0       75 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/fixtures/setups/with-setup-cfg/setup.py
+-rw-r--r--   0        0        0      339 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/fixtures/setups/with-setup-cfg-attr/setup.cfg
+-rw-r--r--   0        0        0       75 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/fixtures/setups/with-setup-cfg-attr/setup.py
+-rw-r--r--   0        0        0        0 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/fixtures/setups/with-setup-cfg-minimal/setup.cfg
+-rw-r--r--   0        0        0       75 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/fixtures/setups/with-setup-cfg-minimal/setup.py
+-rw-r--r--   0        0        0    22054 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/test_authenticator.py
+-rw-r--r--   0        0        0    10896 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/test_cache.py
+-rw-r--r--   0        0        0     6069 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/test_dependency_specification.py
+-rw-r--r--   0        0        0     2374 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/test_extras.py
+-rw-r--r--   0        0        0     6830 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/test_helpers.py
+-rw-r--r--   0        0        0    11278 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/test_password_manager.py
+-rw-r--r--   0        0        0     1114 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/test_patterns.py
+-rw-r--r--   0        0        0     1092 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/test_pip.py
+-rw-r--r--   0        0        0     9111 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/test_setup_reader.py
+-rw-r--r--   0        0        0     2182 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/utils/test_source.py
+-rw-r--r--   0        0        0      607 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/vcs/git/test_backend.py
+-rw-r--r--   0        0        0     2588 2024-03-02 15:26:20.071978 poetry-1.8.2/tests/vcs/git/test_system.py
+-rw-r--r--   0        0        0     6839 1970-01-01 00:00:00.000000 poetry-1.8.2/PKG-INFO
```

### Comparing `poetry-1.8.1/LICENSE` & `poetry-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/README.md` & `poetry-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/pyproject.toml` & `poetry-1.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry"
-version = "1.8.1"
+version = "1.8.2"
 description = "Python dependency management and packaging made easy."
 authors = ["Sébastien Eustace <sebastien@eustace.io>"]
 maintainers = [
     "Arun Babu Neelicattu <arun.neelicattu@gmail.com>",
     "Bjorn Neergaard <bjorn@neersighted.com>",
     "Branch Vincent <branchevincent@gmail.com>",
     "Randy Döring <radoering.poetry@gmail.com>",
```

### Comparing `poetry-1.8.1/src/poetry/config/config.py` & `poetry-1.8.2/src/poetry/config/config.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/config/dict_config_source.py` & `poetry-1.8.2/src/poetry/config/dict_config_source.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/config/file_config_source.py` & `poetry-1.8.2/src/poetry/config/file_config_source.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/config/source.py` & `poetry-1.8.2/src/poetry/config/source.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/application.py` & `poetry-1.8.2/src/poetry/console/application.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/command_loader.py` & `poetry-1.8.2/src/poetry/console/command_loader.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/about.py` & `poetry-1.8.2/src/poetry/console/commands/about.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/add.py` & `poetry-1.8.2/src/poetry/console/commands/add.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,17 @@
                 "You can only specify one package when using the --extras option"
             )
 
         # tomlkit types are awkward to work with, treat content as a mostly untyped
         # dictionary.
         content: dict[str, Any] = self.poetry.file.read()
         poetry_content = content["tool"]["poetry"]
-        project_name = canonicalize_name(poetry_content["name"])
+        project_name = (
+            canonicalize_name(name) if (name := poetry_content.get("name")) else None
+        )
 
         if group == MAIN_GROUP:
             if "dependencies" not in poetry_content:
                 poetry_content["dependencies"] = table()
 
             section = poetry_content["dependencies"]
         else:
```

### Comparing `poetry-1.8.1/src/poetry/console/commands/build.py` & `poetry-1.8.2/src/poetry/console/commands/build.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/cache/clear.py` & `poetry-1.8.2/src/poetry/console/commands/cache/clear.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/cache/list.py` & `poetry-1.8.2/src/poetry/console/commands/cache/list.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/check.py` & `poetry-1.8.2/src/poetry/console/commands/check.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/command.py` & `poetry-1.8.2/src/poetry/console/commands/command.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/config.py` & `poetry-1.8.2/src/poetry/console/commands/config.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/debug/info.py` & `poetry-1.8.2/src/poetry/console/commands/debug/info.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/debug/resolve.py` & `poetry-1.8.2/src/poetry/console/commands/debug/resolve.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/env/info.py` & `poetry-1.8.2/src/poetry/console/commands/env/info.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/env/list.py` & `poetry-1.8.2/src/poetry/console/commands/env/list.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/env/remove.py` & `poetry-1.8.2/src/poetry/console/commands/env/remove.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/env/use.py` & `poetry-1.8.2/src/poetry/console/commands/env/use.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/env_command.py` & `poetry-1.8.2/src/poetry/console/commands/env_command.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/export.py` & `poetry-1.8.2/src/poetry/console/commands/export.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/group_command.py` & `poetry-1.8.2/src/poetry/console/commands/group_command.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/init.py` & `poetry-1.8.2/src/poetry/console/commands/init.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/install.py` & `poetry-1.8.2/src/poetry/console/commands/install.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,16 +187,16 @@
             # No need for an editable install in this case.
             self.line("")
             self.line_error(
                 f"Warning: The current project could not be installed: {e}\n"
                 "If you do not want to install the current project"
                 " use <c1>--no-root</c1>.\n"
                 "If you want to use Poetry only for dependency management"
-                " but not for packaging, you can set the operating mode to "
-                '"non-package" in your pyproject.toml file.\n'
+                " but not for packaging, you can disable package mode by setting"
+                " <c1>package-mode = false</> in your pyproject.toml file.\n"
                 "In a future version of Poetry this warning will become an error!",
                 style="warning",
             )
             return 0
 
         if overwrite:
             self.overwrite(log_install.format(tag="success"))
```

### Comparing `poetry-1.8.1/src/poetry/console/commands/installer_command.py` & `poetry-1.8.2/src/poetry/console/commands/installer_command.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/lock.py` & `poetry-1.8.2/src/poetry/console/commands/lock.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/new.py` & `poetry-1.8.2/src/poetry/console/commands/new.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/publish.py` & `poetry-1.8.2/src/poetry/console/commands/publish.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/remove.py` & `poetry-1.8.2/src/poetry/console/commands/remove.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/run.py` & `poetry-1.8.2/src/poetry/console/commands/run.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/search.py` & `poetry-1.8.2/src/poetry/console/commands/search.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/self/add.py` & `poetry-1.8.2/src/poetry/console/commands/self/add.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/self/install.py` & `poetry-1.8.2/src/poetry/console/commands/self/install.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/self/lock.py` & `poetry-1.8.2/src/poetry/console/commands/self/lock.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/self/remove.py` & `poetry-1.8.2/src/poetry/console/commands/self/remove.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/self/self_command.py` & `poetry-1.8.2/src/poetry/console/commands/self/self_command.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/self/show/__init__.py` & `poetry-1.8.2/src/poetry/console/commands/self/show/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/self/show/plugins.py` & `poetry-1.8.2/src/poetry/console/commands/self/show/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/self/update.py` & `poetry-1.8.2/src/poetry/console/commands/self/update.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/shell.py` & `poetry-1.8.2/src/poetry/console/commands/shell.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/show.py` & `poetry-1.8.2/src/poetry/console/commands/show.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/source/add.py` & `poetry-1.8.2/src/poetry/console/commands/source/add.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/source/remove.py` & `poetry-1.8.2/src/poetry/console/commands/source/remove.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/source/show.py` & `poetry-1.8.2/src/poetry/console/commands/source/show.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/update.py` & `poetry-1.8.2/src/poetry/console/commands/update.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/commands/version.py` & `poetry-1.8.2/src/poetry/console/commands/version.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/io/inputs/run_argv_input.py` & `poetry-1.8.2/src/poetry/console/io/inputs/run_argv_input.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/logging/formatters/builder_formatter.py` & `poetry-1.8.2/src/poetry/console/logging/formatters/builder_formatter.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/logging/io_formatter.py` & `poetry-1.8.2/src/poetry/console/logging/io_formatter.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/console/logging/io_handler.py` & `poetry-1.8.2/src/poetry/console/logging/io_handler.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/factory.py` & `poetry-1.8.2/src/poetry/factory.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/inspection/info.py` & `poetry-1.8.2/src/poetry/inspection/info.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/inspection/lazy_wheel.py` & `poetry-1.8.2/src/poetry/inspection/lazy_wheel.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,23 +37,32 @@
 
     from poetry.utils.authenticator import Authenticator
 
 
 logger = logging.getLogger(__name__)
 
 
-class HTTPRangeRequestUnsupported(Exception):
+class LazyWheelUnsupportedError(Exception):
+    """Raised when a lazy wheel is unsupported."""
+
+
+class HTTPRangeRequestUnsupported(LazyWheelUnsupportedError):
     """Raised when the remote server appears unable to support byte ranges."""
 
 
-class UnsupportedWheel(Exception):
+class HTTPRangeRequestNotRespected(LazyWheelUnsupportedError):
+    """Raised when the remote server tells us that it supports byte ranges
+    but does not respect a respective request."""
+
+
+class UnsupportedWheel(LazyWheelUnsupportedError):
     """Unsupported wheel."""
 
 
-class InvalidWheel(Exception):
+class InvalidWheel(LazyWheelUnsupportedError):
     """Invalid (e.g. corrupt) wheel."""
 
     def __init__(self, location: str, name: str) -> None:
         self.location = location
         self.name = name
 
     def __str__(self) -> str:
@@ -81,14 +90,32 @@
         return metadata
 
     except (BadZipFile, UnsupportedWheel):
         # We assume that these errors have occurred because the wheel contents
         # themselves are invalid, not because we've messed up our bookkeeping
         # and produced an invalid file.
         raise InvalidWheel(url, name)
+    except Exception as e:
+        if isinstance(e, LazyWheelUnsupportedError):
+            # this is expected when the code handles issues with lazy wheel metadata retrieval correctly
+            raise e
+
+        logger.debug(
+            "There was an unexpected %s when handling lazy wheel metadata retrieval for %s from %s: %s",
+            type(e).__name__,
+            name,
+            url,
+            e,
+        )
+
+        # Catch all exception to handle any issues that may have occurred during
+        # attempts to use Lazy Wheel.
+        raise LazyWheelUnsupportedError(
+            f"Attempts to use lazy wheel metadata retrieval for {name} from {url} failed"
+        ) from e
 
 
 class MergeIntervals:
     """Stateful bookkeeping to merge interval graphs."""
 
     def __init__(self, *, left: Iterable[int] = (), right: Iterable[int] = ()) -> None:
         self._left = list(left)
@@ -379,15 +406,17 @@
 
     def _content_length_from_head(self) -> int:
         """Performs a HEAD request to extract the Content-Length.
 
         :raises HTTPRangeRequestUnsupported: if the response fails to indicate support
                                              for "bytes" ranges."""
         self._request_count += 1
-        head = self._session.head(self._url, headers=self._uncached_headers())
+        head = self._session.head(
+            self._url, headers=self._uncached_headers(), allow_redirects=True
+        )
         head.raise_for_status()
         assert head.status_code == codes.ok
         accepted_range = head.headers.get("Accept-Ranges", None)
         if accepted_range != "bytes":
             raise HTTPRangeRequestUnsupported(
                 f"server does not support byte ranges: header was '{accepted_range}'"
             )
@@ -403,15 +432,20 @@
         """Return streaming HTTP response to a range request from start to end."""
         headers = self._uncached_headers()
         headers["Range"] = f"bytes={start}-{end}"
         logger.debug("streamed bytes request: %s", headers["Range"])
         self._request_count += 1
         response = self._session.get(self._url, headers=headers, stream=True)
         response.raise_for_status()
-        assert int(response.headers["Content-Length"]) == (end - start + 1)
+        if int(response.headers["Content-Length"]) != (end - start + 1):
+            raise HTTPRangeRequestNotRespected(
+                f"server did not respect byte range request: "
+                f"requested {end - start + 1} bytes, got "
+                f"{response.headers['Content-Length']} bytes"
+            )
         return response
 
     def _fetch_content_range(self, start: int, end: int) -> Iterator[bytes]:
         """Perform a series of HTTP range requests to cover the specified byte range.
 
         NB: For compatibility with HTTP range requests, the range provided to this
         method must *include* the byte indexed at argument ``end`` (so e.g. ``0-1`` is 2
@@ -586,14 +620,20 @@
                 if accept_ranges == "bytes" and content_length <= initial_chunk_size:
                     return content_length, tail
 
             raise HTTPRangeRequestUnsupported(
                 f"did not receive partial content: got code {code}"
             )
 
+        if "Content-Range" not in tail.headers:
+            raise LazyWheelUnsupportedError(
+                f"file length cannot be determined for {self._url}, "
+                f"did not receive content range header from server"
+            )
+
         file_length = self._parse_full_length_from_content_range(
             tail.headers["Content-Range"]
         )
         return (file_length, tail)
 
     def _extract_content_length(
         self, initial_chunk_size: int
@@ -610,18 +650,21 @@
         except HTTPError as e:
             # Our initial request using a negative byte range was not supported.
             resp = e.response
             code = resp.status_code if resp is not None else None
 
             # This indicates that the requested range from the end was larger than the
             # actual file size: https://www.rfc-editor.org/rfc/rfc9110#status.416.
-            if code == codes.requested_range_not_satisfiable:
+            if (
+                code == codes.requested_range_not_satisfiable
+                and resp is not None
+                and "Content-Range" in resp.headers
+            ):
                 # In this case, we don't have any file content yet, but we do know the
                 # size the file will be, so we can return that and exit here.
-                assert resp is not None
                 file_length = self._parse_full_length_from_content_range(
                     resp.headers["Content-Range"]
                 )
                 return file_length, None
 
             # pypi notably does not support negative byte ranges: see
             # https://github.com/pypi/warehouse/issues/12823.
@@ -634,20 +677,20 @@
             # Avoid trying a negative byte range request against this domain for the
             # rest of the resolve.
             self._domains_without_negative_range.add(domain)
             # Apply a HEAD request to get the real size, and nothing else for now.
             return self._content_length_from_head(), None
 
         # Some servers that do not support negative offsets,
-        # handle a negative offset like "-10" as "0-10".
-        if int(
-            tail.headers["Content-Length"]
-        ) == initial_chunk_size + 1 and tail.headers["Content-Range"].startswith(
-            f"bytes 0-{initial_chunk_size}"
-        ):
+        # handle a negative offset like "-10" as "0-10"...
+        # ... or behave even more strangely, see
+        # https://github.com/python-poetry/poetry/issues/9056#issuecomment-1973273721
+        if int(tail.headers["Content-Length"]) > initial_chunk_size or tail.headers.get(
+            "Content-Range", ""
+        ).startswith("bytes -"):
             tail = None
             self._domains_without_negative_range.add(domain)
         return file_length, tail
 
     def _prefetch_metadata(self, name: str) -> str:
         """Locate the *.dist-info/METADATA entry from a temporary ``ZipFile`` wrapper,
         and download it.
```

### Comparing `poetry-1.8.1/src/poetry/installation/chef.py` & `poetry-1.8.2/src/poetry/installation/chef.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/installation/chooser.py` & `poetry-1.8.2/src/poetry/installation/chooser.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/installation/executor.py` & `poetry-1.8.2/src/poetry/installation/executor.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/installation/installer.py` & `poetry-1.8.2/src/poetry/installation/installer.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/installation/operations/install.py` & `poetry-1.8.2/src/poetry/installation/operations/install.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/installation/operations/operation.py` & `poetry-1.8.2/src/poetry/installation/operations/operation.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/installation/operations/uninstall.py` & `poetry-1.8.2/src/poetry/installation/operations/uninstall.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/installation/operations/update.py` & `poetry-1.8.2/src/poetry/installation/operations/update.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/installation/wheel_installer.py` & `poetry-1.8.2/src/poetry/installation/wheel_installer.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/json/__init__.py` & `poetry-1.8.2/src/poetry/json/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/json/schemas/poetry.json` & `poetry-1.8.2/src/poetry/json/schemas/poetry.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/layouts/layout.py` & `poetry-1.8.2/src/poetry/layouts/layout.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/locations.py` & `poetry-1.8.2/src/poetry/locations.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/masonry/builders/editable.py` & `poetry-1.8.2/src/poetry/masonry/builders/editable.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/mixology/assignment.py` & `poetry-1.8.2/src/poetry/mixology/assignment.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/mixology/failure.py` & `poetry-1.8.2/src/poetry/mixology/failure.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/mixology/incompatibility.py` & `poetry-1.8.2/src/poetry/mixology/incompatibility.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/mixology/incompatibility_cause.py` & `poetry-1.8.2/src/poetry/mixology/incompatibility_cause.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/mixology/partial_solution.py` & `poetry-1.8.2/src/poetry/mixology/partial_solution.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/mixology/result.py` & `poetry-1.8.2/src/poetry/mixology/result.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/mixology/solutions/providers/python_requirement_solution_provider.py` & `poetry-1.8.2/src/poetry/mixology/solutions/providers/python_requirement_solution_provider.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/mixology/solutions/solutions/python_requirement_solution.py` & `poetry-1.8.2/src/poetry/mixology/solutions/solutions/python_requirement_solution.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/mixology/term.py` & `poetry-1.8.2/src/poetry/mixology/term.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/mixology/version_solver.py` & `poetry-1.8.2/src/poetry/mixology/version_solver.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/packages/dependency_package.py` & `poetry-1.8.2/src/poetry/packages/dependency_package.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/packages/direct_origin.py` & `poetry-1.8.2/src/poetry/packages/direct_origin.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/packages/locker.py` & `poetry-1.8.2/src/poetry/packages/locker.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/packages/package_collection.py` & `poetry-1.8.2/src/poetry/packages/package_collection.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/plugins/application_plugin.py` & `poetry-1.8.2/src/poetry/plugins/application_plugin.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/plugins/plugin_manager.py` & `poetry-1.8.2/src/poetry/plugins/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/poetry.py` & `poetry-1.8.2/src/poetry/poetry.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/publishing/publisher.py` & `poetry-1.8.2/src/poetry/publishing/publisher.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/publishing/uploader.py` & `poetry-1.8.2/src/poetry/publishing/uploader.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/puzzle/exceptions.py` & `poetry-1.8.2/src/poetry/puzzle/exceptions.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/puzzle/provider.py` & `poetry-1.8.2/src/poetry/puzzle/provider.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/puzzle/solver.py` & `poetry-1.8.2/src/poetry/puzzle/solver.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/puzzle/transaction.py` & `poetry-1.8.2/src/poetry/puzzle/transaction.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/pyproject/toml.py` & `poetry-1.8.2/src/poetry/pyproject/toml.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/repositories/abstract_repository.py` & `poetry-1.8.2/src/poetry/repositories/abstract_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/repositories/cached_repository.py` & `poetry-1.8.2/src/poetry/repositories/cached_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/repositories/http_repository.py` & `poetry-1.8.2/src/poetry/repositories/http_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from poetry.core.constraints.version import parse_constraint
 from poetry.core.packages.dependency import Dependency
 from poetry.core.utils.helpers import temporary_directory
 from poetry.core.version.markers import parse_marker
 
 from poetry.config.config import Config
 from poetry.inspection.info import PackageInfo
-from poetry.inspection.lazy_wheel import HTTPRangeRequestUnsupported
+from poetry.inspection.lazy_wheel import LazyWheelUnsupportedError
 from poetry.inspection.lazy_wheel import metadata_from_wheel_url
 from poetry.repositories.cached_repository import CachedRepository
 from poetry.repositories.exceptions import PackageNotFound
 from poetry.repositories.exceptions import RepositoryError
 from poetry.repositories.link_sources.html import HTMLPage
 from poetry.utils.authenticator import Authenticator
 from poetry.utils.constants import REQUESTS_TIMEOUT
@@ -118,17 +118,21 @@
         # or we don't know yet, we try range requests.
         raise_accepts_ranges = self._lazy_wheel
         if self._lazy_wheel and self._supports_range_requests.get(netloc, True):
             try:
                 package_info = PackageInfo.from_metadata(
                     metadata_from_wheel_url(link.filename, link.url, self.session)
                 )
-            except HTTPRangeRequestUnsupported:
+            except LazyWheelUnsupportedError as e:
                 # Do not set to False if we already know that the domain supports
                 # range requests for some URLs!
+                self._log(
+                    f"Disabling lazy wheel support for {netloc}: {e}",
+                    level="debug",
+                )
                 raise_accepts_ranges = False
                 self._supports_range_requests.setdefault(netloc, False)
             else:
                 self._supports_range_requests[netloc] = True
                 return package_info
 
         try:
@@ -161,15 +165,15 @@
                 response = self.session.get(link.metadata_url)
                 if link.metadata_hashes and (
                     hash_name := get_highest_priority_hash_type(
                         set(link.metadata_hashes.keys()), f"{link.filename}.metadata"
                     )
                 ):
                     metadata_hash = getattr(hashlib, hash_name)(
-                        response.text.encode()
+                        response.content
                     ).hexdigest()
                     if metadata_hash != link.metadata_hashes[hash_name]:
                         self._log(
                             f"Metadata file hash ({metadata_hash}) does not match"
                             f" expected hash ({link.metadata_hashes[hash_name]})."
                             f" Metadata file for {link.filename} will be ignored.",
                             level="warning",
```

### Comparing `poetry-1.8.1/src/poetry/repositories/installed_repository.py` & `poetry-1.8.2/src/poetry/repositories/installed_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/repositories/legacy_repository.py` & `poetry-1.8.2/src/poetry/repositories/legacy_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/repositories/link_sources/base.py` & `poetry-1.8.2/src/poetry/repositories/link_sources/base.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/repositories/link_sources/html.py` & `poetry-1.8.2/src/poetry/repositories/link_sources/html.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/repositories/link_sources/json.py` & `poetry-1.8.2/src/poetry/repositories/link_sources/json.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/repositories/lockfile_repository.py` & `poetry-1.8.2/src/poetry/repositories/lockfile_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/repositories/parsers/html_page_parser.py` & `poetry-1.8.2/src/poetry/repositories/parsers/html_page_parser.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/repositories/parsers/pypi_search_parser.py` & `poetry-1.8.2/src/poetry/repositories/parsers/pypi_search_parser.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/repositories/pypi_repository.py` & `poetry-1.8.2/src/poetry/repositories/pypi_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/repositories/repository.py` & `poetry-1.8.2/src/poetry/repositories/repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/repositories/repository_pool.py` & `poetry-1.8.2/src/poetry/repositories/repository_pool.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/repositories/single_page_repository.py` & `poetry-1.8.2/src/poetry/repositories/single_page_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/toml/file.py` & `poetry-1.8.2/src/poetry/toml/file.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/utils/_compat.py` & `poetry-1.8.2/src/poetry/utils/_compat.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/utils/authenticator.py` & `poetry-1.8.2/src/poetry/utils/authenticator.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/utils/cache.py` & `poetry-1.8.2/src/poetry/utils/cache.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/utils/dependency_specification.py` & `poetry-1.8.2/src/poetry/utils/dependency_specification.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/utils/env/__init__.py` & `poetry-1.8.2/src/poetry/utils/env/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/utils/env/base_env.py` & `poetry-1.8.2/src/poetry/utils/env/base_env.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/utils/env/env_manager.py` & `poetry-1.8.2/src/poetry/utils/env/env_manager.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/utils/env/exceptions.py` & `poetry-1.8.2/src/poetry/utils/env/exceptions.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/utils/env/generic_env.py` & `poetry-1.8.2/src/poetry/utils/env/generic_env.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/utils/env/mock_env.py` & `poetry-1.8.2/src/poetry/utils/env/mock_env.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/utils/env/null_env.py` & `poetry-1.8.2/src/poetry/utils/env/null_env.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/utils/env/script_strings.py` & `poetry-1.8.2/src/poetry/utils/env/script_strings.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/utils/env/site_packages.py` & `poetry-1.8.2/src/poetry/utils/env/site_packages.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/utils/env/system_env.py` & `poetry-1.8.2/src/poetry/utils/env/system_env.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/utils/env/virtual_env.py` & `poetry-1.8.2/src/poetry/utils/env/virtual_env.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/utils/extras.py` & `poetry-1.8.2/src/poetry/utils/extras.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/utils/helpers.py` & `poetry-1.8.2/src/poetry/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/utils/password_manager.py` & `poetry-1.8.2/src/poetry/utils/password_manager.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/utils/pip.py` & `poetry-1.8.2/src/poetry/utils/pip.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/utils/setup_reader.py` & `poetry-1.8.2/src/poetry/utils/setup_reader.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/utils/shell.py` & `poetry-1.8.2/src/poetry/utils/shell.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/utils/wheel.py` & `poetry-1.8.2/src/poetry/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/vcs/git/backend.py` & `poetry-1.8.2/src/poetry/vcs/git/backend.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/vcs/git/system.py` & `poetry-1.8.2/src/poetry/vcs/git/system.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/src/poetry/version/version_selector.py` & `poetry-1.8.2/src/poetry/version/version_selector.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/config/test_config.py` & `poetry-1.8.2/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/conftest.py` & `poetry-1.8.2/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from poetry.utils.env import EnvManager
 from poetry.utils.env import SystemEnv
 from poetry.utils.env import VirtualEnv
 from tests.helpers import MOCK_DEFAULT_GIT_REVISION
 from tests.helpers import TestLocker
 from tests.helpers import TestRepository
 from tests.helpers import get_package
+from tests.helpers import http_setup_redirect
 from tests.helpers import isolated_environment
 from tests.helpers import mock_clone
 from tests.helpers import mock_download
 
 
 if TYPE_CHECKING:
     from collections.abc import Iterator
@@ -318,14 +319,19 @@
 def http() -> Iterator[type[httpretty.httpretty]]:
     httpretty.reset()
     with httpretty.enabled(allow_net_connect=False):
         yield httpretty
 
 
 @pytest.fixture
+def http_redirector(http: type[httpretty.httpretty]) -> None:
+    http_setup_redirect(http, http.HEAD, http.GET, http.PUT, http.POST)
+
+
+@pytest.fixture
 def project_root() -> Path:
     return Path(__file__).parent.parent
 
 
 @pytest.fixture(scope="session")
 def fixture_base() -> Path:
     return Path(__file__).parent / "fixtures"
@@ -509,7 +515,13 @@
 def venv_flags_default() -> dict[str, bool]:
     return {
         "always-copy": False,
         "system-site-packages": False,
         "no-pip": False,
         "no-setuptools": False,
     }
+
+
+@pytest.fixture(autouse=(os.name == "nt"))
+def httpretty_windows_mock_urllib3_wait_for_socket(mocker: MockerFixture) -> None:
+    # this is a workaround for https://github.com/gabrielfalcao/HTTPretty/issues/442
+    mocker.patch("urllib3.util.wait.select_wait_for_socket", returns=True)
```

### Comparing `poetry-1.8.1/tests/console/commands/cache/conftest.py` & `poetry-1.8.2/tests/console/commands/cache/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/cache/test_clear.py` & `poetry-1.8.2/tests/console/commands/cache/test_clear.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/cache/test_list.py` & `poetry-1.8.2/tests/console/commands/cache/test_list.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/debug/test_resolve.py` & `poetry-1.8.2/tests/console/commands/debug/test_resolve.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/env/conftest.py` & `poetry-1.8.2/tests/console/commands/env/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/env/helpers.py` & `poetry-1.8.2/tests/console/commands/env/helpers.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/env/test_info.py` & `poetry-1.8.2/tests/console/commands/env/test_info.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/env/test_list.py` & `poetry-1.8.2/tests/console/commands/env/test_list.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/env/test_remove.py` & `poetry-1.8.2/tests/console/commands/env/test_remove.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/env/test_use.py` & `poetry-1.8.2/tests/console/commands/env/test_use.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/self/conftest.py` & `poetry-1.8.2/tests/console/commands/self/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/self/fixtures/poetry-1.0.5-darwin.tar.gz` & `poetry-1.8.2/tests/console/commands/self/fixtures/poetry-1.0.5-darwin.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/self/test_add_plugins.py` & `poetry-1.8.2/tests/console/commands/self/test_add_plugins.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/self/test_remove_plugins.py` & `poetry-1.8.2/tests/console/commands/self/test_remove_plugins.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/self/test_self_command.py` & `poetry-1.8.2/tests/console/commands/self/test_self_command.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/self/test_show_plugins.py` & `poetry-1.8.2/tests/console/commands/self/test_show_plugins.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/self/test_update.py` & `poetry-1.8.2/tests/console/commands/self/test_update.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/self/utils.py` & `poetry-1.8.2/tests/console/commands/self/utils.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/source/conftest.py` & `poetry-1.8.2/tests/console/commands/source/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/source/test_add.py` & `poetry-1.8.2/tests/console/commands/source/test_add.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/source/test_remove.py` & `poetry-1.8.2/tests/console/commands/source/test_remove.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/source/test_show.py` & `poetry-1.8.2/tests/console/commands/source/test_show.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/test_about.py` & `poetry-1.8.2/tests/console/commands/test_about.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/test_add.py` & `poetry-1.8.2/tests/console/commands/test_add.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,37 @@
     pyproject: dict[str, Any] = app.poetry.file.read()
     content = pyproject["tool"]["poetry"]
 
     assert "cachy" in content["dependencies"]
     assert content["dependencies"]["cachy"] == "^0.2.0"
 
 
+def test_add_non_package_mode_no_name(
+    repo: TestRepository,
+    project_factory: ProjectFactory,
+    command_tester_factory: CommandTesterFactory,
+) -> None:
+    repo.add_package(get_package("cachy", "0.2.0"))
+
+    poetry = project_factory(
+        name="foobar", pyproject_content="[tool.poetry]\npackage-mode = false\n"
+    )
+    tester = command_tester_factory("add", poetry=poetry)
+    tester.execute("cachy")
+
+    assert isinstance(tester.command, InstallerCommand)
+    assert tester.command.installer.executor.installations_count == 1
+
+    pyproject: dict[str, Any] = poetry.file.read()
+    content = pyproject["tool"]["poetry"]
+
+    assert "cachy" in content["dependencies"]
+    assert content["dependencies"]["cachy"] == "^0.2.0"
+
+
 def test_add_replace_by_constraint(
     app: PoetryTestApplication, repo: TestRepository, tester: CommandTester
 ) -> None:
     repo.add_package(get_package("cachy", "0.1.0"))
     repo.add_package(get_package("cachy", "0.2.0"))
 
     tester.execute("cachy")
```

### Comparing `poetry-1.8.1/tests/console/commands/test_build.py` & `poetry-1.8.2/tests/console/commands/test_build.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/test_check.py` & `poetry-1.8.2/tests/console/commands/test_check.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/test_config.py` & `poetry-1.8.2/tests/console/commands/test_config.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/test_export.py` & `poetry-1.8.2/tests/console/commands/test_export.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/test_init.py` & `poetry-1.8.2/tests/console/commands/test_init.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/test_install.py` & `poetry-1.8.2/tests/console/commands/test_install.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/test_lock.py` & `poetry-1.8.2/tests/console/commands/test_lock.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/test_new.py` & `poetry-1.8.2/tests/console/commands/test_new.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/test_publish.py` & `poetry-1.8.2/tests/console/commands/test_publish.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/test_remove.py` & `poetry-1.8.2/tests/console/commands/test_remove.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/test_run.py` & `poetry-1.8.2/tests/console/commands/test_run.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/test_search.py` & `poetry-1.8.2/tests/console/commands/test_search.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/test_shell.py` & `poetry-1.8.2/tests/console/commands/test_shell.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/test_show.py` & `poetry-1.8.2/tests/console/commands/test_show.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/test_update.py` & `poetry-1.8.2/tests/console/commands/test_update.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/commands/test_version.py` & `poetry-1.8.2/tests/console/commands/test_version.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/conftest.py` & `poetry-1.8.2/tests/console/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/logging/test_io_formatter.py` & `poetry-1.8.2/tests/console/logging/test_io_formatter.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/console/test_application.py` & `poetry-1.8.2/tests/console/test_application.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/bad_scripts_project/no_colon/pyproject.toml` & `poetry-1.8.2/tests/fixtures/bad_scripts_project/no_colon/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/bad_scripts_project/too_many_colon/pyproject.toml` & `poetry-1.8.2/tests/fixtures/bad_scripts_project/too_many_colon/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/build_system_requires_not_available/pyproject.toml` & `poetry-1.8.2/tests/fixtures/build_system_requires_not_available/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/complete.toml` & `poetry-1.8.2/tests/fixtures/complete.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/directory/project_with_transitive_directory_dependencies/setup.py` & `poetry-1.8.2/tests/fixtures/directory/project_with_transitive_directory_dependencies/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl` & `poetry-1.8.2/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/distributions/demo-0.1.0.tar.gz` & `poetry-1.8.2/tests/fixtures/distributions/demo-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/distributions/demo-0.1.2-py2.py3-none-any.whl` & `poetry-1.8.2/tests/fixtures/distributions/demo-0.1.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/distributions/demo_invalid_record-0.1.0-py2.py3-none-any.whl` & `poetry-1.8.2/tests/fixtures/distributions/demo_invalid_record-0.1.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/distributions/demo_invalid_record2-0.1.0-py2.py3-none-any.whl` & `poetry-1.8.2/tests/fixtures/distributions/demo_invalid_record2-0.1.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/distributions/demo_no_pkg_info-0.1.0.tar.gz` & `poetry-1.8.2/tests/fixtures/distributions/demo_no_pkg_info-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/extended_project/pyproject.toml` & `poetry-1.8.2/tests/fixtures/extended_project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/extended_project_without_setup/pyproject.toml` & `poetry-1.8.2/tests/fixtures/extended_project_without_setup/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/extended_with_no_setup/build.py` & `poetry-1.8.2/tests/fixtures/extended_with_no_setup/build.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/extended_with_no_setup/extended/extended.c` & `poetry-1.8.2/tests/fixtures/extended_with_no_setup/extended/extended.c`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/extended_with_no_setup/pyproject.toml` & `poetry-1.8.2/tests/fixtures/extended_with_no_setup/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/git/github.com/demo/no-version/setup.py` & `poetry-1.8.2/tests/fixtures/git/github.com/demo/no-version/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/invalid_pyproject/pyproject.toml` & `poetry-1.8.2/tests/fixtures/invalid_pyproject/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/old_lock/poetry.lock` & `poetry-1.8.2/tests/fixtures/old_lock/poetry.lock`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/outdated_lock/poetry.lock` & `poetry-1.8.2/tests/fixtures/outdated_lock/poetry.lock`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/project_with_git_dev_dependency/pyproject.toml` & `poetry-1.8.2/tests/fixtures/project_with_git_dev_dependency/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/project_with_local_dependencies/pyproject.toml` & `poetry-1.8.2/tests/fixtures/project_with_local_dependencies/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/project_with_setup_calls_script/setup.py` & `poetry-1.8.2/tests/fixtures/project_with_setup_calls_script/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/sample_project/pyproject.toml` & `poetry-1.8.2/tests/fixtures/sample_project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/scripts/scripts/check_argv0.py` & `poetry-1.8.2/tests/fixtures/scripts/scripts/check_argv0.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl` & `poetry-1.8.2/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/simple_project/dist/simple_project-1.2.3.tar.gz` & `poetry-1.8.2/tests/fixtures/simple_project/dist/simple_project-1.2.3.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/simple_project/pyproject.toml` & `poetry-1.8.2/tests/fixtures/simple_project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/up_to_date_lock/poetry.lock` & `poetry-1.8.2/tests/fixtures/up_to_date_lock/poetry.lock`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/wheel_with_no_requires_dist/demo-0.1.0-py2.py3-none-any.whl` & `poetry-1.8.2/tests/fixtures/wheel_with_no_requires_dist/demo-0.1.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/with-include/LICENSE` & `poetry-1.8.2/tests/fixtures/with-include/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/with-include/pyproject.toml` & `poetry-1.8.2/tests/fixtures/with-include/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/with_default_source/pyproject.toml` & `poetry-1.8.2/tests/fixtures/with_default_source/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/with_default_source_and_pypi/pyproject.toml` & `poetry-1.8.2/tests/fixtures/with_default_source_and_pypi/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/with_default_source_legacy/pyproject.toml` & `poetry-1.8.2/tests/fixtures/with_default_source_legacy/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/with_default_source_pypi/pyproject.toml` & `poetry-1.8.2/tests/fixtures/with_default_source_pypi/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/with_local_config/pyproject.toml` & `poetry-1.8.2/tests/fixtures/with_local_config/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/with_multiple_dist_dir/dist/simple_project-1.2.3-py2.py3-none-any.whl` & `poetry-1.8.2/tests/fixtures/with_multiple_dist_dir/dist/simple_project-1.2.3-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/with_multiple_dist_dir/dist/simple_project-1.2.3.tar.gz` & `poetry-1.8.2/tests/fixtures/with_multiple_dist_dir/dist/simple_project-1.2.3.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/with_multiple_dist_dir/other_dist/dist/simple_project-1.2.3-py2.py3-none-any.whl` & `poetry-1.8.2/tests/fixtures/with_multiple_dist_dir/other_dist/dist/simple_project-1.2.3-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/with_multiple_dist_dir/other_dist/dist/simple_project-1.2.3.tar.gz` & `poetry-1.8.2/tests/fixtures/with_multiple_dist_dir/other_dist/dist/simple_project-1.2.3.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/with_multiple_dist_dir/pyproject.toml` & `poetry-1.8.2/tests/fixtures/with_multiple_dist_dir/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/with_path_dependency/poetry.lock` & `poetry-1.8.2/tests/fixtures/with_path_dependency/poetry.lock`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/with_two_default_sources/pyproject.toml` & `poetry-1.8.2/tests/fixtures/with_two_default_sources/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/fixtures/with_two_default_sources_legacy/pyproject.toml` & `poetry-1.8.2/tests/fixtures/with_two_default_sources_legacy/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/helpers.py` & `poetry-1.8.2/tests/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,23 +25,27 @@
 
 
 if TYPE_CHECKING:
     from collections.abc import Iterator
     from typing import Any
     from typing import Mapping
 
+    import httpretty
+
+    from httpretty.core import HTTPrettyRequest
     from poetry.core.constraints.version import Version
     from poetry.core.packages.dependency import Dependency
     from pytest_mock import MockerFixture
     from requests import Session
     from tomlkit.toml_document import TOMLDocument
 
     from poetry.installation.operations.operation import Operation
     from poetry.poetry import Poetry
     from poetry.utils.authenticator import Authenticator
+    from tests.types import HTTPrettyResponse
 
 FIXTURE_PATH = Path(__file__).parent / "fixtures"
 
 # Used as a mock for latest git revision.
 MOCK_DEFAULT_GIT_REVISION = "9cf87a285a2d3fbb0b9fa621997b3acc3631ed24"
 
 
@@ -317,7 +321,29 @@
                     leaf_path, leaf_value = leaf
                     leaf_path.insert(0, key)
                     yield (leaf_path, leaf_value)
         else:
             yield ([], obj)
 
     return {delimiter.join(path): value for path, value in recurse_keys(obj)}
+
+
+def http_setup_redirect(
+    http: type[httpretty.httpretty], *methods: str, status_code: int = 301
+) -> None:
+    redirect_uri_regex = re.compile("^(?P<protocol>https?)://redirect.(?P<uri>.*)$")
+
+    def redirect_request_callback(
+        request: HTTPrettyRequest, uri: str, headers: dict[str, Any]
+    ) -> HTTPrettyResponse:
+        redirect_uri_match = redirect_uri_regex.match(uri)
+        assert redirect_uri_match is not None
+        redirect_uri = f"{redirect_uri_match.group('protocol')}://{redirect_uri_match.group('uri')}"
+        return status_code, {"Location": redirect_uri}, b""
+
+    for method in methods:
+        http.register_uri(
+            method,
+            redirect_uri_regex,
+            status=status_code,
+            body=redirect_request_callback,
+        )
```

### Comparing `poetry-1.8.1/tests/inspection/test_info.py` & `poetry-1.8.2/tests/inspection/test_info.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/inspection/test_lazy_wheel.py` & `poetry-1.8.2/tests/inspection/test_lazy_wheel.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,67 @@
 from __future__ import annotations
 
 import re
 
+from enum import IntEnum
 from pathlib import Path
 from typing import TYPE_CHECKING
 from typing import Any
-from typing import Dict
 from typing import Protocol
-from typing import Tuple
 from urllib.parse import urlparse
 
-import httpretty
 import pytest
 import requests
 
 from requests import codes
 
+from poetry.inspection.lazy_wheel import HTTPRangeRequestNotRespected
 from poetry.inspection.lazy_wheel import HTTPRangeRequestUnsupported
 from poetry.inspection.lazy_wheel import InvalidWheel
+from poetry.inspection.lazy_wheel import LazyWheelUnsupportedError
 from poetry.inspection.lazy_wheel import metadata_from_wheel_url
+from tests.helpers import http_setup_redirect
 
 
 if TYPE_CHECKING:
-    from collections.abc import Callable
+    import httpretty
 
     from httpretty.core import HTTPrettyRequest
+    from pytest_mock import MockerFixture
 
     from tests.types import FixtureDirGetter
-
-    HTTPrettyResponse = Tuple[int, Dict[str, Any], bytes]  # status code, headers, body
-    HTTPrettyRequestCallback = Callable[
-        [HTTPrettyRequest, str, Dict[str, Any]], HTTPrettyResponse
-    ]
+    from tests.types import HTTPPrettyRequestCallbackWrapper
+    from tests.types import HTTPrettyRequestCallback
+    from tests.types import HTTPrettyResponse
 
     class RequestCallbackFactory(Protocol):
         def __call__(
             self,
             *,
             accept_ranges: str | None = "bytes",
             negative_offset_error: tuple[int, bytes] | None = None,
+            ignore_accept_ranges: bool = False,
         ) -> HTTPrettyRequestCallback: ...
 
+    class AssertMetadataFromWheelUrl(Protocol):
+        def __call__(
+            self,
+            *,
+            accept_ranges: str | None = "bytes",
+            negative_offset_error: tuple[int, bytes] | None = None,
+            expected_requests: int = 3,
+            request_callback_wrapper: HTTPPrettyRequestCallbackWrapper | None = None,
+            redirect: bool = True,
+        ) -> None: ...
+
 
-NEGATIVE_OFFSET_AS_POSITIVE = -1
+class NegativeOffsetFailure(IntEnum):
+    # numbers must be negative to avoid conflicts with HTTP status codes
+    as_positive = -1  # JFrog Artifactory bug (RTDEV-38572)
+    one_more = -2  # JFrog Artifactory bug (one more byte than requested)
 
 
 def build_head_response(
     accept_ranges: str | None, content_length: int, response_headers: dict[str, Any]
 ) -> HTTPrettyResponse:
     response_headers["Content-Length"] = content_length
     if accept_ranges:
@@ -55,27 +70,34 @@
 
 
 def build_partial_response(
     rng: str,
     wheel_bytes: bytes,
     response_headers: dict[str, Any],
     *,
-    negative_offset_as_positive: bool = False,
+    negative_offset_failure: NegativeOffsetFailure | None = None,
 ) -> HTTPrettyResponse:
     status_code = 206
     response_headers["Accept-Ranges"] = "bytes"
     total_length = len(wheel_bytes)
     if rng.startswith("-"):
         # negative offset
         offset = int(rng)
-        if negative_offset_as_positive:
+        if negative_offset_failure == NegativeOffsetFailure.as_positive:
             # some servers interpret a negative offset like "-10" as "0-10"
             start = 0
             end = min(-offset, total_length - 1)
             body = wheel_bytes[start : end + 1]
+        elif negative_offset_failure == NegativeOffsetFailure.one_more:
+            # https://github.com/python-poetry/poetry/issues/9056#issuecomment-1973273721
+            offset -= 1  # one more byte
+            start = total_length + offset  # negative start of content range possible!
+            end = total_length - 1
+            body = wheel_bytes[offset:]
+            response_headers["Content-Length"] = -offset  # just wrong...
         else:
             start = total_length + offset
             if start < 0:
                 # wheel is smaller than initial chunk size
                 return 200, response_headers, wheel_bytes
             end = total_length - 1
             body = wheel_bytes[offset:]
@@ -89,14 +111,15 @@
 
 @pytest.fixture
 def handle_request_factory(fixture_dir: FixtureDirGetter) -> RequestCallbackFactory:
     def _factory(
         *,
         accept_ranges: str | None = "bytes",
         negative_offset_error: tuple[int, bytes] | None = None,
+        ignore_accept_ranges: bool = False,
     ) -> HTTPrettyRequestCallback:
         def handle_request(
             request: HTTPrettyRequest, uri: str, response_headers: dict[str, Any]
         ) -> HTTPrettyResponse:
             name = Path(urlparse(uri).path).name
 
             wheel = Path(__file__).parents[1] / (
@@ -118,139 +141,231 @@
             if request.method == "HEAD":
                 return build_head_response(
                     accept_ranges, len(wheel_bytes), response_headers
                 )
 
             rng = request.headers.get("Range", "=").split("=")[1]
 
-            negative_offset_as_positive = False
+            negative_offset_failure = None
             if negative_offset_error and rng.startswith("-"):
                 if negative_offset_error[0] == codes.requested_range_not_satisfiable:
                     response_headers["Content-Range"] = f"bytes */{len(wheel_bytes)}"
-                if negative_offset_error[0] == NEGATIVE_OFFSET_AS_POSITIVE:
-                    negative_offset_as_positive = True
+                if negative_offset_error[0] == NegativeOffsetFailure.as_positive:
+                    negative_offset_failure = NegativeOffsetFailure.as_positive
+                elif negative_offset_error[0] == NegativeOffsetFailure.one_more:
+                    negative_offset_failure = NegativeOffsetFailure.one_more
                 else:
                     return (
                         negative_offset_error[0],
                         response_headers,
                         negative_offset_error[1],
                     )
-            if accept_ranges == "bytes" and rng:
+            if accept_ranges == "bytes" and rng and not ignore_accept_ranges:
                 return build_partial_response(
                     rng,
                     wheel_bytes,
                     response_headers,
-                    negative_offset_as_positive=negative_offset_as_positive,
+                    negative_offset_failure=negative_offset_failure,
                 )
 
             status_code = 200
             body = wheel_bytes
 
             return status_code, response_headers, body
 
         return handle_request
 
     return _factory
 
 
+@pytest.fixture
+def assert_metadata_from_wheel_url(
+    http: type[httpretty.httpretty],
+    handle_request_factory: RequestCallbackFactory,
+) -> AssertMetadataFromWheelUrl:
+    def _assertion(
+        *,
+        accept_ranges: str | None = "bytes",
+        negative_offset_error: tuple[int, bytes] | None = None,
+        expected_requests: int = 3,
+        request_callback_wrapper: HTTPPrettyRequestCallbackWrapper | None = None,
+        redirect: bool = False,
+    ) -> None:
+        latest_requests = http.latest_requests()
+        latest_requests.clear()
+
+        domain = (
+            f"lazy-wheel-{negative_offset_error[0] if negative_offset_error else 0}.com"
+        )
+        uri_regex = re.compile(f"^https://{domain}/.*$")
+        request_callback = handle_request_factory(
+            accept_ranges=accept_ranges, negative_offset_error=negative_offset_error
+        )
+        if request_callback_wrapper is not None:
+            request_callback = request_callback_wrapper(request_callback)
+
+        http.register_uri(http.GET, uri_regex, body=request_callback)
+        http.register_uri(http.HEAD, uri_regex, body=request_callback)
+
+        if redirect:
+            http_setup_redirect(http, http.GET, http.HEAD)
+
+        url_prefix = "redirect." if redirect else ""
+        url = f"https://{url_prefix}{domain}/poetry_core-1.5.0-py3-none-any.whl"
+
+        metadata = metadata_from_wheel_url("poetry-core", url, requests.Session())
+
+        assert metadata["name"] == "poetry-core"
+        assert metadata["version"] == "1.5.0"
+        assert metadata["author"] == "Sébastien Eustace"
+        assert metadata["requires_dist"] == [
+            'importlib-metadata (>=1.7.0) ; python_version < "3.8"'
+        ]
+
+        assert len(latest_requests) == expected_requests
+
+    return _assertion
+
+
 @pytest.mark.parametrize(
     "negative_offset_error",
     [
         None,
         (codes.not_found, b"Not found"),  # Nexus
         (codes.method_not_allowed, b"Method not allowed"),
         (codes.requested_range_not_satisfiable, b"Requested range not satisfiable"),
         (codes.internal_server_error, b"Internal server error"),  # GAR
         (codes.not_implemented, b"Unsupported client range"),  # PyPI
-        (NEGATIVE_OFFSET_AS_POSITIVE, b"handle negative offset as positive"),
+        (NegativeOffsetFailure.as_positive, b"handle negative offset as positive"),
+        (NegativeOffsetFailure.one_more, b"one more byte than requested"),
     ],
 )
 def test_metadata_from_wheel_url(
-    http: type[httpretty.httpretty],
-    handle_request_factory: RequestCallbackFactory,
+    assert_metadata_from_wheel_url: AssertMetadataFromWheelUrl,
     negative_offset_error: tuple[int, bytes] | None,
 ) -> None:
-    domain = (
-        f"lazy-wheel-{negative_offset_error[0] if negative_offset_error else 0}.com"
-    )
-    uri_regex = re.compile(f"^https://{domain}/.*$")
-    request_callback = handle_request_factory(
-        negative_offset_error=negative_offset_error
-    )
-    http.register_uri(http.GET, uri_regex, body=request_callback)
-    http.register_uri(http.HEAD, uri_regex, body=request_callback)
-
-    url = f"https://{domain}/poetry_core-1.5.0-py3-none-any.whl"
-
-    metadata = metadata_from_wheel_url("poetry-core", url, requests.Session())
-
-    assert metadata["name"] == "poetry-core"
-    assert metadata["version"] == "1.5.0"
-    assert metadata["author"] == "Sébastien Eustace"
-    assert metadata["requires_dist"] == [
-        'importlib-metadata (>=1.7.0) ; python_version < "3.8"'
-    ]
-
     # negative offsets supported:
     # 1. end of central directory
     # 2. whole central directory
     # 3. METADATA file
     # negative offsets not supported:
     # 1. failed range request
     # 2. HEAD request
     # 3.-5. see negative offsets 1.-3.
     expected_requests = 3
     if negative_offset_error:
-        if negative_offset_error[0] in (
+        if negative_offset_error[0] in {
             codes.requested_range_not_satisfiable,
-            NEGATIVE_OFFSET_AS_POSITIVE,
-        ):
+            NegativeOffsetFailure.as_positive,
+            NegativeOffsetFailure.one_more,
+        }:
             expected_requests += 1
         else:
             expected_requests += 2
-    latest_requests = http.latest_requests()
-    assert len(latest_requests) == expected_requests
+
+    assert_metadata_from_wheel_url(
+        negative_offset_error=negative_offset_error, expected_requests=expected_requests
+    )
 
     # second wheel -> one less request if negative offsets are not supported
-    latest_requests.clear()
-    metadata_from_wheel_url("poetry-core", url, requests.Session())
     expected_requests = min(expected_requests, 4)
-    latest_requests = httpretty.latest_requests()
-    assert len(latest_requests) == expected_requests
+    assert_metadata_from_wheel_url(
+        negative_offset_error=negative_offset_error, expected_requests=expected_requests
+    )
 
 
-@pytest.mark.parametrize("negative_offset_as_positive", [False, True])
+def test_metadata_from_wheel_url_416_missing_content_range(
+    assert_metadata_from_wheel_url: AssertMetadataFromWheelUrl,
+) -> None:
+    def request_callback_wrapper(
+        request_callback: HTTPrettyRequestCallback,
+    ) -> HTTPrettyRequestCallback:
+        def _wrapped(
+            request: HTTPrettyRequest, uri: str, response_headers: dict[str, Any]
+        ) -> HTTPrettyResponse:
+            status_code, response_headers, body = request_callback(
+                request, uri, response_headers
+            )
+            return (
+                status_code,
+                {
+                    header: response_headers[header]
+                    for header in response_headers
+                    if header.lower() != "content-range"
+                },
+                body,
+            )
+
+        return _wrapped
+
+    assert_metadata_from_wheel_url(
+        negative_offset_error=(
+            codes.requested_range_not_satisfiable,
+            b"Requested range not satisfiable",
+        ),
+        expected_requests=5,
+        request_callback_wrapper=request_callback_wrapper,
+    )
+
+
+def test_metadata_from_wheel_url_with_redirect(
+    assert_metadata_from_wheel_url: AssertMetadataFromWheelUrl,
+) -> None:
+    assert_metadata_from_wheel_url(
+        negative_offset_error=None,
+        expected_requests=6,
+        redirect=True,
+    )
+
+
+def test_metadata_from_wheel_url_with_redirect_after_500(
+    assert_metadata_from_wheel_url: AssertMetadataFromWheelUrl,
+) -> None:
+    assert_metadata_from_wheel_url(
+        negative_offset_error=(codes.internal_server_error, b"Internal server error"),
+        expected_requests=10,
+        redirect=True,
+    )
+
+
+@pytest.mark.parametrize(
+    ("negative_offset_failure", "expected_requests"),
+    [
+        (None, 1),
+        (NegativeOffsetFailure.as_positive, 1),
+        (NegativeOffsetFailure.one_more, 2),
+    ],
+)
 def test_metadata_from_wheel_url_smaller_than_initial_chunk_size(
     http: type[httpretty.httpretty],
     handle_request_factory: RequestCallbackFactory,
-    negative_offset_as_positive: bool,
+    negative_offset_failure: NegativeOffsetFailure | None,
+    expected_requests: int,
 ) -> None:
-    domain = f"tiny-wheel-{str(negative_offset_as_positive).casefold()}.com"
+    domain = f"tiny-wheel-{str(negative_offset_failure).casefold()}.com"
     uri_regex = re.compile(f"^https://{domain}/.*$")
     request_callback = handle_request_factory(
         negative_offset_error=(
-            (NEGATIVE_OFFSET_AS_POSITIVE, b"") if negative_offset_as_positive else None
+            (negative_offset_failure, b"") if negative_offset_failure else None
         )
     )
     http.register_uri(http.GET, uri_regex, body=request_callback)
     http.register_uri(http.HEAD, uri_regex, body=request_callback)
 
     url = f"https://{domain}/zipp-3.5.0-py3-none-any.whl"
 
     metadata = metadata_from_wheel_url("zipp", url, requests.Session())
 
     assert metadata["name"] == "zipp"
     assert metadata["version"] == "3.5.0"
     assert metadata["author"] == "Jason R. Coombs"
     assert len(metadata["requires_dist"]) == 12
 
-    # only one request because server gives a normal response with the entire wheel
-    # except for when server interprets negative offset as positive
     latest_requests = http.latest_requests()
-    assert len(latest_requests) == 1
+    assert len(latest_requests) == expected_requests
 
 
 @pytest.mark.parametrize("accept_ranges", [None, "none"])
 def test_metadata_from_wheel_url_range_requests_not_supported_one_request(
     http: type[httpretty.httpretty],
     handle_request_factory: RequestCallbackFactory,
     accept_ranges: str | None,
@@ -298,14 +413,39 @@
 
     latest_requests = http.latest_requests()
     assert len(latest_requests) == 2
     assert latest_requests[0].method == "GET"
     assert latest_requests[1].method == "HEAD"
 
 
+def test_metadata_from_wheel_url_range_requests_supported_but_not_respected(
+    http: type[httpretty.httpretty],
+    handle_request_factory: RequestCallbackFactory,
+) -> None:
+    domain = "range-requests-not-respected.com"
+    uri_regex = re.compile(f"^https://{domain}/.*$")
+    request_callback = handle_request_factory(
+        negative_offset_error=(codes.method_not_allowed, b"Method not allowed"),
+        ignore_accept_ranges=True,
+    )
+    http.register_uri(http.GET, uri_regex, body=request_callback)
+    http.register_uri(http.HEAD, uri_regex, body=request_callback)
+
+    url = f"https://{domain}/poetry_core-1.5.0-py3-none-any.whl"
+
+    with pytest.raises(HTTPRangeRequestNotRespected):
+        metadata_from_wheel_url("poetry-core", url, requests.Session())
+
+    latest_requests = http.latest_requests()
+    assert len(latest_requests) == 3
+    assert latest_requests[0].method == "GET"
+    assert latest_requests[1].method == "HEAD"
+    assert latest_requests[2].method == "GET"
+
+
 def test_metadata_from_wheel_url_invalid_wheel(
     http: type[httpretty.httpretty],
     handle_request_factory: RequestCallbackFactory,
 ) -> None:
     domain = "invalid-wheel.com"
     uri_regex = re.compile(f"^https://{domain}/.*$")
     request_callback = handle_request_factory()
@@ -316,7 +456,23 @@
 
     with pytest.raises(InvalidWheel):
         metadata_from_wheel_url("demo-missing-dist-info", url, requests.Session())
 
     latest_requests = http.latest_requests()
     assert len(latest_requests) == 1
     assert latest_requests[0].method == "GET"
+
+
+def test_metadata_from_wheel_url_handles_unexpected_errors(
+    mocker: MockerFixture,
+) -> None:
+    mocker.patch(
+        "poetry.inspection.lazy_wheel.LazyWheelOverHTTP.read_metadata",
+        side_effect=RuntimeError(),
+    )
+
+    with pytest.raises(LazyWheelUnsupportedError):
+        metadata_from_wheel_url(
+            "demo-missing-dist-info",
+            "https://runtime-error.com/demo_missing_dist_info-0.1.0-py2.py3-none-any.whl",
+            requests.Session(),
+        )
```

### Comparing `poetry-1.8.1/tests/installation/conftest.py` & `poetry-1.8.2/tests/installation/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/installation/fixtures/extras-with-dependencies.test` & `poetry-1.8.2/tests/installation/fixtures/extras-with-dependencies.test`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/installation/fixtures/extras.test` & `poetry-1.8.2/tests/installation/fixtures/extras.test`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/installation/fixtures/old-lock.test` & `poetry-1.8.2/tests/installation/fixtures/old-lock.test`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/installation/fixtures/update-with-locked-extras.test` & `poetry-1.8.2/tests/installation/fixtures/update-with-locked-extras.test`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/installation/fixtures/with-dependencies-nested-extras.test` & `poetry-1.8.2/tests/installation/fixtures/with-dependencies-nested-extras.test`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/installation/fixtures/with-directory-dependency-poetry-transitive.test` & `poetry-1.8.2/tests/installation/fixtures/with-directory-dependency-poetry-transitive.test`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/installation/fixtures/with-directory-dependency-poetry.test` & `poetry-1.8.2/tests/installation/fixtures/with-directory-dependency-poetry.test`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/installation/fixtures/with-directory-dependency-setuptools.test` & `poetry-1.8.2/tests/installation/fixtures/with-directory-dependency-setuptools.test`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/installation/fixtures/with-duplicate-dependencies.test` & `poetry-1.8.2/tests/installation/fixtures/with-duplicate-dependencies.test`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/installation/fixtures/with-file-dependency-transitive.test` & `poetry-1.8.2/tests/installation/fixtures/with-file-dependency-transitive.test`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/installation/fixtures/with-file-dependency.test` & `poetry-1.8.2/tests/installation/fixtures/with-file-dependency.test`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/installation/fixtures/with-multiple-updates.test` & `poetry-1.8.2/tests/installation/fixtures/with-multiple-updates.test`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/installation/fixtures/with-platform-dependencies.test` & `poetry-1.8.2/tests/installation/fixtures/with-platform-dependencies.test`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/installation/fixtures/with-pypi-repository.test` & `poetry-1.8.2/tests/installation/fixtures/with-pypi-repository.test`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/installation/fixtures/with-same-version-url-dependencies.test` & `poetry-1.8.2/tests/installation/fixtures/with-same-version-url-dependencies.test`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/installation/fixtures/with-sub-dependencies.test` & `poetry-1.8.2/tests/installation/fixtures/with-sub-dependencies.test`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/installation/fixtures/with-url-dependency.test` & `poetry-1.8.2/tests/installation/fixtures/with-url-dependency.test`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/installation/fixtures/with-vcs-dependency-with-extras.test` & `poetry-1.8.2/tests/installation/fixtures/with-vcs-dependency-with-extras.test`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/installation/test_chef.py` & `poetry-1.8.2/tests/installation/test_chef.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/installation/test_chooser.py` & `poetry-1.8.2/tests/installation/test_chooser.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/installation/test_executor.py` & `poetry-1.8.2/tests/installation/test_executor.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/installation/test_installer.py` & `poetry-1.8.2/tests/installation/test_installer.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/installation/test_wheel_installer.py` & `poetry-1.8.2/tests/installation/test_wheel_installer.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/integration/test_utils_vcs_git.py` & `poetry-1.8.2/tests/integration/test_utils_vcs_git.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/json/test_schema_sources.py` & `poetry-1.8.2/tests/json/test_schema_sources.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/masonry/builders/test_editable_builder.py` & `poetry-1.8.2/tests/masonry/builders/test_editable_builder.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/mixology/helpers.py` & `poetry-1.8.2/tests/mixology/helpers.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/mixology/solutions/providers/test_python_requirement_solution_provider.py` & `poetry-1.8.2/tests/mixology/solutions/providers/test_python_requirement_solution_provider.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/mixology/solutions/solutions/test_python_requirement_solution.py` & `poetry-1.8.2/tests/mixology/solutions/solutions/test_python_requirement_solution.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/mixology/test_incompatibility.py` & `poetry-1.8.2/tests/mixology/test_incompatibility.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/mixology/version_solver/conftest.py` & `poetry-1.8.2/tests/mixology/version_solver/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/mixology/version_solver/test_backtracking.py` & `poetry-1.8.2/tests/mixology/version_solver/test_backtracking.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/mixology/version_solver/test_basic_graph.py` & `poetry-1.8.2/tests/mixology/version_solver/test_basic_graph.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/mixology/version_solver/test_dependency_cache.py` & `poetry-1.8.2/tests/mixology/version_solver/test_dependency_cache.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/mixology/version_solver/test_python_constraint.py` & `poetry-1.8.2/tests/mixology/version_solver/test_python_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/mixology/version_solver/test_unsolvable.py` & `poetry-1.8.2/tests/mixology/version_solver/test_unsolvable.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/mixology/version_solver/test_with_lock.py` & `poetry-1.8.2/tests/mixology/version_solver/test_with_lock.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/packages/test_direct_origin.py` & `poetry-1.8.2/tests/packages/test_direct_origin.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/packages/test_locker.py` & `poetry-1.8.2/tests/packages/test_locker.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/plugins/test_plugin_manager.py` & `poetry-1.8.2/tests/plugins/test_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/publishing/test_publisher.py` & `poetry-1.8.2/tests/publishing/test_publisher.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/publishing/test_uploader.py` & `poetry-1.8.2/tests/publishing/test_uploader.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/puzzle/conftest.py` & `poetry-1.8.2/tests/puzzle/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/puzzle/test_provider.py` & `poetry-1.8.2/tests/puzzle/test_provider.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/puzzle/test_solver.py` & `poetry-1.8.2/tests/puzzle/test_solver.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/puzzle/test_transaction.py` & `poetry-1.8.2/tests/puzzle/test_transaction.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/pyproject/conftest.py` & `poetry-1.8.2/tests/pyproject/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/pyproject/test_pyproject_toml.py` & `poetry-1.8.2/tests/pyproject/test_pyproject_toml.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/pyproject/test_pyproject_toml_file.py` & `poetry-1.8.2/tests/pyproject/test_pyproject_toml_file.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/conftest.py` & `poetry-1.8.2/tests/repositories/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/cleo-0.7.6.dist-info/METADATA` & `poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/cleo-0.7.6.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-2.3.4.dist-info/METADATA` & `poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-2.3.4.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-with-import-2.3.4.dist-info/METADATA` & `poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-with-import-2.3.4.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/foo-0.1.0-py3.8.egg` & `poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/foo-0.1.0-py3.8.egg`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/standard-1.2.3.dist-info/METADATA` & `poetry-1.8.2/tests/repositories/fixtures/installed/lib/python3.7/site-packages/standard-1.2.3.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/bender-2.0.5.dist-info/METADATA` & `poetry-1.8.2/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/bender-2.0.5.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/lib64-2.3.4.dist-info/METADATA` & `poetry-1.8.2/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/lib64-2.3.4.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/installed/src/bender/bender.egg-info/PKG-INFO` & `poetry-1.8.2/tests/repositories/fixtures/installed/src/bender/bender.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/installed/src/pendulum/pendulum.egg-info/PKG-INFO` & `poetry-1.8.2/tests/repositories/fixtures/installed/src/pendulum/pendulum.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/installed/vendor/py3.7/attrs-19.3.0.dist-info/METADATA` & `poetry-1.8.2/tests/repositories/fixtures/installed/vendor/py3.7/attrs-19.3.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/legacy/absolute.html` & `poetry-1.8.2/tests/repositories/fixtures/legacy/absolute.html`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/legacy/black.html` & `poetry-1.8.2/tests/repositories/fixtures/legacy/black.html`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/legacy/clikit.html` & `poetry-1.8.2/tests/repositories/fixtures/legacy/clikit.html`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/legacy/discord-py.html` & `poetry-1.8.2/tests/repositories/fixtures/legacy/discord-py.html`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/legacy/futures-partial-yank.html` & `poetry-1.8.2/tests/repositories/fixtures/legacy/futures-partial-yank.html`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/legacy/futures.html` & `poetry-1.8.2/tests/repositories/fixtures/legacy/futures.html`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/legacy/invalid-version.html` & `poetry-1.8.2/tests/repositories/fixtures/legacy/invalid-version.html`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/legacy/ipython.html` & `poetry-1.8.2/tests/repositories/fixtures/legacy/ipython.html`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/legacy/isort.html` & `poetry-1.8.2/tests/repositories/fixtures/legacy/isort.html`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/legacy/poetry-test-py2-py3-metadata-merge.html` & `poetry-1.8.2/tests/repositories/fixtures/legacy/poetry-test-py2-py3-metadata-merge.html`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/legacy/pytest-with-extra-packages.html` & `poetry-1.8.2/tests/repositories/fixtures/legacy/pytest-with-extra-packages.html`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/legacy/pytest.html` & `poetry-1.8.2/tests/repositories/fixtures/legacy/pytest.html`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/legacy/pyyaml.html` & `poetry-1.8.2/tests/repositories/fixtures/legacy/pyyaml.html`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/legacy/relative.html` & `poetry-1.8.2/tests/repositories/fixtures/legacy/relative.html`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/metadata/isort-metadata-4.3.4-py2-none-any.whl.metadata` & `poetry-1.8.2/tests/repositories/fixtures/metadata/isort-metadata-4.3.4-py2-none-any.whl.metadata`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/metadata/isort-metadata-4.3.4-py3-none-any.whl.metadata` & `poetry-1.8.2/tests/repositories/fixtures/metadata/isort-metadata-4.3.4-py3-none-any.whl.metadata`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/SQLAlchemy-1.2.12.tar.gz` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/SQLAlchemy-1.2.12.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/Twisted-18.9.0.tar.bz2` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/Twisted-18.9.0.tar.bz2`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/black-19.10b0-py36-none-any.whl` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/black-19.10b0-py36-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/black-21.11b0-py3-none-any.whl` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/black-21.11b0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/cleo-1.0.0a5-py3-none-any.whl` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/cleo-1.0.0a5-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/clikit-0.2.4-py2.py3-none-any.whl` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/clikit-0.2.4-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/discord.py-2.0.0-py3-none-any.whl` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/discord.py-2.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0-py2-none-any.whl` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0-py2-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0.tar.gz` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/importlib_metadata-1.7.0-py2.py3-none-any.whl` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/importlib_metadata-1.7.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py2-none-any.whl` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py2-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py3-none-any.whl` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0.tar.gz` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/ipython-7.5.0-py3-none-any.whl` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/ipython-7.5.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py2-none-any.whl` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py2-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py3-none-any.whl` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4.tar.gz` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0-py2.py3-none-any.whl` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0.tar.gz` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/pastel-0.1.0.tar.gz` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/pastel-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/poetry_core-1.5.0-py3-none-any.whl` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/poetry_core-1.5.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py2-none-any.whl` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py2-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py3-none-any.whl` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/pytest-3.5.0-py2.py3-none-any.whl` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/pytest-3.5.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/pytest-3.5.1-py2.py3-none-any.whl` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/pytest-3.5.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/python-language-server-0.21.2.tar.gz` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/python-language-server-0.21.2.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.2.tar.gz` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.2.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.3.tar.gz` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.3.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/dists/zipp-3.5.0-py3-none-any.whl` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/dists/zipp-3.5.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/attrs/17.4.0.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/attrs/17.4.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/attrs.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/attrs.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/black/19.10b0.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/black/19.10b0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/black/21.11b0.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/black/21.11b0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/black.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/black.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/cachecontrol/0.12.5.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/cachecontrol/0.12.5.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/cachecontrol.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/cachecontrol.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/cleo/1.0.0a5.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/cleo/1.0.0a5.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/clikit/0.2.4.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/clikit/0.2.4.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/clikit.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/clikit.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/colorama/0.3.9.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/colorama/0.3.9.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/colorama.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/colorama.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/discord-py/2.0.0.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/discord-py/2.0.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/funcsigs/1.0.2.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/funcsigs/1.0.2.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/funcsigs.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/funcsigs.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/hbmqtt/0.9.6.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/hbmqtt/0.9.6.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/hbmqtt.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/hbmqtt.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/importlib-metadata/1.7.0.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/importlib-metadata/1.7.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/importlib-metadata.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/importlib-metadata.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/ipython/4.1.0rc1.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/ipython/4.1.0rc1.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/isort/4.3.4.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/isort/4.3.4.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/isort-metadata/4.3.4.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/isort-metadata/4.3.4.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/isort-metadata.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/isort-metadata.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/isort.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/isort.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/jupyter/1.0.0.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/jupyter/1.0.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/jupyter.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/jupyter.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/lockfile/0.12.2.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/lockfile/0.12.2.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/lockfile.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/lockfile.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/more-itertools/4.1.0.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/more-itertools/4.1.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/more-itertools.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/more-itertools.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/pluggy/0.6.0.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/pluggy/0.6.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/poetry/0.12.4.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/poetry/0.12.4.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/poetry-core/1.5.0.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/poetry-core/1.5.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/poetry-core.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/poetry-core.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/poetry.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/poetry.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/py/1.5.3.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/py/1.5.3.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/py.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/py.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/pygame-music-grid.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/pygame-music-grid.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/pylev/1.3.0.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/pylev/1.3.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/pytest/3.5.0.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/pytest/3.5.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/pytest/3.5.1.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/pytest/3.5.1.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/pytest.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/pytest.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/pyyaml/3.13.0.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/pyyaml/3.13.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/pyyaml.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/pyyaml.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/requests/2.18.4.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/requests/2.18.4.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/requests.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/requests.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/setuptools/39.2.0.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/setuptools/39.2.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/setuptools/67.6.1.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/setuptools/67.6.1.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/setuptools.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/setuptools.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/six/1.11.0.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/six/1.11.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/six.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/six.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/sqlalchemy/1.2.12.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/sqlalchemy/1.2.12.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/toga.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/toga.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/tomlkit/0.5.3.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/tomlkit/0.5.3.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/tomlkit.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/tomlkit.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/trackpy/0.4.1.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/trackpy/0.4.1.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/trackpy.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/trackpy.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/twisted/18.9.0.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/twisted/18.9.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/wheel/0.40.0.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/wheel/0.40.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/wheel.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/wheel.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/zipp/3.5.0.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/zipp/3.5.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/json/zipp.json` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/json/zipp.json`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/pypi.org/search/search.html` & `poetry-1.8.2/tests/repositories/fixtures/pypi.org/search/search.html`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/fixtures/single-page/jax_releases.html` & `poetry-1.8.2/tests/repositories/fixtures/single-page/jax_releases.html`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/link_sources/test_base.py` & `poetry-1.8.2/tests/repositories/link_sources/test_base.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/link_sources/test_html.py` & `poetry-1.8.2/tests/repositories/link_sources/test_html.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/link_sources/test_json.py` & `poetry-1.8.2/tests/repositories/link_sources/test_json.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/parsers/test_html_page_parser.py` & `poetry-1.8.2/tests/repositories/parsers/test_html_page_parser.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/parsers/test_pypi_search_parser.py` & `poetry-1.8.2/tests/repositories/parsers/test_pypi_search_parser.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/test_http_repository.py` & `poetry-1.8.2/tests/repositories/test_http_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/test_installed_repository.py` & `poetry-1.8.2/tests/repositories/test_installed_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/test_legacy_repository.py` & `poetry-1.8.2/tests/repositories/test_legacy_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/test_lockfile_repository.py` & `poetry-1.8.2/tests/repositories/test_lockfile_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/test_pypi_repository.py` & `poetry-1.8.2/tests/repositories/test_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/test_repository.py` & `poetry-1.8.2/tests/repositories/test_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/test_repository_pool.py` & `poetry-1.8.2/tests/repositories/test_repository_pool.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/repositories/test_single_page_repository.py` & `poetry-1.8.2/tests/repositories/test_single_page_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/test_factory.py` & `poetry-1.8.2/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/types.py` & `poetry-1.8.2/tests/types.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,28 +2,40 @@
 
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Protocol
 
 
 if TYPE_CHECKING:
+    from collections.abc import Callable
     from pathlib import Path
+    from typing import Dict
+    from typing import Tuple
 
     import requests
 
     from cleo.io.io import IO
     from cleo.testers.command_tester import CommandTester
+    from httpretty.core import HTTPrettyRequest
 
     from poetry.config.config import Config
     from poetry.config.source import Source
     from poetry.installation import Installer
     from poetry.installation.executor import Executor
     from poetry.poetry import Poetry
     from poetry.utils.env import Env
 
+    HTTPrettyResponse = Tuple[int, Dict[str, Any], bytes]  # status code, headers, body
+    HTTPrettyRequestCallback = Callable[
+        [HTTPrettyRequest, str, Dict[str, Any]], HTTPrettyResponse
+    ]
+    HTTPPrettyRequestCallbackWrapper = Callable[
+        [HTTPrettyRequestCallback], HTTPrettyRequestCallback
+    ]
+
 
 class CommandTesterFactory(Protocol):
     def __call__(
         self,
         command: str,
         poetry: Poetry | None = None,
         installer: Installer | None = None,
```

### Comparing `poetry-1.8.1/tests/utils/env/conftest.py` & `poetry-1.8.2/tests/utils/env/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/utils/env/test_env.py` & `poetry-1.8.2/tests/utils/env/test_env.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/utils/env/test_env_manager.py` & `poetry-1.8.2/tests/utils/env/test_env_manager.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/utils/env/test_env_site_packages.py` & `poetry-1.8.2/tests/utils/env/test_env_site_packages.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/utils/fixtures/pyproject.toml` & `poetry-1.8.2/tests/utils/fixtures/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/utils/fixtures/setups/ansible/setup.py` & `poetry-1.8.2/tests/utils/fixtures/setups/ansible/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/utils/fixtures/setups/flask/setup.py` & `poetry-1.8.2/tests/utils/fixtures/setups/flask/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/utils/fixtures/setups/pendulum/setup.py` & `poetry-1.8.2/tests/utils/fixtures/setups/pendulum/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/utils/fixtures/setups/pyyaml/setup.py` & `poetry-1.8.2/tests/utils/fixtures/setups/pyyaml/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/utils/fixtures/setups/requests/setup.py` & `poetry-1.8.2/tests/utils/fixtures/setups/requests/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/utils/fixtures/setups/sqlalchemy/setup.py` & `poetry-1.8.2/tests/utils/fixtures/setups/sqlalchemy/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/utils/test_authenticator.py` & `poetry-1.8.2/tests/utils/test_authenticator.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/utils/test_cache.py` & `poetry-1.8.2/tests/utils/test_cache.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/utils/test_dependency_specification.py` & `poetry-1.8.2/tests/utils/test_dependency_specification.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/utils/test_extras.py` & `poetry-1.8.2/tests/utils/test_extras.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/utils/test_helpers.py` & `poetry-1.8.2/tests/utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/utils/test_password_manager.py` & `poetry-1.8.2/tests/utils/test_password_manager.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/utils/test_patterns.py` & `poetry-1.8.2/tests/utils/test_patterns.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/utils/test_pip.py` & `poetry-1.8.2/tests/utils/test_pip.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/utils/test_setup_reader.py` & `poetry-1.8.2/tests/utils/test_setup_reader.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/utils/test_source.py` & `poetry-1.8.2/tests/utils/test_source.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/vcs/git/test_backend.py` & `poetry-1.8.2/tests/vcs/git/test_backend.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/tests/vcs/git/test_system.py` & `poetry-1.8.2/tests/vcs/git/test_system.py`

 * *Files identical despite different names*

### Comparing `poetry-1.8.1/PKG-INFO` & `poetry-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry
-Version: 1.8.1
+Version: 1.8.2
 Summary: Python dependency management and packaging made easy.
 Home-page: https://python-poetry.org/
 License: MIT
 Keywords: packaging,dependency,poetry
 Author: Sébastien Eustace
 Author-email: sebastien@eustace.io
 Maintainer: Arun Babu Neelicattu
```

