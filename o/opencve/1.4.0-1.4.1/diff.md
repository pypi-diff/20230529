# Comparing `tmp/opencve-1.4.0.tar.gz` & `tmp/opencve-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencve-1.4.0.tar", last modified: Sun Nov  6 08:19:19 2022, max compression
+gzip compressed data, was "opencve-1.4.1.tar", last modified: Mon May 29 07:17:32 2023, max compression
```

## Comparing `opencve-1.4.0.tar` & `opencve-1.4.1.tar`

### file list

```diff
@@ -1,256 +1,256 @@
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:19.041169 opencve-1.4.0/
--rw-r--r--   0 ncrocfer   (501) staff       (20)     4688 2022-11-06 08:14:24.000000 opencve-1.4.0/LICENSE
--rw-r--r--   0 ncrocfer   (501) staff       (20)      111 2021-10-22 17:18:24.000000 opencve-1.4.0/MANIFEST.in
--rw-r--r--   0 ncrocfer   (501) staff       (20)     5302 2022-11-06 08:19:19.040251 opencve-1.4.0/PKG-INFO
--rw-r--r--   0 ncrocfer   (501) staff       (20)     4666 2022-11-05 09:54:17.000000 opencve-1.4.0/README.md
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.658242 opencve-1.4.0/opencve/
--rw-r--r--   0 ncrocfer   (501) staff       (20)        6 2022-11-06 08:14:24.000000 opencve-1.4.0/opencve/VERSION
--rwxr-xr-x   0 ncrocfer   (501) staff       (20)     2276 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/__init__.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     9306 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/admin.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.685153 opencve-1.4.0/opencve/api/
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1887 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/api/__init__.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1201 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/api/alerts.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1276 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/api/base.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1024 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/api/cves.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      912 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/api/cwes.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      858 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/api/fields.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1711 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/api/products.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1221 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/api/reports.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1032 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/api/subscriptions.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1087 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/api/vendors.py
--rwxr-xr-x   0 ncrocfer   (501) staff       (20)      151 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/app.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.693990 opencve-1.4.0/opencve/checks/
--rw-r--r--   0 ncrocfer   (501) staff       (20)      254 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/checks/__init__.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1955 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/checks/cpes.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1204 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/checks/cvss.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1540 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/checks/cwes.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      615 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/checks/first_time.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1862 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/checks/references.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      778 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/checks/summary.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      653 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/cli.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.702327 opencve-1.4.0/opencve/commands/
--rw-r--r--   0 ncrocfer   (501) staff       (20)      932 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/commands/__init__.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      776 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/commands/celery.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1232 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/commands/create_user.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.707435 opencve-1.4.0/opencve/commands/imports/
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1329 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/commands/imports/__init__.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2307 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/commands/imports/cpe.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     4667 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/commands/imports/cve.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1525 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/commands/imports/cwe.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1238 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/commands/init.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      386 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/commands/upgrade_db.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     3994 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/commands/utils.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      416 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/commands/webserver.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      863 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/configuration.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      936 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/constants.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     5608 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/context.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.725276 opencve-1.4.0/opencve/controllers/
--rw-r--r--   0 ncrocfer   (501) staff       (20)      354 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/controllers/__init__.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      581 2022-11-05 09:54:24.000000 opencve-1.4.0/opencve/controllers/alerts.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1899 2022-11-05 09:54:24.000000 opencve-1.4.0/opencve/controllers/base.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     4931 2022-11-05 09:54:24.000000 opencve-1.4.0/opencve/controllers/cves.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      901 2022-11-05 09:54:24.000000 opencve-1.4.0/opencve/controllers/cwes.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     3249 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/controllers/home.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2149 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/controllers/main.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1716 2022-11-05 09:54:24.000000 opencve-1.4.0/opencve/controllers/products.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      747 2022-11-05 09:54:24.000000 opencve-1.4.0/opencve/controllers/reports.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2964 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/controllers/subscriptions.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      475 2022-11-05 09:54:24.000000 opencve-1.4.0/opencve/controllers/tags.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      748 2022-11-05 09:54:24.000000 opencve-1.4.0/opencve/controllers/vendors.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2149 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/default.cfg
--rw-r--r--   0 ncrocfer   (501) staff       (20)     3255 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/extensions.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     3567 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/forms.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.730094 opencve-1.4.0/opencve/migrations/
--rwxr-xr-x   0 ncrocfer   (501) staff       (20)       38 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/migrations/README
--rw-r--r--   0 ncrocfer   (501) staff       (20)      770 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/migrations/alembic.ini
--rwxr-xr-x   0 ncrocfer   (501) staff       (20)     2807 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/migrations/env.py
--rwxr-xr-x   0 ncrocfer   (501) staff       (20)      412 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/migrations/script.py.mako
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.741587 opencve-1.4.0/opencve/migrations/versions/
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1933 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/migrations/versions/1c7aecfc5f6e_add_indexes_cascade_deletions_reports.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      856 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/migrations/versions/2132d05ea0e2_add_first_time_value_in_event_types_enum.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1382 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/migrations/versions/33cd640e1112_add_indexes_on_cves_summary_and_cve_cve_.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      642 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/migrations/versions/3f755e0484e0_add_settings_columns_in_users_table.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2561 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/migrations/versions/4195eeb432e9_add_tags_tables.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      755 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/migrations/versions/41ad8e9163d4_make_cwe_cwe_id_field_not_nullable.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)    12752 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/migrations/versions/8bdc527d8d49_initial_migration.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1409 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/migrations/versions/f81abceece3d_synchronize_null_cvss_for_existing_cves.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.763457 opencve-1.4.0/opencve/models/
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1875 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/models/__init__.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      973 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/models/alerts.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      563 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/models/changes.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2766 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/models/cve.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      487 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/models/cwe.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      826 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/models/events.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      296 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/models/metas.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      678 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/models/products.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      867 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/models/reports.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1270 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/models/tags.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      284 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/models/tasks.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2689 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/models/users.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      557 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/models/vendors.py
--rwxr-xr-x   0 ncrocfer   (501) staff       (20)     7491 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/settings.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.624915 opencve-1.4.0/opencve/static/
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.776795 opencve-1.4.0/opencve/static/css/
--rw-r--r--   0 ncrocfer   (501) staff       (20)    91501 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/css/AdminLTE.min.css
--rw-r--r--   0 ncrocfer   (501) staff       (20)   121457 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/css/bootstrap.min.css
--rw-r--r--   0 ncrocfer   (501) staff       (20)     6216 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/css/custom.css
--rw-r--r--   0 ncrocfer   (501) staff       (20)    31000 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/css/font-awesome.min.css
--rw-r--r--   0 ncrocfer   (501) staff       (20)    14954 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/css/select2.min.css
--rw-r--r--   0 ncrocfer   (501) staff       (20)     3156 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/css/skin-blue.min.css
--rw-r--r--   0 ncrocfer   (501) staff       (20)    10464 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/css/spectrum.min.css
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.813941 opencve-1.4.0/opencve/static/fonts/
--rw-r--r--   0 ncrocfer   (501) staff       (20)   134808 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/fonts/FontAwesome.otf
--rw-r--r--   0 ncrocfer   (501) staff       (20)   165742 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/fonts/fontawesome-webfont.eot
--rw-r--r--   0 ncrocfer   (501) staff       (20)   444379 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/fonts/fontawesome-webfont.svg
--rw-r--r--   0 ncrocfer   (501) staff       (20)   165548 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 ncrocfer   (501) staff       (20)    98024 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/fonts/fontawesome-webfont.woff
--rw-r--r--   0 ncrocfer   (501) staff       (20)    77160 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 ncrocfer   (501) staff       (20)    20127 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 ncrocfer   (501) staff       (20)   108738 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 ncrocfer   (501) staff       (20)    45404 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 ncrocfer   (501) staff       (20)    23424 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 ncrocfer   (501) staff       (20)    18028 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.837374 opencve-1.4.0/opencve/static/img/
--rw-r--r--   0 ncrocfer   (501) staff       (20)   362221 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/img/deep-green.jpg
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1150 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/img/favicon.ico
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1780 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/img/logo_full_48.png
--rw-r--r--   0 ncrocfer   (501) staff       (20)      592 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/img/logo_white.png
--rw-r--r--   0 ncrocfer   (501) staff       (20)      604 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/img/mail_icon.png
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.881484 opencve-1.4.0/opencve/static/js/
--rw-r--r--   0 ncrocfer   (501) staff       (20)    14717 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/js/adminlte.min.js
--rw-r--r--   0 ncrocfer   (501) staff       (20)    39680 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/js/bootstrap.min.js
--rw-r--r--   0 ncrocfer   (501) staff       (20)   207839 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/js/chart.min.js
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1411 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/js/custom.js
--rw-r--r--   0 ncrocfer   (501) staff       (20)    86927 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/js/jquery.min.js
--rw-r--r--   0 ncrocfer   (501) staff       (20)     6842 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/js/jquery.rainbowJSON.js
--rw-r--r--   0 ncrocfer   (501) staff       (20)    76652 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/js/select2.full.min.js
--rw-r--r--   0 ncrocfer   (501) staff       (20)    27903 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/static/js/spectrum.min.js
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.888194 opencve-1.4.0/opencve/tasks/
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1651 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/tasks/__init__.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     4895 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/tasks/alerts.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     3365 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/tasks/events.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     6380 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/tasks/reports.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.909325 opencve-1.4.0/opencve/templates/
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.912752 opencve-1.4.0/opencve/templates/_includes/
--rw-r--r--   0 ncrocfer   (501) staff       (20)     3740 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/_includes/cvss2.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)     4627 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/_includes/cvss3.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)      563 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/_macros.html
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.919540 opencve-1.4.0/opencve/templates/_welcome/
--rw-r--r--   0 ncrocfer   (501) staff       (20)       63 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/_welcome/analytics.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)      631 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/_welcome/base_welcome.html
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.921128 opencve-1.4.0/opencve/templates/_welcome/css/
--rw-r--r--   0 ncrocfer   (501) staff       (20)      113 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/_welcome/css/style.css
--rw-r--r--   0 ncrocfer   (501) staff       (20)      676 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/_welcome/index.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)      420 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/_welcome/terms.html
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.925912 opencve-1.4.0/opencve/templates/admin/
--rw-r--r--   0 ncrocfer   (501) staff       (20)     4489 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/admin/index.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)      861 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/admin/task.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)      524 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/admin/tasks.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)    10276 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/base.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1413 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/base_blank.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2114 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/change.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)    15009 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/cve.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)    12235 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/cves.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)     4048 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/cwes.html
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.931402 opencve-1.4.0/opencve/templates/emails/
--rw-r--r--   0 ncrocfer   (501) staff       (20)    37115 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/emails/report_message.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)      897 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/emails/report_message.txt
--rw-r--r--   0 ncrocfer   (501) staff       (20)       13 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/emails/report_subject.txt
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.932834 opencve-1.4.0/opencve/templates/errors/
--rw-r--r--   0 ncrocfer   (501) staff       (20)      490 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/errors/404.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)      388 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/flash_messages.html
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.942958 opencve-1.4.0/opencve/templates/flask_user/
--rw-r--r--   0 ncrocfer   (501) staff       (20)      823 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/flask_user/change_password.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)      878 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/flask_user/edit_user_profile.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1098 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/flask_user/forgot_password.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1547 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/flask_user/login.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1830 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/flask_user/register.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1089 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/flask_user/resend_confirm_email.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)    14160 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/home.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)      516 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/messages.html
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.952798 opencve-1.4.0/opencve/templates/profiles/
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1823 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/profiles/base_profile.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)      845 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/profiles/delete_tag.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)     5135 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/profiles/notifications.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)      905 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/profiles/settings.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)     4171 2022-11-05 10:01:08.000000 opencve-1.4.0/opencve/templates/profiles/subscriptions.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)     3948 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/profiles/tags.html
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.963093 opencve-1.4.0/opencve/templates/report/
--rw-r--r--   0 ncrocfer   (501) staff       (20)      203 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/report/cpes_details.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)      403 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/report/cvss_details.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)      203 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/report/cwes_details.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)      240 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/report/first_time_details.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)       55 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/report/new_cve_details.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)      954 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/report/references_details.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)      155 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/report/summary_details.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)     3695 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/report.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1781 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/reports.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)     8176 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/templates/vendors.html
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2343 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/utils.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.970754 opencve-1.4.0/opencve/views/
--rw-r--r--   0 ncrocfer   (501) staff       (20)        0 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/views/__init__.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     3924 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/views/cves.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      359 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/views/cwes.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     6766 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/views/profile.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2270 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/views/reports.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      560 2022-11-05 09:54:17.000000 opencve-1.4.0/opencve/views/vendors.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.672785 opencve-1.4.0/opencve.egg-info/
--rw-r--r--   0 ncrocfer   (501) staff       (20)     5302 2022-11-06 08:19:18.000000 opencve-1.4.0/opencve.egg-info/PKG-INFO
--rw-r--r--   0 ncrocfer   (501) staff       (20)     7125 2022-11-06 08:19:18.000000 opencve-1.4.0/opencve.egg-info/SOURCES.txt
--rw-r--r--   0 ncrocfer   (501) staff       (20)        1 2022-11-06 08:19:18.000000 opencve-1.4.0/opencve.egg-info/dependency_links.txt
--rw-r--r--   0 ncrocfer   (501) staff       (20)       44 2022-11-06 08:19:18.000000 opencve-1.4.0/opencve.egg-info/entry_points.txt
--rw-r--r--   0 ncrocfer   (501) staff       (20)      778 2022-11-06 08:19:18.000000 opencve-1.4.0/opencve.egg-info/requires.txt
--rw-r--r--   0 ncrocfer   (501) staff       (20)       14 2022-11-06 08:19:18.000000 opencve-1.4.0/opencve.egg-info/top_level.txt
--rw-r--r--   0 ncrocfer   (501) staff       (20)      838 2022-11-05 09:54:17.000000 opencve-1.4.0/requirements.txt
--rw-r--r--   0 ncrocfer   (501) staff       (20)       38 2022-11-06 08:19:19.041473 opencve-1.4.0/setup.cfg
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1444 2022-11-05 09:54:17.000000 opencve-1.4.0/setup.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.981453 opencve-1.4.0/tests/
--rw-r--r--   0 ncrocfer   (501) staff       (20)        0 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/__init__.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:18.993676 opencve-1.4.0/tests/api/
--rw-r--r--   0 ncrocfer   (501) staff       (20)        0 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/api/__init__.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     3184 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/api/test_alerts.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2322 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/api/test_cves.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2125 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/api/test_cwes.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     3606 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/api/test_products.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1345 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/api/test_ratelimit.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     3370 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/api/test_reports.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2226 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/api/test_subscriptions.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2154 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/api/test_vendors.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:19.002218 opencve-1.4.0/tests/commands/
--rw-r--r--   0 ncrocfer   (501) staff       (20)        0 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/commands/__init__.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1116 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/commands/test_celery.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2320 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/commands/test_create_user.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      614 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/commands/test_upgrade_db.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     3360 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/commands/test_utils.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      580 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/commands/test_webserver.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     6094 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/conftest.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:19.017970 opencve-1.4.0/tests/controllers/
--rw-r--r--   0 ncrocfer   (501) staff       (20)        0 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/controllers/__init__.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2644 2022-11-05 09:54:24.000000 opencve-1.4.0/tests/controllers/test_base.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     6741 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/controllers/test_cves.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1651 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/controllers/test_cwes.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2204 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/controllers/test_products.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     3098 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/controllers/test_reports.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     5791 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/controllers/test_subscriptions.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2604 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/controllers/test_tags.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1716 2022-11-05 09:54:17.000000 opencve-1.4.0/tests/controllers/test_vendors.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:19.024525 opencve-1.4.0/tests/tasks/
--rw-r--r--   0 ncrocfer   (501) staff       (20)        0 2022-11-05 09:54:18.000000 opencve-1.4.0/tests/tasks/__init__.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     9408 2022-11-05 09:54:18.000000 opencve-1.4.0/tests/tasks/test_alerts.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2922 2022-11-05 09:54:18.000000 opencve-1.4.0/tests/tasks/test_events.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     8583 2022-11-05 09:54:18.000000 opencve-1.4.0/tests/tasks/test_reports.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1036 2022-11-05 09:54:18.000000 opencve-1.4.0/tests/test_admin.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2589 2022-11-05 09:54:18.000000 opencve-1.4.0/tests/test_context.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     3722 2022-11-05 09:54:18.000000 opencve-1.4.0/tests/test_models.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      115 2022-11-05 09:54:18.000000 opencve-1.4.0/tests/test_settings.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2087 2022-11-05 09:54:18.000000 opencve-1.4.0/tests/test_users.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     3202 2022-11-05 09:54:18.000000 opencve-1.4.0/tests/test_utils.py
-drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2022-11-06 08:19:19.038610 opencve-1.4.0/tests/views/
--rw-r--r--   0 ncrocfer   (501) staff       (20)        0 2022-11-05 09:54:18.000000 opencve-1.4.0/tests/views/__init__.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     3545 2022-11-05 09:54:18.000000 opencve-1.4.0/tests/views/test_cves.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)      745 2022-11-05 09:54:18.000000 opencve-1.4.0/tests/views/test_cwes.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     6542 2022-11-05 09:54:18.000000 opencve-1.4.0/tests/views/test_home.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     1634 2022-11-05 09:54:18.000000 opencve-1.4.0/tests/views/test_profile.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     2222 2022-11-05 09:54:18.000000 opencve-1.4.0/tests/views/test_reports.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     6501 2022-11-05 09:54:18.000000 opencve-1.4.0/tests/views/test_tags.py
--rw-r--r--   0 ncrocfer   (501) staff       (20)     4631 2022-11-05 09:54:18.000000 opencve-1.4.0/tests/views/test_vendors.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.760810 opencve-1.4.1/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     4688 2023-05-29 07:16:53.000000 opencve-1.4.1/LICENSE
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      111 2021-10-22 17:18:24.000000 opencve-1.4.1/MANIFEST.in
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     5302 2023-05-29 07:17:32.760004 opencve-1.4.1/PKG-INFO
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     4666 2023-05-29 07:16:47.000000 opencve-1.4.1/README.md
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.377554 opencve-1.4.1/opencve/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)        6 2023-05-29 07:16:53.000000 opencve-1.4.1/opencve/VERSION
+-rwxr-xr-x   0 ncrocfer   (501) staff       (20)     2276 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/__init__.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     9306 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/admin.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.411220 opencve-1.4.1/opencve/api/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1887 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/api/__init__.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1201 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/api/alerts.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1276 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/api/base.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1024 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/api/cves.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      912 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/api/cwes.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      858 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/api/fields.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1711 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/api/products.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1221 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/api/reports.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1032 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/api/subscriptions.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1087 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/api/vendors.py
+-rwxr-xr-x   0 ncrocfer   (501) staff       (20)      151 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/app.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.424576 opencve-1.4.1/opencve/checks/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      254 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/checks/__init__.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1955 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/checks/cpes.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1204 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/checks/cvss.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1540 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/checks/cwes.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      615 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/checks/first_time.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1862 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/checks/references.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      778 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/checks/summary.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      653 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/cli.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.440181 opencve-1.4.1/opencve/commands/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      932 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/commands/__init__.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      776 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/commands/celery.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1232 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/commands/create_user.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.457157 opencve-1.4.1/opencve/commands/imports/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1329 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/commands/imports/__init__.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2307 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/commands/imports/cpe.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     4667 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/commands/imports/cve.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1525 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/commands/imports/cwe.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1238 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/commands/init.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      386 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/commands/upgrade_db.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     3994 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/commands/utils.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      416 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/commands/webserver.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      863 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/configuration.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      936 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/constants.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     5608 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/context.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.514585 opencve-1.4.1/opencve/controllers/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      354 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/controllers/__init__.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      581 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/controllers/alerts.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1899 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/controllers/base.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     4931 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/controllers/cves.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      901 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/controllers/cwes.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     3249 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/controllers/home.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2149 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/controllers/main.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1716 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/controllers/products.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      747 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/controllers/reports.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2964 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/controllers/subscriptions.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      475 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/controllers/tags.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      748 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/controllers/vendors.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2149 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/default.cfg
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     3255 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/extensions.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     3567 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/forms.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.521047 opencve-1.4.1/opencve/migrations/
+-rwxr-xr-x   0 ncrocfer   (501) staff       (20)       38 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/migrations/README
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      770 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/migrations/alembic.ini
+-rwxr-xr-x   0 ncrocfer   (501) staff       (20)     2807 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/migrations/env.py
+-rwxr-xr-x   0 ncrocfer   (501) staff       (20)      412 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/migrations/script.py.mako
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.534054 opencve-1.4.1/opencve/migrations/versions/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1933 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/migrations/versions/1c7aecfc5f6e_add_indexes_cascade_deletions_reports.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      856 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/migrations/versions/2132d05ea0e2_add_first_time_value_in_event_types_enum.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1382 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/migrations/versions/33cd640e1112_add_indexes_on_cves_summary_and_cve_cve_.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      642 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/migrations/versions/3f755e0484e0_add_settings_columns_in_users_table.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2561 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/migrations/versions/4195eeb432e9_add_tags_tables.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      755 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/migrations/versions/41ad8e9163d4_make_cwe_cwe_id_field_not_nullable.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    12752 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/migrations/versions/8bdc527d8d49_initial_migration.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1409 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/migrations/versions/f81abceece3d_synchronize_null_cvss_for_existing_cves.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.554437 opencve-1.4.1/opencve/models/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1875 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/models/__init__.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      973 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/models/alerts.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      563 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/models/changes.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2766 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/models/cve.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      487 2023-05-29 07:16:47.000000 opencve-1.4.1/opencve/models/cwe.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      826 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/models/events.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      296 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/models/metas.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      678 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/models/products.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      867 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/models/reports.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1270 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/models/tags.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      284 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/models/tasks.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2689 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/models/users.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      557 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/models/vendors.py
+-rwxr-xr-x   0 ncrocfer   (501) staff       (20)     7491 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/settings.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.317997 opencve-1.4.1/opencve/static/
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.566216 opencve-1.4.1/opencve/static/css/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    91501 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/css/AdminLTE.min.css
+-rw-r--r--   0 ncrocfer   (501) staff       (20)   121457 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/css/bootstrap.min.css
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     6216 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/css/custom.css
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    31000 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/css/font-awesome.min.css
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    14954 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/css/select2.min.css
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     3156 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/css/skin-blue.min.css
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    10464 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/css/spectrum.min.css
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.586285 opencve-1.4.1/opencve/static/fonts/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)   134808 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/fonts/FontAwesome.otf
+-rw-r--r--   0 ncrocfer   (501) staff       (20)   165742 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 ncrocfer   (501) staff       (20)   444379 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 ncrocfer   (501) staff       (20)   165548 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    98024 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    77160 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    20127 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 ncrocfer   (501) staff       (20)   108738 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    45404 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    23424 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    18028 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.595877 opencve-1.4.1/opencve/static/img/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)   362221 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/img/deep-green.jpg
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1150 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/img/favicon.ico
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1780 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/img/logo_full_48.png
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      592 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/img/logo_white.png
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      604 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/img/mail_icon.png
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.610077 opencve-1.4.1/opencve/static/js/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    14717 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/js/adminlte.min.js
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    39680 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/js/bootstrap.min.js
+-rw-r--r--   0 ncrocfer   (501) staff       (20)   207839 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/js/chart.min.js
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1411 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/js/custom.js
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    86927 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/js/jquery.min.js
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     6842 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/js/jquery.rainbowJSON.js
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    76652 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/js/select2.full.min.js
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    27903 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/static/js/spectrum.min.js
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.616299 opencve-1.4.1/opencve/tasks/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1651 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/tasks/__init__.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     4895 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/tasks/alerts.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     3365 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/tasks/events.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     6380 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/tasks/reports.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.637019 opencve-1.4.1/opencve/templates/
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.639808 opencve-1.4.1/opencve/templates/_includes/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     3740 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/_includes/cvss2.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     4627 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/_includes/cvss3.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      563 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/_macros.html
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.646620 opencve-1.4.1/opencve/templates/_welcome/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)       63 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/_welcome/analytics.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      631 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/_welcome/base_welcome.html
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.648074 opencve-1.4.1/opencve/templates/_welcome/css/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      113 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/_welcome/css/style.css
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      676 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/_welcome/index.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      420 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/_welcome/terms.html
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.652347 opencve-1.4.1/opencve/templates/admin/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     4489 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/admin/index.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      861 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/admin/task.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      524 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/admin/tasks.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    10276 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/base.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1413 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/base_blank.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2114 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/change.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    15284 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/cve.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    12235 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/cves.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     4048 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/cwes.html
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.656605 opencve-1.4.1/opencve/templates/emails/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    37121 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/emails/report_message.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      897 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/emails/report_message.txt
+-rw-r--r--   0 ncrocfer   (501) staff       (20)       13 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/emails/report_subject.txt
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.657937 opencve-1.4.1/opencve/templates/errors/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      490 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/errors/404.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      388 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/flash_messages.html
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.667574 opencve-1.4.1/opencve/templates/flask_user/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      823 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/flask_user/change_password.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      878 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/flask_user/edit_user_profile.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1098 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/flask_user/forgot_password.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1547 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/flask_user/login.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1830 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/flask_user/register.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1089 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/flask_user/resend_confirm_email.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)    14160 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/home.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      516 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/messages.html
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.676319 opencve-1.4.1/opencve/templates/profiles/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1823 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/profiles/base_profile.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      845 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/profiles/delete_tag.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     5135 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/profiles/notifications.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      905 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/profiles/settings.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     4171 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/profiles/subscriptions.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     3948 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/profiles/tags.html
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.686273 opencve-1.4.1/opencve/templates/report/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      203 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/report/cpes_details.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      403 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/report/cvss_details.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      203 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/report/cwes_details.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      240 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/report/first_time_details.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)       55 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/report/new_cve_details.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      954 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/report/references_details.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      155 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/report/summary_details.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     3695 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/report.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1781 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/reports.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     8176 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/templates/vendors.html
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2343 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/utils.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.694906 opencve-1.4.1/opencve/views/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/views/__init__.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     3924 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/views/cves.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      359 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/views/cwes.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     6766 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/views/profile.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2270 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/views/reports.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      560 2023-05-29 07:16:48.000000 opencve-1.4.1/opencve/views/vendors.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.389739 opencve-1.4.1/opencve.egg-info/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     5302 2023-05-29 07:17:31.000000 opencve-1.4.1/opencve.egg-info/PKG-INFO
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     7125 2023-05-29 07:17:32.000000 opencve-1.4.1/opencve.egg-info/SOURCES.txt
+-rw-r--r--   0 ncrocfer   (501) staff       (20)        1 2023-05-29 07:17:31.000000 opencve-1.4.1/opencve.egg-info/dependency_links.txt
+-rw-r--r--   0 ncrocfer   (501) staff       (20)       44 2023-05-29 07:17:31.000000 opencve-1.4.1/opencve.egg-info/entry_points.txt
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      778 2023-05-29 07:17:31.000000 opencve-1.4.1/opencve.egg-info/requires.txt
+-rw-r--r--   0 ncrocfer   (501) staff       (20)       14 2023-05-29 07:17:31.000000 opencve-1.4.1/opencve.egg-info/top_level.txt
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      838 2023-05-29 07:16:48.000000 opencve-1.4.1/requirements.txt
+-rw-r--r--   0 ncrocfer   (501) staff       (20)       38 2023-05-29 07:17:32.761030 opencve-1.4.1/setup.cfg
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1444 2023-05-29 07:16:48.000000 opencve-1.4.1/setup.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.706298 opencve-1.4.1/tests/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/__init__.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.718954 opencve-1.4.1/tests/api/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/api/__init__.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     3184 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/api/test_alerts.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2322 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/api/test_cves.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2125 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/api/test_cwes.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     3606 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/api/test_products.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1345 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/api/test_ratelimit.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     3370 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/api/test_reports.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2226 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/api/test_subscriptions.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2154 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/api/test_vendors.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.728515 opencve-1.4.1/tests/commands/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/commands/__init__.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1116 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/commands/test_celery.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2320 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/commands/test_create_user.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      614 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/commands/test_upgrade_db.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     3360 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/commands/test_utils.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      580 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/commands/test_webserver.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     6094 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/conftest.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.741545 opencve-1.4.1/tests/controllers/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/controllers/__init__.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2644 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/controllers/test_base.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     6741 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/controllers/test_cves.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1651 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/controllers/test_cwes.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2204 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/controllers/test_products.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     3098 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/controllers/test_reports.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     5791 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/controllers/test_subscriptions.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2604 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/controllers/test_tags.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1716 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/controllers/test_vendors.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.746333 opencve-1.4.1/tests/tasks/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/tasks/__init__.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     9408 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/tasks/test_alerts.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2922 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/tasks/test_events.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     8583 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/tasks/test_reports.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1036 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/test_admin.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2589 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/test_context.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     3722 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/test_models.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      115 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/test_settings.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2087 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/test_users.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     3202 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/test_utils.py
+drwxr-xr-x   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:17:32.758683 opencve-1.4.1/tests/views/
+-rw-r--r--   0 ncrocfer   (501) staff       (20)        0 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/views/__init__.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     3545 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/views/test_cves.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)      745 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/views/test_cwes.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     6542 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/views/test_home.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     1634 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/views/test_profile.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     2222 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/views/test_reports.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     6501 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/views/test_tags.py
+-rw-r--r--   0 ncrocfer   (501) staff       (20)     4631 2023-05-29 07:16:48.000000 opencve-1.4.1/tests/views/test_vendors.py
```

### Comparing `opencve-1.4.0/LICENSE` & `opencve-1.4.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
                       A "Security Monitoring and Alerting Service" is a commercial
                       offering that allows third parties (other than your employees
                       and contractors) to access the functionality of the Licensed
                       Work so that such third parties directly benefit from the
                       security monitoring and alerting features of the Licensed Work.
 
