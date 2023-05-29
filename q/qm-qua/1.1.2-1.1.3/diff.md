# Comparing `tmp/qm_qua-1.1.2.tar.gz` & `tmp/qm_qua-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qm_qua-1.1.2.tar", max compression
+gzip compressed data, was "qm_qua-1.1.3.tar", max compression
```

## Comparing `qm_qua-1.1.2.tar` & `qm_qua-1.1.3.tar`

### file list

```diff
@@ -1,135 +1,135 @@
--rw-r--r--   0        0        0    13079 2023-05-11 10:31:12.068640 qm_qua-1.1.2/CHANGELOG.md
--rw-r--r--   0        0        0    14988 2023-05-11 10:31:12.068640 qm_qua-1.1.2/LICENSE
--rw-r--r--   0        0        0      453 2023-05-11 10:31:12.068640 qm_qua-1.1.2/README.md
--rw-r--r--   0        0        0     5346 2023-05-11 10:32:25.829000 qm_qua-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      210 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/QmJob.py
--rw-r--r--   0        0        0      247 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/QmPendingJob.py
--rw-r--r--   0        0        0      221 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/QmQueue.py
--rw-r--r--   0        0        0      307 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/QuaNodeVisitor.py
--rw-r--r--   0        0        0    34119 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/QuantumMachine.py
--rw-r--r--   0        0        0      295 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/QuantumMachinesManager.py
--rw-r--r--   0        0        0     2043 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/StreamMetadata.py
--rw-r--r--   0        0        0     9601 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/_QmJobErrors.py
--rw-r--r--   0        0        0     1629 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/__init__.py
--rw-r--r--   0        0        0      246 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/_controller.py
--rw-r--r--   0        0        0      316 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/_loc.py
--rw-r--r--   0        0        0     2446 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/_report.py
--rw-r--r--   0        0        0      483 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/_results.py
--rw-r--r--   0        0        0        0 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/api/__init__.py
--rw-r--r--   0        0        0     4549 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/base_api.py
--rw-r--r--   0        0        0    17062 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/frontend_api.py
--rw-r--r--   0        0        0      983 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/info_service_api.py
--rw-r--r--   0        0        0     8290 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/job_manager_api.py
--rw-r--r--   0        0        0     3500 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/job_result_api.py
--rw-r--r--   0        0        0        0 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/models/__init__.py
--rw-r--r--   0        0        0     1875 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/models/capabilities.py
--rw-r--r--   0        0        0      553 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/models/compiler.py
--rw-r--r--   0        0        0      484 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/models/debug_data.py
--rw-r--r--   0        0        0      749 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/models/devices.py
--rw-r--r--   0        0        0      252 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/models/info.py
--rw-r--r--   0        0        0      272 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/models/jobs.py
--rw-r--r--   0        0        0      170 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/models/quantum_machine.py
--rw-r--r--   0        0        0     1185 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/models/server_details.py
--rw-r--r--   0        0        0     4641 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/server_detector.py
--rw-r--r--   0        0        0     6424 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/simulation_api.py
--rw-r--r--   0        0        0        0 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/stubs/__init__.py
--rw-r--r--   0        0        0     2059 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/stubs/deprecated_job_manager_stub.py
--rw-r--r--   0        0        0      296 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/capabilities.py
--rw-r--r--   0        0        0        0 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/communication/__init__.py
--rw-r--r--   0        0        0     1076 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/communication/http_redirection.py
--rw-r--r--   0        0        0        0 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/containers/__init__.py
--rw-r--r--   0        0        0      866 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/containers/capabilities_container.py
--rw-r--r--   0        0        0     1980 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/datadog_api.py
--rw-r--r--   0        0        0        0 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/elements/__init__.py
--rw-r--r--   0        0        0     4307 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/elements/basic_element.py
--rw-r--r--   0        0        0     9739 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/elements/element_with_octave.py
--rw-r--r--   0        0        0     6528 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/elements/native_elements.py
--rw-r--r--   0        0        0     9540 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/elements_db.py
--rw-r--r--   0        0        0     2538 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-11 10:32:20.052966 qm_qua-1.1.2/qm/grpc/__init__.py
--rw-r--r--   0        0        0     2070 2023-05-11 10:32:20.052966 qm_qua-1.1.2/qm/grpc/compiler/__init__.py
--rw-r--r--   0        0        0     1054 2023-05-11 10:32:20.052966 qm_qua-1.1.2/qm/grpc/errors/__init__.py
--rw-r--r--   0        0        0    67465 2023-05-11 10:32:20.052966 qm_qua-1.1.2/qm/grpc/frontend/__init__.py
--rw-r--r--   0        0        0      723 2023-05-11 10:32:20.052966 qm_qua-1.1.2/qm/grpc/general_messages/__init__.py
--rw-r--r--   0        0        0     8255 2023-05-11 10:32:20.052966 qm_qua-1.1.2/qm/grpc/job_manager/__init__.py
--rw-r--r--   0        0        0     3128 2023-05-11 10:32:20.052966 qm_qua-1.1.2/qm/grpc/octave_models/__init__.py
--rw-r--r--   0        0        0     8463 2023-05-11 10:32:20.052966 qm_qua-1.1.2/qm/grpc/qm_api/__init__.py
--rw-r--r--   0        0        0     3735 2023-05-11 10:32:20.052966 qm_qua-1.1.2/qm/grpc/qm_manager/__init__.py
--rw-r--r--   0        0        0    31736 2023-05-11 10:32:20.052966 qm_qua-1.1.2/qm/grpc/qua/__init__.py
--rw-r--r--   0        0        0    20057 2023-05-11 10:32:20.052966 qm_qua-1.1.2/qm/grpc/qua_config/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 10:32:22.448980 qm_qua-1.1.2/qm/grpc/quantum_simulator/__init__.py
--rw-r--r--   0        0        0    11363 2023-05-11 10:32:22.448980 qm_qua-1.1.2/qm/grpc/quantum_simulator/v1/__init__.py
--rw-r--r--   0        0        0    22458 2023-05-11 10:32:20.052966 qm_qua-1.1.2/qm/grpc/results_analyser/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 10:32:24.572993 qm_qua-1.1.2/qm/io/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 10:32:24.572993 qm_qua-1.1.2/qm/io/qualang/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 10:32:24.572993 qm_qua-1.1.2/qm/io/qualang/api/__init__.py
--rw-r--r--   0        0        0     2363 2023-05-11 10:32:24.572993 qm_qua-1.1.2/qm/io/qualang/api/v1/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/jobs/__init__.py
--rw-r--r--   0        0        0     3617 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/jobs/base_job.py
--rw-r--r--   0        0        0     8871 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/jobs/job_queue.py
--rw-r--r--   0        0        0     3284 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/jobs/pending_job.py
--rw-r--r--   0        0        0       86 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/jobs/qm_job.py
--rw-r--r--   0        0        0     4412 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/jobs/running_qm_job.py
--rw-r--r--   0        0        0    10406 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/jobs/simulated_job.py
--rw-r--r--   0        0        0      395 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/logger.py
--rw-r--r--   0        0        0      781 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/logging_utils.py
--rw-r--r--   0        0        0      516 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/octave/__init__.py
--rw-r--r--   0        0        0     7763 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/octave/_calibration_config.py
--rw-r--r--   0        0        0    13378 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/octave/_calibration_program.py
--rw-r--r--   0        0        0     5618 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/octave/calibration_db.py
--rw-r--r--   0        0        0      675 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/octave/enums.py
--rw-r--r--   0        0        0    10320 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/octave/octave_config.py
--rw-r--r--   0        0        0    22068 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/octave/octave_manager.py
--rw-r--r--   0        0        0     9018 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/octave/qm_octave.py
--rw-r--r--   0        0        0     1905 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/persistence.py
--rw-r--r--   0        0        0    15425 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/program/ConfigBuilder.py
--rw-r--r--   0        0        0    17971 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/program/StatementsCollection.py
--rw-r--r--   0        0        0      235 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/program/_Program.py
--rw-r--r--   0        0        0     2915 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/program/_ResultAnalysis.py
--rw-r--r--   0        0        0      167 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/program/__init__.py
--rw-r--r--   0        0        0     1261 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/program/_execution_overrides_schema.py
--rw-r--r--   0        0        0    47831 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/program/_qua_config_schema.py
--rw-r--r--   0        0        0    23256 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/program/_qua_config_to_pb.py
--rw-r--r--   0        0        0     3372 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/program/_validate_config_schema.py
--rw-r--r--   0        0        0     4870 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/program/expressions.py
--rw-r--r--   0        0        0     3835 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/program/program.py
--rw-r--r--   0        0        0        0 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/py.typed
--rw-r--r--   0        0        0     3648 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/qua/AnalogMeasureProcess.py
--rw-r--r--   0        0        0      718 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/qua/DigitalMeasureProcess.py
--rw-r--r--   0        0        0       67 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/qua/__init__.py
--rw-r--r--   0        0        0   127669 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/qua/_dsl.py
--rw-r--r--   0        0        0     2755 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/qua/_type_hinting.py
--rw-r--r--   0        0        0    15150 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/qua/lib.py
--rw-r--r--   0        0        0    12834 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/quantum_machines_manager.py
--rw-r--r--   0        0        0      347 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/results/__init__.py
--rw-r--r--   0        0        0    13865 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/results/base_streaming_result_fetcher.py
--rw-r--r--   0        0        0     6051 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/results/multiple_streaming_result_fetcher.py
--rw-r--r--   0        0        0     2987 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/results/simulator_samples.py
--rw-r--r--   0        0        0     3236 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/results/single_streaming_result_fetcher.py
--rw-r--r--   0        0        0     8438 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/results/streaming_result_fetcher.py
--rw-r--r--   0        0        0        0 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/serialization/__init__.py
--rw-r--r--   0        0        0    14445 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/serialization/expression_serializing_visitor.py
--rw-r--r--   0        0        0     9577 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/serialization/generate_qua_script.py
--rw-r--r--   0        0        0     2068 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/serialization/qua_node_visitor.py
--rw-r--r--   0        0        0    25507 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/serialization/qua_serializing_visitor.py
--rw-r--r--   0        0        0      377 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/simulate/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/simulate/credentials.py
--rw-r--r--   0        0        0     3225 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/simulate/interface.py
--rw-r--r--   0        0        0     3549 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/simulate/loopback.py
--rw-r--r--   0        0        0     2896 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/simulate/raw.py
--rw-r--r--   0        0        0    14456 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/sources/logo_qm_square.png
--rw-r--r--   0        0        0      243 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/type_hinting/__init__.py
--rw-r--r--   0        0        0     4860 2023-05-11 10:31:12.364642 qm_qua-1.1.2/qm/type_hinting/config_types.py
--rw-r--r--   0        0        0      239 2023-05-11 10:31:12.364642 qm_qua-1.1.2/qm/type_hinting/exceution_overrides.py
--rw-r--r--   0        0        0      566 2023-05-11 10:31:12.364642 qm_qua-1.1.2/qm/type_hinting/general.py
--rw-r--r--   0        0        0     1929 2023-05-11 10:31:12.364642 qm_qua-1.1.2/qm/type_hinting/simulator_types.py
--rw-r--r--   0        0        0     5916 2023-05-11 10:31:12.364642 qm_qua-1.1.2/qm/user_config.py
--rw-r--r--   0        0        0      789 2023-05-11 10:31:12.364642 qm_qua-1.1.2/qm/utils/__init__.py
--rw-r--r--   0        0        0     1089 2023-05-11 10:31:12.364642 qm_qua-1.1.2/qm/utils/async_utils.py
--rw-r--r--   0        0        0     1559 2023-05-11 10:31:12.364642 qm_qua-1.1.2/qm/utils/deprecation_utils.py
--rw-r--r--   0        0        0     1906 2023-05-11 10:31:12.364642 qm_qua-1.1.2/qm/utils/general_utils.py
--rw-r--r--   0        0        0      945 2023-05-11 10:31:12.364642 qm_qua-1.1.2/qm/utils/protobuf_utils.py
--rw-r--r--   0        0        0     2614 2023-05-11 10:31:12.364642 qm_qua-1.1.2/qm/utils/types_utils.py
--rw-r--r--   0        0        0       22 2023-05-11 10:32:25.829000 qm_qua-1.1.2/qm/version.py
--rw-r--r--   0        0        0    36595 2023-05-11 10:31:12.364642 qm_qua-1.1.2/qm/waveform_report.py
--rw-r--r--   0        0        0     1684 1970-01-01 00:00:00.000000 qm_qua-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    13597 2023-05-29 12:32:51.547130 qm_qua-1.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0    14988 2023-05-29 12:32:51.547130 qm_qua-1.1.3/LICENSE
+-rw-r--r--   0        0        0      453 2023-05-29 12:32:51.547130 qm_qua-1.1.3/README.md
+-rw-r--r--   0        0        0     5373 2023-05-29 12:34:02.080365 qm_qua-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      210 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/QmJob.py
+-rw-r--r--   0        0        0      247 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/QmPendingJob.py
+-rw-r--r--   0        0        0      221 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/QmQueue.py
+-rw-r--r--   0        0        0      307 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/QuaNodeVisitor.py
+-rw-r--r--   0        0        0    34481 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/QuantumMachine.py
+-rw-r--r--   0        0        0      295 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/QuantumMachinesManager.py
+-rw-r--r--   0        0        0     2043 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/StreamMetadata.py
+-rw-r--r--   0        0        0     9601 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/_QmJobErrors.py
+-rw-r--r--   0        0        0     1629 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/__init__.py
+-rw-r--r--   0        0        0      246 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/_controller.py
+-rw-r--r--   0        0        0      316 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/_loc.py
+-rw-r--r--   0        0        0     2446 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/_report.py
+-rw-r--r--   0        0        0      483 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/_results.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/api/__init__.py
+-rw-r--r--   0        0        0     4549 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/api/base_api.py
+-rw-r--r--   0        0        0    17062 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/api/frontend_api.py
+-rw-r--r--   0        0        0      983 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/api/info_service_api.py
+-rw-r--r--   0        0        0     8290 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/api/job_manager_api.py
+-rw-r--r--   0        0        0     3500 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/api/job_result_api.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/api/models/__init__.py
+-rw-r--r--   0        0        0     1875 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/api/models/capabilities.py
+-rw-r--r--   0        0        0     1365 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/api/models/compiler.py
+-rw-r--r--   0        0        0      484 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/api/models/debug_data.py
+-rw-r--r--   0        0        0      749 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/api/models/devices.py
+-rw-r--r--   0        0        0      252 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/api/models/info.py
+-rw-r--r--   0        0        0      272 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/api/models/jobs.py
+-rw-r--r--   0        0        0      170 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/api/models/quantum_machine.py
+-rw-r--r--   0        0        0     1185 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/api/models/server_details.py
+-rw-r--r--   0        0        0     4641 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/api/server_detector.py
+-rw-r--r--   0        0        0     6424 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/api/simulation_api.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/api/stubs/__init__.py
+-rw-r--r--   0        0        0     2059 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/api/stubs/deprecated_job_manager_stub.py
+-rw-r--r--   0        0        0      296 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/capabilities.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/communication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/communication/http_redirection.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/containers/__init__.py
+-rw-r--r--   0        0        0      866 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/containers/capabilities_container.py
+-rw-r--r--   0        0        0     1980 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/datadog_api.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/elements/__init__.py
+-rw-r--r--   0        0        0     4307 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/elements/basic_element.py
+-rw-r--r--   0        0        0     9739 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/elements/element_with_octave.py
+-rw-r--r--   0        0        0     6528 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/elements/native_elements.py
+-rw-r--r--   0        0        0     9242 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/elements_db.py
+-rw-r--r--   0        0        0     2538 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:33:57.800278 qm_qua-1.1.3/qm/grpc/__init__.py
+-rw-r--r--   0        0        0     2070 2023-05-29 12:33:57.800278 qm_qua-1.1.3/qm/grpc/compiler/__init__.py
+-rw-r--r--   0        0        0     1054 2023-05-29 12:33:57.800278 qm_qua-1.1.3/qm/grpc/errors/__init__.py
+-rw-r--r--   0        0        0    67465 2023-05-29 12:33:57.800278 qm_qua-1.1.3/qm/grpc/frontend/__init__.py
+-rw-r--r--   0        0        0      723 2023-05-29 12:33:57.800278 qm_qua-1.1.3/qm/grpc/general_messages/__init__.py
+-rw-r--r--   0        0        0     8255 2023-05-29 12:33:57.800278 qm_qua-1.1.3/qm/grpc/job_manager/__init__.py
+-rw-r--r--   0        0        0     3128 2023-05-29 12:33:57.804278 qm_qua-1.1.3/qm/grpc/octave_models/__init__.py
+-rw-r--r--   0        0        0     8463 2023-05-29 12:33:57.804278 qm_qua-1.1.3/qm/grpc/qm_api/__init__.py
+-rw-r--r--   0        0        0     3735 2023-05-29 12:33:57.804278 qm_qua-1.1.3/qm/grpc/qm_manager/__init__.py
+-rw-r--r--   0        0        0    31736 2023-05-29 12:33:57.804278 qm_qua-1.1.3/qm/grpc/qua/__init__.py
+-rw-r--r--   0        0        0    20057 2023-05-29 12:33:57.804278 qm_qua-1.1.3/qm/grpc/qua_config/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:33:59.612315 qm_qua-1.1.3/qm/grpc/quantum_simulator/__init__.py
+-rw-r--r--   0        0        0    11363 2023-05-29 12:33:59.612315 qm_qua-1.1.3/qm/grpc/quantum_simulator/v1/__init__.py
+-rw-r--r--   0        0        0    22458 2023-05-29 12:33:57.804278 qm_qua-1.1.3/qm/grpc/results_analyser/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:34:01.244348 qm_qua-1.1.3/qm/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:34:01.244348 qm_qua-1.1.3/qm/io/qualang/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:34:01.244348 qm_qua-1.1.3/qm/io/qualang/api/__init__.py
+-rw-r--r--   0        0        0     2363 2023-05-29 12:34:01.244348 qm_qua-1.1.3/qm/io/qualang/api/v1/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/jobs/__init__.py
+-rw-r--r--   0        0        0     3617 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/jobs/base_job.py
+-rw-r--r--   0        0        0     8871 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/jobs/job_queue.py
+-rw-r--r--   0        0        0     3284 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/jobs/pending_job.py
+-rw-r--r--   0        0        0       86 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/jobs/qm_job.py
+-rw-r--r--   0        0        0     4412 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/jobs/running_qm_job.py
+-rw-r--r--   0        0        0    10406 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/jobs/simulated_job.py
+-rw-r--r--   0        0        0      395 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/logger.py
+-rw-r--r--   0        0        0      781 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/logging_utils.py
+-rw-r--r--   0        0        0      516 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/octave/__init__.py
+-rw-r--r--   0        0        0     7763 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/octave/_calibration_config.py
+-rw-r--r--   0        0        0    13378 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/octave/_calibration_program.py
+-rw-r--r--   0        0        0     5618 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/octave/calibration_db.py
+-rw-r--r--   0        0        0      675 2023-05-29 12:32:51.791135 qm_qua-1.1.3/qm/octave/enums.py
+-rw-r--r--   0        0        0    11385 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/octave/octave_config.py
+-rw-r--r--   0        0        0    21634 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/octave/octave_manager.py
+-rw-r--r--   0        0        0     9018 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/octave/qm_octave.py
+-rw-r--r--   0        0        0     1905 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/persistence.py
+-rw-r--r--   0        0        0    15739 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/program/ConfigBuilder.py
+-rw-r--r--   0        0        0    17971 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/program/StatementsCollection.py
+-rw-r--r--   0        0        0      235 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/program/_Program.py
+-rw-r--r--   0        0        0     2915 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/program/_ResultAnalysis.py
+-rw-r--r--   0        0        0      167 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/program/__init__.py
+-rw-r--r--   0        0        0     1261 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/program/_execution_overrides_schema.py
+-rw-r--r--   0        0        0    47997 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/program/_qua_config_schema.py
+-rw-r--r--   0        0        0    23410 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/program/_qua_config_to_pb.py
+-rw-r--r--   0        0        0     3584 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/program/_validate_config_schema.py
+-rw-r--r--   0        0        0     4870 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/program/expressions.py
+-rw-r--r--   0        0        0     3835 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/program/program.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/py.typed
+-rw-r--r--   0        0        0     3648 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/qua/AnalogMeasureProcess.py
+-rw-r--r--   0        0        0      718 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/qua/DigitalMeasureProcess.py
+-rw-r--r--   0        0        0       67 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/qua/__init__.py
+-rw-r--r--   0        0        0   127669 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/qua/_dsl.py
+-rw-r--r--   0        0        0     2755 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/qua/_type_hinting.py
+-rw-r--r--   0        0        0    15150 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/qua/lib.py
+-rw-r--r--   0        0        0    12994 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/quantum_machines_manager.py
+-rw-r--r--   0        0        0      347 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/results/__init__.py
+-rw-r--r--   0        0        0    13865 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/results/base_streaming_result_fetcher.py
+-rw-r--r--   0        0        0     6051 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/results/multiple_streaming_result_fetcher.py
+-rw-r--r--   0        0        0     2987 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/results/simulator_samples.py
+-rw-r--r--   0        0        0     3236 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/results/single_streaming_result_fetcher.py
+-rw-r--r--   0        0        0     8438 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/results/streaming_result_fetcher.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/serialization/__init__.py
+-rw-r--r--   0        0        0    14445 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/serialization/expression_serializing_visitor.py
+-rw-r--r--   0        0        0     9577 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/serialization/generate_qua_script.py
+-rw-r--r--   0        0        0     2068 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/serialization/qua_node_visitor.py
+-rw-r--r--   0        0        0    25507 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/serialization/qua_serializing_visitor.py
+-rw-r--r--   0        0        0      377 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/simulate/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/simulate/credentials.py
+-rw-r--r--   0        0        0     3225 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/simulate/interface.py
+-rw-r--r--   0        0        0     3549 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/simulate/loopback.py
+-rw-r--r--   0        0        0     2896 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/simulate/raw.py
+-rw-r--r--   0        0        0    14456 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/sources/logo_qm_square.png
+-rw-r--r--   0        0        0      243 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/type_hinting/__init__.py
+-rw-r--r--   0        0        0     4860 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/type_hinting/config_types.py
+-rw-r--r--   0        0        0      239 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/type_hinting/exceution_overrides.py
+-rw-r--r--   0        0        0      566 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/type_hinting/general.py
+-rw-r--r--   0        0        0     1929 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/type_hinting/simulator_types.py
+-rw-r--r--   0        0        0     5916 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/user_config.py
+-rw-r--r--   0        0        0      789 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/utils/__init__.py
+-rw-r--r--   0        0        0     1089 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/utils/async_utils.py
+-rw-r--r--   0        0        0     1559 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/utils/deprecation_utils.py
+-rw-r--r--   0        0        0     1906 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/utils/general_utils.py
+-rw-r--r--   0        0        0      945 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/utils/protobuf_utils.py
+-rw-r--r--   0        0        0     2614 2023-05-29 12:32:51.795135 qm_qua-1.1.3/qm/utils/types_utils.py
+-rw-r--r--   0        0        0       22 2023-05-29 12:34:02.080365 qm_qua-1.1.3/qm/version.py
+-rw-r--r--   0        0        0    36748 2023-05-29 12:32:51.799135 qm_qua-1.1.3/qm/waveform_report.py
+-rw-r--r--   0        0        0     1730 1970-01-01 00:00:00.000000 qm_qua-1.1.3/PKG-INFO
```

### Comparing `qm_qua-1.1.2/CHANGELOG.md` & `qm_qua-1.1.3/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
-## Unreleased
+## 1.1.3 - 2023-05-29
+### Fixed
+- Fixed negative IF freq handling in config builder
+- Sticky Element duration is to be given in ns and not clock cycles
+- Fixed a bug that prevents opening many QMMs/QMs due to thread exhaustion when creating Octave clients. 
+- The deprecated `strict` and `flags` arguments now work but give a deprecation warning. 
+- Fixed the version of typing-extensions, to prevent import-error
+
+
+## 1.1.2 - 2023-05-11
 ### Deprecation
 - Moved `qm.QuantumMachinesManager.QuantumMachinesManager` path to `qm.quantum_machines_manager.QuantumMachinesManager`. Old path will be removed in 1.2.0
 
 ### Added
 - Added `qmm.validate_qua_config()` for config validation without opening a qm
 - :guardswoman: Added support for getting clusters by name in `QuantumMachinesManager` 
 - Added a `py.typed` file, that marks the package as supporting type-hints.
