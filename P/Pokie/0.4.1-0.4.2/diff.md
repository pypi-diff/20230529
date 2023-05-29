# Comparing `tmp/Pokie-0.4.1.tar.gz` & `tmp/Pokie-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pokie-0.4.1.tar", last modified: Mon May 22 13:14:59 2023, max compression
+gzip compressed data, was "Pokie-0.4.2.tar", last modified: Mon May 29 17:00:53 2023, max compression
```

## Comparing `Pokie-0.4.1.tar` & `Pokie-0.4.2.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-22 13:14:26.000000 Pokie-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-22 13:14:26.000000 Pokie-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-22 13:14:59.746138 Pokie-0.4.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.738138 Pokie-0.4.1/Pokie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-22 13:14:59.000000 Pokie-0.4.1/Pokie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-05-22 13:14:59.000000 Pokie-0.4.1/Pokie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:14:59.000000 Pokie-0.4.1/Pokie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:14:59.000000 Pokie-0.4.1/Pokie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-22 13:14:59.000000 Pokie-0.4.1/Pokie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 13:14:59.000000 Pokie-0.4.1/Pokie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-22 13:14:26.000000 Pokie-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.738138 Pokie-0.4.1/pokie/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.738138 Pokie-0.4.1/pokie/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/codegen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/codegen/pg/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/codegen/pg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/codegen/pg/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/codegen/pg/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/codegen/pg/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/codegen/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/codegen/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/codegen/textfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/config/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/auth/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/cli/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/cli/user.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/auth/dto/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/dto/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/dto/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/auth/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/plugin/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/auth/repository/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/repository/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/repository/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/auth/service/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/service/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/service/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/service/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/auth/sql/
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/sql/001-auth-schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/auth/view/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/view/account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/base/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/cli/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/cli/db_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/cli/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/cli/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/cli/pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/cli/tpl_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/base/dto/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/dto/records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/base/job/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/job/idle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/base/repository/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/repository/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/repository/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/repository/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/base/service/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/service/autorest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/service/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/service/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/service/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/contrib/base/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/sql/001-settings.sql
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/sql/002-fixtures.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/contrib/base/validators/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/validators/pk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/contrib/mail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/contrib/mail/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/cli/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/contrib/mail/dto/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/dto/records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/contrib/mail/job/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/job/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/contrib/mail/repository/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/repository/repositories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/contrib/mail/service/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/service/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/service/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/contrib/mail/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/sql/001-mail.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/core/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/core/application.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/core/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/core/factories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/core/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/core/factories/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/core/factories/pgsql.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/core/factories/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/core/module.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/core/signal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/http/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/http/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/http/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/http/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/http/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/http/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/plugins/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/rest/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/rest/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/rest/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/util/cli_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-22 13:14:59.746138 Pokie-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-22 13:14:26.000000 Pokie-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:26.000000 Pokie-0.4.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.130009 Pokie-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-29 17:00:19.000000 Pokie-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-29 17:00:19.000000 Pokie-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-29 17:00:53.130009 Pokie-0.4.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/Pokie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-29 17:00:53.000000 Pokie-0.4.2/Pokie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-05-29 17:00:53.000000 Pokie-0.4.2/Pokie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:00:53.000000 Pokie-0.4.2/Pokie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:00:53.000000 Pokie-0.4.2/Pokie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-29 17:00:53.000000 Pokie-0.4.2/Pokie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 17:00:53.000000 Pokie-0.4.2/Pokie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-29 17:00:19.000000 Pokie-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/codegen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/codegen/pg/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/codegen/pg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/codegen/pg/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/codegen/pg/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/codegen/pg/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/codegen/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/codegen/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/codegen/textfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/config/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/contrib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/contrib/auth/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/cli/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/cli/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/contrib/auth/dto/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/dto/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/dto/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/contrib/auth/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/plugin/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/contrib/auth/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/repository/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/repository/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/contrib/auth/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/service/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/service/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/service/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/contrib/auth/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/sql/001-auth-schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/contrib/auth/view/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/auth/view/account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.122009 Pokie-0.4.2/pokie/contrib/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/base/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/cli/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/cli/db_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/cli/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/cli/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/cli/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/cli/tpl_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/base/dto/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/dto/records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/base/job/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/job/idle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/base/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/repository/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/repository/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/repository/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/base/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/service/autorest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/service/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/service/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/service/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/base/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/sql/001-settings.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/sql/002-fixtures.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/base/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/base/validators/pk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/mail/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/cli/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/mail/dto/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/dto/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/mail/job/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/job/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/mail/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/repository/repositories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/mail/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/service/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/service/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/contrib/mail/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/contrib/mail/sql/001-mail.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.126009 Pokie-0.4.2/pokie/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/core/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.130009 Pokie-0.4.2/pokie/core/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/core/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/core/factories/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/core/factories/pgsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/core/factories/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/core/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/core/signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.130009 Pokie-0.4.2/pokie/http/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/http/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/http/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/http/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/http/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/http/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.130009 Pokie-0.4.2/pokie/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/plugins/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.130009 Pokie-0.4.2/pokie/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/rest/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/rest/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.130009 Pokie-0.4.2/pokie/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-29 17:00:19.000000 Pokie-0.4.2/pokie/util/cli_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-29 17:00:53.130009 Pokie-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-29 17:00:19.000000 Pokie-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:53.130009 Pokie-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:19.000000 Pokie-0.4.2/tests/__init__.py
```

### Comparing `Pokie-0.4.1/LICENSE` & `Pokie-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/PKG-INFO` & `Pokie-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pokie
-Version: 0.4.1
+Version: 0.4.2
 Summary: A high-level Python REST web framework based on Flask, Rick and RickDb.
 Home-page: https://git.oddbit.org/OddBit/pokie
 Author: João Pinheiro
 License: BSD-3-Clause
 Project-URL: Documentation, https://docs.oddbit.org/pokie/
 Project-URL: Source, https://git.oddbit.org/OddBit/pokie
 Classifier: Environment :: Web Environment