-Change Date:          2025-11-05
+Change Date:          2026-05-26
 
 Change License:       Apache License, Version 2.0
 
 For information about alternative licensing arrangements for the Software,
 please visit: https://www.opencve.io/
 
 Notice
```

### Comparing `opencve-1.4.0/PKG-INFO` & `opencve-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencve
-Version: 1.4.0
+Version: 1.4.1
 Summary: CVE Alerting Platform
 Home-page: https://github.com/opencve/opencve
 Author: Nicolas Crocfer
 Author-email: ncrocfer@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opencve Version: 1.4.0 Summary: CVE Alerting
+Metadata-Version: 2.1 Name: opencve Version: 1.4.1 Summary: CVE Alerting
 Platform Home-page: https://github.com/opencve/opencve Author: Nicolas Crocfer
 Author-email: ncrocfer@gmail.com Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Requires-Python: >=3.7
 Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
```

### Comparing `opencve-1.4.0/README.md` & `opencve-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/__init__.py` & `opencve-1.4.1/opencve/__init__.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/admin.py` & `opencve-1.4.1/opencve/admin.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/api/__init__.py` & `opencve-1.4.1/opencve/api/__init__.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/api/alerts.py` & `opencve-1.4.1/opencve/api/alerts.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/api/base.py` & `opencve-1.4.1/opencve/api/base.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/api/cves.py` & `opencve-1.4.1/opencve/api/cves.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/api/cwes.py` & `opencve-1.4.1/opencve/api/cwes.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/api/fields.py` & `opencve-1.4.1/opencve/api/fields.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/api/products.py` & `opencve-1.4.1/opencve/api/products.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/api/reports.py` & `opencve-1.4.1/opencve/api/reports.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/api/subscriptions.py` & `opencve-1.4.1/opencve/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/api/vendors.py` & `opencve-1.4.1/opencve/api/vendors.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/checks/cpes.py` & `opencve-1.4.1/opencve/checks/cpes.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/checks/cvss.py` & `opencve-1.4.1/opencve/checks/cvss.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/checks/cwes.py` & `opencve-1.4.1/opencve/checks/cwes.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/checks/first_time.py` & `opencve-1.4.1/opencve/checks/first_time.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/checks/references.py` & `opencve-1.4.1/opencve/checks/references.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/checks/summary.py` & `opencve-1.4.1/opencve/checks/summary.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/cli.py` & `opencve-1.4.1/opencve/cli.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/commands/__init__.py` & `opencve-1.4.1/opencve/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/commands/celery.py` & `opencve-1.4.1/opencve/commands/celery.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/commands/create_user.py` & `opencve-1.4.1/opencve/commands/create_user.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/commands/imports/__init__.py` & `opencve-1.4.1/opencve/commands/imports/__init__.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/commands/imports/cpe.py` & `opencve-1.4.1/opencve/commands/imports/cpe.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/commands/imports/cve.py` & `opencve-1.4.1/opencve/commands/imports/cve.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/commands/imports/cwe.py` & `opencve-1.4.1/opencve/commands/imports/cwe.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/commands/init.py` & `opencve-1.4.1/opencve/commands/init.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/commands/utils.py` & `opencve-1.4.1/opencve/commands/utils.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/configuration.py` & `opencve-1.4.1/opencve/configuration.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/constants.py` & `opencve-1.4.1/opencve/constants.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/context.py` & `opencve-1.4.1/opencve/context.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/controllers/alerts.py` & `opencve-1.4.1/opencve/controllers/alerts.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/controllers/base.py` & `opencve-1.4.1/opencve/controllers/base.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/controllers/cves.py` & `opencve-1.4.1/opencve/controllers/cves.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/controllers/cwes.py` & `opencve-1.4.1/opencve/controllers/cwes.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/controllers/home.py` & `opencve-1.4.1/opencve/controllers/home.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/controllers/main.py` & `opencve-1.4.1/opencve/controllers/main.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/controllers/products.py` & `opencve-1.4.1/opencve/controllers/products.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/controllers/reports.py` & `opencve-1.4.1/opencve/controllers/reports.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/controllers/subscriptions.py` & `opencve-1.4.1/opencve/controllers/subscriptions.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/controllers/vendors.py` & `opencve-1.4.1/opencve/controllers/vendors.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/default.cfg` & `opencve-1.4.1/opencve/default.cfg`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/extensions.py` & `opencve-1.4.1/opencve/extensions.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/forms.py` & `opencve-1.4.1/opencve/forms.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/migrations/alembic.ini` & `opencve-1.4.1/opencve/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/migrations/env.py` & `opencve-1.4.1/opencve/migrations/env.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/migrations/versions/1c7aecfc5f6e_add_indexes_cascade_deletions_reports.py` & `opencve-1.4.1/opencve/migrations/versions/1c7aecfc5f6e_add_indexes_cascade_deletions_reports.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/migrations/versions/2132d05ea0e2_add_first_time_value_in_event_types_enum.py` & `opencve-1.4.1/opencve/migrations/versions/2132d05ea0e2_add_first_time_value_in_event_types_enum.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/migrations/versions/33cd640e1112_add_indexes_on_cves_summary_and_cve_cve_.py` & `opencve-1.4.1/opencve/migrations/versions/33cd640e1112_add_indexes_on_cves_summary_and_cve_cve_.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/migrations/versions/3f755e0484e0_add_settings_columns_in_users_table.py` & `opencve-1.4.1/opencve/migrations/versions/3f755e0484e0_add_settings_columns_in_users_table.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/migrations/versions/4195eeb432e9_add_tags_tables.py` & `opencve-1.4.1/opencve/migrations/versions/4195eeb432e9_add_tags_tables.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/migrations/versions/41ad8e9163d4_make_cwe_cwe_id_field_not_nullable.py` & `opencve-1.4.1/opencve/migrations/versions/41ad8e9163d4_make_cwe_cwe_id_field_not_nullable.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/migrations/versions/8bdc527d8d49_initial_migration.py` & `opencve-1.4.1/opencve/migrations/versions/8bdc527d8d49_initial_migration.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/migrations/versions/f81abceece3d_synchronize_null_cvss_for_existing_cves.py` & `opencve-1.4.1/opencve/migrations/versions/f81abceece3d_synchronize_null_cvss_for_existing_cves.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/models/__init__.py` & `opencve-1.4.1/opencve/models/__init__.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/models/alerts.py` & `opencve-1.4.1/opencve/models/alerts.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/models/changes.py` & `opencve-1.4.1/opencve/models/changes.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/models/cve.py` & `opencve-1.4.1/opencve/models/cve.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/models/events.py` & `opencve-1.4.1/opencve/models/events.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/models/products.py` & `opencve-1.4.1/opencve/models/products.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/models/reports.py` & `opencve-1.4.1/opencve/models/reports.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/models/tags.py` & `opencve-1.4.1/opencve/models/tags.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/models/users.py` & `opencve-1.4.1/opencve/models/users.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/models/vendors.py` & `opencve-1.4.1/opencve/models/vendors.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/settings.py` & `opencve-1.4.1/opencve/settings.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/css/AdminLTE.min.css` & `opencve-1.4.1/opencve/static/css/AdminLTE.min.css`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/css/bootstrap.min.css` & `opencve-1.4.1/opencve/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/css/custom.css` & `opencve-1.4.1/opencve/static/css/custom.css`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/css/font-awesome.min.css` & `opencve-1.4.1/opencve/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/css/select2.min.css` & `opencve-1.4.1/opencve/static/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/css/skin-blue.min.css` & `opencve-1.4.1/opencve/static/css/skin-blue.min.css`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/css/spectrum.min.css` & `opencve-1.4.1/opencve/static/css/spectrum.min.css`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/fonts/FontAwesome.otf` & `opencve-1.4.1/opencve/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/fonts/fontawesome-webfont.eot` & `opencve-1.4.1/opencve/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/fonts/fontawesome-webfont.svg` & `opencve-1.4.1/opencve/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/fonts/fontawesome-webfont.ttf` & `opencve-1.4.1/opencve/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/fonts/fontawesome-webfont.woff` & `opencve-1.4.1/opencve/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/fonts/fontawesome-webfont.woff2` & `opencve-1.4.1/opencve/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/fonts/glyphicons-halflings-regular.eot` & `opencve-1.4.1/opencve/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/fonts/glyphicons-halflings-regular.svg` & `opencve-1.4.1/opencve/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/fonts/glyphicons-halflings-regular.ttf` & `opencve-1.4.1/opencve/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/fonts/glyphicons-halflings-regular.woff` & `opencve-1.4.1/opencve/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/fonts/glyphicons-halflings-regular.woff2` & `opencve-1.4.1/opencve/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/img/deep-green.jpg` & `opencve-1.4.1/opencve/static/img/deep-green.jpg`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/img/favicon.ico` & `opencve-1.4.1/opencve/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/img/logo_full_48.png` & `opencve-1.4.1/opencve/static/img/logo_full_48.png`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/img/logo_white.png` & `opencve-1.4.1/opencve/static/img/logo_white.png`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/img/mail_icon.png` & `opencve-1.4.1/opencve/static/img/mail_icon.png`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/js/adminlte.min.js` & `opencve-1.4.1/opencve/static/js/adminlte.min.js`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/js/bootstrap.min.js` & `opencve-1.4.1/opencve/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/js/chart.min.js` & `opencve-1.4.1/opencve/static/js/chart.min.js`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/js/custom.js` & `opencve-1.4.1/opencve/static/js/custom.js`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/js/jquery.min.js` & `opencve-1.4.1/opencve/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/js/jquery.rainbowJSON.js` & `opencve-1.4.1/opencve/static/js/jquery.rainbowJSON.js`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/js/select2.full.min.js` & `opencve-1.4.1/opencve/static/js/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/static/js/spectrum.min.js` & `opencve-1.4.1/opencve/static/js/spectrum.min.js`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/tasks/__init__.py` & `opencve-1.4.1/opencve/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/tasks/alerts.py` & `opencve-1.4.1/opencve/tasks/alerts.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/tasks/events.py` & `opencve-1.4.1/opencve/tasks/events.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/tasks/reports.py` & `opencve-1.4.1/opencve/tasks/reports.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/_includes/cvss2.html` & `opencve-1.4.1/opencve/templates/_includes/cvss2.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/_includes/cvss3.html` & `opencve-1.4.1/opencve/templates/_includes/cvss3.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/_macros.html` & `opencve-1.4.1/opencve/templates/_macros.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/_welcome/base_welcome.html` & `opencve-1.4.1/opencve/templates/_welcome/base_welcome.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/_welcome/index.html` & `opencve-1.4.1/opencve/templates/_welcome/index.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/admin/index.html` & `opencve-1.4.1/opencve/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/admin/task.html` & `opencve-1.4.1/opencve/templates/admin/task.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/admin/tasks.html` & `opencve-1.4.1/opencve/templates/admin/tasks.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/base.html` & `opencve-1.4.1/opencve/templates/base.html`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         {% if request.endpoint not in ['main.notifications', 'main.tags', 'main.edit_tag', 'main.settings'] %}
         {% include 'flash_messages.html' %}
         {% endif %}
         {% block content %}{% endblock %}
     </div>
 
     <footer class="main-footer">
-        <strong>Copyright &copy; 2021 OpenCVE.</strong>
+        <strong>Copyright &copy; 2023 OpenCVE.</strong>
     </footer>
 
 </div>
 
 <script src="{{ url_for('static', filename='js/jquery.min.js') }}" type="text/javascript"></script>
 <script src="{{ url_for('static', filename='js/bootstrap.min.js') }}" type="text/javascript"></script>
 <script src="{{ url_for('static', filename='js/adminlte.min.js') }}" type="text/javascript"></script>
```

