# Comparing `tmp/pyro-ppl-1.8.4.tar.gz` & `tmp/pyro-ppl-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyro-ppl-1.8.4.tar", last modified: Tue Jan  3 22:30:10 2023, max compression
+gzip compressed data, was "pyro-ppl-1.8.5.tar", last modified: Mon May 29 03:00:47 2023, max compression
```

## Comparing `pyro-ppl-1.8.4.tar` & `pyro-ppl-1.8.5.tar`

### file list

```diff
@@ -1,366 +1,367 @@
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:10.044647 pyro-ppl-1.8.4/
--rw-r--r--   0 fritzo     (501) staff       (20)    11358 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/LICENSE.md
--rw-r--r--   0 fritzo     (501) staff       (20)       60 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/MANIFEST.in
--rw-r--r--   0 fritzo     (501) staff       (20)     4742 2023-01-03 22:30:10.044729 pyro-ppl-1.8.4/PKG-INFO
--rw-r--r--   0 fritzo     (501) staff       (20)     4538 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/README.md
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:09.980047 pyro-ppl-1.8.4/pyro/
--rw-r--r--   0 fritzo     (501) staff       (20)     1391 2023-01-03 22:26:56.000000 pyro-ppl-1.8.4/pyro/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)      113 2023-01-03 22:30:09.000000 pyro-ppl-1.8.4/pyro/_version.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:09.980931 pyro-ppl-1.8.4/pyro/contrib/
--rw-r--r--   0 fritzo     (501) staff       (20)      693 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)      317 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/autoguide.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:09.981607 pyro-ppl-1.8.4/pyro/contrib/autoname/
--rw-r--r--   0 fritzo     (501) staff       (20)      486 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/autoname/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5143 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/autoname/autoname.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8618 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/autoname/named.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6482 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/autoname/scoping.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:09.981964 pyro-ppl-1.8.4/pyro/contrib/bnn/
--rw-r--r--   0 fritzo     (501) staff       (20)      177 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/bnn/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5383 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/bnn/hidden_layer.py
--rw-r--r--   0 fritzo     (501) staff       (20)      490 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/bnn/utils.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:09.982085 pyro-ppl-1.8.4/pyro/contrib/cevae/
--rw-r--r--   0 fritzo     (501) staff       (20)    22960 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/cevae/__init__.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:09.982327 pyro-ppl-1.8.4/pyro/contrib/conjugate/
--rw-r--r--   0 fritzo     (501) staff       (20)        0 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/conjugate/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9073 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/conjugate/infer.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:09.982612 pyro-ppl-1.8.4/pyro/contrib/easyguide/
--rw-r--r--   0 fritzo     (501) staff       (20)      206 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/easyguide/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    12878 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/easyguide/easyguide.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:09.983755 pyro-ppl-1.8.4/pyro/contrib/epidemiology/
--rw-r--r--   0 fritzo     (501) staff       (20)      406 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/epidemiology/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    49835 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/epidemiology/compartmental.py
--rw-r--r--   0 fritzo     (501) staff       (20)    13549 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/epidemiology/distributions.py
--rw-r--r--   0 fritzo     (501) staff       (20)    51169 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/epidemiology/models.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10990 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/epidemiology/util.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:09.984789 pyro-ppl-1.8.4/pyro/contrib/examples/
--rw-r--r--   0 fritzo     (501) staff       (20)        0 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/examples/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6760 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/examples/bart.py
--rw-r--r--   0 fritzo     (501) staff       (20)      694 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/examples/finance.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2896 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/examples/multi_mnist.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1547 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/examples/nextstrain.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6875 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/examples/polyphonic_data_loader.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7442 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/examples/scanvi_data.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1556 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/examples/util.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:09.985353 pyro-ppl-1.8.4/pyro/contrib/forecast/
--rw-r--r--   0 fritzo     (501) staff       (20)      360 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/forecast/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8823 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/forecast/evaluate.py
--rw-r--r--   0 fritzo     (501) staff       (20)    23299 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/forecast/forecaster.py
--rw-r--r--   0 fritzo     (501) staff       (20)    16054 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/forecast/util.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:09.985513 pyro-ppl-1.8.4/pyro/contrib/funsor/
--rw-r--r--   0 fritzo     (501) staff       (20)     1263 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/funsor/__init__.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:09.986813 pyro-ppl-1.8.4/pyro/contrib/funsor/handlers/
--rw-r--r--   0 fritzo     (501) staff       (20)      912 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/funsor/handlers/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9727 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/funsor/handlers/enum_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7625 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/funsor/handlers/named_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)    15224 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/funsor/handlers/plate_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1076 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/funsor/handlers/primitives.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1804 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/funsor/handlers/replay_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8559 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/funsor/handlers/runtime.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3632 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/funsor/handlers/trace_messenger.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:09.987630 pyro-ppl-1.8.4/pyro/contrib/funsor/infer/
--rw-r--r--   0 fritzo     (501) staff       (20)      514 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/funsor/infer/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2922 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/funsor/infer/discrete.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1652 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/funsor/infer/elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1698 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/funsor/infer/trace_elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)    12665 2022-04-10 23:10:00.000000 pyro-ppl-1.8.4/pyro/contrib/funsor/infer/traceenum_elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1882 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/funsor/infer/tracetmc_elbo.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:09.988099 pyro-ppl-1.8.4/pyro/contrib/gp/
--rw-r--r--   0 fritzo     (501) staff       (20)      340 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/gp/__init__.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:09.989556 pyro-ppl-1.8.4/pyro/contrib/gp/kernels/
--rw-r--r--   0 fritzo     (501) staff       (20)     1533 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/gp/kernels/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1577 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/gp/kernels/brownian.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3699 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/gp/kernels/coregionalize.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2646 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/gp/kernels/dot_product.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5740 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/gp/kernels/isotropic.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8446 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/gp/kernels/kernel.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2424 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/gp/kernels/periodic.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1536 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/gp/kernels/static.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:09.991067 pyro-ppl-1.8.4/pyro/contrib/gp/likelihoods/
--rw-r--r--   0 fritzo     (501) staff       (20)      897 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/gp/likelihoods/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1988 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/gp/likelihoods/binary.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1677 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/gp/likelihoods/gaussian.py
--rw-r--r--   0 fritzo     (501) staff       (20)      875 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/gp/likelihoods/likelihood.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2859 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/gp/likelihoods/multi_class.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1884 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/gp/likelihoods/poisson.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:09.993085 pyro-ppl-1.8.4/pyro/contrib/gp/models/
--rw-r--r--   0 fritzo     (501) staff       (20)      546 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/gp/models/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3897 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/gp/models/gplvm.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8932 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/gp/models/gpr.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9145 2022-05-12 17:23:25.000000 pyro-ppl-1.8.4/pyro/contrib/gp/models/model.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11002 2022-06-12 12:50:39.000000 pyro-ppl-1.8.4/pyro/contrib/gp/models/sgpr.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6859 2022-05-12 17:23:25.000000 pyro-ppl-1.8.4/pyro/contrib/gp/models/vgp.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8417 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/gp/models/vsgp.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8058 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/gp/parameterized.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7152 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/gp/util.py
--rw-r--r--   0 fritzo     (501) staff       (20)    15591 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/minipyro.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:09.994132 pyro-ppl-1.8.4/pyro/contrib/mue/
--rw-r--r--   0 fritzo     (501) staff       (20)        0 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/mue/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6066 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/mue/dataloaders.py
--rw-r--r--   0 fritzo     (501) staff       (20)    13358 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/mue/missingdatahmm.py
--rw-r--r--   0 fritzo     (501) staff       (20)    34333 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/mue/models.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9017 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/mue/statearrangers.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:09.994788 pyro-ppl-1.8.4/pyro/contrib/oed/
--rw-r--r--   0 fritzo     (501) staff       (20)     3789 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/oed/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    44802 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/oed/eig.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:09.995319 pyro-ppl-1.8.4/pyro/contrib/oed/glmm/
--rw-r--r--   0 fritzo     (501) staff       (20)     1551 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/oed/glmm/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    16377 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/oed/glmm/glmm.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11375 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/oed/glmm/guides.py
--rw-r--r--   0 fritzo     (501) staff       (20)      867 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/oed/search.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1230 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/oed/util.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:09.995653 pyro-ppl-1.8.4/pyro/contrib/randomvariable/
--rw-r--r--   0 fritzo     (501) staff       (20)      193 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/randomvariable/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5424 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/randomvariable/random_variable.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:09.996338 pyro-ppl-1.8.4/pyro/contrib/timeseries/
--rw-r--r--   0 fritzo     (501) staff       (20)      711 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/timeseries/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2211 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/timeseries/base.py
--rw-r--r--   0 fritzo     (501) staff       (20)    23487 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/timeseries/gp.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6439 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/timeseries/lgssm.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11250 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/timeseries/lgssmgp.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:09.997403 pyro-ppl-1.8.4/pyro/contrib/tracking/
--rw-r--r--   0 fritzo     (501) staff       (20)      167 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/tracking/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    19243 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/tracking/assignment.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3576 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/tracking/distributions.py
--rw-r--r--   0 fritzo     (501) staff       (20)    16561 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/tracking/dynamic_models.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7796 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/tracking/extended_kalman_filter.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7266 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/tracking/hashing.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4544 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/tracking/measurements.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2118 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/contrib/util.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:10.014566 pyro-ppl-1.8.4/pyro/distributions/
--rw-r--r--   0 fritzo     (501) staff       (20)     5548 2022-12-27 22:08:32.000000 pyro-ppl-1.8.4/pyro/distributions/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3985 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/affine_beta.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7393 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/asymmetriclaplace.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4062 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/avf_mvn.py
--rw-r--r--   0 fritzo     (501) staff       (20)    20914 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/coalescent.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2430 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/conditional.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10824 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/conjugate.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4391 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/constraints.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3066 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/delta.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10357 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/diag_normal_mixture.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9013 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/diag_normal_mixture_shared_cov.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8443 2022-04-10 23:10:00.000000 pyro-ppl-1.8.4/pyro/distributions/distribution.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6765 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/empirical.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1885 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/extended.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1290 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/folded.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7983 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/gaussian_scale_mixture.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6571 2022-12-27 22:08:32.000000 pyro-ppl-1.8.4/pyro/distributions/grouped_normal_normal.py
--rw-r--r--   0 fritzo     (501) staff       (20)    54250 2022-10-30 17:11:32.000000 pyro-ppl-1.8.4/pyro/distributions/hmm.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2448 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/improper_uniform.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1429 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/inverse_gamma.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1661 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/kl.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2533 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/lkj.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5719 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/log_normal_negative_binomial.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5474 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/logistic.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6150 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/mixture.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5193 2022-06-12 12:50:39.000000 pyro-ppl-1.8.4/pyro/distributions/multivariate_studentt.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3381 2022-07-16 22:52:12.000000 pyro-ppl-1.8.4/pyro/distributions/nanmasked.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3176 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/omt_mvn.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6881 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/one_one_matching.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8360 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/one_two_matching.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2874 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/ordered_logistic.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3090 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/polya_gamma.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7441 2022-05-12 17:23:25.000000 pyro-ppl-1.8.4/pyro/distributions/projected_normal.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2933 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/rejector.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3637 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/relaxed_straight_through.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1125 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/score_parts.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11564 2022-12-27 22:08:32.000000 pyro-ppl-1.8.4/pyro/distributions/sine_bivariate_von_mises.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7318 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/sine_skewed.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2471 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/softlaplace.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7746 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/spanning_tree.cpp
--rw-r--r--   0 fritzo     (501) staff       (20)    22257 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/spanning_tree.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8208 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/stable.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:10.016043 pyro-ppl-1.8.4/pyro/distributions/testing/
--rw-r--r--   0 fritzo     (501) staff       (20)      215 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/testing/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)      421 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/testing/fakes.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10761 2022-07-10 14:38:43.000000 pyro-ppl-1.8.4/pyro/distributions/testing/gof.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1598 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/testing/naive_dirichlet.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1167 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/testing/rejection_exponential.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8842 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/testing/rejection_gamma.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3610 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/testing/special.py
--rw-r--r--   0 fritzo     (501) staff       (20)    13608 2022-11-06 16:58:27.000000 pyro-ppl-1.8.4/pyro/distributions/torch.py
--rw-r--r--   0 fritzo     (501) staff       (20)    20332 2022-10-02 18:17:50.000000 pyro-ppl-1.8.4/pyro/distributions/torch_distribution.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3142 2022-12-27 22:08:32.000000 pyro-ppl-1.8.4/pyro/distributions/torch_patch.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1180 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/torch_transform.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:10.022858 pyro-ppl-1.8.4/pyro/distributions/transforms/
--rw-r--r--   0 fritzo     (501) staff       (20)     6989 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    16342 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/affine_autoregressive.py
--rw-r--r--   0 fritzo     (501) staff       (20)    15805 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/affine_coupling.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2075 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/basic.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6147 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/batchnorm.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11702 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/block_autoregressive.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4260 2022-10-30 17:11:32.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/cholesky.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3383 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/discrete_cosine.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11680 2022-11-22 19:06:49.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/generalized_channel_permute.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2883 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/haar.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10536 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/householder.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2479 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/lower_cholesky_affine.py
--rw-r--r--   0 fritzo     (501) staff       (20)    13725 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/matrix_exponential.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9794 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/neural_autoregressive.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1072 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/normalize.py
--rw-r--r--   0 fritzo     (501) staff       (20)      921 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/ordered.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5299 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/permute.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8881 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/planar.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7076 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/polynomial.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2138 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/power.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8711 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/radial.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1664 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/softplus.py
--rw-r--r--   0 fritzo     (501) staff       (20)    24458 2022-10-30 02:11:10.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/spline.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11370 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/spline_autoregressive.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6917 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/spline_coupling.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6318 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/sylvester.py
--rw-r--r--   0 fritzo     (501) staff       (20)      809 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/unit_cholesky.py
--rw-r--r--   0 fritzo     (501) staff       (20)      282 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/transforms/utils.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1886 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/unit.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11913 2022-11-06 16:58:27.000000 pyro-ppl-1.8.4/pyro/distributions/util.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2694 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/von_mises_3d.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6861 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/distributions/zero_inflated.py
--rw-r--r--   0 fritzo     (501) staff       (20)      266 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/generic.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:10.027710 pyro-ppl-1.8.4/pyro/infer/
--rw-r--r--   0 fritzo     (501) staff       (20)     2041 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    15986 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/abstract_infer.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:10.029188 pyro-ppl-1.8.4/pyro/infer/autoguide/
--rw-r--r--   0 fritzo     (501) staff       (20)     1618 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/autoguide/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    19662 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/autoguide/effect.py
--rw-r--r--   0 fritzo     (501) staff       (20)    26014 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/autoguide/gaussian.py
--rw-r--r--   0 fritzo     (501) staff       (20)    49080 2022-11-25 23:04:16.000000 pyro-ppl-1.8.4/pyro/infer/autoguide/guides.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8270 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/autoguide/initialization.py
--rw-r--r--   0 fritzo     (501) staff       (20)    16327 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/autoguide/structured.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3089 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/autoguide/utils.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7251 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/csis.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11547 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/discrete.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9519 2022-11-12 16:14:55.000000 pyro-ppl-1.8.4/pyro/infer/elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10044 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/energy_distance.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8063 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/enum.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9701 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/importance.py
--rw-r--r--   0 fritzo     (501) staff       (20)    21726 2022-12-08 14:46:13.000000 pyro-ppl-1.8.4/pyro/infer/inspect.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:10.030557 pyro-ppl-1.8.4/pyro/infer/mcmc/
--rw-r--r--   0 fritzo     (501) staff       (20)      412 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/mcmc/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    23000 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/mcmc/adaptation.py
--rw-r--r--   0 fritzo     (501) staff       (20)    29191 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/mcmc/api.py
--rw-r--r--   0 fritzo     (501) staff       (20)    18829 2023-01-03 21:44:32.000000 pyro-ppl-1.8.4/pyro/infer/mcmc/hmc.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9270 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/mcmc/logger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2347 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/mcmc/mcmc_kernel.py
--rw-r--r--   0 fritzo     (501) staff       (20)    21893 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/mcmc/nuts.py
--rw-r--r--   0 fritzo     (501) staff       (20)    33006 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/mcmc/util.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11083 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/predictive.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9418 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/renyi_elbo.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:10.032655 pyro-ppl-1.8.4/pyro/infer/reparam/
--rw-r--r--   0 fritzo     (501) staff       (20)     1239 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/reparam/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4315 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/reparam/conjugate.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2076 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/reparam/discrete_cosine.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1594 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/reparam/haar.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6406 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/reparam/hmm.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3812 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/reparam/loc_scale.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5549 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/reparam/neutra.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1697 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/reparam/projected_normal.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2627 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/reparam/reparam.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1869 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/reparam/softmax.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2642 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/reparam/split.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10231 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/reparam/stable.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7481 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/reparam/strategies.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4312 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/reparam/structured.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1477 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/reparam/studentt.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1789 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/reparam/transform.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3913 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/reparam/unit_jacobian.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5720 2022-10-02 18:17:50.000000 pyro-ppl-1.8.4/pyro/infer/resampler.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11084 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/rws.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8713 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/smcfilter.py
--rw-r--r--   0 fritzo     (501) staff       (20)    12959 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/svgd.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5947 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/svi.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10334 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/trace_elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8173 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/trace_mean_field_elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10876 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/trace_mmd.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3367 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/trace_tail_adaptive_elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)    23531 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/traceenum_elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)    16984 2022-06-12 12:50:39.000000 pyro-ppl-1.8.4/pyro/infer/tracegraph_elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8714 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/infer/tracetmc_elbo.py
--rw-r--r--   0 fritzo     (501) staff       (20)    12502 2022-11-06 16:58:27.000000 pyro-ppl-1.8.4/pyro/infer/util.py
--rw-r--r--   0 fritzo     (501) staff       (20)      463 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/logger.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:10.033274 pyro-ppl-1.8.4/pyro/nn/
--rw-r--r--   0 fritzo     (501) staff       (20)      602 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/nn/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    13697 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/nn/auto_reg_nn.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5124 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/nn/dense_nn.py
--rw-r--r--   0 fritzo     (501) staff       (20)    31122 2022-11-12 16:14:55.000000 pyro-ppl-1.8.4/pyro/nn/module.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:10.037306 pyro-ppl-1.8.4/pyro/ops/
--rw-r--r--   0 fritzo     (501) staff       (20)        0 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/ops/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4306 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/ops/arrowhead.py
--rw-r--r--   0 fritzo     (501) staff       (20)    22551 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/ops/contract.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3402 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/ops/dual_averaging.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:10.038902 pyro-ppl-1.8.4/pyro/ops/einsum/
--rw-r--r--   0 fritzo     (501) staff       (20)     1486 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/ops/einsum/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4971 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/ops/einsum/adjoint.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2010 2022-10-02 18:17:50.000000 pyro-ppl-1.8.4/pyro/ops/einsum/torch_log.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1952 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/ops/einsum/torch_map.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2234 2022-07-05 20:35:43.000000 pyro-ppl-1.8.4/pyro/ops/einsum/torch_marginal.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2736 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/ops/einsum/torch_sample.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1901 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/ops/einsum/util.py
--rw-r--r--   0 fritzo     (501) staff       (20)    17941 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/ops/gamma_gaussian.py
--rw-r--r--   0 fritzo     (501) staff       (20)    28046 2022-10-30 17:11:32.000000 pyro-ppl-1.8.4/pyro/ops/gaussian.py
--rw-r--r--   0 fritzo     (501) staff       (20)      673 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/ops/hessian.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7458 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/ops/indexing.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5119 2023-01-03 21:44:32.000000 pyro-ppl-1.8.4/pyro/ops/integrator.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5970 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/ops/jit.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3577 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/ops/linalg.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9520 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/ops/newton.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6350 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/ops/packed.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5560 2022-06-12 12:50:39.000000 pyro-ppl-1.8.4/pyro/ops/provenance.py
--rw-r--r--   0 fritzo     (501) staff       (20)    11388 2022-07-05 20:10:55.000000 pyro-ppl-1.8.4/pyro/ops/rings.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7050 2022-05-12 17:23:25.000000 pyro-ppl-1.8.4/pyro/ops/special.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6648 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/ops/ssm_gp.py
--rw-r--r--   0 fritzo     (501) staff       (20)    17109 2022-07-10 14:38:43.000000 pyro-ppl-1.8.4/pyro/ops/stats.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8903 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/ops/streaming.py
--rw-r--r--   0 fritzo     (501) staff       (20)    15783 2022-11-06 16:58:27.000000 pyro-ppl-1.8.4/pyro/ops/tensor_utils.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3405 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/ops/welford.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:10.040290 pyro-ppl-1.8.4/pyro/optim/
--rw-r--r--   0 fritzo     (501) staff       (20)      594 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/optim/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3060 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/optim/adagrad_rmsprop.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3462 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/optim/clipped_adam.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7634 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/optim/dct_adam.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1906 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/optim/horovod.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2351 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/optim/lr_scheduler.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6391 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/optim/multi.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10320 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/optim/optim.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1767 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/optim/pytorch_optimizers.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:10.040516 pyro-ppl-1.8.4/pyro/params/
--rw-r--r--   0 fritzo     (501) staff       (20)      317 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/params/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)    13008 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/params/param_store.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:10.044055 pyro-ppl-1.8.4/pyro/poutine/
--rw-r--r--   0 fritzo     (501) staff       (20)      888 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/__init__.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4795 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/block_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3528 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/broadcast_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6129 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/collapse_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2128 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/condition_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3153 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/do_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     9673 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/enum_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1228 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/escape_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5275 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/guide.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8527 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/handlers.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3849 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/indep_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1744 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/infer_config_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4830 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/lift_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     3139 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/markov_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1239 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/mask_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     8691 2022-06-12 12:50:39.000000 pyro-ppl-1.8.4/pyro/poutine/messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2794 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/plate_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)      664 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/reentrant_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5393 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/reparam_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     2982 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/replay_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)    10404 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/runtime.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1824 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/scale_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     1047 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/seed_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     7654 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/subsample_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     6886 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/trace_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)    20794 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/trace_struct.py
--rw-r--r--   0 fritzo     (501) staff       (20)      821 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/poutine/uncondition_messenger.py
--rw-r--r--   0 fritzo     (501) staff       (20)     4073 2022-11-06 16:58:27.000000 pyro-ppl-1.8.4/pyro/poutine/util.py
--rw-r--r--   0 fritzo     (501) staff       (20)    23173 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/primitives.py
--rw-r--r--   0 fritzo     (501) staff       (20)     5019 2022-11-06 16:58:27.000000 pyro-ppl-1.8.4/pyro/settings.py
--rw-r--r--   0 fritzo     (501) staff       (20)    22051 2022-03-26 17:39:55.000000 pyro-ppl-1.8.4/pyro/util.py
-drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-01-03 22:30:10.044564 pyro-ppl-1.8.4/pyro_ppl.egg-info/
--rw-r--r--   0 fritzo     (501) staff       (20)     4742 2023-01-03 22:30:09.000000 pyro-ppl-1.8.4/pyro_ppl.egg-info/PKG-INFO
--rw-r--r--   0 fritzo     (501) staff       (20)    10556 2023-01-03 22:30:09.000000 pyro-ppl-1.8.4/pyro_ppl.egg-info/SOURCES.txt
--rw-r--r--   0 fritzo     (501) staff       (20)        1 2023-01-03 22:30:09.000000 pyro-ppl-1.8.4/pyro_ppl.egg-info/dependency_links.txt
--rw-r--r--   0 fritzo     (501) staff       (20)      871 2023-01-03 22:30:09.000000 pyro-ppl-1.8.4/pyro_ppl.egg-info/requires.txt
--rw-r--r--   0 fritzo     (501) staff       (20)        5 2023-01-03 22:30:09.000000 pyro-ppl-1.8.4/pyro_ppl.egg-info/top_level.txt
--rw-r--r--   0 fritzo     (501) staff       (20)     1986 2023-01-03 22:30:10.045135 pyro-ppl-1.8.4/setup.cfg
--rw-r--r--   0 fritzo     (501) staff       (20)     5054 2023-01-03 22:26:56.000000 pyro-ppl-1.8.4/setup.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.899750 pyro-ppl-1.8.5/
+-rw-r--r--   0 fritzo     (501) staff       (20)    11358 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/LICENSE.md
+-rw-r--r--   0 fritzo     (501) staff       (20)       60 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/MANIFEST.in
+-rw-r--r--   0 fritzo     (501) staff       (20)     4768 2023-05-29 03:00:47.899828 pyro-ppl-1.8.5/PKG-INFO
+-rw-r--r--   0 fritzo     (501) staff       (20)     4538 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/README.md
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.842709 pyro-ppl-1.8.5/pyro/
+-rw-r--r--   0 fritzo     (501) staff       (20)     1324 2023-05-29 01:08:09.000000 pyro-ppl-1.8.5/pyro/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      113 2023-05-29 03:00:47.000000 pyro-ppl-1.8.5/pyro/_version.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.843481 pyro-ppl-1.8.5/pyro/contrib/
+-rw-r--r--   0 fritzo     (501) staff       (20)      693 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      317 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/autoguide.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.844148 pyro-ppl-1.8.5/pyro/contrib/autoname/
+-rw-r--r--   0 fritzo     (501) staff       (20)      486 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/autoname/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5143 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/autoname/autoname.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8618 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/autoname/named.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6482 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/autoname/scoping.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.844514 pyro-ppl-1.8.5/pyro/contrib/bnn/
+-rw-r--r--   0 fritzo     (501) staff       (20)      177 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/bnn/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5383 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/bnn/hidden_layer.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      490 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/bnn/utils.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.844638 pyro-ppl-1.8.5/pyro/contrib/cevae/
+-rw-r--r--   0 fritzo     (501) staff       (20)    22960 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/cevae/__init__.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.844880 pyro-ppl-1.8.5/pyro/contrib/conjugate/
+-rw-r--r--   0 fritzo     (501) staff       (20)        0 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/conjugate/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     9073 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/conjugate/infer.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.845124 pyro-ppl-1.8.5/pyro/contrib/easyguide/
+-rw-r--r--   0 fritzo     (501) staff       (20)      206 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/easyguide/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    12912 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/contrib/easyguide/easyguide.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.846198 pyro-ppl-1.8.5/pyro/contrib/epidemiology/
+-rw-r--r--   0 fritzo     (501) staff       (20)      406 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/epidemiology/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    49835 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/epidemiology/compartmental.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    13549 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/epidemiology/distributions.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    51169 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/epidemiology/models.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    10990 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/epidemiology/util.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.847433 pyro-ppl-1.8.5/pyro/contrib/examples/
+-rw-r--r--   0 fritzo     (501) staff       (20)        0 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/examples/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6760 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/examples/bart.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      694 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/examples/finance.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2920 2023-05-28 13:37:12.000000 pyro-ppl-1.8.5/pyro/contrib/examples/multi_mnist.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1547 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/examples/nextstrain.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6875 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/examples/polyphonic_data_loader.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7442 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/examples/scanvi_data.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1556 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/examples/util.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.847960 pyro-ppl-1.8.5/pyro/contrib/forecast/
+-rw-r--r--   0 fritzo     (501) staff       (20)      360 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/forecast/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8823 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/forecast/evaluate.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    23299 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/forecast/forecaster.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    16054 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/forecast/util.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.848087 pyro-ppl-1.8.5/pyro/contrib/funsor/
+-rw-r--r--   0 fritzo     (501) staff       (20)     1263 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/__init__.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.849471 pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/
+-rw-r--r--   0 fritzo     (501) staff       (20)      912 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     9727 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/enum_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7623 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/named_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    15224 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/plate_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1076 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/primitives.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1804 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/replay_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8558 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/runtime.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3632 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/trace_messenger.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.850324 pyro-ppl-1.8.5/pyro/contrib/funsor/infer/
+-rw-r--r--   0 fritzo     (501) staff       (20)      514 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/infer/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2921 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/infer/discrete.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1652 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/infer/elbo.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1698 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/infer/trace_elbo.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    12663 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/infer/traceenum_elbo.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1882 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/funsor/infer/tracetmc_elbo.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.850792 pyro-ppl-1.8.5/pyro/contrib/gp/
+-rw-r--r--   0 fritzo     (501) staff       (20)      340 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/__init__.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.851792 pyro-ppl-1.8.5/pyro/contrib/gp/kernels/
+-rw-r--r--   0 fritzo     (501) staff       (20)     1533 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/kernels/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1577 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/kernels/brownian.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3699 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/kernels/coregionalize.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2646 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/kernels/dot_product.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5740 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/kernels/isotropic.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8446 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/kernels/kernel.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2424 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/kernels/periodic.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1536 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/kernels/static.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.852497 pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/
+-rw-r--r--   0 fritzo     (501) staff       (20)      897 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1988 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/binary.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1677 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/gaussian.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      875 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/likelihood.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2859 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/multi_class.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1884 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/poisson.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.853731 pyro-ppl-1.8.5/pyro/contrib/gp/models/
+-rw-r--r--   0 fritzo     (501) staff       (20)      546 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/models/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3897 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/models/gplvm.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8932 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/models/gpr.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     9145 2022-05-12 17:23:25.000000 pyro-ppl-1.8.5/pyro/contrib/gp/models/model.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    11001 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/gp/models/sgpr.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6859 2022-05-12 17:23:25.000000 pyro-ppl-1.8.5/pyro/contrib/gp/models/vgp.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8417 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/models/vsgp.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8058 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/parameterized.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7152 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/gp/util.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    15591 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/minipyro.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.854669 pyro-ppl-1.8.5/pyro/contrib/mue/
+-rw-r--r--   0 fritzo     (501) staff       (20)        0 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/mue/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6063 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/mue/dataloaders.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    13358 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/mue/missingdatahmm.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    34329 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/mue/models.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     9017 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/mue/statearrangers.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.855469 pyro-ppl-1.8.5/pyro/contrib/oed/
+-rw-r--r--   0 fritzo     (501) staff       (20)     3789 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/oed/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    44795 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/oed/eig.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.856010 pyro-ppl-1.8.5/pyro/contrib/oed/glmm/
+-rw-r--r--   0 fritzo     (501) staff       (20)     1551 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/oed/glmm/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    16376 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/oed/glmm/glmm.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    11368 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/oed/glmm/guides.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      867 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/oed/search.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1230 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/oed/util.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.858474 pyro-ppl-1.8.5/pyro/contrib/randomvariable/
+-rw-r--r--   0 fritzo     (501) staff       (20)      193 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/randomvariable/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5424 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/randomvariable/random_variable.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.859404 pyro-ppl-1.8.5/pyro/contrib/timeseries/
+-rw-r--r--   0 fritzo     (501) staff       (20)      711 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/timeseries/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2211 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/timeseries/base.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    23486 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/timeseries/gp.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6439 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/timeseries/lgssm.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    11250 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/timeseries/lgssmgp.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.860368 pyro-ppl-1.8.5/pyro/contrib/tracking/
+-rw-r--r--   0 fritzo     (501) staff       (20)      167 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/tracking/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    19243 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/tracking/assignment.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3576 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/tracking/distributions.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    16560 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/contrib/tracking/dynamic_models.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7796 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/tracking/extended_kalman_filter.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7266 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/tracking/hashing.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     4544 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/contrib/tracking/measurements.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2800 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/contrib/util.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.868761 pyro-ppl-1.8.5/pyro/distributions/
+-rw-r--r--   0 fritzo     (501) staff       (20)     5548 2023-01-03 22:31:38.000000 pyro-ppl-1.8.5/pyro/distributions/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3985 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/affine_beta.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7393 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/asymmetriclaplace.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     4062 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/avf_mvn.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    20914 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/coalescent.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     4815 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/distributions/conditional.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    10824 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/conjugate.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     4391 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/constraints.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3066 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/delta.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    10356 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/distributions/diag_normal_mixture.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     9012 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/distributions/diag_normal_mixture_shared_cov.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8443 2022-04-10 23:10:00.000000 pyro-ppl-1.8.5/pyro/distributions/distribution.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6765 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/empirical.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1885 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/extended.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1290 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/folded.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7983 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/gaussian_scale_mixture.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6571 2023-01-03 22:31:38.000000 pyro-ppl-1.8.5/pyro/distributions/grouped_normal_normal.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    54250 2023-01-13 02:07:01.000000 pyro-ppl-1.8.5/pyro/distributions/hmm.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2448 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/improper_uniform.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1429 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/inverse_gamma.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1661 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/kl.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2533 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/lkj.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5719 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/log_normal_negative_binomial.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5474 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/logistic.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6150 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/mixture.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5193 2022-06-12 12:50:39.000000 pyro-ppl-1.8.5/pyro/distributions/multivariate_studentt.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3381 2022-07-16 22:52:12.000000 pyro-ppl-1.8.5/pyro/distributions/nanmasked.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3176 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/omt_mvn.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6881 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/one_one_matching.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8360 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/one_two_matching.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2874 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/ordered_logistic.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3090 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/polya_gamma.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7441 2022-05-12 17:23:25.000000 pyro-ppl-1.8.5/pyro/distributions/projected_normal.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2933 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/rejector.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3637 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/relaxed_straight_through.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1125 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/score_parts.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    11563 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/distributions/sine_bivariate_von_mises.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7318 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/sine_skewed.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2471 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/softlaplace.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7746 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/spanning_tree.cpp
+-rw-r--r--   0 fritzo     (501) staff       (20)    22257 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/spanning_tree.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8208 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/stable.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.869999 pyro-ppl-1.8.5/pyro/distributions/testing/
+-rw-r--r--   0 fritzo     (501) staff       (20)      215 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/testing/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      421 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/testing/fakes.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    10761 2022-07-10 14:38:43.000000 pyro-ppl-1.8.5/pyro/distributions/testing/gof.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1598 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/testing/naive_dirichlet.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1167 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/testing/rejection_exponential.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8842 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/testing/rejection_gamma.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3610 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/testing/special.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    13608 2022-11-06 16:58:27.000000 pyro-ppl-1.8.5/pyro/distributions/torch.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    20332 2022-10-02 18:17:50.000000 pyro-ppl-1.8.5/pyro/distributions/torch_distribution.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3044 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/distributions/torch_patch.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1452 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/distributions/torch_transform.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.874166 pyro-ppl-1.8.5/pyro/distributions/transforms/
+-rw-r--r--   0 fritzo     (501) staff       (20)     6835 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    16342 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/affine_autoregressive.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    15805 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/affine_coupling.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2075 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/basic.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6147 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/batchnorm.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    11702 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/block_autoregressive.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2115 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/cholesky.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3383 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/discrete_cosine.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    11680 2022-11-22 19:06:49.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/generalized_channel_permute.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2883 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/haar.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    10536 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/householder.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2479 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/lower_cholesky_affine.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    13725 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/matrix_exponential.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     9794 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/neural_autoregressive.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1072 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/normalize.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      921 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/ordered.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5299 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/permute.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8881 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/planar.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7076 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/polynomial.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2138 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/power.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8711 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/radial.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1664 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/softplus.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    24458 2022-10-30 02:11:10.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/spline.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    11370 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/spline_autoregressive.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6917 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/spline_coupling.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6318 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/sylvester.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      809 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/unit_cholesky.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      282 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/transforms/utils.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1886 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/unit.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    11913 2022-11-06 16:58:27.000000 pyro-ppl-1.8.5/pyro/distributions/util.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2694 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/von_mises_3d.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6861 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/distributions/zero_inflated.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      266 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/generic.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.880293 pyro-ppl-1.8.5/pyro/infer/
+-rw-r--r--   0 fritzo     (501) staff       (20)     2041 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    15986 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/abstract_infer.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.881965 pyro-ppl-1.8.5/pyro/infer/autoguide/
+-rw-r--r--   0 fritzo     (501) staff       (20)     1618 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/autoguide/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    19662 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/autoguide/effect.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    26014 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/autoguide/gaussian.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    49080 2022-11-25 23:04:16.000000 pyro-ppl-1.8.5/pyro/infer/autoguide/guides.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8270 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/autoguide/initialization.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    16327 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/autoguide/structured.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3089 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/autoguide/utils.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7251 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/csis.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    11547 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/discrete.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     9535 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/infer/elbo.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    10044 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/energy_distance.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8063 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/enum.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     9701 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/importance.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    21777 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/infer/inspect.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.883482 pyro-ppl-1.8.5/pyro/infer/mcmc/
+-rw-r--r--   0 fritzo     (501) staff       (20)      412 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/mcmc/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    23000 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/mcmc/adaptation.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    29191 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/mcmc/api.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    18829 2023-01-03 22:31:38.000000 pyro-ppl-1.8.5/pyro/infer/mcmc/hmc.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     9270 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/mcmc/logger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2347 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/mcmc/mcmc_kernel.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    21893 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/mcmc/nuts.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    33005 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/infer/mcmc/util.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    11083 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/predictive.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     9418 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/renyi_elbo.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.885931 pyro-ppl-1.8.5/pyro/infer/reparam/
+-rw-r--r--   0 fritzo     (501) staff       (20)     1239 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     4315 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/conjugate.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2076 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/discrete_cosine.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1594 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/haar.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6406 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/hmm.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3812 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/loc_scale.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5549 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/neutra.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1697 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/projected_normal.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2627 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/reparam.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1869 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/softmax.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2642 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/split.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    10231 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/stable.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7481 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/strategies.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     4312 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/structured.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1477 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/studentt.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1789 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/transform.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3913 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/reparam/unit_jacobian.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5720 2022-10-02 18:17:50.000000 pyro-ppl-1.8.5/pyro/infer/resampler.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    11084 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/rws.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8713 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/smcfilter.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    12959 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/svgd.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5947 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/svi.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    10334 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/trace_elbo.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8173 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/trace_mean_field_elbo.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    10876 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/trace_mmd.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3367 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/trace_tail_adaptive_elbo.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    23531 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/traceenum_elbo.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    16979 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/infer/tracegraph_elbo.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8714 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/infer/tracetmc_elbo.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    12502 2022-11-06 16:58:27.000000 pyro-ppl-1.8.5/pyro/infer/util.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      463 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/logger.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.886610 pyro-ppl-1.8.5/pyro/nn/
+-rw-r--r--   0 fritzo     (501) staff       (20)      602 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/nn/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    13697 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/nn/auto_reg_nn.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5124 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/nn/dense_nn.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    31542 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/nn/module.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.890415 pyro-ppl-1.8.5/pyro/ops/
+-rw-r--r--   0 fritzo     (501) staff       (20)        0 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     4306 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/arrowhead.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    22550 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/ops/contract.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3402 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/dual_averaging.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.891519 pyro-ppl-1.8.5/pyro/ops/einsum/
+-rw-r--r--   0 fritzo     (501) staff       (20)     1486 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/einsum/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     4971 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/einsum/adjoint.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2010 2022-10-02 18:17:50.000000 pyro-ppl-1.8.5/pyro/ops/einsum/torch_log.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1952 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/einsum/torch_map.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2234 2022-07-05 20:35:43.000000 pyro-ppl-1.8.5/pyro/ops/einsum/torch_marginal.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2736 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/einsum/torch_sample.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1901 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/einsum/util.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    17941 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/gamma_gaussian.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    28046 2022-10-30 17:11:32.000000 pyro-ppl-1.8.5/pyro/ops/gaussian.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      673 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/hessian.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7458 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/indexing.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5119 2023-01-03 22:31:38.000000 pyro-ppl-1.8.5/pyro/ops/integrator.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5970 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/jit.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3577 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/linalg.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     9520 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/newton.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6350 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/packed.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5651 2023-05-28 15:09:30.000000 pyro-ppl-1.8.5/pyro/ops/provenance.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    11388 2022-07-05 20:10:55.000000 pyro-ppl-1.8.5/pyro/ops/rings.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7050 2022-05-12 17:23:25.000000 pyro-ppl-1.8.5/pyro/ops/special.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6648 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/ssm_gp.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    17109 2022-07-10 14:38:43.000000 pyro-ppl-1.8.5/pyro/ops/stats.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8903 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/streaming.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    15783 2022-11-06 16:58:27.000000 pyro-ppl-1.8.5/pyro/ops/tensor_utils.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3405 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/ops/welford.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.892830 pyro-ppl-1.8.5/pyro/optim/
+-rw-r--r--   0 fritzo     (501) staff       (20)      594 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/optim/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3060 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/optim/adagrad_rmsprop.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3462 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/optim/clipped_adam.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7634 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/optim/dct_adam.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1906 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/optim/horovod.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2351 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/optim/lr_scheduler.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6391 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/optim/multi.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    10610 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/optim/optim.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2064 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/optim/pytorch_optimizers.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.893127 pyro-ppl-1.8.5/pyro/params/
+-rw-r--r--   0 fritzo     (501) staff       (20)      317 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/params/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    13144 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/params/param_store.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.899104 pyro-ppl-1.8.5/pyro/poutine/
+-rw-r--r--   0 fritzo     (501) staff       (20)      922 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/poutine/__init__.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     4794 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/poutine/block_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3528 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/broadcast_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6129 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/collapse_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2128 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/condition_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3152 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/poutine/do_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     9671 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/poutine/enum_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1228 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/escape_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5427 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/poutine/guide.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8605 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/poutine/handlers.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3849 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/indep_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1744 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/infer_config_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     4830 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/lift_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     3139 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/markov_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1239 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/mask_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     8691 2022-06-12 12:50:39.000000 pyro-ppl-1.8.5/pyro/poutine/messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2794 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/plate_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      664 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/reentrant_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5393 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/reparam_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2982 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/replay_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    10402 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/poutine/runtime.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1824 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/scale_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     1047 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/seed_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     7725 2023-05-17 23:24:34.000000 pyro-ppl-1.8.5/pyro/poutine/subsample_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     2935 2023-05-12 13:41:44.000000 pyro-ppl-1.8.5/pyro/poutine/substitute_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     6886 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/trace_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    20794 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/trace_struct.py
+-rw-r--r--   0 fritzo     (501) staff       (20)      821 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/poutine/uncondition_messenger.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     4073 2022-11-06 16:58:27.000000 pyro-ppl-1.8.5/pyro/poutine/util.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    23173 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/primitives.py
+-rw-r--r--   0 fritzo     (501) staff       (20)     5019 2022-11-06 16:58:27.000000 pyro-ppl-1.8.5/pyro/settings.py
+-rw-r--r--   0 fritzo     (501) staff       (20)    22051 2022-03-26 17:39:55.000000 pyro-ppl-1.8.5/pyro/util.py
+drwxr-xr-x   0 fritzo     (501) staff       (20)        0 2023-05-29 03:00:47.899654 pyro-ppl-1.8.5/pyro_ppl.egg-info/
+-rw-r--r--   0 fritzo     (501) staff       (20)     4768 2023-05-29 03:00:47.000000 pyro-ppl-1.8.5/pyro_ppl.egg-info/PKG-INFO
+-rw-r--r--   0 fritzo     (501) staff       (20)    10593 2023-05-29 03:00:47.000000 pyro-ppl-1.8.5/pyro_ppl.egg-info/SOURCES.txt
+-rw-r--r--   0 fritzo     (501) staff       (20)        1 2023-05-29 03:00:47.000000 pyro-ppl-1.8.5/pyro_ppl.egg-info/dependency_links.txt
+-rw-r--r--   0 fritzo     (501) staff       (20)      901 2023-05-29 03:00:47.000000 pyro-ppl-1.8.5/pyro_ppl.egg-info/requires.txt
+-rw-r--r--   0 fritzo     (501) staff       (20)        5 2023-05-29 03:00:47.000000 pyro-ppl-1.8.5/pyro_ppl.egg-info/top_level.txt
+-rw-r--r--   0 fritzo     (501) staff       (20)     1986 2023-05-29 03:00:47.900225 pyro-ppl-1.8.5/setup.cfg
+-rw-r--r--   0 fritzo     (501) staff       (20)     5097 2023-05-28 13:37:12.000000 pyro-ppl-1.8.5/setup.py
```

### Comparing `pyro-ppl-1.8.4/LICENSE.md` & `pyro-ppl-1.8.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/PKG-INFO` & `pyro-ppl-1.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyro-ppl
-Version: 1.8.4
+Version: 1.8.5
 Summary: A Python library for probabilistic modeling and inference
 Home-page: http://pyro.ai
 Author: Uber AI Labs
 License: Apache 2.0
 Project-URL: Documentation, https://docs.pyro.ai
 Project-URL: Source, https://github.com/pyro-ppl/pyro
 Keywords: machine learning statistics probabilistic programming bayesian modeling pytorch
