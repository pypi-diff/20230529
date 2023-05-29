# Comparing `tmp/human-protocol-sdk-1.1.1.tar.gz` & `tmp/human-protocol-sdk-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "human-protocol-sdk-1.1.1.tar", last modified: Mon Feb 27 18:02:06 2023, max compression
+gzip compressed data, was "human-protocol-sdk-1.1.2.tar", last modified: Wed Mar  1 13:18:18 2023, max compression
```

## Comparing `human-protocol-sdk-1.1.1.tar` & `human-protocol-sdk-1.1.2.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.105962 human-protocol-sdk-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-02-27 18:02:06.105962 human-protocol-sdk-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.093962 human-protocol-sdk-1.1.1/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.093962 human-protocol-sdk-1.1.1/contracts/Escrow.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/Escrow.sol/Escrow.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)    60521 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/Escrow.sol/Escrow.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.093962 human-protocol-sdk-1.1.1/contracts/EscrowFactory.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/EscrowFactory.sol/EscrowFactory.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)    86718 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/EscrowFactory.sol/EscrowFactory.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.093962 human-protocol-sdk-1.1.1/contracts/HMToken.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/HMToken.sol/HMToken.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)    37832 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/HMToken.sol/HMToken.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.097962 human-protocol-sdk-1.1.1/contracts/KVStore.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/KVStore.sol/KVStore.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/KVStore.sol/KVStore.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.097962 human-protocol-sdk-1.1.1/contracts/Reputation.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/Reputation.sol/Reputation.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)    48010 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/Reputation.sol/Reputation.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.097962 human-protocol-sdk-1.1.1/contracts/RewardPool.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/RewardPool.sol/RewardPool.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)    39274 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/RewardPool.sol/RewardPool.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.097962 human-protocol-sdk-1.1.1/contracts/Staking.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/Staking.sol/Staking.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)    84832 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/Staking.sol/Staking.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.093962 human-protocol-sdk-1.1.1/contracts/interfaces/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.097962 human-protocol-sdk-1.1.1/contracts/interfaces/HMTokenInterface.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/interfaces/HMTokenInterface.sol/HMTokenInterface.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/interfaces/HMTokenInterface.sol/HMTokenInterface.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.097962 human-protocol-sdk-1.1.1/contracts/interfaces/IEscrow.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/interfaces/IEscrow.sol/IEscrow.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/interfaces/IEscrow.sol/IEscrow.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.097962 human-protocol-sdk-1.1.1/contracts/interfaces/IRewardPool.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/interfaces/IRewardPool.sol/IRewardPool.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/interfaces/IRewardPool.sol/IRewardPool.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.097962 human-protocol-sdk-1.1.1/contracts/interfaces/IStaking.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/interfaces/IStaking.sol/IStaking.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/interfaces/IStaking.sol/IStaking.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.093962 human-protocol-sdk-1.1.1/contracts/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.097962 human-protocol-sdk-1.1.1/contracts/libs/Stakes.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/libs/Stakes.sol/Stakes.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/libs/Stakes.sol/Stakes.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.093962 human-protocol-sdk-1.1.1/contracts/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.097962 human-protocol-sdk-1.1.1/contracts/test/EscrowFactoryV0.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/test/EscrowFactoryV0.sol/EscrowFactoryV0.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)    85229 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/test/EscrowFactoryV0.sol/EscrowFactoryV0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.097962 human-protocol-sdk-1.1.1/contracts/test/ReputationV0.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/test/ReputationV0.sol/ReputationV0.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)    40772 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/test/ReputationV0.sol/ReputationV0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.093962 human-protocol-sdk-1.1.1/contracts/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.097962 human-protocol-sdk-1.1.1/contracts/utils/Math.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/utils/Math.sol/Math.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/utils/Math.sol/Math.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.097962 human-protocol-sdk-1.1.1/contracts/utils/SafeMath.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/utils/SafeMath.sol/SafeMath.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/utils/SafeMath.sol/SafeMath.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.097962 human-protocol-sdk-1.1.1/contracts/utils/SignedSafeMath.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/utils/SignedSafeMath.sol/SignedSafeMath.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-02-27 18:02:04.000000 human-protocol-sdk-1.1.1/contracts/utils/SignedSafeMath.sol/SignedSafeMath.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.097962 human-protocol-sdk-1.1.1/human_protocol_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-27 18:01:54.000000 human-protocol-sdk-1.1.1/human_protocol_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.101962 human-protocol-sdk-1.1.1/human_protocol_sdk/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/human_protocol_sdk/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/human_protocol_sdk/crypto/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/human_protocol_sdk/crypto/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/human_protocol_sdk/eth_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)    76445 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/human_protocol_sdk/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/human_protocol_sdk/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/human_protocol_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.101962 human-protocol-sdk-1.1.1/human_protocol_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-02-27 18:02:06.000000 human-protocol-sdk-1.1.1/human_protocol_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-02-27 18:02:06.000000 human-protocol-sdk-1.1.1/human_protocol_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 18:02:06.000000 human-protocol-sdk-1.1.1/human_protocol_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-27 18:02:06.000000 human-protocol-sdk-1.1.1/human_protocol_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-27 18:02:06.000000 human-protocol-sdk-1.1.1/human_protocol_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 18:02:06.000000 human-protocol-sdk-1.1.1/human_protocol_sdk.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 18:02:06.105962 human-protocol-sdk-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.101962 human-protocol-sdk-1.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.101962 human-protocol-sdk-1.1.1/test/human_protocol_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/test/human_protocol_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.101962 human-protocol-sdk-1.1.1/test/human_protocol_sdk/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/test/human_protocol_sdk/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/test/human_protocol_sdk/crypto/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/test/human_protocol_sdk/crypto/test_encryption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.101962 human-protocol-sdk-1.1.1/test/human_protocol_sdk/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/test/human_protocol_sdk/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/test/human_protocol_sdk/storage/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/test/human_protocol_sdk/storage/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/test/human_protocol_sdk/test_eth_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)    24079 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/test/human_protocol_sdk/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/test/human_protocol_sdk/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 18:02:06.101962 human-protocol-sdk-1.1.1/test/human_protocol_sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/test/human_protocol_sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/test/human_protocol_sdk/utils/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-02-27 17:59:37.000000 human-protocol-sdk-1.1.1/test/human_protocol_sdk/utils/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.803586 human-protocol-sdk-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-01 13:18:18.803586 human-protocol-sdk-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.783586 human-protocol-sdk-1.1.2/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.787586 human-protocol-sdk-1.1.2/contracts/Escrow.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/Escrow.sol/Escrow.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)    60521 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/Escrow.sol/Escrow.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.787586 human-protocol-sdk-1.1.2/contracts/EscrowFactory.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/EscrowFactory.sol/EscrowFactory.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)    86718 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/EscrowFactory.sol/EscrowFactory.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.787586 human-protocol-sdk-1.1.2/contracts/HMToken.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/HMToken.sol/HMToken.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37832 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/HMToken.sol/HMToken.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.787586 human-protocol-sdk-1.1.2/contracts/KVStore.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/KVStore.sol/KVStore.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/KVStore.sol/KVStore.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.787586 human-protocol-sdk-1.1.2/contracts/Reputation.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/Reputation.sol/Reputation.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48010 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/Reputation.sol/Reputation.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.787586 human-protocol-sdk-1.1.2/contracts/RewardPool.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/RewardPool.sol/RewardPool.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39274 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/RewardPool.sol/RewardPool.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.791586 human-protocol-sdk-1.1.2/contracts/Staking.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/Staking.sol/Staking.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)    84832 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/Staking.sol/Staking.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.779586 human-protocol-sdk-1.1.2/contracts/interfaces/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.791586 human-protocol-sdk-1.1.2/contracts/interfaces/HMTokenInterface.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/interfaces/HMTokenInterface.sol/HMTokenInterface.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/interfaces/HMTokenInterface.sol/HMTokenInterface.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.791586 human-protocol-sdk-1.1.2/contracts/interfaces/IEscrow.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/interfaces/IEscrow.sol/IEscrow.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/interfaces/IEscrow.sol/IEscrow.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.791586 human-protocol-sdk-1.1.2/contracts/interfaces/IRewardPool.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/interfaces/IRewardPool.sol/IRewardPool.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/interfaces/IRewardPool.sol/IRewardPool.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.791586 human-protocol-sdk-1.1.2/contracts/interfaces/IStaking.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/interfaces/IStaking.sol/IStaking.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/interfaces/IStaking.sol/IStaking.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.783586 human-protocol-sdk-1.1.2/contracts/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.791586 human-protocol-sdk-1.1.2/contracts/libs/Stakes.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/libs/Stakes.sol/Stakes.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/libs/Stakes.sol/Stakes.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.783586 human-protocol-sdk-1.1.2/contracts/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.791586 human-protocol-sdk-1.1.2/contracts/test/EscrowFactoryV0.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/test/EscrowFactoryV0.sol/EscrowFactoryV0.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)    85229 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/test/EscrowFactoryV0.sol/EscrowFactoryV0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.791586 human-protocol-sdk-1.1.2/contracts/test/ReputationV0.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/test/ReputationV0.sol/ReputationV0.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40772 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/test/ReputationV0.sol/ReputationV0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.783586 human-protocol-sdk-1.1.2/contracts/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.791586 human-protocol-sdk-1.1.2/contracts/utils/Math.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/utils/Math.sol/Math.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/utils/Math.sol/Math.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.791586 human-protocol-sdk-1.1.2/contracts/utils/SafeMath.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/utils/SafeMath.sol/SafeMath.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/utils/SafeMath.sol/SafeMath.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.791586 human-protocol-sdk-1.1.2/contracts/utils/SignedSafeMath.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/utils/SignedSafeMath.sol/SignedSafeMath.dbg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/utils/SignedSafeMath.sol/SignedSafeMath.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.795586 human-protocol-sdk-1.1.2/human_protocol_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-01 13:18:04.000000 human-protocol-sdk-1.1.2/human_protocol_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.799586 human-protocol-sdk-1.1.2/human_protocol_sdk/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/human_protocol_sdk/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/human_protocol_sdk/crypto/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/human_protocol_sdk/crypto/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/human_protocol_sdk/eth_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76490 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/human_protocol_sdk/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/human_protocol_sdk/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/human_protocol_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.799586 human-protocol-sdk-1.1.2/human_protocol_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-01 13:18:18.000000 human-protocol-sdk-1.1.2/human_protocol_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-03-01 13:18:18.000000 human-protocol-sdk-1.1.2/human_protocol_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 13:18:18.000000 human-protocol-sdk-1.1.2/human_protocol_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-01 13:18:18.000000 human-protocol-sdk-1.1.2/human_protocol_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-01 13:18:18.000000 human-protocol-sdk-1.1.2/human_protocol_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 13:18:18.000000 human-protocol-sdk-1.1.2/human_protocol_sdk.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 13:18:18.803586 human-protocol-sdk-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.799586 human-protocol-sdk-1.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.799586 human-protocol-sdk-1.1.2/test/human_protocol_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.799586 human-protocol-sdk-1.1.2/test/human_protocol_sdk/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/crypto/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/crypto/test_encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.803586 human-protocol-sdk-1.1.2/test/human_protocol_sdk/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/storage/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/storage/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/test_eth_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24079 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.803586 human-protocol-sdk-1.1.2/test/human_protocol_sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/utils/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/utils/manifest.py
```

### Comparing `human-protocol-sdk-1.1.1/LICENSE` & `human-protocol-sdk-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/README.md` & `human-protocol-sdk-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/contracts/Escrow.sol/Escrow.json` & `human-protocol-sdk-1.1.2/contracts/Escrow.sol/Escrow.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/contracts/EscrowFactory.sol/EscrowFactory.json` & `human-protocol-sdk-1.1.2/contracts/EscrowFactory.sol/EscrowFactory.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/contracts/HMToken.sol/HMToken.json` & `human-protocol-sdk-1.1.2/contracts/HMToken.sol/HMToken.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/contracts/KVStore.sol/KVStore.json` & `human-protocol-sdk-1.1.2/contracts/KVStore.sol/KVStore.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/contracts/Reputation.sol/Reputation.json` & `human-protocol-sdk-1.1.2/contracts/Reputation.sol/Reputation.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/contracts/RewardPool.sol/RewardPool.json` & `human-protocol-sdk-1.1.2/contracts/RewardPool.sol/RewardPool.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/contracts/Staking.sol/Staking.json` & `human-protocol-sdk-1.1.2/contracts/Staking.sol/Staking.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/contracts/interfaces/HMTokenInterface.sol/HMTokenInterface.json` & `human-protocol-sdk-1.1.2/contracts/interfaces/HMTokenInterface.sol/HMTokenInterface.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/contracts/interfaces/IEscrow.sol/IEscrow.json` & `human-protocol-sdk-1.1.2/contracts/interfaces/IEscrow.sol/IEscrow.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/contracts/interfaces/IRewardPool.sol/IRewardPool.json` & `human-protocol-sdk-1.1.2/contracts/interfaces/IRewardPool.sol/IRewardPool.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/contracts/interfaces/IStaking.sol/IStaking.json` & `human-protocol-sdk-1.1.2/contracts/interfaces/IStaking.sol/IStaking.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/contracts/libs/Stakes.sol/Stakes.json` & `human-protocol-sdk-1.1.2/contracts/libs/Stakes.sol/Stakes.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/contracts/test/EscrowFactoryV0.sol/EscrowFactoryV0.json` & `human-protocol-sdk-1.1.2/contracts/test/EscrowFactoryV0.sol/EscrowFactoryV0.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/contracts/test/ReputationV0.sol/ReputationV0.json` & `human-protocol-sdk-1.1.2/contracts/test/ReputationV0.sol/ReputationV0.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/contracts/utils/Math.sol/Math.json` & `human-protocol-sdk-1.1.2/contracts/utils/Math.sol/Math.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/contracts/utils/SafeMath.sol/SafeMath.json` & `human-protocol-sdk-1.1.2/contracts/utils/SafeMath.sol/SafeMath.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/contracts/utils/SignedSafeMath.sol/SignedSafeMath.json` & `human-protocol-sdk-1.1.2/contracts/utils/SignedSafeMath.sol/SignedSafeMath.json`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/human_protocol_sdk/crypto/__init__.py` & `human-protocol-sdk-1.1.2/human_protocol_sdk/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/human_protocol_sdk/crypto/encryption.py` & `human-protocol-sdk-1.1.2/human_protocol_sdk/crypto/encryption.py`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/human_protocol_sdk/eth_bridge.py` & `human-protocol-sdk-1.1.2/human_protocol_sdk/eth_bridge.py`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/human_protocol_sdk/job.py` & `human-protocol-sdk-1.1.2/human_protocol_sdk/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 #!/usr/bin/env python3
 import logging
 import os
 from decimal import Decimal
 from enum import Enum
-from typing import Dict, List, Tuple, Optional, Any, TypedDict
+from typing import (
+    Dict,
+    List,
+    Tuple,
+    Optional,
+    Any,
+    TypedDict,
+    Union
+)
 
 from basemodels import Manifest
 from eth_keys import keys
 from eth_utils import decode_hex
 from web3 import Web3
 from web3.contract import Contract
 from web3.types import TxReceipt, Wei
@@ -1932,15 +1940,15 @@
 
         for log in tx_receipt.get("logs", {}):
             for topic in log["topics"]:
                 if TRANSFER_EVENT == topic:
                     return True
         return False
 
-    def _find_operator(self, addr: Optional[str]) -> Tuple[str, str] | None:
+    def _find_operator(self, addr: Optional[str]) -> Union[Tuple[str, str], None]:
         """
         Find the operator to execute the transaction from trusted wallets.
 
         Args:
             addr (Optional[str]): Operator address to find.
 
         Returns:
```

