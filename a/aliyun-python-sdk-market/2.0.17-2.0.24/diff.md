# Comparing `tmp/aliyun-python-sdk-market-2.0.17.tar.gz` & `tmp/aliyun-python-sdk-market-2.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-market-2.0.17.tar", last modified: Wed Aug 28 06:37:10 2019, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-market-2.0.24.tar", last modified: Thu Sep  5 06:00:40 2019, max compression
```

## Comparing `aliyun-python-sdk-market-2.0.17.tar` & `aliyun-python-sdk-market-2.0.24.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 admin     (1140) admin     (1140)        0 2019-08-28 06:37:10.000000 aliyun-python-sdk-market-2.0.17/
-drwxrwxr-x   0 admin     (1140) admin     (1140)        0 2019-08-28 06:37:10.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/
-drwxrwxr-x   0 admin     (1140) admin     (1140)        0 2019-08-28 06:37:10.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/
-drwxrwxr-x   0 admin     (1140) admin     (1140)        0 2019-08-28 06:37:10.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/
--rw-rw-r--   0 admin     (1140) admin     (1140)     1253 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/QueryMarketCategoriesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1612 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/CreateCommodityRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1599 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/NotifyContractEventRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1423 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/DescribeCommodityRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1735 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/DescribeInstanceRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1430 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/PushMeteringDataRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2149 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/DescribeProductsRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1697 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/DescribeProductRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2247 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/CreateOrderRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1419 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/DeleteCommodityRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)        0 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/__init__.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1870 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/UploadCommodityFileRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1419 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/DescribeLicenseRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1391 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/DescribeOrderRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1847 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/CreateRateRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1387 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/QueryMarketImagesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     4281 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/DescribeCommoditiesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1569 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/DescribePriceRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1573 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/UpdateCommodityRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1389 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/DescribeRateRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1615 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/ActivateLicenseRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1677 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/BindImagePackageRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1755 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/DescribeInstancesRequest.py
--rw-rw-r--   0 admin     (1140) admin     (1140)        0 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/__init__.py
--rw-rw-r--   0 admin     (1140) admin     (1140)       22 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/__init__.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     2025 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/endpoint.py
--rw-rw-r--   0 admin     (1140) admin     (1140)        0 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/MANIFEST.in
--rw-rw-r--   0 admin     (1140) admin     (1140)     2467 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/setup.py
--rw-rw-r--   0 admin     (1140) admin     (1140)     1553 2019-08-28 06:37:10.000000 aliyun-python-sdk-market-2.0.17/PKG-INFO
--rw-rw-r--   0 admin     (1140) admin     (1140)       59 2019-08-28 06:37:10.000000 aliyun-python-sdk-market-2.0.17/setup.cfg
--rw-rw-r--   0 admin     (1140) admin     (1140)      533 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/README.rst
-drwxrwxr-x   0 admin     (1140) admin     (1140)        0 2019-08-28 06:37:10.000000 aliyun-python-sdk-market-2.0.17/aliyun_python_sdk_market.egg-info/
--rw-rw-r--   0 admin     (1140) admin     (1140)       30 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyun_python_sdk_market.egg-info/requires.txt
--rw-rw-r--   0 admin     (1140) admin     (1140)     1553 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyun_python_sdk_market.egg-info/PKG-INFO
--rw-rw-r--   0 admin     (1140) admin     (1140)       16 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyun_python_sdk_market.egg-info/top_level.txt
--rw-rw-r--   0 admin     (1140) admin     (1140)        1 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyun_python_sdk_market.egg-info/dependency_links.txt
--rw-rw-r--   0 admin     (1140) admin     (1140)     1740 2019-08-28 06:37:09.000000 aliyun-python-sdk-market-2.0.17/aliyun_python_sdk_market.egg-info/SOURCES.txt
+drwxrwxr-x   0 admin     (1140) admin     (1140)        0 2019-09-05 06:00:40.000000 aliyun-python-sdk-market-2.0.24/
+drwxrwxr-x   0 admin     (1140) admin     (1140)        0 2019-09-05 06:00:40.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/
+drwxrwxr-x   0 admin     (1140) admin     (1140)        0 2019-09-05 06:00:40.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/
+drwxrwxr-x   0 admin     (1140) admin     (1140)        0 2019-09-05 06:00:40.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/
+-rw-rw-r--   0 admin     (1140) admin     (1140)     1265 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/QueryMarketCategoriesRequest.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)     1624 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/CreateCommodityRequest.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)     1611 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/NotifyContractEventRequest.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)     1435 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/DescribeCommodityRequest.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)     1747 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/DescribeInstanceRequest.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)     1442 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/PushMeteringDataRequest.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)     2161 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/DescribeProductsRequest.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)     1709 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/DescribeProductRequest.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)     2259 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/CreateOrderRequest.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)     1431 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/DeleteCommodityRequest.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)        0 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/__init__.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)     1882 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/UploadCommodityFileRequest.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)     1431 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/DescribeLicenseRequest.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)     1403 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/DescribeOrderRequest.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)     1859 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/CreateRateRequest.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)     1399 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/QueryMarketImagesRequest.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)     4293 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/DescribeCommoditiesRequest.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)     1581 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/DescribePriceRequest.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)     1585 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/UpdateCommodityRequest.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)     1401 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/DescribeRateRequest.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)     1627 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/ActivateLicenseRequest.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)     1689 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/BindImagePackageRequest.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)     1767 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/DescribeInstancesRequest.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)        0 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/__init__.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)       22 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/__init__.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)     2222 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/endpoint.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)        0 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/MANIFEST.in
+-rw-rw-r--   0 admin     (1140) admin     (1140)     2467 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/setup.py
+-rw-rw-r--   0 admin     (1140) admin     (1140)     1553 2019-09-05 06:00:40.000000 aliyun-python-sdk-market-2.0.24/PKG-INFO
+-rw-rw-r--   0 admin     (1140) admin     (1140)       59 2019-09-05 06:00:40.000000 aliyun-python-sdk-market-2.0.24/setup.cfg
+-rw-rw-r--   0 admin     (1140) admin     (1140)      533 2019-09-05 06:00:38.000000 aliyun-python-sdk-market-2.0.24/README.rst
+drwxrwxr-x   0 admin     (1140) admin     (1140)        0 2019-09-05 06:00:40.000000 aliyun-python-sdk-market-2.0.24/aliyun_python_sdk_market.egg-info/
+-rw-rw-r--   0 admin     (1140) admin     (1140)       30 2019-09-05 06:00:39.000000 aliyun-python-sdk-market-2.0.24/aliyun_python_sdk_market.egg-info/requires.txt
+-rw-rw-r--   0 admin     (1140) admin     (1140)     1553 2019-09-05 06:00:39.000000 aliyun-python-sdk-market-2.0.24/aliyun_python_sdk_market.egg-info/PKG-INFO
+-rw-rw-r--   0 admin     (1140) admin     (1140)       16 2019-09-05 06:00:39.000000 aliyun-python-sdk-market-2.0.24/aliyun_python_sdk_market.egg-info/top_level.txt
+-rw-rw-r--   0 admin     (1140) admin     (1140)        1 2019-09-05 06:00:39.000000 aliyun-python-sdk-market-2.0.24/aliyun_python_sdk_market.egg-info/dependency_links.txt
+-rw-rw-r--   0 admin     (1140) admin     (1140)     1740 2019-09-05 06:00:39.000000 aliyun-python-sdk-market-2.0.24/aliyun_python_sdk_market.egg-info/SOURCES.txt
```

### Comparing `aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/QueryMarketCategoriesRequest.py` & `aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/QueryMarketCategoriesRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmarket.endpoint import endpoint_data
 
 class QueryMarketCategoriesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Market', '2015-11-01', 'QueryMarketCategories')
