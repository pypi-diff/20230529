# Comparing `tmp/pygitguardian-1.6.0.tar.gz` & `tmp/pygitguardian-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygitguardian-1.6.0.tar", last modified: Thu Apr 20 08:43:43 2023, max compression
+gzip compressed data, was "pygitguardian-1.7.0.tar", last modified: Mon May 29 13:50:42 2023, max compression
```

## Comparing `pygitguardian-1.6.0.tar` & `pygitguardian-1.7.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:43:43.045639 pygitguardian-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-04-20 08:43:43.045639 pygitguardian-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:43:43.041639 pygitguardian-1.6.0/pygitguardian/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/pygitguardian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/pygitguardian/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/pygitguardian/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/pygitguardian/iac_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/pygitguardian/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:43:43.045639 pygitguardian-1.6.0/pygitguardian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-04-20 08:43:43.000000 pygitguardian-1.6.0/pygitguardian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-20 08:43:43.000000 pygitguardian-1.6.0/pygitguardian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 08:43:43.000000 pygitguardian-1.6.0/pygitguardian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-20 08:43:43.000000 pygitguardian-1.6.0/pygitguardian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 08:43:43.000000 pygitguardian-1.6.0/pygitguardian.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 08:43:43.000000 pygitguardian-1.6.0/pygitguardian.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-20 08:43:43.045639 pygitguardian-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:43:43.045639 pygitguardian-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18537 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/tests/test_iac_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-20 08:43:32.000000 pygitguardian-1.6.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:50:42.157011 pygitguardian-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-05-29 13:50:42.157011 pygitguardian-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:50:42.153011 pygitguardian-1.7.0/pygitguardian/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/pygitguardian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15585 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/pygitguardian/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/pygitguardian/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/pygitguardian/iac_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18791 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/pygitguardian/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:50:42.153011 pygitguardian-1.7.0/pygitguardian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-05-29 13:50:42.000000 pygitguardian-1.7.0/pygitguardian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-29 13:50:42.000000 pygitguardian-1.7.0/pygitguardian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 13:50:42.000000 pygitguardian-1.7.0/pygitguardian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-29 13:50:42.000000 pygitguardian-1.7.0/pygitguardian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-29 13:50:42.000000 pygitguardian-1.7.0/pygitguardian.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 13:50:42.000000 pygitguardian-1.7.0/pygitguardian.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-29 13:50:42.157011 pygitguardian-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:50:42.157011 pygitguardian-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/tests/test_iac_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-29 13:50:36.000000 pygitguardian-1.7.0/tests/test_utils.py
```

### Comparing `pygitguardian-1.6.0/LICENSE` & `pygitguardian-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygitguardian-1.6.0/PKG-INFO` & `pygitguardian-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygitguardian
-Version: 1.6.0
+Version: 1.7.0
 Summary: Python Wrapper for GitGuardian's API -- Scan security policy breaks everywhere
 Home-page: https://github.com/GitGuardian/py-gitguardian
 Author: GitGuardian
 Author-email: support@gitguardian.com
 Maintainer: GitGuardian
 License: MIT
 Keywords: api-client devsecops secrets-detection security-tools library gitguardian
```

### Comparing `pygitguardian-1.6.0/README.md` & `pygitguardian-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pygitguardian-1.6.0/pygitguardian/client.py` & `pygitguardian-1.7.0/pygitguardian/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,33 +5,31 @@
 from io import BytesIO
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union, cast
 
 import requests
 from requests import Response, Session, codes
 
-from .config import (
-    DEFAULT_API_VERSION,
-    DEFAULT_BASE_URI,
-    DEFAULT_TIMEOUT,
-    MULTI_DOCUMENT_LIMIT,
-)
+from .config import DEFAULT_API_VERSION, DEFAULT_BASE_URI, DEFAULT_TIMEOUT
 from .iac_models import (
     IaCScanParameters,
     IaCScanParametersSchema,
     IaCScanResult,
     IaCScanResultSchema,
 )
 from .models import (
     Detail,
     Document,
     HealthCheckResponse,
+    HoneytokenResponse,
     MultiScanResult,
     QuotaResponse,
     ScanResult,
+    SecretScanPreferences,
+    ServerMetadata,
 )
 
 
 # max files size to create a tar from
 MAX_TAR_CONTENT_SIZE = 30 * 1024 * 1024
 
 
