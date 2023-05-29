# Comparing `tmp/bubble-aide-0.1.0.tar.gz` & `tmp/bubble-aide-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bubble-aide-0.1.0.tar", last modified: Mon May 29 01:44:09 2023, max compression
+gzip compressed data, was "bubble-aide-0.1.1.tar", last modified: Mon May 29 01:45:26 2023, max compression
```

## Comparing `bubble-aide-0.1.0.tar` & `bubble-aide-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 01:44:09.196594 bubble-aide-0.1.0/
--rw-rw-rw-   0        0        0     1083 2023-05-24 02:42:32.000000 bubble-aide-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      707 2023-05-29 01:44:09.195595 bubble-aide-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2061 2023-05-29 01:43:41.000000 bubble-aide-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 01:44:09.179815 bubble-aide-0.1.0/bubble_aide/
--rw-rw-rw-   0        0        0       66 2023-05-25 01:55:47.000000 bubble-aide-0.1.0/bubble_aide/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 01:44:09.191589 bubble-aide-0.1.0/bubble_aide/abc/
--rw-rw-rw-   0        0        0       55 2023-05-26 09:57:09.000000 bubble-aide-0.1.0/bubble_aide/abc/__init__.py
--rw-rw-rw-   0        0        0      191 2023-05-26 09:38:15.000000 bubble-aide-0.1.0/bubble_aide/abc/module.py
--rw-rw-rw-   0        0        0     4879 2023-05-26 09:35:12.000000 bubble-aide-0.1.0/bubble_aide/delegate.py
--rw-rw-rw-   0        0        0    10020 2023-05-26 09:35:12.000000 bubble-aide-0.1.0/bubble_aide/govern.py
--rw-rw-rw-   0        0        0    10036 2023-05-26 10:28:31.000000 bubble-aide-0.1.0/bubble_aide/main.py
--rw-rw-rw-   0        0        0      794 2023-05-26 09:35:12.000000 bubble-aide-0.1.0/bubble_aide/restricting.py
--rw-rw-rw-   0        0        0     1720 2023-05-26 09:35:12.000000 bubble-aide-0.1.0/bubble_aide/reward.py
--rw-rw-rw-   0        0        0     1112 2023-05-26 09:35:12.000000 bubble-aide-0.1.0/bubble_aide/slashing.py
--rw-rw-rw-   0        0        0     5769 2023-05-26 09:35:12.000000 bubble-aide-0.1.0/bubble_aide/staking.py
-drwxrwxrwx   0        0        0        0 2023-05-29 01:44:09.194594 bubble-aide-0.1.0/bubble_aide/statics/
--rw-rw-rw-   0        0        0        0 2023-05-26 06:36:53.000000 bubble-aide-0.1.0/bubble_aide/statics/__init__.py
--rw-rw-rw-   0        0        0    12509 2023-05-26 09:04:44.000000 bubble-aide-0.1.0/bubble_aide/statics/calculator.py
--rw-rw-rw-   0        0        0     3393 2023-05-26 09:37:06.000000 bubble-aide-0.1.0/bubble_aide/statics/contract.py
--rw-rw-rw-   0        0        0     5783 2023-05-25 09:07:03.000000 bubble-aide-0.1.0/bubble_aide/statics/economic.py
--rw-rw-rw-   0        0        0      312 2023-05-26 07:31:21.000000 bubble-aide-0.1.0/bubble_aide/statics/graphqls.py
--rw-rw-rw-   0        0        0      911 2023-05-26 09:05:19.000000 bubble-aide-0.1.0/bubble_aide/statics/node.py
-drwxrwxrwx   0        0        0        0 2023-05-29 01:44:09.195595 bubble-aide-0.1.0/bubble_aide/utils/
--rw-rw-rw-   0        0        0        0 2023-05-26 07:29:33.000000 bubble-aide-0.1.0/bubble_aide/utils/__init__.py
--rw-rw-rw-   0        0        0     3326 2023-05-26 10:03:16.000000 bubble-aide-0.1.0/bubble_aide/utils/utils.py
--rw-rw-rw-   0        0        0      986 2023-05-26 09:37:35.000000 bubble-aide-0.1.0/bubble_aide/utils/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-05-29 01:44:09.191589 bubble-aide-0.1.0/bubble_aide.egg-info/
--rw-rw-rw-   0        0        0      707 2023-05-29 01:44:09.000000 bubble-aide-0.1.0/bubble_aide.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      750 2023-05-29 01:44:09.000000 bubble-aide-0.1.0/bubble_aide.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 01:44:09.000000 bubble-aide-0.1.0/bubble_aide.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-29 01:43:56.000000 bubble-aide-0.1.0/bubble_aide.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      161 2023-05-29 01:44:09.000000 bubble-aide-0.1.0/bubble_aide.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-29 01:44:09.000000 bubble-aide-0.1.0/bubble_aide.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 01:44:09.196594 bubble-aide-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1591 2023-05-29 01:44:05.000000 bubble-aide-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 01:45:26.739841 bubble-aide-0.1.1/
+-rw-rw-rw-   0        0        0     1083 2023-05-24 02:42:32.000000 bubble-aide-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      707 2023-05-29 01:45:26.739004 bubble-aide-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2419 2023-05-29 01:45:12.000000 bubble-aide-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 01:45:26.722418 bubble-aide-0.1.1/bubble_aide/
+-rw-rw-rw-   0        0        0       66 2023-05-25 01:55:47.000000 bubble-aide-0.1.1/bubble_aide/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 01:45:26.734998 bubble-aide-0.1.1/bubble_aide/abc/
+-rw-rw-rw-   0        0        0       55 2023-05-26 09:57:09.000000 bubble-aide-0.1.1/bubble_aide/abc/__init__.py
+-rw-rw-rw-   0        0        0      191 2023-05-26 09:38:15.000000 bubble-aide-0.1.1/bubble_aide/abc/module.py
+-rw-rw-rw-   0        0        0     4879 2023-05-26 09:35:12.000000 bubble-aide-0.1.1/bubble_aide/delegate.py
+-rw-rw-rw-   0        0        0    10020 2023-05-26 09:35:12.000000 bubble-aide-0.1.1/bubble_aide/govern.py
+-rw-rw-rw-   0        0        0    10036 2023-05-26 10:28:31.000000 bubble-aide-0.1.1/bubble_aide/main.py
+-rw-rw-rw-   0        0        0      794 2023-05-26 09:35:12.000000 bubble-aide-0.1.1/bubble_aide/restricting.py
+-rw-rw-rw-   0        0        0     1720 2023-05-26 09:35:12.000000 bubble-aide-0.1.1/bubble_aide/reward.py
+-rw-rw-rw-   0        0        0     1112 2023-05-26 09:35:12.000000 bubble-aide-0.1.1/bubble_aide/slashing.py
+-rw-rw-rw-   0        0        0     5769 2023-05-26 09:35:12.000000 bubble-aide-0.1.1/bubble_aide/staking.py
+drwxrwxrwx   0        0        0        0 2023-05-29 01:45:26.738006 bubble-aide-0.1.1/bubble_aide/statics/
+-rw-rw-rw-   0        0        0        0 2023-05-26 06:36:53.000000 bubble-aide-0.1.1/bubble_aide/statics/__init__.py
+-rw-rw-rw-   0        0        0    12509 2023-05-26 09:04:44.000000 bubble-aide-0.1.1/bubble_aide/statics/calculator.py
+-rw-rw-rw-   0        0        0     3393 2023-05-26 09:37:06.000000 bubble-aide-0.1.1/bubble_aide/statics/contract.py
+-rw-rw-rw-   0        0        0     5783 2023-05-25 09:07:03.000000 bubble-aide-0.1.1/bubble_aide/statics/economic.py
+-rw-rw-rw-   0        0        0      312 2023-05-26 07:31:21.000000 bubble-aide-0.1.1/bubble_aide/statics/graphqls.py
+-rw-rw-rw-   0        0        0      911 2023-05-26 09:05:19.000000 bubble-aide-0.1.1/bubble_aide/statics/node.py
+drwxrwxrwx   0        0        0        0 2023-05-29 01:45:26.739004 bubble-aide-0.1.1/bubble_aide/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-26 07:29:33.000000 bubble-aide-0.1.1/bubble_aide/utils/__init__.py
+-rw-rw-rw-   0        0        0     3326 2023-05-26 10:03:16.000000 bubble-aide-0.1.1/bubble_aide/utils/utils.py
+-rw-rw-rw-   0        0        0      986 2023-05-26 09:37:35.000000 bubble-aide-0.1.1/bubble_aide/utils/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-05-29 01:45:26.734998 bubble-aide-0.1.1/bubble_aide.egg-info/
+-rw-rw-rw-   0        0        0      707 2023-05-29 01:45:26.000000 bubble-aide-0.1.1/bubble_aide.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      750 2023-05-29 01:45:26.000000 bubble-aide-0.1.1/bubble_aide.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 01:45:26.000000 bubble-aide-0.1.1/bubble_aide.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-29 01:43:56.000000 bubble-aide-0.1.1/bubble_aide.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      161 2023-05-29 01:45:26.000000 bubble-aide-0.1.1/bubble_aide.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-29 01:45:26.000000 bubble-aide-0.1.1/bubble_aide.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 01:45:26.739841 bubble-aide-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1591 2023-05-29 01:45:23.000000 bubble-aide-0.1.1/setup.py
```

### Comparing `bubble-aide-0.1.0/LICENSE` & `bubble-aide-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.0/PKG-INFO` & `bubble-aide-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bubble-aide
-Version: 0.1.0
+Version: 0.1.1
 Summary: bubble aide
 Home-page: https://github.com/shinnng/bubble-aide
 Author: Shing
 Author-email: shinnng@outlook.com
 License: MIT
 Keywords: bubble-aide
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bubble-aide-0.1.0/README.md` & `bubble-aide-0.1.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,57 @@
 # bubble-aide
 Bubble区块链助手，能够帮助您便捷、快速的接入Bubble区块链。 
 
 