+		RpcRequest.__init__(self, 'Market', '2015-11-01', 'QueryMarketCategories','yunmarket')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/CreateCommodityRequest.py` & `aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/CreateCommodityRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmarket.endpoint import endpoint_data
 
 class CreateCommodityRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Market', '2015-11-01', 'CreateCommodity')
+		RpcRequest.__init__(self, 'Market', '2015-11-01', 'CreateCommodity','yunmarket')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/NotifyContractEventRequest.py` & `aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/NotifyContractEventRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmarket.endpoint import endpoint_data
 
 class NotifyContractEventRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Market', '2015-11-01', 'NotifyContractEvent')
+		RpcRequest.__init__(self, 'Market', '2015-11-01', 'NotifyContractEvent','yunmarket')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_EventMessage(self):
```

### Comparing `aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/DescribeCommodityRequest.py` & `aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/DeleteCommodityRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmarket.endpoint import endpoint_data
 
-class DescribeCommodityRequest(RpcRequest):
+class DeleteCommodityRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Market', '2015-11-01', 'DescribeCommodity')
+		RpcRequest.__init__(self, 'Market', '2015-11-01', 'DeleteCommodity','yunmarket')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_CommodityId(self):
```

### Comparing `aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/DescribeInstanceRequest.py` & `aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/DescribeInstanceRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,31 +19,31 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmarket.endpoint import endpoint_data
 
 class DescribeInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Market', '2015-11-01', 'DescribeInstance')
