# Comparing `tmp/PyFunceble-4.1.3.tar.gz` & `tmp/PyFunceble-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFunceble-4.1.3.tar", last modified: Sun Nov 20 11:24:20 2022, max compression
+gzip compressed data, was "PyFunceble-4.2.0.tar", last modified: Mon May 29 09:55:36 2023, max compression
```

## Comparing `PyFunceble-4.1.3.tar` & `PyFunceble-4.2.0.tar`

### file list

```diff
@@ -1,337 +1,350 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.701224 PyFunceble-4.1.3/
--rw-r--r--   0 runner    (1001) docker     (121)     3208 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2841 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10783 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    12213 2022-11-20 11:24:20.701224 PyFunceble-4.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.661221 PyFunceble-4.1.3/PyFunceble/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.665222 PyFunceble-4.1.3/PyFunceble/.vscode/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (121)    22726 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.665222 PyFunceble-4.1.3/PyFunceble/checker/
--rw-r--r--   0 runner    (1001) docker     (121)     2434 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.665222 PyFunceble-4.1.3/PyFunceble/checker/availability/
--rw-r--r--   0 runner    (1001) docker     (121)     2479 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/availability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    36049 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/availability/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     7436 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/availability/domain.py
--rw-r--r--   0 runner    (1001) docker     (121)     5007 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/availability/domain_and_ip.py
--rw-r--r--   0 runner    (1001) docker     (121)    12768 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/availability/extra_rules.py
--rw-r--r--   0 runner    (1001) docker     (121)     7069 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/availability/ip.py
--rw-r--r--   0 runner    (1001) docker     (121)     3208 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/availability/params.py
--rw-r--r--   0 runner    (1001) docker     (121)     5232 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/availability/status.py
--rw-r--r--   0 runner    (1001) docker     (121)    10679 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/availability/url.py
--rw-r--r--   0 runner    (1001) docker     (121)    12426 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3194 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/complex_json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     3287 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/params_base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.665222 PyFunceble-4.1.3/PyFunceble/checker/reputation/
--rw-r--r--   0 runner    (1001) docker     (121)     2478 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/reputation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12289 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/reputation/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3022 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/reputation/domain.py
--rw-r--r--   0 runner    (1001) docker     (121)     3598 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/reputation/domain_and_ip.py
--rw-r--r--   0 runner    (1001) docker     (121)     3349 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/reputation/ip.py
--rw-r--r--   0 runner    (1001) docker     (121)     2813 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/reputation/params.py
--rw-r--r--   0 runner    (1001) docker     (121)     4059 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/reputation/status.py
--rw-r--r--   0 runner    (1001) docker     (121)     4111 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/reputation/url.py
--rw-r--r--   0 runner    (1001) docker     (121)     3515 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/status_base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.669222 PyFunceble-4.1.3/PyFunceble/checker/syntax/
--rw-r--r--   0 runner    (1001) docker     (121)     2474 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/syntax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4484 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/syntax/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4819 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/syntax/domain.py
--rw-r--r--   0 runner    (1001) docker     (121)     6897 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/syntax/domain_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5637 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/syntax/ip.py
--rw-r--r--   0 runner    (1001) docker     (121)     8055 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/syntax/ipv4.py
--rw-r--r--   0 runner    (1001) docker     (121)     4392 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/syntax/ipv6.py
--rw-r--r--   0 runner    (1001) docker     (121)     2805 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/syntax/params.py
--rw-r--r--   0 runner    (1001) docker     (121)     4696 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/syntax/second_lvl_domain.py
--rw-r--r--   0 runner    (1001) docker     (121)     3164 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/syntax/status.py
--rw-r--r--   0 runner    (1001) docker     (121)     4243 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/syntax/subdomain.py
--rw-r--r--   0 runner    (1001) docker     (121)     4152 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/syntax/url.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.669222 PyFunceble-4.1.3/PyFunceble/checker/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     2460 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4198 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/checker/utils/whois.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.669222 PyFunceble-4.1.3/PyFunceble/cli/
--rw-r--r--   0 runner    (1001) docker     (121)     2457 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.669222 PyFunceble-4.1.3/PyFunceble/cli/continuous_integration/
--rw-r--r--   0 runner    (1001) docker     (121)     2505 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/continuous_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    38938 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/continuous_integration/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3725 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/continuous_integration/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3959 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/continuous_integration/github_actions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4275 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/continuous_integration/gitlab_ci.py
--rw-r--r--   0 runner    (1001) docker     (121)     3897 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/continuous_integration/jenkins.py
--rw-r--r--   0 runner    (1001) docker     (121)     3889 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/continuous_integration/travis_ci.py
--rw-r--r--   0 runner    (1001) docker     (121)     3605 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/continuous_integration/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    10478 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/credential_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.673222 PyFunceble-4.1.3/PyFunceble/cli/entry_points/
--rw-r--r--   0 runner    (1001) docker     (121)     2442 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5157 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/entry_points/clean.py
--rw-r--r--   0 runner    (1001) docker     (121)     4151 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/entry_points/iana.py
--rw-r--r--   0 runner    (1001) docker     (121)     5668 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/entry_points/production.py
--rw-r--r--   0 runner    (1001) docker     (121)     4336 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/entry_points/public_suffix.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.673222 PyFunceble-4.1.3/PyFunceble/cli/entry_points/pyfunceble/
--rw-r--r--   0 runner    (1001) docker     (121)     2489 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/entry_points/pyfunceble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4759 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/entry_points/pyfunceble/argsparser.py
--rw-r--r--   0 runner    (1001) docker     (121)    45918 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/entry_points/pyfunceble/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     7187 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/execution_time.py
--rw-r--r--   0 runner    (1001) docker     (121)     2580 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/facility.py
--rw-r--r--   0 runner    (1001) docker     (121)     2574 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)    18209 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/file_preloader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.673222 PyFunceble-4.1.3/PyFunceble/cli/filesystem/
--rw-r--r--   0 runner    (1001) docker     (121)     2487 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4817 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/filesystem/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (121)     6390 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/filesystem/counter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4811 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/filesystem/dir_base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.673222 PyFunceble-4.1.3/PyFunceble/cli/filesystem/dir_structure/
--rw-r--r--   0 runner    (1001) docker     (121)     2495 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/filesystem/dir_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4286 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/filesystem/dir_structure/backup.py
--rw-r--r--   0 runner    (1001) docker     (121)     5366 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/filesystem/dir_structure/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5874 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/filesystem/dir_structure/restore.py
--rw-r--r--   0 runner    (1001) docker     (121)     4920 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/filesystem/json_base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.673222 PyFunceble-4.1.3/PyFunceble/cli/filesystem/printer/
--rw-r--r--   0 runner    (1001) docker     (121)     2488 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/filesystem/printer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10779 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/filesystem/printer/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6815 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/filesystem/printer/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     7671 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/filesystem/printer/stdout.py
--rw-r--r--   0 runner    (1001) docker     (121)     5728 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/filesystem/registrar_counter.py
--rw-r--r--   0 runner    (1001) docker     (121)    24041 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/filesystem/status_file.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.673222 PyFunceble-4.1.3/PyFunceble/cli/migrators/
--rw-r--r--   0 runner    (1001) docker     (121)     2442 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/migrators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7291 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/migrators/alembic.py
--rw-r--r--   0 runner    (1001) docker     (121)     3287 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/migrators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.677222 PyFunceble-4.1.3/PyFunceble/cli/migrators/csv_file/
--rw-r--r--   0 runner    (1001) docker     (121)     2447 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/migrators/csv_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5778 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/migrators/csv_file/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3247 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/migrators/csv_file/inactive_source_delete.py
--rw-r--r--   0 runner    (1001) docker     (121)     3185 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/migrators/csv_file/whois_registrar_add.py
--rw-r--r--   0 runner    (1001) docker     (121)     4616 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/migrators/db_base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.677222 PyFunceble-4.1.3/PyFunceble/cli/migrators/file_cleanup/
--rw-r--r--   0 runner    (1001) docker     (121)     2448 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/migrators/file_cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4123 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/migrators/file_cleanup/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2975 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/migrators/file_cleanup/hashes_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     2975 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/migrators/file_cleanup/mining_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     3054 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/migrators/file_cleanup/production_config_file.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.677222 PyFunceble-4.1.3/PyFunceble/cli/migrators/json2csv/
--rw-r--r--   0 runner    (1001) docker     (121)     2447 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/migrators/json2csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4536 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/migrators/json2csv/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6149 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/migrators/json2csv/inactive.py
--rw-r--r--   0 runner    (1001) docker     (121)     5690 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/migrators/json2csv/whois.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.677222 PyFunceble-4.1.3/PyFunceble/cli/migrators/mariadb/
--rw-r--r--   0 runner    (1001) docker     (121)     2456 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/migrators/mariadb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5253 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/migrators/mariadb/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     7051 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/migrators/mariadb/file_and_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     4440 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/migrators/mariadb/whois_record_idna_subject.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.681223 PyFunceble-4.1.3/PyFunceble/cli/processes/
--rw-r--r--   0 runner    (1001) docker     (121)     2650 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/processes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15642 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/processes/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3051 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/processes/chancy_producer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3037 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/processes/chancy_tester.py
--rw-r--r--   0 runner    (1001) docker     (121)     2790 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/processes/dir_files_sorter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2748 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/processes/file_sorter.py
--rw-r--r--   0 runner    (1001) docker     (121)    16946 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/processes/migrator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2710 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/processes/miner.py
--rw-r--r--   0 runner    (1001) docker     (121)     2731 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/processes/producer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2717 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/processes/tester.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.681223 PyFunceble-4.1.3/PyFunceble/cli/processes/workers/
--rw-r--r--   0 runner    (1001) docker     (121)     2448 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/processes/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13952 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/processes/workers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/processes/workers/chancy_producer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3630 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/processes/workers/chancy_tester.py
--rw-r--r--   0 runner    (1001) docker     (121)     6002 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/processes/workers/dir_files_sorter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4136 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/processes/workers/file_sorter.py
--rw-r--r--   0 runner    (1001) docker     (121)     8032 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/processes/workers/file_sorter_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3508 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/processes/workers/migrator.py
--rw-r--r--   0 runner    (1001) docker     (121)     7117 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/processes/workers/miner.py
--rw-r--r--   0 runner    (1001) docker     (121)    16657 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/processes/workers/producer.py
--rw-r--r--   0 runner    (1001) docker     (121)    11724 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/processes/workers/tester.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.681223 PyFunceble-4.1.3/PyFunceble/cli/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)     2441 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9981 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/scripts/iana.py
--rw-r--r--   0 runner    (1001) docker     (121)    17909 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/scripts/production.py
--rw-r--r--   0 runner    (1001) docker     (121)     6483 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/scripts/public_suffix.py
--rw-r--r--   0 runner    (1001) docker     (121)     9628 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/storage.py
--rw-r--r--   0 runner    (1001) docker     (121)     3160 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/storage_facility.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.681223 PyFunceble-4.1.3/PyFunceble/cli/system/
--rw-r--r--   0 runner    (1001) docker     (121)     2512 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4878 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/system/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8360 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/system/integrator.py
--rw-r--r--   0 runner    (1001) docker     (121)    40347 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/system/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.681223 PyFunceble-4.1.3/PyFunceble/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     2455 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3625 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/utils/ascii_logo.py
--rw-r--r--   0 runner    (1001) docker     (121)     4365 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/utils/sort.py
--rw-r--r--   0 runner    (1001) docker     (121)     5628 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/utils/stdout.py
--rw-r--r--   0 runner    (1001) docker     (121)     9635 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (121)    13348 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/cli/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.685223 PyFunceble-4.1.3/PyFunceble/config/
--rw-r--r--   0 runner    (1001) docker     (121)     2458 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12642 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/config/compare.py
--rw-r--r--   0 runner    (1001) docker     (121)    14684 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/config/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.685223 PyFunceble-4.1.3/PyFunceble/converter/
--rw-r--r--   0 runner    (1001) docker     (121)     2440 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12830 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/converter/adblock_input_line2subject.py
--rw-r--r--   0 runner    (1001) docker     (121)     3628 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/converter/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4292 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/converter/cidr2subject.py
--rw-r--r--   0 runner    (1001) docker     (121)     4745 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/converter/input_line2subject.py
--rw-r--r--   0 runner    (1001) docker     (121)     3695 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/converter/internal_url.py
--rw-r--r--   0 runner    (1001) docker     (121)     3656 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/converter/rpz_input_line2subject.py
--rw-r--r--   0 runner    (1001) docker     (121)     9019 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/converter/rpz_policy2subject.py
--rw-r--r--   0 runner    (1001) docker     (121)     5105 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/converter/subject2complements.py
--rw-r--r--   0 runner    (1001) docker     (121)     3986 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/converter/url2netloc.py
--rw-r--r--   0 runner    (1001) docker     (121)     3547 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/converter/wildcard2subject.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.685223 PyFunceble-4.1.3/PyFunceble/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.685223 PyFunceble-4.1.3/PyFunceble/data/alembic/
--rw-r--r--   0 runner    (1001) docker     (121)     2444 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/data/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4750 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/data/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/data/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.689223 PyFunceble-4.1.3/PyFunceble/data/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (121)     1806 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/data/alembic/versions/35c79626ecb9_fix_some_columns.py
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/data/alembic/versions/3a4c55a9320d_add_continue_table.py
--rw-r--r--   0 runner    (1001) docker     (121)     1198 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/data/alembic/versions/3d6f4a33cdb2_add_inactive_table.py
--rw-r--r--   0 runner    (1001) docker     (121)     1294 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/data/alembic/versions/45713fea8097_deletion_uneeded_columns_from_whois_.py
--rw-r--r--   0 runner    (1001) docker     (121)      757 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/data/alembic/versions/459a0d7b8f09_add_idna_subject_column_into_whois.py
--rw-r--r--   0 runner    (1001) docker     (121)      806 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/data/alembic/versions/6f4729deaf03_delete_inactive_source_column.py
--rw-r--r--   0 runner    (1001) docker     (121)     2799 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/data/alembic/versions/7bcf7fa64ba1_rename_created_to_created_at_and.py
--rw-r--r--   0 runner    (1001) docker     (121)     2181 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/data/alembic/versions/83ada95132bf_delete_the_file_table.py
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/data/alembic/versions/912bbcb77a6c_add_registrar_column.py
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/data/alembic/versions/95dc17ddd729_introduction_of_the_session_id_column.py
--rw-r--r--   0 runner    (1001) docker     (121)     2456 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/data/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4236 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/data/alembic/versions/ade87195b0a0_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1721 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/data/alembic/versions/bef7bcaac3f2_make_id_a_bigint.py
--rw-r--r--   0 runner    (1001) docker     (121)      930 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/data/alembic/versions/d8893cd406db_allow_whois_record_to_be_empty_null.py
--rw-r--r--   0 runner    (1001) docker     (121)     2125 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/data/alembic/versions/e04e8301d1a2_deletion_of_the_mined_table.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.689223 PyFunceble-4.1.3/PyFunceble/data/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (121)    11729 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/data/infrastructure/.PyFunceble_production.yaml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/data/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4376 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/data/infrastructure/dir_structure_production.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.689223 PyFunceble-4.1.3/PyFunceble/database/
--rw-r--r--   0 runner    (1001) docker     (121)     2496 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.689223 PyFunceble-4.1.3/PyFunceble/database/credential/
--rw-r--r--   0 runner    (1001) docker     (121)     2466 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/database/credential/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12171 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/database/credential/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2655 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/database/credential/mariadb.py
--rw-r--r--   0 runner    (1001) docker     (121)     2649 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/database/credential/mysql.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.689223 PyFunceble-4.1.3/PyFunceble/database/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)     2450 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/database/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3046 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/database/schemas/autocontinue.py
--rw-r--r--   0 runner    (1001) docker     (121)     2945 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/database/schemas/inactive.py
--rw-r--r--   0 runner    (1001) docker     (121)     3888 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/database/schemas/status.py
--rw-r--r--   0 runner    (1001) docker     (121)     2936 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/database/schemas/whois_record.py
--rw-r--r--   0 runner    (1001) docker     (121)     7324 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/database/session.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.693223 PyFunceble-4.1.3/PyFunceble/database/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (121)     2476 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/database/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2659 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/database/sqlalchemy/all_schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)     3482 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/database/sqlalchemy/base_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.693223 PyFunceble-4.1.3/PyFunceble/dataset/
--rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.693223 PyFunceble-4.1.3/PyFunceble/dataset/autocontinue/
--rw-r--r--   0 runner    (1001) docker     (121)     2465 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/dataset/autocontinue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3503 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/dataset/autocontinue/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6261 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/dataset/autocontinue/csv.py
--rw-r--r--   0 runner    (1001) docker     (121)     4272 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/dataset/autocontinue/mariadb.py
--rw-r--r--   0 runner    (1001) docker     (121)     2703 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/dataset/autocontinue/mysql.py
--rw-r--r--   0 runner    (1001) docker     (121)     5273 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     9678 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/dataset/csv_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     9407 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/dataset/db_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4103 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/dataset/iana.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.693223 PyFunceble-4.1.3/PyFunceble/dataset/inactive/
--rw-r--r--   0 runner    (1001) docker     (121)     2474 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/dataset/inactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3246 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/dataset/inactive/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4003 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/dataset/inactive/csv.py
--rw-r--r--   0 runner    (1001) docker     (121)     3728 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/dataset/inactive/mariadb.py
--rw-r--r--   0 runner    (1001) docker     (121)     2701 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/dataset/inactive/mysql.py
--rw-r--r--   0 runner    (1001) docker     (121)     4078 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/dataset/ipv4_reputation.py
--rw-r--r--   0 runner    (1001) docker     (121)    10540 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/dataset/mariadb_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4179 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/dataset/public_suffix.py
--rw-r--r--   0 runner    (1001) docker     (121)     6717 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/dataset/user_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.693223 PyFunceble-4.1.3/PyFunceble/dataset/whois/
--rw-r--r--   0 runner    (1001) docker     (121)     2471 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/dataset/whois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4036 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/dataset/whois/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6143 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/dataset/whois/csv.py
--rw-r--r--   0 runner    (1001) docker     (121)     6279 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/dataset/whois/mariadb.py
--rw-r--r--   0 runner    (1001) docker     (121)     2686 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/dataset/whois/mysql.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.697224 PyFunceble-4.1.3/PyFunceble/downloader/
--rw-r--r--   0 runner    (1001) docker     (121)     2437 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8839 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/downloader/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2961 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/downloader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3073 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/downloader/iana.py
--rw-r--r--   0 runner    (1001) docker     (121)     3160 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/downloader/ipv4_reputation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3107 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/downloader/public_suffix.py
--rw-r--r--   0 runner    (1001) docker     (121)     3106 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/downloader/user_agents.py
--rw-r--r--   0 runner    (1001) docker     (121)     2795 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/facility.py
--rw-r--r--   0 runner    (1001) docker     (121)     2580 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.697224 PyFunceble-4.1.3/PyFunceble/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)     2433 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7635 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/helpers/command.py
--rw-r--r--   0 runner    (1001) docker     (121)    13773 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/helpers/dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     5980 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/helpers/directory.py
--rw-r--r--   0 runner    (1001) docker     (121)     7481 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/helpers/download.py
--rw-r--r--   0 runner    (1001) docker     (121)     7238 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/helpers/environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (121)     2764 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6579 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/helpers/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     5264 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/helpers/hash.py
--rw-r--r--   0 runner    (1001) docker     (121)     5005 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/helpers/list.py
--rw-r--r--   0 runner    (1001) docker     (121)     6050 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/helpers/merge.py
--rw-r--r--   0 runner    (1001) docker     (121)     6927 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/helpers/regex.py
--rw-r--r--   0 runner    (1001) docker     (121)    16820 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.697224 PyFunceble-4.1.3/PyFunceble/query/
--rw-r--r--   0 runner    (1001) docker     (121)     2504 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17475 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.697224 PyFunceble-4.1.3/PyFunceble/query/dns/
--rw-r--r--   0 runner    (1001) docker     (121)     2469 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/dns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9297 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/dns/nameserver.py
--rw-r--r--   0 runner    (1001) docker     (121)    32785 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/dns/query_tool.py
--rw-r--r--   0 runner    (1001) docker     (121)     6405 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/dns/resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)    11767 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/http_status_code.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.701224 PyFunceble-4.1.3/PyFunceble/query/netinfo/
--rw-r--r--   0 runner    (1001) docker     (121)     2462 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/netinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3189 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/netinfo/address.py
--rw-r--r--   0 runner    (1001) docker     (121)     4562 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/netinfo/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3408 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/netinfo/hostbyaddr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.701224 PyFunceble-4.1.3/PyFunceble/query/record/
--rw-r--r--   0 runner    (1001) docker     (121)     2441 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3424 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/record/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3148 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/record/dns.py
--rw-r--r--   0 runner    (1001) docker     (121)     2945 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/record/whois.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.701224 PyFunceble-4.1.3/PyFunceble/query/requests/
--rw-r--r--   0 runner    (1001) docker     (121)     2472 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/requests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.701224 PyFunceble-4.1.3/PyFunceble/query/requests/adapter/
--rw-r--r--   0 runner    (1001) docker     (121)     2464 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/requests/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9571 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/requests/adapter/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5657 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/requests/adapter/http.py
--rw-r--r--   0 runner    (1001) docker     (121)     6132 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/requests/adapter/https.py
--rw-r--r--   0 runner    (1001) docker     (121)    18032 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/requests/requester.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.701224 PyFunceble-4.1.3/PyFunceble/query/whois/
--rw-r--r--   0 runner    (1001) docker     (121)     2485 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/whois/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.701224 PyFunceble-4.1.3/PyFunceble/query/whois/converter/
--rw-r--r--   0 runner    (1001) docker     (121)     2477 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/whois/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4367 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/whois/converter/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3450 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/whois/converter/digit2digits.py
--rw-r--r--   0 runner    (1001) docker     (121)    13416 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/whois/converter/expiration_date.py
--rw-r--r--   0 runner    (1001) docker     (121)     4321 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/whois/converter/month2unified.py
--rw-r--r--   0 runner    (1001) docker     (121)     4725 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/whois/converter/registrar.py
--rw-r--r--   0 runner    (1001) docker     (121)    14649 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/query/whois/query_tool.py
--rw-r--r--   0 runner    (1001) docker     (121)     2572 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/sessions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6270 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/storage.py
--rw-r--r--   0 runner    (1001) docker     (121)     4823 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/storage_facility.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.701224 PyFunceble-4.1.3/PyFunceble/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     2474 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3910 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/utils/platform.py
--rw-r--r--   0 runner    (1001) docker     (121)     4556 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/utils/profile.py
--rw-r--r--   0 runner    (1001) docker     (121)     8320 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/PyFunceble/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-20 11:24:20.665222 PyFunceble-4.1.3/PyFunceble.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12213 2022-11-20 11:24:20.000000 PyFunceble-4.1.3/PyFunceble.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11195 2022-11-20 11:24:20.000000 PyFunceble-4.1.3/PyFunceble.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-20 11:24:20.000000 PyFunceble-4.1.3/PyFunceble.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-11-20 11:24:20.000000 PyFunceble-4.1.3/PyFunceble.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-11-20 11:24:20.000000 PyFunceble-4.1.3/PyFunceble.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-11-20 11:24:20.000000 PyFunceble-4.1.3/PyFunceble.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11174 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/requirements.docs.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/requirements.test.txt
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/requirements.win.txt
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-11-20 11:24:20.705224 PyFunceble-4.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    10223 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1419 2022-11-20 11:24:12.000000 PyFunceble-4.1.3/version.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.628876 PyFunceble-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12343 2023-05-29 09:55:36.628876 PyFunceble-4.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.584876 PyFunceble-4.2.0/PyFunceble/
+-rw-r--r--   0 runner    (1001) docker     (123)    22809 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.588876 PyFunceble-4.2.0/PyFunceble/checker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.588876 PyFunceble-4.2.0/PyFunceble/checker/availability/
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/availability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37536 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/availability/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/availability/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/availability/domain_and_ip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.588876 PyFunceble-4.2.0/PyFunceble/checker/availability/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/availability/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/availability/extras/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/availability/extras/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/availability/extras/etoxic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/availability/extras/parked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/availability/extras/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/availability/extras/subject_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/availability/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/availability/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/availability/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/availability/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13673 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/complex_json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/params_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.592876 PyFunceble-4.2.0/PyFunceble/checker/reputation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/reputation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/reputation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/reputation/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/reputation/domain_and_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/reputation/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/reputation/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/reputation/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/reputation/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/status_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.592876 PyFunceble-4.2.0/PyFunceble/checker/syntax/
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/syntax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/syntax/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/syntax/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/syntax/domain_and_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/syntax/domain_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/syntax/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/syntax/ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/syntax/ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/syntax/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/syntax/second_lvl_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/syntax/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/syntax/subdomain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/syntax/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.592876 PyFunceble-4.2.0/PyFunceble/checker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/checker/utils/whois.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.592876 PyFunceble-4.2.0/PyFunceble/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.596876 PyFunceble-4.2.0/PyFunceble/cli/continuous_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/continuous_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38944 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/continuous_integration/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/continuous_integration/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/continuous_integration/github_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/continuous_integration/gitlab_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/continuous_integration/jenkins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/continuous_integration/travis_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/continuous_integration/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10602 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/credential_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.596876 PyFunceble-4.2.0/PyFunceble/cli/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/entry_points/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/entry_points/iana.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/entry_points/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/entry_points/public_suffix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.596876 PyFunceble-4.2.0/PyFunceble/cli/entry_points/pyfunceble/
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/entry_points/pyfunceble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/entry_points/pyfunceble/argsparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45951 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/entry_points/pyfunceble/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/execution_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/file_preloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.600876 PyFunceble-4.2.0/PyFunceble/cli/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/filesystem/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/filesystem/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/filesystem/dir_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.600876 PyFunceble-4.2.0/PyFunceble/cli/filesystem/dir_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/filesystem/dir_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/filesystem/dir_structure/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/filesystem/dir_structure/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/filesystem/dir_structure/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/filesystem/json_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.600876 PyFunceble-4.2.0/PyFunceble/cli/filesystem/printer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/filesystem/printer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10785 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/filesystem/printer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/filesystem/printer/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/filesystem/printer/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/filesystem/registrar_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24648 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/filesystem/status_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.600876 PyFunceble-4.2.0/PyFunceble/cli/migrators/
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/migrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/migrators/alembic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/migrators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.604876 PyFunceble-4.2.0/PyFunceble/cli/migrators/csv_file/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/migrators/csv_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/migrators/csv_file/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/migrators/csv_file/inactive_source_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/migrators/csv_file/whois_registrar_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/migrators/db_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.604876 PyFunceble-4.2.0/PyFunceble/cli/migrators/file_cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/migrators/file_cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/migrators/file_cleanup/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/migrators/file_cleanup/hashes_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/migrators/file_cleanup/mining_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/migrators/file_cleanup/production_config_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.604876 PyFunceble-4.2.0/PyFunceble/cli/migrators/json2csv/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/migrators/json2csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/migrators/json2csv/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/migrators/json2csv/inactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/migrators/json2csv/whois.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.604876 PyFunceble-4.2.0/PyFunceble/cli/migrators/mariadb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/migrators/mariadb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/migrators/mariadb/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/migrators/mariadb/file_and_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/migrators/mariadb/whois_record_idna_subject.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.604876 PyFunceble-4.2.0/PyFunceble/cli/processes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/processes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/processes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/processes/chancy_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/processes/chancy_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/processes/dir_files_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/processes/file_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16952 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/processes/migrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/processes/miner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/processes/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/processes/tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.608876 PyFunceble-4.2.0/PyFunceble/cli/processes/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/processes/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13958 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/processes/workers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/processes/workers/chancy_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/processes/workers/chancy_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/processes/workers/dir_files_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/processes/workers/file_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/processes/workers/file_sorter_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/processes/workers/migrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/processes/workers/miner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16991 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/processes/workers/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/processes/workers/tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.608876 PyFunceble-4.2.0/PyFunceble/cli/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9987 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/scripts/iana.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17915 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/scripts/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/scripts/public_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11885 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/storage_facility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.608876 PyFunceble-4.2.0/PyFunceble/cli/system/
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/system/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/system/integrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42652 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/system/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.608876 PyFunceble-4.2.0/PyFunceble/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/utils/ascii_logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/utils/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/utils/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13354 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/cli/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.612876 PyFunceble-4.2.0/PyFunceble/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12648 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/config/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14689 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/config/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.612876 PyFunceble-4.2.0/PyFunceble/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13796 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/converter/adblock_input_line2subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/converter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/converter/cidr2subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/converter/input_line2subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/converter/internal_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/converter/rpz_input_line2subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/converter/rpz_policy2subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/converter/subject2complements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/converter/url2netloc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/converter/wildcard2subject.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.612876 PyFunceble-4.2.0/PyFunceble/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.612876 PyFunceble-4.2.0/PyFunceble/data/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/alembic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.612876 PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.616876 PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/35c79626ecb9_fix_some_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/3a4c55a9320d_add_continue_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/3d6f4a33cdb2_add_inactive_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/45713fea8097_deletion_uneeded_columns_from_whois_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/459a0d7b8f09_add_idna_subject_column_into_whois.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/6f4729deaf03_delete_inactive_source_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/7bcf7fa64ba1_rename_created_to_created_at_and.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/83ada95132bf_delete_the_file_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/912bbcb77a6c_add_registrar_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/95dc17ddd729_introduction_of_the_session_id_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/ade87195b0a0_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/bef7bcaac3f2_make_id_a_bigint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/d8893cd406db_allow_whois_record_to_be_empty_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/e04e8301d1a2_deletion_of_the_mined_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.616876 PyFunceble-4.2.0/PyFunceble/data/alembic/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/alembic/postgresql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/alembic/postgresql/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/alembic/postgresql/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.616876 PyFunceble-4.2.0/PyFunceble/data/alembic/postgresql/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/alembic/postgresql/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/alembic/postgresql/versions/a32ac5d66eee_initial_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.616876 PyFunceble-4.2.0/PyFunceble/data/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)    11622 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/infrastructure/.PyFunceble_production.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/data/infrastructure/dir_structure_production.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.616876 PyFunceble-4.2.0/PyFunceble/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.616876 PyFunceble-4.2.0/PyFunceble/database/credential/
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/database/credential/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/database/credential/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/database/credential/mariadb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/database/credential/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/database/credential/postgresql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.616876 PyFunceble-4.2.0/PyFunceble/database/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/database/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/database/schemas/autocontinue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/database/schemas/inactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/database/schemas/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/database/schemas/whois_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/database/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.616876 PyFunceble-4.2.0/PyFunceble/database/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/database/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/database/sqlalchemy/all_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/database/sqlalchemy/base_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.620876 PyFunceble-4.2.0/PyFunceble/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.620876 PyFunceble-4.2.0/PyFunceble/dataset/autocontinue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/dataset/autocontinue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/dataset/autocontinue/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/dataset/autocontinue/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/dataset/autocontinue/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/dataset/csv_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/dataset/db_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/dataset/iana.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.620876 PyFunceble-4.2.0/PyFunceble/dataset/inactive/
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/dataset/inactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/dataset/inactive/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/dataset/inactive/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/dataset/inactive/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/dataset/ipv4_reputation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/dataset/public_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/dataset/sql_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/dataset/user_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.620876 PyFunceble-4.2.0/PyFunceble/dataset/whois/
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/dataset/whois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/dataset/whois/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/dataset/whois/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/dataset/whois/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.620876 PyFunceble-4.2.0/PyFunceble/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8845 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/downloader/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/downloader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/downloader/iana.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/downloader/ipv4_reputation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/downloader/public_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/downloader/user_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.624876 PyFunceble-4.2.0/PyFunceble/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/helpers/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/helpers/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/helpers/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/helpers/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/helpers/environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/helpers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/helpers/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/helpers/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/helpers/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/helpers/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16825 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.624876 PyFunceble-4.2.0/PyFunceble/query/
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17480 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.624876 PyFunceble-4.2.0/PyFunceble/query/dns/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/dns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/dns/nameserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32791 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/dns/query_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/dns/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11773 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/http_status_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.624876 PyFunceble-4.2.0/PyFunceble/query/netinfo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/netinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/netinfo/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/netinfo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/netinfo/hostbyaddr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.624876 PyFunceble-4.2.0/PyFunceble/query/record/
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/record/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/record/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/record/whois.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.624876 PyFunceble-4.2.0/PyFunceble/query/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/requests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.628876 PyFunceble-4.2.0/PyFunceble/query/requests/adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/requests/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/requests/adapter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/requests/adapter/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/requests/adapter/https.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/requests/requester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.628876 PyFunceble-4.2.0/PyFunceble/query/whois/
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/whois/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.628876 PyFunceble-4.2.0/PyFunceble/query/whois/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/whois/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/whois/converter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/whois/converter/digit2digits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13422 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/whois/converter/expiration_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/whois/converter/month2unified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/whois/converter/registrar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14654 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/query/whois/query_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/storage_facility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.628876 PyFunceble-4.2.0/PyFunceble/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/utils/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/utils/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/PyFunceble/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:36.588876 PyFunceble-4.2.0/PyFunceble.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12343 2023-05-29 09:55:36.000000 PyFunceble-4.2.0/PyFunceble.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-05-29 09:55:36.000000 PyFunceble-4.2.0/PyFunceble.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 09:55:36.000000 PyFunceble-4.2.0/PyFunceble.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-29 09:55:36.000000 PyFunceble-4.2.0/PyFunceble.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-29 09:55:36.000000 PyFunceble-4.2.0/PyFunceble.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 09:55:36.000000 PyFunceble-4.2.0/PyFunceble.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/requirements.docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/requirements.test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/requirements.win.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-29 09:55:36.628876 PyFunceble-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-29 09:55:26.000000 PyFunceble-4.2.0/version.yaml
```

### Comparing `PyFunceble-4.1.3/CODE_OF_CONDUCT.rst` & `PyFunceble-4.2.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `PyFunceble-4.1.3/CONTRIBUTING.rst` & `PyFunceble-4.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `PyFunceble-4.1.3/LICENSE` & `PyFunceble-4.2.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
 
-   Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+   Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PKG-INFO` & `PyFunceble-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFunceble
-Version: 4.1.3
+Version: 4.2.0
 Summary: The tool to check the availability or syntax of domain, IP or URL.
 Home-page: https://github.com/funilrys/PyFunceble
 Author: funilrys
 Author-email: contact@funilrys.com
 License: Apache 2.0
 Project-URL: Documentation, https://pyfunceble.readthedocs.io/en/latest/
 Project-URL: Funding, https://github.com/sponsors/funilrys
@@ -15,18 +15,19 @@
 Classifier: Environment :: Console
 Classifier: Topic :: Internet
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.8, <4
 Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: psql
 Provides-Extra: full
 License-File: LICENSE
 
 .. image:: https://raw.githubusercontent.com/PyFunceble/logo/master/Green/HD/RM.png
 
 The tool to check the availability or syntax of domain, IP or URL
 -----------------------------------------------------------------
@@ -182,14 +183,15 @@
 -   Daniel - `@dnmTX`_
 -   gwarser - `@gwarser`_
 -   Haris Gušić - `@veracioux`_
 -   hawkeye116477 - `@hawkeye116477`_
 -   Human Being - `@T145`_
 -   Imre Kristoffer Eilertsen - `@DandelionSprout`_
 -   jawz101 - `@jawz101`_
+-   Josenilson Ferreira da SIlva - `@Nilsonfsilva`_
 -   keczuppp - `@keczuppp`_
 -   kowith337 - `@kowith337`_
 -   Mitchell Krog - `@mitchellkrogza`_
 -   NeolithEra - `@NeolithEra`_
 -   Odyseus - `@Odyseus`_
 -   opav - `@opav`_
 -   Reza Rizqullah - `@ybreza`_
@@ -259,15 +261,15 @@
 
 ___________________________________________
 
 License
 -------
 ::
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -310,14 +312,15 @@
 .. _@hawkeye116477: https://github.com/hawkeye116477
 .. _@jawz101: https://github.com/jawz101
 .. _@keczuppp: https://github.com/keczuppp
 .. _@kennethreitz: https://github.com/kennethreitz
 .. _@kowith337: https://github.com/kowith337
 .. _@mitchellkrogza: https://github.com/mitchellkrogza
 .. _@NeolithEra: https://github.com/NeolithEra
+.. _@Nilsonfsilva: https://github.com/Nilsonfsilva
 .. _@Odyseus: https://github.com/Odyseus
 .. _@opav: https://github.com/opav
 .. _@pi-hole: https://github.com/pi-hole/pi-hole
 .. _@PromoFaux: https://github.com/PromoFaux
 .. _@publicsuffix: https://github.com/publicsuffix
 .. _@rthalley: https://github.com/rthalley
 .. _@rusty-snake: https://github.com/rusty-snake
```

### Comparing `PyFunceble-4.1.3/PyFunceble/__init__.py` & `PyFunceble-4.2.0/PyFunceble/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -59,14 +59,15 @@
 from PyFunceble.checker.availability.status import AvailabilityCheckerStatus
 from PyFunceble.checker.availability.url import URLAvailabilityChecker
 from PyFunceble.checker.reputation.domain import DomainReputationChecker
 from PyFunceble.checker.reputation.domain_and_ip import DomainAndIPReputationChecker
 from PyFunceble.checker.reputation.ip import IPReputationChecker
 from PyFunceble.checker.reputation.url import URLReputationChecker
 from PyFunceble.checker.syntax.domain import DomainSyntaxChecker