@@ -76,14 +74,25 @@
     """
     return (
         resp.headers["content-type"] == "application/json"
         and resp.status_code == codes.ok
     )
 
 
+def is_create_ok(resp: Response) -> bool:
+    """
+    is_create_ok returns True if the API returns code 201
+    and the content type is JSON.
+    """
+    return (
+        resp.headers["content-type"] == "application/json"
+        and resp.status_code == codes.created
+    )
+
+
 def _create_tar(root_path: Path, filenames: List[str]) -> bytes:
     """
     :param root_path: the root_path from which the tar is created
     :param files: the files which need to be added to the tar, filenames should be the paths relative to the root_path
     :return: a bytes object containing the tar.gz created from the files, with paths relative to root_path
     """
     tar_stream = BytesIO()
@@ -105,14 +114,15 @@
     _version = "undefined"
     session: Session
     api_key: str
     base_uri: str
     timeout: Optional[float]
     user_agent: str
     extra_headers: Dict
+    secret_scan_preferences: SecretScanPreferences
 
     def __init__(
         self,
         api_key: str,
         base_uri: Optional[str] = None,
         session: Optional[Session] = None,
         user_agent: Optional[str] = None,
@@ -162,14 +172,15 @@
 
         self.session.headers.update(
             {
                 "User-Agent": self.user_agent,
                 "Authorization": f"Token {api_key}",
             },
         )
+        self.secret_scan_preferences = SecretScanPreferences()
 
     def request(
         self,
         method: str,
         endpoint: str,
         version: Optional[str] = DEFAULT_API_VERSION,
         extra_headers: Optional[Dict[str, str]] = None,
@@ -237,15 +248,15 @@
             extra_headers=extra_headers,
             **kwargs,
         )
 
     def post(
         self,
         endpoint: str,
-        data: Optional[Dict[str, str]] = None,
+        data: Optional[Dict[str, Any]] = None,
         version: str = DEFAULT_API_VERSION,
         extra_headers: Optional[Dict[str, str]] = None,
         **kwargs: Any,
     ) -> Response:
         return self.request(
             "post",
             endpoint=endpoint,
@@ -292,14 +303,17 @@
         """
 
         doc_dict = {"document": document}
         if filename:
             doc_dict["filename"] = filename
 
         request_obj = Document.SCHEMA.load(doc_dict)
+        Document.SCHEMA.validate_size(
+            request_obj, self.secret_scan_preferences.maximum_document_size
+        )
 
         resp = self.post(
             endpoint="scan",
             data=request_obj,
             extra_headers=extra_headers,
         )
 