-# 安装方法
+##  安装方法
+
 ```shell
 pip install bubble_aide
 ```
 
 
-# 使用方法
+## 使用方法
 
 ```python
 from eth_account import Account
 from bubble_aide import Aide
 
+# 实例化aide
 uri = 'http://192.168.120.121:6789'
 account = Account.from_key('f51ca759562e1daf9e5302d121f933a8152915d34fcbc27e542baf256b5e4b74')
-aide = Aide(uri, account=account)
-print(aide.bub.block_number)
+aide = Aide(uri, account=account)  # account指定用于默认发交易的账户
+print(aide.bub.block_number)    # 打印当前块高
 
+# 发送转账交易
 aide.transfer('0xc1E8e709620Cb29c33B9669C60c0600a9014c881', amount=aide.web3.to_wei(10))
 
+# 调用锁仓合约，锁定金额到目标账户
 plans = [{'Epoch': 2, 'Amount': 100 * 10 ** 18}, {'Epoch': 8, 'Amount': 300 * 10 ** 18}]
 aide.restricting.restricting('0xc1E8e709620Cb29c33B9669C60c0600a9014c881', plans)
 
+# 调用质押委托合约，查看账户处于锁定期的委托信息
 print(aide.delegate.get_delegate_lock_info())
 
+# 部署solidity合约
 false = False
 ture = True
 abi = [{"anonymous": false, "inputs": [{"indexed": false, "internalType": "uint256", "name": "_chainId", "type": "uint256"}], "name": "_putChainID",
         "type": "event"},
        {"inputs": [], "name": "getChainID", "outputs": [{"internalType": "uint256", "name": "", "type": "uint256"}], "stateMutability": "view",
         "type": "function"},
        {"inputs": [], "name": "putChainID", "outputs": [], "stateMutability": "nonpayable", "type": "function"}]
 bytecode = '608060405234801561001057600080fd5b50610107806100206000396000f3fe6080604052348015600f57600080fd5b506004361060325760003560e01c806336319ab0146037578063564b81ef14603f575b600080fd5b603d6059565b005b60456099565b6040516050919060ae565b60405180910390f35b466000819055507f68e891aec7f9596d6e192c48cb82364ec392d423bce80abd6e1ee5ad05860256600054604051608f919060ae565b60405180910390a1565b600046905090565b60a88160c7565b82525050565b600060208201905060c1600083018460a1565b92915050565b600081905091905056fea264697066735822122037a1668252253271128182c71109922cb1e300fb08a7080a0587f360df4071ba64736f6c63430008060033'
 contract = aide.deploy_contract(abi=abi, bytecode=bytecode)
 print(contract.address)
 
+# 调用solidity合约方法
 print(contract.getChainID())
+
+# 发送solidity合约交易
 res = contract.putChainID(1000)
+
+# 解析solidity事件
 print(contract.PutChainID(res))
+
 ```
