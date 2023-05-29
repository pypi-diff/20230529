# Comparing `tmp/gpru-0.0.1.tar.gz` & `tmp/gpru-0.0.2.tar.gz`

## Comparing `gpru-0.0.1.tar` & `gpru-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 gpru-0.0.1/gpru/__init__.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 gpru-0.0.1/gpru/_client.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 gpru-0.0.1/gpru/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.1/gpru/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.1/gpru/azure/__init__.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 gpru-0.0.1/gpru/azure/_api.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 gpru-0.0.1/gpru/azure/_utils.py
--rw-r--r--   0        0        0    37127 2020-02-02 00:00:00.000000 gpru-0.0.1/gpru/azure/preview_2022_03_01.py
--rw-r--r--   0        0        0    40334 2020-02-02 00:00:00.000000 gpru-0.0.1/gpru/azure/preview_2022_06_01.py
--rw-r--r--   0        0        0    54437 2020-02-02 00:00:00.000000 gpru-0.0.1/gpru/azure/preview_2023_03_15.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.1/gpru/azure/py.typed
--rw-r--r--   0        0        0    46855 2020-02-02 00:00:00.000000 gpru-0.0.1/gpru/azure/stable_2022_12_01.py
--rw-r--r--   0        0        0    49096 2020-02-02 00:00:00.000000 gpru-0.0.1/gpru/azure/stable_2023_05_15.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.1/gpru/openai/__init__.py
--rw-r--r--   0        0        0    55110 2020-02-02 00:00:00.000000 gpru-0.0.1/gpru/openai/api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.1/gpru/openai/py.typed
--rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 gpru-0.0.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 gpru-0.0.1/LICENSE
--rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 gpru-0.0.1/README.md
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 gpru-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 gpru-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/__init__.py
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/_client.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/azure/__init__.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/azure/_api.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/azure/_utils.py
+-rw-r--r--   0        0        0    37103 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/azure/preview_2022_03_01.py
+-rw-r--r--   0        0        0    40310 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/azure/preview_2022_06_01.py
+-rw-r--r--   0        0        0    54413 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/azure/preview_2023_03_15.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/azure/py.typed
+-rw-r--r--   0        0        0    46831 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/azure/stable_2022_12_01.py
+-rw-r--r--   0        0        0    49072 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/azure/stable_2023_05_15.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/openai/__init__.py
+-rw-r--r--   0        0        0    55082 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/openai/api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpru-0.0.2/gpru/openai/py.typed
+-rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 gpru-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 gpru-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 gpru-0.0.2/README.md
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 gpru-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5512 2020-02-02 00:00:00.000000 gpru-0.0.2/PKG-INFO
```

### Comparing `gpru-0.0.1/gpru/_client.py` & `gpru-0.0.2/gpru/_client.py`

 * *Files identical despite different names*

### Comparing `gpru-0.0.1/gpru/exceptions.py` & `gpru-0.0.2/gpru/exceptions.py`

 * *Files identical despite different names*

### Comparing `gpru-0.0.1/gpru/azure/_api.py` & `gpru-0.0.2/gpru/azure/_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,37 +9,37 @@
 
 class Api:
     def __init__(  # noqa: PLR0913
         self,
         error_response_model: Type[T],
         endpoint: str,
         api_version: str,
-        api_key: Optional[str] = None,
+        key: Optional[str] = None,
         ad_token: Optional[str] = None,
         timeout: Optional[TimeoutTypes] = DEFAULT_TIMEOUT_CONFIG,
     ) -> None:
         client_kwargs = {
             "params": {"api-version": api_version},
-            "headers": self._build_base_headers(api_key, ad_token),
+            "headers": self._build_base_headers(key, ad_token),
             "http2": True,
             "base_url": f"{endpoint}openai"
             if endpoint.endswith("/")
             else f"{endpoint}/openai",
             "timeout": timeout,
         }
         self._request = request_factory(error_response_model, **client_kwargs)
         self._stream = stream_factory(error_response_model, **client_kwargs)
 
     def _build_base_headers(
-        self, api_key: Optional[str], ad_token: Optional[str]
+        self, key: Optional[str], ad_token: Optional[str]
     ) -> Dict[str, str]:
-        both_none: bool = api_key is None and ad_token is None
-        both_not_none: bool = api_key is not None and ad_token is not None
+        both_none: bool = key is None and ad_token is None
+        both_not_none: bool = key is not None and ad_token is not None
         if both_none or both_not_none:
-            msg = "Either `api_key` or `ad_token` is required."
+            msg = "Either `key` or `ad_token` is required."
             raise InvalidConfigError(msg)
 
         return (
-            {"api-key": api_key}
-            if api_key is not None
+            {"api-key": key}
+            if key is not None
             else {"Authorization": f"Bearer {ad_token}"}
         )
```

### Comparing `gpru-0.0.1/gpru/azure/preview_2022_03_01.py` & `gpru-0.0.2/gpru/azure/preview_2022_03_01.py`

 * *Files 1% similar despite different names*

```diff
@@ -675,30 +675,30 @@
     - [Official authoring API specification](https://github.com/Azure/azure-rest-api-specs/blob/main/specification/cognitiveservices/data-plane/AzureOpenAI/authoring/preview/2022-03-01-preview/azureopenai.json)
     - [Official inference API specification](https://github.com/Azure/azure-rest-api-specs/blob/main/specification/cognitiveservices/data-plane/AzureOpenAI/inference/preview/2022-03-01-preview/inference.json)
     """
 
     def __init__(
         self,
         endpoint: str,
-        api_key: Optional[str] = None,
+        key: Optional[str] = None,
         ad_token: Optional[str] = None,
         timeout: Optional[TimeoutTypes] = DEFAULT_TIMEOUT_CONFIG,
     ) -> None:
         """
         Initialize a client for the Azure OpenAI API version `2022-03-01-preview`.
 
         Notes
         -----
-        Either `api_key` or `ad_token` is required.
+        Either `key` or `ad_token` is required.
 
         Parameters
         ----------
         endpoint : str
             URL in the form of `"https://{your-resource-name}.openai.azure.com/"`
-        api_key : Optional[str]
+        key : Optional[str]
             Secret key for the Azure OpenAI API.
         ad_token : Optional[str]
             Azure Active Directory token.
         timeout : Optional[TimeoutTypes]
             Timeout configuration to use when sending requests, by default
             `DEFAULT_TIMEOUT_CONFIG`. See [HTTPX - Timeout Configuration](https://www.python-httpx.org/advanced/#timeout-configuration)
             for more information.
@@ -708,22 +708,22 @@
         InvalidConfigError
             When the configuration is invalid.
 
         Examples
         --------
         >>> import os
         >>> endpoint = os.environ["AZURE_OPENAI_API_ENDPOINT"]
-        >>> api_key = os.environ["AZURE_OPENAI_API_KEY"]
-        >>> api = AzureOpenAiApi(endpoint, api_key)
+        >>> key = os.environ["AZURE_OPENAI_API_KEY"]
+        >>> api = AzureOpenAiApi(endpoint, key)
         """
         super().__init__(
             ErrorResponse,
             endpoint,
             "2022-03-01-preview",
-            api_key,
+            key,
             ad_token,
             timeout,
         )
 
     def list_deployments(self) -> DeploymentList:
         """
         Get the list of deployments owned by the Azure OpenAI resource.
```

### Comparing `gpru-0.0.1/gpru/azure/preview_2022_06_01.py` & `gpru-0.0.2/gpru/azure/preview_2022_06_01.py`

 * *Files 0% similar despite different names*

```diff
@@ -732,30 +732,30 @@
     - [Official authoring API specification](https://github.com/Azure/azure-rest-api-specs/blob/main/specification/cognitiveservices/data-plane/AzureOpenAI/authoring/preview/2022-06-01-preview/azureopenai.json)
     - [Official inference API specification](https://github.com/Azure/azure-rest-api-specs/blob/main/specification/cognitiveservices/data-plane/AzureOpenAI/inference/preview/2022-06-01-preview/inference.json)
     """
 
     def __init__(
         self,
         endpoint: str,
-        api_key: Optional[str] = None,
+        key: Optional[str] = None,
         ad_token: Optional[str] = None,
         timeout: Optional[TimeoutTypes] = DEFAULT_TIMEOUT_CONFIG,
     ) -> None:
         """
         Initialize a client for the Azure OpenAI API version `2022-06-01-preview`.
 
         Notes
         -----
-        Either `api_key` or `ad_token` is required.
+        Either `key` or `ad_token` is required.
 
         Parameters
         ----------
         endpoint : str
             URL in the form of `"https://{your-resource-name}.openai.azure.com/"`
-        api_key : Optional[str]
+        key : Optional[str]
             Secret key for the Azure OpenAI API.
         ad_token : Optional[str]
             Azure Active Directory token.
         timeout : Optional[TimeoutTypes]
             Timeout configuration to use when sending requests, by default
             `DEFAULT_TIMEOUT_CONFIG`. See [HTTPX - Timeout Configuration](https://www.python-httpx.org/advanced/#timeout-configuration)
             for more information.
@@ -765,22 +765,22 @@
         InvalidConfigError
             When the configuration is invalid.
 
         Examples
         --------
         >>> import os
         >>> endpoint = os.environ["AZURE_OPENAI_API_ENDPOINT"]
-        >>> api_key = os.environ["AZURE_OPENAI_API_KEY"]
-        >>> api = AzureOpenAiApi(endpoint, api_key)
+        >>> key = os.environ["AZURE_OPENAI_API_KEY"]
+        >>> api = AzureOpenAiApi(endpoint, key)
         """
         super().__init__(
             ErrorResponse,
             endpoint,
             "2022-06-01-preview",
-            api_key,
+            key,
             ad_token,
             timeout,
         )
 
     def list_deployments(self) -> DeploymentList:
         """
         Get the list of deployments owned by the Azure OpenAI resource.
```

### Comparing `gpru-0.0.1/gpru/azure/preview_2023_03_15.py` & `gpru-0.0.2/gpru/azure/preview_2023_03_15.py`

 * *Files 0% similar despite different names*

```diff
@@ -1133,30 +1133,30 @@
     - [Official authoring API specification](https://github.com/Azure/azure-rest-api-specs/blob/main/specification/cognitiveservices/data-plane/AzureOpenAI/authoring/preview/2023-03-15-preview/azureopenai.json)
     - [Official inference API specification](https://github.com/Azure/azure-rest-api-specs/blob/main/specification/cognitiveservices/data-plane/AzureOpenAI/inference/preview/2023-03-15-preview/inference.json)
     """
 
     def __init__(
         self,
         endpoint: str,
-        api_key: Optional[str] = None,
+        key: Optional[str] = None,
         ad_token: Optional[str] = None,
         timeout: Optional[TimeoutTypes] = DEFAULT_TIMEOUT_CONFIG,
     ) -> None:
         """
         Initialize a client for the Azure OpenAI API version `2023-03-15-preview`.
 
         Notes
         -----
-        Either `api_key` or `ad_token` is required.
+        Either `key` or `ad_token` is required.
 
         Parameters
         ----------
         endpoint : str
             URL in the form of `"https://{your-resource-name}.openai.azure.com/"`
-        api_key : Optional[str]
+        key : Optional[str]
             Secret key for the Azure OpenAI API.
         ad_token : Optional[str]
             Azure Active Directory token.
         timeout : Optional[TimeoutTypes]
             Timeout configuration to use when sending requests, by default
             `DEFAULT_TIMEOUT_CONFIG`. See [HTTPX - Timeout Configuration](https://www.python-httpx.org/advanced/#timeout-configuration)
             for more information.
@@ -1166,22 +1166,22 @@
         InvalidConfigError
             When the configuration is invalid.
 
         Examples
         --------
         >>> import os
         >>> endpoint = os.environ["AZURE_OPENAI_API_ENDPOINT"]
-        >>> api_key = os.environ["AZURE_OPENAI_API_KEY"]
-        >>> api = AzureOpenAiApi(endpoint, api_key)
+        >>> key = os.environ["AZURE_OPENAI_API_KEY"]
+        >>> api = AzureOpenAiApi(endpoint, key)
         """
         super().__init__(
             ErrorResponse,
             endpoint,
             "2023-03-15-preview",
-            api_key,
+            key,
             ad_token,
             timeout,
         )
 
     def list_deployments(self) -> DeploymentList:
         """
         Get the list of deployments owned by the Azure OpenAI resource.
```

### Comparing `gpru-0.0.1/gpru/azure/stable_2022_12_01.py` & `gpru-0.0.2/gpru/azure/stable_2022_12_01.py`

 * *Files 1% similar despite different names*

```diff
@@ -919,30 +919,30 @@
     - [Official authoring API specification](https://github.com/Azure/azure-rest-api-specs/blob/main/specification/cognitiveservices/data-plane/AzureOpenAI/authoring/stable/2022-12-01/azureopenai.json)
     - [Official inference API specification](https://github.com/Azure/azure-rest-api-specs/blob/main/specification/cognitiveservices/data-plane/AzureOpenAI/inference/stable/2022-12-01/inference.json)
     """
 
     def __init__(
         self,
         endpoint: str,
-        api_key: Optional[str] = None,
+        key: Optional[str] = None,
         ad_token: Optional[str] = None,
         timeout: Optional[TimeoutTypes] = DEFAULT_TIMEOUT_CONFIG,
     ) -> None:
         """
         Initialize a client for the Azure OpenAI API version `2022-12-01`.
 
         Notes
         -----
-        Either `api_key` or `ad_token` is required.
+        Either `key` or `ad_token` is required.
 
         Parameters
         ----------
         endpoint : str
             URL in the form of `"https://{your-resource-name}.openai.azure.com/"`
-        api_key : Optional[str]
+        key : Optional[str]
             Secret key for the Azure OpenAI API.
         ad_token : Optional[str]
             Azure Active Directory token.
         timeout : Optional[TimeoutTypes]
             Timeout configuration to use when sending requests, by default
             `DEFAULT_TIMEOUT_CONFIG`. See [HTTPX - Timeout Configuration](https://www.python-httpx.org/advanced/#timeout-configuration)
             for more information.
@@ -952,22 +952,22 @@
         InvalidConfigError
             When the configuration is invalid.
 
         Examples
         --------
         >>> import os
         >>> endpoint = os.environ["AZURE_OPENAI_API_ENDPOINT"]
-        >>> api_key = os.environ["AZURE_OPENAI_API_KEY"]
-        >>> api = AzureOpenAiApi(endpoint, api_key)
+        >>> key = os.environ["AZURE_OPENAI_API_KEY"]
+        >>> api = AzureOpenAiApi(endpoint, key)
         """
         super().__init__(
             ErrorResponse,
             endpoint,
             "2022-12-01",
-            api_key,
+            key,
             ad_token,
             timeout,
         )
 
     def list_deployments(self) -> DeploymentList:
         """
         Get the list of deployments owned by the Azure OpenAI resource.
```

### Comparing `gpru-0.0.1/gpru/azure/stable_2023_05_15.py` & `gpru-0.0.2/gpru/azure/stable_2023_05_15.py`

 * *Files 1% similar despite different names*

```diff
@@ -1052,30 +1052,30 @@
     - [Official authoring API specification](https://github.com/Azure/azure-rest-api-specs/blob/main/specification/cognitiveservices/data-plane/AzureOpenAI/authoring/stable/2023-05-15/azureopenai.json)
     - [Official inference API specification](https://github.com/Azure/azure-rest-api-specs/blob/main/specification/cognitiveservices/data-plane/AzureOpenAI/inference/stable/2023-05-15/inference.json)
     """
 
     def __init__(
         self,
         endpoint: str,
-        api_key: Optional[str] = None,
+        key: Optional[str] = None,
         ad_token: Optional[str] = None,
         timeout: Optional[TimeoutTypes] = DEFAULT_TIMEOUT_CONFIG,
     ) -> None:
         """
         Initialize a client for the Azure OpenAI API version `2023-05-15`.
 
         Notes
         -----
-        Either `api_key` or `ad_token` is required.
+        Either `key` or `ad_token` is required.
 
         Parameters
         ----------
         endpoint : str
             URL in the form of `"https://{your-resource-name}.openai.azure.com/"`
-        api_key : Optional[str]
+        key : Optional[str]
             Secret key for the Azure OpenAI API.
         ad_token : Optional[str]
             Azure Active Directory token.
         timeout : Optional[TimeoutTypes]
             Timeout configuration to use when sending requests, by default
             `DEFAULT_TIMEOUT_CONFIG`. See [HTTPX - Timeout Configuration](https://www.python-httpx.org/advanced/#timeout-configuration)
             for more information.
@@ -1085,22 +1085,22 @@
         InvalidConfigError
             When the configuration is invalid.
 
         Examples
         --------
         >>> import os
         >>> endpoint = os.environ["AZURE_OPENAI_API_ENDPOINT"]
-        >>> api_key = os.environ["AZURE_OPENAI_API_KEY"]
-        >>> api = AzureOpenAiApi(endpoint, api_key)
+        >>> key = os.environ["AZURE_OPENAI_API_KEY"]
+        >>> api = AzureOpenAiApi(endpoint, key)
         """
         super().__init__(
             ErrorResponse,
             endpoint,
             "2023-05-15",
-            api_key,
+            key,
             ad_token,
             timeout,
         )
 
     def list_files(self) -> FileList:
         """
         Get a list of all files owned by the Azure OpenAI resource. These include user
```

### Comparing `gpru-0.0.1/gpru/openai/api.py` & `gpru-0.0.2/gpru/openai/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1184,25 +1184,25 @@
     Notes
     -----
     Clients for deprecated APIs are not implemented.
     """
 
     def __init__(
         self,
-        api_key: str,
+        key: str,
         organization_id: Optional[str] = None,
         timeout: Optional[TimeoutTypes] = DEFAULT_TIMEOUT_CONFIG,
         base_url: Optional[str] = "https://api.openai.com/v1",
     ) -> None:
         """
         Initialize a client for the OpenAI API version `1.2.0`.
 
         Parameters
         ----------
-        api_key : str
+        key : str
             API key for authentication, which can be found on the [API Keys page](https://platform.openai.com/account/api-keys).
         organization_id : Optional[str]
             Optional value used to specify which organization's subscription quota is
             counted for API requests by users belonging to multiple organizations, which
             can be found on the [Organization's settings page](https://platform.openai.com/account/org-settings).
         timeout : Optional[TimeoutTypes]
             Timeout configuration to use when sending requests, by default
@@ -1210,30 +1210,30 @@
             for more information.
         base_url : Optional[str]
             API endpoint, by default `"https://api.openai.com/v1"`.
 
         Examples
         --------
         >>> import os
-        >>> api_key = os.environ["OPENAI_API_KEY"]
-        >>> api = OpenAiApi(api_key)
+        >>> key = os.environ["OPENAI_API_KEY"]
+        >>> api = OpenAiApi(key)
         """
         client_kwargs = {
-            "headers": self._build_base_headers(api_key, organization_id),
+            "headers": self._build_base_headers(key, organization_id),
             "http2": True,
             "base_url": base_url,
             "timeout": timeout,
         }
         self._request = request_factory(ErrorResponse, **client_kwargs)
         self._stream = stream_factory(ErrorResponse, **client_kwargs)
 
     def _build_base_headers(
-        self, api_key: str, organization_id: Optional[str]
+        self, key: str, organization_id: Optional[str]
     ) -> Dict[str, str]:
-        headers = {"Authorization": f"Bearer {api_key}"}
+        headers = {"Authorization": f"Bearer {key}"}
         if organization_id is not None:
             headers["OpenAI-Organization"] = organization_id
         return headers
 
     def create_completion(
         self, completion_request: CompletionRequest
     ) -> Union[Generator[Completion, None, None], Completion]:
```

### Comparing `gpru-0.0.1/.gitignore` & `gpru-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gpru-0.0.1/LICENSE` & `gpru-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpru-0.0.1/README.md` & `gpru-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 Here is an example of [chat completion](https://platform.openai.com/docs/api-reference/chat/create), also known as [ChatGPT](https://chat.openai.com/).
 
 ```python
 import os
 
 from gpru.openai.api import ChatCompletionRequest, OpenAiApi, UserMessage
 
-api_key = os.environ["OPENAI_API_KEY"]
-api = OpenAiApi(api_key)
+key = os.environ["OPENAI_API_KEY"]
+api = OpenAiApi(key)
 
 req = ChatCompletionRequest(model="gpt-3.5-turbo", messages=[UserMessage("Hello!")])
 chat_completion = api.create_chat_completion(req)
 print(chat_completion.content)
 # Greetings! How can I assist you today?
 ```
 
@@ -75,16 +75,16 @@
 from gpru.azure.stable_2023_05_15 import (
     AzureOpenAiApi,
     ChatCompletionRequest,
     UserMessage,
 )
 
 endpoint = os.environ["AZURE_OPENAI_API_ENDPOINT"]
-api_key = os.environ["AZURE_OPENAI_API_KEY"]
+key = os.environ["AZURE_OPENAI_API_KEY"]
 deployment_id = os.environ["AZURE_OPENAI_API_DEPLOYMENT_ID"]
-api = AzureOpenAiApi(endpoint, api_key)
+api = AzureOpenAiApi(endpoint, key)
 
 req = ChatCompletionRequest(messages=[UserMessage("Hello!")])
 chat_completion = api.create_chat_completion(deployment_id, req)
 print(chat_completion.content)
 # Greetings! How can I assist you today?
 ```
```

### Comparing `gpru-0.0.1/pyproject.toml` & `gpru-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 [tool.hatch.envs.default.scripts]
 cov = [
   "test-cov",
   "cov-report",
 ]
 cov-report = [
   "- coverage combine",
-  "coverage report",
+  "coverage report --show-missing",
 ]
 gen-model = "datamodel-codegen --openapi-scopes=schemas --snake-case-field --use-schema-description --use-field-description --reuse-model --capitalise-enum-members --use-subclass-enum --target-python-version=3.7 --wrap-string-literal --output=models.py {args:}"
 pc-run = "pre-commit run --all-files"
 pc-update = "pre-commit autoupdate"
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
```

### Comparing `gpru-0.0.1/PKG-INFO` & `gpru-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpru
-Version: 0.0.1
+Version: 0.0.2
 Summary: Unofficial Python client library for the OpenAI and Azure OpenAI APIs
 Project-URL: Documentation, https://github.com/sincekmori/gpru#readme
 Project-URL: Issues, https://github.com/sincekmori/gpru/issues
 Project-URL: Source, https://github.com/sincekmori/gpru
 Author-email: Shinsuke Mori <sincekmori@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -77,16 +77,16 @@
 Here is an example of [chat completion](https://platform.openai.com/docs/api-reference/chat/create), also known as [ChatGPT](https://chat.openai.com/).
 
 ```python
 import os
 
 from gpru.openai.api import ChatCompletionRequest, OpenAiApi, UserMessage
 
-api_key = os.environ["OPENAI_API_KEY"]
-api = OpenAiApi(api_key)
+key = os.environ["OPENAI_API_KEY"]
+api = OpenAiApi(key)
 
 req = ChatCompletionRequest(model="gpt-3.5-turbo", messages=[UserMessage("Hello!")])
 chat_completion = api.create_chat_completion(req)
 print(chat_completion.content)
 # Greetings! How can I assist you today?
 ```
 
@@ -108,16 +108,16 @@
 from gpru.azure.stable_2023_05_15 import (
     AzureOpenAiApi,
     ChatCompletionRequest,
     UserMessage,
 )
 
 endpoint = os.environ["AZURE_OPENAI_API_ENDPOINT"]
-api_key = os.environ["AZURE_OPENAI_API_KEY"]
+key = os.environ["AZURE_OPENAI_API_KEY"]
 deployment_id = os.environ["AZURE_OPENAI_API_DEPLOYMENT_ID"]
-api = AzureOpenAiApi(endpoint, api_key)
+api = AzureOpenAiApi(endpoint, key)
 
 req = ChatCompletionRequest(messages=[UserMessage("Hello!")])
 chat_completion = api.create_chat_completion(deployment_id, req)
 print(chat_completion.content)
 # Greetings! How can I assist you today?
 ```
```