+from PyFunceble.checker.syntax.domain_and_ip import DomainAndIPSyntaxChecker
 from PyFunceble.checker.syntax.ip import IPSyntaxChecker
 from PyFunceble.checker.syntax.ipv4 import IPv4SyntaxChecker
 from PyFunceble.checker.syntax.ipv6 import IPv6SyntaxChecker
 from PyFunceble.checker.syntax.second_lvl_domain import SecondLvlDomainSyntaxChecker
 from PyFunceble.checker.syntax.subdomain import SubDomainSyntaxChecker
 from PyFunceble.checker.syntax.url import URLSyntaxChecker
 from PyFunceble.converter.subject2complements import Subject2Complements
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/__init__.py` & `PyFunceble-4.2.0/PyFunceble/checker/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/availability/__init__.py` & `PyFunceble-4.2.0/PyFunceble/checker/availability/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/availability/base.py` & `PyFunceble-4.2.0/PyFunceble/checker/availability/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -58,21 +58,28 @@
 
 from sqlalchemy.orm import Session
 
 import PyFunceble.checker.utils.whois
 import PyFunceble.facility
 import PyFunceble.factory
 import PyFunceble.storage
-from PyFunceble.checker.availability.extra_rules import ExtraRulesHandler
+from PyFunceble.checker.availability.extras.base import ExtraRuleHandlerBase
+from PyFunceble.checker.availability.extras.dns import DNSRulesHandler
+from PyFunceble.checker.availability.extras.etoxic import EToxicHandler
+from PyFunceble.checker.availability.extras.rules import ExtraRulesHandler
+from PyFunceble.checker.availability.extras.subject_switch import (
+    SubjectSwitchRulesHandler,
+)
 from PyFunceble.checker.availability.params import AvailabilityCheckerParams
 from PyFunceble.checker.availability.status import AvailabilityCheckerStatus
 from PyFunceble.checker.base import CheckerBase
 from PyFunceble.checker.syntax.domain import DomainSyntaxChecker
 from PyFunceble.checker.syntax.ip import IPSyntaxChecker
 from PyFunceble.checker.syntax.url import URLSyntaxChecker
+from PyFunceble.converter.url2netloc import Url2Netloc
 from PyFunceble.helpers.regex import RegexHelper
 from PyFunceble.query.dns.query_tool import DNSQueryTool
 from PyFunceble.query.http_status_code import HTTPStatusCode
 from PyFunceble.query.netinfo.address import AddressInfo
 from PyFunceble.query.netinfo.hostbyaddr import HostByAddrInfo
 from PyFunceble.query.whois.query_tool import WhoisQueryTool
 
@@ -122,15 +129,16 @@
     whois_query_tool: Optional[WhoisQueryTool] = None
     addressinfo_query_tool: Optional[AddressInfo] = None
     hostbyaddr_query_tool: Optional[HostByAddrInfo] = None
     http_status_code_query_tool: Optional[HTTPStatusCode] = None
     domain_syntax_checker: Optional[DomainSyntaxChecker] = None
     ip_syntax_checker: Optional[IPSyntaxChecker] = None
     url_syntax_checker: Optional[URLSyntaxChecker] = None
-    extra_rules_handler: Optional[ExtraRulesHandler] = None
+    extra_rules_handlers: Optional[List[ExtraRuleHandlerBase]] = None
+    url2netloc: Optional[Url2Netloc] = None
 
     _use_extra_rules: bool = False
     _use_whois_lookup: bool = False
     _use_dns_lookup: bool = False
     _use_netinfo_lookup: bool = False
     _use_http_code_lookup: bool = False
     _use_reputation_lookup: bool = False
@@ -158,15 +166,21 @@
         self.whois_query_tool = WhoisQueryTool()
         self.addressinfo_query_tool = AddressInfo()
         self.hostbyaddr_query_tool = HostByAddrInfo()
         self.http_status_code_query_tool = HTTPStatusCode()
         self.domain_syntax_checker = DomainSyntaxChecker()
         self.ip_syntax_checker = IPSyntaxChecker()
         self.url_syntax_checker = URLSyntaxChecker()
-        self.extra_rules_handler = ExtraRulesHandler()
+        # WARNING: Put the aggressive one first!
+        self.extra_rules_handlers = [
+            SubjectSwitchRulesHandler(),
+            DNSRulesHandler(),
+            EToxicHandler(),
+            ExtraRulesHandler(),
+        ]
         self.db_session = db_session
 
         self.params = AvailabilityCheckerParams()
 
         self.status = AvailabilityCheckerStatus()
         self.status.params = self.params
         self.status.dns_lookup_record = self.dns_query_tool.lookup_record
@@ -498,21 +512,15 @@
         self.url_syntax_checker.subject = self.idna_subject
 
         self.status = AvailabilityCheckerStatus()
         self.status.params = self.params
         self.status.dns_lookup_record = self.dns_query_tool.lookup_record
         self.status.whois_lookup_record = self.whois_query_tool.lookup_record
 
-        self.status.subject = self.subject
-        self.status.idna_subject = self.idna_subject
-        self.status.status = None
-
-        self.query_syntax_checker()
-
-        return self
+        return super().subject_propagator()
 
     def should_we_continue_test(self, status_post_syntax_checker: str) -> bool:
         """
         Checks if we are allowed to continue a standard testing.
 
         Rules:
             1. No status available yet. Continue to next test method.
@@ -636,15 +644,15 @@
             if method in to_ignore or not method.startswith("guess_"):
                 continue
 
             getattr(self, method)()
 
         return self
 
-    def query_syntax_checker(self) -> "AvailabilityCheckerBase":
+    def query_common_checker(self) -> "AvailabilityCheckerBase":
         """
         Queries the syntax checker.
         """
 
         PyFunceble.facility.Logger.info(
             "Started to check the syntax of %r", self.status.idna_subject
         )
@@ -664,15 +672,15 @@
         self.status.ip_syntax = bool(self.status.ipv4_syntax or self.status.ipv6_syntax)
         self.status.url_syntax = self.url_syntax_checker.is_valid()
 
         PyFunceble.facility.Logger.info(
             "Finished to check the syntax of %r", self.status.idna_subject
         )
 
-        return self
+        return super().query_common_checker()
 
     @CheckerBase.ensure_subject_is_given
     def query_dns_record(self) -> Optional[Dict[str, Optional[List[str]]]]:
         """
         Tries to query the DNS record(s) of the given subject.
 
         .. versionchanged:: 4.1.0b8.dev
@@ -1012,14 +1020,44 @@
             )
 
         PyFunceble.facility.Logger.info(
             "Finished to try to query the status of %r from: Collection Lookup",
             self.status.idna_subject,
         )
 
+        return self
+
+    def try_to_query_status_from_extra_rules(self) -> "AvailabilityCheckerBase":
+        """
+        Tries to query the status from the extra rules.
+        """
+
+        PyFunceble.facility.Logger.info(
+            "Started to try to query the status of %r from: Extra Rules Lookup",
+            self.status.idna_subject,
+        )
+
+        if self.use_extra_rules:
+            for rule_handler in self.extra_rules_handlers:
+                rule_handler.set_status(self.status).start()
+
+                if self.status.status_after_extra_rules:
+                    PyFunceble.facility.Logger.info(
+                        "Could define the status of %r from: Extra Rules Lookup",
+                        self.status.idna_subject,
+                    )
+                    break
+
+        PyFunceble.facility.Logger.info(
+            "Finished to try to query the status of %r from: Extra Rules Lookup",
+            self.status.idna_subject,
+        )
+
+        return self
+
     @CheckerBase.ensure_subject_is_given
     @CheckerBase.update_status_date_after_query
     def query_status(self) -> "AvailabilityCheckerBase":
         """
         Queries the status and for for more action.
         """
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/availability/domain.py` & `PyFunceble-4.2.0/PyFunceble/checker/availability/domain.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -174,14 +174,14 @@
             PyFunceble.facility.Logger.info(
                 "Could not define status the status of %r. Setting to %r",
                 self.status.idna_subject,
                 self.status.status,
             )
 
         if self.use_extra_rules:
-            self.extra_rules_handler.set_status(self.status).start()
+            self.try_to_query_status_from_extra_rules()
 
         return self
 
     @staticmethod
     def is_valid() -> bool:  # pylint: disable=arguments-differ
         raise NotImplementedError()
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/availability/domain_and_ip.py` & `PyFunceble-4.2.0/PyFunceble/cli/utils/sort.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the domains and IP availability checker.
+Provides some utilities related to the sorting mechanism.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,87 +31,92 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-from typing import Union
+from typing import Any, Callable, List, Union
 
-from PyFunceble.checker.availability.base import AvailabilityCheckerBase
-from PyFunceble.checker.availability.domain import DomainAvailabilityChecker
-from PyFunceble.checker.availability.ip import IPAvailabilityChecker
-
-
-class DomainAndIPAvailabilityChecker(AvailabilityCheckerBase):
-    """
-    Provides the interface for checking the availability of a IP or domain.
-
-    :param str subject:
-        Optional, The subject to work with.
-    :param bool use_extra_rules:
-        Optional, Activates/Disables the usage of our own set of extra rules.
-    :param bool use_whois_lookup:
-        Optional, Activates/Disables the usage of the WHOIS lookup to gather
-        the status of the given :code:`subject`.
-    :param bool use_dns_lookup:
-        Optional, Activates/Disables the usage of the DNS lookup to gather the
-        status of the given :code:`subject`.
-    :param bool use_netinfo_lookup:
-        Optional, Activates/Disables the usage of the network information
-        lookup module to gather the status of the given :code:`subject`.
-    :param bool use_http_code_lookup:
-        Optional, Activates/Disables the usage of the HTTP status code lookup
-        to gather the status of the given :code:`subject`.
-    :param bool use_reputation_lookup:
-        Optional, Activates/Disables the usage of the reputation dataset
-        lookup to gather the status of the given :code:`subject`.
-    :param bool do_syntax_check_first:
-        Optional, Activates/Disables the check of the status before the actual
-        status gathering.
-    :param bool use_whois_db:
-        Optional, Activates/Disable the usage of a local database to store the
-        WHOIS datasets.
-    """
-
-    @AvailabilityCheckerBase.ensure_subject_is_given
-    @AvailabilityCheckerBase.update_status_date_after_query
-    def query_status(
-        self,
-    ) -> "DomainAndIPAvailabilityChecker":  # pragma: no cover ## Just a switch.
-        """
-        Queries the result without anything more.
-        """
-
-        query_object: Union[IPAvailabilityChecker, DomainAvailabilityChecker] = None
-
-        if self.status.ip_syntax:
-            query_object = IPAvailabilityChecker()
-        else:
-            query_object = DomainAvailabilityChecker()
-
-        query_object.__dict__ = self.__dict__
-
-        result = query_object.query_status()
-
-        self.__dict__.update(query_object.__dict__)
-
-        return result
-
-    @staticmethod
-    def is_valid() -> bool:  # pylint: disable=arguments-differ
-        raise NotImplementedError()
+import PyFunceble.facility
+import PyFunceble.storage
+from PyFunceble.converter.url2netloc import Url2Netloc
+from PyFunceble.helpers.regex import RegexHelper
+
+
+def standard(element: Any) -> List[Union[int, Any]]:
+    """
+    Provides the key to use for the standard sorting.
+
+    :param element:
+        The element to format.
+    """
+
+    element = element.strip()
+
+    if not element:
+        return []
+
+    regex_helper = RegexHelper()
+
+    element = Url2Netloc(element).get_converted().strip()
+
+    if PyFunceble.facility.ConfigLoader.is_already_loaded():
+        element = regex_helper.set_regex(
+            r"^%s\s+" % PyFunceble.storage.CONFIGURATION.cli_testing.hosts_ip
+        ).replace_match(element, "")
+
+    cleaned = regex_helper.set_regex(r"[^a-zA-Z0-9\.]").replace_match(element, "")
+
+    return [
+        int(x) if x.isdigit() else x
+        for x in regex_helper.set_regex(r"(\d+)").split(cleaned)
+    ]
+
+
+def hierarchical(element: Any) -> List[Union[int, Any]]:
+    """
+    Provides the key to use for the hierarchical sorting.
+
+    :param element:
+        The element to format.
+    """
+
+    element = element.strip()
+
+    if not element:
+        return []
+
+    element = Url2Netloc(element).get_converted().strip()
+
+    if PyFunceble.facility.ConfigLoader.is_already_loaded():
+        element = RegexHelper(
+            r"^%s\s+" % PyFunceble.storage.CONFIGURATION.cli_testing.hosts_ip
+        ).replace_match(element, "")
+
+    return standard(".".join(reversed(element.split("."))))
+
+
+def get_best_sorting_key() -> Callable[[Any], List[Union[int, Any]]]:
+    """
+    Provides the best sorting key from the configuration.
+    """
+
+    if PyFunceble.facility.ConfigLoader.is_already_loaded():
+        if PyFunceble.storage.CONFIGURATION.cli_testing.sorting_mode.hierarchical:
+            return hierarchical
+    return standard
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/availability/extra_rules.py` & `PyFunceble-4.2.0/PyFunceble/checker/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the domains availability checker.
+Provides the base of all checker.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,342 +31,416 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
+import datetime
 import functools
-import socket
-from typing import Callable, List, Optional
+from typing import Optional
 
-from box import Box
+import domain2idna
+from sqlalchemy.orm import Session
 
 import PyFunceble.facility
-import PyFunceble.factory
 import PyFunceble.storage
-from PyFunceble.checker.availability.status import AvailabilityCheckerStatus
-from PyFunceble.helpers.regex import RegexHelper
+from PyFunceble.checker.params_base import CheckerParamsBase
+from PyFunceble.checker.status_base import CheckerStatusBase
+from PyFunceble.converter.url2netloc import Url2Netloc
+from PyFunceble.query.collection import CollectionQueryTool
 
 
-class ExtraRulesHandler:
+class CheckerBase:
     """
-    Provides our very own extra rules handler.
+    Provides the base of all checker.
 
-    :param status:
-        The previously gathered status.
-    :type status:
-        :class:`~PyFunceble.checker.availability.status.AvailabilityCheckerStatus`
+    :param str subject:
+        Optional, The subject to work with.
+    :param bool do_syntax_check_first:
+        Optional, Forces the checker to first perform a syntax check,
+
+        .. warning::
+            This does not apply to the syntax checker - itself.
     """
 
-    _status: Optional[AvailabilityCheckerStatus] = None
+    STD_DO_SYNTAX_CHECK_FIRST: bool = False
+    STD_USE_COLLECTION: bool = False
 
-    regex_active2inactive: dict = {}
+    _do_syntax_check_first: bool = False
+    _use_collection: bool = False
 
-    http_codes_dataset: Optional[Box] = None
+    _subject: Optional[str] = None
+    _idna_subject: Optional[str] = None
 
-    def __init__(self, status: Optional[AvailabilityCheckerStatus] = None) -> None:
-        self.regex_active2inactive = {
-            r"\.000webhostapp\.com": [
-                (self.__switch_to_down_if, 410),
-            ],
-            r"\.24\.eu$": [(self.__switch_to_down_if, 503)],
-            r"\.altervista\.org$": [(self.__switch_to_down_if, 403)],
-            r"\.angelfire\.com$": [(self.__switch_to_down_if, 404)],
-            r"\.blogspot\.": [self.__handle_blogspot],
-            r"\.canalblog\.com$": [(self.__switch_to_down_if, 404)],
-            r"\.dr\.ag$": [(self.__switch_to_down_if, 503)],
-            r"\.fc2\.com$": [self.__handle_fc2_dot_com],
-            r"\.github\.io$": [(self.__switch_to_down_if, 404)],
-            r"\.godaddysites\.com$": [(self.__switch_to_down_if, 404)],
-            r"\.hpg.com.br$": [(self.__switch_to_down_if, 404)],
-            r"\.liveadvert\.com$": [(self.__switch_to_down_if, 404)],
-            r"\.skyrock\.com$": [(self.__switch_to_down_if, 404)],
-            r"\.tumblr\.com$": [(self.__switch_to_down_if, 404)],
-            r"\.wix\.com$": [(self.__switch_to_down_if, 404)],
-            r"\.wordpress\.com$": [self.__handle_wordpress_dot_com],
-            r"\.weebly\.com$": [(self.__switch_to_down_if, 404)],
-        }
+    url2netloc: Optional[Url2Netloc] = None
 
-        if PyFunceble.facility.ConfigLoader.is_already_loaded():
-            self.http_codes_dataset = PyFunceble.storage.HTTP_CODES
+    db_session: Optional[Session] = None
+    collection_query_tool: Optional[CollectionQueryTool] = None
+
+    status: Optional[CheckerStatusBase] = None
+    params: Optional[CheckerParamsBase] = None
+
+    def __init__(
+        self,
+        subject: Optional[str] = None,
+        *,
+        do_syntax_check_first: Optional[bool] = None,
+        db_session: Optional[Session] = None,
+        use_collection: Optional[bool] = None,
+    ) -> None:
+        self.collection_query_tool = CollectionQueryTool()
+        self.url2netloc = Url2Netloc()
+
+        if self.params is None:
+            self.params = CheckerParamsBase()
+
+        if self.status is None:
+            self.status = CheckerStatusBase()
+
+        if subject is not None:
+            self.subject = subject
+
+        if do_syntax_check_first is not None:
+            self.do_syntax_check_first = do_syntax_check_first
         else:
-            self.http_codes_dataset = PyFunceble.storage.STD_HTTP_CODES
+            self.do_syntax_check_first = self.STD_DO_SYNTAX_CHECK_FIRST
 
-        if status is not None:
-            self.status = status
+        if use_collection is not None:
+            self.use_collection = use_collection
+        else:
+            self.guess_and_set_use_collection()
 
-        # Be sure that all settings are loaded proprely!!
-        PyFunceble.factory.Requester.guess_all_settings()
+        self.db_session = db_session
 
-    def ensure_status_is_given(
-        func: Callable[..., "ExtraRulesHandler"]
-    ):  # pylint: disable=no-self-argument
+    def propagate_subject(func):  # pylint: disable=no-self-argument
         """
-        Ensures that the status is given before running the decorated method.
+        Propagates the subject to the object that need it after launching
+        the decorated method.
+        """
+
+        @functools.wraps(func)
+        def wrapper(self, *args, **kwargs):
+            result = func(self, *args, **kwargs)  # pylint: disable=not-callable
+
+            self.subject_propagator()
+
+            return result
+
+        return wrapper
+
+    def ensure_subject_is_given(func):  # pylint: disable=no-self-argument
+        """
+        Ensures that the subject is given before running the decorated method.
 
         :raise TypeError:
             If the subject is not a string.
         """
 
         @functools.wraps(func)
         def wrapper(self, *args, **kwargs):  # pragma: no cover ## Safety!
-            if not self.status:
+            if not isinstance(self.subject, str):
                 raise TypeError(
-                    f"<self.status> should be {AvailabilityCheckerStatus}, "
-                    f"{type(self.status)} given."
+                    f"<self.subject> should be {str}, {type(self.subject)} given."
                 )
 
             return func(self, *args, **kwargs)  # pylint: disable=not-callable
 
         return wrapper
 
+    def query_status_if_missing(func):  # pylint: disable=no-self-argument
+        """
+        Queries the status if it's missing.
+        """
+
+        @functools.wraps(func)
+        def wrapper(self, *args, **kwargs):  # pragma: no cover ## Safety!
+            if not self.status.status or self.status.status is None:
+                self.query_status()
+
+            return func(self, *args, **kwargs)  # pylint: disable=not-callable
+
+        return wrapper
+
+    def update_status_date_after_query(func):  # pylint: disable=no-self-argument
+        """
+        Updates the status dates after running the decorated method.
+        """
+
+        @functools.wraps(func)
+        def wrapper(self, *args, **kwargs):  # pragma: no cover ## Safety!
+            result = func(self, *args, **kwargs)  # pylint: disable=not-callable
+
+            self.status.tested_at = datetime.datetime.utcnow()
+
+            return result
+
+        return wrapper
+
     @property
-    def status(self) -> Optional[AvailabilityCheckerStatus]:
+    def subject(self) -> Optional[str]:
         """
-        Provides the current state of the :code:`_status` attribute.
+        Provides the current state of the :code:`_subject` attribute.
         """
 
-        return self._status
+        return self._subject
 
-    @status.setter
-    def status(self, value: AvailabilityCheckerStatus) -> None:
+    @subject.setter
+    @propagate_subject
+    def subject(self, value: str) -> None:
         """
-        Sets the status to work with.
+        Sets the subject to work with.
 
         :param value:
-            The status to work with.
+            The subject to set.
 
         :raise TypeError:
-            When the given :code:`value` is not a
-            :class:`~PyFunceble.checker.availability.status.AvailabilityCheckerStatus`.
+            When the given :code:`value` is not a :py:class:`str`.
+        :raise ValueError:
+            When the given :code:`value` is empty.
         """
 
-        if not isinstance(value, AvailabilityCheckerStatus):
-            raise TypeError(
-                f"<value> should be {AvailabilityCheckerStatus}, {type(value)} given."
-            )
+        if not isinstance(value, str):
+            raise TypeError(f"<value> should be {str}, {type(value)} given.")
+
+        if not value:
+            raise ValueError("<value> should not be empty.")
 
-        self._status = value
+        self._subject = value
 
-    def set_status(self, value: AvailabilityCheckerStatus) -> "ExtraRulesHandler":
+        try:
+            self.idna_subject = domain2idna.domain2idna(value)
+        except ValueError:
+            self.idna_subject = value
+
+    def set_subject(self, value: str) -> "CheckerBase":
         """
-        Sets the status to work with.
+        Sets the subject to work with.
 
         :param value:
-            The status to work with.
+            The subject to set.
         """
 
-        self.status = value
+        self.subject = value
 
         return self
 
-    def __web_regex_handler(
-        self,
-        url: str,
-        regex_list: List[str],
-        method: Callable[..., "ExtraRulesHandler"],
-    ) -> "ExtraRulesHandler":
+    @property
+    def idna_subject(self) -> Optional[str]:
         """
-        Handles a web request along with a regex filter.
+        Provides the current state of the :code:`_idna_subject` attribute.
         """
 
-        try:
-            req = PyFunceble.factory.Requester.get(url, allow_redirects=True)
+        return self._idna_subject
 
-            for regex in regex_list:
-                if regex in req.text or RegexHelper(regex).match(
-                    req.text, return_match=False
-                ):
-                    method()
-                    break
-        except (
-            PyFunceble.factory.Requester.exceptions.RequestException,
-            PyFunceble.factory.Requester.exceptions.InvalidURL,
-            PyFunceble.factory.Requester.exceptions.Timeout,
-            PyFunceble.factory.Requester.exceptions.ConnectionError,
-            PyFunceble.factory.Requester.urllib3_exceptions.InvalidHeader,
-            socket.timeout,
-        ):
-            pass
+    @idna_subject.setter
+    def idna_subject(self, value: str) -> None:
+        """
+        Sets the subject to work with.
 
-        return self
+        :param value:
+            The subject to set.
 
-    def __regex_registry_handler(self, regex_registry: dict) -> "ExtraRulesHandler":
-        """
-        Handles the standard regex lookup case.
+        :raise TypeError:
+            When the given :code:`value` is not a :py:class:`str`.
+        :raise ValueError:
+            When the given :code:`value` is empty.
         """
 
-        for (
-            regex,
-            data,
-        ) in regex_registry.items():
-            broken = False
-            for element in data:
-                if RegexHelper(regex).match(self.status.subject, return_match=False):
-                    if isinstance(element, tuple):
-                        element[0](*element[1:])
-                    else:
-                        element()
-
-                    broken = True
-                    break
+        if not isinstance(value, str):
+            raise TypeError(f"<value> should be {str}, {type(value)} given.")
 
-            if broken:
-                break
+        if not value:
+            raise ValueError("<value> should not be empty.")
 
-        return self
+        self._idna_subject = value
 
-    def __switch_to_down(self) -> "ExtraRulesHandler":
+    def set_idna_subject(self, value: str) -> "CheckerBase":
         """
-        Switches the status to inactive.
+        Sets the subject to work with.
+
+        :param value:
+            The subject to set.
         """
 
-        self.status.status_after_extra_rules = PyFunceble.storage.STATUS.down
-        self.status.status_source_after_extra_rules = "SPECIAL"
+        self.idna_subject = value
 
         return self
 
-    def __switch_to_down_if(self, status_code: int) -> "ExtraRulesHandler":
+    @property
+    def do_syntax_check_first(self) -> None:
         """
-        Switches the status to inactive if the status code is matching the
-        given one.
+        Provides the current state of the :code:`do_syntax_check_first`
+        attribute.
         """
 
-        if self.status.http_status_code == status_code:
-            self.__switch_to_down()
+        return self._do_syntax_check_first
 
-        return self
-
-    def __switch_to_up(self) -> "ExtraRulesHandler":
+    @do_syntax_check_first.setter
+    def do_syntax_check_first(self, value: bool) -> None:
         """
-        Switches the status to active.
+        Sets the value which allow us to do a syntax check first.
+
+        :param value:
+            The subject to set.
+
+        :raise TypeError:
+            When the given :code:`value` is not a :py:class:`bool`.
         """
 
-        self.status.status_after_extra_rules = PyFunceble.storage.STATUS.up
-        self.status.status_source_after_extra_rules = "SPECIAL"
+        if not isinstance(value, bool):
+            raise TypeError(f"<value> should be {str}, {type(value)} given.")
 
-    def __handle_blogspot(self) -> "ExtraRulesHandler":
+        self._do_syntax_check_first = self.params.do_syntax_check_first = value
+
+    def set_do_syntax_check_first(self, value: bool) -> "CheckerBase":
         """
-        Handles the :code:`blogspot.*` case.
+        Sets the value which allow us to do a syntax check first.
 
-        .. warning::
-            This method assume that we know that we are handling a blogspot domain.
+        :param value:
+            The subject to set.
         """
 
-        regex_blogger = [r"create-blog.g?", r"87065", r"doesn&#8217;t&nbsp;exist"]
+        self.do_syntax_check_first = value
 
-        if self.status.subject.startswith("http:"):
-            url = self.status.subject
-        else:
-            url = f"http://{self.status.subject}:80"
+        return self
 
-        self.__web_regex_handler(url, regex_blogger, self.__switch_to_down)
+    @property
+    def use_collection(self) -> bool:
+        """
+        Provides the current value of the :code:`_use_collection` attribute.
+        """
 
-        return self
+        return self._use_collection
 
-    def __handle_wordpress_dot_com(self) -> "ExtraRulesHandler":
+    @use_collection.setter
+    def use_collection(self, value: bool) -> None:
         """
-        Handles the :code:`wordpress.com` case.
+        Sets the value which authorizes the usage of the Collection.
 
-        .. warning::
-            This method assume that we know that we are handling a blogspot domain.
+        :param value:
+            The value to set.
+
+        :param TypeError:
+            When the given :code:`value` is not a :py:class:`bool`.
         """
 
-        regex_wordpress = [r"doesn&#8217;t&nbsp;exist"]
+        if not isinstance(value, bool):
+            raise TypeError(f"<value> should be {bool}, {type(value)} given.")
 
-        if self.status.subject.startswith("http:"):
-            url = self.status.subject
-        else:
-            url = f"http://{self.status.subject}:80"
+        self._use_collection = self.params.use_collection = value
+
+    def set_use_collection(self, value: bool) -> "CheckerBase":
+        """
+        Sets the value which authorizes the usage of the Collection.
+
+        :param value:
+            The value to set.
+        """
 
-        self.__web_regex_handler(url, regex_wordpress, self.__switch_to_down)
+        self.use_collection = value
 
         return self
 
-    def __handle_fc2_dot_com(self) -> "ExtraRulesHandler":
+    def guess_and_set_use_collection(self) -> "CheckerBase":
+        """
+        Try to guess and set the value of the :code:`use_collection` attribute.
+        """
+
+        if PyFunceble.facility.ConfigLoader.is_already_loaded():
+            if isinstance(PyFunceble.storage.CONFIGURATION.lookup.collection, bool):
+                self.use_collection = PyFunceble.storage.CONFIGURATION.lookup.collection
+            else:
+                self.use_collection = self.STD_USE_COLLECTION
+        else:
+            self.use_collection = self.STD_USE_COLLECTION
+
+    def subject_propagator(self) -> "CheckerBase":
         """
-        Handles the :code:`fc2.com` case.
+        Propagate the currently set subject.
 
         .. warning::
-            This method assume that we know that we are handling a fc2 domain.
+            Be sure to use setup your status first.
         """
 
-        if self.status.subject.startswith("http:"):
-            url = self.status.subject
-        else:
-            url = f"http://{self.status.subject}:80"
+        self.status.subject = self.subject
+        self.status.idna_subject = self.idna_subject
+        self.status.netloc = self.url2netloc.set_data_to_convert(
+            self.idna_subject
+        ).get_converted()
+        self.status.status = None
+
+        return self.query_common_checker()
+
+    def query_common_checker(self) -> "CheckerBase":
+        """
+        Queries the common checkers.
 
-        req = PyFunceble.factory.Requester.get(url, allow_redirects=False)
+        .. warning::
+            Be sure to use setup your status first.
+        """
 
-        if "Location" in req.headers and "error.fc2.com" in req.headers["Location"]:
-            self.__switch_to_down()
+        if not self.status.subject_kind:
+            cls_name = self.__class__.__name__.lower()
+            if (
+                hasattr(self.status, "ip_syntax") and self.status.ip_syntax
+            ) or "ip" in cls_name:
+                self.status.subject_kind = "ip"
+            elif (
+                hasattr(self.status, "url_syntax") and self.status.url_syntax
+            ) or "url" in cls_name:
+                self.status.subject_kind = "url"
+            elif (
+                hasattr(self.status, "domain_syntax") and self.status.domain_syntax
+            ) or "domain" in cls_name:
+                self.status.subject_kind = "domain"
+            else:
+                self.status.subject_kind = "unknown"
 
         return self
 
-    def __handle_active2inactive(self) -> "ExtraRulesHandler":
+    @ensure_subject_is_given
+    def is_valid(self) -> bool:
         """
-        Handles the status deescalation.
+        Provides the result of the validation.
         """
 
-        if self.status.http_status_code:
-            self.__regex_registry_handler(self.regex_active2inactive)
+        raise NotImplementedError()
 
-        return self
+    @ensure_subject_is_given
+    @update_status_date_after_query
+    def query_status(self) -> "CheckerBase":
+        """
+        Queries the status.
+        """
 
-    @ensure_status_is_given
-    def start(self) -> "ExtraRulesHandler":
+        raise NotImplementedError()
+
+    @query_status_if_missing
+    def get_status(self) -> Optional[CheckerStatusBase]:
         """
-        Starts the process.
+        Provides the current state of the status.
+
+        .. note::
+            This method will automatically query status using the
+            :meth:`PyFunceble.checker.base.CheckerBase.query_status` if
+            the
+            :attr:`PyFunceble.checker.status_base.CheckerStatusBase.status`
+            attribute is not set.
         """
 
-        PyFunceble.facility.Logger.info(
-            "Started to check %r against our own set of rules.",
-            self.status.idna_subject,
-        )
-
-        self.status.status_before_extra_rules = self.status.status
-        self.status.status_source_before_extra_rules = self.status.status_source
-
-        if self.status.status_before_extra_rules == PyFunceble.storage.STATUS.up:
-            self.__handle_active2inactive()
-
-        if (
-            not self.status.status_after_extra_rules
-            and self.status.status_before_extra_rules in PyFunceble.storage.STATUS.down
-        ):
-            if self.status.ipv4_range_syntax or self.status.ipv6_range_syntax:
-                self.__switch_to_up()
-
-        if self.status.status_after_extra_rules:
-            self.status.status = self.status.status_after_extra_rules
-            self.status.status_source = self.status.status_source_after_extra_rules
-
-            PyFunceble.facility.Logger.info(
-                "Could define the status of %r from our own set of rules.",
-                self.status.idna_subject,
-            )
-        else:
-            self.status.status_before_extra_rules = None
-            self.status.status_source_before_extra_rules = None
-            self.status.status_after_extra_rules = None
-            self.status.status_source_after_extra_rules = None
-
-        PyFunceble.facility.Logger.info(
-            "Finished to check %r against our own set of rules.",
-            self.status.idna_subject,
-        )
+        return self.status
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/availability/ip.py` & `PyFunceble-4.2.0/PyFunceble/checker/availability/ip.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -166,14 +166,14 @@
             PyFunceble.facility.Logger.info(
                 "Could not define status the status of %r. Setting to %r",
                 self.status.idna_subject,
                 self.status.status,
             )
 
         if self.use_extra_rules:
-            self.extra_rules_handler.set_status(self.status).start()
+            self.try_to_query_status_from_extra_rules()
 
         return self
 
     @staticmethod
     def is_valid() -> bool:  # pylint: disable=arguments-differ
         raise NotImplementedError()
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/availability/params.py` & `PyFunceble-4.2.0/PyFunceble/checker/availability/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/availability/status.py` & `PyFunceble-4.2.0/PyFunceble/checker/availability/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/availability/url.py` & `PyFunceble-4.2.0/PyFunceble/checker/availability/url.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -115,17 +115,21 @@
         self.status = AvailabilityCheckerStatus()
         self.status.params = self.params
         self.status.dns_lookup_record = self.dns_query_tool.lookup_record
         self.status.whois_lookup_record = None
 
         self.status.subject = self.subject
         self.status.idna_subject = self.idna_subject
+        self.status.netloc = self.url2netloc.set_data_to_convert(
+            self.idna_subject
+        ).get_converted()
+
         self.status.status = None
 
-        self.query_syntax_checker()
+        self.query_common_checker()
 
         return self
 
     def try_to_query_status_from_http_status_code(self) -> "URLAvailabilityChecker":
         """
         Tries to query the status from the network information.
         """
@@ -269,12 +273,15 @@
 
             PyFunceble.facility.Logger.info(
                 "Could not define status the status of %r. Setting to %r",
                 self.status.idna_subject,
                 self.status.status,
             )
 
+        if self.use_extra_rules:
+            self.try_to_query_status_from_extra_rules()
+
         return self
 
     @staticmethod
     def is_valid() -> bool:  # pylint: disable=arguments-differ
         raise NotImplementedError()
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/base.py` & `PyFunceble-4.2.0/PyFunceble/database/credential/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the base of all checker.
+Provides the base of all our credential holders.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,381 +31,410 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-import datetime
 import functools
-from typing import Optional
+import os
+from typing import List, Optional
 
-import domain2idna
-from sqlalchemy.orm import Session
-
-import PyFunceble.facility
 import PyFunceble.storage
-from PyFunceble.checker.params_base import CheckerParamsBase
-from PyFunceble.checker.status_base import CheckerStatusBase
-from PyFunceble.query.collection import CollectionQueryTool
+from PyFunceble.helpers.file import FileHelper
 
 
-class CheckerBase:
+class CredentialBase:
     """
-    Provides the base of all checker.
-
-    :param str subject:
-        Optional, The subject to work with.
-    :param bool do_syntax_check_first:
-        Optional, Forces the checker to first perform a syntax check,
-
-        .. warning::
-            This does not apply to the syntax checker - itself.
+    Provides the base of all our credential holder.
     """
 
-    STD_DO_SYNTAX_CHECK_FIRST: bool = False
-    STD_USE_COLLECTION: bool = False
+    STD_HOST: str = "localhost"
+    STD_PORT: int = 3306
+    STD_NAME: str = PyFunceble.storage.PROJECT_NAME.lower()
+    STD_USERNAME: str = PyFunceble.storage.PROJECT_NAME.lower()
+    STD_PASSWORD: str = f"{PyFunceble.storage.PROJECT_NAME}:15_93le"
+    STD_CHARSET: str = "utf8mb4"
+
+    VAR2ENV: dict = {
+        "host": "PYFUNCEBLE_DB_HOST",
+        "port": "PYFUNCEBLE_DB_PORT",
+        "name": "PYFUNCEBLE_DB_NAME",
+        "username": "PYFUNCEBLE_DB_USERNAME",
+        "password": "PYFUNCEBLE_DB_PASSWORD",
+        "charset": "PYFUNCEBLE_DB_CHARSET",
+    }
+    """
+    Maps our credential variable with environment variable.
+    """
 
-    _do_syntax_check_first: bool = False
-    _use_collection: bool = False
+    dotenv_locations: List[str] = []
+    """
+    Provides the location of the dotenv to work with.
 
-    _subject: Optional[str] = None
-    _idna_subject: Optional[str] = None
+    .. warning::
+        The order is important. The last one in the list will be taken as
+        default if everything else is not found in the filesystem.
+    """
 
-    db_session: Optional[Session] = None
-    collection_query_tool: Optional[CollectionQueryTool] = None
+    protocol: Optional[str] = None
 
-    status: Optional[CheckerStatusBase] = None
-    params: Optional[CheckerParamsBase] = None
+    _host: Optional[str] = None
+    _port: Optional[int] = None
+    _name: Optional[str] = None
+    _username: Optional[str] = None
+    _password: Optional[str] = None
+    _charset: Optional[str] = None
 
     def __init__(
         self,
-        subject: Optional[str] = None,
         *,
-        do_syntax_check_first: Optional[bool] = None,
-        db_session: Optional[Session] = None,
-        use_collection: Optional[bool] = None,
+        host: Optional[str] = None,
+        port: Optional[int] = None,
+        name: Optional[str] = None,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+        charset: Optional[str] = None,
     ) -> None:
-        self.collection_query_tool = CollectionQueryTool()
+        if host is not None:
+            self.host = host
+        else:
+            self.host = self.STD_HOST
 
-        if self.params is None:
-            self.params = CheckerParamsBase()
+        if port is not None:
+            self.port = port
+        else:
+            self.port = self.STD_PORT
 
-        if self.status is None:
-            self.status = CheckerStatusBase()
+        if name is not None:
+            self.name = name
+        else:
+            self.name = self.STD_NAME
 
-        if subject is not None:
-            self.subject = subject
+        if username is not None:
+            self.username = username
+        else:
+            self.username = self.STD_USERNAME
 
-        if do_syntax_check_first is not None:
-            self.do_syntax_check_first = do_syntax_check_first
+        if password is not None:
+            self.password = password
         else:
-            self.do_syntax_check_first = self.STD_DO_SYNTAX_CHECK_FIRST
+            self.password = self.STD_PASSWORD
 
-        if use_collection is not None:
-            self.use_collection = use_collection
+        if charset is not None:
+            self.charset = charset
         else:
-            self.guess_and_set_use_collection()
+            self.charset = self.STD_CHARSET
 
-        self.db_session = db_session
+        self.dotenv_locations = [
+            os.path.realpath(PyFunceble.storage.ENV_FILENAME),
+            os.path.join(
+                PyFunceble.storage.CONFIG_DIRECTORY, PyFunceble.storage.ENV_FILENAME
+            ),
+        ]
 
-    def propagate_subject(func):  # pylint: disable=no-self-argument
+    def ensure_protocol_is_given(func):  # pylint: disable=no-self-argument
         """