+		RpcRequest.__init__(self, 'Market', '2015-11-01', 'DescribeInstance','yunmarket')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
-	def get_InstanceId(self):
-		return self.get_query_params().get('InstanceId')
-
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
 		self.add_query_param('OwnerId',OwnerId)
 
+	def get_InstanceId(self):
+		return self.get_query_params().get('InstanceId')
+
+	def set_InstanceId(self,InstanceId):
+		self.add_query_param('InstanceId',InstanceId)
+
 	def get_OrderType(self):
 		return self.get_query_params().get('OrderType')
 
 	def set_OrderType(self,OrderType):
 		self.add_query_param('OrderType',OrderType)
```

### Comparing `aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/PushMeteringDataRequest.py` & `aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/PushMeteringDataRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmarket.endpoint import endpoint_data
 
 class PushMeteringDataRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Market', '2015-11-01', 'PushMeteringData')
+		RpcRequest.__init__(self, 'Market', '2015-11-01', 'PushMeteringData','yunmarket')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/DescribeProductsRequest.py` & `aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/DescribeProductsRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmarket.endpoint import endpoint_data
 
 class DescribeProductsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Market', '2015-11-01', 'DescribeProducts')
+		RpcRequest.__init__(self, 'Market', '2015-11-01', 'DescribeProducts','yunmarket')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_Filters(self):
```

### Comparing `aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/DescribeProductRequest.py` & `aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/DescribeProductRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmarket.endpoint import endpoint_data
 
 class DescribeProductRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Market', '2015-11-01', 'DescribeProduct')
+		RpcRequest.__init__(self, 'Market', '2015-11-01', 'DescribeProduct','yunmarket')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_Code(self):
```

### Comparing `aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/CreateOrderRequest.py` & `aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/CreateOrderRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmarket.endpoint import endpoint_data
 
 class CreateOrderRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Market', '2015-11-01', 'CreateOrder')
+		RpcRequest.__init__(self, 'Market', '2015-11-01', 'CreateOrder','yunmarket')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_OrderSouce(self):
```

### Comparing `aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/DeleteCommodityRequest.py` & `aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/QueryMarketImagesRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmarket.endpoint import endpoint_data
 
-class DeleteCommodityRequest(RpcRequest):
+class QueryMarketImagesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Market', '2015-11-01', 'DeleteCommodity')
+		RpcRequest.__init__(self, 'Market', '2015-11-01', 'QueryMarketImages','yunmarket')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
-	def get_CommodityId(self):
-		return self.get_query_params().get('CommodityId')
+	def get_Param(self):
+		return self.get_query_params().get('Param')
 
-	def set_CommodityId(self,CommodityId):
-		self.add_query_param('CommodityId',CommodityId)
+	def set_Param(self,Param):
+		self.add_query_param('Param',Param)
```

### Comparing `aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/UploadCommodityFileRequest.py` & `aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/UploadCommodityFileRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmarket.endpoint import endpoint_data
 
 class UploadCommodityFileRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Market', '2015-11-01', 'UploadCommodityFile')
+		RpcRequest.__init__(self, 'Market', '2015-11-01', 'UploadCommodityFile','yunmarket')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/DescribeLicenseRequest.py` & `aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/DescribeLicenseRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmarket.endpoint import endpoint_data
 
 class DescribeLicenseRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Market', '2015-11-01', 'DescribeLicense')