@@ -20,19 +29,19 @@
 - Float frequency support - fixed the creation of config classes so integer frequency will always exist
 - Fixed creating a mixer dict-config from protobuf class instance
 - Fixed error raised when fetching saved data in the backwards compatible
 - Fixed creating a digital port dict-config from protobuf class instance
 - Fixed event-loop Windows bug of creating multiple instances of QuantumMachine
 
 
-## [1.1.1] - 2023-03-20
+## 1.1.1 - 2023-03-20
 ### Fixed
 - Fixed long delay while waiting for values
 
-## [1.1.0] - 2023-03-16
+## 1.1.0 - 2023-03-16
 
 ### Deprecation
 - The `hold_offset` entry in the config is deprecated and is replaced by a new `sticky` entry with an improved API
 - Moved `_Program` path to `qm.program.program.Program`. Old path will be removed in 1.2.0
 - Moved `QmJob` path to `qm.jobs.qm_job.QmJob`. Old path will be removed in 1.2.0
 - Moved `QmPendingJob` path to `qm.jobs.pending_job.QmPendingJob`. Old path will be removed in 1.2.0
 - Moved `QmQueue` path to `qm.jobs.job_queue.QmQueue`. Old path will be removed in 1.2.0
@@ -44,14 +53,15 @@
 - `QuantumMachine` no longer has `manager` property
 - `QuantumMachine.peek` is removed (was never implemented)
 - `QuantumMachine.poke` is removed (was never implemented)
 - `IsInt()` function for qua variables is deprecated, use `is_int()` instead, will be removed in 1.2.0
 - `IsFixed()` function for qua variables is deprecated, use `is_fixed()` instead, will be removed in 1.2.0 
 - `IsBool()` function for qua variables is deprecated, use `is_bool()` instead, will be removed in 1.2.0 
 - `set_clock` method of the octave changed API, old API will be removed in 1.2.0.