-        Propagates the subject to the object that need it after launching
-        the decorated method.
+        Ensures that the protocol is given before launching the decorated
+        method.
+
+        :raise ValueError:
+            When the :code:`protocol` is not given.
         """
 
         @functools.wraps(func)
         def wrapper(self, *args, **kwargs):
-            result = func(self, *args, **kwargs)  # pylint: disable=not-callable
-
-            self.subject_propagator()
+            if not self.protocol:
+                raise ValueError("<self.protocol> is not given.")
 
-            return result
+            return func(self, *args, **kwargs)  # pylint: disable=not-callable
 
         return wrapper
 
-    def ensure_subject_is_given(func):  # pylint: disable=no-self-argument
+    @property
+    def host(self) -> Optional[str]:
+        """
+        Provides the current state of the :code:`_host` attribute.
         """
-        Ensures that the subject is given before running the decorated method.
+
+        return self._host
+
+    @host.setter
+    def host(self, value: str) -> None:
+        """
+        Sets the hosts to interact with.
+
+        :param value:
+            The value to set.
 
         :raise TypeError:
-            If the subject is not a string.
+            When the given :code:`value` is not a :py:class:`str`.
+        :raise ValueError:
+            When the given :code:`value` is empty.
         """
 
-        @functools.wraps(func)
-        def wrapper(self, *args, **kwargs):  # pragma: no cover ## Safety!
-            if not isinstance(self.subject, str):
-                raise TypeError(
-                    f"<self.subject> should be {str}, {type(self.subject)} given."
-                )
+        if not isinstance(value, str):
+            raise TypeError(f"<value> should be {str}, {type(value)} given.")
 
-            return func(self, *args, **kwargs)  # pylint: disable=not-callable
+        if not value:
+            raise ValueError("<value> should not be empty.")
 
-        return wrapper
+        self._host = value
 
-    def query_status_if_missing(func):  # pylint: disable=no-self-argument
+    def set_host(self, value: str) -> "CredentialBase":
         """
-        Queries the status if it's missing.
+        Sets the hosts to interact with.
+
+        :param value:
+            The value to set.
         """
 
-        @functools.wraps(func)
-        def wrapper(self, *args, **kwargs):  # pragma: no cover ## Safety!
-            if not self.status.status or self.status.status is None:
-                self.query_status()
+        self.host = value
 
-            return func(self, *args, **kwargs)  # pylint: disable=not-callable
+        return self
 
-        return wrapper
+    @property
+    def port(self) -> Optional[int]:
+        """
+        Provides the current state of the :code:`_port` attribute.
+        """
 
-    def update_status_date_after_query(func):  # pylint: disable=no-self-argument
+        return self._port
+
+    @port.setter
+    def port(self, value: int) -> None:
         """
-        Updates the status dates after running the decorated method.
+        Sets the port to interact with.
+
+        :param value:
+            The value to set.
+
+        :raise TypeError:
+            When the given :code:`value` is not a :py:class:`int`.
         """
 
-        @functools.wraps(func)
-        def wrapper(self, *args, **kwargs):  # pragma: no cover ## Safety!
-            result = func(self, *args, **kwargs)  # pylint: disable=not-callable
+        if not isinstance(value, int):
+            raise TypeError(f"<value> should be {int}, {type(value)} given.")
+
+        self._port = value
 
-            self.status.tested_at = datetime.datetime.utcnow()
+    def set_port(self, value: int) -> "CredentialBase":
+        """
+        Sets the port to interact with.
 
-            return result
+        :param value:
+            The value to set.
+        """
 
-        return wrapper
+        self.port = value
+
+        return self
 
     @property
-    def subject(self) -> Optional[str]:
+    def name(self) -> Optional[str]:
         """
-        Provides the current state of the :code:`_subject` attribute.
+        Provides the current state of the :code:`_name` attribute.
         """
 
-        return self._subject
+        return self._name
 
-    @subject.setter
-    @propagate_subject
-    def subject(self, value: str) -> None:
+    @name.setter
+    def name(self, value: str) -> None:
         """
-        Sets the subject to work with.
+        Sets the name of the database to interact with.
 
         :param value:
-            The subject to set.
+            The value to set.
 
         :raise TypeError:
             When the given :code:`value` is not a :py:class:`str`.
         :raise ValueError:
             When the given :code:`value` is empty.
         """
 
         if not isinstance(value, str):
             raise TypeError(f"<value> should be {str}, {type(value)} given.")
 
         if not value:
             raise ValueError("<value> should not be empty.")
 
-        self._subject = value
-
-        try:
-            self.idna_subject = domain2idna.domain2idna(value)
-        except ValueError:
-            self.idna_subject = value
+        self._name = value
 
-    def set_subject(self, value: str) -> "CheckerBase":
+    def set_name(self, value: str) -> "CredentialBase":
         """
-        Sets the subject to work with.
+        Sets the name of the database to interact with.
 
         :param value:
-            The subject to set.
+            The value to set.
         """
 
-        self.subject = value
+        self.name = value
 
         return self
 
     @property
-    def idna_subject(self) -> Optional[str]:
+    def username(self) -> Optional[str]:
         """
-        Provides the current state of the :code:`_idna_subject` attribute.
+        Provides the current state of the :code:`_username` attribute.
         """
 
-        return self._idna_subject
+        return self._username
 
-    @idna_subject.setter
-    def idna_subject(self, value: str) -> None:
+    @username.setter
+    def username(self, value: str) -> None:
         """
-        Sets the subject to work with.
+        Sets the username to use to authenticate ourselves.
 
         :param value:
-            The subject to set.
+            The value to set.
 
         :raise TypeError:
             When the given :code:`value` is not a :py:class:`str`.
         :raise ValueError:
             When the given :code:`value` is empty.
         """
 
         if not isinstance(value, str):
             raise TypeError(f"<value> should be {str}, {type(value)} given.")
 
         if not value:
             raise ValueError("<value> should not be empty.")
 
-        self._idna_subject = value
+        self._username = value
 
-    def set_idna_subject(self, value: str) -> "CheckerBase":
+    def set_username(self, value: str) -> "CredentialBase":
         """
-        Sets the subject to work with.
+        Sets the username to use to authenticate ourselves.
 
         :param value:
-            The subject to set.
+            The value to set.
         """
 
-        self.idna_subject = value
+        self.username = value
 
         return self
 
     @property
-    def do_syntax_check_first(self) -> None:
+    def password(self) -> Optional[str]:
         """
-        Provides the current state of the :code:`do_syntax_check_first`
-        attribute.
+        Provides the current state of the :code:`_password` attribute.
         """
 
-        return self._do_syntax_check_first
+        return self._password
 
-    @do_syntax_check_first.setter
-    def do_syntax_check_first(self, value: bool) -> None:
+    @password.setter
+    def password(self, value: str) -> None:
         """
-        Sets the value which allow us to do a syntax check first.
+        Sets the password to use to authenticate ourselves.
 
         :param value:
-            The subject to set.
+            The value to set.
 
         :raise TypeError:
-            When the given :code:`value` is not a :py:class:`bool`.
+            When the given :code:`value` is not a :py:class:`str`.
         """
 
-        if not isinstance(value, bool):
+        if not isinstance(value, str):
             raise TypeError(f"<value> should be {str}, {type(value)} given.")
 
-        self._do_syntax_check_first = self.params.do_syntax_check_first = value
+        self._password = value
 
-    def set_do_syntax_check_first(self, value: bool) -> "CheckerBase":
+    def set_password(self, value: str) -> "CredentialBase":
         """
-        Sets the value which allow us to do a syntax check first.
+        Sets the password to use to authenticate ourselves.
 
         :param value:
-            The subject to set.
+            The value to set.
         """
 
-        self.do_syntax_check_first = value
+        self.host = value
 
         return self
 
     @property
-    def use_collection(self) -> bool:
+    def charset(self) -> Optional[str]:
         """
-        Provides the current value of the :code:`_use_collection` attribute.
+        Provides the current state of the :code:`_charset` attribute.
         """
 
-        return self._use_collection
+        return self._charset
 
-    @use_collection.setter
-    def use_collection(self, value: bool) -> None:
+    @charset.setter
+    def charset(self, value: str) -> None:
         """
-        Sets the value which authorizes the usage of the Collection.
+        Sets the charset to use.
 
         :param value:
             The value to set.
 
-        :param TypeError:
-            When the given :code:`value` is not a :py:class:`bool`.
+        :raise TypeError:
+            When the given :code:`value` is not a :py:class:`str`.
+        :raise ValueError:
+            When the given :code:`value` is empty.
         """
 
-        if not isinstance(value, bool):
-            raise TypeError(f"<value> should be {bool}, {type(value)} given.")
+        if not isinstance(value, str):
+            raise TypeError(f"<value> should be {str}, {type(value)} given.")
 
-        self._use_collection = self.params.use_collection = value
+        if not value:
+            raise ValueError("<value> should not be empty.")
+
+        self._charset = value
 
-    def set_use_collection(self, value: bool) -> "CheckerBase":
+    def set_charset(self, value: str) -> "CredentialBase":
         """
-        Sets the value which authorizes the usage of the Collection.
+        Sets the charset to use.
 
         :param value:
             The value to set.
         """
 
-        self.use_collection = value
+        self.charset = value
 
         return self
 
-    def guess_and_set_use_collection(self) -> "CheckerBase":
-        """
-        Try to guess and set the value of the :code:`use_collection` attribute.
-        """
-
-        if PyFunceble.facility.ConfigLoader.is_already_loaded():
-            if isinstance(PyFunceble.storage.CONFIGURATION.lookup.collection, bool):
-                self.use_collection = PyFunceble.storage.CONFIGURATION.lookup.collection
-            else:
-                self.use_collection = self.STD_USE_COLLECTION
-        else:
-            self.use_collection = self.STD_USE_COLLECTION
-
-    def subject_propagator(self) -> "CheckerBase":
+    @ensure_protocol_is_given
+    def get_uri(self) -> str:
         """
-        Propagate the currently set subject.
-
-        .. warning::
-            You are not invited to run this method directly.
-
-            Only the :code:`propagate_subject` decorator should call this
-            method.
+        Provides the SQLAlchemy URI.
         """
 
-        return self
+        if self.host.startswith("/"):
+            return (
+                f"{self.protocol}://{self.username}:{self.password}"
+                f"@localhost/{self.name}?unix_socket={self.host}"
+                f"&charset={self.charset}"
+            )
 
-    @ensure_subject_is_given
-    def is_valid(self) -> bool:
-        """
-        Provides the result of the validation.
-        """
-
-        raise NotImplementedError()
+        return (
+            f"{self.protocol}://{self.username}:{self.password}"
+            f"@{self.host}/{self.name}"
+            f"?charset={self.charset}"
+        )
 
-    @ensure_subject_is_given
-    @update_status_date_after_query
-    def query_status(self) -> "CheckerBase":
+    def get_dot_env_file(self) -> str:
         """
-        Queries the status.
+        Provides the dotenv file to work with.
         """
 
-        raise NotImplementedError()
+        file_helper = FileHelper()
 
-    @query_status_if_missing
-    def get_status(self) -> Optional[CheckerStatusBase]:
-        """
-        Provides the current state of the status.
-
-        .. note::
-            This method will automatically query status using the
-            :meth:`PyFunceble.checker.base.CheckerBase.query_status` if
-            the
-            :attr:`PyFunceble.checker.status_base.CheckerStatusBase.status`
-            attribute is not set.
-        """
+        for file in self.dotenv_locations:
+            if file_helper.set_path(file).exists():
+                return file_helper.path
 
-        return self.status
+        return self.dotenv_locations[-1]
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/complex_json_encoder.py` & `PyFunceble-4.2.0/PyFunceble/checker/complex_json_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/params_base.py` & `PyFunceble-4.2.0/PyFunceble/checker/params_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/reputation/__init__.py` & `PyFunceble-4.2.0/PyFunceble/checker/reputation/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/reputation/base.py` & `PyFunceble-4.2.0/PyFunceble/checker/reputation/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -132,52 +132,47 @@
         self.ip_syntax_checker.subject = self.idna_subject
         self.url_syntax_checker.subject = self.idna_subject
 
         self.status = ReputationCheckerStatus()
         self.status.params = self.params
         self.status.dns_lookup_record = self.dns_query_tool.lookup_record
 
-        self.status.subject = self.subject
-        self.status.idna_subject = self.idna_subject
-
-        self.query_syntax_checker()
-
-        return self
+        return super().subject_propagator()
 
     def should_we_continue_test(self, status_post_syntax_checker: str) -> bool:
         """
         Checks if we are allowed to continue a standard testing.
         """
 
         return bool(
             not self.status.status
             or status_post_syntax_checker == PyFunceble.storage.STATUS.invalid
         )
 
-    def query_syntax_checker(self) -> "ReputationCheckerBase":
+    def query_common_checker(self) -> "ReputationCheckerBase":
         """
-        Queries the syntax checker.
+        Queries the common checkers.
         """
 
         self.status.second_level_domain_syntax = (
             self.domain_syntax_checker.is_valid_second_level()
         )
         self.status.subdomain_syntax = self.domain_syntax_checker.is_valid_subdomain()
-        self.status.domain_syntax = bool(
-            self.status.subdomain_syntax or self.status.second_level_domain_syntax
+        self.status.domain_syntax = bool(self.status.subdomain_syntax) or bool(
+            self.status.second_level_domain_syntax
         )
 
         self.status.ipv4_syntax = self.ip_syntax_checker.is_valid_v4()
         self.status.ipv6_syntax = self.ip_syntax_checker.is_valid_v6()
         self.status.ipv4_range_syntax = self.ip_syntax_checker.is_valid_v4_range()
         self.status.ipv6_range_syntax = self.ip_syntax_checker.is_valid_v6_range()
         self.status.ip_syntax = bool(self.status.ipv4_syntax or self.status.ipv6_syntax)
         self.status.url_syntax = self.url_syntax_checker.is_valid()
 
-        return self
+        return super().query_common_checker()
 
     def query_a_record(self) -> Optional[List[str]]:
         """
         Queries all the A record.
         """
 
         raise NotImplementedError()
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/reputation/domain.py` & `PyFunceble-4.2.0/PyFunceble/checker/reputation/domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/reputation/domain_and_ip.py` & `PyFunceble-4.2.0/PyFunceble/checker/syntax/domain_and_ip.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the domains and IP reputation checker.
+Provides the domains and IP syntax checker.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,57 +31,62 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-from PyFunceble.checker.reputation.base import ReputationCheckerBase
-from PyFunceble.checker.reputation.domain import DomainReputationChecker
-from PyFunceble.checker.reputation.ip import IPReputationChecker
+from typing import Union
 
+from PyFunceble.checker.syntax.base import SyntaxCheckerBase
+from PyFunceble.checker.syntax.domain import DomainSyntaxChecker
+from PyFunceble.checker.syntax.ip import IPSyntaxChecker
 
-class DomainAndIPReputationChecker(ReputationCheckerBase):
+
+class DomainAndIPSyntaxChecker(SyntaxCheckerBase):
     """
-    Provides the interface for checking the reputation of an IP or domain.
+    Provides the interface for checking the syntax of an IP or domain.
 
     :param str subject:
         Optional, The subject to work with.
-    :param bool do_syntax_check_first:
-        Optional, Activates/Disables the check of the status before the actual
-        status gathering.
     """
 
-    @ReputationCheckerBase.ensure_subject_is_given
-    @ReputationCheckerBase.update_status_date_after_query
-    def query_status(self) -> "DomainAndIPReputationChecker":
+    @SyntaxCheckerBase.ensure_subject_is_given
+    @SyntaxCheckerBase.update_status_date_after_query
+    def query_status(
+        self,
+    ) -> "DomainAndIPSyntaxChecker":  # pragma: no cover ## Just a switch.
         """
         Queries the result without anything more.
         """
 
-        if self.status.ip_syntax:
-            query_object = IPReputationChecker()
+        query_object: Union[IPSyntaxChecker, DomainSyntaxChecker] = None
+
+        ip_checker = IPSyntaxChecker(self.subject)
+
+        if ip_checker.is_valid():
+            query_object = ip_checker
         else:
-            query_object = DomainReputationChecker()
+            query_object = DomainSyntaxChecker(self.subject, db_session=self.db_session)
 
-        query_object.__dict__ = self.__dict__
+        query_object.collection_query_tool = self.collection_query_tool
 
         result = query_object.query_status()
 
         self.__dict__.update(query_object.__dict__)
 
         return result
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/reputation/ip.py` & `PyFunceble-4.2.0/PyFunceble/checker/reputation/ip.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/reputation/params.py` & `PyFunceble-4.2.0/PyFunceble/checker/reputation/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/reputation/status.py` & `PyFunceble-4.2.0/PyFunceble/checker/reputation/status.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/reputation/url.py` & `PyFunceble-4.2.0/PyFunceble/checker/reputation/url.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -76,15 +76,14 @@
 
         if ip_syntax_checker.is_valid_v4():
             return [url_base]
 
         if ip_syntax_checker.is_valid_v6() or (
             url_base.startswith("[") and url_base.endswith("]")
         ):
-
             url_base = url_base.replace("[", "").replace("]", "")
 
             result = set()
 
             for subject in (
                 self.dns_query_tool.set_query_record_type("PTR")
                 .set_subject(url_base)
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/status_base.py` & `PyFunceble-4.2.0/PyFunceble/checker/status_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -61,16 +61,19 @@
 
 @dataclasses.dataclass
 class CheckerStatusBase:
     """
     Provides the base of all status classes.
     """
 
+    subject_kind: Optional[str] = None
+
     subject: Optional[str] = None
     idna_subject: Optional[str] = None
+    netloc: Optional[str] = None
 
     status: Optional[str] = None
     status_source: Optional[str] = None
 
     tested_at: Optional[datetime.datetime] = None
 
     params: Optional[CheckerParamsBase] = None
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/syntax/__init__.py` & `PyFunceble-4.2.0/PyFunceble/checker/syntax/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/syntax/base.py` & `PyFunceble-4.2.0/PyFunceble/checker/syntax/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -92,18 +92,15 @@
 
         .. warning::
             You are not invited to run this method directly.
         """
 
         self.status = SyntaxCheckerStatus()
 
-        self.status.subject = self.subject
-        self.status.idna_subject = self.idna_subject
-
-        return self
+        return super().subject_propagator()
 
     @CheckerBase.ensure_subject_is_given
     @CheckerBase.update_status_date_after_query
     def query_status(self) -> "SyntaxCheckerBase":
         """
         Queries the status.
         """
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/syntax/domain.py` & `PyFunceble-4.2.0/PyFunceble/checker/syntax/domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -91,19 +91,17 @@
             You are not invited to run this method directly.
         """
 
         self.second_level_checker.subject = self.idna_subject
         self.subdomain_checker.subject = self.idna_subject
 
         self.status = SyntaxCheckerStatus()
+        self.status.subject_kind = "domain"
 
-        self.status.subject = self.subject
-        self.status.idna_subject = self.idna_subject
-
-        return self
+        return super().subject_propagator()
 
     @DomainSyntaxCheckerBase.ensure_subject_is_given
     def is_valid(self) -> bool:
         """
         Validate the given subject if exists.
         """
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/syntax/domain_base.py` & `PyFunceble-4.2.0/PyFunceble/checker/syntax/domain_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/syntax/ip.py` & `PyFunceble-4.2.0/PyFunceble/checker/syntax/ip.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -84,19 +84,17 @@
             You are not invited to run this method directly.
         """
 
         self.ipv4_checker.subject = self.idna_subject
         self.ipv6_checker.subject = self.idna_subject
 
         self.status = SyntaxCheckerStatus()
+        self.status.subject_kind = "ip"
 
-        self.status.subject = self.subject
-        self.status.idna_subject = self.idna_subject
-
-        return self
+        return super().subject_propagator()
 
     @CheckerBase.ensure_subject_is_given
     def is_valid(self) -> bool:
         """
         Validate the given subject.
         """
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/syntax/ipv4.py` & `PyFunceble-4.2.0/PyFunceble/checker/syntax/ipv4.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/syntax/ipv6.py` & `PyFunceble-4.2.0/PyFunceble/checker/syntax/ipv6.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/syntax/params.py` & `PyFunceble-4.2.0/PyFunceble/checker/syntax/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/syntax/second_lvl_domain.py` & `PyFunceble-4.2.0/PyFunceble/checker/syntax/second_lvl_domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/syntax/status.py` & `PyFunceble-4.2.0/PyFunceble/checker/syntax/status.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/syntax/subdomain.py` & `PyFunceble-4.2.0/PyFunceble/checker/syntax/subdomain.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/syntax/url.py` & `PyFunceble-4.2.0/PyFunceble/checker/syntax/url.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -64,14 +64,19 @@
     """
     Provides an interface to check the syntax of a URL.
 
     :param str subject:
         Optional, The subject to work with.
     """
 
+    def subject_propagator(self) -> CheckerBase:
+        self.status.subject_kind = "url"
+
+        return super().subject_propagator()
+
     @staticmethod
     def get_hostname_from_url(url: str) -> Optional[str]:
         """
         Extract the hostname part of the given URL.
 
         .. versionadded:: 4.1.0b7
         """
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/utils/__init__.py` & `PyFunceble-4.2.0/PyFunceble/converter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides some utilities related to the checkers.
+Provides all the converters.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/checker/utils/whois.py` & `PyFunceble-4.2.0/PyFunceble/checker/utils/whois.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -56,16 +56,15 @@
 
 import PyFunceble.facility
 import PyFunceble.storage
 from PyFunceble.dataset.base import DatasetBase
 from PyFunceble.dataset.csv_base import CSVDatasetBase
 from PyFunceble.dataset.db_base import DBDatasetBase
 from PyFunceble.dataset.whois.csv import CSVWhoisDataset
-from PyFunceble.dataset.whois.mariadb import MariaDBWhoisDataset
-from PyFunceble.dataset.whois.mysql import MySQLWhoisDataset
+from PyFunceble.dataset.whois.sql import SQLDBWhoisDataset
 
 
 def get_whois_dataset_object(
     *, db_session: Optional[Session] = None
 ) -> Union[DatasetBase, CSVDatasetBase, DBDatasetBase]:
     """
     Provides the whois dataset object to work with.
@@ -80,18 +79,20 @@
     """
 
     if PyFunceble.facility.ConfigLoader.is_already_loaded():
         result = None
 
         if PyFunceble.storage.CONFIGURATION.cli_testing.db_type == "csv":
             result = CSVWhoisDataset()
-        elif PyFunceble.storage.CONFIGURATION.cli_testing.db_type == "mariadb":
-            result = MariaDBWhoisDataset(db_session=db_session)
-        elif PyFunceble.storage.CONFIGURATION.cli_testing.db_type == "mysql":
-            result = MySQLWhoisDataset(db_session=db_session)
+        elif PyFunceble.storage.CONFIGURATION.cli_testing.db_type in (
+            "mariadb",
+            "mysql",
+            "postgresql",
+        ):
+            result = SQLDBWhoisDataset(db_session=db_session)
 
         if result:
             result.set_authorized(
                 bool(PyFunceble.storage.CONFIGURATION.cli_testing.whois_db)
             )
 
             return result
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/__init__.py` & `PyFunceble-4.2.0/PyFunceble/cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/continuous_integration/__init__.py` & `PyFunceble-4.2.0/PyFunceble/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
+# pylint: disable=invalid-name
 """
 The tool to check the availability or syntax of domain, IP or URL.
 
 ::
 
 
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides everything we may need for continuous integration aka autosaving and
-auto commiting.
+Provides some global utilities.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -32,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/continuous_integration/base.py` & `PyFunceble-4.2.0/PyFunceble/cli/continuous_integration/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/continuous_integration/exceptions.py` & `PyFunceble-4.2.0/PyFunceble/cli/continuous_integration/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/continuous_integration/github_actions.py` & `PyFunceble-4.2.0/PyFunceble/cli/continuous_integration/github_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/continuous_integration/gitlab_ci.py` & `PyFunceble-4.2.0/PyFunceble/cli/continuous_integration/gitlab_ci.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/continuous_integration/jenkins.py` & `PyFunceble-4.2.0/PyFunceble/cli/continuous_integration/jenkins.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/continuous_integration/travis_ci.py` & `PyFunceble-4.2.0/PyFunceble/cli/continuous_integration/travis_ci.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/continuous_integration/utils.py` & `PyFunceble-4.2.0/PyFunceble/cli/continuous_integration/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/credential_loader.py` & `PyFunceble-4.2.0/PyFunceble/cli/credential_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -56,14 +56,15 @@
 
 import PyFunceble.cli.factory
 import PyFunceble.facility
 import PyFunceble.storage
 from PyFunceble.database.credential.base import CredentialBase
 from PyFunceble.database.credential.mariadb import MariaDBCredential
 from PyFunceble.database.credential.mysql import MySQLCredential
+from PyFunceble.database.credential.postgresql import PostgreSQLCredential
 from PyFunceble.helpers.environment_variable import EnvironmentVariableHelper
 
 
 class CredentialLoader:
     """
     Provides our creadential loader.
 
@@ -75,14 +76,15 @@
         The database type to load the credential for.
     """
 
     DB_TYPE2OBJ: dict = {
         "csv": None,
         "mysql": MySQLCredential,
         "mariadb": MariaDBCredential,
+        "postgresql": PostgreSQLCredential,
     }
 
     credential: Optional[CredentialBase] = None
     """
     The credential (itself).
     """
 
@@ -257,15 +259,14 @@
         Starts the loading of the credential.
 
         :param ignore_cli:
             Ignore questions to end-user.
         """
 
         if not isinstance(self.credential, CredentialBase) and self.authorized:
-
             # We directly share the credential object into the DBSession object.
             # This will let us use the DBSession without having to think about
             # any other headache.
             self.credential = (
                 PyFunceble.cli.factory.DBSession.credential
             ) = self.DB_TYPE2OBJ[self.db_type]()
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/entry_points/__init__.py` & `PyFunceble-4.2.0/PyFunceble/cli/entry_points/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/entry_points/clean.py` & `PyFunceble-4.2.0/PyFunceble/cli/entry_points/clean.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/entry_points/iana.py` & `PyFunceble-4.2.0/PyFunceble/cli/entry_points/iana.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/entry_points/production.py` & `PyFunceble-4.2.0/PyFunceble/cli/entry_points/production.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/entry_points/public_suffix.py` & `PyFunceble-4.2.0/PyFunceble/cli/entry_points/public_suffix.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/entry_points/pyfunceble/__init__.py` & `PyFunceble-4.2.0/PyFunceble/cli/entry_points/pyfunceble/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/entry_points/pyfunceble/argsparser.py` & `PyFunceble-4.2.0/PyFunceble/cli/entry_points/pyfunceble/argsparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -47,27 +47,27 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
 import argparse
-from typing import Optional, Sequence, Text
+from typing import Optional, Sequence
 
 # pylint: disable=raising-bad-type
 
 
 class OurArgumentParser(argparse.ArgumentParser):
     """
     Overwrites some behavior of the default argument parser.
     """
 
     def parse_args(
         self,
-        args: Optional[Sequence[Text]] = None,
+        args: Optional[Sequence[str]] = None,
         namespace: Optional[argparse.Namespace] = None,
     ) -> argparse.Namespace:
         namespace = super().parse_args(args, namespace)
 
         if namespace.lookup__timeout is not None and namespace.lookup__timeout < 0:
             raise self.error("--timeout must be a positive digit.")
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/entry_points/pyfunceble/cli.py` & `PyFunceble-4.2.0/PyFunceble/cli/entry_points/pyfunceble/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -714,18 +714,18 @@
         (
             [
                 "--database-type",
             ],
             {
                 "dest": "cli_testing.db_type",
                 "type": str,
-                "choices": ["csv", "mariadb", "mysql"],
+                "choices": ["csv", "mariadb", "mysql", "postgresql"],
                 "help": "Sets the database engine to use. "
                 "\nYou can choose between the following: "
-                "`csv | mariadb | mysql` %s"
+                "`csv | mariadb | mysql | postgresql` %s"
                 % get_configured_value("cli_testing.db_type"),
             },
         ),
         (
             [
                 "-dbr",
                 "--days-between-db-retest",
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/execution_time.py` & `PyFunceble-4.2.0/PyFunceble/cli/execution_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/facility.py` & `PyFunceble-4.2.0/PyFunceble/cli/facility.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/factory.py` & `PyFunceble-4.2.0/PyFunceble/checker/availability/extras/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides everything which doesn't get through the door of the facility.
+Provides everything related to the extras of the availablity checker.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,25 +31,21 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
-
-from PyFunceble.database.session import DBSession as db_session
-
-DBSession = db_session()
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/file_preloader.py` & `PyFunceble-4.2.0/PyFunceble/cli/file_preloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -447,15 +447,14 @@
                             rpz_policy2subject=self.rpz_policy2subject,
                             rpz_inputline2subject=self.rpz_inputline2subject,
                             inputline2subject=self.inputline2subject,
                             subject2complements=self.subject2complements,
                             url2netloc=self.url2netloc,
                             cidr2subject=self.cidr2subject,
                         ):
-
                             to_send = copy.deepcopy(self.protocol)
                             to_send["subject"] = subject
                             to_send["idna_subject"] = domain2idna(subject)
                             to_send["tested_at"] = datetime.utcnow() - timedelta(
                                 days=365.25 * 20
                             )
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/filesystem/__init__.py` & `PyFunceble-4.2.0/PyFunceble/cli/filesystem/printer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides everything related to our very own filesystem or output structure.
+Provides everything related to what we actually print (output) or to a file.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/filesystem/cleanup.py` & `PyFunceble-4.2.0/PyFunceble/cli/filesystem/cleanup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/filesystem/counter.py` & `PyFunceble-4.2.0/PyFunceble/cli/filesystem/counter.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -47,21 +47,22 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
 import copy
-from typing import Dict, List, Union
+from typing import Dict, List, Tuple, Union
 
 import PyFunceble.cli.storage
 import PyFunceble.cli.utils.testing
 import PyFunceble.storage
 from PyFunceble.checker.status_base import CheckerStatusBase
 from PyFunceble.cli.filesystem.json_base import FilesystemJSONBase
+from PyFunceble.helpers.list import ListHelper
 
 
 class FilesystemCounter(FilesystemJSONBase):
     """
     Provides our counter.
     """
 
@@ -101,14 +102,28 @@
             PyFunceble.storage.STATUS.invalid,
         ],
     }
 
     SOURCE_FILE: str = PyFunceble.cli.storage.COUNTER_FILE
 
     @FilesystemJSONBase.fetch_dataset_beforehand
+    def get_sorted_dataset(self) -> List[Tuple[str, float]]:
+        """
+        Provides the datasets in a sorted manner.
+        """
+
+        return (
+            ListHelper(
+                [(x, y) for x, y in self.dataset["percentage"].items() if x != "total"]
+            )
+            .custom_sort(key_method=lambda x: x[-1], reverse=True)
+            .subject
+        )
+
+    @FilesystemJSONBase.fetch_dataset_beforehand
     def get_dataset_for_printer(self) -> List[Dict[str, Union[str, int]]]:
         """
         Provides the dataset that the printer may understand.
 
         :raise ValueError:
             When the current testing mode is not supported (yet?).
         """
@@ -158,16 +173,20 @@
 
         if "counter" not in self.dataset:
             self.dataset = copy.deepcopy(self.STD_DATASET)
 
         self.dataset["counter"][status.status] += 1
         self.dataset["counter"]["total"] += 1
 
-        self.dataset["percentage"][status.status] = (
-            self.dataset["counter"][status.status] * 100
-        ) / self.dataset["counter"]["total"]
+        for key in self.dataset["percentage"]:
+            if key == "total":
+                continue
+
+            self.dataset["percentage"][key] = (
+                self.dataset["counter"][key] * 100
+            ) / self.dataset["counter"]["total"]
 
         self.dataset["percentage"]["total"] = sum(
             y for x, y in self.dataset["percentage"].items() if x != "total"
         )
 
         return self
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/filesystem/dir_base.py` & `PyFunceble-4.2.0/PyFunceble/cli/filesystem/dir_structure/backup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides a common base to the manipulation of the output directory.
+Provides an interface for the backup of the directory structure.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -47,91 +47,66 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
 import os
-from typing import Optional
 
-import PyFunceble.cli.storage
-from PyFunceble.database.session import DBSession
+import PyFunceble.facility
+from PyFunceble.cli.filesystem.dir_structure.base import DirectoryStructureBase
+from PyFunceble.helpers.dict import DictHelper
+from PyFunceble.helpers.directory import DirectoryHelper
+from PyFunceble.helpers.file import FileHelper
+from PyFunceble.helpers.hash import HashHelper
 
 
-class FilesystemDirBase:
+class DirectoryStructureBackup(DirectoryStructureBase):
     """
-    Provides a common base for the manipulation of our output directory.
+    Provides the base of all dir structure classes.
     """
 
-    _parent_dirname: Optional[str] = None
-    db_session: Optional[DBSession] = None
-
-    def __init__(
-        self,
-        parent_dirname: Optional[str] = None,
-        *,
-        db_session: Optional[DBSession] = None,
-    ) -> None:
-        if parent_dirname is not None:
-            self.parent_dirname = parent_dirname
-        else:
-            self.parent_dirname = PyFunceble.cli.storage.STD_PARENT_DIRNAME
-
-        self.db_session = db_session
-
-    @property
-    def parent_dirname(self) -> Optional[str]:
+    def get_backup_data(self) -> dict:
         """
-        Provides the current state of the :code:`_parent_dirname` attribute.
+        Provides the data which acts as a backup.
         """
 
-        return self._parent_dirname
+        result = {}
+        base_dir = self.get_output_basedir()
+        file_helper = FileHelper()
+        hash_helper = HashHelper()
 
-    @parent_dirname.setter
-    def parent_dirname(self, value: str) -> None:
-        """
-        Sets the parent dirname. The parent dirname is a directory which
-        acts a parent into the output directory.
+        for file in DirectoryHelper(base_dir).list_all_files():
+            file_helper.set_path(file)
+            reduced_path = self.get_path_without_base_dir(file)
 
-        :parm value:
-            The value to set.
+            directory, filename = reduced_path.rsplit(os.sep, 1)
+            file_hash = hash_helper.hash_file(file_helper.path)
 
-        :raise TypeError:
-            When the given :code:`value` is not a :py:class:`str`.
-        :raise ValueError:
-            When the given :code:`value` is empty.
-        """
+            dataset = {filename: {"content": file_helper.read(), "hash": file_hash}}
 
-        if not isinstance(value, str):
-            raise TypeError(f"<value> should be {str}, {type(value)} given.")
+            if directory not in result:
+                result[directory] = dataset
+            else:
+                result[directory].update(dataset)
 
-        if not value:
-            raise ValueError("<value> should not be empty.")
+        PyFunceble.facility.Logger.debug("Dir Structure to backup:\n%r", result)
 
-        self._parent_dirname = value
+        return result
 
-    def set_parent_dirname(self, value: str) -> "FilesystemDirBase":
+    def store_backup(self) -> "DirectoryStructureBackup":
         """
-        Sets the parent dirname. The parent dirname is a directory which
-        acts a parent into the output directory.
-
-        :parm value:
-            The value to set.
+        Stores the backup at the current destination.
         """
 
-        self.parent_dirname = value
+        DictHelper(self.get_backup_data()).to_json_file(self.source_file)
+
+        PyFunceble.facility.Logger.info("Stored backup into: %r", self.source_file)
 
         return self
 
-    def get_output_basedir(self) -> str:
+    def start(self) -> "DirectoryStructureBackup":
         """
-        Provides the output base directory.
-
-        :param create_if_missing:
-            Authorizes the creation of the directory if it's missing.
+        Starts the backup process.
         """
 
-        if self.parent_dirname:
-            return os.path.join(
-                PyFunceble.cli.storage.OUTPUT_DIRECTORY, self.parent_dirname
-            )
-        return PyFunceble.cli.storage.OUTPUT_DIRECTORY
+        return self.cleanup().store_backup()
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/filesystem/dir_structure/__init__.py` & `PyFunceble-4.2.0/PyFunceble/cli/filesystem/dir_structure/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/filesystem/dir_structure/backup.py` & `PyFunceble-4.2.0/PyFunceble/dataset/ipv4_reputation.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides an interface for the backup of the directory structure.
+Provides an interface which let us interact with the IPv4 reputation database.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -47,66 +47,59 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
 import os
+from typing import Any, Optional
 
-import PyFunceble.facility
-from PyFunceble.cli.filesystem.dir_structure.base import DirectoryStructureBase
-from PyFunceble.helpers.dict import DictHelper
-from PyFunceble.helpers.directory import DirectoryHelper
+import PyFunceble.storage
+from PyFunceble.dataset.base import DatasetBase
+from PyFunceble.downloader.ipv4_reputation import IPV4ReputationDownloader
 from PyFunceble.helpers.file import FileHelper