### Comparing `human-protocol-sdk-1.1.1/human_protocol_sdk/storage.py` & `human-protocol-sdk-1.1.2/human_protocol_sdk/storage.py`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/human_protocol_sdk/utils.py` & `human-protocol-sdk-1.1.2/human_protocol_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/human_protocol_sdk.egg-info/SOURCES.txt` & `human-protocol-sdk-1.1.2/human_protocol_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/setup.py` & `human-protocol-sdk-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/test/human_protocol_sdk/crypto/test_crypto.py` & `human-protocol-sdk-1.1.2/test/human_protocol_sdk/crypto/test_crypto.py`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/test/human_protocol_sdk/crypto/test_encryption.py` & `human-protocol-sdk-1.1.2/test/human_protocol_sdk/crypto/test_encryption.py`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/test/human_protocol_sdk/storage/test_bucket.py` & `human-protocol-sdk-1.1.2/test/human_protocol_sdk/storage/test_bucket.py`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/test/human_protocol_sdk/storage/test_storage.py` & `human-protocol-sdk-1.1.2/test/human_protocol_sdk/storage/test_storage.py`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/test/human_protocol_sdk/test_eth_bridge.py` & `human-protocol-sdk-1.1.2/test/human_protocol_sdk/test_eth_bridge.py`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/test/human_protocol_sdk/test_job.py` & `human-protocol-sdk-1.1.2/test/human_protocol_sdk/test_job.py`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/test/human_protocol_sdk/test_utils.py` & `human-protocol-sdk-1.1.2/test/human_protocol_sdk/test_utils.py`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/test/human_protocol_sdk/utils/job.py` & `human-protocol-sdk-1.1.2/test/human_protocol_sdk/utils/job.py`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.1/test/human_protocol_sdk/utils/manifest.py` & `human-protocol-sdk-1.1.2/test/human_protocol_sdk/utils/manifest.py`

 * *Files identical despite different names*