@@ -20,14 +20,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: extras
 Provides-Extra: test
 Provides-Extra: profile
 Provides-Extra: dev
 Provides-Extra: horovod
+Provides-Extra: lightning
 Provides-Extra: funsor
 License-File: LICENSE.md
 
 [Getting Started](http://pyro.ai/examples) |
 [Documentation](http://docs.pyro.ai/) |
 [Community](http://forum.pyro.ai/) |
 [Contributing](https://github.com/pyro-ppl/pyro/blob/master/CONTRIBUTING.md)
```

### Comparing `pyro-ppl-1.8.4/README.md` & `pyro-ppl-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/__init__.py` & `pyro-ppl-1.8.5/pyro/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,39 +24,37 @@
     validation_enabled,
 )
 from pyro.util import set_rng_seed
 
 from . import settings
 
 # After changing this, run scripts/update_version.py
-version_prefix = "1.8.4"
+version_prefix = "1.8.5"
 
 # Get the __version__ string from the auto-generated _version.py file, if exists.
 try:
     from pyro._version import __version__  # type: ignore
 except ImportError:
     __version__ = version_prefix
 
 __all__ = [
     "__version__",
     "barrier",
     "clear_param_store",
     "condition",
     "deterministic",
     "do",
-    "enable_module_local_param",
     "enable_validation",
     "factor",
     "get_param_store",
     "iarange",
     "irange",
     "log",
     "markov",
     "module",
-    "module_local_param_enabled",
     "param",
     "plate",
     "plate",
     "plate_stack",
     "poutine",
     "random_module",
     "render_model",
```

### Comparing `pyro-ppl-1.8.4/pyro/contrib/__init__.py` & `pyro-ppl-1.8.5/pyro/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/autoname/autoname.py` & `pyro-ppl-1.8.5/pyro/contrib/autoname/autoname.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/autoname/named.py` & `pyro-ppl-1.8.5/pyro/contrib/autoname/named.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/autoname/scoping.py` & `pyro-ppl-1.8.5/pyro/contrib/autoname/scoping.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/bnn/hidden_layer.py` & `pyro-ppl-1.8.5/pyro/contrib/bnn/hidden_layer.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/cevae/__init__.py` & `pyro-ppl-1.8.5/pyro/contrib/cevae/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/conjugate/infer.py` & `pyro-ppl-1.8.5/pyro/contrib/conjugate/infer.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/easyguide/easyguide.py` & `pyro-ppl-1.8.5/pyro/contrib/easyguide/easyguide.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,15 +226,15 @@
                 )
             site_batch_shape = torch.Size(site_batch_shape)
             self._site_batch_shapes[site["name"]] = site_batch_shape
             self._site_sizes[site["name"]] = site_batch_shape.numel() * site_event_numel
         self.event_shape = torch.Size([sum(self._site_sizes.values())])
 
     def __getstate__(self):
-        state = self.__dict__.copy()
+        state = getattr(super(), "__getstate__", self.__dict__.copy)()
         state["_guide"] = state["_guide"]()  # weakref -> ref
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
         self._guide = weakref.ref(self._guide)  # ref -> weakref
```

### Comparing `pyro-ppl-1.8.4/pyro/contrib/epidemiology/compartmental.py` & `pyro-ppl-1.8.5/pyro/contrib/epidemiology/compartmental.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/epidemiology/distributions.py` & `pyro-ppl-1.8.5/pyro/contrib/epidemiology/distributions.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/epidemiology/models.py` & `pyro-ppl-1.8.5/pyro/contrib/epidemiology/models.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/epidemiology/util.py` & `pyro-ppl-1.8.5/pyro/contrib/epidemiology/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/examples/bart.py` & `pyro-ppl-1.8.5/pyro/contrib/examples/bart.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/examples/finance.py` & `pyro-ppl-1.8.5/pyro/contrib/examples/finance.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/examples/multi_mnist.py` & `pyro-ppl-1.8.5/pyro/contrib/examples/multi_mnist.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     x = []
     y = []
     for _ in range(n):
         num_digits = np.random.randint(max_digits + 1)
         canvas, labels = sample_multi(num_digits, canvas_size, mnist)
         x.append(canvas)
         y.append(labels)
-    return np.array(x, dtype=np.uint8), y
+    return np.array(x, dtype=np.uint8), np.array(y, dtype=object)
 
 
 def load_mnist(root_path):
     loader = get_data_loader("MNIST", root_path)
     return {
         "digits": loader.dataset.data.cpu().numpy(),
         "labels": loader.dataset.targets,
```

### Comparing `pyro-ppl-1.8.4/pyro/contrib/examples/nextstrain.py` & `pyro-ppl-1.8.5/pyro/contrib/examples/nextstrain.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/examples/polyphonic_data_loader.py` & `pyro-ppl-1.8.5/pyro/contrib/examples/polyphonic_data_loader.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/examples/scanvi_data.py` & `pyro-ppl-1.8.5/pyro/contrib/examples/scanvi_data.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/examples/util.py` & `pyro-ppl-1.8.5/pyro/contrib/examples/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/forecast/evaluate.py` & `pyro-ppl-1.8.5/pyro/contrib/forecast/evaluate.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/forecast/forecaster.py` & `pyro-ppl-1.8.5/pyro/contrib/forecast/forecaster.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/forecast/util.py` & `pyro-ppl-1.8.5/pyro/contrib/forecast/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/funsor/__init__.py` & `pyro-ppl-1.8.5/pyro/contrib/funsor/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/funsor/handlers/__init__.py` & `pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/funsor/handlers/enum_messenger.py` & `pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/enum_messenger.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -230,18 +230,18 @@
     :param extend_fn: function (possibly stochastic) that takes a partial trace and a site,
         and returns a list of extended traces
     :param escape_fn: function (possibly stochastic) that takes a partial trace and a site,
         and returns a boolean value to decide whether to exit
     :param num_samples: optional number of extended traces for extend_fn to return
     :returns: stochastic function decorated with poutine logic
     """
+
     # TODO rewrite this to use purpose-built trace/replay handlers
     def wrapper(wrapped):
         def _fn(*args, **kwargs):
-
             for i in range(max_tries):
                 assert (
                     not queue.empty()
                 ), "trying to get() from an empty queue will deadlock"
 
                 next_trace = queue.get()
                 try:
```

### Comparing `pyro-ppl-1.8.4/pyro/contrib/funsor/handlers/named_messenger.py` & `pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/named_messenger.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,14 @@
                 self._saved_dims |= set(_DIM_STACK.global_frame.name_to_dim.items())
             for name, dim in self._saved_dims:
                 del _DIM_STACK.global_frame[name]
         return super().__exit__(*args, **kwargs)
 
     @staticmethod  # only depends on the global _DIM_STACK state, not self
     def _pyro_to_data(msg):
-
         (funsor_value,) = msg["args"]
         name_to_dim = msg["kwargs"].setdefault("name_to_dim", OrderedDict())
         dim_type = msg["kwargs"].setdefault("dim_type", DimType.LOCAL)
 
         batch_names = tuple(funsor_value.inputs.keys())
 
         # interpret all names/dims as requests since we only run this function once
@@ -78,15 +77,14 @@
         # name_to_dim.update(_DIM_STACK.allocate_name_to_dim(name_to_dim_request))
         name_to_dim.update(_DIM_STACK.allocate(name_to_dim_request))
 
         msg["stop"] = True  # only need to run this once per to_data call
 
     @staticmethod  # only depends on the global _DIM_STACK state, not self
     def _pyro_to_funsor(msg):
-
         if len(msg["args"]) == 2:
             raw_value, output = msg["args"]
         else:
             raw_value = msg["args"][0]
             output = msg["kwargs"].setdefault("output", None)
         dim_to_name = msg["kwargs"].setdefault("dim_to_name", OrderedDict())
         dim_type = msg["kwargs"].setdefault("dim_type", DimType.LOCAL)
```

### Comparing `pyro-ppl-1.8.4/pyro/contrib/funsor/handlers/plate_messenger.py` & `pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/plate_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/funsor/handlers/primitives.py` & `pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/primitives.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/funsor/handlers/replay_messenger.py` & `pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/replay_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/funsor/handlers/runtime.py` & `pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,14 @@
 
             return name, fresh_dim
         raise ValueError(
             "{} and {} not a valid name-dim pair".format(key, value_request)
         )
 
     def allocate(self, key_to_value_request):
-
         # step 1: split into fresh and non-fresh
         key_to_value = OrderedDict()
         for key, value_request in tuple(key_to_value_request.items()):
             value = value_request.value
             for frame in self.current_read_env:
                 if value is None and key in frame:
                     key_to_value[key] = frame[key]
```

### Comparing `pyro-ppl-1.8.4/pyro/contrib/funsor/handlers/trace_messenger.py` & `pyro-ppl-1.8.5/pyro/contrib/funsor/handlers/trace_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/funsor/infer/__init__.py` & `pyro-ppl-1.8.5/pyro/contrib/funsor/infer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/funsor/infer/discrete.py` & `pyro-ppl-1.8.5/pyro/contrib/funsor/infer/discrete.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from pyro.contrib.funsor.handlers.enum_messenger import _get_support_value
 from pyro.contrib.funsor.infer.traceenum_elbo import terms_from_trace
 from pyro.poutine import Trace, block
 from pyro.poutine.util import site_is_subsample
 
 
 def _sample_posterior(model, first_available_dim, temperature, *args, **kwargs):
-
     if temperature == 0:
         sum_op, prod_op = funsor.ops.max, funsor.ops.add
         approx = funsor.approximations.argmax_approximate
     elif temperature == 1:
         sum_op, prod_op = funsor.ops.logaddexp, funsor.ops.add
         approx = funsor.montecarlo.MonteCarlo()
     else:
```

### Comparing `pyro-ppl-1.8.4/pyro/contrib/funsor/infer/elbo.py` & `pyro-ppl-1.8.5/pyro/contrib/funsor/infer/elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/funsor/infer/trace_elbo.py` & `pyro-ppl-1.8.5/pyro/contrib/funsor/infer/trace_elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/funsor/infer/traceenum_elbo.py` & `pyro-ppl-1.8.5/pyro/contrib/funsor/infer/traceenum_elbo.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,14 @@
     )
     return terms
 
 
 @copy_docs_from(_OrigTraceEnum_ELBO)
 class TraceMarkovEnum_ELBO(ELBO):
     def differentiable_loss(self, model, guide, *args, **kwargs):
-
         # get batched, enumerated, to_funsor-ed traces from the guide and model
         with plate(
             size=self.num_particles
         ) if self.num_particles > 1 else contextlib.ExitStack(), enum(
             first_available_dim=(-self.max_plate_nesting - 1)
             if self.max_plate_nesting
             else None
@@ -166,15 +165,14 @@
         with funsor.interpretations.memoize():
             return -to_data(apply_optimizer(elbo))
 
 
 @copy_docs_from(_OrigTraceEnum_ELBO)
 class TraceEnum_ELBO(ELBO):
     def differentiable_loss(self, model, guide, *args, **kwargs):
-
         # get batched, enumerated, to_funsor-ed traces from the guide and model
         with plate(
             size=self.num_particles
         ) if self.num_particles > 1 else contextlib.ExitStack(), enum(
             first_available_dim=(-self.max_plate_nesting - 1)
             if self.max_plate_nesting
             else None
```

### Comparing `pyro-ppl-1.8.4/pyro/contrib/funsor/infer/tracetmc_elbo.py` & `pyro-ppl-1.8.5/pyro/contrib/funsor/infer/tracetmc_elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/gp/kernels/__init__.py` & `pyro-ppl-1.8.5/pyro/contrib/gp/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/gp/kernels/brownian.py` & `pyro-ppl-1.8.5/pyro/contrib/gp/kernels/brownian.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/gp/kernels/coregionalize.py` & `pyro-ppl-1.8.5/pyro/contrib/gp/kernels/coregionalize.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/gp/kernels/dot_product.py` & `pyro-ppl-1.8.5/pyro/contrib/gp/kernels/dot_product.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/gp/kernels/isotropic.py` & `pyro-ppl-1.8.5/pyro/contrib/gp/kernels/isotropic.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/gp/kernels/kernel.py` & `pyro-ppl-1.8.5/pyro/contrib/gp/kernels/kernel.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/gp/kernels/periodic.py` & `pyro-ppl-1.8.5/pyro/contrib/gp/kernels/periodic.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/gp/kernels/static.py` & `pyro-ppl-1.8.5/pyro/contrib/gp/kernels/static.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/gp/likelihoods/__init__.py` & `pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/gp/likelihoods/binary.py` & `pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/binary.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/gp/likelihoods/gaussian.py` & `pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/gaussian.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/gp/likelihoods/likelihood.py` & `pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/likelihood.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/gp/likelihoods/multi_class.py` & `pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/multi_class.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/gp/likelihoods/poisson.py` & `pyro-ppl-1.8.5/pyro/contrib/gp/likelihoods/poisson.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/gp/models/__init__.py` & `pyro-ppl-1.8.5/pyro/contrib/gp/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/gp/models/gplvm.py` & `pyro-ppl-1.8.5/pyro/contrib/gp/models/gplvm.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/gp/models/gpr.py` & `pyro-ppl-1.8.5/pyro/contrib/gp/models/gpr.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/gp/models/model.py` & `pyro-ppl-1.8.5/pyro/contrib/gp/models/model.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/gp/models/sgpr.py` & `pyro-ppl-1.8.5/pyro/contrib/gp/models/sgpr.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,14 @@
         a covariance matrix to help stablize its Cholesky decomposition.
     :param str name: Name of this model.
     """
 
     def __init__(
         self, X, y, kernel, Xu, noise=None, mean_function=None, approx=None, jitter=1e-6
     ):
-
         assert isinstance(
             X, torch.Tensor
         ), "X needs to be a torch Tensor instead of a {}".format(type(X))
         if y is not None:
             assert isinstance(
                 y, torch.Tensor
             ), "y needs to be a torch Tensor instead of a {}".format(type(y))
```

### Comparing `pyro-ppl-1.8.4/pyro/contrib/gp/models/vgp.py` & `pyro-ppl-1.8.5/pyro/contrib/gp/models/vgp.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/gp/models/vsgp.py` & `pyro-ppl-1.8.5/pyro/contrib/gp/models/vsgp.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/gp/parameterized.py` & `pyro-ppl-1.8.5/pyro/contrib/gp/parameterized.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/gp/util.py` & `pyro-ppl-1.8.5/pyro/contrib/gp/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/minipyro.py` & `pyro-ppl-1.8.5/pyro/contrib/minipyro.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/mue/dataloaders.py` & `pyro-ppl-1.8.5/pyro/contrib/mue/dataloaders.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
         source,
         source_type="list",
         alphabet="amino-acid",
         max_length=None,
         include_stop=False,
         device=None,
     ):
-
         super().__init__()
 
         # Determine device
         if device is None:
             device = torch.tensor(0.0).device
         self.device = device
 
@@ -131,19 +130,17 @@
         x = torch.cat(
             [oh, torch.zeros([length - len(seq), len(alphabet)], device=self.device)]
         )
 
         return x
 
     def __len__(self):
-
         return self.data_size
 
     def __getitem__(self, ind):
-
         return (self.seq_data[ind], self.L_data[ind])
 
 
 def write(x, alphabet, file, truncate_stop=False, append=False, scores=None):
     """
     Write sequence samples to file.
```

### Comparing `pyro-ppl-1.8.4/pyro/contrib/mue/missingdatahmm.py` & `pyro-ppl-1.8.5/pyro/contrib/mue/missingdatahmm.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/mue/models.py` & `pyro-ppl-1.8.5/pyro/contrib/mue/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,14 @@
         assert isinstance(indel_prior_bias, float)
         self.indel_prior = torch.tensor([indel_prior_bias, 0.0])
 
         # Initialize state arranger.
         self.statearrange = Profile(latent_seq_length)
 
     def model(self, seq_data, local_scale):
-
         # Latent sequence.
         precursor_seq = pyro.sample(
             "precursor_seq",
             dist.Normal(
                 torch.zeros(self.precursor_seq_shape),
                 self.prior_scale * torch.ones(self.precursor_seq_shape),
             ).to_event(2),
@@ -312,15 +311,14 @@
         super().__init__()
 
         self.input_size = data_length * alphabet_length
         self.f1_mn = nn.Linear(self.input_size, z_dim)
         self.f1_sd = nn.Linear(self.input_size, z_dim)
 
     def forward(self, data):
-
         data = data.reshape(-1, self.input_size)
         z_loc = self.f1_mn(data)
         z_scale = softplus(self.f1_sd(data))
 
         return z_loc, z_scale
 
 
@@ -448,15 +446,14 @@
         self.batch_size = batch_size
 
         # Initialize layers.
         self.encoder = Encoder(data_length, alphabet_length, z_dim)
         self.statearrange = Profile(latent_seq_length)
 
     def decoder(self, z, W, B, inverse_temp):
-
         # Project.
         v = torch.mm(z, W) + B
 
         out = dict()
         if self.indel_factor_dependence:
             # Extract insertion and deletion parameters.
             ind0 = (2 * self.latent_seq_length + 1) * self.latent_alphabet_length
@@ -485,15 +482,14 @@
             [-1, self.latent_seq_length + 1, self.latent_alphabet_length]
         )
         out["insert_seq_logits"] = insert_seq_v - insert_seq_v.logsumexp(-1, True)
 
         return out
 
     def model(self, seq_data, local_scale, local_prior_scale):
-
         # ARD prior.
         if self.ARD_prior:
             # Relevance factors
             alpha = pyro.sample(
                 "alpha",
                 dist.Gamma(torch.ones(self.z_dim), torch.ones(self.z_dim)).to_event(1),
             )
```

### Comparing `pyro-ppl-1.8.4/pyro/contrib/mue/statearrangers.py` & `pyro-ppl-1.8.5/pyro/contrib/mue/statearrangers.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/oed/__init__.py` & `pyro-ppl-1.8.5/pyro/contrib/oed/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/oed/eig.py` & `pyro-ppl-1.8.5/pyro/contrib/oed/eig.py`

 * *Files 0% similar despite different names*

```diff
@@ -533,15 +533,14 @@
     optim,
     return_history=False,
     final_design=None,
     final_num_samples=None,
     *args,
     **kwargs
 ):
-
     loss = _posterior_loss(
         model, guide, observation_labels, target_labels, *args, **kwargs
     )
     return opt_eig_ape_loss(
         design,
         loss,
         num_samples,
@@ -830,15 +829,14 @@
     num_samples,
     num_steps,
     optim,
     return_history=False,
     final_design=None,
     final_num_samples=None,
 ):
-
     if final_design is None:
         final_design = design
     if final_num_samples is None:
         final_num_samples = num_samples
 
     params = None
     history = []
@@ -885,15 +883,14 @@
 
 def _donsker_varadhan_loss(model, T, observation_labels, target_labels):
     """DV loss: to evaluate directly use `donsker_varadhan_eig` setting `num_steps=0`."""
 
     ewma_log = EwmaLog(alpha=0.90)
 
     def loss_fn(design, num_particles, **kwargs):
-
         try:
             pyro.module("T", T)
         except AssertionError:
             pass
 
         expanded_design = lexpand(design, num_particles)
 
@@ -929,15 +926,14 @@
 
 def _posterior_loss(
     model, guide, observation_labels, target_labels, analytic_entropy=False
 ):
     """Posterior loss: to evaluate directly use `posterior_eig` setting `num_steps=0`, `eig=False`."""
 
     def loss_fn(design, num_particles, evaluation=False, **kwargs):
-
         expanded_design = lexpand(design, num_particles)
 
         # Sample from p(y, theta | d)
         trace = poutine.trace(model).get_trace(expanded_design)
         y_dict = {l: trace.nodes[l]["value"] for l in observation_labels}
         theta_dict = {l: trace.nodes[l]["value"] for l in target_labels}
 
@@ -966,15 +962,14 @@
     return loss_fn
 
 
 def _marginal_loss(model, guide, observation_labels, target_labels):
     """Marginal loss: to evaluate directly use `marginal_eig` setting `num_steps=0`."""
 
     def loss_fn(design, num_particles, evaluation=False, **kwargs):
-
         expanded_design = lexpand(design, num_particles)
 
         # Sample from p(y | d)
         trace = poutine.trace(model).get_trace(expanded_design)
         y_dict = {l: trace.nodes[l]["value"] for l in observation_labels}
 
         # Run through q(y | d)
@@ -998,15 +993,14 @@
 
 def _marginal_likelihood_loss(
     model, marginal_guide, likelihood_guide, observation_labels, target_labels
 ):
     """Marginal_likelihood loss: to evaluate directly use `marginal_likelihood_eig` setting `num_steps=0`."""
 
     def loss_fn(design, num_particles, evaluation=False, **kwargs):
-
         expanded_design = lexpand(design, num_particles)
 
         # Sample from p(y | d)
         trace = poutine.trace(model).get_trace(expanded_design)
         y_dict = {l: trace.nodes[l]["value"] for l in observation_labels}
         theta_dict = {l: trace.nodes[l]["value"] for l in target_labels}
 
@@ -1039,15 +1033,14 @@
 
 def _lfire_loss(
     model_marginal, model_conditional, h, observation_labels, target_labels
 ):
     """LFIRE loss: to evaluate directly use `lfire_eig` setting `num_steps=0`."""
 
     def loss_fn(design, num_particles, evaluation=False, **kwargs):
-
         try:
             pyro.module("h", h)
         except AssertionError:
             pass
 
         expanded_design = lexpand(design, num_particles)
         model_conditional_trace = poutine.trace(model_conditional).get_trace(
```

### Comparing `pyro-ppl-1.8.4/pyro/contrib/oed/glmm/__init__.py` & `pyro-ppl-1.8.5/pyro/contrib/oed/glmm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/oed/glmm/glmm.py` & `pyro-ppl-1.8.5/pyro/contrib/oed/glmm/glmm.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 # TODO read from torch float spec
 epsilon = torch.tensor(2**-24)
 
 
 def known_covariance_linear_model(
     coef_means, coef_sds, observation_sd, coef_labels="w", observation_label="y"
 ):
-
     if not isinstance(coef_means, list):
         coef_means = [coef_means]
     if not isinstance(coef_sds, list):
         coef_sds = [coef_sds]
     if not isinstance(coef_labels, list):
         coef_labels = [coef_labels]
```

### Comparing `pyro-ppl-1.8.4/pyro/contrib/oed/glmm/guides.py` & `pyro-ppl-1.8.5/pyro/contrib/oed/glmm/guides.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,30 +65,27 @@
             }
         )
         self.w_sizes = w_sizes
         self.use_softplus = use_softplus
         self.softplus = nn.Softplus()
 
     def get_params(self, y_dict, design, target_labels):
-
         y = torch.cat(list(y_dict.values()), dim=-1)
         return self.linear_model_formula(y, design, target_labels)
 
     def linear_model_formula(self, y, design, target_labels):
-
         if self.use_softplus:
             mu = {l: rmv(self.softplus(self.regressor[l]), y) for l in target_labels}
         else:
             mu = {l: rmv(self.regressor[l], y) for l in target_labels}
         scale_tril = {l: rtril(self.scale_tril[l]) for l in target_labels}
 
         return mu, scale_tril
 
     def forward(self, y_dict, design, observation_labels, target_labels):
-
         pyro.module("posterior_guide", self)
 
         # Returns two dicts from labels -> tensors
         mu, scale_tril = self.get_params(y_dict, design, target_labels)
 
         for l in target_labels:
             w_dist = dist.MultivariateNormal(mu[l], scale_tril=scale_tril[l])
@@ -218,15 +215,14 @@
     def __init__(self, d, n, w_sizes, **kwargs):
         super().__init__(d, w_sizes, **kwargs)
         self.inverse_sigmoid_scale = nn.Parameter(torch.ones(n))
         self.h1_weight = nn.Parameter(torch.ones(n))
         self.h1_bias = nn.Parameter(torch.zeros(n))
 
     def get_params(self, y_dict, design, target_labels):
-
         y = torch.cat(list(y_dict.values()), dim=-1)
 
         # Approx invert transformation on y in expectation
         y, y1m = y.clamp(1e-35, 1), (1.0 - y).clamp(1e-35, 1)
         logited = y.log() - y1m.log()
         y_trans = logited / 0.1
         y_trans = y_trans * self.inverse_sigmoid_scale
@@ -250,15 +246,14 @@
         super().__init__(d, w_sizes, **kwargs)
         self.alpha = nn.Parameter(alpha_init * torch.ones(d))
         self.b0 = nn.Parameter(b0_init * torch.ones(d))
         self.mf = mf
         self.tau_label = tau_label
 
     def get_params(self, y_dict, design, target_labels):
-
         y = torch.cat(list(y_dict.values()), dim=-1)
 
         coefficient_labels = [
             label for label in target_labels if label != self.tau_label
         ]
         mu, scale_tril = self.linear_model_formula(y, design, coefficient_labels)
         mu_vec = torch.cat(list(mu.values()), dim=-1)
@@ -266,15 +261,14 @@
         yty = rvv(y, y)
         ytxmu = rvv(y, rmv(design, mu_vec))
         beta = self.b0 + 0.5 * (yty - ytxmu)
 
         return mu, scale_tril, self.alpha, beta
 
     def forward(self, y_dict, design, observation_labels, target_labels):
-
         pyro.module("ba_guide", self)
 
         mu, scale_tril, alpha, beta = self.get_params(y_dict, design, target_labels)
 
         if self.tau_label in target_labels:
             tau_dist = dist.Gamma(alpha, beta)
             tau = pyro.sample(self.tau_label, tau_dist)
@@ -299,15 +293,14 @@
     """
 
     def __init__(self, guide):
         super().__init__()
         self.guide = guide
 
     def forward(self, design, trace, observation_labels, target_labels):
-
         trace.compute_log_prob()
         prior_lp = sum(trace.nodes[l]["log_prob"] for l in target_labels)
         y_dict = {l: trace.nodes[l]["value"] for l in observation_labels}
         theta_dict = {l: trace.nodes[l]["value"] for l in target_labels}
 
         conditional_guide = pyro.condition(self.guide, data=theta_dict)
         cond_trace = poutine.trace(conditional_guide).get_trace(
```

### Comparing `pyro-ppl-1.8.4/pyro/contrib/oed/search.py` & `pyro-ppl-1.8.5/pyro/contrib/oed/search.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/oed/util.py` & `pyro-ppl-1.8.5/pyro/contrib/oed/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/randomvariable/random_variable.py` & `pyro-ppl-1.8.5/pyro/contrib/randomvariable/random_variable.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/timeseries/__init__.py` & `pyro-ppl-1.8.5/pyro/contrib/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/timeseries/base.py` & `pyro-ppl-1.8.5/pyro/contrib/timeseries/base.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/timeseries/gp.py` & `pyro-ppl-1.8.5/pyro/contrib/timeseries/gp.py`

 * *Files 0% similar despite different names*

```diff
@@ -381,15 +381,14 @@
         nu=1.5,
         dt=1.0,
         obs_dim=1,
         linearly_coupled=False,
         length_scale_init=None,
         obs_noise_scale_init=None,
     ):
-
         if nu != 1.5:
             raise NotImplementedError("The only supported value of nu is 1.5")
 
         self.dt = dt
         self.obs_dim = obs_dim
 
         if obs_noise_scale_init is None:
```

### Comparing `pyro-ppl-1.8.4/pyro/contrib/timeseries/lgssm.py` & `pyro-ppl-1.8.5/pyro/contrib/timeseries/lgssm.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/timeseries/lgssmgp.py` & `pyro-ppl-1.8.5/pyro/contrib/timeseries/lgssmgp.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/tracking/assignment.py` & `pyro-ppl-1.8.5/pyro/contrib/tracking/assignment.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/tracking/distributions.py` & `pyro-ppl-1.8.5/pyro/contrib/tracking/distributions.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/tracking/dynamic_models.py` & `pyro-ppl-1.8.5/pyro/contrib/tracking/dynamic_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,15 +373,14 @@
 
         :param dt: time interval to integrate over.
 
         :return: Read-only covariance (Q) of the native state ``x`` resulting from
             stochastic integration (for use with EKF).
         """
         if dt not in self._Q_cache:
-
             with torch.no_grad():
                 d = self._dimension
                 dt2 = dt * dt
                 dt3 = dt2 * dt
                 Q = torch.zeros(d, d, dtype=self.sa2.dtype, device=self.sa2.device)
                 eye = eye_like(self.sa2, d // 2)
                 Q[: d // 2, : d // 2] = dt3 * eye / 3.0
```

### Comparing `pyro-ppl-1.8.4/pyro/contrib/tracking/extended_kalman_filter.py` & `pyro-ppl-1.8.5/pyro/contrib/tracking/extended_kalman_filter.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/tracking/hashing.py` & `pyro-ppl-1.8.5/pyro/contrib/tracking/hashing.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/tracking/measurements.py` & `pyro-ppl-1.8.5/pyro/contrib/tracking/measurements.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/contrib/util.py` & `pyro-ppl-1.8.5/pyro/contrib/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
+import weakref
 from collections import OrderedDict
 
 import torch
 
 import pyro
 
 
@@ -71,7 +72,26 @@
     return M * torch.tril(torch.ones(M.shape[-2], M.shape[-1]), diagonal=diagonal)
 
 
 def iter_plates_to_shape(shape):
     # Go backwards (right to left)
     for i, s in enumerate(shape[::-1]):
         yield pyro.plate("plate_" + str(i), s)
+
+
+def check_no_weakref(obj, path="", avoid_ids=None):
+    """Attempts to check that an object has no weakrefs."""
+    if avoid_ids is None:
+        avoid_ids = {id(obj)}
+
+    if isinstance(obj, weakref.ref):
+        raise ValueError(f"Weakref found at {path}")
+    elif isinstance(obj, dict):
+        for k, v in obj.items():
+            if id(v) not in avoid_ids:
+                check_no_weakref(v, path + f"[{k}]")
+    elif isinstance(obj, (list, tuple)):
+        for i, v in enumerate(obj):
+            if id(v) not in avoid_ids:
+                check_no_weakref(v, path + f"[{i}]")
+    elif hasattr(obj, "__dict__"):
+        check_no_weakref(obj.__dict__, path)
```

### Comparing `pyro-ppl-1.8.4/pyro/distributions/__init__.py` & `pyro-ppl-1.8.5/pyro/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/affine_beta.py` & `pyro-ppl-1.8.5/pyro/distributions/affine_beta.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/asymmetriclaplace.py` & `pyro-ppl-1.8.5/pyro/distributions/asymmetriclaplace.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/avf_mvn.py` & `pyro-ppl-1.8.5/pyro/distributions/avf_mvn.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/coalescent.py` & `pyro-ppl-1.8.5/pyro/distributions/coalescent.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/conjugate.py` & `pyro-ppl-1.8.5/pyro/distributions/conjugate.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/constraints.py` & `pyro-ppl-1.8.5/pyro/distributions/constraints.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/delta.py` & `pyro-ppl-1.8.5/pyro/distributions/delta.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/diag_normal_mixture.py` & `pyro-ppl-1.8.5/pyro/distributions/diag_normal_mixture.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,14 @@
         z = loc + sigma * white
         ctx.save_for_backward(z, scales, locs, component_logits, pis)
         return z
 
     @staticmethod
     @once_differentiable
     def backward(ctx, grad_output):
-
         z, scales, locs, logits, pis = ctx.saved_tensors
         dim = scales.size(-1)
         K = logits.size(-1)
         g = grad_output  # l b i
         g = g.unsqueeze(-2)  # l b 1 i
         batch_dims = locs.dim() - 2
```

### Comparing `pyro-ppl-1.8.4/pyro/distributions/diag_normal_mixture_shared_cov.py` & `pyro-ppl-1.8.5/pyro/distributions/diag_normal_mixture_shared_cov.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,14 @@
         z = loc + coord_scale * white
         ctx.save_for_backward(z, coord_scale, locs, component_logits, pis)
         return z
 
     @staticmethod
     @once_differentiable
     def backward(ctx, grad_output):
-
         z, coord_scale, locs, component_logits, pis = ctx.saved_tensors
         K = component_logits.size(-1)
         batch_dims = coord_scale.dim() - 1
         g = grad_output  # l b i
 
         z_tilde = z / coord_scale  # l b i
         locs_tilde = locs / coord_scale.unsqueeze(-2)  # b j i
```

### Comparing `pyro-ppl-1.8.4/pyro/distributions/distribution.py` & `pyro-ppl-1.8.5/pyro/distributions/distribution.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/empirical.py` & `pyro-ppl-1.8.5/pyro/distributions/empirical.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/extended.py` & `pyro-ppl-1.8.5/pyro/distributions/extended.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/folded.py` & `pyro-ppl-1.8.5/pyro/distributions/folded.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/gaussian_scale_mixture.py` & `pyro-ppl-1.8.5/pyro/distributions/gaussian_scale_mixture.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/grouped_normal_normal.py` & `pyro-ppl-1.8.5/pyro/distributions/grouped_normal_normal.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/hmm.py` & `pyro-ppl-1.8.5/pyro/distributions/hmm.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/improper_uniform.py` & `pyro-ppl-1.8.5/pyro/distributions/improper_uniform.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/inverse_gamma.py` & `pyro-ppl-1.8.5/pyro/distributions/inverse_gamma.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/kl.py` & `pyro-ppl-1.8.5/pyro/distributions/kl.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/lkj.py` & `pyro-ppl-1.8.5/pyro/distributions/lkj.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/log_normal_negative_binomial.py` & `pyro-ppl-1.8.5/pyro/distributions/log_normal_negative_binomial.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/logistic.py` & `pyro-ppl-1.8.5/pyro/distributions/logistic.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/mixture.py` & `pyro-ppl-1.8.5/pyro/distributions/mixture.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/multivariate_studentt.py` & `pyro-ppl-1.8.5/pyro/distributions/multivariate_studentt.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/nanmasked.py` & `pyro-ppl-1.8.5/pyro/distributions/nanmasked.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/omt_mvn.py` & `pyro-ppl-1.8.5/pyro/distributions/omt_mvn.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/one_one_matching.py` & `pyro-ppl-1.8.5/pyro/distributions/one_one_matching.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/one_two_matching.py` & `pyro-ppl-1.8.5/pyro/distributions/one_two_matching.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/ordered_logistic.py` & `pyro-ppl-1.8.5/pyro/distributions/ordered_logistic.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/polya_gamma.py` & `pyro-ppl-1.8.5/pyro/distributions/polya_gamma.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/projected_normal.py` & `pyro-ppl-1.8.5/pyro/distributions/projected_normal.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/rejector.py` & `pyro-ppl-1.8.5/pyro/distributions/rejector.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/relaxed_straight_through.py` & `pyro-ppl-1.8.5/pyro/distributions/relaxed_straight_through.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/score_parts.py` & `pyro-ppl-1.8.5/pyro/distributions/score_parts.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/sine_bivariate_von_mises.py` & `pyro-ppl-1.8.5/pyro/distributions/sine_bivariate_von_mises.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,14 @@
         psi_loc,
         phi_concentration,
         psi_concentration,
         correlation=None,
         weighted_correlation=None,
         validate_args=None,
     ):
-
         assert (correlation is None) != (weighted_correlation is None)
 
         if weighted_correlation is not None:
             sqrt_ = (
                 torch.sqrt if isinstance(phi_concentration, torch.Tensor) else math.sqrt
             )
             correlation = weighted_correlation * sqrt_(
```

### Comparing `pyro-ppl-1.8.4/pyro/distributions/sine_skewed.py` & `pyro-ppl-1.8.5/pyro/distributions/sine_skewed.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/softlaplace.py` & `pyro-ppl-1.8.5/pyro/distributions/softlaplace.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/spanning_tree.cpp` & `pyro-ppl-1.8.5/pyro/distributions/spanning_tree.cpp`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/spanning_tree.py` & `pyro-ppl-1.8.5/pyro/distributions/spanning_tree.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/stable.py` & `pyro-ppl-1.8.5/pyro/distributions/stable.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/testing/gof.py` & `pyro-ppl-1.8.5/pyro/distributions/testing/gof.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/testing/naive_dirichlet.py` & `pyro-ppl-1.8.5/pyro/distributions/testing/naive_dirichlet.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/testing/rejection_exponential.py` & `pyro-ppl-1.8.5/pyro/distributions/testing/rejection_exponential.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/testing/rejection_gamma.py` & `pyro-ppl-1.8.5/pyro/distributions/testing/rejection_gamma.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/testing/special.py` & `pyro-ppl-1.8.5/pyro/distributions/testing/special.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/torch.py` & `pyro-ppl-1.8.5/pyro/distributions/torch.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/torch_distribution.py` & `pyro-ppl-1.8.5/pyro/distributions/torch_distribution.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/torch_patch.py` & `pyro-ppl-1.8.5/pyro/distributions/torch_patch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,59 @@
 # Copyright (c) 2017-2019 Uber Technologies, Inc.
 # SPDX-License-Identifier: Apache-2.0
 
 import functools
 import math
+import warnings
 import weakref
 
 import torch
 
 
 def patch_dependency(target, root_module=torch):
-    parts = target.split(".")
-    assert parts[0] == root_module.__name__
-    module = root_module
-    for part in parts[1:-1]:
-        module = getattr(module, part)
-    name = parts[-1]
-    old_fn = getattr(module, name, None)
-    old_fn = getattr(old_fn, "_pyro_unpatched", old_fn)  # ensure patching is idempotent
-
-    def decorator(new_fn):
-        try:
-            functools.update_wrapper(new_fn, old_fn)
-        except Exception:
-            for attr in functools.WRAPPER_ASSIGNMENTS:
-                if hasattr(old_fn, attr):
-                    setattr(new_fn, attr, getattr(old_fn, attr))
-        new_fn._pyro_unpatched = old_fn
-        setattr(module, name, new_fn)
-        return new_fn
+    try:
+        parts = target.split(".")
+        assert parts[0] == root_module.__name__
+        module = root_module
+        for part in parts[1:-1]:
+            module = getattr(module, part)
+        name = parts[-1]
+        old_fn = getattr(module, name, None)
+        # Ensure patching is idempotent.
+        old_fn = getattr(old_fn, "_pyro_unpatched", old_fn)
+
+        def decorator(new_fn):
+            try:
+                functools.update_wrapper(new_fn, old_fn)
+            except Exception:
+                for attr in functools.WRAPPER_ASSIGNMENTS:
+                    if hasattr(old_fn, attr):
+                        setattr(new_fn, attr, getattr(old_fn, attr))
+            new_fn._pyro_unpatched = old_fn
+            setattr(module, name, new_fn)
+            return new_fn
+
+    except AttributeError:
+        warnings.warn(f"pyro patch_dependency target is stale: {target}")
+
+        def decorator(new_fn):
+            return new_fn
 
     return decorator
 
 
 # TODO: Move upstream to allow for pickle serialization of transforms
 @patch_dependency("torch.distributions.transforms.Transform.__getstate__")
 def _Transform__getstate__(self):
-    attrs = {}
-    for k, v in self.__dict__.items():
+    super_ = super(torch.distributions.transforms.Transform, self)
+    state = getattr(super_, "__getstate__", self.__dict__.copy)()
+    for k, v in state.items():
         if isinstance(v, weakref.ref):
-            attrs[k] = None
-        else:
-            attrs[k] = v
-    return attrs
+            state[k] = None
+    return state
 
 
 # TODO move upstream
 @patch_dependency("torch.distributions.transforms.Transform.clear_cache")
 def _Transform_clear_cache(self):
     if self._cache_size == 1:
         self._cached_x_y = None, None
@@ -67,25 +75,14 @@
         value, dtype=self.base_dist.scale.dtype, device=self.base_dist.scale.device
     )
     log_prob = self.base_dist.log_prob(value) + math.log(2)
     log_prob.masked_fill_(value.expand(log_prob.shape) < 0, -float("inf"))
     return log_prob
 
 
-# TODO fix batch_shape have an extra singleton dimension upstream
-@patch_dependency("torch.distributions.constraints._PositiveDefinite.check")
-def _PositiveDefinite_check(self, value):
-    matrix_shape = value.shape[-2:]
-    batch_shape = value.shape[:-2]
-    flattened_value = value.reshape((-1,) + matrix_shape)
-    return torch.stack(
-        [torch.linalg.eigvalsh(v)[:1] > 0.0 for v in flattened_value]
-    ).view(batch_shape)
-
-
 @patch_dependency("torch.distributions.constraints._CorrCholesky.check")
 def _CorrCholesky_check(self, value):
     row_norm = torch.linalg.norm(value.detach(), dim=-1)
     unit_row_norm = (row_norm - 1.0).abs().le(1e-4).all(dim=-1)
     return torch.distributions.constraints.lower_cholesky.check(value) & unit_row_norm
```

### Comparing `pyro-ppl-1.8.4/pyro/distributions/torch_transform.py` & `pyro-ppl-1.8.5/pyro/distributions/torch_transform.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,14 +21,20 @@
     """
     This allows us to use a list of `TransformModule` in the same way as
     :class:`~torch.distributions.transform.ComposeTransform`. This is needed
     so that transform parameters are automatically registered by Pyro's param
     store when used in :class:`~pyro.nn.module.PyroModule` instances.
     """
 
-    def __init__(self, parts):
-        super().__init__(parts)
+    def __init__(self, parts, cache_size=0):
+        super().__init__(parts, cache_size=cache_size)
         for part in parts:
-            self.append(part)
+            if isinstance(part, torch.nn.Module):
+                self.append(part)
 
     def __hash__(self):
         return super(torch.nn.Module, self).__hash__()
+
+    def with_cache(self, cache_size=1):
+        if cache_size == self._cache_size:
+            return self
+        return ComposeTransformModule(self.parts, cache_size=cache_size)
```

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/__init__.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     conditional_affine_coupling,
 )
 from .basic import ELUTransform, LeakyReLUTransform, elu, leaky_relu
 from .batchnorm import BatchNorm, batchnorm
 from .block_autoregressive import BlockAutoregressive, block_autoregressive
 from .cholesky import (
     CholeskyTransform,
+    CorrCholeskyTransform,
     CorrLCholeskyTransform,
     CorrMatrixCholeskyTransform,
 )
 from .discrete_cosine import DiscreteCosineTransform
 from .generalized_channel_permute import (
     ConditionalGeneralizedChannelPermute,
     GeneralizedChannelPermute,
@@ -86,25 +87,19 @@
 
 
 @transform_to.register(constraints.sphere)
 def _transform_to_sphere(constraint):
     return Normalize()
 
 
-@biject_to.register(constraints.corr_cholesky)
-@transform_to.register(constraints.corr_cholesky)
-def _transform_to_corr_cholesky(constraint):
-    return CorrLCholeskyTransform()
-
-
 @biject_to.register(constraints.corr_matrix)
 @transform_to.register(constraints.corr_matrix)
 def _transform_to_corr_matrix(constraint):
     return ComposeTransform(
-        [CorrLCholeskyTransform(), CorrMatrixCholeskyTransform().inv]
+        [CorrCholeskyTransform(), CorrMatrixCholeskyTransform().inv]
     )
 
 
 @biject_to.register(constraints.ordered_vector)
 @transform_to.register(constraints.ordered_vector)
 def _transform_to_ordered_vector(constraint):
     return OrderedTransform()
```

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/affine_autoregressive.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/affine_autoregressive.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/affine_coupling.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/affine_coupling.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/basic.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/basic.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/batchnorm.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/batchnorm.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/block_autoregressive.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/block_autoregressive.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/discrete_cosine.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/discrete_cosine.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/generalized_channel_permute.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/generalized_channel_permute.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/haar.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/haar.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/householder.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/householder.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/lower_cholesky_affine.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/lower_cholesky_affine.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/matrix_exponential.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/matrix_exponential.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/neural_autoregressive.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/neural_autoregressive.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/normalize.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/normalize.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/ordered.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/ordered.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/permute.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/permute.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/planar.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/planar.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/polynomial.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/polynomial.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/power.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/power.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/radial.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/radial.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/softplus.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/softplus.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/spline.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/spline.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/spline_autoregressive.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/spline_autoregressive.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/spline_coupling.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/spline_coupling.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/sylvester.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/sylvester.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/transforms/unit_cholesky.py` & `pyro-ppl-1.8.5/pyro/distributions/transforms/unit_cholesky.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/unit.py` & `pyro-ppl-1.8.5/pyro/distributions/unit.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/util.py` & `pyro-ppl-1.8.5/pyro/distributions/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/von_mises_3d.py` & `pyro-ppl-1.8.5/pyro/distributions/von_mises_3d.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/distributions/zero_inflated.py` & `pyro-ppl-1.8.5/pyro/distributions/zero_inflated.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/__init__.py` & `pyro-ppl-1.8.5/pyro/infer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/abstract_infer.py` & `pyro-ppl-1.8.5/pyro/infer/abstract_infer.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/autoguide/__init__.py` & `pyro-ppl-1.8.5/pyro/infer/autoguide/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/autoguide/effect.py` & `pyro-ppl-1.8.5/pyro/infer/autoguide/effect.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/autoguide/gaussian.py` & `pyro-ppl-1.8.5/pyro/infer/autoguide/gaussian.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/autoguide/guides.py` & `pyro-ppl-1.8.5/pyro/infer/autoguide/guides.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/autoguide/initialization.py` & `pyro-ppl-1.8.5/pyro/infer/autoguide/initialization.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/autoguide/structured.py` & `pyro-ppl-1.8.5/pyro/infer/autoguide/structured.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/autoguide/utils.py` & `pyro-ppl-1.8.5/pyro/infer/autoguide/utils.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/csis.py` & `pyro-ppl-1.8.5/pyro/infer/csis.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/discrete.py` & `pyro-ppl-1.8.5/pyro/infer/discrete.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/elbo.py` & `pyro-ppl-1.8.5/pyro/infer/elbo.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,17 +62,18 @@
                 loss.backward()
                 optim.step()
 
         Note that Pyro's global parameter store may cause this new interface to
         behave unexpectedly relative to standard PyTorch when working with
         :class:`~pyro.nn.PyroModule` s.
 
-        Users are therefore strongly encouraged to use this interface in conjunction
-        with :func:`~pyro.enable_module_local_param` which will override the default
-        implicit sharing of parameters across :class:`~pyro.nn.PyroModule` instances.
+        Users are therefore strongly encouraged to use this interface in
+        conjunction with ``pyro.settings.set(module_local_params=True)`` which
+        will override the default implicit sharing of parameters across
+        :class:`~pyro.nn.PyroModule` instances.
 
     :param num_particles: The number of particles/samples used to form the ELBO
         (gradient) estimators.
     :param int max_plate_nesting: Optional bound on max number of nested
         :func:`pyro.plate` contexts. This is only required when enumerating
         over sample sites in parallel, e.g. if a site sets
         ``infer={"enumerate": "parallel"}``. If omitted, ELBO may guess a valid
```

### Comparing `pyro-ppl-1.8.4/pyro/infer/energy_distance.py` & `pyro-ppl-1.8.5/pyro/infer/energy_distance.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/enum.py` & `pyro-ppl-1.8.5/pyro/infer/enum.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/importance.py` & `pyro-ppl-1.8.5/pyro/infer/importance.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/inspect.py` & `pyro-ppl-1.8.5/pyro/infer/inspect.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright Contributors to the Pyro project.
 # SPDX-License-Identifier: Apache-2.0
 
 import itertools
+import os
 from collections import defaultdict
 from pathlib import Path
 from types import SimpleNamespace
 from typing import Callable, Dict, List, Optional, Union
 
 import torch
 
@@ -85,15 +86,15 @@
         variables to dictionaries mapping upstream latent variables on which
         they depend to sets of plates inducing full dependencies.
         That is, included plates introduce quadratically many dependencies as
         in complete-bipartite graphs, whereas excluded plates introduce only
         linearly many dependencies as in independent sets of parallel edges.
         Prior dependencies follow the original model order.
     -   `posterior_dependencies` is a similar dict, but mapping latent
-        variables to the latent or observed sits on which they depend in the
+        variables to the latent or observed sites on which they depend in the
         posterior. Posterior dependencies are reversed from the model order.
 
     Dependencies elide ``pyro.deterministic`` sites and ``pyro.sample(...,
     Delta(...))`` sites.
 
     **Examples**
 
@@ -112,15 +113,15 @@
             "posterior_dependencies": {
                 "a": {"a": set(), "b": set()},
             },
         }
 
     Here is an example where two variables ``a`` and ``b`` start out
     conditionally independent in the prior, but become conditionally dependent
-    in the posterior do the so-called collider variable ``c`` on which they
+    in the posterior to the so-called collider variable ``c`` on which they
     both depend. This is called "moralization" in the graphical model
     literature::
 
         def model_2():
             a = pyro.sample("a", dist.Normal(0, 1))
             b = pyro.sample("b", dist.LogNormal(0, 1))
             c = pyro.sample("c", dist.Normal(a, b))
@@ -138,16 +139,16 @@
                 "b": {"b": set(), "c": set()},
                 "c": {"c": set(), "d": set()},
             },
         }
 
     Dependencies can be more complex in the presence of plates. So far all the
     dict values have been empty sets of plates, but in the following posterior
-    we see that ``c`` depends on itself across the plate ``p``. This means
-    that, among the elements of ``c``, e.g. ``c[0]`` depends on ``c[1]`` (this
+    we see that ``a`` depends on itself across the plate ``p``. This means
+    that, among the elements of ``a``, e.g. ``a[0]`` depends on ``a[1]`` (this
     is why we explicitly allow variables to depend on themselves)::
 
         def model_3():
             with pyro.plate("p", 5):
                 a = pyro.sample("a", dist.Normal(0, 1))
             pyro.sample("b", dist.Normal(a.sum(), 1), obs=torch.tensor(0.0))
 
@@ -568,15 +569,15 @@
     `model rendering tutorial <https://pyro.ai/examples/model_rendering.html>`_ .
 
     :param model: Model to render.
     :param model_args: Tuple of positional arguments to pass to the model, or
         list of tuples for semisupervised models.
     :param model_kwargs: Dict of keyword arguments to pass to the model, or
         list of dicts for semisupervised models.
-    :param str filename: File to save rendered model in.
+    :param str filename: Name of file or path to file to save rendered model in.
     :param bool render_distributions: Whether to include RV distribution
         annotations (and param constraints) in the plot.
     :param bool render_params: Whether to show params inthe plot.
     :returns: A model graph.
     :rtype: graphviz.Digraph
     """
     # Get model relations.
@@ -600,17 +601,17 @@
     ]
     graph_spec = _deep_merge(graph_specs)
 
     # Render.
     graph = render_graph(graph_spec, render_distributions=render_distributions)
 
     if filename is not None:
-        filename = Path(filename)
-        suffix = filename.suffix[1:]  # remove leading period from suffix
-        graph.render(filename.stem, view=False, cleanup=True, format=suffix)
+        suffix = Path(filename).suffix[1:]  # remove leading period from suffix
+        filepath = os.path.splitext(filename)[0]
+        graph.render(filepath, view=False, cleanup=True, format=suffix)
 
     return graph
 
 
 __all__ = [
     "get_dependencies",
     "render_model",
```

### Comparing `pyro-ppl-1.8.4/pyro/infer/mcmc/adaptation.py` & `pyro-ppl-1.8.5/pyro/infer/mcmc/adaptation.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/mcmc/api.py` & `pyro-ppl-1.8.5/pyro/infer/mcmc/api.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/mcmc/hmc.py` & `pyro-ppl-1.8.5/pyro/infer/mcmc/hmc.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/mcmc/logger.py` & `pyro-ppl-1.8.5/pyro/infer/mcmc/logger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/mcmc/mcmc_kernel.py` & `pyro-ppl-1.8.5/pyro/infer/mcmc/mcmc_kernel.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/mcmc/nuts.py` & `pyro-ppl-1.8.5/pyro/infer/mcmc/nuts.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/mcmc/util.py` & `pyro-ppl-1.8.5/pyro/infer/mcmc/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -689,15 +689,14 @@
     parallel = kwargs.pop("parallel", False)
 
     max_plate_nesting = _guess_max_plate_nesting(model, args, kwargs)
     model_trace = prune_subsample_sites(poutine.trace(model).get_trace(*args, **kwargs))
     reshaped_samples = {}
 
     for name, sample in posterior_samples.items():
-
         batch_size, sample_shape = sample.shape[0], sample.shape[1:]
 
         if num_samples is None:
             num_samples = batch_size
 
         elif num_samples != batch_size:
             warnings.warn(
```

### Comparing `pyro-ppl-1.8.4/pyro/infer/predictive.py` & `pyro-ppl-1.8.5/pyro/infer/predictive.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/renyi_elbo.py` & `pyro-ppl-1.8.5/pyro/infer/renyi_elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/reparam/__init__.py` & `pyro-ppl-1.8.5/pyro/infer/reparam/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/reparam/conjugate.py` & `pyro-ppl-1.8.5/pyro/infer/reparam/conjugate.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/reparam/discrete_cosine.py` & `pyro-ppl-1.8.5/pyro/infer/reparam/discrete_cosine.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/reparam/haar.py` & `pyro-ppl-1.8.5/pyro/infer/reparam/haar.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/reparam/hmm.py` & `pyro-ppl-1.8.5/pyro/infer/reparam/hmm.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/reparam/loc_scale.py` & `pyro-ppl-1.8.5/pyro/infer/reparam/loc_scale.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/reparam/neutra.py` & `pyro-ppl-1.8.5/pyro/infer/reparam/neutra.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/reparam/projected_normal.py` & `pyro-ppl-1.8.5/pyro/infer/reparam/projected_normal.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/reparam/reparam.py` & `pyro-ppl-1.8.5/pyro/infer/reparam/reparam.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/reparam/softmax.py` & `pyro-ppl-1.8.5/pyro/infer/reparam/softmax.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/reparam/split.py` & `pyro-ppl-1.8.5/pyro/infer/reparam/split.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/reparam/stable.py` & `pyro-ppl-1.8.5/pyro/infer/reparam/stable.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/reparam/strategies.py` & `pyro-ppl-1.8.5/pyro/infer/reparam/strategies.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/reparam/structured.py` & `pyro-ppl-1.8.5/pyro/infer/reparam/structured.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/reparam/studentt.py` & `pyro-ppl-1.8.5/pyro/infer/reparam/studentt.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/reparam/transform.py` & `pyro-ppl-1.8.5/pyro/infer/reparam/transform.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/reparam/unit_jacobian.py` & `pyro-ppl-1.8.5/pyro/infer/reparam/unit_jacobian.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/resampler.py` & `pyro-ppl-1.8.5/pyro/infer/resampler.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/rws.py` & `pyro-ppl-1.8.5/pyro/infer/rws.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/smcfilter.py` & `pyro-ppl-1.8.5/pyro/infer/smcfilter.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/svgd.py` & `pyro-ppl-1.8.5/pyro/infer/svgd.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/svi.py` & `pyro-ppl-1.8.5/pyro/infer/svi.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/trace_elbo.py` & `pyro-ppl-1.8.5/pyro/infer/trace_elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/trace_mean_field_elbo.py` & `pyro-ppl-1.8.5/pyro/infer/trace_mean_field_elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/trace_mmd.py` & `pyro-ppl-1.8.5/pyro/infer/trace_mmd.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/trace_tail_adaptive_elbo.py` & `pyro-ppl-1.8.5/pyro/infer/trace_tail_adaptive_elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/traceenum_elbo.py` & `pyro-ppl-1.8.5/pyro/infer/traceenum_elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/tracegraph_elbo.py` & `pyro-ppl-1.8.5/pyro/infer/tracegraph_elbo.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,14 @@
         raise ValueError(
             "Unrecognized baseline options: {}".format(options_dict.keys())
         )
     return options_tuple
 
 
 def _construct_baseline(node, guide_site, downstream_cost):
-
     # XXX should the average baseline be in the param store as below?
 
     baseline = 0.0
     baseline_loss = 0.0
 
     (
         nn_baseline,
@@ -173,15 +172,14 @@
             guide_trace.nodes[k]["cond_indep_stack"]
         )
 
     return downstream_costs, downstream_guide_cost_nodes
 
 
 def _compute_elbo(model_trace, guide_trace):
-
     # In ref [1], section 3.2, the part of the surrogate loss computed here is
     # \sum{cost}, which in this case is the ELBO. Instead of using the ELBO,
     # this implementation uses a surrogate ELBO which modifies some entropy
     # terms depending on the parameterization. This reduces the variance of the
     # gradient under some conditions.
 
     elbo = 0.0
@@ -358,31 +356,28 @@
 
         elbo = torch_item(elbo)
         loss = -elbo
         warn_if_nan(loss, "loss")
         return loss
 
     def _loss_and_surrogate_loss(self, model, guide, args, kwargs):
-
         loss = 0.0
         surrogate_loss = 0.0
 
         for model_trace, guide_trace in self._get_traces(model, guide, args, kwargs):
-
             lp, slp = self._loss_and_surrogate_loss_particle(model_trace, guide_trace)
             loss += lp
             surrogate_loss += slp
 
         loss /= self.num_particles
         surrogate_loss /= self.num_particles
 
         return loss, surrogate_loss
 
     def _loss_and_surrogate_loss_particle(self, model_trace, guide_trace):
-
         elbo, surrogate_loss = _compute_elbo(model_trace, guide_trace)
 
         return elbo, surrogate_loss
 
 
 class JitTraceGraph_ELBO(TraceGraph_ELBO):
     """
```

### Comparing `pyro-ppl-1.8.4/pyro/infer/tracetmc_elbo.py` & `pyro-ppl-1.8.5/pyro/infer/tracetmc_elbo.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/infer/util.py` & `pyro-ppl-1.8.5/pyro/infer/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/nn/__init__.py` & `pyro-ppl-1.8.5/pyro/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/nn/auto_reg_nn.py` & `pyro-ppl-1.8.5/pyro/nn/auto_reg_nn.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/nn/dense_nn.py` & `pyro-ppl-1.8.5/pyro/nn/dense_nn.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/nn/module.py` & `pyro-ppl-1.8.5/pyro/nn/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     my_module = PyroModule()
     my_module.x = PyroParam(torch.tensor(1.), constraint=constraints.positive)
     my_module.y = PyroSample(dist.Normal(0, 1))
 
 """
 import functools
 import inspect
+import weakref
 from collections import OrderedDict, namedtuple
 
 import torch
 from torch.distributions import constraints, transform_to
 
 import pyro
 from pyro.ops.provenance import detach_provenance
@@ -499,15 +500,17 @@
                     else:
                         # Update PyroModule ---> ParamStore.
                         _PYRO_PARAM_STORE._constraints[fullname] = constraint
                         _PYRO_PARAM_STORE._params[fullname] = unconstrained_value
                         _PYRO_PARAM_STORE._param_to_name[unconstrained_value] = fullname
                     return pyro.param(fullname, event_dim=event_dim)
                 else:  # Cannot determine supermodule and hence cannot compute fullname.
-                    return transform_to(constraint)(unconstrained_value)
+                    constrained_value = transform_to(constraint)(unconstrained_value)
+                    constrained_value.unconstrained = weakref.ref(unconstrained_value)
+                    return constrained_value
 
         # PyroSample trigger pyro.sample statements.
         if "_pyro_samples" in self.__dict__:
             _pyro_samples = self.__dict__["_pyro_samples"]
             if name in _pyro_samples:
                 prior = _pyro_samples[name]
                 context = self._pyro_context
@@ -657,14 +660,20 @@
                 for p in list(_PYRO_PARAM_STORE.keys()):
                     if p.startswith(fullname):
                         del _PYRO_PARAM_STORE[p]
             return
 
         super().__delattr__(name)
 
+    def __getstate__(self):
+        # Remove weakrefs in preparation for pickling.
+        for param in self.parameters(recurse=True):
+            param.__dict__.pop("unconstrained", None)
+        return getattr(super(), "__getstate__", self.__dict__.copy)()
+
 
 def pyro_method(fn):
     """
     Decorator for top-level methods of a :class:`PyroModule` to enable pyro
     effects and cache ``pyro.sample`` statements.
 
     This should be applied to all public methods that read Pyro-managed
```

### Comparing `pyro-ppl-1.8.4/pyro/ops/arrowhead.py` & `pyro-ppl-1.8.5/pyro/ops/arrowhead.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/ops/contract.py` & `pyro-ppl-1.8.5/pyro/ops/contract.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,14 @@
         # Arbitrarily deterministically choose a leaf.
         leaf = max(tensor_tree, key=len)
         leaf_terms = tensor_tree.pop(leaf)
         leaf_dims = dims_tree.pop(leaf, set())
 
         # Split terms at the current ordinal into connected components.
         for terms, dims in _partition_terms(ring, leaf_terms, leaf_dims):
-
             # Eliminate sum dims via a sumproduct contraction.
             term = ring.sumproduct(terms, dims - local_dims)
 
             # Eliminate extra plate dims via product contractions.
             if leaf == min_ordinal:
                 parent = leaf
             else:
```

### Comparing `pyro-ppl-1.8.4/pyro/ops/dual_averaging.py` & `pyro-ppl-1.8.5/pyro/ops/dual_averaging.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/ops/einsum/__init__.py` & `pyro-ppl-1.8.5/pyro/ops/einsum/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/ops/einsum/adjoint.py` & `pyro-ppl-1.8.5/pyro/ops/einsum/adjoint.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/ops/einsum/torch_log.py` & `pyro-ppl-1.8.5/pyro/ops/einsum/torch_log.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/ops/einsum/torch_map.py` & `pyro-ppl-1.8.5/pyro/ops/einsum/torch_map.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/ops/einsum/torch_marginal.py` & `pyro-ppl-1.8.5/pyro/ops/einsum/torch_marginal.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/ops/einsum/torch_sample.py` & `pyro-ppl-1.8.5/pyro/ops/einsum/torch_sample.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/ops/einsum/util.py` & `pyro-ppl-1.8.5/pyro/ops/einsum/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/ops/gamma_gaussian.py` & `pyro-ppl-1.8.5/pyro/ops/gamma_gaussian.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/ops/gaussian.py` & `pyro-ppl-1.8.5/pyro/ops/gaussian.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/ops/hessian.py` & `pyro-ppl-1.8.5/pyro/ops/hessian.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/ops/indexing.py` & `pyro-ppl-1.8.5/pyro/ops/indexing.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/ops/integrator.py` & `pyro-ppl-1.8.5/pyro/ops/integrator.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/ops/jit.py` & `pyro-ppl-1.8.5/pyro/ops/jit.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/ops/linalg.py` & `pyro-ppl-1.8.5/pyro/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/ops/newton.py` & `pyro-ppl-1.8.5/pyro/ops/newton.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/ops/packed.py` & `pyro-ppl-1.8.5/pyro/ops/packed.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/ops/provenance.py` & `pyro-ppl-1.8.5/pyro/ops/provenance.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,22 +42,23 @@
     :param frozenset provenance: An initial provenance set.
     """
 
     def __new__(cls, data: torch.Tensor, provenance=frozenset(), **kwargs):
         assert not isinstance(data, ProvenanceTensor)
         if not provenance:
             return data
-        return super().__new__(cls)
+        ret = data.as_subclass(cls)
+        ret._t = data  # this makes sure that detach_provenance always
+        # returns the same object. This is important when
+        # using the tensor as key in a dict, e.g. the global
+        # param store
+        return ret
 
     def __init__(self, data, provenance=frozenset()):
         assert isinstance(provenance, frozenset)
-        if isinstance(data, ProvenanceTensor):
-            provenance |= data._provenance
-            data = data._t
-        self._t = data
         self._provenance = provenance
 
     def __repr__(self):
         return "Provenance:\n{}\nTensor:\n{}".format(self._provenance, self._t)
 
     @classmethod
     def __torch_function__(cls, func, types, args=(), kwargs=None):
```

### Comparing `pyro-ppl-1.8.4/pyro/ops/rings.py` & `pyro-ppl-1.8.5/pyro/ops/rings.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/ops/special.py` & `pyro-ppl-1.8.5/pyro/ops/special.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/ops/ssm_gp.py` & `pyro-ppl-1.8.5/pyro/ops/ssm_gp.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/ops/stats.py` & `pyro-ppl-1.8.5/pyro/ops/stats.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/ops/streaming.py` & `pyro-ppl-1.8.5/pyro/ops/streaming.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/ops/tensor_utils.py` & `pyro-ppl-1.8.5/pyro/ops/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/ops/welford.py` & `pyro-ppl-1.8.5/pyro/ops/welford.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/optim/__init__.py` & `pyro-ppl-1.8.5/pyro/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/optim/adagrad_rmsprop.py` & `pyro-ppl-1.8.5/pyro/optim/adagrad_rmsprop.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/optim/clipped_adam.py` & `pyro-ppl-1.8.5/pyro/optim/clipped_adam.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/optim/dct_adam.py` & `pyro-ppl-1.8.5/pyro/optim/dct_adam.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/optim/horovod.py` & `pyro-ppl-1.8.5/pyro/optim/horovod.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/optim/lr_scheduler.py` & `pyro-ppl-1.8.5/pyro/optim/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/optim/multi.py` & `pyro-ppl-1.8.5/pyro/optim/multi.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/optim/optim.py` & `pyro-ppl-1.8.5/pyro/optim/optim.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,18 +134,24 @@
                 state = self._state_waiting_to_be_consumed.pop(param_name, None)
                 if state is not None:
                     _load_state_dict(optimizer, state)
 
             if self.grad_clip[p] is not None:
                 self.grad_clip[p](p)
 
-            if isinstance(
-                self.optim_objs[p], torch.optim.lr_scheduler._LRScheduler
-            ) or isinstance(
-                self.optim_objs[p], torch.optim.lr_scheduler.ReduceLROnPlateau
+            if (
+                hasattr(torch.optim.lr_scheduler, "_LRScheduler")
+                and isinstance(
+                    self.optim_objs[p], torch.optim.lr_scheduler._LRScheduler
+                )
+                or hasattr(torch.optim.lr_scheduler, "LRScheduler")
+                and isinstance(self.optim_objs[p], torch.optim.lr_scheduler.LRScheduler)
+                or isinstance(
+                    self.optim_objs[p], torch.optim.lr_scheduler.ReduceLROnPlateau
+                )
             ):
                 # if optim object was a scheduler, perform an optimizer step
                 self.optim_objs[p].optimizer.step(*args, **kwargs)
             else:
                 self.optim_objs[p].step(*args, **kwargs)
 
     def get_state(self) -> Dict:
@@ -227,15 +233,14 @@
 
         return _clip_grad
 
     def _get_grad_clip_args(self, param: str) -> Dict:
         # if we were passed a fct, we call fct with param info
         # arguments are (module name, param name) e.g. ('mymodule', 'bias')
         if callable(self.pt_clip_args):
-
             # get param name
             param_name = pyro.get_param_store().param_name(param)
             module_name = module_from_param_with_module_name(param_name)
             stripped_param_name = user_param_name(param_name)
 
             # invoke the user-provided callable
             clip_dict = self.pt_clip_args(module_name, stripped_param_name)
```

### Comparing `pyro-ppl-1.8.4/pyro/optim/pytorch_optimizers.py` & `pyro-ppl-1.8.5/pyro/optim/pytorch_optimizers.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,21 +30,24 @@
     )
 
     locals()[_name] = _PyroOptim
     __all__.append(_name)
     del _PyroOptim
 
 # Load all schedulers from PyTorch
+# breaking change in torch >= 1.14: LRScheduler is new base class
+if hasattr(torch.optim.lr_scheduler, "LRScheduler"):
+    _torch_scheduler_base = torch.optim.lr_scheduler.LRScheduler  # type: ignore
+else:  # for torch < 1.13, _LRScheduler is base class
+    _torch_scheduler_base = torch.optim.lr_scheduler._LRScheduler  # type: ignore
+
 for _name, _Optim in torch.optim.lr_scheduler.__dict__.items():
     if not isinstance(_Optim, type):
         continue
-    if (
-        not issubclass(_Optim, torch.optim.lr_scheduler._LRScheduler)
-        and _name != "ReduceLROnPlateau"
-    ):
+    if not issubclass(_Optim, _torch_scheduler_base) and _name != "ReduceLROnPlateau":
         continue
     if _Optim is torch.optim.Optimizer:
         continue
 
     _PyroOptim = (
         lambda _Optim: lambda optim_args, clip_args=None: PyroLRScheduler(
             _Optim, optim_args, clip_args
```

### Comparing `pyro-ppl-1.8.4/pyro/params/param_store.py` & `pyro-ppl-1.8.5/pyro/params/param_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,18 +239,19 @@
     # -------------------------------------------------------------------------------
     # Persistence interface
 
     def get_state(self) -> dict:
         """
         Get the ParamStore state.
         """
-        state = {
-            "params": self._params.copy(),
-            "constraints": self._constraints.copy(),
-        }
+        params = self._params.copy()
+        # Remove weakrefs in preparation for pickling.
+        for param in params.values():
+            param.__dict__.pop("unconstrained", None)
+        state = {"params": params, "constraints": self._constraints.copy()}
         return state
 
     def set_state(self, state: dict):
         """
         Set the ParamStore state using state from a previous :meth:`get_state` call
         """
         assert isinstance(state, dict), "malformed ParamStore state"
```

### Comparing `pyro-ppl-1.8.4/pyro/poutine/__init__.py` & `pyro-ppl-1.8.5/pyro/poutine/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     markov,
     mask,
     queue,
     reparam,
     replay,
     scale,
     seed,
+    substitute,
     trace,
     uncondition,
 )
 from .messenger import unwrap
 from .runtime import NonlocalExit, get_mask
 from .trace_struct import Trace
 from .util import enable_validation, is_validation_enabled
@@ -43,12 +44,13 @@
     "mask",
     "NonlocalExit",
     "replay",
     "reparam",
     "queue",
     "scale",
     "seed",
+    "substitute",
     "trace",
     "Trace",
     "uncondition",
     "unwrap",
 ]
```

### Comparing `pyro-ppl-1.8.4/pyro/poutine/block_messenger.py` & `pyro-ppl-1.8.5/pyro/poutine/block_messenger.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
     # decision rule for hiding:
     if (
         (msg["name"] in hide)
         or (msg_type in hide_types)
         or (is_not_exposed and hide_all)
     ):  # noqa: E129
-
         return True
     # otherwise expose
     else:
         return False
 
 
 def _make_default_hide_fn(hide_all, expose_all, hide, expose, hide_types, expose_types):
```

### Comparing `pyro-ppl-1.8.4/pyro/poutine/broadcast_messenger.py` & `pyro-ppl-1.8.5/pyro/poutine/broadcast_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/poutine/collapse_messenger.py` & `pyro-ppl-1.8.5/pyro/poutine/collapse_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/poutine/condition_messenger.py` & `pyro-ppl-1.8.5/pyro/poutine/condition_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/poutine/do_messenger.py` & `pyro-ppl-1.8.5/pyro/poutine/do_messenger.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
         self._intervener_id = str(id(self))
 
     def _pyro_sample(self, msg):
         if (
             msg.get("_intervener_id", None) != self._intervener_id
             and self.data.get(msg["name"]) is not None
         ):
-
             if msg.get("_intervener_id", None) is not None:
                 warnings.warn(
                     "Attempting to intervene on variable {} multiple times,"
                     "this is almost certainly incorrect behavior".format(msg["name"]),
                     RuntimeWarning,
                 )
```

### Comparing `pyro-ppl-1.8.4/pyro/poutine/enum_messenger.py` & `pyro-ppl-1.8.5/pyro/poutine/enum_messenger.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     assert any(d > 1 for d in fat_sample.shape)
 
     target_shape = (num_samples,) + batch_shape + dist.event_shape
 
     # if this site has any possible ancestors, sample ancestor indices uniformly
     thin_sample = fat_sample
     if thin_sample.shape != target_shape:
-
         index = [Ellipsis] + [slice(None)] * (len(thin_sample.shape) - 1)
         squashed_dims = []
         for squashed_dim, squashed_size in zip(
             range(1, len(thin_sample.shape)), thin_sample.shape[1:]
         ):
             if squashed_size > 1 and (
                 target_shape[squashed_dim] == 1 or squashed_dim == 0
@@ -75,15 +74,14 @@
     assert any(d > 1 for d in fat_sample.shape)
 
     target_shape = (num_samples,) + batch_shape + dist.event_shape
 
     # if this site has any ancestors, choose ancestors from diagonal approximation
     thin_sample = fat_sample
     if thin_sample.shape != target_shape:
-
         index = [Ellipsis] + [slice(None)] * (len(thin_sample.shape) - 1)
         squashed_dims = []
         for squashed_dim, squashed_size in zip(
             range(1, len(thin_sample.shape)), thin_sample.shape[1:]
         ):
             if squashed_size > 1 and (
                 target_shape[squashed_dim] == 1 or squashed_dim == 0
```

### Comparing `pyro-ppl-1.8.4/pyro/poutine/escape_messenger.py` & `pyro-ppl-1.8.5/pyro/poutine/escape_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/poutine/guide.py` & `pyro-ppl-1.8.5/pyro/poutine/guide.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,20 @@
         # Do not register model as submodule
         self._model = (model,)
 
     @property
     def model(self):
         return self._model[0]
 
+    def __getstate__(self):
+        # Avoid pickling the trace.
+        state = super().__getstate__()
+        state.pop("trace")
+        return state
+
     def __call__(self, *args, **kwargs) -> Dict[str, torch.Tensor]:
         """
         Draws posterior samples from the guide and replays the model against
         those samples.
 
         :returns: A dict mapping sample site name to sample value.
             This includes latent, deterministic, and observed values.
```

### Comparing `pyro-ppl-1.8.4/pyro/poutine/handlers.py` & `pyro-ppl-1.8.5/pyro/poutine/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 from .mask_messenger import MaskMessenger
 from .plate_messenger import PlateMessenger  # noqa F403
 from .reparam_messenger import ReparamMessenger
 from .replay_messenger import ReplayMessenger
 from .runtime import NonlocalExit
 from .scale_messenger import ScaleMessenger
 from .seed_messenger import SeedMessenger
+from .substitute_messenger import SubstituteMessenger
 from .trace_messenger import TraceMessenger
 from .uncondition_messenger import UnconditionMessenger
 
 ############################################
 # Begin primitive operations
 ############################################
 
@@ -93,14 +94,15 @@
     MaskMessenger,
     ReparamMessenger,
     ReplayMessenger,
     ScaleMessenger,
     SeedMessenger,
     TraceMessenger,
     UnconditionMessenger,
+    SubstituteMessenger,
 ]
 
 
 def _make_handler(msngr_cls):
     _re1 = re.compile("(.)([A-Z][a-z]+)")
     _re2 = re.compile("([a-z0-9])([A-Z])")
 
@@ -183,15 +185,14 @@
         escape_fn = util.discrete_escape
 
     if num_samples is None:
         num_samples = -1
 
     def wrapper(wrapped):
         def _fn(*args, **kwargs):
-
             for i in range(max_tries):
                 assert (
                     not queue.empty()
                 ), "trying to get() from an empty queue will deadlock"
 
                 next_trace = queue.get()
                 try:
```

### Comparing `pyro-ppl-1.8.4/pyro/poutine/indep_messenger.py` & `pyro-ppl-1.8.5/pyro/poutine/indep_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/poutine/infer_config_messenger.py` & `pyro-ppl-1.8.5/pyro/poutine/infer_config_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/poutine/lift_messenger.py` & `pyro-ppl-1.8.5/pyro/poutine/lift_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/poutine/markov_messenger.py` & `pyro-ppl-1.8.5/pyro/poutine/markov_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/poutine/mask_messenger.py` & `pyro-ppl-1.8.5/pyro/poutine/mask_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/poutine/messenger.py` & `pyro-ppl-1.8.5/pyro/poutine/messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/poutine/plate_messenger.py` & `pyro-ppl-1.8.5/pyro/poutine/plate_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/poutine/reentrant_messenger.py` & `pyro-ppl-1.8.5/pyro/poutine/reentrant_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/poutine/reparam_messenger.py` & `pyro-ppl-1.8.5/pyro/poutine/reparam_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/poutine/replay_messenger.py` & `pyro-ppl-1.8.5/pyro/poutine/replay_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/poutine/runtime.py` & `pyro-ppl-1.8.5/pyro/poutine/runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,14 @@
 
     # msg is used to pass information up and down the stack
     msg = initial_msg
 
     pointer = 0
     # go until time to stop?
     for frame in reversed(stack):
-
         pointer = pointer + 1
 
         frame._process_message(msg)
 
         if msg["stop"]:
             break
 
@@ -249,15 +248,14 @@
         return fn
 
     assert type is not None, "must provide a type label for operation {}".format(fn)
     assert type != "message", "cannot use 'message' as keyword"
 
     @functools.wraps(fn)
     def _fn(*args, **kwargs):
-
         name = kwargs.pop("name", None)
         infer = kwargs.pop("infer", {})
 
         value = kwargs.pop("obs", None)
         is_observed = value is not None
 
         if not am_i_wrapped():
```

### Comparing `pyro-ppl-1.8.4/pyro/poutine/scale_messenger.py` & `pyro-ppl-1.8.5/pyro/poutine/scale_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/poutine/seed_messenger.py` & `pyro-ppl-1.8.5/pyro/poutine/seed_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/poutine/subsample_messenger.py` & `pyro-ppl-1.8.5/pyro/poutine/subsample_messenger.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,17 @@
                             "Inside pyro.plate({}, {}, dim={}) invalid shape of {}: {}".format(
                                 self.name, self.size, self.dim, statement, shape
                             )
                         )
                     # Subsample parameters with known batch semantics.
                     if self.subsample_size < self.size:
                         value = msg["value"]
-                        new_value = value.index_select(dim, self._indices)
+                        new_value = value.index_select(
+                            dim, self._indices.to(value.device)
+                        )
                         if msg["type"] == "param":
                             if hasattr(value, "_pyro_unconstrained_param"):
                                 param = value._pyro_unconstrained_param
                             else:
                                 param = value.unconstrained()
 
                             if not hasattr(param, "_pyro_subsample"):
```

### Comparing `pyro-ppl-1.8.4/pyro/poutine/trace_messenger.py` & `pyro-ppl-1.8.5/pyro/poutine/trace_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/poutine/trace_struct.py` & `pyro-ppl-1.8.5/pyro/poutine/trace_struct.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/poutine/uncondition_messenger.py` & `pyro-ppl-1.8.5/pyro/poutine/uncondition_messenger.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/poutine/util.py` & `pyro-ppl-1.8.5/pyro/poutine/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/primitives.py` & `pyro-ppl-1.8.5/pyro/primitives.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/settings.py` & `pyro-ppl-1.8.5/pyro/settings.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro/util.py` & `pyro-ppl-1.8.5/pyro/util.py`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/pyro_ppl.egg-info/PKG-INFO` & `pyro-ppl-1.8.5/pyro_ppl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyro-ppl
-Version: 1.8.4
+Version: 1.8.5
 Summary: A Python library for probabilistic modeling and inference
 Home-page: http://pyro.ai
 Author: Uber AI Labs
 License: Apache 2.0
 Project-URL: Documentation, https://docs.pyro.ai
 Project-URL: Source, https://github.com/pyro-ppl/pyro
 Keywords: machine learning statistics probabilistic programming bayesian modeling pytorch
@@ -20,14 +20,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: extras
 Provides-Extra: test
 Provides-Extra: profile
 Provides-Extra: dev
 Provides-Extra: horovod
+Provides-Extra: lightning
 Provides-Extra: funsor
 License-File: LICENSE.md
 
 [Getting Started](http://pyro.ai/examples) |
 [Documentation](http://docs.pyro.ai/) |
 [Community](http://forum.pyro.ai/) |
 [Contributing](https://github.com/pyro-ppl/pyro/blob/master/CONTRIBUTING.md)
```

### Comparing `pyro-ppl-1.8.4/pyro_ppl.egg-info/SOURCES.txt` & `pyro-ppl-1.8.5/pyro_ppl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -312,14 +312,15 @@
 pyro/poutine/reentrant_messenger.py
 pyro/poutine/reparam_messenger.py
 pyro/poutine/replay_messenger.py
 pyro/poutine/runtime.py
 pyro/poutine/scale_messenger.py
 pyro/poutine/seed_messenger.py
 pyro/poutine/subsample_messenger.py
+pyro/poutine/substitute_messenger.py
 pyro/poutine/trace_messenger.py
 pyro/poutine/trace_struct.py
 pyro/poutine/uncondition_messenger.py
 pyro/poutine/util.py
 pyro_ppl.egg-info/PKG-INFO
 pyro_ppl.egg-info/SOURCES.txt
 pyro_ppl.egg-info/dependency_links.txt
```

### Comparing `pyro-ppl-1.8.4/pyro_ppl.egg-info/requires.txt` & `pyro-ppl-1.8.5/pyro_ppl.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 numpy>=1.7
 opt_einsum>=2.3.2
 pyro-api>=0.1.1
-torch>=1.11.0
+torch>=2.0.1
 tqdm>=4.36
 
 [dev]
 jupyter>=1.0.0
 graphviz>=0.8
 matplotlib>=1.3
 torchvision>=0.12.0
@@ -48,14 +48,17 @@
 
 [funsor]
 funsor[torch]==0.4.4
 
 [horovod]
 horovod[pytorch]>=0.19
 
+[lightning]
+pytorch_lightning
+
 [profile]
 prettytable
 pytest-benchmark
 snakeviz
 
 [test]
 jupyter>=1.0.0
```

### Comparing `pyro-ppl-1.8.4/setup.cfg` & `pyro-ppl-1.8.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyro-ppl-1.8.4/setup.py` & `pyro-ppl-1.8.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     install_requires=[
         # if you add any additional libraries, please also
         # add them to `docs/requirements.txt`
         # numpy is necessary for some functionality of PyTorch
         "numpy>=1.7",
         "opt_einsum>=2.3.2",
         "pyro-api>=0.1.1",
-        "torch>=1.11.0",
+        "torch>=2.0.1",
         "tqdm>=4.36",
     ],
     extras_require={
         "extras": EXTRAS_REQUIRE,
         "test": EXTRAS_REQUIRE
         + [
             "black>=21.4b0",
@@ -133,14 +133,15 @@
             "pytest-xdist",
             "scipy>=1.1",
             "sphinx",
             "sphinx_rtd_theme",
             "yapf",
         ],
         "horovod": ["horovod[pytorch]>=0.19"],
+        "lightning": ["pytorch_lightning"],
         "funsor": [
             # This must be a released version when Pyro is released.
             # "funsor[torch] @ git+git://github.com/pyro-ppl/funsor.git@7bb52d0eae3046d08a20d1b288544e1a21b4f461",
             "funsor[torch]==0.4.4",
         ],
     },
     python_requires=">=3.7",
```