-from PyFunceble.helpers.hash import HashHelper
 
 
-class DirectoryStructureBackup(DirectoryStructureBase):
+class IPV4ReputationDataset(DatasetBase):
     """
-    Provides the base of all dir structure classes.
+    Provides the interface for the lookup of the IPv4 reputation.
     """
 
-    def get_backup_data(self) -> dict:
-        """
-        Provides the data which acts as a backup.
-        """
-
-        result = {}
-        base_dir = self.get_output_basedir()
-        file_helper = FileHelper()
-        hash_helper = HashHelper()
-
-        for file in DirectoryHelper(base_dir).list_all_files():
-            file_helper.set_path(file)
-            reduced_path = self.get_path_without_base_dir(file)
-
-            directory, filename = reduced_path.rsplit(os.sep, 1)
-            file_hash = hash_helper.hash_file(file_helper.path)
+    STORAGE_INDEX: Optional[str] = None
+    DOWNLOADER: IPV4ReputationDownloader = IPV4ReputationDownloader()
 
-            dataset = {filename: {"content": file_helper.read(), "hash": file_hash}}
+    def __init__(self) -> None:
+        self.source_file = os.path.join(
+            PyFunceble.storage.CONFIG_DIRECTORY,
+            PyFunceble.storage.IPV4_REPUTATION_FILENAME,
+        )
 
-            if directory not in result:
-                result[directory] = dataset
-            else:
-                result[directory].update(dataset)
+    def __contains__(self, value: Any) -> bool:
+        with self.get_content() as file_stream:
+            for line in file_stream:
+                line = line.strip()
 
-        PyFunceble.facility.Logger.debug("Dir Structure to backup:\n%r", result)
+                if line.startswith(f"{value}#"):
+                    return True
 
-        return result
+        return False
 
-    def store_backup(self) -> "DirectoryStructureBackup":
-        """
-        Stores the backup at the current destination.
+    @DatasetBase.ensure_source_file_exists
+    def get_content(self) -> open:
         """
+        Provides a file handler which does let you read the content line by
+        line.
 
-        DictHelper(self.get_backup_data()).to_json_file(self.source_file)
+        :raise FileNotFoundError:
+            When the declared file does not exists.
+        """
 
-        PyFunceble.facility.Logger.info("Stored backup into: %r", self.source_file)
+        file_helper = FileHelper(self.source_file)
 
-        return self
+        if not file_helper.exists() and bool(self.DOWNLOADER):  # pragma: no cover
+            ## pragma reason: Safety.
+            self.DOWNLOADER.start()
 
-    def start(self) -> "DirectoryStructureBackup":
-        """
-        Starts the backup process.
-        """
+            if not file_helper.exists():
+                raise FileNotFoundError(file_helper.path)
 
-        return self.cleanup().store_backup()
+        return file_helper.open("r", encoding="utf-8")
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/filesystem/dir_structure/base.py` & `PyFunceble-4.2.0/PyFunceble/cli/filesystem/dir_structure/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/filesystem/dir_structure/restore.py` & `PyFunceble-4.2.0/PyFunceble/cli/filesystem/dir_structure/restore.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -103,15 +103,14 @@
         file_helper = FileHelper()
 
         if dir_helper.set_path(base_dir).exists():
             for root, _, files in os.walk(dir_helper.path):
                 reduced_path = self.get_path_without_base_dir(root)
 
                 if reduced_path not in backup and root != reduced_path:
-
                     dir_helper.set_path(root).delete()
 
                     PyFunceble.facility.Logger.debug(
                         "Added %r into the list of directories to delete. "
                         "Reason: not found in own dataset.",
                         root,
                     )
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/filesystem/json_base.py` & `PyFunceble-4.2.0/PyFunceble/cli/filesystem/json_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/filesystem/printer/__init__.py` & `PyFunceble-4.2.0/PyFunceble/dataset/inactive/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides everything related to what we actually print (output) or to a file.
+Provides everything related to the inactive database logic(s).
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/filesystem/printer/base.py` & `PyFunceble-4.2.0/PyFunceble/cli/filesystem/printer/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/filesystem/printer/file.py` & `PyFunceble-4.2.0/PyFunceble/cli/filesystem/printer/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/filesystem/printer/stdout.py` & `PyFunceble-4.2.0/PyFunceble/cli/filesystem/printer/stdout.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/filesystem/registrar_counter.py` & `PyFunceble-4.2.0/PyFunceble/cli/filesystem/registrar_counter.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/filesystem/status_file.py` & `PyFunceble-4.2.0/PyFunceble/cli/filesystem/status_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -572,27 +572,42 @@
 
     @ensure_status_is_given
     def generate_plain_file(self) -> "StatusFileGenerator":
         """
         Generates the plain file.
         """
 
+        location = None
+
         if not hasattr(self.status, "ip_syntax") or not self.status.ip_syntax:
             location = os.path.join(
                 self.get_output_basedir(),
                 PyFunceble.cli.storage.OUTPUTS.domains.directory,
                 self.status.status.upper(),
                 PyFunceble.cli.storage.OUTPUTS.domains.filename,
             )
 
             self.file_printer.destination = location
             self.file_printer.dataset = self.status.to_dict()
             self.file_printer.template_to_use = "plain"
             self.file_printer.print_interpolated_line()
 
+        if not hasattr(self.status, "ip_syntax") or self.status.subject_kind == "ip":
+            location = os.path.join(
+                self.get_output_basedir(),
+                PyFunceble.cli.storage.OUTPUTS.ips.directory,
+                self.status.status.upper(),
+                PyFunceble.cli.storage.OUTPUTS.ips.filename,
+            )
+
+            self.file_printer.destination = location
+            self.file_printer.dataset = self.status.to_dict()
+            self.file_printer.template_to_use = "plain"
+            self.file_printer.print_interpolated_line()
+
         return self
 
     @ensure_status_is_given
     def generate_analytic_file(self) -> "StatusFileGenerator":
         """
         Generates the analytic files.
         """
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/migrators/__init__.py` & `PyFunceble-4.2.0/PyFunceble/cli/migrators/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/migrators/alembic.py` & `PyFunceble-4.2.0/PyFunceble/cli/migrators/alembic.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -51,14 +51,15 @@
 """
 
 import functools
 import os
 from typing import Any, Optional
 
 from sqlalchemy.orm import Session
+from sqlalchemy.sql import text
 
 try:
     import importlib.resources as package_resources
 except ImportError:  # pragma: no cover ## Retro compatibility
     import importlib_resources as package_resources
 
 import alembic
@@ -67,31 +68,31 @@
 from alembic.script.base import ScriptDirectory
 
 import PyFunceble.cli.facility
 import PyFunceble.cli.factory
 import PyFunceble.cli.storage
 import PyFunceble.facility
 import PyFunceble.sessions
-from PyFunceble.cli.migrators.mariadb.base import MariaDBMigratorBase
+from PyFunceble.cli.migrators.db_base import DBMigratorBase
 
 
 class Alembic:
     """
     Provides our very own alambic handler.
     """
 
     db_session: Optional[Session] = None
-    migrator_base: Optional[MariaDBMigratorBase] = None
+    migrator_base: Optional[DBMigratorBase] = None
 
     alembic_config: Optional[alembic.config.Config] = None
 
     def __init__(self, db_session: Session) -> None:
         self.db_session = db_session
 
-        self.migrator_base = MariaDBMigratorBase()
+        self.migrator_base = DBMigratorBase()
         self.migrator_base.db_session = db_session
 
     def execute_if_authorized(default: Any = None):  # pylint: disable=no-self-argument
         """
         Executes the decorated method only if we are authorized to process.
         Otherwise, apply the given :code:`default`.
         """
@@ -123,15 +124,19 @@
         Provides the location of our migration directory.
         """
 
         with package_resources.path(
             f"PyFunceble.data.{PyFunceble.cli.storage.ALEMBIC_DIRECTORY_NAME}",
             "__init__.py",
         ) as file_path:
-            return os.path.split(file_path)[0]
+            result = os.path.split(file_path)[0]
+
+        if PyFunceble.storage.CONFIGURATION.cli_testing.db_type == "postgresql":
+            return os.path.join(result, "postgresql")
+        return os.path.join(result, "mysql")
 
     @execute_if_authorized(None)
     def configure(self) -> "Alembic":
         """
         Configure our alembic configuration based on what we need.
         """
 
@@ -156,15 +161,17 @@
 
         revision_id = (
             ScriptDirectory.from_config(self.alembic_config)
             .get_revision(revision)
             .revision
         )
 
-        statement = "SELECT * from alembic_version WHERE version_num = :db_revision"
+        statement = text(
+            "SELECT * from alembic_version WHERE version_num = :db_revision"
+        )
 
         result = self.db_session.execute(statement, {"db_revision": revision_id})
 
         return result.fetchone() is None
 
     @execute_if_authorized(None)
     def upgrade(self, revision: str = "head") -> "Alembic":
@@ -200,15 +207,14 @@
         """
 
         self.configure()
 
         if not self.migrator_base.does_table_exists(
             "alembic_version"
         ) or self.is_revision_different(revision):
