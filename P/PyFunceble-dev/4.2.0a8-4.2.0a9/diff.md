# Comparing `tmp/PyFunceble-dev-4.2.0a8.tar.gz` & `tmp/PyFunceble-dev-4.2.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFunceble-dev-4.2.0a8.tar", last modified: Sat Apr 29 16:43:44 2023, max compression
+gzip compressed data, was "PyFunceble-dev-4.2.0a9.tar", last modified: Sat May 27 11:44:31 2023, max compression
```

## Comparing `PyFunceble-dev-4.2.0a8.tar` & `PyFunceble-dev-4.2.0a9.tar`

### file list

```diff
@@ -1,348 +1,348 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.605258 PyFunceble-dev-4.2.0a8/
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-04-29 16:43:44.605258 PyFunceble-dev-4.2.0a8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.565257 PyFunceble-dev-4.2.0a8/PyFunceble/
--rw-r--r--   0 runner    (1001) docker     (123)    22729 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.565257 PyFunceble-dev-4.2.0a8/PyFunceble/checker/
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.565257 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37672 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/domain_and_ip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.569258 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/parked.py
--rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/subject_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/status.py
--rw-r--r--   0 runner    (1001) docker     (123)    10895 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/url.py
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/complex_json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/params_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.569258 PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/domain_and_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/status_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.569258 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/domain_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/ipv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/ipv6.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/second_lvl_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/subdomain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.573258 PyFunceble-dev-4.2.0a8/PyFunceble/checker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/checker/utils/whois.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.573258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.573258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38941 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/github_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/gitlab_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/jenkins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/travis_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/credential_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.573258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/iana.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/public_suffix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.573258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/pyfunceble/
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/pyfunceble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/pyfunceble/argsparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    45945 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/pyfunceble/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/execution_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/facility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    18211 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/file_preloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.577258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/dir_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.577258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/dir_structure/
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/dir_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/dir_structure/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/dir_structure/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/dir_structure/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/json_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.577258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/printer/
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/printer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/printer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/printer/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/printer/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/registrar_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    24044 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/status_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.577258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/alembic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.577258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/csv_file/
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/csv_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/csv_file/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/csv_file/inactive_source_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/csv_file/whois_registrar_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/db_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.581258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/file_cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/file_cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/file_cleanup/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/file_cleanup/hashes_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/file_cleanup/mining_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/file_cleanup/production_config_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.581258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/json2csv/
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/json2csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/json2csv/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/json2csv/inactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/json2csv/whois.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.581258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/mariadb/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/mariadb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/mariadb/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/mariadb/file_and_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/mariadb/whois_record_idna_subject.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.581258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15645 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/chancy_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/chancy_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/dir_files_sorter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/file_sorter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/migrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/miner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.585258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/chancy_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/chancy_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/dir_files_sorter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/file_sorter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/file_sorter_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/migrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/miner.py
--rw-r--r--   0 runner    (1001) docker     (123)    16601 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.585258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/scripts/iana.py
--rw-r--r--   0 runner    (1001) docker     (123)    17912 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/scripts/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/scripts/public_suffix.py
--rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/storage_facility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.585258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/system/
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/system/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/system/integrator.py
--rw-r--r--   0 runner    (1001) docker     (123)    40349 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/system/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.585258 PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/ascii_logo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13351 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.585258 PyFunceble-dev-4.2.0a8/PyFunceble/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/config/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/config/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.589258 PyFunceble-dev-4.2.0a8/PyFunceble/converter/
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13793 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/converter/adblock_input_line2subject.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/converter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/converter/cidr2subject.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/converter/input_line2subject.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/converter/internal_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/converter/rpz_input_line2subject.py
--rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/converter/rpz_policy2subject.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/converter/subject2complements.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/converter/url2netloc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/converter/wildcard2subject.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.589258 PyFunceble-dev-4.2.0a8/PyFunceble/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.589258 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.589258 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.589258 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/35c79626ecb9_fix_some_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/3a4c55a9320d_add_continue_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/3d6f4a33cdb2_add_inactive_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/45713fea8097_deletion_uneeded_columns_from_whois_.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/459a0d7b8f09_add_idna_subject_column_into_whois.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/6f4729deaf03_delete_inactive_source_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/7bcf7fa64ba1_rename_created_to_created_at_and.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/83ada95132bf_delete_the_file_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/912bbcb77a6c_add_registrar_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/95dc17ddd729_introduction_of_the_session_id_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/ade87195b0a0_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/bef7bcaac3f2_make_id_a_bigint.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/d8893cd406db_allow_whois_record_to_be_empty_null.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/e04e8301d1a2_deletion_of_the_mined_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.593258 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/postgresql/
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/postgresql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/postgresql/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/postgresql/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.593258 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/postgresql/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/postgresql/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/postgresql/versions/a32ac5d66eee_initial_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.593258 PyFunceble-dev-4.2.0a8/PyFunceble/data/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/infrastructure/.PyFunceble_production.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/data/infrastructure/dir_structure_production.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.593258 PyFunceble-dev-4.2.0a8/PyFunceble/database/
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.593258 PyFunceble-dev-4.2.0a8/PyFunceble/database/credential/
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/credential/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/credential/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/credential/mariadb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/credential/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/credential/postgresql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.593258 PyFunceble-dev-4.2.0a8/PyFunceble/database/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/schemas/autocontinue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/schemas/inactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/schemas/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/schemas/whois_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.593258 PyFunceble-dev-4.2.0a8/PyFunceble/database/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/sqlalchemy/all_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/database/sqlalchemy/base_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.597258 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.597258 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/autocontinue/
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/autocontinue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/autocontinue/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/autocontinue/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/autocontinue/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/csv_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/db_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/iana.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.597258 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/inactive/
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/inactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/inactive/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/inactive/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/inactive/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/ipv4_reputation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/public_suffix.py
--rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/sql_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/user_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.597258 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/whois/
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/whois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/whois/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/whois/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/dataset/whois/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.597258 PyFunceble-dev-4.2.0a8/PyFunceble/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/downloader/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/downloader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/downloader/iana.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/downloader/ipv4_reputation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/downloader/public_suffix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/downloader/user_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/facility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.601258 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    13776 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/helpers/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.601258 PyFunceble-dev-4.2.0a8/PyFunceble/query/
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.601258 PyFunceble-dev-4.2.0a8/PyFunceble/query/dns/
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/dns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/dns/nameserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    32788 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/dns/query_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/dns/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/http_status_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.601258 PyFunceble-dev-4.2.0a8/PyFunceble/query/netinfo/
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/netinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/netinfo/address.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/netinfo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/netinfo/hostbyaddr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.601258 PyFunceble-dev-4.2.0a8/PyFunceble/query/record/
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/record/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/record/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/record/whois.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.601258 PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.605258 PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/adapter/
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/adapter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/adapter/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/adapter/https.py
--rw-r--r--   0 runner    (1001) docker     (123)    18035 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/requester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.605258 PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.605258 PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/digit2digits.py
--rw-r--r--   0 runner    (1001) docker     (123)    13419 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/expiration_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/month2unified.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/registrar.py
--rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/query_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/storage_facility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.605258 PyFunceble-dev-4.2.0a8/PyFunceble/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/utils/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/utils/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/PyFunceble/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:43:44.605258 PyFunceble-dev-4.2.0a8/PyFunceble_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-04-29 16:43:44.000000 PyFunceble-dev-4.2.0a8/PyFunceble_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-04-29 16:43:44.000000 PyFunceble-dev-4.2.0a8/PyFunceble_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 16:43:44.000000 PyFunceble-dev-4.2.0a8/PyFunceble_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-29 16:43:44.000000 PyFunceble-dev-4.2.0a8/PyFunceble_dev.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-29 16:43:44.000000 PyFunceble-dev-4.2.0a8/PyFunceble_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 16:43:44.000000 PyFunceble-dev-4.2.0a8/PyFunceble_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/requirements.docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/requirements.test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/requirements.win.txt
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-29 16:43:44.609258 PyFunceble-dev-4.2.0a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-29 16:43:30.000000 PyFunceble-dev-4.2.0a8/version.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.462926 PyFunceble-dev-4.2.0a9/
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12353 2023-05-27 11:44:31.462926 PyFunceble-dev-4.2.0a9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.422926 PyFunceble-dev-4.2.0a9/PyFunceble/
+-rw-r--r--   0 runner    (1001) docker     (123)    22729 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.422926 PyFunceble-dev-4.2.0a9/PyFunceble/checker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.426926 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37672 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/domain_and_ip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.426926 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/parked.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/subject_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10895 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/complex_json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/params_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.426926 PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/domain_and_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/status_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.430926 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/domain_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/second_lvl_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/subdomain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.430926 PyFunceble-dev-4.2.0a9/PyFunceble/checker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/checker/utils/whois.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.430926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.430926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38941 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/github_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/gitlab_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/jenkins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/travis_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/credential_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.430926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/iana.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/public_suffix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.430926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/pyfunceble/
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/pyfunceble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/pyfunceble/argsparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45945 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/pyfunceble/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/execution_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18211 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/file_preloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.434926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/dir_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.434926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/dir_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/dir_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/dir_structure/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/dir_structure/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/dir_structure/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/json_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.434926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/printer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/printer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/printer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/printer/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/printer/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/registrar_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24044 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/status_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.434926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/alembic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.434926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/csv_file/
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/csv_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/csv_file/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/csv_file/inactive_source_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/csv_file/whois_registrar_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/db_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.438926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/file_cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/file_cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/file_cleanup/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/file_cleanup/hashes_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/file_cleanup/mining_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/file_cleanup/production_config_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.438926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/json2csv/
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/json2csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/json2csv/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/json2csv/inactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/json2csv/whois.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.438926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/mariadb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/mariadb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/mariadb/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/mariadb/file_and_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/mariadb/whois_record_idna_subject.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.438926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15645 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/chancy_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/chancy_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/dir_files_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/file_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/migrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/miner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.442926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/chancy_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/chancy_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/dir_files_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/file_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/file_sorter_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/migrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/miner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16601 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.442926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/scripts/iana.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17912 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/scripts/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/scripts/public_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/storage_facility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.442926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/system/
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/system/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/system/integrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40349 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/system/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.442926 PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/ascii_logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13351 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.442926 PyFunceble-dev-4.2.0a9/PyFunceble/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/config/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/config/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.446926 PyFunceble-dev-4.2.0a9/PyFunceble/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13793 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/converter/adblock_input_line2subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/converter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/converter/cidr2subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/converter/input_line2subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/converter/internal_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/converter/rpz_input_line2subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/converter/rpz_policy2subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/converter/subject2complements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/converter/url2netloc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/converter/wildcard2subject.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.446926 PyFunceble-dev-4.2.0a9/PyFunceble/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.446926 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.446926 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.446926 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/35c79626ecb9_fix_some_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/3a4c55a9320d_add_continue_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/3d6f4a33cdb2_add_inactive_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/45713fea8097_deletion_uneeded_columns_from_whois_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/459a0d7b8f09_add_idna_subject_column_into_whois.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/6f4729deaf03_delete_inactive_source_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/7bcf7fa64ba1_rename_created_to_created_at_and.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/83ada95132bf_delete_the_file_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/912bbcb77a6c_add_registrar_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/95dc17ddd729_introduction_of_the_session_id_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/ade87195b0a0_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/bef7bcaac3f2_make_id_a_bigint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/d8893cd406db_allow_whois_record_to_be_empty_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/e04e8301d1a2_deletion_of_the_mined_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.450926 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/postgresql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/postgresql/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/postgresql/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.450926 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/postgresql/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/postgresql/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/postgresql/versions/a32ac5d66eee_initial_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.450926 PyFunceble-dev-4.2.0a9/PyFunceble/data/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/infrastructure/.PyFunceble_production.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/data/infrastructure/dir_structure_production.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.450926 PyFunceble-dev-4.2.0a9/PyFunceble/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.450926 PyFunceble-dev-4.2.0a9/PyFunceble/database/credential/
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/credential/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/credential/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/credential/mariadb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/credential/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/credential/postgresql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.450926 PyFunceble-dev-4.2.0a9/PyFunceble/database/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/schemas/autocontinue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/schemas/inactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/schemas/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/schemas/whois_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.450926 PyFunceble-dev-4.2.0a9/PyFunceble/database/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/sqlalchemy/all_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/database/sqlalchemy/base_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.454926 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.454926 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/autocontinue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/autocontinue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/autocontinue/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/autocontinue/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/autocontinue/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/csv_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/db_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/iana.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.454926 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/inactive/
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/inactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/inactive/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/inactive/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/inactive/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/ipv4_reputation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/public_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/sql_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/user_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.454926 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/whois/
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/whois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/whois/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/whois/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/dataset/whois/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.454926 PyFunceble-dev-4.2.0a9/PyFunceble/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/downloader/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/downloader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/downloader/iana.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/downloader/ipv4_reputation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/downloader/public_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/downloader/user_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.454926 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13776 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/helpers/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.458927 PyFunceble-dev-4.2.0a9/PyFunceble/query/
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.458927 PyFunceble-dev-4.2.0a9/PyFunceble/query/dns/
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/dns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/dns/nameserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32788 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/dns/query_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/dns/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/http_status_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.458927 PyFunceble-dev-4.2.0a9/PyFunceble/query/netinfo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/netinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/netinfo/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/netinfo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/netinfo/hostbyaddr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.458927 PyFunceble-dev-4.2.0a9/PyFunceble/query/record/
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/record/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/record/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/record/whois.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.458927 PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.458927 PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/adapter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/adapter/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/adapter/https.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18035 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/requester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.458927 PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.462926 PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/digit2digits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13419 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/expiration_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/month2unified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/registrar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/query_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/storage_facility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.462926 PyFunceble-dev-4.2.0a9/PyFunceble/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/utils/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/utils/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/PyFunceble/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:44:31.462926 PyFunceble-dev-4.2.0a9/PyFunceble_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12353 2023-05-27 11:44:31.000000 PyFunceble-dev-4.2.0a9/PyFunceble_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-05-27 11:44:31.000000 PyFunceble-dev-4.2.0a9/PyFunceble_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 11:44:31.000000 PyFunceble-dev-4.2.0a9/PyFunceble_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-27 11:44:31.000000 PyFunceble-dev-4.2.0a9/PyFunceble_dev.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-27 11:44:31.000000 PyFunceble-dev-4.2.0a9/PyFunceble_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-27 11:44:31.000000 PyFunceble-dev-4.2.0a9/PyFunceble_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/requirements.docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/requirements.test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/requirements.win.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-27 11:44:31.462926 PyFunceble-dev-4.2.0a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-27 11:44:23.000000 PyFunceble-dev-4.2.0a9/version.yaml
```

### Comparing `PyFunceble-dev-4.2.0a8/CODE_OF_CONDUCT.rst` & `PyFunceble-dev-4.2.0a9/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/CONTRIBUTING.rst` & `PyFunceble-dev-4.2.0a9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/LICENSE` & `PyFunceble-dev-4.2.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PKG-INFO` & `PyFunceble-dev-4.2.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFunceble-dev
-Version: 4.2.0a8
+Version: 4.2.0a9
 Summary: The tool to check the availability or syntax of domain, IP or URL.
 Home-page: https://github.com/funilrys/PyFunceble
 Author: funilrys
 Author-email: contact@funilrys.com
 License: Apache 2.0
 Project-URL: Documentation, https://pyfunceble.readthedocs.io/en/dev/
 Project-URL: Funding, https://github.com/sponsors/funilrys