```

### Comparing `Pokie-0.4.1/Pokie.egg-info/PKG-INFO` & `Pokie-0.4.2/Pokie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pokie
-Version: 0.4.1
+Version: 0.4.2
 Summary: A high-level Python REST web framework based on Flask, Rick and RickDb.
 Home-page: https://git.oddbit.org/OddBit/pokie
 Author: João Pinheiro
 License: BSD-3-Clause
 Project-URL: Documentation, https://docs.oddbit.org/pokie/
 Project-URL: Source, https://git.oddbit.org/OddBit/pokie
 Classifier: Environment :: Web Environment
```

### Comparing `Pokie-0.4.1/Pokie.egg-info/SOURCES.txt` & `Pokie-0.4.2/Pokie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/README.md` & `Pokie-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/codegen/pg/record.py` & `Pokie-0.4.2/pokie/codegen/pg/record.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/codegen/pg/request.py` & `Pokie-0.4.2/pokie/codegen/pg/request.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/codegen/pg/spec.py` & `Pokie-0.4.2/pokie/codegen/pg/spec.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/codegen/template.py` & `Pokie-0.4.2/pokie/codegen/template.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/codegen/textfile.py` & `Pokie-0.4.2/pokie/codegen/textfile.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/config/template.py` & `Pokie-0.4.2/pokie/config/template.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/constants.py` & `Pokie-0.4.2/pokie/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Version
-POKIE_VERSION = ["0", "4", "1"]
+POKIE_VERSION = ["0", "4", "2"]
 
 
 def get_version():
     return ".".join(POKIE_VERSION)
 
 
 # Http Codes