@@ -328,24 +342,30 @@
         :param documents: List of dictionaries containing the keys document
         and, optionally, filename.
             example: [{"document":"example content","filename":"intro.py"}]
         :param extra_headers: additional headers to add to the request
         :param ignore_known_secrets: indicates whether known secrets should be ignored
         :return: Detail or ScanResult response and status code
         """
-        if len(documents) > MULTI_DOCUMENT_LIMIT:
+        max_documents = self.secret_scan_preferences.maximum_documents_per_scan
+        if len(documents) > max_documents:
             raise ValueError(
-                f"too many documents submitted for scan (max={MULTI_DOCUMENT_LIMIT})"
+                f"too many documents submitted for scan (max={max_documents})"
             )
 
         if all(isinstance(doc, dict) for doc in documents):
             request_obj = Document.SCHEMA.load(documents, many=True)
         else:
             raise TypeError("each document must be a dict")
 
+        for document in request_obj:
+            Document.SCHEMA.validate_size(
+                document, self.secret_scan_preferences.maximum_document_size
+            )
+
         params = (
             {"ignore_known_secrets": ignore_known_secrets}
             if ignore_known_secrets
             else {}
         )
         resp = self.post(
             endpoint="multiscan",
@@ -386,14 +406,51 @@
         else:
             obj = load_detail(resp)
 
         obj.status_code = resp.status_code
 
         return obj
 
+    def create_honeytoken(
+        self,
+        name: Optional[str],
+        type_: str,
+        description: Optional[str],
+        extra_headers: Optional[Dict[str, str]] = None,
+    ) -> Union[Detail, HoneytokenResponse]:
+        """
+        Create a honeytoken via the /honeytokens endpoint of the API
+
+        :param name: the honeytoken name
+        :param type_: the honeytoken type
+        :param description: the honeytoken description
+        :param extra_headers: additional headers to add to the request
+        :return: Detail or Honeytoken response and status code
+        """
+        try:
+            resp = self.post(
+                endpoint="honeytokens",
+                extra_headers=extra_headers,
+                data={
+                    "name": name,
+                    "type": type_,
+                    "description": description,
+                },
+            )
+        except requests.exceptions.ReadTimeout:
+            result = Detail("The request timed out.")
+            result.status_code = 504
+        else:
+            if is_create_ok(resp):
+                result = HoneytokenResponse.SCHEMA.load(resp.json())
+            else:
+                result = load_detail(resp)
+            result.status_code = resp.status_code
+        return result
+
     # For IaC Scans
     def iac_directory_scan(
         self,
         directory: Path,
         filenames: List[str],
         scan_parameters: IaCScanParameters,
         extra_headers: Optional[Dict[str, str]] = None,
@@ -419,7 +476,27 @@
                 result = IaCScanResultSchema().load(resp.json())
             else:
                 result = load_detail(resp)
 
             result.status_code = resp.status_code
 
         return result
+
+    def read_metadata(self) -> Optional[Detail]:
+        """
+        Fetch server preferences and store them in `self.secret_scan_preferences`.
+        These preferences are then used by all future secret scans.
+
+        Note that the call fails if the API key is not valid.
+
+        :return: a Detail instance in case of error, None otherwise
+        """
+        resp = self.get("metadata")
+
+        if not is_ok(resp):
+            result = load_detail(resp)
+            result.status_code = resp.status_code
+            return result
+        metadata = ServerMetadata.SCHEMA.load(resp.json())
+
+        self.secret_scan_preferences = metadata.secret_scan_preferences
+        return None
```

### Comparing `pygitguardian-1.6.0/pygitguardian/iac_models.py` & `pygitguardian-1.7.0/pygitguardian/iac_models.py`

 * *Files identical despite different names*

### Comparing `pygitguardian-1.6.0/pygitguardian/models.py` & `pygitguardian-1.7.0/pygitguardian/models.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-from datetime import date
+from dataclasses import dataclass, field
+from datetime import date, datetime
 from typing import Any, ClassVar, Dict, List, Optional, cast
+from uuid import UUID
 
+import marshmallow_dataclass
 from marshmallow import (
     EXCLUDE,
     Schema,
     ValidationError,
     fields,
     post_load,
     pre_load,
     validate,
-    validates,
 )
 
-from .config import DOCUMENT_SIZE_THRESHOLD_BYTES
+from .config import DOCUMENT_SIZE_THRESHOLD_BYTES, MULTI_DOCUMENT_LIMIT
 
 
 class BaseSchema(Schema):
     class Meta:
         ordered = True
         unknown = EXCLUDE
 
 
 class Base:
     SCHEMA: ClassVar[BaseSchema]
 
-    def __init__(self) -> None:
-        self.status_code: Optional[int] = None
+    def __init__(self, status_code: Optional[int] = None) -> None:
+        self.status_code = status_code
 
     def to_json(self) -> str:
         """
         to_json converts model to JSON string.
         """
         return cast(str, self.SCHEMA.dumps(self))
 
@@ -47,25 +49,26 @@
         return self.status_code == 200
 
 
 class DocumentSchema(BaseSchema):
     filename = fields.String(validate=validate.Length(max=256), allow_none=True)
     document = fields.String(required=True)
 
-    @validates("document")
-    def validate_document(self, document: str) -> None:
-        """
-        validate that document is smaller than scan limit
+    @staticmethod
+    def validate_size(document: Dict[str, Any], maximum_size: int) -> None:
+        """Raises a ValidationError if the content of the document is longer than
+        `maximum_size`.
+
+        This is not implemented as a Marshmallow validator because the maximum size can
+        vary.
         """