@@ -183,14 +183,15 @@
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
@@ -311,14 +312,15 @@
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

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/domain.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/domain.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/domain_and_ip.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/domain_and_ip.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/dns.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/dns.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/parked.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/parked.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/rules.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/rules.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/extras/subject_switch.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/extras/subject_switch.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/ip.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/ip.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/params.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/params.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/status.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/status.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/availability/url.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/availability/url.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/complex_json_encoder.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/complex_json_encoder.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/params_base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/params_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/domain.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/domain.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/domain_and_ip.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/domain_and_ip.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/ip.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/ip.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/params.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/params.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/status.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/status.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/reputation/url.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/reputation/url.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/status_base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/status_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/domain.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/domain.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/domain_base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/domain_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/ip.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/ip.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/ipv4.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/ipv4.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/ipv6.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/ipv6.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/params.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/params.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/second_lvl_domain.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/second_lvl_domain.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/status.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/status.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/subdomain.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/subdomain.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/syntax/url.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/syntax/url.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/utils/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/checker/utils/whois.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/checker/utils/whois.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/exceptions.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/github_actions.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/github_actions.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/gitlab_ci.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/gitlab_ci.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/jenkins.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/jenkins.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/travis_ci.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/travis_ci.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/continuous_integration/utils.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/continuous_integration/utils.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/credential_loader.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/credential_loader.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/clean.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/clean.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/iana.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/iana.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/production.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/production.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/public_suffix.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/public_suffix.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/pyfunceble/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/pyfunceble/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/pyfunceble/argsparser.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/pyfunceble/argsparser.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/entry_points/pyfunceble/cli.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/entry_points/pyfunceble/cli.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/execution_time.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/execution_time.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/facility.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/facility.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/factory.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/factory.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/file_preloader.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/file_preloader.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/cleanup.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/cleanup.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/counter.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/counter.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/dir_base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/dir_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/dir_structure/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/dir_structure/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/dir_structure/backup.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/dir_structure/backup.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/dir_structure/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/dir_structure/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/dir_structure/restore.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/dir_structure/restore.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/json_base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/json_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/printer/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/printer/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/printer/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/printer/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/printer/file.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/printer/file.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/printer/stdout.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/printer/stdout.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/registrar_counter.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/registrar_counter.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/filesystem/status_file.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/filesystem/status_file.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/alembic.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/alembic.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/csv_file/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/csv_file/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/csv_file/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/csv_file/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/csv_file/inactive_source_delete.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/csv_file/inactive_source_delete.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/csv_file/whois_registrar_add.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/csv_file/whois_registrar_add.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/db_base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/db_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/file_cleanup/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/file_cleanup/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/file_cleanup/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/file_cleanup/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/file_cleanup/hashes_file.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/file_cleanup/hashes_file.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/file_cleanup/mining_file.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/file_cleanup/mining_file.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/file_cleanup/production_config_file.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/file_cleanup/production_config_file.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/json2csv/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/json2csv/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/json2csv/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/json2csv/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/json2csv/inactive.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/json2csv/inactive.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/json2csv/whois.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/json2csv/whois.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/mariadb/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/mariadb/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/mariadb/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/mariadb/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/mariadb/file_and_status.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/mariadb/file_and_status.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/migrators/mariadb/whois_record_idna_subject.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/migrators/mariadb/whois_record_idna_subject.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/chancy_producer.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/chancy_producer.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/chancy_tester.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/chancy_tester.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/dir_files_sorter.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/dir_files_sorter.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/file_sorter.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/file_sorter.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/migrator.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/migrator.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/miner.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/miner.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/producer.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/producer.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/tester.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/tester.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/chancy_producer.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/chancy_producer.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/chancy_tester.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/chancy_tester.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/dir_files_sorter.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/dir_files_sorter.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/file_sorter.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/file_sorter.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/file_sorter_base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/file_sorter_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/migrator.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/migrator.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/miner.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/miner.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/producer.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/producer.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/processes/workers/tester.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/processes/workers/tester.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/scripts/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/scripts/iana.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/scripts/iana.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/scripts/production.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/scripts/production.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/scripts/public_suffix.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/scripts/public_suffix.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/storage.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/storage.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/storage_facility.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/storage_facility.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/system/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/system/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/system/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/system/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/system/integrator.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/system/integrator.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/system/launcher.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/system/launcher.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/ascii_logo.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/ascii_logo.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/sort.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/sort.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/stdout.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/testing.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/testing.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/cli/utils/version.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/cli/utils/version.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/config/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/config/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/config/compare.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/config/compare.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/config/loader.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/config/loader.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/converter/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/converter/adblock_input_line2subject.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/converter/adblock_input_line2subject.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/converter/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/converter/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/converter/cidr2subject.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/converter/cidr2subject.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/converter/input_line2subject.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/converter/input_line2subject.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/converter/internal_url.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/converter/internal_url.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/converter/rpz_input_line2subject.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/converter/rpz_input_line2subject.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/converter/rpz_policy2subject.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/converter/rpz_policy2subject.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/converter/subject2complements.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/converter/subject2complements.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/converter/url2netloc.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/converter/url2netloc.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/converter/wildcard2subject.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/converter/wildcard2subject.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/env.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/env.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/35c79626ecb9_fix_some_columns.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/35c79626ecb9_fix_some_columns.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/3a4c55a9320d_add_continue_table.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/3a4c55a9320d_add_continue_table.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/3d6f4a33cdb2_add_inactive_table.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/3d6f4a33cdb2_add_inactive_table.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/45713fea8097_deletion_uneeded_columns_from_whois_.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/45713fea8097_deletion_uneeded_columns_from_whois_.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/459a0d7b8f09_add_idna_subject_column_into_whois.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/459a0d7b8f09_add_idna_subject_column_into_whois.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/6f4729deaf03_delete_inactive_source_column.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/6f4729deaf03_delete_inactive_source_column.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/7bcf7fa64ba1_rename_created_to_created_at_and.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/7bcf7fa64ba1_rename_created_to_created_at_and.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/83ada95132bf_delete_the_file_table.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/83ada95132bf_delete_the_file_table.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/912bbcb77a6c_add_registrar_column.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/912bbcb77a6c_add_registrar_column.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/95dc17ddd729_introduction_of_the_session_id_column.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/95dc17ddd729_introduction_of_the_session_id_column.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/ade87195b0a0_base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/ade87195b0a0_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/bef7bcaac3f2_make_id_a_bigint.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/bef7bcaac3f2_make_id_a_bigint.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/d8893cd406db_allow_whois_record_to_be_empty_null.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/d8893cd406db_allow_whois_record_to_be_empty_null.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/mysql/versions/e04e8301d1a2_deletion_of_the_mined_table.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/mysql/versions/e04e8301d1a2_deletion_of_the_mined_table.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/postgresql/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/postgresql/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/postgresql/env.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/postgresql/env.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/postgresql/versions/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/postgresql/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/data/alembic/postgresql/versions/a32ac5d66eee_initial_version.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/data/alembic/postgresql/versions/a32ac5d66eee_initial_version.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/data/infrastructure/.PyFunceble_production.yaml` & `PyFunceble-dev-4.2.0a9/PyFunceble/data/infrastructure/.PyFunceble_production.yaml`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/data/infrastructure/dir_structure_production.json` & `PyFunceble-dev-4.2.0a9/PyFunceble/data/infrastructure/dir_structure_production.json`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/database/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/database/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/database/credential/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/database/credential/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/database/credential/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/database/credential/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/database/credential/mariadb.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/database/credential/mariadb.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/database/credential/mysql.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/database/credential/mysql.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/database/credential/postgresql.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/database/credential/postgresql.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/database/schemas/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/database/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/database/schemas/autocontinue.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/database/schemas/autocontinue.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/database/schemas/inactive.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/database/schemas/inactive.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/database/schemas/status.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/database/schemas/status.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/database/schemas/whois_record.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/database/schemas/whois_record.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/database/session.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/database/session.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/database/sqlalchemy/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/database/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/database/sqlalchemy/all_schemas.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/database/sqlalchemy/all_schemas.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/database/sqlalchemy/base_schema.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/database/sqlalchemy/base_schema.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/autocontinue/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/autocontinue/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/autocontinue/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/autocontinue/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/autocontinue/csv.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/autocontinue/csv.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/autocontinue/sql.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/autocontinue/sql.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/csv_base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/csv_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/db_base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/db_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/iana.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/iana.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/inactive/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/inactive/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/inactive/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/inactive/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/inactive/csv.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/inactive/csv.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/inactive/sql.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/inactive/sql.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/ipv4_reputation.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/ipv4_reputation.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/public_suffix.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/public_suffix.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/sql_base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/sql_base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/user_agent.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/user_agent.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/whois/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/whois/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/whois/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/whois/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/whois/csv.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/whois/csv.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/dataset/whois/sql.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/dataset/whois/sql.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/downloader/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/downloader/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/downloader/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/downloader/exceptions.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/downloader/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/downloader/iana.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/downloader/iana.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/downloader/ipv4_reputation.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/downloader/ipv4_reputation.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/downloader/public_suffix.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/downloader/public_suffix.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/downloader/user_agents.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/downloader/user_agents.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/exceptions.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/facility.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/facility.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/factory.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/factory.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/helpers/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/helpers/command.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/helpers/command.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/helpers/dict.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/helpers/dict.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/helpers/directory.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/helpers/directory.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/helpers/download.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/helpers/download.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/helpers/environment_variable.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/helpers/environment_variable.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/helpers/exceptions.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/helpers/file.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/helpers/file.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/helpers/hash.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/helpers/hash.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/helpers/list.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/helpers/list.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/helpers/merge.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/helpers/merge.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/helpers/regex.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/helpers/regex.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/logger.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/logger.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/collection.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/collection.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/dns/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/dns/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/dns/nameserver.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/dns/nameserver.py`

 * *Files 4% similar despite different names*

```diff
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

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/dns/query_tool.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/dns/query_tool.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/dns/resolver.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/dns/resolver.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/http_status_code.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/http_status_code.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/netinfo/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/netinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/netinfo/address.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/netinfo/address.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/netinfo/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/netinfo/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/netinfo/hostbyaddr.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/netinfo/hostbyaddr.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/record/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/record/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/record/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/record/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/record/dns.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/record/dns.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/record/whois.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/record/whois.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/adapter/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/adapter/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/adapter/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/adapter/http.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/adapter/http.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/adapter/https.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/adapter/https.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/requests/requester.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/requests/requester.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/base.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/base.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/digit2digits.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/digit2digits.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/expiration_date.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/expiration_date.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/month2unified.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/month2unified.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/converter/registrar.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/converter/registrar.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/query/whois/query_tool.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/query/whois/query_tool.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/sessions.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/sessions.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/storage.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 from box import Box
 from dotenv import load_dotenv
 
 from PyFunceble.storage_facility import get_config_directory
 
 PROJECT_NAME: str = "PyFunceble"
