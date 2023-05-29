# Comparing `tmp/dLux-0.9.1.tar.gz` & `tmp/dLux-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dLux-0.9.1.tar", last modified: Tue Nov  8 05:12:55 2022, max compression
+gzip compressed data, was "dLux-0.9.2.tar", last modified: Mon Nov 14 12:23:21 2022, max compression
```

## Comparing `dLux-0.9.1.tar` & `dLux-0.9.2.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.607686 dLux-0.9.1/
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.591721 dLux-0.9.1/.github/
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.594457 dLux-0.9.1/.github/workflows/
--rw-r--r--   0 louis      (501) staff       (20)      848 2022-11-06 01:42:52.000000 dLux-0.9.1/.github/workflows/documentation.yml
--rw-r--r--   0 louis      (501) staff       (20)     1333 2022-11-08 02:49:52.000000 dLux-0.9.1/.github/workflows/tests.yml
--rw-r--r--   0 louis      (501) staff       (20)      137 2022-11-08 02:49:52.000000 dLux-0.9.1/.gitignore
--rw-r--r--   0 louis      (501) staff       (20)     5202 2022-07-26 16:35:15.000000 dLux-0.9.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 louis      (501) staff       (20)     1847 2022-11-08 02:49:52.000000 dLux-0.9.1/CONTRIBUTING.md
--rw-r--r--   0 louis      (501) staff       (20)     1544 2022-05-04 13:56:11.000000 dLux-0.9.1/LICENSE.md
--rw-r--r--   0 louis      (501) staff       (20)       24 2022-11-08 04:52:54.000000 dLux-0.9.1/MANIFEST.in
--rw-r--r--   0 louis      (501) staff       (20)      484 2022-11-08 05:12:55.607557 dLux-0.9.1/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)     4365 2022-11-08 02:49:52.000000 dLux-0.9.1/README.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.595547 dLux-0.9.1/dLux/
--rw-r--r--   0 louis      (501) staff       (20)      942 2022-11-08 05:12:10.000000 dLux-0.9.1/dLux/__init__.py
--rw-r--r--   0 louis      (501) staff       (20)    31104 2022-11-08 02:49:52.000000 dLux-0.9.1/dLux/base.py
--rw-r--r--   0 louis      (501) staff       (20)    58100 2022-11-08 02:49:52.000000 dLux-0.9.1/dLux/core.py
--rw-r--r--   0 louis      (501) staff       (20)    11767 2022-11-08 02:49:52.000000 dLux-0.9.1/dLux/detectors.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.596331 dLux-0.9.1/dLux/dev/
--rw-r--r--   0 louis      (501) staff       (20)    24499 2022-11-06 01:42:52.000000 dLux-0.9.1/dLux/dev/FFTfresnel.py
--rw-r--r--   0 louis      (501) staff       (20)     4400 2022-07-26 16:35:15.000000 dLux-0.9.1/dLux/dev/constants.py
--rw-r--r--   0 louis      (501) staff       (20)    54752 2022-11-06 01:42:52.000000 dLux-0.9.1/dLux/dev/layers.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.596560 dLux-0.9.1/dLux/dev/tests/
--rw-r--r--   0 louis      (501) staff       (20)      395 2022-10-05 21:35:52.000000 dLux-0.9.1/dLux/dev/tests/layers.py
--rw-r--r--   0 louis      (501) staff       (20)       58 2022-07-26 16:35:15.000000 dLux-0.9.1/dLux/dev/tests/source.py
--rw-r--r--   0 louis      (501) staff       (20)    40303 2022-11-08 02:49:52.000000 dLux-0.9.1/dLux/optics.py
--rw-r--r--   0 louis      (501) staff       (20)    29840 2022-11-08 02:49:52.000000 dLux-0.9.1/dLux/propagators.py
--rw-r--r--   0 louis      (501) staff       (20)    33509 2022-11-08 02:49:52.000000 dLux-0.9.1/dLux/sources.py
--rw-r--r--   0 louis      (501) staff       (20)     9497 2022-11-08 02:49:52.000000 dLux-0.9.1/dLux/spectrums.py
--rw-r--r--   0 louis      (501) staff       (20)    11753 2022-11-08 02:49:52.000000 dLux-0.9.1/dLux/spiders.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.597705 dLux-0.9.1/dLux/utils/
--rw-r--r--   0 louis      (501) staff       (20)      799 2022-11-08 02:49:52.000000 dLux-0.9.1/dLux/utils/__init__.py
--rw-r--r--   0 louis      (501) staff       (20)     6555 2022-11-08 02:49:52.000000 dLux-0.9.1/dLux/utils/bayes.py
--rw-r--r--   0 louis      (501) staff       (20)     6585 2022-11-08 02:49:52.000000 dLux-0.9.1/dLux/utils/coordinates.py
--rw-r--r--   0 louis      (501) staff       (20)     2684 2022-11-08 02:49:52.000000 dLux-0.9.1/dLux/utils/gradient_energy.py
--rw-r--r--   0 louis      (501) staff       (20)     2059 2022-11-08 02:49:52.000000 dLux-0.9.1/dLux/utils/helpers.py
--rw-r--r--   0 louis      (501) staff       (20)     7053 2022-11-06 01:42:52.000000 dLux-0.9.1/dLux/utils/hexike.py
--rw-r--r--   0 louis      (501) staff       (20)    11656 2022-11-08 02:49:52.000000 dLux-0.9.1/dLux/utils/interpolation.py
--rw-r--r--   0 louis      (501) staff       (20)     8457 2022-11-08 02:49:52.000000 dLux-0.9.1/dLux/utils/models.py
--rw-r--r--   0 louis      (501) staff       (20)     5807 2022-11-08 02:49:52.000000 dLux-0.9.1/dLux/utils/optics.py
--rw-r--r--   0 louis      (501) staff       (20)     1699 2022-11-06 01:42:52.000000 dLux-0.9.1/dLux/utils/plotting.py
--rw-r--r--   0 louis      (501) staff       (20)      934 2022-11-08 02:49:52.000000 dLux-0.9.1/dLux/utils/units.py
--rw-r--r--   0 louis      (501) staff       (20)     8924 2022-11-06 01:42:52.000000 dLux-0.9.1/dLux/utils/zernike.py
--rw-r--r--   0 louis      (501) staff       (20)    28017 2022-11-08 02:49:52.000000 dLux-0.9.1/dLux/wavefronts.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.596029 dLux-0.9.1/dLux.egg-info/
--rw-r--r--   0 louis      (501) staff       (20)      484 2022-11-08 05:12:55.000000 dLux-0.9.1/dLux.egg-info/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)     4212 2022-11-08 05:12:55.000000 dLux-0.9.1/dLux.egg-info/SOURCES.txt
--rw-r--r--   0 louis      (501) staff       (20)        1 2022-11-08 05:12:55.000000 dLux-0.9.1/dLux.egg-info/dependency_links.txt
--rw-r--r--   0 louis      (501) staff       (20)       74 2022-11-08 05:12:55.000000 dLux-0.9.1/dLux.egg-info/requires.txt
--rw-r--r--   0 louis      (501) staff       (20)       16 2022-11-08 05:12:55.000000 dLux-0.9.1/dLux.egg-info/top_level.txt
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.593006 dLux-0.9.1/docs/
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.597806 dLux-0.9.1/docs/assets/
--rw-r--r--   0 louis      (501) staff       (20)   534462 2022-11-06 01:42:52.000000 dLux-0.9.1/docs/assets/logo.jpg
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.598277 dLux-0.9.1/docs/base/
--rw-r--r--   0 louis      (501) staff       (20)       19 2022-11-06 01:42:52.000000 dLux-0.9.1/docs/base/base.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.598988 dLux-0.9.1/docs/core/
--rw-r--r--   0 louis      (501) staff       (20)       23 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/core/detector.md
--rw-r--r--   0 louis      (501) staff       (20)       21 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/core/filter.md
--rw-r--r--   0 louis      (501) staff       (20)       24 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/core/instrument.md
--rw-r--r--   0 louis      (501) staff       (20)       20 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/core/model.md
--rw-r--r--   0 louis      (501) staff       (20)       28 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/core/optical_system.md
--rw-r--r--   0 louis      (501) staff       (20)       21 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/core/optics.md
--rw-r--r--   0 louis      (501) staff       (20)       20 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/core/scene.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.599465 dLux-0.9.1/docs/detectors/
--rw-r--r--   0 louis      (501) staff       (20)       30 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/detectors/add_constant.md
--rw-r--r--   0 louis      (501) staff       (20)       30 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/detectors/apply_jitter.md
--rw-r--r--   0 louis      (501) staff       (20)       37 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/detectors/apply_pixel_response.md
--rw-r--r--   0 louis      (501) staff       (20)       34 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/detectors/apply_saturation.md
--rw-r--r--   0 louis      (501) staff       (20)       36 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/detectors/integer_downsample.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.600473 dLux-0.9.1/docs/optics/
--rw-r--r--   0 louis      (501) staff       (20)       23 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/optics/add_opd.md
--rw-r--r--   0 louis      (501) staff       (20)       25 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/optics/add_phase.md
--rw-r--r--   0 louis      (501) staff       (20)       32 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/optics/apply_basis_climb.md
--rw-r--r--   0 louis      (501) staff       (20)       30 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/optics/apply_basis_opd.md
--rw-r--r--   0 louis      (501) staff       (20)       33 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/optics/circular_aperture.md
--rw-r--r--   0 louis      (501) staff       (20)       33 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/optics/compound_aperture.md
--rw-r--r--   0 louis      (501) staff       (20)       32 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/optics/create_wavefront.md
--rw-r--r--   0 louis      (501) staff       (20)       35 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/optics/normalise_wavefront.md
--rw-r--r--   0 louis      (501) staff       (20)       30 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/optics/tilt_wavefront.md
--rw-r--r--   0 louis      (501) staff       (20)       34 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/optics/transmissive_optic.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.592427 dLux-0.9.1/docs/propagators/
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.601127 dLux-0.9.1/docs/propagators/abstract/
--rw-r--r--   0 louis      (501) staff       (20)       38 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/propagators/abstract/angular_propagator.md
--rw-r--r--   0 louis      (501) staff       (20)       40 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/propagators/abstract/cartesian_propagator.md
--rw-r--r--   0 louis      (501) staff       (20)       36 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/propagators/abstract/far_field_fresnel.md
--rw-r--r--   0 louis      (501) staff       (20)       45 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/propagators/abstract/fixed_sampling_propagator.md
--rw-r--r--   0 louis      (501) staff       (20)       32 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/propagators/abstract/propagator.md
--rw-r--r--   0 louis      (501) staff       (20)       48 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/propagators/abstract/variable_sampling_propagator.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.601629 dLux-0.9.1/docs/propagators/concrete/
--rw-r--r--   0 louis      (501) staff       (20)       32 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/propagators/concrete/angular_fft.md
--rw-r--r--   0 louis      (501) staff       (20)       32 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/propagators/concrete/angular_mft.md
--rw-r--r--   0 louis      (501) staff       (20)       34 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/propagators/concrete/cartesian_fft.md
--rw-r--r--   0 louis      (501) staff       (20)       38 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/propagators/concrete/cartesian_fresnel.md
--rw-r--r--   0 louis      (501) staff       (20)       34 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/propagators/concrete/cartesian_mft.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.602212 dLux-0.9.1/docs/sources/
--rw-r--r--   0 louis      (501) staff       (20)       34 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/sources/array_distribution.md
--rw-r--r--   0 louis      (501) staff       (20)       29 2022-11-06 01:42:52.000000 dLux-0.9.1/docs/sources/binary_source.md
--rw-r--r--   0 louis      (501) staff       (20)       33 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/sources/multi_point_source.md
--rw-r--r--   0 louis      (501) staff       (20)       39 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/sources/point_and_extended_source.md
--rw-r--r--   0 louis      (501) staff       (20)       36 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/sources/point_extended_source.md
--rw-r--r--   0 louis      (501) staff       (20)       28 2022-11-06 01:42:52.000000 dLux-0.9.1/docs/sources/point_source.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.602544 dLux-0.9.1/docs/spectrums/
--rw-r--r--   0 louis      (501) staff       (20)       33 2022-11-06 01:42:52.000000 dLux-0.9.1/docs/spectrums/array_spectrum.md
--rw-r--r--   0 louis      (501) staff       (20)       36 2022-11-06 01:42:52.000000 dLux-0.9.1/docs/spectrums/combined_spectrum.md
--rw-r--r--   0 louis      (501) staff       (20)       38 2022-11-06 01:42:52.000000 dLux-0.9.1/docs/spectrums/polynomial_spectrum.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.592960 dLux-0.9.1/docs/utils/
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.603116 dLux-0.9.1/docs/utils/bayes/
--rw-r--r--   0 louis      (501) staff       (20)       41 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/bayes/calculate_covariance.md
--rw-r--r--   0 louis      (501) staff       (20)       38 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/bayes/calculate_entropy.md
--rw-r--r--   0 louis      (501) staff       (20)       36 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/bayes/chi2_likelihood.md
--rw-r--r--   0 louis      (501) staff       (20)       40 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/bayes/chi2_log_likelihood.md
--rw-r--r--   0 louis      (501) staff       (20)       39 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/bayes/poisson_likelihood.md
--rw-r--r--   0 louis      (501) staff       (20)       43 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/bayes/poisson_log_likelihood.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.603870 dLux-0.9.1/docs/utils/coordinates/
--rw-r--r--   0 louis      (501) staff       (20)       45 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/coordinates/cartesian_to_polar.md
--rw-r--r--   0 louis      (501) staff       (20)       50 2022-11-06 01:42:52.000000 dLux-0.9.1/docs/utils/coordinates/get_coordinates_vector.md
--rw-r--r--   0 louis      (501) staff       (20)       49 2022-11-06 01:42:52.000000 dLux-0.9.1/docs/utils/coordinates/get_pixel_coordinates.md
--rw-r--r--   0 louis      (501) staff       (20)       47 2022-11-06 01:42:52.000000 dLux-0.9.1/docs/utils/coordinates/get_pixel_positions.md
--rw-r--r--   0 louis      (501) staff       (20)       49 2022-11-06 01:42:52.000000 dLux-0.9.1/docs/utils/coordinates/get_polar_coordinates.md
--rw-r--r--   0 louis      (501) staff       (20)       47 2022-11-06 01:42:52.000000 dLux-0.9.1/docs/utils/coordinates/get_polar_positions.md
--rw-r--r--   0 louis      (501) staff       (20)       48 2022-11-06 01:42:52.000000 dLux-0.9.1/docs/utils/coordinates/get_positions_vector.md
--rw-r--r--   0 louis      (501) staff       (20)       45 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/coordinates/polar_to_cartesian.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.604235 dLux-0.9.1/docs/utils/gradient_energy/
--rw-r--r--   0 louis      (501) staff       (20)       37 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/gradient_energy/get_GE.md
--rw-r--r--   0 louis      (501) staff       (20)       38 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/gradient_energy/get_RGE.md
--rw-r--r--   0 louis      (501) staff       (20)       39 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/gradient_energy/get_RWGE.md
--rw-r--r--   0 louis      (501) staff       (20)       46 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/gradient_energy/get_radial_mask.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.604329 dLux-0.9.1/docs/utils/helpers/
--rw-r--r--   0 louis      (501) staff       (20)       41 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/helpers/list_to_dictionary.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.604973 dLux-0.9.1/docs/utils/interpolation/
--rw-r--r--   0 louis      (501) staff       (20)       43 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/interpolation/fourier_rotate.md
--rw-r--r--   0 louis      (501) staff       (20)       49 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/interpolation/generate_coordinates.md
--rw-r--r--   0 louis      (501) staff       (20)       40 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/interpolation/interpolate.md
--rw-r--r--   0 louis      (501) staff       (20)       46 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/interpolation/interpolate_field.md
--rw-r--r--   0 louis      (501) staff       (20)       35 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/interpolation/rotate.md
--rw-r--r--   0 louis      (501) staff       (20)       41 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/interpolation/rotate_field.md
--rw-r--r--   0 louis      (501) staff       (20)       40 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/interpolation/scale_array.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.605175 dLux-0.9.1/docs/utils/models/
--rw-r--r--   0 louis      (501) staff       (20)       43 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/models/simple_optical_system.md
--rw-r--r--   0 louis      (501) staff       (20)       29 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/models/toliman.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.605744 dLux-0.9.1/docs/utils/optics/
--rw-r--r--   0 louis      (501) staff       (20)       42 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/optics/get_airy_pixel_scale.md
--rw-r--r--   0 louis      (501) staff       (20)       37 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/optics/get_fringe_size.md
--rw-r--r--   0 louis      (501) staff       (20)       37 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/optics/get_pixel_scale.md
--rw-r--r--   0 louis      (501) staff       (20)       43 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/optics/get_pixels_per_fringe.md
--rw-r--r--   0 louis      (501) staff       (20)       34 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/optics/opd_to_phase.md
--rw-r--r--   0 louis      (501) staff       (20)       34 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/optics/phase_to_opd.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.605941 dLux-0.9.1/docs/utils/units/
--rw-r--r--   0 louis      (501) staff       (20)       42 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/units/arcseconds_to_radians.md
--rw-r--r--   0 louis      (501) staff       (20)       42 2022-11-08 02:49:52.000000 dLux-0.9.1/docs/utils/units/radians_to_arcseconds.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.606314 dLux-0.9.1/docs/wavefronts/
--rw-r--r--   0 louis      (501) staff       (20)       37 2022-11-06 01:42:52.000000 dLux-0.9.1/docs/wavefronts/angular_wavefront.md
--rw-r--r--   0 louis      (501) staff       (20)       39 2022-11-06 01:42:52.000000 dLux-0.9.1/docs/wavefronts/cartesian_wavefront.md
--rw-r--r--   0 louis      (501) staff       (20)       45 2022-11-06 01:42:52.000000 dLux-0.9.1/docs/wavefronts/far_field_fresnel_wavefront.md
--rw-r--r--   0 louis      (501) staff       (20)       35 2022-11-06 01:42:52.000000 dLux-0.9.1/docs/wavefronts/wavefront.md
--rw-r--r--   0 louis      (501) staff       (20)     6938 2022-11-08 02:49:52.000000 dLux-0.9.1/mkdocs.yml
--rw-r--r--   0 louis      (501) staff       (20)       89 2022-11-08 02:49:52.000000 dLux-0.9.1/requirements.txt
--rw-r--r--   0 louis      (501) staff       (20)       38 2022-11-08 05:12:55.607720 dLux-0.9.1/setup.cfg
--rw-r--r--   0 louis      (501) staff       (20)     1487 2022-11-08 04:44:33.000000 dLux-0.9.1/setup.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-08 05:12:55.607400 dLux-0.9.1/tests/
--rw-r--r--   0 louis      (501) staff       (20)    11915 2022-11-08 02:49:52.000000 dLux-0.9.1/tests/base.py
--rw-r--r--   0 louis      (501) staff       (20)    21925 2022-11-08 02:49:52.000000 dLux-0.9.1/tests/core.py
--rw-r--r--   0 louis      (501) staff       (20)     8220 2022-11-08 02:49:52.000000 dLux-0.9.1/tests/detectors.py
--rw-r--r--   0 louis      (501) staff       (20)     9595 2022-08-10 07:46:26.000000 dLux-0.9.1/tests/integration.py
--rw-r--r--   0 louis      (501) staff       (20)    20463 2022-11-08 02:49:52.000000 dLux-0.9.1/tests/optics.py
--rw-r--r--   0 louis      (501) staff       (20)    20682 2022-11-08 02:49:52.000000 dLux-0.9.1/tests/propagators.py
--rw-r--r--   0 louis      (501) staff       (20)    25863 2022-11-08 02:49:52.000000 dLux-0.9.1/tests/sources.py
--rw-r--r--   0 louis      (501) staff       (20)     8165 2022-11-08 02:49:52.000000 dLux-0.9.1/tests/spectrums.py
--rw-r--r--   0 louis      (501) staff       (20)      536 2022-11-08 02:49:52.000000 dLux-0.9.1/tests/utilities.py
--rw-r--r--   0 louis      (501) staff       (20)      187 2022-11-08 02:49:52.000000 dLux-0.9.1/tests/utils.py
--rw-r--r--   0 louis      (501) staff       (20)    16248 2022-11-08 02:49:52.000000 dLux-0.9.1/tests/wavefronts.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.304215 dLux-0.9.2/
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.282648 dLux-0.9.2/.github/
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.286033 dLux-0.9.2/.github/workflows/
+-rw-r--r--   0 louis      (501) staff       (20)      848 2022-11-06 01:42:52.000000 dLux-0.9.2/.github/workflows/documentation.yml
+-rw-r--r--   0 louis      (501) staff       (20)     1337 2022-11-14 06:31:53.000000 dLux-0.9.2/.github/workflows/tests.yml
+-rw-r--r--   0 louis      (501) staff       (20)      137 2022-11-08 02:49:52.000000 dLux-0.9.2/.gitignore
+-rw-r--r--   0 louis      (501) staff       (20)     5202 2022-07-26 16:35:15.000000 dLux-0.9.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 louis      (501) staff       (20)     1847 2022-11-08 02:49:52.000000 dLux-0.9.2/CONTRIBUTING.md
+-rw-r--r--   0 louis      (501) staff       (20)     1544 2022-05-04 13:56:11.000000 dLux-0.9.2/LICENSE.md
+-rw-r--r--   0 louis      (501) staff       (20)       24 2022-11-08 04:52:54.000000 dLux-0.9.2/MANIFEST.in
+-rw-r--r--   0 louis      (501) staff       (20)      484 2022-11-14 12:23:21.304084 dLux-0.9.2/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)     4365 2022-11-08 02:49:52.000000 dLux-0.9.2/README.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.287066 dLux-0.9.2/dLux/
+-rw-r--r--   0 louis      (501) staff       (20)      896 2022-11-14 12:21:01.000000 dLux-0.9.2/dLux/__init__.py
+-rw-r--r--   0 louis      (501) staff       (20)    58237 2022-11-14 07:11:41.000000 dLux-0.9.2/dLux/core.py
+-rw-r--r--   0 louis      (501) staff       (20)    11789 2022-11-14 06:25:28.000000 dLux-0.9.2/dLux/detectors.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.288521 dLux-0.9.2/dLux/dev/
+-rw-r--r--   0 louis      (501) staff       (20)    24499 2022-11-06 01:42:52.000000 dLux-0.9.2/dLux/dev/FFTfresnel.py
+-rw-r--r--   0 louis      (501) staff       (20)     4400 2022-07-26 16:35:15.000000 dLux-0.9.2/dLux/dev/constants.py
+-rw-r--r--   0 louis      (501) staff       (20)    54752 2022-11-06 01:42:52.000000 dLux-0.9.2/dLux/dev/layers.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.289297 dLux-0.9.2/dLux/dev/tests/
+-rw-r--r--   0 louis      (501) staff       (20)      395 2022-10-05 21:35:52.000000 dLux-0.9.2/dLux/dev/tests/layers.py
+-rw-r--r--   0 louis      (501) staff       (20)       58 2022-07-26 16:35:15.000000 dLux-0.9.2/dLux/dev/tests/source.py
+-rw-r--r--   0 louis      (501) staff       (20)    40325 2022-11-14 06:25:24.000000 dLux-0.9.2/dLux/optics.py
+-rw-r--r--   0 louis      (501) staff       (20)    29840 2022-11-08 02:49:52.000000 dLux-0.9.2/dLux/propagators.py
+-rw-r--r--   0 louis      (501) staff       (20)    33531 2022-11-14 06:25:16.000000 dLux-0.9.2/dLux/sources.py
+-rw-r--r--   0 louis      (501) staff       (20)     9519 2022-11-14 06:25:11.000000 dLux-0.9.2/dLux/spectrums.py
+-rw-r--r--   0 louis      (501) staff       (20)    11774 2022-11-14 06:25:07.000000 dLux-0.9.2/dLux/spiders.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.290518 dLux-0.9.2/dLux/utils/
+-rw-r--r--   0 louis      (501) staff       (20)      799 2022-11-08 02:49:52.000000 dLux-0.9.2/dLux/utils/__init__.py
+-rw-r--r--   0 louis      (501) staff       (20)     6555 2022-11-08 02:49:52.000000 dLux-0.9.2/dLux/utils/bayes.py
+-rw-r--r--   0 louis      (501) staff       (20)     6585 2022-11-08 02:49:52.000000 dLux-0.9.2/dLux/utils/coordinates.py
+-rw-r--r--   0 louis      (501) staff       (20)     2684 2022-11-08 02:49:52.000000 dLux-0.9.2/dLux/utils/gradient_energy.py
+-rw-r--r--   0 louis      (501) staff       (20)     2059 2022-11-08 02:49:52.000000 dLux-0.9.2/dLux/utils/helpers.py
+-rw-r--r--   0 louis      (501) staff       (20)     7053 2022-11-06 01:42:52.000000 dLux-0.9.2/dLux/utils/hexike.py
+-rw-r--r--   0 louis      (501) staff       (20)    11656 2022-11-08 02:49:52.000000 dLux-0.9.2/dLux/utils/interpolation.py
+-rw-r--r--   0 louis      (501) staff       (20)     8457 2022-11-08 02:49:52.000000 dLux-0.9.2/dLux/utils/models.py
+-rw-r--r--   0 louis      (501) staff       (20)     5874 2022-11-09 04:16:33.000000 dLux-0.9.2/dLux/utils/optics.py
+-rw-r--r--   0 louis      (501) staff       (20)     1699 2022-11-06 01:42:52.000000 dLux-0.9.2/dLux/utils/plotting.py
+-rw-r--r--   0 louis      (501) staff       (20)      934 2022-11-08 02:49:52.000000 dLux-0.9.2/dLux/utils/units.py
+-rw-r--r--   0 louis      (501) staff       (20)     8924 2022-11-06 01:42:52.000000 dLux-0.9.2/dLux/utils/zernike.py
+-rw-r--r--   0 louis      (501) staff       (20)    28039 2022-11-14 06:25:02.000000 dLux-0.9.2/dLux/wavefronts.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.287618 dLux-0.9.2/dLux.egg-info/
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.287860 dLux-0.9.2/dLux.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 louis      (501) staff       (20)     4181 2022-11-14 12:17:58.000000 dLux-0.9.2/dLux.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 louis      (501) staff       (20)       81 2022-11-14 12:17:58.000000 dLux-0.9.2/dLux.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-r--r--   0 louis      (501) staff       (20)      484 2022-11-14 12:23:21.000000 dLux-0.9.2/dLux.egg-info/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)     4294 2022-11-14 12:23:21.000000 dLux-0.9.2/dLux.egg-info/SOURCES.txt
+-rw-r--r--   0 louis      (501) staff       (20)        1 2022-11-14 12:23:21.000000 dLux-0.9.2/dLux.egg-info/dependency_links.txt
+-rw-r--r--   0 louis      (501) staff       (20)       81 2022-11-14 12:23:21.000000 dLux-0.9.2/dLux.egg-info/requires.txt
+-rw-r--r--   0 louis      (501) staff       (20)       16 2022-11-14 12:23:21.000000 dLux-0.9.2/dLux.egg-info/top_level.txt
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.290617 dLux-0.9.2/docs/
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.290718 dLux-0.9.2/docs/assets/
+-rw-r--r--   0 louis      (501) staff       (20)   534462 2022-11-06 01:42:52.000000 dLux-0.9.2/docs/assets/logo.jpg
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.291684 dLux-0.9.2/docs/core/
+-rw-r--r--   0 louis      (501) staff       (20)       23 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/core/detector.md
+-rw-r--r--   0 louis      (501) staff       (20)       21 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/core/filter.md
+-rw-r--r--   0 louis      (501) staff       (20)       24 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/core/instrument.md
+-rw-r--r--   0 louis      (501) staff       (20)       20 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/core/model.md
+-rw-r--r--   0 louis      (501) staff       (20)       28 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/core/optical_system.md
+-rw-r--r--   0 louis      (501) staff       (20)       21 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/core/optics.md
+-rw-r--r--   0 louis      (501) staff       (20)       20 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/core/scene.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.292145 dLux-0.9.2/docs/detectors/
+-rw-r--r--   0 louis      (501) staff       (20)       30 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/detectors/add_constant.md
+-rw-r--r--   0 louis      (501) staff       (20)       30 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/detectors/apply_jitter.md
+-rw-r--r--   0 louis      (501) staff       (20)       37 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/detectors/apply_pixel_response.md
+-rw-r--r--   0 louis      (501) staff       (20)       34 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/detectors/apply_saturation.md
+-rw-r--r--   0 louis      (501) staff       (20)       36 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/detectors/integer_downsample.md
+-rw-r--r--   0 louis      (501) staff       (20)     4364 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/index.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.293064 dLux-0.9.2/docs/optics/
+-rw-r--r--   0 louis      (501) staff       (20)       23 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/optics/add_opd.md
+-rw-r--r--   0 louis      (501) staff       (20)       25 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/optics/add_phase.md
+-rw-r--r--   0 louis      (501) staff       (20)       32 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/optics/apply_basis_climb.md
+-rw-r--r--   0 louis      (501) staff       (20)       30 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/optics/apply_basis_opd.md
+-rw-r--r--   0 louis      (501) staff       (20)       33 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/optics/circular_aperture.md
+-rw-r--r--   0 louis      (501) staff       (20)       33 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/optics/compound_aperture.md
+-rw-r--r--   0 louis      (501) staff       (20)       32 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/optics/create_wavefront.md
+-rw-r--r--   0 louis      (501) staff       (20)       35 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/optics/normalise_wavefront.md
+-rw-r--r--   0 louis      (501) staff       (20)       30 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/optics/tilt_wavefront.md
+-rw-r--r--   0 louis      (501) staff       (20)       34 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/optics/transmissive_optic.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.283350 dLux-0.9.2/docs/propagators/
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.293633 dLux-0.9.2/docs/propagators/abstract/
+-rw-r--r--   0 louis      (501) staff       (20)       38 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/propagators/abstract/angular_propagator.md
+-rw-r--r--   0 louis      (501) staff       (20)       40 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/propagators/abstract/cartesian_propagator.md
+-rw-r--r--   0 louis      (501) staff       (20)       36 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/propagators/abstract/far_field_fresnel.md
+-rw-r--r--   0 louis      (501) staff       (20)       45 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/propagators/abstract/fixed_sampling_propagator.md
+-rw-r--r--   0 louis      (501) staff       (20)       32 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/propagators/abstract/propagator.md
+-rw-r--r--   0 louis      (501) staff       (20)       48 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/propagators/abstract/variable_sampling_propagator.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.294101 dLux-0.9.2/docs/propagators/concrete/
+-rw-r--r--   0 louis      (501) staff       (20)       32 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/propagators/concrete/angular_fft.md
+-rw-r--r--   0 louis      (501) staff       (20)       32 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/propagators/concrete/angular_mft.md
+-rw-r--r--   0 louis      (501) staff       (20)       34 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/propagators/concrete/cartesian_fft.md
+-rw-r--r--   0 louis      (501) staff       (20)       38 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/propagators/concrete/cartesian_fresnel.md
+-rw-r--r--   0 louis      (501) staff       (20)       34 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/propagators/concrete/cartesian_mft.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.294660 dLux-0.9.2/docs/sources/
+-rw-r--r--   0 louis      (501) staff       (20)       34 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/sources/array_distribution.md
+-rw-r--r--   0 louis      (501) staff       (20)       29 2022-11-06 01:42:52.000000 dLux-0.9.2/docs/sources/binary_source.md
+-rw-r--r--   0 louis      (501) staff       (20)       33 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/sources/multi_point_source.md
+-rw-r--r--   0 louis      (501) staff       (20)       39 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/sources/point_and_extended_source.md
+-rw-r--r--   0 louis      (501) staff       (20)       36 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/sources/point_extended_source.md
+-rw-r--r--   0 louis      (501) staff       (20)       28 2022-11-06 01:42:52.000000 dLux-0.9.2/docs/sources/point_source.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.294950 dLux-0.9.2/docs/spectrums/
+-rw-r--r--   0 louis      (501) staff       (20)       33 2022-11-06 01:42:52.000000 dLux-0.9.2/docs/spectrums/array_spectrum.md
+-rw-r--r--   0 louis      (501) staff       (20)       36 2022-11-06 01:42:52.000000 dLux-0.9.2/docs/spectrums/combined_spectrum.md
+-rw-r--r--   0 louis      (501) staff       (20)       38 2022-11-06 01:42:52.000000 dLux-0.9.2/docs/spectrums/polynomial_spectrum.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.283898 dLux-0.9.2/docs/utils/
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.295519 dLux-0.9.2/docs/utils/bayes/
+-rw-r--r--   0 louis      (501) staff       (20)       41 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/bayes/calculate_covariance.md
+-rw-r--r--   0 louis      (501) staff       (20)       38 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/bayes/calculate_entropy.md
+-rw-r--r--   0 louis      (501) staff       (20)       36 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/bayes/chi2_likelihood.md
+-rw-r--r--   0 louis      (501) staff       (20)       40 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/bayes/chi2_log_likelihood.md
+-rw-r--r--   0 louis      (501) staff       (20)       39 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/bayes/poisson_likelihood.md
+-rw-r--r--   0 louis      (501) staff       (20)       43 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/bayes/poisson_log_likelihood.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.296293 dLux-0.9.2/docs/utils/coordinates/
+-rw-r--r--   0 louis      (501) staff       (20)       45 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/coordinates/cartesian_to_polar.md
+-rw-r--r--   0 louis      (501) staff       (20)       50 2022-11-06 01:42:52.000000 dLux-0.9.2/docs/utils/coordinates/get_coordinates_vector.md
+-rw-r--r--   0 louis      (501) staff       (20)       49 2022-11-06 01:42:52.000000 dLux-0.9.2/docs/utils/coordinates/get_pixel_coordinates.md
+-rw-r--r--   0 louis      (501) staff       (20)       47 2022-11-06 01:42:52.000000 dLux-0.9.2/docs/utils/coordinates/get_pixel_positions.md
+-rw-r--r--   0 louis      (501) staff       (20)       49 2022-11-06 01:42:52.000000 dLux-0.9.2/docs/utils/coordinates/get_polar_coordinates.md
+-rw-r--r--   0 louis      (501) staff       (20)       47 2022-11-06 01:42:52.000000 dLux-0.9.2/docs/utils/coordinates/get_polar_positions.md
+-rw-r--r--   0 louis      (501) staff       (20)       48 2022-11-06 01:42:52.000000 dLux-0.9.2/docs/utils/coordinates/get_positions_vector.md
+-rw-r--r--   0 louis      (501) staff       (20)       45 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/coordinates/polar_to_cartesian.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.296674 dLux-0.9.2/docs/utils/gradient_energy/
+-rw-r--r--   0 louis      (501) staff       (20)       37 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/gradient_energy/get_GE.md
+-rw-r--r--   0 louis      (501) staff       (20)       38 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/gradient_energy/get_RGE.md
+-rw-r--r--   0 louis      (501) staff       (20)       39 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/gradient_energy/get_RWGE.md
+-rw-r--r--   0 louis      (501) staff       (20)       46 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/gradient_energy/get_radial_mask.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.296776 dLux-0.9.2/docs/utils/helpers/
+-rw-r--r--   0 louis      (501) staff       (20)       41 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/helpers/list_to_dictionary.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.297451 dLux-0.9.2/docs/utils/interpolation/
+-rw-r--r--   0 louis      (501) staff       (20)       43 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/interpolation/fourier_rotate.md
+-rw-r--r--   0 louis      (501) staff       (20)       49 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/interpolation/generate_coordinates.md
+-rw-r--r--   0 louis      (501) staff       (20)       40 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/interpolation/interpolate.md
+-rw-r--r--   0 louis      (501) staff       (20)       46 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/interpolation/interpolate_field.md
+-rw-r--r--   0 louis      (501) staff       (20)       35 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/interpolation/rotate.md
+-rw-r--r--   0 louis      (501) staff       (20)       41 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/interpolation/rotate_field.md
+-rw-r--r--   0 louis      (501) staff       (20)       40 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/interpolation/scale_array.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.301399 dLux-0.9.2/docs/utils/models/
+-rw-r--r--   0 louis      (501) staff       (20)       43 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/models/simple_optical_system.md
+-rw-r--r--   0 louis      (501) staff       (20)       29 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/models/toliman.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.302035 dLux-0.9.2/docs/utils/optics/
+-rw-r--r--   0 louis      (501) staff       (20)       42 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/optics/get_airy_pixel_scale.md
+-rw-r--r--   0 louis      (501) staff       (20)       37 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/optics/get_fringe_size.md
+-rw-r--r--   0 louis      (501) staff       (20)       37 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/optics/get_pixel_scale.md
+-rw-r--r--   0 louis      (501) staff       (20)       43 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/optics/get_pixels_per_fringe.md
+-rw-r--r--   0 louis      (501) staff       (20)       34 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/optics/opd_to_phase.md
+-rw-r--r--   0 louis      (501) staff       (20)       34 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/optics/phase_to_opd.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.302239 dLux-0.9.2/docs/utils/units/
+-rw-r--r--   0 louis      (501) staff       (20)       42 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/units/arcseconds_to_radians.md
+-rw-r--r--   0 louis      (501) staff       (20)       42 2022-11-08 02:49:52.000000 dLux-0.9.2/docs/utils/units/radians_to_arcseconds.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.302623 dLux-0.9.2/docs/wavefronts/
+-rw-r--r--   0 louis      (501) staff       (20)       37 2022-11-06 01:42:52.000000 dLux-0.9.2/docs/wavefronts/angular_wavefront.md
+-rw-r--r--   0 louis      (501) staff       (20)       39 2022-11-06 01:42:52.000000 dLux-0.9.2/docs/wavefronts/cartesian_wavefront.md
+-rw-r--r--   0 louis      (501) staff       (20)       45 2022-11-06 01:42:52.000000 dLux-0.9.2/docs/wavefronts/far_field_fresnel_wavefront.md
+-rw-r--r--   0 louis      (501) staff       (20)       35 2022-11-06 01:42:52.000000 dLux-0.9.2/docs/wavefronts/wavefront.md
+-rw-r--r--   0 louis      (501) staff       (20)     6995 2022-11-14 06:53:08.000000 dLux-0.9.2/mkdocs.yml
+-rw-r--r--   0 louis      (501) staff       (20)       96 2022-11-14 06:25:47.000000 dLux-0.9.2/requirements.txt
+-rw-r--r--   0 louis      (501) staff       (20)       38 2022-11-14 12:23:21.304253 dLux-0.9.2/setup.cfg
+-rw-r--r--   0 louis      (501) staff       (20)     1487 2022-11-08 04:44:33.000000 dLux-0.9.2/setup.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2022-11-14 12:23:21.303909 dLux-0.9.2/tests/
+-rw-r--r--   0 louis      (501) staff       (20)    21925 2022-11-08 02:49:52.000000 dLux-0.9.2/tests/core.py
+-rw-r--r--   0 louis      (501) staff       (20)     8220 2022-11-08 02:49:52.000000 dLux-0.9.2/tests/detectors.py
+-rw-r--r--   0 louis      (501) staff       (20)     9595 2022-08-10 07:46:26.000000 dLux-0.9.2/tests/integration.py
+-rw-r--r--   0 louis      (501) staff       (20)    20463 2022-11-08 02:49:52.000000 dLux-0.9.2/tests/optics.py
+-rw-r--r--   0 louis      (501) staff       (20)    20682 2022-11-08 02:49:52.000000 dLux-0.9.2/tests/propagators.py
+-rw-r--r--   0 louis      (501) staff       (20)    25863 2022-11-08 02:49:52.000000 dLux-0.9.2/tests/sources.py
+-rw-r--r--   0 louis      (501) staff       (20)     8165 2022-11-08 02:49:52.000000 dLux-0.9.2/tests/spectrums.py
+-rw-r--r--   0 louis      (501) staff       (20)      536 2022-11-08 02:49:52.000000 dLux-0.9.2/tests/utilities.py
+-rw-r--r--   0 louis      (501) staff       (20)      187 2022-11-08 02:49:52.000000 dLux-0.9.2/tests/utils.py
+-rw-r--r--   0 louis      (501) staff       (20)    16248 2022-11-08 02:49:52.000000 dLux-0.9.2/tests/wavefronts.py
```

### Comparing `dLux-0.9.1/.github/workflows/documentation.yml` & `dLux-0.9.2/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/.github/workflows/tests.yml` & `dLux-0.9.2/.github/workflows/tests.yml`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
         run: |
           python -m pip install --upgrade pip
           pip install --quiet pytest
           pip install --quiet -r requirements.txt
           pip install --quiet .
 
       # ===== Tests =====
-      - name: base tests
-        run: pytest --quiet tests/base.py
+      # - name: base tests
+      #   run: pytest --quiet tests/base.py
 
       - name: core tests
         run: pytest --quiet tests/core.py
 
       - name: spectrum tests
         run: pytest --quiet tests/spectrums.py
```

