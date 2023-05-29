# Comparing `tmp/pocketbasex-0.2.2.tar.gz` & `tmp/pocketbasex-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocketbasex-0.2.2.tar", max compression
+gzip compressed data, was "pocketbasex-0.8.2.tar", max compression
```

## Comparing `pocketbasex-0.2.2.tar` & `pocketbasex-0.8.2.tar`

### file list

```diff
@@ -1,36 +1,32 @@
--rw-r--r--   0        0        0     1572 2023-01-05 16:11:48.371857 pocketbasex-0.2.2/README.md
--rw-r--r--   0        0        0      325 2023-01-13 17:26:28.249801 pocketbasex-0.2.2/pocketbase/__init__.py
--rw-r--r--   0        0        0     4341 2023-01-13 17:26:28.250234 pocketbasex-0.2.2/pocketbase/client.py
--rw-r--r--   0        0        0      222 2023-01-13 17:26:28.250409 pocketbasex-0.2.2/pocketbase/models/__init__.py
--rw-r--r--   0        0        0      492 2023-01-13 17:26:28.250746 pocketbasex-0.2.2/pocketbase/models/admin.py
--rw-r--r--   0        0        0      956 2023-01-13 17:26:28.250872 pocketbasex-0.2.2/pocketbase/models/collection.py
--rw-r--r--   0        0        0      399 2023-01-13 17:26:28.250962 pocketbasex-0.2.2/pocketbase/models/external_auth.py
--rw-r--r--   0        0        0      389 2023-01-13 17:26:28.251047 pocketbasex-0.2.2/pocketbase/models/file_upload.py
--rw-r--r--   0        0        0      767 2023-01-13 17:26:28.251134 pocketbasex-0.2.2/pocketbase/models/log_request.py
--rw-r--r--   0        0        0      905 2023-01-13 17:26:28.251285 pocketbasex-0.2.2/pocketbase/models/record.py
--rw-r--r--   0        0        0      908 2023-01-13 17:26:28.251372 pocketbasex-0.2.2/pocketbase/models/user.py
--rw-r--r--   0        0        0      108 2023-01-13 17:26:28.251462 pocketbasex-0.2.2/pocketbase/models/utils/__init__.py
--rw-r--r--   0        0        0      933 2023-01-13 17:26:28.251555 pocketbasex-0.2.2/pocketbase/models/utils/base_model.py
--rw-r--r--   0        0        0      313 2023-01-13 17:26:28.251640 pocketbasex-0.2.2/pocketbase/models/utils/list_result.py
--rw-r--r--   0        0        0      293 2023-01-13 17:26:28.251727 pocketbasex-0.2.2/pocketbase/models/utils/schema_field.py
--rw-r--r--   0        0        0      288 2023-01-13 17:26:28.251839 pocketbasex-0.2.2/pocketbase/services/__init__.py
--rw-r--r--   0        0        0     3623 2023-01-13 17:26:28.252266 pocketbasex-0.2.2/pocketbase/services/admins.py
--rw-r--r--   0        0        0     1112 2023-01-13 17:26:28.252390 pocketbasex-0.2.2/pocketbase/services/collections.py
--rw-r--r--   0        0        0     2042 2023-01-13 17:26:28.252493 pocketbasex-0.2.2/pocketbase/services/logs.py
--rw-r--r--   0        0        0     4296 2023-01-13 17:26:28.252586 pocketbasex-0.2.2/pocketbase/services/realtime.py
--rw-r--r--   0        0        0      969 2023-01-13 17:26:28.252675 pocketbasex-0.2.2/pocketbase/services/records.py
--rw-r--r--   0        0        0     1510 2023-01-13 17:26:28.252791 pocketbasex-0.2.2/pocketbase/services/settings.py
--rw-r--r--   0        0        0     8958 2023-01-13 17:26:28.253196 pocketbasex-0.2.2/pocketbase/services/users.py
--rw-r--r--   0        0        0      168 2023-01-13 17:26:28.253343 pocketbasex-0.2.2/pocketbase/services/utils/__init__.py
--rw-r--r--   0        0        0     3675 2023-01-13 17:26:28.253720 pocketbasex-0.2.2/pocketbase/services/utils/base_crud_service.py
--rw-r--r--   0        0        0      178 2023-01-13 17:26:28.253881 pocketbasex-0.2.2/pocketbase/services/utils/base_service.py
--rw-r--r--   0        0        0     2015 2023-01-13 17:26:28.254135 pocketbasex-0.2.2/pocketbase/services/utils/crud_service.py
--rw-r--r--   0        0        0     4032 2023-01-13 17:26:28.254254 pocketbasex-0.2.2/pocketbase/services/utils/sse.py
--rw-r--r--   0        0        0     2126 2023-01-13 17:26:28.254430 pocketbasex-0.2.2/pocketbase/services/utils/sub_crud_service.py
--rw-r--r--   0        0        0       88 2023-01-13 17:26:28.254521 pocketbasex-0.2.2/pocketbase/stores/__init__.py
--rw-r--r--   0        0        0     1229 2023-01-13 17:26:28.254597 pocketbasex-0.2.2/pocketbase/stores/base_auth_store.py
--rw-r--r--   0        0        0     1775 2023-01-13 17:26:28.254687 pocketbasex-0.2.2/pocketbase/stores/local_auth_store.py
--rw-r--r--   0        0        0      494 2023-01-13 17:26:28.254765 pocketbasex-0.2.2/pocketbase/utils.py
--rw-r--r--   0        0        0     1794 2023-01-13 17:28:40.236301 pocketbasex-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2418 1970-01-01 00:00:00.000000 pocketbasex-0.2.2/setup.py
--rw-r--r--   0        0        0     2359 1970-01-01 00:00:00.000000 pocketbasex-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2253 2023-05-29 07:08:33.000579 pocketbasex-0.8.2/README.md
+-rw-r--r--   0        0        0      304 2023-05-29 07:08:33.000749 pocketbasex-0.8.2/pocketbase/__init__.py
+-rw-r--r--   0        0        0     4837 2023-05-29 07:29:55.747739 pocketbasex-0.8.2/pocketbase/client.py
+-rw-r--r--   0        0        0      199 2023-05-29 07:08:33.001071 pocketbasex-0.8.2/pocketbase/models/__init__.py
+-rw-r--r--   0        0        0      305 2023-05-29 07:30:44.365862 pocketbasex-0.8.2/pocketbase/models/admin.py
+-rw-r--r--   0        0        0     1296 2023-05-29 07:08:33.001322 pocketbasex-0.8.2/pocketbase/models/collection.py
+-rw-r--r--   0        0        0      486 2023-05-29 07:08:33.001479 pocketbasex-0.8.2/pocketbase/models/external_auth.py
+-rw-r--r--   0        0        0      390 2023-05-29 07:08:33.001632 pocketbasex-0.8.2/pocketbase/models/file_upload.py
+-rw-r--r--   0        0        0      767 2023-05-29 07:06:16.887327 pocketbasex-0.8.2/pocketbase/models/log_request.py
+-rw-r--r--   0        0        0      711 2023-05-29 07:30:52.288196 pocketbasex-0.8.2/pocketbase/models/record.py
+-rw-r--r--   0        0        0      108 2023-05-29 07:06:16.887517 pocketbasex-0.8.2/pocketbase/models/utils/__init__.py
+-rw-r--r--   0        0        0      880 2023-05-29 07:08:33.001972 pocketbasex-0.8.2/pocketbase/models/utils/base_model.py
+-rw-r--r--   0        0        0      313 2023-05-29 07:06:16.887636 pocketbasex-0.8.2/pocketbase/models/utils/list_result.py
+-rw-r--r--   0        0        0      293 2023-05-29 07:06:16.887695 pocketbasex-0.8.2/pocketbase/models/utils/schema_field.py
+-rw-r--r--   0        0        0      292 2023-05-29 07:08:33.002164 pocketbasex-0.8.2/pocketbase/services/__init__.py
+-rw-r--r--   0        0        0     4906 2023-05-29 07:08:33.002300 pocketbasex-0.8.2/pocketbase/services/admin_service.py
+-rw-r--r--   0        0        0     1118 2023-05-29 07:08:33.002402 pocketbasex-0.8.2/pocketbase/services/collection_service.py
+-rw-r--r--   0        0        0     2048 2023-05-29 07:08:33.002513 pocketbasex-0.8.2/pocketbase/services/log_service.py
+-rw-r--r--   0        0        0     5186 2023-05-29 07:08:33.002627 pocketbasex-0.8.2/pocketbase/services/realtime_service.py
+-rw-r--r--   0        0        0     9534 2023-05-29 07:08:33.002746 pocketbasex-0.8.2/pocketbase/services/record_service.py
+-rw-r--r--   0        0        0     1517 2023-05-29 07:08:33.002835 pocketbasex-0.8.2/pocketbase/services/settings_service.py
+-rw-r--r--   0        0        0      123 2023-05-29 07:08:33.002985 pocketbasex-0.8.2/pocketbase/services/utils/__init__.py
+-rw-r--r--   0        0        0     4256 2023-05-29 07:30:44.366387 pocketbasex-0.8.2/pocketbase/services/utils/base_crud_service.py
+-rw-r--r--   0        0        0      178 2023-05-29 07:06:16.888485 pocketbasex-0.8.2/pocketbase/services/utils/base_service.py
+-rw-r--r--   0        0        0     2703 2023-05-29 07:30:44.366682 pocketbasex-0.8.2/pocketbase/services/utils/crud_service.py
+-rw-r--r--   0        0        0     4032 2023-05-29 07:06:16.888611 pocketbasex-0.8.2/pocketbase/services/utils/sse.py
+-rw-r--r--   0        0        0       88 2023-05-29 07:06:16.888771 pocketbasex-0.8.2/pocketbase/stores/__init__.py
+-rw-r--r--   0        0        0     1278 2023-05-29 07:08:33.003434 pocketbasex-0.8.2/pocketbase/stores/base_auth_store.py
+-rw-r--r--   0        0        0     1785 2023-05-29 07:08:33.003591 pocketbasex-0.8.2/pocketbase/stores/local_auth_store.py
+-rw-r--r--   0        0        0     1011 2023-05-29 07:08:33.003786 pocketbasex-0.8.2/pocketbase/utils.py
+-rw-r--r--   0        0        0     1851 2023-05-29 07:30:44.367021 pocketbasex-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     3040 1970-01-01 00:00:00.000000 pocketbasex-0.8.2/PKG-INFO
```

### Comparing `pocketbasex-0.2.2/pocketbase/client.py` & `pocketbasex-0.8.2/pocketbase/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,84 +1,74 @@
 from __future__ import annotations
