# Comparing `tmp/v_quantum_annealing-0.0.0.tar.gz` & `tmp/v_quantum_annealing-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "v_quantum_annealing-0.0.0.tar", last modified: Sun May 28 13:28:24 2023, max compression
+gzip compressed data, was "v_quantum_annealing-0.0.1.tar", last modified: Sun May 28 17:52:31 2023, max compression
```

## Comparing `v_quantum_annealing-0.0.0.tar` & `v_quantum_annealing-0.0.1.tar`

### file list

```diff
@@ -1,119 +1,187 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 13:28:24.953229 v_quantum_annealing-0.0.0/
--rw-rw-rw-   0        0        0     8738 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.0/CMakeLists.txt
--rw-rw-rw-   0        0        0       72 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.0/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    11560 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.0/LICENSE
--rw-rw-rw-   0        0        0     1289 2023-05-27 18:46:55.000000 v_quantum_annealing-0.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0    12457 2023-05-28 13:28:24.954226 v_quantum_annealing-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     9292 2023-05-27 18:59:08.000000 v_quantum_annealing-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 13:28:24.377343 v_quantum_annealing-0.0.0/cmake/
--rw-rw-rw-   0        0        0     5390 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.0/cmake/FindGcov.cmake
--rw-rw-rw-   0        0        0    13074 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.0/cmake/FindLcov.cmake
--rw-rw-rw-   0        0        0     9299 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.0/cmake/Findcodecov.cmake
--rw-rw-rw-   0        0        0     4712 2023-05-27 18:59:08.000000 v_quantum_annealing-0.0.0/cmake/GenerateDocs.cmake
--rw-rw-rw-   0        0        0     2000 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.0/cmake/PythonAutoDetectOSX.cmake
--rw-rw-rw-   0        0        0     1129 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.0/cmake/llvm-cov-wrapper
--rw-rw-rw-   0        0        0     1222 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.0/doc-requirements.in
-drwxrwxrwx   0        0        0        0 2023-05-28 13:28:24.428207 v_quantum_annealing-0.0.0/external/
--rw-rw-rw-   0        0        0     1002 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/external/cimod.cmake
--rw-rw-rw-   0        0        0     1704 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/external/eigen.cmake
--rw-rw-rw-   0        0        0      724 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.0/external/googletest.cmake
--rw-rw-rw-   0        0        0      781 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.0/external/json.cmake
--rw-rw-rw-   0        0        0      465 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.0/external/pybind11-json.cmake
-drwxrwxrwx   0        0        0        0 2023-05-28 13:28:24.438179 v_quantum_annealing-0.0.0/include/
--rw-rw-rw-   0        0        0     2163 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.0/include/CMakeLists.txt
--rw-rw-rw-   0        0        0     4646 2023-05-27 18:46:58.000000 v_quantum_annealing-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     1540 2023-05-28 13:28:24.957221 v_quantum_annealing-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1270 2023-05-27 19:26:39.000000 v_quantum_annealing-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 13:28:24.525011 v_quantum_annealing-0.0.0/tests/
--rw-rw-rw-   0        0        0     1756 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.0/tests/CMakeLists.txt
--rw-rw-rw-   0        0        0        0 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 13:28:24.548947 v_quantum_annealing-0.0.0/tests/__pycache__/
--rw-rw-rw-   0        0        0      127 2023-05-23 08:09:01.000000 v_quantum_annealing-0.0.0/tests/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    13004 2023-05-23 08:09:01.000000 v_quantum_annealing-0.0.0/tests/__pycache__/test_cxx.cpython-39-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0      127 2023-05-23 08:09:01.000000 v_quantum_annealing-0.0.0/tests/__pycache__/test_gpu.cpython-39-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0    34580 2023-05-23 08:09:01.000000 v_quantum_annealing-0.0.0/tests/__pycache__/test_hubo.cpython-39-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0     5551 2023-05-23 08:09:02.000000 v_quantum_annealing-0.0.0/tests/__pycache__/test_model.cpython-39-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0     8200 2023-05-23 08:09:02.000000 v_quantum_annealing-0.0.0/tests/__pycache__/test_sampler.cpython-39-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0     1848 2023-05-23 08:09:03.000000 v_quantum_annealing-0.0.0/tests/__pycache__/test_sqa.cpython-39-pytest-7.3.1.pyc
--rw-rw-rw-   0        0        0     2147 2023-05-23 08:09:03.000000 v_quantum_annealing-0.0.0/tests/__pycache__/test_utils.cpython-39-pytest-7.3.1.pyc
-drwxrwxrwx   0        0        0        0 2023-05-28 13:28:24.579863 v_quantum_annealing-0.0.0/tests/cxxtest/
--rw-rw-rw-   0        0        0     1944 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/tests/cxxtest/cxxtest.cpp
-drwxrwxrwx   0        0        0        0 2023-05-28 13:28:24.627736 v_quantum_annealing-0.0.0/tests/cxxtest/graph/
--rw-rw-rw-   0        0        0      774 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.0/tests/cxxtest/graph/all.hpp
--rw-rw-rw-   0        0        0     6099 2023-05-27 18:38:59.000000 v_quantum_annealing-0.0.0/tests/cxxtest/graph/binary_polynomial_model.hpp
--rw-rw-rw-   0        0        0     5882 2023-05-27 18:39:02.000000 v_quantum_annealing-0.0.0/tests/cxxtest/graph/ising_polynomial_model.hpp
--rw-rw-rw-   0        0        0     4569 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/tests/cxxtest/graph/polynomial.hpp
--rw-rw-rw-   0        0        0     7048 2023-05-27 18:39:20.000000 v_quantum_annealing-0.0.0/tests/cxxtest/graph/quadratic.hpp
--rw-rw-rw-   0        0        0    38994 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/tests/cxxtest/polynomial_test.hpp
-drwxrwxrwx   0        0        0        0 2023-05-28 13:28:24.647047 v_quantum_annealing-0.0.0/tests/cxxtest/result/
--rw-rw-rw-   0        0        0      665 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.0/tests/cxxtest/result/all.hpp
--rw-rw-rw-   0        0        0     2742 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/tests/cxxtest/result/result.hpp
-drwxrwxrwx   0        0        0        0 2023-05-28 13:28:24.738801 v_quantum_annealing-0.0.0/tests/cxxtest/sampler/
--rw-rw-rw-   0        0        0      856 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.0/tests/cxxtest/sampler/all.hpp
--rw-rw-rw-   0        0        0     2406 2023-05-27 18:39:25.000000 v_quantum_annealing-0.0.0/tests/cxxtest/sampler/binary_polynomial_sa_sampler.hpp
--rw-rw-rw-   0        0        0     3165 2023-05-27 18:39:29.000000 v_quantum_annealing-0.0.0/tests/cxxtest/sampler/gpu.hpp
--rw-rw-rw-   0        0        0     2394 2023-05-27 18:39:31.000000 v_quantum_annealing-0.0.0/tests/cxxtest/sampler/ising_polynomial_sa_sampler.hpp
--rw-rw-rw-   0        0        0     4278 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/tests/cxxtest/sampler/k_local.hpp
--rw-rw-rw-   0        0        0     5302 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/tests/cxxtest/sampler/polynomial.hpp
--rw-rw-rw-   0        0        0     6371 2023-05-27 18:39:39.000000 v_quantum_annealing-0.0.0/tests/cxxtest/sampler/quadraitc.hpp
--rw-rw-rw-   0        0        0     6773 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/tests/cxxtest/sampler/swendsen_wang.hpp
-drwxrwxrwx   0        0        0        0 2023-05-28 13:28:24.801633 v_quantum_annealing-0.0.0/tests/cxxtest/system/
--rw-rw-rw-   0        0        0      826 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.0/tests/cxxtest/system/all.hpp
--rw-rw-rw-   0        0        0     7805 2023-05-27 18:39:44.000000 v_quantum_annealing-0.0.0/tests/cxxtest/system/binary_polynomial_sa_system.hpp
--rw-rw-rw-   0        0        0     1355 2023-05-27 18:39:49.000000 v_quantum_annealing-0.0.0/tests/cxxtest/system/classical_ising.hpp
--rw-rw-rw-   0        0        0     4055 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/tests/cxxtest/system/classical_ising_polynomial.hpp
--rw-rw-rw-   0        0        0     9297 2023-05-27 18:39:52.000000 v_quantum_annealing-0.0.0/tests/cxxtest/system/ising_polynomial_sa_system.hpp
--rw-rw-rw-   0        0        0     2412 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/tests/cxxtest/system/k_local.hpp
--rw-rw-rw-   0        0        0    15769 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/tests/cxxtest/testcase.hpp
-drwxrwxrwx   0        0        0        0 2023-05-28 13:28:24.848511 v_quantum_annealing-0.0.0/tests/cxxtest/utility/
--rw-rw-rw-   0        0        0      709 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.0/tests/cxxtest/utility/all.hpp
--rw-rw-rw-   0        0        0     3794 2023-05-27 18:39:57.000000 v_quantum_annealing-0.0.0/tests/cxxtest/utility/eigen.hpp
--rw-rw-rw-   0        0        0     6368 2023-05-27 18:39:59.000000 v_quantum_annealing-0.0.0/tests/cxxtest/utility/gpu.hpp
--rw-rw-rw-   0        0        0     1930 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/tests/cxxtest/utility/union_find.hpp
--rw-rw-rw-   0        0        0    28004 2023-05-27 18:59:08.000000 v_quantum_annealing-0.0.0/tests/test_cxx.py
--rw-rw-rw-   0        0        0     5754 2023-05-27 18:59:08.000000 v_quantum_annealing-0.0.0/tests/test_gpu.py
--rw-rw-rw-   0        0        0    60920 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/tests/test_hubo.py
--rw-rw-rw-   0        0        0     6313 2023-05-27 18:59:08.000000 v_quantum_annealing-0.0.0/tests/test_model.py
--rw-rw-rw-   0        0        0    10119 2023-05-27 18:59:08.000000 v_quantum_annealing-0.0.0/tests/test_sampler.py
--rw-rw-rw-   0        0        0     1181 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/tests/test_sqa.py
--rw-rw-rw-   0        0        0     1973 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-28 13:28:24.898374 v_quantum_annealing-0.0.0/v_quantum_annealing/
--rw-rw-rw-   0        0        0     2240 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/CMakeLists.txt
--rw-rw-rw-   0        0        0     1086 2023-05-27 18:59:08.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/__init__.py
--rw-rw-rw-   0        0        0     2953 2023-05-27 18:59:08.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/compile_config.hpp
--rw-rw-rw-   0        0        0    44916 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/declare.hpp
--rw-rw-rw-   0        0        0    15541 2023-05-27 18:59:08.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/main.cpp
-drwxrwxrwx   0        0        0        0 2023-05-28 13:28:23.970430 v_quantum_annealing-0.0.0/v_quantum_annealing/model/
--rw-rw-rw-   0        0        0      887 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/model/__init__.py
--rw-rw-rw-   0        0        0    14251 2023-05-27 18:59:08.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/model/chimera_model.py
--rw-rw-rw-   0        0        0     9000 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/model/king_graph.py
--rw-rw-rw-   0        0        0    23547 2023-05-27 18:59:08.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/model/model.py
-drwxrwxrwx   0        0        0        0 2023-05-28 13:28:24.095098 v_quantum_annealing-0.0.0/v_quantum_annealing/sampler/
--rw-rw-rw-   0        0        0      529 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/sampler/__init__.py
--rw-rw-rw-   0        0        0     4272 2023-05-27 18:59:08.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/sampler/base_sa_sample_hubo.py
-drwxrwxrwx   0        0        0        0 2023-05-28 13:28:24.155936 v_quantum_annealing-0.0.0/v_quantum_annealing/sampler/chimera_gpu/
--rw-rw-rw-   0        0        0      320 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/sampler/chimera_gpu/__init__.py
--rw-rw-rw-   0        0        0     2328 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/sampler/chimera_gpu/base_gpu_chimera.py
--rw-rw-rw-   0        0        0     4975 2023-05-27 18:59:08.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/sampler/chimera_gpu/gpu_sa_sampler.py
--rw-rw-rw-   0        0        0     5812 2023-05-27 18:59:08.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/sampler/chimera_gpu/gpu_sqa_sampler.py
--rw-rw-rw-   0        0        0     5240 2023-05-27 18:59:08.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/sampler/csqa_sampler.py
--rw-rw-rw-   0        0        0     1089 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/sampler/response.py
--rw-rw-rw-   0        0        0    25497 2023-05-27 18:59:08.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/sampler/sa_sampler.py
--rw-rw-rw-   0        0        0     8944 2023-05-27 18:59:08.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/sampler/sampler.py
--rw-rw-rw-   0        0        0    12920 2023-05-27 18:59:08.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/sampler/sqa_sampler.py
-drwxrwxrwx   0        0        0        0 2023-05-28 13:28:24.299550 v_quantum_annealing-0.0.0/v_quantum_annealing/utils/
--rw-rw-rw-   0        0        0      767 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/utils/__init__.py
--rw-rw-rw-   0        0        0    10117 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/utils/benchmark.py
--rw-rw-rw-   0        0        0     1283 2023-05-27 18:59:08.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/utils/cxx_cast.py
--rw-rw-rw-   0        0        0      855 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/utils/decorator.py
--rw-rw-rw-   0        0        0      992 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/utils/graph_utils.py
--rw-rw-rw-   0        0        0     2085 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/utils/res_convertor.py
--rw-rw-rw-   0        0        0       36 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/utils/time_measure.py
--rw-rw-rw-   0        0        0      975 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.0/v_quantum_annealing/variable_type.py
-drwxrwxrwx   0        0        0        0 2023-05-28 13:28:24.945249 v_quantum_annealing-0.0.0/v_quantum_annealing.egg-info/
--rw-rw-rw-   0        0        0    12457 2023-05-28 13:28:23.000000 v_quantum_annealing-0.0.0/v_quantum_annealing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4560 2023-05-28 13:28:23.000000 v_quantum_annealing-0.0.0/v_quantum_annealing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 13:28:23.000000 v_quantum_annealing-0.0.0/v_quantum_annealing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-23 08:08:59.000000 v_quantum_annealing-0.0.0/v_quantum_annealing.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      130 2023-05-28 13:28:23.000000 v_quantum_annealing-0.0.0/v_quantum_annealing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-28 13:28:23.000000 v_quantum_annealing-0.0.0/v_quantum_annealing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:31.131653 v_quantum_annealing-0.0.1/
+-rw-rw-rw-   0        0        0     8738 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.1/CMakeLists.txt
+-rw-rw-rw-   0        0        0       72 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.1/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11560 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1289 2023-05-27 18:46:55.000000 v_quantum_annealing-0.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1285 2023-05-28 17:52:31.131653 v_quantum_annealing-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9292 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:30.844421 v_quantum_annealing-0.0.1/cmake/
+-rw-rw-rw-   0        0        0     5390 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.1/cmake/FindGcov.cmake
+-rw-rw-rw-   0        0        0    13074 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.1/cmake/FindLcov.cmake
+-rw-rw-rw-   0        0        0     9299 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.1/cmake/Findcodecov.cmake
+-rw-rw-rw-   0        0        0     4712 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.1/cmake/GenerateDocs.cmake
+-rw-rw-rw-   0        0        0     2000 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.1/cmake/PythonAutoDetectOSX.cmake
+-rw-rw-rw-   0        0        0     1129 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.1/cmake/llvm-cov-wrapper
+-rw-rw-rw-   0        0        0     1222 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.1/doc-requirements.in
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:30.853398 v_quantum_annealing-0.0.1/external/
+-rw-rw-rw-   0        0        0     1002 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/external/cimod.cmake
+-rw-rw-rw-   0        0        0     1704 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/external/eigen.cmake
+-rw-rw-rw-   0        0        0      724 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.1/external/googletest.cmake
+-rw-rw-rw-   0        0        0      781 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.1/external/json.cmake
+-rw-rw-rw-   0        0        0      465 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.1/external/pybind11-json.cmake
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:30.856390 v_quantum_annealing-0.0.1/include/
+-rw-rw-rw-   0        0        0     2163 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.1/include/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:30.698811 v_quantum_annealing-0.0.1/include/v_quantum_annealing/
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:30.860380 v_quantum_annealing-0.0.1/include/v_quantum_annealing/algorithm/
+-rw-rw-rw-   0        0        0     3209 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/algorithm/algorithm.hpp
+-rw-rw-rw-   0        0        0      696 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/algorithm/all.hpp
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:30.883319 v_quantum_annealing-0.0.1/include/v_quantum_annealing/graph/
+-rw-rw-rw-   0        0        0     1119 2023-05-28 15:16:57.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/graph/all.hpp
+-rw-rw-rw-   0        0        0     9623 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/graph/binary_polynomial_model.hpp
+-rw-rw-rw-   0        0        0    15447 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/graph/chimera.hpp
+-rw-rw-rw-   0        0        0      864 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/graph/converter.hpp
+-rw-rw-rw-   0        0        0     5234 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/graph/csr_sparse.hpp
+-rw-rw-rw-   0        0        0     7667 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/graph/dense.hpp
+-rw-rw-rw-   0        0        0     2580 2023-05-27 18:36:30.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/graph/graph.hpp
+-rw-rw-rw-   0        0        0     9568 2023-05-27 18:36:33.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/graph/ising_polynomial_model.hpp
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:30.885312 v_quantum_annealing-0.0.1/include/v_quantum_annealing/graph/json/
+-rw-rw-rw-   0        0        0     4445 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/graph/json/parse.hpp
+-rw-rw-rw-   0        0        0    11197 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/graph/polynomial.hpp
+-rw-rw-rw-   0        0        0     8292 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/graph/sparse.hpp
+-rw-rw-rw-   0        0        0    10587 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/graph/square.hpp
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:30.888305 v_quantum_annealing-0.0.1/include/v_quantum_annealing/result/
+-rw-rw-rw-   0        0        0      696 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/result/all.hpp
+-rw-rw-rw-   0        0        0     5182 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/result/get_solution.hpp
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:30.890298 v_quantum_annealing-0.0.1/include/v_quantum_annealing/sampler/
+-rw-rw-rw-   0        0        0    10600 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/sampler/sa_sampler.hpp
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:30.920219 v_quantum_annealing-0.0.1/include/v_quantum_annealing/system/
+-rw-rw-rw-   0        0        0     1152 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/system/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1375 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/system/all.hpp
+-rw-rw-rw-   0        0        0     6273 2023-05-27 18:36:52.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/system/binary_polynomial_sa_system.hpp
+-rw-rw-rw-   0        0        0     7177 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/system/classical_ising.hpp
+-rw-rw-rw-   0        0        0    21800 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/system/classical_ising_polynomial.hpp
+-rw-rw-rw-   0        0        0    15146 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/system/continuous_time_ising.hpp
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:30.924208 v_quantum_annealing-0.0.1/include/v_quantum_annealing/system/gpu/
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:30.932188 v_quantum_annealing-0.0.1/include/v_quantum_annealing/system/gpu/chimera_cuda/
+-rw-rw-rw-   0        0        0     5580 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/system/gpu/chimera_cuda/index.hpp
+-rw-rw-rw-   0        0        0    14580 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.cu
+-rw-rw-rw-   0        0        0     1715 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/system/gpu/chimera_cuda/kernel.hpp
+-rw-rw-rw-   0        0        0     2863 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/system/gpu/chimera_gpu_classical.hpp
+-rw-rw-rw-   0        0        0    16583 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/system/gpu/chimera_gpu_transverse.hpp
+-rw-rw-rw-   0        0        0     5467 2023-05-27 18:37:04.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/system/ising_polynomial_sa_system.hpp
+-rw-rw-rw-   0        0        0    24703 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/system/k_local_polynomial.hpp
+-rw-rw-rw-   0        0        0      821 2023-05-27 18:37:09.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/system/sa_system.hpp
+-rw-rw-rw-   0        0        0     3382 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/system/system.hpp
+-rw-rw-rw-   0        0        0    19919 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/system/transverse_ising.hpp
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:30.946151 v_quantum_annealing-0.0.1/include/v_quantum_annealing/updater/
+-rw-rw-rw-   0        0        0     1054 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/updater/all.hpp
+-rw-rw-rw-   0        0        0    19581 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/updater/continuous_time_swendsen_wang.hpp
+-rw-rw-rw-   0        0        0     5433 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/updater/gpu.hpp
+-rw-rw-rw-   0        0        0     3854 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/updater/k_local.hpp
+-rw-rw-rw-   0        0        0    13730 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/updater/single_spin_flip.hpp
+-rw-rw-rw-   0        0        0     6487 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/updater/swendsen_wang.hpp
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:30.974075 v_quantum_annealing-0.0.1/include/v_quantum_annealing/utility/
+-rw-rw-rw-   0        0        0     1020 2023-05-27 18:38:11.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/utility/create_geometric_progression.hpp
+-rw-rw-rw-   0        0        0     1144 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/utility/disable_eigen_warning.hpp
+-rw-rw-rw-   0        0        0     5923 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/utility/eigen.hpp
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:30.976069 v_quantum_annealing-0.0.1/include/v_quantum_annealing/utility/fmath/
+-rw-rw-rw-   0        0        0    26304 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/utility/fmath/fmath.hpp
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:30.980059 v_quantum_annealing-0.0.1/include/v_quantum_annealing/utility/gpu/
+-rw-rw-rw-   0        0        0     8392 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/utility/gpu/cublas.hpp
+-rw-rw-rw-   0        0        0     3026 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/utility/gpu/handle_error.hpp
+-rw-rw-rw-   0        0        0     2666 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/utility/gpu/memory.hpp
+-rw-rw-rw-   0        0        0     1067 2023-05-27 18:38:16.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/utility/index_type.hpp
+-rw-rw-rw-   0        0        0     1302 2023-05-27 18:38:18.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/utility/insert_or_assign.hpp
+-rw-rw-rw-   0        0        0     1083 2023-05-27 18:38:20.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/utility/memory.hpp
+-rw-rw-rw-   0        0        0     3638 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/utility/pairhash.hpp
+-rw-rw-rw-   0        0        0     4019 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/utility/random.hpp
+-rw-rw-rw-   0        0        0    10601 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/utility/schedule_list.hpp
+-rw-rw-rw-   0        0        0      818 2023-05-27 18:38:30.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/utility/thres_hold.hpp
+-rw-rw-rw-   0        0        0     2409 2023-05-27 18:38:32.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/utility/type_traits.hpp
+-rw-rw-rw-   0        0        0     2274 2023-05-27 18:38:33.000000 v_quantum_annealing-0.0.1/include/v_quantum_annealing/utility/union_find.hpp
+-rw-rw-rw-   0        0        0     4646 2023-05-27 18:46:58.000000 v_quantum_annealing-0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1578 2023-05-28 17:52:31.134646 v_quantum_annealing-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1342 2023-05-28 17:52:18.000000 v_quantum_annealing-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:31.006987 v_quantum_annealing-0.0.1/tests/
+-rw-rw-rw-   0        0        0     1756 2023-05-28 17:40:55.000000 v_quantum_annealing-0.0.1/tests/CMakeLists.txt
+-rw-rw-rw-   0        0        0        0 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:31.026935 v_quantum_annealing-0.0.1/tests/__pycache__/
+-rw-rw-rw-   0        0        0      127 2023-05-23 08:09:01.000000 v_quantum_annealing-0.0.1/tests/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    13004 2023-05-23 08:09:01.000000 v_quantum_annealing-0.0.1/tests/__pycache__/test_cxx.cpython-39-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0      127 2023-05-23 08:09:01.000000 v_quantum_annealing-0.0.1/tests/__pycache__/test_gpu.cpython-39-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0    34580 2023-05-23 08:09:01.000000 v_quantum_annealing-0.0.1/tests/__pycache__/test_hubo.cpython-39-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0     5551 2023-05-23 08:09:02.000000 v_quantum_annealing-0.0.1/tests/__pycache__/test_model.cpython-39-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0     8200 2023-05-23 08:09:02.000000 v_quantum_annealing-0.0.1/tests/__pycache__/test_sampler.cpython-39-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0     1848 2023-05-23 08:09:03.000000 v_quantum_annealing-0.0.1/tests/__pycache__/test_sqa.cpython-39-pytest-7.3.1.pyc
+-rw-rw-rw-   0        0        0     2147 2023-05-23 08:09:03.000000 v_quantum_annealing-0.0.1/tests/__pycache__/test_utils.cpython-39-pytest-7.3.1.pyc
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:31.033919 v_quantum_annealing-0.0.1/tests/cxxtest/
+-rw-rw-rw-   0        0        0     1944 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/tests/cxxtest/cxxtest.cpp
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:31.041894 v_quantum_annealing-0.0.1/tests/cxxtest/graph/
+-rw-rw-rw-   0        0        0      774 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.1/tests/cxxtest/graph/all.hpp
+-rw-rw-rw-   0        0        0     6099 2023-05-27 18:38:59.000000 v_quantum_annealing-0.0.1/tests/cxxtest/graph/binary_polynomial_model.hpp
+-rw-rw-rw-   0        0        0     5882 2023-05-27 18:39:02.000000 v_quantum_annealing-0.0.1/tests/cxxtest/graph/ising_polynomial_model.hpp
+-rw-rw-rw-   0        0        0     4569 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/tests/cxxtest/graph/polynomial.hpp
+-rw-rw-rw-   0        0        0     7048 2023-05-27 18:39:20.000000 v_quantum_annealing-0.0.1/tests/cxxtest/graph/quadratic.hpp
+-rw-rw-rw-   0        0        0    38994 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/tests/cxxtest/polynomial_test.hpp
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:31.044885 v_quantum_annealing-0.0.1/tests/cxxtest/result/
+-rw-rw-rw-   0        0        0      665 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.1/tests/cxxtest/result/all.hpp
+-rw-rw-rw-   0        0        0     2742 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/tests/cxxtest/result/result.hpp
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:31.059846 v_quantum_annealing-0.0.1/tests/cxxtest/sampler/
+-rw-rw-rw-   0        0        0      856 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.1/tests/cxxtest/sampler/all.hpp
+-rw-rw-rw-   0        0        0     2406 2023-05-27 18:39:25.000000 v_quantum_annealing-0.0.1/tests/cxxtest/sampler/binary_polynomial_sa_sampler.hpp
+-rw-rw-rw-   0        0        0     3165 2023-05-27 18:39:29.000000 v_quantum_annealing-0.0.1/tests/cxxtest/sampler/gpu.hpp
+-rw-rw-rw-   0        0        0     2394 2023-05-27 18:39:31.000000 v_quantum_annealing-0.0.1/tests/cxxtest/sampler/ising_polynomial_sa_sampler.hpp
+-rw-rw-rw-   0        0        0     4278 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/tests/cxxtest/sampler/k_local.hpp
+-rw-rw-rw-   0        0        0     5302 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/tests/cxxtest/sampler/polynomial.hpp
+-rw-rw-rw-   0        0        0     6371 2023-05-27 18:39:39.000000 v_quantum_annealing-0.0.1/tests/cxxtest/sampler/quadraitc.hpp
+-rw-rw-rw-   0        0        0     6773 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/tests/cxxtest/sampler/swendsen_wang.hpp
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:31.071814 v_quantum_annealing-0.0.1/tests/cxxtest/system/
+-rw-rw-rw-   0        0        0      826 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.1/tests/cxxtest/system/all.hpp
+-rw-rw-rw-   0        0        0     7805 2023-05-27 18:39:44.000000 v_quantum_annealing-0.0.1/tests/cxxtest/system/binary_polynomial_sa_system.hpp
+-rw-rw-rw-   0        0        0     1355 2023-05-27 18:39:49.000000 v_quantum_annealing-0.0.1/tests/cxxtest/system/classical_ising.hpp
+-rw-rw-rw-   0        0        0     4055 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/tests/cxxtest/system/classical_ising_polynomial.hpp
+-rw-rw-rw-   0        0        0     9297 2023-05-27 18:39:52.000000 v_quantum_annealing-0.0.1/tests/cxxtest/system/ising_polynomial_sa_system.hpp
+-rw-rw-rw-   0        0        0     2412 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/tests/cxxtest/system/k_local.hpp
+-rw-rw-rw-   0        0        0    15769 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/tests/cxxtest/testcase.hpp
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:31.077798 v_quantum_annealing-0.0.1/tests/cxxtest/utility/
+-rw-rw-rw-   0        0        0      709 2023-05-22 08:20:45.000000 v_quantum_annealing-0.0.1/tests/cxxtest/utility/all.hpp
+-rw-rw-rw-   0        0        0     3794 2023-05-27 18:39:57.000000 v_quantum_annealing-0.0.1/tests/cxxtest/utility/eigen.hpp
+-rw-rw-rw-   0        0        0     6368 2023-05-27 18:39:59.000000 v_quantum_annealing-0.0.1/tests/cxxtest/utility/gpu.hpp
+-rw-rw-rw-   0        0        0     1930 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/tests/cxxtest/utility/union_find.hpp
+-rw-rw-rw-   0        0        0    28004 2023-05-28 14:44:36.000000 v_quantum_annealing-0.0.1/tests/test_cxx.py
+-rw-rw-rw-   0        0        0     5754 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.1/tests/test_gpu.py
+-rw-rw-rw-   0        0        0    60920 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/tests/test_hubo.py
+-rw-rw-rw-   0        0        0     6313 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.1/tests/test_model.py
+-rw-rw-rw-   0        0        0    10119 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.1/tests/test_sampler.py
+-rw-rw-rw-   0        0        0     1181 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/tests/test_sqa.py
+-rw-rw-rw-   0        0        0     1973 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:31.084779 v_quantum_annealing-0.0.1/v_quantum_annealing/
+-rw-rw-rw-   0        0        0     2240 2023-05-28 17:40:55.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1086 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/__init__.py
+-rw-rw-rw-   0        0        0     2953 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/compile_config.hpp
+-rw-rw-rw-   0        0        0    44916 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/declare.hpp
+-rw-rw-rw-   0        0        0    15541 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/main.cpp
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:30.782601 v_quantum_annealing-0.0.1/v_quantum_annealing/model/
+-rw-rw-rw-   0        0        0      887 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/model/__init__.py
+-rw-rw-rw-   0        0        0    14251 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/model/chimera_model.py
+-rw-rw-rw-   0        0        0     9000 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/model/king_graph.py
+-rw-rw-rw-   0        0        0    23547 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/model/model.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:30.800540 v_quantum_annealing-0.0.1/v_quantum_annealing/sampler/
+-rw-rw-rw-   0        0        0      529 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/sampler/__init__.py
+-rw-rw-rw-   0        0        0     4272 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/sampler/base_sa_sample_hubo.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:30.808518 v_quantum_annealing-0.0.1/v_quantum_annealing/sampler/chimera_gpu/
+-rw-rw-rw-   0        0        0      320 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/sampler/chimera_gpu/__init__.py
+-rw-rw-rw-   0        0        0     2328 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/sampler/chimera_gpu/base_gpu_chimera.py
+-rw-rw-rw-   0        0        0     4975 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/sampler/chimera_gpu/gpu_sa_sampler.py
+-rw-rw-rw-   0        0        0     5812 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/sampler/chimera_gpu/gpu_sqa_sampler.py
+-rw-rw-rw-   0        0        0     5240 2023-05-28 14:52:35.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/sampler/csqa_sampler.py
+-rw-rw-rw-   0        0        0     1089 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/sampler/response.py
+-rw-rw-rw-   0        0        0    25497 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/sampler/sa_sampler.py
+-rw-rw-rw-   0        0        0     8944 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/sampler/sampler.py
+-rw-rw-rw-   0        0        0    12920 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/sampler/sqa_sampler.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:30.828464 v_quantum_annealing-0.0.1/v_quantum_annealing/utils/
+-rw-rw-rw-   0        0        0      767 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/utils/__init__.py
+-rw-rw-rw-   0        0        0    10117 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/utils/benchmark.py
+-rw-rw-rw-   0        0        0     1283 2023-05-28 14:44:34.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/utils/cxx_cast.py
+-rw-rw-rw-   0        0        0      855 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/utils/decorator.py
+-rw-rw-rw-   0        0        0      992 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/utils/graph_utils.py
+-rw-rw-rw-   0        0        0     2085 2023-05-27 18:56:34.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/utils/res_convertor.py
+-rw-rw-rw-   0        0        0       36 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/utils/time_measure.py
+-rw-rw-rw-   0        0        0      975 2023-05-27 18:26:03.000000 v_quantum_annealing-0.0.1/v_quantum_annealing/variable_type.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:52:31.122678 v_quantum_annealing-0.0.1/v_quantum_annealing.egg-info/
+-rw-rw-rw-   0        0        0     1285 2023-05-28 17:52:30.000000 v_quantum_annealing-0.0.1/v_quantum_annealing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7487 2023-05-28 17:52:30.000000 v_quantum_annealing-0.0.1/v_quantum_annealing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 17:52:30.000000 v_quantum_annealing-0.0.1/v_quantum_annealing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-23 08:08:59.000000 v_quantum_annealing-0.0.1/v_quantum_annealing.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      130 2023-05-28 17:52:30.000000 v_quantum_annealing-0.0.1/v_quantum_annealing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-28 17:52:30.000000 v_quantum_annealing-0.0.1/v_quantum_annealing.egg-info/top_level.txt
```

### Comparing `v_quantum_annealing-0.0.0/CMakeLists.txt` & `v_quantum_annealing-0.0.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/LICENSE` & `v_quantum_annealing-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/MANIFEST.in` & `v_quantum_annealing-0.0.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/README.md` & `v_quantum_annealing-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/cmake/FindGcov.cmake` & `v_quantum_annealing-0.0.1/cmake/FindGcov.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/cmake/FindLcov.cmake` & `v_quantum_annealing-0.0.1/cmake/FindLcov.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/cmake/Findcodecov.cmake` & `v_quantum_annealing-0.0.1/cmake/Findcodecov.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/cmake/GenerateDocs.cmake` & `v_quantum_annealing-0.0.1/cmake/GenerateDocs.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/cmake/PythonAutoDetectOSX.cmake` & `v_quantum_annealing-0.0.1/cmake/PythonAutoDetectOSX.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/cmake/llvm-cov-wrapper` & `v_quantum_annealing-0.0.1/cmake/llvm-cov-wrapper`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/doc-requirements.in` & `v_quantum_annealing-0.0.1/doc-requirements.in`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/external/cimod.cmake` & `v_quantum_annealing-0.0.1/external/cimod.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/external/eigen.cmake` & `v_quantum_annealing-0.0.1/external/eigen.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/external/googletest.cmake` & `v_quantum_annealing-0.0.1/external/googletest.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/external/json.cmake` & `v_quantum_annealing-0.0.1/external/json.cmake`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/include/CMakeLists.txt` & `v_quantum_annealing-0.0.1/include/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/pyproject.toml` & `v_quantum_annealing-0.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/setup.cfg` & `v_quantum_annealing-0.0.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,97 +1,99 @@
 00000000: 5b69 6e73 7461 6c6c 5f6c 6962 5d0d 0a6f  [install_lib]..o
 00000010: 7074 696d 697a 6520 3d20 310d 0a63 6f6d  ptimize = 1..com
 00000020: 7069 6c65 203d 2031 0d0a 0d0a 5b61 6c69  pile = 1....[ali
 00000030: 6173 6573 5d0d 0a74 6573 7420 3d20 7079  ases]..test = py
 00000040: 7465 7374 0d0a 0d0a 5b6d 6574 6164 6174  test....[metadat
 00000050: 615d 0d0a 6e61 6d65 203d 2076 5f71 7561  a]..name = v_qua
 00000060: 6e74 756d 5f61 6e6e 6561 6c69 6e67 0d0a  ntum_annealing..
-00000070: 7572 6c20 3d20 6874 7470 733a 2f2f 7777  url = https://ww
-00000080: 772e 765f 7175 616e 7475 6d5f 616e 6e65  w.v_quantum_anne
-00000090: 616c 696e 672e 6f72 670d 0a61 7574 686f  aling.org..autho
-000000a0: 7220 3d20 4a69 6a20 496e 632e 0d0a 6175  r = Jij Inc...au
-000000b0: 7468 6f72 5f65 6d61 696c 203d 2063 616f  thor_email = cao
-000000c0: 7472 756f 6e67 3035 3131 4067 6d61 696c  truong0511@gmail
-000000d0: 2e63 6f6d 0d0a 6465 7363 7269 7074 696f  .com..descriptio
-000000e0: 6e20 3d20 4672 616d 6577 6f72 6b20 666f  n = Framework fo
-000000f0: 7220 7468 6520 4973 696e 6720 6d6f 6465  r the Ising mode
-00000100: 6c20 616e 6420 5155 424f 2e0d 0a6c 6f6e  l and QUBO...lon
-00000110: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
-00000120: 6669 6c65 3a20 5245 4144 4d45 2e6d 640d  file: README.md.
-00000130: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-00000140: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
-00000150: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
-00000160: 6c69 6365 6e73 655f 6669 6c65 7320 3d20  license_files = 
-00000170: 4c49 4345 4e53 450d 0a6c 6963 656e 7365  LICENSE..license
-00000180: 203d 2041 7061 6368 6520 4c69 6365 6e73   = Apache Licens
-00000190: 6520 322e 300d 0a63 6c61 7373 6966 6965  e 2.0..classifie
-000001a0: 7273 203d 200d 0a09 4c69 6365 6e73 6520  rs = ...License 
-000001b0: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-000001c0: 3a3a 2041 7061 6368 6520 536f 6674 7761  :: Apache Softwa
-000001d0: 7265 204c 6963 656e 7365 0d0a 0949 6e74  re License...Int
-000001e0: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
-000001f0: 3a20 5363 6965 6e63 652f 5265 7365 6172  : Science/Resear
-00000200: 6368 0d0a 0950 726f 6772 616d 6d69 6e67  ch...Programming
-00000210: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000220: 686f 6e0d 0a09 5072 6f67 7261 6d6d 696e  hon...Programmin
-00000230: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000240: 7468 6f6e 203a 3a20 332e 370d 0a09 5072  thon :: 3.7...Pr
-00000250: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000260: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000270: 332e 380d 0a09 5072 6f67 7261 6d6d 696e  3.8...Programmin
-00000280: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000290: 7468 6f6e 203a 3a20 332e 390d 0a09 5072  thon :: 3.9...Pr
-000002a0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000002b0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000002c0: 332e 3130 0d0a 0950 726f 6772 616d 6d69  3.10...Programmi
-000002d0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000002e0: 7974 686f 6e20 3a3a 2033 203a 3a20 4f6e  ython :: 3 :: On
-000002f0: 6c79 0d0a 0950 726f 6772 616d 6d69 6e67  ly...Programming
-00000300: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000310: 686f 6e20 3a3a 2049 6d70 6c65 6d65 6e74  hon :: Implement
-00000320: 6174 696f 6e20 3a3a 2043 5079 7468 6f6e  ation :: CPython
-00000330: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
-00000340: 7465 6d20 3a3a 204d 6963 726f 736f 6674  tem :: Microsoft
-00000350: 203a 3a20 5769 6e64 6f77 730d 0a09 4f70   :: Windows...Op
-00000360: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-00000370: 3a20 504f 5349 580d 0a09 4f70 6572 6174  : POSIX...Operat
-00000380: 696e 6720 5379 7374 656d 203a 3a20 556e  ing System :: Un
-00000390: 6978 0d0a 094f 7065 7261 7469 6e67 2053  ix...Operating S
-000003a0: 7973 7465 6d20 3a3a 204d 6163 4f53 0d0a  ystem :: MacOS..
-000003b0: 7072 6f6a 6563 745f 7572 6c73 203d 200d  project_urls = .
-000003c0: 0a09 536f 7572 6365 3d68 7474 7073 3a2f  ..Source=https:/
-000003d0: 2f67 6974 6875 622e 636f 6d2f 762d 7175  /github.com/v-qu
-000003e0: 616e 7475 6d2d 6a73 632f 562d 5155 414e  antum-jsc/V-QUAN
-000003f0: 5455 4d2d 414e 4e45 414c 494e 470d 0a09  TUM-ANNEALING...
-00000400: 446f 6375 6d65 6e74 6174 696f 6e3d 6874  Documentation=ht
-00000410: 7470 733a 2f2f 765f 7175 616e 7475 6d5f  tps://v_quantum_
-00000420: 616e 6e65 616c 696e 672e 6769 7468 7562  annealing.github
-00000430: 2e69 6f2f 765f 7175 616e 7475 6d5f 616e  .io/v_quantum_an
-00000440: 6e65 616c 696e 670d 0a09 5265 6665 7265  nealing...Refere
-00000450: 6e63 653d 6874 7470 733a 2f2f 7265 662e  nce=https://ref.
-00000460: 765f 7175 616e 7475 6d5f 616e 6e65 616c  v_quantum_anneal
-00000470: 696e 672e 6f72 672f 696e 6465 782e 6874  ing.org/index.ht
-00000480: 6d6c 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  ml....[options].
-00000490: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
-000004a0: 203d 203e 3d33 2e37 2c20 3c33 2e31 310d   = >=3.7, <3.11.
-000004b0: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
-000004c0: 7320 3d20 0d0a 096e 756d 7079 203e 3d31  s = ...numpy >=1
-000004d0: 2e31 372e 332c 203c 2031 2e32 352e 300d  .17.3, < 1.25.0.
-000004e0: 0a09 6469 6d6f 6420 3c20 302e 3133 2e30  ..dimod < 0.13.0
-000004f0: 0d0a 0973 6369 7079 203e 3d20 312e 372e  ...scipy >= 1.7.
-00000500: 332c 203c 2031 2e31 312e 300d 0a09 7265  3, < 1.11.0...re
-00000510: 7175 6573 7473 203e 3d20 322e 3238 2e30  quests >= 2.28.0
-00000520: 2c20 3c20 322e 3239 2e30 0d0a 096a 696a  , < 2.29.0...jij
-00000530: 2d63 696d 6f64 203e 3d20 312e 302e 302c  -cimod >= 1.0.0,
-00000540: 203c 2031 2e32 2e33 0d0a 0974 7970 696e   < 1.2.3...typin
-00000550: 672d 6578 7465 6e73 696f 6e73 203e 3d20  g-extensions >= 
-00000560: 342e 322e 300d 0a74 6573 7473 5f72 6571  4.2.0..tests_req
-00000570: 7569 7265 203d 200d 0a09 7079 7465 7374  uire = ...pytest
-00000580: 0d0a 0970 7974 6573 742d 6d6f 636b 0d0a  ...pytest-mock..
-00000590: 0970 7974 6573 742d 636f 760d 0a09 7079  .pytest-cov...py
-000005a0: 7465 7374 2d72 756e 6e65 720d 0a09 7079  test-runner...py
-000005b0: 7465 7374 2d72 616e 646f 6d6c 790d 0a09  test-randomly...
-000005c0: 7079 7465 7374 2d73 7065 630d 0a09 636f  pytest-spec...co
-000005d0: 7665 7261 6765 0d0a 0d0a 5b65 6767 5f69  verage....[egg_i
-000005e0: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
-000005f0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
-00000600: 0d0a 0d0a                                ....
+00000070: 7572 6c20 3d20 6874 7470 733a 2f2f 762d  url = https://v-
+00000080: 7175 616e 7475 6d2d 7465 6368 6e6f 6c6f  quantum-technolo
+00000090: 6779 2e63 6f6d 0d0a 6175 7468 6f72 203d  gy.com..author =
+000000a0: 2022 562d 5155 414e 5455 4d20 4a53 4322   "V-QUANTUM JSC"
+000000b0: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
+000000c0: 206e 7174 6869 6e68 4076 2d71 7561 6e74   nqthinh@v-quant
+000000d0: 756d 2d74 6563 686e 6f6c 6f67 792e 636f  um-technology.co
+000000e0: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
+000000f0: 2022 4672 616d 6577 6f72 6b20 666f 7220   "Framework for 
+00000100: 7468 6520 4973 696e 6720 6d6f 6465 6c20  the Ising model 
+00000110: 616e 6420 5155 424f 2e22 0d0a 6c6f 6e67  and QUBO."..long
+00000120: 5f64 6573 6372 6970 7469 6f6e 203d 2022  _description = "
+00000130: 6669 6c65 3a20 5245 4144 4d45 2e6d 6422  file: README.md"
+00000140: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+00000150: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
+00000160: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0d  = text/markdown.
+00000170: 0a6c 6963 656e 7365 5f66 696c 6573 203d  .license_files =
+00000180: 204c 4943 454e 5345 0d0a 6c69 6365 6e73   LICENSE..licens
+00000190: 6520 3d20 2241 7061 6368 6520 4c69 6365  e = "Apache Lice
+000001a0: 6e73 6520 322e 3022 0d0a 7665 7273 696f  nse 2.0"..versio
+000001b0: 6e20 3d20 2230 2e30 2e31 220d 0a63 6c61  n = "0.0.1"..cla
+000001c0: 7373 6966 6965 7273 203d 200d 0a09 4c69  ssifiers = ...Li
+000001d0: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+000001e0: 726f 7665 6420 3a3a 2041 7061 6368 6520  roved :: Apache 
+000001f0: 536f 6674 7761 7265 204c 6963 656e 7365  Software License
+00000200: 0d0a 0949 6e74 656e 6465 6420 4175 6469  ...Intended Audi
+00000210: 656e 6365 203a 3a20 5363 6965 6e63 652f  ence :: Science/
+00000220: 5265 7365 6172 6368 0d0a 0950 726f 6772  Research...Progr
+00000230: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000240: 3a3a 2050 7974 686f 6e0d 0a09 5072 6f67  :: Python...Prog
+00000250: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000260: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000270: 370d 0a09 5072 6f67 7261 6d6d 696e 6720  7...Programming 
+00000280: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000290: 6f6e 203a 3a20 332e 380d 0a09 5072 6f67  on :: 3.8...Prog
+000002a0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000002b0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000002c0: 390d 0a09 5072 6f67 7261 6d6d 696e 6720  9...Programming 
+000002d0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000002e0: 6f6e 203a 3a20 332e 3130 0d0a 0950 726f  on :: 3.10...Pro
+000002f0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000300: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000310: 203a 3a20 4f6e 6c79 0d0a 0950 726f 6772   :: Only...Progr
+00000320: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000330: 3a3a 2050 7974 686f 6e20 3a3a 2049 6d70  :: Python :: Imp
+00000340: 6c65 6d65 6e74 6174 696f 6e20 3a3a 2043  lementation :: C
+00000350: 5079 7468 6f6e 0d0a 094f 7065 7261 7469  Python...Operati
+00000360: 6e67 2053 7973 7465 6d20 3a3a 204d 6963  ng System :: Mic
+00000370: 726f 736f 6674 203a 3a20 5769 6e64 6f77  rosoft :: Window
+00000380: 730d 0a09 4f70 6572 6174 696e 6720 5379  s...Operating Sy
+00000390: 7374 656d 203a 3a20 504f 5349 580d 0a09  stem :: POSIX...
+000003a0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+000003b0: 203a 3a20 556e 6978 0d0a 094f 7065 7261   :: Unix...Opera
+000003c0: 7469 6e67 2053 7973 7465 6d20 3a3a 204d  ting System :: M
+000003d0: 6163 4f53 0d0a 7072 6f6a 6563 745f 7572  acOS..project_ur
+000003e0: 6c73 203d 200d 0a09 536f 7572 6365 3d68  ls = ...Source=h
+000003f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000400: 6d2f 762d 7175 616e 7475 6d2d 6a73 632f  m/v-quantum-jsc/
+00000410: 562d 5155 414e 5455 4d2d 414e 4e45 414c  V-QUANTUM-ANNEAL
+00000420: 494e 470d 0a09 446f 6375 6d65 6e74 6174  ING...Documentat
+00000430: 696f 6e3d 6874 7470 733a 2f2f 765f 7175  ion=https://v_qu
+00000440: 616e 7475 6d5f 616e 6e65 616c 696e 672e  antum_annealing.
+00000450: 6769 7468 7562 2e69 6f2f 765f 7175 616e  github.io/v_quan
+00000460: 7475 6d5f 616e 6e65 616c 696e 670d 0a09  tum_annealing...
+00000470: 5265 6665 7265 6e63 653d 6874 7470 733a  Reference=https:
+00000480: 2f2f 7265 662e 765f 7175 616e 7475 6d5f  //ref.v_quantum_
+00000490: 616e 6e65 616c 696e 672e 6f72 672f 696e  annealing.org/in
+000004a0: 6465 782e 6874 6d6c 0d0a 0d0a 5b6f 7074  dex.html....[opt
+000004b0: 696f 6e73 5d0d 0a70 7974 686f 6e5f 7265  ions]..python_re
+000004c0: 7175 6972 6573 203d 203e 3d33 2e37 2c20  quires = >=3.7, 
+000004d0: 3c33 2e31 310d 0a69 6e73 7461 6c6c 5f72  <3.11..install_r
+000004e0: 6571 7569 7265 7320 3d20 0d0a 096e 756d  equires = ...num
+000004f0: 7079 203e 3d31 2e31 372e 332c 203c 2031  py >=1.17.3, < 1
+00000500: 2e32 352e 300d 0a09 6469 6d6f 6420 3c20  .25.0...dimod < 
+00000510: 302e 3133 2e30 0d0a 0973 6369 7079 203e  0.13.0...scipy >
+00000520: 3d20 312e 372e 332c 203c 2031 2e31 312e  = 1.7.3, < 1.11.
+00000530: 300d 0a09 7265 7175 6573 7473 203e 3d20  0...requests >= 
+00000540: 322e 3238 2e30 2c20 3c20 322e 3239 2e30  2.28.0, < 2.29.0
+00000550: 0d0a 0976 7161 2d63 696d 6f64 203e 3d20  ...vqa-cimod >= 
+00000560: 312e 302e 302c 203c 2031 2e32 2e33 0d0a  1.0.0, < 1.2.3..
+00000570: 0974 7970 696e 672d 6578 7465 6e73 696f  .typing-extensio
+00000580: 6e73 203e 3d20 342e 322e 300d 0a74 6573  ns >= 4.2.0..tes
+00000590: 7473 5f72 6571 7569 7265 203d 200d 0a09  ts_require = ...
+000005a0: 7079 7465 7374 0d0a 0970 7974 6573 742d  pytest...pytest-
+000005b0: 6d6f 636b 0d0a 0970 7974 6573 742d 636f  mock...pytest-co
+000005c0: 760d 0a09 7079 7465 7374 2d72 756e 6e65  v...pytest-runne
+000005d0: 720d 0a09 7079 7465 7374 2d72 616e 646f  r...pytest-rando
+000005e0: 6d6c 790d 0a09 7079 7465 7374 2d73 7065  mly...pytest-spe
+000005f0: 630d 0a09 636f 7665 7261 6765 0d0a 0d0a  c...coverage....
+00000600: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
+00000610: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
+00000620: 7465 203d 2030 0d0a 0d0a                 te = 0....
```

