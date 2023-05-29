# Comparing `tmp/pulsar_data_collection-0.1.1.tar.gz` & `tmp/pulsar_data_collection-0.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulsar_data_collection-0.1.1.tar", max compression
+gzip compressed data, was "pulsar_data_collection-0.2.0rc0.tar", max compression
```

## Comparing `pulsar_data_collection-0.1.1.tar` & `pulsar_data_collection-0.2.0rc0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     5768 2022-12-20 16:16:05.919927 pulsar_data_collection-0.1.1/README.md
--rw-r--r--   0        0        0        0 2022-12-20 16:16:05.919927 pulsar_data_collection-0.1.1/pulsar_data_collection/__init__.py
--rw-r--r--   0        0        0      117 2022-12-20 16:16:05.919927 pulsar_data_collection-0.1.1/pulsar_data_collection/data_capture/__init__.py
--rw-r--r--   0        0        0     7384 2022-12-20 16:16:05.919927 pulsar_data_collection-0.1.1/pulsar_data_collection/data_capture/data_capture.py
--rw-r--r--   0        0        0      324 2022-12-20 16:16:05.923927 pulsar_data_collection-0.1.1/pulsar_data_collection/data_capture/exceptions.py
--rw-r--r--   0        0        0        0 2022-12-20 16:16:05.923927 pulsar_data_collection-0.1.1/pulsar_data_collection/db_connectors/influxdb/__init__.py
--rw-r--r--   0        0        0      526 2022-12-20 16:16:05.923927 pulsar_data_collection-0.1.1/pulsar_data_collection/db_connectors/influxdb/config.py
--rw-r--r--   0        0        0     1372 2022-12-20 16:16:05.923927 pulsar_data_collection-0.1.1/pulsar_data_collection/db_connectors/influxdb/db_connection.py
--rw-r--r--   0        0        0     1047 2022-12-20 16:16:05.923927 pulsar_data_collection-0.1.1/pulsar_data_collection/db_connectors/influxdb/queries.py
--rw-r--r--   0        0        0     1391 2022-12-20 16:16:05.923927 pulsar_data_collection-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6909 1970-01-01 00:00:00.000000 pulsar_data_collection-0.1.1/setup.py
--rw-r--r--   0        0        0     6638 1970-01-01 00:00:00.000000 pulsar_data_collection-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-29 15:24:47.407213 pulsar_data_collection-0.2.0rc0/LICENSE
+-rw-r--r--   0        0        0     5204 2023-05-29 15:24:47.407213 pulsar_data_collection-0.2.0rc0/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 15:24:47.407213 pulsar_data_collection-0.2.0rc0/pulsar_data_collection/__init__.py
+-rw-r--r--   0        0        0       95 2023-05-29 15:24:47.407213 pulsar_data_collection-0.2.0rc0/pulsar_data_collection/config.py
+-rw-r--r--   0        0        0        0 2023-05-29 15:24:47.407213 pulsar_data_collection-0.2.0rc0/pulsar_data_collection/database_connectors/__init__.py
+-rw-r--r--   0        0        0      812 2023-05-29 15:24:47.407213 pulsar_data_collection-0.2.0rc0/pulsar_data_collection/database_connectors/database_actions.py
+-rw-r--r--   0        0        0     4385 2023-05-29 15:24:47.407213 pulsar_data_collection-0.2.0rc0/pulsar_data_collection/database_connectors/influxdb.py
+-rw-r--r--   0        0        0     2700 2023-05-29 15:24:47.407213 pulsar_data_collection-0.2.0rc0/pulsar_data_collection/models.py
+-rw-r--r--   0        0        0     1476 2023-05-29 15:24:47.407213 pulsar_data_collection-0.2.0rc0/pulsar_data_collection/pulse.py
+-rw-r--r--   0        0        0     1716 2023-05-29 15:24:47.407213 pulsar_data_collection-0.2.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     6177 1970-01-01 00:00:00.000000 pulsar_data_collection-0.2.0rc0/setup.py
+-rw-r--r--   0        0        0     5977 1970-01-01 00:00:00.000000 pulsar_data_collection-0.2.0rc0/PKG-INFO
```

### Comparing `pulsar_data_collection-0.1.1/README.md` & `pulsar_data_collection-0.2.0rc0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,147 +1,103 @@
 # pulsar_data_collection
 