+- Deprecated the `strict` and `flags` kwargs arguments in the `execute` and `simulate` functions.
 
 ### Added
 - Added auto correction for config dict in IDEs, when creating a config, add the following: `config: DictQuaConfig = {...}`.
 - :guardswoman: Added the option to invert the digital markers in a quantum machine by indicating it in the config.
 - :guardswoman: Support `fast_frame_rotation`, a frame rotation with a cosine and sine rotation matrix rather than an angle.  
 - Added support for floating point numbers in the `intermediate_frequency` field of `element` .
 - :guardswoman: Conditional `play` is extended to both the digital pulse if defined for operation.
```

### Comparing `qm_qua-1.1.2/LICENSE` & `qm_qua-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/pyproject.toml` & `qm_qua-1.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qm-qua"
-version = "1.1.2"
+version = "1.1.3"
 description = "QUA language SDK to control a Quantum Computer"
 readme = "README.md"
 authors = ["Quantum Machines <info@quantum-machines.co>"]
 
 packages = [
     { include = "qm" },
     { include = "qm/py.typed" }
@@ -26,14 +26,15 @@
 numpy = "^1.17.0"
 tinydb = "^4.6.1"
 certifi = { version = "*", optional = true }
 datadog-api-client = "^2.6.0"
 deprecation = "^2.1.0"
 dependency_injector = "^4.41.0"
 qm-octave = "^1.1.0"
+typing-extensions = "^4.5"
 
 grpclib = { version = "^0.4.3rc3", python = "^3.10", allow-prereleases = true }
 plotly = "^5.13.0"
 httpx = { version = "^0.23.3", extras = ["http2"] }
 
 [tool.poetry.dev-dependencies]
 grpcio = "1.39.0"
```

### Comparing `qm_qua-1.1.2/qm/QuantumMachine.py` & `qm_qua-1.1.3/qm/QuantumMachine.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from qm.jobs.running_qm_job import RunningQmJob
 from qm.api.job_manager_api import JobManagerApi
 from qm.octave.octave_manager import OctaveManager
 from qm.simulate.interface import SimulationConfig
 from qm.elements_db import ElementsDB, init_elements
 from qm.utils.types_utils import convert_object_type
 from qm.api.models.capabilities import ServerCapabilities
-from qm.api.models.compiler import CompilerOptionArguments
+from qm.api.models.compiler import CompilerOptionArguments, standardize_compiler_params
 from qm.program.ConfigBuilder import convert_msg_to_config
 from qm._QmJobErrors import InvalidDigitalInputPolarityError
 from qm.elements.element_with_octave import ElementWithOctave
 from qm.type_hinting.config_types import DictQuaConfig, PortReferenceType, DigitalInputPortConfigType
 from qm.type_hinting.general import Value, Number, PathLike, NumpySupportedFloat, NumpySupportedValue
 from qm.elements.native_elements import MixInputsElement, SingleInputElement, static_set_mixer_correction
 from qm.exceptions import (
@@ -130,14 +130,17 @@
         return self._frontend.close_quantum_machine(self._id)
 
     def simulate(
         self,
         program: Program,
         simulate: SimulationConfig,
         compiler_options: Optional[CompilerOptionArguments] = None,
+        *,
+        strict: Optional[bool] = None,
+        flags: Optional[List[str]] = None,
     ) -> SimulatedJob:
         """Simulate the outputs of a deterministic QUA program.
 
         Equivalent to ``execute()`` with ``simulate=SimulationConfig`` (see example).
 
         Note:
             A simulated job does not support calling QuantumMachine API functions.
@@ -163,28 +166,32 @@
             program: A QUA ``program()`` object to execute
             simulate: A ``SimulationConfig`` configuration object
             kwargs: additional parameteres to pass to execute
 
         Returns:
             a ``QmJob`` object (see QM Job API).
         """
+        standardized_compiler_options = standardize_compiler_params(compiler_options, strict, flags)
         job: SimulatedJob = cast(
-            SimulatedJob, self.execute(program, simulate=simulate, compiler_options=compiler_options)
+            SimulatedJob, self.execute(program, simulate=simulate, compiler_options=standardized_compiler_options)
         )
         return job
 
     def execute(
         self,
         program: Program,
         duration_limit: int = 1000,
         data_limit: int = 20000,
         force_execution: int = False,
         dry_run: int = False,
         simulate: Optional[SimulationConfig] = None,
         compiler_options: Optional[CompilerOptionArguments] = None,
+        *,
+        strict: Optional[bool] = None,
+        flags: Optional[List[str]] = None,
     ) -> RunningQmJob:
         """Executes a program and returns an job object to keep track of execution and get
         results.
 
         Note:
 
             Calling execute will halt any currently running program and clear the current
@@ -206,35 +213,34 @@
         if type(program) is not Program:
             raise Exception("program argument must be of type qm.program.Program")
         if program.metadata.uses_command_timestamps and not self._capabilities.supports_command_timestamps:
             raise UnsupportedCapabilityError("timestamping commands is supported from QOP 2.2 or above")
         if program.metadata.uses_fast_frame_rotation and not self._capabilities.supports_fast_frame_rotation:
             raise UnsupportedCapabilityError("fast frame rotation is supported from QOP 2.2 or above")
 
-        if compiler_options is None:
-            compiler_options = CompilerOptionArguments()
+        standardized_compiler_options = standardize_compiler_params(compiler_options, strict, flags)
 
         if simulate is not None:
             job_id, simulated_response_part = self._simulation_api.simulate(
-                self.get_config(), program, simulate, compiler_options
+                self.get_config(), program, simulate, standardized_compiler_options
             )
             return SimulatedJob(
                 job_id=job_id,
                 frontend_api=self._frontend,
                 capabilities=self._capabilities,
                 store=self._store,
                 simulated_response=simulated_response_part,
             )
 
         self._queue.clear()
         current_running_job = self.get_running_job()
         if current_running_job is not None:
             current_running_job.halt()
 
-        pending_job = self._queue.add(program, compiler_options)
+        pending_job = self._queue.add(program, standardized_compiler_options)
         logger.info("Executing program")
         return pending_job.wait_for_execution(timeout=5)
 
     def compile(
         self,
         program: Program,
         compiler_options: Optional[CompilerOptionArguments] = None,
```

### Comparing `qm_qua-1.1.2/qm/StreamMetadata.py` & `qm_qua-1.1.3/qm/StreamMetadata.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/_QmJobErrors.py` & `qm_qua-1.1.3/qm/_QmJobErrors.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/__init__.py` & `qm_qua-1.1.3/qm/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/_report.py` & `qm_qua-1.1.3/qm/_report.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/api/base_api.py` & `qm_qua-1.1.3/qm/api/base_api.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/api/frontend_api.py` & `qm_qua-1.1.3/qm/api/frontend_api.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/api/info_service_api.py` & `qm_qua-1.1.3/qm/api/info_service_api.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/api/job_manager_api.py` & `qm_qua-1.1.3/qm/api/job_manager_api.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/api/job_result_api.py` & `qm_qua-1.1.3/qm/api/job_result_api.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/api/models/capabilities.py` & `qm_qua-1.1.3/qm/api/models/capabilities.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/api/models/devices.py` & `qm_qua-1.1.3/qm/api/models/devices.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/api/models/server_details.py` & `qm_qua-1.1.3/qm/api/models/server_details.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/api/server_detector.py` & `qm_qua-1.1.3/qm/api/server_detector.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/api/simulation_api.py` & `qm_qua-1.1.3/qm/api/simulation_api.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/api/stubs/deprecated_job_manager_stub.py` & `qm_qua-1.1.3/qm/api/stubs/deprecated_job_manager_stub.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/communication/http_redirection.py` & `qm_qua-1.1.3/qm/communication/http_redirection.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/containers/capabilities_container.py` & `qm_qua-1.1.3/qm/containers/capabilities_container.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/datadog_api.py` & `qm_qua-1.1.3/qm/datadog_api.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/elements/basic_element.py` & `qm_qua-1.1.3/qm/elements/basic_element.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/elements/element_with_octave.py` & `qm_qua-1.1.3/qm/elements/element_with_octave.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/elements/native_elements.py` & `qm_qua-1.1.3/qm/elements/native_elements.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/elements_db.py` & `qm_qua-1.1.3/qm/elements_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     QuaConfig,
     QuaConfigMixInputs,
     QuaConfigSingleInput,
     QuaConfigMultipleInputs,
     QuaConfigDacPortReference,
     QuaConfigSingleInputCollection,
 )
+from qm.octave.octave_config import get_device
 
 MaybeOctaveInputPort = Optional[OctaveIfInputPort]
 
 
 class ElementNotFound(KeyError):
     def __init__(self, key: str):
         self._key = key
@@ -122,15 +123,14 @@
     return ElementsDB(elements)
 
 
 class _OctavesContainer:
     def __init__(self, pb_config: QuaConfig, octave_config: Optional[QmOctaveConfig] = None):
         self._pb_config = pb_config
         self._octave_config = octave_config or QmOctaveConfig()
-        self._octave_clients_cache: Dict[str, Octave] = {}
 
     def _get_connections_to_octave(self, element_port: QuaConfigDacPortReference) -> MaybeOctaveInputPort:
         controller, number = element_port.controller, element_port.number
         controller_config = self._pb_config.v1_beta.controllers[controller]
         connection = controller_config.analog_outputs[number].octave_connectivity
         if betterproto.serialized_on_wire(connection):
             return connection
@@ -204,21 +204,12 @@
             client=client,
             octave_if_input_port_number=int(i_octave_input_port.port_name.name[-1]),
             downconversion_client=downconversion_client,
             octave_rf_input_port_number=downconversion_port_number,
         )
 
     def _get_octave_client(self, device_name: str) -> Octave:
-        if device_name in self._octave_clients_cache:
-            return self._octave_clients_cache[device_name]
-
         device_connection_info = self._octave_config.devices[device_name]
         loopbacks = self._get_loopbacks(device_name)
-        client = Octave(
-            host=device_connection_info.host,
-            port=device_connection_info.port,
-            port_mapping=loopbacks,
-            octave_name=device_name,
-            fan=self._octave_config.fan,
+        return get_device(
+            device_connection_info, loop_backs=loopbacks, octave_name=device_name, fan=self._octave_config.fan
         )
-        self._octave_clients_cache[device_name] = client
-        return client
```

### Comparing `qm_qua-1.1.2/qm/exceptions.py` & `qm_qua-1.1.3/qm/exceptions.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/grpc/compiler/__init__.py` & `qm_qua-1.1.3/qm/grpc/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/grpc/errors/__init__.py` & `qm_qua-1.1.3/qm/grpc/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/grpc/frontend/__init__.py` & `qm_qua-1.1.3/qm/grpc/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/grpc/general_messages/__init__.py` & `qm_qua-1.1.3/qm/grpc/general_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/grpc/job_manager/__init__.py` & `qm_qua-1.1.3/qm/grpc/job_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/grpc/octave_models/__init__.py` & `qm_qua-1.1.3/qm/grpc/octave_models/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/grpc/qm_api/__init__.py` & `qm_qua-1.1.3/qm/grpc/qm_api/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/grpc/qm_manager/__init__.py` & `qm_qua-1.1.3/qm/grpc/qm_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/grpc/qua/__init__.py` & `qm_qua-1.1.3/qm/grpc/qua/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/grpc/qua_config/__init__.py` & `qm_qua-1.1.3/qm/grpc/qua_config/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/grpc/quantum_simulator/v1/__init__.py` & `qm_qua-1.1.3/qm/grpc/quantum_simulator/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/grpc/results_analyser/__init__.py` & `qm_qua-1.1.3/qm/grpc/results_analyser/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/io/qualang/api/v1/__init__.py` & `qm_qua-1.1.3/qm/io/qualang/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/jobs/base_job.py` & `qm_qua-1.1.3/qm/jobs/base_job.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/jobs/job_queue.py` & `qm_qua-1.1.3/qm/jobs/job_queue.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/jobs/pending_job.py` & `qm_qua-1.1.3/qm/jobs/pending_job.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/jobs/running_qm_job.py` & `qm_qua-1.1.3/qm/jobs/running_qm_job.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/jobs/simulated_job.py` & `qm_qua-1.1.3/qm/jobs/simulated_job.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/logging_utils.py` & `qm_qua-1.1.3/qm/logging_utils.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/octave/__init__.py` & `qm_qua-1.1.3/qm/octave/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/octave/_calibration_config.py` & `qm_qua-1.1.3/qm/octave/_calibration_config.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/octave/_calibration_program.py` & `qm_qua-1.1.3/qm/octave/_calibration_program.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/octave/calibration_db.py` & `qm_qua-1.1.3/qm/octave/calibration_db.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/octave/enums.py` & `qm_qua-1.1.3/qm/octave/enums.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/octave/octave_config.py` & `qm_qua-1.1.3/qm/octave/octave_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import re
 import logging
 import warnings
 import dataclasses
+from functools import lru_cache
 from typing import Dict, List, Tuple, Union, Generic, TypeVar, Optional
 
 from deprecation import deprecated
-from octave_sdk import OctaveOutput, OctaveLOSource
+from octave_sdk import OctaveOutput, OctaveLOSource, Octave
 
 from qm.octave.calibration_db import CalibrationDB
 
 logger = logging.getLogger(__name__)
 
 ConnectionMapping = Dict[Tuple[str, int], Tuple[str, str]]
 
@@ -71,23 +72,53 @@
         return 5
 
 
 def _convert_number_to_octave_port(name: str, port: int) -> List:
     return [(name, f"I{port}"), (name, f"Q{port}")]
 
 
+@lru_cache(maxsize=None)
+def _cached_get_device(
+    connection_info: ConnectionInfo, loop_backs: Tuple[Tuple[OctaveLOSource, OctaveOutput], ...], octave_name: str
+) -> Octave:
+    loop_backs = {input_port: output_port for input_port, output_port in loop_backs}
+    return Octave(
+        host=connection_info.host,
+        port=connection_info.port,
+        port_mapping=loop_backs,
+        octave_name=octave_name,
+    )
+
+
+def get_device(
+    connection_info: ConnectionInfo, loop_backs: Dict[OctaveLOSource, OctaveOutput], octave_name: str, fan=None
+) -> Octave:
+    client = _cached_get_device(connection_info, loop_backs=tuple(sorted(loop_backs.items())), octave_name=octave_name)
+    if fan is not None:
+        client._set_fan(fan)
+    return client
+
+
 class QmOctaveConfig:
     def __init__(self, fan=None) -> None:
         self._devices: Dict[str, ConnectionInfo] = {}
         self._calibration_db_path: Optional[str] = None
         self._loopbacks: Optional[Dict[LoopbackInfo[OctaveLOSource], LoopbackInfo[OctaveOutput]]] = None
         self._opx_octave_port_mapping: Optional[ConnectionMapping] = None
         self._calibration_db: Optional[CalibrationDB] = None
         self._fan = fan
 
+    def get_device(self, device_name):
+        return get_device(
+            connection_info=self._devices[device_name],
+            loop_backs=self.get_lo_loopbacks_by_octave(device_name),
+            octave_name=device_name,
+            fan=self._fan,
+        )
+
     @property
     def fan(self):
         return self._fan
 
     def add_device_info(self, name: str, host: str, port: int):
         """Sets the octave info  - the IP address can be either the router ip or the actual ip
         depends on the installation configuration (cluster or standalone mode)
```

### Comparing `qm_qua-1.1.2/qm/octave/octave_manager.py` & `qm_qua-1.1.3/qm/octave/octave_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,24 +175,16 @@
     def _initialize(self):
         self._octave_clients: Dict[str, Octave] = {}
         devices = self._octave_config.get_devices()
 
         if devices is not None and len(devices) > 0:
             if not OCTAVE_SDK_LOADED:
                 raise OctaveSDKException("Octave sdk is not installed")
-            for device_name, connection_info in devices.items():
-                loop_backs = self._octave_config.get_lo_loopbacks_by_octave(device_name)
-                loop_backs = {input_port: output_port for input_port, output_port in loop_backs.items()}
-                self._octave_clients[device_name] = Octave(
-                    host=connection_info.host,
-                    port=connection_info.port,
-                    port_mapping=loop_backs,
-                    octave_name=device_name,
-                    fan=self._octave_config.fan,
-                )
+            for device_name in devices:
+                self._octave_clients[device_name] = self._octave_config.get_device(device_name)
 
     def set_octave_configuration(self, config: QmOctaveConfig):
         """Args:
         config
         """
         self._check_and_set_config(config)
         self._initialize()
```

### Comparing `qm_qua-1.1.2/qm/octave/qm_octave.py` & `qm_qua-1.1.3/qm/octave/qm_octave.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/persistence.py` & `qm_qua-1.1.3/qm/persistence.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/program/ConfigBuilder.py` & `qm_qua-1.1.3/qm/program/ConfigBuilder.py`

 * *Files 3% similar despite different names*

```diff
@@ -302,17 +302,23 @@
         if "timeOfFlight" in data:
             element_config_data["time_of_flight"] = int(data["timeOfFlight"])
 
         if "smearing" in data:
             element_config_data["smearing"] = int(data["smearing"])
 
         if "intermediateFrequencyOscillatorDouble" in data:
-            element_config_data["intermediate_frequency"] = float(data["intermediateFrequencyOscillatorDouble"])
+            freq = float(data["intermediateFrequencyOscillatorDouble"])
+            if "intermediateFrequencyNegative" in data and bool(data["intermediateFrequencyNegative"]):
+                freq = -freq
+            element_config_data["intermediate_frequency"] = freq
         elif "intermediateFrequencyOscillator" in data:
-            element_config_data["intermediate_frequency"] = float(data["intermediateFrequencyOscillator"])
+            freq = float(data["intermediateFrequencyOscillator"])
+            if "intermediateFrequencyNegative" in data and bool(data["intermediateFrequencyNegative"]):
+                freq = -freq
+            element_config_data["intermediate_frequency"] = freq
         elif "namedOscillator" in data:
             element_config_data["oscillator"] = str(data["namedOscillator"])
         elif "intermediateFrequencyDouble" in data:
             freq = float(data["intermediateFrequencyDouble"])
             if "intermediateFrequencyNegative" in data and bool(data["intermediateFrequencyNegative"]):
                 freq = -freq
             element_config_data["intermediate_frequency"] = freq
```

### Comparing `qm_qua-1.1.2/qm/program/StatementsCollection.py` & `qm_qua-1.1.3/qm/program/StatementsCollection.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/program/_ResultAnalysis.py` & `qm_qua-1.1.3/qm/program/_ResultAnalysis.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/program/_execution_overrides_schema.py` & `qm_qua-1.1.3/qm/program/_execution_overrides_schema.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/program/_qua_config_schema.py` & `qm_qua-1.1.3/qm/program/_qua_config_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     octave_connection_to_pb,
 )
 from qm.program._validate_config_schema import (
     validate_oscillator,
     validate_output_tof,
     validate_used_inputs,
     validate_output_smearing,
+    validate_sticky_duration,
     validate_arbitrary_waveform,
     validate_timetagging_parameters,
 )
 
 logger = logging.getLogger(__name__)
 
 
@@ -798,15 +799,15 @@
     class Meta:
         title = "Sticky"
         description = "When defined, makes the element sticky"
 
     @post_load(pass_many=False)
     def build(self, data, **kwargs):
         item = qua_config.QuaConfigSticky()
-        item.duration = data.get("duration", 1)
+        item.duration = data.get("duration", 4)
         item.analog = data.get("analog")
         if "digital" in data:
             item.digital = data.get("digital")
         return item
 
 
 class MixInputSchema(Schema):
@@ -1060,22 +1061,24 @@
                         qua_config.QuaConfigOutputPulseParametersPolarity.ASCENDING
                     )
                 elif polarity == "BELOW" or polarity == "DESCENDING":
                     el.output_pulse_parameters.derivative_polarity = (
                         qua_config.QuaConfigOutputPulseParametersPolarity.DESCENDING
                     )
         if "sticky" in data:
+            validate_sticky_duration(data["sticky"].duration)
             if capabilities.supports_sticky_elements:
                 el.sticky = data["sticky"]
+                el.sticky.duration = int(el.sticky.duration / 4)
             else:
                 if data["sticky"].digital:
                     raise ConfigValidationException(
                         f"Server does not support digital sticky used in element " f"'{el}'"
                     )
-                el.hold_offset = qua_config.QuaConfigHoldOffset(duration=data["sticky"].duration)
+                el.hold_offset = qua_config.QuaConfigHoldOffset(duration=int(data["sticky"].duration / 4))
 
         elif "hold_offset" in data:
             if capabilities.supports_sticky_elements:
                 el.sticky = qua_config.QuaConfigSticky(
                     analog=True, digital=False, duration=data["hold_offset"].duration
                 )
             else:
```

### Comparing `qm_qua-1.1.2/qm/program/_qua_config_to_pb.py` & `qm_qua-1.1.3/qm/program/_qua_config_to_pb.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from qm.api.models.capabilities import ServerCapabilities
 from qm.containers.capabilities_container import CapabilitiesContainer
 from qm.program._validate_config_schema import (
     validate_oscillator,
     validate_output_tof,
     validate_used_inputs,
     validate_output_smearing,
+    validate_sticky_duration,
     validate_arbitrary_waveform,
     validate_timetagging_parameters,
 )
 
 
 class OctaveConnectionAmbiguity(Exception):
     def __str__(self):