+		RpcRequest.__init__(self, 'Market', '2015-11-01', 'DescribeLicense','yunmarket')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_LicenseCode(self):
```

### Comparing `aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/DescribeOrderRequest.py` & `aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/DescribeOrderRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmarket.endpoint import endpoint_data
 
 class DescribeOrderRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Market', '2015-11-01', 'DescribeOrder')
+		RpcRequest.__init__(self, 'Market', '2015-11-01', 'DescribeOrder','yunmarket')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_OrderId(self):
```

### Comparing `aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/CreateRateRequest.py` & `aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/CreateRateRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmarket.endpoint import endpoint_data
 
 class CreateRateRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Market', '2015-11-01', 'CreateRate')
+		RpcRequest.__init__(self, 'Market', '2015-11-01', 'CreateRate','yunmarket')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_Score(self):
```

### Comparing `aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/QueryMarketImagesRequest.py` & `aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/DescribeRateRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmarket.endpoint import endpoint_data
 
-class QueryMarketImagesRequest(RpcRequest):
+class DescribeRateRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Market', '2015-11-01', 'QueryMarketImages')
+		RpcRequest.__init__(self, 'Market', '2015-11-01', 'DescribeRate','yunmarket')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
-	def get_Param(self):
-		return self.get_query_params().get('Param')
+	def get_OrderId(self):
+		return self.get_query_params().get('OrderId')
 
-	def set_Param(self,Param):
-		self.add_query_param('Param',Param)
+	def set_OrderId(self,OrderId):
+		self.add_query_param('OrderId',OrderId)
```

### Comparing `aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/DescribeCommoditiesRequest.py` & `aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/DescribeCommoditiesRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmarket.endpoint import endpoint_data
 
 class DescribeCommoditiesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Market', '2015-11-01', 'DescribeCommodities')
+		RpcRequest.__init__(self, 'Market', '2015-11-01', 'DescribeCommodities','yunmarket')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_CommodityGmtModifiedTo(self):
@@ -99,17 +99,17 @@
 	def get_CommodityAuditStatuses(self):
 		return self.get_query_params().get('CommodityAuditStatuses')
 
 	def set_CommodityAuditStatuses(self,CommodityAuditStatuses):
 		self.add_query_param('CommodityAuditStatuses',CommodityAuditStatuses)
 
 	def get_Properties(self):
-		return self.get_body_params().get('Properties')
+		return self.get_query_params().get('Properties')
 
 	def set_Properties(self,Properties):
-		self.add_body_params('Properties', Properties)
+		self.add_query_param('Properties',Properties)
 
 	def get_CommodityCategoryIds(self):
 		return self.get_query_params().get('CommodityCategoryIds')
 
 	def set_CommodityCategoryIds(self,CommodityCategoryIds):
 		self.add_query_param('CommodityCategoryIds',CommodityCategoryIds)
```

### Comparing `aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/DescribePriceRequest.py` & `aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/DescribePriceRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmarket.endpoint import endpoint_data
 
 class DescribePriceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Market', '2015-11-01', 'DescribePrice')
+		RpcRequest.__init__(self, 'Market', '2015-11-01', 'DescribePrice','yunmarket')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_Commodity(self):
```

### Comparing `aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/UpdateCommodityRequest.py` & `aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/UpdateCommodityRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmarket.endpoint import endpoint_data
 
 class UpdateCommodityRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Market', '2015-11-01', 'UpdateCommodity')
+		RpcRequest.__init__(self, 'Market', '2015-11-01', 'UpdateCommodity','yunmarket')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_CommodityId(self):
```

### Comparing `aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/DescribeRateRequest.py` & `aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/DescribeCommodityRequest.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmarket.endpoint import endpoint_data
 
-class DescribeRateRequest(RpcRequest):
+class DescribeCommodityRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Market', '2015-11-01', 'DescribeRate')
+		RpcRequest.__init__(self, 'Market', '2015-11-01', 'DescribeCommodity','yunmarket')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
-	def get_OrderId(self):
-		return self.get_query_params().get('OrderId')
+	def get_CommodityId(self):
+		return self.get_query_params().get('CommodityId')
 
