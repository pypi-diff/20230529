# Comparing `tmp/reduct_py-1.3.1-py3-none-any.whl.zip` & `tmp/reduct_py-1.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9866 bytes, number of entries: 10
--rw-r--r--  2.0 unx      320 b- defN 23-Jan-30 21:32 reduct/__init__.py
--rw-r--r--  2.0 unx     9284 b- defN 23-Jan-30 21:32 reduct/bucket.py
--rw-r--r--  2.0 unx     6151 b- defN 23-Jan-30 21:32 reduct/client.py
--rw-r--r--  2.0 unx      481 b- defN 23-Jan-30 21:32 reduct/error.py
--rw-r--r--  2.0 unx     2994 b- defN 23-Jan-30 21:32 reduct/http.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jan-30 21:32 reduct_py-1.3.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4963 b- defN 23-Jan-30 21:32 reduct_py-1.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-30 21:32 reduct_py-1.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jan-30 21:32 reduct_py-1.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      757 b- defN 23-Jan-30 21:32 reduct_py-1.3.1.dist-info/RECORD
-10 files, 26118 bytes uncompressed, 8588 bytes compressed:  67.1%
+Zip file size: 10242 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      320 b- defN 23-May-29 21:15 reduct/__init__.py
+-rw-r--r--  2.0 unx    11150 b- defN 23-May-29 21:15 reduct/bucket.py
+-rw-r--r--  2.0 unx     6151 b- defN 23-May-29 21:15 reduct/client.py
+-rw-r--r--  2.0 unx      481 b- defN 23-May-29 21:15 reduct/error.py
+-rw-r--r--  2.0 unx     3188 b- defN 23-May-29 21:15 reduct/http.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-May-29 21:15 reduct_py-1.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5002 b- defN 23-May-29 21:15 reduct_py-1.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-29 21:15 reduct_py-1.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-29 21:15 reduct_py-1.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      758 b- defN 23-May-29 21:15 reduct_py-1.4.0.dist-info/RECORD
+10 files, 28218 bytes uncompressed, 8964 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: reduct/error.py
 Comment: 
 
 Filename: reduct/http.py
 Comment: 
 
-Filename: reduct_py-1.3.1.dist-info/LICENSE
+Filename: reduct_py-1.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: reduct_py-1.3.1.dist-info/METADATA
+Filename: reduct_py-1.4.0.dist-info/METADATA
 Comment: 
 
-Filename: reduct_py-1.3.1.dist-info/WHEEL
+Filename: reduct_py-1.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: reduct_py-1.3.1.dist-info/top_level.txt
+Filename: reduct_py-1.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: reduct_py-1.3.1.dist-info/RECORD
+Filename: reduct_py-1.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## reduct/bucket.py