-
             PyFunceble.facility.Logger.info(
                 "Started downgrade (%r) of the database schema(s).", revision
             )
 
             alembic_command.downgrade(self.alembic_config, revision)
 
             PyFunceble.facility.Logger.info(
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/migrators/base.py` & `PyFunceble-4.2.0/PyFunceble/cli/migrators/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/migrators/csv_file/__init__.py` & `PyFunceble-4.2.0/PyFunceble/cli/migrators/csv_file/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/migrators/csv_file/base.py` & `PyFunceble-4.2.0/PyFunceble/cli/migrators/csv_file/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/migrators/csv_file/inactive_source_delete.py` & `PyFunceble-4.2.0/PyFunceble/cli/migrators/csv_file/inactive_source_delete.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/migrators/csv_file/whois_registrar_add.py` & `PyFunceble-4.2.0/PyFunceble/cli/migrators/csv_file/whois_registrar_add.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/migrators/db_base.py` & `PyFunceble-4.2.0/PyFunceble/cli/migrators/mariadb/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the base of all our database migration.
+Provides the base of all mariadb related migrations.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -47,30 +47,29 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
 import functools
-from typing import Any
+from typing import Any, Generator, Tuple
+
+from sqlalchemy.sql import text
 
 import PyFunceble.cli.facility
 import PyFunceble.cli.factory
 import PyFunceble.sessions
-from PyFunceble.cli.migrators.base import MigratorBase
+from PyFunceble.cli.migrators.db_base import DBMigratorBase
 
 
-class DBMigratorBase(MigratorBase):
+class MariaDBMigratorBase(DBMigratorBase):
     """
-    Provides the base of all our database migration.
+    Provides the base of all our mariadb migration.
     """
 
-    def __init__(self, print_action_to_stdout: bool = False) -> None:
-        super().__init__(print_action_to_stdout=print_action_to_stdout)
-
     def execute_if_authorized(default: Any = None):  # pylint: disable=no-self-argument
         """
         Executes the decorated method only if we are authorized to process.
         Otherwise, apply the given :code:`default`.
         """
 
         def inner_metdhod(func):
@@ -80,51 +79,57 @@
                     return func(self, *args, **kwargs)  # pylint: disable=not-callable
                 return self if default is None else default
 
             return wrapper
 
         return inner_metdhod
 
+    def get_rows(
+        self, statement: str, limit: int = 20
+    ) -> Generator[Tuple[str, int], dict, None]:
+        """
+        Run the given statement with a defined limit, and yield each row.
+
+        .. warning::
+            If you don't delete the given rows, this method will be infinite.
+        """
+
+        statement += f" LIMIT {limit}"
+
+        while True:
+            db_result = list(self.db_session.execute(text(statement)).fetchall())
+
+            if not db_result:
+                break
+
+            for result in db_result:
+                yield dict(result)
+
     @property
-    def authorized(self):
+    def authorized(self) -> bool:
         """
-        Provides the authorization to run.
+        Provides the authorization to process.
         """
 
         return PyFunceble.cli.facility.CredentialLoader.is_already_loaded()
 
-    def does_table_exists(self, table_name: str) -> bool:
+    @execute_if_authorized(None)
+    def migrate(self) -> "MariaDBMigratorBase":
         """
-        Checks if the table exists.
-
-        :param table_name:
-            The name of the table to check.
+        Provides the migration (itself).
         """
 
-        statement = (
-            "SELECT COUNT(*) "
-            "FROM information_schema.tables "
-            "WHERE table_schema = :database_name "
-            "AND table_name = :table_name "
-        )
+        raise NotImplementedError()
 
-        result = self.db_session.execute(
-            statement,
-            {
-                # pylint: disable=line-too-long
-                "database_name": PyFunceble.cli.facility.CredentialLoader.credential.name,
-                "table_name": table_name,
-            },
-        )
+    @execute_if_authorized(None)
+    def start(self) -> "MariaDBMigratorBase":
+        """
+        Starts the migration if wanted.
+        """
 
-        result = dict(result.fetchone())
+        PyFunceble.facility.Logger.info("Started migration.")
 
-        if result["COUNT(*)"] != 1:
-            return False
-        return True
+        self.migrate()
 
-    def start(self) -> "MigratorBase":
-        """
-        Starts the migration.
-        """
+        PyFunceble.facility.Logger.info("Finished migration.")
 
-        raise NotImplementedError()
+        return self
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/migrators/file_cleanup/__init__.py` & `PyFunceble-4.2.0/PyFunceble/data/alembic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,39 +7,39 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the file cleanup migrators.
+Provides the alembic data.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
-    https://pyfunceble.github.io/#/special-thanks
+    https://pyfunceble.github.io/special-thanks.html
 
 Contributors:
-    https://pyfunceble.github.io/#/contributors
+    https://pyfunceble.github.io/contributors.html
 
 Project link:
     https://github.com/funilrys/PyFunceble
 
 Project documentation:
     https://pyfunceble.readthedocs.io/en/latest/
 
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/migrators/file_cleanup/base.py` & `PyFunceble-4.2.0/PyFunceble/cli/migrators/file_cleanup/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/migrators/file_cleanup/hashes_file.py` & `PyFunceble-4.2.0/PyFunceble/cli/migrators/file_cleanup/hashes_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/migrators/file_cleanup/mining_file.py` & `PyFunceble-4.2.0/PyFunceble/cli/migrators/file_cleanup/mining_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/migrators/file_cleanup/production_config_file.py` & `PyFunceble-4.2.0/PyFunceble/cli/migrators/file_cleanup/production_config_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/migrators/json2csv/__init__.py` & `PyFunceble-4.2.0/PyFunceble/cli/migrators/json2csv/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/migrators/json2csv/base.py` & `PyFunceble-4.2.0/PyFunceble/cli/migrators/json2csv/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/migrators/json2csv/inactive.py` & `PyFunceble-4.2.0/PyFunceble/cli/migrators/json2csv/inactive.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/migrators/json2csv/whois.py` & `PyFunceble-4.2.0/PyFunceble/cli/migrators/json2csv/whois.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/migrators/mariadb/__init__.py` & `PyFunceble-4.2.0/PyFunceble/cli/migrators/mariadb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/migrators/mariadb/base.py` & `PyFunceble-4.2.0/PyFunceble/helpers/hash.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the base of all mariadb related migrations.
+Provides the hashing helpers.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,125 +31,139 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-import functools
-from typing import Any, Generator, Tuple
+from typing import Optional, Union
 
-import PyFunceble.cli.facility
-import PyFunceble.cli.factory
-import PyFunceble.sessions
-from PyFunceble.cli.migrators.base import MigratorBase
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives import hashes
 
+from PyFunceble.helpers.file import FileHelper
 
-class MariaDBMigratorBase(MigratorBase):
+
+class HashHelper:
     """
-    Provides the base of all our mariadb migration.
+    Simplify the hashing of data or file content.
+
+    :param str algo:
+        The algorithm to use for hashing.
+
+    :raise ValueError: When the given algo is not known.
     """
 
-    def execute_if_authorized(default: Any = None):  # pylint: disable=no-self-argument
+    _algo: str = "SHA512_224"
+
+    def __init__(self, algo: Optional[str] = None):
+        if algo is not None:
+            self.algo = algo
+
+    @property
+    def algo(self) -> str:
         """
-        Executes the decorated method only if we are authorized to process.
-        Otherwise, apply the given :code:`default`.
+        Provides the current state fo the :code:`_algo` attribute.
         """
 
-        def inner_metdhod(func):
-            @functools.wraps(func)
-            def wrapper(self, *args, **kwargs):
-                if self.authorized:
-                    return func(self, *args, **kwargs)  # pylint: disable=not-callable
-                return self if default is None else default
+        return self._algo
 
-            return wrapper
+    @algo.setter
+    def algo(self, value: str) -> None:
+        """
+        Sets the algorithm to work with.
 
-        return inner_metdhod
+        :param value:
+            The name of the hash to use.
 
-    def does_table_exists(self, name: str) -> bool:
-        """
-        Checks if the given table name exists.
+        :raise TypeError:
+            When :code:`value` is not a :py:class:`str`.
         """
 
-        statement = (
-            "SELECT COUNT(*) "
-            "FROM information_schema.tables "
-            "WHERE table_schema = :database_name "
-            "AND table_name = :table_name "
-        )
+        if not isinstance(value, str):
+            raise TypeError(f"<value> should be {str}, {type(value)} given.")
 
-        result = self.db_session.execute(
-            statement,
-            {
-                "database_name": PyFunceble.cli.factory.DBSession.credential.name,
-                "table_name": name,
-            },
-        ).fetchone()
+        value = value.upper()
 
-        return result["COUNT(*)"] == 1
+        if not hasattr(hashes, value):
+            raise ValueError(
+                f"<value> ({value!r}) in an unknown algorithm ({self.algo!r})."
+            )
 
-    def get_rows(
-        self, statement: str, limit: int = 20
-    ) -> Generator[Tuple[str, int], dict, None]:
-        """
-        Run the given statement with a defined limit, and yield each row.
+        self._algo = value
 
-        .. warning::
-            If you don't delete the given rows, this method will be infinite.
+    def set_algo(self, value: str) -> "HashHelper":
         """
+        Sets the algorithm to work with.
 
-        statement += f" LIMIT {limit}"
-
-        while True:
-            db_result = list(self.db_session.execute(statement).fetchall())
+        :param value:
+            The name of the hash to use.
+        """
 
-            if not db_result:
-                break
+        self.algo = value
 
-            for result in db_result:
-                yield dict(result)
+        return self
 
-    @property
-    def authorized(self) -> bool:
+    def __get_hash(self) -> hashes.Hash:
         """
-        Provides the authorization to process.
+        Provides the Hash to use.
         """
 
-        return PyFunceble.cli.facility.CredentialLoader.is_already_loaded()
+        return hashes.Hash(getattr(hashes, self.algo)(), backend=default_backend())
 
-    @execute_if_authorized(None)
-    def migrate(self) -> "MariaDBMigratorBase":
+    def hash_file(self, file_path: str) -> str:
         """
-        Provides the migration (itself).
+        Hashes the content of the given file.
+
+        :param file_path:
+            The path of the file to read.
         """
 
-        raise NotImplementedError()
+        block_size = 4096
+
+        digest = self.__get_hash()
+
+        with FileHelper(file_path).open("rb") as file_stream:
+            block = file_stream.read(block_size)
 
-    @execute_if_authorized(None)
-    def start(self) -> "MariaDBMigratorBase":
+            while block:
+                digest.update(block)
+                block = file_stream.read(block_size)
+
+        return digest.finalize().hex()
+
+    def hash_data(self, data: Union[str, bytes]) -> str:
         """
-        Starts the migration if wanted.
+        Hashes the given data.
+
+        :param data:
+            The data to hash.
+
+        :raise TypeError:
+            When :code:`data` is not :py:class:`str` or :py:class:`bytes`.
         """
 
-        PyFunceble.facility.Logger.info("Started migration.")
+        if not isinstance(data, (bytes, str)):
+            raise TypeError(f"<data> should be {bytes} or {str}, {type(data)}, given.")
 
-        self.migrate()
+        if isinstance(data, str):
+            data = data.encode()
 
-        PyFunceble.facility.Logger.info("Finished migration.")
+        digest = self.__get_hash()
+        digest.update(data)
 
-        return self
+        return digest.finalize().hex()
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/migrators/mariadb/file_and_status.py` & `PyFunceble-4.2.0/PyFunceble/cli/migrators/mariadb/file_and_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -48,14 +48,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
 import domain2idna
+from sqlalchemy.sql import text
 
 import PyFunceble.cli.facility
 import PyFunceble.cli.factory
 import PyFunceble.cli.utils.testing
 import PyFunceble.facility
 import PyFunceble.sessions
 import PyFunceble.storage
@@ -92,15 +93,14 @@
 
         inactive_dataset = PyFunceble.cli.utils.testing.get_inactive_dataset_object()
         continue_dataset = PyFunceble.cli.utils.testing.get_continue_databaset_object()
 
         drop_table = True
 
         for file_info in self.get_rows("SELECT * from pyfunceble_file"):
-
             if (
                 self.continuous_integration
                 and self.continuous_integration.is_time_exceeded()
             ):
                 drop_table = False
                 break
 
@@ -140,44 +140,44 @@
 
                 PyFunceble.facility.Logger.info(
                     "Added %r into %r", to_send["idna_subject"], continue_dataset
                 )
 
                 # pylint: disable=line-too-long
                 self.db_session.execute(
-                    f"DELETE from pyfunceble_status WHERE id = {status['id']}"
+                    text(f"DELETE from pyfunceble_status WHERE id = {status['id']}")
                 )
                 self.db_session.commit()
 
                 PyFunceble.facility.Logger.debug(
                     "Deleted from pyfunceble_status: \n%r", status
                 )
 
             if drop_table:
                 # pylint: disable=line-too-long
                 self.db_session.execute(
-                    f"DELETE from pyfunceble_file WHERE id = {file_info['id']}"
+                    text(f"DELETE from pyfunceble_file WHERE id = {file_info['id']}")
                 )
                 self.db_session.commit()
 
                 PyFunceble.facility.Logger.debug(
                     "Deleted from pyfunceble_file: \n%r", file_info
                 )
             else:
                 PyFunceble.facility.Logger.debug(
                     "Not deleted from pyfunceble_file (not authorized): \n%r", file_info
                 )
 
         if drop_table:
-            self.db_session.execute("DROP TABLE pyfunceble_file")
+            self.db_session.execute(text("DROP TABLE pyfunceble_file"))
             self.db_session.commit()
 
             PyFunceble.facility.Logger.debug("Deleted pyfunceble_file table.")
 
-            self.db_session.execute("DROP TABLE pyfunceble_status")
+            self.db_session.execute(text("DROP TABLE pyfunceble_status"))
             self.db_session.commit()
 
             PyFunceble.facility.Logger.debug("Deleted pyfunceble_status table.")
 
             self.done = True
         else:
             PyFunceble.facility.Logger.debug(
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/migrators/mariadb/whois_record_idna_subject.py` & `PyFunceble-4.2.0/PyFunceble/cli/migrators/mariadb/whois_record_idna_subject.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/processes/__init__.py` & `PyFunceble-4.2.0/PyFunceble/cli/processes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/processes/base.py` & `PyFunceble-4.2.0/PyFunceble/cli/processes/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/processes/chancy_producer.py` & `PyFunceble-4.2.0/PyFunceble/cli/processes/chancy_producer.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/processes/chancy_tester.py` & `PyFunceble-4.2.0/PyFunceble/cli/processes/chancy_tester.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/processes/dir_files_sorter.py` & `PyFunceble-4.2.0/PyFunceble/cli/processes/dir_files_sorter.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/processes/file_sorter.py` & `PyFunceble-4.2.0/PyFunceble/cli/processes/file_sorter.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/processes/migrator.py` & `PyFunceble-4.2.0/PyFunceble/cli/processes/migrator.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/processes/miner.py` & `PyFunceble-4.2.0/PyFunceble/cli/processes/miner.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/processes/producer.py` & `PyFunceble-4.2.0/PyFunceble/cli/processes/producer.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/processes/tester.py` & `PyFunceble-4.2.0/PyFunceble/cli/processes/tester.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/processes/workers/__init__.py` & `PyFunceble-4.2.0/PyFunceble/cli/processes/workers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/processes/workers/base.py` & `PyFunceble-4.2.0/PyFunceble/cli/processes/workers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/processes/workers/chancy_producer.py` & `PyFunceble-4.2.0/PyFunceble/cli/processes/workers/chancy_producer.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/processes/workers/chancy_tester.py` & `PyFunceble-4.2.0/PyFunceble/cli/processes/workers/chancy_tester.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/processes/workers/dir_files_sorter.py` & `PyFunceble-4.2.0/PyFunceble/cli/processes/workers/dir_files_sorter.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/processes/workers/file_sorter.py` & `PyFunceble-4.2.0/PyFunceble/cli/processes/workers/file_sorter.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/processes/workers/file_sorter_base.py` & `PyFunceble-4.2.0/PyFunceble/cli/processes/workers/file_sorter_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/processes/workers/migrator.py` & `PyFunceble-4.2.0/PyFunceble/cli/processes/workers/migrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -65,15 +65,14 @@
     to handle the mining of dataset to test.
     """
 
     STD_NAME: str = "pyfunceble_migrator_worker"
 
     def run(self) -> None:
         try:
-
             try:
                 self.target(self.continuous_integration, db_session=self.db_session)
             except TypeError:
                 self.target(self.continuous_integration)
             self._child_connection.send(None)
         except Exception as exception:  # pylint: disable=broad-except
             PyFunceble.facility.Logger.critical(
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/processes/workers/miner.py` & `PyFunceble-4.2.0/PyFunceble/cli/processes/workers/miner.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/processes/workers/producer.py` & `PyFunceble-4.2.0/PyFunceble/cli/processes/workers/producer.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -211,19 +211,17 @@
             # from the database.
 
             self.whois_dataset.update(
                 {
                     "subject": test_result.subject,
                     "idna_subject": test_result.idna_subject,
                     "expiration_date": test_result.expiration_date,
-                    "epoch": str(
-                        datetime.datetime.strptime(
-                            test_result.expiration_date, "%d-%b-%Y"
-                        ).timestamp()
-                    ),
+                    "epoch": datetime.datetime.strptime(
+                        test_result.expiration_date, "%d-%b-%Y"
+                    ).timestamp(),
                     "registrar": test_result.registrar,
                 }
             )
 
     def run_inactive_backup(
         self, test_dataset: dict, test_result: CheckerStatusBase
     ) -> None:
@@ -344,24 +342,32 @@
             self.status_file_generator.allow_plain_files = previous_allow_plain_file
 
     def run_counter(self, test_dataset: dict, test_result: CheckerStatusBase) -> None:
         """
         Runs the counter of the current file.
         """
 
-        if (
-            test_dataset["destination"]
-            and not PyFunceble.storage.CONFIGURATION.cli_testing.file_generation.no_file
-        ):
+        if not PyFunceble.storage.CONFIGURATION.cli_testing.file_generation.no_file:
             # Note: We don't want hidden data to be counted.
 
-            self.counter.set_parent_dirname(test_dataset["destination"]).count(
-                test_result
+            self.counter.set_differ_to_inline(True).set_parent_dirname(
+                test_dataset["destination"]
+            )
+            self.registrar_counter.set_differ_to_inline(True).set_parent_dirname(
+                test_dataset["destination"]
             )
 
+            self.counter.count(test_result)
+
+            if hasattr(test_result, "registrar") and test_result.registrar:
+                self.registrar_counter.count(test_result.registrar)
+
+            self.counter.set_differ_to_inline(False)
+            self.registrar_counter.set_differ_to_inline(False)
+
             if hasattr(test_result, "registrar") and test_result.registrar:
                 self.registrar_counter.set_parent_dirname(
                     test_dataset["destination"]
                 ).count(test_result.registrar)
 
     def target(self, consumed: Any) -> Optional[Tuple[Any, ...]]:
         if not isinstance(consumed, tuple):
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/processes/workers/tester.py` & `PyFunceble-4.2.0/PyFunceble/cli/processes/workers/tester.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -57,15 +57,15 @@
 import PyFunceble.facility
 import PyFunceble.factory
 from PyFunceble.checker.availability.domain_and_ip import DomainAndIPAvailabilityChecker
 from PyFunceble.checker.availability.url import URLAvailabilityChecker
 from PyFunceble.checker.base import CheckerBase
 from PyFunceble.checker.reputation.domain_and_ip import DomainAndIPReputationChecker
 from PyFunceble.checker.reputation.url import URLReputationChecker
-from PyFunceble.checker.syntax.domain import DomainSyntaxChecker
+from PyFunceble.checker.syntax.domain_and_ip import DomainAndIPSyntaxChecker
 from PyFunceble.checker.syntax.ip import IPSyntaxChecker
 from PyFunceble.checker.syntax.url import URLSyntaxChecker
 from PyFunceble.cli.processes.workers.base import WorkerBase
 from PyFunceble.cli.utils.stdout import print_single_line
 from PyFunceble.dataset.autocontinue.base import ContinueDatasetBase
 from PyFunceble.dataset.autocontinue.csv import CSVContinueDataset
 from PyFunceble.dataset.inactive.base import InactiveDatasetBase
@@ -97,15 +97,15 @@
         self.inactive_dataset = (
             PyFunceble.cli.utils.testing.get_inactive_dataset_object(
                 db_session=self.db_session
             )
         )
 
         self.known_testing_objects = {
-            "SYNTAX": {"domain": DomainSyntaxChecker, "url": URLSyntaxChecker},
+            "SYNTAX": {"domain": DomainAndIPSyntaxChecker, "url": URLSyntaxChecker},
             "AVAILABILITY": {
                 "domain": DomainAndIPAvailabilityChecker,
                 "url": URLAvailabilityChecker,
             },
             "REPUTATION": {
                 "domain": DomainAndIPReputationChecker,
                 "url": URLReputationChecker,
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/scripts/__init__.py` & `PyFunceble-4.2.0/PyFunceble/cli/scripts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/scripts/iana.py` & `PyFunceble-4.2.0/PyFunceble/cli/scripts/iana.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/scripts/production.py` & `PyFunceble-4.2.0/PyFunceble/cli/scripts/production.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/scripts/public_suffix.py` & `PyFunceble-4.2.0/PyFunceble/cli/scripts/public_suffix.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/storage.py` & `PyFunceble-4.2.0/PyFunceble/cli/storage.py`

 * *Files 23% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -63,48 +63,90 @@
 
 if PlatformUtility.is_unix() and sys.stdin.encoding == "utf-8":
     STD_EPILOG: str = (
         f"Crafted with {colorama.Fore.RED}♥{colorama.Fore.RESET} by "
         f"{colorama.Style.BRIGHT}{colorama.Fore.CYAN}Nissar Chababy (@funilrys)"
         f"{colorama.Style.RESET_ALL} "
         f"with the help of\n{colorama.Style.BRIGHT}{colorama.Fore.GREEN}"
-        f"https://git.io/JkUPS{colorama.Style.RESET_ALL} "
+        f"https://pyfunceble.github.io/#/contributors{colorama.Style.RESET_ALL} "
         f"&& {colorama.Style.BRIGHT}{colorama.Fore.GREEN}"
-        f"https://git.io/JkUPF{colorama.Style.RESET_ALL}"
+        f"https://pyfunceble.github.io/#/special-thanks{colorama.Style.RESET_ALL}"
     )
 
     ASCII_PYFUNCEBLE = """
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
     """
+
+    ASCII_PYUNCEBLE_RESULT = """
+                          █
+                        ████    ██
+                     ███ ██   █████   ███
+               ███ █████    █████   █████
+             ██████████   █████   █████
+           ██████████   █████   ██████   ██
+         ██████████   █████   ██████   ████
+       ███████████████████████████   █████
+      ██████████████████████████   ████
+     ████████ █████ ██████████   █████
+     ███████   ███   ███████   █████
+     █████████████████████   █████
+     ████████████████████  █████
+     ███████         █████████
+      ████████     █████████
+        ██████████████████
+          ██████████████
+               ████
+
+    """
     DONE: str = f"{colorama.Fore.GREEN}✔"
     ERROR: str = f"{colorama.Fore.RED}✘"
 else:
     STD_EPILOG: str = (
         f"Crafted with {colorama.Fore.RED}HEART{colorama.Fore.RESET} by "
         f"{colorama.Style.BRIGHT}{colorama.Fore.CYAN}Nissar Chababy (@funilrys)"
         f"{colorama.Style.RESET_ALL} "
         f"with the help of\n{colorama.Style.BRIGHT}{colorama.Fore.GREEN}"
-        f"https://git.io/JkUPS{colorama.Style.RESET_ALL} "
+        f"https://pyfunceble.github.io/#/contributors{colorama.Style.RESET_ALL} "
         f"&& {colorama.Style.BRIGHT}{colorama.Fore.GREEN}"
-        f"https://git.io/JkUPF{colorama.Style.RESET_ALL}"
+        f"https://pyfunceble.github.io/#/special-thanks{colorama.Style.RESET_ALL}"
     )
     ASCII_PYFUNCEBLE = """
     ########  ##    ## ######## ##     ## ##    ##  ######  ######## ########  ##       ########
     ##     ##  ##  ##  ##       ##     ## ###   ## ##    ## ##       ##     ## ##       ##
     ##     ##   ####   ##       ##     ## ####  ## ##       ##       ##     ## ##       ##
     ########     ##    ######   ##     ## ## ## ## ##       ######   ########  ##       ######
     ##           ##    ##       ##     ## ##  #### ##       ##       ##     ## ##       ##
     ##           ##    ##       ##     ## ##   ### ##    ## ##       ##     ## ##       ##
     ##           ##    ##        #######  ##    ##  ######  ######## ########  ######## ########
-"""
+    """
+    ASCII_PYUNCEBLE_RESULT = """
+                          .
+                        :==:    ::
+                     .:. ..   :-=-.   .:.
+               .:. .-==-    :-=-:   .-==:
+             .-==--==-.   :-=-:   .-==:
+           .-===-==-.   :-=-:   .-==:.   ..
+         .-==-====:   :-==.   .-==:.   :==-
+       .-==--=====-::-==-=:..-==:.   ..--.
+      :===============-=======:.   :-=:
+     :=-===:  .-=-. .-======:.   :==-.
+     -=====.   --:   -====-.   :==-.
+     =======--=====-====:.   :==-.
+     -=====---:::::---==.  :==-.
+     .==--=.         -===-==-.
+      .-==--:      .-=-===-.
+        :-====-----=====-.
+          .:-=======--:.
+               ....
+    """
     DONE: str = f"{colorama.Fore.GREEN}DONE"
     ERROR: str = f"{colorama.Fore.RED}ERROR"
 
 VERSION_DUMP_LINK: str = (
     "https://raw.githubusercontent.com/funilrys/PyFunceble/master/version.yaml"
 )
 
@@ -130,14 +172,15 @@
 PRE_LOADER_FILE = "preload.json"
 
 STD_PARENT_DIRNAME: str = "__pyfunceble_origin__"
 STD_LOGGING_DIRNAME: str = "__pyfunceble_loggging__"
 
 UNIX_OUTPUTS: dict = {
     "domains": {"filename": "list"},
+    "ips": {"filename": "list"},
     "hosts": {"filename": "hosts", "ip_filename": "ips"},
     "analytic": {
         "filenames": {
             "potentially_down": "down_or_potentially_down",
             "potentially_up": "potentially_up",
             "up": "active_and_merged_in_results",
             "suspicious": "suspicious_and_merged_in_results",
@@ -148,14 +191,15 @@
             "inactive_not_retested": "inactive_not_retested",
         },
     },
 }
 
 WIN_OUTPUTS: dict = {
     "domains": {"filename": "list.txt"},
+    "ips": {"filename": "list.txt"},
     "hosts": {"filename": "hosts.txt", "ip_filename": "ips.txt"},
     "analytic": {
         "filenames": {
             "potentially_down": "down_or_potentially_down.txt",
             "potentially_up": "potentially_up.txt",
             "up": "active_and_merged_in_results.txt",
             "suspicious": "suspicious_and_merged_in_results.txt",
@@ -166,14 +210,15 @@
             "inactive_not_retested": "inactive_not_retested.txt",
         },
     },
 }
 
 UNIVERSAL_OUTPUTS: dict = {
     "domains": {"directory": "domains", "filename": "list"},
+    "ips": {"directory": "ips", "filename": "list"},
     "hosts": {"directory": "hosts", "filename": "hosts", "ip_filename": "ips"},
     "analytic": {
         "directories": {
             "parent": "Analytic",
             "potentially_down": "POTENTIALLY_INACTIVE",
             "potentially_up": "POTENTIALLY_ACTIVE",
             "up": "ACTIVE",
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/storage_facility.py` & `PyFunceble-4.2.0/PyFunceble/cli/storage_facility.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/system/__init__.py` & `PyFunceble-4.2.0/PyFunceble/cli/system/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/system/base.py` & `PyFunceble-4.2.0/PyFunceble/cli/system/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/system/integrator.py` & `PyFunceble-4.2.0/PyFunceble/cli/system/integrator.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/system/launcher.py` & `PyFunceble-4.2.0/PyFunceble/cli/system/launcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -112,14 +112,15 @@
 from PyFunceble.converter.rpz_policy2subject import RPZPolicy2Subject
 from PyFunceble.converter.subject2complements import Subject2Complements
 from PyFunceble.converter.url2netloc import Url2Netloc
 from PyFunceble.converter.wildcard2subject import Wildcard2Subject
 from PyFunceble.dataset.autocontinue.base import ContinueDatasetBase
 from PyFunceble.dataset.autocontinue.csv import CSVContinueDataset
 from PyFunceble.dataset.inactive.base import InactiveDatasetBase
+from PyFunceble.helpers.directory import DirectoryHelper
 from PyFunceble.helpers.download import DownloadHelper
 from PyFunceble.helpers.file import FileHelper
 
 
 class SystemLauncher(SystemBase):
     """
     Provides the system tests launcher.
@@ -546,15 +547,14 @@
                     )
 
                 self.__start_core_processes()
 
                 for subject in self.continue_dataset.get_to_test(
                     protocol["session_id"]
                 ):
-
                     self.ci_stop_in_the_middle_if_time_exceeded()
 
                     to_send = copy.deepcopy(protocol)
                     to_send["subject"], to_send["idna_subject"] = subject, subject
                     to_send["from_preload"] = True
 
                     self.tester_process_manager.add_to_input_queue(
@@ -651,21 +651,23 @@
 
     def generate_waiting_files(self) -> "SystemLauncher":
         """
         Generates all the files that needs to be generated when all status
         are proceeses.
         """
 
-        def generate_percentage_file(parent_dirname: str) -> None:
+        def generate_percentage_file(parent_dirname: Union[str, None]) -> None:
             """
             Generates the percentage file.
             """
 
             if not PyFunceble.storage.CONFIGURATION.cli_testing.file_generation.no_file:
-                self.counter.set_parent_dirname(parent_dirname)
+                self.counter.set_differ_to_inline(True).set_parent_dirname(
+                    parent_dirname
+                )
 
                 destination = os.path.join(
                     self.counter.get_output_basedir(),
                     PyFunceble.cli.storage.OUTPUTS.logs.directories.parent,
                     PyFunceble.cli.storage.OUTPUTS.logs.directories.percentage,
                     PyFunceble.cli.storage.OUTPUTS.logs.filenames.percentage,
                 )
@@ -688,21 +690,23 @@
 
                         if not stdout_header_printed:
                             self.stdout_printer.print_header()
                             stdout_header_printed = True
 
                         self.stdout_printer.print_interpolated_line()
 
-        def generate_registrar_file(parent_dirname: str) -> None:
+        def generate_registrar_file(parent_dirname: Union[str, None]) -> None:
             """
             Generates the registrar file.
             """
 
             if not PyFunceble.storage.CONFIGURATION.cli_testing.file_generation.no_file:
-                self.registrar_counter.set_parent_dirname(parent_dirname)
+                self.registrar_counter.set_differ_to_inline(True).set_parent_dirname(
+                    parent_dirname
+                )
 
                 destination = os.path.join(
                     self.counter.get_output_basedir(),
                     PyFunceble.cli.storage.OUTPUTS.logs.directories.parent,
                     PyFunceble.cli.storage.OUTPUTS.logs.directories.percentage,
                     PyFunceble.cli.storage.OUTPUTS.logs.filenames.registrar,
                 )
@@ -729,19 +733,57 @@
                         if not stdout_header_printed:
                             self.stdout_printer.print_header()
                             stdout_header_printed = True
 
                         self.stdout_printer.print_interpolated_line()
                         registrar_limit += 1
 
+        def print_result_ascii(parent_dirname: Union[str, None]) -> None:
+            """
+            Generates the result repr.
+            """
+
+            # pylint: disable=line-too-long
+            if (
+                not PyFunceble.storage.CONFIGURATION.cli_testing.file_generation.no_file
+                and not PyFunceble.storage.CONFIGURATION.cli_testing.display_mode.quiet
+                and PyFunceble.cli.utils.stdout.get_template_to_use() != "simple"
+            ):
+                self.counter.set_differ_to_inline(True).set_parent_dirname(
+                    parent_dirname
+                )
+
+                print(
+                    PyFunceble.cli.utils.ascii_logo.get_result_representation(
+                        self.counter.get_sorted_dataset()[0][0]
+                    )
+                )
+
+        no_destination_found = []
+        amount_protocol_without_dest = len(
+            [x["destination"] for x in self.testing_protocol if not x["destination"]]
+        )
+
         for protocol in self.testing_protocol:
             if not protocol["destination"]:
-                continue
+                if any(no_destination_found):
+                    continue
 
-            generate_percentage_file(protocol["destination"])
+                if amount_protocol_without_dest >= 2:
+                    # Show percentage, only if the amount of subjects is > 2.
+                    generate_percentage_file(protocol["destination"])
+            else:
+                generate_percentage_file(protocol["destination"])
+
+            if protocol["checker_type"] in self.registrar_counter.SUPPORTED_TEST_MODES:
+                generate_registrar_file(protocol["destination"])
+
+            print_result_ascii(protocol["destination"])
+
+            no_destination_found.append(not protocol["destination"])
 
             if protocol["checker_type"] in self.registrar_counter.SUPPORTED_TEST_MODES:
                 generate_registrar_file(protocol["destination"])
 
             # pylint: disable=line-too-long
             if (
                 PyFunceble.storage.CONFIGURATION.cli_testing.file_generation.merge_output_dirs
@@ -828,23 +870,39 @@
                     os.path.join(
                         protocol["output_dir"],
                         PyFunceble.cli.storage.PRE_LOADER_FILE,
                     )
                 ).delete()
                 PyFunceble.facility.Logger.debug("Deleted: %r.", file_helper.path)
 
+        def remove_inline_dest(protocol: dict) -> None:
+            """
+            Remove the inline destination - when necessary.
+
+            :param protocl:
+                The protocol to work with.
+            """
+
+            if not protocol["destination"]:
+                DirectoryHelper(
+                    self.counter.set_differ_to_inline(True)
+                    .set_parent_dirname(protocol["destination"])
+                    .get_output_basedir()
+                ).delete()
+
         file_helper = FileHelper()
 
         for protocol in self.testing_protocol:
             if "destination" in protocol or "output_dir" in protocol:
                 remove_running_file(protocol)
                 remove_trigger_file(protocol)
 
                 remove_continue_dataset(protocol)
                 remove_preload_dataset(protocol)
+                remove_inline_dest(protocol)
 
         return self
 
     def run_standard_end_instructions(self) -> "SystemLauncher":
         """
         Runns our standard "end" instructions.
 
@@ -994,14 +1052,15 @@
                 # Reason: We have to continue.
                 self.run_ci_saving_instructions()
             elif self.continuous_integration.authorized:
                 # Includes the run_standard_end_instructions call.
                 self.run_ci_end_saving_instructions()
             else:
                 self.run_standard_end_instructions()
+
         except (KeyboardInterrupt, StopExecution):
             pass
         except Exception as exception:  # pylint: disable=broad-except
             PyFunceble.facility.Logger.critical(
                 "Fatal error.",
                 exc_info=True,
             )
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/utils/__init__.py` & `PyFunceble-4.2.0/PyFunceble/query/netinfo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides some utilities related to the CLI.
+Provides all our network info related subdmodules.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/utils/ascii_logo.py` & `PyFunceble-4.2.0/PyFunceble/query/record/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides some utilities related to the ascii logo.
+Provides the base of all our record classes.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,71 +31,61 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-import colorama
+import dataclasses
+import json
+from typing import Any
 
-import PyFunceble.cli.storage
-import PyFunceble.facility
-import PyFunceble.storage
 
-
-def colorify(color: str) -> str:
+@dataclasses.dataclass
+class RecordBase:
     """
-    Colorify the logo with the given color.
-
-    :param color:
-        The name of the color to apply.
-
-        .. warning::
-            The given color name must be one of the supported
-            by colorama.
-
-    :raise ValueError:
-        When the given :code:`color` is unsupported.
+    Provides the base of all query record classes.
     """
 
-    color = color.upper()
-
-    if not hasattr(colorama.Fore, color):
-        raise ValueError(f"<color> ({color!r}) is not supported.")
-
-    color_to_apply = getattr(colorama.Fore, color)
-    result = []
-
-    to_color = PyFunceble.cli.storage.ASCII_PYFUNCEBLE
-
-    if (
-        PyFunceble.facility.ConfigLoader.is_already_loaded()
-        and PyFunceble.storage.CONFIGURATION.cli_testing.display_mode.colour
-    ):
-        for line in to_color.split("\n"):
-            result.append(f"{color_to_apply}{line}{colorama.Fore.RESET}")
-
-        return "\n".join(result)
-    return to_color
-
-
-def get_home_representation() -> str:
-    """
-    Provides our home ASCII logo representation.
-    """
+    def __getitem__(self, key: str) -> Any:
+        return getattr(self, key)
 
-    return colorify("yellow")
+    def to_dict(self) -> dict:
+        """
+        Provides the dict representation of the current object.
+        """
+
+        return {
+            x: y if not hasattr(y, "to_dict") else y.to_dict()
+            for x, y in self.__dict__.items()
+            if not x.startswith("__")
+        }
+
+    def to_json(self, *, pretty_print: bool = False) -> str:
+        """
+        Provides the JSON representation of the current object.
+
+        :param pretty_print:
+            If True, the JSON will be formatted.
+        """
+
+        return json.dumps(
+            self.to_dict(),
+            indent=4 if pretty_print else None,
+            ensure_ascii=False,
+            sort_keys=True if pretty_print else None,
+        )
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/utils/sort.py` & `PyFunceble-4.2.0/PyFunceble/dataset/whois/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides some utilities related to the sorting mechanism.
+Provides the base of all WHOIS related dataset.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,92 +31,79 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-from typing import Any, Callable, List, Union
+from datetime import datetime
+from typing import List, Union
 
-import PyFunceble.facility
-import PyFunceble.storage
-from PyFunceble.converter.url2netloc import Url2Netloc
-from PyFunceble.helpers.regex import RegexHelper
+from PyFunceble.database.sqlalchemy.all_schemas import WhoisRecord
+from PyFunceble.dataset.db_base import DBDatasetBase
 
 
-def standard(element: Any) -> List[Union[int, Any]]:
+class WhoisDatasetBase(DBDatasetBase):
     """
-    Provides the key to use for the standard sorting.
-
-    :param element:
-        The element to format.
+    Provides the base of all Whois related interface.
     """
 
-    element = element.strip()
-
-    if not element:
-        return []
-
-    regex_helper = RegexHelper()
-
-    element = Url2Netloc(element).get_converted().strip()
-
-    if PyFunceble.facility.ConfigLoader.is_already_loaded():
-        element = regex_helper.set_regex(
-            r"^%s\s+" % PyFunceble.storage.CONFIGURATION.cli_testing.hosts_ip
-        ).replace_match(element, "")
-
-    cleaned = regex_helper.set_regex(r"[^a-zA-Z0-9\.]").replace_match(element, "")
-
-    return [
-        int(x) if x.isdigit() else x
-        for x in regex_helper.set_regex(r"(\d+)").split(cleaned)
+    FIELDS: List[str] = [
+        "subject",
+        "idna_subject",
+        "expiration_date",
+        "epoch",
+        "registrar",
     ]
 
+    COMPARISON_FIELDS: List[str] = ["subject", "idna_subject"]
 
-def hierarchical(element: Any) -> List[Union[int, Any]]:
-    """
-    Provides the key to use for the hierarchical sorting.
-
-    :param element:
-        The element to format.
-    """
-
-    element = element.strip()
-
-    if not element:
-        return []
-
-    element = Url2Netloc(element).get_converted().strip()
-
-    if PyFunceble.facility.ConfigLoader.is_already_loaded():
-        element = RegexHelper(
-            r"^%s\s+" % PyFunceble.storage.CONFIGURATION.cli_testing.hosts_ip
-        ).replace_match(element, "")
-
-    return standard(".".join(reversed(element.split("."))))
-
-
-def get_best_sorting_key() -> Callable[[Any], List[Union[int, Any]]]:
-    """
-    Provides the best sorting key from the configuration.
-    """
+    @staticmethod
+    def is_expired(row: Union[dict, WhoisRecord]) -> bool:
+        """
+        Given a row, we look if the row is expired.
+        """
+
+        if isinstance(row, WhoisRecord):
+            to_check = row.epoch
+        elif "epoch" in row:
+            to_check = row["epoch"]
+        else:
+            return True
+
+        return datetime.utcnow() > datetime.fromtimestamp(float(to_check))
+
+    @DBDatasetBase.execute_if_authorized(None)
+    def get_filtered_row(self, row: Union[dict, WhoisRecord]) -> dict:
+        """
+        Removes all unkowns fields (not declared) from the given row.
+
+        :param row:
+            The row to work with.
+        """
+
+        if isinstance(row, WhoisDatasetBase):
+            row = row.to_dict()
+
+        result = super().get_filtered_row(row)
+
+        if "epoch" in result and isinstance(result["epoch"], float):
+            # We do this here because we have to convert to a string in
+            # order to be able to write into the CSV file.
+            result["epoch"] = str(result["epoch"])
 
-    if PyFunceble.facility.ConfigLoader.is_already_loaded():
-        if PyFunceble.storage.CONFIGURATION.cli_testing.sorting_mode.hierarchical:
-            return hierarchical
-    return standard
+        return result
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/utils/stdout.py` & `PyFunceble-4.2.0/PyFunceble/cli/utils/stdout.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/utils/testing.py` & `PyFunceble-4.2.0/PyFunceble/cli/utils/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -61,22 +61,20 @@
 from PyFunceble.converter.input_line2subject import InputLine2Subject
 from PyFunceble.converter.rpz_input_line2subject import RPZInputLine2Subject
 from PyFunceble.converter.rpz_policy2subject import RPZPolicy2Subject
 from PyFunceble.converter.subject2complements import Subject2Complements
 from PyFunceble.converter.url2netloc import Url2Netloc
 from PyFunceble.converter.wildcard2subject import Wildcard2Subject
 from PyFunceble.dataset.autocontinue.csv import CSVContinueDataset
-from PyFunceble.dataset.autocontinue.mariadb import MariaDBContinueDataset
-from PyFunceble.dataset.autocontinue.mysql import MySQLContinueDataset
+from PyFunceble.dataset.autocontinue.sql import SQLDBContinueDataset
 from PyFunceble.dataset.base import DatasetBase
 from PyFunceble.dataset.csv_base import CSVDatasetBase
 from PyFunceble.dataset.db_base import DBDatasetBase
 from PyFunceble.dataset.inactive.csv import CSVInactiveDataset
-from PyFunceble.dataset.inactive.mariadb import MariaDBInactiveDataset
-from PyFunceble.dataset.inactive.mysql import MySQLInactiveDataset
+from PyFunceble.dataset.inactive.sql import SQLDBInactiveDataset
 from PyFunceble.helpers.list import ListHelper
 from PyFunceble.helpers.regex import RegexHelper
 
 
 def get_testing_mode() -> str:
     """
     Tries to provides the testing mode to apply to the CLI.
@@ -105,18 +103,20 @@
         When the given database type is unkown.
     """
 
     result = None
 
     if PyFunceble.storage.CONFIGURATION.cli_testing.db_type in "csv":
         result = CSVContinueDataset()
-    elif PyFunceble.storage.CONFIGURATION.cli_testing.db_type == "mariadb":
-        result = MariaDBContinueDataset(db_session=db_session)
-    elif PyFunceble.storage.CONFIGURATION.cli_testing.db_type == "mysql":
-        result = MySQLContinueDataset(db_session=db_session)
+    elif PyFunceble.storage.CONFIGURATION.cli_testing.db_type in (
+        "mariadb",
+        "mysql",
+        "postgresql",
+    ):
+        result = SQLDBContinueDataset(db_session=db_session)
 
     if result:
         result.set_authorized(
             bool(PyFunceble.storage.CONFIGURATION.cli_testing.autocontinue)
         )
 
         return result
@@ -140,18 +140,20 @@
         When the given database type is unkown.
     """
 
     result = None
 
     if PyFunceble.storage.CONFIGURATION.cli_testing.db_type == "csv":
         result = CSVInactiveDataset()
-    elif PyFunceble.storage.CONFIGURATION.cli_testing.db_type == "mariadb":
-        result = MariaDBInactiveDataset(db_session=db_session)
-    elif PyFunceble.storage.CONFIGURATION.cli_testing.db_type == "mysql":
-        result = MySQLInactiveDataset(db_session=db_session)
+    elif PyFunceble.storage.CONFIGURATION.cli_testing.db_type in (
+        "mariadb",
+        "mysql",
+        "postgresql",
+    ):
+        result = SQLDBInactiveDataset(db_session=db_session)
 
     if result:
         result.set_authorized(
             bool(PyFunceble.storage.CONFIGURATION.cli_testing.inactive_db)
         )
 
         return result
```

### Comparing `PyFunceble-4.1.3/PyFunceble/cli/utils/version.py` & `PyFunceble-4.2.0/PyFunceble/cli/utils/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/config/__init__.py` & `PyFunceble-4.2.0/PyFunceble/config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/config/compare.py` & `PyFunceble-4.2.0/PyFunceble/config/compare.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/config/loader.py` & `PyFunceble-4.2.0/PyFunceble/config/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -343,15 +343,14 @@
 
         if (
             not config
             or not isinstance(config, dict)
             or self.merge_upstream
             or is_3_x_version(config)
         ):  # pragma: no cover ## Testing the underlying comparison method is sufficent
-
             config = ConfigComparison(
                 local_config=config,
                 upstream_config=self.dict_helper.from_yaml_file(
                     self.path_to_default_config
                 ),
             ).get_merged()
```

### Comparing `PyFunceble-4.1.3/PyFunceble/converter/__init__.py` & `PyFunceble-4.2.0/PyFunceble/query/record/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides all the converters.
+Provides all records classes.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/converter/adblock_input_line2subject.py` & `PyFunceble-4.2.0/PyFunceble/converter/adblock_input_line2subject.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -63,23 +63,30 @@
     """
     Provides an interface for the conversion or extraction of valuable subjects
     from an inputted AdBlock line.
     """
 
     _aggressive: bool = False
 
-    __regex_helper: Optional[RegexHelper] = None
+    _regex_helper: Optional[RegexHelper] = None
 
     def __init__(
-        self, data_to_convert: Optional[Any] = None, aggressive: bool = False
+        self,
+        data_to_convert: Optional[Any] = None,
+        aggressive: bool = False,
+        *,
+        regex_helper: Optional[RegexHelper] = None,
     ) -> None:
         if aggressive is not None:
             self.aggressive = aggressive
 
-        self.__regex_helper = RegexHelper()
+        if regex_helper is None:
+            self._regex_helper = RegexHelper()
+        else:
+            self._regex_helper = regex_helper
 
         super().__init__(data_to_convert=data_to_convert)
 
     @ConverterBase.data_to_convert.setter
     def data_to_convert(self, value: Any) -> None:
         """
         Overrites the default behavior.
@@ -164,15 +171,15 @@
 
         :param decoded:
             The decoded part to split.
         """
 
         result = set()
 
-        rematch = self.__regex_helper.set_regex(r"((?:[^~\*,]+))").match(
+        rematch = self._regex_helper.set_regex(r"((?:[^~\*,]+))").match(
             decoded, rematch=True, return_match=True
         )
 
         if rematch:
             result.update({self.extract_base(x) for x in rematch})
 
         return result
@@ -197,15 +204,15 @@
             if "domain=" in rule:
                 rule = rule.replace("domain=", "").replace("|", ",")
 
                 result.update(self._decode_multiple_subject(rule))
                 continue
 
             if "href" in rule:
-                matched = self.__regex_helper.set_regex(
+                matched = self._regex_helper.set_regex(
                     r"((?:\"|\')(.*)(?:\"|\'))"
                 ).match(rule, return_match=True, rematch=True, group=1)
 
                 if matched:
                     result.add(self.extract_base(matched))
                 continue
 
@@ -265,27 +272,29 @@
             local_line = local_line.replace("|", "", 1)
             local_line = "".join(local_line.rsplit("|", 1))
 
             result.add(self.extract_base(local_line))
 
         return {x for x in result if "." in x}
 
-    def _decode_v3(self, line: str) -> Set[str]:
+    def _decode_v3(self, line: str, *, aggressive: bool = False) -> Set[str]:
         """
         Implementation of our third decoding mode.
 
         In this mode, we try to decode the simple:
 
             ||ads.example.com^$script,image,domain=example.com|~foo.example.info
             ||ads.example.com$script,image,domain=example.com|~foo.example.info
 
         rule.
 
         :param line:
             The line to decode.
+        :param aggressive:
+            Whether we should aggressively extract datasets.
         """
 
         result = set()
 
         local_line = line.strip()
 
         if not local_line.startswith("||"):
@@ -295,42 +304,44 @@
             v1_mode, options = local_line.split("$", 1)
 
             if not v1_mode.endswith("^"):
                 v1_mode += "^"
 
             result.update(self._decode_v1(v1_mode))
 
-            if self.aggressive:
+            if aggressive:
                 result.update(self._decode_options(options.split(",")))
         elif "^" not in local_line:
             result.update(self._decode_v1(f"{local_line}^"))
         else:
             result.update(self._decode_v1(local_line[: local_line.find("^") + 1]))
 
         return {x for x in result if "." in x}
 
-    def _decode_v4(self, line: str) -> Set[str]:
+    def _decode_v4(self, line: str, *, aggressive: bool = False) -> Set[str]:
         """
         Implementation of our fourth decoding mode.
 
         In this mode, we try to decode the simple:
 
             @@||ads.example.com/notbanner^$~script
 
         rule.
 
         :param line:
             The line to decode.
+        :param aggressive:
+            Whether we should aggressively extract datasets.
         """
 
         result = set()
         local_line = line.strip()
 
         if (
-            not self.aggressive
+            not aggressive
             or not local_line.startswith("@@||")
             or "^$" not in local_line
         ):
             return result
 
         v1_mode, options = local_line.split("$", 1)
 
@@ -338,35 +349,37 @@
             {self.extract_base(x) for x in self._decode_v1(v1_mode.replace("@@", ""))}
         )
 
         result.update(self._decode_options(options.split(",")))
 
         return {x for x in result if "." in x}
 
-    def _decode_v5(self, line: str) -> Set[str]:
+    def _decode_v5(self, line: str, *, aggressive: bool = False) -> Set[str]:
         """
         Implementation of our fifth decoding mode.
 
         In this mode, we try to decode the simple:
 
             example.com,example.net##.advert
             exception.example.com#@#.advert
             example.com,example.net#?#div:-abp-has(> div > img.advert)
             exception.example.com#@#div:-abp-has(> div > img.advert)
 
         rule.
 
         :param line:
             The line to decode.
+        :param aggressive:
+            Whether we should aggressively extract datasets.
         """
 
         local_line = line.strip()
         result = set()
 
-        if not self.aggressive:
+        if not aggressive:
             return result
 
         separators = ["##", "#@#", "#?#"]
 
         obj_of_interest, options = "", ""
 
         for separator in separators:
@@ -375,33 +388,35 @@
                 break
 
         result.update(self._decode_multiple_subject(obj_of_interest))
         result.update(self._decode_options(options.split(",")))
 
         return {x for x in result if "." in x}
 
-    def _decode_v6(self, line: str) -> Set[str]:
+    def _decode_v6(self, line: str, *, aggressive: bool = False) -> Set[str]:
         """
         Implementation of our sixth decoding mode.
 
         In this mode we try to decode the simple:
 
             $domain=exam.pl|elpmaxe.pl|example.pl
             ^hello^$domain=example.com
 
         rule.
 
         :param line:
             The line to decode.
+        :param aggressive:
+            Whether we should aggressively extract datasets.
         """
 
         local_line = line.strip()
         result = set()
 
-        if not self.aggressive:
+        if not aggressive:
             return result
 
         separators = ["$"]
 
         for separator in separators:
             if separator not in line:
                 continue
@@ -413,19 +428,31 @@
         return {x for x in result if "." in x}
 
     def get_converted(self) -> List[str]:
         """
         Provides the converted data.
         """
 
+        return self.convert(self.data_to_convert, aggressive=self.aggressive)
+
+    def convert(self, data: Any, *, aggressive: bool = False) -> List[str]:
+        """
+        Converts the given dataset.
+
+        :param data:
+            The data to convert.
+        :param aggressive:
+            Whether we should aggressively extract datasets.
+        """
+
         result = set()
 
-        if not self.should_be_ignored(self.data_to_convert.strip()):
-            result.update(self._decode_v1(self.data_to_convert))
-            result.update(self._decode_v2(self.data_to_convert))
-            result.update(self._decode_v3(self.data_to_convert))
-            result.update(self._decode_v5(self.data_to_convert))
-            result.update(self._decode_v6(self.data_to_convert))
+        if not self.should_be_ignored(data.strip()):
+            result.update(self._decode_v1(data))
+            result.update(self._decode_v2(data))
+            result.update(self._decode_v3(data, aggressive=aggressive))
+            result.update(self._decode_v5(data, aggressive=aggressive))
+            result.update(self._decode_v6(data, aggressive=aggressive))
 
-        result.update(self._decode_v4(self.data_to_convert))
+        result.update(self._decode_v4(data, aggressive=aggressive))
 
         return ListHelper(list(result)).sort().subject
```

### Comparing `PyFunceble-4.1.3/PyFunceble/converter/base.py` & `PyFunceble-4.2.0/PyFunceble/converter/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -97,7 +97,14 @@
 
     def get_converted(self) -> Optional[Any]:
         """
         Provides the converted data.
         """
 
         raise NotImplementedError()
+
+    def convert(self, data: Any) -> Optional[Any]:
+        """
+        Converts the given dataset.
+        """
+
+        raise NotImplementedError()
```

### Comparing `PyFunceble-4.1.3/PyFunceble/converter/cidr2subject.py` & `PyFunceble-4.2.0/PyFunceble/converter/cidr2subject.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -61,18 +61,26 @@
 class CIDR2Subject(ConverterBase):
     """
     Converts/Extracts the subjects of from the given CIDR.
     """
 
     ip_syntax_checker: Optional[IPSyntaxChecker] = None
 
-    def __init__(self, data_to_convert: Optional[Any] = None) -> None:
+    def __init__(
+        self,
+        data_to_convert: Optional[Any] = None,
+        *,
+        ip_syntax_checker: Optional[IPSyntaxChecker] = None,
+    ) -> None:
         super().__init__(data_to_convert=data_to_convert)
 
-        self.ip_syntax_checker = IPSyntaxChecker()
+        if ip_syntax_checker is None:
+            self.ip_syntax_checker = IPSyntaxChecker()
+        else:
+            self.ip_syntax_checker = ip_syntax_checker
 
     @ConverterBase.data_to_convert.setter
     def data_to_convert(self, value: Any) -> None:
         """
         Overrites the default behavior.
 
         :raise TypeError:
@@ -86,17 +94,27 @@
         super(CIDR2Subject, self.__class__).data_to_convert.fset(self, value)
 
     def get_converted(self) -> List[str]:
         """
         Provides the subject-s to test.
         """
 
+        return self.convert(self.data_to_convert)
+
+    def convert(self, data: Any) -> List[str]:
+        """
+        Converts the given dataset.
+
+        :param data:
+            The data to convert.
+        """
+
         result = set()
 
-        subject = self.data_to_convert.strip()
+        subject = data.strip()
 
         if subject:
             try:
                 self.ip_syntax_checker.set_subject(subject)
                 if self.ip_syntax_checker.is_valid_v4_range():
                     result.update(
                         str(x) for x in IPv4Network(self.ip_syntax_checker.subject)
```

### Comparing `PyFunceble-4.1.3/PyFunceble/converter/input_line2subject.py` & `PyFunceble-4.2.0/PyFunceble/converter/input_line2subject.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -84,17 +84,27 @@
         super(InputLine2Subject, self.__class__).data_to_convert.fset(self, value)
 
     def get_converted(self) -> List[str]:
         """
         Provides the subject to test.
         """
 
+        return self.convert(self.data_to_convert)
+
+    def convert(self, data: Any) -> List[str]:
+        """
+        Converts the given dataset.
+
+        :param data:
+            The data to convert.
+        """
+
         result = []
 
-        subject = self.data_to_convert.strip()
+        subject = data.strip()
 
         if subject and (
             not subject.startswith(self.COMMENT)
             and any(not subject.startswith(x) for x in self.PARTICULAR_COMMENT)
         ):
             if self.COMMENT in subject:
                 subject = subject[: subject.find(self.COMMENT)].strip()
```

### Comparing `PyFunceble-4.1.3/PyFunceble/converter/internal_url.py` & `PyFunceble-4.2.0/PyFunceble/converter/internal_url.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -83,10 +83,20 @@
         super(InternalUrlConverter, self.__class__).data_to_convert.fset(self, value)
 
     def get_converted(self) -> str:
         """
         Provides the converted data (after conversion)
         """
 
+        return self.convert(self.data_to_convert)
+
+    def convert(self, data: Any) -> str:
+        """
+        Converts the given dataset.
+
+        :param data:
+            The data to convert.
+        """
+
         if VersionUtility(PyFunceble.storage.PROJECT_VERSION).is_dev():
-            return self.data_to_convert.replace("master", "dev")
-        return self.data_to_convert.replace("dev", "master")
+            return data.replace("master", "dev")
+        return data.replace("dev", "master")
```

### Comparing `PyFunceble-4.1.3/PyFunceble/converter/rpz_input_line2subject.py` & `PyFunceble-4.2.0/PyFunceble/converter/rpz_input_line2subject.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -48,15 +48,15 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 # pylint: enable=line-too-long
 
-from typing import List
+from typing import Any, List
 
 from PyFunceble.converter.input_line2subject import InputLine2Subject
 
 
 class RPZInputLine2Subject(InputLine2Subject):
     """
     Converts/Extracts the subject from the given RPZ inputline.
@@ -66,16 +66,26 @@
     SPECIAL: list = ["$", "@"]
 
     def get_converted(self) -> List[str]:
         """
         Provides the converted data.
         """
 
+        return self.convert(self.data_to_convert)
+
+    def convert(self, data: Any) -> List[str]:
+        """
+        Converts the given dataset.
+
+        :param data:
+            The data to convert.
+        """
+
         result = []
-        subject = self.data_to_convert.strip()
+        subject = data.strip()
 
         if (
             subject
             and not any(subject.startswith(x) for x in self.COMMENT)
             and not any(subject.startswith(x) for x in self.SPECIAL)
         ):
             for comment_sign in self.COMMENT:
```

### Comparing `PyFunceble-4.1.3/PyFunceble/converter/rpz_policy2subject.py` & `PyFunceble-4.2.0/PyFunceble/converter/rpz_policy2subject.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -64,28 +64,35 @@
     """
 
     CLEANUP_MARKERS: list = [".rpz-nsdname"]
     IP_MARKERS: list = [".rpz-client-ip", ".rpz-ip", ".rpz-nsip"]
 
     _soa: Optional[str] = None
     _soas: List[str] = []
+    wilcard2subject: Optional[Wildcard2Subject] = None
 
     def __init__(
         self,
         data_to_convert: Optional[Any] = None,
         soas: Optional[List[str]] = None,
         soa: Optional[str] = None,
+        *,
+        wildcard2subject: Optional[Wildcard2Subject] = None,
     ) -> None:
-
         if soas is not None:
             self.soas = soas
 
         if soa is not None:
             self.soa = soa
 
+        if wildcard2subject is not None:
+            self.wilcard2subject = wildcard2subject
+        else:
+            self.wilcard2subject = Wildcard2Subject()
+
         super().__init__(data_to_convert=data_to_convert)
 
     @property
     def soa(self) -> Optional[str]:
         """
         Provides the currently set SOA.
         """
@@ -253,26 +260,36 @@
         return result
 
     def get_converted(self) -> Optional[str]:
         """
         Provides the converted data.
         """
 
-        subject = self.data_to_convert.strip()
+        return self.convert(self.data_to_convert)
+
+    def convert(self, data: Any) -> Optional[str]:
+        """
+        Converts the given dataset.
+
+        :param data:
+            The data to convert.
+        """
+
+        subject = data.strip()
 
         if (
             subject
             and not any(subject.startswith(x) for x in self.COMMENT)
             and not any(subject.startswith(x) for x in self.SPECIAL)
         ):
             for comment_sign in self.COMMENT:
                 if comment_sign in subject:
                     subject = self.remove_marker(subject, comment_sign).strip()
 
-            subject = Wildcard2Subject(subject).get_converted()
+            subject = self.wilcard2subject.convert(subject)
 
             if self._soas:
                 for soa in self._soas:
                     subject = self.remove_marker(subject, f".{soa}")
                     subject = self.remove_marker(subject, soa)
 
             found_cleanup_marker = self.get_matching_cleanup_marker(subject)
```

### Comparing `PyFunceble-4.1.3/PyFunceble/converter/subject2complements.py` & `PyFunceble-4.2.0/PyFunceble/converter/subject2complements.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -126,20 +126,30 @@
         return self
 
     def get_converted(self) -> List[str]:
         """
         Provides the converted data.
         """
 
+        return self.convert(self.data_to_convert)
+
+    def convert(self, data: Any) -> List[str]:
+        """
+        Converts the given dataset.
+
+        :param data:
+            The data to convert.
+        """
+
         result = []
 
-        checker = DomainSyntaxChecker(self.data_to_convert)
+        checker = DomainSyntaxChecker(data)
 
-        if self.include_given and self.data_to_convert not in result:
-            result.append(self.data_to_convert)
+        if self.include_given and data not in result:
+            result.append(data)
 
-        if self.data_to_convert.startswith("www."):
-            result.append(self.data_to_convert[4:])
+        if data.startswith("www."):
+            result.append(data[4:])
         elif checker.is_valid_second_level():
-            result.append(f"www.{self.data_to_convert}")
+            result.append(f"www.{data}")
 
         return result
```

### Comparing `PyFunceble-4.1.3/PyFunceble/converter/url2netloc.py` & `PyFunceble-4.2.0/PyFunceble/query/whois/converter/month2unified.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides a way to convert/extract the network location of a given URL.
+Provides a way to convert a given month to our unified format.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,75 +31,76 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-import urllib.parse
-from typing import Any
+from typing import Any, Dict, List
 
-from PyFunceble.converter.base import ConverterBase
+from PyFunceble.query.whois.converter.base import ConverterBase
 
 
-class Url2Netloc(ConverterBase):
+class Month2Unified(ConverterBase):
     """
-    Provides the interface for the conversion/extration of the network location
-    of a given URL.
+    Converts the given month into our unified format.
     """
 
+    MAP: Dict[str, List[str]] = {
+        "jan": [str(1), "01", "jan", "january", "jan."],
+        "feb": [str(2), "02", "feb", "february", "feb."],
+        "mar": [str(3), "03", "mar", "march", "mar."],
+        "apr": [str(4), "04", "apr", "april", "apr."],
+        "may": [str(5), "05", "may"],
+        "jun": [str(6), "06", "jun", "june", "jun."],
+        "jul": [str(7), "07", "jul", "july", "jul."],
+        "aug": [str(8), "08", "aug", "august", "aug."],
+        "sep": [str(9), "09", "sep", "september", "sep.", "sept", "sept."],
+        "oct": [str(10), "oct", "october", "oct."],
+        "nov": [str(11), "nov", "november", "nov."],
+        "dec": [str(12), "dec", "december", "dec."],
+    }
+
     @ConverterBase.data_to_convert.setter
     def data_to_convert(self, value: Any) -> None:
         """
         Overrites the default behavior.
 
         :raise TypeError:
             When the given data to convert is not :py:class:`str`
-        :raise ValueError:
-            When the given data to convert is empty.
         """
 
         if not isinstance(value, str):
             raise TypeError(f"<value> should be {str}, {type(value)} given.")
 
-        if not value:
-            raise ValueError("<value> should not be empty.")
-
         # pylint: disable=no-member
-        super(Url2Netloc, self.__class__).data_to_convert.fset(self, value)
+        super(Month2Unified, self.__class__).data_to_convert.fset(self, value)
 
+    @ConverterBase.ensure_data_to_convert_is_given
     def get_converted(self) -> str:
         """
         Provides the converted data (after conversion)
-        """
 
-        parsed_url = urllib.parse.urlparse(self.data_to_convert)
-
-        if not parsed_url.netloc and parsed_url.path:
-            netloc = parsed_url.path
-        elif parsed_url.netloc:
-            netloc = parsed_url.netloc
-        else:  # pragma: no cover ## Safety
-            netloc = self.data_to_convert
-
-        if "//" in netloc:
-            netloc = netloc[netloc.find("//") + 2 :]
+        .. warning::
+            If no month is found, the given data is given as response.
+        """
 
-        if "/" in netloc:
-            netloc = netloc[: netloc.find("/")]
+        for to_return, possibilities in self.MAP.items():
+            if self.data_to_convert.lower() in possibilities:
+                return to_return
 
-        return netloc
+        return self.data_to_convert
```

### Comparing `PyFunceble-4.1.3/PyFunceble/converter/wildcard2subject.py` & `PyFunceble-4.2.0/PyFunceble/converter/wildcard2subject.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -80,15 +80,25 @@
         super(Wildcard2Subject, self.__class__).data_to_convert.fset(self, value)
 
     def get_converted(self) -> str:
         """
         Provides the converted data.
         """
 
-        subject = self.data_to_convert.strip()
+        return self.convert(self.data_to_convert)
+
+    def convert(self, data: Any) -> str:
+        """
+        Converts the given dataset.
+
+        :param data:
+            The data to convert.
+        """
+
+        subject = data.strip()
 
         if not subject:
             return None
 
         if subject.startswith(self.WILDCARD):
             return subject[2:]
```

### Comparing `PyFunceble-4.1.3/PyFunceble/data/alembic/__init__.py` & `PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/data/alembic/env.py` & `PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -53,16 +53,16 @@
 # pylint: skip-file
 # flake8: noqa
 
 from alembic import context
 from sqlalchemy import engine_from_config, pool
 
 import PyFunceble.cli.facility
+import PyFunceble.database.sqlalchemy.all_schemas
 import PyFunceble.facility
-from PyFunceble.database.sqlalchemy.all_schemas import Continue, Inactive, WhoisRecord
 from PyFunceble.database.sqlalchemy.base_schema import SchemaBase
 
 config = context.config
 target_metadata = SchemaBase.metadata
 
 if not PyFunceble.facility.ConfigLoader.is_already_loaded():
     # We load the configuration because we don't want to manually give
```

### Comparing `PyFunceble-4.1.3/PyFunceble/data/alembic/versions/35c79626ecb9_fix_some_columns.py` & `PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/35c79626ecb9_fix_some_columns.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-4.1.3/PyFunceble/data/alembic/versions/3a4c55a9320d_add_continue_table.py` & `PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/3a4c55a9320d_add_continue_table.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-4.1.3/PyFunceble/data/alembic/versions/3d6f4a33cdb2_add_inactive_table.py` & `PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/3d6f4a33cdb2_add_inactive_table.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-4.1.3/PyFunceble/data/alembic/versions/45713fea8097_deletion_uneeded_columns_from_whois_.py` & `PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/45713fea8097_deletion_uneeded_columns_from_whois_.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-4.1.3/PyFunceble/data/alembic/versions/459a0d7b8f09_add_idna_subject_column_into_whois.py` & `PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/459a0d7b8f09_add_idna_subject_column_into_whois.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-4.1.3/PyFunceble/data/alembic/versions/6f4729deaf03_delete_inactive_source_column.py` & `PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/6f4729deaf03_delete_inactive_source_column.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-4.1.3/PyFunceble/data/alembic/versions/7bcf7fa64ba1_rename_created_to_created_at_and.py` & `PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/7bcf7fa64ba1_rename_created_to_created_at_and.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-4.1.3/PyFunceble/data/alembic/versions/83ada95132bf_delete_the_file_table.py` & `PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/83ada95132bf_delete_the_file_table.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-4.1.3/PyFunceble/data/alembic/versions/912bbcb77a6c_add_registrar_column.py` & `PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/912bbcb77a6c_add_registrar_column.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-4.1.3/PyFunceble/data/alembic/versions/95dc17ddd729_introduction_of_the_session_id_column.py` & `PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/95dc17ddd729_introduction_of_the_session_id_column.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-4.1.3/PyFunceble/data/alembic/versions/__init__.py` & `PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/data/alembic/versions/ade87195b0a0_base.py` & `PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/ade87195b0a0_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-4.1.3/PyFunceble/data/alembic/versions/bef7bcaac3f2_make_id_a_bigint.py` & `PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/bef7bcaac3f2_make_id_a_bigint.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-4.1.3/PyFunceble/data/alembic/versions/d8893cd406db_allow_whois_record_to_be_empty_null.py` & `PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/d8893cd406db_allow_whois_record_to_be_empty_null.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-4.1.3/PyFunceble/data/alembic/versions/e04e8301d1a2_deletion_of_the_mined_table.py` & `PyFunceble-4.2.0/PyFunceble/data/alembic/mysql/versions/e04e8301d1a2_deletion_of_the_mined_table.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-4.1.3/PyFunceble/data/infrastructure/.PyFunceble_production.yaml` & `PyFunceble-4.2.0/PyFunceble/data/infrastructure/.PyFunceble_production.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
   # Activates the expansion of CIDR to single addresses.
   cidr_expand: False
 
   # Sets the cooldown time to apply between each tests.
   cooldown_time: 0.0
 
   # Sets the Database Connector type to use.
-  # Available: csv | mariadb | mysql
+  # Available: csv | mariadb | mysql | postgresql
   db_type: csv
 
   # Sets the filter to apply while reading the given input.
   # For example, if you give `\.info`, we will only test the subjects who match
   # `\.info`.
   file_filter: null
 
@@ -280,17 +280,14 @@
   delay: 0.0
 
 # Not Implemented yet. Reserved for future usage and implementation.
 share_logs: False
 
 user_agent:
   # Provides everything related to the user agent choice.
-  # Note:
-  #   Please report to https://git.io/JLWe5 for more insight about the
-  #   browser and platform available..
 
   browser: chrome
   platform: linux
 
   # Sets the user agent to use.
   # WARNING: If given, this will be used systematically.
   custom: null
```

### Comparing `PyFunceble-4.1.3/PyFunceble/data/infrastructure/dir_structure_production.json` & `PyFunceble-4.2.0/PyFunceble/data/infrastructure/dir_structure_production.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7586206896551724%*

 * *Differences: {"'ips'": "OrderedDict([('.gitignore', OrderedDict([('content', "*

 * *          "'*\\n!.gitignore\\n!/ACTIVE/\\n!/INACTIVE/\\n!/INVALID/\\n!/MALICIOUS/\\n!/SANE/\\n!/VALID/\\n'), "*

 * *          "('hash', 'a273966a13322ad4da9fbad4bd7247ca046de503de543c6f909e5e2b')]))])",*

 * * "'ips/ACTIVE'": "OrderedDict([('.gitignore', OrderedDict([('content', '*\\n!.gitignore\\n'), "*

 * *                 "('hash', '0bd551cb904befcee06b7a99ef7ac54dba91ee21b5944c78759c1e4b')]))])",*

 * * "'ips/INACTIVE'": "OrderedDict([('.gitignore', OrderedDic […]*

```diff
@@ -109,14 +109,56 @@
     },
     "hosts/VALID": {
         ".gitignore": {
             "content": "*\n!.gitignore\n",
             "hash": "0bd551cb904befcee06b7a99ef7ac54dba91ee21b5944c78759c1e4b"
         }
     },
+    "ips": {
+        ".gitignore": {
+            "content": "*\n!.gitignore\n!/ACTIVE/\n!/INACTIVE/\n!/INVALID/\n!/MALICIOUS/\n!/SANE/\n!/VALID/\n",
+            "hash": "a273966a13322ad4da9fbad4bd7247ca046de503de543c6f909e5e2b"
+        }
+    },
+    "ips/ACTIVE": {
+        ".gitignore": {
+            "content": "*\n!.gitignore\n",
+            "hash": "0bd551cb904befcee06b7a99ef7ac54dba91ee21b5944c78759c1e4b"
+        }
+    },
+    "ips/INACTIVE": {
+        ".gitignore": {
+            "content": "*\n!.gitignore\n",
+            "hash": "0bd551cb904befcee06b7a99ef7ac54dba91ee21b5944c78759c1e4b"
+        }
+    },
+    "ips/INVALID": {
+        ".gitignore": {
+            "content": "*\n!.gitignore\n",
+            "hash": "0bd551cb904befcee06b7a99ef7ac54dba91ee21b5944c78759c1e4b"
+        }
+    },
+    "ips/MALICIOUS": {
+        ".gitignore": {
+            "content": "*\n!.gitignore\n",
+            "hash": "0bd551cb904befcee06b7a99ef7ac54dba91ee21b5944c78759c1e4b"
+        }
+    },
+    "ips/SANE": {
+        ".gitignore": {
+            "content": "*\n!.gitignore\n",
+            "hash": "0bd551cb904befcee06b7a99ef7ac54dba91ee21b5944c78759c1e4b"
+        }
+    },
+    "ips/VALID": {
+        ".gitignore": {
+            "content": "*\n!.gitignore\n",
+            "hash": "0bd551cb904befcee06b7a99ef7ac54dba91ee21b5944c78759c1e4b"
+        }
+    },
     "logs": {
         ".gitignore": {
             "content": "*\n!.gitignore\n!/date_format/\n!/no_referrer/\n!/percentage/\n!/whois/\n",
             "hash": "7e533b26a45b8712a1ed4895b52b2cc798a03a632074800af98a52e7"
         }
     },
     "logs/percentage": {
```

### Comparing `PyFunceble-4.1.3/PyFunceble/database/__init__.py` & `PyFunceble-4.2.0/PyFunceble/database/sqlalchemy/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides everything related to the structure and connection with external databases.
+Provides everything related to everything we do with SQLAlchemy.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/database/credential/__init__.py` & `PyFunceble-4.2.0/PyFunceble/downloader/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides everything related to our credential holders.
+Provides all downloaders.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/database/credential/mariadb.py` & `PyFunceble-4.2.0/PyFunceble/database/credential/mariadb.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/database/credential/mysql.py` & `PyFunceble-4.2.0/PyFunceble/database/credential/mysql.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/database/schemas/__init__.py` & `PyFunceble-4.2.0/PyFunceble/database/schemas/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/database/schemas/autocontinue.py` & `PyFunceble-4.2.0/PyFunceble/database/schemas/autocontinue.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/database/schemas/inactive.py` & `PyFunceble-4.2.0/PyFunceble/database/schemas/inactive.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/database/schemas/status.py` & `PyFunceble-4.2.0/PyFunceble/database/schemas/status.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/database/schemas/whois_record.py` & `PyFunceble-4.2.0/PyFunceble/database/schemas/whois_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/database/session.py` & `PyFunceble-4.2.0/PyFunceble/database/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/database/sqlalchemy/__init__.py` & `PyFunceble-4.2.0/PyFunceble/dataset/whois/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides everything related to everything we do with SQLAlchemy.
+Provides everything related to the whois database logic(s).
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/database/sqlalchemy/all_schemas.py` & `PyFunceble-4.2.0/PyFunceble/database/sqlalchemy/all_schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/database/sqlalchemy/base_schema.py` & `PyFunceble-4.2.0/PyFunceble/database/sqlalchemy/base_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/dataset/__init__.py` & `PyFunceble-4.2.0/PyFunceble/cli/continuous_integration/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides all the dataset interaction submodules
+Provides everything we may need for continuous integration aka autosaving and
+auto commiting.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/dataset/autocontinue/__init__.py` & `PyFunceble-4.2.0/PyFunceble/dataset/autocontinue/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/dataset/autocontinue/base.py` & `PyFunceble-4.2.0/PyFunceble/dataset/autocontinue/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/dataset/autocontinue/csv.py` & `PyFunceble-4.2.0/PyFunceble/dataset/autocontinue/csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -105,15 +105,14 @@
     def update_source_file_afterwards(func):  # pylint: disable=no-self-argument
         """
         Updates the source file before launching the decorated method.
         """
 
         @functools.wraps(func)
         def wrapper(self, *args, **kwargs):
-
             result = func(self, *args, **kwargs)  # pylint: disable=not-callable
 
             self.source_file = os.path.join(
                 self.base_directory, PyFunceble.cli.storage.AUTOCONTINUE_FILE
             )
 
             return result
```

### Comparing `PyFunceble-4.1.3/PyFunceble/dataset/autocontinue/mariadb.py` & `PyFunceble-4.2.0/PyFunceble/dataset/autocontinue/sql.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -53,28 +53,28 @@
 from datetime import datetime, timedelta
 from typing import Generator, Tuple
 
 import PyFunceble.cli.factory
 import PyFunceble.sessions
 from PyFunceble.database.sqlalchemy.all_schemas import Continue
 from PyFunceble.dataset.autocontinue.base import ContinueDatasetBase
-from PyFunceble.dataset.mariadb_base import MariaDBDatasetBase
+from PyFunceble.dataset.sql_base import SQLDBDatasetBase
 
 
-class MariaDBContinueDataset(MariaDBDatasetBase, ContinueDatasetBase):
+class SQLDBContinueDataset(SQLDBDatasetBase, ContinueDatasetBase):
     """
     Provides the interface for the management and the Continue dataset unser
     mariadb.
     """
 
     ORM_OBJ: Continue = Continue
 
-    @MariaDBDatasetBase.execute_if_authorized(None)
+    @SQLDBDatasetBase.execute_if_authorized(None)
     # pylint: disable=arguments-differ
-    def cleanup(self, *, session_id: str) -> "MariaDBContinueDataset":
+    def cleanup(self, *, session_id: str) -> "SQLDBContinueDataset":
         """
         Cleanups the dataset. Meaning that we delete every entries which are
         needed anymore.
 
         :param source:
             The source to delete.
         :param session_id:
@@ -88,15 +88,15 @@
 
         PyFunceble.facility.Logger.debug(
             "Deleted data related to %s (session_id", session_id
         )
 
         return self
 
-    @MariaDBDatasetBase.execute_if_authorized(None)
+    @SQLDBDatasetBase.execute_if_authorized(None)
     def get_to_test(self, session_id: str) -> Generator[Tuple[str], str, None]:
         twenty_years_ago = datetime.utcnow() - timedelta(days=365.25 * 20)
 
         result = (
             self.db_session.query(self.ORM_OBJ)
             .filter(self.ORM_OBJ.session_id == session_id)
             .filter(self.ORM_OBJ.tested_at < twenty_years_ago)
```

### Comparing `PyFunceble-4.1.3/PyFunceble/dataset/autocontinue/mysql.py` & `PyFunceble-4.2.0/PyFunceble/cli/utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the interface for the continue MySQL management.
+Provides some utilities related to the CLI.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,30 +31,21 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
-
-from PyFunceble.dataset.autocontinue.mariadb import MariaDBContinueDataset
-
-
-class MySQLContinueDataset(MariaDBContinueDataset):
-    """
-    Provides the interface for the management and the Continue dataset under
-    mysql.
-    """
```

### Comparing `PyFunceble-4.1.3/PyFunceble/dataset/base.py` & `PyFunceble-4.2.0/PyFunceble/dataset/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/dataset/csv_base.py` & `PyFunceble-4.2.0/PyFunceble/dataset/csv_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/dataset/db_base.py` & `PyFunceble-4.2.0/PyFunceble/dataset/db_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/dataset/iana.py` & `PyFunceble-4.2.0/PyFunceble/dataset/iana.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/dataset/inactive/__init__.py` & `PyFunceble-4.2.0/PyFunceble/helpers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides everything related to the inactive database logic(s).
+Provides the helpers.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/dataset/inactive/base.py` & `PyFunceble-4.2.0/PyFunceble/dataset/inactive/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/dataset/inactive/csv.py` & `PyFunceble-4.2.0/PyFunceble/dataset/inactive/csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -73,15 +73,14 @@
 
         return super().__post_init__()
 
     @CSVDatasetBase.execute_if_authorized(None)
     def get_to_retest(
         self, destination: str, checker_type: str, *, min_days: Optional[int]
     ) -> Generator[Tuple[str, str, Optional[int]], dict, None]:
-
         days_ago = datetime.utcnow() - timedelta(days=min_days)
 
         for dataset in self.get_filtered_content(
             {"destination": destination, "checker_type": checker_type}
         ):
             if not isinstance(dataset["tested_at"], datetime):
                 try:
```

### Comparing `PyFunceble-4.1.3/PyFunceble/dataset/inactive/mariadb.py` & `PyFunceble-4.2.0/PyFunceble/dataset/inactive/sql.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -51,31 +51,30 @@
 """
 
 from datetime import datetime, timedelta
 from typing import Generator, Optional, Tuple
 
 from PyFunceble.database.sqlalchemy.all_schemas import Inactive
 from PyFunceble.dataset.inactive.base import InactiveDatasetBase
-from PyFunceble.dataset.mariadb_base import MariaDBDatasetBase
+from PyFunceble.dataset.sql_base import SQLDBDatasetBase
 
 
-class MariaDBInactiveDataset(MariaDBDatasetBase, InactiveDatasetBase):
+class SQLDBInactiveDataset(SQLDBDatasetBase, InactiveDatasetBase):
     """
     Provides tht interface for the management and the WHOIS dataset under
     mariadb.
     """
 
     ORM_OBJ: Inactive = Inactive
 
-    @MariaDBDatasetBase.execute_if_authorized(None)
-    @MariaDBDatasetBase.ensure_orm_obj_is_given
+    @SQLDBDatasetBase.execute_if_authorized(None)
+    @SQLDBDatasetBase.ensure_orm_obj_is_given
     def get_to_retest(
         self, destination: str, checker_type: str, *, min_days: Optional[int]
     ) -> Generator[Tuple[str, str, Optional[int]], dict, None]:
-
         days_ago = datetime.utcnow() - timedelta(days=min_days)
 
         result = (
             self.db_session.query(self.ORM_OBJ)
             .filter(self.ORM_OBJ.destination == destination)
             .filter(self.ORM_OBJ.checker_type == checker_type)
             .filter(self.ORM_OBJ.tested_at < days_ago)
```

### Comparing `PyFunceble-4.1.3/PyFunceble/dataset/inactive/mysql.py` & `PyFunceble-4.2.0/PyFunceble/query/record/whois.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the interface for the inactive DB (mysql) management.
+Provides the record class of the whois query tool.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,30 +31,44 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-from PyFunceble.dataset.inactive.mariadb import MariaDBInactiveDataset
+import dataclasses
+from typing import Optional
 
+from PyFunceble.query.record.base import RecordBase
 
-class MySQLInactiveDataset(MariaDBInactiveDataset):
+
+@dataclasses.dataclass
+class WhoisQueryToolRecord(RecordBase):
     """
-    Provides tht interface for the management and the WHOIS dataset under
-    mysql.
+    Provides a record of an executed request.
     """
+
+    server: Optional[str] = None
+    port: Optional[str] = None
+
+    query_timeout: Optional[float] = None
+
+    subject: Optional[str] = None
+
+    record: Optional[str] = None
+    expiration_date: Optional[str] = None
+    registrar: Optional[str] = None
```

### Comparing `PyFunceble-4.1.3/PyFunceble/dataset/ipv4_reputation.py` & `PyFunceble-4.2.0/PyFunceble/query/netinfo/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides an interface which let us interact with the IPv4 reputation database.
+Provides the base of all checker.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,75 +31,106 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-import os
+import functools
 from typing import Any, Optional
 
-import PyFunceble.storage
-from PyFunceble.dataset.base import DatasetBase
-from PyFunceble.downloader.ipv4_reputation import IPV4ReputationDownloader
-from PyFunceble.helpers.file import FileHelper
 
-
-class IPV4ReputationDataset(DatasetBase):
+class NetInfoBase:
     """
-    Provides the interface for the lookup of the IPv4 reputation.
+    Provides the base of network information classes.
     """
 
-    STORAGE_INDEX: Optional[str] = None
-    DOWNLOADER: IPV4ReputationDownloader = IPV4ReputationDownloader()
+    _subject: Optional[str] = None
+    base: Optional[str] = None
+
+    def __init__(self, subject: Optional[str] = None) -> None:
+        if subject is not None:
+            self.subject = subject
+
+    def ensure_subject_is_given(func):  # pylint: disable=no-self-argument
+        """
+        Ensures that the subject is given before running the decorated method.
+
+        :raise TypeError:
+            If the subject is not a string.
+        """
 
-    def __init__(self) -> None:
-        self.source_file = os.path.join(
-            PyFunceble.storage.CONFIG_DIRECTORY,
-            PyFunceble.storage.IPV4_REPUTATION_FILENAME,
-        )
+        @functools.wraps(func)
+        def wrapper(self, *args, **kwargs):
+            if not isinstance(self.subject, str):
+                raise TypeError(
+                    f"<self.subject> should be {str}, {type(self.subject)} given."
+                )
 
-    def __contains__(self, value: Any) -> bool:
-        with self.get_content() as file_stream:
-            for line in file_stream:
-                line = line.strip()
+            return func(self, *args, **kwargs)  # pylint: disable=not-callable
 
-                if line.startswith(f"{value}#"):
-                    return True
+        return wrapper
 
-        return False
+    @property
+    def subject(self) -> Optional[str]:
+        """
+        Provides the current state of the :code:`_subject` attribute.
+        """
 
-    @DatasetBase.ensure_source_file_exists
-    def get_content(self) -> open:
+        return self._subject
+
+    @subject.setter
+    def subject(self, value: str) -> None:
         """
-        Provides a file handler which does let you read the content line by
-        line.
+        Sets the subject to work with.
+
+        :param value:
+            The subject to set.
 
-        :raise FileNotFoundError:
-            When the declared file does not exists.
+        :raise TypeError:
+            When the given :code:`value` is not a :py:class:`str`.
+        :raise ValueError:
+            When the given :code:`value` is empty.
         """
 
-        file_helper = FileHelper(self.source_file)
+        if not isinstance(value, str):
+            raise TypeError(f"<value> should be {str}, {type(value)} given.")
 
-        if not file_helper.exists() and bool(self.DOWNLOADER):  # pragma: no cover
-            ## pragma reason: Safety.
-            self.DOWNLOADER.start()
+        if not value:
+            raise ValueError("<value> should not be empty.")
 
-            if not file_helper.exists():
-                raise FileNotFoundError(file_helper.path)
+        self._subject = value
+
+    def set_subject(self, value: str) -> "NetInfoBase":
+        """
+        Sets the subject to work with.
+
+        :param value:
+            The subject to set.
+        """
+
+        self.subject = value
+
+        return self
+
+    @ensure_subject_is_given
+    def get_info(self) -> Any:
+        """
+        Provides the wanted network information.
+        """
 
-        return file_helper.open("r", encoding="utf-8")
+        raise NotImplementedError()
```

### Comparing `PyFunceble-4.1.3/PyFunceble/dataset/mariadb_base.py` & `PyFunceble-4.2.0/PyFunceble/dataset/sql_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -58,17 +58,17 @@
 from sqlalchemy.orm import Session
 
 import PyFunceble.cli.factory
 import PyFunceble.sessions
 from PyFunceble.dataset.db_base import DBDatasetBase
 
 
-class MariaDBDatasetBase(DBDatasetBase):
+class SQLDBDatasetBase(DBDatasetBase):
     """
-    Provides the base of all MariaDB stored dataset.
+    Provides the base of all SQLDB stored dataset.
     """
 
     STD_KEEP_SESSION_OPEN: bool = False
     ORM_OBJ = None
 
     db_session: Optional[Session] = None
 
@@ -117,15 +117,15 @@
 
         for row in self.db_session.query(self.ORM_OBJ):
             row = row.to_dict()
 
             yield row
 
     @DBDatasetBase.execute_if_authorized(None)
-    def update(self, row, *, ignore_if_exist: bool = False) -> "MariaDBDatasetBase":
+    def update(self, row, *, ignore_if_exist: bool = False) -> "SQLDBDatasetBase":
         """
         Adds the given dataset into the database if it does not exists.
         Update otherwise.
 
         .. note::
             This should be the preferred method for introduction of new dataset.
 
@@ -164,15 +164,15 @@
         PyFunceble.facility.Logger.debug("Updated row:\n%r", row)
         PyFunceble.facility.Logger.info("Finished to update row.")
 
         return self
 
     @DBDatasetBase.execute_if_authorized(None)
     @ensure_orm_obj_is_given
-    def remove(self, row) -> "MariaDBDatasetBase":
+    def remove(self, row) -> "SQLDBDatasetBase":
         """
         Removes the given dataset from the database.
 
         :param row:
             The row or dataset to check.
 
         :raise TypeError:
@@ -272,15 +272,15 @@
         for field in self.COMPARISON_FIELDS:
             result = result.filter(getattr(self.ORM_OBJ, field) == row[field])
 
         return result.first()
 
     @DBDatasetBase.execute_if_authorized(None)
     @ensure_orm_obj_is_given
-    def add(self, row) -> "MariaDBDatasetBase":
+    def add(self, row) -> "SQLDBDatasetBase":
         """
         Adds the given dataset into the database.
 
         :param row:
             The row or dataset to add.
 
         :raise TypeError:
@@ -305,15 +305,15 @@
             if "expiration_date" not in row and "epoch" not in row:
                 raise exception
 
             y2k38_limit = datetime(2037, 12, 31, 0, 0)
             new_date = datetime.fromtimestamp(float(row["epoch"]))
             new_date -= new_date - y2k38_limit
 
-            row["epoch"] = str(new_date.timestamp())
+            row["epoch"] = new_date.timestamp()
             row["expiration_date"] = new_date.strftime("%d-%b-%Y")
 
             self.db_session.execute(self.ORM_OBJ.__table__.insert(), row)
             self.db_session.commit()
 
         PyFunceble.facility.Logger.debug("Added row:\n%r", row)
         PyFunceble.facility.Logger.info("Finished to add row.")
```

### Comparing `PyFunceble-4.1.3/PyFunceble/dataset/public_suffix.py` & `PyFunceble-4.2.0/PyFunceble/dataset/public_suffix.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/dataset/user_agent.py` & `PyFunceble-4.2.0/PyFunceble/dataset/user_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/dataset/whois/__init__.py` & `PyFunceble-4.2.0/PyFunceble/database/credential/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides everything related to the whois database logic(s).
+Provides everything related to our credential holders.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/dataset/whois/base.py` & `PyFunceble-4.2.0/PyFunceble/cli/migrators/db_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the base of all WHOIS related dataset.
+Provides the base of all our database migration.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,79 +31,82 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-from datetime import datetime
-from typing import List, Union
+import functools
+from typing import Any
 
-from PyFunceble.database.sqlalchemy.all_schemas import WhoisRecord
-from PyFunceble.dataset.db_base import DBDatasetBase
+import sqlalchemy
 
+import PyFunceble.cli.facility
+import PyFunceble.cli.factory
+import PyFunceble.sessions
+from PyFunceble.cli.migrators.base import MigratorBase
 
-class WhoisDatasetBase(DBDatasetBase):
+
+class DBMigratorBase(MigratorBase):
     """
-    Provides the base of all Whois related interface.
+    Provides the base of all our database migration.
     """
 
-    FIELDS: List[str] = [
-        "subject",
-        "idna_subject",
-        "expiration_date",
-        "epoch",
-        "registrar",
-    ]
-
-    COMPARISON_FIELDS: List[str] = ["subject", "idna_subject"]
+    def __init__(self, print_action_to_stdout: bool = False) -> None:
+        super().__init__(print_action_to_stdout=print_action_to_stdout)
 
-    @staticmethod
-    def is_expired(row: Union[dict, WhoisRecord]) -> bool:
+    def execute_if_authorized(default: Any = None):  # pylint: disable=no-self-argument
         """
-        Given a row, we look if the row is expired.
+        Executes the decorated method only if we are authorized to process.
+        Otherwise, apply the given :code:`default`.
         """
 
-        if isinstance(row, WhoisRecord):
-            to_check = row.epoch
-        elif "epoch" in row:
-            to_check = row["epoch"]
-        else:
-            return True
+        def inner_metdhod(func):
+            @functools.wraps(func)
+            def wrapper(self, *args, **kwargs):
+                if self.authorized:
+                    return func(self, *args, **kwargs)  # pylint: disable=not-callable
+                return self if default is None else default
 
-        return datetime.utcnow() > datetime.fromtimestamp(float(to_check))
+            return wrapper
 
-    @DBDatasetBase.execute_if_authorized(None)
-    def get_filtered_row(self, row: Union[dict, WhoisRecord]) -> dict:
+        return inner_metdhod
+
+    @property
+    def authorized(self):
+        """
+        Provides the authorization to run.
         """
-        Removes all unkowns fields (not declared) from the given row.
 
-        :param row:
-            The row to work with.
+        return PyFunceble.cli.facility.CredentialLoader.is_already_loaded()
+
+    def does_table_exists(self, table_name: str) -> bool:
         """
+        Checks if the table exists.
 
-        if isinstance(row, WhoisDatasetBase):
-            row = row.to_dict()
+        :param table_name:
+            The name of the table to check.
+        """
 
-        result = super().get_filtered_row(row)
+        return sqlalchemy.inspect(PyFunceble.sessions.DB_ENGINE).has_table(table_name)
 
-        if "epoch" in result and isinstance(result["epoch"], float):
-            # We do this here because we have to convert to a string in
-            # order to be able to write into the CSV file.
-            result["epoch"] = str(result["epoch"])
+    def start(self) -> "MigratorBase":
+        """
+        Starts the migration.
+        """
 
-        return result
+        raise NotImplementedError()
```

### Comparing `PyFunceble-4.1.3/PyFunceble/dataset/whois/csv.py` & `PyFunceble-4.2.0/PyFunceble/dataset/whois/csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/dataset/whois/mariadb.py` & `PyFunceble-4.2.0/PyFunceble/dataset/whois/sql.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the interface for the WHOIS DB (mariadb) management.
+Provides the interface for the WHOIS DB (sql) management.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -58,27 +58,27 @@
 
 import PyFunceble.cli.factory
 import PyFunceble.cli.storage
 import PyFunceble.facility
 import PyFunceble.sessions
 import PyFunceble.storage
 from PyFunceble.database.sqlalchemy.all_schemas import WhoisRecord
-from PyFunceble.dataset.mariadb_base import MariaDBDatasetBase
+from PyFunceble.dataset.sql_base import SQLDBDatasetBase
 from PyFunceble.dataset.whois.base import WhoisDatasetBase
 
 
-class MariaDBWhoisDataset(MariaDBDatasetBase, WhoisDatasetBase):
+class SQLDBWhoisDataset(SQLDBDatasetBase, WhoisDatasetBase):
     """
     Provides the interface for the management of the WHOIS database under
     (mariadb).
     """
 
     ORM_OBJ: WhoisRecord = WhoisRecord
 
-    @MariaDBDatasetBase.execute_if_authorized(None)
+    @SQLDBDatasetBase.execute_if_authorized(None)
     def __contains__(self, value: str) -> bool:
         try:
             return (
                 self.db_session.query(self.ORM_OBJ)
                 .filter(
                     sqlalchemy.or_(
                         self.ORM_OBJ.subject == value,
@@ -87,15 +87,15 @@
                 )
                 .first()
                 is not None
             )
         except ProgrammingError:
             return None
 
-    @MariaDBDatasetBase.execute_if_authorized(None)
+    @SQLDBDatasetBase.execute_if_authorized(None)
     def __getitem__(self, value: Any) -> Optional[WhoisRecord]:
         try:
             return (
                 self.db_session.query(self.ORM_OBJ)
                 .filter(
                     sqlalchemy.or_(
                         self.ORM_OBJ.subject == value,
@@ -103,29 +103,29 @@
                     )
                 )
                 .first()
             )
         except ProgrammingError:
             return None
 
-    @MariaDBDatasetBase.execute_if_authorized(None)
+    @SQLDBDatasetBase.execute_if_authorized(None)
     def get_content(self) -> Generator[dict, None, None]:
         """
         Provides a generator which provides the next dataset to read.
         """
 
         for row in super().get_content():
             row["epoch"] = float(row["epoch"])
 
             yield row
 
-    @MariaDBDatasetBase.execute_if_authorized(None)
+    @SQLDBDatasetBase.execute_if_authorized(None)
     def update(
         self, row: Union[dict, WhoisRecord], *, ignore_if_exist: bool = False
-    ) -> "MariaDBWhoisDataset":
+    ) -> "SQLDBWhoisDataset":
         """
         Adds the given dataset into the database if it does not exists.
         Update otherwise.
 
         ..note::
             This should be the prefered method for introduction of new dataset.
 
@@ -150,16 +150,16 @@
             except ProgrammingError:
                 pass
         else:
             PyFunceble.facility.Logger.debug("Expired dataset:\n%r", row)
 
         return self
 
-    @MariaDBDatasetBase.execute_if_authorized(None)
-    def cleanup(self) -> "MariaDBWhoisDataset":
+    @SQLDBDatasetBase.execute_if_authorized(None)
+    def cleanup(self) -> "SQLDBWhoisDataset":
         """
         Cleanups the dataset. Meaning that we delete every entries which are
         in the past.
         """
 
         current_timestamp = int(datetime.utcnow().timestamp())
```

### Comparing `PyFunceble-4.1.3/PyFunceble/dataset/whois/mysql.py` & `PyFunceble-4.2.0/PyFunceble/downloader/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+# pylint:disable=line-too-long
 """
 The tool to check the availability or syntax of domain, IP or URL.
 
 ::
 
 
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the interface for the WHOIS DB (mysql) management.
+Provides the exceptions related to the downloader.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,30 +32,41 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-from PyFunceble.dataset.whois.mariadb import MariaDBWhoisDataset
+import PyFunceble.exceptions
 
 
-class MySQLWhoisDataset(MariaDBWhoisDataset):
+class PyFuncebleDownloaderException(PyFunceble.exceptions.PyFuncebleException):
     """
-    Provides the interface for the management of the WHOIS database under
-    mysql.
+    Describes the downloader (related) exceptions.
+    """
+
+
+class NoDownloadDestinationGiven(PyFuncebleDownloaderException):
+    """
+    Describes the fact that the download destination was not declared.
+    """
+
+
+class NoDownloadLinkGiven(PyFuncebleDownloaderException):
+    """
+    Describes the fact that no download link was declared.
     """
```

### Comparing `PyFunceble-4.1.3/PyFunceble/downloader/__init__.py` & `PyFunceble-4.2.0/PyFunceble/data/alembic/postgresql/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,39 +7,39 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides all downloaders.
+Provides the alembic data.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
-    https://pyfunceble.github.io/#/special-thanks
+    https://pyfunceble.github.io/special-thanks.html
 
 Contributors:
-    https://pyfunceble.github.io/#/contributors
+    https://pyfunceble.github.io/contributors.html
 
 Project link:
     https://github.com/funilrys/PyFunceble
 
 Project documentation:
     https://pyfunceble.readthedocs.io/en/latest/
 
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/downloader/base.py` & `PyFunceble-4.2.0/PyFunceble/downloader/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/downloader/exceptions.py` & `PyFunceble-4.2.0/PyFunceble/downloader/iana.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# pylint:disable=line-too-long
 """
 The tool to check the availability or syntax of domain, IP or URL.
 
 ::
 
 
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the exceptions related to the downloader.
+Provides the downloader of the latest iana database file.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -32,41 +31,48 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-import PyFunceble.exceptions
+import os
 
+import PyFunceble.storage
+from PyFunceble.downloader.base import DownloaderBase
 
-class PyFuncebleDownloaderException(PyFunceble.exceptions.PyFuncebleException):
+
+class IANADownloader(DownloaderBase):
     """
-    Describes the downloader (related) exceptions.
+    Provides the downloader of our iana file.
     """
 
+    DOWNTIME_INDEX: str = "iana"
+    DOWNLOAD_FREQUENCY: int = 1
 
-class NoDownloadDestinationGiven(PyFuncebleDownloaderException):
-    """
-    Describes the fact that the download destination was not declared.
-    """
+    def __init__(self) -> None:
+        self.destination = os.path.join(
+            PyFunceble.storage.CONFIG_DIRECTORY,
+            PyFunceble.storage.IANA_DUMP_FILENAME,
+        )
+        self.download_link = PyFunceble.storage.IANA_DUMP_LINK
 
+        super().__init__()
 
-class NoDownloadLinkGiven(PyFuncebleDownloaderException):
-    """
-    Describes the fact that no download link was declared.
-    """
+    @property
+    def authorized(self) -> bool:
+        return True
```

### Comparing `PyFunceble-4.1.3/PyFunceble/downloader/iana.py` & `PyFunceble-4.2.0/PyFunceble/downloader/user_agents.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the downloader of the latest iana database file.
+Provides the downloader of the latest user agents database file.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -52,27 +52,27 @@
 
 import os
 
 import PyFunceble.storage
 from PyFunceble.downloader.base import DownloaderBase
 
 
-class IANADownloader(DownloaderBase):
+class UserAgentsDownloader(DownloaderBase):
     """
-    Provides the downloader of our iana file.
+    Provides the downloader of our user agent file.
     """
 
-    DOWNTIME_INDEX: str = "iana"
+    DOWNTIME_INDEX: str = "user_agents"
     DOWNLOAD_FREQUENCY: int = 1
 
     def __init__(self) -> None:
         self.destination = os.path.join(
             PyFunceble.storage.CONFIG_DIRECTORY,
-            PyFunceble.storage.IANA_DUMP_FILENAME,
+            PyFunceble.storage.USER_AGENT_FILENAME,
         )
-        self.download_link = PyFunceble.storage.IANA_DUMP_LINK
+        self.download_link = PyFunceble.storage.USER_AGENT_DUMP_LINK
 
         super().__init__()
 
     @property
     def authorized(self) -> bool:
         return True
```

### Comparing `PyFunceble-4.1.3/PyFunceble/downloader/ipv4_reputation.py` & `PyFunceble-4.2.0/PyFunceble/downloader/ipv4_reputation.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/downloader/public_suffix.py` & `PyFunceble-4.2.0/PyFunceble/downloader/public_suffix.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/downloader/user_agents.py` & `PyFunceble-4.2.0/PyFunceble/facility.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the downloader of the latest user agents database file.
+Provides everything which we may need while running.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,48 +31,28 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-import os
+from PyFunceble.config.loader import ConfigLoader as config_loader
+from PyFunceble.logger import Logger as logger
 
-import PyFunceble.storage
-from PyFunceble.downloader.base import DownloaderBase
+ConfigLoader = config_loader()
 
-
-class UserAgentsDownloader(DownloaderBase):
-    """
-    Provides the downloader of our user agent file.
-    """
-
-    DOWNTIME_INDEX: str = "user_agents"
-    DOWNLOAD_FREQUENCY: int = 1
-
-    def __init__(self) -> None:
-        self.destination = os.path.join(
-            PyFunceble.storage.CONFIG_DIRECTORY,
-            PyFunceble.storage.USER_AGENT_FILENAME,
-        )
-        self.download_link = PyFunceble.storage.USER_AGENT_DUMP_LINK
-
-        super().__init__()
-
-    @property
-    def authorized(self) -> bool:
-        return True
+Logger = logger()
```

### Comparing `PyFunceble-4.1.3/PyFunceble/exceptions.py` & `PyFunceble-4.2.0/PyFunceble/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/facility.py` & `PyFunceble-4.2.0/PyFunceble/query/netinfo/hostbyaddr.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides everything which we may need while running.
+Provides an interface to get the information of a given host.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,28 +31,59 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-from PyFunceble.config.loader import ConfigLoader as config_loader
-from PyFunceble.logger import Logger as logger
+import socket
+from typing import Optional
 
-ConfigLoader = config_loader()
+from PyFunceble.query.netinfo.base import NetInfoBase
 
-Logger = logger()
+
+class HostByAddrInfo(NetInfoBase):
+    """
+    Provides the information of a given address/IP.
+    """
+
+    @NetInfoBase.ensure_subject_is_given
+    def get_info(self) -> Optional[dict]:
+        """
+        Fetch and provides the information of the given hosts.
+
+        :return:
+            A dictionnary with the following format or :py:class:`None` if nothing
+            was found.
+
+            ::
+
+                {
+                    "hostname": "",
+                    "aliases": [],
+                    "ips": []
+                }
+        """
+
+        try:
+            request = socket.gethostbyaddr(self.subject)
+
+            return {"hostname": request[0], "aliases": request[1], "ips": request[2]}
+        except (socket.gaierror, socket.herror):
+            pass
+
+        return dict()  # pylint: disable=use-dict-literal
```

### Comparing `PyFunceble-4.1.3/PyFunceble/factory.py` & `PyFunceble-4.2.0/PyFunceble/dataset/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides everything which doesn't get through the door of the facility.
+Provides all the dataset interaction submodules
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,25 +31,21 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
-
-from PyFunceble.query.requests.requester import Requester as requester
-
-Requester = requester()
```

### Comparing `PyFunceble-4.1.3/PyFunceble/helpers/__init__.py` & `PyFunceble-4.2.0/PyFunceble/query/dns/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the helpers.
+Provides everything related to our very own dns resolver.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/helpers/command.py` & `PyFunceble-4.2.0/PyFunceble/helpers/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -69,15 +69,14 @@
 
     def __init__(
         self,
         command: Optional[Union[str, list]] = None,
         *,
         encoding: Optional[str] = None,
     ) -> None:
-
         if command is not None:
             self.command = command
 
         if encoding is not None:
             self.encoding = encoding
 
     @property
```

### Comparing `PyFunceble-4.1.3/PyFunceble/helpers/dict.py` & `PyFunceble-4.2.0/PyFunceble/helpers/dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/helpers/directory.py` & `PyFunceble-4.2.0/PyFunceble/helpers/directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/helpers/download.py` & `PyFunceble-4.2.0/PyFunceble/helpers/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/helpers/environment_variable.py` & `PyFunceble-4.2.0/PyFunceble/helpers/environment_variable.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,29 +31,30 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
+import logging
 import os
 from typing import Any, Optional, Union
 
 import dotenv
 
 
 class EnvironmentVariableHelper:
@@ -70,14 +71,16 @@
     def __init__(self, name: Optional[str] = None, env_file_path: Optional[str] = None):
         if name is not None:
             self.name = name
 
         if env_file_path is not None:
             self.env_file_path = env_file_path
 
+        logging.getLogger("dotenv").setLevel(logging.CRITICAL)
+
     @property
     def name(self) -> Optional[str]:
         """
         Provides the current state of the :code:`_name` attribute.
         """
 
         return self._name
```

### Comparing `PyFunceble-4.1.3/PyFunceble/helpers/exceptions.py` & `PyFunceble-4.2.0/PyFunceble/helpers/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/helpers/file.py` & `PyFunceble-4.2.0/PyFunceble/helpers/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/helpers/hash.py` & `PyFunceble-4.2.0/PyFunceble/query/requests/adapter/http.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the hashing helpers.
+Provides the our HTTP adapter.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,139 +31,104 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-from typing import Optional, Union
+import urllib.parse
 
-from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives import hashes
+import requests
 
-from PyFunceble.helpers.file import FileHelper
+import PyFunceble.facility
+import PyFunceble.storage
+from PyFunceble.query.requests.adapter.base import RequestAdapterBase
 
 
-class HashHelper:
+class RequestHTTPAdapter(RequestAdapterBase):
     """
-    Simplify the hashing of data or file content.
-
-    :param str algo:
-        The algorithm to use for hashing.
-
-    :raise ValueError: When the given algo is not known.
+    Provides our HTTP adapter.
     """
 
-    _algo: str = "SHA512_224"
-
-    def __init__(self, algo: Optional[str] = None):
-        if algo is not None:
-            self.algo = algo
-
-    @property
-    def algo(self) -> str:
-        """
-        Provides the current state fo the :code:`_algo` attribute.
-        """
-
-        return self._algo
-
-    @algo.setter
-    def algo(self, value: str) -> None:
+    # pylint: disable=arguments-differ
+    def send(self, request, **kwargs) -> requests.Response:
         """
-        Sets the algorithm to work with.
+        Overwrite the upstream :code:`send` method.
 
-        :param value:
-            The name of the hash to use.
-
-        :raise TypeError:
-            When :code:`value` is not a :py:class:`str`.
-        """
+        We basically do the same. We only ensure that we request the IP from the chosen
+        DNS record.
 
-        if not isinstance(value, str):
-            raise TypeError(f"<value> should be {str}, {type(value)} given.")
-
-        value = value.upper()
-
-        if not hasattr(hashes, value):
-            raise ValueError(
-                f"<value> ({value!r}) in an unknown algorithm ({self.algo!r})."
+        :param request: The :class:`PreparedRequest <PreparedRequest>` being sent.
+        :param stream: (optional) Whether to stream the request content.
+        :param timeout: (optional) How long to wait for the server to send
+            data before giving up, as a float, or
+            a :ref:`(connect timeout, read timeout) <timeouts>` tuple.
+        :type timeout: float or tuple or urllib3 Timeout object
+        :param verify: (optional) Either a boolean, in which case it controls whether
+            we verify the server's TLS certificate, or a string, in which case it
+            must be a path to a CA bundle to use
+        :param cert: (optional) Any user-provided SSL certificate to be trusted.
+        :param proxies: (optional) The proxies dictionary to apply to the request.
+        :rtype: requests.Response
+
+        .. versionchanged:: 4.1.0b16
+            When a proxy is given, it is acceptable to have an unresolvable
+            subject. The proxy should handle the situation and give us back a
+            proper status or error.
+        """
+
+        kwargs["timeout"] = self.timeout
+
+        parsed_url = urllib.parse.urlparse(request.url)
+        hostname_ip = self.resolve(parsed_url.hostname)
+
+        kwargs["proxies"] = self.fetch_proxy_from_pattern(parsed_url.hostname)
+
+        PyFunceble.facility.Logger.debug("Parsed URL: %r", parsed_url)
+        PyFunceble.facility.Logger.debug("Resolved IP: %r", hostname_ip)
+        PyFunceble.facility.Logger.debug("KWARGS: %r", kwargs)
+        PyFunceble.facility.Logger.debug(
+            "Pool Manager: %r", self.poolmanager.connection_pool_kw
+        )
+
+        if hostname_ip or kwargs["proxies"]:
+            if hostname_ip:
+                request.url = request.url.replace(
+                    f"{parsed_url.scheme}://{parsed_url.hostname}",
+                    f"{parsed_url.scheme}://{hostname_ip}",
+                )
+
+            # Ensure that the Hosts header is present. Otherwise, connection might
+            # not work.
+            request.headers["Host"] = parsed_url.hostname
+        else:
+            self.poolmanager.connection_pool_kw.pop(
+                "server_hostname", PyFunceble.storage.NOT_RESOLVED_STD_HOSTNAME
+            )
+            self.poolmanager.connection_pool_kw.pop(
+                "assert_hostname", PyFunceble.storage.NOT_RESOLVED_STD_HOSTNAME
             )
 
-        self._algo = value
-
-    def set_algo(self, value: str) -> "HashHelper":
-        """
-        Sets the algorithm to work with.
-
-        :param value:
-            The name of the hash to use.
-        """
-
-        self.algo = value
-
-        return self
-
-    def __get_hash(self) -> hashes.Hash:
-        """
-        Provides the Hash to use.
-        """
-
-        return hashes.Hash(getattr(hashes, self.algo)(), backend=default_backend())
-
-    def hash_file(self, file_path: str) -> str:
-        """
-        Hashes the content of the given file.
-
-        :param file_path:
-            The path of the file to read.
-        """
-
-        block_size = 4096
-
-        digest = self.__get_hash()
-
-        with FileHelper(file_path).open("rb") as file_stream:
-            block = file_stream.read(block_size)
-
-            while block:
-                digest.update(block)
-                block = file_stream.read(block_size)
-
-        return digest.finalize().hex()
-
-    def hash_data(self, data: Union[str, bytes]) -> str:
-        """
-        Hashes the given data.
-
-        :param data:
-            The data to hash.
-
-        :raise TypeError:
-            When :code:`data` is not :py:class:`str` or :py:class:`bytes`.
-        """
-
-        if not isinstance(data, (bytes, str)):
-            raise TypeError(f"<data> should be {bytes} or {str}, {type(data)}, given.")
+            return self.fake_response()
 
-        if isinstance(data, str):
-            data = data.encode()
+        # raise Exception(hostname_ip, parsed_url, parsed_url.hostname, kwargs)
+        response = super().send(request, **kwargs)
 
-        digest = self.__get_hash()
-        digest.update(data)
+        if hostname_ip:
+            response.url = response.url.replace(hostname_ip, parsed_url.hostname)
 
-        return digest.finalize().hex()
+        return response
```

### Comparing `PyFunceble-4.1.3/PyFunceble/helpers/list.py` & `PyFunceble-4.2.0/PyFunceble/helpers/list.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/helpers/merge.py` & `PyFunceble-4.2.0/PyFunceble/helpers/merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/helpers/regex.py` & `PyFunceble-4.2.0/PyFunceble/helpers/regex.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/logger.py` & `PyFunceble-4.2.0/PyFunceble/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -118,15 +118,14 @@
     def __init__(
         self,
         *,
         activated: Optional[bool] = None,
         min_level: Optional[int] = None,
         output_dir: Optional[str] = None,
     ) -> None:
-
         if output_dir:
             self.output_directory = output_dir
         else:
             self.output_directory = os.path.join(
                 PyFunceble.cli.storage.OUTPUT_DIRECTORY,
                 PyFunceble.cli.storage.OUTPUTS.logs.directories.parent,
             )
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/__init__.py` & `PyFunceble-4.2.0/PyFunceble/database/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides everything related queries and communication with target resources
-and information.
+Provides everything related to the structure and connection with external databases.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -32,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/collection.py` & `PyFunceble-4.2.0/PyFunceble/query/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -111,15 +111,14 @@
     def __init__(
         self,
         *,
         token: Optional[str] = None,
         url_base: Optional[str] = None,
         preferred_status_origin: Optional[str] = None,
     ) -> None:
-
         if token is not None:
             self.token = token
         else:
             self.token = EnvironmentVariableHelper(
                 "PYFUNCEBLE_COLLECTION_API_TOKEN"
             ).get_value(default="")
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/dns/__init__.py` & `PyFunceble-4.2.0/PyFunceble/query/whois/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides everything related to our very own dns resolver.
+Provides everything related to the way we get or manipulate WHOIS record.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/dns/nameserver.py` & `PyFunceble-4.2.0/PyFunceble/query/dns/nameserver.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -63,14 +63,21 @@
 
 
 class Nameservers:
     """
     Provides an interface to get the right nameserver to communicate with.
     """
 
+    DEFAULT_NAMESERVERS: List[str] = [
+        "9.9.9.10",
+        "149.112.112.10",
+        "2620:fe::10",
+        "2620:fe::fe:10",
+    ]
+
     nameservers: Optional[List[str]] = None
     nameserver_ports: Optional[dict] = None
 
     protocol: Optional[str] = None
 
     domain_syntax_checker: DomainSyntaxChecker = DomainSyntaxChecker()
     url_syntax_checker: URLSyntaxChecker = URLSyntaxChecker()
@@ -243,19 +250,27 @@
         if PyFunceble.facility.ConfigLoader.is_already_loaded():
             if PyFunceble.storage.CONFIGURATION.dns.server:
                 if isinstance(PyFunceble.storage.CONFIGURATION.dns.server, list):
                     self.set_nameservers(PyFunceble.storage.CONFIGURATION.dns.server)
                 else:
                     self.set_nameservers([PyFunceble.storage.CONFIGURATION.dns.server])
             else:  # pragma: no cover
+                try:
+                    ## Well, I don't like playing with the default resolver.
+                    self.set_nameservers(
+                        dns.resolver.get_default_resolver().nameservers
+                    )
+                except dns.resolver.NoResolverConfiguration:
+                    self.set_nameservers(self.DEFAULT_NAMESERVERS)
+        else:  # pragma: no cover
+            try:
                 ## Well, I don't like playing with the default resolver.
                 self.set_nameservers(dns.resolver.get_default_resolver().nameservers)
-        else:  # pragma: no cover
-            ## Well, I don't like playing with the default resolver.
-            self.set_nameservers(dns.resolver.get_default_resolver().nameservers)
+            except dns.resolver.NoResolverConfiguration:
+                self.set_nameservers(self.DEFAULT_NAMESERVERS)
 
         return self
 
     def guess_all_settings(
         self,
     ) -> "Nameservers":  # pragma: no cover ## Method themselves are more important
         """
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/dns/query_tool.py` & `PyFunceble-4.2.0/PyFunceble/query/dns/query_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/dns/resolver.py` & `PyFunceble-4.2.0/PyFunceble/query/dns/resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/http_status_code.py` & `PyFunceble-4.2.0/PyFunceble/query/http_status_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/netinfo/__init__.py` & `PyFunceble-4.2.0/PyFunceble/data/alembic/postgresql/versions/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,39 +7,39 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides all our network info related subdmodules.
+Provides the alembic migrations files.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
-    https://pyfunceble.github.io/#/special-thanks
+    https://pyfunceble.github.io/special-thanks.html
 
 Contributors:
-    https://pyfunceble.github.io/#/contributors
+    https://pyfunceble.github.io/contributors.html
 
 Project link:
     https://github.com/funilrys/PyFunceble
 
 Project documentation:
     https://pyfunceble.readthedocs.io/en/latest/
 
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/netinfo/address.py` & `PyFunceble-4.2.0/PyFunceble/query/netinfo/address.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/netinfo/base.py` & `PyFunceble-4.2.0/PyFunceble/converter/url2netloc.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the base of all checker.
+Provides a way to convert/extract the network location of a given URL.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,106 +31,117 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-import functools
+import urllib.parse
 from typing import Any, Optional
 
+from PyFunceble.converter.base import ConverterBase
 
-class NetInfoBase:
+
+class Url2Netloc(ConverterBase):
     """
-    Provides the base of network information classes.
+    Provides the interface for the conversion/extration of the network location
+    of a given URL.
     """
 
-    _subject: Optional[str] = None
-    base: Optional[str] = None
-
-    def __init__(self, subject: Optional[str] = None) -> None:
-        if subject is not None:
-            self.subject = subject
+    parsed_url: Optional[urllib.parse.ParseResult] = None
+    """
+    Expose the parsed URL.
+    """
 
-    def ensure_subject_is_given(func):  # pylint: disable=no-self-argument
+    @ConverterBase.data_to_convert.setter
+    def data_to_convert(self, value: Any) -> None:
         """
-        Ensures that the subject is given before running the decorated method.
+        Overrites the default behavior.
 
         :raise TypeError:
-            If the subject is not a string.
+            When the given data to convert is not :py:class:`str`
+        :raise ValueError:
+            When the given data to convert is empty.
         """
 
-        @functools.wraps(func)
-        def wrapper(self, *args, **kwargs):
-            if not isinstance(self.subject, str):
-                raise TypeError(
-                    f"<self.subject> should be {str}, {type(self.subject)} given."
-                )
+        if not isinstance(value, str):
+            raise TypeError(f"<value> should be {str}, {type(value)} given.")
 
-            return func(self, *args, **kwargs)  # pylint: disable=not-callable
+        if not value:
+            raise ValueError("<value> should not be empty.")
 
-        return wrapper
+        # pylint: disable=no-member
+        super(Url2Netloc, self.__class__).data_to_convert.fset(self, value)
 
-    @property
-    def subject(self) -> Optional[str]:
+    @staticmethod
+    def parse_single_url(data) -> Optional[urllib.parse.ParseResult]:
         """
-        Provides the current state of the :code:`_subject` attribute.
+        Parses the URL.
         """
 
-        return self._subject
+        if data:
+            if "[" in data and "]" not in data or "]" in data and "[" not in data:
+                # Own wrapper around "Invalid IPv6 URL" when
+                # http://example.org."] is given (for example.)
+                data = data.replace("[", "").replace("]", "")
+
+            return urllib.parse.urlparse(data)
+        return None
 
-    @subject.setter
-    def subject(self, value: str) -> None:
+    def parse_url(self) -> "Url2Netloc":
+        """
+        Parses the URL.
         """
-        Sets the subject to work with.
 
-        :param value:
-            The subject to set.
+        self.parsed_url = self.parse_single_url(self.data_to_convert)
 
-        :raise TypeError:
-            When the given :code:`value` is not a :py:class:`str`.
-        :raise ValueError:
-            When the given :code:`value` is empty.
-        """
+        return self
 
-        if not isinstance(value, str):
-            raise TypeError(f"<value> should be {str}, {type(value)} given.")
+    def get_converted(self) -> str:
+        """
+        Provides the converted data (after conversion)
+        """
 
-        if not value:
-            raise ValueError("<value> should not be empty.")
+        # Retrocompatibility.
+        self.parse_url()
 
-        self._subject = value
+        return self.convert(self.data_to_convert)
 
-    def set_subject(self, value: str) -> "NetInfoBase":
+    def convert(self, data: Any) -> str:
         """
-        Sets the subject to work with.
+        Converts the given dataset.
 
-        :param value:
-            The subject to set.
+        :param data:
+            The data to convert.
         """
 
-        self.subject = value
+        parsed_url = self.parse_single_url(data)
 
-        return self
+        if not parsed_url.netloc and parsed_url.path:
+            netloc = parsed_url.path
+        elif parsed_url.netloc:
+            netloc = parsed_url.netloc
+        else:  # pragma: no cover ## Safety
+            netloc = data
 
-    @ensure_subject_is_given
-    def get_info(self) -> Any:
-        """
-        Provides the wanted network information.
-        """
+        if "//" in netloc:
+            netloc = netloc[netloc.find("//") + 2 :]
+
+        if "/" in netloc:
+            netloc = netloc[: netloc.find("/")]
 
-        raise NotImplementedError()
+        return netloc
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/netinfo/hostbyaddr.py` & `PyFunceble-4.2.0/PyFunceble/query/whois/converter/digit2digits.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides an interface to get the information of a given host.
+Provides an easy way to convert a digit string to 2 digits.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,59 +31,58 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
+# pylint: enable=line-too-long
 
-import socket
-from typing import Optional
+from typing import Any
 
-from PyFunceble.query.netinfo.base import NetInfoBase
+from PyFunceble.query.whois.converter.base import ConverterBase
 
 
-class HostByAddrInfo(NetInfoBase):
+class Digit2Digits(ConverterBase):
     """
-    Provides the information of a given address/IP.
+    Converts a given digit to a 2 digits string.
     """
 
-    @NetInfoBase.ensure_subject_is_given
-    def get_info(self) -> Optional[dict]:
+    @ConverterBase.data_to_convert.setter
+    def data_to_convert(self, value: Any) -> Any:
         """
-        Fetch and provides the information of the given hosts.
+        Overrites the default behavior.
 
-        :return:
-            A dictionnary with the following format or :py:class:`None` if nothing
-            was found.
-
-            ::
-
-                {
-                    "hostname": "",
-                    "aliases": [],
-                    "ips": []
-                }
+        :param value:
+            The data to convert.
+
+        :raise TypeError:
+            When the given data to convert is not :py:class:`str`
         """
 
-        try:
-            request = socket.gethostbyaddr(self.subject)
+        if not isinstance(value, str):
+            raise TypeError(f"<value> should be {str}, {type(value)} given.")
+
+        # pylint: disable=no-member
+        super(Digit2Digits, self.__class__).data_to_convert.fset(self, value)
 
-            return {"hostname": request[0], "aliases": request[1], "ips": request[2]}
-        except (socket.gaierror, socket.herror):
-            pass
+    @ConverterBase.ensure_data_to_convert_is_given
+    def get_converted(self) -> str:
+        """
+        Provides the converted data (after conversion)
+        """
 
-        return dict()  # pylint: disable=use-dict-literal
+        return str(self.data_to_convert).zfill(2)
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/record/__init__.py` & `PyFunceble-4.2.0/PyFunceble/cli/filesystem/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides all records classes.
+Provides everything related to our very own filesystem or output structure.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/record/base.py` & `PyFunceble-4.2.0/PyFunceble/query/record/dns.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the base of all our record classes.
+Provides the record class of the dns query tool.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -47,45 +47,33 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
 import dataclasses
-import json
-from typing import Any
+from typing import List, Optional
+
+from PyFunceble.query.record.base import RecordBase
 
 
 @dataclasses.dataclass
-class RecordBase:
+class DNSQueryToolRecord(RecordBase):
     """
-    Provides the base of all query record classes.
+    Provides a record of an executed request.
     """
 
-    def __getitem__(self, key: str) -> Any:
-        return getattr(self, key)
+    # pylint: disable=too-many-instance-attributes
+
+    nameserver: Optional[str] = None
+    port: Optional[int] = None
+    follow_nameserver_order: Optional[bool] = None
+    preferred_protocol: Optional[str] = None
+    used_protocol: Optional[str] = None
+
+    query_record_type: Optional[str] = None
+    query_timeout: Optional[float] = None
+
+    subject: Optional[str] = None
+    dns_name: Optional[str] = None
 
-    def to_dict(self) -> dict:
-        """
-        Provides the dict representation of the current object.
-        """
-
-        return {
-            x: y if not hasattr(y, "to_dict") else y.to_dict()
-            for x, y in self.__dict__.items()
-            if not x.startswith("__")
-        }
-
-    def to_json(self, *, pretty_print: bool = False) -> str:
-        """
-        Provides the JSON representation of the current object.
-
-        :param pretty_print:
-            If True, the JSON will be formatted.
-        """
-
-        return json.dumps(
-            self.to_dict(),
-            indent=4 if pretty_print else None,
-            ensure_ascii=False,
-            sort_keys=True if pretty_print else None,
-        )
+    response: Optional[List[str]] = None
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/record/whois.py` & `PyFunceble-4.2.0/PyFunceble/checker/utils/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the record class of the whois query tool.
+Provides some utilities related to the checkers.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,44 +31,21 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
-
-import dataclasses
-from typing import Optional
-
-from PyFunceble.query.record.base import RecordBase
-
-
-@dataclasses.dataclass
-class WhoisQueryToolRecord(RecordBase):
-    """
-    Provides a record of an executed request.
-    """
-
-    server: Optional[str] = None
-    port: Optional[str] = None
-
-    query_timeout: Optional[float] = None
-
-    subject: Optional[str] = None
-
-    record: Optional[str] = None
-    expiration_date: Optional[str] = None
-    registrar: Optional[str] = None
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/requests/__init__.py` & `PyFunceble-4.2.0/PyFunceble/cli/migrators/file_cleanup/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides everything related to our very own request handler.
+Provides the file cleanup migrators.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/requests/adapter/__init__.py` & `PyFunceble-4.2.0/PyFunceble/factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides everything related to our request adapters.
+Provides everything which doesn't get through the door of the facility.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,21 +31,25 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
+
+from PyFunceble.query.requests.requester import Requester as requester
+
+Requester = requester()
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/requests/adapter/base.py` & `PyFunceble-4.2.0/PyFunceble/query/requests/adapter/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/requests/adapter/http.py` & `PyFunceble-4.2.0/PyFunceble/query/requests/adapter/https.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the our HTTP adapter.
+Provides the our HTTPS adapter.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -55,15 +55,15 @@
 import requests
 
 import PyFunceble.facility
 import PyFunceble.storage
 from PyFunceble.query.requests.adapter.base import RequestAdapterBase
 
 
-class RequestHTTPAdapter(RequestAdapterBase):
+class RequestHTTPSAdapter(RequestAdapterBase):
     """
     Provides our HTTP adapter.
     """
 
     # pylint: disable=arguments-differ
     def send(self, request, **kwargs) -> requests.Response:
         """
@@ -108,27 +108,41 @@
         if hostname_ip or kwargs["proxies"]:
             if hostname_ip:
                 request.url = request.url.replace(
                     f"{parsed_url.scheme}://{parsed_url.hostname}",
                     f"{parsed_url.scheme}://{hostname_ip}",
                 )
 
+            if parsed_url.scheme == "https":
+                self.poolmanager.connection_pool_kw[
+                    "server_hostname"
+                ] = parsed_url.hostname
+                self.poolmanager.connection_pool_kw[
+                    "assert_hostname"
+                ] = parsed_url.hostname
+
             # Ensure that the Hosts header is present. Otherwise, connection might
             # not work.
             request.headers["Host"] = parsed_url.hostname
         else:
             self.poolmanager.connection_pool_kw.pop(
                 "server_hostname", PyFunceble.storage.NOT_RESOLVED_STD_HOSTNAME
             )
             self.poolmanager.connection_pool_kw.pop(
                 "assert_hostname", PyFunceble.storage.NOT_RESOLVED_STD_HOSTNAME
             )
 
+            self.poolmanager.connection_pool_kw.pop(
+                "server_hostname", parsed_url.hostname
+            )
+            self.poolmanager.connection_pool_kw.pop(
+                "assert_hostname", parsed_url.hostname
+            )
+
             return self.fake_response()
 
-        # raise Exception(hostname_ip, parsed_url, parsed_url.hostname, kwargs)
         response = super().send(request, **kwargs)
 
         if hostname_ip:
             response.url = response.url.replace(hostname_ip, parsed_url.hostname)
 
         return response
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/requests/adapter/https.py` & `PyFunceble-4.2.0/PyFunceble/storage.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+# pylint:disable=invalid-name, cyclic-import
 """
 The tool to check the availability or syntax of domain, IP or URL.
 
 ::
 
 
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the our HTTPS adapter.
+Provides a central storage place.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,118 +32,161 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-import urllib.parse
-
-import requests
-
-import PyFunceble.facility
-import PyFunceble.storage
-from PyFunceble.query.requests.adapter.base import RequestAdapterBase
-
-
-class RequestHTTPSAdapter(RequestAdapterBase):
-    """
-    Provides our HTTP adapter.
-    """
-
-    # pylint: disable=arguments-differ
-    def send(self, request, **kwargs) -> requests.Response:
-        """
-        Overwrite the upstream :code:`send` method.
-
-        We basically do the same. We only ensure that we request the IP from the chosen
-        DNS record.
-
-        :param request: The :class:`PreparedRequest <PreparedRequest>` being sent.
-        :param stream: (optional) Whether to stream the request content.
-        :param timeout: (optional) How long to wait for the server to send
-            data before giving up, as a float, or
-            a :ref:`(connect timeout, read timeout) <timeouts>` tuple.
-        :type timeout: float or tuple or urllib3 Timeout object
-        :param verify: (optional) Either a boolean, in which case it controls whether
-            we verify the server's TLS certificate, or a string, in which case it
-            must be a path to a CA bundle to use
-        :param cert: (optional) Any user-provided SSL certificate to be trusted.
-        :param proxies: (optional) The proxies dictionary to apply to the request.
-        :rtype: requests.Response
-
-        .. versionchanged:: 4.1.0b16
-            When a proxy is given, it is acceptable to have an unresolvable
-            subject. The proxy should handle the situation and give us back a
-            proper status or error.
-        """
-
-        kwargs["timeout"] = self.timeout
-
-        parsed_url = urllib.parse.urlparse(request.url)
-        hostname_ip = self.resolve(parsed_url.hostname)
-
-        kwargs["proxies"] = self.fetch_proxy_from_pattern(parsed_url.hostname)
-
-        PyFunceble.facility.Logger.debug("Parsed URL: %r", parsed_url)
-        PyFunceble.facility.Logger.debug("Resolved IP: %r", hostname_ip)
-        PyFunceble.facility.Logger.debug("KWARGS: %r", kwargs)
-        PyFunceble.facility.Logger.debug(
-            "Pool Manager: %r", self.poolmanager.connection_pool_kw
-        )
-
-        if hostname_ip or kwargs["proxies"]:
-            if hostname_ip:
-                request.url = request.url.replace(
-                    f"{parsed_url.scheme}://{parsed_url.hostname}",
-                    f"{parsed_url.scheme}://{hostname_ip}",
-                )
-
-            if parsed_url.scheme == "https":
-                self.poolmanager.connection_pool_kw[
-                    "server_hostname"
-                ] = parsed_url.hostname
-                self.poolmanager.connection_pool_kw[
-                    "assert_hostname"
-                ] = parsed_url.hostname
-
-            # Ensure that the Hosts header is present. Otherwise, connection might
-            # not work.
-            request.headers["Host"] = parsed_url.hostname
-        else:
-            self.poolmanager.connection_pool_kw.pop(
-                "server_hostname", PyFunceble.storage.NOT_RESOLVED_STD_HOSTNAME
-            )
-            self.poolmanager.connection_pool_kw.pop(
-                "assert_hostname", PyFunceble.storage.NOT_RESOLVED_STD_HOSTNAME
-            )
-
-            self.poolmanager.connection_pool_kw.pop(
-                "server_hostname", parsed_url.hostname
-            )
-            self.poolmanager.connection_pool_kw.pop(
-                "assert_hostname", parsed_url.hostname
-            )
-
-            return self.fake_response()
-
-        response = super().send(request, **kwargs)
-
-        if hostname_ip:
-            response.url = response.url.replace(hostname_ip, parsed_url.hostname)
-
-        return response
+import os
+import secrets
+from typing import Optional
+
+from box import Box
+from dotenv import load_dotenv
+
+from PyFunceble.storage_facility import get_config_directory
+
+PROJECT_NAME: str = "PyFunceble"
+PROJECT_VERSION: str = "4.2.0. (Blue Duckling: Ixora)"
+
+DISTRIBUTED_CONFIGURATION_FILENAME: str = ".PyFunceble_production.yaml"
+DISTRIBUTED_DIR_STRUCTURE_FILENAME: str = "dir_structure_production.json"
+
+IANA_DUMP_FILENAME: str = "iana-domains-db.json"
+PUBLIC_SUFFIX_DUMP_FILENAME: str = "public-suffix.json"
+CONFIGURATION_FILENAME: str = ".PyFunceble.yaml"
+CONFIGURATION_OVERWRITE_FILENAME: str = ".PyFunceble.overwrite.yaml"
+ENV_FILENAME: str = ".pyfunceble-env"
+DOWN_FILENAME: str = ".pyfunceble_intern_downtime.json"
+USER_AGENT_FILENAME: str = "user_agents.json"
+IPV4_REPUTATION_FILENAME: str = "ipv4_reputation.data"
+
+# pylint: disable=line-too-long
+IANA_DUMP_LINK: str = (
+    "https://raw.githubusercontent.com/PyFunceble/iana/master/iana-domains-db.json"
+)
+PUBLIC_SUFFIX_DUMP_LINK: str = "https://raw.githubusercontent.com/PyFunceble/public-suffix/master/public-suffix.json"
+USER_AGENT_DUMP_LINK: str = (
+    "https://raw.githubusercontent.com/PyFunceble/user_agents/master/user_agents.json"
+)
+IPV4_REPUTATION_DUMP_LINK: str = "https://reputation.alienvault.com/reputation.data"
+
+SHORT_REPO_LINK: str = "https://pyfunceble.github.io"
+REPO_LINK: str = "https://github.com/funilrys/PyFunceble"
+
+NOT_RESOLVED_STD_HOSTNAME: str = f"pyfunceble-{secrets.token_hex(12)}.com"
+
+IANA: Optional[dict] = {}
+PUBLIC_SUFFIX: Optional[dict] = {}
+USER_AGENTS: Optional[dict] = {}
+
+load_dotenv(".env")
+load_dotenv(ENV_FILENAME)
+
+CONFIG_DIRECTORY: str = get_config_directory(
+    project_name=PROJECT_NAME, project_version=PROJECT_VERSION
+)
+load_dotenv(os.path.join(CONFIG_DIRECTORY, ".env"))
+load_dotenv(os.path.join(CONFIG_DIRECTORY, ENV_FILENAME))
+
+# This is for the case that the environment variable are telling us something
+# else.
+CONFIG_DIRECTORY: str = get_config_directory(
+    project_name=PROJECT_NAME, project_version=PROJECT_VERSION
+)
+
+
+CONFIGURATION: Optional[Box] = Box({})
+FLATTEN_CONFIGURATION: Optional[dict] = {}
+STATUS: Optional[Box] = Box(
+    {
+        "up": "ACTIVE",
+        "down": "INACTIVE",
+        "valid": "VALID",
+        "invalid": "INVALID",
+        "malicious": "MALICIOUS",
+        "sane": "SANE",
+    },
+    frozen_box=True,
+)
+HTTP_CODES: Optional[Box] = Box({})
+COLLECTION: Optional[Box] = Box({})
+LINKS: Optional[Box] = Box({})
+PROXY: Optional[Box] = Box({})
+
+
+STD_HTTP_CODES: Optional[Box] = Box(
+    {
+        "list": {
+            "up": [
+                100,
+                101,
+                102,
+                200,
+                201,
+                202,
+                203,
+                204,
+                205,
+                206,
+                207,
+                208,
+                226,
+                429,
+            ],
+            "potentially_up": [
+                300,
+                301,
+                302,
+                303,
+                304,
+                305,
+                307,
+                308,
+                403,
+                405,
+                406,
+                407,
+                408,
+                411,
+                413,
+                417,
+                418,
+                421,
+                422,
+                423,
+                424,
+                426,
+                428,
+                431,
+                500,
+                501,
+                502,
+                503,
+                504,
+                505,
+                506,
+                507,
+                508,
+                510,
+                511,
+            ],
+            "potentially_down": [400, 402, 404, 409, 410, 412, 414, 415, 416, 451],
+        },
+    },
+    frozen_box=True,
+)
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/requests/requester.py` & `PyFunceble-4.2.0/PyFunceble/query/requests/requester.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/whois/__init__.py` & `PyFunceble-4.2.0/PyFunceble/query/whois/converter/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides everything related to the way we get or manipulate WHOIS record.
+Provides the converter or extractor around the WHOIS query logic.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/whois/converter/__init__.py` & `PyFunceble-4.2.0/PyFunceble/cli/factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides the converter or extractor around the WHOIS query logic.
+Provides everything which doesn't get through the door of the facility.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,21 +31,25 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
+
+from PyFunceble.database.session import DBSession as db_session
+
+DBSession = db_session()
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/whois/converter/base.py` & `PyFunceble-4.2.0/PyFunceble/query/whois/converter/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/whois/converter/digit2digits.py` & `PyFunceble-4.2.0/PyFunceble/checker/reputation/domain_and_ip.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides an easy way to convert a digit string to 2 digits.
+Provides the domains and IP reputation checker.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,58 +31,69 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
-# pylint: enable=line-too-long
 
-from typing import Any
+from PyFunceble.checker.reputation.base import ReputationCheckerBase
+from PyFunceble.checker.reputation.domain import DomainReputationChecker
+from PyFunceble.checker.reputation.ip import IPReputationChecker
 
-from PyFunceble.query.whois.converter.base import ConverterBase
 
-
-class Digit2Digits(ConverterBase):
+class DomainAndIPReputationChecker(ReputationCheckerBase):
     """
-    Converts a given digit to a 2 digits string.
+    Provides the interface for checking the reputation of an IP or domain.
+
+    :param str subject:
+        Optional, The subject to work with.
+    :param bool do_syntax_check_first:
+        Optional, Activates/Disables the check of the status before the actual
+        status gathering.
     """
 
-    @ConverterBase.data_to_convert.setter
-    def data_to_convert(self, value: Any) -> Any:
+    @ReputationCheckerBase.ensure_subject_is_given
+    @ReputationCheckerBase.update_status_date_after_query
+    def query_status(self) -> "DomainAndIPReputationChecker":
         """
-        Overrites the default behavior.
-
-        :param value:
-            The data to convert.
-
-        :raise TypeError:
-            When the given data to convert is not :py:class:`str`
+        Queries the result without anything more.
         """
 
-        if not isinstance(value, str):
-            raise TypeError(f"<value> should be {str}, {type(value)} given.")
+        if self.status.ip_syntax:
+            query_object = IPReputationChecker(
+                self.subject,
+                do_syntax_check_first=self.do_syntax_check_first,
+                db_session=self.db_session,
+                use_collection=self.use_collection,
+            )
+        else:
+            query_object = DomainReputationChecker(
+                self.subject,
+                do_syntax_check_first=self.do_syntax_check_first,
+                db_session=self.db_session,
+                use_collection=self.use_collection,
+            )
+
+        query_object.ipv4_reputation_query_tool = self.ipv4_reputation_query_tool
+        query_object.collection_query_tool = self.collection_query_tool
+        query_object.dns_query_tool = self.dns_query_tool
 
-        # pylint: disable=no-member
-        super(Digit2Digits, self.__class__).data_to_convert.fset(self, value)
+        result = query_object.query_status()
 
-    @ConverterBase.ensure_data_to_convert_is_given
-    def get_converted(self) -> str:
-        """
-        Provides the converted data (after conversion)
-        """
+        self.__dict__.update(query_object.__dict__)
 
-        return str(self.data_to_convert).zfill(2)
+        return result
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/whois/converter/expiration_date.py` & `PyFunceble-4.2.0/PyFunceble/query/whois/converter/expiration_date.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/whois/converter/month2unified.py` & `PyFunceble-4.2.0/PyFunceble/utils/profile.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+# pylint: disable=invalid-name
 """
 The tool to check the availability or syntax of domain, IP or URL.
 
 ::
 
 
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides a way to convert a given month to our unified format.
+Provides some global utilities.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -31,76 +32,102 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-from typing import Any, Dict, List
+import contextlib
+import cProfile
+import io
+import linecache
+import pstats
+import tracemalloc
 
-from PyFunceble.query.whois.converter.base import ConverterBase
 
+@contextlib.contextmanager
+def profile_it(*, sort_stats: str = "cumulative", show_callers: bool = False):
+    """
+    Provides a context manager which will activates the profiling of our
+    source code.
+
+    :param sort_starts:
+        The column to sort.
+    :param show_callers:
+        Authorizes the output of the callers.
+    """
+
+    profiler = cProfile.Profile()
+    profiler.enable()
+
+    yield
+
+    profiler.disable()
+
+    our_stream = io.StringIO()
 
-class Month2Unified(ConverterBase):
+    profiler_starts = pstats.Stats(profiler, stream=our_stream)
+
+    if sort_stats:
+        profiler_starts.sort_stats(sort_stats)
+
+    profiler_starts.print_stats()
+
+    if show_callers:
+        profiler_starts.print_callees()
+
+    print(our_stream.getvalue())
+
+
+@contextlib.contextmanager
+def profile_memory(stats_mode: str = "lineno", top_limit: int = 10):
     """
-    Converts the given month into our unified format.
+    Provides a context manager which will activates memory profiling of our
+    source code.
     """
 
-    MAP: Dict[str, List[str]] = {
-        "jan": [str(1), "01", "jan", "january", "jan."],
-        "feb": [str(2), "02", "feb", "february", "feb."],
-        "mar": [str(3), "03", "mar", "march", "mar."],
-        "apr": [str(4), "04", "apr", "april", "apr."],
-        "may": [str(5), "05", "may"],
-        "jun": [str(6), "06", "jun", "june", "jun."],
-        "jul": [str(7), "07", "jul", "july", "jul."],
-        "aug": [str(8), "08", "aug", "august", "aug."],
-        "sep": [str(9), "09", "sep", "september", "sep.", "sept", "sept."],
-        "oct": [str(10), "oct", "october", "oct."],
-        "nov": [str(11), "nov", "november", "nov."],
-        "dec": [str(12), "dec", "december", "dec."],
-    }
-
-    @ConverterBase.data_to_convert.setter
-    def data_to_convert(self, value: Any) -> None:
-        """
-        Overrites the default behavior.
-
-        :raise TypeError:
-            When the given data to convert is not :py:class:`str`
-        """
-
-        if not isinstance(value, str):
-            raise TypeError(f"<value> should be {str}, {type(value)} given.")
-
-        # pylint: disable=no-member
-        super(Month2Unified, self.__class__).data_to_convert.fset(self, value)
-
-    @ConverterBase.ensure_data_to_convert_is_given
-    def get_converted(self) -> str:
-        """
-        Provides the converted data (after conversion)
-
-        .. warning::
-            If no month is found, the given data is given as response.
-        """
-
-        for to_return, possibilities in self.MAP.items():
-            if self.data_to_convert.lower() in possibilities:
-                return to_return
+    tracemalloc.start()
+
+    yield
 
-        return self.data_to_convert
+    snapshot = tracemalloc.take_snapshot()
+    snapshot = snapshot.filter_traces(
+        (
+            tracemalloc.Filter(False, "<frozen importlib._bootstrap>"),
+            tracemalloc.Filter(False, "<unknown>"),
+            tracemalloc.Filter(False, "<frozen importlib._bootstrap_external>"),
+        )
+    )
+    top_stats = snapshot.statistics(stats_mode)
+
+    print("Top %s lines" % top_limit)
+    for index, stat in enumerate(top_stats[:top_limit], 1):
+        frame = stat.traceback[0]
+        print(
+            "#%s: %s:%s: %.1f KiB"
+            % (index, frame.filename, frame.lineno, stat.size / 1024)
+        )
+        line = linecache.getline(frame.filename, frame.lineno).strip()
+        if line:
+            print("    %s" % line)
+
+    other = top_stats[top_limit:]
+    if other:
+        size = sum(stat.size for stat in other)
+        print("%s other: %.1f KiB" % (len(other), size / 1024))
+    total = sum(stat.size for stat in top_stats)
+    print("Total allocated size: %.1f KiB" % (total / 1024))
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/whois/converter/registrar.py` & `PyFunceble-4.2.0/PyFunceble/query/whois/converter/registrar.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/query/whois/query_tool.py` & `PyFunceble-4.2.0/PyFunceble/query/whois/query_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -385,15 +385,14 @@
     ) -> str:  # pragma: no cover ## The effect of the response of this method
         ## are more important.
         """
         Queries the WHOIS record and return the current object.
         """
 
         if self.lookup_record.record is None:
-
             if not self.server:
                 whois_server = self.get_whois_server()
             else:
                 whois_server = self.server
 
             if whois_server:
                 self.lookup_record.server = whois_server
```

### Comparing `PyFunceble-4.1.3/PyFunceble/sessions.py` & `PyFunceble-4.2.0/PyFunceble/sessions.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/storage.py` & `PyFunceble-4.2.0/PyFunceble/checker/availability/domain_and_ip.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# pylint:disable=invalid-name, cyclic-import
 """
 The tool to check the availability or syntax of domain, IP or URL.
 
 ::
 
 
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides a central storage place.
+Provides the domains and IP availability checker.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -32,161 +31,116 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-import os
-import secrets
-from typing import Optional
-
-from box import Box
-from dotenv import load_dotenv
-
-from PyFunceble.storage_facility import get_config_directory
-
-PROJECT_NAME: str = "PyFunceble"
-PROJECT_VERSION: str = "4.1.3. (Blue Duckling: Dahlia)"
-
-DISTRIBUTED_CONFIGURATION_FILENAME: str = ".PyFunceble_production.yaml"
-DISTRIBUTED_DIR_STRUCTURE_FILENAME: str = "dir_structure_production.json"
-
-IANA_DUMP_FILENAME: str = "iana-domains-db.json"
-PUBLIC_SUFFIX_DUMP_FILENAME: str = "public-suffix.json"
-CONFIGURATION_FILENAME: str = ".PyFunceble.yaml"
-CONFIGURATION_OVERWRITE_FILENAME: str = ".PyFunceble.overwrite.yaml"
-ENV_FILENAME: str = ".pyfunceble-env"
-DOWN_FILENAME: str = ".pyfunceble_intern_downtime.json"
-USER_AGENT_FILENAME: str = "user_agents.json"
-IPV4_REPUTATION_FILENAME: str = "ipv4_reputation.data"
-
-# pylint: disable=line-too-long
-IANA_DUMP_LINK: str = (
-    "https://raw.githubusercontent.com/PyFunceble/iana/master/iana-domains-db.json"
-)
-PUBLIC_SUFFIX_DUMP_LINK: str = "https://raw.githubusercontent.com/PyFunceble/public-suffix/master/public-suffix.json"
-USER_AGENT_DUMP_LINK: str = (
-    "https://raw.githubusercontent.com/PyFunceble/user_agents/master/user_agents.json"
-)
-IPV4_REPUTATION_DUMP_LINK: str = "https://reputation.alienvault.com/reputation.data"
-
-SHORT_REPO_LINK: str = "https://git.io/vpZoI"
-REPO_LINK: str = "https://github.com/funilrys/PyFunceble"
-
-NOT_RESOLVED_STD_HOSTNAME: str = f"pyfunceble-{secrets.token_hex(12)}.com"
-
-IANA: Optional[dict] = {}
-PUBLIC_SUFFIX: Optional[dict] = {}
-USER_AGENTS: Optional[dict] = {}
-
-load_dotenv(".env")
-load_dotenv(ENV_FILENAME)
-
-CONFIG_DIRECTORY: str = get_config_directory(
-    project_name=PROJECT_NAME, project_version=PROJECT_VERSION
-)
-load_dotenv(os.path.join(CONFIG_DIRECTORY, ".env"))
-load_dotenv(os.path.join(CONFIG_DIRECTORY, ENV_FILENAME))
-
-# This is for the case that the environment variable are telling us something
-# else.
-CONFIG_DIRECTORY: str = get_config_directory(
-    project_name=PROJECT_NAME, project_version=PROJECT_VERSION
-)
-
-
-CONFIGURATION: Optional[Box] = Box({})
-FLATTEN_CONFIGURATION: Optional[dict] = {}
-STATUS: Optional[Box] = Box(
-    {
-        "up": "ACTIVE",
-        "down": "INACTIVE",
-        "valid": "VALID",
-        "invalid": "INVALID",
-        "malicious": "MALICIOUS",
-        "sane": "SANE",
-    },
-    frozen_box=True,
-)
-HTTP_CODES: Optional[Box] = Box({})
-COLLECTION: Optional[Box] = Box({})
-LINKS: Optional[Box] = Box({})
-PROXY: Optional[Box] = Box({})
-
-
-STD_HTTP_CODES: Optional[Box] = Box(
-    {
-        "list": {
-            "up": [
-                100,
-                101,
-                102,
-                200,
-                201,
-                202,
-                203,
-                204,
-                205,
-                206,
-                207,
-                208,
-                226,
-                429,
-            ],
-            "potentially_up": [
-                300,
-                301,
-                302,
-                303,
-                304,
-                305,
-                307,
-                308,
-                403,
-                405,
-                406,
-                407,
-                408,
-                411,
-                413,
-                417,
-                418,
-                421,
-                422,
-                423,
-                424,
-                426,
-                428,
-                431,
-                500,
-                501,
-                502,
-                503,
-                504,
-                505,
-                506,
-                507,
-                508,
-                510,
-                511,
-            ],
-            "potentially_down": [400, 402, 404, 409, 410, 412, 414, 415, 416, 451],
-        },
-    },
-    frozen_box=True,
-)
+from typing import Union
+
+from PyFunceble.checker.availability.base import AvailabilityCheckerBase
+from PyFunceble.checker.availability.domain import DomainAvailabilityChecker
+from PyFunceble.checker.availability.ip import IPAvailabilityChecker
+
+
+class DomainAndIPAvailabilityChecker(AvailabilityCheckerBase):
+    """
+    Provides the interface for checking the availability of a IP or domain.
+
+    :param str subject:
+        Optional, The subject to work with.
+    :param bool use_extra_rules:
+        Optional, Activates/Disables the usage of our own set of extra rules.
+    :param bool use_whois_lookup:
+        Optional, Activates/Disables the usage of the WHOIS lookup to gather
+        the status of the given :code:`subject`.
+    :param bool use_dns_lookup:
+        Optional, Activates/Disables the usage of the DNS lookup to gather the
+        status of the given :code:`subject`.
+    :param bool use_netinfo_lookup:
+        Optional, Activates/Disables the usage of the network information
+        lookup module to gather the status of the given :code:`subject`.
+    :param bool use_http_code_lookup:
+        Optional, Activates/Disables the usage of the HTTP status code lookup
+        to gather the status of the given :code:`subject`.
+    :param bool use_reputation_lookup:
+        Optional, Activates/Disables the usage of the reputation dataset
+        lookup to gather the status of the given :code:`subject`.
+    :param bool do_syntax_check_first:
+        Optional, Activates/Disables the check of the status before the actual
+        status gathering.
+    :param bool use_whois_db:
+        Optional, Activates/Disable the usage of a local database to store the
+        WHOIS datasets.
+    """
+
+    @AvailabilityCheckerBase.ensure_subject_is_given
+    @AvailabilityCheckerBase.update_status_date_after_query
+    def query_status(
+        self,
+    ) -> "DomainAndIPAvailabilityChecker":  # pragma: no cover ## Just a switch.
+        """
+        Queries the result without anything more.
+        """
+
+        query_object: Union[IPAvailabilityChecker, DomainAvailabilityChecker] = None
+
+        if self.status.ip_syntax:
+            query_object = IPAvailabilityChecker(
+                self.subject,
+                use_extra_rules=self.use_extra_rules,
+                use_whois_lookup=self.use_whois_lookup,
+                use_dns_lookup=self.use_dns_lookup,
+                use_netinfo_lookup=self.use_netinfo_lookup,
+                use_http_code_lookup=self.use_http_code_lookup,
+                use_reputation_lookup=self.use_reputation_lookup,
+                do_syntax_check_first=self.do_syntax_check_first,
+                db_session=self.db_session,
+                use_whois_db=self.use_whois_db,
+                use_collection=self.use_collection,
+            )
+        else:
+            query_object = DomainAvailabilityChecker(
+                self.subject,
+                use_extra_rules=self.use_extra_rules,
+                use_whois_lookup=self.use_whois_lookup,
+                use_dns_lookup=self.use_dns_lookup,
+                use_netinfo_lookup=self.use_netinfo_lookup,
+                use_http_code_lookup=self.use_http_code_lookup,
+                use_reputation_lookup=self.use_reputation_lookup,
+                do_syntax_check_first=self.do_syntax_check_first,
+                db_session=self.db_session,
+                use_whois_db=self.use_whois_db,
+                use_collection=self.use_collection,
+            )
+
+        query_object.dns_query_tool = self.dns_query_tool
+        query_object.whois_query_tool = self.whois_query_tool
+        query_object.collection_query_tool = self.collection_query_tool
+        query_object.hostbyaddr_query_tool = self.hostbyaddr_query_tool
+        query_object.addressinfo_query_tool = self.addressinfo_query_tool
+        query_object.http_status_code_query_tool = self.http_status_code_query_tool
+
+        result = query_object.query_status()
+
+        self.__dict__.update(query_object.__dict__)
+
+        return result
+
+    @staticmethod
+    def is_valid() -> bool:  # pylint: disable=arguments-differ
+        raise NotImplementedError()
```

### Comparing `PyFunceble-4.1.3/PyFunceble/storage_facility.py` & `PyFunceble-4.2.0/PyFunceble/storage_facility.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/utils/__init__.py` & `PyFunceble-4.2.0/PyFunceble/query/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# pylint: disable=invalid-name
 """
 The tool to check the availability or syntax of domain, IP or URL.
 
 ::
 
 
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides some global utilities.
+Provides everything related queries and communication with target resources
+and information.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -32,15 +32,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/utils/platform.py` & `PyFunceble-4.2.0/PyFunceble/utils/platform.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble/utils/profile.py` & `PyFunceble-4.2.0/PyFunceble/cli/utils/ascii_logo.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# pylint: disable=invalid-name
 """
 The tool to check the availability or syntax of domain, IP or URL.
 
 ::
 
 
     ██████╗ ██╗   ██╗███████╗██╗   ██╗███╗   ██╗ ██████╗███████╗██████╗ ██╗     ███████╗
     ██╔══██╗╚██╗ ██╔╝██╔════╝██║   ██║████╗  ██║██╔════╝██╔════╝██╔══██╗██║     ██╔════╝
     ██████╔╝ ╚████╔╝ █████╗  ██║   ██║██╔██╗ ██║██║     █████╗  ██████╔╝██║     █████╗
     ██╔═══╝   ╚██╔╝  ██╔══╝  ██║   ██║██║╚██╗██║██║     ██╔══╝  ██╔══██╗██║     ██╔══╝
     ██║        ██║   ██║     ╚██████╔╝██║ ╚████║╚██████╗███████╗██████╔╝███████╗███████╗
     ╚═╝        ╚═╝   ╚═╝      ╚═════╝ ╚═╝  ╚═══╝ ╚═════╝╚══════╝╚═════╝ ╚══════╝╚══════╝
 
-Provides some global utilities.
+Provides some utilities related to the ascii logo.
 
 Author:
     Nissar Chababy, @funilrys, contactTATAfunilrysTODTODcom
 
 Special thanks:
     https://pyfunceble.github.io/#/special-thanks
 
@@ -32,102 +31,96 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 """
 
-import contextlib
-import cProfile
-import io
-import linecache
-import pstats
-import tracemalloc
+import colorama
 
+import PyFunceble.cli.storage
+import PyFunceble.facility
+import PyFunceble.storage
 
-@contextlib.contextmanager
-def profile_it(*, sort_stats: str = "cumulative", show_callers: bool = False):
-    """
-    Provides a context manager which will activates the profiling of our
-    source code.
 
-    :param sort_starts:
-        The column to sort.
-    :param show_callers:
-        Authorizes the output of the callers.
+def colorify(color: str, *, text=None) -> str:
     """
+    Colorify the logo with the given color.
 
-    profiler = cProfile.Profile()
-    profiler.enable()
+    :param color:
+        The name of the color to apply.
 
-    yield
+        .. warning::
+            The given color name must be one of the supported
+            by colorama.
 
-    profiler.disable()
+    :raise ValueError:
+        When the given :code:`color` is unsupported.
+    """
 
-    our_stream = io.StringIO()
+    color = color.upper()
 
-    profiler_starts = pstats.Stats(profiler, stream=our_stream)
+    if not text:
+        to_color = PyFunceble.cli.storage.ASCII_PYFUNCEBLE
+    else:
+        to_color = text
 
-    if sort_stats:
-        profiler_starts.sort_stats(sort_stats)
+    if not hasattr(colorama.Fore, color):
+        raise ValueError(f"<color> ({color!r}) is not supported.")
 
-    profiler_starts.print_stats()
+    color_to_apply = getattr(colorama.Fore, color)
+    result = []
 
-    if show_callers:
-        profiler_starts.print_callees()
+    if (
+        PyFunceble.facility.ConfigLoader.is_already_loaded()
+        and PyFunceble.storage.CONFIGURATION.cli_testing.display_mode.colour
+    ):
+        for line in to_color.split("\n"):
+            result.append(f"{color_to_apply}{line}{colorama.Fore.RESET}")
 
-    print(our_stream.getvalue())
+        return "\n".join(result)
+    return to_color
 
 
-@contextlib.contextmanager
-def profile_memory(stats_mode: str = "lineno", top_limit: int = 10):
+def get_home_representation() -> str:
     """
-    Provides a context manager which will activates memory profiling of our
-    source code.
+    Provides our home ASCII logo representation.
     """
 
-    tracemalloc.start()
+    return colorify("yellow")
 
-    yield
 
-    snapshot = tracemalloc.take_snapshot()
-    snapshot = snapshot.filter_traces(
-        (
-            tracemalloc.Filter(False, "<frozen importlib._bootstrap>"),
-            tracemalloc.Filter(False, "<unknown>"),
-            tracemalloc.Filter(False, "<frozen importlib._bootstrap_external>"),
-        )
-    )
-    top_stats = snapshot.statistics(stats_mode)
+def get_result_representation(status: str) -> str:
+    """
+    Provides our result ASCII logo representation.
+    """
 
-    print("Top %s lines" % top_limit)
-    for index, stat in enumerate(top_stats[:top_limit], 1):
-        frame = stat.traceback[0]
-        print(
-            "#%s: %s:%s: %.1f KiB"
-            % (index, frame.filename, frame.lineno, stat.size / 1024)
-        )
-        line = linecache.getline(frame.filename, frame.lineno).strip()
-        if line:
-            print("    %s" % line)
+    if status in (
+        PyFunceble.storage.STATUS.up,
+        PyFunceble.storage.STATUS.valid,
+        PyFunceble.storage.STATUS.sane,
+    ):
+        color = "green"
+    elif status in (
+        PyFunceble.storage.STATUS.down,
+        PyFunceble.storage.STATUS.malicious,
+    ):
+        color = "red"
+    else:
+        color = "cyan"
 
-    other = top_stats[top_limit:]
-    if other:
-        size = sum(stat.size for stat in other)
-        print("%s other: %.1f KiB" % (len(other), size / 1024))
-    total = sum(stat.size for stat in top_stats)
-    print("Total allocated size: %.1f KiB" % (total / 1024))
+    return colorify(color, text=PyFunceble.cli.storage.ASCII_PYUNCEBLE_RESULT)
```

### Comparing `PyFunceble-4.1.3/PyFunceble/utils/version.py` & `PyFunceble-4.2.0/PyFunceble/utils/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PyFunceble-4.1.3/PyFunceble.egg-info/PKG-INFO` & `PyFunceble-4.2.0/PyFunceble.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFunceble
-Version: 4.1.3
+Version: 4.2.0
 Summary: The tool to check the availability or syntax of domain, IP or URL.
 Home-page: https://github.com/funilrys/PyFunceble
 Author: funilrys
 Author-email: contact@funilrys.com
 License: Apache 2.0
 Project-URL: Documentation, https://pyfunceble.readthedocs.io/en/latest/
 Project-URL: Funding, https://github.com/sponsors/funilrys
@@ -15,18 +15,19 @@
 Classifier: Environment :: Console
 Classifier: Topic :: Internet
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.8, <4
 Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: psql
 Provides-Extra: full
 License-File: LICENSE
 
 .. image:: https://raw.githubusercontent.com/PyFunceble/logo/master/Green/HD/RM.png
 
 The tool to check the availability or syntax of domain, IP or URL
 -----------------------------------------------------------------
@@ -182,14 +183,15 @@
 -   Daniel - `@dnmTX`_
 -   gwarser - `@gwarser`_
 -   Haris Gušić - `@veracioux`_
 -   hawkeye116477 - `@hawkeye116477`_
 -   Human Being - `@T145`_
 -   Imre Kristoffer Eilertsen - `@DandelionSprout`_
 -   jawz101 - `@jawz101`_
+-   Josenilson Ferreira da SIlva - `@Nilsonfsilva`_
 -   keczuppp - `@keczuppp`_
 -   kowith337 - `@kowith337`_
 -   Mitchell Krog - `@mitchellkrogza`_
 -   NeolithEra - `@NeolithEra`_
 -   Odyseus - `@Odyseus`_
 -   opav - `@opav`_
 -   Reza Rizqullah - `@ybreza`_
@@ -259,15 +261,15 @@
 
 ___________________________________________
 
 License
 -------
 ::
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -310,14 +312,15 @@
 .. _@hawkeye116477: https://github.com/hawkeye116477
 .. _@jawz101: https://github.com/jawz101
 .. _@keczuppp: https://github.com/keczuppp
 .. _@kennethreitz: https://github.com/kennethreitz
 .. _@kowith337: https://github.com/kowith337
 .. _@mitchellkrogza: https://github.com/mitchellkrogza
 .. _@NeolithEra: https://github.com/NeolithEra
+.. _@Nilsonfsilva: https://github.com/Nilsonfsilva
 .. _@Odyseus: https://github.com/Odyseus
 .. _@opav: https://github.com/opav
 .. _@pi-hole: https://github.com/pi-hole/pi-hole
 .. _@PromoFaux: https://github.com/PromoFaux
 .. _@publicsuffix: https://github.com/publicsuffix
 .. _@rthalley: https://github.com/rthalley
 .. _@rusty-snake: https://github.com/rusty-snake
```

### Comparing `PyFunceble-4.1.3/PyFunceble.egg-info/SOURCES.txt` & `PyFunceble-4.2.0/PyFunceble.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -21,40 +21,46 @@
 PyFunceble/storage_facility.py
 PyFunceble.egg-info/PKG-INFO
 PyFunceble.egg-info/SOURCES.txt
 PyFunceble.egg-info/dependency_links.txt
 PyFunceble.egg-info/entry_points.txt
 PyFunceble.egg-info/requires.txt
 PyFunceble.egg-info/top_level.txt
-PyFunceble/.vscode/settings.json
 PyFunceble/checker/__init__.py
 PyFunceble/checker/base.py
 PyFunceble/checker/complex_json_encoder.py
 PyFunceble/checker/params_base.py
 PyFunceble/checker/status_base.py
 PyFunceble/checker/availability/__init__.py
 PyFunceble/checker/availability/base.py
 PyFunceble/checker/availability/domain.py
 PyFunceble/checker/availability/domain_and_ip.py
-PyFunceble/checker/availability/extra_rules.py
 PyFunceble/checker/availability/ip.py
 PyFunceble/checker/availability/params.py
 PyFunceble/checker/availability/status.py
 PyFunceble/checker/availability/url.py
+PyFunceble/checker/availability/extras/__init__.py
+PyFunceble/checker/availability/extras/base.py
+PyFunceble/checker/availability/extras/dns.py
+PyFunceble/checker/availability/extras/etoxic.py
+PyFunceble/checker/availability/extras/parked.py
+PyFunceble/checker/availability/extras/rules.py
+PyFunceble/checker/availability/extras/subject_switch.py
 PyFunceble/checker/reputation/__init__.py
 PyFunceble/checker/reputation/base.py
 PyFunceble/checker/reputation/domain.py
 PyFunceble/checker/reputation/domain_and_ip.py
 PyFunceble/checker/reputation/ip.py
 PyFunceble/checker/reputation/params.py
 PyFunceble/checker/reputation/status.py
 PyFunceble/checker/reputation/url.py
 PyFunceble/checker/syntax/__init__.py
 PyFunceble/checker/syntax/base.py
 PyFunceble/checker/syntax/domain.py
+PyFunceble/checker/syntax/domain_and_ip.py
 PyFunceble/checker/syntax/domain_base.py
 PyFunceble/checker/syntax/ip.py
 PyFunceble/checker/syntax/ipv4.py
 PyFunceble/checker/syntax/ipv6.py
 PyFunceble/checker/syntax/params.py
 PyFunceble/checker/syntax/second_lvl_domain.py
 PyFunceble/checker/syntax/status.py
@@ -169,72 +175,76 @@
 PyFunceble/converter/rpz_input_line2subject.py
 PyFunceble/converter/rpz_policy2subject.py
 PyFunceble/converter/subject2complements.py
 PyFunceble/converter/url2netloc.py
 PyFunceble/converter/wildcard2subject.py
 PyFunceble/data/__init__.py
 PyFunceble/data/alembic/__init__.py
-PyFunceble/data/alembic/env.py
-PyFunceble/data/alembic/script.py.mako
-PyFunceble/data/alembic/versions/35c79626ecb9_fix_some_columns.py
-PyFunceble/data/alembic/versions/3a4c55a9320d_add_continue_table.py
-PyFunceble/data/alembic/versions/3d6f4a33cdb2_add_inactive_table.py
-PyFunceble/data/alembic/versions/45713fea8097_deletion_uneeded_columns_from_whois_.py
-PyFunceble/data/alembic/versions/459a0d7b8f09_add_idna_subject_column_into_whois.py
-PyFunceble/data/alembic/versions/6f4729deaf03_delete_inactive_source_column.py
-PyFunceble/data/alembic/versions/7bcf7fa64ba1_rename_created_to_created_at_and.py
-PyFunceble/data/alembic/versions/83ada95132bf_delete_the_file_table.py
-PyFunceble/data/alembic/versions/912bbcb77a6c_add_registrar_column.py
-PyFunceble/data/alembic/versions/95dc17ddd729_introduction_of_the_session_id_column.py
-PyFunceble/data/alembic/versions/__init__.py
-PyFunceble/data/alembic/versions/ade87195b0a0_base.py
-PyFunceble/data/alembic/versions/bef7bcaac3f2_make_id_a_bigint.py
-PyFunceble/data/alembic/versions/d8893cd406db_allow_whois_record_to_be_empty_null.py
-PyFunceble/data/alembic/versions/e04e8301d1a2_deletion_of_the_mined_table.py
+PyFunceble/data/alembic/mysql/__init__.py
+PyFunceble/data/alembic/mysql/env.py
+PyFunceble/data/alembic/mysql/script.py.mako
+PyFunceble/data/alembic/mysql/versions/35c79626ecb9_fix_some_columns.py
+PyFunceble/data/alembic/mysql/versions/3a4c55a9320d_add_continue_table.py
+PyFunceble/data/alembic/mysql/versions/3d6f4a33cdb2_add_inactive_table.py
+PyFunceble/data/alembic/mysql/versions/45713fea8097_deletion_uneeded_columns_from_whois_.py
+PyFunceble/data/alembic/mysql/versions/459a0d7b8f09_add_idna_subject_column_into_whois.py
+PyFunceble/data/alembic/mysql/versions/6f4729deaf03_delete_inactive_source_column.py
+PyFunceble/data/alembic/mysql/versions/7bcf7fa64ba1_rename_created_to_created_at_and.py
+PyFunceble/data/alembic/mysql/versions/83ada95132bf_delete_the_file_table.py
+PyFunceble/data/alembic/mysql/versions/912bbcb77a6c_add_registrar_column.py
+PyFunceble/data/alembic/mysql/versions/95dc17ddd729_introduction_of_the_session_id_column.py
+PyFunceble/data/alembic/mysql/versions/__init__.py
+PyFunceble/data/alembic/mysql/versions/ade87195b0a0_base.py
+PyFunceble/data/alembic/mysql/versions/bef7bcaac3f2_make_id_a_bigint.py
+PyFunceble/data/alembic/mysql/versions/d8893cd406db_allow_whois_record_to_be_empty_null.py
+PyFunceble/data/alembic/mysql/versions/e04e8301d1a2_deletion_of_the_mined_table.py
+PyFunceble/data/alembic/postgresql/__init__.py
+PyFunceble/data/alembic/postgresql/env.py
+PyFunceble/data/alembic/postgresql/script.py.mako
+PyFunceble/data/alembic/postgresql/versions/__init__.py
+PyFunceble/data/alembic/postgresql/versions/a32ac5d66eee_initial_version.py
 PyFunceble/data/infrastructure/.PyFunceble_production.yaml
 PyFunceble/data/infrastructure/__init__.py
 PyFunceble/data/infrastructure/dir_structure_production.json
 PyFunceble/database/__init__.py
 PyFunceble/database/session.py
 PyFunceble/database/credential/__init__.py
 PyFunceble/database/credential/base.py
 PyFunceble/database/credential/mariadb.py
 PyFunceble/database/credential/mysql.py
+PyFunceble/database/credential/postgresql.py
 PyFunceble/database/schemas/__init__.py
 PyFunceble/database/schemas/autocontinue.py
 PyFunceble/database/schemas/inactive.py
 PyFunceble/database/schemas/status.py
 PyFunceble/database/schemas/whois_record.py
 PyFunceble/database/sqlalchemy/__init__.py
 PyFunceble/database/sqlalchemy/all_schemas.py
 PyFunceble/database/sqlalchemy/base_schema.py
 PyFunceble/dataset/__init__.py
 PyFunceble/dataset/base.py
 PyFunceble/dataset/csv_base.py
 PyFunceble/dataset/db_base.py
 PyFunceble/dataset/iana.py
 PyFunceble/dataset/ipv4_reputation.py
-PyFunceble/dataset/mariadb_base.py
 PyFunceble/dataset/public_suffix.py
+PyFunceble/dataset/sql_base.py
 PyFunceble/dataset/user_agent.py
 PyFunceble/dataset/autocontinue/__init__.py
 PyFunceble/dataset/autocontinue/base.py
 PyFunceble/dataset/autocontinue/csv.py
-PyFunceble/dataset/autocontinue/mariadb.py
-PyFunceble/dataset/autocontinue/mysql.py
+PyFunceble/dataset/autocontinue/sql.py
 PyFunceble/dataset/inactive/__init__.py
 PyFunceble/dataset/inactive/base.py
 PyFunceble/dataset/inactive/csv.py
-PyFunceble/dataset/inactive/mariadb.py
-PyFunceble/dataset/inactive/mysql.py
+PyFunceble/dataset/inactive/sql.py
 PyFunceble/dataset/whois/__init__.py
 PyFunceble/dataset/whois/base.py
 PyFunceble/dataset/whois/csv.py
-PyFunceble/dataset/whois/mariadb.py
-PyFunceble/dataset/whois/mysql.py
+PyFunceble/dataset/whois/sql.py
 PyFunceble/downloader/__init__.py
 PyFunceble/downloader/base.py
 PyFunceble/downloader/exceptions.py
 PyFunceble/downloader/iana.py
 PyFunceble/downloader/ipv4_reputation.py
 PyFunceble/downloader/public_suffix.py
 PyFunceble/downloader/user_agents.py
```

### Comparing `PyFunceble-4.1.3/PyFunceble.egg-info/requires.txt` & `PyFunceble-4.2.0/PyFunceble.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,76 @@
-domain2idna>=1.12.0
-inflection
-PyMySQL
-colorama
-SQLAlchemy~=1.3.20
 packaging
-python-box[all]~=6.0.0
-python-dotenv
-requests[socks]<3
-PyYAML
-cryptography>=3.3.2
 shtab
-setuptools
 alembic
+colorama
 dnspython[doh]~=2.0.0
+domain2idna~=1.12.0
+PyYAML
+inflection
+requests[socks]<3
+cryptography>=3.3.2
+setuptools>=65.5.1
+python-dotenv
+PyMySQL
+python-box[all]~=6.0.0
+SQLAlchemy~=2.0
 
 [dev]
 pylint
-flake8
 black
+flake8
 isort
 
 [docs]
-alabaster<0.8,>=0.7
 sphinx_rtd_theme
-Pygments>=2.0
 sphinx>=3.4.3
+alabaster<0.8,>=0.7
+Pygments>=2.0
 
 [full]
-PyMySQL
+Pygments>=2.0
+alembic
+flake8
+domain2idna~=1.12.0
+PyYAML
 inflection
-colorama
-isort
-coverage
-domain2idna>=1.12.0
+SQLAlchemy~=2.0
 packaging
+pylint
+PyMySQL
 python-box[all]~=6.0.0
 alabaster<0.8,>=0.7
-PyYAML
-flake8
-black
-Pygments>=2.0
-python-dotenv
-requests[socks]<3
+coverage
+dnspython[doh]~=2.0.0
 sphinx_rtd_theme
-cryptography>=3.3.2
-SQLAlchemy~=1.3.20
-alembic
 tox
+isort
+cryptography>=3.3.2
+setuptools>=65.5.1
+python-dotenv
+shtab
+colorama
+black
+requests[socks]<3
 sphinx>=3.4.3
-pylint
+
+[psql]
+packaging
 shtab
-setuptools
+alembic
+colorama
 dnspython[doh]~=2.0.0
+psycopg2
+domain2idna~=1.12.0
+PyYAML
+inflection
+requests[socks]<3
+cryptography>=3.3.2
+setuptools>=65.5.1
+python-dotenv
+PyMySQL
+python-box[all]~=6.0.0
+SQLAlchemy~=2.0
 
 [test]
-coverage
 tox
+coverage
```

### Comparing `PyFunceble-4.1.3/README.rst` & `PyFunceble-4.2.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -154,14 +154,15 @@
 -   Daniel - `@dnmTX`_
 -   gwarser - `@gwarser`_
 -   Haris Gušić - `@veracioux`_
 -   hawkeye116477 - `@hawkeye116477`_
 -   Human Being - `@T145`_
 -   Imre Kristoffer Eilertsen - `@DandelionSprout`_
 -   jawz101 - `@jawz101`_
+-   Josenilson Ferreira da SIlva - `@Nilsonfsilva`_
 -   keczuppp - `@keczuppp`_
 -   kowith337 - `@kowith337`_
 -   Mitchell Krog - `@mitchellkrogza`_
 -   NeolithEra - `@NeolithEra`_
 -   Odyseus - `@Odyseus`_
 -   opav - `@opav`_
 -   Reza Rizqullah - `@ybreza`_
@@ -231,15 +232,15 @@
 
 ___________________________________________
 
 License
 -------
 ::
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -282,14 +283,15 @@
 .. _@hawkeye116477: https://github.com/hawkeye116477
 .. _@jawz101: https://github.com/jawz101
 .. _@keczuppp: https://github.com/keczuppp
 .. _@kennethreitz: https://github.com/kennethreitz
 .. _@kowith337: https://github.com/kowith337
 .. _@mitchellkrogza: https://github.com/mitchellkrogza
 .. _@NeolithEra: https://github.com/NeolithEra
+.. _@Nilsonfsilva: https://github.com/Nilsonfsilva
 .. _@Odyseus: https://github.com/Odyseus
 .. _@opav: https://github.com/opav
 .. _@pi-hole: https://github.com/pi-hole/pi-hole
 .. _@PromoFaux: https://github.com/PromoFaux
 .. _@publicsuffix: https://github.com/publicsuffix
 .. _@rthalley: https://github.com/rthalley
 .. _@rusty-snake: https://github.com/rusty-snake
```

### Comparing `PyFunceble-4.1.3/setup.py` & `PyFunceble-4.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 Project homepage:
     https://pyfunceble.github.io/
 
 License:
 ::
 
 
-    Copyright 2017, 2018, 2019, 2020, 2022 Nissar Chababy
+    Copyright 2017, 2018, 2019, 2020, 2022, 2023 Nissar Chababy
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -136,14 +136,15 @@
     """
 
     mode2files = {
         "standard": ["requirements.txt"],
         "dev": ["requirements.dev.txt"],
         "docs": ["requirements.docs.txt"],
         "test": ["requirements.test.txt"],
+        "psql": ["requirements.txt"],
     }
 
     if is_win_platform():
         for mode, files in mode2files.items():
             new_files = set()
 
             for file in files:
@@ -172,14 +173,17 @@
                     line = line[: line.find("#")].strip()
 
                 if not line:
                     continue
 
                 result.add(line)
 
+    if mode == "psql":
+        result.add("psycopg2")
+
     return list(result)
 
 
 def get_version():
     """
     This function will extract the version from PyFunceble/__init__.py
     """
@@ -207,20 +211,21 @@
     return open("README.rst", encoding="utf-8").read()
 
 
 if __name__ == "__main__":
     setuptools.setup(
         name="PyFunceble",
         version=get_version(),
-        python_requires=">=3.6, <4",
+        python_requires=">=3.8, <4",
         install_requires=get_requirements(mode="standard"),
         extras_require={
             "docs": get_requirements(mode="docs"),
             "dev": get_requirements(mode="dev"),
             "test": get_requirements(mode="test"),
+            "psql": get_requirements(mode="psql"),
             "full": get_requirements(mode="full"),
         },
         description="The tool to check the availability or syntax of domain, IP or URL.",
         long_description=get_long_description(),
         author="funilrys",
         author_email="contact@funilrys.com",
         license="Apache 2.0",
```