-Pulsar data collection SDK is an open-source Python library for
-pushing/processing/collecting features, predictions and metadata. Works with different
-data storages, at this point InfluxDB is implemented.
+[![PyPI Latest Release](https://img.shields.io/pypi/v/pulsar-data-collection.svg)](https://pypi.org/project/pulsar-data-collection/)
+[![Package Status](https://img.shields.io/pypi/status/pulsar-data-collection.svg)](https://pypi.org/project/pulsar-data-collection/)
+[![License](https://img.shields.io/pypi/l/pulsar-data-collection.svg)](https://github.com/Rocket-Science-Development/pulsar_data_collection/blob/main/LICENSE)
+[![Coverage](https://codecov.io/github/pandas-dev/pandas/coverage.svg?branch=main)](https://codecov.io/gh/pandas-dev/pandas)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
-## Getting started
+## What is it?
 
-Install Pulsar Data Collection with pip:
-
-```bash
-python3 -m pip install --upgrade pip
-python3 -m pip install --upgrade pulsar-data-collection
-```
-
-### Components
+**pulsar-data-collection** is a package for collecting and pushing data (features, predictions, and metadata) from an inference/prediction Jupyter notebook or Python micro-service serving a ML model (Flask, FastAPI) to a Database. It aims to provide an easy and flexible way to log data point used to perform predictions, prediction, and other relevant metadate informing the context in which the model is perform its predection. Once this data is stored, it will be used to compute metrics in order to provide ML models monitoring using our [pulsar-metrics](https://github.com/Rocket-Science-Development/pulsar_metrics) package. Further demonstration on how these packages are leveraged can found in [pulsar-demo](https://github.com/Rocket-Science-Development/pulsar_demo).
 
-There are two core components in data collection SDK: storage engine and data capture.
-Right now storage engine implemented only for InfluxDb, it helps to make ingestion and digestion operations
-to the database.
-
-#### Data Capture
-
-`DataCapture` class helps to ingest dataset to database with needed parameters and needed format for future
-digestion and metrics calculation without any significant changes of data.
-
-It requires `storage_engine` (available only influxdb right now), `operation_type` (`DATABASE_OPERATION_TYPE_INSERT_PREDICTION`,
-`DATABASE_OPERATION_TYPE_METRICS`),  `login_url` (object of DatabaseLogin class) as input parameters.
-
-Operation type `DATABASE_OPERATION_TYPE_INSERT_PREDICTION` uses for any ingestion operations to the database.
-It requires additional parameters: `model_id`, `model_version`, `data_id`", `y_name`, `pred_name` what describes
-an input dataset.
-For operation type `DATABASE_OPERATION_TYPE_METRICS` what commonly uses for retrieving dataset ready for metrics
-calculation these parameters aren't required.
-
-The last and probably one the most important class to work with is `DataWithPrediction`.
-It requires two parameters as input: `prediction`, `data_points`. Where `prediction` is prediction value of the model,
-and `data_points` is features dataset. `Push` method of the `DataCapture` takes object of `DataWithPrediction` as
-required parameter, and after that makes ingestion operation to database with data transforming, like adding timestamp,
-changing name of prediction column in dataset, combining features with prediction into single dataset, creating
-influxdb unique cache, etc.
-
-List of methods of `DataCapture` class:
-
-- push(data: DataWithPrediction)
-- ingests data to the db after preprocessing it;
-- collect(filters: dict) - retrieves data from db;
-- collect_eval_timestamp - retrieves the newest timestamp in the database;
-- push_eval_timestamp(eval_df: df) - ingesting new one timestamp into db;
-- push_metrics(metrics_df: df) - ingesting metrics dataframe to the database after calculations
+We currently support writing to InfluxDB v2.6.1, support for other technologies is coming
 
-### Example usage
+## Main Features
 
-Initialize Database credentials:
+Here are just a few of the things that pandas does well:
 
-```python
-from pulsar_data_collection.data_capture import DatabaseLogin
-database_login = DatabaseLogin(db_host=<db_host>), db_port=<db_port>, db_user=<db_user>, db_password=<db_password>, protocol=<db_protocol>)
-```
+- Collect data related to a model's lifecycle in production, i.e, data points, predictions, and metadata
+- Can be used inside a Python inference micro-service or a Jupyter Notebook used to perform predictions
+- Easy and flexible interface that has the ability to integrate with provided support of storage solution as well as the ability to easily integrate with custom storage solutions.
+- Lightweight package to limit the impact on the inference/prediction service performance
 
-Initialize DataCapture class, depends on operation type use appropriate constant.
-For inserting data into the database:
+## Where to get it
 
-```python
-from pulsar_data_collection.data_capture import DataCapture, DATABASE_OPERATION_TYPE_INSERT_PREDICTION
+The source code is currently hosted on GitHub at: [https://github.com/Rocket-Science-Development/pulsar_data_collection](https://github.com/Rocket-Science-Development/pulsar_data_collection)
 
-dat_predict = DataWithPrediction(prediction=prediction, data_points=to_predict)
-
-dat_capture = DataCapture(
-    storage_engine="influxdb",
-    model_id=<model_id>,
-    model_version=<model_verstion>,
-    data_id=<data_id>,
-    y_name=<y_name>,
-    pred_name=<pred_name>,
-    operation_type=<operation_type>,
-    login_url=<database_login>,
-)
+Binary installers for the latest released version are available at the [Python Package Index (PyPI)](https://pypi.org/project/pulsar-data-collection/)
+Install Pulsar Data Collection with pip:
 
-dat_capture.push(dat_predict)
+```sh
+pip install pulsar-data-collection
 ```
 
-For collecting data from the database:
+### Example usage
 
 ```python
-from pulsar_data_collection.data_capture import DataCapture, DATABASE_OPERATION_TYPE_METRICS
-
-dat_capture = DataCapture(
+import pickle as pkl
+from datetime import datetime as dt
+from datetime import timezone
+from pathlib import Path
+
+import pandas as pd
+
+from pulsar_data_collection.models import DataWithPrediction, PulseParameters
+from pulsar_data_collection.pulse import Pulse
+
+# init paths
+model_path = Path("path_to_model")
+inference_dataset = pd.read_csv("path_of_data_for_prediction", header=0)
+reference_data = "path_or_location_reference_data_used_to_train_the_model"
+
+params = PulseParameters(
+    model_id="model_id",
+    model_version="model_version",
+    data_id="reference_data_id",
+    reference_data_storage=reference_data,
+    target_name="target_feature_name",
     storage_engine="influxdb",
-    operation_type=DATABASE_OPERATION_TYPE_METRICS,
-    login_url=database_login
+    timestamp_column_name="_time",
+    login={
+        "url": "url_influxdb",
+        "token": "mytoken",
+        "org": "pulsarml",
+        "bucket_name": "demo",
+    },
+    other_labels={"timezone": "EST", "reference_dataset": reference_data},
 )
 
-dat_capture.collect()
-```
+pulse = Pulse(data=params)
 
-Collection the newest prediction data what wasn't precessed
+pickle_model = pkl.load(open(model_path, "rb"))
+prediction_simple = pickle_model.predict(inference_dataset)
 
-```python
-# receiving the last period of data
-
-last_eval_timestamp = dat_capture.collect_eval_timestamp()
-
-# if last period exists, collecting only data what wasn't collected previously
-if last_eval_timestamp:
-    last_eval_timestamp_str = last_eval_timestamp.strftime('%Y-%m-%d %H:%M:%S')
-    db_df = pd.DataFrame(dat_capture.collect({"time": f">= '{last_eval_timestamp_str}'"}).get("prediction"))
-else:
-    db_df = pd.DataFrame(dat_capture.collect().get("prediction"))
-```
-
-Example of pushing calculated metrics:
-
-```python
-dat_capture.push_metrics(df_result_drift)
-```
-
-Example of pushing the timestamp when metrics were calculated:
+time = dt.now(timezone.utc).strftime("%Y-%m-%dT%H:%M:%SZ")
+capture_params = DataWithPrediction(
+    data_points=inference_dataset,
+    predictions=pd.DataFrame(prediction_simple, columns=["prediction"]),
+    timestamp=time,
+    features_names=inference_dataset.columns.tolist(),
+)
 
-```python
-dat_capture.push_eval_timestamp(eval_timestamp_df)
+pulse.capture_data(data=capture_params)
 ```
-TODO: add use cases of input dataframes: metrics, prediction, datapoint
 
 ## About [PulsarML](https://pulsar.ml/)
 
 PulsarML is a project helping with monitoring your models and gain powerful insights into its performance.
 
 We released two Open Source packages :
 
-- [pulsar-data-collection](https://github.com/Rocket-Science-Development/pulsar_data_collection) :  lightweight python SDK enabling data collection of features, predictions and metadata from an ML model serving code/micro-service
+- [pulsar-data-collection](https://github.com/Rocket-Science-Development/pulsar_data_collection) :  lightweight python package enabling data collection of features, predictions and metadata from an ML model serving code/micro-service
+
 - [pulsar-metrics](https://github.com/Rocket-Science-Development/pulsar_metrics) : library for evaluating and monitoring data and concept drift with an extensive set of metrics. It also offers the possibility to use custom metrics defined by the user.
 
 We also created [pulsar demo](https://github.com/Rocket-Science-Development/pulsar_demo) to display an example use-case showing how to leverage both packages to implement model monitoring and performance management.
 
 Want to interact with the community? join our [slack channel](https://pulsarml.slack.com)
 
 Powered by [Rocket Science Development](https://rocketscience.one/)
 
-## Contributing
-
-1. Fork this repository, develop, and test your changes
-2. open an issue
-3. Submit a pull request with a reference to the issue
-
-TODO: add use cases of input dataframes: metrics, prediction, datapoint
```

### Comparing `pulsar_data_collection-0.1.1/pyproject.toml` & `pulsar_data_collection-0.2.0rc0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 [tool.poetry]
 name = "pulsar-data-collection"
-version = "0.1.1"
+version = "0.2.0rc"
 description = "sdk enabling data collection from model serving code for our MPM solution"
 authors = [
     "Pulsar team <pulsar@data-rs.io>"
     ]
 readme = "README.md"
 homepage = "https://github.com/Rocket-Science-Development/pulsar_data_collection"
-license = "MIT"
+license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^1.4.2"
-pysqlite3 = "^0.4.7"
-SQLAlchemy = "^1.4.39"
-influxdb-client = {extras = ["ciso"], version = "^1.31.0"}
+influxdb-client = {extras = ["async"], version = "^1.36.1"}
 pydantic = "^1.6.2"
-influxdb = "5.3.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.3.0"
 isort = "^5.10.1"
 pre-commit = "^2.19.0"
 pytest = "^7.1.2"
-matplotlib = "^3.5.2"
 scikit-learn = "^1.1.1"
-jupyter = "^1.0.0"
-fastapi = "^0.88.0"
-uvicorn = "^0.20.0"
 flake8 = "^6.0.0"
 flake8-pyproject = "^1.2.1"
+pylint = "^2.15.10"
+mypy = "^0.991"
+bandit = "^1.7.4"
+pytest-mock = "^3.10.0"
+pytest-docker = "^1.0.1"
+python-dotenv = "^1.0.0"
+
 
 [tool.black]
 line-length = 130
 target-version = ['py36', 'py37', 'py38', 'py39']
 include = '\.pyi?$'
 extend-exclude = '''
 /(
@@ -57,10 +57,26 @@
 ignore = ['E231', 'E241']
 per-file-ignores = [
     '__init__.py:F401',
 ]
 max-line-length = 130
 count = true
 
+[tool.bandit]
+targets = ["pulsar_data_collection"]
+exclude_dirs = ["tests"]
+
+[tool.mypy]
+plugins = [ "pydantic.mypy",]
+
+[tool.pydantic-mypy]
+init_forbid_extra = true
+init_typed = true
+warn_required_dynamic_aliases = true
+warn_untyped_fields = true
+
+[tool.pytest.ini_options]
+pythonpath = [".", "pulsar_data_collection", "tests"]
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pulsar_data_collection-0.1.1/PKG-INFO` & `pulsar_data_collection-0.2.0rc0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,170 +1,123 @@
 Metadata-Version: 2.1
 Name: pulsar-data-collection
-Version: 0.1.1
+Version: 0.2.0rc0
 Summary: sdk enabling data collection from model serving code for our MPM solution
 Home-page: https://github.com/Rocket-Science-Development/pulsar_data_collection
-License: MIT
+License: Apache-2.0
 Author: Pulsar team
 Author-email: pulsar@data-rs.io
 Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: SQLAlchemy (>=1.4.39,<2.0.0)
-Requires-Dist: influxdb (==5.3.1)
-Requires-Dist: influxdb-client[ciso] (>=1.31.0,<2.0.0)
+Requires-Dist: influxdb-client[async] (>=1.36.1,<2.0.0)
 Requires-Dist: pandas (>=1.4.2,<2.0.0)
 Requires-Dist: pydantic (>=1.6.2,<2.0.0)
-Requires-Dist: pysqlite3 (>=0.4.7,<0.5.0)
 Description-Content-Type: text/markdown
 
 # pulsar_data_collection
 
-Pulsar data collection SDK is an open-source Python library for
-pushing/processing/collecting features, predictions and metadata. Works with different
-data storages, at this point InfluxDB is implemented.
+[![PyPI Latest Release](https://img.shields.io/pypi/v/pulsar-data-collection.svg)](https://pypi.org/project/pulsar-data-collection/)
+[![Package Status](https://img.shields.io/pypi/status/pulsar-data-collection.svg)](https://pypi.org/project/pulsar-data-collection/)
+[![License](https://img.shields.io/pypi/l/pulsar-data-collection.svg)](https://github.com/Rocket-Science-Development/pulsar_data_collection/blob/main/LICENSE)
+[![Coverage](https://codecov.io/github/pandas-dev/pandas/coverage.svg?branch=main)](https://codecov.io/gh/pandas-dev/pandas)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
-## Getting started
+## What is it?
 
-Install Pulsar Data Collection with pip:
-
-```bash
-python3 -m pip install --upgrade pip
-python3 -m pip install --upgrade pulsar-data-collection
-```
-
-### Components
+**pulsar-data-collection** is a package for collecting and pushing data (features, predictions, and metadata) from an inference/prediction Jupyter notebook or Python micro-service serving a ML model (Flask, FastAPI) to a Database. It aims to provide an easy and flexible way to log data point used to perform predictions, prediction, and other relevant metadate informing the context in which the model is perform its predection. Once this data is stored, it will be used to compute metrics in order to provide ML models monitoring using our [pulsar-metrics](https://github.com/Rocket-Science-Development/pulsar_metrics) package. Further demonstration on how these packages are leveraged can found in [pulsar-demo](https://github.com/Rocket-Science-Development/pulsar_demo).
 
-There are two core components in data collection SDK: storage engine and data capture.
-Right now storage engine implemented only for InfluxDb, it helps to make ingestion and digestion operations
-to the database.
-
-#### Data Capture
-
-`DataCapture` class helps to ingest dataset to database with needed parameters and needed format for future
-digestion and metrics calculation without any significant changes of data.
-
-It requires `storage_engine` (available only influxdb right now), `operation_type` (`DATABASE_OPERATION_TYPE_INSERT_PREDICTION`,
-`DATABASE_OPERATION_TYPE_METRICS`),  `login_url` (object of DatabaseLogin class) as input parameters.
-
-Operation type `DATABASE_OPERATION_TYPE_INSERT_PREDICTION` uses for any ingestion operations to the database.
-It requires additional parameters: `model_id`, `model_version`, `data_id`", `y_name`, `pred_name` what describes
-an input dataset.
-For operation type `DATABASE_OPERATION_TYPE_METRICS` what commonly uses for retrieving dataset ready for metrics
-calculation these parameters aren't required.
-
-The last and probably one the most important class to work with is `DataWithPrediction`.
-It requires two parameters as input: `prediction`, `data_points`. Where `prediction` is prediction value of the model,
-and `data_points` is features dataset. `Push` method of the `DataCapture` takes object of `DataWithPrediction` as
-required parameter, and after that makes ingestion operation to database with data transforming, like adding timestamp,
-changing name of prediction column in dataset, combining features with prediction into single dataset, creating
-influxdb unique cache, etc.
-
-List of methods of `DataCapture` class:
-
-- push(data: DataWithPrediction)
-- ingests data to the db after preprocessing it;
-- collect(filters: dict) - retrieves data from db;
-- collect_eval_timestamp - retrieves the newest timestamp in the database;
-- push_eval_timestamp(eval_df: df) - ingesting new one timestamp into db;
-- push_metrics(metrics_df: df) - ingesting metrics dataframe to the database after calculations
+We currently support writing to InfluxDB v2.6.1, support for other technologies is coming
 
-### Example usage
+## Main Features
 
-Initialize Database credentials:
+Here are just a few of the things that pandas does well:
 
-```python
-from pulsar_data_collection.data_capture import DatabaseLogin
-database_login = DatabaseLogin(db_host=<db_host>), db_port=<db_port>, db_user=<db_user>, db_password=<db_password>, protocol=<db_protocol>)
-```
+- Collect data related to a model's lifecycle in production, i.e, data points, predictions, and metadata
+- Can be used inside a Python inference micro-service or a Jupyter Notebook used to perform predictions
+- Easy and flexible interface that has the ability to integrate with provided support of storage solution as well as the ability to easily integrate with custom storage solutions.
+- Lightweight package to limit the impact on the inference/prediction service performance
 
-Initialize DataCapture class, depends on operation type use appropriate constant.
-For inserting data into the database:
+## Where to get it
 
-```python
-from pulsar_data_collection.data_capture import DataCapture, DATABASE_OPERATION_TYPE_INSERT_PREDICTION
+The source code is currently hosted on GitHub at: [https://github.com/Rocket-Science-Development/pulsar_data_collection](https://github.com/Rocket-Science-Development/pulsar_data_collection)
 
-dat_predict = DataWithPrediction(prediction=prediction, data_points=to_predict)
-
-dat_capture = DataCapture(
-    storage_engine="influxdb",
-    model_id=<model_id>,
-    model_version=<model_verstion>,
-    data_id=<data_id>,
-    y_name=<y_name>,
-    pred_name=<pred_name>,
-    operation_type=<operation_type>,
-    login_url=<database_login>,
-)
+Binary installers for the latest released version are available at the [Python Package Index (PyPI)](https://pypi.org/project/pulsar-data-collection/)
+Install Pulsar Data Collection with pip:
 
-dat_capture.push(dat_predict)
+```sh
+pip install pulsar-data-collection
 ```
 
-For collecting data from the database:
+### Example usage
 
 ```python
-from pulsar_data_collection.data_capture import DataCapture, DATABASE_OPERATION_TYPE_METRICS
-
-dat_capture = DataCapture(
+import pickle as pkl
+from datetime import datetime as dt
+from datetime import timezone
+from pathlib import Path
+
+import pandas as pd
+
+from pulsar_data_collection.models import DataWithPrediction, PulseParameters
+from pulsar_data_collection.pulse import Pulse
+
+# init paths
+model_path = Path("path_to_model")
+inference_dataset = pd.read_csv("path_of_data_for_prediction", header=0)
+reference_data = "path_or_location_reference_data_used_to_train_the_model"
+
+params = PulseParameters(
+    model_id="model_id",
+    model_version="model_version",
+    data_id="reference_data_id",
+    reference_data_storage=reference_data,
+    target_name="target_feature_name",
     storage_engine="influxdb",
-    operation_type=DATABASE_OPERATION_TYPE_METRICS,
-    login_url=database_login
+    timestamp_column_name="_time",
+    login={
+        "url": "url_influxdb",
+        "token": "mytoken",
+        "org": "pulsarml",
+        "bucket_name": "demo",
+    },
+    other_labels={"timezone": "EST", "reference_dataset": reference_data},
 )
 
-dat_capture.collect()
-```
+pulse = Pulse(data=params)
 
-Collection the newest prediction data what wasn't precessed
+pickle_model = pkl.load(open(model_path, "rb"))
+prediction_simple = pickle_model.predict(inference_dataset)
 
-```python
-# receiving the last period of data
-
-last_eval_timestamp = dat_capture.collect_eval_timestamp()
-
-# if last period exists, collecting only data what wasn't collected previously
-if last_eval_timestamp:
-    last_eval_timestamp_str = last_eval_timestamp.strftime('%Y-%m-%d %H:%M:%S')
-    db_df = pd.DataFrame(dat_capture.collect({"time": f">= '{last_eval_timestamp_str}'"}).get("prediction"))
-else:
-    db_df = pd.DataFrame(dat_capture.collect().get("prediction"))
-```
-
-Example of pushing calculated metrics:
-
-```python
-dat_capture.push_metrics(df_result_drift)
-```
-
-Example of pushing the timestamp when metrics were calculated:
+time = dt.now(timezone.utc).strftime("%Y-%m-%dT%H:%M:%SZ")
+capture_params = DataWithPrediction(
+    data_points=inference_dataset,
+    predictions=pd.DataFrame(prediction_simple, columns=["prediction"]),
+    timestamp=time,
+    features_names=inference_dataset.columns.tolist(),
+)
 
-```python
-dat_capture.push_eval_timestamp(eval_timestamp_df)
+pulse.capture_data(data=capture_params)
 ```
-TODO: add use cases of input dataframes: metrics, prediction, datapoint
 
 ## About [PulsarML](https://pulsar.ml/)
 
 PulsarML is a project helping with monitoring your models and gain powerful insights into its performance.
 
 We released two Open Source packages :
 
-- [pulsar-data-collection](https://github.com/Rocket-Science-Development/pulsar_data_collection) :  lightweight python SDK enabling data collection of features, predictions and metadata from an ML model serving code/micro-service
+- [pulsar-data-collection](https://github.com/Rocket-Science-Development/pulsar_data_collection) :  lightweight python package enabling data collection of features, predictions and metadata from an ML model serving code/micro-service
+
 - [pulsar-metrics](https://github.com/Rocket-Science-Development/pulsar_metrics) : library for evaluating and monitoring data and concept drift with an extensive set of metrics. It also offers the possibility to use custom metrics defined by the user.
 
 We also created [pulsar demo](https://github.com/Rocket-Science-Development/pulsar_demo) to display an example use-case showing how to leverage both packages to implement model monitoring and performance management.
 
 Want to interact with the community? join our [slack channel](https://pulsarml.slack.com)
 
 Powered by [Rocket Science Development](https://rocketscience.one/)
 
-## Contributing
-
-1. Fork this repository, develop, and test your changes
-2. open an issue
-3. Submit a pull request with a reference to the issue
-
-TODO: add use cases of input dataframes: metrics, prediction, datapoint
```

