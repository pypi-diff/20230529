# Comparing `tmp/deep_proto-0.9.dev0.tar.gz` & `tmp/deep_proto-1.0.0.tar.gz`

## Comparing `deep_proto-0.9.dev0.tar` & `deep_proto-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 deep_proto-0.9.dev0/src/deepproto/proto/common/v1/common_pb2.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 deep_proto-0.9.dev0/src/deepproto/proto/poll/v1/poll_pb2.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 deep_proto-0.9.dev0/src/deepproto/proto/poll/v1/poll_pb2_grpc.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 deep_proto-0.9.dev0/src/deepproto/proto/resource/v1/resource_pb2.py
--rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 deep_proto-0.9.dev0/src/deepproto/proto/tracepoint/v1/tracepoint_pb2.py
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 deep_proto-0.9.dev0/src/deepproto/proto/tracepoint/v1/tracepoint_pb2_grpc.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 deep_proto-0.9.dev0/.gitignore
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 deep_proto-0.9.dev0/pyproject.toml
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 deep_proto-0.9.dev0/../../README.md
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 deep_proto-0.9.dev0/PKG-INFO
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 deep_proto-1.0.0/deepproto/proto/common/v1/common_pb2.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 deep_proto-1.0.0/deepproto/proto/poll/v1/poll_pb2.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 deep_proto-1.0.0/deepproto/proto/poll/v1/poll_pb2_grpc.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 deep_proto-1.0.0/deepproto/proto/resource/v1/resource_pb2.py
+-rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 deep_proto-1.0.0/deepproto/proto/tracepoint/v1/tracepoint_pb2.py
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 deep_proto-1.0.0/deepproto/proto/tracepoint/v1/tracepoint_pb2_grpc.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 deep_proto-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 deep_proto-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 deep_proto-1.0.0/../../README_PYTHON.md
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 deep_proto-1.0.0/PKG-INFO
```

### Comparing `deep_proto-0.9.dev0/src/deepproto/proto/common/v1/common_pb2.py` & `deep_proto-1.0.0/deepproto/proto/common/v1/common_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&deepproto/proto/common/v1/common.proto\x12\x19\x64\x65\x65pproto.proto.common.v1\"\x84\x02\n\x08\x41nyValue\x12\x16\n\x0cstring_value\x18\x01 \x01(\tH\x00\x12\x14\n\nbool_value\x18\x02 \x01(\x08H\x00\x12\x13\n\tint_value\x18\x03 \x01(\x03H\x00\x12\x16\n\x0c\x64ouble_value\x18\x04 \x01(\x01H\x00\x12<\n\x0b\x61rray_value\x18\x05 \x01(\x0b\x32%.deepproto.proto.common.v1.ArrayValueH\x00\x12?\n\x0ckvlist_value\x18\x06 \x01(\x0b\x32\'.deepproto.proto.common.v1.KeyValueListH\x00\x12\x15\n\x0b\x62ytes_value\x18\x07 \x01(\x0cH\x00\x42\x07\n\x05value\"A\n\nArrayValue\x12\x33\n\x06values\x18\x01 \x03(\x0b\x32#.deepproto.proto.common.v1.AnyValue\"C\n\x0cKeyValueList\x12\x33\n\x06values\x18\x01 \x03(\x0b\x32#.deepproto.proto.common.v1.KeyValue\"K\n\x08KeyValue\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.deepproto.proto.common.v1.AnyValueB\\\n\"com.intergral.deep.proto.common.v1P\x01Z4github.com/intergral/deep-proto/proto/deep/common/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&deepproto/proto/common/v1/common.proto\x12\x19\x64\x65\x65pproto.proto.common.v1\"\x84\x02\n\x08\x41nyValue\x12\x16\n\x0cstring_value\x18\x01 \x01(\tH\x00\x12\x14\n\nbool_value\x18\x02 \x01(\x08H\x00\x12\x13\n\tint_value\x18\x03 \x01(\x03H\x00\x12\x16\n\x0c\x64ouble_value\x18\x04 \x01(\x01H\x00\x12<\n\x0b\x61rray_value\x18\x05 \x01(\x0b\x32%.deepproto.proto.common.v1.ArrayValueH\x00\x12?\n\x0ckvlist_value\x18\x06 \x01(\x0b\x32\'.deepproto.proto.common.v1.KeyValueListH\x00\x12\x15\n\x0b\x62ytes_value\x18\x07 \x01(\x0cH\x00\x42\x07\n\x05value\"A\n\nArrayValue\x12\x33\n\x06values\x18\x01 \x03(\x0b\x32#.deepproto.proto.common.v1.AnyValue\"C\n\x0cKeyValueList\x12\x33\n\x06values\x18\x01 \x03(\x0b\x32#.deepproto.proto.common.v1.KeyValue\"K\n\x08KeyValue\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.deepproto.proto.common.v1.AnyValueBT\n\"com.intergral.deep.proto.common.v1P\x01Z,github.com/intergral/go-deep-proto/common/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'deepproto.proto.common.v1.common_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\"com.intergral.deep.proto.common.v1P\001Z4github.com/intergral/deep-proto/proto/deep/common/v1'
+  DESCRIPTOR._serialized_options = b'\n\"com.intergral.deep.proto.common.v1P\001Z,github.com/intergral/go-deep-proto/common/v1'
   _ANYVALUE._serialized_start=70
   _ANYVALUE._serialized_end=330
   _ARRAYVALUE._serialized_start=332
   _ARRAYVALUE._serialized_end=397
   _KEYVALUELIST._serialized_start=399
   _KEYVALUELIST._serialized_end=466
   _KEYVALUE._serialized_start=468