### Comparing `dLux-0.9.1/CODE_OF_CONDUCT.md` & `dLux-0.9.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/CONTRIBUTING.md` & `dLux-0.9.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/LICENSE.md` & `dLux-0.9.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/README.md` & `dLux-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/dLux/__init__.py` & `dLux-0.9.2/dLux/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 name = "dLux"
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 # Import as modules
-from . import base
 from . import core
 from . import detectors
 from . import optics
 from . import wavefronts
 from . import propagators
 from . import utils
 from . import sources
 from . import spectrums
 
 # Import core functions from modules
-from .base        import *
 from .core        import *
 from .detectors   import *
 from .optics      import *
 from .wavefronts  import *
 from .propagators import *
 from .sources     import *
 from .spectrums   import *
```

### Comparing `dLux-0.9.1/dLux/core.py` & `dLux-0.9.2/dLux/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 import jax.numpy as np
 from jax import vmap
 from jax.tree_util import tree_map, tree_flatten
 from jax.scipy.ndimage import map_coordinates
 from equinox import tree_at, static_field
+from zodiax import ExtendedBase
 from collections import OrderedDict
 from copy import deepcopy
 from functools import partial
 import dLux
 
 
 __all__ = ["model", "OpticalSystem", "Instrument", "Optics", "Scene",
@@ -170,15 +171,15 @@
         # Apply detector
         image = detector.apply_detector(psf) if detector is not None else psf
 
         # Flatten
         return image.flatten() if flatten else image
 
 
-class Instrument(dLux.base.ExtendedBase):
+class Instrument(ExtendedBase):
     """
     A high level class desgined to model the behaviour of a telescope. It
     stores a series different ∂Lux objects, and primarily passes the relevant
     information between these objects in order to coherently model some
     telescope observation.
 
     Attributes
@@ -406,22 +407,21 @@
             The key of the item to be searched for in the sub-dictionaries.
 
         Returns
         -------
         item : object
             The item corresponding to the supplied key in the sub-dictionaries.
         """
-
-        if self.optics is not None and hasattr(self.optics, 'layers') and \
+        if 'optics' in vars(self) and hasattr(self.optics, 'layers') and \
                                         key in self.optics.layers.keys():
             return self.optics.layers[key]
-        elif self.detector is not None and hasattr(self.detector, 'layers') and\
+        elif 'detector' in vars(self) and hasattr(self.detector, 'layers') and \
                                         key in self.detector.layers.keys():
             return self.detector.layers[key]
-        elif self.scene is not None and hasattr(self.scene, 'sources') and \
+        elif 'scene' in vars(self) and hasattr(self.scene, 'sources') and \
                                         key in self.scene.sources.keys():
             return self.scene.sources[key]
         else:
             raise AttributeError("'{}' object has no attribute '{}'"\
                                  .format(type(self), key))
 
 
@@ -477,29 +477,33 @@
         -------
         image : Array, Pytree
             The image of the scene modelled through the optics with detector and
             filter effects applied if they are supplied. Returns either as a
             single array (if return_tree is false), or a pytree like object
             with matching tree strucutre as the input scene/sources/source.
         """
-        optics = optics if 'optics' in kwargs else self.optics
+        if 'optics' in kwargs:
+            optics = kwargs['optics']
+            kwargs.pop('optics')
+        else:
+            optics = self.optics
         kwargs['detector'] = self.detector if 'detector' not in kwargs \
                                                         else kwargs['detector']
         kwargs['filter']   = self.filter   if 'filter'   not in kwargs \
                                                         else kwargs['filter']
         if 'scene' not in kwargs and \
            'source' not in kwargs and \
            'sources' not in kwargs:
             kwargs['scene'] = self.scene
 
         return model(optics,
                      **kwargs)
 
 
-class Optics(dLux.base.ExtendedBase):
+class Optics(ExtendedBase):
     """
     A high level class desgined to model the behaviour of some optical systems
     response to wavefronts.
 
     Attributes
     ----------
     layers: dict
@@ -542,15 +546,15 @@
             The key of the item to be searched for in the layers dictionary.
 
         Returns
         -------
         item : object
             The item corresponding to the supplied key in the layers dictionary.
         """
-        if key in self.layers.keys():
+        if 'layers' in vars(self) and key in self.layers.keys():
             return self.layers[key]
         else:
             raise AttributeError("'{}' object has no attribute '{}'"\
                                  .format(type(self), key))
 
 
     def propagate_mono(self       : Optics,
@@ -755,15 +759,15 @@
             filter effects applied if they are supplied. Returns either as a
             single array (if return_tree is false), or a pytree like object
             with matching tree strucutre as the input scene/sources/source.
         """
         return model(self, **kwargs)
 
 
-class Scene(dLux.base.ExtendedBase):
+class Scene(ExtendedBase):
     """
     A high level class representing some 'astrophysical scene', which is
     composed of dLux.sources.Sources.
 
     Attributes
     ----------
     sources : dict
@@ -806,15 +810,15 @@
 
         Returns
         -------
         item : object
             The item corresponding to the supplied key in the sources
             dictionary.
         """
-        if key in self.sources.keys():
+        if 'sources' in vars(self) and key in self.sources.keys():
             return self.sources[key]
         else:
             raise AttributeError("'{}' object has no attribute '{}'"\
                                  .format(type(self), key))
 
 
     def normalise(self : Scene) -> Scene:
@@ -871,15 +875,15 @@
             filter effects applied if they are supplied. Returns either as a
             single array (if return_tree is false), or a pytree like object
             with matching tree strucutre as the input scene/sources/source.
         """
         return model(optics, scene=self, **kwargs)
 
 
-class Detector(dLux.base.ExtendedBase):
+class Detector(ExtendedBase):
     """
     A high level class desgined to model the behaviour of some detectors
     response to some psf.
 
     Attributes
     ----------
     layers: dict
@@ -924,15 +928,15 @@
             The key of the item to be searched for in the layers dictionary.
 
         Returns
         -------
         item : object
             The item corresponding to the supplied key in the layers dictionary.
         """
-        if key in self.layers.keys():
+        if 'layers' in vars(self) and key in self.layers.keys():
             return self.layers[key]
         else:
             raise AttributeError("'{}' object has no attribute '{}'"\
                                  .format(type(self), key))
 
 
     def apply_detector(self  : Instrument,
@@ -1031,15 +1035,15 @@
             filter effects applied if they are supplied. Returns either as a
             single array (if return_tree is false), or a pytree like object
             with matching tree strucutre as the input scene/sources/source.
         """
         return model(optics, detector=self, **kwargs)
 
 
-class Filter(dLux.base.ExtendedBase):
+class Filter(ExtendedBase):
     """
     A class for modelling optical filters.
 
     Attributes
     ----------
     wavelengths : Array
         The wavelengths at which the filter is defined.
@@ -1213,15 +1217,15 @@
             with matching tree strucutre as the input scene/sources/source.
         """
         return model(optics, filter=self, **kwargs)
 
 
 
 """Legacy code"""
-class OpticalSystem(dLux.base.ExtendedBase):
+class OpticalSystem(ExtendedBase):
     """ Optical System class, Equinox Modle
     
     DOCSTRING NOT COMPLETE
     
     A Class to store and apply properties external to the optical system
     Ie: stellar positions and spectra
```

### Comparing `dLux-0.9.1/dLux/detectors.py` & `dLux-0.9.2/dLux/detectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from __future__ import annotations
 import jax.numpy as np
 from abc import ABC, abstractmethod
 from jax.scipy.signal import convolve
 from jax.scipy.stats import norm
 from equinox import tree_at, static_field
+from zodiax import ExtendedBase
 import dLux
 from dLux.utils.interpolation import rotate, fourier_rotate
 
 
 
 __all__ = ["ApplyPixelResponse", "ApplyJitter", "ApplySaturation",
            "AddConstant", "IntegerDownsample", "Rotate"]
 
 
 Array = np.ndarray
 
 
-class DetectorLayer(dLux.base.ExtendedBase, ABC):
+class DetectorLayer(ExtendedBase, ABC):
     """
     A base Detector layer class to help with type checking throuhgout the rest
     of the software.
 
     Attributes
     ----------
     name : str
```

### Comparing `dLux-0.9.1/dLux/dev/FFTfresnel.py` & `dLux-0.9.2/dLux/dev/FFTfresnel.py`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/dLux/dev/constants.py` & `dLux-0.9.2/dLux/dev/constants.py`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/dLux/dev/layers.py` & `dLux-0.9.2/dLux/dev/layers.py`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/dLux/optics.py` & `dLux-0.9.2/dLux/optics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from __future__ import annotations
 import jax.numpy as np
 from jax import vmap
 from jax.scipy.ndimage import map_coordinates
 from jax.tree_util import tree_map
 from jax.lax import stop_gradient
 from equinox import tree_at, static_field
+from zodiax import ExtendedBase
 from abc import ABC, abstractmethod
 from inspect import signature
 import dLux
 
 
 __all__ = ["CreateWavefront", "TiltWavefront", "CircularAperture",
            "NormaliseWavefront", "ApplyBasisOPD", "AddPhase", "AddOPD",
            "TransmissiveOptic", "CompoundAperture", "ApplyBasisCLIMB",
            "Rotate"]
 
 
 Array = np.ndarray
 
 
-class OpticalLayer(dLux.base.ExtendedBase, ABC):
+class OpticalLayer(ExtendedBase, ABC):
     """
     A base Optical layer class to help with type checking throuhgout the rest
     of the software. Instantiates the apply method which inspects the function
     signature of the __call__ method in order to only pass and return the
     parameters dictionary if it is needed and modified.
 
     Attributes
```

### Comparing `dLux-0.9.1/dLux/propagators.py` & `dLux-0.9.2/dLux/propagators.py`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/dLux/sources.py` & `dLux-0.9.2/dLux/sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from __future__ import annotations
 import jax.numpy as np
 from jax.scipy.signal import convolve
 from jax import vmap
 from equinox import tree_at, static_field
+from zodiax import ExtendedBase
 from abc import ABC, abstractmethod
 import dLux
 
 
 __all__ = ["PointSource", "MultiPointSource", "ArrayDistribution",
            "BinarySource", "PointExtendedSource", "PointAndExtendedSource"]
 
 
 Array = np.ndarray
 
 
 ########################
 ### Abstract Classes ###
 ########################
-class Source(dLux.base.ExtendedBase, ABC):
+class Source(ExtendedBase, ABC):
     """
     Base class for source objects. The idea of these source classes is to allow
     an arbitrary parametrisation of the underlying astrophyical objects. Each
     source object requires a normalise(), format_inputs(), and model() methods,
     along with the regular getter and setter methods.
 
     The normalise() method should return a new instance of the class with all
```

### Comparing `dLux-0.9.1/dLux/spectrums.py` & `dLux-0.9.2/dLux/spectrums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from __future__ import annotations
 from abc import ABC, abstractmethod
 import jax.numpy as np
 from equinox import tree_at
+from zodiax import ExtendedBase
 from jax import vmap
 import dLux
 
 
 __all__ = ["ArraySpectrum", "PolynomialSpectrum", "CombinedSpectrum"]
 
 
 Array = np.ndarray
 
 
-class Spectrum(dLux.base.ExtendedBase, ABC):
+class Spectrum(ExtendedBase, ABC):
     """
     Abstract base class for arbitrary spectral parametrisations.
 
     Attributes
     ----------
     wavelengths : Array, meters
         The array of wavelengths at which the spectrum is defined.
```

### Comparing `dLux-0.9.1/dLux/spiders.py` & `dLux-0.9.2/dLux/spiders.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 import abc 
 import jax
 import typing
 import equinox
 import functools
 import dLux
 import dLux.utils
-import jax.numpy as np 
+import jax.numpy as np
 import matplotlib.pyplot as pyplot
+from zodiax import ExtendedBase
 
 
 Layer = typing.TypeVar("Layer")
 
 
-class Spider(dLux.base.ExtendedBase, abc.ABC):
+class Spider(ExtendedBase, abc.ABC):
     """
     An abstraction on the concept of an optical spider for a space telescope.
     These are the things that hold up the secondary mirrors. For example,
 
     Parameters
     ----------
     number_of_pixels: int
```

### Comparing `dLux-0.9.1/dLux/utils/__init__.py` & `dLux-0.9.2/dLux/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/dLux/utils/bayes.py` & `dLux-0.9.2/dLux/utils/bayes.py`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/dLux/utils/coordinates.py` & `dLux-0.9.2/dLux/utils/coordinates.py`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/dLux/utils/gradient_energy.py` & `dLux-0.9.2/dLux/utils/gradient_energy.py`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/dLux/utils/helpers.py` & `dLux-0.9.2/dLux/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/dLux/utils/hexike.py` & `dLux-0.9.2/dLux/utils/hexike.py`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/dLux/utils/interpolation.py` & `dLux-0.9.2/dLux/utils/interpolation.py`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/dLux/utils/models.py` & `dLux-0.9.2/dLux/utils/models.py`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/dLux/utils/optics.py` & `dLux-0.9.2/dLux/utils/optics.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,16 @@
     at the given sampling rate.
 
     Parameters
     ----------
     sampling_rate : Array
         The rate at which to sample the diffraction fringes. A value of 2 will
         give nyquist sampled pixels.
+    wavelength : Array, meters
+        The observation wavelength.
     aperture : Array, meters
         The size of the aperture.
     focal_length : Array = None
         The focal length of the optical system. If none is provided, the pixel
         scale is given in units of radians per pixel, else it is given in
         meters per pixel.
```

### Comparing `dLux-0.9.1/dLux/utils/plotting.py` & `dLux-0.9.2/dLux/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/dLux/utils/units.py` & `dLux-0.9.2/dLux/utils/units.py`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/dLux/utils/zernike.py` & `dLux-0.9.2/dLux/utils/zernike.py`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/dLux/wavefronts.py` & `dLux-0.9.2/dLux/wavefronts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 import jax.numpy as np
 from jax import vmap
 from equinox import tree_at
+from zodiax import ExtendedBase
 from enum import IntEnum
 from abc import ABC
 from dLux.utils.coordinates import get_pixel_coordinates
 from dLux.utils.interpolation import interpolate_field, rotate_field
 import dLux
 
 __all__ = ["PlaneType", "CartesianWavefront", "AngularWavefront",
@@ -24,15 +25,15 @@
     Intermediate. This will be done with the Near-Field Fresnel implementation.
     """
     Pupil = 1
     Focal = 2
     Intermediate = 3
 
 
-class Wavefront(dLux.base.ExtendedBase, ABC):
+class Wavefront(ExtendedBase, ABC):
     """
     A class representing some wavefront, designed to track the various
     parameters such as wavelength, pixel_scale, amplitude and phase, as well as
     a helper parmeter, plane_type.
 
     All wavefronts currently only support square amplitude and phase arrays.
```

### Comparing `dLux-0.9.1/dLux.egg-info/SOURCES.txt` & `dLux-0.9.2/dLux.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 README.md
 mkdocs.yml
 requirements.txt
 setup.py
 .github/workflows/documentation.yml
 .github/workflows/tests.yml
 dLux/__init__.py
-dLux/base.py
 dLux/core.py
 dLux/detectors.py
 dLux/optics.py
 dLux/propagators.py
 dLux/sources.py
 dLux/spectrums.py
 dLux/spiders.py
@@ -37,16 +36,16 @@
 dLux/utils/hexike.py
 dLux/utils/interpolation.py
 dLux/utils/models.py
 dLux/utils/optics.py
 dLux/utils/plotting.py
 dLux/utils/units.py
 dLux/utils/zernike.py
+docs/index.md
 docs/assets/logo.jpg
-docs/base/base.md
 docs/core/detector.md
 docs/core/filter.md
 docs/core/instrument.md
 docs/core/model.md
 docs/core/optical_system.md
 docs/core/optics.md
 docs/core/scene.md
@@ -121,15 +120,14 @@
 docs/utils/optics/phase_to_opd.md
 docs/utils/units/arcseconds_to_radians.md
 docs/utils/units/radians_to_arcseconds.md
 docs/wavefronts/angular_wavefront.md
 docs/wavefronts/cartesian_wavefront.md
 docs/wavefronts/far_field_fresnel_wavefront.md
 docs/wavefronts/wavefront.md
-tests/base.py
 tests/core.py
 tests/detectors.py
 tests/integration.py
 tests/optics.py
 tests/propagators.py
 tests/sources.py
 tests/spectrums.py
```

### Comparing `dLux-0.9.1/docs/assets/logo.jpg` & `dLux-0.9.2/docs/assets/logo.jpg`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/mkdocs.yml` & `dLux-0.9.2/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -44,23 +44,24 @@
             show_if_no_docstring: yes
       custom_templates: templates
 
 # ===== Navigation =====
 nav:
     - Home: index.md
     - Tutorials:
-        - Interfacing with PyTrees: notebooks/PyTree_interface.ipynb
+        # - Interfacing with PyTrees: notebooks/PyTree_interface.ipynb
         - Phase Retrieval:          notebooks/phase_retrieval_demo.ipynb
         - Phase Mask Design:        notebooks/designing_a_mask.ipynb
         - Pixel Level Calibration:  notebooks/flatfield_calibration.ipynb
         - Fisher Information:       notebooks/fisher_information.ipynb
         - Parameter Inference:      notebooks/HMC.ipynb
 
-    - Base:
-        - Base:      base/base.md
+    # - Base:
+    #     - Base:         base/base.md
+    #     - ExtendedBase: base/extended_base.md
 
     - Core:
         - Telescope: core/instrument.md
         - Optics:    core/optics.md
         - Scene:     core/scene.md
         - Detector:  core/detector.md
         - Filter:    core/filter.md
```

### Comparing `dLux-0.9.1/setup.py` & `dLux-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/tests/core.py` & `dLux-0.9.2/tests/core.py`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/tests/detectors.py` & `dLux-0.9.2/tests/detectors.py`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/tests/integration.py` & `dLux-0.9.2/tests/integration.py`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/tests/optics.py` & `dLux-0.9.2/tests/optics.py`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/tests/propagators.py` & `dLux-0.9.2/tests/propagators.py`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/tests/sources.py` & `dLux-0.9.2/tests/sources.py`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/tests/spectrums.py` & `dLux-0.9.2/tests/spectrums.py`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/tests/utilities.py` & `dLux-0.9.2/tests/utilities.py`

 * *Files identical despite different names*

### Comparing `dLux-0.9.1/tests/wavefronts.py` & `dLux-0.9.2/tests/wavefronts.py`

 * *Files identical despite different names*