+
+
```

### Comparing `bubble-aide-0.1.0/bubble_aide/delegate.py` & `bubble-aide-0.1.1/bubble_aide/delegate.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.0/bubble_aide/govern.py` & `bubble-aide-0.1.1/bubble_aide/govern.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.0/bubble_aide/main.py` & `bubble-aide-0.1.1/bubble_aide/main.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.0/bubble_aide/restricting.py` & `bubble-aide-0.1.1/bubble_aide/restricting.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.0/bubble_aide/reward.py` & `bubble-aide-0.1.1/bubble_aide/reward.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.0/bubble_aide/slashing.py` & `bubble-aide-0.1.1/bubble_aide/slashing.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.0/bubble_aide/staking.py` & `bubble-aide-0.1.1/bubble_aide/staking.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.0/bubble_aide/statics/calculator.py` & `bubble-aide-0.1.1/bubble_aide/statics/calculator.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.0/bubble_aide/statics/contract.py` & `bubble-aide-0.1.1/bubble_aide/statics/contract.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.0/bubble_aide/statics/economic.py` & `bubble-aide-0.1.1/bubble_aide/statics/economic.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.0/bubble_aide/statics/node.py` & `bubble-aide-0.1.1/bubble_aide/statics/node.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.0/bubble_aide/utils/utils.py` & `bubble-aide-0.1.1/bubble_aide/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.0/bubble_aide/utils/wrapper.py` & `bubble-aide-0.1.1/bubble_aide/utils/wrapper.py`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.0/bubble_aide.egg-info/PKG-INFO` & `bubble-aide-0.1.1/bubble_aide.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bubble-aide
-Version: 0.1.0
+Version: 0.1.1
 Summary: bubble aide
 Home-page: https://github.com/shinnng/bubble-aide
 Author: Shing
 Author-email: shinnng@outlook.com
 License: MIT
 Keywords: bubble-aide
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bubble-aide-0.1.0/bubble_aide.egg-info/SOURCES.txt` & `bubble-aide-0.1.1/bubble_aide.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bubble-aide-0.1.0/setup.py` & `bubble-aide-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 with open('./README.md', encoding='utf-8') as readme:
     long_description = readme.read()
 
 setup(
     name='bubble-aide',
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version='0.1.0',
+    version='0.1.1',
     description="""bubble aide""",
     # long_description=long_description,
     # long_description_content_type='text/markdown',
     author='Shing',
     author_email='shinnng@outlook.com',
     url='https://github.com/shinnng/bubble-aide',
     include_package_data=True,
```