#### html2text {}

```diff
@@ -37,9 +37,9 @@
   Vendors_&_Products_(CPE)
 % if is_active( "main.cwes") %}class="active"{% endif %}>
   Categories_(CWE)
 
 {% if request.endpoint not in ['main.notifications', 'main.tags',
 'main.edit_tag', 'main.settings'] %} {% include 'flash_messages.html' %} {%
 endif %} {% block content %}{% endblock %}
- Copyright © 2021 OpenCVE.
+ Copyright © 2023 OpenCVE.
  {% if config.INCLUDE_ANALYTICS %} {% include 'analytics.html' %} {% endif %}
```

### Comparing `opencve-1.4.0/opencve/templates/base_blank.html` & `opencve-1.4.1/opencve/templates/base_blank.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/change.html` & `opencve-1.4.1/opencve/templates/change.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/cve.html` & `opencve-1.4.1/opencve/templates/cve.html`

 * *Files 1% similar despite different names*

```diff
@@ -216,20 +216,24 @@
                 <div class="box-header">
                     <div class="box-title">Information</div>
                 </div>
                 <div class="box-body">
                     <p><strong>Published :</strong> {{ cve.created_at.strftime('%Y-%m-%d %H:%M') }}</p>
                     <p><strong>Updated :</strong> {{ cve.updated_at.strftime('%Y-%m-%d %H:%M') }}</p>
                     <hr/>
+                    
                     <p><strong><i class="fa fa-external-link"></i> NVD link :</strong> <a
                             href="https://nvd.nist.gov/vuln/detail/{{ cve.cve_id }}" target="_blank">{{
                         cve.cve_id }}</a></p>
                     <p><strong><i class="fa fa-external-link"></i> Mitre link :</strong> <a
                             href="https://cve.mitre.org/cgi-bin/cvename.cgi?name={{ cve.cve_id }}" target="_blank">{{
                         cve.cve_id }}</a></p>
+                        <p><strong><i class="fa fa-external-link"></i> CVE.ORG link :</strong> <a
+                            href="https://www.cve.org/CVERecord?id={{ cve.cve_id }}" target="_blank">{{
+                            cve.cve_id }}</a></p>
                     <hr/>
                     <p><strong><i class="fa fa-code"></i> JSON object :</strong> <a class="pointer" data-toggle="modal"
                                                                                     data-target="#modal-default">View</a>
                     </p>
                 </div>
             </div>
 
@@ -322,8 +326,8 @@
             </div>
         </form>
       </div>
     </div>
 </div>
 
 
-{% endblock %}
+{% endblock %}
```

