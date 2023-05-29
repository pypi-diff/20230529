# Comparing `tmp/vector_pipelines-0.0.2.tar.gz` & `tmp/vector_pipelines-0.0.3.tar.gz`

## Comparing `vector_pipelines-0.0.2.tar` & `vector_pipelines-0.0.3.tar`

### file list

```diff
@@ -1,33 +1,36 @@
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/Makefile
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/.github/workflows/smokeshow.yaml
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/.github/workflows/test.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/tests/test_pipeline.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/tests/components/__init__.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/tests/components/test_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/tests/components/embeddings/__init__.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/tests/components/embeddings/test_sentence_transformers.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/cli/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/cli/app.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/cli/service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/components/__init__.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/components/config.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/components/init.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/components/service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/components/embeddings/__init__.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/components/embeddings/base.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/components/embeddings/sentence_transformers.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/components/embeddings/service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/grpc/__init__.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/grpc/embeddings_pb2.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/grpc/embeddings_pb2.pyi
--rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/grpc/embeddings_pb2_grpc.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/vector_pipelines/proto/embeddings.proto
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/LICENSE
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/README.md
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 vector_pipelines-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/Makefile
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/.github/workflows/smokeshow.yaml
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/docker/Dockerfile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/tests/test_pipeline.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/tests/components/__init__.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/tests/components/test_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/tests/components/embeddings/__init__.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/tests/components/embeddings/test_sentence_transformers.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/vector_pipelines/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/vector_pipelines/cli/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/vector_pipelines/cli/app.py
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/vector_pipelines/cli/service.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/vector_pipelines/components/__init__.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/vector_pipelines/components/factory.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/vector_pipelines/components/init.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/vector_pipelines/components/service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/vector_pipelines/components/embeddings/__init__.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/vector_pipelines/components/embeddings/base.py
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/vector_pipelines/components/embeddings/sentence_transformers.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/vector_pipelines/components/embeddings/service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/vector_pipelines/grpc/__init__.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/vector_pipelines/grpc/embeddings_pb2.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/vector_pipelines/grpc/embeddings_pb2.pyi
+-rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/vector_pipelines/grpc/embeddings_pb2_grpc.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/vector_pipelines/proto/embeddings.proto
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/vector_pipelines/utils/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/vector_pipelines/utils/imports.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/LICENSE
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/README.md
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 vector_pipelines-0.0.3/PKG-INFO
```