```

### Comparing `deep_proto-0.9.dev0/src/deepproto/proto/poll/v1/poll_pb2.py` & `deep_proto-1.0.0/deepproto/proto/poll/v1/poll_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 _sym_db = _symbol_database.Default()
 
 
 from deepproto.proto.resource.v1 import resource_pb2 as deepproto_dot_proto_dot_resource_dot_v1_dot_resource__pb2
 from deepproto.proto.tracepoint.v1 import tracepoint_pb2 as deepproto_dot_proto_dot_tracepoint_dot_v1_dot_tracepoint__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"deepproto/proto/poll/v1/poll.proto\x12\x17\x64\x65\x65pproto.proto.poll.v1\x1a*deepproto/proto/resource/v1/resource.proto\x1a.deepproto/proto/tracepoint/v1/tracepoint.proto\"h\n\x0bPollRequest\x12\n\n\x02ts\x18\x01 \x01(\x03\x12\x14\n\x0c\x63urrent_hash\x18\x02 \x01(\t\x12\x37\n\x08resource\x18\x03 \x01(\x0b\x32%.deepproto.proto.resource.v1.Resource\"\xb1\x01\n\x0cPollResponse\x12\n\n\x02ts\x18\x01 \x01(\x03\x12\x14\n\x0c\x63urrent_hash\x18\x02 \x01(\t\x12\x41\n\x08response\x18\x03 \x03(\x0b\x32/.deepproto.proto.tracepoint.v1.TracePointConfig\x12<\n\rresponse_type\x18\x04 \x01(\x0e\x32%.deepproto.proto.poll.v1.ResponseType*)\n\x0cResponseType\x12\r\n\tNO_CHANGE\x10\x00\x12\n\n\x06UPDATE\x10\x01\x32\x63\n\nPollConfig\x12U\n\x04poll\x12$.deepproto.proto.poll.v1.PollRequest\x1a%.deepproto.proto.poll.v1.PollResponse\"\x00\x42X\n com.intergral.deep.proto.poll.v1P\x01Z2github.com/intergral/deep-proto/proto/deep/poll/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"deepproto/proto/poll/v1/poll.proto\x12\x17\x64\x65\x65pproto.proto.poll.v1\x1a*deepproto/proto/resource/v1/resource.proto\x1a.deepproto/proto/tracepoint/v1/tracepoint.proto\"n\n\x0bPollRequest\x12\x10\n\x08ts_nanos\x18\x01 \x01(\x06\x12\x14\n\x0c\x63urrent_hash\x18\x02 \x01(\t\x12\x37\n\x08resource\x18\x03 \x01(\x0b\x32%.deepproto.proto.resource.v1.Resource\"\xb7\x01\n\x0cPollResponse\x12\x10\n\x08ts_nanos\x18\x01 \x01(\x06\x12\x14\n\x0c\x63urrent_hash\x18\x02 \x01(\t\x12\x41\n\x08response\x18\x03 \x03(\x0b\x32/.deepproto.proto.tracepoint.v1.TracePointConfig\x12<\n\rresponse_type\x18\x04 \x01(\x0e\x32%.deepproto.proto.poll.v1.ResponseType*)\n\x0cResponseType\x12\r\n\tNO_CHANGE\x10\x00\x12\n\n\x06UPDATE\x10\x01\x32\x63\n\nPollConfig\x12U\n\x04poll\x12$.deepproto.proto.poll.v1.PollRequest\x1a%.deepproto.proto.poll.v1.PollResponse\"\x00\x42P\n com.intergral.deep.proto.poll.v1P\x01Z*github.com/intergral/go-deep-proto/poll/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'deepproto.proto.poll.v1.poll_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n com.intergral.deep.proto.poll.v1P\001Z2github.com/intergral/deep-proto/proto/deep/poll/v1'