#### html2text {}

```diff
@@ -64,14 +64,16 @@
 Published : {{ cve.created_at.strftime('%Y-%m-%d %H:%M') }}
 Updated : {{ cve.updated_at.strftime('%Y-%m-%d %H:%M') }}
 ===============================================================================
  NVD link :
  {{_cve.cve_idÂ }}
  Mitre link :
  {{_cve.cve_idÂ }}
+ CVE.ORG link :
+ {{_cve.cve_idÂ }}
 ===============================================================================
  JSON object :
  View
 Products Affected
 {% if vendors %}
 {% for vendor, products in vendors.items() %}
 {{ vendor }}
```

### Comparing `opencve-1.4.0/opencve/templates/cves.html` & `opencve-1.4.1/opencve/templates/cves.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/cwes.html` & `opencve-1.4.1/opencve/templates/cwes.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/emails/report_message.html` & `opencve-1.4.1/opencve/templates/emails/report_message.html`

 * *Files 1% similar despite different names*

```diff
@@ -422,16 +422,16 @@
                                                                        border="0">
                                                                     <tbody>
                                                                     <tr>
                                                                         <td valign="top" class="textContent">
                                                                             <div style="text-align:center;font-family:Helvetica,Arial,sans-serif;font-size:15px;margin-bottom:0;margin-top:3px;color:#5F5F5F;line-height:135%;">
                                                                                 <a style="color:#ffffff;"
                                                                                    target="_blank"
-                                                                                   href="https://twitter.com/opencve">Follow
-                                                                                    OpenCVE on Twitter</a></div>
+                                                                                   href="https://github.com/opencve/opencve">Follow
+                                                                                    OpenCVE on Github</a></div>
                                                                         </td>
                                                                     </tr>
                                                                     </tbody>
                                                                 </table>
                                                                 <!-- // CONTENT TABLE -->
 
                                                             </td>
@@ -480,15 +480,15 @@
                                                 <td align="center" valign="top" width="600"
                                                     class="flexibleContainerCell">
                                                     <table border="0" cellpadding="20" cellspacing="0" width="100%">
                                                         <tr>
                                                             <td valign="top" bgcolor="#E1E1E1">
 
                                                                 <div style="font-family:Helvetica,Arial,sans-serif;font-size:13px;color:#828282;text-align:center;line-height:120%">
-                                                                    <div>Copyright &#169; 2021 <a
+                                                                    <div>Copyright &#169; 2023 <a
                                                                             href="https://opencve.io" target="_blank"
                                                                             style="text-decoration:none;color:#828282"><span
                                                                             style="color:#828282">OpenCVE.io</span></a>.
                                                                         All&nbsp;rights&nbsp;reserved.
                                                                     </div>
                                                                     <div>If you do not want to receive emails, you can
                                                                         unsubscribe <a
```