-	def set_OrderId(self,OrderId):
-		self.add_query_param('OrderId',OrderId)
+	def set_CommodityId(self,CommodityId):
+		self.add_query_param('CommodityId',CommodityId)
```

### Comparing `aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/ActivateLicenseRequest.py` & `aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/ActivateLicenseRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmarket.endpoint import endpoint_data
 
 class ActivateLicenseRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Market', '2015-11-01', 'ActivateLicense')
+		RpcRequest.__init__(self, 'Market', '2015-11-01', 'ActivateLicense','yunmarket')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_Identification(self):
```

### Comparing `aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/BindImagePackageRequest.py` & `aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/BindImagePackageRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmarket.endpoint import endpoint_data
 
 class BindImagePackageRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Market', '2015-11-01', 'BindImagePackage')
+		RpcRequest.__init__(self, 'Market', '2015-11-01', 'BindImagePackage','yunmarket')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_EcsInstanceId(self):
```

### Comparing `aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/request/v20151101/DescribeInstancesRequest.py` & `aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/request/v20151101/DescribeInstancesRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkmarket.endpoint import endpoint_data
 
 class DescribeInstancesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Market', '2015-11-01', 'DescribeInstances')
+		RpcRequest.__init__(self, 'Market', '2015-11-01', 'DescribeInstances','yunmarket')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_PageSize(self):
```

### Comparing `aliyun-python-sdk-market-2.0.17/aliyunsdkmarket/endpoint.py` & `aliyun-python-sdk-market-2.0.24/aliyunsdkmarket/endpoint.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,19 +22,23 @@
 	def __init__(self):
 		self.endpoint_map = {
 			"cn-shenzhen": "market.aliyuncs.com",
 			"cn-beijing": "market.aliyuncs.com",
 			"ap-south-1": "market.ap-southeast-1.aliyuncs.com",
 			"eu-west-1": "market.ap-southeast-1.aliyuncs.com",
 			"ap-northeast-1": "market.ap-southeast-1.aliyuncs.com",
+			"cn-shenzhen-finance-1": "market.aliyuncs.com",
 			"me-east-1": "market.ap-southeast-1.aliyuncs.com",
 			"cn-chengdu": "market.aliyuncs.com",
+			"cn-north-2-gov-1": "market.aliyuncs.com",
 			"cn-qingdao": "market.aliyuncs.com",
 			"cn-shanghai": "market.aliyuncs.com",
+			"cn-shanghai-finance-1": "market.aliyuncs.com",
 			"cn-hongkong": "market.aliyuncs.com",
+			"cn-hangzhou-finance": "market.aliyuncs.com",
 			"ap-southeast-2": "market.ap-southeast-1.aliyuncs.com",
 			"ap-southeast-3": "market.ap-southeast-1.aliyuncs.com",
 			"eu-central-1": "market.ap-southeast-1.aliyuncs.com",
 			"cn-huhehaote": "market.aliyuncs.com",
 			"ap-southeast-5": "market.ap-southeast-1.aliyuncs.com",
 			"us-east-1": "market.ap-southeast-1.aliyuncs.com",
 			"cn-zhangjiakou": "market.aliyuncs.com",
```

### Comparing `aliyun-python-sdk-market-2.0.17/setup.py` & `aliyun-python-sdk-market-2.0.24/setup.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-market-2.0.17/PKG-INFO` & `aliyun-python-sdk-market-2.0.24/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-market
-Version: 2.0.17
+Version: 2.0.24
 Summary: The market module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-market
```

### Comparing `aliyun-python-sdk-market-2.0.17/README.rst` & `aliyun-python-sdk-market-2.0.24/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-market-2.0.17/aliyun_python_sdk_market.egg-info/PKG-INFO` & `aliyun-python-sdk-market-2.0.24/aliyun_python_sdk_market.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-market
-Version: 2.0.17
+Version: 2.0.24
 Summary: The market module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-market
```

### Comparing `aliyun-python-sdk-market-2.0.17/aliyun_python_sdk_market.egg-info/SOURCES.txt` & `aliyun-python-sdk-market-2.0.24/aliyun_python_sdk_market.egg-info/SOURCES.txt`

 * *Files identical despite different names*