-        encoded = document.encode("utf-8", errors="replace")
-        if len(encoded) > DOCUMENT_SIZE_THRESHOLD_BYTES:
+        encoded = document["document"].encode("utf-8", errors="replace")
+        if len(encoded) > maximum_size:
             raise ValidationError(
-                "file exceeds the maximum allowed size of {}B".format(
-                    DOCUMENT_SIZE_THRESHOLD_BYTES
-                )
+                f"file exceeds the maximum allowed size of {maximum_size}B"
             )
 
     @post_load
     def replace_0_bytes(self, in_data: Dict[str, Any], **kwargs: Any) -> Dict[str, Any]:
         doc = in_data["document"]
         # Our API does not accept 0 bytes in documents, so replace them with the replacement character
         in_data["document"] = doc.replace("\0", "\uFFFD")
@@ -111,30 +114,32 @@
         error = data.pop("error", None)
         if error is not None:
             data["detail"] = str(error)
 
         return data
 
     @post_load
-    def make_detail_response(self, data: Dict[str, str], **kwargs: Any) -> "Detail":
+    def make_detail_response(self, data: Dict[str, Any], **kwargs: Any) -> "Detail":
         return Detail(**data)
 
 
 class Detail(Base):
     """Detail is a response object mostly returned on error or when the
     api output is a simple string.
 
     Attributes:
         detail (str): response string
     """
 
     SCHEMA = DetailSchema()
 
-    def __init__(self, detail: str, **kwargs: Any) -> None:
-        super().__init__()
+    def __init__(
+        self, detail: str, status_code: Optional[int] = None, **kwargs: Any
+    ) -> None:
+        super().__init__(status_code=status_code)
         self.detail = detail
 
     def __repr__(self) -> str:
         return f"{self.status_code}:{self.detail}"
 
 
 class MatchSchema(BaseSchema):
@@ -481,14 +486,112 @@
         super().__init__()
         self.content = content
 
     def __repr__(self) -> str:
         return f"content:{repr(self.content)}"
 
 