#### html2text {}

```diff
@@ -16,11 +16,11 @@
  {{ alert.cve.summary|truncate(230) }}
  {% if alert.events|length > 0 %}
  Change{% if alert.events|length > 1 %}s{% endif %} : {% for event in
  alert.events %}{{ event.type.value }}{% if not loop.last %}, {% endif %}{%
  endfor %}
  {% endif %}
                                          ►_View_the_full_report
-                                        Follow_OpenCVE_on_Twitter
+                                        Follow_OpenCVE_on_Github
 
-        Copyright © 2021 OpenCVE.io. All rights reserved.
+        Copyright © 2023 OpenCVE.io. All rights reserved.
         If you do not want to receive emails, you can unsubscribe here.
```

### Comparing `opencve-1.4.0/opencve/templates/emails/report_message.txt` & `opencve-1.4.1/opencve/templates/emails/report_message.txt`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/flask_user/change_password.html` & `opencve-1.4.1/opencve/templates/flask_user/change_password.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/flask_user/edit_user_profile.html` & `opencve-1.4.1/opencve/templates/flask_user/edit_user_profile.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/flask_user/forgot_password.html` & `opencve-1.4.1/opencve/templates/flask_user/forgot_password.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/flask_user/login.html` & `opencve-1.4.1/opencve/templates/flask_user/login.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/flask_user/register.html` & `opencve-1.4.1/opencve/templates/flask_user/register.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/flask_user/resend_confirm_email.html` & `opencve-1.4.1/opencve/templates/flask_user/resend_confirm_email.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/home.html` & `opencve-1.4.1/opencve/templates/home.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/messages.html` & `opencve-1.4.1/opencve/templates/messages.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/profiles/base_profile.html` & `opencve-1.4.1/opencve/templates/profiles/base_profile.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/profiles/delete_tag.html` & `opencve-1.4.1/opencve/templates/profiles/delete_tag.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/profiles/notifications.html` & `opencve-1.4.1/opencve/templates/profiles/notifications.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/profiles/settings.html` & `opencve-1.4.1/opencve/templates/profiles/settings.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/profiles/subscriptions.html` & `opencve-1.4.1/opencve/templates/profiles/subscriptions.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/profiles/tags.html` & `opencve-1.4.1/opencve/templates/profiles/tags.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/report/references_details.html` & `opencve-1.4.1/opencve/templates/report/references_details.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/report.html` & `opencve-1.4.1/opencve/templates/report.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/reports.html` & `opencve-1.4.1/opencve/templates/reports.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/templates/vendors.html` & `opencve-1.4.1/opencve/templates/vendors.html`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/utils.py` & `opencve-1.4.1/opencve/utils.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/views/cves.py` & `opencve-1.4.1/opencve/views/cves.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/views/profile.py` & `opencve-1.4.1/opencve/views/profile.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/views/reports.py` & `opencve-1.4.1/opencve/views/reports.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve/views/vendors.py` & `opencve-1.4.1/opencve/views/vendors.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve.egg-info/PKG-INFO` & `opencve-1.4.1/opencve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencve
-Version: 1.4.0
+Version: 1.4.1
 Summary: CVE Alerting Platform
 Home-page: https://github.com/opencve/opencve
 Author: Nicolas Crocfer
 Author-email: ncrocfer@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opencve Version: 1.4.0 Summary: CVE Alerting