### Comparing `vector_pipelines-0.0.2/Makefile` & `vector_pipelines-0.0.3/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -23,9 +23,13 @@
 test:
 	coverage run -m pytest
 
 .PHONY: compile-proto
 compile-proto:
 	python -m grpc_tools.protoc -I vector_pipelines/grpc=vector_pipelines/proto --python_out=. --pyi_out=. --grpc_python_out=. vector_pipelines/proto/*.proto
 
+.PHONY: build-docker
+build-docker:
+	docker build -f docker/Dockerfile -t vector-pipelines .
+
 .PHONY: all
 all: format lint mypy test
```

### Comparing `vector_pipelines-0.0.2/.github/workflows/release.yaml` & `vector_pipelines-0.0.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `vector_pipelines-0.0.2/.github/workflows/smokeshow.yaml` & `vector_pipelines-0.0.3/.github/workflows/smokeshow.yaml`

 * *Files identical despite different names*

### Comparing `vector_pipelines-0.0.2/.github/workflows/test.yaml` & `vector_pipelines-0.0.3/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `vector_pipelines-0.0.2/tests/components/test_base.py` & `vector_pipelines-0.0.3/tests/components/test_base.py`

 * *Files identical despite different names*

### Comparing `vector_pipelines-0.0.2/tests/components/embeddings/test_sentence_transformers.py` & `vector_pipelines-0.0.3/tests/components/embeddings/test_sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `vector_pipelines-0.0.2/vector_pipelines/components/init.py` & `vector_pipelines-0.0.3/vector_pipelines/components/init.py`

 * *Files identical despite different names*

### Comparing `vector_pipelines-0.0.2/vector_pipelines/components/service.py` & `vector_pipelines-0.0.3/vector_pipelines/components/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from __future__ import annotations
 
 from concurrent import futures
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 import grpc
 
+if TYPE_CHECKING:
+    from pydantic import BaseModel
+
 
 class Serviceable:
     """Base class for components that can be served as gRPC services."""
 
+    config_cls: type[BaseModel]
+
     def add_services(self, server: grpc.Server) -> None:
         """Add servicers to the gRPC server.
 
         Args:
             server: The gRPC server to add servicers to.
         """
         raise NotImplementedError
```

### Comparing `vector_pipelines-0.0.2/vector_pipelines/components/embeddings/base.py` & `vector_pipelines-0.0.3/vector_pipelines/components/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `vector_pipelines-0.0.2/vector_pipelines/components/embeddings/sentence_transformers.py` & `vector_pipelines-0.0.3/vector_pipelines/components/embeddings/sentence_transformers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from __future__ import annotations
 
-from typing import Any, Literal, Union
+from typing import Any, Union
 
 from pydantic import BaseModel
-from sentence_transformers import SentenceTransformer
 
 from vector_pipelines.components.embeddings.base import Embeddings
+from vector_pipelines.components.factory import register_component
 from vector_pipelines.components.init import initialized
+from vector_pipelines.utils.imports import _SENTENCE_TRANSFORMERS_AVAILABLE
+
+if _SENTENCE_TRANSFORMERS_AVAILABLE:
+    from sentence_transformers import SentenceTransformer
 
 
 class SentenceTransformersEmbeddingsConfig(BaseModel):
     """The configuration for the `SentenceTransformersEmbeddings` class.
 
     Attributes:
         model_name_or_path: The name of the model to use or the path to a directory
@@ -18,37 +22,40 @@
         device: The device to use for the model. If `cpu`, the CPU will be used. If
             `cuda`, the GPU will be used. If `cuda:X`, the GPU with index `X` will be
             used. Defaults to `cpu`.
         normalize_embeddings: Whether to normalize the embeddings or not. Defaults to
             `False`.
     """
 
-    component_name: Literal["sentence_transformers_embeddings"] = (
-        "sentence_transformers_embeddings"
-    )
-    import_path = "vector_pipelines.components.embeddings.sentence_transformers.SentenceTransformersEmbeddings"
-
     model_name_or_path: str
     device: str = "cpu"
     normalize_embeddings: bool = False
 
 
+@register_component("sentence_transformers_embeddings")
 class SentenceTransformersEmbeddings(Embeddings):
     """A wrapper for the `sentence-transformers` library to generate embeddings.
 
     Attributes:
         config: the configuration for the Sentence Transformers model.
         model: The Sentence Transformers model.
     """
 
+    config_cls = SentenceTransformersEmbeddingsConfig
     config: SentenceTransformersEmbeddingsConfig
     model: Union[SentenceTransformer, None] = None
 
     def __init__(self, **kwargs: Any) -> None:
         super().__init__()
+        if not _SENTENCE_TRANSFORMERS_AVAILABLE:
+            raise ImportError(
+                "The `sentence-transformers` package is required to use"
+                " `SentenceTransformerEmbeddings` class. Install it with `pip install"
+                " vector-pipelines[sentence-transformers]`."
+            )
         self.config = SentenceTransformersEmbeddingsConfig(**kwargs)
 
     def init(self) -> None:
         self.model = SentenceTransformer(
             model_name_or_path=self.config.model_name_or_path, device=self.config.device
         )
         super().init()
@@ -61,15 +68,7 @@
         return embeddings
 
     @property
     @initialized
     def vector_size(self) -> int:
         embedding_size: int = self.model.get_sentence_embedding_dimension()  # type: ignore
         return embedding_size
-
-
-if __name__ == "__main__":
-    import sys
-
-    module = sys.modules[__name__]
-    package_name = module.__package__
-    print(f"{package_name}.ServiceSettings")
```

### Comparing `vector_pipelines-0.0.2/vector_pipelines/components/embeddings/service.py` & `vector_pipelines-0.0.3/vector_pipelines/components/embeddings/service.py`

 * *Files identical despite different names*

### Comparing `vector_pipelines-0.0.2/vector_pipelines/grpc/embeddings_pb2.py` & `vector_pipelines-0.0.3/vector_pipelines/grpc/embeddings_pb2.py`

 * *Files identical despite different names*

### Comparing `vector_pipelines-0.0.2/vector_pipelines/grpc/embeddings_pb2.pyi` & `vector_pipelines-0.0.3/vector_pipelines/grpc/embeddings_pb2.pyi`

 * *Files identical despite different names*

### Comparing `vector_pipelines-0.0.2/vector_pipelines/grpc/embeddings_pb2_grpc.py` & `vector_pipelines-0.0.3/vector_pipelines/grpc/embeddings_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vector_pipelines-0.0.2/.gitignore` & `vector_pipelines-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `vector_pipelines-0.0.2/LICENSE` & `vector_pipelines-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_pipelines-0.0.2/pyproject.toml` & `vector_pipelines-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
   "mypy ==1.2.0",
   "pre-commit >=3.2.2",
   "pytest >=7.2.0",
   "coverage[toml] >=7.0.0",
   "grpcio-tools >=1.54.0",
 ]
 grpc = [
+  "protobuf >=4.0.0",
   "grpcio >=1.54.0",
   "dill >=0.3.4",
 ]
 sentence_transformers = [
   "sentence-transformers >=2.0.0",
 ]
 
@@ -64,14 +65,17 @@
 exclude = [
   "vector_pipelines/grpc/*.py"
 ]
 
 [tool.ruff.isort]
 required-imports = ["from __future__ import annotations"]
 
+[tool.ruff.per-file-ignores]
+"vector_pipelines/cli/*.py" = ["B008"]
+
 [tool.coverage.run]
 source = ["vector_pipelines"]
 parallel = true
 branch = true
 context = '${CONTEXT}'
 
 [tool.mypy]
```

### Comparing `vector_pipelines-0.0.2/PKG-INFO` & `vector_pipelines-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-pipelines
-Version: 0.0.2
+Version: 0.0.3
 Summary: Create scalable vector search powered pipelines with ease
 Project-URL: Documentation, https://github.com/gabrielmbmb/vector-pipelines#readme
 Project-URL: Issues, https://github.com/gabrielmbmb/vector-pipelines/issues
 Project-URL: Source, https://github.com/gabrielmbmb/vector-pipelines
 Author-email: Gabriel Martín Blázquez <gmartinbdev@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -26,13 +26,14 @@
 Requires-Dist: mypy==1.2.0; extra == 'dev'
 Requires-Dist: pre-commit>=3.2.2; extra == 'dev'
 Requires-Dist: pytest>=7.2.0; extra == 'dev'
 Requires-Dist: ruff==0.0.263; extra == 'dev'
 Provides-Extra: grpc
 Requires-Dist: dill>=0.3.4; extra == 'grpc'
 Requires-Dist: grpcio>=1.54.0; extra == 'grpc'
+Requires-Dist: protobuf>=4.0.0; extra == 'grpc'
 Provides-Extra: sentence-transformers
 Requires-Dist: sentence-transformers>=2.0.0; extra == 'sentence-transformers'
 Description-Content-Type: text/markdown
 
 # vector-pipelines
 A framework for creating vector search engine powered applications
```

