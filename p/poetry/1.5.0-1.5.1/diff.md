# Comparing `tmp/poetry-1.5.0.tar.gz` & `tmp/poetry-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry-1.5.0.tar", max compression
+gzip compressed data, was "poetry-1.5.1.tar", max compression
```

## Comparing `poetry-1.5.0.tar` & `poetry-1.5.1.tar`

### file list

```diff
@@ -1,707 +1,707 @@
--rw-r--r--   0        0        0     1070 2023-05-19 12:27:02.278399 poetry-1.5.0/LICENSE
--rw-r--r--   0        0        0     4547 2023-05-19 12:27:02.278399 poetry-1.5.0/README.md
--rw-r--r--   0        0        0     5512 2023-05-19 12:27:02.290399 poetry-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      146 2023-05-19 12:27:02.290399 poetry-1.5.0/src/poetry/__main__.py
--rw-r--r--   0        0        0      342 2023-05-19 12:27:02.290399 poetry-1.5.0/src/poetry/__version__.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.290399 poetry-1.5.0/src/poetry/config/__init__.py
--rw-r--r--   0        0        0     9746 2023-05-19 12:27:02.290399 poetry-1.5.0/src/poetry/config/config.py
--rw-r--r--   0        0        0      261 2023-05-19 12:27:02.290399 poetry-1.5.0/src/poetry/config/config_source.py
--rw-r--r--   0        0        0     1018 2023-05-19 12:27:02.290399 poetry-1.5.0/src/poetry/config/dict_config_source.py
--rw-r--r--   0        0        0     2339 2023-05-19 12:27:02.290399 poetry-1.5.0/src/poetry/config/file_config_source.py
--rw-r--r--   0        0        0     1396 2023-05-19 12:27:02.290399 poetry-1.5.0/src/poetry/config/source.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.290399 poetry-1.5.0/src/poetry/console/__init__.py
--rw-r--r--   0        0        0    12551 2023-05-19 12:27:02.290399 poetry-1.5.0/src/poetry/console/application.py
--rw-r--r--   0        0        0      615 2023-05-19 12:27:02.290399 poetry-1.5.0/src/poetry/console/command_loader.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.290399 poetry-1.5.0/src/poetry/console/commands/__init__.py
--rw-r--r--   0        0        0      893 2023-05-19 12:27:02.290399 poetry-1.5.0/src/poetry/console/commands/about.py
--rw-r--r--   0        0        0    10690 2023-05-19 12:27:02.290399 poetry-1.5.0/src/poetry/console/commands/add.py
--rw-r--r--   0        0        0     1081 2023-05-19 12:27:02.290399 poetry-1.5.0/src/poetry/console/commands/build.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.290399 poetry-1.5.0/src/poetry/console/commands/cache/__init__.py
--rw-r--r--   0        0        0     2411 2023-05-19 12:27:02.290399 poetry-1.5.0/src/poetry/console/commands/cache/clear.py
--rw-r--r--   0        0        0      634 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/cache/list.py
--rw-r--r--   0        0        0     3360 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/check.py
--rw-r--r--   0        0        0     1118 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/command.py
--rw-r--r--   0        0        0    11027 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/config.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/debug/__init__.py
--rw-r--r--   0        0        0      764 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/debug/info.py
--rw-r--r--   0        0        0     4484 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/debug/resolve.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/env/__init__.py
--rw-r--r--   0        0        0     2600 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/env/info.py
--rw-r--r--   0        0        0      822 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/env/list.py
--rw-r--r--   0        0        0     1478 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/env/remove.py
--rw-r--r--   0        0        0      706 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/env/use.py
--rw-r--r--   0        0        0      544 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/env_command.py
--rw-r--r--   0        0        0     4370 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/group_command.py
--rw-r--r--   0        0        0    17346 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/init.py
--rw-r--r--   0        0        0     6637 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/install.py
--rw-r--r--   0        0        0      907 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/installer_command.py
--rw-r--r--   0        0        0     1513 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/lock.py
--rw-r--r--   0        0        0     3000 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/new.py
--rw-r--r--   0        0        0     2776 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/publish.py
--rw-r--r--   0        0        0     5163 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/remove.py
--rw-r--r--   0        0        0     3261 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/run.py
--rw-r--r--   0        0        0      786 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/search.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/self/__init__.py
--rw-r--r--   0        0        0     1261 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/self/add.py
--rw-r--r--   0        0        0      973 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/self/install.py
--rw-r--r--   0        0        0      642 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/self/lock.py
--rw-r--r--   0        0        0      607 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/self/remove.py
--rw-r--r--   0        0        0     4503 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/self/self_command.py
--rw-r--r--   0        0        0     1209 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/self/show/__init__.py
--rw-r--r--   0        0        0     4036 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/self/show/plugins.py
--rw-r--r--   0        0        0     1802 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/self/update.py
--rw-r--r--   0        0        0     1527 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/shell.py
--rw-r--r--   0        0        0    20399 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/show.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/source/__init__.py
--rw-r--r--   0        0        0     5487 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/source/add.py
--rw-r--r--   0        0        0     1181 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/source/remove.py
--rw-r--r--   0        0        0     1614 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/source/show.py
--rw-r--r--   0        0        0     1547 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/update.py
--rw-r--r--   0        0        0     3775 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/commands/version.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/events/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/events/console_events.py
--rw-r--r--   0        0        0      174 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/io/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/io/inputs/__init__.py
--rw-r--r--   0        0        0     2516 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/io/inputs/run_argv_input.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/logging/__init__.py
--rw-r--r--   0        0        0       99 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/logging/filters.py
--rw-r--r--   0        0        0      336 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/logging/formatters/__init__.py
--rw-r--r--   0        0        0      788 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/logging/formatters/builder_formatter.py
--rw-r--r--   0        0        0      132 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/logging/formatters/formatter.py
--rw-r--r--   0        0        0     1026 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/logging/io_formatter.py
--rw-r--r--   0        0        0      702 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/console/logging/io_handler.py
--rw-r--r--   0        0        0      134 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/exceptions.py
--rw-r--r--   0        0        0    13389 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/factory.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/inspection/__init__.py
--rw-r--r--   0        0        0    21805 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/inspection/info.py
--rw-r--r--   0        0        0      114 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/installation/__init__.py
--rw-r--r--   0        0        0     6441 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/installation/chef.py
--rw-r--r--   0        0        0     6887 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/installation/chooser.py
--rw-r--r--   0        0        0    37137 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/installation/executor.py
--rw-r--r--   0        0        0    15285 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/installation/installer.py
--rw-r--r--   0        0        0      262 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/installation/operations/__init__.py
--rw-r--r--   0        0        0      906 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/installation/operations/install.py
--rw-r--r--   0        0        0     1315 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/installation/operations/operation.py
--rw-r--r--   0        0        0      959 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/installation/operations/uninstall.py
--rw-r--r--   0        0        0     1540 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/installation/operations/update.py
--rw-r--r--   0        0        0     3725 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/installation/wheel_installer.py
--rw-r--r--   0        0        0     1281 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/json/__init__.py
--rw-r--r--   0        0        0     2127 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/json/schemas/poetry.json
--rw-r--r--   0        0        0      310 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/layouts/__init__.py
--rw-r--r--   0        0        0     5970 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/layouts/layout.py
--rw-r--r--   0        0        0      202 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/layouts/src.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/layouts/standard.py
--rw-r--r--   0        0        0     1669 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/locations.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/masonry/__init__.py
--rw-r--r--   0        0        0      497 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/masonry/api.py
--rw-r--r--   0        0        0      129 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/masonry/builders/__init__.py
--rw-r--r--   0        0        0     9537 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/masonry/builders/editable.py
--rw-r--r--   0        0        0      467 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/mixology/__init__.py
--rw-r--r--   0        0        0     1555 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/mixology/assignment.py
--rw-r--r--   0        0        0    10186 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/mixology/failure.py
--rw-r--r--   0        0        0    15346 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/mixology/incompatibility.py
--rw-r--r--   0        0        0     1903 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/mixology/incompatibility_cause.py
--rw-r--r--   0        0        0     7080 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/mixology/partial_solution.py
--rw-r--r--   0        0        0      676 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/mixology/result.py
--rw-r--r--   0        0        0      211 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/mixology/set_relation.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/mixology/solutions/__init__.py
--rw-r--r--   0        0        0      214 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/mixology/solutions/providers/__init__.py
--rw-r--r--   0        0        0     1091 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/mixology/solutions/providers/python_requirement_solution_provider.py
--rw-r--r--   0        0        0      189 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/mixology/solutions/solutions/__init__.py
--rw-r--r--   0        0        0     2281 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/mixology/solutions/solutions/python_requirement_solution.py
--rw-r--r--   0        0        0     6904 2023-05-19 12:27:02.294399 poetry-1.5.0/src/poetry/mixology/term.py
--rw-r--r--   0        0        0    19937 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/mixology/version_solver.py
--rw-r--r--   0        0        0      273 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/packages/__init__.py
--rw-r--r--   0        0        0     1297 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/packages/dependency_package.py
--rw-r--r--   0        0        0     3352 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/packages/direct_origin.py
--rw-r--r--   0        0        0    17760 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/packages/locker.py
--rw-r--r--   0        0        0      921 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/packages/package_collection.py
--rw-r--r--   0        0        0      185 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/plugins/__init__.py
--rw-r--r--   0        0        0      687 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/plugins/application_plugin.py
--rw-r--r--   0        0        0      435 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/plugins/base_plugin.py
--rw-r--r--   0        0        0      484 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/plugins/plugin.py
--rw-r--r--   0        0        0     2537 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/plugins/plugin_manager.py
--rw-r--r--   0        0        0     2491 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/poetry.py
--rw-r--r--   0        0        0      112 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/publishing/__init__.py
--rw-r--r--   0        0        0     2893 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/publishing/publisher.py
--rw-r--r--   0        0        0    12586 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/publishing/uploader.py
--rw-r--r--   0        0        0       99 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/puzzle/__init__.py
--rw-r--r--   0        0        0      799 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/puzzle/exceptions.py
--rw-r--r--   0        0        0    37604 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/puzzle/provider.py
--rw-r--r--   0        0        0    11184 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/puzzle/solver.py
--rw-r--r--   0        0        0     5304 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/puzzle/transaction.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/py.typed
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/pyproject/__init__.py
--rw-r--r--   0        0        0     1740 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/pyproject/toml.py
--rw-r--r--   0        0        0      198 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/repositories/__init__.py
--rw-r--r--   0        0        0      833 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/repositories/abstract_repository.py
--rw-r--r--   0        0        0     2553 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/repositories/cached_repository.py
--rw-r--r--   0        0        0      173 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/repositories/exceptions.py
--rw-r--r--   0        0        0    11396 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/repositories/http_repository.py
--rw-r--r--   0        0        0    10307 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/repositories/installed_repository.py
--rw-r--r--   0        0        0     4474 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/repositories/legacy_repository.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/repositories/link_sources/__init__.py
--rw-r--r--   0        0        0     3835 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/repositories/link_sources/base.py
--rw-r--r--   0        0        0     1955 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/repositories/link_sources/html.py
--rw-r--r--   0        0        0     1227 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/repositories/link_sources/json.py
--rw-r--r--   0        0        0      841 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/repositories/lockfile_repository.py
--rw-r--r--   0        0        0     8417 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/repositories/pypi_repository.py
--rw-r--r--   0        0        0     3978 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/repositories/repository.py
--rw-r--r--   0        0        0     6646 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/repositories/repository_pool.py
--rw-r--r--   0        0        0      753 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/repositories/single_page_repository.py
--rw-r--r--   0        0        0      157 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/toml/__init__.py
--rw-r--r--   0        0        0      198 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/toml/exceptions.py
--rw-r--r--   0        0        0     1364 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/toml/file.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/utils/__init__.py
--rw-r--r--   0        0        0     1565 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/utils/_compat.py
--rw-r--r--   0        0        0    17281 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/utils/authenticator.py
--rw-r--r--   0        0        0     8537 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/utils/cache.py
--rw-r--r--   0        0        0      302 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/utils/constants.py
--rw-r--r--   0        0        0     7625 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/utils/dependency_specification.py
--rw-r--r--   0        0        0    65234 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/utils/env.py
--rw-r--r--   0        0        0     1857 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/utils/extras.py
--rw-r--r--   0        0        0     7407 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/utils/helpers.py
--rw-r--r--   0        0        0     7151 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/utils/password_manager.py
--rw-r--r--   0        0        0      406 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/utils/patterns.py
--rw-r--r--   0        0        0     1446 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/utils/pip.py
--rw-r--r--   0        0        0    12018 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/utils/setup_reader.py
--rw-r--r--   0        0        0     4471 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/utils/shell.py
--rw-r--r--   0        0        0      446 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/utils/source.py
--rw-r--r--   0        0        0     1361 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/utils/wheel.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/vcs/__init__.py
--rw-r--r--   0        0        0       95 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/vcs/git/__init__.py
--rw-r--r--   0        0        0    16083 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/vcs/git/backend.py
--rw-r--r--   0        0        0     1787 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/vcs/git/system.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/version/__init__.py
--rw-r--r--   0        0        0     1573 2023-05-19 12:27:02.298399 poetry-1.5.0/src/poetry/version/version_selector.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.298399 poetry-1.5.0/tests/__init__.py
--rw-r--r--   0        0        0      281 2023-05-19 12:27:02.298399 poetry-1.5.0/tests/compat.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.298399 poetry-1.5.0/tests/config/__init__.py
--rw-r--r--   0        0        0     2436 2023-05-19 12:27:02.298399 poetry-1.5.0/tests/config/test_config.py
--rw-r--r--   0        0        0    13408 2023-05-19 12:27:02.298399 poetry-1.5.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.298399 poetry-1.5.0/tests/console/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.298399 poetry-1.5.0/tests/console/commands/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.298399 poetry-1.5.0/tests/console/commands/cache/__init__.py
--rw-r--r--   0        0        0     1458 2023-05-19 12:27:02.298399 poetry-1.5.0/tests/console/commands/cache/conftest.py
--rw-r--r--   0        0        0     2269 2023-05-19 12:27:02.298399 poetry-1.5.0/tests/console/commands/cache/test_clear.py
--rw-r--r--   0        0        0      832 2023-05-19 12:27:02.298399 poetry-1.5.0/tests/console/commands/cache/test_list.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.298399 poetry-1.5.0/tests/console/commands/debug/__init__.py
--rw-r--r--   0        0        0     1807 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/debug/test_resolve.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/env/__init__.py
--rw-r--r--   0        0        0     2349 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/env/conftest.py
--rw-r--r--   0        0        0     1163 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/env/helpers.py
--rw-r--r--   0        0        0     1592 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/env/test_info.py
--rw-r--r--   0        0        0     2039 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/env/test_list.py
--rw-r--r--   0        0        0     2920 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/env/test_remove.py
--rw-r--r--   0        0        0     4701 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/env/test_use.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/self/__init__.py
--rw-r--r--   0        0        0     2244 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/self/conftest.py
--rw-r--r--   0        0        0       65 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/self/fixtures/poetry-1.0.5-darwin.sha256sum
--rw-r--r--   0        0        0     1041 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/self/fixtures/poetry-1.0.5-darwin.tar.gz
--rw-r--r--   0        0        0     7543 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/self/test_add_plugins.py
--rw-r--r--   0        0        0     3034 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/self/test_remove_plugins.py
--rw-r--r--   0        0        0     1596 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/self/test_self_command.py
--rw-r--r--   0        0        0     5885 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/self/test_show_plugins.py
--rw-r--r--   0        0        0     2151 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/self/test_update.py
--rw-r--r--   0        0        0     1167 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/self/utils.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/source/__init__.py
--rw-r--r--   0        0        0     4105 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/source/conftest.py
--rw-r--r--   0        0        0    10226 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/source/test_add.py
--rw-r--r--   0        0        0     2902 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/source/test_remove.py
--rw-r--r--   0        0        0     4943 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/source/test_show.py
--rw-r--r--   0        0        0      835 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/test_about.py
--rw-r--r--   0        0        0    43041 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/test_add.py
--rw-r--r--   0        0        0     1330 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/test_build.py
--rw-r--r--   0        0        0     2032 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/test_check.py
--rw-r--r--   0        0        0    16027 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/test_config.py
--rw-r--r--   0        0        0    29808 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/test_init.py
--rw-r--r--   0        0        0    14192 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/test_install.py
--rw-r--r--   0        0        0    10295 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/test_lock.py
--rw-r--r--   0        0        0     6001 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/test_new.py
--rw-r--r--   0        0        0     3758 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/test_publish.py
--rw-r--r--   0        0        0    10882 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/test_remove.py
--rw-r--r--   0        0        0     6649 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/test_run.py
--rw-r--r--   0        0        0     2568 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/test_search.py
--rw-r--r--   0        0        0     2568 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/test_shell.py
--rw-r--r--   0        0        0    68924 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/test_show.py
--rw-r--r--   0        0        0     2341 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/test_update.py
--rw-r--r--   0        0        0     2588 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/commands/test_version.py
--rw-r--r--   0        0        0     4627 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/conftest.py
--rw-r--r--   0        0        0     3277 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/console/test_application.py
--rw-r--r--   0        0        0       22 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/build_system_requires_not_available/README.rst
--rw-r--r--   0        0        0      676 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/build_system_requires_not_available/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/build_system_requires_not_available/simple_project/__init__.py
--rw-r--r--   0        0        0     1168 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/complete.toml
--rw-r--r--   0        0        0      406 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/deleted_directory_dependency/poetry.lock
--rw-r--r--   0        0        0      234 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/deleted_directory_dependency/pyproject.toml
--rw-r--r--   0        0        0      428 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/deleted_file_dependency/poetry.lock
--rw-r--r--   0        0        0      234 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/deleted_file_dependency/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/directory/project_with_transitive_directory_dependencies/project_with_transitive_directory_dependencies/__init__.py
--rw-r--r--   0        0        0      418 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/directory/project_with_transitive_directory_dependencies/pyproject.toml
--rw-r--r--   0        0        0      574 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/directory/project_with_transitive_directory_dependencies/setup.py
--rw-r--r--   0        0        0      234 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/directory/project_with_transitive_file_dependencies/inner-directory-project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/directory/project_with_transitive_file_dependencies/project_with_transitive_file_dependencies/__init__.py
--rw-r--r--   0        0        0      385 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/directory/project_with_transitive_file_dependencies/pyproject.toml
--rw-r--r--   0        0        0     1116 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1003 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/distributions/demo-0.1.0.tar.gz
--rw-r--r--   0        0        0     1552 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/distributions/demo-0.1.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1169 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/distributions/demo_invalid_record-0.1.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1307 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/distributions/demo_invalid_record2-0.1.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0       22 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/excluded_subpackage/README.rst
--rw-r--r--   0        0        0       59 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/excluded_subpackage/example/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/excluded_subpackage/example/test/__init__.py
--rw-r--r--   0        0        0      159 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/excluded_subpackage/example/test/excluded.py
--rw-r--r--   0        0        0      329 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/excluded_subpackage/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/extended_project/README.rst
--rw-r--r--   0        0        0      362 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/extended_project/build.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/extended_project/extended_project/__init__.py
--rw-r--r--   0        0        0      652 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/extended_project/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/extended_project_without_setup/README.rst
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/extended_project_without_setup/build.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/extended_project_without_setup/extended_project/__init__.py
--rw-r--r--   0        0        0      756 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/extended_project_without_setup/pyproject.toml
--rw-r--r--   0        0        0       18 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/extended_with_no_setup/README.md
--rw-r--r--   0        0        0      859 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/extended_with_no_setup/build.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/extended_with_no_setup/extended/__init__.py
--rw-r--r--   0        0        0      888 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/extended_with_no_setup/extended/extended.c
--rw-r--r--   0        0        0      581 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/extended_with_no_setup/pyproject.toml
--rw-r--r--   0        0        0       59 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/git/github.com/demo/demo/demo/__init__.py
--rw-r--r--   0        0        0      226 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/git/github.com/demo/demo/demo.egg-info/PKG-INFO
--rw-r--r--   0        0        0      164 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/git/github.com/demo/demo/demo.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/git/github.com/demo/demo/demo.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       43 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/git/github.com/demo/demo/demo.egg-info/requires.txt
--rw-r--r--   0        0        0        5 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/git/github.com/demo/demo/demo.egg-info/top_level.txt
--rw-r--r--   0        0        0      429 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/git/github.com/demo/demo/setup.py
--rw-r--r--   0        0        0       93 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/git/github.com/demo/namespace-package-one/namespace_package/__init__.py
--rw-r--r--   0        0        0       50 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/git/github.com/demo/namespace-package-one/namespace_package/one/__init__.py
--rw-r--r--   0        0        0      402 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/git/github.com/demo/namespace-package-one/setup.py
--rw-r--r--   0        0        0       59 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/git/github.com/demo/no-dependencies/demo/__init__.py
--rw-r--r--   0        0        0      214 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/git/github.com/demo/no-dependencies/demo.egg-info/PKG-INFO
--rw-r--r--   0        0        0      137 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/git/github.com/demo/no-dependencies/demo.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/git/github.com/demo/no-dependencies/demo.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        5 2023-05-19 12:27:02.302399 poetry-1.5.0/tests/fixtures/git/github.com/demo/no-dependencies/demo.egg-info/top_level.txt
--rw-r--r--   0        0        0      329 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/git/github.com/demo/no-dependencies/setup.py
--rw-r--r--   0        0        0       59 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/git/github.com/demo/no-version/demo/__init__.py
--rw-r--r--   0        0        0      696 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/git/github.com/demo/no-version/setup.py
--rw-r--r--   0        0        0      254 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/PKG-INFO
--rw-r--r--   0        0        0      164 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       43 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/requires.txt
--rw-r--r--   0        0        0        5 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/top_level.txt
--rw-r--r--   0        0        0       59 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/git/github.com/demo/non-canonical-name/demo/__init__.py
--rw-r--r--   0        0        0      429 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/git/github.com/demo/non-canonical-name/setup.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/git/github.com/demo/poetry-plugin/poetry_plugin/__init__.py
--rw-r--r--   0        0        0      349 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/git/github.com/demo/poetry-plugin/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/git/github.com/demo/poetry-plugin2/subdir/poetry_plugin/__init__.py
--rw-r--r--   0        0        0      349 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/git/github.com/demo/poetry-plugin2/subdir/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/git/github.com/demo/prerelease/prerelease/__init__.py
--rw-r--r--   0        0        0      268 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/git/github.com/demo/prerelease/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/git/github.com/demo/pyproject-demo/demo/__init__.py
--rw-r--r--   0        0        0      275 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/git/github.com/demo/pyproject-demo/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/git/github.com/demo/subdirectories/one/one/__init__.py
--rw-r--r--   0        0        0      244 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/git/github.com/demo/subdirectories/one/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/git/github.com/demo/subdirectories/one-copy/one/__init__.py
--rw-r--r--   0        0        0      244 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/git/github.com/demo/subdirectories/one-copy/pyproject.toml
--rw-r--r--   0        0        0      252 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/git/github.com/demo/subdirectories/two/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/git/github.com/demo/subdirectories/two/two/__init__.py
--rw-r--r--   0        0        0       34 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/incompatible_lock/poetry.lock
--rw-r--r--   0        0        0      320 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/incompatible_lock/pyproject.toml
--rw-r--r--   0        0        0      378 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/inspection/demo/pyproject.toml
--rw-r--r--   0        0        0      225 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/inspection/demo_no_setup_pkg_info_no_deps/PKG-INFO
--rw-r--r--   0        0        0      461 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/inspection/demo_no_setup_pkg_info_no_deps/pyproject.toml
--rw-r--r--   0        0        0      225 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/inspection/demo_only_requires_txt.egg-info/PKG-INFO
--rw-r--r--   0        0        0       64 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/inspection/demo_only_requires_txt.egg-info/requires.txt
--rw-r--r--   0        0        0      300 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/inspection/demo_poetry_package/pyproject.toml
--rw-r--r--   0        0        0      225 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/inspection/demo_with_obsolete_egg_info/demo-0.1.0.egg-info/PKG-INFO
--rw-r--r--   0        0        0       64 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/inspection/demo_with_obsolete_egg_info/demo-0.1.0.egg-info/requires.txt
--rw-r--r--   0        0        0      378 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/inspection/demo_with_obsolete_egg_info/pyproject.toml
--rw-r--r--   0        0        0       26 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/invalid_lock/poetry.lock
--rw-r--r--   0        0        0      320 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/invalid_lock/pyproject.toml
--rw-r--r--   0        0        0      408 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/invalid_pyproject/pyproject.toml
--rw-r--r--   0        0        0      406 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/missing_directory_dependency/poetry.lock
--rw-r--r--   0        0        0      299 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/missing_directory_dependency/pyproject.toml
--rw-r--r--   0        0        0      428 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/missing_file_dependency/poetry.lock
--rw-r--r--   0        0        0      324 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/missing_file_dependency/pyproject.toml
--rw-r--r--   0        0        0       32 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/no_name_project/README.rst
--rw-r--r--   0        0        0      306 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/no_name_project/pyproject.toml
--rw-r--r--   0        0        0      762 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/old_lock/poetry.lock
--rw-r--r--   0        0        0      320 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/old_lock/pyproject.toml
--rw-r--r--   0        0        0      430 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/old_lock_path_dependency/poetry.lock
--rw-r--r--   0        0        0      336 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/old_lock_path_dependency/pyproject.toml
--rw-r--r--   0        0        0      247 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/old_lock_path_dependency/quix/pyproject.toml
--rw-r--r--   0        0        0     6512 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/outdated_lock/poetry.lock
--rw-r--r--   0        0        0      311 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/outdated_lock/pyproject.toml
--rw-r--r--   0        0        0      309 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/private_pyproject/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/project_with_extras/project_with_extras/__init__.py
--rw-r--r--   0        0        0      402 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/project_with_extras/pyproject.toml
--rw-r--r--   0        0        0      881 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/project_with_git_dev_dependency/pyproject.toml
--rw-r--r--   0        0        0      893 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/project_with_local_dependencies/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/project_with_multi_constraints_dependency/project/__init__.py
--rw-r--r--   0        0        0      394 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/project_with_multi_constraints_dependency/pyproject.toml
--rw-r--r--   0        0        0      264 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/project_with_nested_local/bar/pyproject.toml
--rw-r--r--   0        0        0      262 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/project_with_nested_local/foo/pyproject.toml
--rw-r--r--   0        0        0      324 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/project_with_nested_local/pyproject.toml
--rw-r--r--   0        0        0      221 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/project_with_nested_local/quix/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/project_with_setup/my_package/__init__.py
--rw-r--r--   0        0        0      239 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/project_with_setup/project_with_setup.egg-info/PKG-INFO
--rw-r--r--   0        0        0      201 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/project_with_setup/project_with_setup.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/project_with_setup/project_with_setup.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       38 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/project_with_setup/project_with_setup.egg-info/requires.txt
--rw-r--r--   0        0        0       11 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/project_with_setup/project_with_setup.egg-info/top_level.txt
--rw-r--r--   0        0        0      416 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/project_with_setup/setup.py
--rw-r--r--   0        0        0       22 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/sample_project/README.rst
--rw-r--r--   0        0        0     1501 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/sample_project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/scripts/README.md
--rw-r--r--   0        0        0      400 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/scripts/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/scripts/scripts/__init__.py
--rw-r--r--   0        0        0      557 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/scripts/scripts/check_argv0.py
--rw-r--r--   0        0        0      122 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/scripts/scripts/exit_code.py
--rw-r--r--   0        0        0      128 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/scripts/scripts/return_code.py
--rw-r--r--   0        0        0       22 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/simple_project/README.rst
--rw-r--r--   0        0        0     1320 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1106 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/simple_project/dist/simple_project-1.2.3.tar.gz
--rw-r--r--   0        0        0      775 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/simple_project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/simple_project/simple_project/__init__.py
--rw-r--r--   0        0        0     6404 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/up_to_date_lock/poetry.lock
--rw-r--r--   0        0        0      313 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/up_to_date_lock/pyproject.toml
--rw-r--r--   0        0        0     1722 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/wheel_with_no_requires_dist/demo-0.1.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1062 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/with-include/LICENSE
--rw-r--r--   0        0        0       22 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/with-include/README.rst
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/with-include/extra_dir/README.md
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/with-include/extra_dir/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/with-include/extra_dir/sub_pkg/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/with-include/extra_dir/sub_pkg/vcs_excluded.txt
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/with-include/extra_dir/vcs_excluded.txt
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/with-include/for_wheel_only/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/with-include/my_module.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/with-include/notes.txt
--rw-r--r--   0        0        0       59 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/with-include/package_with_include/__init__.py
--rw-r--r--   0        0        0     1259 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/with-include/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/with-include/src/src_package/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/with-include/tests/__init__.py
--rw-r--r--   0        0        0      153 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/with_conditional_path_deps/demo_one/pyproject.toml
--rw-r--r--   0        0        0      153 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/with_conditional_path_deps/demo_two/pyproject.toml
--rw-r--r--   0        0        0      257 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/with_conditional_path_deps/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/with_default_source/README.rst
--rw-r--r--   0        0        0     1428 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/with_default_source/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/with_default_source_and_pypi/README.rst
--rw-r--r--   0        0        0     1467 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/with_default_source_and_pypi/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/with_default_source_legacy/README.rst
--rw-r--r--   0        0        0     1426 2023-05-19 12:27:02.306399 poetry-1.5.0/tests/fixtures/with_default_source_legacy/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_default_source_pypi/README.rst
--rw-r--r--   0        0        0     1393 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_default_source_pypi/pyproject.toml
--rw-r--r--   0        0        0      370 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_explicit_pypi_and_other/pyproject.toml
--rw-r--r--   0        0        0      402 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_explicit_pypi_and_other_explicit/pyproject.toml
--rw-r--r--   0        0        0      301 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_explicit_pypi_no_other/pyproject.toml
--rw-r--r--   0        0        0      352 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_explicit_source/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_local_config/README.rst
--rw-r--r--   0        0        0       48 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_local_config/poetry.toml
--rw-r--r--   0        0        0     1331 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_local_config/pyproject.toml
--rw-r--r--   0        0        0       28 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_multiple_readme_files/README-1.rst
--rw-r--r--   0        0        0       20 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_multiple_readme_files/README-2.rst
--rw-r--r--   0        0        0       79 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_multiple_readme_files/my_package/__init__.py
--rw-r--r--   0        0        0      286 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_multiple_readme_files/pyproject.toml
--rw-r--r--   0        0        0      425 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_non_default_multiple_secondary_sources/pyproject.toml
--rw-r--r--   0        0        0      413 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_non_default_multiple_secondary_sources_legacy/pyproject.toml
--rw-r--r--   0        0        0      402 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_non_default_multiple_sources/pyproject.toml
--rw-r--r--   0        0        0      396 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_non_default_multiple_sources_legacy/pyproject.toml
--rw-r--r--   0        0        0      509 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_non_default_multiple_sources_pypi/pyproject.toml
--rw-r--r--   0        0        0      333 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_non_default_secondary_source/pyproject.toml
--rw-r--r--   0        0        0      327 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_non_default_secondary_source_legacy/pyproject.toml
--rw-r--r--   0        0        0      331 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_non_default_source_explicit/pyproject.toml
--rw-r--r--   0        0        0      310 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_non_default_source_implicit/pyproject.toml
--rw-r--r--   0        0        0      214 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_path_dependency/bazz/setup.py
--rw-r--r--   0        0        0     3370 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_path_dependency/poetry.lock
--rw-r--r--   0        0        0      305 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_path_dependency/pyproject.toml
--rw-r--r--   0        0        0      364 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_supplemental_source/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_two_default_sources/README.rst
--rw-r--r--   0        0        0     1518 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_two_default_sources/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_two_default_sources_legacy/README.rst
--rw-r--r--   0        0        0     1520 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/fixtures/with_two_default_sources_legacy/pyproject.toml
--rw-r--r--   0        0        0     8794 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/helpers.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/inspection/__init__.py
--rw-r--r--   0        0        0     7707 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/inspection/test_info.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/__init__.py
--rw-r--r--   0        0        0      564 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/extras-with-dependencies.test
--rw-r--r--   0        0        0      530 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/extras.test
--rw-r--r--   0        0        0      402 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/install-no-dev.test
--rw-r--r--   0        0        0       95 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/no-dependencies.test
--rw-r--r--   0        0        0     4081 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/old-lock.test
--rw-r--r--   0        0        0      188 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/remove.test
--rw-r--r--   0        0        0      188 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/update-with-lock.test
--rw-r--r--   0        0        0      698 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/update-with-locked-extras.test
--rw-r--r--   0        0        0      410 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/with-conditional-dependency.test
--rw-r--r--   0        0        0      509 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/with-dependencies-extras.test
--rw-r--r--   0        0        0      631 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/with-dependencies-nested-extras.test
--rw-r--r--   0        0        0      295 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/with-dependencies.test
--rw-r--r--   0        0        0     2168 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/with-directory-dependency-poetry-transitive.test
--rw-r--r--   0        0        0      598 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/with-directory-dependency-poetry.test
--rw-r--r--   0        0        0      641 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/with-directory-dependency-setuptools.test
--rw-r--r--   0        0        0      471 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/with-duplicate-dependencies-update.test
--rw-r--r--   0        0        0      841 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/with-duplicate-dependencies.test
--rw-r--r--   0        0        0     1379 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/with-file-dependency-transitive.test
--rw-r--r--   0        0        0      676 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/with-file-dependency.test
--rw-r--r--   0        0        0      752 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/with-multiple-updates.test
--rw-r--r--   0        0        0      469 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/with-optional-dependencies.test
--rw-r--r--   0        0        0      565 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/with-platform-dependencies.test
--rw-r--r--   0        0        0      297 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/with-prereleases.test
--rw-r--r--   0        0        0     5109 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/with-pypi-repository.test
--rw-r--r--   0        0        0      424 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/with-python-versions.test
--rw-r--r--   0        0        0     1146 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/with-same-version-url-dependencies.test
--rw-r--r--   0        0        0      579 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/with-sub-dependencies.test
--rw-r--r--   0        0        0      686 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/with-url-dependency.test
--rw-r--r--   0        0        0      708 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/with-vcs-dependency-with-extras.test
--rw-r--r--   0        0        0      491 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/with-vcs-dependency-without-ref.test
--rw-r--r--   0        0        0      478 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/fixtures/with-wheel-dependency-no-requires-dist.test
--rw-r--r--   0        0        0     3266 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/test_chef.py
--rw-r--r--   0        0        0    11122 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/test_chooser.py
--rw-r--r--   0        0        0    42642 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/test_executor.py
--rw-r--r--   0        0        0    79863 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/test_installer.py
--rw-r--r--   0        0        0     2706 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/installation/test_wheel_installer.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/integration/__init__.py
--rw-r--r--   0        0        0    12051 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/integration/test_utils_vcs_git.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/json/__init__.py
--rw-r--r--   0        0        0      338 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/json/fixtures/source/complete_invalid_priority.toml
--rw-r--r--   0        0        0      352 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/json/fixtures/source/complete_invalid_priority_legacy_and_new.toml
--rw-r--r--   0        0        0      282 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/json/fixtures/source/complete_invalid_url.toml
--rw-r--r--   0        0        0      337 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/json/fixtures/source/complete_valid.toml
--rw-r--r--   0        0        0      349 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/json/fixtures/source/complete_valid_legacy.toml
--rw-r--r--   0        0        0     1761 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/json/test_schema_sources.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/masonry/builders/__init__.py
--rw-r--r--   0        0        0       22 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/masonry/builders/fixtures/excluded_subpackage/README.rst
--rw-r--r--   0        0        0       59 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/masonry/builders/fixtures/excluded_subpackage/example/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/masonry/builders/fixtures/excluded_subpackage/example/test/__init__.py
--rw-r--r--   0        0        0      176 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/masonry/builders/fixtures/excluded_subpackage/example/test/excluded.py
--rw-r--r--   0        0        0      329 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/masonry/builders/fixtures/excluded_subpackage/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/masonry/builders/fixtures/pep_561_stub_only/pkg-stubs/__init__.pyi
--rw-r--r--   0        0        0       83 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/masonry/builders/fixtures/pep_561_stub_only/pkg-stubs/module.pyi
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/masonry/builders/fixtures/pep_561_stub_only/pkg-stubs/subpkg/__init__.pyi
--rw-r--r--   0        0        0      261 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/masonry/builders/fixtures/pep_561_stub_only/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/__init__.pyi
--rw-r--r--   0        0        0       83 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/module.pyi
--rw-r--r--   0        0        0        8 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/py.typed
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/subpkg/__init__.pyi
--rw-r--r--   0        0        0      291 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pyproject.toml
--rw-r--r--   0        0        0      294 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/masonry/builders/fixtures/pep_561_stub_only_src/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/masonry/builders/fixtures/pep_561_stub_only_src/src/pkg-stubs/__init__.pyi
--rw-r--r--   0        0        0       83 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/masonry/builders/fixtures/pep_561_stub_only_src/src/pkg-stubs/module.pyi
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/masonry/builders/fixtures/pep_561_stub_only_src/src/pkg-stubs/subpkg/__init__.pyi
--rw-r--r--   0        0        0    10586 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/masonry/builders/test_editable_builder.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/mixology/__init__.py
--rw-r--r--   0        0        0     2188 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/mixology/helpers.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/mixology/solutions/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/mixology/solutions/providers/__init__.py
--rw-r--r--   0        0        0     1449 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/mixology/solutions/providers/test_python_requirement_solution_provider.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/mixology/solutions/solutions/__init__.py
--rw-r--r--   0        0        0     1470 2023-05-19 12:27:02.310399 poetry-1.5.0/tests/mixology/solutions/solutions/test_python_requirement_solution.py
--rw-r--r--   0        0        0      109 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/mixology/version_solver/__init__.py
--rw-r--r--   0        0        0     1066 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/mixology/version_solver/conftest.py
--rw-r--r--   0        0        0     6890 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/mixology/version_solver/test_backtracking.py
--rw-r--r--   0        0        0     4326 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/mixology/version_solver/test_basic_graph.py
--rw-r--r--   0        0        0     4415 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/mixology/version_solver/test_dependency_cache.py
--rw-r--r--   0        0        0     1153 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/mixology/version_solver/test_python_constraint.py
--rw-r--r--   0        0        0     5226 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/mixology/version_solver/test_unsolvable.py
--rw-r--r--   0        0        0     7700 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/mixology/version_solver/test_with_lock.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/packages/__init__.py
--rw-r--r--   0        0        0     1890 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/packages/test_direct_origin.py
--rw-r--r--   0        0        0    30095 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/packages/test_locker.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/plugins/__init__.py
--rw-r--r--   0        0        0     3198 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/plugins/test_plugin_manager.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/publishing/__init__.py
--rw-r--r--   0        0        0     6438 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/publishing/test_publisher.py
--rw-r--r--   0        0        0     4720 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/publishing/test_uploader.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/puzzle/__init__.py
--rw-r--r--   0        0        0      528 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/puzzle/conftest.py
--rw-r--r--   0        0        0    23737 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/puzzle/test_provider.py
--rw-r--r--   0        0        0   124462 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/puzzle/test_solver.py
--rw-r--r--   0        0        0     5634 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/puzzle/test_transaction.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/pyproject/__init__.py
--rw-r--r--   0        0        0      813 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/pyproject/conftest.py
--rw-r--r--   0        0        0     1379 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/pyproject/test_pyproject_toml.py
--rw-r--r--   0        0        0      755 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/pyproject/test_pyproject_toml_file.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/__init__.py
--rw-r--r--   0        0        0    16009 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/cleo-0.7.6.dist-info/METADATA
--rw-r--r--   0        0        0      110 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/directory_pep_610-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0       81 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/directory_pep_610-1.2.3.dist-info/direct_url.json
--rw-r--r--   0        0        0      719 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-2.3.4.dist-info/METADATA
--rw-r--r--   0        0        0      731 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-with-import-2.3.4.dist-info/METADATA
--rw-r--r--   0        0        0       10 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-with-import.pth
--rw-r--r--   0        0        0       18 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable.pth
--rw-r--r--   0        0        0      119 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable_directory_pep_610-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0      105 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable_directory_pep_610-1.2.3.dist-info/direct_url.json
--rw-r--r--   0        0        0      105 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/file_pep_610-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0      182 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/file_pep_610-1.2.3.dist-info/direct_url.json
--rw-r--r--   0        0        0     1306 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/foo-0.1.0-py3.8.egg
--rw-r--r--   0        0        0      104 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0      159 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610-1.2.3.dist-info/direct_url.json
--rw-r--r--   0        0        0      125 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610_no_requested_version-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0      141 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610_no_requested_version-1.2.3.dist-info/direct_url.json
--rw-r--r--   0        0        0      117 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610_subdirectory-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0      200 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610_subdirectory-1.2.3.dist-info/direct_url.json
--rw-r--r--   0        0        0      719 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/standard-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0        9 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/standard.pth
--rw-r--r--   0        0        0      104 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/url_pep_610-1.2.3.dist-info/METADATA
--rw-r--r--   0        0        0      102 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/url_pep_610-1.2.3.dist-info/direct_url.json
--rw-r--r--   0        0        0      717 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/bender-2.0.5.dist-info/METADATA
--rw-r--r--   0        0        0       20 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/bender.pth
--rw-r--r--   0        0        0      710 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/lib64-2.3.4.dist-info/METADATA
--rw-r--r--   0        0        0      717 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/src/bender/bender.egg-info/PKG-INFO
--rw-r--r--   0        0        0     8866 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/src/pendulum/pendulum.egg-info/PKG-INFO
--rw-r--r--   0        0        0       87 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/src/pendulum/pendulum.egg-info/requires.txt
--rw-r--r--   0        0        0     9020 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/installed/vendor/py3.7/attrs-19.3.0.dist-info/METADATA
--rw-r--r--   0        0        0      731 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/legacy/absolute.html
--rw-r--r--   0        0        0      790 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/legacy/black.html
--rw-r--r--   0        0        0     1455 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/legacy/clikit.html
--rw-r--r--   0        0        0      746 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/legacy/discord-py.html
--rw-r--r--   0        0        0      759 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/legacy/futures-partial-yank.html
--rw-r--r--   0        0        0      747 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/legacy/futures.html
--rw-r--r--   0        0        0      625 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/legacy/invalid-version.html
--rw-r--r--   0        0        0     1433 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/legacy/ipython.html
--rw-r--r--   0        0        0      917 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/legacy/isort.html
--rw-r--r--   0        0        0      333 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/legacy/jupyter.html
--rw-r--r--   0        0        0      348 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/legacy/missing-version.html
--rw-r--r--   0        0        0      401 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/legacy/pastel.html
--rw-r--r--   0        0        0      534 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/legacy/poetry-test-py2-py3-metadata-merge.html
--rw-r--r--   0        0        0      802 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/legacy/pytest.html
--rw-r--r--   0        0        0      467 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/legacy/python-language-server.html
--rw-r--r--   0        0        0      941 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/legacy/pyyaml.html
--rw-r--r--   0        0        0      687 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/legacy/relative.html
--rw-r--r--   0        0        0      473 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/legacy/tomlkit.html
--rw-r--r--   0        0        0    18499 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/SQLAlchemy-1.2.12.tar.gz
--rw-r--r--   0        0        0     9634 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/Twisted-18.9.0.tar.bz2
--rw-r--r--   0        0        0     1940 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/black-19.10b0-py36-none-any.whl
--rw-r--r--   0        0        0    14949 2023-05-19 12:27:02.314399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/black-21.11b0-py3-none-any.whl
--rw-r--r--   0        0        0    78701 2023-05-19 12:27:02.318399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/cleo-1.0.0a5-py3-none-any.whl
--rw-r--r--   0        0        0     2329 2023-05-19 12:27:02.318399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/clikit-0.2.4-py2.py3-none-any.whl
--rw-r--r--   0        0        0     2290 2023-05-19 12:27:02.318399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/discord.py-2.0.0-py3-none-any.whl
--rw-r--r--   0        0        0    15847 2023-05-19 12:27:02.318399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0-py2-none-any.whl
--rw-r--r--   0        0        0    18359 2023-05-19 12:27:02.318399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0.tar.gz
--rw-r--r--   0        0        0    31809 2023-05-19 12:27:02.318399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/importlib_metadata-1.7.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0    23473 2023-05-19 12:27:02.318399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py2-none-any.whl
--rw-r--r--   0        0        0    23475 2023-05-19 12:27:02.318399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py3-none-any.whl
--rw-r--r--   0        0        0    15795 2023-05-19 12:27:02.318399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0.tar.gz
--rw-r--r--   0        0        0    22352 2023-05-19 12:27:02.318399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/ipython-7.5.0-py3-none-any.whl
--rw-r--r--   0        0        0    45393 2023-05-19 12:27:02.318399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py2-none-any.whl
--rw-r--r--   0        0        0    45352 2023-05-19 12:27:02.318399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py3-none-any.whl
--rw-r--r--   0        0        0    56070 2023-05-19 12:27:02.318399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4.tar.gz
--rw-r--r--   0        0        0     2736 2023-05-19 12:27:02.318399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0    12916 2023-05-19 12:27:02.318399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0.tar.gz
--rw-r--r--   0        0        0     4490 2023-05-19 12:27:02.318399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/pastel-0.1.0.tar.gz
--rw-r--r--   0        0        0   464992 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/poetry_core-1.5.0-py3-none-any.whl
--rw-r--r--   0        0        0     1213 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py2-none-any.whl
--rw-r--r--   0        0        0     1218 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py3-none-any.whl
--rw-r--r--   0        0        0     3691 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/pytest-3.5.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0     3708 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/pytest-3.5.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0    54076 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/python-language-server-0.21.2.tar.gz
--rw-r--r--   0        0        0    29813 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.2.tar.gz
--rw-r--r--   0        0        0    29864 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.3.tar.gz
--rw-r--r--   0        0        0     5700 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/zipp-3.5.0-py3-none-any.whl
--rw-r--r--   0        0        0     3421 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/attrs/17.4.0.json
--rw-r--r--   0        0        0      856 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/attrs.json
--rw-r--r--   0        0        0    62683 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/black/19.10b0.json
--rw-r--r--   0        0        0     5924 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/black/21.11b0.json
--rw-r--r--   0        0        0     1709 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/black.json
--rw-r--r--   0        0        0     2298 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/cachecontrol/0.12.5.json
--rw-r--r--   0        0        0     2425 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/cachecontrol.json
--rw-r--r--   0        0        0     3035 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/cleo/1.0.0a5.json
--rw-r--r--   0        0        0     3745 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/clikit/0.2.4.json
--rw-r--r--   0        0        0      997 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/clikit.json
--rw-r--r--   0        0        0     2922 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/colorama/0.3.9.json
--rw-r--r--   0        0        0      867 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/colorama.json
--rw-r--r--   0        0        0     4035 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/discord-py/2.0.0.json
--rw-r--r--   0        0        0     2944 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/funcsigs/1.0.2.json
--rw-r--r--   0        0        0      867 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/funcsigs.json
--rw-r--r--   0        0        0     3838 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/hbmqtt/0.9.6.json
--rw-r--r--   0        0        0    14437 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/hbmqtt.json
--rw-r--r--   0        0        0     5331 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/importlib-metadata/1.7.0.json
--rw-r--r--   0        0        0     1065 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/importlib-metadata.json
--rw-r--r--   0        0        0     5984 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/ipython/4.1.0rc1.json
--rw-r--r--   0        0        0    21476 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/isort/4.3.4.json
--rw-r--r--   0        0        0     1221 2023-05-19 12:27:02.322399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/isort.json
--rw-r--r--   0        0        0     3969 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/jupyter/1.0.0.json
--rw-r--r--   0        0        0     1217 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/jupyter.json
--rw-r--r--   0        0        0     2931 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/lockfile/0.12.2.json
--rw-r--r--   0        0        0      871 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/lockfile.json
--rw-r--r--   0        0        0     3552 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/more-itertools/4.1.0.json
--rw-r--r--   0        0        0     1284 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/more-itertools.json
--rw-r--r--   0        0        0     2328 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/pluggy/0.6.0.json
--rw-r--r--   0        0        0      470 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/pluggy.json
--rw-r--r--   0        0        0     3180 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/poetry/0.12.4.json
--rw-r--r--   0        0        0     3555 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/poetry-core/1.5.0.json
--rw-r--r--   0        0        0      897 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/poetry-core.json
--rw-r--r--   0        0        0     4561 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/poetry.json
--rw-r--r--   0        0        0     3095 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/py/1.5.3.json
--rw-r--r--   0        0        0      837 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/py.json
--rw-r--r--   0        0        0      931 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/pygame-music-grid.json
--rw-r--r--   0        0        0     4469 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/pylev/1.3.0.json
--rw-r--r--   0        0        0      495 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/pylev.json
--rw-r--r--   0        0        0     6933 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/pytest/3.5.0.json
--rw-r--r--   0        0        0     7555 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/pytest/3.5.1.json
--rw-r--r--   0        0        0      857 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/pytest.json
--rw-r--r--   0        0        0    14143 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/pyyaml/3.13.0.json
--rw-r--r--   0        0        0     7805 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/pyyaml.json
--rw-r--r--   0        0        0     3142 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/requests/2.18.4.json
--rw-r--r--   0        0        0    67409 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/requests.json
--rw-r--r--   0        0        0     5315 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/setuptools/39.2.0.json
--rw-r--r--   0        0        0     8423 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/setuptools/67.6.1.json
--rw-r--r--   0        0        0     1843 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/setuptools.json
--rw-r--r--   0        0        0     2387 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/six/1.11.0.json
--rw-r--r--   0        0        0      846 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/six.json
--rw-r--r--   0        0        0     8870 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/sqlalchemy/1.2.12.json
--rw-r--r--   0        0        0      484 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/sqlalchemy.json
--rw-r--r--   0        0        0     6109 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/toga.json
--rw-r--r--   0        0        0    11126 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/tomlkit/0.5.3.json
--rw-r--r--   0        0        0     1892 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/tomlkit.json
--rw-r--r--   0        0        0     3184 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/trackpy/0.4.1.json
--rw-r--r--   0        0        0      838 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/trackpy.json
--rw-r--r--   0        0        0    11606 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/twisted/18.9.0.json
--rw-r--r--   0        0        0      477 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/twisted.json
--rw-r--r--   0        0        0     4483 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/wheel/0.40.0.json
--rw-r--r--   0        0        0     1041 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/wheel.json
--rw-r--r--   0        0        0     5188 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/zipp/3.5.0.json
--rw-r--r--   0        0        0      907 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/zipp.json
--rw-r--r--   0        0        0   224197 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/pypi.org/search/search.html
--rw-r--r--   0        0        0     3407 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/fixtures/single-page/jax_releases.html
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/link_sources/__init__.py
--rw-r--r--   0        0        0     3108 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/link_sources/test_base.py
--rw-r--r--   0        0        0     2999 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/link_sources/test_html.py
--rw-r--r--   0        0        0    10933 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/test_installed_repository.py
--rw-r--r--   0        0        0    17437 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/test_legacy_repository.py
--rw-r--r--   0        0        0     1788 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/test_lockfile_repository.py
--rw-r--r--   0        0        0    11500 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/test_pypi_repository.py
--rw-r--r--   0        0        0     2321 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/test_repository.py
--rw-r--r--   0        0        0    12604 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/test_repository_pool.py
--rw-r--r--   0        0        0     1998 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/repositories/test_single_page_repository.py
--rw-r--r--   0        0        0    20928 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/test_factory.py
--rw-r--r--   0        0        0      399 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/test_helpers.py
--rw-r--r--   0        0        0     1665 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/types.py
--rw-r--r--   0        0        0        0 2023-05-19 12:27:02.326399 poetry-1.5.0/tests/utils/__init__.py
--rw-r--r--   0        0        0      384 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/conftest.py
--rw-r--r--   0        0        0      604 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/fixtures/pyproject.toml
--rw-r--r--   0        0        0      371 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/fixtures/setups/ansible/requirements.txt
--rw-r--r--   0        0        0    10765 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/fixtures/setups/ansible/setup.py
--rw-r--r--   0        0        0      271 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/fixtures/setups/extras_require_with_vars/setup.py
--rw-r--r--   0        0        0     2581 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/fixtures/setups/flask/setup.py
--rw-r--r--   0        0        0     1353 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/fixtures/setups/pendulum/setup.py
--rw-r--r--   0        0        0    11825 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/fixtures/setups/pyyaml/setup.py
--rw-r--r--   0        0        0     3366 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/fixtures/setups/requests/setup.py
--rw-r--r--   0        0        0      290 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/fixtures/setups/setuptools_setup/setup.py
--rw-r--r--   0        0        0     6272 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/fixtures/setups/sqlalchemy/setup.py
--rw-r--r--   0        0        0      302 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/fixtures/setups/with-setup-cfg/setup.cfg
--rw-r--r--   0        0        0       75 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/fixtures/setups/with-setup-cfg/setup.py
--rw-r--r--   0        0        0      339 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/fixtures/setups/with-setup-cfg-attr/setup.cfg
--rw-r--r--   0        0        0       75 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/fixtures/setups/with-setup-cfg-attr/setup.py
--rw-r--r--   0        0        0    20949 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/test_authenticator.py
--rw-r--r--   0        0        0    12266 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/test_cache.py
--rw-r--r--   0        0        0     5922 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/test_dependency_specification.py
--rw-r--r--   0        0        0    56209 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/test_env.py
--rw-r--r--   0        0        0     1562 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/test_env_site.py
--rw-r--r--   0        0        0     2374 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/test_extras.py
--rw-r--r--   0        0        0     4953 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/test_helpers.py
--rw-r--r--   0        0        0     8460 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/test_password_manager.py
--rw-r--r--   0        0        0     1114 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/test_patterns.py
--rw-r--r--   0        0        0     1092 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/test_pip.py
--rw-r--r--   0        0        0     6756 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/test_setup_reader.py
--rw-r--r--   0        0        0     2182 2023-05-19 12:27:02.330399 poetry-1.5.0/tests/utils/test_source.py
--rw-r--r--   0        0        0     6968 1970-01-01 00:00:00.000000 poetry-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-29 16:05:02.480011 poetry-1.5.1/LICENSE
+-rw-r--r--   0        0        0     4547 2023-05-29 16:05:02.480011 poetry-1.5.1/README.md
+-rw-r--r--   0        0        0     5512 2023-05-29 16:05:02.496012 poetry-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0      146 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/__main__.py
+-rw-r--r--   0        0        0      342 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/__version__.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/config/__init__.py
+-rw-r--r--   0        0        0     9746 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/config/config.py
+-rw-r--r--   0        0        0      261 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/config/config_source.py
+-rw-r--r--   0        0        0     1018 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/config/dict_config_source.py
+-rw-r--r--   0        0        0     2339 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/config/file_config_source.py
+-rw-r--r--   0        0        0     1396 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/config/source.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/__init__.py
+-rw-r--r--   0        0        0    12551 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/application.py
+-rw-r--r--   0        0        0      615 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/command_loader.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/__init__.py
+-rw-r--r--   0        0        0      893 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/about.py
+-rw-r--r--   0        0        0    10690 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/add.py
+-rw-r--r--   0        0        0     1081 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/build.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/cache/__init__.py
+-rw-r--r--   0        0        0     2411 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/cache/clear.py
+-rw-r--r--   0        0        0      634 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/cache/list.py
+-rw-r--r--   0        0        0     3360 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/check.py
+-rw-r--r--   0        0        0     1118 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/command.py
+-rw-r--r--   0        0        0    11027 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/config.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/debug/__init__.py
+-rw-r--r--   0        0        0      764 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/debug/info.py
+-rw-r--r--   0        0        0     4484 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/debug/resolve.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/env/__init__.py
+-rw-r--r--   0        0        0     2600 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/env/info.py
+-rw-r--r--   0        0        0      822 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/env/list.py
+-rw-r--r--   0        0        0     1478 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/env/remove.py
+-rw-r--r--   0        0        0      706 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/env/use.py
+-rw-r--r--   0        0        0      544 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/env_command.py
+-rw-r--r--   0        0        0     4370 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/group_command.py
+-rw-r--r--   0        0        0    17346 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/init.py
+-rw-r--r--   0        0        0     6637 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/install.py
+-rw-r--r--   0        0        0      907 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/installer_command.py
+-rw-r--r--   0        0        0     1513 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/lock.py
+-rw-r--r--   0        0        0     3000 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/new.py
+-rw-r--r--   0        0        0     2776 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/publish.py
+-rw-r--r--   0        0        0     5163 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/remove.py
+-rw-r--r--   0        0        0     3261 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/run.py
+-rw-r--r--   0        0        0      786 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/search.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/self/__init__.py
+-rw-r--r--   0        0        0     1261 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/self/add.py
+-rw-r--r--   0        0        0      973 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/self/install.py
+-rw-r--r--   0        0        0      642 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/self/lock.py
+-rw-r--r--   0        0        0      607 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/self/remove.py
+-rw-r--r--   0        0        0     4503 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/self/self_command.py
+-rw-r--r--   0        0        0     1209 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/self/show/__init__.py
+-rw-r--r--   0        0        0     4036 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/self/show/plugins.py
+-rw-r--r--   0        0        0     1802 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/self/update.py
+-rw-r--r--   0        0        0     1527 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/shell.py
+-rw-r--r--   0        0        0    20399 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/show.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/source/__init__.py
+-rw-r--r--   0        0        0     5487 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/source/add.py
+-rw-r--r--   0        0        0     1181 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/source/remove.py
+-rw-r--r--   0        0        0     1614 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/source/show.py
+-rw-r--r--   0        0        0     1547 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/update.py
+-rw-r--r--   0        0        0     3775 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/commands/version.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/events/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/events/console_events.py
+-rw-r--r--   0        0        0      174 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/io/inputs/__init__.py
+-rw-r--r--   0        0        0     2516 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/io/inputs/run_argv_input.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/logging/__init__.py
+-rw-r--r--   0        0        0       99 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/logging/filters.py
+-rw-r--r--   0        0        0      336 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/logging/formatters/__init__.py
+-rw-r--r--   0        0        0      788 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/logging/formatters/builder_formatter.py
+-rw-r--r--   0        0        0      132 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/logging/formatters/formatter.py
+-rw-r--r--   0        0        0     1026 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/logging/io_formatter.py
+-rw-r--r--   0        0        0      702 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/console/logging/io_handler.py
+-rw-r--r--   0        0        0      134 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/exceptions.py
+-rw-r--r--   0        0        0    13389 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/factory.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.496012 poetry-1.5.1/src/poetry/inspection/__init__.py
+-rw-r--r--   0        0        0    21805 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/inspection/info.py
+-rw-r--r--   0        0        0      114 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/installation/__init__.py
+-rw-r--r--   0        0        0     6441 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/installation/chef.py
+-rw-r--r--   0        0        0     6887 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/installation/chooser.py
+-rw-r--r--   0        0        0    37137 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/installation/executor.py
+-rw-r--r--   0        0        0    15285 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/installation/installer.py
+-rw-r--r--   0        0        0      262 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/installation/operations/__init__.py
+-rw-r--r--   0        0        0      906 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/installation/operations/install.py
+-rw-r--r--   0        0        0     1315 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/installation/operations/operation.py
+-rw-r--r--   0        0        0      959 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/installation/operations/uninstall.py
+-rw-r--r--   0        0        0     1540 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/installation/operations/update.py
+-rw-r--r--   0        0        0     3967 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/installation/wheel_installer.py
+-rw-r--r--   0        0        0     1281 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/json/__init__.py
+-rw-r--r--   0        0        0     2127 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/json/schemas/poetry.json
+-rw-r--r--   0        0        0      310 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/layouts/__init__.py
+-rw-r--r--   0        0        0     5970 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/layouts/layout.py
+-rw-r--r--   0        0        0      202 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/layouts/src.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/layouts/standard.py
+-rw-r--r--   0        0        0     1669 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/locations.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/masonry/__init__.py
+-rw-r--r--   0        0        0      497 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/masonry/api.py
+-rw-r--r--   0        0        0      129 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/masonry/builders/__init__.py
+-rw-r--r--   0        0        0     9537 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/masonry/builders/editable.py
+-rw-r--r--   0        0        0      467 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/mixology/__init__.py
+-rw-r--r--   0        0        0     1555 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/mixology/assignment.py
+-rw-r--r--   0        0        0    10186 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/mixology/failure.py
+-rw-r--r--   0        0        0    15346 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/mixology/incompatibility.py
+-rw-r--r--   0        0        0     1903 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/mixology/incompatibility_cause.py
+-rw-r--r--   0        0        0     7080 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/mixology/partial_solution.py
+-rw-r--r--   0        0        0      676 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/mixology/result.py
+-rw-r--r--   0        0        0      211 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/mixology/set_relation.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/mixology/solutions/__init__.py
+-rw-r--r--   0        0        0      214 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/mixology/solutions/providers/__init__.py
+-rw-r--r--   0        0        0     1091 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/mixology/solutions/providers/python_requirement_solution_provider.py
+-rw-r--r--   0        0        0      189 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/mixology/solutions/solutions/__init__.py
+-rw-r--r--   0        0        0     2281 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/mixology/solutions/solutions/python_requirement_solution.py
+-rw-r--r--   0        0        0     6904 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/mixology/term.py
+-rw-r--r--   0        0        0    22904 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/mixology/version_solver.py
+-rw-r--r--   0        0        0      273 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/packages/__init__.py
+-rw-r--r--   0        0        0     1297 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/packages/dependency_package.py
+-rw-r--r--   0        0        0     3352 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/packages/direct_origin.py
+-rw-r--r--   0        0        0    17760 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/packages/locker.py
+-rw-r--r--   0        0        0      921 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/packages/package_collection.py
+-rw-r--r--   0        0        0      185 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/plugins/__init__.py
+-rw-r--r--   0        0        0      687 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/plugins/application_plugin.py
+-rw-r--r--   0        0        0      435 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/plugins/base_plugin.py
+-rw-r--r--   0        0        0      484 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/plugins/plugin.py
+-rw-r--r--   0        0        0     2537 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/plugins/plugin_manager.py
+-rw-r--r--   0        0        0     2491 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/poetry.py
+-rw-r--r--   0        0        0      112 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/publishing/__init__.py
+-rw-r--r--   0        0        0     2893 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/publishing/publisher.py
+-rw-r--r--   0        0        0    12586 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/publishing/uploader.py
+-rw-r--r--   0        0        0       99 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/puzzle/__init__.py
+-rw-r--r--   0        0        0      799 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/puzzle/exceptions.py
+-rw-r--r--   0        0        0    37505 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/puzzle/provider.py
+-rw-r--r--   0        0        0    11184 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/puzzle/solver.py
+-rw-r--r--   0        0        0     5304 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/puzzle/transaction.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/py.typed
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/pyproject/__init__.py
+-rw-r--r--   0        0        0     1740 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/pyproject/toml.py
+-rw-r--r--   0        0        0      198 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/repositories/__init__.py
+-rw-r--r--   0        0        0      833 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/repositories/abstract_repository.py
+-rw-r--r--   0        0        0     2553 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/repositories/cached_repository.py
+-rw-r--r--   0        0        0      173 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/repositories/exceptions.py
+-rw-r--r--   0        0        0    11241 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/repositories/http_repository.py
+-rw-r--r--   0        0        0    10307 2023-05-29 16:05:02.500012 poetry-1.5.1/src/poetry/repositories/installed_repository.py
+-rw-r--r--   0        0        0     4474 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/repositories/legacy_repository.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/repositories/link_sources/__init__.py
+-rw-r--r--   0        0        0     3835 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/repositories/link_sources/base.py
+-rw-r--r--   0        0        0     1955 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/repositories/link_sources/html.py
+-rw-r--r--   0        0        0     1227 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/repositories/link_sources/json.py
+-rw-r--r--   0        0        0      841 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/repositories/lockfile_repository.py
+-rw-r--r--   0        0        0     8417 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/repositories/pypi_repository.py
+-rw-r--r--   0        0        0     3978 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/repositories/repository.py
+-rw-r--r--   0        0        0     6646 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/repositories/repository_pool.py
+-rw-r--r--   0        0        0      753 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/repositories/single_page_repository.py
+-rw-r--r--   0        0        0      157 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/toml/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/toml/exceptions.py
+-rw-r--r--   0        0        0     1364 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/toml/file.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/utils/__init__.py
+-rw-r--r--   0        0        0     1565 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/utils/_compat.py
+-rw-r--r--   0        0        0    16980 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/utils/authenticator.py
+-rw-r--r--   0        0        0     8537 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/utils/cache.py
+-rw-r--r--   0        0        0      302 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/utils/constants.py
+-rw-r--r--   0        0        0     7625 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/utils/dependency_specification.py
+-rw-r--r--   0        0        0    65484 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/utils/env.py
+-rw-r--r--   0        0        0     1857 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/utils/extras.py
+-rw-r--r--   0        0        0     7409 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/utils/helpers.py
+-rw-r--r--   0        0        0     7151 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/utils/password_manager.py
+-rw-r--r--   0        0        0      406 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/utils/patterns.py
+-rw-r--r--   0        0        0     1446 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/utils/pip.py
+-rw-r--r--   0        0        0    12018 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/utils/setup_reader.py
+-rw-r--r--   0        0        0     4471 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/utils/shell.py
+-rw-r--r--   0        0        0      446 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/utils/source.py
+-rw-r--r--   0        0        0     1361 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/utils/wheel.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/vcs/__init__.py
+-rw-r--r--   0        0        0       95 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/vcs/git/__init__.py
+-rw-r--r--   0        0        0    16083 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/vcs/git/backend.py
+-rw-r--r--   0        0        0     1787 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/vcs/git/system.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/version/__init__.py
+-rw-r--r--   0        0        0     1573 2023-05-29 16:05:02.504012 poetry-1.5.1/src/poetry/version/version_selector.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/__init__.py
+-rw-r--r--   0        0        0      281 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/compat.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/config/__init__.py
+-rw-r--r--   0        0        0     2436 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/config/test_config.py
+-rw-r--r--   0        0        0    13408 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/cache/__init__.py
+-rw-r--r--   0        0        0     1458 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/cache/conftest.py
+-rw-r--r--   0        0        0     2269 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/cache/test_clear.py
+-rw-r--r--   0        0        0      832 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/cache/test_list.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/debug/__init__.py
+-rw-r--r--   0        0        0     1807 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/debug/test_resolve.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/env/__init__.py
+-rw-r--r--   0        0        0     2349 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/env/conftest.py
+-rw-r--r--   0        0        0     1163 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/env/helpers.py
+-rw-r--r--   0        0        0     1592 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/env/test_info.py
+-rw-r--r--   0        0        0     2039 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/env/test_list.py
+-rw-r--r--   0        0        0     2920 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/env/test_remove.py
+-rw-r--r--   0        0        0     4701 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/env/test_use.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/self/__init__.py
+-rw-r--r--   0        0        0     2244 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/self/conftest.py
+-rw-r--r--   0        0        0       65 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/self/fixtures/poetry-1.0.5-darwin.sha256sum
+-rw-r--r--   0        0        0     1041 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/self/fixtures/poetry-1.0.5-darwin.tar.gz
+-rw-r--r--   0        0        0     7543 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/self/test_add_plugins.py
+-rw-r--r--   0        0        0     3034 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/self/test_remove_plugins.py
+-rw-r--r--   0        0        0     1596 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/self/test_self_command.py
+-rw-r--r--   0        0        0     5885 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/self/test_show_plugins.py
+-rw-r--r--   0        0        0     2151 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/self/test_update.py
+-rw-r--r--   0        0        0     1167 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/self/utils.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/source/__init__.py
+-rw-r--r--   0        0        0     4105 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/source/conftest.py
+-rw-r--r--   0        0        0    10226 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/source/test_add.py
+-rw-r--r--   0        0        0     2902 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/source/test_remove.py
+-rw-r--r--   0        0        0     4943 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/source/test_show.py
+-rw-r--r--   0        0        0      835 2023-05-29 16:05:02.504012 poetry-1.5.1/tests/console/commands/test_about.py
+-rw-r--r--   0        0        0    43041 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/console/commands/test_add.py
+-rw-r--r--   0        0        0     1330 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/console/commands/test_build.py
+-rw-r--r--   0        0        0     2032 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/console/commands/test_check.py
+-rw-r--r--   0        0        0    16027 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/console/commands/test_config.py
+-rw-r--r--   0        0        0    29808 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/console/commands/test_init.py
+-rw-r--r--   0        0        0    14192 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/console/commands/test_install.py
+-rw-r--r--   0        0        0    10295 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/console/commands/test_lock.py
+-rw-r--r--   0        0        0     6001 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/console/commands/test_new.py
+-rw-r--r--   0        0        0     3758 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/console/commands/test_publish.py
+-rw-r--r--   0        0        0    10882 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/console/commands/test_remove.py
+-rw-r--r--   0        0        0     6649 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/console/commands/test_run.py
+-rw-r--r--   0        0        0     2568 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/console/commands/test_search.py
+-rw-r--r--   0        0        0     2568 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/console/commands/test_shell.py
+-rw-r--r--   0        0        0    68924 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/console/commands/test_show.py
+-rw-r--r--   0        0        0     2341 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/console/commands/test_update.py
+-rw-r--r--   0        0        0     2588 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/console/commands/test_version.py
+-rw-r--r--   0        0        0     4627 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/console/conftest.py
+-rw-r--r--   0        0        0     3277 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/console/test_application.py
+-rw-r--r--   0        0        0       22 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/build_system_requires_not_available/README.rst
+-rw-r--r--   0        0        0      676 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/build_system_requires_not_available/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/build_system_requires_not_available/simple_project/__init__.py
+-rw-r--r--   0        0        0     1168 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/complete.toml
+-rw-r--r--   0        0        0      406 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/deleted_directory_dependency/poetry.lock
+-rw-r--r--   0        0        0      234 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/deleted_directory_dependency/pyproject.toml
+-rw-r--r--   0        0        0      428 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/deleted_file_dependency/poetry.lock
+-rw-r--r--   0        0        0      234 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/deleted_file_dependency/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/directory/project_with_transitive_directory_dependencies/project_with_transitive_directory_dependencies/__init__.py
+-rw-r--r--   0        0        0      418 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/directory/project_with_transitive_directory_dependencies/pyproject.toml
+-rw-r--r--   0        0        0      574 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/directory/project_with_transitive_directory_dependencies/setup.py
+-rw-r--r--   0        0        0      234 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/directory/project_with_transitive_file_dependencies/inner-directory-project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/directory/project_with_transitive_file_dependencies/project_with_transitive_file_dependencies/__init__.py
+-rw-r--r--   0        0        0      385 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/directory/project_with_transitive_file_dependencies/pyproject.toml
+-rw-r--r--   0        0        0     1116 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1003 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/distributions/demo-0.1.0.tar.gz
+-rw-r--r--   0        0        0     1552 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/distributions/demo-0.1.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1169 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/distributions/demo_invalid_record-0.1.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1307 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/distributions/demo_invalid_record2-0.1.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0       22 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/excluded_subpackage/README.rst
+-rw-r--r--   0        0        0       59 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/excluded_subpackage/example/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/excluded_subpackage/example/test/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/excluded_subpackage/example/test/excluded.py
+-rw-r--r--   0        0        0      329 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/excluded_subpackage/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/extended_project/README.rst
+-rw-r--r--   0        0        0      362 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/extended_project/build.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/extended_project/extended_project/__init__.py
+-rw-r--r--   0        0        0      652 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/extended_project/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/extended_project_without_setup/README.rst
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/extended_project_without_setup/build.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/extended_project_without_setup/extended_project/__init__.py
+-rw-r--r--   0        0        0      756 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/extended_project_without_setup/pyproject.toml
+-rw-r--r--   0        0        0       18 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/extended_with_no_setup/README.md
+-rw-r--r--   0        0        0      859 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/extended_with_no_setup/build.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/extended_with_no_setup/extended/__init__.py
+-rw-r--r--   0        0        0      888 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/extended_with_no_setup/extended/extended.c
+-rw-r--r--   0        0        0      581 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/extended_with_no_setup/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/git/github.com/demo/demo/demo/__init__.py
+-rw-r--r--   0        0        0      226 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/git/github.com/demo/demo/demo.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      164 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/git/github.com/demo/demo/demo.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/git/github.com/demo/demo/demo.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       43 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/git/github.com/demo/demo/demo.egg-info/requires.txt
+-rw-r--r--   0        0        0        5 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/git/github.com/demo/demo/demo.egg-info/top_level.txt
+-rw-r--r--   0        0        0      429 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/git/github.com/demo/demo/setup.py
+-rw-r--r--   0        0        0       93 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/git/github.com/demo/namespace-package-one/namespace_package/__init__.py
+-rw-r--r--   0        0        0       50 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/git/github.com/demo/namespace-package-one/namespace_package/one/__init__.py
+-rw-r--r--   0        0        0      402 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/git/github.com/demo/namespace-package-one/setup.py
+-rw-r--r--   0        0        0       59 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/git/github.com/demo/no-dependencies/demo/__init__.py
+-rw-r--r--   0        0        0      214 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/git/github.com/demo/no-dependencies/demo.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      137 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/git/github.com/demo/no-dependencies/demo.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/git/github.com/demo/no-dependencies/demo.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        5 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/git/github.com/demo/no-dependencies/demo.egg-info/top_level.txt
+-rw-r--r--   0        0        0      329 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/git/github.com/demo/no-dependencies/setup.py
+-rw-r--r--   0        0        0       59 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/git/github.com/demo/no-version/demo/__init__.py
+-rw-r--r--   0        0        0      696 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/git/github.com/demo/no-version/setup.py
+-rw-r--r--   0        0        0      254 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      164 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2023-05-29 16:05:02.508013 poetry-1.5.1/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       43 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/requires.txt
+-rw-r--r--   0        0        0        5 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/git/github.com/demo/non-canonical-name/Demo.egg-info/top_level.txt
+-rw-r--r--   0        0        0       59 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/git/github.com/demo/non-canonical-name/demo/__init__.py
+-rw-r--r--   0        0        0      429 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/git/github.com/demo/non-canonical-name/setup.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/git/github.com/demo/poetry-plugin/poetry_plugin/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/git/github.com/demo/poetry-plugin/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/git/github.com/demo/poetry-plugin2/subdir/poetry_plugin/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/git/github.com/demo/poetry-plugin2/subdir/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/git/github.com/demo/prerelease/prerelease/__init__.py
+-rw-r--r--   0        0        0      268 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/git/github.com/demo/prerelease/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/git/github.com/demo/pyproject-demo/demo/__init__.py
+-rw-r--r--   0        0        0      275 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/git/github.com/demo/pyproject-demo/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/git/github.com/demo/subdirectories/one/one/__init__.py
+-rw-r--r--   0        0        0      244 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/git/github.com/demo/subdirectories/one/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/git/github.com/demo/subdirectories/one-copy/one/__init__.py
+-rw-r--r--   0        0        0      244 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/git/github.com/demo/subdirectories/one-copy/pyproject.toml
+-rw-r--r--   0        0        0      252 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/git/github.com/demo/subdirectories/two/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/git/github.com/demo/subdirectories/two/two/__init__.py
+-rw-r--r--   0        0        0       34 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/incompatible_lock/poetry.lock
+-rw-r--r--   0        0        0      320 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/incompatible_lock/pyproject.toml
+-rw-r--r--   0        0        0      378 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/inspection/demo/pyproject.toml
+-rw-r--r--   0        0        0      225 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/inspection/demo_no_setup_pkg_info_no_deps/PKG-INFO
+-rw-r--r--   0        0        0      461 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/inspection/demo_no_setup_pkg_info_no_deps/pyproject.toml
+-rw-r--r--   0        0        0      225 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/inspection/demo_only_requires_txt.egg-info/PKG-INFO
+-rw-r--r--   0        0        0       64 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/inspection/demo_only_requires_txt.egg-info/requires.txt
+-rw-r--r--   0        0        0      300 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/inspection/demo_poetry_package/pyproject.toml
+-rw-r--r--   0        0        0      225 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/inspection/demo_with_obsolete_egg_info/demo-0.1.0.egg-info/PKG-INFO
+-rw-r--r--   0        0        0       64 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/inspection/demo_with_obsolete_egg_info/demo-0.1.0.egg-info/requires.txt
+-rw-r--r--   0        0        0      378 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/inspection/demo_with_obsolete_egg_info/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/invalid_lock/poetry.lock
+-rw-r--r--   0        0        0      320 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/invalid_lock/pyproject.toml
+-rw-r--r--   0        0        0      408 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/invalid_pyproject/pyproject.toml
+-rw-r--r--   0        0        0      406 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/missing_directory_dependency/poetry.lock
+-rw-r--r--   0        0        0      299 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/missing_directory_dependency/pyproject.toml
+-rw-r--r--   0        0        0      428 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/missing_file_dependency/poetry.lock
+-rw-r--r--   0        0        0      324 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/missing_file_dependency/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/no_name_project/README.rst
+-rw-r--r--   0        0        0      306 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/no_name_project/pyproject.toml
+-rw-r--r--   0        0        0      762 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/old_lock/poetry.lock
+-rw-r--r--   0        0        0      320 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/old_lock/pyproject.toml
+-rw-r--r--   0        0        0      430 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/old_lock_path_dependency/poetry.lock
+-rw-r--r--   0        0        0      336 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/old_lock_path_dependency/pyproject.toml
+-rw-r--r--   0        0        0      247 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/old_lock_path_dependency/quix/pyproject.toml
+-rw-r--r--   0        0        0     6512 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/outdated_lock/poetry.lock
+-rw-r--r--   0        0        0      311 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/outdated_lock/pyproject.toml
+-rw-r--r--   0        0        0      309 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/private_pyproject/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/project_with_extras/project_with_extras/__init__.py
+-rw-r--r--   0        0        0      402 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/project_with_extras/pyproject.toml
+-rw-r--r--   0        0        0      881 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/project_with_git_dev_dependency/pyproject.toml
+-rw-r--r--   0        0        0      893 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/project_with_local_dependencies/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/project_with_multi_constraints_dependency/project/__init__.py
+-rw-r--r--   0        0        0      394 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/project_with_multi_constraints_dependency/pyproject.toml
+-rw-r--r--   0        0        0      264 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/project_with_nested_local/bar/pyproject.toml
+-rw-r--r--   0        0        0      262 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/project_with_nested_local/foo/pyproject.toml
+-rw-r--r--   0        0        0      324 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/project_with_nested_local/pyproject.toml
+-rw-r--r--   0        0        0      221 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/project_with_nested_local/quix/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/project_with_setup/my_package/__init__.py
+-rw-r--r--   0        0        0      239 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      201 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       38 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/requires.txt
+-rw-r--r--   0        0        0       11 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/top_level.txt
+-rw-r--r--   0        0        0      416 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/project_with_setup/setup.py
+-rw-r--r--   0        0        0       22 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/sample_project/README.rst
+-rw-r--r--   0        0        0     1501 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/sample_project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/scripts/README.md
+-rw-r--r--   0        0        0      400 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/scripts/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/scripts/scripts/__init__.py
+-rw-r--r--   0        0        0      557 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/scripts/scripts/check_argv0.py
+-rw-r--r--   0        0        0      122 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/scripts/scripts/exit_code.py
+-rw-r--r--   0        0        0      128 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/scripts/scripts/return_code.py
+-rw-r--r--   0        0        0       22 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/simple_project/README.rst
+-rw-r--r--   0        0        0     1320 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1106 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/simple_project/dist/simple_project-1.2.3.tar.gz
+-rw-r--r--   0        0        0      775 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/simple_project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/simple_project/simple_project/__init__.py
+-rw-r--r--   0        0        0     6404 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/up_to_date_lock/poetry.lock
+-rw-r--r--   0        0        0      313 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/up_to_date_lock/pyproject.toml
+-rw-r--r--   0        0        0     1722 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/wheel_with_no_requires_dist/demo-0.1.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1062 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/with-include/LICENSE
+-rw-r--r--   0        0        0       22 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/with-include/README.rst
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/with-include/extra_dir/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/with-include/extra_dir/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/with-include/extra_dir/sub_pkg/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/with-include/extra_dir/sub_pkg/vcs_excluded.txt
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/with-include/extra_dir/vcs_excluded.txt
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/with-include/for_wheel_only/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/with-include/my_module.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/with-include/notes.txt
+-rw-r--r--   0        0        0       59 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/with-include/package_with_include/__init__.py
+-rw-r--r--   0        0        0     1259 2023-05-29 16:05:02.512013 poetry-1.5.1/tests/fixtures/with-include/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with-include/src/src_package/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with-include/tests/__init__.py
+-rw-r--r--   0        0        0      153 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_conditional_path_deps/demo_one/pyproject.toml
+-rw-r--r--   0        0        0      153 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_conditional_path_deps/demo_two/pyproject.toml
+-rw-r--r--   0        0        0      257 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_conditional_path_deps/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_default_source/README.rst
+-rw-r--r--   0        0        0     1428 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_default_source/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_default_source_and_pypi/README.rst
+-rw-r--r--   0        0        0     1467 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_default_source_and_pypi/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_default_source_legacy/README.rst
+-rw-r--r--   0        0        0     1426 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_default_source_legacy/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_default_source_pypi/README.rst
+-rw-r--r--   0        0        0     1393 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_default_source_pypi/pyproject.toml
+-rw-r--r--   0        0        0      370 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_explicit_pypi_and_other/pyproject.toml
+-rw-r--r--   0        0        0      402 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_explicit_pypi_and_other_explicit/pyproject.toml
+-rw-r--r--   0        0        0      301 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_explicit_pypi_no_other/pyproject.toml
+-rw-r--r--   0        0        0      352 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_explicit_source/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_local_config/README.rst
+-rw-r--r--   0        0        0       48 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_local_config/poetry.toml
+-rw-r--r--   0        0        0     1331 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_local_config/pyproject.toml
+-rw-r--r--   0        0        0       28 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_multiple_readme_files/README-1.rst
+-rw-r--r--   0        0        0       20 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_multiple_readme_files/README-2.rst
+-rw-r--r--   0        0        0       79 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_multiple_readme_files/my_package/__init__.py
+-rw-r--r--   0        0        0      286 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_multiple_readme_files/pyproject.toml
+-rw-r--r--   0        0        0      425 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_non_default_multiple_secondary_sources/pyproject.toml
+-rw-r--r--   0        0        0      413 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_non_default_multiple_secondary_sources_legacy/pyproject.toml
+-rw-r--r--   0        0        0      402 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_non_default_multiple_sources/pyproject.toml
+-rw-r--r--   0        0        0      396 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_non_default_multiple_sources_legacy/pyproject.toml
+-rw-r--r--   0        0        0      509 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_non_default_multiple_sources_pypi/pyproject.toml
+-rw-r--r--   0        0        0      333 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_non_default_secondary_source/pyproject.toml
+-rw-r--r--   0        0        0      327 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_non_default_secondary_source_legacy/pyproject.toml
+-rw-r--r--   0        0        0      331 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_non_default_source_explicit/pyproject.toml
+-rw-r--r--   0        0        0      310 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_non_default_source_implicit/pyproject.toml
+-rw-r--r--   0        0        0      214 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_path_dependency/bazz/setup.py
+-rw-r--r--   0        0        0     3370 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_path_dependency/poetry.lock
+-rw-r--r--   0        0        0      305 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_path_dependency/pyproject.toml
+-rw-r--r--   0        0        0      364 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_supplemental_source/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_two_default_sources/README.rst
+-rw-r--r--   0        0        0     1518 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_two_default_sources/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_two_default_sources_legacy/README.rst
+-rw-r--r--   0        0        0     1520 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/fixtures/with_two_default_sources_legacy/pyproject.toml
+-rw-r--r--   0        0        0     8794 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/helpers.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/inspection/__init__.py
+-rw-r--r--   0        0        0     7707 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/inspection/test_info.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/__init__.py
+-rw-r--r--   0        0        0      564 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/extras-with-dependencies.test
+-rw-r--r--   0        0        0      530 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/extras.test
+-rw-r--r--   0        0        0      402 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/install-no-dev.test
+-rw-r--r--   0        0        0       95 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/no-dependencies.test
+-rw-r--r--   0        0        0     4081 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/old-lock.test
+-rw-r--r--   0        0        0      188 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/remove.test
+-rw-r--r--   0        0        0      188 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/update-with-lock.test
+-rw-r--r--   0        0        0      698 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/update-with-locked-extras.test
+-rw-r--r--   0        0        0      410 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/with-conditional-dependency.test
+-rw-r--r--   0        0        0      509 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/with-dependencies-extras.test
+-rw-r--r--   0        0        0      631 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/with-dependencies-nested-extras.test
+-rw-r--r--   0        0        0      295 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/with-dependencies.test
+-rw-r--r--   0        0        0     2168 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/with-directory-dependency-poetry-transitive.test
+-rw-r--r--   0        0        0      598 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/with-directory-dependency-poetry.test
+-rw-r--r--   0        0        0      641 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/with-directory-dependency-setuptools.test
+-rw-r--r--   0        0        0      471 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/with-duplicate-dependencies-update.test
+-rw-r--r--   0        0        0      841 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/with-duplicate-dependencies.test
+-rw-r--r--   0        0        0     1379 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/with-file-dependency-transitive.test
+-rw-r--r--   0        0        0      676 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/with-file-dependency.test
+-rw-r--r--   0        0        0      752 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/with-multiple-updates.test
+-rw-r--r--   0        0        0      469 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/with-optional-dependencies.test
+-rw-r--r--   0        0        0      565 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/with-platform-dependencies.test
+-rw-r--r--   0        0        0      297 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/with-prereleases.test
+-rw-r--r--   0        0        0     5109 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/with-pypi-repository.test
+-rw-r--r--   0        0        0      424 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/with-python-versions.test
+-rw-r--r--   0        0        0     1146 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/with-same-version-url-dependencies.test
+-rw-r--r--   0        0        0      579 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/with-sub-dependencies.test
+-rw-r--r--   0        0        0      686 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/with-url-dependency.test
+-rw-r--r--   0        0        0      708 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/with-vcs-dependency-with-extras.test
+-rw-r--r--   0        0        0      491 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/with-vcs-dependency-without-ref.test
+-rw-r--r--   0        0        0      478 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/fixtures/with-wheel-dependency-no-requires-dist.test
+-rw-r--r--   0        0        0     3266 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/test_chef.py
+-rw-r--r--   0        0        0    11122 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/test_chooser.py
+-rw-r--r--   0        0        0    42722 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/test_executor.py
+-rw-r--r--   0        0        0    81903 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/test_installer.py
+-rw-r--r--   0        0        0     2706 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/installation/test_wheel_installer.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/integration/__init__.py
+-rw-r--r--   0        0        0    12051 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/integration/test_utils_vcs_git.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.516013 poetry-1.5.1/tests/json/__init__.py
+-rw-r--r--   0        0        0      338 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/json/fixtures/source/complete_invalid_priority.toml
+-rw-r--r--   0        0        0      352 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/json/fixtures/source/complete_invalid_priority_legacy_and_new.toml
+-rw-r--r--   0        0        0      282 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/json/fixtures/source/complete_invalid_url.toml
+-rw-r--r--   0        0        0      337 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/json/fixtures/source/complete_valid.toml
+-rw-r--r--   0        0        0      349 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/json/fixtures/source/complete_valid_legacy.toml
+-rw-r--r--   0        0        0     1761 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/json/test_schema_sources.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/masonry/builders/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/masonry/builders/fixtures/excluded_subpackage/README.rst
+-rw-r--r--   0        0        0       59 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/masonry/builders/fixtures/excluded_subpackage/example/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/masonry/builders/fixtures/excluded_subpackage/example/test/__init__.py
+-rw-r--r--   0        0        0      176 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/masonry/builders/fixtures/excluded_subpackage/example/test/excluded.py
+-rw-r--r--   0        0        0      329 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/masonry/builders/fixtures/excluded_subpackage/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/masonry/builders/fixtures/pep_561_stub_only/pkg-stubs/__init__.pyi
+-rw-r--r--   0        0        0       83 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/masonry/builders/fixtures/pep_561_stub_only/pkg-stubs/module.pyi
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/masonry/builders/fixtures/pep_561_stub_only/pkg-stubs/subpkg/__init__.pyi
+-rw-r--r--   0        0        0      261 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/masonry/builders/fixtures/pep_561_stub_only/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/__init__.pyi
+-rw-r--r--   0        0        0       83 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/module.pyi
+-rw-r--r--   0        0        0        8 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/py.typed
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/subpkg/__init__.pyi
+-rw-r--r--   0        0        0      291 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pyproject.toml
+-rw-r--r--   0        0        0      294 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/masonry/builders/fixtures/pep_561_stub_only_src/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/masonry/builders/fixtures/pep_561_stub_only_src/src/pkg-stubs/__init__.pyi
+-rw-r--r--   0        0        0       83 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/masonry/builders/fixtures/pep_561_stub_only_src/src/pkg-stubs/module.pyi
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/masonry/builders/fixtures/pep_561_stub_only_src/src/pkg-stubs/subpkg/__init__.pyi
+-rw-r--r--   0        0        0    10586 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/masonry/builders/test_editable_builder.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/mixology/__init__.py
+-rw-r--r--   0        0        0     2188 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/mixology/helpers.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/mixology/solutions/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/mixology/solutions/providers/__init__.py
+-rw-r--r--   0        0        0     1449 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/mixology/solutions/providers/test_python_requirement_solution_provider.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/mixology/solutions/solutions/__init__.py
+-rw-r--r--   0        0        0     1470 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/mixology/solutions/solutions/test_python_requirement_solution.py
+-rw-r--r--   0        0        0      109 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/mixology/version_solver/__init__.py
+-rw-r--r--   0        0        0     1066 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/mixology/version_solver/conftest.py
+-rw-r--r--   0        0        0     6890 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/mixology/version_solver/test_backtracking.py
+-rw-r--r--   0        0        0     4326 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/mixology/version_solver/test_basic_graph.py
+-rw-r--r--   0        0        0     7554 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/mixology/version_solver/test_dependency_cache.py
+-rw-r--r--   0        0        0     1153 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/mixology/version_solver/test_python_constraint.py
+-rw-r--r--   0        0        0     5226 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/mixology/version_solver/test_unsolvable.py
+-rw-r--r--   0        0        0     7700 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/mixology/version_solver/test_with_lock.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/packages/__init__.py
+-rw-r--r--   0        0        0     1890 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/packages/test_direct_origin.py
+-rw-r--r--   0        0        0    30095 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/packages/test_locker.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/plugins/__init__.py
+-rw-r--r--   0        0        0     3198 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/plugins/test_plugin_manager.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/publishing/__init__.py
+-rw-r--r--   0        0        0     6438 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/publishing/test_publisher.py
+-rw-r--r--   0        0        0     4720 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/publishing/test_uploader.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/puzzle/__init__.py
+-rw-r--r--   0        0        0      528 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/puzzle/conftest.py
+-rw-r--r--   0        0        0    25026 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/puzzle/test_provider.py
+-rw-r--r--   0        0        0   128806 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/puzzle/test_solver.py
+-rw-r--r--   0        0        0     5634 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/puzzle/test_transaction.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/pyproject/__init__.py
+-rw-r--r--   0        0        0      813 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/pyproject/conftest.py
+-rw-r--r--   0        0        0     1379 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/pyproject/test_pyproject_toml.py
+-rw-r--r--   0        0        0      755 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/pyproject/test_pyproject_toml_file.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/repositories/__init__.py
+-rw-r--r--   0        0        0    16009 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/cleo-0.7.6.dist-info/METADATA
+-rw-r--r--   0        0        0      110 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/directory_pep_610-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0       81 2023-05-29 16:05:02.520013 poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/directory_pep_610-1.2.3.dist-info/direct_url.json
+-rw-r--r--   0        0        0      719 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-2.3.4.dist-info/METADATA
+-rw-r--r--   0        0        0      731 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-with-import-2.3.4.dist-info/METADATA
+-rw-r--r--   0        0        0       10 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-with-import.pth
+-rw-r--r--   0        0        0       18 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable.pth
+-rw-r--r--   0        0        0      119 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable_directory_pep_610-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0      105 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable_directory_pep_610-1.2.3.dist-info/direct_url.json
+-rw-r--r--   0        0        0      105 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/file_pep_610-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0      182 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/file_pep_610-1.2.3.dist-info/direct_url.json
+-rw-r--r--   0        0        0     1306 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/foo-0.1.0-py3.8.egg
+-rw-r--r--   0        0        0      104 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0      159 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610-1.2.3.dist-info/direct_url.json
+-rw-r--r--   0        0        0      125 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610_no_requested_version-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0      141 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610_no_requested_version-1.2.3.dist-info/direct_url.json
+-rw-r--r--   0        0        0      117 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610_subdirectory-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0      200 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/git_pep_610_subdirectory-1.2.3.dist-info/direct_url.json
+-rw-r--r--   0        0        0      719 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/standard-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0        9 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/standard.pth
+-rw-r--r--   0        0        0      104 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/url_pep_610-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0      102 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/url_pep_610-1.2.3.dist-info/direct_url.json
+-rw-r--r--   0        0        0      717 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/bender-2.0.5.dist-info/METADATA
+-rw-r--r--   0        0        0       20 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/bender.pth
+-rw-r--r--   0        0        0      710 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/lib64-2.3.4.dist-info/METADATA
+-rw-r--r--   0        0        0      717 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/src/bender/bender.egg-info/PKG-INFO
+-rw-r--r--   0        0        0     8866 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/src/pendulum/pendulum.egg-info/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/src/pendulum/pendulum.egg-info/requires.txt
+-rw-r--r--   0        0        0     9020 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/installed/vendor/py3.7/attrs-19.3.0.dist-info/METADATA
+-rw-r--r--   0        0        0      731 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/legacy/absolute.html
+-rw-r--r--   0        0        0      790 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/legacy/black.html
+-rw-r--r--   0        0        0     1455 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/legacy/clikit.html
+-rw-r--r--   0        0        0      746 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/legacy/discord-py.html
+-rw-r--r--   0        0        0      759 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/legacy/futures-partial-yank.html
+-rw-r--r--   0        0        0      747 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/legacy/futures.html
+-rw-r--r--   0        0        0      625 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/legacy/invalid-version.html
+-rw-r--r--   0        0        0     1433 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/legacy/ipython.html
+-rw-r--r--   0        0        0      917 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/legacy/isort.html
+-rw-r--r--   0        0        0      333 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/legacy/jupyter.html
+-rw-r--r--   0        0        0      348 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/legacy/missing-version.html
+-rw-r--r--   0        0        0      401 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/legacy/pastel.html
+-rw-r--r--   0        0        0      534 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/legacy/poetry-test-py2-py3-metadata-merge.html
+-rw-r--r--   0        0        0      802 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/legacy/pytest.html
+-rw-r--r--   0        0        0      467 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/legacy/python-language-server.html
+-rw-r--r--   0        0        0      941 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/legacy/pyyaml.html
+-rw-r--r--   0        0        0      687 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/legacy/relative.html
+-rw-r--r--   0        0        0      473 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/legacy/tomlkit.html
+-rw-r--r--   0        0        0    18499 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/SQLAlchemy-1.2.12.tar.gz
+-rw-r--r--   0        0        0     9634 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/Twisted-18.9.0.tar.bz2
+-rw-r--r--   0        0        0     1940 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/black-19.10b0-py36-none-any.whl
+-rw-r--r--   0        0        0    14949 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/black-21.11b0-py3-none-any.whl
+-rw-r--r--   0        0        0    78701 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/cleo-1.0.0a5-py3-none-any.whl
+-rw-r--r--   0        0        0     2329 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/clikit-0.2.4-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     2290 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/discord.py-2.0.0-py3-none-any.whl
+-rw-r--r--   0        0        0    15847 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0-py2-none-any.whl
+-rw-r--r--   0        0        0    18359 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0.tar.gz
+-rw-r--r--   0        0        0    31809 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/importlib_metadata-1.7.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    23473 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py2-none-any.whl
+-rw-r--r--   0        0        0    23475 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py3-none-any.whl
+-rw-r--r--   0        0        0    15795 2023-05-29 16:05:02.524014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0.tar.gz
+-rw-r--r--   0        0        0    22352 2023-05-29 16:05:02.528014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/ipython-7.5.0-py3-none-any.whl
+-rw-r--r--   0        0        0    45393 2023-05-29 16:05:02.528014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py2-none-any.whl
+-rw-r--r--   0        0        0    45352 2023-05-29 16:05:02.528014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py3-none-any.whl
+-rw-r--r--   0        0        0    56070 2023-05-29 16:05:02.528014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4.tar.gz
+-rw-r--r--   0        0        0     2736 2023-05-29 16:05:02.528014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    12916 2023-05-29 16:05:02.528014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0.tar.gz
+-rw-r--r--   0        0        0     4490 2023-05-29 16:05:02.528014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/pastel-0.1.0.tar.gz
+-rw-r--r--   0        0        0   464992 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/poetry_core-1.5.0-py3-none-any.whl
+-rw-r--r--   0        0        0     1213 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py2-none-any.whl
+-rw-r--r--   0        0        0     1218 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0     3691 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/pytest-3.5.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     3708 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/pytest-3.5.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    54076 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/python-language-server-0.21.2.tar.gz
+-rw-r--r--   0        0        0    29813 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.2.tar.gz
+-rw-r--r--   0        0        0    29864 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.3.tar.gz
+-rw-r--r--   0        0        0     5700 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/zipp-3.5.0-py3-none-any.whl
+-rw-r--r--   0        0        0     3421 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/attrs/17.4.0.json
+-rw-r--r--   0        0        0      856 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/attrs.json
+-rw-r--r--   0        0        0    62683 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/black/19.10b0.json
+-rw-r--r--   0        0        0     5924 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/black/21.11b0.json
+-rw-r--r--   0        0        0     1709 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/black.json
+-rw-r--r--   0        0        0     2298 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/cachecontrol/0.12.5.json
+-rw-r--r--   0        0        0     2425 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/cachecontrol.json
+-rw-r--r--   0        0        0     3035 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/cleo/1.0.0a5.json
+-rw-r--r--   0        0        0     3745 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/clikit/0.2.4.json
+-rw-r--r--   0        0        0      997 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/clikit.json
+-rw-r--r--   0        0        0     2922 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/colorama/0.3.9.json
+-rw-r--r--   0        0        0      867 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/colorama.json
+-rw-r--r--   0        0        0     4035 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/discord-py/2.0.0.json
+-rw-r--r--   0        0        0     2944 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/funcsigs/1.0.2.json
+-rw-r--r--   0        0        0      867 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/funcsigs.json
+-rw-r--r--   0        0        0     3838 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/hbmqtt/0.9.6.json
+-rw-r--r--   0        0        0    14437 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/hbmqtt.json
+-rw-r--r--   0        0        0     5331 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/importlib-metadata/1.7.0.json
+-rw-r--r--   0        0        0     1065 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/importlib-metadata.json
+-rw-r--r--   0        0        0     5984 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/ipython/4.1.0rc1.json
+-rw-r--r--   0        0        0    21476 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/isort/4.3.4.json
+-rw-r--r--   0        0        0     1221 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/isort.json
+-rw-r--r--   0        0        0     3969 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/jupyter/1.0.0.json
+-rw-r--r--   0        0        0     1217 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/jupyter.json
+-rw-r--r--   0        0        0     2931 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/lockfile/0.12.2.json
+-rw-r--r--   0        0        0      871 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/lockfile.json
+-rw-r--r--   0        0        0     3552 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/more-itertools/4.1.0.json
+-rw-r--r--   0        0        0     1284 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/more-itertools.json
+-rw-r--r--   0        0        0     2328 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/pluggy/0.6.0.json
+-rw-r--r--   0        0        0      470 2023-05-29 16:05:02.532014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/pluggy.json
+-rw-r--r--   0        0        0     3180 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/poetry/0.12.4.json
+-rw-r--r--   0        0        0     3555 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/poetry-core/1.5.0.json
+-rw-r--r--   0        0        0      897 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/poetry-core.json
+-rw-r--r--   0        0        0     4561 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/poetry.json
+-rw-r--r--   0        0        0     3095 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/py/1.5.3.json
+-rw-r--r--   0        0        0      837 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/py.json
+-rw-r--r--   0        0        0      931 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/pygame-music-grid.json
+-rw-r--r--   0        0        0     4469 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/pylev/1.3.0.json
+-rw-r--r--   0        0        0      495 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/pylev.json
+-rw-r--r--   0        0        0     6933 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/pytest/3.5.0.json
+-rw-r--r--   0        0        0     7555 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/pytest/3.5.1.json
+-rw-r--r--   0        0        0      857 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/pytest.json
+-rw-r--r--   0        0        0    14143 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/pyyaml/3.13.0.json
+-rw-r--r--   0        0        0     7805 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/pyyaml.json
+-rw-r--r--   0        0        0     3142 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/requests/2.18.4.json
+-rw-r--r--   0        0        0    67409 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/requests.json
+-rw-r--r--   0        0        0     5315 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/setuptools/39.2.0.json
+-rw-r--r--   0        0        0     8423 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/setuptools/67.6.1.json
+-rw-r--r--   0        0        0     1843 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/setuptools.json
+-rw-r--r--   0        0        0     2387 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/six/1.11.0.json
+-rw-r--r--   0        0        0      846 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/six.json
+-rw-r--r--   0        0        0     8870 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/sqlalchemy/1.2.12.json
+-rw-r--r--   0        0        0      484 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/sqlalchemy.json
+-rw-r--r--   0        0        0     6109 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/toga.json
+-rw-r--r--   0        0        0    11126 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/tomlkit/0.5.3.json
+-rw-r--r--   0        0        0     1892 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/tomlkit.json
+-rw-r--r--   0        0        0     3184 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/trackpy/0.4.1.json
+-rw-r--r--   0        0        0      838 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/trackpy.json
+-rw-r--r--   0        0        0    11606 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/twisted/18.9.0.json
+-rw-r--r--   0        0        0      477 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/twisted.json
+-rw-r--r--   0        0        0     4483 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/wheel/0.40.0.json
+-rw-r--r--   0        0        0     1041 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/wheel.json
+-rw-r--r--   0        0        0     5188 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/zipp/3.5.0.json
+-rw-r--r--   0        0        0      907 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/zipp.json
+-rw-r--r--   0        0        0   224197 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/pypi.org/search/search.html
+-rw-r--r--   0        0        0     3407 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/fixtures/single-page/jax_releases.html
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/link_sources/__init__.py
+-rw-r--r--   0        0        0     3108 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/link_sources/test_base.py
+-rw-r--r--   0        0        0     2999 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/link_sources/test_html.py
+-rw-r--r--   0        0        0    10933 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/test_installed_repository.py
+-rw-r--r--   0        0        0    17437 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/test_legacy_repository.py
+-rw-r--r--   0        0        0     1788 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/test_lockfile_repository.py
+-rw-r--r--   0        0        0    11500 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/test_pypi_repository.py
+-rw-r--r--   0        0        0     2321 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/test_repository.py
+-rw-r--r--   0        0        0    12604 2023-05-29 16:05:02.536014 poetry-1.5.1/tests/repositories/test_repository_pool.py
+-rw-r--r--   0        0        0     1998 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/repositories/test_single_page_repository.py
+-rw-r--r--   0        0        0    20928 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/test_factory.py
+-rw-r--r--   0        0        0      399 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/test_helpers.py
+-rw-r--r--   0        0        0     1665 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/types.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/__init__.py
+-rw-r--r--   0        0        0      384 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/conftest.py
+-rw-r--r--   0        0        0      604 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/fixtures/pyproject.toml
+-rw-r--r--   0        0        0      371 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/fixtures/setups/ansible/requirements.txt
+-rw-r--r--   0        0        0    10765 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/fixtures/setups/ansible/setup.py
+-rw-r--r--   0        0        0      271 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/fixtures/setups/extras_require_with_vars/setup.py
+-rw-r--r--   0        0        0     2581 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/fixtures/setups/flask/setup.py
+-rw-r--r--   0        0        0     1353 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/fixtures/setups/pendulum/setup.py
+-rw-r--r--   0        0        0    11825 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/fixtures/setups/pyyaml/setup.py
+-rw-r--r--   0        0        0     3366 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/fixtures/setups/requests/setup.py
+-rw-r--r--   0        0        0      290 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/fixtures/setups/setuptools_setup/setup.py
+-rw-r--r--   0        0        0     6272 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/fixtures/setups/sqlalchemy/setup.py
+-rw-r--r--   0        0        0      302 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/fixtures/setups/with-setup-cfg/setup.cfg
+-rw-r--r--   0        0        0       75 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/fixtures/setups/with-setup-cfg/setup.py
+-rw-r--r--   0        0        0      339 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/fixtures/setups/with-setup-cfg-attr/setup.cfg
+-rw-r--r--   0        0        0       75 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/fixtures/setups/with-setup-cfg-attr/setup.py
+-rw-r--r--   0        0        0    20408 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/test_authenticator.py
+-rw-r--r--   0        0        0    12266 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/test_cache.py
+-rw-r--r--   0        0        0     5922 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/test_dependency_specification.py
+-rw-r--r--   0        0        0    56459 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/test_env.py
+-rw-r--r--   0        0        0     1562 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/test_env_site.py
+-rw-r--r--   0        0        0     2374 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/test_extras.py
+-rw-r--r--   0        0        0     4953 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/test_helpers.py
+-rw-r--r--   0        0        0     8460 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/test_password_manager.py
+-rw-r--r--   0        0        0     1114 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/test_patterns.py
+-rw-r--r--   0        0        0     1092 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/test_pip.py
+-rw-r--r--   0        0        0     6756 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/test_setup_reader.py
+-rw-r--r--   0        0        0     2182 2023-05-29 16:05:02.540015 poetry-1.5.1/tests/utils/test_source.py
+-rw-r--r--   0        0        0     6968 1970-01-01 00:00:00.000000 poetry-1.5.1/PKG-INFO
```

### Comparing `poetry-1.5.0/LICENSE` & `poetry-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/README.md` & `poetry-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/pyproject.toml` & `poetry-1.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry"
-version = "1.5.0"
+version = "1.5.1"
 description = "Python dependency management and packaging made easy."
 authors = ["Sébastien Eustace <sebastien@eustace.io>"]
 maintainers = [
     "Arun Babu Neelicattu <arun.neelicattu@gmail.com>",
     "Bjorn Neergaard <bjorn@neersighted.com>",
     "Branch Vincent <branchevincent@gmail.com>",
     "Randy Döring <radoering.poetry@gmail.com>",
@@ -28,16 +28,16 @@
 [tool.poetry.urls]
 Changelog = "https://python-poetry.org/history/"
 
 # Requirements
 [tool.poetry.dependencies]
 python = "^3.7"
 
-poetry-core = "1.6.0"
-poetry-plugin-export = "^1.3.1"
+poetry-core = "1.6.1"
+poetry-plugin-export = "^1.4.0"
 "backports.cached-property" = { version = "^1.0.2", python = "<3.8" }
 build = "^0.10.0"
 cachecontrol = { version = "^0.12.9", extras = ["filecache"] }
 cleo = "^2.0.0"
 crashtest = "^0.4.1"
 dulwich = "^0.21.2"
 filelock = "^3.8.0"
```

### Comparing `poetry-1.5.0/src/poetry/config/config.py` & `poetry-1.5.1/src/poetry/config/config.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/config/dict_config_source.py` & `poetry-1.5.1/src/poetry/config/dict_config_source.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/config/file_config_source.py` & `poetry-1.5.1/src/poetry/config/file_config_source.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/config/source.py` & `poetry-1.5.1/src/poetry/config/source.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/application.py` & `poetry-1.5.1/src/poetry/console/application.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/command_loader.py` & `poetry-1.5.1/src/poetry/console/command_loader.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/about.py` & `poetry-1.5.1/src/poetry/console/commands/about.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/add.py` & `poetry-1.5.1/src/poetry/console/commands/add.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/build.py` & `poetry-1.5.1/src/poetry/console/commands/build.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/cache/clear.py` & `poetry-1.5.1/src/poetry/console/commands/cache/clear.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/cache/list.py` & `poetry-1.5.1/src/poetry/console/commands/cache/list.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/check.py` & `poetry-1.5.1/src/poetry/console/commands/check.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/command.py` & `poetry-1.5.1/src/poetry/console/commands/command.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/config.py` & `poetry-1.5.1/src/poetry/console/commands/config.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/debug/info.py` & `poetry-1.5.1/src/poetry/console/commands/debug/info.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/debug/resolve.py` & `poetry-1.5.1/src/poetry/console/commands/debug/resolve.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/env/info.py` & `poetry-1.5.1/src/poetry/console/commands/env/info.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/env/list.py` & `poetry-1.5.1/src/poetry/console/commands/env/list.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/env/remove.py` & `poetry-1.5.1/src/poetry/console/commands/env/remove.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/env/use.py` & `poetry-1.5.1/src/poetry/console/commands/env/use.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/env_command.py` & `poetry-1.5.1/src/poetry/console/commands/env_command.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/group_command.py` & `poetry-1.5.1/src/poetry/console/commands/group_command.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/init.py` & `poetry-1.5.1/src/poetry/console/commands/init.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/install.py` & `poetry-1.5.1/src/poetry/console/commands/install.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/installer_command.py` & `poetry-1.5.1/src/poetry/console/commands/installer_command.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/lock.py` & `poetry-1.5.1/src/poetry/console/commands/lock.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/new.py` & `poetry-1.5.1/src/poetry/console/commands/new.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/publish.py` & `poetry-1.5.1/src/poetry/console/commands/publish.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/remove.py` & `poetry-1.5.1/src/poetry/console/commands/remove.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/run.py` & `poetry-1.5.1/src/poetry/console/commands/run.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/search.py` & `poetry-1.5.1/src/poetry/console/commands/search.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/self/add.py` & `poetry-1.5.1/src/poetry/console/commands/self/add.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/self/install.py` & `poetry-1.5.1/src/poetry/console/commands/self/install.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/self/lock.py` & `poetry-1.5.1/src/poetry/console/commands/self/lock.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/self/remove.py` & `poetry-1.5.1/src/poetry/console/commands/self/remove.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/self/self_command.py` & `poetry-1.5.1/src/poetry/console/commands/self/self_command.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/self/show/__init__.py` & `poetry-1.5.1/src/poetry/console/commands/self/show/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/self/show/plugins.py` & `poetry-1.5.1/src/poetry/console/commands/self/show/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/self/update.py` & `poetry-1.5.1/src/poetry/console/commands/self/update.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/shell.py` & `poetry-1.5.1/src/poetry/console/commands/shell.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/show.py` & `poetry-1.5.1/src/poetry/console/commands/show.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/source/add.py` & `poetry-1.5.1/src/poetry/console/commands/source/add.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/source/remove.py` & `poetry-1.5.1/src/poetry/console/commands/source/remove.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/source/show.py` & `poetry-1.5.1/src/poetry/console/commands/source/show.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/update.py` & `poetry-1.5.1/src/poetry/console/commands/update.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/commands/version.py` & `poetry-1.5.1/src/poetry/console/commands/version.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/io/inputs/run_argv_input.py` & `poetry-1.5.1/src/poetry/console/io/inputs/run_argv_input.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/logging/formatters/builder_formatter.py` & `poetry-1.5.1/src/poetry/console/logging/formatters/builder_formatter.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/logging/io_formatter.py` & `poetry-1.5.1/src/poetry/console/logging/io_formatter.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/console/logging/io_handler.py` & `poetry-1.5.1/src/poetry/console/logging/io_handler.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/factory.py` & `poetry-1.5.1/src/poetry/factory.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/inspection/info.py` & `poetry-1.5.1/src/poetry/inspection/info.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/installation/chef.py` & `poetry-1.5.1/src/poetry/installation/chef.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/installation/chooser.py` & `poetry-1.5.1/src/poetry/installation/chooser.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/installation/executor.py` & `poetry-1.5.1/src/poetry/installation/executor.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/installation/installer.py` & `poetry-1.5.1/src/poetry/installation/installer.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/installation/operations/install.py` & `poetry-1.5.1/src/poetry/installation/operations/install.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/installation/operations/operation.py` & `poetry-1.5.1/src/poetry/installation/operations/operation.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/installation/operations/uninstall.py` & `poetry-1.5.1/src/poetry/installation/operations/uninstall.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/installation/operations/update.py` & `poetry-1.5.1/src/poetry/installation/operations/update.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/installation/wheel_installer.py` & `poetry-1.5.1/src/poetry/installation/wheel_installer.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,15 +97,18 @@
 
     def enable_bytecode_compilation(self, enable: bool = True) -> None:
         self._destination.bytecode_optimization_levels = (-1,) if enable else ()
 
     def install(self, wheel: Path) -> None:
         with WheelFile.open(wheel) as source:
             try:
-                source.validate_record()
+                # Content validation is temporarily disabled because of
+                # pypa/installer's out of memory issues with big wheels. See
+                # https://github.com/python-poetry/poetry/issues/7983
+                source.validate_record(validate_contents=False)
             except _WheelFileValidationError as e:
                 self.invalid_wheels[wheel] = e.issues
             install(
                 source=source,
                 destination=self._destination.for_source(source),
                 # Additional metadata that is generated by the installation tool.
                 additional_metadata={
```

### Comparing `poetry-1.5.0/src/poetry/json/__init__.py` & `poetry-1.5.1/src/poetry/json/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/json/schemas/poetry.json` & `poetry-1.5.1/src/poetry/json/schemas/poetry.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/layouts/layout.py` & `poetry-1.5.1/src/poetry/layouts/layout.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/locations.py` & `poetry-1.5.1/src/poetry/locations.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/masonry/builders/editable.py` & `poetry-1.5.1/src/poetry/masonry/builders/editable.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/mixology/assignment.py` & `poetry-1.5.1/src/poetry/mixology/assignment.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/mixology/failure.py` & `poetry-1.5.1/src/poetry/mixology/failure.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/mixology/incompatibility.py` & `poetry-1.5.1/src/poetry/mixology/incompatibility.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/mixology/incompatibility_cause.py` & `poetry-1.5.1/src/poetry/mixology/incompatibility_cause.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/mixology/partial_solution.py` & `poetry-1.5.1/src/poetry/mixology/partial_solution.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/mixology/result.py` & `poetry-1.5.1/src/poetry/mixology/result.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/mixology/solutions/providers/python_requirement_solution_provider.py` & `poetry-1.5.1/src/poetry/mixology/solutions/providers/python_requirement_solution_provider.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/mixology/solutions/solutions/python_requirement_solution.py` & `poetry-1.5.1/src/poetry/mixology/solutions/solutions/python_requirement_solution.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/mixology/term.py` & `poetry-1.5.1/src/poetry/mixology/term.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/mixology/version_solver.py` & `poetry-1.5.1/src/poetry/mixology/version_solver.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from __future__ import annotations
 
+import collections
 import functools
 import time
 
 from typing import TYPE_CHECKING
+from typing import Optional
+from typing import Tuple
 
 from poetry.core.packages.dependency import Dependency
 
 from poetry.mixology.failure import SolveFailure
 from poetry.mixology.incompatibility import Incompatibility
 from poetry.mixology.incompatibility_cause import ConflictCause
 from poetry.mixology.incompatibility_cause import NoVersionsCause
@@ -24,55 +27,101 @@
     from poetry.packages import DependencyPackage
     from poetry.puzzle.provider import Provider
 
 
 _conflict = object()
 
 
+DependencyCacheKey = Tuple[
+    str, Optional[str], Optional[str], Optional[str], Optional[str]
+]
+
+
 class DependencyCache:
     """
     A cache of the valid dependencies.
 
     The key observation here is that during the search - except at backtracking
     - once we have decided that a dependency is invalid, we never need check it
     again.
     """
 
     def __init__(self, provider: Provider) -> None:
-        self.provider = provider
-        self.cache: dict[
-            tuple[str, str | None, str | None, str | None, str | None],
-            list[DependencyPackage],
-        ] = {}
+        self._provider = provider
+
+        # self._cache maps a package name to a stack of cached package lists,
+        # ordered by the decision level which added them to the cache. This is
+        # done so that when backtracking we can maintain cache entries from
+        # previous decision levels, while clearing cache entries from only the
+        # rolled back levels.
+        #
+        # In order to maintain the integrity of the cache, `clear_level()`
+        # needs to be called in descending order as decision levels are
+        # backtracked so that the correct items can be popped from the stack.
+        self._cache: dict[DependencyCacheKey, list[list[DependencyPackage]]] = (
+            collections.defaultdict(list)
+        )
+        self._cached_dependencies_by_level: dict[int, list[DependencyCacheKey]] = (
+            collections.defaultdict(list)
+        )
+
+        self._search_for_cached = functools.lru_cache(maxsize=128)(self._search_for)
+
+    def _search_for(
+        self,
+        dependency: Dependency,
+        key: DependencyCacheKey,
+    ) -> list[DependencyPackage]:
+        cache_entries = self._cache[key]
+        if cache_entries:
+            packages = [
+                p
+                for p in cache_entries[-1]
+                if dependency.constraint.allows(p.package.version)
+            ]
+        else:
+            packages = None
 
-        self.search_for = functools.lru_cache(maxsize=128)(self._search_for)
+        # provider.search_for() normally does not include pre-release packages
+        # (unless requested), but will include them if there are no other
+        # eligible package versions for a version constraint.
+        #
+        # Therefore, if the eligible versions have been filtered down to
+        # nothing, we need to call provider.search_for() again as it may return
+        # additional results this time.
+        if not packages:
+            packages = self._provider.search_for(dependency)
 
-    def _search_for(self, dependency: Dependency) -> list[DependencyPackage]:
+        return packages
+
+    def search_for(
+        self,
+        dependency: Dependency,
+        decision_level: int,
+    ) -> list[DependencyPackage]:
         key = (
             dependency.complete_name,
             dependency.source_type,
             dependency.source_url,
             dependency.source_reference,
             dependency.source_subdirectory,
         )
 
-        packages = self.cache.get(key)
-        if packages is None:
-            packages = self.provider.search_for(dependency)
-        else:
-            packages = [
-                p for p in packages if dependency.constraint.allows(p.package.version)
-            ]
-
-        self.cache[key] = packages
+        packages = self._search_for_cached(dependency, key)
+        if not self._cache[key] or self._cache[key][-1] is not packages:
+            self._cache[key].append(packages)
+            self._cached_dependencies_by_level[decision_level].append(key)
 
         return packages
 
-    def clear(self) -> None:
-        self.cache.clear()
+    def clear_level(self, level: int) -> None:
+        if level in self._cached_dependencies_by_level:
+            self._search_for_cached.cache_clear()
+            for key in self._cached_dependencies_by_level.pop(level):
+                self._cache[key].pop()
 
 
 class VersionSolver:
     """
     The version solver that finds a set of package versions that satisfy the
     root package's dependencies.
 
@@ -82,14 +131,17 @@
 
     def __init__(self, root: ProjectPackage, provider: Provider) -> None:
         self._root = root
         self._provider = provider
         self._dependency_cache = DependencyCache(provider)
         self._incompatibilities: dict[str, list[Incompatibility]] = {}
         self._contradicted_incompatibilities: set[Incompatibility] = set()
+        self._contradicted_incompatibilities_by_level: dict[
+            int, set[Incompatibility]
+        ] = collections.defaultdict(set)
         self._solution = PartialSolution()
 
     @property
     def solution(self) -> PartialSolution:
         return self._solution
 
     def solve(self) -> SolverResult:
@@ -180,14 +232,17 @@
             relation = self._solution.relation(term)
 
             if relation == SetRelation.DISJOINT:
                 # If term is already contradicted by _solution, then
                 # incompatibility is contradicted as well and there's nothing new we
                 # can deduce from it.
                 self._contradicted_incompatibilities.add(incompatibility)
+                self._contradicted_incompatibilities_by_level[
+                    self._solution.decision_level
+                ].add(incompatibility)
                 return None
             elif relation == SetRelation.OVERLAPPING:
                 # If more than one term is inconclusive, we can't deduce anything about
                 # incompatibility.
                 if unsatisfied is not None:
                     return None
 
@@ -198,14 +253,17 @@
 
         # If *all* terms in incompatibility are satisfied by _solution, then
         # incompatibility is satisfied and we have a conflict.
         if unsatisfied is None:
             return _conflict
 
         self._contradicted_incompatibilities.add(incompatibility)
+        self._contradicted_incompatibilities_by_level[
+            self._solution.decision_level
+        ].add(incompatibility)
 
         adverb = "not " if unsatisfied.is_positive() else ""
         self._log(f"derived: {adverb}{unsatisfied.dependency}")
 
         self._solution.derive(
             unsatisfied.dependency, not unsatisfied.is_positive(), incompatibility
         )
@@ -291,17 +349,24 @@
 
             # using assert to suppress mypy [union-attr]
             assert most_recent_satisfier is not None
             if (
                 previous_satisfier_level < most_recent_satisfier.decision_level
                 or most_recent_satisfier.cause is None
             ):
+                for level in range(
+                    self._solution.decision_level, previous_satisfier_level, -1
+                ):
+                    if level in self._contradicted_incompatibilities_by_level:
+                        self._contradicted_incompatibilities.difference_update(
+                            self._contradicted_incompatibilities_by_level.pop(level),
+                        )
+                    self._dependency_cache.clear_level(level)
+
                 self._solution.backtrack(previous_satisfier_level)
-                self._contradicted_incompatibilities.clear()
-                self._dependency_cache.clear()
                 if new_incompatibility:
                     self._add_incompatibility(incompatibility)
 
                 return incompatibility
 
             # Create a new incompatibility by combining incompatibility with the
             # incompatibility that caused most_recent_satisfier to be assigned. Doing
@@ -391,15 +456,19 @@
 
             use_latest = dependency.name in self._provider.use_latest
             if not use_latest:
                 locked = self._provider.get_locked(dependency)
                 if locked:
                     return is_specific_marker, Preference.LOCKED, 1
 
-            num_packages = len(self._dependency_cache.search_for(dependency))
+            num_packages = len(
+                self._dependency_cache.search_for(
+                    dependency, self._solution.decision_level
+                )
+            )
 
             if num_packages < 2:
                 preference = Preference.NO_CHOICE
             elif use_latest:
                 preference = Preference.USE_LATEST
             else:
                 preference = Preference.DEFAULT
@@ -408,15 +477,17 @@
         if len(unsatisfied) == 1:
             dependency = unsatisfied[0]
         else:
             dependency = min(*unsatisfied, key=_get_min)
 
         locked = self._provider.get_locked(dependency)
         if locked is None:
-            packages = self._dependency_cache.search_for(dependency)
+            packages = self._dependency_cache.search_for(
+                dependency, self._solution.decision_level
+            )
             package = next(iter(packages), None)
 
             if package is None:
                 # If there are no versions that satisfy the constraint,
                 # add an incompatibility that indicates that.
                 self._add_incompatibility(
                     Incompatibility([Term(dependency, True)], NoVersionsCause())
```

### Comparing `poetry-1.5.0/src/poetry/packages/dependency_package.py` & `poetry-1.5.1/src/poetry/packages/dependency_package.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/packages/direct_origin.py` & `poetry-1.5.1/src/poetry/packages/direct_origin.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/packages/locker.py` & `poetry-1.5.1/src/poetry/packages/locker.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/packages/package_collection.py` & `poetry-1.5.1/src/poetry/packages/package_collection.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/plugins/application_plugin.py` & `poetry-1.5.1/src/poetry/plugins/application_plugin.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/plugins/plugin_manager.py` & `poetry-1.5.1/src/poetry/plugins/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/poetry.py` & `poetry-1.5.1/src/poetry/poetry.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/publishing/publisher.py` & `poetry-1.5.1/src/poetry/publishing/publisher.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/publishing/uploader.py` & `poetry-1.5.1/src/poetry/publishing/uploader.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/puzzle/exceptions.py` & `poetry-1.5.1/src/poetry/puzzle/exceptions.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/puzzle/provider.py` & `poetry-1.5.1/src/poetry/puzzle/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,20 +276,16 @@
             return PackageCollection(dependency, [package])
 
         # If we've previously found a direct-origin package that meets this dependency,
         # use it.
         #
         # We rely on the VersionSolver resolving direct-origin dependencies first.
         direct_origin_package = self._direct_origin_packages.get(dependency.name)
-        if direct_origin_package is not None:
-            packages = (
-                [direct_origin_package]
-                if dependency.constraint.allows(direct_origin_package.version)
-                else []
-            )
+        if direct_origin_package and direct_origin_package.satisfies(dependency):
+            packages = [direct_origin_package]
             return PackageCollection(dependency, packages)
 
         packages = self._pool.find_packages(dependency)
 
         packages.sort(
             key=lambda p: (
                 not p.yanked,
```

### Comparing `poetry-1.5.0/src/poetry/puzzle/solver.py` & `poetry-1.5.1/src/poetry/puzzle/solver.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/puzzle/transaction.py` & `poetry-1.5.1/src/poetry/puzzle/transaction.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/pyproject/toml.py` & `poetry-1.5.1/src/poetry/pyproject/toml.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/repositories/abstract_repository.py` & `poetry-1.5.1/src/poetry/repositories/abstract_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/repositories/cached_repository.py` & `poetry-1.5.1/src/poetry/repositories/cached_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/repositories/http_repository.py` & `poetry-1.5.1/src/poetry/repositories/http_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,23 +72,19 @@
         return self._authenticator.authenticated_url(url=self.url)
 
     def _download(self, url: str, dest: Path) -> None:
         return download_file(url, dest, session=self.session)
 
     @contextmanager
     def _cached_or_downloaded_file(self, link: Link) -> Iterator[Path]:
-        filepath = self._authenticator.get_cached_file_for_url(link.url)
-        if filepath:
+        self._log(f"Downloading: {link.url}", level="debug")
+        with temporary_directory() as temp_dir:
+            filepath = Path(temp_dir) / link.filename
+            self._download(link.url, filepath)
             yield filepath
-        else:
-            self._log(f"Downloading: {link.url}", level="debug")
-            with temporary_directory() as temp_dir:
-                filepath = Path(temp_dir) / link.filename
-                self._download(link.url, filepath)
-                yield filepath
 
     def _get_info_from_wheel(self, url: str) -> PackageInfo:
         from poetry.inspection.info import PackageInfo
 
         with self._cached_or_downloaded_file(Link(url)) as filepath:
             return PackageInfo.from_wheel(filepath)
```

### Comparing `poetry-1.5.0/src/poetry/repositories/installed_repository.py` & `poetry-1.5.1/src/poetry/repositories/installed_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/repositories/legacy_repository.py` & `poetry-1.5.1/src/poetry/repositories/legacy_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/repositories/link_sources/base.py` & `poetry-1.5.1/src/poetry/repositories/link_sources/base.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/repositories/link_sources/html.py` & `poetry-1.5.1/src/poetry/repositories/link_sources/html.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/repositories/link_sources/json.py` & `poetry-1.5.1/src/poetry/repositories/link_sources/json.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/repositories/lockfile_repository.py` & `poetry-1.5.1/src/poetry/repositories/lockfile_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/repositories/pypi_repository.py` & `poetry-1.5.1/src/poetry/repositories/pypi_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/repositories/repository.py` & `poetry-1.5.1/src/poetry/repositories/repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/repositories/repository_pool.py` & `poetry-1.5.1/src/poetry/repositories/repository_pool.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/repositories/single_page_repository.py` & `poetry-1.5.1/src/poetry/repositories/single_page_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/toml/file.py` & `poetry-1.5.1/src/poetry/toml/file.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/utils/_compat.py` & `poetry-1.5.1/src/poetry/utils/_compat.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/utils/authenticator.py` & `poetry-1.5.1/src/poetry/utils/authenticator.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import lockfile
 import requests
 import requests.auth
 import requests.exceptions
 
 from cachecontrol import CacheControlAdapter
 from cachecontrol.caches import FileCache
-from cachecontrol.caches.file_cache import url_to_file_path
 from filelock import FileLock
 
 from poetry.config.config import Config
 from poetry.exceptions import PoetryException
 from poetry.utils.constants import REQUESTS_TIMEOUT
 from poetry.utils.constants import RETRY_AFTER_HEADER
 from poetry.utils.constants import STATUS_FORCELIST
@@ -460,21 +459,14 @@
 
     def _get_certs_for_url(self, url: str) -> RepositoryCertificateConfig:
         selected = self.get_repository_config_for_url(url)
         if selected:
             return selected.certs(config=self._config)
         return RepositoryCertificateConfig()
 
-    def get_cached_file_for_url(self, url: str) -> Path | None:
-        if self._cache_control is None:
-            return None
-
-        path = Path(url_to_file_path(url, self._cache_control))
-        return path if path.exists() else None
-
 
 _authenticator: Authenticator | None = None
 
 
 def get_default_authenticator() -> Authenticator:
     global _authenticator
```

### Comparing `poetry-1.5.0/src/poetry/utils/cache.py` & `poetry-1.5.1/src/poetry/utils/cache.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/utils/dependency_specification.py` & `poetry-1.5.1/src/poetry/utils/dependency_specification.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/utils/env.py` & `poetry-1.5.1/src/poetry/utils/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -694,15 +694,15 @@
         conda_env_name = os.environ.get("CONDA_DEFAULT_ENV")
         # It's probably not a good idea to pollute Conda's global "base" env, since
         # most users have it activated all the time.
         in_venv = env_prefix is not None and conda_env_name != "base"
 
         if not in_venv or env is not None:
             # Checking if a local virtualenv exists
-            if self.use_in_project_venv():
+            if self.in_project_venv_exists():
                 venv = self.in_project_venv
 
                 return VirtualEnv(venv)
 
             create_venv = self._poetry.config.get("virtualenvs.create", True)
 
             if not create_venv:
@@ -732,15 +732,15 @@
         if name is None:
             name = self._poetry.package.name
 
         venv_name = self.generate_env_name(name, str(self._poetry.file.path.parent))
         venv_path = self._poetry.config.virtualenvs_path
         env_list = [VirtualEnv(p) for p in sorted(venv_path.glob(f"{venv_name}-py*"))]
 
-        if self.use_in_project_venv():
+        if self.in_project_venv_exists():
             venv = self.in_project_venv
             env_list.insert(0, VirtualEnv(venv))
         return env_list
 
     @staticmethod
     def check_env_is_for_current_project(env: str, base_env_name: str) -> bool:
         """
@@ -851,14 +851,22 @@
 
         return VirtualEnv(venv_path, venv_path)
 
     def use_in_project_venv(self) -> bool:
         in_project: bool | None = self._poetry.config.get("virtualenvs.in-project")
         if in_project is not None:
             return in_project
+
+        return self.in_project_venv.is_dir()
+
+    def in_project_venv_exists(self) -> bool:
+        in_project: bool | None = self._poetry.config.get("virtualenvs.in-project")
+        if in_project is False:
+            return False
+
         return self.in_project_venv.is_dir()
 
     def create_venv(
         self,
         name: str | None = None,
         executable: Path | None = None,
         force: bool = False,
@@ -1242,15 +1250,15 @@
         return implementation
 
     @property
     def python(self) -> Path:
         """
         Path to current python executable
         """
-        return self._bin(self._executable)
+        return Path(self._bin(self._executable))
 
     @property
     def marker_env(self) -> dict[str, Any]:
         if self._marker_env is None:
             self._marker_env = self.get_marker_env()
 
         return self._marker_env
@@ -1310,15 +1318,15 @@
     @property
     def pip(self) -> Path:
         """
         Path to current pip executable
         """
         # we do not use as_posix() here due to issues with windows pathlib2
         # implementation
-        path = self._bin(self._pip_executable)
+        path = Path(self._bin(self._pip_executable))
         if not path.exists():
             return self.pip_embedded
         return path
 
     @property
     def platform(self) -> str:
         return sys.platform
@@ -1430,15 +1438,15 @@
     def get_python_implementation(self) -> str:
         raise NotImplementedError()
 
     def get_marker_env(self) -> dict[str, Any]:
         raise NotImplementedError()
 
     def get_pip_command(self, embedded: bool = False) -> list[str]:
-        if embedded or not self._bin(self._pip_executable).exists():
+        if embedded or not Path(self._bin(self._pip_executable)).exists():
             return [str(self.python), str(self.pip_embedded)]
         # run as module so that pip can update itself on Windows
         return [str(self.python), "-m", "pip"]
 
     def get_supported_tags(self) -> list[Tag]:
         raise NotImplementedError()
 
@@ -1460,15 +1468,15 @@
 
     def get_command_from_bin(self, bin: str) -> list[str]:
         if bin == "pip":
             # when pip is required we need to ensure that we fallback to
             # embedded pip when pip is not available in the environment
             return self.get_pip_command()
 
-        return [str(self._bin(bin))]
+        return [self._bin(bin)]
 
     def run(self, bin: str, *args: str, **kwargs: Any) -> str:
         cmd = self.get_command_from_bin(bin) + list(args)
         return self._run(cmd, **kwargs)
 
     def run_pip(self, *args: str, **kwargs: Any) -> str:
         pip = self.get_pip_command()
@@ -1540,15 +1548,15 @@
             self._script_dirs = [
                 Path(scripts) if scripts is not None else self._bin_dir
             ]
             if self.userbase:
                 self._script_dirs.append(self.userbase / self._script_dirs[0].name)
         return self._script_dirs
 
-    def _bin(self, bin: str) -> Path:
+    def _bin(self, bin: str) -> str:
         """
         Return path to the given executable.
         """
         if self._is_windows and not bin.endswith(".exe"):
             bin_path = self._bin_dir / (bin + ".exe")
         else:
             bin_path = self._bin_dir / bin
@@ -1561,19 +1569,19 @@
             if self._is_windows:
                 if not bin.endswith(".exe"):
                     bin_path = self._path / (bin + ".exe")
                 else:
                     bin_path = self._path / bin
 
                 if bin_path.exists():
-                    return bin_path
+                    return str(bin_path)
 
-            return Path(bin)
+            return bin
 
-        return bin_path
+        return str(bin_path)
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, Env):
             return False
 
         return other.__class__ == self.__class__ and other.path == self.path
 
@@ -1879,16 +1887,16 @@
     def execute(self, bin: str, *args: str, **kwargs: Any) -> int:
         self.executed.append([bin, *list(args)])
 
         if self._execute:
             return super().execute(bin, *args, **kwargs)
         return 0
 
-    def _bin(self, bin: str) -> Path:
-        return Path(bin)
+    def _bin(self, bin: str) -> str:
+        return bin
 
 
 @contextmanager
 def ephemeral_environment(
     executable: Path | None = None,
     flags: dict[str, bool] | None = None,
 ) -> Iterator[VirtualEnv]:
```

### Comparing `poetry-1.5.0/src/poetry/utils/extras.py` & `poetry-1.5.1/src/poetry/utils/extras.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/utils/helpers.py` & `poetry-1.5.1/src/poetry/utils/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,15 +117,15 @@
             fetched_size = 0
             last_percent = 0
 
             # if less than 1MB, we simply show that we're downloading
             # but skip the updating
             set_indicator = total_size > 1024 * 1024
 
-        with dest.open("wb") as f:
+        with atomic_open(dest) as f:
             for chunk in response.iter_content(chunk_size=chunk_size):
                 if chunk:
                     f.write(chunk)
 
                     if set_indicator:
                         fetched_size += len(chunk)
                         percent = (fetched_size * 100) // total_size
```

### Comparing `poetry-1.5.0/src/poetry/utils/password_manager.py` & `poetry-1.5.1/src/poetry/utils/password_manager.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/utils/pip.py` & `poetry-1.5.1/src/poetry/utils/pip.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/utils/setup_reader.py` & `poetry-1.5.1/src/poetry/utils/setup_reader.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/utils/shell.py` & `poetry-1.5.1/src/poetry/utils/shell.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/utils/wheel.py` & `poetry-1.5.1/src/poetry/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/vcs/git/backend.py` & `poetry-1.5.1/src/poetry/vcs/git/backend.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/vcs/git/system.py` & `poetry-1.5.1/src/poetry/vcs/git/system.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/src/poetry/version/version_selector.py` & `poetry-1.5.1/src/poetry/version/version_selector.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/config/test_config.py` & `poetry-1.5.1/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/conftest.py` & `poetry-1.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/cache/conftest.py` & `poetry-1.5.1/tests/console/commands/cache/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/cache/test_clear.py` & `poetry-1.5.1/tests/console/commands/cache/test_clear.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/cache/test_list.py` & `poetry-1.5.1/tests/console/commands/cache/test_list.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/debug/test_resolve.py` & `poetry-1.5.1/tests/console/commands/debug/test_resolve.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/env/conftest.py` & `poetry-1.5.1/tests/console/commands/env/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/env/helpers.py` & `poetry-1.5.1/tests/console/commands/env/helpers.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/env/test_info.py` & `poetry-1.5.1/tests/console/commands/env/test_info.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/env/test_list.py` & `poetry-1.5.1/tests/console/commands/env/test_list.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/env/test_remove.py` & `poetry-1.5.1/tests/console/commands/env/test_remove.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/env/test_use.py` & `poetry-1.5.1/tests/console/commands/env/test_use.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/self/conftest.py` & `poetry-1.5.1/tests/console/commands/self/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/self/fixtures/poetry-1.0.5-darwin.tar.gz` & `poetry-1.5.1/tests/console/commands/self/fixtures/poetry-1.0.5-darwin.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/self/test_add_plugins.py` & `poetry-1.5.1/tests/console/commands/self/test_add_plugins.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/self/test_remove_plugins.py` & `poetry-1.5.1/tests/console/commands/self/test_remove_plugins.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/self/test_self_command.py` & `poetry-1.5.1/tests/console/commands/self/test_self_command.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/self/test_show_plugins.py` & `poetry-1.5.1/tests/console/commands/self/test_show_plugins.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/self/test_update.py` & `poetry-1.5.1/tests/console/commands/self/test_update.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/self/utils.py` & `poetry-1.5.1/tests/console/commands/self/utils.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/source/conftest.py` & `poetry-1.5.1/tests/console/commands/source/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/source/test_add.py` & `poetry-1.5.1/tests/console/commands/source/test_add.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/source/test_remove.py` & `poetry-1.5.1/tests/console/commands/source/test_remove.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/source/test_show.py` & `poetry-1.5.1/tests/console/commands/source/test_show.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/test_about.py` & `poetry-1.5.1/tests/console/commands/test_about.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/test_add.py` & `poetry-1.5.1/tests/console/commands/test_add.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/test_build.py` & `poetry-1.5.1/tests/console/commands/test_build.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/test_check.py` & `poetry-1.5.1/tests/console/commands/test_check.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/test_config.py` & `poetry-1.5.1/tests/console/commands/test_config.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/test_init.py` & `poetry-1.5.1/tests/console/commands/test_init.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/test_install.py` & `poetry-1.5.1/tests/console/commands/test_install.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/test_lock.py` & `poetry-1.5.1/tests/console/commands/test_lock.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/test_new.py` & `poetry-1.5.1/tests/console/commands/test_new.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/test_publish.py` & `poetry-1.5.1/tests/console/commands/test_publish.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/test_remove.py` & `poetry-1.5.1/tests/console/commands/test_remove.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/test_run.py` & `poetry-1.5.1/tests/console/commands/test_run.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/test_search.py` & `poetry-1.5.1/tests/console/commands/test_search.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/test_shell.py` & `poetry-1.5.1/tests/console/commands/test_shell.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/test_show.py` & `poetry-1.5.1/tests/console/commands/test_show.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/test_update.py` & `poetry-1.5.1/tests/console/commands/test_update.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/commands/test_version.py` & `poetry-1.5.1/tests/console/commands/test_version.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/conftest.py` & `poetry-1.5.1/tests/console/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/console/test_application.py` & `poetry-1.5.1/tests/console/test_application.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/build_system_requires_not_available/pyproject.toml` & `poetry-1.5.1/tests/fixtures/build_system_requires_not_available/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/complete.toml` & `poetry-1.5.1/tests/fixtures/complete.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/directory/project_with_transitive_directory_dependencies/setup.py` & `poetry-1.5.1/tests/fixtures/directory/project_with_transitive_directory_dependencies/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl` & `poetry-1.5.1/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/distributions/demo-0.1.0.tar.gz` & `poetry-1.5.1/tests/fixtures/distributions/demo-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/distributions/demo-0.1.2-py2.py3-none-any.whl` & `poetry-1.5.1/tests/fixtures/distributions/demo-0.1.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/distributions/demo_invalid_record-0.1.0-py2.py3-none-any.whl` & `poetry-1.5.1/tests/fixtures/distributions/demo_invalid_record-0.1.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/distributions/demo_invalid_record2-0.1.0-py2.py3-none-any.whl` & `poetry-1.5.1/tests/fixtures/distributions/demo_invalid_record2-0.1.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/extended_project/pyproject.toml` & `poetry-1.5.1/tests/fixtures/extended_project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/extended_project_without_setup/pyproject.toml` & `poetry-1.5.1/tests/fixtures/extended_project_without_setup/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/extended_with_no_setup/build.py` & `poetry-1.5.1/tests/fixtures/extended_with_no_setup/build.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/extended_with_no_setup/extended/extended.c` & `poetry-1.5.1/tests/fixtures/extended_with_no_setup/extended/extended.c`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/extended_with_no_setup/pyproject.toml` & `poetry-1.5.1/tests/fixtures/extended_with_no_setup/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/git/github.com/demo/no-version/setup.py` & `poetry-1.5.1/tests/fixtures/git/github.com/demo/no-version/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/old_lock/poetry.lock` & `poetry-1.5.1/tests/fixtures/old_lock/poetry.lock`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/outdated_lock/poetry.lock` & `poetry-1.5.1/tests/fixtures/outdated_lock/poetry.lock`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/project_with_git_dev_dependency/pyproject.toml` & `poetry-1.5.1/tests/fixtures/project_with_git_dev_dependency/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/project_with_local_dependencies/pyproject.toml` & `poetry-1.5.1/tests/fixtures/project_with_local_dependencies/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/sample_project/pyproject.toml` & `poetry-1.5.1/tests/fixtures/sample_project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/scripts/scripts/check_argv0.py` & `poetry-1.5.1/tests/fixtures/scripts/scripts/check_argv0.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl` & `poetry-1.5.1/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/simple_project/dist/simple_project-1.2.3.tar.gz` & `poetry-1.5.1/tests/fixtures/simple_project/dist/simple_project-1.2.3.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/simple_project/pyproject.toml` & `poetry-1.5.1/tests/fixtures/simple_project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/up_to_date_lock/poetry.lock` & `poetry-1.5.1/tests/fixtures/up_to_date_lock/poetry.lock`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/wheel_with_no_requires_dist/demo-0.1.0-py2.py3-none-any.whl` & `poetry-1.5.1/tests/fixtures/wheel_with_no_requires_dist/demo-0.1.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/with-include/LICENSE` & `poetry-1.5.1/tests/fixtures/with-include/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/with-include/pyproject.toml` & `poetry-1.5.1/tests/fixtures/with-include/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/with_default_source/pyproject.toml` & `poetry-1.5.1/tests/fixtures/with_default_source/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/with_default_source_and_pypi/pyproject.toml` & `poetry-1.5.1/tests/fixtures/with_default_source_and_pypi/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/with_default_source_legacy/pyproject.toml` & `poetry-1.5.1/tests/fixtures/with_default_source_legacy/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/with_default_source_pypi/pyproject.toml` & `poetry-1.5.1/tests/fixtures/with_default_source_pypi/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/with_local_config/pyproject.toml` & `poetry-1.5.1/tests/fixtures/with_local_config/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/with_path_dependency/poetry.lock` & `poetry-1.5.1/tests/fixtures/with_path_dependency/poetry.lock`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/with_two_default_sources/pyproject.toml` & `poetry-1.5.1/tests/fixtures/with_two_default_sources/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/fixtures/with_two_default_sources_legacy/pyproject.toml` & `poetry-1.5.1/tests/fixtures/with_two_default_sources_legacy/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/helpers.py` & `poetry-1.5.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/inspection/test_info.py` & `poetry-1.5.1/tests/inspection/test_info.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/installation/fixtures/extras-with-dependencies.test` & `poetry-1.5.1/tests/installation/fixtures/extras-with-dependencies.test`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/installation/fixtures/extras.test` & `poetry-1.5.1/tests/installation/fixtures/extras.test`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/installation/fixtures/old-lock.test` & `poetry-1.5.1/tests/installation/fixtures/old-lock.test`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/installation/fixtures/update-with-locked-extras.test` & `poetry-1.5.1/tests/installation/fixtures/update-with-locked-extras.test`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/installation/fixtures/with-dependencies-nested-extras.test` & `poetry-1.5.1/tests/installation/fixtures/with-dependencies-nested-extras.test`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/installation/fixtures/with-directory-dependency-poetry-transitive.test` & `poetry-1.5.1/tests/installation/fixtures/with-directory-dependency-poetry-transitive.test`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/installation/fixtures/with-directory-dependency-poetry.test` & `poetry-1.5.1/tests/installation/fixtures/with-directory-dependency-poetry.test`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/installation/fixtures/with-directory-dependency-setuptools.test` & `poetry-1.5.1/tests/installation/fixtures/with-directory-dependency-setuptools.test`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/installation/fixtures/with-duplicate-dependencies.test` & `poetry-1.5.1/tests/installation/fixtures/with-duplicate-dependencies.test`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/installation/fixtures/with-file-dependency-transitive.test` & `poetry-1.5.1/tests/installation/fixtures/with-file-dependency-transitive.test`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/installation/fixtures/with-file-dependency.test` & `poetry-1.5.1/tests/installation/fixtures/with-file-dependency.test`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/installation/fixtures/with-multiple-updates.test` & `poetry-1.5.1/tests/installation/fixtures/with-multiple-updates.test`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/installation/fixtures/with-platform-dependencies.test` & `poetry-1.5.1/tests/installation/fixtures/with-platform-dependencies.test`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/installation/fixtures/with-pypi-repository.test` & `poetry-1.5.1/tests/installation/fixtures/with-pypi-repository.test`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/installation/fixtures/with-same-version-url-dependencies.test` & `poetry-1.5.1/tests/installation/fixtures/with-same-version-url-dependencies.test`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/installation/fixtures/with-sub-dependencies.test` & `poetry-1.5.1/tests/installation/fixtures/with-sub-dependencies.test`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/installation/fixtures/with-url-dependency.test` & `poetry-1.5.1/tests/installation/fixtures/with-url-dependency.test`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/installation/fixtures/with-vcs-dependency-with-extras.test` & `poetry-1.5.1/tests/installation/fixtures/with-vcs-dependency-with-extras.test`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/installation/test_chef.py` & `poetry-1.5.1/tests/installation/test_chef.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/installation/test_chooser.py` & `poetry-1.5.1/tests/installation/test_chooser.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/installation/test_executor.py` & `poetry-1.5.1/tests/installation/test_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,14 +331,15 @@
         assert expected in error
         assert error.count("is yanked") == 1
     else:
         assert expected not in error
         assert error.count("yanked") == 0
 
 
+@pytest.mark.skip(reason="https://github.com/python-poetry/poetry/issues/7983")
 def test_execute_prints_warning_for_invalid_wheels(
     config: Config,
     pool: RepositoryPool,
     io: BufferedIO,
     tmp_path: Path,
     mock_file_downloads: None,
     env: MockEnv,
```

### Comparing `poetry-1.5.0/tests/installation/test_installer.py` & `poetry-1.5.1/tests/installation/test_installer.py`

 * *Files 1% similar despite different names*

```diff
@@ -2655,7 +2655,78 @@
     assert installer.executor.installations[0] == Package(
         "torch",
         version,
         source_type=source_type,
         source_url=source_url,
         source_reference=source_reference,
     )
+
+
+@pytest.mark.parametrize("env_platform", ["darwin", "linux"])
+def test_explicit_source_dependency_with_direct_origin_dependency(
+    pool: RepositoryPool,
+    locker: Locker,
+    installed: CustomInstalledRepository,
+    config: Config,
+    repo: Repository,
+    package: ProjectPackage,
+    env_platform: str,
+) -> None:
+    """
+    A dependency with explicit source should not be satisfied by
+    a direct origin dependency even if there is a version match.
+    """
+    package.add_dependency(
+        Factory.create_dependency(
+            "demo",
+            {
+                "markers": "sys_platform != 'darwin'",
+                "url": "https://python-poetry.org/distributions/demo-0.1.0-py2.py3-none-any.whl",
+            },
+        )
+    )
+    package.add_dependency(
+        Factory.create_dependency(
+            "demo",
+            {
+                "version": "0.1.0",
+                "markers": "sys_platform == 'darwin'",
+                "source": "repo",
+            },
+        )
+    )
+    # The url demo dependency depends on pendulum.
+    repo.add_package(get_package("pendulum", "1.4.4"))
+    repo.add_package(get_package("demo", "0.1.0"))
+
+    installer = Installer(
+        NullIO(),
+        MockEnv(platform=env_platform),
+        package,
+        locker,
+        pool,
+        config,
+        installed=installed,
+        executor=Executor(
+            MockEnv(platform=env_platform),
+            pool,
+            config,
+            NullIO(),
+        ),
+    )
+
+    result = installer.run()
+
+    assert result == 0
+    assert isinstance(installer.executor, Executor)
+    if env_platform == "linux":
+        assert installer.executor.installations == [
+            Package("pendulum", "1.4.4"),
+            Package(
+                "demo",
+                "0.1.0",
+                source_type="url",
+                source_url="https://python-poetry.org/distributions/demo-0.1.0-py2.py3-none-any.whl",
+            ),
+        ]
+    else:
+        assert installer.executor.installations == [Package("demo", "0.1.0")]
```

### Comparing `poetry-1.5.0/tests/installation/test_wheel_installer.py` & `poetry-1.5.1/tests/installation/test_wheel_installer.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/integration/test_utils_vcs_git.py` & `poetry-1.5.1/tests/integration/test_utils_vcs_git.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/json/test_schema_sources.py` & `poetry-1.5.1/tests/json/test_schema_sources.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/masonry/builders/test_editable_builder.py` & `poetry-1.5.1/tests/masonry/builders/test_editable_builder.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/mixology/helpers.py` & `poetry-1.5.1/tests/mixology/helpers.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/mixology/solutions/providers/test_python_requirement_solution_provider.py` & `poetry-1.5.1/tests/mixology/solutions/providers/test_python_requirement_solution_provider.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/mixology/solutions/solutions/test_python_requirement_solution.py` & `poetry-1.5.1/tests/mixology/solutions/solutions/test_python_requirement_solution.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/mixology/version_solver/conftest.py` & `poetry-1.5.1/tests/mixology/version_solver/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/mixology/version_solver/test_backtracking.py` & `poetry-1.5.1/tests/mixology/version_solver/test_backtracking.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/mixology/version_solver/test_basic_graph.py` & `poetry-1.5.1/tests/mixology/version_solver/test_basic_graph.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/mixology/version_solver/test_python_constraint.py` & `poetry-1.5.1/tests/mixology/version_solver/test_python_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/mixology/version_solver/test_unsolvable.py` & `poetry-1.5.1/tests/mixology/version_solver/test_unsolvable.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/mixology/version_solver/test_with_lock.py` & `poetry-1.5.1/tests/mixology/version_solver/test_with_lock.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/packages/test_direct_origin.py` & `poetry-1.5.1/tests/packages/test_direct_origin.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/packages/test_locker.py` & `poetry-1.5.1/tests/packages/test_locker.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/plugins/test_plugin_manager.py` & `poetry-1.5.1/tests/plugins/test_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/publishing/test_publisher.py` & `poetry-1.5.1/tests/publishing/test_publisher.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/publishing/test_uploader.py` & `poetry-1.5.1/tests/publishing/test_uploader.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/puzzle/conftest.py` & `poetry-1.5.1/tests/puzzle/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/puzzle/test_provider.py` & `poetry-1.5.1/tests/puzzle/test_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             [Package("foo", "3")],
             [Package("foo", "2a", source_type="url", source_url=SOME_URL)],
         ),
         (
             Dependency("foo", ">=2"),
             URLDependency("foo", SOME_URL),
             [Package("foo", "3")],
-            [],
+            [Package("foo", "3")],
         ),
         (
             Dependency("foo", ">=1", extras=["bar"]),
             URLDependency("foo", SOME_URL),
             [Package("foo", "3")],
             [Package("foo", "2a", source_type="url", source_url=SOME_URL)],
         ),
@@ -718,7 +718,42 @@
 
     provider.complete_package(DependencyPackage(package.to_dependency(), package))
 
     if with_extra:
         spy.assert_called()
     else:
         spy.assert_not_called()
+
+
+def test_source_dependency_is_satisfied_by_direct_origin(
+    provider: Provider, repository: Repository
+) -> None:
+    direct_origin_package = Package("foo", "1.1", source_type="url")
+    repository.add_package(Package("foo", "1.0"))
+    provider._direct_origin_packages = {"foo": direct_origin_package}
+    dep = Dependency("foo", ">=1")
+
+    assert provider.search_for(dep) == [direct_origin_package]
+
+
+def test_explicit_source_dependency_is_not_satisfied_by_direct_origin(
+    provider: Provider, repository: Repository
+) -> None:
+    repo_package = Package("foo", "1.0")
+    repository.add_package(repo_package)
+    provider._direct_origin_packages = {"foo": Package("foo", "1.1", source_type="url")}
+    dep = Dependency("foo", ">=1")
+    dep.source_name = repository.name
+
+    assert provider.search_for(dep) == [repo_package]
+
+
+def test_source_dependency_is_not_satisfied_by_incompatible_direct_origin(
+    provider: Provider, repository: Repository
+) -> None:
+    repo_package = Package("foo", "2.0")
+    repository.add_package(repo_package)
+    provider._direct_origin_packages = {"foo": Package("foo", "1.0", source_type="url")}
+    dep = Dependency("foo", ">=2")
+    dep.source_name = repository.name
+
+    assert provider.search_for(dep) == [repo_package]
```

### Comparing `poetry-1.5.0/tests/puzzle/test_solver.py` & `poetry-1.5.1/tests/puzzle/test_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1179,14 +1179,72 @@
         [
             {"job": "install", "package": package_b},
             {"job": "install", "package": package_a},
         ],
     )
 
 
+def test_solver_with_dependency_and_prerelease_sub_dependencies_increasing_constraints(
+    solver: Solver,
+    repo: Repository,
+    package: ProjectPackage,
+    mocker: MockerFixture,
+) -> None:
+    """Regression test to ensure the solver eventually uses pre-release
+    dependencies if the package is progressively constrained enough.
+
+    This is different from test_solver_with_dependency_and_prerelease_sub_dependencies
+    above because it also has a wildcard dependency on B at the root level.
+    This causes the solver to first narrow B's candidate versions down to
+    {0.9.0} at an early level, then eventually down to the empty set once A's
+    dependencies are processed at a later level.
+
+    Once the candidate version set is narrowed down to the empty set, the
+    solver should re-evaluate available candidate versions from the source, but
+    include pre-release versions this time as there are no other options.
+    """
+    # Note: The order matters here; B must be added before A or the solver
+    # evaluates A first and we don't encounter the issue. This is a bit
+    # fragile, but the mock call assertions ensure this ordering is maintained.
+    package.add_dependency(Factory.create_dependency("B", "*"))
+    package.add_dependency(Factory.create_dependency("A", "*"))
+
+    package_a = get_package("A", "1.0")
+    package_a.add_dependency(Factory.create_dependency("B", ">0.9.0"))
+
+    repo.add_package(package_a)
+    repo.add_package(get_package("B", "0.9.0"))
+    package_b = get_package("B", "1.0.0.dev4")
+    repo.add_package(package_b)
+
+    search_for_spy = mocker.spy(solver._provider, "search_for")
+    transaction = solver.solve()
+
+    check_solver_result(
+        transaction,
+        [
+            {"job": "install", "package": package_b},
+            {"job": "install", "package": package_a},
+        ],
+    )
+
+    # The assertions below aren't really the point of this test, but are just
+    # being used to ensure the dependency resolution ordering remains the same.
+    search_calls = [
+        call[1][0]
+        for call in search_for_spy.mock_calls
+        if call[1][0].name in ("a", "b")
+    ]
+    assert search_calls == [
+        Dependency("a", "*"),
+        Dependency("b", "*"),
+        Dependency("b", ">0.9.0"),
+    ]
+
+
 def test_solver_circular_dependency(
     solver: Solver, repo: Repository, package: ProjectPackage
 ) -> None:
     package.add_dependency(Factory.create_dependency("A", "*"))
 
     package_a = get_package("A", "1.0")
     package_a.add_dependency(Factory.create_dependency("B", "^1.0"))
@@ -3375,14 +3433,77 @@
 
     # This is not solvable since the demo version is pinned
     # via the git dependency
     with pytest.raises(SolverProblemError):
         solver.solve()
 
 
+@pytest.mark.parametrize("explicit_source", [True, False])
+def test_solver_cannot_choose_url_dependency_for_explicit_source(
+    solver: Solver,
+    repo: Repository,
+    package: ProjectPackage,
+    explicit_source: bool,
+) -> None:
+    """A direct origin dependency cannot satisfy a version dependency with an explicit
+    source. (It can satisfy a version dependency without an explicit source.)
+    """
+    package.add_dependency(
+        Factory.create_dependency(
+            "demo",
+            {
+                "markers": "sys_platform != 'darwin'",
+                "url": "https://foo.bar/distributions/demo-0.1.0-py2.py3-none-any.whl",
+            },
+        )
+    )
+    package.add_dependency(
+        Factory.create_dependency(
+            "demo",
+            {
+                "version": "0.1.0",
+                "markers": "sys_platform == 'darwin'",
+                "source": "repo" if explicit_source else None,
+            },
+        )
+    )
+
+    package_pendulum = get_package("pendulum", "1.4.4")
+    package_demo = get_package("demo", "0.1.0")
+    package_demo_url = Package(
+        "demo",
+        "0.1.0",
+        source_type="url",
+        source_url="https://foo.bar/distributions/demo-0.1.0-py2.py3-none-any.whl",
+    )
+    # The url demo dependency depends on pendulum.
+    repo.add_package(package_pendulum)
+    repo.add_package(package_demo)
+
+    transaction = solver.solve()
+
+    if explicit_source:
+        # direct origin cannot satisfy explicit source
+        # -> package_demo MUST be included
+        expected = [
+            {"job": "install", "package": package_pendulum},
+            {"job": "install", "package": package_demo_url},
+            {"job": "install", "package": package_demo},
+        ]
+    else:
+        # direct origin can satisfy dependency without source
+        # -> package_demo NEED NOT (but could) be included
+        expected = [
+            {"job": "install", "package": package_pendulum},
+            {"job": "install", "package": package_demo_url},
+        ]
+
+    check_solver_result(transaction, expected)
+
+
 def test_solver_should_not_update_same_version_packages_if_installed_has_no_source_type(
     package: ProjectPackage, repo: Repository, pool: RepositoryPool, io: NullIO
 ) -> None:
     package.add_dependency(Factory.create_dependency("foo", "1.0.0"))
 
     foo = Package(
         "foo",
```

### Comparing `poetry-1.5.0/tests/puzzle/test_transaction.py` & `poetry-1.5.1/tests/puzzle/test_transaction.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/pyproject/conftest.py` & `poetry-1.5.1/tests/pyproject/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/pyproject/test_pyproject_toml.py` & `poetry-1.5.1/tests/pyproject/test_pyproject_toml.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/pyproject/test_pyproject_toml_file.py` & `poetry-1.5.1/tests/pyproject/test_pyproject_toml_file.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/cleo-0.7.6.dist-info/METADATA` & `poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/cleo-0.7.6.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-2.3.4.dist-info/METADATA` & `poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-2.3.4.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-with-import-2.3.4.dist-info/METADATA` & `poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/editable-with-import-2.3.4.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/foo-0.1.0-py3.8.egg` & `poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/foo-0.1.0-py3.8.egg`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/installed/lib/python3.7/site-packages/standard-1.2.3.dist-info/METADATA` & `poetry-1.5.1/tests/repositories/fixtures/installed/lib/python3.7/site-packages/standard-1.2.3.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/bender-2.0.5.dist-info/METADATA` & `poetry-1.5.1/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/bender-2.0.5.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/lib64-2.3.4.dist-info/METADATA` & `poetry-1.5.1/tests/repositories/fixtures/installed/lib64/python3.7/site-packages/lib64-2.3.4.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/installed/src/bender/bender.egg-info/PKG-INFO` & `poetry-1.5.1/tests/repositories/fixtures/installed/src/bender/bender.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/installed/src/pendulum/pendulum.egg-info/PKG-INFO` & `poetry-1.5.1/tests/repositories/fixtures/installed/src/pendulum/pendulum.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/installed/vendor/py3.7/attrs-19.3.0.dist-info/METADATA` & `poetry-1.5.1/tests/repositories/fixtures/installed/vendor/py3.7/attrs-19.3.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/legacy/absolute.html` & `poetry-1.5.1/tests/repositories/fixtures/legacy/absolute.html`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/legacy/black.html` & `poetry-1.5.1/tests/repositories/fixtures/legacy/black.html`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/legacy/clikit.html` & `poetry-1.5.1/tests/repositories/fixtures/legacy/clikit.html`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/legacy/discord-py.html` & `poetry-1.5.1/tests/repositories/fixtures/legacy/discord-py.html`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/legacy/futures-partial-yank.html` & `poetry-1.5.1/tests/repositories/fixtures/legacy/futures-partial-yank.html`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/legacy/futures.html` & `poetry-1.5.1/tests/repositories/fixtures/legacy/futures.html`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/legacy/invalid-version.html` & `poetry-1.5.1/tests/repositories/fixtures/legacy/invalid-version.html`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/legacy/ipython.html` & `poetry-1.5.1/tests/repositories/fixtures/legacy/ipython.html`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/legacy/isort.html` & `poetry-1.5.1/tests/repositories/fixtures/legacy/isort.html`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/legacy/poetry-test-py2-py3-metadata-merge.html` & `poetry-1.5.1/tests/repositories/fixtures/legacy/poetry-test-py2-py3-metadata-merge.html`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/legacy/pytest.html` & `poetry-1.5.1/tests/repositories/fixtures/legacy/pytest.html`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/legacy/pyyaml.html` & `poetry-1.5.1/tests/repositories/fixtures/legacy/pyyaml.html`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/legacy/relative.html` & `poetry-1.5.1/tests/repositories/fixtures/legacy/relative.html`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/SQLAlchemy-1.2.12.tar.gz` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/SQLAlchemy-1.2.12.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/Twisted-18.9.0.tar.bz2` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/Twisted-18.9.0.tar.bz2`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/black-19.10b0-py36-none-any.whl` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/black-19.10b0-py36-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/black-21.11b0-py3-none-any.whl` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/black-21.11b0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/cleo-1.0.0a5-py3-none-any.whl` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/cleo-1.0.0a5-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/clikit-0.2.4-py2.py3-none-any.whl` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/clikit-0.2.4-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/discord.py-2.0.0-py3-none-any.whl` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/discord.py-2.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0-py2-none-any.whl` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0-py2-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0.tar.gz` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/importlib_metadata-1.7.0-py2.py3-none-any.whl` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/importlib_metadata-1.7.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py2-none-any.whl` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py2-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py3-none-any.whl` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0.tar.gz` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/ipython-7.5.0-py3-none-any.whl` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/ipython-7.5.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py2-none-any.whl` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py2-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py3-none-any.whl` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4.tar.gz` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0-py2.py3-none-any.whl` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0.tar.gz` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/pastel-0.1.0.tar.gz` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/pastel-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/poetry_core-1.5.0-py3-none-any.whl` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/poetry_core-1.5.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py2-none-any.whl` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py2-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py3-none-any.whl` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/pytest-3.5.0-py2.py3-none-any.whl` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/pytest-3.5.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/pytest-3.5.1-py2.py3-none-any.whl` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/pytest-3.5.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/python-language-server-0.21.2.tar.gz` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/python-language-server-0.21.2.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.2.tar.gz` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.2.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.3.tar.gz` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.3.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/dists/zipp-3.5.0-py3-none-any.whl` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/dists/zipp-3.5.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/attrs/17.4.0.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/attrs/17.4.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/attrs.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/attrs.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/black/19.10b0.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/black/19.10b0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/black/21.11b0.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/black/21.11b0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/black.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/black.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/cachecontrol/0.12.5.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/cachecontrol/0.12.5.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/cachecontrol.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/cachecontrol.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/cleo/1.0.0a5.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/cleo/1.0.0a5.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/clikit/0.2.4.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/clikit/0.2.4.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/clikit.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/clikit.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/colorama/0.3.9.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/colorama/0.3.9.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/colorama.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/colorama.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/discord-py/2.0.0.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/discord-py/2.0.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/funcsigs/1.0.2.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/funcsigs/1.0.2.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/funcsigs.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/funcsigs.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/hbmqtt/0.9.6.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/hbmqtt/0.9.6.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/hbmqtt.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/hbmqtt.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/importlib-metadata/1.7.0.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/importlib-metadata/1.7.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/importlib-metadata.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/importlib-metadata.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/ipython/4.1.0rc1.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/ipython/4.1.0rc1.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/isort/4.3.4.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/isort/4.3.4.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/isort.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/isort.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/jupyter/1.0.0.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/jupyter/1.0.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/jupyter.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/jupyter.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/lockfile/0.12.2.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/lockfile/0.12.2.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/lockfile.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/lockfile.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/more-itertools/4.1.0.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/more-itertools/4.1.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/more-itertools.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/more-itertools.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/pluggy/0.6.0.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/pluggy/0.6.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/poetry/0.12.4.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/poetry/0.12.4.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/poetry-core/1.5.0.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/poetry-core/1.5.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/poetry-core.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/poetry-core.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/poetry.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/poetry.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/py/1.5.3.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/py/1.5.3.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/py.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/py.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/pygame-music-grid.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/pygame-music-grid.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/pylev/1.3.0.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/pylev/1.3.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/pytest/3.5.0.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/pytest/3.5.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/pytest/3.5.1.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/pytest/3.5.1.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/pytest.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/pytest.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/pyyaml/3.13.0.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/pyyaml/3.13.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/pyyaml.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/pyyaml.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/requests/2.18.4.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/requests/2.18.4.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/requests.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/requests.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/setuptools/39.2.0.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/setuptools/39.2.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/setuptools/67.6.1.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/setuptools/67.6.1.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/setuptools.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/setuptools.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/six/1.11.0.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/six/1.11.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/six.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/six.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/sqlalchemy/1.2.12.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/sqlalchemy/1.2.12.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/toga.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/toga.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/tomlkit/0.5.3.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/tomlkit/0.5.3.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/tomlkit.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/tomlkit.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/trackpy/0.4.1.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/trackpy/0.4.1.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/trackpy.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/trackpy.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/twisted/18.9.0.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/twisted/18.9.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/wheel/0.40.0.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/wheel/0.40.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/wheel.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/wheel.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/zipp/3.5.0.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/zipp/3.5.0.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/json/zipp.json` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/json/zipp.json`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/pypi.org/search/search.html` & `poetry-1.5.1/tests/repositories/fixtures/pypi.org/search/search.html`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/fixtures/single-page/jax_releases.html` & `poetry-1.5.1/tests/repositories/fixtures/single-page/jax_releases.html`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/link_sources/test_base.py` & `poetry-1.5.1/tests/repositories/link_sources/test_base.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/link_sources/test_html.py` & `poetry-1.5.1/tests/repositories/link_sources/test_html.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/test_installed_repository.py` & `poetry-1.5.1/tests/repositories/test_installed_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/test_legacy_repository.py` & `poetry-1.5.1/tests/repositories/test_legacy_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/test_lockfile_repository.py` & `poetry-1.5.1/tests/repositories/test_lockfile_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/test_pypi_repository.py` & `poetry-1.5.1/tests/repositories/test_pypi_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/test_repository.py` & `poetry-1.5.1/tests/repositories/test_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/test_repository_pool.py` & `poetry-1.5.1/tests/repositories/test_repository_pool.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/repositories/test_single_page_repository.py` & `poetry-1.5.1/tests/repositories/test_single_page_repository.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/test_factory.py` & `poetry-1.5.1/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/types.py` & `poetry-1.5.1/tests/types.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/utils/fixtures/pyproject.toml` & `poetry-1.5.1/tests/utils/fixtures/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/utils/fixtures/setups/ansible/setup.py` & `poetry-1.5.1/tests/utils/fixtures/setups/ansible/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/utils/fixtures/setups/flask/setup.py` & `poetry-1.5.1/tests/utils/fixtures/setups/flask/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/utils/fixtures/setups/pendulum/setup.py` & `poetry-1.5.1/tests/utils/fixtures/setups/pendulum/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/utils/fixtures/setups/pyyaml/setup.py` & `poetry-1.5.1/tests/utils/fixtures/setups/pyyaml/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/utils/fixtures/setups/requests/setup.py` & `poetry-1.5.1/tests/utils/fixtures/setups/requests/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/utils/fixtures/setups/sqlalchemy/setup.py` & `poetry-1.5.1/tests/utils/fixtures/setups/sqlalchemy/setup.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/utils/test_authenticator.py` & `poetry-1.5.1/tests/utils/test_authenticator.py`

 * *Files 2% similar despite different names*

```diff
@@ -623,30 +623,14 @@
     assert not two_ssh.password
 
     three = authenticator.get_credentials_for_git_url("https://foo.bar/org/three.git")
     assert not three.username
     assert not three.password
 
 
-def test_authenticator_get_cached_file_for_url__cache_miss(config: Config) -> None:
-    authenticator = Authenticator(config, NullIO())
-    assert (
-        authenticator.get_cached_file_for_url("https://foo.bar/cache/miss.whl") is None
-    )
-
-
-def test_authenticator_get_cached_file_for_url__cache_hit(config: Config) -> None:
-    authenticator = Authenticator(config, NullIO())
-    url = "https://foo.bar/files/foo-0.1.0.tar.gz"
-
-    authenticator._cache_control.set(url, b"hello")
-
-    assert authenticator.get_cached_file_for_url(url)
-
-
 @pytest.mark.parametrize(
     ("ca_cert", "client_cert", "result"),
     [
         (None, None, RepositoryCertificateConfig()),
         (
             "path/to/ca.pem",
             "path/to/client.pem",
```

### Comparing `poetry-1.5.0/tests/utils/test_cache.py` & `poetry-1.5.1/tests/utils/test_cache.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/utils/test_dependency_specification.py` & `poetry-1.5.1/tests/utils/test_dependency_specification.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/utils/test_env.py` & `poetry-1.5.1/tests/utils/test_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -1824,7 +1824,14 @@
     with python_wrapper.open("w") as f:
         f.write(f"@echo {wrapped_python}")
     os.environ["PATH"] = str(python_wrapper.parent) + os.pathsep + os.environ["PATH"]
 
     active_python = EnvManager(poetry)._detect_active_python()
 
     assert active_python == wrapped_python
+
+
+def test_command_from_bin_preserves_relative_path(manager: EnvManager) -> None:
+    # https://github.com/python-poetry/poetry/issues/7959
+    env = manager.get()
+    command = env.get_command_from_bin("./foo.py")
+    assert command == ["./foo.py"]
```

### Comparing `poetry-1.5.0/tests/utils/test_env_site.py` & `poetry-1.5.1/tests/utils/test_env_site.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/utils/test_extras.py` & `poetry-1.5.1/tests/utils/test_extras.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/utils/test_helpers.py` & `poetry-1.5.1/tests/utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/utils/test_password_manager.py` & `poetry-1.5.1/tests/utils/test_password_manager.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/utils/test_patterns.py` & `poetry-1.5.1/tests/utils/test_patterns.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/utils/test_pip.py` & `poetry-1.5.1/tests/utils/test_pip.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/utils/test_setup_reader.py` & `poetry-1.5.1/tests/utils/test_setup_reader.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/tests/utils/test_source.py` & `poetry-1.5.1/tests/utils/test_source.py`

 * *Files identical despite different names*

### Comparing `poetry-1.5.0/PKG-INFO` & `poetry-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry
-Version: 1.5.0
+Version: 1.5.1
 Summary: Python dependency management and packaging made easy.
 Home-page: https://python-poetry.org/
 License: MIT
 Keywords: packaging,dependency,poetry
 Author: Sébastien Eustace
 Author-email: sebastien@eustace.io
 Maintainer: Arun Babu Neelicattu
@@ -32,16 +32,16 @@
 Requires-Dist: jsonschema (>=4.10.0,<5.0.0)
 Requires-Dist: keyring (>=23.9.0,<24.0.0)
 Requires-Dist: lockfile (>=0.12.2,<0.13.0)
 Requires-Dist: packaging (>=20.4)
 Requires-Dist: pexpect (>=4.7.0,<5.0.0)
 Requires-Dist: pkginfo (>=1.9.4,<2.0.0)
 Requires-Dist: platformdirs (>=3.0.0,<4.0.0)
-Requires-Dist: poetry-core (==1.6.0)
-Requires-Dist: poetry-plugin-export (>=1.3.1,<2.0.0)
+Requires-Dist: poetry-core (==1.6.1)
+Requires-Dist: poetry-plugin-export (>=1.4.0,<2.0.0)
 Requires-Dist: pyproject-hooks (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.18,<3.0)
 Requires-Dist: requests-toolbelt (>=0.9.1,<2)
 Requires-Dist: shellingham (>=1.5,<2.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
 Requires-Dist: tomlkit (>=0.11.4,<1.0.0)
 Requires-Dist: trove-classifiers (>=2022.5.19)
```