-from pocketbase.services.admins import Admins
-from pocketbase.stores.base_auth_store import BaseAuthStore
-from pocketbase.services.settings import Settings
-from pocketbase.services.users import Users
-from pocketbase.services.records import Records
-from pocketbase.services.realtime import Realtime
-from pocketbase.services.logs import Logs
-from pocketbase.services.collections import Collections
-from pocketbase.models import FileUpload
 
-from typing import Any
+from typing import Any, Dict
+from urllib.parse import quote, urlencode
 
 import httpx
 
-
-class ClientResponseError(Exception):
-    url: str = ""
-    status: int = 0
-    data: dict = {}
-    is_abort: bool = False
-    original_error: Any | None = None
-
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(*args)
-        self.url = kwargs.get("url", "")
-        self.status = kwargs.get("status", 0)
-        self.data = kwargs.get("data", {})
-        self.is_abort = kwargs.get("is_abort", False)
-        self.original_error = kwargs.get("original_error", None)
+from pocketbase.models import FileUpload
+from pocketbase.models.record import Record
+from pocketbase.services.admin_service import AdminService
+from pocketbase.services.collection_service import CollectionService
+from pocketbase.services.log_service import LogService
+from pocketbase.services.realtime_service import RealtimeService
+from pocketbase.services.record_service import RecordService
+from pocketbase.services.settings_service import SettingsService
+from pocketbase.stores.base_auth_store import BaseAuthStore
+from pocketbase.utils import ClientResponseError
 
 
 class Client:
     base_url: str
     lang: str
     auth_store: BaseAuthStore
-    settings: Settings
-    admins: Admins
-    users: Users
-    collections: Collections
-    records: Records
-    logs: Logs
-    realtime: Realtime
+    settings: SettingsService
+    admins: AdminService
+    records: Record
+    collections: CollectionService
+    records: RecordService
+    logs: LogService
+    realtime: RealtimeService
+    record_service: Dict[str, RecordService]
 
     def __init__(
         self,
         base_url: str = "/",
         lang: str = "en-US",
         auth_store: BaseAuthStore | None = None,
+        timeout: float = 120,
     ) -> None:
         self.base_url = base_url
         self.lang = lang
         self.auth_store = auth_store or BaseAuthStore()  # LocalAuthStore()
+        self.timeout = timeout
         # services
-        self.admins = Admins(self)
-        self.users = Users(self)
-        self.records = Records(self)
-        self.collections = Collections(self)
-        self.logs = Logs(self)
-        self.settings = Settings(self)
-        self.realtime = Realtime(self)
+        self.admins = AdminService(self)
+        self.collections = CollectionService(self)
+        self.logs = LogService(self)
+        self.settings = SettingsService(self)
+        self.realtime = RealtimeService(self)
+        self.record_service = {}
+
+    def collection(self, id_or_name: str) -> RecordService:
+        """Returns the RecordService associated to the specified collection."""
+        if id_or_name not in self.record_service:
+            self.record_service[id_or_name] = RecordService(self, id_or_name)
+        return self.record_service[id_or_name]
 
     def send(self, path: str, req_config: dict[str:Any]) -> Any:
         """Sends an api http request."""
         config = {"method": "GET"}
         config.update(req_config)
         # check if Authorization header can be added
         if self.auth_store.token and (
             "headers" not in config or "Authorization" not in config["headers"]
         ):
-            auth_type = "Admin"
-            if hasattr(self.auth_store.model, "verified"):
-                auth_type = "User"
             config["headers"] = config.get("headers", {})