+class HoneytokenResponseSchema(BaseSchema):
+    id = fields.UUID()
+    name = fields.String()
+    description = fields.String(allow_none=True)
+    created_at = fields.AwareDateTime()
+    gitguardian_url = fields.URL()
+    status = fields.String()
+    triggered_at = fields.AwareDateTime(allow_none=True)
+    revoked_at = fields.AwareDateTime(allow_none=True)
+    open_events_count = fields.Int(allow_none=True)
+    type_ = fields.String(data_key="type")
+    creator_id = fields.Int(allow_none=True)
+    revoker_id = fields.Int(allow_none=True)
+    creator_api_token_id = fields.String(allow_none=True)
+    revoker_api_token_id = fields.String(allow_none=True)
+    token = fields.Mapping(key=fields.String(), value=fields.String())
+    tags = fields.List(fields.String())
+
+    @post_load
+    def make_honeytoken_response(
+        self, data: Dict[str, Any], **kwargs: Any
+    ) -> "HoneytokenResponse":
+        return HoneytokenResponse(**data)
+
+
+class HoneytokenResponse(Base):
+    """
+    honeytoken creation in the GitGuardian API.
+    Allows users to create and get a honeytoken.
+    Example:
+        {
+            "id": "d45a123f-b15d-4fea-abf6-ff2a8479de5b",
+            "name": "honeytoken A",
+            "description": "honeytoken used in the repository AA",
+            "created_at": "2019-08-22T14:15:22Z",
+            "gitguardian_url":
+                "https://dashboard.gitguardian.com/workspace/1/honeytokens/d45a123f-b15d-4fea-abf6-ff2a8479de5b",
+            "status": "active",
+            "triggered_at": "2019-08-22T14:15:22Z",
+            "revoked_at": "2019-08-22T14:15:22Z",
+            "open_events_count": 122,
+            "type": "AWS",
+            "creator_id": 122,
+            "revoker_id": 122,
+            "creator_api_token_id": null,
+            "revoker_api_token_id": null,
+            "token": {
+                "access_token_id": "AAAA",
+                "secret_key": "BBB"
+            },
+        "tags": ["publicly_exposed"]
+        }
+    """
+
+    SCHEMA = HoneytokenResponseSchema()
+
+    def __init__(
+        self,
+        id: UUID,
+        name: str,
+        description: Optional[str],
+        created_at: datetime,
+        gitguardian_url: str,
+        status: str,
+        triggered_at: Optional[datetime],
+        revoked_at: Optional[datetime],
+        open_events_count: Optional[int],
+        type_: str,
+        creator_id: Optional[int],
+        revoker_id: Optional[int],
+        creator_api_token_id: Optional[str],
+        revoker_api_token_id: Optional[str],
+        token: Dict[str, str],
+        tags: List[str],
+        **kwargs: Any,
+    ) -> None:
+        super().__init__()
+        self.id = id
+        self.name = name
+        self.description = description
+        self.created_at = created_at
+        self.gitguardian_url = gitguardian_url
+        self.status = status
+        self.triggered_at = triggered_at
+        self.revoked_at = revoked_at
+        self.open_events_count = open_events_count
+        self.type_ = type_
+        self.creator_id = creator_id
+        self.revoker_id = revoker_id
+        self.creator_api_token_id = creator_api_token_id
+        self.revoker_api_token_id = revoker_api_token_id
+        self.token = token
+        self.tags = tags
+
+    def __repr__(self) -> str:
+        return f"honeytoken:{self.id} {self.name}"
+
+
 class HealthCheckResponseSchema(BaseSchema):
     detail = fields.String(allow_none=False)
     status_code = fields.Int(allow_none=False)
     app_version = fields.String(allow_none=True)
     secrets_engine_version = fields.String(allow_none=True)
 
 
@@ -517,7 +620,27 @@
             "secrets engine version:{}".format(
                 self.detail,
                 self.status_code,
                 self.app_version or "",
                 self.secrets_engine_version or "",
             )
         )
+
+
+@dataclass
+class SecretScanPreferences:
+    maximum_document_size: int = DOCUMENT_SIZE_THRESHOLD_BYTES
+    maximum_documents_per_scan: int = MULTI_DOCUMENT_LIMIT
+
+
+@dataclass
+class ServerMetadata(Base):
+    version: str
+    preferences: Dict[str, Any]
+    secret_scan_preferences: SecretScanPreferences = field(
+        default_factory=SecretScanPreferences
+    )
+
+
+ServerMetadata.SCHEMA = marshmallow_dataclass.class_schema(
+    ServerMetadata, base_schema=BaseSchema
+)()
```

### Comparing `pygitguardian-1.6.0/pygitguardian.egg-info/PKG-INFO` & `pygitguardian-1.7.0/pygitguardian.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygitguardian
-Version: 1.6.0
+Version: 1.7.0
 Summary: Python Wrapper for GitGuardian's API -- Scan security policy breaks everywhere
 Home-page: https://github.com/GitGuardian/py-gitguardian
 Author: GitGuardian
 Author-email: support@gitguardian.com
 Maintainer: GitGuardian
 License: MIT
 Keywords: api-client devsecops secrets-detection security-tools library gitguardian