-  _RESPONSETYPE._serialized_start=441
-  _RESPONSETYPE._serialized_end=482
+  DESCRIPTOR._serialized_options = b'\n com.intergral.deep.proto.poll.v1P\001Z*github.com/intergral/go-deep-proto/poll/v1'
+  _RESPONSETYPE._serialized_start=453
+  _RESPONSETYPE._serialized_end=494
   _POLLREQUEST._serialized_start=155
-  _POLLREQUEST._serialized_end=259
-  _POLLRESPONSE._serialized_start=262
-  _POLLRESPONSE._serialized_end=439
-  _POLLCONFIG._serialized_start=484
-  _POLLCONFIG._serialized_end=583
+  _POLLREQUEST._serialized_end=265
+  _POLLRESPONSE._serialized_start=268
+  _POLLRESPONSE._serialized_end=451
+  _POLLCONFIG._serialized_start=496
+  _POLLCONFIG._serialized_end=595
 # @@protoc_insertion_point(module_scope)
```

### Comparing `deep_proto-0.9.dev0/src/deepproto/proto/poll/v1/poll_pb2_grpc.py` & `deep_proto-1.0.0/deepproto/proto/poll/v1/poll_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `deep_proto-0.9.dev0/src/deepproto/proto/resource/v1/resource_pb2.py` & `deep_proto-1.0.0/deepproto/proto/resource/v1/resource_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from deepproto.proto.common.v1 import common_pb2 as deepproto_dot_proto_dot_common_dot_v1_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*deepproto/proto/resource/v1/resource.proto\x12\x1b\x64\x65\x65pproto.proto.resource.v1\x1a&deepproto/proto/common/v1/common.proto\"e\n\x08Resource\x12\x37\n\nattributes\x18\x01 \x03(\x0b\x32#.deepproto.proto.common.v1.KeyValue\x12 \n\x18\x64ropped_attributes_count\x18\x02 \x01(\rB\x83\x01\n\"io.opentelemetry.proto.resource.v1B\rResourceProtoP\x01Z*go.opentelemetry.io/proto/otlp/resource/v1\xaa\x02\x1fOpenTelemetry.Proto.Resource.V1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*deepproto/proto/resource/v1/resource.proto\x12\x1b\x64\x65\x65pproto.proto.resource.v1\x1a&deepproto/proto/common/v1/common.proto\"e\n\x08Resource\x12\x37\n\nattributes\x18\x01 \x03(\x0b\x32#.deepproto.proto.common.v1.KeyValue\x12 \n\x18\x64ropped_attributes_count\x18\x02 \x01(\rBX\n$com.intergral.deep.proto.resource.v1P\x01Z.github.com/intergral/go-deep-proto/resource/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'deepproto.proto.resource.v1.resource_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\"io.opentelemetry.proto.resource.v1B\rResourceProtoP\001Z*go.opentelemetry.io/proto/otlp/resource/v1\252\002\037OpenTelemetry.Proto.Resource.V1'
+  DESCRIPTOR._serialized_options = b'\n$com.intergral.deep.proto.resource.v1P\001Z.github.com/intergral/go-deep-proto/resource/v1'
   _RESOURCE._serialized_start=115
   _RESOURCE._serialized_end=216
 # @@protoc_insertion_point(module_scope)
```