```

### Comparing `Pokie-0.4.1/pokie/contrib/auth/cli/acl.py` & `Pokie-0.4.2/pokie/contrib/auth/cli/acl.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/auth/cli/user.py` & `Pokie-0.4.2/pokie/contrib/auth/cli/user.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/auth/dto/acl.py` & `Pokie-0.4.2/pokie/contrib/auth/dto/acl.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/auth/module.py` & `Pokie-0.4.2/pokie/contrib/auth/module.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/auth/plugin/db.py` & `Pokie-0.4.2/pokie/contrib/auth/plugin/db.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/auth/repository/acl.py` & `Pokie-0.4.2/pokie/contrib/auth/repository/acl.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/auth/repository/user.py` & `Pokie-0.4.2/pokie/contrib/auth/repository/user.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/auth/service/acl.py` & `Pokie-0.4.2/pokie/contrib/auth/service/acl.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/auth/service/auth.py` & `Pokie-0.4.2/pokie/contrib/auth/service/auth.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/auth/service/user.py` & `Pokie-0.4.2/pokie/contrib/auth/service/user.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/auth/sql/001-auth-schema.sql` & `Pokie-0.4.2/pokie/contrib/auth/sql/001-auth-schema.sql`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/auth/view/account.py` & `Pokie-0.4.2/pokie/contrib/auth/view/account.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/base/cli/base.py` & `Pokie-0.4.2/pokie/contrib/base/cli/base.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/base/cli/db.py` & `Pokie-0.4.2/pokie/contrib/base/cli/db.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/base/cli/db_codegen.py` & `Pokie-0.4.2/pokie/contrib/base/cli/db_codegen.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/base/cli/fixture.py` & `Pokie-0.4.2/pokie/contrib/base/cli/fixture.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/base/cli/job.py` & `Pokie-0.4.2/pokie/contrib/base/cli/job.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/base/cli/tpl_codegen.py` & `Pokie-0.4.2/pokie/contrib/base/cli/tpl_codegen.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/base/module.py` & `Pokie-0.4.2/pokie/contrib/base/module.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/base/repository/settings.py` & `Pokie-0.4.2/pokie/contrib/base/repository/settings.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/base/repository/validator.py` & `Pokie-0.4.2/pokie/contrib/base/repository/validator.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/base/service/autorest.py` & `Pokie-0.4.2/pokie/contrib/base/service/autorest.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/base/service/fixture.py` & `Pokie-0.4.2/pokie/contrib/base/service/fixture.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/base/service/settings.py` & `Pokie-0.4.2/pokie/contrib/base/service/settings.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/base/service/validator.py` & `Pokie-0.4.2/pokie/contrib/base/service/validator.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/base/validators/pk.py` & `Pokie-0.4.2/pokie/contrib/base/validators/pk.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/mail/cli/queue.py` & `Pokie-0.4.2/pokie/contrib/mail/cli/queue.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/mail/dto/records.py` & `Pokie-0.4.2/pokie/contrib/mail/dto/records.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/mail/helpers.py` & `Pokie-0.4.2/pokie/contrib/mail/helpers.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/mail/job/queue.py` & `Pokie-0.4.2/pokie/contrib/mail/job/queue.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/mail/module.py` & `Pokie-0.4.2/pokie/contrib/mail/module.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/mail/repository/repositories.py` & `Pokie-0.4.2/pokie/contrib/mail/repository/repositories.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/mail/service/queue.py` & `Pokie-0.4.2/pokie/contrib/mail/service/queue.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/mail/service/template.py` & `Pokie-0.4.2/pokie/contrib/mail/service/template.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/contrib/mail/sql/001-mail.sql` & `Pokie-0.4.2/pokie/contrib/mail/sql/001-mail.sql`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/core/application.py` & `Pokie-0.4.2/pokie/core/application.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/core/command.py` & `Pokie-0.4.2/pokie/core/command.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/core/factories/login.py` & `Pokie-0.4.2/pokie/core/factories/login.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/core/factories/pgsql.py` & `Pokie-0.4.2/pokie/core/factories/pgsql.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/core/factories/redis.py` & `Pokie-0.4.2/pokie/core/factories/redis.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/core/signal.py` & `Pokie-0.4.2/pokie/core/signal.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/http/helpers.py` & `Pokie-0.4.2/pokie/http/helpers.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/http/rest.py` & `Pokie-0.4.2/pokie/http/rest.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/http/routes.py` & `Pokie-0.4.2/pokie/http/routes.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/http/view.py` & `Pokie-0.4.2/pokie/http/view.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 from typing import Any, Optional, Callable
 from flask import request
 from flask.views import MethodView
 from flask.typing import ResponseReturnValue