-            config["headers"].update(
-                {"Authorization": f"Bearer {self.auth_store.token}"}
-            )
+            config["headers"].update({"Authorization": self.auth_store.token})
         # build url + path
         url = self.build_url(path)
         # send the request
         method = config.get("method", "GET")
         params = config.get("params", None)
         headers = config.get("headers", None)
         body = config.get("body", None)
@@ -102,15 +92,15 @@
                 method=method,
                 url=url,
                 params=params,
                 headers=headers,
                 json=body,
                 data=data,
                 files=files,
-                timeout=120,
+                timeout=self.timeout,
             )
         except Exception as e:
             raise ClientResponseError(
                 f"General request error. Original error: {e}",
                 original_error=e,
             )
         try:
@@ -122,14 +112,29 @@
                 f"{response.reason_phrase}: {response.json()['message']}",
                 url=response.url,
                 status=response.status_code,
                 data=data,
             )
         return data
 
+    def get_file_url(self, record: Record, filename: str, query_params: dict):
+        parts = [
+            "api",
+            "files",
+            quote(record.collection_id or record.collection_name),
+            quote(record.id),
+            quote(filename),
+        ]
+        result = self.build_url("/".join(parts))
+        if len(query_params) != 0:
+            params: str = urlencode(query_params)
+            result += "&" if "?" in result else "?"
+            result += params
+        return result
+
     def build_url(self, path: str) -> str:
         url = self.base_url
         if not self.base_url.endswith("/"):
             url += "/"
         if path.startswith("/"):
             path = path[1:]
         return url + path
```

### Comparing `pocketbasex-0.2.2/pocketbase/models/collection.py` & `pocketbasex-0.8.2/pocketbase/models/collection.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,28 +2,45 @@
 
 from pocketbase.models.utils.base_model import BaseModel
 from pocketbase.models.utils.schema_field import SchemaField
 
 
 class Collection(BaseModel):
     name: str
+    type: str
     schema: list[SchemaField]
     system: bool
     list_rule: str | None
     view_rule: str | None
     create_rule: str | None
     update_rule: str | None
     delete_rule: str | None
+    options: dict
 
     def load(self, data: dict) -> None:
         super().load(data)
         self.name = data.get("name", "")
         self.system = data.get("system", False)
+        self.type = data.get("type", "base")
+        self.options = data.get("options", {})
+
+        # rules
         self.list_rule = data.get("listRule", None)
         self.view_rule = data.get("viewRule", None)
         self.create_rule = data.get("createRule", None)
         self.update_rule = data.get("updateRule", None)
         self.delete_rule = data.get("deleteRule", "")
+
+        # schema
         schema = data.get("schema", [])
         self.schema = []
         for field in schema:
             self.schema.append(SchemaField(**field))
+
+    def is_base(self):
+        return self.type == "base"
+
+    def is_auth(self):
+        return self.type == "auth"
+
+    def is_single(self):
+        return self.type == "single"
```

### Comparing `pocketbasex-0.2.2/pocketbase/models/log_request.py` & `pocketbasex-0.8.2/pocketbase/models/log_request.py`

 * *Files identical despite different names*

### Comparing `pocketbasex-0.2.2/pocketbase/models/record.py` & `pocketbasex-0.8.2/pocketbase/models/record.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,23 +7,19 @@
 class Record(BaseModel):
     collection_id: str
     collection_name: str
     expand: dict
 
     def load(self, data: dict) -> None:
         super().load(data)
+        self.expand = {}
         for key, value in data.items():
             key = camel_to_snake(key).replace("@", "")
             setattr(self, key, value)
-        self.collection_id = data.get("@collectionId", "")
-        self.collection_name = data.get("@collectionName", "")
-        expand = data.get("@expand", {})
-        if expand:
-            self.expand = expand
-            self.load_expanded()
+        self.load_expanded()
 
     @classmethod
     def parse_expanded(cls, data: dict):
         return cls(data)
 
     def load_expanded(self) -> None:
         for key, value in self.expand.items():
```

### Comparing `pocketbasex-0.2.2/pocketbase/models/utils/base_model.py` & `pocketbasex-0.8.2/pocketbase/models/utils/base_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,8 +26,8 @@
         self.id = data.pop("id", "")
         self.created = to_datetime(data.pop("created", ""))
         self.updated = to_datetime(data.pop("updated", ""))
 
     @property
     def is_new(self) -> bool:
         """Returns whether the current loaded data represent a stored db record."""
-        return not self.id or self.id == "00000000-0000-0000-0000-000000000000"
+        return not self.id
```

### Comparing `pocketbasex-0.2.2/pocketbase/services/admins.py` & `pocketbasex-0.8.2/pocketbase/services/utils/base_crud_service.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,111 +1,128 @@
 from __future__ import annotations
 
-from pocketbase.models.utils.base_model import BaseModel
-from pocketbase.services.utils.crud_service import CrudService
-from pocketbase.models.admin import Admin
-
+from abc import ABC
+from urllib.parse import quote
+from pocketbase.utils import ClientResponseError
 
-class AdminAuthResponse:
-    token: str
-    admin: Admin
-
-    def __init__(self, token: str, admin: Admin, **kwargs) -> None:
-        self.token = token
-        self.admin = admin
-        for key, value in kwargs.items():
-            setattr(self, key, value)
+from pocketbase.models.utils.base_model import BaseModel
+from pocketbase.models.utils.list_result import ListResult
+from pocketbase.services.utils.base_service import BaseService
 
 
-class Admins(CrudService):
+class BaseCrudService(BaseService, ABC):
     def decode(self, data: dict) -> BaseModel:
-        return Admin(data)
+        """Response data decoder"""
 
-    def base_crud_path(self) -> str:
-        return "/api/admins"
+    def _get_full_list(
+        self, 
+        base_path: str,
+        batch: int = 200, 
+        expand: str = None,
+        filter: str = None,
+        sort: str = None,
+        query: dict = None,
+        headers: dict = None,
+    ) -> list[BaseModel]:
+        result: list[BaseModel] = []
+
+        def request(result: list[BaseModel], page: int) -> list:
+            list = self._get_list(
+                base_path,
+                page=page,
+                per_page=batch,
+                expand=expand,
+                filter=filter,
+                sort=sort,
+                query=query,
+                headers=headers,
+            )
+            items = list.items
+            total_items = list.total_items
+            result += items
+            if len(items) > 0 and total_items > len(result):
+                return request(result, page + 1)
+            return result
+
+        return request(result, 1)
 