### Comparing `deep_proto-0.9.dev0/src/deepproto/proto/tracepoint/v1/tracepoint_pb2.py` & `deep_proto-1.0.0/deepproto/proto/tracepoint/v1/tracepoint_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,40 +10,40 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from deepproto.proto.common.v1 import common_pb2 as deepproto_dot_proto_dot_common_dot_v1_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.deepproto/proto/tracepoint/v1/tracepoint.proto\x12\x1d\x64\x65\x65pproto.proto.tracepoint.v1\x1a&deepproto/proto/common/v1/common.proto\"\xc4\x01\n\x10TracePointConfig\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x0f\n\x07line_no\x18\x03 \x01(\x05\x12G\n\x04\x61rgs\x18\x04 \x03(\x0b\x32\x39.deepproto.proto.tracepoint.v1.TracePointConfig.ArgsEntry\x12\x0f\n\x07watches\x18\x05 \x03(\t\x1a+\n\tArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"9\n\nVariableId\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\tmodifiers\x18\x03 \x03(\t\"\x98\x01\n\x08Variable\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\x0c\n\x04hash\x18\x03 \x01(\t\x12;\n\x08\x63hildren\x18\x04 \x03(\x0b\x32).deepproto.proto.tracepoint.v1.VariableId\x12\x16\n\ttruncated\x18\x05 \x01(\x08H\x00\x88\x01\x01\x42\x0c\n\n_truncated\"\xe7\x03\n\nStackFrame\x12\x11\n\tfile_name\x18\x01 \x01(\t\x12\x13\n\x0bmethod_name\x18\x02 \x01(\t\x12\x13\n\x0bline_number\x18\x03 \x01(\x05\x12\x17\n\nclass_name\x18\x04 \x01(\tH\x00\x88\x01\x01\x12\x15\n\x08is_async\x18\x05 \x01(\x08H\x01\x88\x01\x01\x12\x1a\n\rcolumn_number\x18\x06 \x01(\x05H\x02\x88\x01\x01\x12!\n\x14transpiled_file_name\x18\x07 \x01(\tH\x03\x88\x01\x01\x12#\n\x16transpiled_line_number\x18\x08 \x01(\x05H\x04\x88\x01\x01\x12%\n\x18transpiled_column_number\x18\t \x01(\x05H\x05\x88\x01\x01\x12<\n\tvariables\x18\n \x03(\x0b\x32).deepproto.proto.tracepoint.v1.VariableId\x12\x16\n\tapp_frame\x18\x0b \x01(\x08H\x06\x88\x01\x01\x42\r\n\x0b_class_nameB\x0b\n\t_is_asyncB\x10\n\x0e_column_numberB\x17\n\x15_transpiled_file_nameB\x19\n\x17_transpiled_line_numberB\x1b\n\x19_transpiled_column_numberB\x0c\n\n_app_frame\"\x85\x01\n\x0bWatchResult\x12\x12\n\nexpression\x18\x01 \x01(\t\x12@\n\x0bgood_result\x18\x02 \x01(\x0b\x32).deepproto.proto.tracepoint.v1.VariableIdH\x00\x12\x16\n\x0c\x65rror_result\x18\x03 \x01(\tH\x00\x42\x08\n\x06result\"\x8e\x04\n\x08Snapshot\x12\n\n\x02id\x18\x01 \x01(\t\x12\x43\n\ntracepoint\x18\x02 \x01(\x0b\x32/.deepproto.proto.tracepoint.v1.TracePointConfig\x12J\n\nvar_lookup\x18\x03 \x03(\x0b\x32\x36.deepproto.proto.tracepoint.v1.Snapshot.VarLookupEntry\x12\n\n\x02ts\x18\x04 \x01(\x03\x12\x39\n\x06\x66rames\x18\x05 \x03(\x0b\x32).deepproto.proto.tracepoint.v1.StackFrame\x12;\n\x07watches\x18\x06 \x03(\x0b\x32*.deepproto.proto.tracepoint.v1.WatchResult\x12\x37\n\nattributes\x18\x07 \x03(\x0b\x32#.deepproto.proto.common.v1.KeyValue\x12\x16\n\x0enanos_duration\x18\x08 \x01(\x03\x12\x35\n\x08resource\x18\t \x03(\x0b\x32#.deepproto.proto.common.v1.KeyValue\x1aY\n\x0eVarLookupEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x36\n\x05value\x18\x02 \x01(\x0b\x32\'.deepproto.proto.tracepoint.v1.Variable:\x02\x38\x01\"\x12\n\x10SnapshotResponse2u\n\x0fSnapshotService\x12\x62\n\x04send\x12\'.deepproto.proto.tracepoint.v1.Snapshot\x1a/.deepproto.proto.tracepoint.v1.SnapshotResponse\"\x00\x42\x64\n&com.intergral.deep.proto.tracepoint.v1P\x01Z8github.com/intergral/deep-proto/proto/deep/tracepoint/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.deepproto/proto/tracepoint/v1/tracepoint.proto\x12\x1d\x64\x65\x65pproto.proto.tracepoint.v1\x1a&deepproto/proto/common/v1/common.proto\"\x80\x02\n\x10TracePointConfig\x12\n\n\x02ID\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x13\n\x0bline_number\x18\x03 \x01(\r\x12G\n\x04\x61rgs\x18\x04 \x03(\x0b\x32\x39.deepproto.proto.tracepoint.v1.TracePointConfig.ArgsEntry\x12\x0f\n\x07watches\x18\x05 \x03(\t\x12\x36\n\ttargeting\x18\x06 \x03(\x0b\x32#.deepproto.proto.common.v1.KeyValue\x1a+\n\tArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"g\n\nVariableID\x12\n\n\x02ID\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\tmodifiers\x18\x03 \x03(\t\x12\x1a\n\roriginal_name\x18\x04 \x01(\tH\x00\x88\x01\x01\x42\x10\n\x0e_original_name\"\x98\x01\n\x08Variable\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\x0c\n\x04hash\x18\x03 \x01(\t\x12;\n\x08\x63hildren\x18\x04 \x03(\x0b\x32).deepproto.proto.tracepoint.v1.VariableID\x12\x16\n\ttruncated\x18\x05 \x01(\x08H\x00\x88\x01\x01\x42\x0c\n\n_truncated\"\x93\x04\n\nStackFrame\x12\x11\n\tfile_name\x18\x01 \x01(\t\x12\x13\n\x0bmethod_name\x18\x02 \x01(\t\x12\x13\n\x0bline_number\x18\x03 \x01(\r\x12\x17\n\nclass_name\x18\x04 \x01(\tH\x00\x88\x01\x01\x12\x15\n\x08is_async\x18\x05 \x01(\x08H\x01\x88\x01\x01\x12\x1a\n\rcolumn_number\x18\x06 \x01(\rH\x02\x88\x01\x01\x12!\n\x14transpiled_file_name\x18\x07 \x01(\tH\x03\x88\x01\x01\x12#\n\x16transpiled_line_number\x18\x08 \x01(\rH\x04\x88\x01\x01\x12%\n\x18transpiled_column_number\x18\t \x01(\rH\x05\x88\x01\x01\x12<\n\tvariables\x18\n \x03(\x0b\x32).deepproto.proto.tracepoint.v1.VariableID\x12\x16\n\tapp_frame\x18\x0b \x01(\x08H\x06\x88\x01\x01\x12\x19\n\x0cnative_frame\x18\x0c \x01(\x08H\x07\x88\x01\x01\x42\r\n\x0b_class_nameB\x0b\n\t_is_asyncB\x10\n\x0e_column_numberB\x17\n\x15_transpiled_file_nameB\x19\n\x17_transpiled_line_numberB\x1b\n\x19_transpiled_column_numberB\x0c\n\n_app_frameB\x0f\n\r_native_frame\"\x85\x01\n\x0bWatchResult\x12\x12\n\nexpression\x18\x01 \x01(\t\x12@\n\x0bgood_result\x18\x02 \x01(\x0b\x32).deepproto.proto.tracepoint.v1.VariableIDH\x00\x12\x16\n\x0c\x65rror_result\x18\x03 \x01(\tH\x00\x42\x08\n\x06result\"\x94\x04\n\x08Snapshot\x12\n\n\x02ID\x18\x01 \x01(\x0c\x12\x43\n\ntracepoint\x18\x02 \x01(\x0b\x32/.deepproto.proto.tracepoint.v1.TracePointConfig\x12J\n\nvar_lookup\x18\x03 \x03(\x0b\x32\x36.deepproto.proto.tracepoint.v1.Snapshot.VarLookupEntry\x12\x10\n\x08ts_nanos\x18\x04 \x01(\x06\x12\x39\n\x06\x66rames\x18\x05 \x03(\x0b\x32).deepproto.proto.tracepoint.v1.StackFrame\x12;\n\x07watches\x18\x06 \x03(\x0b\x32*.deepproto.proto.tracepoint.v1.WatchResult\x12\x37\n\nattributes\x18\x07 \x03(\x0b\x32#.deepproto.proto.common.v1.KeyValue\x12\x16\n\x0e\x64uration_nanos\x18\x08 \x01(\x04\x12\x35\n\x08resource\x18\t \x03(\x0b\x32#.deepproto.proto.common.v1.KeyValue\x1aY\n\x0eVarLookupEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x36\n\x05value\x18\x02 \x01(\x0b\x32\'.deepproto.proto.tracepoint.v1.Variable:\x02\x38\x01\"\x12\n\x10SnapshotResponse2u\n\x0fSnapshotService\x12\x62\n\x04send\x12\'.deepproto.proto.tracepoint.v1.Snapshot\x1a/.deepproto.proto.tracepoint.v1.SnapshotResponse\"\x00\x42\\\n&com.intergral.deep.proto.tracepoint.v1P\x01Z0github.com/intergral/go-deep-proto/tracepoint/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'deepproto.proto.tracepoint.v1.tracepoint_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n&com.intergral.deep.proto.tracepoint.v1P\001Z8github.com/intergral/deep-proto/proto/deep/tracepoint/v1'
+  DESCRIPTOR._serialized_options = b'\n&com.intergral.deep.proto.tracepoint.v1P\001Z0github.com/intergral/go-deep-proto/tracepoint/v1'
   _TRACEPOINTCONFIG_ARGSENTRY._options = None
   _TRACEPOINTCONFIG_ARGSENTRY._serialized_options = b'8\001'
   _SNAPSHOT_VARLOOKUPENTRY._options = None
   _SNAPSHOT_VARLOOKUPENTRY._serialized_options = b'8\001'
   _TRACEPOINTCONFIG._serialized_start=122