-PROJECT_VERSION: str = "4.2.0a8.dev (Blue Duckling: Ixora)"
+PROJECT_VERSION: str = "4.2.0a9.dev (Blue Duckling: Ixora)"
 
 DISTRIBUTED_CONFIGURATION_FILENAME: str = ".PyFunceble_production.yaml"
 DISTRIBUTED_DIR_STRUCTURE_FILENAME: str = "dir_structure_production.json"
 
 IANA_DUMP_FILENAME: str = "iana-domains-db.json"
 PUBLIC_SUFFIX_DUMP_FILENAME: str = "public-suffix.json"
 CONFIGURATION_FILENAME: str = ".PyFunceble.yaml"
```

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/storage_facility.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/storage_facility.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/utils/__init__.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/utils/platform.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/utils/platform.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/utils/profile.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/utils/profile.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble/utils/version.py` & `PyFunceble-dev-4.2.0a9/PyFunceble/utils/version.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble_dev.egg-info/PKG-INFO` & `PyFunceble-dev-4.2.0a9/PyFunceble_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFunceble-dev
-Version: 4.2.0a8
+Version: 4.2.0a9
 Summary: The tool to check the availability or syntax of domain, IP or URL.
 Home-page: https://github.com/funilrys/PyFunceble
 Author: funilrys
 Author-email: contact@funilrys.com
 License: Apache 2.0
 Project-URL: Documentation, https://pyfunceble.readthedocs.io/en/dev/
 Project-URL: Funding, https://github.com/sponsors/funilrys
@@ -183,14 +183,15 @@
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
@@ -311,14 +312,15 @@
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

### Comparing `PyFunceble-dev-4.2.0a8/PyFunceble_dev.egg-info/SOURCES.txt` & `PyFunceble-dev-4.2.0a9/PyFunceble_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/README.rst` & `PyFunceble-dev-4.2.0a9/README.rst`

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

### Comparing `PyFunceble-dev-4.2.0a8/setup.py` & `PyFunceble-dev-4.2.0a9/setup.py`

 * *Files identical despite different names*

### Comparing `PyFunceble-dev-4.2.0a8/version.yaml` & `PyFunceble-dev-4.2.0a9/version.yaml`

 * *Files identical despite different names*

```diff
@@ -1,8 +1,8 @@
-current_version: '4.2.0a8.dev (Blue Duckling: Ixora)'
+current_version: '4.2.0a9.dev (Blue Duckling: Ixora)'
 deprecated:
 - 3.0.21
 - 3.1.20
 - 3.2.13
 - 4.0.0a1
 - 4.1.0b1
 - 4.2.0a1
```

