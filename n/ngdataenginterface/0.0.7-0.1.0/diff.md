# Comparing `tmp/ngdataenginterface-0.0.7.tar.gz` & `tmp/ngdataenginterface-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngdataenginterface-0.0.7.tar", max compression
+gzip compressed data, was "ngdataenginterface-0.1.0.tar", max compression
```

## Comparing `ngdataenginterface-0.0.7.tar` & `ngdataenginterface-0.1.0.tar`

### file list

```diff
@@ -1,10 +1,15 @@
--rw-r--r--   0        0        0     2934 2023-05-24 21:21:18.472560 ngdataenginterface-0.0.7/README.md
--rw-r--r--   0        0        0      348 2023-05-24 21:21:18.472560 ngdataenginterface-0.0.7/ngdataenginterface/__init__.py
--rw-r--r--   0        0        0     3598 2023-05-24 21:21:18.472560 ngdataenginterface-0.0.7/ngdataenginterface/analytical.py
--rw-r--r--   0        0        0     3382 2023-05-24 21:21:18.472560 ngdataenginterface-0.0.7/ngdataenginterface/aws_interface.py
--rw-r--r--   0        0        0     2704 2023-05-24 21:21:18.472560 ngdataenginterface-0.0.7/ngdataenginterface/process.py
--rw-r--r--   0        0        0     1816 2023-05-24 21:21:18.472560 ngdataenginterface-0.0.7/ngdataenginterface/spark_manager.py
--rw-r--r--   0        0        0    12412 2023-05-24 21:21:18.472560 ngdataenginterface-0.0.7/ngdataenginterface/table.py
--rw-r--r--   0        0        0     2046 2023-05-24 21:21:18.472560 ngdataenginterface-0.0.7/ngdataenginterface/utils.py
--rw-r--r--   0        0        0      395 2023-05-24 21:21:18.472560 ngdataenginterface-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 ngdataenginterface-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     2934 2023-05-29 19:16:09.082496 ngdataenginterface-0.1.0/README.md
+-rw-r--r--   0        0        0      348 2023-05-29 19:16:09.082496 ngdataenginterface-0.1.0/ngdataenginterface/__init__.py
+-rw-r--r--   0        0        0     3808 2023-05-29 19:16:09.082496 ngdataenginterface-0.1.0/ngdataenginterface/analytical.py
+-rw-r--r--   0        0        0     3392 2023-05-29 19:16:09.082496 ngdataenginterface-0.1.0/ngdataenginterface/aws_interface.py
+-rw-r--r--   0        0        0     2704 2023-05-29 19:16:09.082496 ngdataenginterface-0.1.0/ngdataenginterface/process.py
+-rw-r--r--   0        0        0      517 2023-05-29 19:16:09.082496 ngdataenginterface-0.1.0/ngdataenginterface/scripts/__init__.py
+-rw-r--r--   0        0        0     2124 2023-05-29 19:16:09.082496 ngdataenginterface-0.1.0/ngdataenginterface/scripts/create_analytical_tables.py
+-rw-r--r--   0        0        0     1516 2023-05-29 19:16:09.082496 ngdataenginterface-0.1.0/ngdataenginterface/scripts/landing_to_raw.py
+-rw-r--r--   0        0        0     2015 2023-05-29 19:16:09.082496 ngdataenginterface-0.1.0/ngdataenginterface/scripts/raw_to_trusted.py
+-rw-r--r--   0        0        0     1508 2023-05-29 19:16:09.082496 ngdataenginterface-0.1.0/ngdataenginterface/scripts/trusted_to_analytics.py
+-rw-r--r--   0        0        0     1836 2023-05-29 19:16:09.083496 ngdataenginterface-0.1.0/ngdataenginterface/spark_manager.py
+-rw-r--r--   0        0        0    13389 2023-05-29 19:16:09.083496 ngdataenginterface-0.1.0/ngdataenginterface/table.py
+-rw-r--r--   0        0        0     2780 2023-05-29 19:16:09.083496 ngdataenginterface-0.1.0/ngdataenginterface/utils.py
+-rw-r--r--   0        0        0      395 2023-05-29 19:16:09.083496 ngdataenginterface-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 ngdataenginterface-0.1.0/PKG-INFO
```

### Comparing `ngdataenginterface-0.0.7/README.md` & `ngdataenginterface-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.7/ngdataenginterface/analytical.py` & `ngdataenginterface-0.1.0/ngdataenginterface/analytical.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,20 @@
         self.read = self._init_tables(
             read_params, date, aws_interface, spark_manager, overwrite
         )
         self.write = self._init_tables(
             write_params, date, aws_interface, spark_manager, overwrite
         )
         self.aggregation_function = aggregation_function
