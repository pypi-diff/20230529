# Comparing `tmp/vmware-nsxlib-19.3.0.tar.gz` & `tmp/vmware-nsxlib-19.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmware-nsxlib-19.3.0.tar", last modified: Mon Apr  3 21:23:15 2023, max compression
+gzip compressed data, was "vmware-nsxlib-19.3.1.tar", last modified: Thu May  4 16:56:27 2023, max compression
```

## Comparing `vmware-nsxlib-19.3.0.tar` & `vmware-nsxlib-19.3.1.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.485784 vmware-nsxlib-19.3.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1893 2023-04-03 21:23:15.000000 vmware-nsxlib-19.3.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36983 2023-04-03 21:23:15.000000 vmware-nsxlib-19.3.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2023-04-03 21:23:15.485784 vmware-nsxlib-19.3.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/babel.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.465784 vmware-nsxlib-19.3.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.465784 vmware-nsxlib-19.3.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2463 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/doc/source/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      493 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/doc/source/readme.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/doc/source/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.461784 vmware-nsxlib-19.3.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.465784 vmware-nsxlib-19.3.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/releasenotes/notes/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.465784 vmware-nsxlib-19.3.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.465784 vmware-nsxlib-19.3.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.469784 vmware-nsxlib-19.3.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9050 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7980 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/run_tests.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1249 2023-04-03 21:23:15.485784 vmware-nsxlib-19.3.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      610 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3496 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.469784 vmware-nsxlib-19.3.0/vmware_nsxlib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1089 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/_i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.469784 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.469784 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.473784 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8272 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/mocks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15186 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/nsxlib_testcase.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.477784 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1385 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/policy_testcase.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1505 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/test_alb_auth_token_provider.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18601 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28725 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/test_ipsec_vpn_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    85381 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/test_lb_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   309672 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/test_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27223 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/test_transaction.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12798 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_cert.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14792 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25132 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1049 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_cluster_management.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23560 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30338 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_load_balancer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7433 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_native_dhcp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8249 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_ns_group_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12060 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_qos_switching_profile.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   114892 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19717 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_router.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29487 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_security.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3403 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_trust_management.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25449 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14669 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_vpn_ipsec.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.481784 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10813 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16955 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12546 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/client_cert.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36269 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/cluster_management.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14235 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4972 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    45071 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/core_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1833 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/debug_retry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7654 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16620 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/lib.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21966 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/load_balancer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3199 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/native_dhcp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6043 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/ns_group_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6617 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/nsx_constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.485784 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11579 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/alb_auth_token_provider.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3361 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    93127 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/core_defs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   225612 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/core_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9618 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/ipsec_vpn_defs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21062 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/ipsec_vpn_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19214 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/lb_defs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    57319 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/lb_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8336 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/transaction.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      681 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33384 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15738 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/router.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25997 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/security.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1420 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/token_provider.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5643 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/trust_management.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29341 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15442 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/v3/vpn_ipsec.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      684 2023-04-03 21:22:52.000000 vmware-nsxlib-19.3.0/vmware_nsxlib/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-03 21:23:15.469784 vmware-nsxlib-19.3.0/vmware_nsxlib.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2023-04-03 21:23:15.000000 vmware-nsxlib-19.3.0/vmware_nsxlib.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3398 2023-04-03 21:23:15.000000 vmware-nsxlib-19.3.0/vmware_nsxlib.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-03 21:23:15.000000 vmware-nsxlib-19.3.0/vmware_nsxlib.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-03 21:23:15.000000 vmware-nsxlib-19.3.0/vmware_nsxlib.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-04-03 21:23:15.000000 vmware-nsxlib-19.3.0/vmware_nsxlib.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2023-04-03 21:23:15.000000 vmware-nsxlib-19.3.0/vmware_nsxlib.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2023-04-03 21:23:15.000000 vmware-nsxlib-19.3.0/vmware_nsxlib.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 16:56:27.116489 vmware-nsxlib-19.3.1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1893 2023-05-04 16:56:26.000000 vmware-nsxlib-19.3.1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37042 2023-05-04 16:56:26.000000 vmware-nsxlib-19.3.1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2023-05-04 16:56:27.116489 vmware-nsxlib-19.3.1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/babel.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 16:56:27.100489 vmware-nsxlib-19.3.1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 16:56:27.104489 vmware-nsxlib-19.3.1/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2463 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/doc/source/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      493 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/doc/source/readme.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/doc/source/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 16:56:27.100489 vmware-nsxlib-19.3.1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 16:56:27.104489 vmware-nsxlib-19.3.1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/releasenotes/notes/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 16:56:27.104489 vmware-nsxlib-19.3.1/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 16:56:27.104489 vmware-nsxlib-19.3.1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 16:56:27.104489 vmware-nsxlib-19.3.1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9050 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7980 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/run_tests.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1249 2023-05-04 16:56:27.116489 vmware-nsxlib-19.3.1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      610 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3496 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 16:56:27.104489 vmware-nsxlib-19.3.1/vmware_nsxlib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1089 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/_i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 16:56:27.104489 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 16:56:27.104489 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 16:56:27.108489 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8272 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/mocks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15186 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/nsxlib_testcase.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 16:56:27.108489 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/policy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/policy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1385 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/policy/policy_testcase.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1505 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/policy/test_alb_auth_token_provider.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18601 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/policy/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28725 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/policy/test_ipsec_vpn_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    85381 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/policy/test_lb_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   309672 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/policy/test_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27223 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/policy/test_transaction.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12798 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_cert.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14792 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25132 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1049 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_cluster_management.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23560 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30338 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_load_balancer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7433 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_native_dhcp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8249 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_ns_group_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12060 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_qos_switching_profile.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   114892 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19717 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_router.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29487 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_security.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3403 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_trust_management.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25449 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14669 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_vpn_ipsec.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 16:56:27.112489 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10813 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16955 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12546 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/client_cert.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36269 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/cluster_management.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14235 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4972 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    45071 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/core_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1833 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/debug_retry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7654 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16620 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/lib.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21966 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/load_balancer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3199 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/native_dhcp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6043 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/ns_group_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6617 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/nsx_constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 16:56:27.116489 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/policy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11579 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/policy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/policy/alb_auth_token_provider.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3361 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/policy/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    93127 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/policy/core_defs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   225610 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/policy/core_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9618 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/policy/ipsec_vpn_defs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21062 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/policy/ipsec_vpn_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19214 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/policy/lb_defs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    57319 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/policy/lb_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8336 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/policy/transaction.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      681 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/policy/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33384 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15738 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/router.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25997 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/security.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1420 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/token_provider.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5643 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/trust_management.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29341 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15442 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/v3/vpn_ipsec.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      684 2023-05-04 16:56:01.000000 vmware-nsxlib-19.3.1/vmware_nsxlib/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-04 16:56:27.104489 vmware-nsxlib-19.3.1/vmware_nsxlib.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2023-05-04 16:56:26.000000 vmware-nsxlib-19.3.1/vmware_nsxlib.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3398 2023-05-04 16:56:27.000000 vmware-nsxlib-19.3.1/vmware_nsxlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-04 16:56:26.000000 vmware-nsxlib-19.3.1/vmware_nsxlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-04 16:56:26.000000 vmware-nsxlib-19.3.1/vmware_nsxlib.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-04 16:56:26.000000 vmware-nsxlib-19.3.1/vmware_nsxlib.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2023-05-04 16:56:26.000000 vmware-nsxlib-19.3.1/vmware_nsxlib.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2023-05-04 16:56:26.000000 vmware-nsxlib-19.3.1/vmware_nsxlib.egg-info/top_level.txt
```

### Comparing `vmware-nsxlib-19.3.0/AUTHORS` & `vmware-nsxlib-19.3.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/CONTRIBUTING.rst` & `vmware-nsxlib-19.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/ChangeLog` & `vmware-nsxlib-19.3.1/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+19.3.1
+------
+
+* Enable H-API delete for Policy Tier1 Api
+
 19.3.0
 ------
 
 * Update version check to use POST API when restore vif
 * Revert "Revert "Add sync\_realization while creating ip-pool/ip-subnet for nsx-keeper""
 * Add ip\_release\_delay when creating IpPool
 * Revert "Add sync\_realization while creating ip-pool/ip-subnet for nsx-keeper"