-  _TRACEPOINTCONFIG._serialized_end=318
-  _TRACEPOINTCONFIG_ARGSENTRY._serialized_start=275
-  _TRACEPOINTCONFIG_ARGSENTRY._serialized_end=318
-  _VARIABLEID._serialized_start=320
-  _VARIABLEID._serialized_end=377
-  _VARIABLE._serialized_start=380
-  _VARIABLE._serialized_end=532
-  _STACKFRAME._serialized_start=535
-  _STACKFRAME._serialized_end=1022
-  _WATCHRESULT._serialized_start=1025
-  _WATCHRESULT._serialized_end=1158
-  _SNAPSHOT._serialized_start=1161
-  _SNAPSHOT._serialized_end=1687
-  _SNAPSHOT_VARLOOKUPENTRY._serialized_start=1598
-  _SNAPSHOT_VARLOOKUPENTRY._serialized_end=1687
-  _SNAPSHOTRESPONSE._serialized_start=1689
-  _SNAPSHOTRESPONSE._serialized_end=1707
-  _SNAPSHOTSERVICE._serialized_start=1709
-  _SNAPSHOTSERVICE._serialized_end=1826
+  _TRACEPOINTCONFIG._serialized_end=378
+  _TRACEPOINTCONFIG_ARGSENTRY._serialized_start=335
+  _TRACEPOINTCONFIG_ARGSENTRY._serialized_end=378
+  _VARIABLEID._serialized_start=380
+  _VARIABLEID._serialized_end=483
+  _VARIABLE._serialized_start=486
+  _VARIABLE._serialized_end=638
+  _STACKFRAME._serialized_start=641
+  _STACKFRAME._serialized_end=1172
+  _WATCHRESULT._serialized_start=1175
+  _WATCHRESULT._serialized_end=1308
+  _SNAPSHOT._serialized_start=1311
+  _SNAPSHOT._serialized_end=1843
+  _SNAPSHOT_VARLOOKUPENTRY._serialized_start=1754
+  _SNAPSHOT_VARLOOKUPENTRY._serialized_end=1843
+  _SNAPSHOTRESPONSE._serialized_start=1845
+  _SNAPSHOTRESPONSE._serialized_end=1863
+  _SNAPSHOTSERVICE._serialized_start=1865
+  _SNAPSHOTSERVICE._serialized_end=1982
 # @@protoc_insertion_point(module_scope)
```

### Comparing `deep_proto-0.9.dev0/src/deepproto/proto/tracepoint/v1/tracepoint_pb2_grpc.py` & `deep_proto-1.0.0/deepproto/proto/tracepoint/v1/tracepoint_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `deep_proto-0.9.dev0/pyproject.toml` & `deep_proto-1.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "deep-proto"
 description = "DEEP Python Protobuf"
-readme = "../../README.md"
-license = "Apache-2.0"
+readme = "../../README_PYTHON.md"
+license = "AGPL-3.0-only"
 requires-python = ">3.7"
 authors = [
+    { name = "Intergral GmbH", email = "support@intergral.com" },
     { name = "Ben Donnelly", email = "b.w.donnelly1@gmail.com" }
 ]
 classifiers = [
-    "Development Status :: 1 - Planning",
+    "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
-    "License :: OSI Approved :: Apache Software License",
+    "License :: OSI Approved :: GNU Affero General Public License v3",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Typing :: Typed",
 ]
 dependencies = []
-version = "0.9-dev"
+version = "1.0.0"
 
 [tool.hatch.build.targets.sdist]
 include = [
-    "src/deepproto",
+    "deepproto",
 ]
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/deepproto"]
+packages = ["deepproto"]
```