### Comparing `v_quantum_annealing-0.0.0/setup.py` & `v_quantum_annealing-0.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,18 +22,21 @@
 setup_requires = [
     "numpy",
     "pybind11 >=2.10.0, < 2.11.0",
     "cmake > 3.20",
     "scikit-build > 0.16.0"
 ]
 
-if any(arg in sys.argv for arg in ("pytest", "test")):
-    setup_requires.append("pytest-runner")
+__version__ = "0.0.1"
 
 setup(
+    name="v_quantum_annealing", 
+    version=__version__,  
+    author = "V-QUANTUM JSC",
+    author_email = "nqthinh@v-quantum-technology.com",
     setup_requires=setup_requires,
     packages=[
         "v_quantum_annealing",
         "v_quantum_annealing.model",
         "v_quantum_annealing.sampler",
         "v_quantum_annealing.sampler.chimera_gpu",
         "v_quantum_annealing.utils",
```

### Comparing `v_quantum_annealing-0.0.0/tests/CMakeLists.txt` & `v_quantum_annealing-0.0.1/tests/CMakeLists.txt`

 * *Files 20% similar despite different names*

```diff
@@ -10,45 +10,45 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 #include(GoogleTest)
 
-add_executable(cxxjij_test
+add_executable(cxxvqa_test
     cxxtest/cxxtest.cpp
 )
 
 if(ENABLE_COVERAGE AND (NOT MSVC))
-  add_coverage(cxxjij_test)
+  add_coverage(cxxvqa_test)
 endif()
 
 if(CUDAToolkit_FOUND)
-    set_target_properties(cxxjij_test PROPERTIES
+    set_target_properties(cxxvqa_test PROPERTIES
         CXX_VISIBILITY_PRESET "hidden"
         INTERPROCEDURAL_OPTIMIZATION TRUE
         POSITION_INDEPENDENT_CODE ON
         CUDA_VISIBILITY_PRESET "hidden"
         CUDA_SEPARABLE_COMPILATION ON
     )
 endif()
 
-target_include_directories(cxxjij_test PRIVATE
+target_include_directories(cxxvqa_test PRIVATE
   ${CMAKE_CURRENT_SOURCE_DIR}
 )
 
-target_compile_definitions(cxxjij_test PRIVATE
+target_compile_definitions(cxxvqa_test PRIVATE
     BUILD_TESTING=OFF
 )
 
-target_link_libraries(cxxjij_test PRIVATE
+target_link_libraries(cxxvqa_test PRIVATE
     nlohmann_json::nlohmann_json
-    cxxjij_header_only
+    cxxvqa_header_only
     $<IF:$<TARGET_EXISTS:Eigen3::Eigen>,Eigen3::Eigen,openjij-eigen_lib>
     $<IF:$<TARGET_EXISTS:GTest::gtest>,GTest::gtest,gtest>
     $<IF:$<TARGET_EXISTS:GTest::gtest_main>,GTest::gtest_main,gtest_main>
     $<IF:$<TARGET_EXISTS:GTest::gmock>,GTest::gmock,gmock>
     $<IF:$<TARGET_EXISTS:GTest::gmock_main>,GTest::gmock_main,gmock_main>
-    $<$<TARGET_EXISTS:cxxjij_chimera_gpu_kernel>:cxxjij_chimera_gpu_kernel>
+    $<$<TARGET_EXISTS:cxxvqa_chimera_gpu_kernel>:cxxvqa_chimera_gpu_kernel>
 )
 
-gtest_discover_tests(cxxjij_test)
+gtest_discover_tests(cxxvqa_test)
```

### Comparing `v_quantum_annealing-0.0.0/tests/__pycache__/test_cxx.cpython-39-pytest-7.3.1.pyc` & `v_quantum_annealing-0.0.1/tests/__pycache__/test_cxx.cpython-39-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/__pycache__/test_hubo.cpython-39-pytest-7.3.1.pyc` & `v_quantum_annealing-0.0.1/tests/__pycache__/test_hubo.cpython-39-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/__pycache__/test_model.cpython-39-pytest-7.3.1.pyc` & `v_quantum_annealing-0.0.1/tests/__pycache__/test_model.cpython-39-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/__pycache__/test_sampler.cpython-39-pytest-7.3.1.pyc` & `v_quantum_annealing-0.0.1/tests/__pycache__/test_sampler.cpython-39-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/__pycache__/test_sqa.cpython-39-pytest-7.3.1.pyc` & `v_quantum_annealing-0.0.1/tests/__pycache__/test_sqa.cpython-39-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/__pycache__/test_utils.cpython-39-pytest-7.3.1.pyc` & `v_quantum_annealing-0.0.1/tests/__pycache__/test_utils.cpython-39-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/cxxtest.cpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/cxxtest.cpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/graph/all.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/graph/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/graph/binary_polynomial_model.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/graph/binary_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/graph/ising_polynomial_model.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/graph/ising_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/graph/polynomial.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/graph/polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/graph/quadratic.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/graph/quadratic.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/polynomial_test.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/polynomial_test.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/result/all.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/result/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/result/result.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/result/result.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/sampler/all.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/sampler/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/sampler/binary_polynomial_sa_sampler.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/sampler/binary_polynomial_sa_sampler.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/sampler/gpu.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/sampler/gpu.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/sampler/ising_polynomial_sa_sampler.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/sampler/ising_polynomial_sa_sampler.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/sampler/k_local.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/sampler/k_local.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/sampler/polynomial.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/sampler/polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/sampler/quadraitc.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/sampler/quadraitc.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/sampler/swendsen_wang.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/sampler/swendsen_wang.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/system/all.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/system/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/system/binary_polynomial_sa_system.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/system/binary_polynomial_sa_system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/system/classical_ising.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/system/classical_ising.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/system/classical_ising_polynomial.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/system/classical_ising_polynomial.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/system/ising_polynomial_sa_system.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/system/ising_polynomial_sa_system.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/system/k_local.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/system/k_local.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/testcase.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/testcase.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/utility/all.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/utility/all.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/utility/eigen.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/utility/eigen.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/utility/gpu.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/utility/gpu.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/cxxtest/utility/union_find.hpp` & `v_quantum_annealing-0.0.1/tests/cxxtest/utility/union_find.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/test_cxx.py` & `v_quantum_annealing-0.0.1/tests/test_cxx.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/test_gpu.py` & `v_quantum_annealing-0.0.1/tests/test_gpu.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/test_hubo.py` & `v_quantum_annealing-0.0.1/tests/test_hubo.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/test_model.py` & `v_quantum_annealing-0.0.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/test_sampler.py` & `v_quantum_annealing-0.0.1/tests/test_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/test_sqa.py` & `v_quantum_annealing-0.0.1/tests/test_sqa.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/tests/test_utils.py` & `v_quantum_annealing-0.0.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/CMakeLists.txt` & `v_quantum_annealing-0.0.1/v_quantum_annealing/CMakeLists.txt`

 * *Files 20% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-message(CHECK_START "cxxjij")
+message(CHECK_START "cxxvqa")
 list(APPEND CMAKE_MESSAGE_INDENT "  ")
 
-message(STATUS "Build cxxjij")
+message(STATUS "Build cxxvqa")
 
-set(python_module_name cxxjij)
+set(python_module_name cxxvqa)
 
 add_library(${python_module_name} MODULE main.cpp)
 
 target_include_directories(${python_module_name} PRIVATE
   ${CMAKE_CURRENT_SOURCE_DIR}
 )
 
@@ -51,20 +51,20 @@
 endif()
 
 target_compile_definitions(${python_module_name} PRIVATE 
     PYTHON_VERSION_INFO=${PYTHON_VERSION_STRING}
 )
 
 target_link_libraries(${python_module_name}  PRIVATE
-      cxxjij_header_only
+      cxxvqa_header_only
       pybind11::module
       pybind11::thin_lto
       pybind11::windows_extras
       pybind11_json
       nlohmann_json::nlohmann_json
-      $<$<TARGET_EXISTS:cxxjij_chimera_gpu_kernel_static>:cxxjij_chimera_gpu_kernel_static>
+      $<$<TARGET_EXISTS:cxxvqa_chimera_gpu_kernel_static>:cxxvqa_chimera_gpu_kernel_static>
 )
 
 install(TARGETS ${python_module_name} LIBRARY DESTINATION .)
 
 list(POP_BACK CMAKE_MESSAGE_INDENT)
 message(CHECK_PASS "Finished")
```

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/__init__.py` & `v_quantum_annealing-0.0.1/v_quantum_annealing/__init__.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/compile_config.hpp` & `v_quantum_annealing-0.0.1/v_quantum_annealing/compile_config.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/declare.hpp` & `v_quantum_annealing-0.0.1/v_quantum_annealing/declare.hpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/main.cpp` & `v_quantum_annealing-0.0.1/v_quantum_annealing/main.cpp`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/model/__init__.py` & `v_quantum_annealing-0.0.1/v_quantum_annealing/model/__init__.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/model/chimera_model.py` & `v_quantum_annealing-0.0.1/v_quantum_annealing/model/chimera_model.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/model/king_graph.py` & `v_quantum_annealing-0.0.1/v_quantum_annealing/model/king_graph.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/model/model.py` & `v_quantum_annealing-0.0.1/v_quantum_annealing/model/model.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/sampler/__init__.py` & `v_quantum_annealing-0.0.1/v_quantum_annealing/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/sampler/base_sa_sample_hubo.py` & `v_quantum_annealing-0.0.1/v_quantum_annealing/sampler/base_sa_sample_hubo.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/sampler/chimera_gpu/base_gpu_chimera.py` & `v_quantum_annealing-0.0.1/v_quantum_annealing/sampler/chimera_gpu/base_gpu_chimera.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/sampler/chimera_gpu/gpu_sa_sampler.py` & `v_quantum_annealing-0.0.1/v_quantum_annealing/sampler/chimera_gpu/gpu_sa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/sampler/chimera_gpu/gpu_sqa_sampler.py` & `v_quantum_annealing-0.0.1/v_quantum_annealing/sampler/chimera_gpu/gpu_sqa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/sampler/csqa_sampler.py` & `v_quantum_annealing-0.0.1/v_quantum_annealing/sampler/csqa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/sampler/response.py` & `v_quantum_annealing-0.0.1/v_quantum_annealing/sampler/response.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/sampler/sa_sampler.py` & `v_quantum_annealing-0.0.1/v_quantum_annealing/sampler/sa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/sampler/sampler.py` & `v_quantum_annealing-0.0.1/v_quantum_annealing/sampler/sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/sampler/sqa_sampler.py` & `v_quantum_annealing-0.0.1/v_quantum_annealing/sampler/sqa_sampler.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/utils/__init__.py` & `v_quantum_annealing-0.0.1/v_quantum_annealing/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/utils/benchmark.py` & `v_quantum_annealing-0.0.1/v_quantum_annealing/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/utils/cxx_cast.py` & `v_quantum_annealing-0.0.1/v_quantum_annealing/utils/cxx_cast.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/utils/decorator.py` & `v_quantum_annealing-0.0.1/v_quantum_annealing/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/utils/graph_utils.py` & `v_quantum_annealing-0.0.1/v_quantum_annealing/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/utils/res_convertor.py` & `v_quantum_annealing-0.0.1/v_quantum_annealing/utils/res_convertor.py`

 * *Files identical despite different names*

### Comparing `v_quantum_annealing-0.0.0/v_quantum_annealing/variable_type.py` & `v_quantum_annealing-0.0.1/v_quantum_annealing/variable_type.py`

 * *Files identical despite different names*

