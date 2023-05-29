# Comparing `tmp/gwcelery-2.1.0.tar.gz` & `tmp/gwcelery-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwcelery-2.1.0.tar", max compression
+gzip compressed data, was "gwcelery-2.1.1.tar", max compression
```

## Comparing `gwcelery-2.1.0.tar` & `gwcelery-2.1.1.tar`

### file list

```diff
@@ -1,232 +1,232 @@
--rw-r--r--   0        0        0    94846 2023-05-20 06:06:22.743731 gwcelery-2.1.0/CHANGES.rst
--rw-r--r--   0        0        0       64 2023-05-18 19:27:39.643149 gwcelery-2.1.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0    19716 2023-05-18 19:27:39.643149 gwcelery-2.1.0/LICENSE.rst
--rw-r--r--   0        0        0     1351 2023-05-18 19:27:39.643149 gwcelery-2.1.0/README.rst
--rw-r--r--   0        0        0      634 2023-05-18 19:27:39.644149 gwcelery-2.1.0/doc/Makefile
--rw-r--r--   0        0        0   191486 2023-05-18 19:27:39.645149 gwcelery-2.1.0/doc/_static/acceptance-tests-checklist.png
--rw-r--r--   0        0        0   241593 2023-05-18 19:27:39.647149 gwcelery-2.1.0/doc/_static/celeryevent-screenshot.png
--rw-r--r--   0        0        0   206465 2023-05-18 19:27:39.649149 gwcelery-2.1.0/doc/_static/deployment-screenshot.png
--rw-r--r--   0        0        0   161306 2023-05-18 19:27:39.650149 gwcelery-2.1.0/doc/_static/flask-screenshot.png
--rw-r--r--   0        0        0   328056 2023-05-18 19:27:39.653149 gwcelery-2.1.0/doc/_static/flower-screenshot.png
--rw-r--r--   0        0        0   114719 2023-05-18 19:27:39.654149 gwcelery-2.1.0/doc/_static/logo-0.5x.png
--rw-r--r--   0        0        0   351955 2023-05-18 19:27:39.657150 gwcelery-2.1.0/doc/_static/logo.png
--rw-r--r--   0        0        0   230777 2023-05-18 19:27:39.659150 gwcelery-2.1.0/doc/_static/sentry-screenshot.png
--rwxr-xr-x   0        0        0     7356 2023-05-18 19:27:39.659150 gwcelery-2.1.0/doc/conf.py
--rw-r--r--   0        0        0     4346 2023-05-18 19:27:39.659150 gwcelery-2.1.0/doc/configuration.rst
--rw-r--r--   0        0        0     5698 2023-05-18 19:27:39.659150 gwcelery-2.1.0/doc/contributing.rst
--rw-r--r--   0        0        0     7202 2023-05-18 19:27:39.659150 gwcelery-2.1.0/doc/deployment.rst
--rw-r--r--   0        0        0    10176 2023-05-18 19:27:39.660150 gwcelery-2.1.0/doc/design.rst
--rw-r--r--   0        0        0      486 2023-05-18 19:27:39.660150 gwcelery-2.1.0/doc/gwcelery.conf.rst
--rw-r--r--   0        0        0      284 2023-05-18 19:27:39.660150 gwcelery-2.1.0/doc/gwcelery.email.rst
--rw-r--r--   0        0        0      329 2023-05-18 19:27:39.660150 gwcelery-2.1.0/doc/gwcelery.igwn_alert.rst
--rw-r--r--   0        0        0      227 2023-05-18 19:27:39.660150 gwcelery-2.1.0/doc/gwcelery.rst
--rw-r--r--   0        0        0       79 2023-05-18 19:27:39.660150 gwcelery-2.1.0/doc/gwcelery.sentry.rst
--rw-r--r--   0        0        0       97 2023-05-18 19:27:39.660150 gwcelery-2.1.0/doc/gwcelery.tasks.alerts.rst
--rw-r--r--   0        0        0      103 2023-05-18 19:27:39.660150 gwcelery-2.1.0/doc/gwcelery.tasks.bayestar.rst
--rw-r--r--   0        0        0      107 2023-05-18 19:27:39.660150 gwcelery-2.1.0/doc/gwcelery.tasks.circulars.rst
--rw-r--r--   0        0        0       98 2023-05-18 19:27:39.660150 gwcelery-2.1.0/doc/gwcelery.tasks.condor.rst
--rw-r--r--   0        0        0     2404 2023-05-18 19:27:39.660150 gwcelery-2.1.0/doc/gwcelery.tasks.detchar.rst
--rw-r--r--   0        0        0     1110 2023-05-18 19:27:39.661150 gwcelery-2.1.0/doc/gwcelery.tasks.em_bright.rst
--rw-r--r--   0        0        0      129 2023-05-18 19:27:39.661150 gwcelery-2.1.0/doc/gwcelery.tasks.external_skymaps.rst
--rw-r--r--   0        0        0     6738 2023-05-18 19:27:39.661150 gwcelery-2.1.0/doc/gwcelery.tasks.external_triggers.rst
--rw-r--r--   0        0        0      112 2023-05-18 19:27:39.661150 gwcelery-2.1.0/doc/gwcelery.tasks.first2years.rst
--rw-r--r--   0        0        0       88 2023-05-18 19:27:39.661150 gwcelery-2.1.0/doc/gwcelery.tasks.gcn.rst
--rw-r--r--   0        0        0      100 2023-05-18 19:27:39.661150 gwcelery-2.1.0/doc/gwcelery.tasks.gracedb.rst
--rw-r--r--   0        0        0      109 2023-05-18 19:27:39.661150 gwcelery-2.1.0/doc/gwcelery.tasks.igwn_alert.rst
--rw-r--r--   0        0        0      109 2023-05-18 19:27:39.661150 gwcelery-2.1.0/doc/gwcelery.tasks.inference.rst
--rw-r--r--   0        0        0     8111 2023-05-18 19:27:39.661150 gwcelery-2.1.0/doc/gwcelery.tasks.orchestrator.rst
--rw-r--r--   0        0        0      100 2023-05-18 19:27:39.661150 gwcelery-2.1.0/doc/gwcelery.tasks.p_astro.rst
--rw-r--r--   0        0        0       94 2023-05-18 19:27:39.661150 gwcelery-2.1.0/doc/gwcelery.tasks.raven.rst
--rw-r--r--   0        0        0      628 2023-05-18 19:27:39.662150 gwcelery-2.1.0/doc/gwcelery.tasks.rst
--rw-r--r--   0        0        0      100 2023-05-18 19:27:39.662150 gwcelery-2.1.0/doc/gwcelery.tasks.skymaps.rst
--rw-r--r--   0        0        0     7161 2023-05-18 19:27:39.662150 gwcelery-2.1.0/doc/gwcelery.tasks.superevents.rst
--rw-r--r--   0        0        0       97 2023-05-18 19:27:39.662150 gwcelery-2.1.0/doc/gwcelery.tools.condor.rst
--rw-r--r--   0        0        0       94 2023-05-18 19:27:39.662150 gwcelery-2.1.0/doc/gwcelery.tools.flask.rst
--rw-r--r--   0        0        0       97 2023-05-18 19:27:39.662150 gwcelery-2.1.0/doc/gwcelery.tools.nagios.rst
--rw-r--r--   0        0        0      185 2023-05-18 19:27:39.662150 gwcelery-2.1.0/doc/gwcelery.tools.rst
--rw-r--r--   0        0        0       73 2023-05-18 19:27:39.662150 gwcelery-2.1.0/doc/gwcelery.util.rst
--rw-r--r--   0        0        0      507 2023-05-18 19:27:39.662150 gwcelery-2.1.0/doc/gwcelery.voevent.rst
--rw-r--r--   0        0        0     3564 2023-05-18 19:27:39.662150 gwcelery-2.1.0/doc/htcondor.rst
--rw-r--r--   0        0        0     1576 2023-05-18 19:27:39.662150 gwcelery-2.1.0/doc/index.rst
--rw-r--r--   0        0        0      800 2023-05-18 19:27:39.663150 gwcelery-2.1.0/doc/make.bat
--rw-r--r--   0        0        0     4416 2023-05-18 19:27:39.663150 gwcelery-2.1.0/doc/monitoring.rst
--rw-r--r--   0        0        0     5312 2023-05-18 19:27:39.663150 gwcelery-2.1.0/doc/quickstart.rst
--rw-r--r--   0        0        0     1149 2023-05-18 19:27:39.663150 gwcelery-2.1.0/gwcelery/__init__.py
--rw-r--r--   0        0        0    18447 2023-05-18 19:27:39.663150 gwcelery-2.1.0/gwcelery/_version.py
--rw-r--r--   0        0        0    15596 2023-05-19 03:09:23.772937 gwcelery-2.1.0/gwcelery/conf/__init__.py
--rw-r--r--   0        0        0     1014 2023-05-18 19:27:39.664150 gwcelery-2.1.0/gwcelery/conf/dev.py
--rw-r--r--   0        0        0      403 2023-05-18 19:27:39.664150 gwcelery-2.1.0/gwcelery/conf/development.py
--rw-r--r--   0        0        0     1026 2023-05-18 19:27:39.664150 gwcelery-2.1.0/gwcelery/conf/minikube.py
--rw-r--r--   0        0        0     1722 2023-05-18 19:27:39.664150 gwcelery-2.1.0/gwcelery/conf/playground.py
--rw-r--r--   0        0        0     3541 2023-05-18 19:27:39.664150 gwcelery-2.1.0/gwcelery/conf/production.py
--rw-r--r--   0        0        0     2040 2023-05-18 19:27:39.664150 gwcelery-2.1.0/gwcelery/conf/test.py
--rw-r--r--   0        0        0        0 2023-05-20 06:06:22.811733 gwcelery-2.1.0/gwcelery/data/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 06:06:22.813733 gwcelery-2.1.0/gwcelery/data/first2years/__init__.py
--rw-r--r--   0        0        0   731421 2023-05-18 19:27:39.667150 gwcelery-2.1.0/gwcelery/data/first2years/gstlal.xml.gz
--rwxr-xr-x   0        0        0     2785 2023-05-18 19:27:39.668150 gwcelery-2.1.0/gwcelery/data/gwcelery.sub
--rw-r--r--   0        0        0      505 2023-05-18 19:27:39.668150 gwcelery-2.1.0/gwcelery/email/__init__.py
--rw-r--r--   0        0        0     3317 2023-05-18 19:27:39.668150 gwcelery-2.1.0/gwcelery/email/bootsteps.py
--rw-r--r--   0        0        0      995 2023-05-18 19:27:39.668150 gwcelery-2.1.0/gwcelery/email/signals.py
--rw-r--r--   0        0        0     1457 2023-05-18 19:27:39.668150 gwcelery-2.1.0/gwcelery/flask.py
--rw-r--r--   0        0        0      529 2023-05-18 19:27:39.668150 gwcelery-2.1.0/gwcelery/igwn_alert/__init__.py
--rw-r--r--   0        0        0     4484 2023-05-18 19:27:39.668150 gwcelery-2.1.0/gwcelery/igwn_alert/bootsteps.py
--rw-r--r--   0        0        0      608 2023-05-18 19:27:39.669150 gwcelery-2.1.0/gwcelery/igwn_alert/signals.py
--rw-r--r--   0        0        0      275 2023-05-18 19:27:39.669150 gwcelery-2.1.0/gwcelery/jinja.py
--rw-r--r--   0        0        0      305 2023-05-18 19:27:39.669150 gwcelery-2.1.0/gwcelery/kafka/__init__.py
--rw-r--r--   0        0        0    10431 2023-05-18 19:27:39.669150 gwcelery-2.1.0/gwcelery/kafka/bootsteps.py
--rw-r--r--   0        0        0      522 2023-05-18 19:27:39.669150 gwcelery-2.1.0/gwcelery/kafka/signals.py
--rw-r--r--   0        0        0     2567 2023-05-18 19:27:39.669150 gwcelery-2.1.0/gwcelery/sentry/__init__.py
--rw-r--r--   0        0        0       34 2023-05-18 19:27:39.669150 gwcelery-2.1.0/gwcelery/sentry/integrations/__init__.py
--rw-r--r--   0        0        0      832 2023-05-18 19:27:39.670150 gwcelery-2.1.0/gwcelery/sentry/integrations/condor.py
--rw-r--r--   0        0        0      836 2023-05-18 19:27:39.670150 gwcelery-2.1.0/gwcelery/sentry/integrations/requests.py
--rw-r--r--   0        0        0      939 2023-05-18 19:27:39.670150 gwcelery-2.1.0/gwcelery/sentry/integrations/subprocess.py
--rw-r--r--   0        0        0     1302 2023-05-18 19:27:39.670150 gwcelery-2.1.0/gwcelery/static/typeahead.css
--rw-r--r--   0        0        0     4124 2023-05-18 19:27:39.670150 gwcelery-2.1.0/gwcelery/static/vega/index.html
--rw-r--r--   0        0        0      515 2023-05-18 19:27:39.670150 gwcelery-2.1.0/gwcelery/tasks/__init__.py
--rw-r--r--   0        0        0    13597 2023-05-19 06:44:52.288984 gwcelery-2.1.0/gwcelery/tasks/alerts.py
--rw-r--r--   0        0        0     2672 2023-05-18 19:27:39.671150 gwcelery-2.1.0/gwcelery/tasks/bayestar.py
--rw-r--r--   0        0        0     1535 2023-05-19 06:44:52.288984 gwcelery-2.1.0/gwcelery/tasks/circulars.py
--rw-r--r--   0        0        0     7502 2023-05-18 19:27:39.671150 gwcelery-2.1.0/gwcelery/tasks/condor.py
--rw-r--r--   0        0        0     2692 2023-05-18 19:27:39.671150 gwcelery-2.1.0/gwcelery/tasks/core.py
--rw-r--r--   0        0        0    21515 2023-05-19 21:39:54.349367 gwcelery-2.1.0/gwcelery/tasks/detchar.py
--rw-r--r--   0        0        0     4863 2023-05-18 19:27:39.671150 gwcelery-2.1.0/gwcelery/tasks/em_bright.py
--rw-r--r--   0        0        0    21951 2023-05-18 19:27:39.672150 gwcelery-2.1.0/gwcelery/tasks/external_skymaps.py
--rw-r--r--   0        0        0    23806 2023-05-20 00:18:20.105305 gwcelery-2.1.0/gwcelery/tasks/external_triggers.py
--rw-r--r--   0        0        0     6832 2023-05-18 19:27:39.672150 gwcelery-2.1.0/gwcelery/tasks/first2years.py
--rw-r--r--   0        0        0     6384 2023-05-18 19:27:39.672150 gwcelery-2.1.0/gwcelery/tasks/first2years_external.py
--rw-r--r--   0        0        0     4831 2023-05-18 19:27:39.672150 gwcelery-2.1.0/gwcelery/tasks/gcn.py
--rw-r--r--   0        0        0    11079 2023-05-18 19:27:39.673150 gwcelery-2.1.0/gwcelery/tasks/gracedb.py
--rw-r--r--   0        0        0     6105 2023-05-19 19:57:48.392739 gwcelery-2.1.0/gwcelery/tasks/gwskynet.py
--rw-r--r--   0        0        0     2453 2023-05-18 19:27:39.673150 gwcelery-2.1.0/gwcelery/tasks/igwn_alert.py
--rw-r--r--   0        0        0    41859 2023-05-20 02:48:26.929777 gwcelery-2.1.0/gwcelery/tasks/inference.py
--rw-r--r--   0        0        0     1406 2023-05-18 19:27:39.673150 gwcelery-2.1.0/gwcelery/tasks/legacy_gracedb.py
--rw-r--r--   0        0        0     7772 2023-05-18 19:27:39.674150 gwcelery-2.1.0/gwcelery/tasks/notice_text.py
--rw-r--r--   0        0        0    46819 2023-05-19 16:53:56.117563 gwcelery-2.1.0/gwcelery/tasks/orchestrator.py
--rw-r--r--   0        0        0     5796 2023-05-18 19:27:39.674150 gwcelery-2.1.0/gwcelery/tasks/p_astro.py
--rw-r--r--   0        0        0    20999 2023-05-20 00:18:20.106305 gwcelery-2.1.0/gwcelery/tasks/raven.py
--rw-r--r--   0        0        0     2242 2023-05-18 19:27:39.675150 gwcelery-2.1.0/gwcelery/tasks/rrt_utils.py
--rw-r--r--   0        0        0    12528 2023-05-18 19:27:39.675150 gwcelery-2.1.0/gwcelery/tasks/skymaps.py
--rw-r--r--   0        0        0    23631 2023-05-18 19:27:39.675150 gwcelery-2.1.0/gwcelery/tasks/superevents.py
--rw-r--r--   0        0        0     1084 2023-05-18 19:27:39.676150 gwcelery-2.1.0/gwcelery/templates/fits_header.jinja2
--rw-r--r--   0        0        0    35556 2023-05-19 06:44:52.290984 gwcelery-2.1.0/gwcelery/templates/index.jinja2
--rw-r--r--   0        0        0     8505 2023-05-18 19:27:39.676150 gwcelery-2.1.0/gwcelery/templates/lalinference.jinja2
--rw-r--r--   0        0        0     9496 2023-05-19 03:09:23.773937 gwcelery-2.1.0/gwcelery/templates/rapidpe.jinja2
--rw-r--r--   0        0        0      806 2023-05-18 19:27:39.676150 gwcelery-2.1.0/gwcelery/templates/vector_table.jinja2
--rw-r--r--   0        0        0        0 2023-05-20 06:06:22.815733 gwcelery-2.1.0/gwcelery/tests/__init__.py
--rw-r--r--   0        0        0     4388 2023-05-18 19:27:39.677150 gwcelery-2.1.0/gwcelery/tests/conftest.py
--rw-r--r--   0        0        0      976 2023-05-18 19:27:39.677150 gwcelery-2.1.0/gwcelery/tests/data/G000012_S0040_preferred.json
--rw-r--r--   0        0        0     6258 2023-05-18 19:27:39.677150 gwcelery-2.1.0/gwcelery/tests/data/G298048-1-Initial.xml
--rw-r--r--   0        0        0      599 2023-05-18 19:27:39.677150 gwcelery-2.1.0/gwcelery/tests/data/G298048_log.json
--rw-r--r--   0        0        0      150 2023-05-18 19:27:39.677150 gwcelery-2.1.0/gwcelery/tests/data/H1L1V1-mean_counts-1126051217-61603201.json
--rw-r--r--   0        0        0      974 2023-05-18 19:27:39.677150 gwcelery-2.1.0/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json
--rw-r--r--   0        0        0    17572 2023-05-18 19:27:39.677150 gwcelery-2.1.0/gwcelery/tests/data/MS220722v.xml
--rw-r--r--   0        0        0   777600 2023-05-18 19:27:39.683150 gwcelery-2.1.0/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits
--rw-r--r--   0        0        0     8220 2023-05-18 19:27:39.683150 gwcelery-2.1.0/gwcelery/tests/data/S230413b.json
--rw-r--r--   0        0        0     7255 2023-05-18 19:27:39.683150 gwcelery-2.1.0/gwcelery/tests/data/S230413g.json
--rw-r--r--   0        0        0     7721 2023-05-18 19:27:39.683150 gwcelery-2.1.0/gwcelery/tests/data/S230413h.json
--rw-r--r--   0        0        0     3387 2023-05-18 19:27:39.683150 gwcelery-2.1.0/gwcelery/tests/data/T0212_S0039_preferred.json
--rw-r--r--   0        0        0     3384 2023-05-18 19:27:39.683150 gwcelery-2.1.0/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json
--rw-r--r--   0        0        0     5210 2023-05-18 19:27:39.683150 gwcelery-2.1.0/gwcelery/tests/data/T0219_S0041_nopreferred.json
--rw-r--r--   0        0        0        0 2023-05-20 06:06:22.815733 gwcelery-2.1.0/gwcelery/tests/data/__init__.py
--rw-r--r--   0        0        0     2290 2023-05-18 19:27:39.684150 gwcelery-2.1.0/gwcelery/tests/data/agile_grb_gcn.xml
--rw-r--r--   0        0        0   854036 2023-05-18 19:27:39.689151 gwcelery-2.1.0/gwcelery/tests/data/coinc.xml
--rw-r--r--   0        0        0     6175 2023-05-18 19:27:39.689151 gwcelery-2.1.0/gwcelery/tests/data/externaltrigger_original_data.xml
--rw-r--r--   0        0        0     5482 2023-05-18 19:27:39.689151 gwcelery-2.1.0/gwcelery/tests/data/fermi_grb_gcn.xml
--rw-r--r--   0        0        0     5469 2023-05-18 19:27:39.689151 gwcelery-2.1.0/gwcelery/tests/data/fermi_initial_grb_gcn.xml
--rw-r--r--   0        0        0     5865 2023-05-18 19:27:39.689151 gwcelery-2.1.0/gwcelery/tests/data/fermi_noise_gcn.xml
--rw-r--r--   0        0        0     5864 2023-05-18 19:27:39.689151 gwcelery-2.1.0/gwcelery/tests/data/fermi_noise_gcn_2.xml
--rw-r--r--   0        0        0     4914 2023-05-18 19:27:39.689151 gwcelery-2.1.0/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml
--rw-r--r--   0        0        0     4914 2023-05-18 19:27:39.690151 gwcelery-2.1.0/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml
--rw-r--r--   0        0        0     3407 2023-05-18 19:27:39.690151 gwcelery-2.1.0/gwcelery/tests/data/fits_header_result.html
--rw-r--r--   0        0        0      882 2023-05-18 19:27:39.690151 gwcelery-2.1.0/gwcelery/tests/data/gracedb_externaltrigger_log.json
--rw-r--r--   0        0        0      446 2023-05-18 19:27:39.690151 gwcelery-2.1.0/gwcelery/tests/data/gracedb_setrigger_log.json
--rw-r--r--   0        0        0      870 2023-05-18 19:27:39.690151 gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_detchar.json
--rw-r--r--   0        0        0     2025 2023-05-18 19:27:39.690151 gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_exttrig_creation.json
--rw-r--r--   0        0        0     2007 2023-05-18 19:27:39.690151 gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json
--rw-r--r--   0        0        0      166 2023-05-18 19:27:39.690151 gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_fits.json
--rw-r--r--   0        0        0      101 2023-05-18 19:27:39.690151 gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_label_dqv.json
--rw-r--r--   0        0        0      743 2023-05-18 19:27:39.690151 gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_psd.json
--rw-r--r--   0        0        0     2020 2023-05-18 19:27:39.691151 gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_snews_creation.json
--rw-r--r--   0        0        0     2012 2023-05-18 19:27:39.691151 gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_snews_test_creation.json
--rw-r--r--   0        0        0     2028 2023-05-18 19:27:39.691151 gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_subgrb_creation.json
--rw-r--r--   0        0        0     1235 2023-05-18 19:27:39.691151 gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_superevent_creation.json
--rw-r--r--   0        0        0      107 2023-05-18 19:27:39.691151 gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_superevent_label.json
--rw-r--r--   0        0        0     5021 2023-05-18 19:27:39.691151 gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_voevent.json
--rw-r--r--   0        0        0     4429 2023-05-18 19:27:39.691151 gwcelery-2.1.0/gwcelery/tests/data/integral_grb_gcn.xml
--rw-r--r--   0        0        0     4295 2023-05-18 19:27:39.691151 gwcelery-2.1.0/gwcelery/tests/data/integral_mdc_gcn.xml
--rw-r--r--   0        0        0        0 2023-05-20 06:06:22.817733 gwcelery-2.1.0/gwcelery/tests/data/llhoft/__init__.py
--rw-r--r--   0        0        0    14614 2023-05-18 19:27:39.692151 gwcelery-2.1.0/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf
--rw-r--r--   0        0        0        0 2023-05-20 06:06:22.817733 gwcelery-2.1.0/gwcelery/tests/data/llhoft/fail/L1/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 06:06:22.817733 gwcelery-2.1.0/gwcelery/tests/data/llhoft/fail/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 06:06:22.817733 gwcelery-2.1.0/gwcelery/tests/data/llhoft/omegascan/__init__.py
--rw-r--r--   0        0        0   516419 2023-05-18 19:27:39.693151 gwcelery-2.1.0/gwcelery/tests/data/llhoft/omegascan/scanme.gwf
--rw-r--r--   0        0        0    14630 2023-05-18 19:27:39.694151 gwcelery-2.1.0/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf
--rw-r--r--   0        0        0        0 2023-05-20 06:06:22.818733 gwcelery-2.1.0/gwcelery/tests/data/llhoft/pass/H1/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 06:06:22.818733 gwcelery-2.1.0/gwcelery/tests/data/llhoft/pass/__init__.py
--rw-r--r--   0        0        0    13099 2023-05-18 19:27:39.694151 gwcelery-2.1.0/gwcelery/tests/data/lvalert_event_creation.json
--rw-r--r--   0        0        0     9060 2023-05-18 19:27:39.694151 gwcelery-2.1.0/gwcelery/tests/data/lvalert_xmpp.xml
--rw-r--r--   0        0        0      864 2023-05-18 19:27:39.694151 gwcelery-2.1.0/gwcelery/tests/data/mock_superevent_object.json
--rw-r--r--   0        0        0   445440 2023-05-18 19:27:39.696151 gwcelery-2.1.0/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite
--rw-r--r--   0        0        0   294426 2023-05-18 19:27:39.697151 gwcelery-2.1.0/gwcelery/tests/data/psd.xml.gz
--rw-r--r--   0        0        0    11520 2023-05-18 19:27:39.698151 gwcelery-2.1.0/gwcelery/tests/data/rrt_small_area.fits
--rw-r--r--   0        0        0     2964 2023-05-18 19:27:39.698151 gwcelery-2.1.0/gwcelery/tests/data/sample_events.json
--rw-r--r--   0        0        0     3648 2023-05-18 19:27:39.698151 gwcelery-2.1.0/gwcelery/tests/data/samples.hdf5
--rw-r--r--   0        0        0      616 2023-05-18 19:27:39.698151 gwcelery-2.1.0/gwcelery/tests/data/scaler_set_all.pickle
--rw-r--r--   0        0        0     6169 2023-05-18 19:27:39.698151 gwcelery-2.1.0/gwcelery/tests/data/snews_gcn.xml
--rw-r--r--   0        0        0     6161 2023-05-18 19:27:39.698151 gwcelery-2.1.0/gwcelery/tests/data/snews_gcn_test.xml
--rw-r--r--   0        0        0     9583 2023-05-18 19:27:39.698151 gwcelery-2.1.0/gwcelery/tests/data/superevents.json
--rw-r--r--   0        0        0     7713 2023-05-18 19:27:39.698151 gwcelery-2.1.0/gwcelery/tests/data/swift_grb_gcn.xml
--rw-r--r--   0        0        0   581918 2023-05-18 19:27:39.701151 gwcelery-2.1.0/gwcelery/tests/data/test_classifier.pickle
--rw-r--r--   0        0        0     4042 2023-05-18 19:27:39.701151 gwcelery-2.1.0/gwcelery/tests/process.py
--rw-r--r--   0        0        0     2307 2023-05-18 19:27:39.702151 gwcelery-2.1.0/gwcelery/tests/test_sentry.py
--rw-r--r--   0        0        0     1705 2023-05-18 19:27:39.702151 gwcelery-2.1.0/gwcelery/tests/test_tasks_alerts.py
--rw-r--r--   0        0        0     4916 2023-05-18 19:27:39.702151 gwcelery-2.1.0/gwcelery/tests/test_tasks_alerts_validate.py
--rw-r--r--   0        0        0     1439 2023-05-18 19:27:39.702151 gwcelery-2.1.0/gwcelery/tests/test_tasks_bayestar.py
--rw-r--r--   0        0        0     3007 2023-05-19 06:44:52.291984 gwcelery-2.1.0/gwcelery/tests/test_tasks_circulars.py
--rw-r--r--   0        0        0     4550 2023-05-18 19:27:39.702151 gwcelery-2.1.0/gwcelery/tests/test_tasks_condor.py
--rw-r--r--   0        0        0    15811 2023-05-19 21:39:54.350367 gwcelery-2.1.0/gwcelery/tests/test_tasks_detchar.py
--rw-r--r--   0        0        0     2317 2023-05-18 19:27:39.703151 gwcelery-2.1.0/gwcelery/tests/test_tasks_em_bright.py
--rw-r--r--   0        0        0    12322 2023-05-18 19:27:39.703151 gwcelery-2.1.0/gwcelery/tests/test_tasks_external_skymaps.py
--rw-r--r--   0        0        0    34773 2023-05-20 00:18:20.108305 gwcelery-2.1.0/gwcelery/tests/test_tasks_external_triggers.py
--rw-r--r--   0        0        0     1816 2023-05-18 19:27:39.703151 gwcelery-2.1.0/gwcelery/tests/test_tasks_first2years.py
--rw-r--r--   0        0        0     4555 2023-05-18 19:27:39.703151 gwcelery-2.1.0/gwcelery/tests/test_tasks_first2years_external.py
--rw-r--r--   0        0        0     1826 2023-05-18 19:27:39.703151 gwcelery-2.1.0/gwcelery/tests/test_tasks_gcn.py
--rw-r--r--   0        0        0     1655 2023-05-18 19:27:39.704151 gwcelery-2.1.0/gwcelery/tests/test_tasks_gcn_validate.py
--rw-r--r--   0        0        0     5739 2023-05-18 19:27:39.704151 gwcelery-2.1.0/gwcelery/tests/test_tasks_gracedb.py
--rw-r--r--   0        0        0     9591 2023-05-18 19:27:39.704151 gwcelery-2.1.0/gwcelery/tests/test_tasks_gwskynet.py
--rw-r--r--   0        0        0     3662 2023-05-18 19:27:39.704151 gwcelery-2.1.0/gwcelery/tests/test_tasks_igwn_alert.py
--rw-r--r--   0        0        0    22955 2023-05-20 02:48:26.929777 gwcelery-2.1.0/gwcelery/tests/test_tasks_inference.py
--rw-r--r--   0        0        0    33299 2023-05-18 19:27:39.705151 gwcelery-2.1.0/gwcelery/tests/test_tasks_orchestrator.py
--rw-r--r--   0        0        0     1647 2023-05-18 19:27:39.705151 gwcelery-2.1.0/gwcelery/tests/test_tasks_p_astro.py
--rw-r--r--   0        0        0    25523 2023-05-20 00:18:20.109305 gwcelery-2.1.0/gwcelery/tests/test_tasks_raven.py
--rw-r--r--   0        0        0     4724 2023-05-18 19:27:39.705151 gwcelery-2.1.0/gwcelery/tests/test_tasks_rrt_utils.py
--rw-r--r--   0        0        0     5035 2023-05-18 19:27:39.705151 gwcelery-2.1.0/gwcelery/tests/test_tasks_skymaps.py
--rw-r--r--   0        0        0    40127 2023-05-18 19:27:39.706151 gwcelery-2.1.0/gwcelery/tests/test_tasks_superevents.py
--rw-r--r--   0        0        0      637 2023-05-18 19:27:39.706151 gwcelery-2.1.0/gwcelery/tests/test_tempfile.py
--rw-r--r--   0        0        0     3520 2023-05-18 19:27:39.706151 gwcelery-2.1.0/gwcelery/tests/test_tools_condor.py
--rw-r--r--   0        0        0     1098 2023-05-18 19:27:39.706151 gwcelery-2.1.0/gwcelery/tests/test_tools_condor_submit_helper.py
--rw-r--r--   0        0        0      633 2023-05-18 19:27:39.706151 gwcelery-2.1.0/gwcelery/tests/test_tools_flask.py
--rw-r--r--   0        0        0     9668 2023-05-18 19:27:39.706151 gwcelery-2.1.0/gwcelery/tests/test_tools_nagios.py
--rw-r--r--   0        0        0      269 2023-05-18 19:27:39.706151 gwcelery-2.1.0/gwcelery/tests/test_util.py
--rw-r--r--   0        0        0    22392 2023-05-19 06:44:52.292984 gwcelery-2.1.0/gwcelery/tests/test_views.py
--rw-r--r--   0        0        0      216 2023-05-18 19:27:39.707151 gwcelery-2.1.0/gwcelery/tools/__init__.py
--rw-r--r--   0        0        0     2948 2023-05-18 19:27:39.707151 gwcelery-2.1.0/gwcelery/tools/condor.py
--rw-r--r--   0        0        0     1120 2023-05-18 19:27:39.707151 gwcelery-2.1.0/gwcelery/tools/condor_submit_helper.py
--rw-r--r--   0        0        0     1938 2023-05-18 19:27:39.707151 gwcelery-2.1.0/gwcelery/tools/flask.py
--rw-r--r--   0        0        0     6624 2023-05-18 19:27:39.707151 gwcelery-2.1.0/gwcelery/tools/nagios.py
--rw-r--r--   0        0        0      413 2023-05-18 19:27:39.707151 gwcelery-2.1.0/gwcelery/util/__init__.py
--rw-r--r--   0        0        0     1007 2023-05-18 19:27:39.707151 gwcelery-2.1.0/gwcelery/util/cmdline.py
--rw-r--r--   0        0        0      453 2023-05-18 19:27:39.707151 gwcelery-2.1.0/gwcelery/util/matplotlib.py
--rw-r--r--   0        0        0      390 2023-05-18 19:27:39.708151 gwcelery-2.1.0/gwcelery/util/proxy.py
--rw-r--r--   0        0        0      514 2023-05-18 19:27:39.708151 gwcelery-2.1.0/gwcelery/util/resources.py
--rw-r--r--   0        0        0      253 2023-05-18 19:27:39.708151 gwcelery-2.1.0/gwcelery/util/sphinx.py
--rw-r--r--   0        0        0      941 2023-05-18 19:27:39.708151 gwcelery-2.1.0/gwcelery/util/tempfile.py
--rw-r--r--   0        0        0    19058 2023-05-19 06:44:52.293984 gwcelery-2.1.0/gwcelery/views.py
--rw-r--r--   0        0        0      365 2023-05-18 19:27:39.708151 gwcelery-2.1.0/gwcelery/voevent/__init__.py
--rw-r--r--   0        0        0     6387 2023-05-18 19:27:39.708151 gwcelery-2.1.0/gwcelery/voevent/bootsteps.py
--rw-r--r--   0        0        0     1063 2023-05-18 19:27:39.709151 gwcelery-2.1.0/gwcelery/voevent/logging.py
--rw-r--r--   0        0        0      779 2023-05-18 19:27:39.709151 gwcelery-2.1.0/gwcelery/voevent/signals.py
--rw-r--r--   0        0        0      852 2023-05-18 19:27:39.709151 gwcelery-2.1.0/gwcelery/voevent/subscriber.py
--rw-r--r--   0        0        0     1454 2023-05-18 19:27:39.709151 gwcelery-2.1.0/gwcelery/voevent/util.py
--rw-r--r--   0        0        0     6035 2023-05-20 06:06:36.345167 gwcelery-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     4519 1970-01-01 00:00:00.000000 gwcelery-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    95189 2023-05-29 15:18:35.905637 gwcelery-2.1.1/CHANGES.rst
+-rw-r--r--   0        0        0       64 2023-05-29 15:18:35.906637 gwcelery-2.1.1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0    19716 2023-05-29 15:18:35.906637 gwcelery-2.1.1/LICENSE.rst
+-rw-r--r--   0        0        0     1351 2023-05-29 15:18:35.906637 gwcelery-2.1.1/README.rst
+-rw-r--r--   0        0        0      634 2023-05-29 15:18:35.906637 gwcelery-2.1.1/doc/Makefile
+-rw-r--r--   0        0        0   191486 2023-05-29 15:18:35.908637 gwcelery-2.1.1/doc/_static/acceptance-tests-checklist.png
+-rw-r--r--   0        0        0   241593 2023-05-29 15:18:35.910637 gwcelery-2.1.1/doc/_static/celeryevent-screenshot.png
+-rw-r--r--   0        0        0   206465 2023-05-29 15:18:35.911637 gwcelery-2.1.1/doc/_static/deployment-screenshot.png
+-rw-r--r--   0        0        0   161306 2023-05-29 15:18:35.912637 gwcelery-2.1.1/doc/_static/flask-screenshot.png
+-rw-r--r--   0        0        0   328056 2023-05-29 15:18:35.913637 gwcelery-2.1.1/doc/_static/flower-screenshot.png
+-rw-r--r--   0        0        0   114719 2023-05-29 15:18:35.914637 gwcelery-2.1.1/doc/_static/logo-0.5x.png
+-rw-r--r--   0        0        0   351955 2023-05-29 15:18:35.917637 gwcelery-2.1.1/doc/_static/logo.png
+-rw-r--r--   0        0        0   230777 2023-05-29 15:18:35.918637 gwcelery-2.1.1/doc/_static/sentry-screenshot.png
+-rwxr-xr-x   0        0        0     7356 2023-05-29 15:18:35.919637 gwcelery-2.1.1/doc/conf.py
+-rw-r--r--   0        0        0     4346 2023-05-29 15:18:35.919637 gwcelery-2.1.1/doc/configuration.rst
+-rw-r--r--   0        0        0     5698 2023-05-29 15:18:35.919637 gwcelery-2.1.1/doc/contributing.rst
+-rw-r--r--   0        0        0     7202 2023-05-29 15:18:35.919637 gwcelery-2.1.1/doc/deployment.rst
+-rw-r--r--   0        0        0    10176 2023-05-29 15:18:35.919637 gwcelery-2.1.1/doc/design.rst
+-rw-r--r--   0        0        0      486 2023-05-29 15:18:35.919637 gwcelery-2.1.1/doc/gwcelery.conf.rst
+-rw-r--r--   0        0        0      284 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.email.rst
+-rw-r--r--   0        0        0      329 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.igwn_alert.rst
+-rw-r--r--   0        0        0      227 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.rst
+-rw-r--r--   0        0        0       79 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.sentry.rst
+-rw-r--r--   0        0        0       97 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.tasks.alerts.rst
+-rw-r--r--   0        0        0      103 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.tasks.bayestar.rst
+-rw-r--r--   0        0        0      107 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.tasks.circulars.rst
+-rw-r--r--   0        0        0       98 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.tasks.condor.rst
+-rw-r--r--   0        0        0     2404 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.tasks.detchar.rst
+-rw-r--r--   0        0        0     1110 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.tasks.em_bright.rst
+-rw-r--r--   0        0        0      129 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.tasks.external_skymaps.rst
+-rw-r--r--   0        0        0     6738 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.tasks.external_triggers.rst
+-rw-r--r--   0        0        0      112 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.tasks.first2years.rst
+-rw-r--r--   0        0        0       88 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tasks.gcn.rst
+-rw-r--r--   0        0        0      100 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tasks.gracedb.rst
+-rw-r--r--   0        0        0      109 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tasks.igwn_alert.rst
+-rw-r--r--   0        0        0      109 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tasks.inference.rst
+-rw-r--r--   0        0        0     8111 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tasks.orchestrator.rst
+-rw-r--r--   0        0        0      100 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tasks.p_astro.rst
+-rw-r--r--   0        0        0       94 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tasks.raven.rst
+-rw-r--r--   0        0        0      628 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tasks.rst
+-rw-r--r--   0        0        0      100 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tasks.skymaps.rst
+-rw-r--r--   0        0        0     7161 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tasks.superevents.rst
+-rw-r--r--   0        0        0       97 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tools.condor.rst
+-rw-r--r--   0        0        0       94 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tools.flask.rst
+-rw-r--r--   0        0        0       97 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tools.nagios.rst
+-rw-r--r--   0        0        0      185 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tools.rst
+-rw-r--r--   0        0        0       73 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.util.rst
+-rw-r--r--   0        0        0      507 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.voevent.rst
+-rw-r--r--   0        0        0     3564 2023-05-29 15:18:35.922637 gwcelery-2.1.1/doc/htcondor.rst
+-rw-r--r--   0        0        0     1576 2023-05-29 15:18:35.922637 gwcelery-2.1.1/doc/index.rst
+-rw-r--r--   0        0        0      800 2023-05-29 15:18:35.922637 gwcelery-2.1.1/doc/make.bat
+-rw-r--r--   0        0        0     4416 2023-05-29 15:18:35.922637 gwcelery-2.1.1/doc/monitoring.rst
+-rw-r--r--   0        0        0     5312 2023-05-29 15:18:35.922637 gwcelery-2.1.1/doc/quickstart.rst
+-rw-r--r--   0        0        0     1149 2023-05-29 15:18:35.922637 gwcelery-2.1.1/gwcelery/__init__.py
+-rw-r--r--   0        0        0    18447 2023-05-29 15:18:35.922637 gwcelery-2.1.1/gwcelery/_version.py
+-rw-r--r--   0        0        0    15596 2023-05-29 15:18:35.922637 gwcelery-2.1.1/gwcelery/conf/__init__.py
+-rw-r--r--   0        0        0     1014 2023-05-29 15:18:35.922637 gwcelery-2.1.1/gwcelery/conf/dev.py
+-rw-r--r--   0        0        0      403 2023-05-29 15:18:35.922637 gwcelery-2.1.1/gwcelery/conf/development.py
+-rw-r--r--   0        0        0     1026 2023-05-29 15:18:35.922637 gwcelery-2.1.1/gwcelery/conf/minikube.py
+-rw-r--r--   0        0        0     1722 2023-05-29 15:18:35.923637 gwcelery-2.1.1/gwcelery/conf/playground.py
+-rw-r--r--   0        0        0     3541 2023-05-29 15:18:35.923637 gwcelery-2.1.1/gwcelery/conf/production.py
+-rw-r--r--   0        0        0     2040 2023-05-29 15:18:35.923637 gwcelery-2.1.1/gwcelery/conf/test.py
+-rw-r--r--   0        0        0        0 2023-05-29 15:18:36.000637 gwcelery-2.1.1/gwcelery/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 15:18:36.001637 gwcelery-2.1.1/gwcelery/data/first2years/__init__.py
+-rw-r--r--   0        0        0   731421 2023-05-29 15:18:35.925637 gwcelery-2.1.1/gwcelery/data/first2years/gstlal.xml.gz
+-rwxr-xr-x   0        0        0     2785 2023-05-29 15:18:35.925637 gwcelery-2.1.1/gwcelery/data/gwcelery.sub
+-rw-r--r--   0        0        0      505 2023-05-29 15:18:35.926637 gwcelery-2.1.1/gwcelery/email/__init__.py
+-rw-r--r--   0        0        0     3317 2023-05-29 15:18:35.926637 gwcelery-2.1.1/gwcelery/email/bootsteps.py
+-rw-r--r--   0        0        0      995 2023-05-29 15:18:35.926637 gwcelery-2.1.1/gwcelery/email/signals.py
+-rw-r--r--   0        0        0     1457 2023-05-29 15:18:35.926637 gwcelery-2.1.1/gwcelery/flask.py
+-rw-r--r--   0        0        0      529 2023-05-29 15:18:35.926637 gwcelery-2.1.1/gwcelery/igwn_alert/__init__.py
+-rw-r--r--   0        0        0     4484 2023-05-29 15:18:35.926637 gwcelery-2.1.1/gwcelery/igwn_alert/bootsteps.py
+-rw-r--r--   0        0        0      608 2023-05-29 15:18:35.926637 gwcelery-2.1.1/gwcelery/igwn_alert/signals.py
+-rw-r--r--   0        0        0      275 2023-05-29 15:18:35.926637 gwcelery-2.1.1/gwcelery/jinja.py
+-rw-r--r--   0        0        0      305 2023-05-29 15:18:35.926637 gwcelery-2.1.1/gwcelery/kafka/__init__.py
+-rw-r--r--   0        0        0    10431 2023-05-29 15:18:35.927637 gwcelery-2.1.1/gwcelery/kafka/bootsteps.py
+-rw-r--r--   0        0        0      522 2023-05-29 15:18:35.927637 gwcelery-2.1.1/gwcelery/kafka/signals.py
+-rw-r--r--   0        0        0     2567 2023-05-29 15:18:35.927637 gwcelery-2.1.1/gwcelery/sentry/__init__.py
+-rw-r--r--   0        0        0       34 2023-05-29 15:18:35.927637 gwcelery-2.1.1/gwcelery/sentry/integrations/__init__.py
+-rw-r--r--   0        0        0      832 2023-05-29 15:18:35.927637 gwcelery-2.1.1/gwcelery/sentry/integrations/condor.py
+-rw-r--r--   0        0        0      836 2023-05-29 15:18:35.927637 gwcelery-2.1.1/gwcelery/sentry/integrations/requests.py
+-rw-r--r--   0        0        0      939 2023-05-29 15:18:35.927637 gwcelery-2.1.1/gwcelery/sentry/integrations/subprocess.py
+-rw-r--r--   0        0        0     1302 2023-05-29 15:18:35.927637 gwcelery-2.1.1/gwcelery/static/typeahead.css
+-rw-r--r--   0        0        0     4124 2023-05-29 15:18:35.927637 gwcelery-2.1.1/gwcelery/static/vega/index.html
+-rw-r--r--   0        0        0      515 2023-05-29 15:18:35.927637 gwcelery-2.1.1/gwcelery/tasks/__init__.py
+-rw-r--r--   0        0        0    13597 2023-05-29 15:18:35.928637 gwcelery-2.1.1/gwcelery/tasks/alerts.py
+-rw-r--r--   0        0        0     2672 2023-05-29 15:18:35.928637 gwcelery-2.1.1/gwcelery/tasks/bayestar.py
+-rw-r--r--   0        0        0     1535 2023-05-29 15:18:35.928637 gwcelery-2.1.1/gwcelery/tasks/circulars.py
+-rw-r--r--   0        0        0     7502 2023-05-29 15:18:35.928637 gwcelery-2.1.1/gwcelery/tasks/condor.py
+-rw-r--r--   0        0        0     2692 2023-05-29 15:18:35.928637 gwcelery-2.1.1/gwcelery/tasks/core.py
+-rw-r--r--   0        0        0    21515 2023-05-29 15:18:35.929637 gwcelery-2.1.1/gwcelery/tasks/detchar.py
+-rw-r--r--   0        0        0     4863 2023-05-29 15:18:35.929637 gwcelery-2.1.1/gwcelery/tasks/em_bright.py
+-rw-r--r--   0        0        0    21951 2023-05-29 15:18:35.929637 gwcelery-2.1.1/gwcelery/tasks/external_skymaps.py
+-rw-r--r--   0        0        0    23806 2023-05-29 15:18:35.929637 gwcelery-2.1.1/gwcelery/tasks/external_triggers.py
+-rw-r--r--   0        0        0     6832 2023-05-29 15:18:35.929637 gwcelery-2.1.1/gwcelery/tasks/first2years.py
+-rw-r--r--   0        0        0     6384 2023-05-29 15:18:35.929637 gwcelery-2.1.1/gwcelery/tasks/first2years_external.py
+-rw-r--r--   0        0        0     4831 2023-05-29 15:18:35.929637 gwcelery-2.1.1/gwcelery/tasks/gcn.py
+-rw-r--r--   0        0        0    11079 2023-05-29 15:18:35.930637 gwcelery-2.1.1/gwcelery/tasks/gracedb.py
+-rw-r--r--   0        0        0     6105 2023-05-29 15:18:35.930637 gwcelery-2.1.1/gwcelery/tasks/gwskynet.py
+-rw-r--r--   0        0        0     2453 2023-05-29 15:18:35.930637 gwcelery-2.1.1/gwcelery/tasks/igwn_alert.py
+-rw-r--r--   0        0        0    41859 2023-05-29 15:18:35.930637 gwcelery-2.1.1/gwcelery/tasks/inference.py
+-rw-r--r--   0        0        0     1406 2023-05-29 15:18:35.930637 gwcelery-2.1.1/gwcelery/tasks/legacy_gracedb.py
+-rw-r--r--   0        0        0     7772 2023-05-29 15:18:35.930637 gwcelery-2.1.1/gwcelery/tasks/notice_text.py
+-rw-r--r--   0        0        0    46819 2023-05-29 15:18:35.931637 gwcelery-2.1.1/gwcelery/tasks/orchestrator.py
+-rw-r--r--   0        0        0     5796 2023-05-29 15:18:35.931637 gwcelery-2.1.1/gwcelery/tasks/p_astro.py
+-rw-r--r--   0        0        0    20999 2023-05-29 15:18:35.931637 gwcelery-2.1.1/gwcelery/tasks/raven.py
+-rw-r--r--   0        0        0     2242 2023-05-29 15:18:35.931637 gwcelery-2.1.1/gwcelery/tasks/rrt_utils.py
+-rw-r--r--   0        0        0    12528 2023-05-29 15:18:35.932637 gwcelery-2.1.1/gwcelery/tasks/skymaps.py
+-rw-r--r--   0        0        0    23631 2023-05-29 15:18:35.932637 gwcelery-2.1.1/gwcelery/tasks/superevents.py
+-rw-r--r--   0        0        0     1084 2023-05-29 15:18:35.932637 gwcelery-2.1.1/gwcelery/templates/fits_header.jinja2
+-rw-r--r--   0        0        0    35556 2023-05-29 15:18:35.932637 gwcelery-2.1.1/gwcelery/templates/index.jinja2
+-rw-r--r--   0        0        0     8505 2023-05-29 15:18:35.932637 gwcelery-2.1.1/gwcelery/templates/lalinference.jinja2
+-rw-r--r--   0        0        0     9496 2023-05-29 15:18:35.933637 gwcelery-2.1.1/gwcelery/templates/rapidpe.jinja2
+-rw-r--r--   0        0        0      806 2023-05-29 15:18:35.933637 gwcelery-2.1.1/gwcelery/templates/vector_table.jinja2
+-rw-r--r--   0        0        0        0 2023-05-29 15:18:36.003637 gwcelery-2.1.1/gwcelery/tests/__init__.py
+-rw-r--r--   0        0        0     4388 2023-05-29 15:18:35.933637 gwcelery-2.1.1/gwcelery/tests/conftest.py
+-rw-r--r--   0        0        0      976 2023-05-29 15:18:35.933637 gwcelery-2.1.1/gwcelery/tests/data/G000012_S0040_preferred.json
+-rw-r--r--   0        0        0     6258 2023-05-29 15:18:35.933637 gwcelery-2.1.1/gwcelery/tests/data/G298048-1-Initial.xml
+-rw-r--r--   0        0        0      599 2023-05-29 15:18:35.933637 gwcelery-2.1.1/gwcelery/tests/data/G298048_log.json
+-rw-r--r--   0        0        0      150 2023-05-29 15:18:35.933637 gwcelery-2.1.1/gwcelery/tests/data/H1L1V1-mean_counts-1126051217-61603201.json
+-rw-r--r--   0        0        0      974 2023-05-29 15:18:35.933637 gwcelery-2.1.1/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json
+-rw-r--r--   0        0        0    17572 2023-05-29 15:18:35.933637 gwcelery-2.1.1/gwcelery/tests/data/MS220722v.xml
+-rw-r--r--   0        0        0   777600 2023-05-29 15:18:35.938637 gwcelery-2.1.1/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits
+-rw-r--r--   0        0        0     8220 2023-05-29 15:18:35.938637 gwcelery-2.1.1/gwcelery/tests/data/S230413b.json
+-rw-r--r--   0        0        0     7255 2023-05-29 15:18:35.938637 gwcelery-2.1.1/gwcelery/tests/data/S230413g.json
+-rw-r--r--   0        0        0     7721 2023-05-29 15:18:35.938637 gwcelery-2.1.1/gwcelery/tests/data/S230413h.json
+-rw-r--r--   0        0        0     3387 2023-05-29 15:18:35.939637 gwcelery-2.1.1/gwcelery/tests/data/T0212_S0039_preferred.json
+-rw-r--r--   0        0        0     3384 2023-05-29 15:18:35.939637 gwcelery-2.1.1/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json
+-rw-r--r--   0        0        0     5210 2023-05-29 15:18:35.939637 gwcelery-2.1.1/gwcelery/tests/data/T0219_S0041_nopreferred.json
+-rw-r--r--   0        0        0        0 2023-05-29 15:18:36.003637 gwcelery-2.1.1/gwcelery/tests/data/__init__.py
+-rw-r--r--   0        0        0     2290 2023-05-29 15:18:35.939637 gwcelery-2.1.1/gwcelery/tests/data/agile_grb_gcn.xml
+-rw-r--r--   0        0        0   854036 2023-05-29 15:18:35.943637 gwcelery-2.1.1/gwcelery/tests/data/coinc.xml
+-rw-r--r--   0        0        0     6175 2023-05-29 15:18:35.943637 gwcelery-2.1.1/gwcelery/tests/data/externaltrigger_original_data.xml
+-rw-r--r--   0        0        0     5482 2023-05-29 15:18:35.943637 gwcelery-2.1.1/gwcelery/tests/data/fermi_grb_gcn.xml
+-rw-r--r--   0        0        0     5469 2023-05-29 15:18:35.944637 gwcelery-2.1.1/gwcelery/tests/data/fermi_initial_grb_gcn.xml
+-rw-r--r--   0        0        0     5865 2023-05-29 15:18:35.944637 gwcelery-2.1.1/gwcelery/tests/data/fermi_noise_gcn.xml
+-rw-r--r--   0        0        0     5864 2023-05-29 15:18:35.944637 gwcelery-2.1.1/gwcelery/tests/data/fermi_noise_gcn_2.xml
+-rw-r--r--   0        0        0     4914 2023-05-29 15:18:35.944637 gwcelery-2.1.1/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml
+-rw-r--r--   0        0        0     4914 2023-05-29 15:18:35.944637 gwcelery-2.1.1/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml
+-rw-r--r--   0        0        0     3407 2023-05-29 15:18:35.944637 gwcelery-2.1.1/gwcelery/tests/data/fits_header_result.html
+-rw-r--r--   0        0        0      882 2023-05-29 15:18:35.944637 gwcelery-2.1.1/gwcelery/tests/data/gracedb_externaltrigger_log.json
+-rw-r--r--   0        0        0      446 2023-05-29 15:18:35.944637 gwcelery-2.1.1/gwcelery/tests/data/gracedb_setrigger_log.json
+-rw-r--r--   0        0        0      870 2023-05-29 15:18:35.944637 gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_detchar.json
+-rw-r--r--   0        0        0     2025 2023-05-29 15:18:35.944637 gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_exttrig_creation.json
+-rw-r--r--   0        0        0     2007 2023-05-29 15:18:35.944637 gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json
+-rw-r--r--   0        0        0      166 2023-05-29 15:18:35.944637 gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_fits.json
+-rw-r--r--   0        0        0      101 2023-05-29 15:18:35.945637 gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_label_dqv.json
+-rw-r--r--   0        0        0      743 2023-05-29 15:18:35.945637 gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_psd.json
+-rw-r--r--   0        0        0     2020 2023-05-29 15:18:35.945637 gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_snews_creation.json
+-rw-r--r--   0        0        0     2012 2023-05-29 15:18:35.945637 gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_snews_test_creation.json
+-rw-r--r--   0        0        0     2028 2023-05-29 15:18:35.945637 gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_subgrb_creation.json
+-rw-r--r--   0        0        0     1235 2023-05-29 15:18:35.945637 gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_superevent_creation.json
+-rw-r--r--   0        0        0      107 2023-05-29 15:18:35.945637 gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_superevent_label.json
+-rw-r--r--   0        0        0     5021 2023-05-29 15:18:35.945637 gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_voevent.json
+-rw-r--r--   0        0        0     4429 2023-05-29 15:18:35.945637 gwcelery-2.1.1/gwcelery/tests/data/integral_grb_gcn.xml
+-rw-r--r--   0        0        0     4295 2023-05-29 15:18:35.946637 gwcelery-2.1.1/gwcelery/tests/data/integral_mdc_gcn.xml
+-rw-r--r--   0        0        0        0 2023-05-29 15:18:36.004637 gwcelery-2.1.1/gwcelery/tests/data/llhoft/__init__.py
+-rw-r--r--   0        0        0    14614 2023-05-29 15:18:35.946637 gwcelery-2.1.1/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf
+-rw-r--r--   0        0        0        0 2023-05-29 15:18:36.004637 gwcelery-2.1.1/gwcelery/tests/data/llhoft/fail/L1/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 15:18:36.004637 gwcelery-2.1.1/gwcelery/tests/data/llhoft/fail/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 15:18:36.004637 gwcelery-2.1.1/gwcelery/tests/data/llhoft/omegascan/__init__.py
+-rw-r--r--   0        0        0   516419 2023-05-29 15:18:35.948637 gwcelery-2.1.1/gwcelery/tests/data/llhoft/omegascan/scanme.gwf
+-rw-r--r--   0        0        0    14630 2023-05-29 15:18:35.949637 gwcelery-2.1.1/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf
+-rw-r--r--   0        0        0        0 2023-05-29 15:18:36.004637 gwcelery-2.1.1/gwcelery/tests/data/llhoft/pass/H1/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 15:18:36.004637 gwcelery-2.1.1/gwcelery/tests/data/llhoft/pass/__init__.py
+-rw-r--r--   0        0        0    13099 2023-05-29 15:18:35.949637 gwcelery-2.1.1/gwcelery/tests/data/lvalert_event_creation.json
+-rw-r--r--   0        0        0     9060 2023-05-29 15:18:35.949637 gwcelery-2.1.1/gwcelery/tests/data/lvalert_xmpp.xml
+-rw-r--r--   0        0        0      864 2023-05-29 15:18:35.949637 gwcelery-2.1.1/gwcelery/tests/data/mock_superevent_object.json
+-rw-r--r--   0        0        0   445440 2023-05-29 15:18:35.951637 gwcelery-2.1.1/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite
+-rw-r--r--   0        0        0   294426 2023-05-29 15:18:35.952637 gwcelery-2.1.1/gwcelery/tests/data/psd.xml.gz
+-rw-r--r--   0        0        0    11520 2023-05-29 15:18:35.952637 gwcelery-2.1.1/gwcelery/tests/data/rrt_small_area.fits
+-rw-r--r--   0        0        0     2964 2023-05-29 15:18:35.952637 gwcelery-2.1.1/gwcelery/tests/data/sample_events.json
+-rw-r--r--   0        0        0     3648 2023-05-29 15:18:35.953637 gwcelery-2.1.1/gwcelery/tests/data/samples.hdf5
+-rw-r--r--   0        0        0      616 2023-05-29 15:18:35.953637 gwcelery-2.1.1/gwcelery/tests/data/scaler_set_all.pickle
+-rw-r--r--   0        0        0     6169 2023-05-29 15:18:35.953637 gwcelery-2.1.1/gwcelery/tests/data/snews_gcn.xml
+-rw-r--r--   0        0        0     6161 2023-05-29 15:18:35.953637 gwcelery-2.1.1/gwcelery/tests/data/snews_gcn_test.xml
+-rw-r--r--   0        0        0     9583 2023-05-29 15:18:35.953637 gwcelery-2.1.1/gwcelery/tests/data/superevents.json
+-rw-r--r--   0        0        0     7713 2023-05-29 15:18:35.953637 gwcelery-2.1.1/gwcelery/tests/data/swift_grb_gcn.xml
+-rw-r--r--   0        0        0   581918 2023-05-29 15:18:35.955637 gwcelery-2.1.1/gwcelery/tests/data/test_classifier.pickle
+-rw-r--r--   0        0        0     4042 2023-05-29 15:18:35.955637 gwcelery-2.1.1/gwcelery/tests/process.py
+-rw-r--r--   0        0        0     2307 2023-05-29 15:18:35.955637 gwcelery-2.1.1/gwcelery/tests/test_sentry.py
+-rw-r--r--   0        0        0     1705 2023-05-29 15:18:35.955637 gwcelery-2.1.1/gwcelery/tests/test_tasks_alerts.py
+-rw-r--r--   0        0        0     4916 2023-05-29 15:18:35.955637 gwcelery-2.1.1/gwcelery/tests/test_tasks_alerts_validate.py
+-rw-r--r--   0        0        0     1439 2023-05-29 15:18:35.955637 gwcelery-2.1.1/gwcelery/tests/test_tasks_bayestar.py
+-rw-r--r--   0        0        0     3007 2023-05-29 15:18:35.956637 gwcelery-2.1.1/gwcelery/tests/test_tasks_circulars.py
+-rw-r--r--   0        0        0     4550 2023-05-29 15:18:35.956637 gwcelery-2.1.1/gwcelery/tests/test_tasks_condor.py
+-rw-r--r--   0        0        0    15811 2023-05-29 15:18:35.956637 gwcelery-2.1.1/gwcelery/tests/test_tasks_detchar.py
+-rw-r--r--   0        0        0     2317 2023-05-29 15:18:35.956637 gwcelery-2.1.1/gwcelery/tests/test_tasks_em_bright.py
+-rw-r--r--   0        0        0    12322 2023-05-29 15:18:35.956637 gwcelery-2.1.1/gwcelery/tests/test_tasks_external_skymaps.py
+-rw-r--r--   0        0        0    34773 2023-05-29 15:18:35.956637 gwcelery-2.1.1/gwcelery/tests/test_tasks_external_triggers.py
+-rw-r--r--   0        0        0     1816 2023-05-29 15:18:35.956637 gwcelery-2.1.1/gwcelery/tests/test_tasks_first2years.py
+-rw-r--r--   0        0        0     4555 2023-05-29 15:18:35.956637 gwcelery-2.1.1/gwcelery/tests/test_tasks_first2years_external.py
+-rw-r--r--   0        0        0     1826 2023-05-29 15:18:35.957637 gwcelery-2.1.1/gwcelery/tests/test_tasks_gcn.py
+-rw-r--r--   0        0        0     1655 2023-05-29 15:18:35.957637 gwcelery-2.1.1/gwcelery/tests/test_tasks_gcn_validate.py
+-rw-r--r--   0        0        0     5739 2023-05-29 15:18:35.957637 gwcelery-2.1.1/gwcelery/tests/test_tasks_gracedb.py
+-rw-r--r--   0        0        0     9591 2023-05-29 15:18:35.957637 gwcelery-2.1.1/gwcelery/tests/test_tasks_gwskynet.py
+-rw-r--r--   0        0        0     3662 2023-05-29 15:18:35.957637 gwcelery-2.1.1/gwcelery/tests/test_tasks_igwn_alert.py
+-rw-r--r--   0        0        0    22955 2023-05-29 15:18:35.957637 gwcelery-2.1.1/gwcelery/tests/test_tasks_inference.py
+-rw-r--r--   0        0        0    33299 2023-05-29 15:18:35.957637 gwcelery-2.1.1/gwcelery/tests/test_tasks_orchestrator.py
+-rw-r--r--   0        0        0     1647 2023-05-29 15:18:35.957637 gwcelery-2.1.1/gwcelery/tests/test_tasks_p_astro.py
+-rw-r--r--   0        0        0    25523 2023-05-29 15:18:35.958637 gwcelery-2.1.1/gwcelery/tests/test_tasks_raven.py
+-rw-r--r--   0        0        0     4724 2023-05-29 15:18:35.958637 gwcelery-2.1.1/gwcelery/tests/test_tasks_rrt_utils.py
+-rw-r--r--   0        0        0     5035 2023-05-29 15:18:35.958637 gwcelery-2.1.1/gwcelery/tests/test_tasks_skymaps.py
+-rw-r--r--   0        0        0    40127 2023-05-29 15:18:35.958637 gwcelery-2.1.1/gwcelery/tests/test_tasks_superevents.py
+-rw-r--r--   0        0        0      637 2023-05-29 15:18:35.958637 gwcelery-2.1.1/gwcelery/tests/test_tempfile.py
+-rw-r--r--   0        0        0     3520 2023-05-29 15:18:35.958637 gwcelery-2.1.1/gwcelery/tests/test_tools_condor.py
+-rw-r--r--   0        0        0     1098 2023-05-29 15:18:35.958637 gwcelery-2.1.1/gwcelery/tests/test_tools_condor_submit_helper.py
+-rw-r--r--   0        0        0      633 2023-05-29 15:18:35.958637 gwcelery-2.1.1/gwcelery/tests/test_tools_flask.py
+-rw-r--r--   0        0        0     9668 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/tests/test_tools_nagios.py
+-rw-r--r--   0        0        0      269 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/tests/test_util.py
+-rw-r--r--   0        0        0    22392 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/tests/test_views.py
+-rw-r--r--   0        0        0      216 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/tools/__init__.py
+-rw-r--r--   0        0        0     2948 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/tools/condor.py
+-rw-r--r--   0        0        0     1120 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/tools/condor_submit_helper.py
+-rw-r--r--   0        0        0     1938 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/tools/flask.py
+-rw-r--r--   0        0        0     6624 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/tools/nagios.py
+-rw-r--r--   0        0        0      413 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/util/__init__.py
+-rw-r--r--   0        0        0     1007 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/util/cmdline.py
+-rw-r--r--   0        0        0      453 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/util/matplotlib.py
+-rw-r--r--   0        0        0      390 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/util/proxy.py
+-rw-r--r--   0        0        0      514 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/util/resources.py
+-rw-r--r--   0        0        0      253 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/util/sphinx.py
+-rw-r--r--   0        0        0      941 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/util/tempfile.py
+-rw-r--r--   0        0        0    19058 2023-05-29 15:18:35.960637 gwcelery-2.1.1/gwcelery/views.py
+-rw-r--r--   0        0        0      365 2023-05-29 15:18:35.960637 gwcelery-2.1.1/gwcelery/voevent/__init__.py
+-rw-r--r--   0        0        0     6387 2023-05-29 15:18:35.960637 gwcelery-2.1.1/gwcelery/voevent/bootsteps.py
+-rw-r--r--   0        0        0     1063 2023-05-29 15:18:35.960637 gwcelery-2.1.1/gwcelery/voevent/logging.py
+-rw-r--r--   0        0        0      779 2023-05-29 15:18:35.960637 gwcelery-2.1.1/gwcelery/voevent/signals.py
+-rw-r--r--   0        0        0      852 2023-05-29 15:18:35.960637 gwcelery-2.1.1/gwcelery/voevent/subscriber.py
+-rw-r--r--   0        0        0     1454 2023-05-29 15:18:35.960637 gwcelery-2.1.1/gwcelery/voevent/util.py
+-rw-r--r--   0        0        0     6099 2023-05-29 15:18:46.862686 gwcelery-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4525 1970-01-01 00:00:00.000000 gwcelery-2.1.1/PKG-INFO
```

### Comparing `gwcelery-2.1.0/CHANGES.rst` & `gwcelery-2.1.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 Changelog
 =========
 
