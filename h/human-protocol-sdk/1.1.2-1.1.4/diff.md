# Comparing `tmp/human-protocol-sdk-1.1.2.tar.gz` & `tmp/human-protocol-sdk-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "human-protocol-sdk-1.1.2.tar", last modified: Wed Mar  1 13:18:18 2023, max compression
+gzip compressed data, was "human-protocol-sdk-1.1.4.tar", last modified: Mon May 29 17:13:40 2023, max compression
```

## Comparing `human-protocol-sdk-1.1.2.tar` & `human-protocol-sdk-1.1.4.tar`

### file list

```diff
@@ -1,100 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.803586 human-protocol-sdk-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-01 13:18:18.803586 human-protocol-sdk-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.783586 human-protocol-sdk-1.1.2/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.787586 human-protocol-sdk-1.1.2/contracts/Escrow.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/Escrow.sol/Escrow.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)    60521 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/Escrow.sol/Escrow.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.787586 human-protocol-sdk-1.1.2/contracts/EscrowFactory.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/EscrowFactory.sol/EscrowFactory.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)    86718 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/EscrowFactory.sol/EscrowFactory.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.787586 human-protocol-sdk-1.1.2/contracts/HMToken.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/HMToken.sol/HMToken.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)    37832 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/HMToken.sol/HMToken.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.787586 human-protocol-sdk-1.1.2/contracts/KVStore.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/KVStore.sol/KVStore.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/KVStore.sol/KVStore.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.787586 human-protocol-sdk-1.1.2/contracts/Reputation.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/Reputation.sol/Reputation.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)    48010 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/Reputation.sol/Reputation.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.787586 human-protocol-sdk-1.1.2/contracts/RewardPool.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/RewardPool.sol/RewardPool.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)    39274 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/RewardPool.sol/RewardPool.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.791586 human-protocol-sdk-1.1.2/contracts/Staking.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/Staking.sol/Staking.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)    84832 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/Staking.sol/Staking.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.779586 human-protocol-sdk-1.1.2/contracts/interfaces/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.791586 human-protocol-sdk-1.1.2/contracts/interfaces/HMTokenInterface.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/interfaces/HMTokenInterface.sol/HMTokenInterface.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/interfaces/HMTokenInterface.sol/HMTokenInterface.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.791586 human-protocol-sdk-1.1.2/contracts/interfaces/IEscrow.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/interfaces/IEscrow.sol/IEscrow.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/interfaces/IEscrow.sol/IEscrow.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.791586 human-protocol-sdk-1.1.2/contracts/interfaces/IRewardPool.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/interfaces/IRewardPool.sol/IRewardPool.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/interfaces/IRewardPool.sol/IRewardPool.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.791586 human-protocol-sdk-1.1.2/contracts/interfaces/IStaking.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/interfaces/IStaking.sol/IStaking.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/interfaces/IStaking.sol/IStaking.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.783586 human-protocol-sdk-1.1.2/contracts/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.791586 human-protocol-sdk-1.1.2/contracts/libs/Stakes.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/libs/Stakes.sol/Stakes.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/libs/Stakes.sol/Stakes.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.783586 human-protocol-sdk-1.1.2/contracts/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.791586 human-protocol-sdk-1.1.2/contracts/test/EscrowFactoryV0.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/test/EscrowFactoryV0.sol/EscrowFactoryV0.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)    85229 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/test/EscrowFactoryV0.sol/EscrowFactoryV0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.791586 human-protocol-sdk-1.1.2/contracts/test/ReputationV0.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/test/ReputationV0.sol/ReputationV0.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)    40772 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/test/ReputationV0.sol/ReputationV0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.783586 human-protocol-sdk-1.1.2/contracts/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.791586 human-protocol-sdk-1.1.2/contracts/utils/Math.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/utils/Math.sol/Math.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/utils/Math.sol/Math.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.791586 human-protocol-sdk-1.1.2/contracts/utils/SafeMath.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/utils/SafeMath.sol/SafeMath.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/utils/SafeMath.sol/SafeMath.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.791586 human-protocol-sdk-1.1.2/contracts/utils/SignedSafeMath.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/utils/SignedSafeMath.sol/SignedSafeMath.dbg.json
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-01 13:18:17.000000 human-protocol-sdk-1.1.2/contracts/utils/SignedSafeMath.sol/SignedSafeMath.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.795586 human-protocol-sdk-1.1.2/human_protocol_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-01 13:18:04.000000 human-protocol-sdk-1.1.2/human_protocol_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.799586 human-protocol-sdk-1.1.2/human_protocol_sdk/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/human_protocol_sdk/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/human_protocol_sdk/crypto/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/human_protocol_sdk/crypto/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/human_protocol_sdk/eth_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)    76490 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/human_protocol_sdk/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/human_protocol_sdk/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/human_protocol_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.799586 human-protocol-sdk-1.1.2/human_protocol_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-01 13:18:18.000000 human-protocol-sdk-1.1.2/human_protocol_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-03-01 13:18:18.000000 human-protocol-sdk-1.1.2/human_protocol_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 13:18:18.000000 human-protocol-sdk-1.1.2/human_protocol_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-01 13:18:18.000000 human-protocol-sdk-1.1.2/human_protocol_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-01 13:18:18.000000 human-protocol-sdk-1.1.2/human_protocol_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 13:18:18.000000 human-protocol-sdk-1.1.2/human_protocol_sdk.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 13:18:18.803586 human-protocol-sdk-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.799586 human-protocol-sdk-1.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.799586 human-protocol-sdk-1.1.2/test/human_protocol_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.799586 human-protocol-sdk-1.1.2/test/human_protocol_sdk/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/crypto/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/crypto/test_encryption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.803586 human-protocol-sdk-1.1.2/test/human_protocol_sdk/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/storage/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/storage/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/test_eth_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)    24079 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 13:18:18.803586 human-protocol-sdk-1.1.2/test/human_protocol_sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/utils/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-03-01 13:15:23.000000 human-protocol-sdk-1.1.2/test/human_protocol_sdk/utils/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:13:40.473731 human-protocol-sdk-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-29 17:11:26.000000 human-protocol-sdk-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-29 17:11:26.000000 human-protocol-sdk-1.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-29 17:13:40.469731 human-protocol-sdk-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-05-29 17:11:26.000000 human-protocol-sdk-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:13:40.461731 human-protocol-sdk-1.1.4/human_protocol_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-29 17:13:38.000000 human-protocol-sdk-1.1.4/human_protocol_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-05-29 17:11:26.000000 human-protocol-sdk-1.1.4/human_protocol_sdk/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22607 2023-05-29 17:11:26.000000 human-protocol-sdk-1.1.4/human_protocol_sdk/escrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-29 17:11:26.000000 human-protocol-sdk-1.1.4/human_protocol_sdk/kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11595 2023-05-29 17:11:26.000000 human-protocol-sdk-1.1.4/human_protocol_sdk/staking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-05-29 17:11:26.000000 human-protocol-sdk-1.1.4/human_protocol_sdk/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-29 17:11:26.000000 human-protocol-sdk-1.1.4/human_protocol_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:13:40.465731 human-protocol-sdk-1.1.4/human_protocol_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-29 17:13:40.000000 human-protocol-sdk-1.1.4/human_protocol_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-29 17:13:40.000000 human-protocol-sdk-1.1.4/human_protocol_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:13:40.000000 human-protocol-sdk-1.1.4/human_protocol_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-29 17:13:40.000000 human-protocol-sdk-1.1.4/human_protocol_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 17:13:40.000000 human-protocol-sdk-1.1.4/human_protocol_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:13:40.000000 human-protocol-sdk-1.1.4/human_protocol_sdk.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-29 17:11:26.000000 human-protocol-sdk-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:13:40.473731 human-protocol-sdk-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-29 17:11:26.000000 human-protocol-sdk-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:13:40.465731 human-protocol-sdk-1.1.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:11:26.000000 human-protocol-sdk-1.1.4/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:13:40.465731 human-protocol-sdk-1.1.4/test/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:11:26.000000 human-protocol-sdk-1.1.4/test/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19852 2023-05-29 17:11:26.000000 human-protocol-sdk-1.1.4/test/e2e/test_staking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:13:40.469731 human-protocol-sdk-1.1.4/test/human_protocol_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:11:26.000000 human-protocol-sdk-1.1.4/test/human_protocol_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76407 2023-05-29 17:11:26.000000 human-protocol-sdk-1.1.4/test/human_protocol_sdk/test_escrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-05-29 17:11:26.000000 human-protocol-sdk-1.1.4/test/human_protocol_sdk/test_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-05-29 17:11:26.000000 human-protocol-sdk-1.1.4/test/human_protocol_sdk/test_staking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-05-29 17:11:26.000000 human-protocol-sdk-1.1.4/test/human_protocol_sdk/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:13:40.469731 human-protocol-sdk-1.1.4/test/human_protocol_sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-29 17:11:26.000000 human-protocol-sdk-1.1.4/test/human_protocol_sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-29 17:11:26.000000 human-protocol-sdk-1.1.4/test/human_protocol_sdk/utils/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-29 17:11:26.000000 human-protocol-sdk-1.1.4/test/human_protocol_sdk/utils/manifest.py
```

### Comparing `human-protocol-sdk-1.1.2/LICENSE` & `human-protocol-sdk-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `human-protocol-sdk-1.1.2/test/human_protocol_sdk/utils/manifest.py` & `human-protocol-sdk-1.1.4/test/human_protocol_sdk/utils/manifest.py`

 * *Files identical despite different names*