```

### Comparing `vmware-nsxlib-19.3.0/LICENSE` & `vmware-nsxlib-19.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/PKG-INFO` & `vmware-nsxlib-19.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: vmware-nsxlib
-Version: 19.3.0
+Version: 19.3.1
 Summary: A common library that interfaces with VMware NSX
 Home-page: https://opendev.org/x/vmware-nsxlib
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: TESt:wq
```

### Comparing `vmware-nsxlib-19.3.0/doc/source/conf.py` & `vmware-nsxlib-19.3.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/releasenotes/source/conf.py` & `vmware-nsxlib-19.3.1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/requirements.txt` & `vmware-nsxlib-19.3.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/run_tests.sh` & `vmware-nsxlib-19.3.1/run_tests.sh`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/setup.cfg` & `vmware-nsxlib-19.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/setup.py` & `vmware-nsxlib-19.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/test-requirements.txt` & `vmware-nsxlib-19.3.1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/tox.ini` & `vmware-nsxlib-19.3.1/tox.ini`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/__init__.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/__init__.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/_i18n.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/_i18n.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/base.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/base.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/mocks.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/mocks.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/nsxlib_testcase.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/nsxlib_testcase.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/policy_testcase.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/policy/policy_testcase.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/test_alb_auth_token_provider.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/policy/test_alb_auth_token_provider.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/test_api.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/policy/test_api.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/test_ipsec_vpn_resources.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/policy/test_ipsec_vpn_resources.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/test_lb_resources.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/policy/test_lb_resources.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/test_resources.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/policy/test_resources.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/policy/test_transaction.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/policy/test_transaction.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_cert.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_cert.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_client.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_client.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_cluster.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_cluster.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_cluster_management.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_cluster_management.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_constants.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_constants.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_load_balancer.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_load_balancer.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_native_dhcp.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_native_dhcp.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_ns_group_manager.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_ns_group_manager.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_qos_switching_profile.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_qos_switching_profile.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_resources.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_resources.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_router.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_router.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_security.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_security.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_trust_management.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_trust_management.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_utils.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_utils.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/tests/unit/v3/test_vpn_ipsec.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/tests/unit/v3/test_vpn_ipsec.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/__init__.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/client.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/client.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/client_cert.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/client_cert.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/cluster.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/cluster.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/cluster_management.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/cluster_management.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/config.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/config.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/constants.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/constants.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/core_resources.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/core_resources.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/debug_retry.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/debug_retry.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/exceptions.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/exceptions.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/lib.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/lib.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/load_balancer.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/load_balancer.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/native_dhcp.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/native_dhcp.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/ns_group_manager.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/ns_group_manager.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/nsx_constants.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/nsx_constants.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/__init__.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/alb_auth_token_provider.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/policy/alb_auth_token_provider.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/constants.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/policy/constants.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/core_defs.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/policy/core_defs.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/core_resources.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/policy/core_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1132,15 +1132,15 @@
                                    tenant=tenant)
 
         self._create_or_store(tier1_def)
         return tier1_id
 
     def delete(self, tier1_id, tenant=constants.POLICY_INFRA_TENANT):
         tier1_def = self.entry_def(tier1_id=tier1_id, tenant=tenant)