-from flask import current_app, jsonify
+from flask import current_app
 from flask_login import current_user
 from rick.serializer.json import ExtendedJsonEncoder
 from rick.form import RequestRecord
 
 from .response import JsonRequestError, JsonStatus
 from pokie.constants import (
     HTTP_OK,
@@ -55,15 +55,15 @@
         # optional override of internal options
         for name, value in kwargs.items():
             attr = getattr(self, name, None)
             if attr is not None and not callable(attr):
                 setattr(self, name, value)
 
     def _hook_request(
-        self, method: str, *args: Any, **kwargs: Any
+            self, method: str, *args: Any, **kwargs: Any
     ) -> Optional[ResponseReturnValue]:
         """
         Dispatch hook: de-serialize request
         If body is not json, will use flask form data
 
         :param method: method name in lowercase
         :param args:
@@ -136,15 +136,15 @@
 
             return current_app.ensure_sync(handler)(*args, **kwargs)
         except Exception as e:
             return self.exception_handler(e)
 
     @classmethod
     def view_method(
-        cls, action_method: str, name=None, *class_args: Any, **class_kwargs: Any
+            cls, action_method: str, name=None, *class_args: Any, **class_kwargs: Any
     ) -> Callable:
         """
         Variant of Flask's as_view that supports custom handlers for actions
         :param action_method: method to be called on dispatch 
         :param name: optional route name
         :param class_args: 
         :param class_kwargs: 
@@ -204,23 +204,23 @@
         :param data:
         :param code:
         :return:
         """
         indent = None
         separators = (",", ":")
 
-        if current_app.config["JSONIFY_PRETTYPRINT_REGULAR"] or current_app.debug:
+        if current_app.json.compact or current_app.debug:
             indent = 2
             separators = (", ", ": ")
 
         data = json.dumps(
             data, indent=indent, separators=separators, cls=ExtendedJsonEncoder
         )
         return current_app.response_class(
-            data, status=code, mimetype=current_app.config["JSONIFY_MIMETYPE"]
+            data, status=code, mimetype=current_app.json.mimetype
         )
 
     def error(self, message=None, code=HTTP_BADREQ):
         data = JsonStatus(
             success=False, message=message if message else "operation failed"
         )
         return self.json(data, code)
@@ -263,15 +263,15 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         # auth first
         self.dispatch_hooks = ["_hook_auth"] + self.dispatch_hooks
         self.user = current_user
 
     def _hook_auth(
-        self, method: str, *args: Any, **kwargs: Any
+            self, method: str, *args: Any, **kwargs: Any
     ) -> Optional[ResponseReturnValue]:
         if not current_user.is_authenticated:
             return self.denied()
 
         for acl in self.acl:
             if not self.user.can_access(acl):
                 return self.forbidden()
```

### Comparing `Pokie-0.4.1/pokie/plugins/auth.py` & `Pokie-0.4.2/pokie/plugins/auth.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/rest/mixin.py` & `Pokie-0.4.2/pokie/rest/mixin.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/rest/service.py` & `Pokie-0.4.2/pokie/rest/service.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/pokie/util/cli_args.py` & `Pokie-0.4.2/pokie/util/cli_args.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.4.1/setup.cfg` & `Pokie-0.4.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 packages = find:
 include_package_data = true
 zip_safe = false
 install_requires = 
 	rick-db>=1.1.2
 	rick>=0.6.0
 	rick-mailer>=1.0.1
-	Flask>=2.2.2
+	Flask>=2.3.0
 	Flask-Login>=0.6.2
 	iso8601>=0.1.16
 	setuptools>=60.0.0
 	tabulate>=0.9.0
 
 [options.extras_require]
 redis = redis
```