+        self.meta = {
+            "spark": spark_manager.spark,
+            "aws_interface": aws_interface,
+            "date": date,
+            "session_name": "analytical_tables"
+        }
         # Set up logging
         self.logger = logging.getLogger(__name__)
         self.logger.setLevel(log_level)  # Set the log level
 
     @staticmethod
     def _init_tables(
         params: Dict[str, dict],
@@ -65,37 +71,36 @@
     def prepare_inputs(self) -> None:
         """
         Prepare the inputs by reading data from the tables.
         """
         self.logger.info("Preparing inputs...")
         try:
             self.inputs = {
-                table_name: table.read_table()
-                for table_name, table in self.read.items()
+                table_name: {"df": table.read_table()} for table_name, table in self.read.items()
             }
             self.logger.debug(f"Prepared inputs: {self.inputs}")
         except Exception as e:
             self.logger.error(f"Failed to prepare inputs: {e}")
             raise e
         self.logger.info("Inputs prepared successfully.")
 
     def run(self) -> None:
         """
         Run the aggregation function and write the output back to the tables.
         """
         self.logger.info("Running the aggregation function...")
         try:
             self.prepare_inputs()
-            print("\ninputs: ", self.inputs, "\n")
-            print("\nagg:", self.aggregation_function, "\n")
-            self.output = self.aggregation_function(inputs=self.inputs)
+            # print("\ninputs: ", self.inputs, "\n")
+            # print("\nagg:", self.aggregation_function, "\n")
+            self.output = self.aggregation_function(inputs=self.inputs, meta = self.meta)
             self.logger.debug(f"Aggregation output: {self.output}")
-            print("\noutput2: ", self.output, "\n")
+            # print("\noutput2: ", self.output, "\n")
             for table_name, table in self.write.items():
-                print("\noutput: ", self.output[table_name], "\n")
+                # print("\noutput: ", self.output[table_name], "\n")
                 table.write_table(self.output[table_name])
             self.logger.info(
                 "Successfully ran the aggregation function and wrote output to tables."
             )
         except Exception as e:
             self.logger.error(f"Failed to run the aggregation function: {e}")
             raise e
```

### Comparing `ngdataenginterface-0.0.7/ngdataenginterface/aws_interface.py` & `ngdataenginterface-0.1.0/ngdataenginterface/aws_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import boto3
 import json
 import ast
 
 
 class AWSManager:
-    def __init__(self, region_name, aws_access_key_id, aws_secret_access_key):
+    def __init__(self, region_name, aws_access_key_id=None, aws_secret_access_key=None):
         self.s3_client = boto3.client(
             "s3",
             region_name=region_name,
             aws_access_key_id=aws_access_key_id,
             aws_secret_access_key=aws_secret_access_key,
         )
         self.s3_resource = boto3.resource(
```

### Comparing `ngdataenginterface-0.0.7/ngdataenginterface/process.py` & `ngdataenginterface-0.1.0/ngdataenginterface/process.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.7/ngdataenginterface/spark_manager.py` & `ngdataenginterface-0.1.0/ngdataenginterface/spark_manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pyspark import SQLContext
 from pyspark.sql import SparkSession
 from pyspark.conf import SparkConf
 
 
 class SparkManager:
-    def set_spark_config(self, name, aws_access_key_id, aws_secret_access_key):
+    def set_spark_config(self, name, aws_access_key_id=None, aws_secret_access_key=None):
         # Create a SparkConf object and set the application name
         config = SparkConf().setAppName(name)
 
         # Set the Parquet datetimeRebaseModeInRead, datetimeRebaseModeInWrite, and int96RebaseModeInWrite to "LEGACY"
         config.set("spark.sql.parquet.datetimeRebaseModeInRead", "LEGACY")
         config.set("spark.sql.parquet.datetimeRebaseModeInWrite", "LEGACY")
         config.set("spark.sql.parquet.int96RebaseModeInWrite", "LEGACY")
@@ -21,15 +21,15 @@
         # If the credentials are not provided, the Spark application will use the IAM role assigned to the EMR cluster
         if aws_access_key_id and aws_secret_access_key:
             config.set("spark.hadoop.fs.s3a.access.key", aws_access_key_id)
             config.set("spark.hadoop.fs.s3a.secret.key", aws_secret_access_key)
 
         return config
 
-    def __init__(self, aws_access_key_id, aws_secret_access_key, app_name):
+    def __init__(self, app_name, aws_access_key_id=None, aws_secret_access_key=None):
         # Set the Spark configuration based on the provided AWS credentials and application name
         conf = self.set_spark_config(
             name=app_name,
             aws_access_key_id=aws_access_key_id,
             aws_secret_access_key=aws_secret_access_key,
         )
         self.conf = conf
```

### Comparing `ngdataenginterface-0.0.7/ngdataenginterface/table.py` & `ngdataenginterface-0.1.0/ngdataenginterface/table.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 import json
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from dateutil.relativedelta import relativedelta
-
+from typing import Optional
 from pyspark import SQLContext
 from pyspark.sql.types import *
 from pyspark.sql.functions import lit
 from pyspark.sql import DataFrame
 
 from ngdataenginterface.aws_interface import AWSInterface
 from ngdataenginterface.spark_manager import SparkManager
@@ -29,30 +29,36 @@
 @dataclass
 class PathParams:
     env: str
     bucket_name: str
     object_path: str
     partition: str
     file_type: str
+    schema_path: Optional[str] = None
 
     def input_validation(self, data):
         # table validation
         assert "bucket_name" in data.keys(), "Couldn`t find `bucket_name` in path input"
         assert "object_path" in data.keys(), "Couldn`t find `object_path` in path input"
         assert "partition" in data.keys(), "Couldn`t find `partition` in path input"
         assert "file_type" in data.keys(), "Couldn`t find `file_type` in path input"
+        if self.schema_path is not None:
+            assert (
+                "schema_path" in data.keys()
+            ), "Couldn't find `schema_path` in path input"
 
     @classmethod
     def from_dict(cls, data: dict[str, str]):
         instance = cls(
             env=data["env"],
             bucket_name=data["bucket_name"],
             object_path=data["object_path"],
             partition=data["partition"],
             file_type=data["file_type"],
+            schema_path=data.get("schema_path"),
         )
 
         instance.input_validation(data)
         return instance
 
 
 @dataclass
@@ -172,25 +178,29 @@
         """
         Generate the path for the table.
 
         Returns:
             str: The table path.
         """
         logger.info("Generating table path.")
-        return f"{self.path.object_path}/table"
+        if self.path.schema_path is None:
+            return f"{self.path.object_path}/table"
+        return self.path.object_path
 
     def schema_path(self):
         """
         Generate the path for the schema.
 
         Returns:
             str: The schema path.
         """
         logger.info("Generating schema path.")
-        return f"{self.path.object_path}/schema.json"
+        if self.path.schema_path is None:
+            return f"{self.path.object_path}/schema.json"
+        return self.path.schema_path
 
     def table_path_with_partition(self):
         """
         Generate the table path with the partition.
 
         Returns:
             str: The table path with the partition.
@@ -249,17 +259,24 @@
             ValueError: If there is an issue retrieving or handling the schema.
         """
         logger.info("Retrieving schema.")
         logger.info("Bucket Name: %s", self.path.bucket_name)
         logger.info("Object Path: %s", self.schema_path())
 
         # Get the object from AWS S3 bucket
+        if self.path.schema_path is None:
+            bucket_name = self.path.bucket_name
+            object_path = self.schema_path()
+        else:
+            bucket_name = self.schema_path()["bucket_name"]  # type: ignore
+            object_path = self.schema_path()["object_path"]  # type: ignore
+
         schema_object = self.aws_interface.get_object_aws(
-            self.path.bucket_name,
-            self.schema_path(),
+            bucket_name,
+            object_path,
         )
 
         # Decode the object to string
         schema_str = schema_object.decode("utf8").replace("\n    ", "")
 
         try:
             # Convert the string to JSON
@@ -319,17 +336,22 @@
         Raises:
             ValueError: If there is an issue with putting the schema object to AWS S3.
         """
         # Get the PySpark schema from the DataFrame
         pyspark_schema = df.schema.jsonValue()
 
         try:
-            self.aws_interface.put_object_aws(
-                self.path.bucket_name, self.schema_path(), pyspark_schema
-            )
+            if self.path.schema_path is None:
+                bucket_name = self.path.bucket_name
+                object_path = self.schema_path()
+            else:
+                bucket_name = self.schema_path()["bucket_name"]  # type: ignore
+                object_path = self.schema_path()["object_path"]  # type: ignore
+
+            self.aws_interface.put_object_aws(bucket_name, object_path, pyspark_schema)
         except Exception as e:
             raise ValueError("Error writing schema: {}".format(str(e)))
 
     def delete_table_to_overwrite(self):
         """
         Delete the destination table if overwrite is set to True in the metadata.
 
@@ -374,15 +396,14 @@
         # Check if the table should be saved partitioned
         if partitions != [""]:
             for part in partitions:
                 # Add the partition column in the table
                 df = df.withColumn(part, lit(PARTITION_MAP[part](self.meta.date)))
             # Write the table partitioned
             df.write.partitionBy(partitions).mode("append").format(file_type).save(path)
-            print("\nescreveu:")
             # df.show()
         else:
             # Write the table without partition
             df.write.mode("append").format(file_type).save(path)
 
         # Write the schema
         try:
```

### Comparing `ngdataenginterface-0.0.7/ngdataenginterface/utils.py` & `ngdataenginterface-0.1.0/ngdataenginterface/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -53,7 +53,30 @@
 
 
 def handle_execution_date_args(dt: str):
     match = re.search(r"(?<=\.).+?(?=\:)", dt)
     if match:
         dt = dt.replace(f".{match.group()[:-3]}", "")
     return datetime.strptime("".join(dt.rsplit(":", 1)), "%Y-%m-%dT%H:%M:%S%z")
+
+
+def handle_input_api(env,read_params, ng_prefix = "ngcash"):
+        layer = read_params["layer"]
+        object_path = read_params["object_path"]
+        partition = read_params["partition"]
+        file_type = read_params["file_type"]
+        input_dict =  {
+            "env": env,
+            "bucket_name": f"{ng_prefix}-datalake-{env}-{layer}",
+            "object_path": object_path,
+            "partition": partition,
+            "file_type": file_type,
+        }
+        if read_params.get('schema_path') is not None:
+            input_dict['schema_path'] = {
+            "bucket_name": f"{ng_prefix}-datalake-{env}-repository",
+            "object_path": read_params['schema_path']
+        }
+        return input_dict
+
+
+
```

### Comparing `ngdataenginterface-0.0.7/PKG-INFO` & `ngdataenginterface-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngdataenginterface
-Version: 0.0.7
+Version: 0.1.0
 Summary: A library for facilitating the development of data engineering pipelines
 Author: NG.CASH
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