+Metadata-Version: 2.1 Name: opencve Version: 1.4.1 Summary: CVE Alerting
 Platform Home-page: https://github.com/opencve/opencve Author: Nicolas Crocfer
 Author-email: ncrocfer@gmail.com Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Requires-Python: >=3.7
 Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
```

### Comparing `opencve-1.4.0/opencve.egg-info/SOURCES.txt` & `opencve-1.4.1/opencve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/opencve.egg-info/requires.txt` & `opencve-1.4.1/opencve.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 psycopg2-binary==2.8.4
 Redis==3.3.11
 arrow==0.13.1
 celery==4.3.0
 cpe==1.2.1
 untangle==1.1.1
 cssmin==0.2.0
-jsmin==2.2.2
+jsmin==3.0.1
 requests==2.23.0
 nested-lookup==0.2.18
 deepdiff==4.0.7
 gunicorn==20.0.4
 vine==1.3.0
 click==7.1.2
 werkzeug==1.0.1
```

### Comparing `opencve-1.4.0/requirements.txt` & `opencve-1.4.1/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # Misc
 arrow==0.13.1
 celery==4.3.0
 cpe==1.2.1
 untangle==1.1.1
 cssmin==0.2.0
-jsmin==2.2.2
+jsmin==3.0.1
 requests==2.23.0
 nested-lookup==0.2.18
 deepdiff==4.0.7
 gunicorn==20.0.4
 vine==1.3.0
 click==7.1.2
 werkzeug==1.0.1