+2.1.1 "Lone Island Mountain Devil" (2023-05-29)
+-----------------------------------------------
+
+-   Upgrade ligo-followup-advocate to v1.2.3
+
+-   Bump ligo.em-bright to v1.1.3 to be compatible with schema of online PE
+    files with spinning waveforms.
+
+-   Pin astropy to "!=5.3" until a bug plotting omega scans with gwpy is
+    resolved.
+
 2.1.0 "Jersey Devil" (2023-05-19)
 ---------------------------------
 
 -   Add GWSkyNet to annotate CBC all-sky search superevents. Only the
     superevents that meet the following conditions will be annotated by
     GWSkyNet: 1. A network of signal-to-noise ratio of greater
     than or equal to 7.0; 2. The SNRs in at least two detectors are no less
```

### Comparing `gwcelery-2.1.0/LICENSE.rst` & `gwcelery-2.1.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/README.rst` & `gwcelery-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/Makefile` & `gwcelery-2.1.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/_static/acceptance-tests-checklist.png` & `gwcelery-2.1.1/doc/_static/acceptance-tests-checklist.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/_static/celeryevent-screenshot.png` & `gwcelery-2.1.1/doc/_static/celeryevent-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/_static/deployment-screenshot.png` & `gwcelery-2.1.1/doc/_static/deployment-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/_static/flask-screenshot.png` & `gwcelery-2.1.1/doc/_static/flask-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/_static/flower-screenshot.png` & `gwcelery-2.1.1/doc/_static/flower-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/_static/logo-0.5x.png` & `gwcelery-2.1.1/doc/_static/logo-0.5x.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/_static/logo.png` & `gwcelery-2.1.1/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/_static/sentry-screenshot.png` & `gwcelery-2.1.1/doc/_static/sentry-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/conf.py` & `gwcelery-2.1.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/configuration.rst` & `gwcelery-2.1.1/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/contributing.rst` & `gwcelery-2.1.1/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/deployment.rst` & `gwcelery-2.1.1/doc/deployment.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/design.rst` & `gwcelery-2.1.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/gwcelery.tasks.detchar.rst` & `gwcelery-2.1.1/doc/gwcelery.tasks.detchar.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/gwcelery.tasks.em_bright.rst` & `gwcelery-2.1.1/doc/gwcelery.tasks.em_bright.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/gwcelery.tasks.external_triggers.rst` & `gwcelery-2.1.1/doc/gwcelery.tasks.external_triggers.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/gwcelery.tasks.orchestrator.rst` & `gwcelery-2.1.1/doc/gwcelery.tasks.orchestrator.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/gwcelery.tasks.rst` & `gwcelery-2.1.1/doc/gwcelery.tasks.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/gwcelery.tasks.superevents.rst` & `gwcelery-2.1.1/doc/gwcelery.tasks.superevents.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/htcondor.rst` & `gwcelery-2.1.1/doc/htcondor.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/index.rst` & `gwcelery-2.1.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/make.bat` & `gwcelery-2.1.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/monitoring.rst` & `gwcelery-2.1.1/doc/monitoring.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/doc/quickstart.rst` & `gwcelery-2.1.1/doc/quickstart.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/__init__.py` & `gwcelery-2.1.1/gwcelery/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/_version.py` & `gwcelery-2.1.1/gwcelery/_version.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/conf/__init__.py` & `gwcelery-2.1.1/gwcelery/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/conf/dev.py` & `gwcelery-2.1.1/gwcelery/conf/dev.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/conf/minikube.py` & `gwcelery-2.1.1/gwcelery/conf/minikube.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/conf/playground.py` & `gwcelery-2.1.1/gwcelery/conf/playground.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/conf/production.py` & `gwcelery-2.1.1/gwcelery/conf/production.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/conf/test.py` & `gwcelery-2.1.1/gwcelery/conf/test.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/data/first2years/gstlal.xml.gz` & `gwcelery-2.1.1/gwcelery/data/first2years/gstlal.xml.gz`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/data/gwcelery.sub` & `gwcelery-2.1.1/gwcelery/data/gwcelery.sub`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/email/bootsteps.py` & `gwcelery-2.1.1/gwcelery/email/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/email/signals.py` & `gwcelery-2.1.1/gwcelery/email/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/flask.py` & `gwcelery-2.1.1/gwcelery/flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/igwn_alert/__init__.py` & `gwcelery-2.1.1/gwcelery/igwn_alert/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/igwn_alert/bootsteps.py` & `gwcelery-2.1.1/gwcelery/igwn_alert/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/igwn_alert/signals.py` & `gwcelery-2.1.1/gwcelery/igwn_alert/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/kafka/bootsteps.py` & `gwcelery-2.1.1/gwcelery/kafka/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/kafka/signals.py` & `gwcelery-2.1.1/gwcelery/kafka/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/sentry/__init__.py` & `gwcelery-2.1.1/gwcelery/sentry/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/sentry/integrations/condor.py` & `gwcelery-2.1.1/gwcelery/sentry/integrations/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/sentry/integrations/requests.py` & `gwcelery-2.1.1/gwcelery/sentry/integrations/requests.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/sentry/integrations/subprocess.py` & `gwcelery-2.1.1/gwcelery/sentry/integrations/subprocess.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/static/typeahead.css` & `gwcelery-2.1.1/gwcelery/static/typeahead.css`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/static/vega/index.html` & `gwcelery-2.1.1/gwcelery/static/vega/index.html`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/__init__.py` & `gwcelery-2.1.1/gwcelery/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/alerts.py` & `gwcelery-2.1.1/gwcelery/tasks/alerts.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/bayestar.py` & `gwcelery-2.1.1/gwcelery/tasks/bayestar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/circulars.py` & `gwcelery-2.1.1/gwcelery/tasks/circulars.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/condor.py` & `gwcelery-2.1.1/gwcelery/tasks/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/core.py` & `gwcelery-2.1.1/gwcelery/tasks/core.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/detchar.py` & `gwcelery-2.1.1/gwcelery/tasks/detchar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/em_bright.py` & `gwcelery-2.1.1/gwcelery/tasks/em_bright.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/external_skymaps.py` & `gwcelery-2.1.1/gwcelery/tasks/external_skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/external_triggers.py` & `gwcelery-2.1.1/gwcelery/tasks/external_triggers.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/first2years.py` & `gwcelery-2.1.1/gwcelery/tasks/first2years.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/first2years_external.py` & `gwcelery-2.1.1/gwcelery/tasks/first2years_external.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/gcn.py` & `gwcelery-2.1.1/gwcelery/tasks/gcn.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/gracedb.py` & `gwcelery-2.1.1/gwcelery/tasks/gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/gwskynet.py` & `gwcelery-2.1.1/gwcelery/tasks/gwskynet.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/igwn_alert.py` & `gwcelery-2.1.1/gwcelery/tasks/igwn_alert.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/inference.py` & `gwcelery-2.1.1/gwcelery/tasks/inference.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/legacy_gracedb.py` & `gwcelery-2.1.1/gwcelery/tasks/legacy_gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/notice_text.py` & `gwcelery-2.1.1/gwcelery/tasks/notice_text.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/orchestrator.py` & `gwcelery-2.1.1/gwcelery/tasks/orchestrator.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/p_astro.py` & `gwcelery-2.1.1/gwcelery/tasks/p_astro.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/raven.py` & `gwcelery-2.1.1/gwcelery/tasks/raven.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/rrt_utils.py` & `gwcelery-2.1.1/gwcelery/tasks/rrt_utils.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/skymaps.py` & `gwcelery-2.1.1/gwcelery/tasks/skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tasks/superevents.py` & `gwcelery-2.1.1/gwcelery/tasks/superevents.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/templates/fits_header.jinja2` & `gwcelery-2.1.1/gwcelery/templates/fits_header.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/templates/index.jinja2` & `gwcelery-2.1.1/gwcelery/templates/index.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/templates/lalinference.jinja2` & `gwcelery-2.1.1/gwcelery/templates/lalinference.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/templates/rapidpe.jinja2` & `gwcelery-2.1.1/gwcelery/templates/rapidpe.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/templates/vector_table.jinja2` & `gwcelery-2.1.1/gwcelery/templates/vector_table.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/conftest.py` & `gwcelery-2.1.1/gwcelery/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/G000012_S0040_preferred.json` & `gwcelery-2.1.1/gwcelery/tests/data/G000012_S0040_preferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/G298048-1-Initial.xml` & `gwcelery-2.1.1/gwcelery/tests/data/G298048-1-Initial.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/G298048_log.json` & `gwcelery-2.1.1/gwcelery/tests/data/G298048_log.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json` & `gwcelery-2.1.1/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/MS220722v.xml` & `gwcelery-2.1.1/gwcelery/tests/data/MS220722v.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits` & `gwcelery-2.1.1/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/S230413b.json` & `gwcelery-2.1.1/gwcelery/tests/data/S230413b.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/S230413g.json` & `gwcelery-2.1.1/gwcelery/tests/data/S230413g.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/S230413h.json` & `gwcelery-2.1.1/gwcelery/tests/data/S230413h.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/T0212_S0039_preferred.json` & `gwcelery-2.1.1/gwcelery/tests/data/T0212_S0039_preferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json` & `gwcelery-2.1.1/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/T0219_S0041_nopreferred.json` & `gwcelery-2.1.1/gwcelery/tests/data/T0219_S0041_nopreferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/agile_grb_gcn.xml` & `gwcelery-2.1.1/gwcelery/tests/data/agile_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/coinc.xml` & `gwcelery-2.1.1/gwcelery/tests/data/coinc.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/externaltrigger_original_data.xml` & `gwcelery-2.1.1/gwcelery/tests/data/externaltrigger_original_data.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/fermi_grb_gcn.xml` & `gwcelery-2.1.1/gwcelery/tests/data/fermi_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/fermi_initial_grb_gcn.xml` & `gwcelery-2.1.1/gwcelery/tests/data/fermi_initial_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/fermi_noise_gcn.xml` & `gwcelery-2.1.1/gwcelery/tests/data/fermi_noise_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/fermi_noise_gcn_2.xml` & `gwcelery-2.1.1/gwcelery/tests/data/fermi_noise_gcn_2.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml` & `gwcelery-2.1.1/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml` & `gwcelery-2.1.1/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/fits_header_result.html` & `gwcelery-2.1.1/gwcelery/tests/data/fits_header_result.html`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/gracedb_externaltrigger_log.json` & `gwcelery-2.1.1/gwcelery/tests/data/gracedb_externaltrigger_log.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_detchar.json` & `gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_detchar.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_exttrig_creation.json` & `gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_exttrig_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json` & `gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_psd.json` & `gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_psd.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_snews_creation.json` & `gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_snews_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_snews_test_creation.json` & `gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_snews_test_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_subgrb_creation.json` & `gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_subgrb_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_superevent_creation.json` & `gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_superevent_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/igwn_alert_voevent.json` & `gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_voevent.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/integral_grb_gcn.xml` & `gwcelery-2.1.1/gwcelery/tests/data/integral_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/integral_mdc_gcn.xml` & `gwcelery-2.1.1/gwcelery/tests/data/integral_mdc_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf` & `gwcelery-2.1.1/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/llhoft/omegascan/scanme.gwf` & `gwcelery-2.1.1/gwcelery/tests/data/llhoft/omegascan/scanme.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf` & `gwcelery-2.1.1/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/lvalert_event_creation.json` & `gwcelery-2.1.1/gwcelery/tests/data/lvalert_event_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/lvalert_xmpp.xml` & `gwcelery-2.1.1/gwcelery/tests/data/lvalert_xmpp.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/mock_superevent_object.json` & `gwcelery-2.1.1/gwcelery/tests/data/mock_superevent_object.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite` & `gwcelery-2.1.1/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/psd.xml.gz` & `gwcelery-2.1.1/gwcelery/tests/data/psd.xml.gz`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/rrt_small_area.fits` & `gwcelery-2.1.1/gwcelery/tests/data/rrt_small_area.fits`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/sample_events.json` & `gwcelery-2.1.1/gwcelery/tests/data/sample_events.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/samples.hdf5` & `gwcelery-2.1.1/gwcelery/tests/data/samples.hdf5`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/scaler_set_all.pickle` & `gwcelery-2.1.1/gwcelery/tests/data/scaler_set_all.pickle`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/snews_gcn.xml` & `gwcelery-2.1.1/gwcelery/tests/data/snews_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/snews_gcn_test.xml` & `gwcelery-2.1.1/gwcelery/tests/data/snews_gcn_test.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/superevents.json` & `gwcelery-2.1.1/gwcelery/tests/data/superevents.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/swift_grb_gcn.xml` & `gwcelery-2.1.1/gwcelery/tests/data/swift_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/data/test_classifier.pickle` & `gwcelery-2.1.1/gwcelery/tests/data/test_classifier.pickle`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/process.py` & `gwcelery-2.1.1/gwcelery/tests/process.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_sentry.py` & `gwcelery-2.1.1/gwcelery/tests/test_sentry.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tasks_alerts.py` & `gwcelery-2.1.1/gwcelery/tests/test_tasks_alerts.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tasks_alerts_validate.py` & `gwcelery-2.1.1/gwcelery/tests/test_tasks_alerts_validate.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tasks_bayestar.py` & `gwcelery-2.1.1/gwcelery/tests/test_tasks_bayestar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tasks_circulars.py` & `gwcelery-2.1.1/gwcelery/tests/test_tasks_circulars.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tasks_condor.py` & `gwcelery-2.1.1/gwcelery/tests/test_tasks_condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tasks_detchar.py` & `gwcelery-2.1.1/gwcelery/tests/test_tasks_detchar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tasks_em_bright.py` & `gwcelery-2.1.1/gwcelery/tests/test_tasks_em_bright.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tasks_external_skymaps.py` & `gwcelery-2.1.1/gwcelery/tests/test_tasks_external_skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tasks_external_triggers.py` & `gwcelery-2.1.1/gwcelery/tests/test_tasks_external_triggers.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tasks_first2years.py` & `gwcelery-2.1.1/gwcelery/tests/test_tasks_first2years.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tasks_first2years_external.py` & `gwcelery-2.1.1/gwcelery/tests/test_tasks_first2years_external.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tasks_gcn.py` & `gwcelery-2.1.1/gwcelery/tests/test_tasks_gcn.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tasks_gcn_validate.py` & `gwcelery-2.1.1/gwcelery/tests/test_tasks_gcn_validate.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tasks_gracedb.py` & `gwcelery-2.1.1/gwcelery/tests/test_tasks_gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tasks_gwskynet.py` & `gwcelery-2.1.1/gwcelery/tests/test_tasks_gwskynet.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tasks_igwn_alert.py` & `gwcelery-2.1.1/gwcelery/tests/test_tasks_igwn_alert.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tasks_inference.py` & `gwcelery-2.1.1/gwcelery/tests/test_tasks_inference.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tasks_orchestrator.py` & `gwcelery-2.1.1/gwcelery/tests/test_tasks_orchestrator.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tasks_p_astro.py` & `gwcelery-2.1.1/gwcelery/tests/test_tasks_p_astro.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tasks_raven.py` & `gwcelery-2.1.1/gwcelery/tests/test_tasks_raven.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tasks_rrt_utils.py` & `gwcelery-2.1.1/gwcelery/tests/test_tasks_rrt_utils.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tasks_skymaps.py` & `gwcelery-2.1.1/gwcelery/tests/test_tasks_skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tasks_superevents.py` & `gwcelery-2.1.1/gwcelery/tests/test_tasks_superevents.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tempfile.py` & `gwcelery-2.1.1/gwcelery/tests/test_tempfile.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tools_condor.py` & `gwcelery-2.1.1/gwcelery/tests/test_tools_condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tools_condor_submit_helper.py` & `gwcelery-2.1.1/gwcelery/tests/test_tools_condor_submit_helper.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tools_flask.py` & `gwcelery-2.1.1/gwcelery/tests/test_tools_flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_tools_nagios.py` & `gwcelery-2.1.1/gwcelery/tests/test_tools_nagios.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tests/test_views.py` & `gwcelery-2.1.1/gwcelery/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tools/condor.py` & `gwcelery-2.1.1/gwcelery/tools/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tools/condor_submit_helper.py` & `gwcelery-2.1.1/gwcelery/tools/condor_submit_helper.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tools/flask.py` & `gwcelery-2.1.1/gwcelery/tools/flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/tools/nagios.py` & `gwcelery-2.1.1/gwcelery/tools/nagios.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/util/cmdline.py` & `gwcelery-2.1.1/gwcelery/util/cmdline.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/util/resources.py` & `gwcelery-2.1.1/gwcelery/util/resources.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/util/tempfile.py` & `gwcelery-2.1.1/gwcelery/util/tempfile.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/views.py` & `gwcelery-2.1.1/gwcelery/views.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/voevent/bootsteps.py` & `gwcelery-2.1.1/gwcelery/voevent/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/voevent/logging.py` & `gwcelery-2.1.1/gwcelery/voevent/logging.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/voevent/signals.py` & `gwcelery-2.1.1/gwcelery/voevent/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/voevent/subscriber.py` & `gwcelery-2.1.1/gwcelery/voevent/subscriber.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/gwcelery/voevent/util.py` & `gwcelery-2.1.1/gwcelery/voevent/util.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.0/pyproject.toml` & `gwcelery-2.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gwcelery"
-version = "2.1.0"
+version = "2.1.1"
 description = "Low-latency pipeline for annotating IGWN events"
 readme = "README.rst"
 authors = [
     "Deep Chatterjee <deep.chatterjee@ligo.org>",
     "Cody Messick <cody.messick@ligo.org>",
     "Geoffrey Mo <geoffrey.mo@ligo.org>",
     "Leo Singer <leo.singer@ligo.org>"
@@ -48,15 +48,15 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://git.ligo.org/emfollow/gwcelery/issues"
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.11"
 adc-streaming = ">=2.3.0"  # https://github.com/astronomy-commons/adc-streaming/pull/62
-astropy = ">=4.3.1"  # https://github.com/astropy/astropy/issues/11879
+astropy = ">=4.3.1,!=5.3"  # https://github.com/astropy/astropy/issues/11879, https://github.com/gwpy/gwpy/issues/1629
 bilby = ">=2.1.1"
 bilby_pipe = "==1.0.10"
 celery = {version = ">=5.1", extras = ["redis"]}
 ciecplib = {version = "*", extras = ["kerberos"]}  # for renew-cert.sh
 click = ">=7"
 comet = "*"
 confluent-kafka = "^1.9.2"
@@ -71,19 +71,19 @@
 hop-client = ">=0.7.0"  # https://github.com/scimma/hop-client/pull/176
 igwn-alert = ">=0.2.2"
 igwn-gwalert-schema = "^1.0.0"
 imapclient = "*"
 importlib-metadata = { version = "*"}
 jinja2 = ">=2.11.2"  # https://github.com/pallets/jinja/issues/1168
 lalsuite = ">=6.82"  # https://git.ligo.org/lscsoft/lalsuite/-/issues/414
-ligo-followup-advocate = ">=1.2.2"
+ligo-followup-advocate = ">=1.2.3"
 ligo-gracedb = ">=2.7.5"  # https://git.ligo.org/lscsoft/gracedb-client/-/issues/28
 ligo-raven = ">=3.2"
 ligo-segments = "*"
-"ligo.em-bright" = ">=1.1.2"  # https://git.ligo.org/computing/sccb/-/issues/1166
+"ligo.em-bright" = ">=1.1.3"  # https://git.ligo.org/emfollow/em-properties/em-bright/-/issues/34
 "ligo.skymap" = ">=1.0.4"  # https://git.ligo.org/lscsoft/ligo.skymap/-/merge_requests/299
 lscsoft-glue = "*"
 lxml = "*"
 matplotlib = "<3.7"  # Matplotlib changed an axes behaviour which breaks some of our plotting scripts. When gwpy has a new release, we can unpin this.
 numba = ">=0.56"  # Poetry update chooses an old version of numba and its deps that break the python3.9 and 3.10 build tests if this is not specified; dependence on numba comes from rift. Version chosen because it adds python 3.10 support. This requirement can be dropped here if RIFT adds it https://git.ligo.org/rapidpe-rift/rift/-/issues/24
 numpy = "*"
 p_astro = ">=1.0.1"  # https://git.ligo.org/lscsoft/p-astro/-/merge_requests/40
```

### Comparing `gwcelery-2.1.0/PKG-INFO` & `gwcelery-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwcelery
-Version: 2.1.0
+Version: 2.1.1
 Summary: Low-latency pipeline for annotating IGWN events
 Home-page: https://git.ligo.org/emfollow/gwcelery
 License: GPL-2.0+
 Author: Deep Chatterjee
 Author-email: deep.chatterjee@ligo.org
 Requires-Python: >=3.9,<3.11
 Classifier: Development Status :: 4 - Beta
@@ -19,15 +19,15 @@
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides-Extra: doc
 Provides-Extra: test
 Requires-Dist: GWSkyNet (>=2.3.0)
 Requires-Dist: RIFT (>=0.0.15.7)
 Requires-Dist: adc-streaming (>=2.3.0)
-Requires-Dist: astropy (>=4.3.1)
+Requires-Dist: astropy (>=4.3.1,!=5.3)
 Requires-Dist: bilby (>=2.1.1)
 Requires-Dist: bilby_pipe (==1.0.10)
 Requires-Dist: celery[redis] (>=5.1)
 Requires-Dist: ciecplib[kerberos]
 Requires-Dist: click (>=7)
 Requires-Dist: comet
 Requires-Dist: confluent-kafka (>=1.9.2,<2.0.0)
@@ -42,20 +42,20 @@
 Requires-Dist: hop-client (>=0.7.0)
 Requires-Dist: igwn-alert (>=0.2.2)
 Requires-Dist: igwn-gwalert-schema (>=1.0.0,<2.0.0)
 Requires-Dist: imapclient
 Requires-Dist: importlib-metadata
 Requires-Dist: jinja2 (>=2.11.2)
 Requires-Dist: lalsuite (>=6.82)
-Requires-Dist: ligo-followup-advocate (>=1.2.2)
+Requires-Dist: ligo-followup-advocate (>=1.2.3)
 Requires-Dist: ligo-gracedb (>=2.7.5)
 Requires-Dist: ligo-raven (>=3.2)
 Requires-Dist: ligo-rrt-chat (>=0.1.1)
 Requires-Dist: ligo-segments
-Requires-Dist: ligo.em-bright (>=1.1.2)
+Requires-Dist: ligo.em-bright (>=1.1.3)
 Requires-Dist: ligo.skymap (>=1.0.4)
 Requires-Dist: lscsoft-glue
 Requires-Dist: lxml
 Requires-Dist: matplotlib (<3.7)
 Requires-Dist: numba (>=0.56)
 Requires-Dist: numpy
 Requires-Dist: p_astro (>=1.0.1)
```