-    def auth_response(self, response_data: dict) -> AdminAuthResponse:
-        """Prepare successful authorize response."""
-        admin = self.decode(response_data.pop("admin", {}))
-        token = response_data.pop("token", "")
-        if token and admin:
-            self.client.auth_store.save(token, admin)
-        return AdminAuthResponse(token=token, admin=admin, **response_data)
-
-    def auth_with_password(
-        self, email: str, password: str, body_params: dict = {}, query_params: dict = {}
-    ) -> AdminAuthResponse:
-        """
-        Authenticate an admin account by its email and password
-        and returns a new admin token and data.
-
-        On success this method automatically updates the client's AuthStore data.
-        """
-        body_params.update({"identity": email, "password": password})
+    # https://github.com/pocketbase/dart-sdk/blob/cb04918f918de8b5815212bb1a52941fc6fe0e10/lib/src/services/base_crud_service.dart#L56
+    def _get_list(
+        self,
+        base_path: str,
+        *,
+        page: int = 1, 
+        per_page: int = 30,
+        expand: str = None,
+        filter: str = None,
+        sort: str = None,
+        query: dict = None,
+        headers: dict = None,
+    ) -> ListResult:
+        query = query or {}
+        headers = headers or {}
+        enriched_query = query.copy()
+        enriched_query.update({"page": page, "perPage": per_page, "expand": expand, "filter": filter, "sort": sort})
         response_data = self.client.send(
-            self.base_crud_path() + "/auth-with-password",
-            {
-                "method": "POST",
-                "params": query_params,
-                "body": body_params,
-                "headers": {"Authorization": ""},
-            },
-        )
-        return self.auth_response(response_data)
-
-    def refresh(
-        self, body_params: dict = {}, query_params: dict = {}
-    ) -> AdminAuthResponse:
-        """
-        Refreshes the current admin authenticated instance and
-        returns a new token and admin data.
-
-        On success this method automatically updates the client's AuthStore data.
-        """
-        return self.auth_response(
+            base_path, {"method": "GET", "params": enriched_query, "headers": headers}
+        )
+        items: list[BaseModel] = []
+        if "items" in response_data:
+            response_data["items"] = response_data["items"] or []
+            for item in response_data["items"]:
+                items.append(self.decode(item))
+        return ListResult(
+            response_data.get("page", 1),
+            response_data.get("perPage", 0),
+            response_data.get("totalItems", 0),
+            response_data.get("totalPages", 0),
+            items,
+        )
+
+    def _get_one(self, base_path: str, id: str, query_params: dict = {}) -> BaseModel:
+        return self.decode(
             self.client.send(
-                self.base_crud_path() + "/refresh",
-                {"method": "POST", "params": query_params, "body": body_params},
+                f"{base_path}/{quote(id)}", {"method": "GET", "params": query_params}
             )
         )
 
-    def requestPasswordReset(
-        self, email: str, body_params: dict = {}, query_params: dict = {}
-    ) -> bool:
-        """Sends admin password reset request."""
-        body_params.update({"email": email})
-        self.client.send(
-            self.base_crud_path() + "/request-password-reset",
+    def _get_first_list_item(self, base_path: str, filter: str, query_params={}):
+        query_params.update(
             {
-                "method": "POST",
-                "params": query_params,
-                "body": body_params,
-            },
+                "filter": filter,
+                "$cancelKey": "one_by_filter_" + base_path + "_" + filter,
+            }
         )
-        return True
+        result = self._get_list(base_path, 1, 1, query_params)
+        try:
+            if len(result.items) == 0:
+                raise
+        except:
+            raise ClientResponseError(
+                "The requested resource wasn't found.", status=404
+            )
 