```diff
@@ -1,8 +1,9 @@
 """Bucket API"""
+import asyncio
 import json
 import time
 from contextlib import asynccontextmanager
 from dataclasses import dataclass
 from enum import Enum
 from typing import (
     Optional,
@@ -101,15 +102,15 @@
     """Record in a query"""
 
     timestamp: int
     """UNIX timestamp in microseconds"""
     size: int
     """size of data"""
     last: bool
-    """last record in the query"""
+    """last record in the query. Deprecated: doesn't work for some cases"""
     content_type: str
     """content type of data"""
     read_all: Callable[[None], Awaitable[bytes]]
     """read all data"""
     read: Callable[[int], AsyncIterator[bytes]]
     """read data in chunks"""
 
@@ -210,15 +211,15 @@
         Raises:
             ReductError: if there is an HTTP error
         Examples:
             >>> async def reader():
             >>>     async with bucket.read("entry", timestamp=123456789) as record:
             >>>         data = await record.read_all()
         """
-        params = {"ts": timestamp} if timestamp else None
+        params = {"ts": int(timestamp)} if timestamp else None
         async with self._http.request(
             "GET", f"/b/{self.name}/{entry_name}", params=params
         ) as resp:
             yield _parse_record(resp)
 
     async def write(
         self,
@@ -251,15 +252,16 @@
             >>>
             >>> async def sender():
             >>>     for chunk in [b"part1", b"part2", b"part3"]:
             >>>         yield chunk
             >>> await bucket.write("entry-1", sender(), content_length=15)
 
         """
-        params = {"ts": timestamp if timestamp else time.time_ns() / 1000}
+        timestamp = timestamp if timestamp else time.time_ns() / 1000
+        params = {"ts": int(timestamp)}
         await self._http.request_all(
             "POST",
             f"/b/{self.name}/{entry_name}",
             params=params,
             data=data,
             content_length=content_length if content_length is not None else len(data),
             **kwargs,
@@ -279,54 +281,100 @@
         Args:
             entry_name: name of entry in the bucket
             start: the beginning of the time interval
             stop: the end of the time interval
             ttl: Time To Live of the request in seconds
         Keyword Args:
             include (dict): query records which have all labels from this dict
-            exclude (dict): querz records which doesn't have all labels from this dict
+            exclude (dict): query records which doesn't have all labels from this dict
         Returns:
              AsyncIterator[Record]: iterator to the records
 
         Examples:
             >>> async for record in bucket.query("entry-1", stop=time.time_ns() / 1000):
             >>>     data: bytes = record.read_all()
             >>>     # or
             >>>     async for chunk in record.read(n=1024):
             >>>         print(chunk)
         """
+        query_id = await self._query(entry_name, start, stop, ttl, **kwargs)
+        last = False
+        while not last:
+            async with self._http.request(
+                "GET", f"/b/{self.name}/{entry_name}?q={query_id}"
+            ) as resp:
+                if resp.status == 204:
+                    return
+                last = int(resp.headers["x-reduct-last"]) != 0
+                yield _parse_record(resp, last)
+
+    async def get_full_info(self) -> BucketFullInfo:
+        """
+        Get full information about bucket (settings, statistics, entries)
+        """
+        return BucketFullInfo.parse_raw(
+            await self._http.request_all("GET", f"/b/{self.name}")
+        )
+
+    async def subscribe(
+        self, entry_name: str, start: Optional[int] = None, poll_interval=1.0, **kwargs
+    ) -> AsyncIterator[Record]:
+        """
+        Query records from the start timestamp and wait for new records
+
+        Args:
+            entry_name: name of entry in the bucket
+            start: the beginning timestamp to read records
+            poll_interval: inteval to ask new records in seconds
+        Keyword Args:
+            include (dict): query records which have all labels from this dict
+            exclude (dict): query records which doesn't have all labels from this dict
+        Returns:
+             AsyncIterator[Record]: iterator to the records
+
+        Examples:
+            >>> async for record in bucket.subscribes("entry-1"):
+            >>>     data: bytes = record.read_all()
+            >>>     # or
+            >>>     async for chunk in record.read(n=1024):
+            >>>         print(chunk)
+        """
+        query_id = await self._query(
+            entry_name, start, None, poll_interval * 2 + 1, continuous=True, **kwargs
+        )
+        while True:
+            async with self._http.request(
+                "GET", f"/b/{self.name}/{entry_name}?q={query_id}"
+            ) as resp:
+                if resp.status == 204:
+                    await asyncio.sleep(poll_interval)
+                    continue
+
+                yield _parse_record(resp, False)
+
+    async def _query(self, entry_name, start, stop, ttl, **kwargs):
         params = {}
         if start:
-            params["start"] = start
+            params["start"] = int(start)
         if stop:
-            params["stop"] = stop
+            params["stop"] = int(stop)
         if ttl:
-            params["ttl"] = ttl
+            params["ttl"] = int(ttl)
+
         if "include" in kwargs:
             for name, value in kwargs["include"].items():
                 params[f"include-{name}"] = str(value)
         if "exclude" in kwargs:
             for name, value in kwargs["exclude"].items():
                 params[f"exclude-{name}"] = str(value)
 
+        if "continuous" in kwargs:
+            params["continuous"] = "true" if kwargs["continuous"] else "false"
+
         url = f"/b/{self.name}/{entry_name}"
         data = await self._http.request_all(
             "GET",
             f"{url}/q",
             params=params,
         )
         query_id = json.loads(data)["id"]
-        last = False
-        while not last:
-            async with self._http.request("GET", f"{url}?q={query_id}") as resp:
-                if resp.status == 204:
-                    return
-                last = int(resp.headers["x-reduct-last"]) != 0
-                yield _parse_record(resp, last)
-
-    async def get_full_info(self) -> BucketFullInfo:
-        """
-        Get full information about bucket (settings, statistics, entries)
-        """
-        return BucketFullInfo.parse_raw(
-            await self._http.request_all("GET", f"/b/{self.name}")
-        )
+        return query_id
```