@@ -410,26 +411,28 @@
 
     if "oscillator" in data:
         element.named_oscillator = data["oscillator"]
     elif "intermediate_frequency" not in data:
         element.no_oscillator = Empty()
 
     if "sticky" in data:
+        if "duration" in data["sticky"]:
+            validate_sticky_duration(data["sticky"]["duration"])
         if capabilities.supports_sticky_elements:
             element.sticky = qua_config.QuaConfigSticky(
                 analog=data["sticky"].get("analog", True),
                 digital=data["sticky"].get("digital", False),
-                duration=data["sticky"].get("duration", 1),
+                duration=int(data["sticky"].get("duration", 4) / 4),
             )
         else:
             if "digital" in data["sticky"] and data["sticky"]["digital"]:
                 raise ConfigValidationException(
                     f"Server does not support digital sticky used in element " f"'{element_name}'"
                 )
-            element.hold_offset = qua_config.QuaConfigHoldOffset(duration=data["sticky"].get("duration", 1))
+            element.hold_offset = qua_config.QuaConfigHoldOffset(duration=int(data["sticky"].get("duration", 4) / 4))
 
     elif "hold_offset" in data:
         if capabilities.supports_sticky_elements:
             element.sticky = qua_config.QuaConfigSticky(
                 analog=True,
                 digital=False,
                 duration=data["hold_offset"].get("duration", 1),
```

### Comparing `qm_qua-1.1.2/qm/program/_validate_config_schema.py` & `qm_qua-1.1.3/qm/program/_validate_config_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,22 @@
     if len(used_inputs) > 1:
         raise ValidationError(
             f"Can't support more than a single input type. " f"Used {', '.join(used_inputs)}",
             field_name="",
         )
 
 
+def validate_sticky_duration(duration):
+    if (duration % 4) != 0:
+        raise ValidationError(
+            "Sticky's element duration must be a dividable by 4",
+            field_name="duration",
+        )
+
+
 def validate_arbitrary_waveform(is_overridable, has_max_allowed_error, has_sampling_rate):
     if is_overridable and has_max_allowed_error:
         raise ValidationError("Overridable waveforms cannot have property 'max_allowed_error'")
     if is_overridable and has_sampling_rate:
         raise ValidationError("Overridable waveforms cannot have property 'sampling_rate_key'")
     if has_max_allowed_error and has_sampling_rate:
         raise ValidationError("Cannot use both 'max_allowed_error' and 'sampling_rate'")
```

### Comparing `qm_qua-1.1.2/qm/program/expressions.py` & `qm_qua-1.1.3/qm/program/expressions.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/program/program.py` & `qm_qua-1.1.3/qm/program/program.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/qua/AnalogMeasureProcess.py` & `qm_qua-1.1.3/qm/qua/AnalogMeasureProcess.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/qua/DigitalMeasureProcess.py` & `qm_qua-1.1.3/qm/qua/DigitalMeasureProcess.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/qua/_dsl.py` & `qm_qua-1.1.3/qm/qua/_dsl.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/qua/_type_hinting.py` & `qm_qua-1.1.3/qm/qua/_type_hinting.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/qua/lib.py` & `qm_qua-1.1.3/qm/qua/lib.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/quantum_machines_manager.py` & `qm_qua-1.1.3/qm/quantum_machines_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from qm.api.server_detector import detect_server
 from qm.octave.octave_manager import OctaveManager
 from qm.simulate.interface import SimulationConfig
 from qm.persistence import BaseStore, SimpleFileStore
 from qm.api.models.server_details import ServerDetails
 from qm.type_hinting.config_types import DictQuaConfig
 from qm.program._qua_config_to_pb import load_config_pb
-from qm.api.models.compiler import CompilerOptionArguments
+from qm.api.models.compiler import CompilerOptionArguments, standardize_compiler_params
 from qm.octave.calibration_db import load_from_calibration_db
 from qm.exceptions import QmmException, ConfigValidationException
 from qm.program._qua_config_schema import validate_config_capabilities
 from qm.containers.capabilities_container import create_capabilities_container
 
 logger = logging.getLogger(__name__)
 
@@ -71,17 +71,14 @@
             logger.error(message)
             raise QmmException(message)
 
         self._credentials = credentials
         self._cluster_name = cluster_name
         self._store = store if store else SimpleFileStore(file_store_root)
 
-        self._octave_config = octave
-        self._octave_manager = OctaveManager(octave, self)
-
         self._server_details = self._initialize_connection(
             timeout=timeout,
             add_debug_data=add_debug_data,
             connection_headers=connection_headers,
         )
 
         self._caps = self._server_details.capabilities
@@ -246,14 +243,17 @@
 
     def simulate(
         self,
         config: DictQuaConfig,
         program: Program,
         simulate: SimulationConfig,
         compiler_options: Optional[CompilerOptionArguments] = None,
+        *,
+        strict: Optional[bool] = None,
+        flags: Optional[List[str]] = None,
     ) -> SimulatedJob:
         """Simulate the outputs of a deterministic QUA program.
 
         The following example shows a simple execution of the simulator, where the
         associated config object is omitted for brevity.
 
         Example:
@@ -268,23 +268,23 @@
 
             job = qmm.simulate(config, prog, SimulationConfig(duration=100))
             ```
         Args:
             config: A QM config
             program: A QUA ``program()`` object to execute
             simulate: A ``SimulationConfig`` configuration object
-            kwargs: additional parameters to pass to execute
+            compiler_options: additional parameters to pass to execute
+            strict: a deprecated option for the compiler
+            flags: deprecated way to provide flags to the compiler
 
         Returns:
             a ``QmJob`` object (see QM Job API).
         """
-        if compiler_options is None:
-            compiler_options = CompilerOptionArguments()
-
-        job_id, simulated_response_part = self._simulation_api.simulate(config, program, simulate, compiler_options)
+        standardized_options = standardize_compiler_params(compiler_options, strict, flags)
+        job_id, simulated_response_part = self._simulation_api.simulate(config, program, simulate, standardized_options)
         return SimulatedJob(
             job_id=job_id,
             frontend_api=self._frontend,
             capabilities=self._server_details.capabilities,
             store=self._store,
             simulated_response=simulated_response_part,
         )
```

### Comparing `qm_qua-1.1.2/qm/results/base_streaming_result_fetcher.py` & `qm_qua-1.1.3/qm/results/base_streaming_result_fetcher.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/results/multiple_streaming_result_fetcher.py` & `qm_qua-1.1.3/qm/results/multiple_streaming_result_fetcher.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/results/simulator_samples.py` & `qm_qua-1.1.3/qm/results/simulator_samples.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/results/single_streaming_result_fetcher.py` & `qm_qua-1.1.3/qm/results/single_streaming_result_fetcher.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/results/streaming_result_fetcher.py` & `qm_qua-1.1.3/qm/results/streaming_result_fetcher.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/serialization/expression_serializing_visitor.py` & `qm_qua-1.1.3/qm/serialization/expression_serializing_visitor.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/serialization/generate_qua_script.py` & `qm_qua-1.1.3/qm/serialization/generate_qua_script.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/serialization/qua_node_visitor.py` & `qm_qua-1.1.3/qm/serialization/qua_node_visitor.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/serialization/qua_serializing_visitor.py` & `qm_qua-1.1.3/qm/serialization/qua_serializing_visitor.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/simulate/credentials.py` & `qm_qua-1.1.3/qm/simulate/credentials.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/simulate/interface.py` & `qm_qua-1.1.3/qm/simulate/interface.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/simulate/loopback.py` & `qm_qua-1.1.3/qm/simulate/loopback.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/simulate/raw.py` & `qm_qua-1.1.3/qm/simulate/raw.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/sources/logo_qm_square.png` & `qm_qua-1.1.3/qm/sources/logo_qm_square.png`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/type_hinting/config_types.py` & `qm_qua-1.1.3/qm/type_hinting/config_types.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/type_hinting/general.py` & `qm_qua-1.1.3/qm/type_hinting/general.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/type_hinting/simulator_types.py` & `qm_qua-1.1.3/qm/type_hinting/simulator_types.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/user_config.py` & `qm_qua-1.1.3/qm/user_config.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/utils/__init__.py` & `qm_qua-1.1.3/qm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/utils/async_utils.py` & `qm_qua-1.1.3/qm/utils/async_utils.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/utils/deprecation_utils.py` & `qm_qua-1.1.3/qm/utils/deprecation_utils.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/utils/general_utils.py` & `qm_qua-1.1.3/qm/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/utils/protobuf_utils.py` & `qm_qua-1.1.3/qm/utils/protobuf_utils.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/utils/types_utils.py` & `qm_qua-1.1.3/qm/utils/types_utils.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.2/qm/waveform_report.py` & `qm_qua-1.1.3/qm/waveform_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -825,29 +825,34 @@
             yanchor="bottom",
         )
         return
 
     def _setup_figure(self) -> None:
         self._figure = go.Figure()
         with_samples = self._samples is not None
-        num_rows = max(self._num_rows, 4)
+        minimum_number_of_rows = 4
+        num_rows = max(self._num_rows, minimum_number_of_rows)
         titles = [f"Analog-Out-{a}" for a in self._report.analog_output_ports_in_use()] + [
             f"Digital-Out-{d}" for d in self._report.digital_output_ports_in_use()
         ]
         if with_samples:
             zipped: List[Any] = list(zip(titles, [[]] * self._num_output_rows))
             titles: List[Any] = [item for z in zipped for item in z]  # type: ignore[no-redef]
         titles += [f"Analog-In-{a}" for a in self._report.adcs_ports_in_use()]
 
         if with_samples:
             specs = ([[{"t": 1.2 / (num_rows * 5)}]] + [[{"b": 1.2 / (num_rows * 5)}]]) * (
                 self._num_output_rows // 2
             ) + [[{"t": 1 / (num_rows * 4)}]] * len(self._report.adcs_ports_in_use())
         else:
             specs = [[{"t": 1 / (num_rows * 4)}]] * num_rows
+
+        if len(specs) < minimum_number_of_rows:
+            specs += [[{}]] * (4 - len(specs))
+
         self._figure.set_subplots(
             rows=num_rows,
             cols=1,
             subplot_titles=titles,
             vertical_spacing=0.1 / num_rows,
             specs=specs,
         )
```

### Comparing `qm_qua-1.1.2/PKG-INFO` & `qm_qua-1.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qm-qua
-Version: 1.1.2
+Version: 1.1.3
 Summary: QUA language SDK to control a Quantum Computer
 Author: Quantum Machines
 Author-email: info@quantum-machines.co
 Requires-Python: >=3.7,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,14 +22,15 @@
 Requires-Dist: marshmallow (>=3.0.0,<4.0.0)
 Requires-Dist: marshmallow-polyfield (>=5.7,<6.0)
 Requires-Dist: numpy (>=1.17.0,<2.0.0)
 Requires-Dist: plotly (>=5.13.0,<6.0.0)
 Requires-Dist: protobuf (>=3.17.3,<4.0.0)
 Requires-Dist: qm-octave (>=1.1.0,<2.0.0)
 Requires-Dist: tinydb (>=4.6.1,<5.0.0)
+Requires-Dist: typing-extensions (>=4.5,<5.0)
 Description-Content-Type: text/markdown
 
 
 # QM-QUA SDK
 
 QUA is a pulse-level language used to control a Quantum System.
 Read more about it and it's uses here: https://arxiv.org/abs/2303.03816
```