```

### Comparing `pygitguardian-1.6.0/pyproject.toml` & `pygitguardian-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pygitguardian-1.6.0/setup.py` & `pygitguardian-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `pygitguardian-1.6.0/tests/test_client.py` & `pygitguardian-1.7.0/tests/test_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,21 @@
 from pygitguardian import GGClient
 from pygitguardian.client import is_ok, load_detail
 from pygitguardian.config import (
     DEFAULT_BASE_URI,
     DOCUMENT_SIZE_THRESHOLD_BYTES,
     MULTI_DOCUMENT_LIMIT,
 )
-from pygitguardian.models import Detail, MultiScanResult, QuotaResponse, ScanResult
+from pygitguardian.models import (
+    Detail,
+    HoneytokenResponse,
+    MultiScanResult,
+    QuotaResponse,
+    ScanResult,
+)
 
 from .conftest import my_vcr
 
 
 FILENAME = ".env"
 DOCUMENT = """
     import urllib.request
@@ -642,7 +648,81 @@
 
     assert client.app_version is app_version_value
     assert client.secrets_engine_version is secrets_engine_version_value
 
     other_client = GGClient(api_key="")
     assert other_client.app_version is app_version_value
     assert other_client.secrets_engine_version is secrets_engine_version_value
+
+
+@patch("requests.Session.request")
+def test_create_honeytoken(
+    request_mock: Mock,
+    client: GGClient,
+):
+    """
+    GIVEN a ggclient
+    WHEN calling create_honeytoken with parameters
+    THEN the parameters are passed in the request and the returned honeytoken use the parameters
+    """
+    mock_response = Mock(spec=Response)
+    mock_response.headers = {"content-type": "application/json"}
+    mock_response.status_code = 201
+    mock_response.json.return_value = {
+        "id": "d45a123f-b15d-4fea-abf6-ff2a8479de5b",
+        "name": "honeytoken A",
+        "description": "honeytoken used in the repository AA",
+        "created_at": "2019-08-22T14:15:22Z",
+        "gitguardian_url": "https://dashboard.gitguardian.com/workspace/1/honeytokens/d45a123f-b15d-4fea-abf6-ff2a8479de5b",  # noqa: E501
+        "status": "active",
+        "triggered_at": "2019-08-22T14:15:22Z",
+        "revoked_at": None,
+        "open_events_count": 2,
+        "type": "AWS",
+        "creator_id": 122,
+        "revoker_id": None,
+        "creator_api_token_id": None,
+        "revoker_api_token_id": None,
+        "token": {"access_token_id": "AAAA", "secret_key": "BBB"},
+        "tags": ["publicly_exposed"],
+    }
+
+    request_mock.return_value = mock_response
+
+    result = client.create_honeytoken(
+        name="honeytoken A",
+        description="honeytoken used in the repository AA",
+        type_="AWS",
+    )
+
+    assert request_mock.called
+    assert isinstance(result, HoneytokenResponse)
+
+
+@patch("requests.Session.request")
+def test_create_honeytoken_error(
+    request_mock: Mock,
+    client: GGClient,
+):
+    """
+    GIVEN a ggclient
+    WHEN calling create_honeytoken with parameters without the right access
+    THEN I get a Detail objects containing the error detail
+    """
+    mock_response = Mock(spec=Response)
+    mock_response.headers = {"content-type": "application/json"}
+    mock_response.status_code = 400
+    mock_response.json.return_value = {
+        "detail": "Not authorized",
+    }
+
+    request_mock.return_value = mock_response
+
+    result = client.create_honeytoken(
+        name="honeytoken A",
+        description="honeytoken used in the repository AA",
+        type_="AWS",
+    )
+
+    assert request_mock.called
+    assert isinstance(result, Detail)
+    result.status_code == 400
```

### Comparing `pygitguardian-1.6.0/tests/test_iac_models.py` & `pygitguardian-1.7.0/tests/test_iac_models.py`

 * *Files identical despite different names*

### Comparing `pygitguardian-1.6.0/tests/test_utils.py` & `pygitguardian-1.7.0/tests/test_utils.py`

 * *Files identical despite different names*