-    def confirmPasswordReset(
-        self,
-        password_reset_token: str,
-        password: str,
-        password_confirm: str,
-        body_params: dict = {},
-        query_params: dict = {},
-    ) -> AdminAuthResponse:
-        """Confirms admin password reset request."""
-        body_params.update(
-            {
-                "token": password_reset_token,
-                "password": password,
-                "passwordConfirm": password_confirm,
-            }
+    def _create(
+        self, base_path: str, body_params: dict = {}, query_params: dict = {}
+    ) -> BaseModel:
+        return self.decode(
+            self.client.send(
+                base_path,
+                {"method": "POST", "params": query_params, "body": body_params},
+            )
         )
-        return self.auth_response(
+
+    def _update(
+        self, base_path: str, id: str, body_params: dict = {}, query_params: dict = {}
+    ) -> BaseModel:
+        return self.decode(
             self.client.send(
-                self.base_crud_path() + "/confirm-password-reset",
-                {
-                    "method": "POST",
-                    "params": query_params,
-                    "body": body_params,
-                },
+                f"{base_path}/{quote(id)}",
+                {"method": "PATCH", "params": query_params, "body": body_params},
             )
         )
+
+    def _delete(self, base_path: str, id: str, query_params: dict = {}) -> bool:
+        self.client.send(
+            f"{base_path}/{quote(id)}", {"method": "DELETE", "params": query_params}
+        )
+        return True
```

### Comparing `pocketbasex-0.2.2/pocketbase/services/collections.py` & `pocketbasex-0.8.2/pocketbase/services/collection_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from pocketbase.services.utils.crud_service import CrudService
 from pocketbase.models.utils.base_model import BaseModel
 from pocketbase.models.collection import Collection
 
 
-class Collections(CrudService):
+class CollectionService(CrudService):
     def decode(self, data: dict) -> BaseModel:
         return Collection(data)
 
     def base_crud_path(self) -> str:
         return "/api/collections"
 
     def import_collections(
```

### Comparing `pocketbasex-0.2.2/pocketbase/services/logs.py` & `pocketbasex-0.8.2/pocketbase/services/log_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 @dataclass
 class HourlyStats:
     total: int
     date: Union[str, datetime.datetime]
 
 
-class Logs(BaseService):
+class LogService(BaseService):
     def get_request_list(
         self, page: int = 1, per_page: int = 30, query_params: dict = {}
     ) -> ListResult:
         """Returns paginated logged requests list."""
         query_params.update({"page": page, "perPage": per_page})
         response_data = self.client.send(
             "/api/logs/requests",
```

### Comparing `pocketbasex-0.2.2/pocketbase/services/settings.py` & `pocketbasex-0.8.2/pocketbase/services/settings_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from pocketbase.services.utils.base_service import BaseService
 
 
-class Settings(BaseService):
+class SettingsService(BaseService):
     def get_all(self, query_params: dict = {}) -> dict:
         """Fetch all available app settings."""
         return self.client.send(
             "/api/settings",
             {"method": "GET", "params": query_params},
         )
```

### Comparing `pocketbasex-0.2.2/pocketbase/services/users.py` & `pocketbasex-0.8.2/pocketbase/services/record_service.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from __future__ import annotations
-
 from dataclasses import dataclass
-from typing import Any
-from urllib.parse import quote
+from typing import List
+
+from urllib.parse import quote, urlencode
+from pocketbase.services.realtime_service import Callable, MessageData
 
-from pocketbase.services.utils.crud_service import CrudService
 from pocketbase.models.utils.base_model import BaseModel
-from pocketbase.models.user import User
-from pocketbase.models.external_auth import ExternalAuth
+from pocketbase.models.record import Record
+from pocketbase.services.utils.crud_service import CrudService
+from pocketbase.utils import camel_to_snake
 
 
-class UserAuthResponse:
+class RecordAuthResponse:
     token: str
-    user: User
+    record: Record
 
-    def __init__(self, token: str, user: User, **kwargs) -> None:
+    def __init__(self, token: str, record: Record, **kwargs) -> None:
         self.token = token
-        self.user = user
+        self.record = record
         for key, value in kwargs.items():
             setattr(self, key, value)
 
 
 @dataclass
 class AuthProviderInfo:
     name: str
@@ -29,253 +30,246 @@
     code_challenge: str
     code_challenge_method: str
     auth_url: str
 
 
 @dataclass
 class AuthMethodsList:
+    username_password: bool
     email_password: bool
     auth_providers: list[AuthProviderInfo]
 
 
-class Users(CrudService):
+class RecordService(CrudService):
+    collection_id_or_name: str
+
+    def __init__(self, client, collection_id_or_name) -> None:
+        super().__init__(client)
+        self.collection_id_or_name = collection_id_or_name
+
     def decode(self, data: dict) -> BaseModel:
-        return User(data)
+        return Record(data)
 
     def base_crud_path(self) -> str:
-        return "/api/collections/users"
+        return self.base_collection_path() + "/records"
 
-    def auth_response(self, response_data: Any) -> UserAuthResponse:
-        """Prepare successful authorization response."""
-        user = self.decode(response_data.pop("user", {}))
+    def base_collection_path(self) -> str:
+        """Returns the current collection service base path."""
+        return "/api/collections/" + quote(self.collection_id_or_name)
+
+    def get_file_url(
+        self, record: Record, filename: str, query_params: dict = {}
+    ) -> str:
+        """Builds and returns an absolute record file url."""
+        base_url = self.client.base_url
+        if base_url.endswith("/"):
+            base_url = base_url[:-1]
+        result = f"{base_url}/api/files/{record.collection_id}/{record.id}/{filename}"
+        if query_params:
+            result += "?" + urlencode(query_params)
+        return result
+
+    def subscribe(self, callback: Callable[[MessageData], None]):
+        """Subscribe to realtime changes of any record from the collection."""
+        return self.client.realtime.subscribe(self.collection_id_or_name, callback)
+
+    def subscribeOne(self, record_id: str, callback: Callable[[MessageData], None]):
+        """Subscribe to the realtime changes of a single record in the collection."""
+        return self.client.realtime.subscribe(
+            self.collection_id_or_name + "/" + record_id, callback
+        )
+
+    def unsubscribe(self, *record_ids: List[str]):
+        """Subscribe to the realtime changes of a single record in the collection."""
+        if record_ids and len(record_ids) == 0:
+            subs = []
+            for id in record_ids:
+                subs.append(self.collection_id_or_name + "/" + id)
+            return self.client.realtime.unsubscribe(*subs)
+        return self.client.realtime.subscribe_by_prefix(self.collection_id_or_name)
+
+    def update(self, id: str, body_params: dict = {}, query_params: dict = {}):
+        """
+        If the current `client.auth_store.model` matches with the updated id, then
+        on success the `client.auth_store.model` will be updated with the result.
+        """
+        item = super().update(id, body_params)  # super(Record).update
+        try:
+            if (
+                self.client.auth_store.model.collection_id is not None
+                and item.id == self.client.auth_store.model.id
+            ):
+                self.client.auth_store.save(self.client.auth_store.token, item)
+        except:
+            pass
+        return item
+
+    def delete(self, id: str, body_params: dict = {}, query_params: dict = {}):
+        """
+        If the current `client.auth_store.model` matches with the deleted id,
+        then on success the `client.auth_store` will be cleared.
+        """
+        success = super().delete(id, body_params)  # super(Record).delete
+        try:
+            if (
+                success
+                and self.client.auth_store.model.collection_id is not None
+                and id == self.client.auth_store.model.id
+            ):
+                self.client.auth_store.clear()
+        except:
+            pass
+        return success
+
+    def auth_response(self, response_data: dict) -> RecordAuthResponse:
+        """Prepare successful collection authorization response."""
+        record = self.decode(response_data.pop("record", {}))
         token = response_data.pop("token", "")
-        if token and user:
-            self.client.auth_store.save(token, user)
-        return UserAuthResponse(token=token, user=user, **response_data)
+        if token and record:
+            self.client.auth_store.save(token, record)
+        return RecordAuthResponse(token=token, record=record, **response_data)
 
-    def list_auth_methods(self, query_params: dict = {}) -> AuthMethodsList:
-        """Returns all available application auth methods."""
+    def list_auth_methods(self, query_params: str = {}):
+        """Returns all available collection auth methods."""
         response_data = self.client.send(
-            self.base_crud_path() + "/auth-methods",
+            self.base_collection_path() + "/auth-methods",
             {"method": "GET", "params": query_params},
         )
-        email_password = response_data.get("emailPassword", False)
+        username_password = response_data.pop("usernamePassword", False)
+        email_password = response_data.pop("emailPassword", False)
+
+        def apply_pythonic_keys(ap):
+            pythonic_keys_ap = {
+                camel_to_snake(key).replace("@", ""): value for key, value in ap.items()
+            }
+            return pythonic_keys_ap
+
         auth_providers = [
-            AuthProviderInfo(auth_provider)
-            for auth_provider in response_data.get("authProviders", [])
+            AuthProviderInfo(**auth_provider)
+            for auth_provider in map(
+                apply_pythonic_keys, response_data.get("authProviders", [])
+            )
         ]
-        return AuthMethodsList(email_password, auth_providers)
+        return AuthMethodsList(username_password, email_password, auth_providers)
 
     def auth_with_password(
-        self, email: str, password: str, body_params: dict = {}, query_params: dict = {}
-    ) -> UserAuthResponse:
+        self,
+        username_or_email: str,
+        password: str,
+        body_params: dict = {},
+        query_params: dict = {},
+    ) -> RecordAuthResponse:
         """
-        Authenticate an admin account by its email and password
-        and returns a new admin token and data.
+        Authenticate a single auth collection record via its username/email and password.
 
-        On success this method automatically updates the client's AuthStore data.
+        On success, this method also automatically updates
+        the client's AuthStore data and returns:
+        - the authentication token
+        - the authenticated record model
         """
-        body_params.update({"identity": email, "password": password})
+        body_params.update({"identity": username_or_email, "password": password})
         response_data = self.client.send(
-            self.base_crud_path() + "/auth-with-password",
+            self.base_collection_path() + "/auth-with-password",
             {
                 "method": "POST",
                 "params": query_params,
                 "body": body_params,
                 "headers": {"Authorization": ""},
             },
         )
         return self.auth_response(response_data)
 
-    def auth_via_oauth2(
+    def auth_with_oauth2(
         self,
         provider: str,
         code: str,
         code_verifier: str,
-        redirect_url: str,
-        body_params: dict = {},
-        query_params: dict = {},
-    ) -> UserAuthResponse:
+        redirct_url: str,
+        create_data={},
+        body_params={},
+        query_params={},
+    ):
         """
-        Authenticate a user via OAuth2 client provider.
+        Authenticate a single auth collection record with OAuth2.
 
         On success, this method also automatically updates
         the client's AuthStore data and returns:
-        - new user authentication token
-        - the authenticated user model record
-        - the OAuth2 user profile data (eg. name, email, avatar, etc.)
+        - the authentication token
+        - the authenticated record model
+        - the OAuth2 account data (eg. name, email, avatar, etc.)
         """
         body_params.update(
             {
                 "provider": provider,
                 "code": code,
                 "codeVerifier": code_verifier,
-                "redirectUrl": redirect_url,
+                "redirectUrl": redirct_url,
+                "createData": create_data,
             }
         )
         response_data = self.client.send(
-            self.base_crud_path() + "/auth-via-oauth2",
+            self.base_collection_path() + "/auth-with-oauth2",
             {
                 "method": "POST",
                 "params": query_params,
                 "body": body_params,
-                "headers": {"Authorization": ""},
             },
         )
         return self.auth_response(response_data)
 
-    def refresh(
+    def authRefresh(
         self, body_params: dict = {}, query_params: dict = {}
-    ) -> UserAuthResponse:
+    ) -> RecordAuthResponse:
         """
-        Refreshes the current user authenticated instance and
-        returns a new token and user data.
+        Refreshes the current authenticated record instance and
+        returns a new token and record data.
 
-        On success this method also automatically updates the client's AuthStore data.
+        On success this method also automatically updates the client's AuthStore.
         """
         return self.auth_response(
             self.client.send(
-                self.base_crud_path() + "/refresh",
+                self.base_collection_path() + "/auth-refresh",
                 {"method": "POST", "params": query_params, "body": body_params},
             )
         )
 
-    def request_password_reset(
+    def requestPasswordReset(
         self, email: str, body_params: dict = {}, query_params: dict = {}
     ) -> bool:
-        """Sends user password reset request."""
+        """Sends auth record password reset request."""
         body_params.update({"email": email})
         self.client.send(
-            self.base_crud_path() + "/request-password-reset",
+            self.base_collection_path() + "/request-password-reset",
             {
                 "method": "POST",
                 "params": query_params,
                 "body": body_params,
             },
         )
         return True
 
-    def confirm_password_reset(
+    def confirmPasswordReset(
         self,
         password_reset_token: str,
         password: str,
         password_confirm: str,
         body_params: dict = {},
         query_params: dict = {},
-    ) -> UserAuthResponse:
-        """Confirms user password reset request."""
+    ) -> RecordAuthResponse:
+        """Confirms auth record password reset reque"""
         body_params.update(
             {
                 "token": password_reset_token,
                 "password": password,
                 "passwordConfirm": password_confirm,
             }
         )
         return self.auth_response(
             self.client.send(
-                self.base_crud_path() + "/confirm-password-reset",
+                self.base_collection_path() + "/confirm-password-reset",
                 {
                     "method": "POST",
                     "params": query_params,
                     "body": body_params,
                 },
             )
         )
-
-    def request_verification(
-        self, email: str, body_params: dict = {}, query_params: dict = {}
-    ) -> bool:
-        """Sends user verification email request."""
-        body_params.update({"email": email})
-        self.client.send(
-            self.base_crud_path() + "/request-verification",
-            {
-                "method": "POST",
-                "params": query_params,
-                "body": body_params,
-            },
-        )
-        return True
-
-    def confirm_verification(
-        self, verification_token: str, body_params: dict = {}, query_params: dict = {}
-    ) -> UserAuthResponse:
-        """Confirms user email verification request."""
-        body_params.update(
-            {
-                "token": verification_token,
-            }
-        )
-        return self.auth_response(
-            self.client.send(
-                self.base_crud_path() + "/confirm-verification",
-                {
-                    "method": "POST",
-                    "params": query_params,
-                    "body": body_params,
-                },
-            )
-        )
-
-    def request_email_change(
-        self, new_email: str, body_params: dict = {}, query_params: dict = {}
-    ) -> bool:
-        """Sends an email change request to the authenticated user."""
-        body_params.update({"newEmail": new_email})
-        self.client.send(
-            self.base_crud_path() + "/request-email-change",
-            {
-                "method": "POST",
-                "params": query_params,
-                "body": body_params,
-            },
-        )
-        return True
-
-    def confirm_email_change(
-        self,
-        email_change_token: str,
-        password: str,
-        body_params: dict = {},
-        query_params: dict = {},
-    ) -> UserAuthResponse:
-        """Confirms user new email address."""
-        body_params.update(
-            {
-                "token": email_change_token,
-                "password": password,
-            }
-        )
-        return self.auth_response(
-            self.client.send(
-                self.base_crud_path() + "/confirm-email-change",
-                {
-                    "method": "POST",
-                    "params": query_params,
-                    "body": body_params,
-                },
-            )
-        )
-
-    def list_external_auths(
-        self, user_id: str, query_params: dict = {}
-    ) -> list[ExternalAuth]:
-        """Lists all linked external auth providers for the specified user."""
-        response_data = self.client.send(
-            self.base_crud_path() + "/" + quote(user_id) + "/external-auths",
-            {"method": "GET", "params": query_params},
-        )
-        return [ExternalAuth(item) for item in response_data]
-
-    def unlink_external_auth(
-        self, user_id: str, provider: str, query_params: dict = {}
-    ) -> bool:
-        """Unlink a single external auth provider from the specified user."""
-        self.client.send(
-            self.base_crud_path()
-            + "/"
-            + quote(user_id)
-            + "/external-auths/"
-            + quote(provider),
-            {"method": "DELETE", "params": query_params},
-        )
-        return True
```

### Comparing `pocketbasex-0.2.2/pocketbase/services/utils/crud_service.py` & `pocketbasex-0.8.2/pocketbase/services/utils/crud_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,17 @@
             batch=batch,
             expand=expand,
             filter=filter,
             sort=sort,
             query=query,
             headers=headers,
         )
+    #     self, batch: int = 200, query_params: dict = {}
+    # ) -> list[BaseModel]:
+    #     return self._get_full_list(self.base_crud_path(), batch, query_params)
 
     def get_list(
         self,
         page: int = 1, 
         per_page: int = 30,
         expand: str = None,
         filter: str = None,
@@ -47,15 +50,30 @@
             expand=expand,
             filter=filter,
             sort=sort,
             query=query,
             headers=headers,
         )
 
+    def _get_first_list_item(self, base_path: str, filter: str, query_params):
+        """
+        Returns the first found item by the specified filter.
+
+        Internally it calls `getList(1, 1, { filter })` and returns the
+        first found item.
+
+        For consistency with `getOne`, this method will throw a 404
+        ClientResponseError if no item was found.
+        """
+        return self._get_first_list_item(base_path, filter, query_params)
+
     def get_one(self, id: str, query_params: dict = {}) -> BaseModel:
+        """
+        Returns single item by its id.
+        """
         return self._get_one(self.base_crud_path(), id, query_params)
 
     def create(self, body_params: dict = {}, query_params: dict = {}) -> BaseModel:
         return self._create(self.base_crud_path(), body_params, query_params)
 
     def update(
         self, id: str, body_params: dict = {}, query_params: dict = {}
```

### Comparing `pocketbasex-0.2.2/pocketbase/services/utils/sse.py` & `pocketbasex-0.8.2/pocketbase/services/utils/sse.py`

 * *Files identical despite different names*

### Comparing `pocketbasex-0.2.2/pocketbase/stores/base_auth_store.py` & `pocketbasex-0.8.2/pocketbase/stores/base_auth_store.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 from __future__ import annotations
 
 from abc import ABC
 
 from pocketbase.models.admin import Admin
-from pocketbase.models.user import User
+from pocketbase.models.record import Record
 
 
 class BaseAuthStore(ABC):
     """
     Base AuthStore class that is intended to be extended by all other
     PocketBase AuthStore implementations.
     """
 
     base_token: str
-    base_model: User | Admin | None
+    base_model: Record | Admin | None
 
     def __init__(
-        self, base_token: str = "", base_model: User | Admin | None = None
+        self, base_token: str = "", base_model: Record | Admin | None = None
     ) -> None:
         super().__init__()
         self.base_token = base_token
         self.base_model = base_model
 
     @property
     def token(self) -> str | None:
         """Retrieves the stored token (if any)."""
         return self.base_token
 
     @property
-    def model(self) -> User | Admin | None:
+    def model(self) -> Record | Admin | None:
         """Retrieves the stored model data (if any)."""
         return self.base_model
 
-    def save(self, token: str = "", model: User | Admin | None = None) -> None:
+    def save(self, token: str = "", model: Record | Admin | None = None) -> None:
         """Saves the provided new token and model data in the auth store."""
-        self.base_token = token
-        self.base_model = model
+
+        self.base_token = token if token else ""
+        self.base_model = model if model else None
 
     def clear(self) -> None:
         """Removes the stored token and model data form the auth store."""
         self.base_token = None
         self.base_model = None
```

### Comparing `pocketbasex-0.2.2/pocketbase/stores/local_auth_store.py` & `pocketbasex-0.8.2/pocketbase/stores/local_auth_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 from __future__ import annotations
 
 from typing import Any
 import pickle
 import os
 
 from pocketbase.stores.base_auth_store import BaseAuthStore
-from pocketbase.models.user import User
+from pocketbase.models.record import Record
 from pocketbase.models.admin import Admin
 
 
 class LocalAuthStore(BaseAuthStore):
     filename: str
     filepath: str
 
     def __init__(
         self,
         filename: str = "pocketbase_auth.data",
         filepath: str = "",
         base_token: str = "",
-        base_model: User | Admin | None = None,
+        base_model: Record | Admin | None = None,
     ) -> None:
         super().__init__(base_token, base_model)
         self.filename = filename
         self.filepath = filepath
         self.complete_filepath = os.path.join(filepath, filename)
 
     @property
     def token(self) -> str:
         data = self._storage_get(self.complete_filepath)
         if not data or "token" not in data:
             return None
         return data["token"]
 
     @property
-    def model(self) -> User | Admin | None:
+    def model(self) -> Record | Admin | None:
         data = self._storage_get(self.complete_filepath)
         if not data or "model" not in data:
             return None
         return data["model"]
 
-    def save(self, token: str = "", model: User | Admin | None = None) -> None:
+    def save(self, token: str = "", model: Record | Admin | None = None) -> None:
         self._storage_set(self.complete_filepath, {"token": token, "model": model})
         super().save(token, model)
 
     def clear(self) -> None:
         self._storage_remove(self.complete_filepath)
         super().clear()
```

### Comparing `pocketbasex-0.2.2/pyproject.toml` & `pocketbasex-0.8.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 ]
 description = "PocketBase SDK for python."
 requires-python = ">=3.7"
 license = "MIT"
 authors = [
     { name = "Aziz Berkay Yesilyurt", email = "abyesilyurt@gmail.com" },
     { name = "Vithor Jaeger", email = "vaphes@gmail.com" },
+    { name = "Max Amling", email = "max-amling@web.de" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -20,26 +21,25 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
 ]
 keywords = "pocketbase sdk"
 dependencies = ["httpx>=0.23.0"]
 dynamic = ["readme", "version"]
-
 [project.urls]
 "Homepage" = "https://github.com/abyesilyurt/pocketbase"
 "Source" = "https://github.com/abyesilyurt/pocketbase"
 "Bug Tracker" = "https://github.com/abyesilyurt/pocketbase/issues"
 
 [tool.poetry]
 name = "pocketbasex"
 packages = [
     { include = "pocketbase" },
 ]
-version = "0.2.2"
+version = "0.8.2"
 description = "PocketBase SDK for python."
 authors = ["Aziz Berkay Yesilyurt <abyesilyurt@gmail.com>", "Vithor Jaeger <vaphes@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/abyesilyurt/pocketbase"
 repository = "https://github.com/abyesilyurt/pocketbase"
 keywords = ["pocketbase", "sdk"]
```

### Comparing `pocketbasex-0.2.2/setup.py` & `pocketbasex-0.8.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,107 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pocketbasex
+Version: 0.8.2
+Summary: PocketBase SDK for python.
+Home-page: https://github.com/abyesilyurt/pocketbase
+Keywords: pocketbase,sdk
+Author: Aziz Berkay Yesilyurt
+Author-email: abyesilyurt@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Project-URL: Bug Tracker, https://github.com/abyesilyurt/pocketbase/issues
+Project-URL: Repository, https://github.com/abyesilyurt/pocketbase
+Description-Content-Type: text/markdown
 
-packages = \
-['pocketbase',
- 'pocketbase.models',
- 'pocketbase.models.utils',
- 'pocketbase.services',
- 'pocketbase.services.utils',
- 'pocketbase.stores']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['httpx>=0.23.0,<0.24.0']
-
-setup_kwargs = {
-    'name': 'pocketbasex',
-    'version': '0.2.2',
-    'description': 'PocketBase SDK for python.',
-    'long_description': '# PocketBase Python SDK\n\n[![Tests](https://github.com/vaphes/pocketbase/actions/workflows/tests.yml/badge.svg)](https://github.com/vaphes/pocketbase/actions/workflows/tests.yml)\n\nPython client SDK for the <a href="https://pocketbase.io/">PocketBase</a> backend.\n\nThis is in early development, and at first is just a translation of <a href="https://github.com/pocketbase/js-sdk">the javascript lib</a> using <a href="https://github.com/encode/httpx/">HTTPX</a>.\n\n---\n\n## Installation\n\nInstall PocketBase using pip:\n\n```shell\n$ pip install pocketbase\n```\n\n## Usage\n\nThe rule of thumb here is just to use it as you would <a href="https://github.com/pocketbase/js-sdk">the javascript lib</a>, but in a pythonic way of course!\n\n```python\nfrom pocketbase import PocketBase # Client also works the same\n\nclient = PocketBase(\'http://127.0.0.1:8090\')\n\n...\n\n# list and filter "example" collection records\nresult = client.records.get_list(\n    "example", 1, 20, {"filter": \'status = true && created > "2022-08-01 10:00:00"\'}\n)\n\n# authenticate as regular user\nuser_data = client.users.auth_via_email("test@example.com", "123456")\n\n# or as admin\nadmin_data = client.admins.auth_via_email("test@example.com", "123456")\n\n# and much more...\n```\n> More detailed API docs and copy-paste examples could be found in the [API documentation for each service](https://pocketbase.io/docs/api-authentication). Just remember to \'pythonize it\' 🙃.\n\n\n<p align="center"><i>The PocketBase Python SDK is <a href="https://github.com/vaphes/pocketbase/blob/master/LICENCE.txt">MIT licensed</a> code.</p>',
-    'author': 'Aziz Berkay Yesilyurt',
-    'author_email': 'abyesilyurt@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/abyesilyurt/pocketbase',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+# PocketBase Python SDK
 
+[![Tests](https://github.com/vaphes/pocketbase/actions/workflows/tests.yml/badge.svg)](https://github.com/vaphes/pocketbase/actions/workflows/tests.yml)
+
+Python client SDK for the <a href="https://pocketbase.io/">PocketBase</a> backend.
+
+This is in early development, and at first is just a translation of <a href="https://github.com/pocketbase/js-sdk">the javascript lib</a> using <a href="https://github.com/encode/httpx/">HTTPX</a>.
+
+---
+
+## Installation
+
+Install PocketBase using PIP:
+
+```shell
+python3 -m pip install pocketbase
+```
+
+## Usage
+
+The rule of thumb here is just to use it as you would <a href="https://github.com/pocketbase/js-sdk">the javascript lib</a>, but in a pythonic way of course!
+
+```python
+from pocketbase import PocketBase  # Client also works the same
+from pocketbase.client import FileUpload
+
+client = PocketBase('http://127.0.0.1:8090')
+
+# authenticate as regular user
+user_data = client.collection("users").auth_with_password(
+    "user@example.com", "0123456789")
+
+# or as admin
+admin_data = client.admins.auth_with_password("test@example.com", "0123456789")
+
+# list and filter "example" collection records
+result = client.collection("example").get_list(
+    1, 20, {"filter": 'status = true && created > "2022-08-01 10:00:00"'})
+
+# create record and upload file to image field
+result = client.collection("example").create(
+    {
+        "status": "true",
+        "image": FileUpload(("image.png", open("image.png", "rb"))),
+    })
+
+# and much more...
+```
+> More detailed API docs and copy-paste examples could be found in the [API documentation for each service](https://pocketbase.io/docs/api-authentication). Just remember to 'pythonize it' 🙃.
+
+## Development
+
+These are the requirements for local development:
+
+* Python 3.7+
+* Poetry (https://python-poetry.org/)
+
+You can install locally:
+
+```shell
+poetry install
+```
+
+Or can build and generate a package:
+
+```shell
+poetry build
+```
+
+But if you are using only PIP, use this command:
+
+```shell
+python3 -m pip install -e .
+```
+
+## Tests
+
+To execute the tests use this command:
+
+```
+poetry run pytest
+```
+
+## License
+
+The PocketBase Python SDK is <a href="https://github.com/vaphes/pocketbase/blob/master/LICENCE.txt">MIT licensed</a> code.
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,30 +1,37 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['pocketbase', 'pocketbase.models', 'pocketbase.models.utils',
-'pocketbase.services', 'pocketbase.services.utils', 'pocketbase.stores']
-package_data = \ {'': ['*']} install_requires = \ ['httpx>=0.23.0,<0.24.0']
-setup_kwargs = { 'name': 'pocketbasex', 'version': '0.2.2', 'description':
-'PocketBase SDK for python.', 'long_description': '# PocketBase Python SDK\n\n
-[![Tests](https://github.com/vaphes/pocketbase/actions/workflows/tests.yml/
-badge.svg)](https://github.com/vaphes/pocketbase/actions/workflows/
-tests.yml)\n\nPython client SDK for the PocketBase backend.\n\nThis is in early
-development, and at first is just a translation of the_javascript_lib using
-HTTPX.\n\n---\n\n## Installation\n\nInstall PocketBase using pip:
-\n\n```shell\n$ pip install pocketbase\n```\n\n## Usage\n\nThe rule of thumb
-here is just to use it as you would the_javascript_lib, but in a pythonic way
-of course!\n\n```python\nfrom pocketbase import PocketBase # Client also works
-the same\n\nclient = PocketBase(\'http://127.0.0.1:8090\')\n\n...\n\n# list and
-filter "example" collection records\nresult = client.records.get_list(\n
-"example", 1, 20, {"filter": \'status = true && created > "2022-08-01 10:00:
-00"\'}\n)\n\n# authenticate as regular user\nuser_data =
-client.users.auth_via_email("test@example.com", "123456")\n\n# or as
-admin\nadmin_data = client.admins.auth_via_email("test@example.com",
-"123456")\n\n# and much more...\n```\n> More detailed API docs and copy-paste
-examples could be found in the [API documentation for each service](https://
-pocketbase.io/docs/api-authentication). Just remember to \'pythonize it\'
-ð.\n\n\n
-                The PocketBase Python SDK is MIT_licensed code.
-', 'author': 'Aziz Berkay Yesilyurt', 'author_email': 'abyesilyurt@gmail.com',
-'maintainer': 'None', 'maintainer_email': 'None', 'url': 'https://github.com/
-abyesilyurt/pocketbase', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.7,<4.0', } setup
-(**setup_kwargs)
+Metadata-Version: 2.1 Name: pocketbasex Version: 0.8.2 Summary: PocketBase SDK
+for python. Home-page: https://github.com/abyesilyurt/pocketbase Keywords:
+pocketbase,sdk Author: Aziz Berkay Yesilyurt Author-email:
+abyesilyurt@gmail.com Requires-Python: >=3.7,<4.0 Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: httpx
+(>=0.23.0,<0.24.0) Project-URL: Bug Tracker, https://github.com/abyesilyurt/
+pocketbase/issues Project-URL: Repository, https://github.com/abyesilyurt/
+pocketbase Description-Content-Type: text/markdown # PocketBase Python SDK [!
+[Tests](https://github.com/vaphes/pocketbase/actions/workflows/tests.yml/
+badge.svg)](https://github.com/vaphes/pocketbase/actions/workflows/tests.yml)
+Python client SDK for the PocketBase backend. This is in early development, and
+at first is just a translation of the_javascript_lib using HTTPX. --- ##
+Installation Install PocketBase using PIP: ```shell python3 -m pip install
+pocketbase ``` ## Usage The rule of thumb here is just to use it as you would
+the_javascript_lib, but in a pythonic way of course! ```python from pocketbase
+import PocketBase # Client also works the same from pocketbase.client import
+FileUpload client = PocketBase('http://127.0.0.1:8090') # authenticate as
+regular user user_data = client.collection("users").auth_with_password
+( "user@example.com", "0123456789") # or as admin admin_data =
+client.admins.auth_with_password("test@example.com", "0123456789") # list and
+filter "example" collection records result = client.collection
+("example").get_list( 1, 20, {"filter": 'status = true && created > "2022-08-01
+10:00:00"'}) # create record and upload file to image field result =
+client.collection("example").create( { "status": "true", "image": FileUpload(
+("image.png", open("image.png", "rb"))), }) # and much more... ``` > More
+detailed API docs and copy-paste examples could be found in the [API
+documentation for each service](https://pocketbase.io/docs/api-authentication).
+Just remember to 'pythonize it' ð. ## Development These are the requirements
+for local development: * Python 3.7+ * Poetry (https://python-poetry.org/) You
+can install locally: ```shell poetry install ``` Or can build and generate a
+package: ```shell poetry build ``` But if you are using only PIP, use this
+command: ```shell python3 -m pip install -e . ``` ## Tests To execute the tests
+use this command: ``` poetry run pytest ``` ## License The PocketBase Python
+SDK is MIT_licensed code.
```

