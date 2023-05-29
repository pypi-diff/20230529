# Comparing `tmp/pdm-2.6.1.tar.gz` & `tmp/pdm-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-2.6.1.tar", last modified: Wed May 10 03:28:09 2023, max compression
+gzip compressed data, was "pdm-2.7.0.tar", last modified: Mon May 29 04:11:10 2023, max compression
```

## Comparing `pdm-2.6.1.tar` & `pdm-2.7.0.tar`

### file list

```diff
@@ -1,272 +1,272 @@
--rw-r--r--   0        0        0   119286 2023-05-10 03:27:52.210642 pdm-2.6.1/CHANGELOG.md
--rw-r--r--   0        0        0     1075 2023-05-10 03:27:52.210642 pdm-2.6.1/LICENSE
--rw-r--r--   0        0        0     1075 2023-05-10 03:27:52.210642 pdm-2.6.1/LICENSE
--rw-r--r--   0        0        0     7986 2023-05-10 03:27:52.210642 pdm-2.6.1/README.md
--rw-r--r--   0        0        0     7986 2023-05-10 03:27:52.210642 pdm-2.6.1/README.md
--rw-r--r--   0        0        0     4448 2023-05-10 03:28:09.714369 pdm-2.6.1/pyproject.toml
--rw-r--r--   0        0        0       65 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/__main__.py
--rw-r--r--   0        0        0      316 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/__version__.py
--rw-r--r--   0        0        0     2432 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/_types.py
--rw-r--r--   0        0        0      237 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/builders/__init__.py
--rw-r--r--   0        0        0    11850 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/builders/base.py
--rw-r--r--   0        0        0     1755 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/builders/editable.py
--rw-r--r--   0        0        0      656 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/builders/sdist.py
--rw-r--r--   0        0        0     1073 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/builders/wheel.py
--rw-r--r--   0        0        0        0 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/cli/__init__.py
--rw-r--r--   0        0        0    33958 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/cli/actions.py
--rw-r--r--   0        0        0        0 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/cli/commands/__init__.py
--rw-r--r--   0        0        0     2404 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/cli/commands/add.py
--rw-r--r--   0        0        0     2174 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/cli/commands/base.py
--rw-r--r--   0        0        0     2380 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/cli/commands/build.py
--rw-r--r--   0        0        0     6529 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/cli/commands/cache.py
--rw-r--r--   0        0        0     1324 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/cli/commands/completion.py
--rw-r--r--   0        0        0     6186 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/cli/commands/config.py
--rw-r--r--   0        0        0     2948 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/cli/commands/export.py
--rw-r--r--   0        0        0     3136 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/cli/commands/fix/__init__.py
--rw-r--r--   0        0        0     2309 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/cli/commands/fix/fixers.py
--rw-r--r--   0        0        0     1071 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/cli/commands/import_cmd.py
--rw-r--r--   0        0        0     3032 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/cli/commands/info.py
--rw-r--r--   0        0        0     5860 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/cli/commands/init.py
--rw-r--r--   0        0        0     3500 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/cli/commands/install.py
--rw-r--r--   0        0        0    15743 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/cli/commands/list.py
--rw-r--r--   0        0        0     2196 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/cli/commands/lock.py
--rw-r--r--   0        0        0     6161 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/cli/commands/publish/__init__.py
--rw-r--r--   0        0        0     7904 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/cli/commands/publish/package.py
--rw-r--r--   0        0        0     6424 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/cli/commands/publish/repository.py
--rw-r--r--   0        0        0     1672 2023-05-10 03:27:52.214642 pdm-2.6.1/src/pdm/cli/commands/remove.py
--rw-r--r--   0        0        0    15360 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/cli/commands/run.py
--rw-r--r--   0        0        0     2436 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/cli/commands/search.py
--rw-r--r--   0        0        0     9364 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/cli/commands/self_cmd.py
--rw-r--r--   0        0        0     2896 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/cli/commands/show.py
--rw-r--r--   0        0        0     1447 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/cli/commands/sync.py
--rw-r--r--   0        0        0     2392 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/cli/commands/update.py
--rw-r--r--   0        0        0     1318 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/cli/commands/use.py
--rw-r--r--   0        0        0     1683 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/cli/commands/venv/__init__.py
--rw-r--r--   0        0        0     2426 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/cli/commands/venv/activate.py
--rw-r--r--   0        0        0     6171 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/cli/commands/venv/backends.py
--rw-r--r--   0        0        0     2155 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/cli/commands/venv/create.py
--rw-r--r--   0        0        0      819 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/cli/commands/venv/list.py
--rw-r--r--   0        0        0     2195 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/cli/commands/venv/purge.py
--rw-r--r--   0        0        0     1279 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/cli/commands/venv/remove.py
--rw-r--r--   0        0        0     2759 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/cli/commands/venv/utils.py
--rw-r--r--   0        0        0        0 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/cli/completions/__init__.py
--rw-r--r--   0        0        0     5069 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/cli/completions/pdm.bash
--rw-r--r--   0        0        0    37780 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/cli/completions/pdm.fish
--rw-r--r--   0        0        0    18548 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/cli/completions/pdm.ps1
--rw-r--r--   0        0        0    25037 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/cli/completions/pdm.zsh
--rw-r--r--   0        0        0     3840 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/cli/filters.py
--rw-r--r--   0        0        0     1481 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/cli/hooks.py
--rw-r--r--   0        0        0    10407 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/cli/options.py
--rw-r--r--   0        0        0    24638 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/cli/utils.py
--rw-r--r--   0        0        0     2409 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/compat.py
--rw-r--r--   0        0        0     9744 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/core.py
--rw-r--r--   0        0        0      825 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/environments/__init__.py
--rw-r--r--   0        0        0     8780 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/environments/base.py
--rw-r--r--   0        0        0     3560 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/environments/local.py
--rw-r--r--   0        0        0     1600 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/environments/python.py
--rw-r--r--   0        0        0     1365 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/exceptions.py
--rw-r--r--   0        0        0     1086 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/formats/__init__.py
--rw-r--r--   0        0        0     3215 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/formats/base.py
--rw-r--r--   0        0        0     5741 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/formats/flit.py
--rw-r--r--   0        0        0     2349 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/formats/pipfile.py
--rw-r--r--   0        0        0     7289 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/formats/poetry.py
--rw-r--r--   0        0        0     7131 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/formats/requirements.py
--rw-r--r--   0        0        0     2271 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/formats/setup_py.py
--rw-r--r--   0        0        0      119 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/installers/__init__.py
--rw-r--r--   0        0        0     1320 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/installers/core.py
--rw-r--r--   0        0        0    10908 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/installers/installers.py
--rw-r--r--   0        0        0     2091 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/installers/manager.py
--rw-r--r--   0        0        0     2226 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/installers/packages.py
--rw-r--r--   0        0        0    18026 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/installers/synchronizers.py
--rw-r--r--   0        0        0    10903 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/installers/uninstallers.py
--rw-r--r--   0        0        0        0 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/models/__init__.py
--rw-r--r--   0        0        0     2111 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/models/auth.py
--rw-r--r--   0        0        0     4394 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/models/backends.py
--rw-r--r--   0        0        0    10872 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/models/caches.py
--rw-r--r--   0        0        0    24340 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/models/candidates.py
--rw-r--r--   0        0        0      287 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/models/environment.py
--rw-r--r--   0        0        0     1714 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/models/in_process/__init__.py
--rw-r--r--   0        0        0     2049 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/models/in_process/get_abi_tag.py
--rw-r--r--   0        0        0     6182 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/models/in_process/parse_setup.py
--rw-r--r--   0        0        0     1165 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/models/in_process/pep508.py
--rw-r--r--   0        0        0     1653 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/models/in_process/sysconfig_get_paths.py
--rw-r--r--   0        0        0     5701 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/models/markers.py
--rw-r--r--   0        0        0     3507 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/models/project_info.py
--rw-r--r--   0        0        0     2111 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/models/python.py
--rw-r--r--   0        0        0      318 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/models/python_max_versions.json
--rw-r--r--   0        0        0    20893 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/models/repositories.py
--rw-r--r--   0        0        0    17998 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/models/requirements.py
--rw-r--r--   0        0        0     2313 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/models/search.py
--rw-r--r--   0        0        0     2414 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/models/session.py
--rw-r--r--   0        0        0    14482 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/models/setup.py
--rw-r--r--   0        0        0    16337 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/models/specifiers.py
--rw-r--r--   0        0        0     1300 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/models/venv.py
--rw-r--r--   0        0        0     5899 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/models/versions.py
--rw-r--r--   0        0        0     2721 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/models/working_set.py
--rw-r--r--   0        0        0        0 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/pep582/__init__.py
--rw-r--r--   0        0        0     4481 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/pep582/sitecustomize.py
--rw-r--r--   0        0        0      134 2023-05-10 03:27:52.218642 pdm-2.6.1/src/pdm/project/__init__.py
--rw-r--r--   0        0        0    15969 2023-05-10 03:27:52.222642 pdm-2.6.1/src/pdm/project/config.py
--rw-r--r--   0        0        0    26706 2023-05-10 03:27:52.222642 pdm-2.6.1/src/pdm/project/core.py
--rw-r--r--   0        0        0     2093 2023-05-10 03:27:52.222642 pdm-2.6.1/src/pdm/project/lockfile.py
--rw-r--r--   0        0        0     3385 2023-05-10 03:27:52.222642 pdm-2.6.1/src/pdm/project/project_file.py
--rw-r--r--   0        0        0     1070 2023-05-10 03:27:52.222642 pdm-2.6.1/src/pdm/project/toml_file.py
--rw-r--r--   0        0        0        0 2023-05-10 03:27:52.222642 pdm-2.6.1/src/pdm/py.typed
--rw-r--r--   0        0        0    19689 2023-05-10 03:27:52.222642 pdm-2.6.1/src/pdm/pytest.py
--rw-r--r--   0        0        0       61 2023-05-10 03:27:52.222642 pdm-2.6.1/src/pdm/resolver/__init__.py
--rw-r--r--   0        0        0     1954 2023-05-10 03:27:52.222642 pdm-2.6.1/src/pdm/resolver/core.py
--rw-r--r--   0        0        0    13119 2023-05-10 03:27:52.222642 pdm-2.6.1/src/pdm/resolver/providers.py
--rw-r--r--   0        0        0     1580 2023-05-10 03:27:52.222642 pdm-2.6.1/src/pdm/resolver/python.py
--rw-r--r--   0        0        0     3742 2023-05-10 03:27:52.222642 pdm-2.6.1/src/pdm/resolver/reporters.py
--rw-r--r--   0        0        0     4027 2023-05-10 03:27:52.222642 pdm-2.6.1/src/pdm/signals.py
--rw-r--r--   0        0        0     7966 2023-05-10 03:27:52.222642 pdm-2.6.1/src/pdm/termui.py
--rw-r--r--   0        0        0    13744 2023-05-10 03:27:52.222642 pdm-2.6.1/src/pdm/utils.py
--rw-r--r--   0        0        0       72 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/cli/__init__.py
--rw-r--r--   0        0        0     2631 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/cli/conftest.py
--rw-r--r--   0        0        0    12370 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/cli/test_add.py
--rw-r--r--   0        0        0     5784 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/cli/test_build.py
--rw-r--r--   0        0        0     5229 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/cli/test_cache.py
--rw-r--r--   0        0        0     7489 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/cli/test_config.py
--rw-r--r--   0        0        0     2029 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/cli/test_fix.py
--rw-r--r--   0        0        0    10375 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/cli/test_hooks.py
--rw-r--r--   0        0        0     4454 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/cli/test_init.py
--rw-r--r--   0        0        0    11265 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/cli/test_install.py
--rw-r--r--   0        0        0    28998 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/cli/test_list.py
--rw-r--r--   0        0        0     6324 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/cli/test_lock.py
--rw-r--r--   0        0        0     7748 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/cli/test_others.py
--rw-r--r--   0        0        0     5722 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/cli/test_publish.py
--rw-r--r--   0        0        0     3872 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/cli/test_remove.py
--rw-r--r--   0        0        0    29259 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/cli/test_run.py
--rw-r--r--   0        0        0     3599 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/cli/test_self_command.py
--rw-r--r--   0        0        0     8888 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/cli/test_update.py
--rw-r--r--   0        0        0     2942 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/cli/test_use.py
--rw-r--r--   0        0        0    10430 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/cli/test_venv.py
--rw-r--r--   0        0        0     3079 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/conftest.py
--rw-r--r--   0        0        0      235 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/fixtures/Pipfile
--rw-r--r--   0        0        0        0 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/fixtures/__init__.py
--rw-r--r--   0        0        0    49497 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
--rw-r--r--   0        0        0      546 2023-05-10 03:27:52.222642 pdm-2.6.1/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
--rw-r--r--   0        0        0   422824 2023-05-10 03:27:52.226642 pdm-2.6.1/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1254 2023-05-10 03:27:52.226642 pdm-2.6.1/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
--rw-r--r--   0        0        0     1254 2023-05-10 03:27:52.226642 pdm-2.6.1/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1038 2023-05-10 03:27:52.226642 pdm-2.6.1/tests/fixtures/artifacts/demo-0.0.1.tar.gz
--rw-r--r--   0        0        0     2615 2023-05-10 03:27:52.226642 pdm-2.6.1/tests/fixtures/artifacts/demo-0.0.1.zip
--rw-r--r--   0        0        0     4595 2023-05-10 03:27:52.226642 pdm-2.6.1/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
--rw-r--r--   0        0        0     5359 2023-05-10 03:27:52.226642 pdm-2.6.1/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0    56715 2023-05-10 03:27:52.226642 pdm-2.6.1/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
--rw-r--r--   0        0        0     6138 2023-05-10 03:27:52.226642 pdm-2.6.1/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5786 2023-05-10 03:27:52.226642 pdm-2.6.1/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
--rw-r--r--   0        0        0    17978 2023-05-10 03:27:52.226642 pdm-2.6.1/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
--rw-r--r--   0        0        0    24489 2023-05-10 03:27:52.226642 pdm-2.6.1/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0   156727 2023-05-10 03:27:52.226642 pdm-2.6.1/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl
--rw-r--r--   0        0        0     1401 2023-05-10 03:27:52.226642 pdm-2.6.1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl
--rw-r--r--   0        0        0     1405 2023-05-10 03:27:52.226642 pdm-2.6.1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl
--rw-r--r--   0        0        0   305481 2023-05-10 03:27:52.230642 pdm-2.6.1/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
--rw-r--r--   0        0        0   531270 2023-05-10 03:27:52.234642 pdm-2.6.1/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
--rw-r--r--   0        0        0  1232518 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
--rw-r--r--   0        0        0    26662 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
--rw-r--r--   0        0        0    35301 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5312 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
--rw-r--r--   0        0        0      326 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/index/demo.html
--rw-r--r--   0        0        0      511 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/index/future-fstrings.html
--rw-r--r--   0        0        0      262 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/index/pep345-legacy.html
--rw-r--r--   0        0        0      262 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/index/wheel.html
--rw-r--r--   0        0        0        0 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/__init__.py
--rw-r--r--   0        0        0       42 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-#-with-hash/demo.py
--rw-r--r--   0        0        0      332 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-#-with-hash/setup.py
--rw-r--r--   0        0        0       26 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-combined-extras/demo.py
--rw-r--r--   0        0        0      462 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-combined-extras/pyproject.toml
--rw-r--r--   0        0        0       42 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-failure-no-dep/demo.py
--rw-r--r--   0        0        0      246 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-failure-no-dep/setup.py
--rw-r--r--   0        0        0       42 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-failure/demo.py
--rw-r--r--   0        0        0      345 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-failure/setup.py
--rw-r--r--   0        0        0       12 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-module/LICENSE
--rw-r--r--   0        0        0       24 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-module/README.md
--rw-r--r--   0        0        0       14 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-module/bar_module.py
--rw-r--r--   0        0        0       36 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-module/foo_module.py
--rw-r--r--   0        0        0      442 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-module/pyproject.toml
--rw-r--r--   0        0        0     3983 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
--rw-r--r--   0        0        0      318 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
--rw-r--r--   0        0        0      157 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
--rw-r--r--   0        0        0       12 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-package/LICENSE
--rw-r--r--   0        0        0       24 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-package/README.md
--rw-r--r--   0        0        0       16 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-package/data_out.json
--rw-r--r--   0        0        0       22 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-package/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-package/my_package/data.json
--rw-r--r--   0        0        0    29800 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-package/pdm.lock
--rw-r--r--   0        0        0      574 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-package/pyproject.toml
--rw-r--r--   0        0        0      122 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-package/requirements.ini
--rw-r--r--   0        0        0     7521 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-package/requirements.txt
--rw-r--r--   0        0        0      211 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-package/requirements_simple.txt
--rw-r--r--   0        0        0      728 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-package/setup.txt
--rw-r--r--   0        0        0       21 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-package/single_module.py
--rw-r--r--   0        0        0       18 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-parent-package/README.md
--rw-r--r--   0        0        0       22 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-parent-package/package-a/foo.py
--rw-r--r--   0        0        0      120 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-parent-package/package-a/setup.py
--rw-r--r--   0        0        0       22 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-parent-package/package-b/bar.py
--rw-r--r--   0        0        0      197 2023-05-10 03:27:52.238642 pdm-2.6.1/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
--rw-r--r--   0        0        0       42 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/demo-prerelease/demo.py
--rw-r--r--   0        0        0      334 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/demo-prerelease/setup.py
--rw-r--r--   0        0        0       12 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/demo-src-package/LICENSE
--rw-r--r--   0        0        0       24 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/demo-src-package/README.md
--rw-r--r--   0        0        0       16 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/demo-src-package/data_out.json
--rw-r--r--   0        0        0      456 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/demo-src-package/pyproject.toml
--rw-r--r--   0        0        0       21 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/demo-src-package/single_module.py
--rw-r--r--   0        0        0       22 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/demo-src-package/src/my_package/data.json
--rw-r--r--   0        0        0       42 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/demo/demo.py
--rw-r--r--   0        0        0      332 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/demo/setup.py
--rw-r--r--   0        0        0       26 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/demo_extras/demo.py
--rw-r--r--   0        0        0      250 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/demo_extras/setup.py
--rw-r--r--   0        0        0        0 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/flit-demo/README.rst
--rw-r--r--   0        0        0        0 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/flit-demo/doc/index.html
--rw-r--r--   0        0        0       49 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/flit-demo/flit.py
--rw-r--r--   0        0        0      969 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/flit-demo/pyproject.toml
--rw-r--r--   0        0        0       12 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/poetry-demo/mylib.py
--rw-r--r--   0        0        0      863 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/poetry-demo/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/test-hatch-static/README.md
--rw-r--r--   0        0        0      386 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/test-hatch-static/pyproject.toml
--rw-r--r--   0        0        0       11 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/test-monorepo/README.md
--rw-r--r--   0        0        0        0 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/test-monorepo/core/core.py
--rw-r--r--   0        0        0      179 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/test-monorepo/core/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/test-monorepo/package_a/alice.py
--rw-r--r--   0        0        0      231 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/test-monorepo/package_b/bob.py
--rw-r--r--   0        0        0      231 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
--rw-r--r--   0        0        0      237 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/test-monorepo/pyproject.toml
--rw-r--r--   0        0        0      380 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/test-plugin-pdm/hello.py
--rw-r--r--   0        0        0      312 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
--rw-r--r--   0        0        0      380 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/test-plugin/hello.py
--rw-r--r--   0        0        0      168 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/test-plugin/setup.py
--rw-r--r--   0        0        0        0 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/test-removal/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/test-removal/bar.py
--rw-r--r--   0        0        0        0 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/test-removal/foo.py
--rw-r--r--   0        0        0        0 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/test-removal/subdir/__init__.py
--rw-r--r--   0        0        0       10 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/test-setuptools/AUTHORS
--rw-r--r--   0        0        0       12 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/test-setuptools/README.md
--rw-r--r--   0        0        0       22 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/test-setuptools/mymodule.py
--rw-r--r--   0        0        0      398 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/test-setuptools/setup.cfg
--rw-r--r--   0        0        0      308 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/projects/test-setuptools/setup.py
--rw-r--r--   0        0        0     1525 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/pypi.json
--rw-r--r--   0        0        0     1329 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/pyproject.toml
--rw-r--r--   0        0        0       20 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/requirements-include.txt
--rw-r--r--   0        0        0      502 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/fixtures/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/models/__init__.py
--rw-r--r--   0        0        0     3814 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/models/test_backends.py
--rw-r--r--   0        0        0    13285 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/models/test_candidates.py
--rw-r--r--   0        0        0     1971 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/models/test_marker.py
--rw-r--r--   0        0        0     2679 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/models/test_requirements.py
--rw-r--r--   0        0        0     2526 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/models/test_setup_parsing.py
--rw-r--r--   0        0        0     3418 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/models/test_specifiers.py
--rw-r--r--   0        0        0     2703 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/models/test_versions.py
--rw-r--r--   0        0        0        0 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/resolver/__init__.py
--rw-r--r--   0        0        0    11567 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/resolver/test_resolve.py
--rw-r--r--   0        0        0     7187 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/test_formats.py
--rw-r--r--   0        0        0     7231 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/test_installer.py
--rw-r--r--   0        0        0     1829 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/test_integration.py
--rw-r--r--   0        0        0     3361 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/test_plugin.py
--rw-r--r--   0        0        0    11478 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/test_project.py
--rw-r--r--   0        0        0     1103 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/test_signals.py
--rw-r--r--   0        0        0     4364 2023-05-10 03:27:52.242642 pdm-2.6.1/tests/test_utils.py
--rw-r--r--   0        0        0     9669 1970-01-01 00:00:00.000000 pdm-2.6.1/PKG-INFO
+-rw-r--r--   0        0        0   121652 2023-05-29 04:11:03.270091 pdm-2.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1075 2023-05-29 04:11:03.270091 pdm-2.7.0/LICENSE
+-rw-r--r--   0        0        0     1075 2023-05-29 04:11:03.270091 pdm-2.7.0/LICENSE
+-rw-r--r--   0        0        0     7986 2023-05-29 04:11:03.270091 pdm-2.7.0/README.md
+-rw-r--r--   0        0        0     7986 2023-05-29 04:11:03.270091 pdm-2.7.0/README.md
+-rw-r--r--   0        0        0     4384 2023-05-29 04:11:10.474134 pdm-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/__main__.py
+-rw-r--r--   0        0        0      316 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/__version__.py
+-rw-r--r--   0        0        0     3282 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/_types.py
+-rw-r--r--   0        0        0      237 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/builders/__init__.py
+-rw-r--r--   0        0        0    11850 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/builders/base.py
+-rw-r--r--   0        0        0     1755 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/builders/editable.py
+-rw-r--r--   0        0        0      656 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/builders/sdist.py
+-rw-r--r--   0        0        0     1073 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/builders/wheel.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/__init__.py
+-rw-r--r--   0        0        0    30077 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/actions.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2404 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/add.py
+-rw-r--r--   0        0        0     2174 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/base.py
+-rw-r--r--   0        0        0     4236 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/build.py
+-rw-r--r--   0        0        0     6529 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/cache.py
+-rw-r--r--   0        0        0     1324 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/completion.py
+-rw-r--r--   0        0        0     5812 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/config.py
+-rw-r--r--   0        0        0     2948 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/export.py
+-rw-r--r--   0        0        0     3136 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/fix/__init__.py
+-rw-r--r--   0        0        0     2309 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/fix/fixers.py
+-rw-r--r--   0        0        0     1071 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/import_cmd.py
+-rw-r--r--   0        0        0     3032 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/info.py
+-rw-r--r--   0        0        0     8510 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/init.py
+-rw-r--r--   0        0        0     3589 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/install.py
+-rw-r--r--   0        0        0    15743 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/list.py
+-rw-r--r--   0        0        0     2196 2023-05-29 04:11:03.274091 pdm-2.7.0/src/pdm/cli/commands/lock.py
+-rw-r--r--   0        0        0     6596 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/publish/__init__.py
+-rw-r--r--   0        0        0     8027 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/publish/package.py
+-rw-r--r--   0        0        0     6782 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/publish/repository.py
+-rw-r--r--   0        0        0     1672 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/remove.py
+-rw-r--r--   0        0        0    15445 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/run.py
+-rw-r--r--   0        0        0     2436 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/search.py
+-rw-r--r--   0        0        0     9364 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/self_cmd.py
+-rw-r--r--   0        0        0     2896 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/show.py
+-rw-r--r--   0        0        0     1447 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/sync.py
+-rw-r--r--   0        0        0     2392 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/update.py
+-rw-r--r--   0        0        0     1318 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/use.py
+-rw-r--r--   0        0        0     1683 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/venv/__init__.py
+-rw-r--r--   0        0        0     2426 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/venv/activate.py
+-rw-r--r--   0        0        0     6171 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/venv/backends.py
+-rw-r--r--   0        0        0     2155 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/venv/create.py
+-rw-r--r--   0        0        0      819 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/venv/list.py
+-rw-r--r--   0        0        0     2195 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/venv/purge.py
+-rw-r--r--   0        0        0     1279 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/venv/remove.py
+-rw-r--r--   0        0        0     2759 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/commands/venv/utils.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/completions/__init__.py
+-rw-r--r--   0        0        0     5083 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/completions/pdm.bash
+-rw-r--r--   0        0        0    38005 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/completions/pdm.fish
+-rw-r--r--   0        0        0    18567 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/completions/pdm.ps1
+-rw-r--r--   0        0        0    25089 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/completions/pdm.zsh
+-rw-r--r--   0        0        0     3840 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/filters.py
+-rw-r--r--   0        0        0     1481 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/hooks.py
+-rw-r--r--   0        0        0    10461 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/options.py
+-rw-r--r--   0        0        0    24722 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/cli/utils.py
+-rw-r--r--   0        0        0     2226 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/compat.py
+-rw-r--r--   0        0        0    10647 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/core.py
+-rw-r--r--   0        0        0      825 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/environments/__init__.py
+-rw-r--r--   0        0        0     8850 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/environments/base.py
+-rw-r--r--   0        0        0     3560 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/environments/local.py
+-rw-r--r--   0        0        0     1600 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/environments/python.py
+-rw-r--r--   0        0        0     1365 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/exceptions.py
+-rw-r--r--   0        0        0     1202 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/formats/__init__.py
+-rw-r--r--   0        0        0     3215 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/formats/base.py
+-rw-r--r--   0        0        0     5788 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/formats/flit.py
+-rw-r--r--   0        0        0     2400 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/formats/pipfile.py
+-rw-r--r--   0        0        0     7474 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/formats/poetry.py
+-rw-r--r--   0        0        0     7190 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/formats/requirements.py
+-rw-r--r--   0        0        0     2309 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/formats/setup_py.py
+-rw-r--r--   0        0        0      119 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/installers/__init__.py
+-rw-r--r--   0        0        0     1390 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/installers/core.py
+-rw-r--r--   0        0        0    10901 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/installers/installers.py
+-rw-r--r--   0        0        0     2091 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/installers/manager.py
+-rw-r--r--   0        0        0     2226 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/installers/packages.py
+-rw-r--r--   0        0        0    18161 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/installers/synchronizers.py
+-rw-r--r--   0        0        0    10990 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/installers/uninstallers.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/__init__.py
+-rw-r--r--   0        0        0     3162 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/auth.py
+-rw-r--r--   0        0        0     4394 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/backends.py
+-rw-r--r--   0        0        0    10910 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/caches.py
+-rw-r--r--   0        0        0    26568 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/candidates.py
+-rw-r--r--   0        0        0      287 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/environment.py
+-rw-r--r--   0        0        0     1714 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/in_process/__init__.py
+-rw-r--r--   0        0        0     2049 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/in_process/get_abi_tag.py
+-rw-r--r--   0        0        0     6182 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/in_process/parse_setup.py
+-rw-r--r--   0        0        0     1165 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/in_process/pep508.py
+-rw-r--r--   0        0        0     1653 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/in_process/sysconfig_get_paths.py
+-rw-r--r--   0        0        0     5701 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/markers.py
+-rw-r--r--   0        0        0     3507 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/project_info.py
+-rw-r--r--   0        0        0     2195 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/python.py
+-rw-r--r--   0        0        0      318 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/python_max_versions.json
+-rw-r--r--   0        0        0    21031 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/repositories.py
+-rw-r--r--   0        0        0    18068 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/requirements.py
+-rw-r--r--   0        0        0     2313 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/search.py
+-rw-r--r--   0        0        0     1340 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/session.py
+-rw-r--r--   0        0        0    14482 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/setup.py
+-rw-r--r--   0        0        0    16337 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/specifiers.py
+-rw-r--r--   0        0        0     1300 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/venv.py
+-rw-r--r--   0        0        0     5924 2023-05-29 04:11:03.278091 pdm-2.7.0/src/pdm/models/versions.py
+-rw-r--r--   0        0        0     2721 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/models/working_set.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/pep582/__init__.py
+-rw-r--r--   0        0        0     4481 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/pep582/sitecustomize.py
+-rw-r--r--   0        0        0      134 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/project/__init__.py
+-rw-r--r--   0        0        0    16002 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/project/config.py
+-rw-r--r--   0        0        0    27041 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/project/core.py
+-rw-r--r--   0        0        0     2093 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/project/lockfile.py
+-rw-r--r--   0        0        0     3385 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/project/project_file.py
+-rw-r--r--   0        0        0     1070 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/project/toml_file.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/py.typed
+-rw-r--r--   0        0        0    19876 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/pytest.py
+-rw-r--r--   0        0        0       61 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/resolver/__init__.py
+-rw-r--r--   0        0        0     1954 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/resolver/core.py
+-rw-r--r--   0        0        0    13119 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/resolver/providers.py
+-rw-r--r--   0        0        0     1580 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/resolver/python.py
+-rw-r--r--   0        0        0     3742 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/resolver/reporters.py
+-rw-r--r--   0        0        0     4027 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/signals.py
+-rw-r--r--   0        0        0     8054 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/termui.py
+-rw-r--r--   0        0        0    13866 2023-05-29 04:11:03.282091 pdm-2.7.0/src/pdm/utils.py
+-rw-r--r--   0        0        0       72 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/__init__.py
+-rw-r--r--   0        0        0     3723 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/conftest.py
+-rw-r--r--   0        0        0    12370 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_add.py
+-rw-r--r--   0        0        0     5799 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_build.py
+-rw-r--r--   0        0        0     5229 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_cache.py
+-rw-r--r--   0        0        0     9286 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_config.py
+-rw-r--r--   0        0        0     2029 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_fix.py
+-rw-r--r--   0        0        0    10375 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_hooks.py
+-rw-r--r--   0        0        0     4496 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_init.py
+-rw-r--r--   0        0        0    11265 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_install.py
+-rw-r--r--   0        0        0    28998 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_list.py
+-rw-r--r--   0        0        0     6324 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_lock.py
+-rw-r--r--   0        0        0     7796 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_others.py
+-rw-r--r--   0        0        0     6052 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_publish.py
+-rw-r--r--   0        0        0     3872 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_remove.py
+-rw-r--r--   0        0        0    29259 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_run.py
+-rw-r--r--   0        0        0     3599 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_self_command.py
+-rw-r--r--   0        0        0     8888 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_update.py
+-rw-r--r--   0        0        0     2942 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_use.py
+-rw-r--r--   0        0        0    10430 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/cli/test_venv.py
+-rw-r--r--   0        0        0     3079 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/conftest.py
+-rw-r--r--   0        0        0      235 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/fixtures/Pipfile
+-rw-r--r--   0        0        0        0 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0    49497 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
+-rw-r--r--   0        0        0      546 2023-05-29 04:11:03.282091 pdm-2.7.0/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
+-rw-r--r--   0        0        0   422824 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1254 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
+-rw-r--r--   0        0        0     1254 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1038 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/demo-0.0.1.tar.gz
+-rw-r--r--   0        0        0     2615 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/demo-0.0.1.zip
+-rw-r--r--   0        0        0     4595 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
+-rw-r--r--   0        0        0     5359 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    56715 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
+-rw-r--r--   0        0        0     6138 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5786 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
+-rw-r--r--   0        0        0    17978 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
+-rw-r--r--   0        0        0    24489 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0   156727 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl
+-rw-r--r--   0        0        0     1401 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0     1405 2023-05-29 04:11:03.286091 pdm-2.7.0/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl
+-rw-r--r--   0        0        0   305481 2023-05-29 04:11:03.290091 pdm-2.7.0/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
+-rw-r--r--   0        0        0   531270 2023-05-29 04:11:03.290091 pdm-2.7.0/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
+-rw-r--r--   0        0        0  1232518 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
+-rw-r--r--   0        0        0    26662 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
+-rw-r--r--   0        0        0    35301 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5312 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
+-rw-r--r--   0        0        0      326 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/index/demo.html
+-rw-r--r--   0        0        0      511 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/index/future-fstrings.html
+-rw-r--r--   0        0        0      262 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/index/pep345-legacy.html
+-rw-r--r--   0        0        0      262 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/index/wheel.html
+-rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/__init__.py
+-rw-r--r--   0        0        0       42 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-#-with-hash/demo.py
+-rw-r--r--   0        0        0      332 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-#-with-hash/setup.py
+-rw-r--r--   0        0        0       26 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-combined-extras/demo.py
+-rw-r--r--   0        0        0      462 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-combined-extras/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-failure-no-dep/demo.py
+-rw-r--r--   0        0        0      246 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-failure-no-dep/setup.py
+-rw-r--r--   0        0        0       42 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-failure/demo.py
+-rw-r--r--   0        0        0      345 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-failure/setup.py
+-rw-r--r--   0        0        0       12 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-module/LICENSE
+-rw-r--r--   0        0        0       24 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-module/README.md
+-rw-r--r--   0        0        0       14 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-module/bar_module.py
+-rw-r--r--   0        0        0       36 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-module/foo_module.py
+-rw-r--r--   0        0        0      442 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-module/pyproject.toml
+-rw-r--r--   0        0        0     3983 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
+-rw-r--r--   0        0        0      318 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
+-rw-r--r--   0        0        0       12 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package/README.md
+-rw-r--r--   0        0        0       16 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package/data_out.json
+-rw-r--r--   0        0        0       22 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package/my_package/data.json
+-rw-r--r--   0        0        0    29800 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package/pdm.lock
+-rw-r--r--   0        0        0      574 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package/requirements.ini
+-rw-r--r--   0        0        0     7521 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package/requirements.txt
+-rw-r--r--   0        0        0      211 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package/requirements_simple.txt
+-rw-r--r--   0        0        0      728 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package/setup.txt
+-rw-r--r--   0        0        0       21 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-package/single_module.py
+-rw-r--r--   0        0        0       18 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-parent-package/README.md
+-rw-r--r--   0        0        0       22 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-parent-package/package-a/foo.py
+-rw-r--r--   0        0        0      120 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-parent-package/package-a/setup.py
+-rw-r--r--   0        0        0       22 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-parent-package/package-b/bar.py
+-rw-r--r--   0        0        0      197 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-prerelease/demo.py
+-rw-r--r--   0        0        0      334 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-prerelease/setup.py
+-rw-r--r--   0        0        0       12 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-src-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-src-package/README.md
+-rw-r--r--   0        0        0       16 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-src-package/data_out.json
+-rw-r--r--   0        0        0      456 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-src-package/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-src-package/single_module.py
+-rw-r--r--   0        0        0       22 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo-src-package/src/my_package/data.json
+-rw-r--r--   0        0        0       42 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo/demo.py
+-rw-r--r--   0        0        0      332 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo/setup.py
+-rw-r--r--   0        0        0       26 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo_extras/demo.py
+-rw-r--r--   0        0        0      250 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/demo_extras/setup.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/flit-demo/README.rst
+-rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/flit-demo/doc/index.html
+-rw-r--r--   0        0        0       49 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/flit-demo/flit.py
+-rw-r--r--   0        0        0      969 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/flit-demo/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/poetry-demo/mylib.py
+-rw-r--r--   0        0        0      863 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/poetry-demo/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-hatch-static/README.md
+-rw-r--r--   0        0        0      386 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-hatch-static/pyproject.toml
+-rw-r--r--   0        0        0       11 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-monorepo/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-monorepo/core/core.py
+-rw-r--r--   0        0        0      179 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-monorepo/core/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-monorepo/package_a/alice.py
+-rw-r--r--   0        0        0      231 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-monorepo/package_b/bob.py
+-rw-r--r--   0        0        0      231 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
+-rw-r--r--   0        0        0      237 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-monorepo/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-plugin-pdm/hello.py
+-rw-r--r--   0        0        0      312 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-plugin/hello.py
+-rw-r--r--   0        0        0      168 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-plugin/setup.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-removal/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-removal/bar.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-removal/foo.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-removal/subdir/__init__.py
+-rw-r--r--   0        0        0       10 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-setuptools/AUTHORS
+-rw-r--r--   0        0        0       12 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-setuptools/README.md
+-rw-r--r--   0        0        0       22 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-setuptools/mymodule.py
+-rw-r--r--   0        0        0      398 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-setuptools/setup.cfg
+-rw-r--r--   0        0        0      308 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/projects/test-setuptools/setup.py
+-rw-r--r--   0        0        0     1525 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/pypi.json
+-rw-r--r--   0        0        0     1329 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/pyproject.toml
+-rw-r--r--   0        0        0       20 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/requirements-include.txt
+-rw-r--r--   0        0        0      502 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/fixtures/requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/models/__init__.py
+-rw-r--r--   0        0        0     3814 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/models/test_backends.py
+-rw-r--r--   0        0        0    13344 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/models/test_candidates.py
+-rw-r--r--   0        0        0     1971 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/models/test_marker.py
+-rw-r--r--   0        0        0     2679 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/models/test_requirements.py
+-rw-r--r--   0        0        0     2526 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/models/test_setup_parsing.py
+-rw-r--r--   0        0        0     3418 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/models/test_specifiers.py
+-rw-r--r--   0        0        0     2703 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/models/test_versions.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/resolver/__init__.py
+-rw-r--r--   0        0        0    11567 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/resolver/test_resolve.py
+-rw-r--r--   0        0        0     7190 2023-05-29 04:11:03.298092 pdm-2.7.0/tests/test_formats.py
+-rw-r--r--   0        0        0     7231 2023-05-29 04:11:03.302091 pdm-2.7.0/tests/test_installer.py
+-rw-r--r--   0        0        0     1829 2023-05-29 04:11:03.302091 pdm-2.7.0/tests/test_integration.py
+-rw-r--r--   0        0        0     3435 2023-05-29 04:11:03.302091 pdm-2.7.0/tests/test_plugin.py
+-rw-r--r--   0        0        0    12209 2023-05-29 04:11:03.302091 pdm-2.7.0/tests/test_project.py
+-rw-r--r--   0        0        0     1103 2023-05-29 04:11:03.302091 pdm-2.7.0/tests/test_signals.py
+-rw-r--r--   0        0        0     4419 2023-05-29 04:11:03.302091 pdm-2.7.0/tests/test_utils.py
+-rw-r--r--   0        0        0     9599 1970-01-01 00:00:00.000000 pdm-2.7.0/PKG-INFO
```

### Comparing `pdm-2.6.1/CHANGELOG.md` & `pdm-2.7.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+Release v2.7.0 (2023-05-29)
+---------------------------
+
+### Features & Improvements
+
+- When keyring is available, either by importing or by CLI, the credentials of repositories and PyPI indexes will be saved into it. [#1908](https://github.com/pdm-project/pdm/issues/1908)
+- Add support for reading metadata from simple index directly. [#1919](https://github.com/pdm-project/pdm/issues/1919)
+- Add a configuration to specify constant command arguments for every pdm invocation. [#1923](https://github.com/pdm-project/pdm/issues/1923)
+- Add ability to skip SSL verification for publish repositories via `repository.custom.verify_ssl` config option as well as new command line argument of `publish` command. [#1928](https://github.com/pdm-project/pdm/issues/1928)
+- Use lazy import to reduce the startup time of the CLI. [#1929](https://github.com/pdm-project/pdm/issues/1929)
+- Add the local plugin scripts to `PATH` env var. [#1944](https://github.com/pdm-project/pdm/issues/1944)
+
+### Bug Fixes
+
+- Don't use install cache when installing build requirements to avoid race condition. [#1869](https://github.com/pdm-project/pdm/issues/1869)
+- Fix a number of `ResourceWarning`s when running the test suite with warnings enabled. [#1915](https://github.com/pdm-project/pdm/issues/1915)
+- Fix a bug that dev-dependencies group gets updated with the optional dependencies, causing the hash mismatch. [#1916](https://github.com/pdm-project/pdm/issues/1916)
+- Fix format conversion error from Poetry when `tool.poetry.build` doesn't exist. [#1935](https://github.com/pdm-project/pdm/issues/1935)
+- Add timeout when fetching .gitignore from GitHub. [#1937](https://github.com/pdm-project/pdm/issues/1937)
+- Keep the variables in the URL credentials when exporting. [#1939](https://github.com/pdm-project/pdm/issues/1939)
+- Convert to boolean when setting verify_ssl for custom indexes. [#1945](https://github.com/pdm-project/pdm/issues/1945)
+- `pdm import` clobbers `build-system.requires` value in `pyproject.toml`. [#1948](https://github.com/pdm-project/pdm/issues/1948)
+
+### Documentation
+
+- Update publish.md to use run instead of runs to match GitHub Actions steps documentation [#1936](https://github.com/pdm-project/pdm/issues/1936)
+- Update advanced.md to use `pdm sync` instead of `pdm install --no-lock`. [#1947](https://github.com/pdm-project/pdm/issues/1947)
+
+
 Release v2.6.1 (2023-05-10)
 ---------------------------
 
 ### Bug Fixes
 
 - Fix the error when publishing using trusted publisher. [#1868](https://github.com/pdm-project/pdm/issues/1868)
 - Fix a bug that `PATH` env var isn't set correctly when running under non-isolation mode. [#1904](https://github.com/pdm-project/pdm/issues/1904)
@@ -759,15 +788,15 @@
   `pdm add --no-editable` will now override the `editable` mode of the given packages. [#1011](https://github.com/pdm-project/pdm/issues/1011)
 - Re-calculate the file hashes when running `pdm lock --refresh`. [#1019](https://github.com/pdm-project/pdm/issues/1019)
 
 ### Bug Fixes
 
 - Fix a bug that requirement with extras isn't resolved to the version as specified by the range. [#1001](https://github.com/pdm-project/pdm/issues/1001)
 - Replace the `${PROJECT_ROOT}` in the output of `pdm list`. [#1004](https://github.com/pdm-project/pdm/issues/1004)
-- Further fix the python path issue of MacOS system installed Python. [#1023](https://github.com/pdm-project/pdm/issues/1023)
+- Further fix the python path issue of macOS system installed Python. [#1023](https://github.com/pdm-project/pdm/issues/1023)
 - Fix the install path issue on Python 3.10 installed from homebrew. [#996](https://github.com/pdm-project/pdm/issues/996)
 
 ### Improved Documentation
 
 - Document how to install PDM inside a project with Pyprojectx. [#1004](https://github.com/pdm-project/pdm/issues/1004)
 
 ### Dependencies
@@ -1031,15 +1060,15 @@
 
 ### Bug Fixes
 
 - Fix the patching of sysconfig in PEP 582 initialization script. [#796](https://github.com/pdm-project/pdm/issues/796)
 
 ### Miscellany
 
-- Fix an installation failure of the bootstrap script on MacOS Catalina. [#793](https://github.com/pdm-project/pdm/issues/793)
+- Fix an installation failure of the bootstrap script on macOS Catalina. [#793](https://github.com/pdm-project/pdm/issues/793)
 - Add a basic benchmarking script. [#794](https://github.com/pdm-project/pdm/issues/794)
 
 
 Release v1.11.2 (2021-12-10)
 ----------------------------
 
 ### Bug Fixes
@@ -1346,15 +1375,15 @@
 - Add an option `-u/--unconstrained` to support unconstraining version specifiers when adding packages. [#501](https://github.com/pdm-project/pdm/issues/501)
 
 ### Bug Fixes
 
 - Fix the format of dependency arrays when a new value is appended. [#487](https://github.com/pdm-project/pdm/issues/487)
 - Allow missing email attribute for authors and maintainers. [#492](https://github.com/pdm-project/pdm/issues/492)
 - Fix a bug that editable install shouldn't require pyproject.toml to be valid. [#497](https://github.com/pdm-project/pdm/issues/497)
-- Fix a bug on MacOS that purelib and platlib paths of isolated build envs cannot be substituted correctly if the Python is a framework build. [#502](https://github.com/pdm-project/pdm/issues/502)
+- Fix a bug on macOS that purelib and platlib paths of isolated build envs cannot be substituted correctly if the Python is a framework build. [#502](https://github.com/pdm-project/pdm/issues/502)
 - Fix the version sort of candidates. [#506](https://github.com/pdm-project/pdm/issues/506)
 
 
 Release v1.6.2 (2021-05-31)
 ---------------------------
 
 No significant changes.
```

### Comparing `pdm-2.6.1/LICENSE` & `pdm-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/README.md` & `pdm-2.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 **For Windows**
 
 ```powershell
 (Invoke-WebRequest -Uri https://raw.githubusercontent.com/pdm-project/pdm/main/install-pdm.py -UseBasicParsing).Content | python -
 ```
 
 For security reasons, you should verify the checksum of `install-pdm.py`.
-The sha256 checksum is: `ce0a116987b2667231391d13dd005006433114033cac74aa18f0b2dec5538d03`
+The sha256 checksum is: `06abd94a6678636eba640529bf91b242759363c45d3620cdfabaa0053d826b30`
 
 The installer will install PDM into the user site and the location depends on the system:
 
 - `$HOME/.local/bin` for Unix
 - `%APPDATA%\Python\Scripts` on Windows
 
 You can pass additional options to the script to control how PDM is installed:
@@ -117,15 +117,15 @@
   -d DEP, --dep DEP | envvar: PDM_DEPS     Specify additional dependencies, can be given multiple times
 ```
 
 You can either pass the options after the script or set the env var value.
 
 ### Alternative Installation Methods
 
-If you are on MacOS and using `homebrew`, install it by:
+If you are on macOS and using `homebrew`, install it by:
 
 ```bash
 brew install pdm
 ```
 
 If you are on Windows and using [Scoop](https://scoop.sh/), install it by:
```

#### html2text {}

```diff
@@ -57,28 +57,28 @@
 Like Pip, PDM provides an installation script that will install PDM into an
 isolated environment. **For Linux/Mac** ```bash curl -sSL https://
 raw.githubusercontent.com/pdm-project/pdm/main/install-pdm.py | python3 - ```
 **For Windows** ```powershell (Invoke-WebRequest -Uri https://
 raw.githubusercontent.com/pdm-project/pdm/main/install-pdm.py -
 UseBasicParsing).Content | python - ``` For security reasons, you should verify
 the checksum of `install-pdm.py`. The sha256 checksum is:
-`ce0a116987b2667231391d13dd005006433114033cac74aa18f0b2dec5538d03` The
+`06abd94a6678636eba640529bf91b242759363c45d3620cdfabaa0053d826b30` The
 installer will install PDM into the user site and the location depends on the
 system: - `$HOME/.local/bin` for Unix - `%APPDATA%\Python\Scripts` on Windows
 You can pass additional options to the script to control how PDM is installed:
 ``` usage: install-pdm.py [-h] [-v VERSION] [--prerelease] [--remove] [-p PATH]
 [-d DEP] optional arguments: -h, --help show this help message and exit -
 v VERSION, --version VERSION | envvar: PDM_VERSION Specify the version to be
 installed, or HEAD to install from the main branch --prerelease | envvar:
 PDM_PRERELEASE Allow prereleases to be installed --remove | envvar: PDM_REMOVE
 Remove the PDM installation -p PATH, --path PATH | envvar: PDM_HOME Specify the
 location to install PDM -d DEP, --dep DEP | envvar: PDM_DEPS Specify additional
 dependencies, can be given multiple times ``` You can either pass the options
 after the script or set the env var value. ### Alternative Installation Methods
-If you are on MacOS and using `homebrew`, install it by: ```bash brew install
+If you are on macOS and using `homebrew`, install it by: ```bash brew install
 pdm ``` If you are on Windows and using [Scoop](https://scoop.sh/), install it
 by: ``` scoop bucket add frostming https://github.com/frostming/scoop-
 frostming.git scoop install pdm ``` Otherwise, it is recommended to install
 `pdm` in an isolated environment with `pipx`: ```bash pipx install pdm ``` Or
 you can install it under a user site: ```bash pip install --user pdm ``` With
 [asdf-vm](https://asdf-vm.com/) ```bash asdf plugin add pdm asdf install pdm
 latest ``` ## Quickstart **Initialize a new PDM project** ```bash pdm init ```
```

### Comparing `pdm-2.6.1/pyproject.toml` & `pdm-2.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,16 @@
     "unearth>=0.9.0",
     "findpython>=0.2.2",
     "tomlkit>=0.11.1,<1",
     "shellingham>=1.3.2",
     "python-dotenv>=0.15",
     "resolvelib>=1.0.1",
     "installer<0.8,>=0.7",
-    "cachecontrol[filecache]>=0.12.11",
+    "cacheyou[filecache]",
     "tomli>=1.1.0; python_version < \"3.11\"",
-    "typing-extensions; python_version < \"3.8\"",
     "importlib-metadata>=3.6; python_version < \"3.10\"",
 ]
 readme = "README.md"
 keywords = [
     "packaging",
     "dependency",
     "workflow",
@@ -38,15 +37,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-version = "2.6.1"
+version = "2.7.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://pdm.fming.dev"
 Repository = "https://github.com/pdm-project/pdm"
```

### Comparing `pdm-2.6.1/src/pdm/_types.py` & `pdm-2.7.0/src/pdm/_types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,64 @@
 from __future__ import annotations
 
-import dataclasses
-from typing import Any, Dict, List, NamedTuple, Tuple, TypeVar, Union
+import dataclasses as dc
+from typing import TYPE_CHECKING, Any, Dict, List, NamedTuple, Tuple, TypeVar, Union
 
-from pdm.compat import Protocol
+if TYPE_CHECKING:
+    from typing import Protocol
 
 
-@dataclasses.dataclass
-class RepositoryConfig:
+@dc.dataclass
+class _RepositoryConfig:
+    """Private dataclass to be subclassed"""
+
+    config_prefix: str
+    name: str
+
     url: str | None = None
     username: str | None = None
-    password: str | None = None
+    _password: str | None = dc.field(default=None, repr=False)
     verify_ssl: bool | None = None
     type: str | None = None
     ca_certs: str | None = None
 
-    config_prefix: str | None = None
-    name: str | None = None
+
+class RepositoryConfig(_RepositoryConfig):
+    def __init__(self, *args: Any, password: str | None = None, **kwargs: Any) -> None:
+        kwargs["_password"] = password
+        super().__init__(*args, **kwargs)
+
+    @property
+    def password(self) -> str | None:
+        if self._password is None:
+            from pdm.models.auth import keyring
+
+            service = f"pdm-{self.config_prefix}-{self.name}"
+            result = keyring.get_auth_info(service, self.username)
+            if result is not None:
+                self._password = result[1]
+        return self._password
+
+    @password.setter
+    def password(self, value: str) -> None:
+        self._password = value
 
     def passive_update(self, other: RepositoryConfig | None = None, **kwargs: Any) -> None:
         """An update method that prefers the existing value over the new one."""
         if other is not None:
             for k in other.__dataclass_fields__:
                 v = getattr(other, k)
                 if getattr(self, k) is None and v is not None:
                     setattr(self, k, v)
         for k, v in kwargs.items():
             if getattr(self, k) is None and v is not None:
                 setattr(self, k, v)
 
     def __rich__(self) -> str:
-        config_prefix = f"{self.config_prefix}." if self.config_prefix is not None else ""
+        config_prefix = f"{self.config_prefix}.{self.name}." if self.name else f"{self.config_prefix}."
         lines: list[str] = []
         if self.url:
             lines.append(f"[primary]{config_prefix}url[/] = {self.url}")
         if self.username:
             lines.append(f"[primary]{config_prefix}username[/] = {self.username}")
         if self.password:
             lines.append(f"[primary]{config_prefix}password[/] = [i]<hidden>[/]")
@@ -53,32 +77,31 @@
 
 class Package(NamedTuple):
     name: str
     version: str
     summary: str
 
 
-class Comparable(Protocol):
-    def __lt__(self, __other: Any) -> bool:
-        ...
-
-
-SpinnerT = TypeVar("SpinnerT", bound="Spinner")
+SearchResult = List[Package]
 
 
-class Spinner(Protocol):
-    def update(self, text: str) -> None:
-        ...
+if TYPE_CHECKING:
 
-    def __enter__(self: SpinnerT) -> SpinnerT:
-        ...
+    class Comparable(Protocol):
+        def __lt__(self, __other: Any) -> bool:
+            ...
 
-    def __exit__(self, *args: Any) -> None:
-        ...
+    SpinnerT = TypeVar("SpinnerT", bound="Spinner")
 
+    class Spinner(Protocol):
+        def update(self, text: str) -> None:
+            ...
 
-class RichProtocol(Protocol):
-    def __rich__(self) -> str:
-        ...
+        def __enter__(self: SpinnerT) -> SpinnerT:
+            ...
 
+        def __exit__(self, *args: Any) -> None:
+            ...
 
-SearchResult = List[Package]
+    class RichProtocol(Protocol):
+        def __rich__(self) -> str:
+            ...
```

### Comparing `pdm-2.6.1/src/pdm/builders/base.py` & `pdm-2.7.0/src/pdm/builders/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/builders/editable.py` & `pdm-2.7.0/src/pdm/builders/editable.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/builders/sdist.py` & `pdm-2.7.0/src/pdm/builders/sdist.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/builders/wheel.py` & `pdm-2.7.0/src/pdm/builders/wheel.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/actions.py` & `pdm-2.7.0/src/pdm/cli/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from __future__ import annotations
 
 import contextlib
 import datetime
 import hashlib
 import json
 import os
-import shutil
 import sys
 import textwrap
 import warnings
 from argparse import Namespace
 from collections import defaultdict
 from itertools import chain
-from pathlib import Path
-from typing import Collection, Iterable, Mapping, cast
+from typing import Collection, Iterable, cast
 
 import tomlkit
 from resolvelib.reporters import BaseReporter
 from resolvelib.resolvers import ResolutionImpossible, ResolutionTooDeep, Resolver
 from tomlkit.items import Array
 
 from pdm import termui
@@ -32,18 +30,15 @@
     get_pep582_path,
     merge_dictionary,
     save_version_specifiers,
     set_env_in_reg,
 )
 from pdm.environments import BareEnvironment, PythonLocalEnvironment
 from pdm.exceptions import NoPythonVersion, PdmUsageError, ProjectError
-from pdm.formats import FORMATS
-from pdm.formats.base import array_of_inline_tables, make_array, make_inline_table
-from pdm.models.backends import DEFAULT_BACKEND, BuildBackend
-from pdm.models.caches import JSONFileCache
+from pdm.models.backends import DEFAULT_BACKEND
 from pdm.models.candidates import Candidate
 from pdm.models.python import PythonInfo
 from pdm.models.requirements import Requirement, parse_requirement, strip_extras
 from pdm.models.specifiers import get_specifier
 from pdm.project import Project
 from pdm.resolver import resolve
 from pdm.utils import cd, normalize_name
@@ -461,131 +456,29 @@
             no_self=no_self,
             dry_run=dry_run,
             fail_fast=fail_fast,
             hooks=hooks,
         )
 
 
-def do_build(
-    project: Project,
-    sdist: bool = True,
-    wheel: bool = True,
-    dest: str = "dist",
-    clean: bool = True,
-    config_settings: Mapping[str, str] | None = None,
-    hooks: HookManager | None = None,
-) -> None:
-    """Build artifacts for distribution."""
-    from pdm.builders import SdistBuilder, WheelBuilder
-
-    hooks = hooks or HookManager(project)
-
-    if project.is_global:
-        raise ProjectError("Not allowed to build based on the global project.")
-    if not wheel and not sdist:
-        project.core.ui.echo("All artifacts are disabled, nothing to do.", err=True)
-        return
-    if not os.path.isabs(dest):
-        dest = project.root.joinpath(dest).as_posix()
-    if clean:
-        shutil.rmtree(dest, ignore_errors=True)
-    if not os.path.exists(dest):
-        os.makedirs(dest, exist_ok=True)
-    hooks.try_emit("pre_build", dest=dest, config_settings=config_settings)
-    artifacts: list[str] = []
-    with project.core.ui.logging("build"):
-        if sdist:
-            project.core.ui.echo("Building sdist...")
-            loc = SdistBuilder(project.root, project.environment).build(dest, config_settings)
-            project.core.ui.echo(f"Built sdist at {loc}")
-            artifacts.append(loc)
-        if wheel:
-            project.core.ui.echo("Building wheel...")
-            loc = WheelBuilder(project.root, project.environment).build(dest, config_settings)
-            project.core.ui.echo(f"Built wheel at {loc}")
-            artifacts.append(loc)
-    hooks.try_emit("post_build", artifacts=artifacts, config_settings=config_settings)
-
-
-def do_init(
-    project: Project,
-    name: str = "",
-    version: str = "",
-    description: str = "",
-    license: str = "MIT",
-    author: str = "",
-    email: str = "",
-    python_requires: str = "",
-    build_backend: type[BuildBackend] | None = None,
-    hooks: HookManager | None = None,
-) -> None:
-    """Bootstrap the project and create a pyproject.toml"""
-    hooks = hooks or HookManager(project)
-    data = {
-        "project": {
-            "name": name,
-            "version": version,
-            "description": description,
-            "authors": array_of_inline_tables([{"name": author, "email": email}]),
-            "license": make_inline_table({"text": license}),
-            "dependencies": make_array([], True),
-        },
-    }
-    if build_backend is not None:
-        data["build-system"] = build_backend.build_system()
-    if python_requires and python_requires != "*":
-        data["project"]["requires-python"] = python_requires
-    if name and version:
-        readme = next(project.root.glob("README*"), None)
-        if readme is None:
-            readme = project.root.joinpath("README.md")
-            readme.write_text(f"# {name}\n\n{description}\n", encoding="utf-8")
-        data["project"]["readme"] = readme.name
-    get_specifier(python_requires)
-    project.pyproject._data.update(data)
-    project.pyproject.write()
-    _write_gitignore(project.root.joinpath(".gitignore"))
-    hooks.try_emit("post_init")
-
-
-def _write_gitignore(path: Path) -> None:
-    import requests
-
-    url = "https://raw.githubusercontent.com/github/gitignore/master/Python.gitignore"
-    if not path.exists():
-        try:
-            resp = requests.get(url)
-            resp.raise_for_status()
-        except requests.exceptions.RequestException:
-            content = "\n".join(["build/", "dist/", "*.egg-info/", "__pycache__/", "*.py[cod]"]) + "\n"
-        else:
-            content = resp.text
-        content += ".pdm-python\n"
-    else:
-        content = path.read_text(encoding="utf-8")
-        if ".pdm-python" in content:
-            return
-        content += ".pdm-python\n"
-    path.write_text(content, encoding="utf-8")
-
-
 def do_use(
     project: Project,
     python: str = "",
     first: bool = False,
     ignore_remembered: bool = False,
     ignore_requires_python: bool = False,
     save: bool = True,
     venv: str | None = None,
     hooks: HookManager | None = None,
 ) -> PythonInfo:
     """Use the specified python version and save in project config.
     The python can be a version string or interpreter path.
     """
     from pdm.cli.commands.venv.utils import get_venv_with_name
+    from pdm.models.caches import JSONFileCache
 
     def version_matcher(py_version: PythonInfo) -> bool:
         return py_version.valid and (
             ignore_requires_python or project.python_requires.contains(str(py_version.version), True)
         )
 
     hooks = hooks or HookManager(project)
@@ -625,22 +518,22 @@
             raise NoPythonVersion(f"No Python interpreter matching [success]{python}[/] is found.")
         if not matching_interpreters:
             project.core.ui.echo("Interpreters found but not matching:", err=True)
             for py in found_interpreters:
                 info = py.identifier if py.valid else "Invalid"
                 project.core.ui.echo(f"  - {py.path} ({info})", err=True)
             raise NoPythonVersion(
-                f"No python is found meeting the requirement [success]python {str(project.python_requires)}[/]"
+                f"No python is found meeting the requirement [success]python {project.python_requires!s}[/]"
             )
         if first or len(matching_interpreters) == 1:
             selected_python = matching_interpreters[0]
         else:
             project.core.ui.echo("Please enter the Python interpreter to use")
             for i, py_version in enumerate(matching_interpreters):
-                project.core.ui.echo(f"{i}. [success]{str(py_version.path)}[/] ({py_version.identifier})")
+                project.core.ui.echo(f"{i}. [success]{py_version.path!s}[/] ({py_version.identifier})")
             selection = termui.ask(
                 "Please select",
                 default="0",
                 prompt_type=int,
                 choices=[str(i) for i in range(len(matching_interpreters))],
                 show_choices=False,
             )
@@ -649,15 +542,15 @@
             use_cache.set(python, selected_python.path.as_posix())
 
     if not save:
         return selected_python
     saved_python = project._saved_python
     old_python = PythonInfo.from_path(saved_python) if saved_python else None
     project.core.ui.echo(
-        f"Using Python interpreter: [success]{str(selected_python.path)}[/] ({selected_python.identifier})"
+        f"Using Python interpreter: [success]{selected_python.path!s}[/] ({selected_python.identifier})"
     )
     project.python = selected_python
     if project.environment.is_local:
         project.core.ui.echo(
             "Using __pypackages__ because non-venv Python is used.",
             style="primary",
             err=True,
@@ -682,14 +575,16 @@
     """Import project metadata from given file.
 
     :param project: the project instance
     :param filename: the file name
     :param format: the file format, or guess if not given.
     :param options: other options parsed to the CLI.
     """
+    from pdm.formats import FORMATS
+
     if not format:
         for key in FORMATS:
             if FORMATS[key].check_fingerprint(project, filename):
                 break
         else:
             raise PdmUsageError(
                 "Can't derive the file format automatically, please specify it via '-f/--format' option."
@@ -711,15 +606,15 @@
     if "project" not in pyproject:
         pyproject.add("project", tomlkit.table())
         pyproject["project"].add(tomlkit.comment("PEP 621 project metadata"))
         pyproject["project"].add(tomlkit.comment("See https://www.python.org/dev/peps/pep-0621/"))
 
     merge_dictionary(pyproject["project"], project_data)
     merge_dictionary(pyproject["tool"]["pdm"], settings)
-    pyproject["build-system"] = DEFAULT_BACKEND.build_system()
+    pyproject.setdefault("build-system", DEFAULT_BACKEND.build_system())
 
     if "requires-python" not in pyproject["project"]:
         python_version = f"{project.python.major}.{project.python.minor}"
         pyproject["project"]["requires-python"] = f">={python_version}"
         project.core.ui.echo(
             "The project's [primary]requires-python[/] has been set to [primary]>="
             f"{python_version}[/]. You can change it later if necessary."
```

### Comparing `pdm-2.6.1/src/pdm/cli/commands/add.py` & `pdm-2.7.0/src/pdm/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/commands/base.py` & `pdm-2.7.0/src/pdm/cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/commands/build.py` & `pdm-2.7.0/src/pdm/cli/commands/update.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,77 @@
 import argparse
 
 from pdm.cli import actions
 from pdm.cli.commands.base import BaseCommand
+from pdm.cli.filters import GroupSelection
 from pdm.cli.hooks import HookManager
 from pdm.cli.options import (
-    no_isolation_option,
-    project_option,
+    groups_group,
+    install_group,
+    lockfile_option,
+    prerelease_option,
+    save_strategy_group,
     skip_option,
-    verbose_option,
+    unconstrained_option,
+    update_strategy_group,
+    venv_option,
 )
 from pdm.project import Project
 
 
 class Command(BaseCommand):
-    """Build artifacts for distribution"""
+    """Update package(s) in pyproject.toml"""
 
-    arguments = [verbose_option, project_option, no_isolation_option, skip_option]
+    arguments = [
+        *BaseCommand.arguments,
+        groups_group,
+        install_group,
+        lockfile_option,
+        save_strategy_group,
+        update_strategy_group,
+        prerelease_option,
+        unconstrained_option,
+        skip_option,
+        venv_option,
+    ]
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
-            "--no-sdist",
-            dest="sdist",
-            default=True,
-            action="store_false",
-            help="Don't build source tarballs",
+            "-t",
+            "--top",
+            action="store_true",
+            help="Only update those listed in pyproject.toml",
         )
         parser.add_argument(
-            "--no-wheel",
-            dest="wheel",
-            default=True,
-            action="store_false",
-            help="Don't build wheels",
+            "--dry-run",
+            "--outdated",
+            action="store_true",
+            dest="dry_run",
+            help="Show the difference only without modifying the lockfile content",
         )
-        parser.add_argument("-d", "--dest", default="dist", help="Target directory to put artifacts")
         parser.add_argument(
-            "--no-clean",
-            dest="clean",
+            "--no-sync",
+            dest="sync",
             default=True,
             action="store_false",
-            help="Do not clean the target directory",
-        )
-        parser.add_argument(
-            "--config-setting",
-            "-C",
-            action="append",
-            help="Pass options to the backend. options with a value must be "
-            'specified after "=": `--config-setting=--opt(=value)` '
-            "or `-C--opt(=value)`",
+            help="Only update lock file but do not sync packages",
         )
+        parser.add_argument("packages", nargs="*", help="If packages are given, only update them")
+        parser.set_defaults(dev=None)
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
-        config_settings = None
-        if options.config_setting:
-            config_settings = {}
-            for item in options.config_setting:
-                name, _, value = item.partition("=")
-                if name not in config_settings:
-                    config_settings[name] = value
-                else:
-                    if not isinstance(config_settings[name], list):
-                        config_settings[name] = [config_settings[name]]
-                    config_settings[name].append(value)
-        actions.do_build(
+        actions.do_update(
             project,
-            sdist=options.sdist,
-            wheel=options.wheel,
-            dest=options.dest,
-            clean=options.clean,
-            config_settings=config_settings,
+            selection=GroupSelection.from_options(project, options),
+            save=options.save_strategy or project.config["strategy.save"],
+            strategy=options.update_strategy or project.config["strategy.update"],
+            unconstrained=options.unconstrained,
+            top=options.top,
+            dry_run=options.dry_run,
+            packages=options.packages,
+            sync=options.sync,
+            no_editable=options.no_editable,
+            no_self=options.no_self,
+            prerelease=options.prerelease,
+            fail_fast=options.fail_fast,
             hooks=HookManager(project, options.skip),
         )
```

### Comparing `pdm-2.6.1/src/pdm/cli/commands/cache.py` & `pdm-2.7.0/src/pdm/cli/commands/cache.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/commands/completion.py` & `pdm-2.7.0/src/pdm/cli/commands/completion.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/commands/config.py` & `pdm-2.7.0/src/pdm/cli/commands/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 from typing import Any, Mapping
 
 from pdm import termui
 from pdm._types import RepositoryConfig
 from pdm.cli.commands.base import BaseCommand
 from pdm.project import Project
-from pdm.project.config import DEFAULT_REPOSITORIES, REPOSITORY, Config
+from pdm.project.config import DEFAULT_REPOSITORIES, REPOSITORY, SOURCE, Config
 
 
 class Command(BaseCommand):
     """Display the current configuration"""
 
     ui: termui.UI
 
@@ -71,33 +71,26 @@
                 if canonical_key in supersedes:
                     superseded = True
                 deprecated = f"[error](deprecating: {key})[/]"
             elif key not in Config._config_map and not (key.startswith("pypi.") or key.startswith(REPOSITORY)):
                 continue
             extra_style = "dim" if superseded else None
             if canonical_key not in Config._config_map:
-                if key.startswith("pypi."):
-                    index = key.split(".")[1]
+                prefix, name = key.split(".", 1)
+                if prefix in (SOURCE, REPOSITORY):
+                    title = "non-default PyPI index" if prefix == SOURCE else "custom repository"
                     self.ui.echo(
-                        f"[warning]# Configuration of non-default Pypi index `{index}`",
+                        f"[warning]# Configuration of {title} `{name}`",
                         style=extra_style,
                         verbosity=termui.Verbosity.DETAIL,
                     )
-                    self.ui.echo(RepositoryConfig(**config[key], config_prefix=key))
-                elif key.startswith(REPOSITORY):
-                    for item in config[key]:
-                        self.ui.echo(
-                            f"[warning]# Configuration of custom repository `{item}`",
-                            style=extra_style,
-                            verbosity=termui.Verbosity.DETAIL,
-                        )
-                        repository = dict(config[key][item])
-                        if "url" not in repository and item in DEFAULT_REPOSITORIES:
-                            repository["url"] = DEFAULT_REPOSITORIES[item]
-                        self.ui.echo(RepositoryConfig(**repository, config_prefix=f"{key}.{item}"))
+                    repository = RepositoryConfig(**config[key], config_prefix=prefix, name=name)
+                    if not repository.url and name in DEFAULT_REPOSITORIES:
+                        repository.url = DEFAULT_REPOSITORIES[name]
+                    self.ui.echo(repository)
                 continue
             config_item = Config._config_map[canonical_key]
             self.ui.echo(
                 f"[warning]# {config_item.description}",
                 style=extra_style,
                 verbosity=termui.Verbosity.DETAIL,
             )
```

### Comparing `pdm-2.6.1/src/pdm/cli/commands/export.py` & `pdm-2.7.0/src/pdm/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/commands/fix/__init__.py` & `pdm-2.7.0/src/pdm/cli/commands/fix/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/commands/fix/fixers.py` & `pdm-2.7.0/src/pdm/cli/commands/fix/fixers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/commands/import_cmd.py` & `pdm-2.7.0/src/pdm/cli/commands/import_cmd.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/commands/info.py` & `pdm-2.7.0/src/pdm/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/commands/init.py` & `pdm-2.7.0/src/pdm/cli/commands/publish/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,144 +1,176 @@
 from __future__ import annotations
 
 import argparse
+import os
+from typing import TYPE_CHECKING
 
-from pdm import termui
-from pdm.cli import actions
+from rich.progress import (
+    BarColumn,
+    DownloadColumn,
+    TimeRemainingColumn,
+    TransferSpeedColumn,
+)
+
+from pdm.cli.commands import build
 from pdm.cli.commands.base import BaseCommand
+from pdm.cli.commands.publish.package import PackageFile
+from pdm.cli.commands.publish.repository import Repository
 from pdm.cli.hooks import HookManager
-from pdm.cli.options import skip_option
-from pdm.models.backends import _BACKENDS, DEFAULT_BACKEND, BuildBackend, get_backend
-from pdm.models.python import PythonInfo
-from pdm.models.venv import get_venv_python
-from pdm.project import Project
-from pdm.utils import get_user_email_from_git
+from pdm.cli.options import project_option, skip_option, verbose_option
+from pdm.exceptions import PdmUsageError, PublishError
+from pdm.termui import logger
+
+if TYPE_CHECKING:
+    from requests import Response
+
+    from pdm.project import Project
 
 
 class Command(BaseCommand):
-    """Initialize a pyproject.toml for PDM"""
+    """Build and publish the project to PyPI"""
 
-    def __init__(self, parser: argparse.ArgumentParser) -> None:
-        super().__init__(parser)
-        self.interactive = True
-
-    def set_interactive(self, value: bool) -> None:
-        self.interactive = value
-
-    def ask(self, question: str, default: str) -> str:
-        if not self.interactive:
-            return default
-        return termui.ask(question, default=default)
+    arguments = [verbose_option, project_option, skip_option]
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
-        skip_option.add_to_parser(parser)
         parser.add_argument(
-            "-n",
-            "--non-interactive",
+            "-r",
+            "--repository",
+            help="The repository name or url to publish the package to [env var: PDM_PUBLISH_REPO]",
+        )
+        parser.add_argument(
+            "-u",
+            "--username",
+            help="The username to access the repository [env var: PDM_PUBLISH_USERNAME]",
+        )
+        parser.add_argument(
+            "-P",
+            "--password",
+            help="The password to access the repository [env var: PDM_PUBLISH_PASSWORD]",
+        )
+        parser.add_argument(
+            "-S",
+            "--sign",
             action="store_true",
-            help="Don't ask questions but use default values",
+            help="Upload the package with PGP signature",
+        )
+        parser.add_argument(
+            "-i",
+            "--identity",
+            help="GPG identity used to sign files.",
+        )
+        parser.add_argument(
+            "-c",
+            "--comment",
+            help="The comment to include with the distribution file.",
+        )
+        parser.add_argument(
+            "--no-build",
+            action="store_false",
+            dest="build",
+            help="Don't build the package before publishing",
         )
-        parser.add_argument("--python", help="Specify the Python version/path to use")
-        parser.add_argument("--backend", choices=list(_BACKENDS), help="Specify the build backend")
-        parser.add_argument("--lib", action="store_true", help="Create a library project")
-        parser.set_defaults(search_parent=False)
+        group = parser.add_mutually_exclusive_group()
+        group.add_argument(
+            "--no-very-ssl", action="store_false", dest="verify_ssl", help="Disable SSL verification", default=None
+        )
+        group.add_argument(
+            "--ca-certs",
+            dest="ca_certs",
+            help="The path to a PEM-encoded Certificate Authority bundle to use"
+            " for publish server validation [env var: PDM_PUBLISH_CA_CERTS]",
+        )
+
+    @staticmethod
+    def _make_package(filename: str, signatures: dict[str, str], options: argparse.Namespace) -> PackageFile:
+        p = PackageFile.from_filename(filename, options.comment)
+        if p.base_filename in signatures:
+            p.add_gpg_signature(signatures[p.base_filename], p.base_filename + ".asc")
+        elif options.sign:
+            p.sign(options.identity)
+        return p
+
+    @staticmethod
+    def _check_response(response: Response) -> None:
+        import requests
+
+        message = ""
+        if response.status_code == 410 and "pypi.python.org" in response.url:
+            message = (
+                "Uploading to these sites is deprecated. "
+                "Try using https://upload.pypi.org/legacy/ "
+                "(or https://test.pypi.org/legacy/) instead."
+            )
+        elif response.status_code == 405 and "pypi.org" in response.url:
+            message = "It appears you're trying to upload to pypi.org but have an invalid URL."
+        else:
+            try:
+                response.raise_for_status()
+            except requests.HTTPError as err:
+                message = str(err)
+        if message:
+            raise PublishError(message)
+
+    @staticmethod
+    def get_repository(project: Project, options: argparse.Namespace) -> Repository:
+        repository = options.repository or os.getenv("PDM_PUBLISH_REPO", "pypi")
+        username = options.username or os.getenv("PDM_PUBLISH_USERNAME")
+        password = options.password or os.getenv("PDM_PUBLISH_PASSWORD")
+        ca_certs = options.ca_certs or os.getenv("PDM_PUBLISH_CA_CERTS")
+
+        config = project.global_config.get_repository_config(repository, "repository")
+        if config is None:
+            raise PdmUsageError(f"Missing repository config of {repository}")
+        assert config.url is not None
+        if username is not None:
+            config.username = username
+        if password is not None:
+            config.password = password
+        if ca_certs is not None:
+            config.ca_certs = ca_certs
+        if options.verify_ssl is False:
+            config.verify_ssl = options.verify_ssl
+        return Repository(project, config.url, config.username, config.password, config.ca_certs, config.verify_ssl)
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         hooks = HookManager(project, options.skip)
-        if project.pyproject.exists():
-            project.core.ui.echo("pyproject.toml already exists, update it now.", style="primary")
-        else:
-            project.core.ui.echo("Creating a pyproject.toml for PDM...", style="primary")
-        self.set_interactive(not options.non_interactive)
 
-        if self.interactive:
-            python = actions.do_use(
-                project,
-                options.python or "",
-                first=bool(options.python),
-                ignore_remembered=True,
-                ignore_requires_python=True,
-                hooks=hooks,
-            )
-        else:
-            python = actions.do_use(
-                project,
-                options.python or "3",
-                first=True,
-                ignore_remembered=True,
-                ignore_requires_python=True,
-                save=False,
-                hooks=hooks,
-            )
-        if project.config["python.use_venv"] and python.get_venv() is None:
-            if not self.interactive or termui.confirm(
-                f"Would you like to create a virtualenv with [success]{python.executable}[/]?",
-                default=True,
-            ):
-                try:
-                    path = project._create_virtualenv()
-                    python = project.python = PythonInfo.from_path(get_venv_python(path))
-                except Exception as e:  # pragma: no cover
-                    project.core.ui.echo(
-                        f"Error occurred when creating virtualenv: {e}\nPlease fix it and create later.",
-                        style="error",
-                        err=True,
-                    )
-        if python.get_venv() is None:
-            project.core.ui.echo(
-                "You are using the PEP 582 mode, no virtualenv is created.\n"
-                "For more info, please visit https://peps.python.org/pep-0582/",
-                style="success",
-            )
-        is_library = options.lib
-        if not is_library and self.interactive:
-            is_library = termui.confirm(
-                "Is the project a library that is installable?\n"
-                "If yes, we will need to ask a few more questions to include "
-                "the project name and build backend"
+        hooks.try_emit("pre_publish")
+
+        if options.build:
+            build.Command.do_build(project, hooks=hooks)
+
+        package_files = [str(p) for p in project.root.joinpath("dist").iterdir() if not p.name.endswith(".asc")]
+        signatures = {p.stem: str(p) for p in project.root.joinpath("dist").iterdir() if p.name.endswith(".asc")}
+
+        repository = self.get_repository(project, options)
+        uploaded: list[PackageFile] = []
+        with project.core.ui.make_progress(
+            " [progress.percentage]{task.percentage:>3.0f}%",
+            BarColumn(),
+            DownloadColumn(),
+            "•",
+            TimeRemainingColumn(
+                compact=True,
+                elapsed_when_finished=True,
+            ),
+            "•",
+            TransferSpeedColumn(),
+        ) as progress, project.core.ui.logging("publish"):
+            packages = sorted(
+                (self._make_package(p, signatures, options) for p in package_files),
+                # Upload wheels first if they exist.
+                key=lambda p: not p.base_filename.endswith(".whl"),
             )
-        build_backend: type[BuildBackend] | None = None
-        if is_library:
-            name = self.ask("Project name", project.root.name)
-            version = self.ask("Project version", "0.1.0")
-            description = self.ask("Project description", "")
-            if options.backend:
-                build_backend = get_backend(options.backend)
-            elif self.interactive:
-                all_backends = list(_BACKENDS)
-                project.core.ui.echo("Which build backend to use?")
-                for i, backend in enumerate(all_backends):
-                    project.core.ui.echo(f"{i}. [success]{backend}[/]")
-                selected_backend = termui.ask(
-                    "Please select",
-                    prompt_type=int,
-                    choices=[str(i) for i in range(len(all_backends))],
-                    show_choices=False,
-                    default=0,
-                )
-                build_backend = get_backend(all_backends[int(selected_backend)])
-            else:
-                build_backend = DEFAULT_BACKEND
-        else:
-            name, version, description = "", "", ""
-        license = self.ask("License(SPDX name)", "MIT")
+            for package in packages:
+                resp = repository.upload(package, progress)
+                logger.debug("Response from %s:\n%s %s", resp.url, resp.status_code, resp.reason)
+                self._check_response(resp)
+                uploaded.append(package)
+
+        release_urls = repository.get_release_urls(uploaded)
+        if release_urls:
+            project.core.ui.echo("\n[success]View at:")
+            for url in release_urls:
+                project.core.ui.echo(url)
 
-        git_user, git_email = get_user_email_from_git()
-        author = self.ask("Author name", git_user)
-        email = self.ask("Author email", git_email)
-        python_version = f"{python.major}.{python.minor}"
-        python_requires = self.ask("Python requires('*' to allow any)", f">={python_version}")
-
-        actions.do_init(
-            project,
-            name=name,
-            version=version,
-            description=description,
-            license=license,
-            author=author,
-            email=email,
-            python_requires=python_requires,
-            build_backend=build_backend,
-            hooks=hooks,
-        )
-        if self.interactive:
-            actions.ask_for_import(project)
+        hooks.try_emit("post_publish")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pdm-2.6.1/src/pdm/cli/commands/install.py` & `pdm-2.7.0/src/pdm/cli/commands/install.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,17 @@
         ]
         if not plugins:
             return
         plugin_root = project.root / ".pdm-plugins"
         environment = PythonEnvironment(project, python=sys.executable, prefix=str(plugin_root))
         with project.core.ui.open_spinner("[success]Installing plugins...[/]"):
             with project.core.ui.logging("install-plugins"):
-                install_requirements(plugins, environment, clean=True)
+                install_requirements(
+                    plugins, environment, clean=True, use_install_cache=project.config["install.cache"]
+                )
             if not plugin_root.joinpath(".gitignore").exists():
                 plugin_root.joinpath(".gitignore").write_text("*\n")
         project.core.ui.echo("Plugins are installed successfully into [primary].pdm-plugins[/].")
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         if not project.pyproject.is_valid and termui.is_interactive():
             actions.ask_for_import(project)
```

### Comparing `pdm-2.6.1/src/pdm/cli/commands/list.py` & `pdm-2.7.0/src/pdm/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/commands/lock.py` & `pdm-2.7.0/src/pdm/cli/commands/lock.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/commands/publish/__init__.py` & `pdm-2.7.0/tests/cli/test_publish.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,164 +1,159 @@
-from __future__ import annotations
-
-import argparse
 import os
+from argparse import Namespace
 
-import requests
-from rich.progress import (
-    BarColumn,
-    DownloadColumn,
-    TimeRemainingColumn,
-    TransferSpeedColumn,
-)
+import pytest
 
-from pdm.cli import actions
-from pdm.cli.commands.base import BaseCommand
+from pdm.cli.commands.publish import Command as PublishCommand
 from pdm.cli.commands.publish.package import PackageFile
 from pdm.cli.commands.publish.repository import Repository
-from pdm.cli.hooks import HookManager
-from pdm.cli.options import project_option, skip_option, verbose_option
-from pdm.exceptions import PdmUsageError, PublishError
-from pdm.project import Project
-from pdm.termui import logger
-
-
-class Command(BaseCommand):
-    """Build and publish the project to PyPI"""
-
-    arguments = [verbose_option, project_option, skip_option]
-
-    def add_arguments(self, parser: argparse.ArgumentParser) -> None:
-        parser.add_argument(
-            "-r",
-            "--repository",
-            help="The repository name or url to publish the package to [env var: PDM_PUBLISH_REPO]",
-        )
-        parser.add_argument(
-            "-u",
-            "--username",
-            help="The username to access the repository [env var: PDM_PUBLISH_USERNAME]",
-        )
-        parser.add_argument(
-            "-P",
-            "--password",
-            help="The password to access the repository [env var: PDM_PUBLISH_PASSWORD]",
-        )
-        parser.add_argument(
-            "-S",
-            "--sign",
-            action="store_true",
-            help="Upload the package with PGP signature",
-        )
-        parser.add_argument(
-            "-i",
-            "--identity",
-            help="GPG identity used to sign files.",
-        )
-        parser.add_argument(
-            "-c",
-            "--comment",
-            help="The comment to include with the distribution file.",
-        )
-        parser.add_argument(
-            "--no-build",
-            action="store_false",
-            dest="build",
-            help="Don't build the package before publishing",
-        )
-        parser.add_argument(
-            "--ca-certs",
-            dest="ca_certs",
-            help="The path to a PEM-encoded Certificate Authority bundle to use"
-            " for publish server validation [env var: PDM_PUBLISH_CA_CERTS]",
-        )
+from tests import FIXTURES
+
+pytestmark = pytest.mark.usefixtures("mock_run_gpg")
 
-    @staticmethod
-    def _make_package(filename: str, signatures: dict[str, str], options: argparse.Namespace) -> PackageFile:
-        p = PackageFile.from_filename(filename, options.comment)
-        if p.base_filename in signatures:
-            p.add_gpg_signature(signatures[p.base_filename], p.base_filename + ".asc")
-        elif options.sign:
-            p.sign(options.identity)
-        return p
-
-    @staticmethod
-    def _check_response(response: requests.Response) -> None:
-        message = ""
-        if response.status_code == 410 and "pypi.python.org" in response.url:
-            message = (
-                "Uploading to these sites is deprecated. "
-                "Try using https://upload.pypi.org/legacy/ "
-                "(or https://test.pypi.org/legacy/) instead."
-            )
-        elif response.status_code == 405 and "pypi.org" in response.url:
-            message = "It appears you're trying to upload to pypi.org but have an invalid URL."
-        else:
-            try:
-                response.raise_for_status()
-            except requests.HTTPError as err:
-                message = str(err)
-        if message:
-            raise PublishError(message)
-
-    @staticmethod
-    def get_repository(project: Project, options: argparse.Namespace) -> Repository:
-        repository = options.repository or os.getenv("PDM_PUBLISH_REPO", "pypi")
-        username = options.username or os.getenv("PDM_PUBLISH_USERNAME")
-        password = options.password or os.getenv("PDM_PUBLISH_PASSWORD")
-        ca_certs = options.ca_certs or os.getenv("PDM_PUBLISH_CA_CERTS")
-
-        config = project.global_config.get_repository_config(repository)
-        if config is None:
-            raise PdmUsageError(f"Missing repository config of {repository}")
-        assert config.url is not None
-        if username is not None:
-            config.username = username
-        if password is not None:
-            config.password = password
-        if ca_certs is not None:
-            config.ca_certs = ca_certs
-        return Repository(project, config.url, config.username, config.password, config.ca_certs)
-
-    def handle(self, project: Project, options: argparse.Namespace) -> None:
-        hooks = HookManager(project, options.skip)
-
-        hooks.try_emit("pre_publish")
-
-        if options.build:
-            actions.do_build(project, hooks=hooks)
-
-        package_files = [str(p) for p in project.root.joinpath("dist").iterdir() if not p.name.endswith(".asc")]
-        signatures = {p.stem: str(p) for p in project.root.joinpath("dist").iterdir() if p.name.endswith(".asc")}
-
-        repository = self.get_repository(project, options)
-        uploaded: list[PackageFile] = []
-        with project.core.ui.make_progress(
-            " [progress.percentage]{task.percentage:>3.0f}%",
-            BarColumn(),
-            DownloadColumn(),
-            "•",
-            TimeRemainingColumn(
-                compact=True,
-                elapsed_when_finished=True,
-            ),
-            "•",
-            TransferSpeedColumn(),
-        ) as progress, project.core.ui.logging("publish"):
-            packages = sorted(
-                (self._make_package(p, signatures, options) for p in package_files),
-                # Upload wheels first if they exist.
-                key=lambda p: not p.base_filename.endswith(".whl"),
-            )
-            for package in packages:
-                resp = repository.upload(package, progress)
-                logger.debug("Response from %s:\n%s %s", resp.url, resp.status_code, resp.reason)
-                self._check_response(resp)
-                uploaded.append(package)
-
-        release_urls = repository.get_release_urls(uploaded)
-        if release_urls:
-            project.core.ui.echo("\n[success]View at:")
-            for url in release_urls:
-                project.core.ui.echo(url)
 
-        hooks.try_emit("post_publish")
+@pytest.mark.parametrize(
+    "filename",
+    ["demo-0.0.1-py2.py3-none-any.whl", "demo-0.0.1.tar.gz", "demo-0.0.1.zip"],
+)
+def test_package_parse_metadata(filename):
+    fullpath = FIXTURES / "artifacts" / filename
+    package = PackageFile.from_filename(str(fullpath), None)
+    assert package.base_filename == filename
+    meta = package.metadata_dict
+    assert meta["name"] == "demo"
+    assert meta["version"] == "0.0.1"
+    assert all(f"{hash_name}_digest" in meta for hash_name in ["md5", "sha256", "blake2_256"])
+
+    if filename.endswith(".whl"):
+        assert meta["pyversion"] == "py2.py3"
+        assert meta["filetype"] == "bdist_wheel"
+    else:
+        assert meta["pyversion"] == "source"
+        assert meta["filetype"] == "sdist"
+
+
+def test_parse_metadata_with_non_ascii_chars():
+    fullpath = FIXTURES / "artifacts" / "caj2pdf-restructured-0.1.0a6.tar.gz"
+    package = PackageFile.from_filename(str(fullpath), None)
+    meta = package.metadata_dict
+    assert meta["summary"] == "caj2pdf 重新组织，方便打包与安装"  # noqa: RUF001
+    assert meta["author_email"] == "张三 <san@zhang.me>"
+    assert meta["description"].strip() == "# caj2pdf\n\n测试中文项目"
+
+
+def test_package_add_signature(tmp_path):
+    package = PackageFile.from_filename(str(FIXTURES / "artifacts/demo-0.0.1-py2.py3-none-any.whl"), None)
+    tmp_path.joinpath("signature.asc").write_bytes(b"test gpg signature")
+    package.add_gpg_signature(str(tmp_path / "signature.asc"), "signature.asc")
+    assert package.gpg_signature == ("signature.asc", b"test gpg signature")
+
+
+def test_package_call_gpg_sign():
+    package = PackageFile.from_filename(str(FIXTURES / "artifacts/demo-0.0.1-py2.py3-none-any.whl"), None)
+    try:
+        package.sign(None)
+    finally:
+        try:
+            os.unlink(package.filename + ".asc")
+        except OSError:
+            pass
+    assert package.gpg_signature == (package.base_filename + ".asc", b"fake signature")
+
+
+def test_repository_get_release_urls(project):
+    package_files = [
+        PackageFile.from_filename(str(FIXTURES / "artifacts" / fn), None)
+        for fn in [
+            "demo-0.0.1-py2.py3-none-any.whl",
+            "demo-0.0.1.tar.gz",
+            "demo-0.0.1.zip",
+        ]
+    ]
+    repository = Repository(project, "https://upload.pypi.org/legacy/", "abc", "123", None)
+    assert repository.get_release_urls(package_files) == {"https://pypi.org/project/demo/0.0.1/"}
+
+    repository = Repository(project, "https://example.pypi.org/legacy/", "abc", "123", None)
+    assert not repository.get_release_urls(package_files)
+
+
+@pytest.mark.usefixtures("prepare_packages")
+def test_publish_pick_up_asc_files(project, uploaded, pdm):
+    for p in list(project.root.joinpath("dist").iterdir()):
+        with open(str(p) + ".asc", "w") as f:
+            f.write("fake signature")
+
+    pdm(
+        ["publish", "--no-build", "--username=abc", "--password=123"],
+        obj=project,
+        strict=True,
+    )
+    # Test wheels are uploaded first
+    assert uploaded[0].base_filename.endswith(".whl")
+    for package in uploaded:
+        assert package.gpg_signature == (
+            package.base_filename + ".asc",
+            b"fake signature",
+        )
+
+
+@pytest.mark.usefixtures("prepare_packages")
+def test_publish_package_with_signature(project, uploaded, pdm):
+    pdm(
+        ["publish", "--no-build", "-S", "--username=abc", "--password=123"],
+        obj=project,
+        strict=True,
+    )
+    for package in uploaded:
+        assert package.gpg_signature == (
+            package.base_filename + ".asc",
+            b"fake signature",
+        )
+
+
+@pytest.mark.usefixtures("local_finder")
+def test_publish_and_build_in_one_run(fixture_project, pdm, mock_pypi):
+    project = fixture_project("demo-module")
+    result = pdm(["publish", "--username=abc", "--password=123"], obj=project, strict=True).output
+
+    mock_pypi.assert_called()
+    assert "Uploading demo_module-0.1.0-py3-none-any.whl" in result
+    assert "Uploading demo-module-0.1.0.tar.gz" in result
+    assert "https://pypi.org/project/demo-module/0.1.0/" in result
+
+
+def test_publish_cli_args_and_env_var_precedence(project, monkeypatch):
+    repo = PublishCommand.get_repository(
+        project,
+        Namespace(repository=None, username="foo", password="bar", ca_certs="custom.pem", verify_ssl=True),
+    )
+    assert repo.url == "https://upload.pypi.org/legacy/"
+    assert repo.session.auth == ("foo", "bar")
+    assert repo.session.verify == "custom.pem"
+
+    with monkeypatch.context() as m:
+        m.setenv("PDM_PUBLISH_USERNAME", "bar")
+        m.setenv("PDM_PUBLISH_PASSWORD", "secret")
+        m.setenv("PDM_PUBLISH_REPO", "testpypi")
+        m.setenv("PDM_PUBLISH_CA_CERTS", "override.pem")
+
+        repo = PublishCommand.get_repository(
+            project,
+            Namespace(repository=None, username=None, password=None, ca_certs=None, verify_ssl=True),
+        )
+        assert repo.url == "https://test.pypi.org/legacy/"
+        assert repo.session.auth == ("bar", "secret")
+        assert repo.session.verify == "override.pem"
+
+        repo = PublishCommand.get_repository(
+            project,
+            Namespace(repository="pypi", username="foo", password=None, ca_certs="custom.pem", verify_ssl=True),
+        )
+        assert repo.url == "https://upload.pypi.org/legacy/"
+        assert repo.session.auth == ("foo", "secret")
+        assert repo.session.verify == "custom.pem"
+
+
+def test_repository_get_credentials_from_keyring(project, keyring):
+    keyring.save_auth_info("https://test.org/upload", "foo", "barbaz")
+    repository = Repository(project, "https://test.org/upload", None, None, None)
+    assert repository.session.auth == ("foo", "barbaz")
```

### Comparing `pdm-2.6.1/src/pdm/cli/commands/publish/package.py` & `pdm-2.7.0/src/pdm/cli/commands/publish/package.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,17 @@
 import email.message
 import email.policy
 import hashlib
 import io
 import os
 import re
 import subprocess
-import tarfile
-import zipfile
 from dataclasses import dataclass
 from typing import IO, Any, cast
 
-from unearth.preparer import has_leading_dir, split_leading_dir
-
 from pdm.exceptions import PdmUsageError, ProjectError
 from pdm.termui import logger
 from pdm.utils import normalize_name
 
 DIST_EXTENSIONS = {
     ".whl": "bdist_wheel",
     ".tar.bz2": "sdist",
@@ -92,14 +88,18 @@
         else:
             metadata = cls.read_metadata_from_tar(filename)
             py_ver = "source"
         return cls(filename, metadata, comment, py_ver, filetype)
 
     @staticmethod
     def read_metadata_from_tar(filename: str) -> email.message.Message:
+        import tarfile
+
+        from unearth.preparer import has_leading_dir, split_leading_dir
+
         if filename.endswith(".gz"):
             mode = "r:gz"
         elif filename.endswith(".bz2"):
             mode = "r:bz2"
         else:
             logger.warning(f"Can't determine the compression mode for {filename}")
             mode = "r:*"
@@ -110,25 +110,31 @@
                 fn = split_leading_dir(m.name)[1] if has_leading else m.name
                 if fn == "PKG-INFO":
                     return parse_metadata(cast(IO[bytes], tar.extractfile(m)))
         raise ProjectError(f"No PKG-INFO found in {filename}")
 
     @staticmethod
     def read_metadata_from_zip(filename: str) -> email.message.Message:
+        import zipfile
+
+        from unearth.preparer import has_leading_dir, split_leading_dir
+
         with zipfile.ZipFile(filename, allowZip64=True) as zip:
             filenames = zip.namelist()
             has_leading = has_leading_dir(filenames)
             for name in filenames:
                 fn = split_leading_dir(name)[1] if has_leading else name
                 if fn == "PKG-INFO":
                     return parse_metadata(zip.open(name))
         raise ProjectError(f"No PKG-INFO found in {filename}")
 
     @staticmethod
     def read_metadata_from_wheel(filename: str) -> email.message.Message:
+        import zipfile
+
         with zipfile.ZipFile(filename, allowZip64=True) as zip:
             for fn in zip.namelist():
                 if fn.replace("\\", "/").endswith(".dist-info/METADATA"):
                     return parse_metadata(zip.open(fn))
         raise ProjectError(f"No egg-info is found in {filename}")
 
     def add_gpg_signature(self, filename: str, signature_name: str) -> None:
```

### Comparing `pdm-2.6.1/src/pdm/cli/commands/publish/repository.py` & `pdm-2.7.0/src/pdm/cli/commands/publish/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,70 +1,79 @@
 from __future__ import annotations
 
 import os
 import pathlib
 import weakref
-from typing import Any, Iterable
+from typing import TYPE_CHECKING, Any, Iterable
 from urllib.parse import urlparse, urlunparse
 
-import requests
-import requests_toolbelt
 import rich.progress
-from unearth.auth import get_keyring_provider
 
 from pdm import termui
 from pdm.cli.commands.publish.package import PackageFile
 from pdm.exceptions import PdmUsageError
 from pdm.project import Project
 from pdm.project.config import DEFAULT_REPOSITORIES
 
-keyring = get_keyring_provider()
+if TYPE_CHECKING:
+    from requests import Response
 
 
 class Repository:
     def __init__(
         self,
         project: Project,
         url: str,
         username: str | None,
         password: str | None,
         ca_certs: str | None,
+        verify_ssl: bool | None = True,
     ) -> None:
         self.url = url
         self.session = project.environment._build_session([])
-        if ca_certs is not None:
+        if verify_ssl is False:
+            self.session.verify = verify_ssl
+        elif ca_certs is not None:
             self.session.set_ca_certificates(pathlib.Path(ca_certs))
         self._credentials_to_save: tuple[str, str, str] | None = None
         self.ui = project.core.ui
         username, password = self._ensure_credentials(username, password)
         self.session.auth = (username, password)
         weakref.finalize(self, self.session.close)
 
     def _ensure_credentials(self, username: str | None, password: str | None) -> tuple[str, str]:
+        from pdm.models.auth import keyring
+
         netloc = urlparse(self.url).netloc
         if username and password:
             return username, password
         if password:
             return "__token__", password
+        if keyring.enabled:
+            auth = keyring.get_auth_info(self.url, username)
+            if auth is not None:
+                return auth
         token = self._get_pypi_token_via_oidc()
         if token is not None:
             return "__token__", token
         if not termui.is_interactive():
             raise PdmUsageError("Username and password are required")
         username, password, save = self._prompt_for_credentials(netloc, username)
-        if save and keyring is not None and termui.confirm("Save credentials to keyring?"):
+        if save and keyring.enabled and termui.confirm("Save credentials to keyring?"):
             self._credentials_to_save = (netloc, username, password)
         return username, password
 
     def _get_pypi_token_via_oidc(self) -> str | None:
         ACTIONS_ID_TOKEN_REQUEST_TOKEN = os.getenv("ACTIONS_ID_TOKEN_REQUEST_TOKEN")
         ACTIONS_ID_TOKEN_REQUEST_URL = os.getenv("ACTIONS_ID_TOKEN_REQUEST_URL")
         if not ACTIONS_ID_TOKEN_REQUEST_TOKEN or not ACTIONS_ID_TOKEN_REQUEST_URL:
             return None
         self.ui.echo("Getting PyPI token via GitHub Actions OIDC...")
+        import requests
+
         try:
             parsed_url = urlparse(self.url)
             audience_url = urlunparse(parsed_url._replace(path="/_/oidc/audience"))
             resp = self.session.get(audience_url)
             resp.raise_for_status()
 
             resp = self.session.get(
@@ -85,25 +94,28 @@
         else:
             if os.getenv("GITHUB_ACTIONS"):
                 # tell GitHub Actions to mask the token in any console logs
                 print(f"::add-mask::{token}")
             return token
 
     def _prompt_for_credentials(self, service: str, username: str | None) -> tuple[str, str, bool]:
-        if keyring is not None:
+        from pdm.models.auth import keyring
+
+        if keyring.enabled:
             cred = keyring.get_auth_info(service, username)
             if cred is not None:
                 return cred[0], cred[1], False
         if username is None:
             username = termui.ask("[primary]Username")
         password = termui.ask("[primary]Password", password=True)
         return username, password, True
 
     def _save_credentials(self, service: str, username: str, password: str) -> None:
-        assert keyring is not None
+        from pdm.models.auth import keyring
+
         self.ui.echo("Saving credentials to keyring")
         keyring.save_auth_info(service, username, password)
 
     @staticmethod
     def _convert_to_list_of_tuples(data: dict[str, Any]) -> list[tuple[str, Any]]:
         result: list[tuple[str, Any]] = []
         for key, value in data.items():
@@ -119,15 +131,17 @@
             base = "https://pypi.org/"
         elif self.url.startswith(DEFAULT_REPOSITORIES["testpypi"].rstrip("/")):
             base = "https://test.pypi.org/"
         else:
             return set()
         return {f"{base}project/{package.metadata['name']}/{package.metadata['version']}/" for package in packages}
 
-    def upload(self, package: PackageFile, progress: rich.progress.Progress) -> requests.Response:
+    def upload(self, package: PackageFile, progress: rich.progress.Progress) -> Response:
+        import requests_toolbelt
+
         payload = package.metadata_dict
         payload.update(
             {
                 ":action": "file_upload",
                 "protocol_version": "1",
             }
         )
```

### Comparing `pdm-2.6.1/src/pdm/cli/commands/remove.py` & `pdm-2.7.0/src/pdm/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/commands/run.py` & `pdm-2.7.0/src/pdm/cli/commands/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,39 +5,39 @@
 import os
 import re
 import shlex
 import signal
 import subprocess
 import sys
 from types import FrameType
-from typing import Any, Callable, Iterator, Mapping, NamedTuple, Sequence, cast
+from typing import TYPE_CHECKING, Mapping, NamedTuple, Sequence, cast
 
 from rich import print_json
 
 from pdm import termui
 from pdm.cli.commands.base import BaseCommand
 from pdm.cli.hooks import HookManager
 from pdm.cli.options import skip_option, venv_option
 from pdm.cli.utils import check_project_file, get_pep582_path
-from pdm.compat import TypedDict
 from pdm.exceptions import PdmUsageError
 from pdm.project import Project
 from pdm.signals import pdm_signals
 from pdm.utils import is_path_relative_to
 
+if TYPE_CHECKING:
+    from typing import Any, Callable, Iterator, TypedDict
 
-class EnvFileOptions(TypedDict, total=True):
-    override: str
+    class EnvFileOptions(TypedDict, total=True):
+        override: str
 
-
-class TaskOptions(TypedDict, total=False):
-    env: Mapping[str, str]
-    env_file: EnvFileOptions | str | None
-    help: str
-    site_packages: bool
+    class TaskOptions(TypedDict, total=False):
+        env: Mapping[str, str]
+        env_file: EnvFileOptions | str | None
+        help: str
+        site_packages: bool
 
 
 def exec_opts(*options: TaskOptions | None) -> dict[str, Any]:
     return dict(
         env={k: v for opts in options if opts for k, v in opts.get("env", {}).items()},
         **{k: v for opts in options if opts for k, v in opts.items() if k not in ("env", "help")},
     )
@@ -84,15 +84,15 @@
 
     TYPES = ["cmd", "shell", "call", "composite"]
     OPTIONS = ["env", "env_file", "help", "site_packages"]
 
     def __init__(self, project: Project, hooks: HookManager) -> None:
         self.project = project
         global_options = cast(
-            TaskOptions,
+            "TaskOptions",
             self.project.scripts.get("_", {}) if self.project.scripts else {},
         )
         self.global_options = global_options.copy()
         self.hooks = hooks
 
     def get_task(self, script_name: str) -> Task | None:
         if script_name not in self.project.scripts:
@@ -112,15 +112,15 @@
                     break
             else:
                 raise PdmUsageError(f"Script type must be one of ({', '.join(self.TYPES)})")
             options = script.copy()
         unknown_options = set(options) - set(self.OPTIONS)
         if unknown_options:
             raise PdmUsageError(f"Unknown options for task {script_name}: {', '.join(unknown_options)}")
-        return Task(kind, script_name, value, cast(TaskOptions, options))
+        return Task(kind, script_name, value, cast("TaskOptions", options))
 
     def _run_process(
         self,
         args: Sequence[str] | str,
         chdir: bool = False,
         shell: bool = False,
         site_packages: bool = False,
@@ -237,14 +237,15 @@
             f"Running {task}: [success]{str(args)}[/]",
             err=True,
             verbosity=termui.Verbosity.DETAIL,
         )
         if kind == "composite":
             args = list(args)
             should_interpolate = any(RE_ARGS_PLACEHOLDER.search(script) for script in value)
+            code = 0
             for script in value:
                 if should_interpolate:
                     script, _ = interpolate(script, args)
                 split = shlex.split(script)
                 cmd = split[0]
                 subargs = split[1:] + ([] if should_interpolate else args)
                 code = self.run(cmd, subargs, options)
```

### Comparing `pdm-2.6.1/src/pdm/cli/commands/search.py` & `pdm-2.7.0/src/pdm/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/commands/self_cmd.py` & `pdm-2.7.0/src/pdm/cli/commands/self_cmd.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/commands/show.py` & `pdm-2.7.0/src/pdm/cli/commands/show.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/commands/sync.py` & `pdm-2.7.0/src/pdm/cli/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/commands/update.py` & `pdm-2.7.0/src/pdm/cli/commands/venv/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,77 +1,42 @@
+from __future__ import annotations
+
 import argparse
 
-from pdm.cli import actions
-from pdm.cli.commands.base import BaseCommand
-from pdm.cli.filters import GroupSelection
-from pdm.cli.hooks import HookManager
-from pdm.cli.options import (
-    groups_group,
-    install_group,
-    lockfile_option,
-    prerelease_option,
-    save_strategy_group,
-    skip_option,
-    unconstrained_option,
-    update_strategy_group,
-    venv_option,
-)
 from pdm.project import Project
+from pdm.cli.commands.base import BaseCommand
+from pdm.cli.commands.venv.activate import ActivateCommand
+from pdm.cli.commands.venv.create import CreateCommand
+from pdm.cli.commands.venv.list import ListCommand
+from pdm.cli.commands.venv.purge import PurgeCommand
+from pdm.cli.commands.venv.remove import RemoveCommand
+from pdm.cli.commands.venv.utils import get_venv_with_name
+from pdm.cli.options import Option
 
 
 class Command(BaseCommand):
-    """Update package(s) in pyproject.toml"""
+    """Virtualenv management"""
 
-    arguments = [
-        *BaseCommand.arguments,
-        groups_group,
-        install_group,
-        lockfile_option,
-        save_strategy_group,
-        update_strategy_group,
-        prerelease_option,
-        unconstrained_option,
-        skip_option,
-        venv_option,
-    ]
+    name = "venv"
+    arguments: list[Option] = []
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
-        parser.add_argument(
-            "-t",
-            "--top",
-            action="store_true",
-            help="Only update those listed in pyproject.toml",
-        )
-        parser.add_argument(
-            "--dry-run",
-            "--outdated",
-            action="store_true",
-            dest="dry_run",
-            help="Show the difference only without modifying the lockfile content",
-        )
-        parser.add_argument(
-            "--no-sync",
-            dest="sync",
-            default=True,
-            action="store_false",
-            help="Only update lock file but do not sync packages",
-        )
-        parser.add_argument("packages", nargs="*", help="If packages are given, only update them")
-        parser.set_defaults(dev=None)
+        group = parser.add_mutually_exclusive_group()
+        group.add_argument("--path", help="Show the path to the given virtualenv")
+        group.add_argument("--python", help="Show the python interpreter path for the given virtualenv")
+        subparser = parser.add_subparsers()
+        CreateCommand.register_to(subparser, "create")
+        ListCommand.register_to(subparser, "list")
+        RemoveCommand.register_to(subparser, "remove")
+        ActivateCommand.register_to(subparser, "activate")
+        PurgeCommand.register_to(subparser, "purge")
+        self.parser = parser
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
-        actions.do_update(
-            project,
-            selection=GroupSelection.from_options(project, options),
-            save=options.save_strategy or project.config["strategy.save"],
-            strategy=options.update_strategy or project.config["strategy.update"],
-            unconstrained=options.unconstrained,
-            top=options.top,
-            dry_run=options.dry_run,
-            packages=options.packages,
-            sync=options.sync,
-            no_editable=options.no_editable,
-            no_self=options.no_self,
-            prerelease=options.prerelease,
-            fail_fast=options.fail_fast,
-            hooks=HookManager(project, options.skip),
-        )
+        if options.path:
+            venv = get_venv_with_name(project, options.path)
+            project.core.ui.echo(str(venv.root))
+        elif options.python:
+            venv = get_venv_with_name(project, options.python)
+            project.core.ui.echo(str(venv.interpreter))
+        else:
+            self.parser.print_help()
```

### Comparing `pdm-2.6.1/src/pdm/cli/commands/use.py` & `pdm-2.7.0/src/pdm/cli/commands/use.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/commands/venv/__init__.py` & `pdm-2.7.0/src/pdm/cli/commands/venv/remove.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,34 @@
-from __future__ import annotations
-
 import argparse
+import shutil
+from pathlib import Path
 
-from pdm.project import Project
+from pdm import termui
 from pdm.cli.commands.base import BaseCommand
-from pdm.cli.commands.venv.activate import ActivateCommand
-from pdm.cli.commands.venv.create import CreateCommand
-from pdm.cli.commands.venv.list import ListCommand
-from pdm.cli.commands.venv.purge import PurgeCommand
-from pdm.cli.commands.venv.remove import RemoveCommand
 from pdm.cli.commands.venv.utils import get_venv_with_name
-from pdm.cli.options import Option
+from pdm.cli.options import verbose_option
+from pdm.project import Project
 
 
-class Command(BaseCommand):
-    """Virtualenv management"""
+class RemoveCommand(BaseCommand):
+    """Remove the virtualenv with the given name"""
 
-    name = "venv"
-    arguments: list[Option] = []
+    arguments = [verbose_option]
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
-        group = parser.add_mutually_exclusive_group()
-        group.add_argument("--path", help="Show the path to the given virtualenv")
-        group.add_argument("--python", help="Show the python interpreter path for the given virtualenv")
-        subparser = parser.add_subparsers()
-        CreateCommand.register_to(subparser, "create")
-        ListCommand.register_to(subparser, "list")
-        RemoveCommand.register_to(subparser, "remove")
-        ActivateCommand.register_to(subparser, "activate")
-        PurgeCommand.register_to(subparser, "purge")
-        self.parser = parser
+        parser.add_argument(
+            "-y",
+            "--yes",
+            action="store_true",
+            help="Answer yes on the following question",
+        )
+        parser.add_argument("env", help="The key of the virtualenv")
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
-        if options.path:
-            venv = get_venv_with_name(project, options.path)
-            project.core.ui.echo(str(venv.root))
-        elif options.python:
-            venv = get_venv_with_name(project, options.python)
-            project.core.ui.echo(str(venv.interpreter))
-        else:
-            self.parser.print_help()
+        project.core.ui.echo("Virtualenvs created with this project:")
+        venv = get_venv_with_name(project, options.env)
+        if options.yes or termui.confirm(f"[warning]Will remove: [success]{venv.root}[/], continue?", default=True):
+            shutil.rmtree(venv.root)
+            saved_python = project._saved_python
+            if saved_python and Path(saved_python).parent.parent == venv.root:
+                project._saved_python = None
+            project.core.ui.echo("Removed successfully!")
```

### Comparing `pdm-2.6.1/src/pdm/cli/commands/venv/activate.py` & `pdm-2.7.0/src/pdm/cli/commands/venv/activate.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/commands/venv/backends.py` & `pdm-2.7.0/src/pdm/cli/commands/venv/backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/commands/venv/create.py` & `pdm-2.7.0/src/pdm/cli/commands/venv/create.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/commands/venv/list.py` & `pdm-2.7.0/src/pdm/cli/commands/venv/list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/commands/venv/purge.py` & `pdm-2.7.0/src/pdm/cli/commands/venv/purge.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/commands/venv/utils.py` & `pdm-2.7.0/src/pdm/cli/commands/venv/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/completions/pdm.bash` & `pdm-2.7.0/src/pdm/cli/completions/pdm.bash`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             ;;
 
             (plugin)
             opts="--help --verbose"
             ;;
 
             (publish)
-            opts="--ca-certs --comment --help --identity --no-build --password --project --repository --sign --skip --username --verbose"
+            opts="--ca-certs --comment --help --identity --no-build --no-very-ssl --password --project --repository --sign --skip --username --verbose"
             ;;
 
             (remove)
             opts="--dev --dry-run --fail-fast --global --group --help --lockfile --no-editable --no-isolation --no-self --no-sync --project --skip --venv --verbose"
             ;;
 
             (run)
```

### Comparing `pdm-2.6.1/src/pdm/cli/completions/pdm.fish` & `pdm-2.7.0/src/pdm/cli/completions/pdm.fish`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l fail-fast -d 'Abort on first installation error'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l group -d 'Specify the target dependency group to add into'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l lockfile -d 'Specify another lockfile path. Default: pdm.lock. [env var: PDM_LOCKFILE]'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l no-editable -d 'Install non-editable versions for all packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l no-isolation -d 'Do not isolate the build in a clean environment'
-complete -c pdm -A -n '__fish_seen_subcommand_from add' -l no-self -d 'Don\'t install the project itself'
+complete -c pdm -A -n '__fish_seen_subcommand_from add' -l no-self -d 'Don\'t install the project itself. [env var: PDM_NO_SELF]'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l no-sync -d 'Only write pyproject.toml and do not sync the working set'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l prerelease -d 'Allow prereleases to be pinned'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l save-compatible -d 'Save compatible version specifiers'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l save-exact -d 'Save exact version specifiers'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l save-minimum -d 'Save minimum version specifiers'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l save-wildcard -d 'Save wildcard version specifiers'
@@ -163,15 +163,15 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l group -d 'Select group of optional-dependencies separated by comma or dev-dependencies (with `-d`). Can be supplied multiple times, use ":all" to include all groups under the same species.'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l lockfile -d 'Specify another lockfile path. Default: pdm.lock. [env var: PDM_LOCKFILE]'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l no-default -d 'Don\'t include dependencies from the default group'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l no-editable -d 'Install non-editable versions for all packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l no-isolation -d 'Do not isolate the build in a clean environment'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l no-lock -d 'Don\'t do lock if the lock file is not found or outdated'
-complete -c pdm -A -n '__fish_seen_subcommand_from install' -l no-self -d 'Don\'t install the project itself'
+complete -c pdm -A -n '__fish_seen_subcommand_from install' -l no-self -d 'Don\'t install the project itself. [env var: PDM_NO_SELF]'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l plugins -d 'Install the plugins specified in pyproject.toml'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l production -d 'Unselect dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
@@ -215,14 +215,15 @@
 
 # publish
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l ca-certs -d 'The path to a PEM-encoded Certificate Authority bundle to use for publish server validation [env var: PDM_PUBLISH_CA_CERTS]'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l comment -d 'The comment to include with the distribution file.'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l identity -d 'GPG identity used to sign files.'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l no-build -d 'Don\'t build the package before publishing'
+complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l no-very-ssl -d 'Disable SSL verification'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l password -d 'The password to access the repository [env var: PDM_PUBLISH_PASSWORD]'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l repository -d 'The repository name or url to publish the package to [env var: PDM_PUBLISH_REPO]'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l sign -d 'Upload the package with PGP signature'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l username -d 'The username to access the repository [env var: PDM_PUBLISH_USERNAME]'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
@@ -233,15 +234,15 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l fail-fast -d 'Abort on first installation error'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l group -d 'Specify the target dependency group to remove from'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l lockfile -d 'Specify another lockfile path. Default: pdm.lock. [env var: PDM_LOCKFILE]'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l no-editable -d 'Install non-editable versions for all packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l no-isolation -d 'Do not isolate the build in a clean environment'
-complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l no-self -d 'Don\'t install the project itself'
+complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l no-self -d 'Don\'t install the project itself. [env var: PDM_NO_SELF]'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l no-sync -d 'Only write pyproject.toml and do not uninstall packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # run
@@ -284,15 +285,15 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l group -d 'Select group of optional-dependencies separated by comma or dev-dependencies (with `-d`). Can be supplied multiple times, use ":all" to include all groups under the same species.'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l lockfile -d 'Specify another lockfile path. Default: pdm.lock. [env var: PDM_LOCKFILE]'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l no-default -d 'Don\'t include dependencies from the default group'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l no-editable -d 'Install non-editable versions for all packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l no-isolation -d 'Do not isolate the build in a clean environment'
-complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l no-self -d 'Don\'t install the project itself'
+complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l no-self -d 'Don\'t install the project itself. [env var: PDM_NO_SELF]'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l only-keep -d 'Only keep the selected packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l production -d 'Unselect dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l reinstall -d 'Force reinstall existing dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
@@ -303,15 +304,15 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l group -d 'Select group of optional-dependencies separated by comma or dev-dependencies (with `-d`). Can be supplied multiple times, use ":all" to include all groups under the same species.'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l lockfile -d 'Specify another lockfile path. Default: pdm.lock. [env var: PDM_LOCKFILE]'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l no-default -d 'Don\'t include dependencies from the default group'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l no-editable -d 'Install non-editable versions for all packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l no-isolation -d 'Do not isolate the build in a clean environment'
-complete -c pdm -A -n '__fish_seen_subcommand_from update' -l no-self -d 'Don\'t install the project itself'
+complete -c pdm -A -n '__fish_seen_subcommand_from update' -l no-self -d 'Don\'t install the project itself. [env var: PDM_NO_SELF]'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l no-sync -d 'Only update lock file but do not sync packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l outdated -d 'Show the difference only without modifying the lockfile content'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l prerelease -d 'Allow prereleases to be pinned'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l production -d 'Unselect dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l save-compatible -d 'Save compatible version specifiers'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l save-exact -d 'Save exact version specifiers'
```

### Comparing `pdm-2.6.1/src/pdm/cli/completions/pdm.ps1` & `pdm-2.7.0/src/pdm/cli/completions/pdm.ps1`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,15 @@
                     }
                 }
                 break
             }
             "publish" {
                 $completer.AddOpts(
                     @(
-                        [Option]::new(@("-r", "--repository", "-u", "--username", "-P", "--password", "-S", "--sign", "-i", "--identity", "-c", "--comment", "--no-build", "--ca-certs")),
+                        [Option]::new(@("-r", "--repository", "-u", "--username", "-P", "--password", "-S", "--sign", "-i", "--identity", "-c", "--comment", "--no-build", "--ca-certs", "--no-verify-ssl")),
                         $skipOption,
                         $projectOption
                     ))
                 break
             }
             "remove" {
                 $completer.AddOpts(
```

### Comparing `pdm-2.6.1/src/pdm/cli/completions/pdm.zsh` & `pdm-2.7.0/src/pdm/cli/completions/pdm.zsh`

 * *Files 0% similar despite different names*

```diff
@@ -294,14 +294,15 @@
         {-r,--repository}'[The repository name or url to publish the package to }[env var: PDM_PUBLISH_REPO]]:repository:'
         {-u,--username}'[The username to access the repository [env var: PDM_PUBLISH_USERNAME]]:username:'
         {-P,--password}'[The password to access the repository [env var: PDM_PUBLISH_PASSWORD]]:password:'
         {-S,--sign}'[Upload the package with PGP signature]'
         {-i,--identity}'[GPG identity used to sign files.]:gpg identity:'
         {-k,--skip}'[Skip some tasks and/or hooks by their comma-separated names]'
         {-c,--comment}'[The comment to include with the distribution file.]:comment:'
+        "--no-verify-ssl[Disable SSL verification]"
         "--ca-certs[The path to a PEM-encoded Certificate Authority bundle to use for publish server validation]:cacerts:_files"
         "--no-build[Don't build the package before publishing]"
       )
       ;;
     remove)
       arguments+=(
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
```

### Comparing `pdm-2.6.1/src/pdm/cli/filters.py` & `pdm-2.7.0/src/pdm/cli/filters.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/hooks.py` & `pdm-2.7.0/src/pdm/cli/hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/cli/options.py` & `pdm-2.7.0/src/pdm/cli/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 import argparse
 import os
 import sys
 from functools import partial
-from typing import Any, Sequence, cast
+from typing import TYPE_CHECKING, cast
 
-from pdm.cli.actions import print_pep582_command
-from pdm.compat import Protocol
-from pdm.project import Project
+if TYPE_CHECKING:
+    from typing import Any, Protocol, Sequence
 
+    from pdm.project import Project
 
-class ActionCallback(Protocol):
-    def __call__(self, project: Project, namespace: argparse.Namespace, values: str | Sequence[Any] | None) -> None:
-        ...
+    class ActionCallback(Protocol):
+        def __call__(self, project: Project, namespace: argparse.Namespace, values: str | Sequence[Any] | None) -> None:
+            ...
 
 
 class Option:
     """A reusable option object which delegates all arguments
     to parser.add_argument().
     """
 
@@ -145,14 +145,16 @@
     default=os.getenv("PDM_LOCKFILE"),
     help="Specify another lockfile path. Default: pdm.lock. [env var: PDM_LOCKFILE]",
 )
 
 
 @Option("--pep582", const="AUTO", metavar="SHELL", nargs="?", help="Print the command line to be eval'd by the shell")
 def pep582_option(project: Project, namespace: argparse.Namespace, values: str | Sequence[Any] | None) -> None:
+    from pdm.cli.actions import print_pep582_command
+
     print_pep582_command(project, cast(str, values))
     sys.exit(0)
 
 
 install_group = ArgumentGroup("Install options")
 install_group.add_argument(
     "--no-editable",
```

### Comparing `pdm-2.6.1/src/pdm/cli/utils.py` & `pdm-2.7.0/src/pdm/cli/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,14 @@
 import tomlkit
 from packaging.specifiers import SpecifierSet
 from resolvelib.structs import DirectedGraph
 from rich.tree import Tree
 
 from pdm import termui
 from pdm.exceptions import PdmArgumentError, ProjectError
-from pdm.formats import FORMATS
-from pdm.formats.base import make_array, make_inline_table
 from pdm.models.requirements import (
     Requirement,
     filter_requirements_with_extras,
     parse_requirement,
     strip_extras,
 )
 from pdm.models.specifiers import PySpecSet, get_specifier
@@ -435,14 +433,15 @@
     project: Project,
     mapping: dict[str, Candidate],
     fetched_dependencies: dict[tuple[str, str | None], list[Requirement]],
 ) -> dict:
     """Format lock file from a dict of resolved candidates, a mapping of dependencies
     and a collection of package summaries.
     """
+    from pdm.formats.base import make_array, make_inline_table
 
     packages = tomlkit.aot()
     file_hashes = tomlkit.table()
     for k, v in sorted(mapping.items()):
         base = tomlkit.table()
         base.update(v.as_lockfile_entry(project.root))
         base.add("summary", v.summary or "")
@@ -505,14 +504,16 @@
         raise ProjectError(
             "The pyproject.toml has not been initialized yet. You can do this by running [success]`pdm init`[/]."
         ) from None
 
 
 def find_importable_files(project: Project) -> Iterable[tuple[str, Path]]:
     """Find all possible files that can be imported"""
+    from pdm.formats import FORMATS
+
     for filename in (
         "Pipfile",
         "pyproject.toml",
         "requirements.in",
         "requirements.txt",
         "setup.py",
     ):
@@ -562,15 +563,15 @@
         result = [
             "Unable to find a resolution because the following dependencies don't work "
             "on all Python versions in the range of the project's `requires-python`: "
             f"[success]{pyspec}[/]."
         ]
         for req, parent in conflicting:
             pyspec &= req.specifier
-            info_lines.add(f"  {req.as_line()} (from {repr(parent)})")
+            info_lines.add(f"  {req.as_line()} (from {parent!r})")
         result.extend(sorted(info_lines))
         if pyspec.is_impossible:
             result.append("Consider changing the version specifiers of the dependencies to be compatible")
         else:
             result.append(
                 "A possible solution is to change the value of `requires-python` "
                 f"in pyproject.toml to [success]{pyspec}[/]."
@@ -605,17 +606,18 @@
     properly. This will update the target dictionary in place.
     List values will be extended, but only if the value is not already in the list.
     """
     for key, value in input.items():
         if key not in target:
             target[key] = value
         elif isinstance(value, dict):
-            target[key].update(value)
+            merge_dictionary(target[key], value)
         elif isinstance(value, list):
-            target[key].extend([x for x in value if x not in target[key]])
+            target[key].extend(x for x in value if x not in target[key])
+            target[key].multiline(True)  # type: ignore[attr-defined]
         else:
             target[key] = value
 
 
 def fetch_hashes(repository: BaseRepository, mapping: Mapping[str, Candidate]) -> None:
     """Fetch hashes for candidates in parallel"""
```

### Comparing `pdm-2.6.1/src/pdm/compat.py` & `pdm-2.7.0/src/pdm/compat.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,20 +29,17 @@
     resources_open_binary = importlib.resources.open_binary
     resources_read_text = importlib.resources.read_text
     resources_path = importlib.resources.path
 
 
 if sys.version_info >= (3, 8):
     from functools import cached_property
-    from typing import Literal, Protocol, TypedDict
 else:
     from typing import Any, Callable, Generic, TypeVar, overload
 
-    from typing_extensions import Literal, Protocol, TypedDict
-
     _T = TypeVar("_T")
     _C = TypeVar("_C")
 
     class cached_property(Generic[_T]):
         def __init__(self, func: Callable[[Any], _T]):
             self.func = func
             self.attr_name = func.__name__
@@ -69,16 +66,8 @@
 else:
     import importlib_metadata
 
 
 Distribution = importlib_metadata.Distribution
 
 
-__all__ = [
-    "tomllib",
-    "cached_property",
-    "importlib_metadata",
-    "Literal",
-    "Protocol",
-    "TypedDict",
-    "Distribution",
-]
+__all__ = ["tomllib", "cached_property", "importlib_metadata", "Distribution"]
```

### Comparing `pdm-2.6.1/src/pdm/core.py` & `pdm-2.7.0/src/pdm/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,32 +10,36 @@
 import argparse
 import importlib
 import itertools
 import os
 import pkgutil
 import sys
 from pathlib import Path
-from typing import Any, Iterable, cast
+from typing import TYPE_CHECKING, cast
 
 from resolvelib import Resolver
 
 from pdm import termui
 from pdm.__version__ import __version__
-from pdm.cli.actions import check_update
-from pdm.cli.commands.base import BaseCommand
 from pdm.cli.options import ignore_python_option, pep582_option, verbose_option
 from pdm.cli.utils import ArgumentParser, ErrorArgumentParser
 from pdm.compat import importlib_metadata
 from pdm.exceptions import PdmArgumentError, PdmUsageError
 from pdm.installers import InstallManager, Synchronizer
 from pdm.models.repositories import PyPIRepository
 from pdm.project import Project
-from pdm.project.config import Config, ConfigItem
+from pdm.project.config import Config
 from pdm.utils import is_in_zipapp
 
+if TYPE_CHECKING:
+    from typing import Any, Iterable
+
+    from pdm.cli.commands.base import BaseCommand
+    from pdm.project.config import ConfigItem
+
 COMMANDS_MODULE_PATH = importlib.import_module("pdm.cli.commands").__path__
 
 
 class Core:
     """A high level object that manages all classes and configurations"""
 
     parser: argparse.ArgumentParser
@@ -148,25 +152,36 @@
         if getattr(options, "use_venv", None):
             use_venv(project, cast(str, options.use_venv))
 
         if command is None:
             self.parser.error("No command given")
         command.handle(project, options)
 
+    def _get_cli_args(self, args: list[str], obj: Project | None) -> list[str]:
+        project = self.create_project(is_global=False) if obj is None else obj
+        if project.is_global:
+            return args
+        config = project.pyproject.settings.get("options", {})
+        (pos, command) = next(((i, arg) for i, arg in enumerate(args) if not arg.startswith("-")), (-1, None))
+        if command and command in config:
+            # add args after the command
+            args[pos + 1 : pos + 1] = list(config[command])
+        return args
+
     def main(
         self,
         args: list[str] | None = None,
         prog_name: str | None = None,
         obj: Project | None = None,
         **extra: Any,
     ) -> None:
         """The main entry function"""
 
         # Ensure same behavior while testing and using the CLI
-        args = args or sys.argv[1:]
+        args = self._get_cli_args(args or sys.argv[1:], obj)
         # Keep it for after project parsing to check if its a defined script
         root_script = None
         try:
             options = self.parser.parse_args(args)
         except PdmArgumentError as e:
             # Failed to parse, try to give all to `run` command as shortcut
             # and keep to root script (first non-dashed param) to check existence
@@ -195,14 +210,16 @@
                 err=True,
             )
             if should_show_tb:
                 self.ui.echo("Add '-v' to see the detailed traceback", style="warning", err=True)
             sys.exit(1)
         else:
             if project.config["check_update"] and not is_in_zipapp():
+                from pdm.cli.actions import check_update
+
                 check_update(project)
 
     def register_command(self, command: type[BaseCommand], name: str | None = None) -> None:
         """Register a subcommand to the subparsers,
         with an optional name of the subcommand.
 
         Args:
@@ -231,15 +248,19 @@
 
         import site
         import sysconfig
 
         base = str(project.root / ".pdm-plugins")
         replace_vars = {"base": base, "platbase": base}
         scheme = "nt" if os.name == "nt" else "posix_prefix"
-        site.addsitedir(sysconfig.get_path("purelib", scheme, replace_vars))
+        purelib = sysconfig.get_path("purelib", scheme, replace_vars)
+        scripts = sysconfig.get_path("scripts", scheme, replace_vars)
+        site.addsitedir(purelib)
+        if os.path.exists(scripts):
+            os.environ["PATH"] = os.pathsep.join([scripts, os.getenv("PATH", "")])
 
     def load_plugins(self) -> None:
         """Import and load plugins under `pdm.plugin` namespace
         A plugin is a callable that accepts the core object as the only argument.
 
         Example:
             ```python
```

### Comparing `pdm-2.6.1/src/pdm/environments/__init__.py` & `pdm-2.7.0/src/pdm/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/environments/base.py` & `pdm-2.7.0/src/pdm/environments/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,46 +7,43 @@
 import subprocess
 import sys
 import tempfile
 from contextlib import contextmanager
 from pathlib import Path
 from typing import TYPE_CHECKING, Generator
 
-import unearth
-
-from pdm import termui
 from pdm.compat import cached_property
 from pdm.exceptions import BuildError, PdmUsageError
-from pdm.models.auth import PdmBasicAuth
 from pdm.models.in_process import get_pep508_environment, get_python_abi_tag
 from pdm.models.python import PythonInfo
-from pdm.models.session import PDMSession
 from pdm.models.working_set import WorkingSet
 from pdm.utils import get_trusted_hosts, is_pip_compatible_with_python
 
 if TYPE_CHECKING:
+    import unearth
+
     from pdm._types import RepositoryConfig
+    from pdm.models.session import PDMSession
     from pdm.project import Project
 
 
 class BaseEnvironment(abc.ABC):
     """Environment dependent stuff related to the selected Python interpreter."""
 
     is_local = False
 
     def __init__(self, project: Project, *, python: str | None = None) -> None:
         """
         :param project: the project instance
         """
+        from pdm.models.auth import PdmBasicAuth
+
         self.python_requires = project.python_requires
         self.project = project
-        self.auth = PdmBasicAuth(
-            self.project.sources,
-            self.project.core.ui.verbosity >= termui.Verbosity.DETAIL,
-        )
+        self.auth = PdmBasicAuth(project.core.ui, self.project.sources)
         if python is None:
             self._interpreter = project.python
         else:
             self._interpreter = PythonInfo.from_path(python)
 
     @property
     def is_global(self) -> bool:
@@ -69,19 +66,23 @@
         this_path = self.get_paths()["scripts"]
         python_root = os.path.dirname(project.python.executable)
         new_path = os.pathsep.join([this_path, os.getenv("PATH", ""), python_root])
         return {"PATH": new_path, "PDM_PROJECT_ROOT": str(project.root)}
 
     @cached_property
     def target_python(self) -> unearth.TargetPython:
+        from unearth import TargetPython
+
         python_version = self.interpreter.version_tuple
         python_abi_tag = get_python_abi_tag(str(self.interpreter.executable))
-        return unearth.TargetPython(python_version, [python_abi_tag])
+        return TargetPython(python_version, [python_abi_tag])
 
     def _build_session(self, trusted_hosts: list[str]) -> PDMSession:
+        from pdm.models.session import PDMSession
+
         ca_certs = self.project.config.get("pypi.ca_certs")
         session = PDMSession(
             cache_dir=self.project.cache("http"),
             trusted_hosts=trusted_hosts,
             ca_certificates=Path(ca_certs) if ca_certs is not None else None,
         )
         certfn = self.project.config.get("pypi.client_cert")
@@ -100,27 +101,29 @@
     ) -> Generator[unearth.PackageFinder, None, None]:
         """Return the package finder of given index sources.
 
         :param sources: a list of sources the finder should search in.
         :param ignore_compatibility: whether to ignore the python version
             and wheel tags.
         """
+        from unearth import PackageFinder
+
         if sources is None:
             sources = self.project.sources
         if not sources:
             raise PdmUsageError(
                 "You must specify at least one index in pyproject.toml or config.\n"
                 "The 'pypi.ignore_stored_index' config value is "
                 f"{self.project.config['pypi.ignore_stored_index']}"
             )
 
         trusted_hosts = get_trusted_hosts(sources)
 
         session = self._build_session(trusted_hosts)
-        finder = unearth.PackageFinder(
+        finder = PackageFinder(
             session=session,
             target_python=self.target_python,
             ignore_compatibility=ignore_compatibility,
             no_binary=os.getenv("PDM_NO_BINARY", "").split(","),
             only_binary=os.getenv("PDM_ONLY_BINARY", "").split(","),
             prefer_binary=os.getenv("PDM_PREFER_BINARY", "").split(","),
             respect_source_order=self.project.pyproject.settings.get("resolution", {}).get(
@@ -159,24 +162,26 @@
         # Fallback to use shutil.which to find the executable
         this_path = self.get_paths()["scripts"]
         python_root = os.path.dirname(self.interpreter.executable)
         new_path = os.pathsep.join([this_path, os.getenv("PATH", ""), python_root])
         return shutil.which(command, path=new_path)
 
     def _download_pip_wheel(self, path: str | Path) -> None:
+        from unearth import UnpackError
+
         download_error = BuildError("Can't get a working copy of pip for the project")
         with self.get_finder([self.project.default_source]) as finder:
             finder.only_binary = ["pip"]
             best_match = finder.find_best_match("pip").best
             if not best_match:
                 raise download_error
             with tempfile.TemporaryDirectory(prefix="pip-download-") as dirname:
                 try:
                     downloaded = finder.download_and_unpack(best_match.link, dirname, dirname)
-                except unearth.UnpackError as e:
+                except UnpackError as e:
                     raise download_error from e
                 shutil.move(str(downloaded), path)
 
     @cached_property
     def pip_command(self) -> list[str]:
         """Get a pip command for this environment, and download one if not available.
         Return a list of args like ['python', '-m', 'pip']
```

### Comparing `pdm-2.6.1/src/pdm/environments/local.py` & `pdm-2.7.0/src/pdm/environments/local.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/environments/python.py` & `pdm-2.7.0/src/pdm/environments/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/exceptions.py` & `pdm-2.7.0/src/pdm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/formats/__init__.py` & `pdm-2.7.0/src/pdm/formats/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 from __future__ import annotations
 
-from argparse import Namespace
-from pathlib import Path
-from typing import Iterable, Mapping, Union, cast
+from typing import TYPE_CHECKING, cast
 
-from pdm.compat import Protocol
 from pdm.formats import flit, pipfile, poetry, requirements, setup_py
-from pdm.models.candidates import Candidate
-from pdm.models.requirements import Requirement
-from pdm.project import Project
-
-ExportItems = Union[Iterable[Candidate], Iterable[Requirement]]
-
-
-class _Format(Protocol):
-    def check_fingerprint(self, project: Project | None, filename: str | Path) -> bool:
-        ...
-
-    def convert(
-        self,
-        project: Project | None,
-        filename: str | Path,
-        options: Namespace | None,
-    ) -> tuple[Mapping, Mapping]:
-        ...
 
-    def export(self, project: Project, candidates: ExportItems, options: Namespace | None) -> str:
-        ...
+if TYPE_CHECKING:
+    from argparse import Namespace
+    from pathlib import Path
+    from typing import Iterable, Mapping, Protocol, Union
+
+    from pdm.models.candidates import Candidate
+    from pdm.models.requirements import Requirement
+    from pdm.project import Project
+
+    ExportItems = Union[Iterable[Candidate], Iterable[Requirement]]
+
+    class _Format(Protocol):
+        def check_fingerprint(self, project: Project | None, filename: str | Path) -> bool:
+            ...
+
+        def convert(
+            self,
+            project: Project | None,
+            filename: str | Path,
+            options: Namespace | None,
+        ) -> tuple[Mapping, Mapping]:
+            ...
+
+        def export(self, project: Project, candidates: ExportItems, options: Namespace | None) -> str:
+            ...
 
 
 FORMATS: Mapping[str, _Format] = {
-    "pipfile": cast(_Format, pipfile),
-    "poetry": cast(_Format, poetry),
-    "flit": cast(_Format, flit),
-    "setuppy": cast(_Format, setup_py),
-    "requirements": cast(_Format, requirements),
+    "pipfile": cast("_Format", pipfile),
+    "poetry": cast("_Format", poetry),
+    "flit": cast("_Format", flit),
+    "setuppy": cast("_Format", setup_py),
+    "requirements": cast("_Format", requirements),
 }
```

### Comparing `pdm-2.6.1/src/pdm/formats/base.py` & `pdm-2.7.0/src/pdm/formats/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/formats/flit.py` & `pdm-2.7.0/src/pdm/formats/flit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from __future__ import annotations
 
 import ast
 import os
-from argparse import Namespace
-from os import PathLike
 from pathlib import Path
-from typing import Any, List, Mapping, cast
+from typing import TYPE_CHECKING, Any, List, Mapping, cast
 
 from pdm.compat import tomllib
 from pdm.formats.base import (
     MetaConverter,
     Unset,
     array_of_inline_tables,
     convert_from,
     make_array,
     make_inline_table,
 )
-from pdm.project import Project
 from pdm.utils import cd
 
+if TYPE_CHECKING:
+    from argparse import Namespace
+    from os import PathLike
+
+    from pdm.project import Project
+
 
 def check_fingerprint(project: Project | None, filename: PathLike) -> bool:
     with open(filename, "rb") as fp:
         try:
             data = tomllib.load(fp)
         except tomllib.TOMLDecodeError:
             return False
```

### Comparing `pdm-2.6.1/src/pdm/formats/pipfile.py` & `pdm-2.7.0/src/pdm/formats/pipfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from __future__ import annotations
 
 import functools
 import operator
 import os
-from argparse import Namespace
-from os import PathLike
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 from packaging.markers import default_environment
 
-from pdm._types import RequirementDict
 from pdm.compat import tomllib
 from pdm.formats.base import make_array
 from pdm.models.markers import Marker
 from pdm.models.requirements import Requirement
-from pdm.project import Project
+
+if TYPE_CHECKING:
+    from argparse import Namespace
+    from os import PathLike
+
+    from pdm._types import RequirementDict
+    from pdm.project import Project
 
 MARKER_KEYS = list(default_environment().keys())
 
 
 def convert_pipfile_requirement(name: str, req: RequirementDict) -> str:
     if isinstance(req, dict):
         markers: list[Marker] = []
```

### Comparing `pdm-2.6.1/src/pdm/formats/poetry.py` & `pdm-2.7.0/src/pdm/formats/poetry.py`

 * *Files 7% similar despite different names*

```diff
@@ -146,38 +146,43 @@
         self.settings["dev-dependencies"] = {
             "dev": make_array([r for key, req in value.items() for r in _convert_req(key, req)], True),
         }
         raise Unset()
 
     @convert_from()
     def includes(self, source: dict[str, list[str] | str]) -> list[str]:
-        result: list[str] = []
+        includes: list[str] = []
+        source_includes: list[str] = []
         for item in source.pop("packages", []):
             assert isinstance(item, dict)
             include = item["include"]
             if item.get("from"):
                 include = f"{item.get('from')}/{include}"
-            result.append(include)
-        result.extend(source.pop("include", []))
-        self.settings.setdefault("build", {})["includes"] = result
+            includes.append(include)
+        for item in source.pop("include", []):
+            if not isinstance(item, dict):
+                includes.append(item)
+            else:
+                dest = source_includes if "sdist" in item.get("format", "") else includes
+                dest.append(item["path"])
+        self.settings.setdefault("build", {})["includes"] = includes
         raise Unset()
 
     @convert_from("exclude")
     def excludes(self, value: list[str]) -> None:
         self.settings.setdefault("build", {})["excludes"] = value
         raise Unset()
 
     @convert_from("build")
     def build(self, value: str | dict) -> None:
-        run_setuptools = True
+        value = {}
         if isinstance(value, dict):
             if "generate-setup-file" in value:
-                run_setuptools = cast(bool, value["generate-setup-file"])
-            value = value["script"]
-        self.settings.setdefault("build", {}).update({"setup-script": value, "run-setuptools": run_setuptools})
+                value["run-setuptools"] = cast(bool, value["generate-setup-file"])
+        self.settings.setdefault("build", {}).update(value)
         raise Unset()
 
     @convert_from("source")
     def sources(self, value: list[dict[str, Any]]) -> None:
         self.settings["source"] = [
             {
                 "name": item.get("name", ""),
```

### Comparing `pdm-2.6.1/src/pdm/formats/requirements.py` & `pdm-2.7.0/src/pdm/formats/requirements.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from __future__ import annotations
 
 import argparse
 import dataclasses
 import hashlib
 import shlex
 import urllib.parse
-from argparse import Namespace
-from os import PathLike
-from typing import Any, Mapping
+from typing import TYPE_CHECKING, Any, Mapping
 
 from pdm.formats.base import make_array
-from pdm.models.candidates import Candidate
 from pdm.models.requirements import Requirement, parse_requirement
-from pdm.project import Project
-from pdm.utils import expand_env_vars_in_auth
+
+if TYPE_CHECKING:
+    from argparse import Namespace
+    from os import PathLike
+
+    from pdm.models.candidates import Candidate
+    from pdm.project import Project
 
 
 class RequirementParser:
     """Reference:
     https://pip.pypa.io/en/stable/reference/requirements-file-format/
     """
 
@@ -168,28 +170,30 @@
 
 
 def export(
     project: Project,
     candidates: list[Candidate] | list[Requirement],
     options: Namespace,
 ) -> str:
+    from pdm.models.candidates import Candidate
+
     lines = ["# This file is @generated by PDM.\n# Please do not edit it manually.\n\n"]
-    for candidate in sorted(candidates, key=lambda x: x.identify()):
+    for candidate in sorted(candidates, key=lambda x: x.identify()):  # type: ignore[attr-defined]
         if isinstance(candidate, Candidate):
             req = dataclasses.replace(candidate.req, specifier=f"=={candidate.version}", marker=None)
         else:
             assert isinstance(candidate, Requirement)
             req = candidate
         lines.append(project.backend.expand_line(req.as_line()))
         if options.hashes and getattr(candidate, "hashes", None):
             for item in sorted(set(candidate.hashes.values())):  # type: ignore[attr-defined]
                 lines.append(f" \\\n    --hash={item}")
         lines.append("\n")
     sources = project.pyproject.settings.get("source", [])
     for source in sources:
-        url = expand_env_vars_in_auth(source["url"])
+        url = source["url"]
         prefix = "--index-url" if source["name"] == "pypi" else "--extra-index-url"
         lines.append(f"{prefix} {url}\n")
         if not source.get("verify_ssl", True):
             host = urllib.parse.urlparse(url).hostname
             lines.append(f"--trusted-host {host}\n")
     return "".join(lines)
```

### Comparing `pdm-2.6.1/src/pdm/formats/setup_py.py` & `pdm-2.7.0/src/pdm/formats/setup_py.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 
 import os
 from pathlib import Path
-from typing import Any, Mapping
+from typing import TYPE_CHECKING, Any, Mapping
 
 from pdm.formats.base import array_of_inline_tables, make_array, make_inline_table
-from pdm.project import Project
+
+if TYPE_CHECKING:
+    from pdm.project import Project
 
 
 def check_fingerprint(project: Project, filename: Path) -> bool:
     return os.path.basename(filename) == "setup.py"
 
 
 def convert(project: Project, filename: Path, options: Any | None) -> tuple[Mapping[str, Any], Mapping[str, Any]]:
```

### Comparing `pdm-2.6.1/src/pdm/installers/core.py` & `pdm-2.7.0/src/pdm/installers/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pdm.installers.synchronizers import BaseSynchronizer
 from pdm.models.requirements import Requirement
 from pdm.models.specifiers import PySpecSet
 from pdm.resolver.core import resolve
 
 
 def install_requirements(
-    reqs: list[Requirement], environment: BaseEnvironment, clean: bool = False
+    reqs: list[Requirement], environment: BaseEnvironment, clean: bool = False, use_install_cache: bool = False
 ) -> None:  # pragma: no cover
     """Resolve and install the given requirements into the environment."""
     project = environment.project
     # Rewrite the python requires to only resolve for the current python version.
     environment.python_requires = PySpecSet(f"=={environment.interpreter.version}")
     provider = project.get_provider(ignore_compatibility=False)
     reporter = project.get_reporter(reqs)
@@ -24,9 +24,9 @@
             req.relocate(backend)  # type: ignore[attr-defined]
     resolved, _ = resolve(
         resolver,
         reqs,
         environment.python_requires,
         max_rounds=resolve_max_rounds,
     )
-    syncer = BaseSynchronizer(resolved, environment, clean=clean, retry_times=0)
+    syncer = BaseSynchronizer(resolved, environment, clean=clean, retry_times=0, use_install_cache=use_install_cache)
     syncer.synchronize()
```

### Comparing `pdm-2.6.1/src/pdm/installers/installers.py` & `pdm-2.7.0/src/pdm/installers/installers.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,28 +46,25 @@
 
 @lru_cache()
 def _is_namespace_package(root: str) -> bool:
     if not _is_python_package(root):
         return False
     if not os.path.exists(os.path.join(root, "__init__.py")):  # PEP 420 style
         return True
-    int_py_lines = [
-        line.strip()
-        for line in Path(root, "__init__.py").open(encoding="utf-8")
-        if line.strip() and not line.strip().startswith("#")
-    ]
+    with Path(root, "__init__.py").open(encoding="utf-8") as f:
+        init_py_lines = [line.strip() for line in f if line.strip() and not line.strip().startswith("#")]
     namespace_identifiers = [
         # pkg_resources style
         "__import__('pkg_resources').declare_namespace(__name__)",
         # pkgutil style
         "__path__ = __import__('pkgutil').extend_path(__path__, __name__)",
     ]
     checker = namespace_identifiers[:]
     checker.extend(item.replace("'", '"') for item in namespace_identifiers)
-    return any(line in checker for line in int_py_lines)
+    return any(line in checker for line in init_py_lines)
 
 
 def _create_symlinks_recursively(source: str, destination: str) -> Iterable[str]:
     """Create symlinks recursively from source to destination.
     Caveats: This don't work for pkgutil or pkg_resources namespace packages.
     package  <-- link
         __init__.py
```

### Comparing `pdm-2.6.1/src/pdm/installers/manager.py` & `pdm-2.7.0/src/pdm/installers/manager.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/installers/packages.py` & `pdm-2.7.0/src/pdm/installers/packages.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/installers/synchronizers.py` & `pdm-2.7.0/src/pdm/installers/synchronizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,23 +107,26 @@
         dry_run: bool = False,
         retry_times: int = 1,
         install_self: bool = False,
         no_editable: bool | Collection[str] = False,
         reinstall: bool = False,
         only_keep: bool = False,
         fail_fast: bool = False,
+        use_install_cache: bool | None = None,
     ) -> None:
         self.requested_candidates = candidates
         self.environment = environment
         self.clean = clean
         self.dry_run = dry_run
         self.retry_times = retry_times
         self.no_editable = no_editable
         self.install_self = install_self
-        self.use_install_cache = environment.project.config["install.cache"]
+        if use_install_cache is None:
+            use_install_cache = environment.project.config["install.cache"]
+        self.use_install_cache = use_install_cache
         self.reinstall = reinstall
         self.only_keep = only_keep
         self.parallel = environment.project.config["install.parallel"]
         self.fail_fast = fail_fast
 
         self.working_set = environment.get_working_set()
         self.ui = environment.project.core.ui
```

### Comparing `pdm-2.6.1/src/pdm/installers/uninstallers.py` & `pdm-2.7.0/src/pdm/installers/uninstallers.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,16 @@
             egg_link_path = cast("Path | None", getattr(dist, "link_file", None))
             if not egg_link_path:
                 termui.logger.warn(
                     "No egg link is found for editable distribution %s, do nothing.",
                     dist.metadata["Name"],
                 )
             else:
-                link_pointer = os.path.normcase(egg_link_path.open("rb").readline().decode().strip())
+                with egg_link_path.open("rb") as f:
+                    link_pointer = os.path.normcase(f.readline().decode().strip())
                 if link_pointer != dist_location:
                     raise UninstallError(
                         f"The link pointer in {egg_link_path} doesn't match "
                         f"the location of {dist.metadata['Name']}(at {dist_location}"
                     )
                 instance.add_path(str(egg_link_path))
                 instance.add_pth(link_pointer)
@@ -189,15 +190,16 @@
 
     def add_path(self, path: str) -> None:
         normalized_path = os.path.normcase(os.path.expanduser(os.path.abspath(path)))
         self._paths.add(normalized_path)
         if path.endswith(".py"):
             self._paths.update(_cache_file_from_source(normalized_path))
         elif path.replace("\\", "/").endswith(".dist-info/REFER_TO"):
-            line = open(path, "rb").readline().decode().strip()
+            with open(path, "rb") as f:
+                line = f.readline().decode().strip()
             if line:
                 self.refer_to = line
 
 
 class StashedRemovePaths(BaseRemovePaths):
     """Stash the paths to temporarily location and remove them after commit"""
 
@@ -213,15 +215,16 @@
     def remove(self) -> None:
         self._remove_pth()
         self._stash_files()
 
     def _remove_pth(self) -> None:
         if not self._pth_entries:
             return
-        self._saved_pth = open(self._pth_file, "rb").read()
+        with open(self._pth_file, "rb") as f:
+            self._saved_pth = f.read()
         endline = "\r\n" if b"\r\n" in self._saved_pth else "\n"
         lines = self._saved_pth.decode().splitlines()
         for item in self._pth_entries:
             termui.logger.debug("Removing pth entry: %s", item)
             lines.remove(item)
         with open(self._pth_file, "wb") as f:
             f.write((endline.join(lines) + endline).encode("utf8"))
```

### Comparing `pdm-2.6.1/src/pdm/models/backends.py` & `pdm-2.7.0/src/pdm/models/backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/models/caches.py` & `pdm-2.7.0/src/pdm/models/caches.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 import hashlib
 import json
 import os
 from functools import lru_cache
 from pathlib import Path
 from typing import TYPE_CHECKING, BinaryIO, Generic, Iterable, TypeVar, cast
 
-import requests
-from cachecontrol.cache import BaseCache
-from cachecontrol.caches import FileCache
+from cacheyou.cache import BaseCache
+from cacheyou.caches import FileCache
 from packaging.utils import canonicalize_name, parse_wheel_filename
 
 from pdm._types import CandidateInfo
 from pdm.exceptions import PdmException
 from pdm.models.candidates import Candidate
 from pdm.termui import logger
 from pdm.utils import atomic_open_for_write, create_tracked_tempdir
 
 if TYPE_CHECKING:
     from packaging.tags import Tag
+    from requests import Session
     from unearth import Link, TargetPython
 
 KT = TypeVar("KT")
 VT = TypeVar("VT")
 
 
 class JSONFileCache(Generic[KT, VT]):
@@ -104,34 +104,36 @@
 
     FAVORITE_HASH = "sha256"
     STRONG_HASHES = ["sha256", "sha384", "sha512"]
 
     def __init__(self, directory: Path) -> None:
         self.directory = directory
 
-    def _read_from_link(self, link: Link, session: requests.Session) -> Iterable[bytes]:
+    def _read_from_link(self, link: Link, session: Session) -> Iterable[bytes]:
         if link.is_file:
             with open(link.file_path, "rb") as f:
                 yield from f
         else:
-            resp = session.get(link.normalized, stream=True)
-            try:
-                resp.raise_for_status()
-            except requests.HTTPError as e:
-                raise PdmException(f"Failed to read from {link.redacted}: {e}") from e
-            yield from resp.iter_content(chunk_size=8096)
+            import requests
+
+            with session.get(link.normalized, stream=True) as resp:
+                try:
+                    resp.raise_for_status()
+                except requests.HTTPError as e:
+                    raise PdmException(f"Failed to read from {link.redacted}: {e}") from e
+                yield from resp.iter_content(chunk_size=8192)
 
-    def _get_file_hash(self, link: Link, session: requests.Session) -> str:
+    def _get_file_hash(self, link: Link, session: Session) -> str:
         h = hashlib.new(self.FAVORITE_HASH)
         logger.debug("Downloading link %s for calculating hash", link.redacted)
         for chunk in self._read_from_link(link, session):
             h.update(chunk)
         return ":".join([h.name, h.hexdigest()])
 
-    def get_hash(self, link: Link, session: requests.Session) -> str:
+    def get_hash(self, link: Link, session: Session) -> str:
         # If there is no link hash (i.e., md5, sha256, etc.), we don't want
         # to store it.
         hash_value = self.get(link.url_without_fragment)
         if not hash_value:
             if link.hashes and link.hashes.keys() & self.STRONG_HASHES:
                 logger.debug("Using hash in link for %s", link.redacted)
                 hash_name = next(k for k in self.STRONG_HASHES if k in link.hashes)
```

### Comparing `pdm-2.6.1/src/pdm/models/candidates.py` & `pdm-2.7.0/src/pdm/models/candidates.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 import dataclasses
+import hashlib
 import os
 import re
 import warnings
 from functools import lru_cache
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import TYPE_CHECKING, Any, Iterable, cast, no_type_check
 from zipfile import ZipFile
 
 from packaging.utils import parse_wheel_filename
-from unearth import Link, vcs_support
 
 from pdm import termui
 from pdm.builders import EditableBuilder, WheelBuilder
 from pdm.compat import cached_property
 from pdm.compat import importlib_metadata as im
 from pdm.exceptions import BuildError, CandidateNotFound, InvalidPyVersion
 from pdm.models.backends import get_backend, get_backend_by_spec
@@ -24,27 +24,26 @@
     Requirement,
     VcsRequirement,
     _egg_info_re,
     filter_requirements_with_extras,
 )
 from pdm.models.setup import Setup
 from pdm.models.specifiers import PySpecSet
-from pdm.project.project_file import PyProject
 from pdm.utils import (
     cd,
     convert_hashes,
     create_tracked_tempdir,
     get_rev_from_url,
     normalize_name,
     path_to_url,
     url_without_fragments,
 )
 
 if TYPE_CHECKING:
-    from unearth import Package, PackageFinder
+    from unearth import Link, Package, PackageFinder
 
     from pdm.environments import BaseEnvironment
 
 
 def _dist_info_files(whl_zip: ZipFile) -> list[str]:
     """Identify the .dist-info folder inside a wheel ZipFile."""
     res = []
@@ -103,14 +102,29 @@
         new_found = attempt_to_find()
         if new_found is not None:
             found = new_found
         finder.ignore_compatibility = False
     return found
 
 
+class MetadataDistribution(im.Distribution):
+    """A wrapper around a single METADATA file to provide the Distribution interface"""
+
+    def __init__(self, text: str) -> None:
+        self.text = text
+
+    def locate_file(self, path: str | os.PathLike[str]) -> os.PathLike[str]:
+        return Path()
+
+    def read_text(self, filename: str) -> str | None:
+        if filename != "":
+            return None
+        return self.text
+
+
 class Candidate:
     """A concrete candidate that can be downloaded and installed.
     A candidate comes from the PyPI index of a package, or from the requirement itself
     (for file or VCS requirements). Each candidate has a name, version and several
     dependencies together with package metadata.
     """
 
@@ -139,15 +153,15 @@
         :param version: the version of the candidate.
         :param link: the file link of the candidate.
         """
         self.req = req
         self.name = name or self.req.project_name
         self.version = version
         if link is None and not req.is_named:
-            link = cast(Link, req.as_file_link())  # type: ignore[attr-defined]
+            link = cast("Link", req.as_file_link())  # type: ignore[attr-defined]
         self.link = link
         self.summary = ""
         self.hashes: dict[Link, str] | None = None
 
         self._requires_python: str | None = None
         self._prepared: PreparedCandidate | None = None
 
@@ -289,14 +303,16 @@
         if link is None:
             return None
         url = self.environment.project.backend.expand_line(link.normalized)
         return dataclasses.replace(link, url=url)
 
     @cached_property
     def revision(self) -> str:
+        from unearth import vcs_support
+
         if not (self._source_dir and os.path.exists(self._source_dir)):
             # It happens because the cached wheel is hit and the source code isn't
             # pulled to local. In this case the link url must contain the full commit
             # hash which can be taken as the revision safely.
             # See more info at https://github.com/pdm-project/pdm/issues/349
             rev = get_rev_from_url(self.candidate.link.url)  # type: ignore[union-attr]
             if rev:
@@ -369,27 +385,26 @@
         builder = builder_cls(str(self._unpacked_dir), self.environment)
         build_dir = self._get_wheel_dir()
         os.makedirs(build_dir, exist_ok=True)
         termui.logger.info("Running PEP 517 backend to build a wheel for %s", self.link)
         self.wheel = Path(builder.build(build_dir, metadata_directory=self._metadata_dir))
         return self.wheel
 
-    def obtain(self, allow_all: bool = False) -> None:
+    def obtain(self, allow_all: bool = False, unpack: bool = True) -> None:
         """Fetch the link of the candidate and unpack to local if necessary.
 
         :param allow_all: If true, don't validate the wheel tag nor hashes
+        :param unpack: Whether to download and unpack the link if it's not local
         """
         if self.wheel:
             if self._wheel_compatible(self.wheel.name, allow_all):
                 return
         elif self._source_dir and self._source_dir.exists():
             return
-        hash_options = None
-        if not allow_all and self.candidate.hashes:
-            hash_options = convert_hashes(self.candidate.hashes)
+
         with self.environment.get_finder() as finder:
             if not self.link or self.link.is_wheel and not self._wheel_compatible(self.link.filename, allow_all):
                 if self.req.is_file_or_url:
                     raise CandidateNotFound(f"The URL requirement {self.req.as_line()} is a wheel but incompatible")
                 self.link = self.wheel = None  # reset the incompatible wheel
                 self.link = _find_best_match_link(
                     finder,
@@ -404,87 +419,136 @@
                 if not self.candidate.link:
                     self.candidate.link = self.link
             if allow_all and not self.req.editable:
                 cached = self._get_cached_wheel()
                 if cached:
                     self.wheel = cached
                     return
+            if unpack:
+                self._unpack(validate_hashes=not allow_all)
+
+    def _unpack(self, validate_hashes: bool = False) -> None:
+        hash_options = None
+        if validate_hashes and self.candidate.hashes:
+            hash_options = convert_hashes(self.candidate.hashes)
+        assert self.link is not None
+        with self.environment.get_finder() as finder:
             with TemporaryDirectory(prefix="pdm-download-") as tmpdir:
                 build_dir = self._get_build_dir()
                 if self.link.is_wheel:
                     download_dir = build_dir
                 else:
                     download_dir = tmpdir
                 result = finder.download_and_unpack(self.link, build_dir, download_dir, hash_options)
                 if self.link.is_wheel:
                     self.wheel = result
                 else:
                     self._source_dir = Path(build_dir)
                     self._unpacked_dir = result
 
     def prepare_metadata(self, force_build: bool = False) -> im.Distribution:
-        self.obtain(allow_all=True)
-        metadir_parent = create_tracked_tempdir(prefix="pdm-meta-")
+        self.obtain(allow_all=True, unpack=False)
+
+        metadata_parent = create_tracked_tempdir(prefix="pdm-meta-")
         if self.wheel:
-            # Get metadata from METADATA inside the wheel
-            self._metadata_dir = _get_wheel_metadata_from_wheel(self.wheel, metadir_parent)
-            return im.PathDistribution(Path(self._metadata_dir))
+            return self._get_metadata_from_wheel(self.wheel, metadata_parent)
+
+        assert self.link is not None
+        if self.link.dist_info_metadata:
+            assert self.link.dist_info_link
+            dist = self._get_metadata_from_metadata_link(self.link.dist_info_link, self.link.dist_info_metadata)
+            if dist is not None:
+                return dist
+
+        self._unpack(validate_hashes=False)
+        if self.wheel:  # check again if the wheel is downloaded to local
+            return self._get_metadata_from_wheel(self.wheel, metadata_parent)
 
         assert self._unpacked_dir, "Source directory isn't ready yet"
-        # Try getting from PEP 621 metadata
         pyproject_toml = self._unpacked_dir / "pyproject.toml"
-        if pyproject_toml.exists() and not force_build:
-            pyproject = PyProject(pyproject_toml, ui=self.environment.project.core.ui)
-            metadata = pyproject.metadata.unwrap()
-            if not metadata:
-                termui.logger.warn("Failed to parse pyproject.toml")
-            else:
-                dynamic_fields = metadata.get("dynamic", [])
-                # Use the parse result only when all are static
-                if set(dynamic_fields).isdisjoint(
-                    {
-                        "name",
-                        "version",
-                        "dependencies",
-                        "optional-dependencies",
-                        "requires-python",
-                    }
-                ):
-                    try:
-                        backend_cls = get_backend_by_spec(pyproject.build_system)
-                    except Exception:
-                        # no variable expansion
-                        backend_cls = get_backend("setuptools")
-                    backend = backend_cls(self._unpacked_dir)
-                    setup = Setup(
-                        name=metadata.get("name"),
-                        summary=metadata.get("description"),
-                        version=metadata.get("version"),
-                        install_requires=list(
-                            map(
-                                backend.expand_line,
-                                metadata.get("dependencies", []),
-                            )
-                        ),
-                        extras_require={
-                            k: list(map(backend.expand_line, v))
-                            for k, v in metadata.get("optional-dependencies", {}).items()
-                        },
-                        python_requires=metadata.get("requires-python"),
-                    )
-                    return setup.as_dist()
+        if not force_build and pyproject_toml.exists():
+            dist = self._get_metadata_from_project(pyproject_toml)
+            if dist is not None:
+                return dist
+
         # If all fail, try building the source to get the metadata
+        return self._get_metadata_from_build(self._unpacked_dir, metadata_parent)
+
+    def _get_metadata_from_metadata_link(
+        self, link: Link, medata_hash: bool | dict[str, str] | None
+    ) -> im.Distribution | None:
+        with self.environment.get_finder() as finder:
+            resp = finder.session.get(link.normalized, headers={"Cache-Control": "max-age=0"})
+            if isinstance(medata_hash, dict):
+                hash_name, hash_value = next(iter(medata_hash.items()))
+                if hashlib.new(hash_name, resp.content).hexdigest() != hash_value:
+                    termui.logger.warn("Metadata hash mismatch for %s, ignoring the metadata", link)
+                    return None
+            return MetadataDistribution(resp.text)
+
+    def _get_metadata_from_wheel(self, wheel: Path, metadata_parent: str) -> im.Distribution:
+        # Get metadata from METADATA inside the wheel
+        self._metadata_dir = _get_wheel_metadata_from_wheel(wheel, metadata_parent)
+        return im.PathDistribution(Path(self._metadata_dir))
+
+    def _get_metadata_from_project(self, pyproject_toml: Path) -> im.Distribution | None:
+        # Try getting from PEP 621 metadata
+        from pdm.project.project_file import PyProject
+
+        pyproject = PyProject(pyproject_toml, ui=self.environment.project.core.ui)
+        metadata = pyproject.metadata.unwrap()
+        if not metadata:
+            termui.logger.warn("Failed to parse pyproject.toml")
+            return None
+
+        dynamic_fields = metadata.get("dynamic", [])
+        # Use the parse result only when all are static
+        if not set(dynamic_fields).isdisjoint(
+            {
+                "name",
+                "version",
+                "dependencies",
+                "optional-dependencies",
+                "requires-python",
+            }
+        ):
+            return None
+
+        try:
+            backend_cls = get_backend_by_spec(pyproject.build_system)
+        except Exception:
+            # no variable expansion
+            backend_cls = get_backend("setuptools")
+        backend = backend_cls(pyproject_toml.parent)
+        setup = Setup(
+            name=metadata.get("name"),
+            summary=metadata.get("description"),
+            version=metadata.get("version"),
+            install_requires=list(
+                map(
+                    backend.expand_line,
+                    metadata.get("dependencies", []),
+                )
+            ),
+            extras_require={
+                k: list(map(backend.expand_line, v)) for k, v in metadata.get("optional-dependencies", {}).items()
+            },
+            python_requires=metadata.get("requires-python"),
+        )
+        return setup.as_dist()
+
+    def _get_metadata_from_build(self, source_dir: Path, metadata_parent: str) -> im.Distribution:
         builder = EditableBuilder if self.req.editable else WheelBuilder
         try:
             termui.logger.info("Running PEP 517 backend to get metadata for %s", self.link)
-            self._metadata_dir = builder(self._unpacked_dir, self.environment).prepare_metadata(metadir_parent)
+            self._metadata_dir = builder(source_dir, self.environment).prepare_metadata(metadata_parent)
         except BuildError:
             termui.logger.warn("Failed to build package, try parsing project files.")
             try:
-                setup = Setup.from_directory(self._unpacked_dir)
+                setup = Setup.from_directory(source_dir)
             except Exception:
                 message = "Failed to parse the project files, dependencies may be missing"
                 termui.logger.warn(message)
                 warnings.warn(message, RuntimeWarning, stacklevel=1)
                 setup = Setup()
             return setup.as_dist()
         else:
@@ -508,14 +572,16 @@
         extras = self.req.extras or ()
         return filter_requirements_with_extras(
             self.req.project_name, self.metadata.requires or [], extras  # type: ignore[arg-type]
         )
 
     def should_cache(self) -> bool:
         """Determine whether to cache the dependencies and built wheel."""
+        from unearth import vcs_support
+
         link, source_dir = self.candidate.link, self._source_dir
         if self.req.editable:
             return False
         if self.req.is_named:
             return True
         if self.req.is_vcs:
             if not source_dir:
```

### Comparing `pdm-2.6.1/src/pdm/models/in_process/__init__.py` & `pdm-2.7.0/src/pdm/models/in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/models/in_process/get_abi_tag.py` & `pdm-2.7.0/src/pdm/models/in_process/get_abi_tag.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/models/in_process/parse_setup.py` & `pdm-2.7.0/src/pdm/models/in_process/parse_setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/models/in_process/pep508.py` & `pdm-2.7.0/src/pdm/models/in_process/pep508.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/models/in_process/sysconfig_get_paths.py` & `pdm-2.7.0/src/pdm/models/in_process/sysconfig_get_paths.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/models/markers.py` & `pdm-2.7.0/src/pdm/models/markers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/models/project_info.py` & `pdm-2.7.0/src/pdm/models/project_info.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/models/python.py` & `pdm-2.7.0/src/pdm/models/python.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 from __future__ import annotations
 
 import os
 from pathlib import Path
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
-from findpython import PythonVersion
 from packaging.version import InvalidVersion, Version
 
 from pdm.compat import cached_property
 from pdm.models.venv import VirtualEnv
 
+if TYPE_CHECKING:
+    from findpython import PythonVersion
+
 
 class PythonInfo:
     """
     A convenient helper class that holds all information of a Python interepreter.
     """
 
     def __init__(self, py_version: PythonVersion) -> None:
         self._py_ver = py_version
 
     @classmethod
     def from_path(cls, path: str | Path) -> PythonInfo:
+        from findpython import PythonVersion
+
         py_ver = PythonVersion(Path(path))
         return cls(py_ver)
 
     @cached_property
     def valid(self) -> bool:
         return self._py_ver.executable.exists() and self._py_ver.is_valid()
```

### Comparing `pdm-2.6.1/src/pdm/models/repositories.py` & `pdm-2.7.0/src/pdm/models/repositories.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 
 import dataclasses
 import posixpath
 import sys
 from functools import wraps
 from typing import TYPE_CHECKING, Any, Callable, Iterable, Mapping, TypeVar, cast
 
-from unearth import Link
-from unearth.utils import LazySequence
-
 from pdm import termui
 from pdm.exceptions import CandidateInfoNotFound, CandidateNotFound
 from pdm.models.candidates import Candidate, make_candidate
 from pdm.models.requirements import (
     Requirement,
     filter_requirements_with_extras,
     parse_requirement,
@@ -24,14 +21,16 @@
     normalize_name,
     path_to_url,
     url_to_path,
     url_without_fragments,
 )
 
 if TYPE_CHECKING:
+    from unearth import Link
+
     from pdm._types import CandidateInfo, RepositoryConfig, SearchResult
     from pdm.environments import BaseEnvironment
 
 ALLOW_ALL_PYTHON = PySpecSet()
 T = TypeVar("T", bound="BaseRepository")
 
 
@@ -119,14 +118,16 @@
         project = self.environment.project
         return requirement.is_named and project.name is not None and requirement.key == normalize_name(project.name)
 
     def make_this_candidate(self, requirement: Requirement) -> Candidate:
         """Make a candidate for this package.
         In this case the finder will look for a candidate from the package sources
         """
+        from unearth import Link
+
         project = self.environment.project
         assert project.name
         link = Link.from_path(project.root)
         candidate = make_candidate(requirement, project.name, link=link)
         candidate.prepare(self.environment).metadata
         return candidate
 
@@ -137,14 +138,15 @@
         ignore_requires_python: bool = False,
     ) -> Iterable[Candidate]:
         """Find candidates of the given NamedRequirement. Let it to be implemented in
         subclasses.
         """
         # `allow_prereleases` is None means leave it to specifier to decide whether to
         # include prereleases
+        from unearth.utils import LazySequence
 
         if self.is_this_package(requirement):
             return [self.make_this_candidate(requirement)]
         requires_python = requirement.requires_python & self.environment.python_requires
         cans = LazySequence(self._find_candidates(requirement))
         applicable_cans = LazySequence(
             c
@@ -219,15 +221,15 @@
         """Adds the local package as a candidate only if the candidate
         name is the same as the local package."""
         project = self.environment.project
         if not project.name or candidate.name != project.name:
             raise CandidateInfoNotFound(candidate) from None
 
         reqs = project.pyproject.metadata.get("dependencies", [])
-        extra_dependencies = project.pyproject.settings.get("dev-dependencies", {})
+        extra_dependencies = project.pyproject.settings.get("dev-dependencies", {}).copy()
         extra_dependencies.update(project.pyproject.metadata.get("optional-dependencies", {}))
         if candidate.req.extras is not None:
             reqs = sum(
                 (extra_dependencies.get(g, []) for g in candidate.req.extras),
                 [],
             )
 
@@ -247,26 +249,26 @@
             and candidate.req.is_local_dir  # type: ignore[attr-defined]
         ):
             return None
         if candidate.hashes:
             return candidate.hashes
         req = candidate.req.as_pinned_version(candidate.version)
         comes_from = candidate.link.comes_from if candidate.link else None
-        result: dict[str, str] = {}
+        result: dict[Link, str] = {}
         logged = False
         respect_source_order = self.environment.project.pyproject.settings.get("resolution", {}).get(
             "respect-source-order", False
         )
         if req.is_named and respect_source_order and comes_from:
             sources = [s for s in self.sources if comes_from.startswith(s.url)]
         else:
             sources = self.sources
         with self.environment.get_finder(sources, self.ignore_compatibility) as finder:
             if req.is_file_or_url:
-                this_link = cast(Link, candidate.prepare(self.environment).link)
+                this_link = cast("Link", candidate.prepare(self.environment).link)
                 links: list[Link] = [this_link]
             else:  # the req must be a named requirement
                 links = [package.link for package in finder.find_matches(req.as_line())]
             for link in links:
                 if not link or link.is_vcs or link.is_file and link.file_path.is_dir():
                     # The links found can still be a local directory or vcs, skippping it.
                     continue
@@ -335,14 +337,16 @@
         yield self._get_dependencies_from_cache
         yield self._get_dependency_from_local_package
         if self.environment.project.config["pypi.json_api"]:
             yield self._get_dependencies_from_json
         yield self._get_dependencies_from_metadata
 
     def _find_candidates(self, requirement: Requirement) -> Iterable[Candidate]:
+        from unearth.utils import LazySequence
+
         sources = self.get_filtered_sources(requirement)
         with self.environment.get_finder(sources, self.ignore_compatibility) as finder:
             cans = LazySequence(
                 Candidate.from_installation_candidate(c, requirement)
                 for c in finder.find_all_packages(requirement.project_name, allow_yanked=requirement.is_pinned)
             )
         if not cans:
@@ -392,14 +396,16 @@
         self._read_lockfile(lockfile)
 
     @property
     def all_candidates(self) -> dict[str, Candidate]:
         return {can.req.identify(): can for can in self.packages.values()}
 
     def _read_lockfile(self, lockfile: Mapping[str, Any]) -> None:
+        from unearth import Link
+
         root = self.environment.project.root
         with cd(root):
             for package in lockfile.get("package", []):
                 version = package.get("version")
                 if version:
                     package["version"] = f"=={version}"
                 package_name = package.pop("name")
```

### Comparing `pdm-2.6.1/src/pdm/models/requirements.py` & `pdm-2.7.0/src/pdm/models/requirements.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from typing import TYPE_CHECKING, Any, Sequence, TypeVar, cast
 
 from packaging.markers import InvalidMarker
 from packaging.requirements import InvalidRequirement
 from packaging.requirements import Requirement as PackageRequirement
 from packaging.specifiers import SpecifierSet
 from packaging.utils import parse_sdist_filename, parse_wheel_filename
-from unearth import Link
 
 from pdm.compat import Distribution
 from pdm.exceptions import ExtrasWarning, RequirementError
 from pdm.models.backends import BuildBackend, get_relative_path
 from pdm.models.markers import Marker, get_marker, split_marker_extras
 from pdm.models.setup import Setup
 from pdm.models.specifiers import PySpecSet, fix_legacy_specifier, get_specifier
@@ -34,14 +33,16 @@
     path_to_url,
     path_without_fragments,
     url_to_path,
     url_without_fragments,
 )
 
 if TYPE_CHECKING:
+    from unearth import Link
+
     from pdm._types import RequirementDict
 
 
 VCS_SCHEMA = ("git", "hg", "svn", "bzr")
 _vcs_req_re = re.compile(
     rf"(?P<url>(?P<vcs>{'|'.join(VCS_SCHEMA)})\+[^\s;]+)(?P<marker>[\t ]*;[^\n]+)?",
     flags=re.IGNORECASE,
@@ -210,14 +211,16 @@
             req = parse_requirement(line.split("-e ", 1)[-1], True)
         else:
             req = parse_requirement(line, False)
         return self.key == req.key
 
     @classmethod
     def from_pkg_requirement(cls, req: PackageRequirement) -> Requirement:
+        from unearth import Link
+
         kwargs = {
             "name": req.name,
             "extras": req.extras,
             "specifier": req.specifier,
             "marker": get_marker(req.marker),
         }
         if getattr(req, "url", None):
@@ -225,15 +228,15 @@
             klass = VcsRequirement if link.is_vcs else FileRequirement
             return klass(url=req.url, **kwargs)
         else:
             return NamedRequirement(**kwargs)  # type: ignore[arg-type]
 
     def _format_marker(self) -> str:
         if self.marker:
-            return f"; {str(self.marker)}"
+            return f"; {self.marker!s}"
         return ""
 
 
 @dataclasses.dataclass(eq=False)
 class NamedRequirement(Requirement):
     def as_line(self) -> str:
         extras = f"[{','.join(sorted(self.extras))}]" if self.extras else ""
@@ -307,14 +310,16 @@
         return self.path and self.path.exists() or False
 
     @property
     def is_local_dir(self) -> bool:
         return self.is_local and cast(Path, self.path).is_dir()
 
     def as_file_link(self) -> Link:
+        from unearth import Link
+
         url = self.get_full_url()
         # only subdirectory is useful in a file link
         if self.subdirectory:
             url += f"#subdirectory={self.subdirectory}"
         return Link(url)
 
     def get_full_url(self) -> str:
```

### Comparing `pdm-2.6.1/src/pdm/models/search.py` & `pdm-2.7.0/src/pdm/models/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/models/session.py` & `pdm-2.7.0/src/pdm/models/session.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,29 @@
 import functools
 from pathlib import Path
 from typing import Any
 
-from cachecontrol.adapter import CacheControlAdapter
-from cachecontrol.serialize import Serializer as LegacySerializer
+from cacheyou.adapter import CacheControlAdapter
 from requests_toolbelt.utils import user_agent
 from unearth.session import InsecureMixin, PyPISession
 
 from pdm.__version__ import __version__
 
 
-class Serializer(LegacySerializer):
-    """Patch for the compatibility of cachecontrol serializer.
-    It should be removed when cachecontrol supports urllib3 2.0.
-    """
-
-    def dumps(self, request, response, body=None):  # type: ignore[no-untyped-def]
-        if not hasattr(response, "strict"):
-            # XXX: urllib3 2.0 removes this attribute
-            response.strict = False
-        return super().dumps(request, response, body)
-
-    def prepare_response(self, request, cached, body_file=None):  # type: ignore[no-untyped-def]
-        # We don't need to pass strict to HTTPResponse
-        cached["response"].pop("strict", None)
-        # urllib3 2.0 changes the default to True, which causes a double read issue
-        # See https://github.com/ionrock/cachecontrol/issues/295
-        cached["response"]["enforce_content_length"] = False
-        return super().prepare_response(request, cached, body_file)
-
-
 class InsecureCacheControlAdapter(InsecureMixin, CacheControlAdapter):
     pass
 
 
 class PDMSession(PyPISession):
     def __init__(self, *, cache_dir: Path, **kwargs: Any) -> None:
         from pdm.models.caches import SafeFileCache
 
         cache = SafeFileCache(str(cache_dir))
-        serializer = Serializer()
-        self.secure_adapter_cls = functools.partial(CacheControlAdapter, cache=cache, serializer=serializer)
-        self.insecure_adapter_cls = functools.partial(InsecureCacheControlAdapter, cache=cache, serializer=serializer)
+        self.secure_adapter_cls = functools.partial(CacheControlAdapter, cache=cache)
+        self.insecure_adapter_cls = functools.partial(InsecureCacheControlAdapter, cache=cache)
         super().__init__(**kwargs)
         self.headers["User-Agent"] = self._make_user_agent()
 
     def _make_user_agent(self) -> str:
         return user_agent.UserAgentBuilder("pdm", __version__).include_implementation().build()
 
     # HACK: make the sessions identical to functools.lru_cache
```

### Comparing `pdm-2.6.1/src/pdm/models/setup.py` & `pdm-2.7.0/src/pdm/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/models/specifiers.py` & `pdm-2.7.0/src/pdm/models/specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/models/venv.py` & `pdm-2.7.0/src/pdm/models/venv.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/models/versions.py` & `pdm-2.7.0/src/pdm/models/versions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from __future__ import annotations
 
 import re
-from typing import Any, Union, overload
+from typing import TYPE_CHECKING, overload
 
-from pdm.compat import Literal
 from pdm.exceptions import InvalidPyVersion
 
-VersionBit = Union[int, Literal["*"]]  # noqa: F722
+if TYPE_CHECKING:
+    from typing import Any, Literal, Union
+
+    VersionBit = Union[int, Literal["*"]]
+
 PRE_RELEASE_SEGMENT_RE = re.compile(
     r"(?P<digit>\d+)(?P<type>a|b|rc)(?P<n>\d*)",
     flags=re.IGNORECASE,
 )
 
 
 class Version:
```

### Comparing `pdm-2.6.1/src/pdm/models/working_set.py` & `pdm-2.7.0/src/pdm/models/working_set.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/pep582/sitecustomize.py` & `pdm-2.7.0/src/pdm/pep582/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/project/config.py` & `pdm-2.7.0/src/pdm/project/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import tomlkit
 
 from pdm import termui
 from pdm._types import RepositoryConfig
 from pdm.exceptions import NoConfigError, PdmUsageError
 
 REPOSITORY = "repository"
+SOURCE = "pypi"
 DEFAULT_REPOSITORIES = {
     "pypi": "https://upload.pypi.org/legacy/",
     "testpypi": "https://test.pypi.org/legacy/",
 }
 
 ui = termui.UI()
 
@@ -28,17 +29,17 @@
 
     E.g. ["python"]["use_venv"] will be loaded as "python.use_venv" key.
     """
 
     def get_item(sub_data: Mapping[str, Any]) -> dict[str, Any]:
         result: dict[str, Any] = {}
         for k, v in sub_data.items():
-            if k == "pypi":
+            if k in (REPOSITORY, SOURCE):
                 result.update((f"{k}.{sub_k}", sub_v) for sub_k, sub_v in v.items())
-            elif k != REPOSITORY and isinstance(v, Mapping):
+            elif isinstance(v, Mapping):
                 result.update({f"{k}.{sub_k}": sub_v for sub_k, sub_v in get_item(v).items()})
             else:
                 result.update({k: v})
         return result
 
     if not file_path.is_file():
         return {}
@@ -244,18 +245,18 @@
             raise PdmUsageError("Theme can only be loaded from global config")
         return rich.theme.Theme({k[6:]: v for k, v in self.items() if k.startswith("theme.")})
 
     @property
     def self_data(self) -> dict[str, Any]:
         return dict(self._file_data)
 
-    def iter_sources(self) -> Iterator[tuple[str, RepositoryConfig]]:
+    def iter_sources(self) -> Iterator[RepositoryConfig]:
         for name, data in self._data.items():
-            if name.startswith("pypi.") and name not in self._config_map:
-                yield name[5:], RepositoryConfig(**data)
+            if name.startswith(f"{SOURCE}.") and name not in self._config_map:
+                yield RepositoryConfig(**data, name=name[len(SOURCE) + 1 :], config_prefix=SOURCE)
 
     def _save_config(self) -> None:
         """Save the changed to config file."""
         self.config_file.parent.mkdir(parents=True, exist_ok=True)
         toml_data: dict[str, Any] = {}
         for key, value in self._file_data.items():
             *parts, last = key.split(".")
@@ -267,29 +268,23 @@
             temp[last] = value
 
         with self.config_file.open("w", encoding="utf-8") as fp:
             tomlkit.dump(toml_data, fp)
 
     def __getitem__(self, key: str) -> Any:
         parts = key.split(".")
-        if parts[0] == REPOSITORY:
+        if parts[0] in (REPOSITORY, SOURCE) and key not in self._config_map:
             if len(parts) < 2:
-                raise PdmUsageError("Must specify a repository name")
-            repo = self.get_repository_config(parts[1])
+                raise PdmUsageError(f"Must specify a {parts[0]} name")
+            repo = self.get_repository_config(parts[1], parts[0])
             if repo is None:
-                raise KeyError(f"No repository named {parts[1]}")
+                raise KeyError(f"No {parts[0]} named {parts[1]}")
 
             value = getattr(repo, parts[2]) if len(parts) >= 3 else repo
             return value
-        elif parts[0] == "pypi" and key not in self._config_map and len(parts) >= 2:
-            index_key = ".".join(parts[:2])
-            if index_key not in self._data:
-                raise KeyError(f"No PyPI index named {parts[1]}")
-            source = self._data[index_key]
-            return source[parts[2]] if len(parts) >= 3 else RepositoryConfig(**self._data[index_key])
 
         if key not in self._config_map and key not in self.deprecated:
             raise NoConfigError(key)
         config_key = self.deprecated.get(key, key)
         config = self._config_map[config_key]
         env_var = config.env_var
         if env_var is not None and env_var in os.environ:
@@ -300,28 +295,31 @@
             elif config.replace:
                 result = self._data[config.replace]
             else:
                 raise NoConfigError(key) from None
         return config.coerce(result)
 
     def __setitem__(self, key: str, value: Any) -> None:
+        from pdm.models.auth import keyring
+
         parts = key.split(".")
-        if parts[0] == REPOSITORY:
+        if parts[0] in (REPOSITORY, SOURCE) and key not in self._config_map:
             if len(parts) < 3:
-                raise PdmUsageError("Set repository config with [success]repository.{name}.{attr}")
-            self._file_data.setdefault(parts[0], {}).setdefault(parts[1], {}).setdefault(parts[2], value)
-            self._save_config()
-            return
-        if parts[0] == "pypi" and key not in self._config_map:
-            if len(parts) < 3:
-                raise PdmUsageError("Set index config with [success]pypi.{name}.{attr}")
+                raise PdmUsageError(f"Set {parts[0]} config with [success]{parts[0]}.{{name}}.{{attr}}")
             index_key = ".".join(parts[:2])
+            username = self._data.get(index_key, {}).get("username")
+            service = f'pdm-{index_key.replace(".", "-")}'
+            if parts[2] == "password" and self.is_global and keyring.save_auth_info(service, username, value):
+                return
+            if parts[2] == "verify_ssl":
+                value = ensure_boolean(value)
             self._file_data.setdefault(index_key, {})[parts[2]] = value
             self._save_config()
             return
+
         if key not in self._config_map and key not in self.deprecated:
             raise NoConfigError(key)
         config_key = self.deprecated.get(key, key)
         config = self._config_map[config_key]
         if not self.is_global and config.global_only:
             raise ValueError(f"Config item '{key}' is not allowed to set in project config.")
 
@@ -340,72 +338,76 @@
     def __len__(self) -> int:
         return len(self._data)
 
     def __iter__(self) -> Iterator[str]:
         keys: set[str] = set()
         for key in self._data:
             if key in self.deprecated:
-                keys.add(self.deprecated[key])
-            elif key != REPOSITORY:
-                keys.add(key)
+                key = self.deprecated[key]
+            keys.add(key)
         return iter(keys)
 
     def __delitem__(self, key: str) -> None:
         parts = key.split(".")
-        if parts[0] == REPOSITORY:
-            if len(parts) < 2:
-                raise PdmUsageError("Should specify the name of repository")
-            if len(parts) >= 3:
-                del self._file_data.get(REPOSITORY, {}).get(parts[1], {})[parts[2]]
-            else:
-                del self._file_data.get(REPOSITORY, {})[parts[1]]
-            self._save_config()
-            return
-        if parts[0] == "pypi" and key not in self._config_map:
+        if parts[0] in (REPOSITORY, SOURCE) and key not in self._config_map:
             if len(parts) < 2:
-                raise PdmUsageError("Should specify the name of index")
+                raise PdmUsageError(f"Should specify the name of {parts[0]}")
             if len(parts) >= 3:
                 index_key, attr = key.rsplit(".", 1)
                 del self._file_data.get(index_key, {})[attr]
             else:
                 del self._file_data[key]
             self._save_config()
             return
+
         config_key = self.deprecated.get(key, key)
         config = self._config_map[config_key]
         self._file_data.pop(config_key, None)
         if config.replace:
             self._file_data.pop(config.replace, None)
 
         env_var = config.env_var
         if env_var is not None and env_var in os.environ:
             ui.echo(
                 "WARNING: the config is shadowed by env var '{}', set value won't take effect.".format(env_var),
                 style="warning",
             )
         self._save_config()
 
-    def get_repository_config(self, name_or_url: str) -> RepositoryConfig | None:
-        """Get a repository by name or url."""
-        if not self.is_global:  # pragma: no cover
-            raise NoConfigError("repository")
-        repositories: Mapping[str, RepositoryConfig] = {
-            k: RepositoryConfig(**v) for k, v in self._data.get(REPOSITORY, {}).items()
-        }
+    def get_repository_config(self, name_or_url: str, prefix: str) -> RepositoryConfig | None:
+        """Get a repository or source by name or url."""
+        if not self.is_global and prefix == REPOSITORY:  # pragma: no cover
+            raise NoConfigError(prefix)
+        repositories: dict[str, RepositoryConfig] = {}
+        for k, v in self._data.items():
+            if not k.startswith(f"{prefix}.") or k in self._config_map:
+                continue
+            key = k[len(prefix) + 1 :]
+            repositories[key] = RepositoryConfig(**v, name=key, config_prefix=prefix)
         config: RepositoryConfig | None = None
         if "://" in name_or_url:
             config = next(
                 (v for v in repositories.values() if v.url == name_or_url),
-                RepositoryConfig(name_or_url),
+                RepositoryConfig(url=name_or_url, name="__unknown__", config_prefix=prefix),
             )
         else:
             config = repositories.get(name_or_url)
 
+        if prefix == SOURCE:
+            return config
+
         if name_or_url in DEFAULT_REPOSITORIES:
             if config is None:
-                return RepositoryConfig(DEFAULT_REPOSITORIES[name_or_url])
+                return RepositoryConfig(url=DEFAULT_REPOSITORIES[name_or_url], name=name_or_url, config_prefix=prefix)
             config.passive_update(url=DEFAULT_REPOSITORIES[name_or_url])
         if name_or_url in DEFAULT_REPOSITORIES.values():
+            name = next(k for k, v in DEFAULT_REPOSITORIES.items() if v == name_or_url)
             if config is None:
-                return RepositoryConfig(name_or_url)
+                return RepositoryConfig(
+                    name=name,
+                    config_prefix=prefix,
+                    url=name_or_url,
+                )
             config.passive_update(url=name_or_url)
+            if config.name == "__unknown__":
+                config.name = name
         return config
```

### Comparing `pdm-2.6.1/src/pdm/project/core.py` & `pdm-2.7.0/src/pdm/project/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,28 +5,22 @@
 import os
 import re
 import shutil
 import sys
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Iterable, cast
 
-import platformdirs
 import tomlkit
-from findpython import Finder
 from tomlkit.items import Array
-from unearth import Link
 
 from pdm import termui
 from pdm._types import RepositoryConfig
 from pdm.compat import cached_property
-from pdm.environments import BaseEnvironment, PythonEnvironment, PythonLocalEnvironment
 from pdm.exceptions import NoPythonVersion, PdmUsageError, ProjectError
 from pdm.models.backends import BuildBackend, get_backend_by_spec
-from pdm.models.caches import CandidateInfoCache, HashCache, WheelCache, get_wheel_cache
-from pdm.models.candidates import Candidate, make_candidate
 from pdm.models.python import PythonInfo
 from pdm.models.repositories import BaseRepository, LockedRepository
 from pdm.models.requirements import Requirement, parse_requirement, strip_extras
 from pdm.models.specifiers import PySpecSet
 from pdm.project.config import Config
 from pdm.project.lockfile import Lockfile
 from pdm.project.project_file import PyProject
@@ -37,18 +31,22 @@
     find_project_root,
     find_python_in_path,
     normalize_name,
     path_to_url,
 )
 
 if TYPE_CHECKING:
+    from findpython import Finder
     from resolvelib.reporters import BaseReporter
 
     from pdm._types import Spinner
     from pdm.core import Core
+    from pdm.environments import BaseEnvironment
+    from pdm.models.caches import CandidateInfoCache, HashCache, WheelCache
+    from pdm.models.candidates import Candidate
     from pdm.resolver.providers import BaseProvider
 
 
 PYENV_ROOT = os.path.expanduser(os.getenv("PYENV_ROOT", "~/.pyenv"))
 
 
 class Project:
@@ -68,14 +66,16 @@
     def __init__(
         self,
         core: Core,
         root_path: str | Path | None,
         is_global: bool = False,
         global_config: str | Path | None = None,
     ) -> None:
+        import platformdirs
+
         self._lockfile: Lockfile | None = None
         self._environment: BaseEnvironment | None = None
         self._python: PythonInfo | None = None
         self.core = core
 
         if global_config is None:
             global_config = platformdirs.user_config_path("pdm") / "config.toml"
@@ -239,14 +239,16 @@
                     note("[success]__pypackages__[/] is detected, using the PEP 582 mode")
                 self.python = py_version
                 return py_version
 
         raise NoPythonVersion(f"No Python that satisfies {self.python_requires} is found on the system.")
 
     def get_environment(self) -> BaseEnvironment:
+        from pdm.environments import PythonEnvironment, PythonLocalEnvironment
+
         """Get the environment selected by this project"""
 
         if self.is_global:
             env = PythonEnvironment(self)
             # Rewrite global project's python requires to be
             # compatible with the exact version
             env.python_requires = PySpecSet(f"=={self.python.version}")
@@ -365,30 +367,31 @@
     def allow_prereleases(self) -> bool | None:
         return self.pyproject.settings.get("allow_prereleases")
 
     @property
     def default_source(self) -> RepositoryConfig:
         """Get the default source from the pypi setting"""
         return RepositoryConfig(
+            config_prefix="pypi",
             name="pypi",
             url=self.config["pypi.url"],
             verify_ssl=self.config["pypi.verify_ssl"],
             username=self.config.get("pypi.username"),
             password=self.config.get("pypi.password"),
         )
 
     @property
     def sources(self) -> list[RepositoryConfig]:
         result: dict[str, RepositoryConfig] = {}
         for source in self.pyproject.settings.get("source", []):
-            result[source["name"]] = RepositoryConfig(**source)
+            result[source["name"]] = RepositoryConfig(**source, config_prefix="pypi")
 
-        def merge_sources(other_sources: Iterable[tuple[str, RepositoryConfig]]) -> None:
-            for name, source in other_sources:
-                source.name = name
+        def merge_sources(other_sources: Iterable[RepositoryConfig]) -> None:
+            for source in other_sources:
+                name = source.name
                 if name in result:
                     result[name].passive_update(source)
                 else:
                     result[name] = source
 
         if not self.config.get("pypi.ignore_stored_index", False):
             if "pypi" not in result:  # put pypi source at the beginning
@@ -519,14 +522,18 @@
         toml_data["metadata"].update(self.get_lock_metadata(groups, cross_platform=cross_platform))
         self.lockfile.set_data(toml_data)
 
         if write:
             self.lockfile.write(show_message)
 
     def make_self_candidate(self, editable: bool = True) -> Candidate:
+        from unearth import Link
+
+        from pdm.models.candidates import make_candidate
+
         req = parse_requirement(path_to_url(self.root.as_posix()), editable)
         assert self.name
         req.name = self.name
         can = make_candidate(req, name=self.name, link=Link.from_path(self.root))
         can.prepare(self.environment).metadata
         return can
 
@@ -606,22 +613,28 @@
             path.mkdir(parents=True, exist_ok=True)
         except OSError:
             # The path could be not accessible
             pass
         return path
 
     def make_wheel_cache(self) -> WheelCache:
+        from pdm.models.caches import get_wheel_cache
+
         return get_wheel_cache(self.cache("wheels"))
 
     def make_candidate_info_cache(self) -> CandidateInfoCache:
+        from pdm.models.caches import CandidateInfoCache
+
         python_hash = hashlib.sha1(str(self.environment.python_requires).encode()).hexdigest()
         file_name = f"package_meta_{python_hash}.json"
         return CandidateInfoCache(self.cache("metadata") / file_name)
 
     def make_hash_cache(self) -> HashCache:
+        from pdm.models.caches import HashCache
+
         return HashCache(directory=self.cache("hashes"))
 
     def find_interpreters(self, python_spec: str | None = None) -> Iterable[PythonInfo]:
         """Return an iterable of interpreter paths that matches the given specifier,
         which can be:
             1. a version specifier like 3.7
             2. an absolute path
@@ -662,14 +675,16 @@
             yield PythonInfo(entry)
         if not python_spec:
             # Lastly, return the host Python as well
             this_python = getattr(sys, "_base_executable", sys.executable)
             yield PythonInfo.from_path(this_python)
 
     def _get_python_finder(self) -> Finder:
+        from findpython import Finder
+
         from pdm.cli.commands.venv.utils import VenvProvider
 
         finder = Finder(resolve_symlinks=True)
         if self.config["python.use_venv"]:
             finder.add_provider(VenvProvider(self), 0)
         return finder
```

### Comparing `pdm-2.6.1/src/pdm/project/lockfile.py` & `pdm-2.7.0/src/pdm/project/lockfile.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/project/project_file.py` & `pdm-2.7.0/src/pdm/project/project_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/project/toml_file.py` & `pdm-2.7.0/src/pdm/project/toml_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/pytest.py` & `pdm-2.7.0/src/pdm/pytest.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,15 @@
 
 import pytest
 import requests
 from packaging.version import parse as parse_version
 from pytest_mock import MockerFixture
 from unearth import Link
 
-from pdm.cli.actions import do_init
 from pdm.cli.hooks import HookManager
-from pdm.compat import Protocol
 from pdm.core import Core
 from pdm.environments import BaseEnvironment, PythonEnvironment
 from pdm.exceptions import CandidateInfoNotFound
 from pdm.installers.installers import install_wheel
 from pdm.models.backends import get_backend
 from pdm.models.candidates import Candidate
 from pdm.models.repositories import BaseRepository
@@ -66,14 +64,16 @@
 )
 from pdm.models.session import PDMSession
 from pdm.project.config import Config
 from pdm.project.core import Project
 from pdm.utils import find_python_in_path, normalize_name, path_to_url
 
 if TYPE_CHECKING:
+    from typing import Protocol
+
     from _pytest.fixtures import SubRequest
 
     from pdm._types import CandidateInfo, RepositoryConfig
 
 
 class LocalFileAdapter(requests.adapters.BaseAdapter):
     """
@@ -333,18 +333,21 @@
 
     Returns:
         a definition of the mocked indexes
     """
     return {}
 
 
+_build_session = BaseEnvironment._build_session
+
+
 @pytest.fixture
 def pdm_session(pypi_indexes: IndexesDefinition) -> Callable[[Any], PDMSession]:
     def get_pypi_session(*args: Any, **kwargs: Any) -> PDMSession:
-        session = PDMSession(*args, **kwargs)
+        session = _build_session(*args, **kwargs)
         for root, specs in pypi_indexes.items():
             index, overrides, strip = specs if isinstance(specs, tuple) else (specs, None, False)
             session.mount(root, LocalFileAdapter(index, overrides=overrides, strip_suffix=strip))
         return session
 
     return get_pypi_session
 
@@ -385,15 +388,15 @@
     test_home = tmp_path / ".pdm-home"
     test_home.mkdir(parents=True)
     test_home.joinpath("config.toml").write_text(
         '[global_project]\npath = "{}"\n'.format(test_home.joinpath("global-project").as_posix())
     )
     p = core.create_project(tmp_path, global_config=test_home.joinpath("config.toml").as_posix())
     p.global_config["venv.location"] = str(tmp_path / "venvs")
-    mocker.patch("pdm.environments.base.PDMSession", pdm_session)
+    mocker.patch.object(BaseEnvironment, "_build_session", pdm_session)
     mocker.patch("pdm.builders.base.EnvBuilder.get_shared_env", return_value=str(build_env))
     tmp_path.joinpath("caches").mkdir(parents=True)
     p.global_config["cache_dir"] = tmp_path.joinpath("caches").as_posix()
     python_path = find_python_in_path(sys.base_prefix)
     if python_path is None:
         raise ValueError("Unable to find a Python path")
     p._saved_python = python_path.as_posix()
@@ -412,16 +415,18 @@
 def project(project_no_init: Project) -> Project:
     """
     A fixture creating an initialized test project for the current test.
 
     Returns:
         The initialized project
     """
+    from pdm.cli.commands.init import Command
+
     hooks = HookManager(project_no_init, ["post_init"])
-    do_init(
+    Command.do_init(
         project_no_init,
         "test_project",
         "0.0.0",
         hooks=hooks,
         build_backend=get_backend("pdm-pep517"),
     )
     # Clean the cached property
@@ -543,38 +548,40 @@
     def print(self) -> None:
         """A debugging facility"""
         print("# exit code:", self.exit_code)
         print("# stdout:", self.stdout, sep="\n")
         print("# stderr:", self.stderr, sep="\n")
 
 
-class PDMCallable(Protocol):
-    """The PDM fixture callable signature"""
+if TYPE_CHECKING:
 
-    def __call__(
-        self,
-        args: str | list[str],
-        strict: bool = False,
-        input: str | None = None,
-        obj: Project | None = None,
-        env: Mapping[str, str] | None = None,
-        **kwargs: Any,
-    ) -> RunResult:
-        """
-        Args:
-            args: the command arguments as a single lexable string or a strings array
-            strict: raise an exception on failure instead of returning if enabled
-            input: an optional string to be submitted too `stdin`
-            obj: an optional existing `Project`.
-            env: override the environment variables with those
-
-        Returns:
-            The command result
-        """
-        ...
+    class PDMCallable(Protocol):
+        """The PDM fixture callable signature"""
+
+        def __call__(
+            self,
+            args: str | list[str],
+            strict: bool = False,
+            input: str | None = None,
+            obj: Project | None = None,
+            env: Mapping[str, str] | None = None,
+            **kwargs: Any,
+        ) -> RunResult:
+            """
+            Args:
+                args: the command arguments as a single lexable string or a strings array
+                strict: raise an exception on failure instead of returning if enabled
+                input: an optional string to be submitted too `stdin`
+                obj: an optional existing `Project`.
+                env: override the environment variables with those
+
+            Returns:
+                The command result
+            """
+            ...
 
 
 @pytest.fixture
 def pdm(core: Core, monkeypatch: pytest.MonkeyPatch) -> PDMCallable:
     """
     A fixture alloowing to execute PDM commands
```

### Comparing `pdm-2.6.1/src/pdm/resolver/core.py` & `pdm-2.7.0/src/pdm/resolver/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/resolver/providers.py` & `pdm-2.7.0/src/pdm/resolver/providers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/resolver/python.py` & `pdm-2.7.0/src/pdm/resolver/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/resolver/reporters.py` & `pdm-2.7.0/src/pdm/resolver/reporters.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/signals.py` & `pdm-2.7.0/src/pdm/signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/src/pdm/termui.py` & `pdm-2.7.0/src/pdm/termui.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,24 +2,27 @@
 
 import atexit
 import contextlib
 import enum
 import logging
 import os
 from tempfile import mktemp
-from typing import Any, Iterator, Sequence
+from typing import TYPE_CHECKING
 
 from rich.box import ROUNDED
 from rich.console import Console
 from rich.progress import Progress, ProgressColumn
 from rich.prompt import Confirm, IntPrompt, Prompt
 from rich.table import Table
 from rich.theme import Theme
 
-from pdm._types import RichProtocol, Spinner, SpinnerT
+if TYPE_CHECKING:
+    from typing import Any, Iterator, Sequence
+
+    from pdm._types import RichProtocol, Spinner, SpinnerT
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 logger.addHandler(logging.NullHandler())
 unearth_logger = logging.getLogger("unearth")
 unearth_logger.setLevel(logging.DEBUG)
 
@@ -244,14 +247,15 @@
                 )
             raise
         else:
             atexit.register(cleanup)
         finally:
             logger.removeHandler(handler)
             unearth_logger.removeHandler(handler)
+            handler.close()
 
     def open_spinner(self, title: str) -> Spinner:
         """Open a spinner as a context manager."""
         if self.verbosity >= Verbosity.DETAIL or not is_interactive():
             return DummySpinner(title)
         else:
             return _err_console.status(title, spinner=SPINNER, spinner_style="primary")
```

### Comparing `pdm-2.6.1/src/pdm/utils.py` & `pdm-2.7.0/src/pdm/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,21 +13,28 @@
 import subprocess
 import sys
 import sysconfig
 import tempfile
 import urllib.parse as parse
 import warnings
 from pathlib import Path
-from re import Match
-from typing import IO, Any, Iterator
+from typing import TYPE_CHECKING
 
 from packaging.version import Version
 
-from pdm._types import RepositoryConfig
-from pdm.compat import Distribution, importlib_metadata
+from pdm.compat import importlib_metadata
+
+if TYPE_CHECKING:
+    from re import Match
+    from typing import IO, Any, Iterator
+
+    from unearth import Link
+
+    from pdm._types import RepositoryConfig
+    from pdm.compat import Distribution
 
 _egg_fragment_re = re.compile(r"(.*)[#&]egg=[^&]*")
 
 try:
     _packaging_version = importlib_metadata.version("packaging")
 except Exception:
     from packaging import __version__ as _packaging_version
@@ -83,15 +90,15 @@
         if path.parent == path:
             # Root path is reached
             break
         path = path.parent
     return None
 
 
-def convert_hashes(hashes: dict[str, str]) -> dict[str, list[str]]:
+def convert_hashes(hashes: dict[Link, str]) -> dict[str, list[str]]:
     """Convert Pipfile.lock hash lines into InstallRequirement option format.
 
     The option format uses a str-list mapping. Keys are hash algorithms, and
     the list contains all values of that algorithm.
     """
     result: dict[str, list[str]] = {}
     for hash_value in hashes.values():
```

### Comparing `pdm-2.6.1/tests/cli/conftest.py` & `pdm-2.7.0/tests/cli/conftest.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import pytest
 import requests
 from pytest_mock import MockerFixture
 
 from pdm.cli.commands.publish.package import PackageFile
 from pdm.cli.commands.publish.repository import Repository
+from pdm.models.auth import Keyring, keyring
 from tests import FIXTURES
 
 
 @pytest.fixture
 def mock_run_gpg(mocker: MockerFixture):
     def mock_run_gpg(args):
         signature_file = args[-1] + ".asc"
@@ -95,7 +96,33 @@
             sys.stdout = io.TextIOWrapper(sys.stdout.buffer, newline='\\n')
             name = sys.argv[1]
             vars = " ".join([f"{v}={os.getenv(v)}" for v in sys.argv[2:]])
             print(f"{name} CALLED with {vars}" if vars else f"{name} CALLED")
             """
         )
     )
+
+
+@pytest.fixture(name="keyring")
+def keyring_fixture(mocker: MockerFixture, monkeypatch: pytest.MonkeyPatch) -> Keyring:
+    from unearth.auth import AuthInfo, KeyringBaseProvider
+
+    class MockKeyringProvider(KeyringBaseProvider):
+        def __init__(self) -> None:
+            self._store: dict[str, dict[str, str]] = {}
+
+        def save_auth_info(self, url: str, username: str, password: str) -> None:
+            self._store.setdefault(url, {})[username] = password
+
+        def get_auth_info(self, url: str, username: str | None) -> AuthInfo | None:
+            d = self._store.get(url, {})
+            if username is not None and username in d:
+                return username, d[username]
+            if username is None and d:
+                return next(iter(d.items()))
+            return None
+
+    provider = MockKeyringProvider()
+    mocker.patch("unearth.auth.get_keyring_provider", return_value=provider)
+    monkeypatch.setattr(keyring, "provider", provider)
+    monkeypatch.setattr(keyring, "enabled", True)
+    return keyring
```

### Comparing `pdm-2.6.1/tests/cli/test_add.py` & `pdm-2.7.0/tests/cli/test_add.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/cli/test_build.py` & `pdm-2.7.0/tests/cli/test_build.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import tarfile
 import zipfile
 
 import pytest
 
-from pdm.cli import actions
+from pdm.cli.commands.build import Command
 
 pytestmark = pytest.mark.usefixtures("local_finder")
 
 
 def get_tarball_names(path):
     with tarfile.open(path, "r:gz") as tar:
         return tar.getnames()
@@ -15,28 +15,28 @@
 
 def get_wheel_names(path):
     with zipfile.ZipFile(path) as zf:
         return zf.namelist()
 
 
 def test_build_command(project, pdm, mocker):
-    do_build = mocker.patch.object(actions, "do_build")
+    do_build = mocker.patch.object(Command, "do_build")
     pdm(["build"], obj=project)
     do_build.assert_called_once()
 
 
 def test_build_global_project_forbidden(pdm):
     result = pdm(["build", "-g"])
     assert result.exit_code != 0
 
 
 def test_build_single_module(fixture_project):
     project = fixture_project("demo-module")
 
-    actions.do_build(project)
+    Command.do_build(project)
     tar_names = get_tarball_names(project.root / "dist/demo-module-0.1.0.tar.gz")
     for name in [
         "foo_module.py",
         "bar_module.py",
         "LICENSE",
         "pyproject.toml",
         "PKG-INFO",
@@ -51,21 +51,21 @@
         assert name not in zip_names
 
 
 def test_build_single_module_with_readme(fixture_project):
     project = fixture_project("demo-module")
     project.pyproject.metadata["readme"] = "README.md"
     project.pyproject.write()
-    actions.do_build(project)
+    Command.do_build(project)
     assert "demo-module-0.1.0/README.md" in get_tarball_names(project.root / "dist/demo-module-0.1.0.tar.gz")
 
 
 def test_build_package(fixture_project):
     project = fixture_project("demo-package")
-    actions.do_build(project)
+    Command.do_build(project)
 
     tar_names = get_tarball_names(project.root / "dist/demo-package-0.1.0.tar.gz")
     assert "demo-package-0.1.0/my_package/__init__.py" in tar_names
     assert "demo-package-0.1.0/my_package/data.json" in tar_names
     assert "demo-package-0.1.0/single_module.py" not in tar_names
     assert "demo-package-0.1.0/data_out.json" not in tar_names
 
@@ -74,15 +74,15 @@
     assert "my_package/data.json" in zip_names
     assert "single_module.py" not in zip_names
     assert "data_out.json" not in zip_names
 
 
 def test_build_src_package(fixture_project):
     project = fixture_project("demo-src-package")
-    actions.do_build(project)
+    Command.do_build(project)
 
     tar_names = get_tarball_names(project.root / "dist/demo-package-0.1.0.tar.gz")
     assert "demo-package-0.1.0/src/my_package/__init__.py" in tar_names
     assert "demo-package-0.1.0/src/my_package/data.json" in tar_names
 
     zip_names = get_wheel_names(project.root / "dist/demo_package-0.1.0-py3-none-any.whl")
     assert "my_package/__init__.py" in zip_names
@@ -94,15 +94,15 @@
     project.pyproject.settings["includes"] = [
         "my_package/",
         "single_module.py",
         "data_out.json",
     ]
     project.pyproject.settings["excludes"] = ["my_package/*.json"]
     project.pyproject.write()
-    actions.do_build(project)
+    Command.do_build(project)
 
     tar_names = get_tarball_names(project.root / "dist/demo-package-0.1.0.tar.gz")
     assert "demo-package-0.1.0/my_package/__init__.py" in tar_names
     assert "demo-package-0.1.0/my_package/data.json" not in tar_names
     assert "demo-package-0.1.0/single_module.py" in tar_names
     assert "demo-package-0.1.0/data_out.json" in tar_names
 
@@ -113,28 +113,28 @@
     assert "data_out.json" in zip_names
 
 
 def test_build_src_package_by_include(fixture_project):
     project = fixture_project("demo-src-package")
     project.pyproject.settings["includes"] = ["src/my_package"]
     project.pyproject.write()
-    actions.do_build(project)
+    Command.do_build(project)
 
     tar_names = get_tarball_names(project.root / "dist/demo-package-0.1.0.tar.gz")
     assert "demo-package-0.1.0/src/my_package/__init__.py" in tar_names
     assert "demo-package-0.1.0/src/my_package/data.json" in tar_names
 
     zip_names = get_wheel_names(project.root / "dist/demo_package-0.1.0-py3-none-any.whl")
     assert "my_package/__init__.py" in zip_names
     assert "my_package/data.json" in zip_names
 
 
 def test_build_with_config_settings(fixture_project):
     project = fixture_project("demo-src-package")
-    actions.do_build(project, config_settings={"--plat-name": "win_amd64"})
+    Command.do_build(project, config_settings={"--plat-name": "win_amd64"})
 
     assert (project.root / "dist/demo_package-0.1.0-py3-none-win_amd64.whl").exists()
 
 
 def test_cli_build_with_config_settings(fixture_project, pdm):
     project = fixture_project("demo-src-package")
     result = pdm(["build", "-C--plat-name=win_amd64"], obj=project)
@@ -155,8 +155,8 @@
     result = pdm(args, obj=project)
     assert result.exit_code == int(isolated)
 
 
 def test_build_ignoring_pip_environment(fixture_project, monkeypatch):
     project = fixture_project("demo-module")
     monkeypatch.setenv("PIP_REQUIRE_VIRTUALENV", "1")
-    actions.do_build(project)
+    Command.do_build(project)
```

### Comparing `pdm-2.6.1/tests/cli/test_cache.py` & `pdm-2.7.0/tests/cli/test_cache.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/cli/test_config.py` & `pdm-2.7.0/tests/cli/test_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -83,29 +83,29 @@
         monkeypatch.setenv("PDM_CONFIG_FILE", "global_config.toml")
         result = pdm(["config", "project_max_depth"])
         assert result.exit_code == 0
         assert result.output.strip() == "9"
 
 
 def test_default_repository_setting(project):
-    repository = project.global_config.get_repository_config("pypi")
+    repository = project.global_config.get_repository_config("pypi", "repository")
     assert repository.url == "https://upload.pypi.org/legacy/"
     assert repository.username is None
     assert repository.password is None
 
-    repository = project.global_config.get_repository_config("testpypi")
+    repository = project.global_config.get_repository_config("testpypi", "repository")
     assert repository.url == "https://test.pypi.org/legacy/"
 
-    repository = project.global_config.get_repository_config("nonexist")
+    repository = project.global_config.get_repository_config("nonexist", "repository")
     assert repository is None
 
 
 def test_repository_config_not_available_on_project(project):
     with pytest.raises(PdmUsageError):
-        project.project_config.get_repository_config("pypi")
+        project.project_config.get_repository_config("pypi", "repository")
 
 
 def test_repository_config_key_short(project):
     with pytest.raises(PdmUsageError):
         project.global_config["repository.test"] = {"url": "https://example.org/simple"}
 
     with pytest.raises(PdmUsageError):
@@ -114,21 +114,21 @@
     with pytest.raises(PdmUsageError):
         del project.global_config["repository"]
 
 
 def test_repository_overwrite_default(project):
     project.global_config["repository.pypi.username"] = "foo"
     project.global_config["repository.pypi.password"] = "bar"
-    repository = project.global_config.get_repository_config("pypi")
+    repository = project.global_config.get_repository_config("pypi", "repository")
     assert repository.url == "https://upload.pypi.org/legacy/"
     assert repository.username == "foo"
     assert repository.password == "bar"
 
     project.global_config["repository.pypi.url"] = "https://example.pypi.org/legacy/"
-    repository = project.global_config.get_repository_config("pypi")
+    repository = project.global_config.get_repository_config("pypi", "repository")
     assert repository.url == "https://example.pypi.org/legacy/"
 
 
 def test_hide_password_in_output_repository(project, pdm):
     assert project.global_config["repository.pypi.password"] is None
     project.global_config["repository.pypi.username"] = "testuser"
     project.global_config["repository.pypi.password"] = "secret"
@@ -151,22 +151,22 @@
     result = pdm(["config"], obj=project)
     assert "pypi.extra.password" in result.output
     assert "<hidden>" in result.output
 
 
 def test_config_get_repository(project, pdm):
     config = project.global_config["repository.pypi"]
-    assert config == project.global_config.get_repository_config("pypi")
+    assert config == project.global_config.get_repository_config("pypi", "repository")
     assert project.global_config["repository.pypi.url"] == "https://upload.pypi.org/legacy/"
 
     result = pdm(["config", "repository.pypi"], obj=project, strict=True)
-    assert result.stdout.strip() == "url = https://upload.pypi.org/legacy/"
+    assert result.stdout.strip() == "repository.pypi.url = https://upload.pypi.org/legacy/"
 
     assert (
-        project.global_config.get_repository_config("https://example.pypi.org/legacy/").url
+        project.global_config.get_repository_config("https://example.pypi.org/legacy/", "repository").url
         == "https://example.pypi.org/legacy/"
     )
 
     result = pdm(["config", "repository.pypi.url"], obj=project, strict=True)
     assert result.stdout.strip() == "https://upload.pypi.org/legacy/"
 
 
@@ -177,11 +177,54 @@
     assert project.global_config["repository.pypi.username"] == "foo"
     del project.global_config["repository.pypi.username"]
     assert project.global_config["repository.pypi.username"] is None
 
 
 def test_config_del_repository(project):
     project.global_config["repository.test.url"] = "https://example.org/simple"
-    assert project.global_config.get_repository_config("test") is not None
+    assert project.global_config.get_repository_config("test", "repository") is not None
 
     del project.global_config["repository.test"]
-    assert project.global_config.get_repository_config("test") is None
+    assert project.global_config.get_repository_config("test", "repository") is None
+
+
+def test_config_password_save_into_keyring(project, keyring):
+    project.global_config.update(
+        {
+            "pypi.extra.url": "https://extra.pypi.org/simple",
+            "pypi.extra.username": "foo",
+            "pypi.extra.password": "barbaz",
+            "repository.pypi.username": "frost",
+            "repository.pypi.password": "password",
+        }
+    )
+
+    assert project.global_config["pypi.extra.password"] == "barbaz"
+    assert project.global_config["repository.pypi.password"] == "password"
+
+    assert keyring.enabled
+    assert keyring.get_auth_info("pdm-pypi-extra", "foo") == ("foo", "barbaz")
+    assert keyring.get_auth_info("pdm-repository-pypi", None) == ("frost", "password")
+
+
+def test_keyring_operation_error_disables_itself(project, keyring, mocker):
+    saver = mocker.patch.object(keyring.provider, "save_auth_info", side_effect=RuntimeError())
+    getter = mocker.patch.object(keyring.provider, "get_auth_info")
+    project.global_config.update(
+        {
+            "pypi.extra.url": "https://extra.pypi.org/simple",
+            "pypi.extra.username": "foo",
+            "pypi.extra.password": "barbaz",
+            "repository.pypi.username": "frost",
+            "repository.pypi.password": "password",
+        }
+    )
+
+    assert project.global_config["pypi.extra.password"] == "barbaz"
+    assert project.global_config["repository.pypi.password"] == "password"
+
+    saver.assert_called_once()
+    getter.assert_not_called()
+
+    assert not keyring.enabled
+    assert keyring.get_auth_info("pdm-pypi-extra", "foo") is None
+    assert keyring.get_auth_info("pdm-repository-pypi", None) is None
```

### Comparing `pdm-2.6.1/tests/cli/test_fix.py` & `pdm-2.7.0/tests/cli/test_fix.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/cli/test_hooks.py` & `pdm-2.7.0/tests/cli/test_hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/cli/test_init.py` & `pdm-2.7.0/tests/cli/test_init.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import sys
 from unittest.mock import ANY
 
 import pytest
 
 from pdm.cli import actions
+from pdm.cli.commands.init import Command
 from pdm.models.backends import get_backend
 from pdm.models.python import PythonInfo
 
 PYTHON_VERSION = f"{sys.version_info[0]}.{sys.version_info[1]}"
 
 
 def test_init_validate_python_requires(project_no_init):
     with pytest.raises(ValueError):
-        actions.do_init(project_no_init, python_requires="3.7")
+        Command.do_init(project_no_init, python_requires="3.7")
 
 
 def test_init_command(project_no_init, pdm, mocker):
     mocker.patch(
         "pdm.cli.commands.init.get_user_email_from_git",
         return_value=("Testing", "me@example.org"),
     )
-    do_init = mocker.patch.object(actions, "do_init")
+    do_init = mocker.patch.object(Command, "do_init")
     pdm(["init"], input="\n\n\n\n\n\n", strict=True, obj=project_no_init)
     python_version = f"{project_no_init.python.major}.{project_no_init.python.minor}"
     do_init.assert_called_with(
         project_no_init,
         name="",
         version="",
         description="",
@@ -38,15 +39,15 @@
 
 
 def test_init_command_library(project_no_init, pdm, mocker):
     mocker.patch(
         "pdm.cli.commands.init.get_user_email_from_git",
         return_value=("Testing", "me@example.org"),
     )
-    do_init = mocker.patch.object(actions, "do_init")
+    do_init = mocker.patch.object(Command, "do_init")
     result = pdm(
         ["init"],
         input="\ny\ntest-project\n\nTest Project\n1\n\n\n\n\n",
         obj=project_no_init,
     )
     assert result.exit_code == 0
     python_version = f"{project_no_init.python.major}.{project_no_init.python.minor}"
@@ -65,15 +66,15 @@
 
 
 def test_init_non_interactive(project_no_init, pdm, mocker):
     mocker.patch(
         "pdm.cli.commands.init.get_user_email_from_git",
         return_value=("Testing", "me@example.org"),
     )
-    do_init = mocker.patch.object(actions, "do_init")
+    do_init = mocker.patch.object(Command, "do_init")
     do_use = mocker.patch.object(actions, "do_use", return_value=PythonInfo.from_path(sys.executable))
     result = pdm(["init", "-n"], obj=project_no_init)
     assert result.exit_code == 0
     python_version = f"{project_no_init.python.major}.{project_no_init.python.minor}"
     do_use.assert_called_once_with(
         project_no_init,
         ANY,
```

### Comparing `pdm-2.6.1/tests/cli/test_install.py` & `pdm-2.7.0/tests/cli/test_install.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/cli/test_list.py` & `pdm-2.7.0/tests/cli/test_list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/cli/test_lock.py` & `pdm-2.7.0/tests/cli/test_lock.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/cli/test_others.py` & `pdm-2.7.0/tests/cli/test_others.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 from pdm.models.requirements import parse_requirement
 from pdm.utils import cd
 from tests import FIXTURES
 
 
 @pytest.mark.usefixtures("project_no_init", "local_finder")
 def test_build_distributions(tmp_path, core):
+    from pdm.cli.commands.build import Command
+
     project = core.create_project()
-    actions.do_build(project, dest=tmp_path.as_posix())
+    Command.do_build(project, dest=tmp_path.as_posix())
     wheel = next(tmp_path.glob("*.whl"))
     assert wheel.name.startswith("pdm-")
     tarball = next(tmp_path.glob("*.tar.gz"))
     assert tarball.exists()
 
 
 def test_project_no_init_error(project_no_init, pdm):
```

### Comparing `pdm-2.6.1/tests/cli/test_remove.py` & `pdm-2.7.0/tests/cli/test_remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/cli/test_run.py` & `pdm-2.7.0/tests/cli/test_run.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/cli/test_self_command.py` & `pdm-2.7.0/tests/cli/test_self_command.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/cli/test_update.py` & `pdm-2.7.0/tests/cli/test_update.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/cli/test_use.py` & `pdm-2.7.0/tests/cli/test_use.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/cli/test_venv.py` & `pdm-2.7.0/tests/cli/test_venv.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/conftest.py` & `pdm-2.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl` & `pdm-2.7.0/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz` & `pdm-2.7.0/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl` & `pdm-2.7.0/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl` & `pdm-2.7.0/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl` & `pdm-2.7.0/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/artifacts/demo-0.0.1.tar.gz` & `pdm-2.7.0/tests/fixtures/artifacts/demo-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/artifacts/demo-0.0.1.zip` & `pdm-2.7.0/tests/fixtures/artifacts/demo-0.0.1.zip`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl` & `pdm-2.7.0/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl` & `pdm-2.7.0/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl` & `pdm-2.7.0/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl` & `pdm-2.7.0/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz` & `pdm-2.7.0/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl` & `pdm-2.7.0/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl` & `pdm-2.7.0/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl` & `pdm-2.7.0/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl` & `pdm-2.7.0/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl` & `pdm-2.7.0/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl` & `pdm-2.7.0/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl` & `pdm-2.7.0/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl` & `pdm-2.7.0/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl` & `pdm-2.7.0/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl` & `pdm-2.7.0/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl` & `pdm-2.7.0/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock` & `pdm-2.7.0/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/projects/demo-package/pdm.lock` & `pdm-2.7.0/tests/fixtures/projects/demo-package/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/projects/demo-package/pyproject.toml` & `pdm-2.7.0/tests/fixtures/projects/demo-package/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/projects/demo-package/requirements.txt` & `pdm-2.7.0/tests/fixtures/projects/demo-package/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/projects/demo-package/setup.txt` & `pdm-2.7.0/tests/fixtures/projects/demo-package/setup.txt`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/projects/flit-demo/pyproject.toml` & `pdm-2.7.0/tests/fixtures/projects/flit-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/projects/poetry-demo/pyproject.toml` & `pdm-2.7.0/tests/fixtures/projects/poetry-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/pypi.json` & `pdm-2.7.0/tests/fixtures/pypi.json`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/fixtures/pyproject.toml` & `pdm-2.7.0/tests/fixtures/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/models/test_backends.py` & `pdm-2.7.0/tests/models/test_backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/models/test_candidates.py` & `pdm-2.7.0/tests/models/test_candidates.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,14 +297,16 @@
     assert not candidate.requires_python
 
 
 def test_find_candidates_from_find_links(project):
     repo = project.get_repository()
     repo.sources = [
         RepositoryConfig(
+            name="test",
+            config_prefix="pypi",
             url="http://fixtures.test/index/demo.html",
             verify_ssl=False,
             type="find_links",
         )
     ]
     candidates = list(repo.find_candidates(parse_requirement("demo")))
     assert len(candidates) == 2
```

### Comparing `pdm-2.6.1/tests/models/test_marker.py` & `pdm-2.7.0/tests/models/test_marker.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/models/test_requirements.py` & `pdm-2.7.0/tests/models/test_requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/models/test_setup_parsing.py` & `pdm-2.7.0/tests/models/test_setup_parsing.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/models/test_specifiers.py` & `pdm-2.7.0/tests/models/test_specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/models/test_versions.py` & `pdm-2.7.0/tests/models/test_versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/resolver/test_resolve.py` & `pdm-2.7.0/tests/resolver/test_resolve.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/test_formats.py` & `pdm-2.7.0/tests/test_formats.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,20 +131,20 @@
     assert "webassets==2.0" in group
     assert 'whoosh==2.7.4; sys_platform == "win32"' in group
     assert "-e git+https://github.com/pypa/pip.git@main#egg=pip" not in group
     assert "-e git+https://github.com/pypa/pip.git@main#egg=pip" in dev_group
     assert not result.get("dependencies")
 
 
-def test_export_expand_env_vars_in_source(project, monkeypatch):
+def test_keep_env_vars_in_source(project, monkeypatch):
     monkeypatch.setenv("USER", "foo")
     monkeypatch.setenv("PASSWORD", "bar")
     project.pyproject.settings["source"] = [{"url": "https://${USER}:${PASSWORD}@test.pypi.org/simple", "name": "pypi"}]
     result = requirements.export(project, [], Namespace())
-    assert result.strip().splitlines()[-1] == "--index-url https://foo:bar@test.pypi.org/simple"
+    assert result.strip().splitlines()[-1] == "--index-url https://${USER}:${PASSWORD}@test.pypi.org/simple"
 
 
 def test_export_replace_project_root(project):
     artifact = FIXTURES / "artifacts/first-2.0.2-py2.py3-none-any.whl"
     shutil.copy2(artifact, project.root)
     with cd(project.root):
         req = parse_requirement(f"./{artifact.name}")
```

### Comparing `pdm-2.6.1/tests/test_installer.py` & `pdm-2.7.0/tests/test_installer.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/test_integration.py` & `pdm-2.7.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/test_plugin.py` & `pdm-2.7.0/tests/test_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 from unittest import mock
 
 import pytest
 
 from pdm.cli.commands.base import BaseCommand
 from pdm.compat import importlib_metadata
 from pdm.project.config import ConfigItem
@@ -103,15 +104,16 @@
     assert result.output.strip() == "Hello world"
 
     result = pdm(["config", "foo"])
     assert result.output.strip() == "bar"
 
 
 @pytest.mark.usefixtures("local_finder")
-def test_project_plugin_library(pdm, project, core):
+def test_project_plugin_library(pdm, project, core, monkeypatch):
+    monkeypatch.setattr(sys, "path", sys.path[:])
     project.pyproject.settings["plugins"] = ["pdm-hello"]
     pdm(["install", "--plugins"], obj=project, strict=True)
     assert project.root.joinpath(".pdm-plugins").exists()
     assert "pdm-hello" not in project.environment.get_working_set()
     with cd(project.root):
         core.load_plugins()
         result = pdm(["hello", "Frost"], strict=True)
```

### Comparing `pdm-2.6.1/tests/test_project.py` & `pdm-2.7.0/tests/test_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -310,7 +310,23 @@
     sources = project.sources
     assert [source.name for source in sources] == ["pypi", "custom"]
     custom_source = sources[1]
     assert custom_source.url == "https://custom.pypi.org/simple"
     assert custom_source.verify_ssl is False
     assert custom_source.username == "foo"
     assert custom_source.password == "bar"
+
+
+def test_invoke_pdm_adding_configured_args(project, pdm, mocker):
+    project.pyproject.settings["options"] = {
+        "install": ["--no-self", "--no-editable"],
+        "add": ["--no-isolation"],
+        "lock": ["--no-cross-platform"],
+    }
+    project.pyproject.write()
+    parser = mocker.patch("argparse.ArgumentParser.parse_args")
+    pdm(["add", "requests"], obj=project)
+    parser.assert_called_with(["add", "--no-isolation", "requests"])
+    pdm(["install", "--check"], obj=project)
+    parser.assert_called_with(["install", "--no-self", "--no-editable", "--check"])
+    pdm(["lock", "--lockfile", "pdm.2.lock"], obj=project)
+    parser.assert_called_with(["lock", "--no-cross-platform", "--lockfile", "pdm.2.lock"])
```

### Comparing `pdm-2.6.1/tests/test_signals.py` & `pdm-2.7.0/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.6.1/tests/test_utils.py` & `pdm-2.7.0/tests/test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pathlib
 import sys
 
 import pytest
+import tomlkit
 
 from pdm import utils
 from pdm.cli import utils as cli_utils
 from pdm.cli.filters import GroupSelection
 from pdm.exceptions import PdmUsageError
 
 
@@ -64,18 +65,20 @@
         posix_path_to_executable,
     )
 
     assert not utils.find_python_in_path(tmp_path)
 
 
 def test_merge_dictionary():
-    target = {
-        "existing_dict": {"foo": "bar", "hello": "world"},
-        "existing_list": ["hello"],
-    }
+    target = tomlkit.item(
+        {
+            "existing_dict": {"foo": "bar", "hello": "world"},
+            "existing_list": ["hello"],
+        }
+    )
     input_dict = {
         "existing_dict": {"foo": "baz"},
         "existing_list": ["world"],
         "new_dict": {"name": "Sam"},
     }
     cli_utils.merge_dictionary(target, input_dict)
     assert target == {
```

### Comparing `pdm-2.6.1/PKG-INFO` & `pdm-2.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm
-Version: 2.6.1
+Version: 2.7.0
 Summary: A modern Python package and dependency manager supporting the latest PEP standards
 Keywords: packaging dependency workflow
 Author-Email: Frost Ming <mianghong@gmail.com>
 License: MIT
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -28,17 +28,16 @@
 Requires-Dist: unearth>=0.9.0
 Requires-Dist: findpython>=0.2.2
 Requires-Dist: tomlkit<1,>=0.11.1
 Requires-Dist: shellingham>=1.3.2
 Requires-Dist: python-dotenv>=0.15
 Requires-Dist: resolvelib>=1.0.1
 Requires-Dist: installer<0.8,>=0.7
-Requires-Dist: cachecontrol[filecache]>=0.12.11
+Requires-Dist: cacheyou[filecache]
 Requires-Dist: tomli>=1.1.0; python_version < "3.11"
-Requires-Dist: typing-extensions; python_version < "3.8"
 Requires-Dist: importlib-metadata>=3.6; python_version < "3.10"
 Requires-Dist: pytest; extra == "pytest"
 Requires-Dist: pytest-mock; extra == "pytest"
 Provides-Extra: pytest
 Description-Content-Type: text/markdown
 
 <div align="center">
@@ -134,15 +133,15 @@
 **For Windows**
 
 ```powershell
 (Invoke-WebRequest -Uri https://raw.githubusercontent.com/pdm-project/pdm/main/install-pdm.py -UseBasicParsing).Content | python -
 ```
 
 For security reasons, you should verify the checksum of `install-pdm.py`.
-The sha256 checksum is: `ce0a116987b2667231391d13dd005006433114033cac74aa18f0b2dec5538d03`
+The sha256 checksum is: `06abd94a6678636eba640529bf91b242759363c45d3620cdfabaa0053d826b30`
 
 The installer will install PDM into the user site and the location depends on the system:
 
 - `$HOME/.local/bin` for Unix
 - `%APPDATA%\Python\Scripts` on Windows
 
 You can pass additional options to the script to control how PDM is installed:
@@ -160,15 +159,15 @@
   -d DEP, --dep DEP | envvar: PDM_DEPS     Specify additional dependencies, can be given multiple times
 ```
 
 You can either pass the options after the script or set the env var value.
 
 ### Alternative Installation Methods
 
-If you are on MacOS and using `homebrew`, install it by:
+If you are on macOS and using `homebrew`, install it by:
 
 ```bash
 brew install pdm
 ```
 
 If you are on Windows and using [Scoop](https://scoop.sh/), install it by:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdm Version: 2.6.1 Summary: A modern Python package
+Metadata-Version: 2.1 Name: pdm Version: 2.7.0 Summary: A modern Python package
 and dependency manager supporting the latest PEP standards Keywords: packaging
 dependency workflow Author-Email: Frost Ming
 gmail.com> License: MIT Classifier: Topic :: Software Development :: Build
 Tools Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -11,17 +11,16 @@
 Project-URL: Changelog, https://pdm.fming.dev/latest/dev/changelog/ Requires-
 Python: >=3.7 Requires-Dist: blinker Requires-Dist: certifi Requires-Dist:
 packaging!=22.0,>=20.9 Requires-Dist: platformdirs Requires-Dist: rich>=12.3.0
 Requires-Dist: virtualenv>=20 Requires-Dist: pyproject-hooks Requires-Dist:
 requests-toolbelt Requires-Dist: unearth>=0.9.0 Requires-Dist:
 findpython>=0.2.2 Requires-Dist: tomlkit<1,>=0.11.1 Requires-Dist:
 shellingham>=1.3.2 Requires-Dist: python-dotenv>=0.15 Requires-Dist:
-resolvelib>=1.0.1 Requires-Dist: installer<0.8,>=0.7 Requires-Dist:
-cachecontrol[filecache]>=0.12.11 Requires-Dist: tomli>=1.1.0; python_version <
-"3.11" Requires-Dist: typing-extensions; python_version < "3.8" Requires-Dist:
+resolvelib>=1.0.1 Requires-Dist: installer<0.8,>=0.7 Requires-Dist: cacheyou
+[filecache] Requires-Dist: tomli>=1.1.0; python_version < "3.11" Requires-Dist:
 importlib-metadata>=3.6; python_version < "3.10" Requires-Dist: pytest; extra
 == "pytest" Requires-Dist: pytest-mock; extra == "pytest" Provides-Extra:
 pytest Description-Content-Type: text/markdown
 # PDM A modern Python package and dependency manager supporting the latest PEP
       standards. [ä¸­æçæ¬è¯´æ](README_zh.md) ![PDM logo](https://
 raw.githubusercontent.com/pdm-project/pdm/main/docs/docs/assets/logo_big.png)
  [![Docs](https://img.shields.io/badge/Docs-mkdocs-blue?style=for-the-badge)]
@@ -80,28 +79,28 @@
 Like Pip, PDM provides an installation script that will install PDM into an
 isolated environment. **For Linux/Mac** ```bash curl -sSL https://
 raw.githubusercontent.com/pdm-project/pdm/main/install-pdm.py | python3 - ```
 **For Windows** ```powershell (Invoke-WebRequest -Uri https://
 raw.githubusercontent.com/pdm-project/pdm/main/install-pdm.py -
 UseBasicParsing).Content | python - ``` For security reasons, you should verify
 the checksum of `install-pdm.py`. The sha256 checksum is:
-`ce0a116987b2667231391d13dd005006433114033cac74aa18f0b2dec5538d03` The
+`06abd94a6678636eba640529bf91b242759363c45d3620cdfabaa0053d826b30` The
 installer will install PDM into the user site and the location depends on the
 system: - `$HOME/.local/bin` for Unix - `%APPDATA%\Python\Scripts` on Windows
 You can pass additional options to the script to control how PDM is installed:
 ``` usage: install-pdm.py [-h] [-v VERSION] [--prerelease] [--remove] [-p PATH]
 [-d DEP] optional arguments: -h, --help show this help message and exit -
 v VERSION, --version VERSION | envvar: PDM_VERSION Specify the version to be
 installed, or HEAD to install from the main branch --prerelease | envvar:
 PDM_PRERELEASE Allow prereleases to be installed --remove | envvar: PDM_REMOVE
 Remove the PDM installation -p PATH, --path PATH | envvar: PDM_HOME Specify the
 location to install PDM -d DEP, --dep DEP | envvar: PDM_DEPS Specify additional
 dependencies, can be given multiple times ``` You can either pass the options
 after the script or set the env var value. ### Alternative Installation Methods
-If you are on MacOS and using `homebrew`, install it by: ```bash brew install
+If you are on macOS and using `homebrew`, install it by: ```bash brew install
 pdm ``` If you are on Windows and using [Scoop](https://scoop.sh/), install it
 by: ``` scoop bucket add frostming https://github.com/frostming/scoop-
 frostming.git scoop install pdm ``` Otherwise, it is recommended to install
 `pdm` in an isolated environment with `pipx`: ```bash pipx install pdm ``` Or
 you can install it under a user site: ```bash pip install --user pdm ``` With
 [asdf-vm](https://asdf-vm.com/) ```bash asdf plugin add pdm asdf install pdm
 latest ``` ## Quickstart **Initialize a new PDM project** ```bash pdm init ```
```