## reduct/http.py

```diff
@@ -27,16 +27,22 @@
     @asynccontextmanager
     async def request(
         self, method: str, path: str = "", **kwargs
     ) -> AsyncIterator[ClientResponse]:
         """HTTP request with ReductError exception"""
 
         extra_headers = {}
+
         if "content_length" in kwargs:
-            extra_headers["Content-Length"] = str(kwargs["content_length"])
+            content_length = kwargs["content_length"]
+            extra_headers["Content-Length"] = str(content_length)
+            if content_length > 256_000:
+                # Use 100-continue for large files
+                extra_headers["Expect"] = "100-continue"
+
             del kwargs["content_length"]
 
         if "content_type" in kwargs:
             extra_headers["Content-Type"] = str(kwargs["content_type"])
             del kwargs["content_type"]
 
         if "labels" in kwargs:
@@ -49,15 +55,14 @@
             try:
                 async with session.request(
                     method,
                     f"{self.url}{path.strip()}",
                     headers=dict(self.headers, **extra_headers),
                     **kwargs,
                 ) as response:
-
                     if response.ok:
                         yield response
                     else:
                         if "x-reduct-error" in response.headers:
                             raise ReductError(
                                 response.status,
                                 response.headers["x-reduct-error"],
```

## Comparing `reduct_py-1.3.1.dist-info/LICENSE` & `reduct_py-1.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `reduct_py-1.3.1.dist-info/METADATA` & `reduct_py-1.4.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reduct-py
-Version: 1.3.1
+Version: 1.4.0
 Summary: ReductStore Client SDK for Python
 Author: Ciaran Moyne
 Author-email: Alexey Timin <atimin@gmail.com>
 Maintainer-email: Alexey Timin <atimin@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Alexey Timin
@@ -70,16 +70,20 @@
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/reduct-py)](https://pypi.org/project/reduct-py/)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/reductstore/reduct-py/ci.yml?branch=main)](https://github.com/reductstore/reduct-py/actions)
 
 This package provides an asynchronous HTTP client for interacting with the [ReductStore](https://www.reduct.store) service.
 
 ## Features
 
-* Supports the [ReductStore HTTP API v1.3](https://docs.reduct.store/http-api)
-* Asynchronous and based on aiohttp and pydantic
+* Supports the [ReductStore HTTP API v1.4](https://docs.reduct.store/http-api)
+* Bucket management
+* API Token management
+* Write, read and query data
+* Labels
+* Subscription on new data
 
 ## Install
 
 To install this package, run the following command:
 
 ```
 pip install reduct-py
@@ -91,16 +95,16 @@
 
 ```python
 import time
 import asyncio
 from reduct import Client, Bucket
 
 async def main():
-    # Create a client for interacting with the ReductStore service
-    client = Client('https://play.reduct.store', api_token="reduct")
+    # Create a client for interacting with a ReductStore service
+    client = Client("http://localhost:80383")
 
     # Create a bucket and store a reference to it in the `bucket` variable
     bucket: Bucket = await client.create_bucket("my-bucket", exist_ok=True)
 
     # Write data to the bucket
     ts = time.time_ns() / 1000
     await bucket.write("entry-1", b"Hey!!", ts)
@@ -111,13 +115,13 @@
         print(data)
 
 # Run the main function
 loop = asyncio.get_event_loop()
 loop.run_until_complete(main())
 ```
 
-For more examples, see the [Quick Start](https://py.reduct.store/en/latest/docs/quick-start/).
+For more examples, see the [Quick Start](https://py.reduct.storgit ce/en/latest/docs/quick-start/).
 
 ## References
 
 * [Documentation](https://py.reduct.store/)
 * [ReductStore HTTP API](https://docs.reduct.store/http-api)
```