-        self._delete_with_retry(tier1_def)
+        self._delete_or_store(tier1_def)
 
     def get(self, tier1_id, tenant=constants.POLICY_INFRA_TENANT,
             silent=False):
         tier1_def = self.entry_def(tier1_id=tier1_id, tenant=tenant)
         return self.policy_api.get(tier1_def, silent=silent)
 
     def get_path(self, tier1_id, tenant=constants.POLICY_INFRA_TENANT):
```

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/ipsec_vpn_defs.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/policy/ipsec_vpn_defs.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/ipsec_vpn_resources.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/policy/ipsec_vpn_resources.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/lb_defs.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/policy/lb_defs.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/lb_resources.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/policy/lb_resources.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/transaction.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/policy/transaction.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/policy/utils.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/policy/utils.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/resources.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/resources.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/router.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/router.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/security.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/security.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/token_provider.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/token_provider.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/trust_management.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/trust_management.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/utils.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/utils.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/v3/vpn_ipsec.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/v3/vpn_ipsec.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib/version.py` & `vmware-nsxlib-19.3.1/vmware_nsxlib/version.py`

 * *Files identical despite different names*

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib.egg-info/PKG-INFO` & `vmware-nsxlib-19.3.1/vmware_nsxlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: vmware-nsxlib
-Version: 19.3.0
+Version: 19.3.1
 Summary: A common library that interfaces with VMware NSX
 Home-page: https://opendev.org/x/vmware-nsxlib
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: TESt:wq
```

### Comparing `vmware-nsxlib-19.3.0/vmware_nsxlib.egg-info/SOURCES.txt` & `vmware-nsxlib-19.3.1/vmware_nsxlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