```

### Comparing `opencve-1.4.0/setup.py` & `opencve-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/api/test_alerts.py` & `opencve-1.4.1/tests/api/test_alerts.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/api/test_cves.py` & `opencve-1.4.1/tests/api/test_cves.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/api/test_cwes.py` & `opencve-1.4.1/tests/api/test_cwes.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/api/test_products.py` & `opencve-1.4.1/tests/api/test_products.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/api/test_ratelimit.py` & `opencve-1.4.1/tests/api/test_ratelimit.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/api/test_reports.py` & `opencve-1.4.1/tests/api/test_reports.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/api/test_subscriptions.py` & `opencve-1.4.1/tests/api/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/api/test_vendors.py` & `opencve-1.4.1/tests/api/test_vendors.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/commands/test_celery.py` & `opencve-1.4.1/tests/commands/test_celery.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/commands/test_create_user.py` & `opencve-1.4.1/tests/commands/test_create_user.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/commands/test_upgrade_db.py` & `opencve-1.4.1/tests/commands/test_upgrade_db.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/commands/test_utils.py` & `opencve-1.4.1/tests/commands/test_utils.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/commands/test_webserver.py` & `opencve-1.4.1/tests/commands/test_webserver.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/conftest.py` & `opencve-1.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/controllers/test_base.py` & `opencve-1.4.1/tests/controllers/test_base.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/controllers/test_cves.py` & `opencve-1.4.1/tests/controllers/test_cves.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/controllers/test_cwes.py` & `opencve-1.4.1/tests/controllers/test_cwes.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/controllers/test_products.py` & `opencve-1.4.1/tests/controllers/test_products.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/controllers/test_reports.py` & `opencve-1.4.1/tests/controllers/test_reports.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/controllers/test_subscriptions.py` & `opencve-1.4.1/tests/controllers/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/controllers/test_tags.py` & `opencve-1.4.1/tests/controllers/test_tags.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/controllers/test_vendors.py` & `opencve-1.4.1/tests/controllers/test_vendors.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/tasks/test_alerts.py` & `opencve-1.4.1/tests/tasks/test_alerts.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/tasks/test_events.py` & `opencve-1.4.1/tests/tasks/test_events.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/tasks/test_reports.py` & `opencve-1.4.1/tests/tasks/test_reports.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/test_admin.py` & `opencve-1.4.1/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/test_context.py` & `opencve-1.4.1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/test_models.py` & `opencve-1.4.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/test_users.py` & `opencve-1.4.1/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/test_utils.py` & `opencve-1.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/views/test_cves.py` & `opencve-1.4.1/tests/views/test_cves.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/views/test_cwes.py` & `opencve-1.4.1/tests/views/test_cwes.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/views/test_home.py` & `opencve-1.4.1/tests/views/test_home.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/views/test_profile.py` & `opencve-1.4.1/tests/views/test_profile.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/views/test_reports.py` & `opencve-1.4.1/tests/views/test_reports.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/views/test_tags.py` & `opencve-1.4.1/tests/views/test_tags.py`

 * *Files identical despite different names*

### Comparing `opencve-1.4.0/tests/views/test_vendors.py` & `opencve-1.4.1/tests/views/test_vendors.py`

 * *Files identical despite different names*

