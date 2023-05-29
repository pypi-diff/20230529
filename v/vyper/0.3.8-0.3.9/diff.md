# Comparing `tmp/vyper-0.3.8.tar.gz` & `tmp/vyper-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vyper-0.3.8.tar", last modified: Tue May 23 15:01:34 2023, max compression
+gzip compressed data, was "vyper-0.3.9.tar", last modified: Mon May 29 15:36:52 2023, max compression
```

## Comparing `vyper-0.3.8.tar` & `vyper-0.3.9.tar`

### file list

```diff
@@ -1,543 +1,543 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.587607 vyper-0.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.527604 vyper-0.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.527604 vyper-0.3.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-23 15:01:16.000000 vyper-0.3.8/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-23 15:01:16.000000 vyper-0.3.8/.github/ISSUE_TEMPLATE/vip.md
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-23 15:01:16.000000 vyper-0.3.8/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.527604 vyper-0.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-23 15:01:16.000000 vyper-0.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-23 15:01:16.000000 vyper-0.3.8/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-23 15:01:16.000000 vyper-0.3.8/.github/workflows/era-tester.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-23 15:01:16.000000 vyper-0.3.8/.github/workflows/ghcr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-23 15:01:16.000000 vyper-0.3.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-05-23 15:01:16.000000 vyper-0.3.8/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-23 15:01:16.000000 vyper-0.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-23 15:01:16.000000 vyper-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-23 15:01:16.000000 vyper-0.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-23 15:01:16.000000 vyper-0.3.8/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-23 15:01:16.000000 vyper-0.3.8/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-05-23 15:01:17.000000 vyper-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-23 15:01:17.000000 vyper-0.3.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-23 15:01:34.587607 vyper-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-23 15:01:17.000000 vyper-0.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-23 15:01:17.000000 vyper-0.3.8/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.535604 vyper-0.3.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.519604 vyper-0.3.8/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.535604 vyper-0.3.8/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/_static/css/dark.css
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/_static/css/toggle.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.535604 vyper-0.3.8/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/_static/js/toggle.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.535604 vyper-0.3.8/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/_templates/versions.html
--rw-r--r--   0 runner    (1001) docker     (123)    36099 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/built-in-functions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/compiler-exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/compiling-a-contract.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/constants-and-vars.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/control-structures.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/deploying-contracts.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/event-logging.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/installing-vyper.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/interfaces.rst
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/natspec.rst
--rw-r--r--   0 runner    (1001) docker     (123)    57259 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/resources.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/scoping-and-declarations.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/statements.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/structure-of-a-contract.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15593 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/style-guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/testing-contracts-brownie.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/testing-contracts-ethtester.rst
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/testing-contracts.rst
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/toctree.rst
--rw-r--r--   0 runner    (1001) docker     (123)    22576 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/types.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/versioning.rst
--rw-r--r--   0 runner    (1001) docker     (123)    29136 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/vyper-by-example.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-23 15:01:17.000000 vyper-0.3.8/docs/vyper-logo-transparent.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.535604 vyper-0.3.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.535604 vyper-0.3.8/examples/auctions/
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-05-23 15:01:17.000000 vyper-0.3.8/examples/auctions/blind_auction.vy
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-23 15:01:17.000000 vyper-0.3.8/examples/auctions/simple_open_auction.vy
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-23 15:01:17.000000 vyper-0.3.8/examples/crowdfund.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.535604 vyper-0.3.8/examples/factory/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-23 15:01:17.000000 vyper-0.3.8/examples/factory/Exchange.vy
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-23 15:01:17.000000 vyper-0.3.8/examples/factory/Factory.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.535604 vyper-0.3.8/examples/market_maker/
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-23 15:01:17.000000 vyper-0.3.8/examples/market_maker/on_chain_market_maker.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.535604 vyper-0.3.8/examples/name_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-23 15:01:17.000000 vyper-0.3.8/examples/name_registry/name_registry.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.535604 vyper-0.3.8/examples/safe_remote_purchase/
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-23 15:01:17.000000 vyper-0.3.8/examples/safe_remote_purchase/safe_remote_purchase.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.535604 vyper-0.3.8/examples/stock/
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-05-23 15:01:17.000000 vyper-0.3.8/examples/stock/company.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.535604 vyper-0.3.8/examples/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-23 15:01:17.000000 vyper-0.3.8/examples/storage/advanced_storage.vy
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-23 15:01:17.000000 vyper-0.3.8/examples/storage/storage.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.535604 vyper-0.3.8/examples/tokens/
--rw-r--r--   0 runner    (1001) docker     (123)    15232 2023-05-23 15:01:17.000000 vyper-0.3.8/examples/tokens/ERC1155ownable.vy
--rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-05-23 15:01:17.000000 vyper-0.3.8/examples/tokens/ERC20.vy
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-05-23 15:01:17.000000 vyper-0.3.8/examples/tokens/ERC4626.vy
--rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-05-23 15:01:17.000000 vyper-0.3.8/examples/tokens/ERC721.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.535604 vyper-0.3.8/examples/voting/
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-23 15:01:17.000000 vyper-0.3.8/examples/voting/ballot.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.535604 vyper-0.3.8/examples/wallet/
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-23 15:01:17.000000 vyper-0.3.8/examples/wallet/wallet.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.535604 vyper-0.3.8/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      265 2023-05-23 15:01:17.000000 vyper-0.3.8/hooks/build
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.539605 vyper-0.3.8/logo/
--rw-r--r--   0 runner    (1001) docker     (123)    42373 2023-05-23 15:01:17.000000 vyper-0.3.8/logo/vyper-logo-flat.png
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-23 15:01:17.000000 vyper-0.3.8/logo/vyper-logo-flat.svg
--rw-r--r--   0 runner    (1001) docker     (123)    38259 2023-05-23 15:01:17.000000 vyper-0.3.8/logo/vyper-logo-transparent.png
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-23 15:01:17.000000 vyper-0.3.8/logo/vyper-logo-transparent.svg
--rw-r--r--   0 runner    (1001) docker     (123)   647034 2023-05-23 15:01:17.000000 vyper-0.3.8/logo/vyper-logo.ai
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-23 15:01:17.000000 vyper-0.3.8/make.cmd
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-23 15:01:17.000000 vyper-0.3.8/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      239 2023-05-23 15:01:17.000000 vyper-0.3.8/quicktest.sh
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-23 15:01:17.000000 vyper-0.3.8/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-23 15:01:34.587607 vyper-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-23 15:01:17.000000 vyper-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.539605 vyper-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.539605 vyper-0.3.8/tests/ast/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.543605 vyper-0.3.8/tests/ast/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/ast/nodes/test_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/ast/nodes/test_compare_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/ast/nodes/test_evaluate_binop_decimal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/ast/nodes/test_evaluate_binop_int.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/ast/nodes/test_evaluate_boolop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/ast/nodes/test_evaluate_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/ast/nodes/test_evaluate_subscript.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/ast/nodes/test_evaluate_unaryop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/ast/nodes/test_from_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/ast/nodes/test_get_children.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/ast/nodes/test_get_descendants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/ast/nodes/test_hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/ast/nodes/test_replace_in_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/ast/test_folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/ast/test_natspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/ast/test_pre_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/base_conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.523604 vyper-0.3.8/tests/builtins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.543605 vyper-0.3.8/tests/builtins/folding/
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/builtins/folding/test_abs.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/builtins/folding/test_addmod_mulmod.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/builtins/folding/test_bitwise.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/builtins/folding/test_epsilon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/builtins/folding/test_floor_ceil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/builtins/folding/test_fold_as_wei_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/builtins/folding/test_keccak_sha.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/builtins/folding/test_len.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/builtins/folding/test_min_max.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/builtins/folding/test_powmod.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.523604 vyper-0.3.8/tests/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.543605 vyper-0.3.8/tests/cli/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/cli/outputs/test_storage_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/cli/outputs/test_storage_layout_overrides.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.543605 vyper-0.3.8/tests/cli/vyper_compile/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/cli/vyper_compile/test_compile_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/cli/vyper_compile/test_import_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/cli/vyper_compile/test_parse_args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.547605 vyper-0.3.8/tests/cli/vyper_json/
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/cli/vyper_json/test_compile_from_input_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/cli/vyper_json/test_compile_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/cli/vyper_json/test_get_contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/cli/vyper_json/test_get_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/cli/vyper_json/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/cli/vyper_json/test_output_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/cli/vyper_json/test_output_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/cli/vyper_json/test_parse_args_vyperjson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.547605 vyper-0.3.8/tests/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.547605 vyper-0.3.8/tests/compiler/asm/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/compiler/asm/test_asm_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.547605 vyper-0.3.8/tests/compiler/ir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/compiler/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/compiler/ir/test_compile_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/compiler/ir/test_optimize_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/compiler/ir/test_repeat.py
--rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/compiler/ir/test_with.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/compiler/test_bytecode_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/compiler/test_calldatacopy.py
--rw-r--r--   0 runner    (1001) docker     (123)    24862 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/compiler/test_compile_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/compiler/test_opcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/compiler/test_pre_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/compiler/test_sha3_32.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/compiler/test_source_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.547605 vyper-0.3.8/tests/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.547605 vyper-0.3.8/tests/examples/auctions/
--rw-r--r--   0 runner    (1001) docker     (123)    12478 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/examples/auctions/test_blind_auction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/examples/auctions/test_simple_open_auction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.547605 vyper-0.3.8/tests/examples/company/
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/examples/company/test_company.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/examples/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.547605 vyper-0.3.8/tests/examples/crowdfund/
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/examples/crowdfund/test_crowdfund_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.551605 vyper-0.3.8/tests/examples/factory/
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/examples/factory/test_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.551605 vyper-0.3.8/tests/examples/market_maker/
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/examples/market_maker/test_on_chain_market_maker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.551605 vyper-0.3.8/tests/examples/name_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/examples/name_registry/test_name_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.551605 vyper-0.3.8/tests/examples/safe_remote_purchase/
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/examples/safe_remote_purchase/test_safe_remote_purchase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.551605 vyper-0.3.8/tests/examples/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/examples/storage/test_advanced_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/examples/storage/test_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.551605 vyper-0.3.8/tests/examples/tokens/
--rw-r--r--   0 runner    (1001) docker     (123)    14584 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/examples/tokens/test_erc1155.py
--rw-r--r--   0 runner    (1001) docker     (123)    14626 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/examples/tokens/test_erc20.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/examples/tokens/test_erc4626.py
--rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/examples/tokens/test_erc721.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.551605 vyper-0.3.8/tests/examples/voting/
--rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/examples/voting/test_ballot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.551605 vyper-0.3.8/tests/examples/wallet/
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/examples/wallet/test_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.551605 vyper-0.3.8/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/fixtures/memorymock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.551605 vyper-0.3.8/tests/functional/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.551605 vyper-0.3.8/tests/functional/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/functional/codegen/test_struct_return.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/functional/codegen/test_tuple_return.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.551605 vyper-0.3.8/tests/functional/semantics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.551605 vyper-0.3.8/tests/functional/semantics/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/functional/semantics/analysis/test_array_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/functional/semantics/analysis/test_cyclic_function_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/functional/semantics/analysis/test_for_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/functional/semantics/analysis/test_potential_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/functional/semantics/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/functional/semantics/test_namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.555605 vyper-0.3.8/tests/functional/semantics/types/
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/functional/semantics/types/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/functional/semantics/types/test_pure_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/functional/semantics/types/test_size_in_bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/functional/semantics/types/test_type_from_abi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/functional/semantics/types/test_type_from_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/functional/test_storage_slots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.555605 vyper-0.3.8/tests/fuzzing/
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/fuzzing/test_exponents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.555605 vyper-0.3.8/tests/grammar/
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/grammar/test_grammar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.555605 vyper-0.3.8/tests/parser/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.555605 vyper-0.3.8/tests/parser/ast_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/ast_utils/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/ast_utils/test_ast_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.559605 vyper-0.3.8/tests/parser/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/exceptions/test_argument_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/exceptions/test_call_violation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/exceptions/test_constancy_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/exceptions/test_function_declaration_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/exceptions/test_instantiation_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/exceptions/test_invalid_literal_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/exceptions/test_invalid_payable.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/exceptions/test_invalid_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/exceptions/test_invalid_type_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/exceptions/test_namespace_collision.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/exceptions/test_overflow_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/exceptions/test_structure_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/exceptions/test_syntax_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/exceptions/test_type_mismatch_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/exceptions/test_undeclared_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/exceptions/test_variable_declaration_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/exceptions/test_vyper_exception_pos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.563606 vyper-0.3.8/tests/parser/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.563606 vyper-0.3.8/tests/parser/features/arithmetic/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/arithmetic/test_division.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/arithmetic/test_modulo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.563606 vyper-0.3.8/tests/parser/features/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/decorators/test_nonreentrant.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/decorators/test_payable.py
--rw-r--r--   0 runner    (1001) docker     (123)    14672 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/decorators/test_private.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/decorators/test_public.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/decorators/test_pure.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/decorators/test_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.563606 vyper-0.3.8/tests/parser/features/external_contracts/
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/external_contracts/test_erc20_abi.py
--rw-r--r--   0 runner    (1001) docker     (123)    58262 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/external_contracts/test_external_contract_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/external_contracts/test_modifiable_external_contract_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/external_contracts/test_self_call_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.563606 vyper-0.3.8/tests/parser/features/iteration/
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/iteration/test_break.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/iteration/test_continue.py
--rw-r--r--   0 runner    (1001) docker     (123)    14417 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/iteration/test_for_in_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/iteration/test_for_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/iteration/test_range_in.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/test_address_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/test_assert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/test_assert_unreachable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/test_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/test_bytes_map_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    17561 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/test_clampers.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/test_comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/test_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/test_conditionals.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/test_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/test_gas.py
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/test_immutable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/test_internal_call.py
--rw-r--r--   0 runner    (1001) docker     (123)    33790 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/test_logging_bytes_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/test_logging_from_call.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/test_memory_dealloc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/test_packing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/test_reverting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/test_short_circuiting.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/test_string_map_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/test_ternary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/features/test_transient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.571606 vyper-0.3.8/tests/parser/functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_abi.py
--rw-r--r--   0 runner    (1001) docker     (123)    12558 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_abi_decode.py
--rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_abi_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_addmod.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_as_wei_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_bitwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_block_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_ceil.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)    19453 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_create_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_default_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_default_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_ec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_ecrecover.py
--rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_extract32.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_floor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16188 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_is_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_keccak256.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_method_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_minmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_minmax_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_mkstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_mulmod.py
--rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_raw_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_return.py
--rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_return_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_return_tuple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_send.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_sha256.py
--rw-r--r--   0 runner    (1001) docker     (123)    10390 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_unary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/functions/test_unsafe_math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.571606 vyper-0.3.8/tests/parser/globals/
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/globals/test_getters.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/globals/test_globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/globals/test_setters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.571606 vyper-0.3.8/tests/parser/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/integration/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/integration/test_crowdfund.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/integration/test_escrow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.571606 vyper-0.3.8/tests/parser/parser_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/parser_utils/test_annotate_and_optimize_ast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.575606 vyper-0.3.8/tests/parser/syntax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_abi_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_address_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_ann_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_as_uint256.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_as_wei_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_blockscope.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_bool_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_chainid.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_code_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_codehash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_conditionals.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_create_with_code_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_dynamic_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_extract32.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_for_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_functions_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_immutables.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_invalids.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_keccak256.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_len.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_minmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_minmax_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_msg_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_nested_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_no_none.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_print.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_public.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_raw_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_return_tuple.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_self_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_selfdestruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_send.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_ternary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_tuple_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/test_unbalanced_return.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.575606 vyper-0.3.8/tests/parser/syntax/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/utils/test_event_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/utils/test_function_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/syntax/utils/test_variable_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/test_call_graph_stability.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.575606 vyper-0.3.8/tests/parser/types/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.575606 vyper-0.3.8/tests/parser/types/numbers/
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/types/numbers/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/types/numbers/test_decimals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/types/numbers/test_isqrt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/types/numbers/test_signed_ints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/types/numbers/test_sqrt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/types/numbers/test_unsigned_ints.py
--rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/types/test_bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/types/test_bytes_literal.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/types/test_bytes_zero_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)    49324 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/types/test_dynamic_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/types/test_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2377 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/types/test_identifier_naming.py
--rw-r--r--   0 runner    (1001) docker     (123)    23319 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/types/test_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/types/test_node_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/types/test_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/types/test_string_literal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.575606 vyper-0.3.8/tests/parser/types/value/
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/parser/types/value/test_as_wei_value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.575606 vyper-0.3.8/tests/signatures/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/signatures/test_invalid_function_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/signatures/test_method_id_conflicts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-05-23 15:01:17.000000 vyper-0.3.8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-23 15:01:17.000000 vyper-0.3.8/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.579606 vyper-0.3.8/vyper/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/abi_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.579606 vyper-0.3.8/vyper/ast/
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/ast/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/ast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/ast/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9622 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/ast/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/ast/expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/ast/folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/ast/grammar.lark
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/ast/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/ast/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/ast/natspec.py
--rw-r--r--   0 runner    (1001) docker     (123)    44488 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/ast/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/ast/nodes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/ast/pre_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/ast/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/ast/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.579606 vyper-0.3.8/vyper/builtins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/builtins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16343 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/builtins/_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/builtins/_signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/builtins/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    92662 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/builtins/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.583607 vyper-0.3.8/vyper/builtins/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/builtins/interfaces/ERC165.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/builtins/interfaces/ERC20.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/builtins/interfaces/ERC20Detailed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/builtins/interfaces/ERC4626.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/builtins/interfaces/ERC721.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/builtins/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.583607 vyper-0.3.8/vyper/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/cli/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11182 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/cli/vyper_compile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1894 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/cli/vyper_ir.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18889 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/cli/vyper_json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3805 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/cli/vyper_serve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.583607 vyper-0.3.8/vyper/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/codegen/abi_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/codegen/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/codegen/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    39472 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/codegen/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/codegen/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    30185 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/codegen/expr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/codegen/external_call.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.583607 vyper-0.3.8/vyper/codegen/function_definitions/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/codegen/function_definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/codegen/function_definitions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/codegen/function_definitions/external_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/codegen/function_definitions/internal_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/codegen/function_definitions/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/codegen/global_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    21590 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/codegen/ir_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/codegen/keccak256_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/codegen/memory_allocator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/codegen/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/codegen/return_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/codegen/self_call.py
--rw-r--r--   0 runner    (1001) docker     (123)    16378 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/codegen/stmt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.583607 vyper-0.3.8/vyper/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/compiler/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/compiler/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10041 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/compiler/phases.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/compiler/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/compiler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.583607 vyper-0.3.8/vyper/evm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/evm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/evm/address_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/evm/opcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.587607 vyper-0.3.8/vyper/ir/
--rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/ir/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39171 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/ir/compile_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)    23828 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/ir/optimizer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1076 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/ir/s_expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.587607 vyper-0.3.8/vyper/semantics/
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/semantics/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/semantics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.587607 vyper-0.3.8/vyper/semantics/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/semantics/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/semantics/analysis/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/semantics/analysis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/semantics/analysis/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/semantics/analysis/data_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/semantics/analysis/levenshtein_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24757 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/semantics/analysis/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    14227 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/semantics/analysis/module.py
--rw-r--r--   0 runner    (1001) docker     (123)    22704 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/semantics/analysis/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/semantics/data_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/semantics/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/semantics/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.587607 vyper-0.3.8/vyper/semantics/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/semantics/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/semantics/types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/semantics/types/bytestrings.py
--rw-r--r--   0 runner    (1001) docker     (123)    24304 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/semantics/types/function.py
--rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/semantics/types/primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/semantics/types/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/semantics/types/subscriptable.py
--rw-r--r--   0 runner    (1001) docker     (123)    20687 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/semantics/types/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/semantics/types/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 15:01:34.000000 vyper-0.3.8/vyper/version.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 15:01:30.000000 vyper-0.3.8/vyper/vyper_git_commithash.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-23 15:01:17.000000 vyper-0.3.8/vyper/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:34.579606 vyper-0.3.8/vyper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-23 15:01:34.000000 vyper-0.3.8/vyper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16239 2023-05-23 15:01:34.000000 vyper-0.3.8/vyper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 15:01:34.000000 vyper-0.3.8/vyper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-23 15:01:34.000000 vyper-0.3.8/vyper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-23 15:01:34.000000 vyper-0.3.8/vyper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 15:01:34.000000 vyper-0.3.8/vyper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.984714 vyper-0.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.948714 vyper-0.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.948714 vyper-0.3.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-29 15:36:36.000000 vyper-0.3.9/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-29 15:36:36.000000 vyper-0.3.9/.github/ISSUE_TEMPLATE/vip.md
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-29 15:36:36.000000 vyper-0.3.9/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.948714 vyper-0.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-29 15:36:36.000000 vyper-0.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-29 15:36:36.000000 vyper-0.3.9/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-29 15:36:36.000000 vyper-0.3.9/.github/workflows/era-tester.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-29 15:36:36.000000 vyper-0.3.9/.github/workflows/ghcr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-29 15:36:36.000000 vyper-0.3.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-05-29 15:36:36.000000 vyper-0.3.9/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-29 15:36:36.000000 vyper-0.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-29 15:36:36.000000 vyper-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-29 15:36:36.000000 vyper-0.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-29 15:36:36.000000 vyper-0.3.9/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-29 15:36:36.000000 vyper-0.3.9/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-05-29 15:36:36.000000 vyper-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-29 15:36:36.000000 vyper-0.3.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-29 15:36:52.984714 vyper-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-29 15:36:36.000000 vyper-0.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-29 15:36:36.000000 vyper-0.3.9/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.952714 vyper-0.3.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.940714 vyper-0.3.9/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.952714 vyper-0.3.9/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/_static/css/dark.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/_static/css/toggle.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.952714 vyper-0.3.9/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/_static/js/toggle.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.952714 vyper-0.3.9/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/_templates/versions.html
+-rw-r--r--   0 runner    (1001) docker     (123)    36099 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/built-in-functions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/compiler-exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/compiling-a-contract.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/constants-and-vars.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/control-structures.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/deploying-contracts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/event-logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/installing-vyper.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/interfaces.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/natspec.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    57821 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/resources.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/scoping-and-declarations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/statements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/structure-of-a-contract.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15593 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/style-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/testing-contracts-brownie.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/testing-contracts-ethtester.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/testing-contracts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/toctree.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    22576 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/types.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/versioning.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    29136 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/vyper-by-example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-29 15:36:36.000000 vyper-0.3.9/docs/vyper-logo-transparent.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.952714 vyper-0.3.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.952714 vyper-0.3.9/examples/auctions/
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-05-29 15:36:36.000000 vyper-0.3.9/examples/auctions/blind_auction.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-29 15:36:36.000000 vyper-0.3.9/examples/auctions/simple_open_auction.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-29 15:36:36.000000 vyper-0.3.9/examples/crowdfund.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.952714 vyper-0.3.9/examples/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-29 15:36:36.000000 vyper-0.3.9/examples/factory/Exchange.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-29 15:36:36.000000 vyper-0.3.9/examples/factory/Factory.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.952714 vyper-0.3.9/examples/market_maker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-29 15:36:36.000000 vyper-0.3.9/examples/market_maker/on_chain_market_maker.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.952714 vyper-0.3.9/examples/name_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-29 15:36:36.000000 vyper-0.3.9/examples/name_registry/name_registry.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.952714 vyper-0.3.9/examples/safe_remote_purchase/
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-29 15:36:36.000000 vyper-0.3.9/examples/safe_remote_purchase/safe_remote_purchase.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.952714 vyper-0.3.9/examples/stock/
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-05-29 15:36:36.000000 vyper-0.3.9/examples/stock/company.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.952714 vyper-0.3.9/examples/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-29 15:36:36.000000 vyper-0.3.9/examples/storage/advanced_storage.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-29 15:36:36.000000 vyper-0.3.9/examples/storage/storage.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.952714 vyper-0.3.9/examples/tokens/
+-rw-r--r--   0 runner    (1001) docker     (123)    15232 2023-05-29 15:36:36.000000 vyper-0.3.9/examples/tokens/ERC1155ownable.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-05-29 15:36:36.000000 vyper-0.3.9/examples/tokens/ERC20.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-05-29 15:36:36.000000 vyper-0.3.9/examples/tokens/ERC4626.vy
+-rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-05-29 15:36:36.000000 vyper-0.3.9/examples/tokens/ERC721.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.952714 vyper-0.3.9/examples/voting/
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-29 15:36:36.000000 vyper-0.3.9/examples/voting/ballot.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.952714 vyper-0.3.9/examples/wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-29 15:36:36.000000 vyper-0.3.9/examples/wallet/wallet.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.952714 vyper-0.3.9/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      265 2023-05-29 15:36:36.000000 vyper-0.3.9/hooks/build
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.952714 vyper-0.3.9/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)    42373 2023-05-29 15:36:36.000000 vyper-0.3.9/logo/vyper-logo-flat.png
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-29 15:36:36.000000 vyper-0.3.9/logo/vyper-logo-flat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    38259 2023-05-29 15:36:36.000000 vyper-0.3.9/logo/vyper-logo-transparent.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-29 15:36:36.000000 vyper-0.3.9/logo/vyper-logo-transparent.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   647034 2023-05-29 15:36:36.000000 vyper-0.3.9/logo/vyper-logo.ai
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-29 15:36:36.000000 vyper-0.3.9/make.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-29 15:36:36.000000 vyper-0.3.9/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      239 2023-05-29 15:36:36.000000 vyper-0.3.9/quicktest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-29 15:36:36.000000 vyper-0.3.9/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-29 15:36:52.984714 vyper-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-29 15:36:36.000000 vyper-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.952714 vyper-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.956714 vyper-0.3.9/tests/ast/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.956714 vyper-0.3.9/tests/ast/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/ast/nodes/test_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/ast/nodes/test_compare_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/ast/nodes/test_evaluate_binop_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/ast/nodes/test_evaluate_binop_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/ast/nodes/test_evaluate_boolop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/ast/nodes/test_evaluate_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/ast/nodes/test_evaluate_subscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/ast/nodes/test_evaluate_unaryop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/ast/nodes/test_from_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/ast/nodes/test_get_children.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/ast/nodes/test_get_descendants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/ast/nodes/test_hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/ast/nodes/test_replace_in_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/ast/test_folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/ast/test_natspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/ast/test_pre_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/base_conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.944714 vyper-0.3.9/tests/builtins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.956714 vyper-0.3.9/tests/builtins/folding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/builtins/folding/test_abs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/builtins/folding/test_addmod_mulmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/builtins/folding/test_bitwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/builtins/folding/test_epsilon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/builtins/folding/test_floor_ceil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/builtins/folding/test_fold_as_wei_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/builtins/folding/test_keccak_sha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/builtins/folding/test_len.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/builtins/folding/test_min_max.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/builtins/folding/test_powmod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.944714 vyper-0.3.9/tests/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.956714 vyper-0.3.9/tests/cli/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/cli/outputs/test_storage_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/cli/outputs/test_storage_layout_overrides.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.956714 vyper-0.3.9/tests/cli/vyper_compile/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/cli/vyper_compile/test_compile_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/cli/vyper_compile/test_import_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/cli/vyper_compile/test_parse_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.956714 vyper-0.3.9/tests/cli/vyper_json/
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/cli/vyper_json/test_compile_from_input_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/cli/vyper_json/test_compile_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/cli/vyper_json/test_get_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/cli/vyper_json/test_get_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/cli/vyper_json/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/cli/vyper_json/test_output_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/cli/vyper_json/test_output_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/cli/vyper_json/test_parse_args_vyperjson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.956714 vyper-0.3.9/tests/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.956714 vyper-0.3.9/tests/compiler/asm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/compiler/asm/test_asm_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.960714 vyper-0.3.9/tests/compiler/ir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/compiler/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/compiler/ir/test_compile_ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/compiler/ir/test_optimize_ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/compiler/ir/test_repeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/compiler/ir/test_with.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/compiler/test_bytecode_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/compiler/test_calldatacopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24862 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/compiler/test_compile_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/compiler/test_opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/compiler/test_pre_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/compiler/test_sha3_32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/compiler/test_source_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.960714 vyper-0.3.9/tests/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.960714 vyper-0.3.9/tests/examples/auctions/
+-rw-r--r--   0 runner    (1001) docker     (123)    12478 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/examples/auctions/test_blind_auction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/examples/auctions/test_simple_open_auction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.960714 vyper-0.3.9/tests/examples/company/
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/examples/company/test_company.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/examples/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.960714 vyper-0.3.9/tests/examples/crowdfund/
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/examples/crowdfund/test_crowdfund_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.960714 vyper-0.3.9/tests/examples/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/examples/factory/test_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.960714 vyper-0.3.9/tests/examples/market_maker/
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/examples/market_maker/test_on_chain_market_maker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.960714 vyper-0.3.9/tests/examples/name_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/examples/name_registry/test_name_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.960714 vyper-0.3.9/tests/examples/safe_remote_purchase/
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/examples/safe_remote_purchase/test_safe_remote_purchase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.960714 vyper-0.3.9/tests/examples/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/examples/storage/test_advanced_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/examples/storage/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.960714 vyper-0.3.9/tests/examples/tokens/
+-rw-r--r--   0 runner    (1001) docker     (123)    14584 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/examples/tokens/test_erc1155.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14626 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/examples/tokens/test_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/examples/tokens/test_erc4626.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/examples/tokens/test_erc721.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.960714 vyper-0.3.9/tests/examples/voting/
+-rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/examples/voting/test_ballot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.960714 vyper-0.3.9/tests/examples/wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/examples/wallet/test_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.960714 vyper-0.3.9/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/fixtures/memorymock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.960714 vyper-0.3.9/tests/functional/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.960714 vyper-0.3.9/tests/functional/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/functional/codegen/test_struct_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/functional/codegen/test_tuple_return.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.960714 vyper-0.3.9/tests/functional/semantics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.960714 vyper-0.3.9/tests/functional/semantics/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/functional/semantics/analysis/test_array_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/functional/semantics/analysis/test_cyclic_function_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/functional/semantics/analysis/test_for_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/functional/semantics/analysis/test_potential_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/functional/semantics/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/functional/semantics/test_namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.960714 vyper-0.3.9/tests/functional/semantics/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/functional/semantics/types/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/functional/semantics/types/test_pure_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/functional/semantics/types/test_size_in_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/functional/semantics/types/test_type_from_abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/functional/semantics/types/test_type_from_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/functional/test_storage_slots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.960714 vyper-0.3.9/tests/fuzzing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/fuzzing/test_exponents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.960714 vyper-0.3.9/tests/grammar/
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/grammar/test_grammar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.960714 vyper-0.3.9/tests/parser/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.960714 vyper-0.3.9/tests/parser/ast_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/ast_utils/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/ast_utils/test_ast_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.964714 vyper-0.3.9/tests/parser/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/exceptions/test_argument_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/exceptions/test_call_violation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/exceptions/test_constancy_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/exceptions/test_function_declaration_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/exceptions/test_instantiation_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/exceptions/test_invalid_literal_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/exceptions/test_invalid_payable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/exceptions/test_invalid_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/exceptions/test_invalid_type_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/exceptions/test_namespace_collision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/exceptions/test_overflow_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/exceptions/test_structure_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/exceptions/test_syntax_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/exceptions/test_type_mismatch_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/exceptions/test_undeclared_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/exceptions/test_variable_declaration_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/exceptions/test_vyper_exception_pos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.964714 vyper-0.3.9/tests/parser/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.964714 vyper-0.3.9/tests/parser/features/arithmetic/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/arithmetic/test_division.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/arithmetic/test_modulo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.964714 vyper-0.3.9/tests/parser/features/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/decorators/test_nonreentrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/decorators/test_payable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14672 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/decorators/test_private.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/decorators/test_public.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/decorators/test_pure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/decorators/test_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.964714 vyper-0.3.9/tests/parser/features/external_contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/external_contracts/test_erc20_abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58262 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/external_contracts/test_external_contract_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/external_contracts/test_modifiable_external_contract_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/external_contracts/test_self_call_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.968714 vyper-0.3.9/tests/parser/features/iteration/
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/iteration/test_break.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/iteration/test_continue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14417 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/iteration/test_for_in_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/iteration/test_for_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/iteration/test_range_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/test_address_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/test_assert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/test_assert_unreachable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/test_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/test_bytes_map_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17561 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/test_clampers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/test_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/test_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/test_conditionals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/test_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/test_gas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/test_immutable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/test_internal_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33790 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/test_logging_bytes_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/test_logging_from_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/test_memory_dealloc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/test_packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/test_reverting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/test_short_circuiting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/test_string_map_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/test_ternary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/features/test_transient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.968714 vyper-0.3.9/tests/parser/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12558 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_abi_decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_abi_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_addmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_as_wei_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_bitwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_block_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_ceil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19453 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_create_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_default_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_default_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_ec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_ecrecover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_extract32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_floor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16188 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_is_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_method_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_minmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_minmax_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_mkstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_mulmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_raw_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_return_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_return_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10390 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_unary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/functions/test_unsafe_math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.968714 vyper-0.3.9/tests/parser/globals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/globals/test_getters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/globals/test_globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/globals/test_setters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.968714 vyper-0.3.9/tests/parser/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/integration/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/integration/test_crowdfund.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/integration/test_escrow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.968714 vyper-0.3.9/tests/parser/parser_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/parser_utils/test_annotate_and_optimize_ast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.972714 vyper-0.3.9/tests/parser/syntax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_abi_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_address_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_ann_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_as_uint256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_as_wei_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_blockscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_bool_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_chainid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_code_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_codehash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_conditionals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_create_with_code_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_dynamic_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_extract32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_for_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_functions_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_immutables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_invalids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_len.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_minmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_minmax_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_msg_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_nested_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_no_none.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_print.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_public.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_raw_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_return_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_self_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_selfdestruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_ternary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_tuple_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/test_unbalanced_return.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.972714 vyper-0.3.9/tests/parser/syntax/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/utils/test_event_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/utils/test_function_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/syntax/utils/test_variable_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/test_call_graph_stability.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.976714 vyper-0.3.9/tests/parser/types/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.976714 vyper-0.3.9/tests/parser/types/numbers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/types/numbers/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/types/numbers/test_decimals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/types/numbers/test_isqrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/types/numbers/test_signed_ints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/types/numbers/test_sqrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/types/numbers/test_unsigned_ints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/types/test_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/types/test_bytes_literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/types/test_bytes_zero_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49324 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/types/test_dynamic_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/types/test_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2377 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/types/test_identifier_naming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23319 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/types/test_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/types/test_node_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/types/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/types/test_string_literal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.976714 vyper-0.3.9/tests/parser/types/value/
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/parser/types/value/test_as_wei_value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.976714 vyper-0.3.9/tests/signatures/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/signatures/test_invalid_function_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/signatures/test_method_id_conflicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-05-29 15:36:36.000000 vyper-0.3.9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-29 15:36:36.000000 vyper-0.3.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.976714 vyper-0.3.9/vyper/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/abi_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.980714 vyper-0.3.9/vyper/ast/
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/ast/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/ast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/ast/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9622 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/ast/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/ast/expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/ast/folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/ast/grammar.lark
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/ast/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/ast/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/ast/natspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44488 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/ast/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/ast/nodes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/ast/pre_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/ast/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/ast/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.980714 vyper-0.3.9/vyper/builtins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/builtins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16343 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/builtins/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/builtins/_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/builtins/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92709 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/builtins/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.980714 vyper-0.3.9/vyper/builtins/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/builtins/interfaces/ERC165.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/builtins/interfaces/ERC20.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/builtins/interfaces/ERC20Detailed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/builtins/interfaces/ERC4626.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/builtins/interfaces/ERC721.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/builtins/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.980714 vyper-0.3.9/vyper/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/cli/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11182 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/cli/vyper_compile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1894 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/cli/vyper_ir.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18894 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/cli/vyper_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3805 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/cli/vyper_serve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.980714 vyper-0.3.9/vyper/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/codegen/abi_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/codegen/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/codegen/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39472 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/codegen/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/codegen/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30185 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/codegen/expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/codegen/external_call.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.980714 vyper-0.3.9/vyper/codegen/function_definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/codegen/function_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/codegen/function_definitions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/codegen/function_definitions/external_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/codegen/function_definitions/internal_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/codegen/function_definitions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/codegen/global_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21590 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/codegen/ir_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/codegen/keccak256_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/codegen/memory_allocator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/codegen/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/codegen/return_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/codegen/self_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16378 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/codegen/stmt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.980714 vyper-0.3.9/vyper/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/compiler/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/compiler/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10041 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/compiler/phases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/compiler/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/compiler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.984714 vyper-0.3.9/vyper/evm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/evm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/evm/address_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/evm/opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.984714 vyper-0.3.9/vyper/ir/
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/ir/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39327 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/ir/compile_ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23828 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/ir/optimizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1076 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/ir/s_expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.984714 vyper-0.3.9/vyper/semantics/
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/semantics/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/semantics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.984714 vyper-0.3.9/vyper/semantics/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/semantics/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/semantics/analysis/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/semantics/analysis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/semantics/analysis/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/semantics/analysis/data_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/semantics/analysis/levenshtein_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24757 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/semantics/analysis/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14227 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/semantics/analysis/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22704 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/semantics/analysis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/semantics/data_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/semantics/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/semantics/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.984714 vyper-0.3.9/vyper/semantics/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/semantics/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/semantics/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/semantics/types/bytestrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24304 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/semantics/types/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/semantics/types/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/semantics/types/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/semantics/types/subscriptable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20687 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/semantics/types/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/semantics/types/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-29 15:36:52.000000 vyper-0.3.9/vyper/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 15:36:49.000000 vyper-0.3.9/vyper/vyper_git_commithash.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-29 15:36:36.000000 vyper-0.3.9/vyper/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:36:52.976714 vyper-0.3.9/vyper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-29 15:36:52.000000 vyper-0.3.9/vyper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16239 2023-05-29 15:36:52.000000 vyper-0.3.9/vyper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 15:36:52.000000 vyper-0.3.9/vyper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-29 15:36:52.000000 vyper-0.3.9/vyper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-29 15:36:52.000000 vyper-0.3.9/vyper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 15:36:52.000000 vyper-0.3.9/vyper.egg-info/top_level.txt
```

### Comparing `vyper-0.3.8/.github/ISSUE_TEMPLATE/bug.md` & `vyper-0.3.9/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/.github/ISSUE_TEMPLATE/vip.md` & `vyper-0.3.9/.github/ISSUE_TEMPLATE/vip.md`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/.github/workflows/build.yml` & `vyper-0.3.9/.github/workflows/build.yml`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     shell: bash
 
 jobs:
   unix-build:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        os: [ubuntu-latest, macos-latest]
+        os: [ubuntu-20.04, macos-latest]
 
     steps:
       - uses: actions/checkout@v2
         with:
             # grab the commit passed in via `tag`, if any
             ref: ${{ github.event.inputs.tag }}
             # need to fetch unshallow so that setuptools_scm can infer the version
```

### Comparing `vyper-0.3.8/.github/workflows/codeql.yml` & `vyper-0.3.9/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/.github/workflows/era-tester.yml` & `vyper-0.3.9/.github/workflows/era-tester.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/.github/workflows/ghcr.yml` & `vyper-0.3.9/.github/workflows/ghcr.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/.github/workflows/publish.yml` & `vyper-0.3.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/.github/workflows/test.yml` & `vyper-0.3.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/.pre-commit-config.yaml` & `vyper-0.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/Dockerfile` & `vyper-0.3.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/LICENSE` & `vyper-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/Makefile` & `vyper-0.3.9/Makefile`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/PKG-INFO` & `vyper-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vyper
-Version: 0.3.8
+Version: 0.3.9
 Summary: Vyper: the Pythonic Programming Language for the EVM
 Home-page: https://github.com/vyperlang/vyper
 Author: Vyper Team
 Author-email: 
 License: Apache License 2.0
 Keywords: ethereum evm smart contract language
 Classifier: Intended Audience :: Developers
```

### Comparing `vyper-0.3.8/README.md` & `vyper-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/SECURITY.md` & `vyper-0.3.9/SECURITY.md`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/Makefile` & `vyper-0.3.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/_static/css/dark.css` & `vyper-0.3.9/docs/_static/css/dark.css`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/_static/css/toggle.css` & `vyper-0.3.9/docs/_static/css/toggle.css`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/_static/js/toggle.js` & `vyper-0.3.9/docs/_static/js/toggle.js`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/_templates/versions.html` & `vyper-0.3.9/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/built-in-functions.rst` & `vyper-0.3.9/docs/built-in-functions.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/compiler-exceptions.rst` & `vyper-0.3.9/docs/compiler-exceptions.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/compiling-a-contract.rst` & `vyper-0.3.9/docs/compiling-a-contract.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/conf.py` & `vyper-0.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/constants-and-vars.rst` & `vyper-0.3.9/docs/constants-and-vars.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/contributing.rst` & `vyper-0.3.9/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/control-structures.rst` & `vyper-0.3.9/docs/control-structures.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/deploying-contracts.rst` & `vyper-0.3.9/docs/deploying-contracts.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/event-logging.rst` & `vyper-0.3.9/docs/event-logging.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/index.rst` & `vyper-0.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/installing-vyper.rst` & `vyper-0.3.9/docs/installing-vyper.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/interfaces.rst` & `vyper-0.3.9/docs/interfaces.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/make.bat` & `vyper-0.3.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/natspec.rst` & `vyper-0.3.9/docs/natspec.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/release-notes.rst` & `vyper-0.3.9/docs/release-notes.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,27 @@
     to convert links to nice rst links:
     :'<,'>s/\v(https:\/\/github.com\/vyperlang\/vyper\/pull\/)(\d+)/(`#\2 <\1\2>`_)/g
     ex. in: https://github.com/vyperlang/vyper/pull/3373
     ex. out: (`#3373 <https://github.com/vyperlang/vyper/pull/3373>`_)
     for advisory links:
     :'<,'>s/\v(https:\/\/github.com\/vyperlang\/vyper\/security\/advisories\/)([-A-Za-z0-9]+)/(`\2 <\1\2>`_)/g
 
+v0.3.9 ("Common Adder")
+******
+
+Date released: 2023-05-29
+
+This is a patch release fix for v0.3.8. @bout3fiddy discovered a codesize regression for blueprint contracts in v0.3.8 which is fixed in this release. @bout3fiddy also discovered a runtime performance (gas) regression for default functions in v0.3.8 which is fixed in this release.
+
+Fixes:
+
+- initcode codesize blowup (`#3450 <https://github.com/vyperlang/vyper/pull/3450>`_)
+- add back global calldatasize check for contracts with default fn (`#3463 <https://github.com/vyperlang/vyper/pull/3463>`_)
+
+
 v0.3.8
 ******
 
 Date released: 2023-05-23
 
 Non-breaking changes and improvements:
```

### Comparing `vyper-0.3.8/docs/resources.rst` & `vyper-0.3.9/docs/resources.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/scoping-and-declarations.rst` & `vyper-0.3.9/docs/scoping-and-declarations.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/statements.rst` & `vyper-0.3.9/docs/statements.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/structure-of-a-contract.rst` & `vyper-0.3.9/docs/structure-of-a-contract.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/style-guide.rst` & `vyper-0.3.9/docs/style-guide.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/testing-contracts-brownie.rst` & `vyper-0.3.9/docs/testing-contracts-brownie.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/testing-contracts-ethtester.rst` & `vyper-0.3.9/docs/testing-contracts-ethtester.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/testing-contracts.rst` & `vyper-0.3.9/docs/testing-contracts.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/toctree.rst` & `vyper-0.3.9/docs/toctree.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/types.rst` & `vyper-0.3.9/docs/types.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/versioning.rst` & `vyper-0.3.9/docs/versioning.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/vyper-by-example.rst` & `vyper-0.3.9/docs/vyper-by-example.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/docs/vyper-logo-transparent.svg` & `vyper-0.3.9/docs/vyper-logo-transparent.svg`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/examples/auctions/blind_auction.vy` & `vyper-0.3.9/examples/auctions/blind_auction.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/examples/auctions/simple_open_auction.vy` & `vyper-0.3.9/examples/auctions/simple_open_auction.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/examples/crowdfund.vy` & `vyper-0.3.9/examples/crowdfund.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/examples/factory/Exchange.vy` & `vyper-0.3.9/examples/factory/Exchange.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/examples/factory/Factory.vy` & `vyper-0.3.9/examples/factory/Factory.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/examples/market_maker/on_chain_market_maker.vy` & `vyper-0.3.9/examples/market_maker/on_chain_market_maker.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/examples/safe_remote_purchase/safe_remote_purchase.vy` & `vyper-0.3.9/examples/safe_remote_purchase/safe_remote_purchase.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/examples/stock/company.vy` & `vyper-0.3.9/examples/stock/company.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/examples/tokens/ERC1155ownable.vy` & `vyper-0.3.9/examples/tokens/ERC1155ownable.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/examples/tokens/ERC20.vy` & `vyper-0.3.9/examples/tokens/ERC20.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/examples/tokens/ERC4626.vy` & `vyper-0.3.9/examples/tokens/ERC4626.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/examples/tokens/ERC721.vy` & `vyper-0.3.9/examples/tokens/ERC721.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/examples/voting/ballot.vy` & `vyper-0.3.9/examples/voting/ballot.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/examples/wallet/wallet.vy` & `vyper-0.3.9/examples/wallet/wallet.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/logo/vyper-logo-flat.png` & `vyper-0.3.9/logo/vyper-logo-flat.png`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/logo/vyper-logo-flat.svg` & `vyper-0.3.9/logo/vyper-logo-flat.svg`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/logo/vyper-logo-transparent.png` & `vyper-0.3.9/logo/vyper-logo-transparent.png`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/logo/vyper-logo-transparent.svg` & `vyper-0.3.9/logo/vyper-logo-transparent.svg`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/logo/vyper-logo.ai` & `vyper-0.3.9/logo/vyper-logo.ai`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/make.cmd` & `vyper-0.3.9/make.cmd`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/setup.cfg` & `vyper-0.3.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/setup.py` & `vyper-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/ast/nodes/test_compare_nodes.py` & `vyper-0.3.9/tests/ast/nodes/test_compare_nodes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/ast/nodes/test_evaluate_binop_decimal.py` & `vyper-0.3.9/tests/ast/nodes/test_evaluate_binop_decimal.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/ast/nodes/test_evaluate_binop_int.py` & `vyper-0.3.9/tests/ast/nodes/test_evaluate_binop_int.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/ast/nodes/test_evaluate_boolop.py` & `vyper-0.3.9/tests/ast/nodes/test_evaluate_boolop.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/ast/nodes/test_evaluate_compare.py` & `vyper-0.3.9/tests/ast/nodes/test_evaluate_compare.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/ast/nodes/test_evaluate_subscript.py` & `vyper-0.3.9/tests/ast/nodes/test_evaluate_subscript.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/ast/nodes/test_evaluate_unaryop.py` & `vyper-0.3.9/tests/ast/nodes/test_evaluate_unaryop.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/ast/nodes/test_from_node.py` & `vyper-0.3.9/tests/ast/nodes/test_from_node.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/ast/nodes/test_get_children.py` & `vyper-0.3.9/tests/ast/nodes/test_get_children.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/ast/nodes/test_get_descendants.py` & `vyper-0.3.9/tests/ast/nodes/test_get_descendants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/ast/nodes/test_hex.py` & `vyper-0.3.9/tests/ast/nodes/test_hex.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/ast/nodes/test_replace_in_tree.py` & `vyper-0.3.9/tests/ast/nodes/test_replace_in_tree.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/ast/test_folding.py` & `vyper-0.3.9/tests/ast/test_folding.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/ast/test_natspec.py` & `vyper-0.3.9/tests/ast/test_natspec.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/ast/test_pre_parser.py` & `vyper-0.3.9/tests/ast/test_pre_parser.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/base_conftest.py` & `vyper-0.3.9/tests/base_conftest.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/builtins/folding/test_abs.py` & `vyper-0.3.9/tests/builtins/folding/test_abs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/builtins/folding/test_addmod_mulmod.py` & `vyper-0.3.9/tests/builtins/folding/test_addmod_mulmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/builtins/folding/test_bitwise.py` & `vyper-0.3.9/tests/builtins/folding/test_bitwise.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/builtins/folding/test_epsilon.py` & `vyper-0.3.9/tests/builtins/folding/test_epsilon.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/builtins/folding/test_floor_ceil.py` & `vyper-0.3.9/tests/builtins/folding/test_floor_ceil.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/builtins/folding/test_fold_as_wei_value.py` & `vyper-0.3.9/tests/builtins/folding/test_fold_as_wei_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/builtins/folding/test_keccak_sha.py` & `vyper-0.3.9/tests/builtins/folding/test_keccak_sha.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/builtins/folding/test_len.py` & `vyper-0.3.9/tests/builtins/folding/test_len.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/builtins/folding/test_min_max.py` & `vyper-0.3.9/tests/builtins/folding/test_min_max.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/builtins/folding/test_powmod.py` & `vyper-0.3.9/tests/builtins/folding/test_powmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/cli/outputs/test_storage_layout.py` & `vyper-0.3.9/tests/cli/outputs/test_storage_layout.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/cli/outputs/test_storage_layout_overrides.py` & `vyper-0.3.9/tests/cli/outputs/test_storage_layout_overrides.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/cli/vyper_compile/test_compile_files.py` & `vyper-0.3.9/tests/cli/vyper_compile/test_compile_files.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/cli/vyper_compile/test_import_paths.py` & `vyper-0.3.9/tests/cli/vyper_compile/test_import_paths.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/cli/vyper_compile/test_parse_args.py` & `vyper-0.3.9/tests/cli/vyper_compile/test_parse_args.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/cli/vyper_json/test_compile_from_input_dict.py` & `vyper-0.3.9/tests/cli/vyper_json/test_compile_from_input_dict.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/cli/vyper_json/test_compile_json.py` & `vyper-0.3.9/tests/cli/vyper_json/test_compile_json.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/cli/vyper_json/test_get_contracts.py` & `vyper-0.3.9/tests/cli/vyper_json/test_get_contracts.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/cli/vyper_json/test_get_settings.py` & `vyper-0.3.9/tests/cli/vyper_json/test_get_settings.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/cli/vyper_json/test_interfaces.py` & `vyper-0.3.9/tests/cli/vyper_json/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/cli/vyper_json/test_output_dict.py` & `vyper-0.3.9/tests/cli/vyper_json/test_output_dict.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/cli/vyper_json/test_output_selection.py` & `vyper-0.3.9/tests/cli/vyper_json/test_output_selection.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/cli/vyper_json/test_parse_args_vyperjson.py` & `vyper-0.3.9/tests/cli/vyper_json/test_parse_args_vyperjson.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/compiler/ir/test_compile_ir.py` & `vyper-0.3.9/tests/compiler/ir/test_compile_ir.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/compiler/ir/test_optimize_ir.py` & `vyper-0.3.9/tests/compiler/ir/test_optimize_ir.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/compiler/ir/test_with.py` & `vyper-0.3.9/tests/compiler/ir/test_with.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/compiler/test_compile_code.py` & `vyper-0.3.9/tests/compiler/test_compile_code.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/compiler/test_opcodes.py` & `vyper-0.3.9/tests/compiler/test_opcodes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/compiler/test_pre_parser.py` & `vyper-0.3.9/tests/compiler/test_pre_parser.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/compiler/test_sha3_32.py` & `vyper-0.3.9/tests/compiler/test_sha3_32.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/compiler/test_source_map.py` & `vyper-0.3.9/tests/compiler/test_source_map.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/conftest.py` & `vyper-0.3.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/examples/auctions/test_blind_auction.py` & `vyper-0.3.9/tests/examples/auctions/test_blind_auction.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/examples/auctions/test_simple_open_auction.py` & `vyper-0.3.9/tests/examples/auctions/test_simple_open_auction.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/examples/company/test_company.py` & `vyper-0.3.9/tests/examples/company/test_company.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/examples/crowdfund/test_crowdfund_example.py` & `vyper-0.3.9/tests/examples/crowdfund/test_crowdfund_example.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/examples/factory/test_factory.py` & `vyper-0.3.9/tests/examples/factory/test_factory.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/examples/market_maker/test_on_chain_market_maker.py` & `vyper-0.3.9/tests/examples/market_maker/test_on_chain_market_maker.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/examples/safe_remote_purchase/test_safe_remote_purchase.py` & `vyper-0.3.9/tests/examples/safe_remote_purchase/test_safe_remote_purchase.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/examples/storage/test_advanced_storage.py` & `vyper-0.3.9/tests/examples/storage/test_advanced_storage.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/examples/storage/test_storage.py` & `vyper-0.3.9/tests/examples/storage/test_storage.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/examples/tokens/test_erc1155.py` & `vyper-0.3.9/tests/examples/tokens/test_erc1155.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/examples/tokens/test_erc20.py` & `vyper-0.3.9/tests/examples/tokens/test_erc20.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/examples/tokens/test_erc4626.py` & `vyper-0.3.9/tests/examples/tokens/test_erc4626.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/examples/tokens/test_erc721.py` & `vyper-0.3.9/tests/examples/tokens/test_erc721.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/examples/voting/test_ballot.py` & `vyper-0.3.9/tests/examples/voting/test_ballot.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/examples/wallet/test_wallet.py` & `vyper-0.3.9/tests/examples/wallet/test_wallet.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/fixtures/memorymock.py` & `vyper-0.3.9/tests/fixtures/memorymock.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/functional/codegen/test_struct_return.py` & `vyper-0.3.9/tests/functional/codegen/test_struct_return.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/functional/codegen/test_tuple_return.py` & `vyper-0.3.9/tests/functional/codegen/test_tuple_return.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/functional/semantics/analysis/test_array_index.py` & `vyper-0.3.9/tests/functional/semantics/analysis/test_array_index.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/functional/semantics/analysis/test_cyclic_function_calls.py` & `vyper-0.3.9/tests/functional/semantics/analysis/test_cyclic_function_calls.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/functional/semantics/analysis/test_for_loop.py` & `vyper-0.3.9/tests/functional/semantics/analysis/test_for_loop.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/functional/semantics/analysis/test_potential_types.py` & `vyper-0.3.9/tests/functional/semantics/analysis/test_potential_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/functional/semantics/conftest.py` & `vyper-0.3.9/tests/functional/semantics/conftest.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/functional/semantics/test_namespace.py` & `vyper-0.3.9/tests/functional/semantics/test_namespace.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/functional/semantics/types/test_event.py` & `vyper-0.3.9/tests/functional/semantics/types/test_event.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/functional/semantics/types/test_pure_types.py` & `vyper-0.3.9/tests/functional/semantics/types/test_pure_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/functional/semantics/types/test_size_in_bytes.py` & `vyper-0.3.9/tests/functional/semantics/types/test_size_in_bytes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/functional/semantics/types/test_type_from_abi.py` & `vyper-0.3.9/tests/functional/semantics/types/test_type_from_abi.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/functional/semantics/types/test_type_from_annotation.py` & `vyper-0.3.9/tests/functional/semantics/types/test_type_from_annotation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/functional/test_storage_slots.py` & `vyper-0.3.9/tests/functional/test_storage_slots.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/fuzzing/test_exponents.py` & `vyper-0.3.9/tests/fuzzing/test_exponents.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/grammar/test_grammar.py` & `vyper-0.3.9/tests/grammar/test_grammar.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/ast_utils/test_ast.py` & `vyper-0.3.9/tests/parser/ast_utils/test_ast.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/ast_utils/test_ast_dict.py` & `vyper-0.3.9/tests/parser/ast_utils/test_ast_dict.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/exceptions/test_argument_exception.py` & `vyper-0.3.9/tests/parser/exceptions/test_argument_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/exceptions/test_call_violation.py` & `vyper-0.3.9/tests/parser/exceptions/test_call_violation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/exceptions/test_constancy_exception.py` & `vyper-0.3.9/tests/parser/exceptions/test_constancy_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/exceptions/test_function_declaration_exception.py` & `vyper-0.3.9/tests/parser/exceptions/test_function_declaration_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/exceptions/test_instantiation_exception.py` & `vyper-0.3.9/tests/parser/exceptions/test_instantiation_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/exceptions/test_invalid_literal_exception.py` & `vyper-0.3.9/tests/parser/exceptions/test_invalid_literal_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/exceptions/test_invalid_payable.py` & `vyper-0.3.9/tests/parser/exceptions/test_invalid_payable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/exceptions/test_invalid_reference.py` & `vyper-0.3.9/tests/parser/exceptions/test_invalid_reference.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/exceptions/test_invalid_type_exception.py` & `vyper-0.3.9/tests/parser/exceptions/test_invalid_type_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/exceptions/test_namespace_collision.py` & `vyper-0.3.9/tests/parser/exceptions/test_namespace_collision.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/exceptions/test_overflow_exception.py` & `vyper-0.3.9/tests/parser/exceptions/test_overflow_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/exceptions/test_structure_exception.py` & `vyper-0.3.9/tests/parser/exceptions/test_structure_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/exceptions/test_syntax_exception.py` & `vyper-0.3.9/tests/parser/exceptions/test_syntax_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/exceptions/test_type_mismatch_exception.py` & `vyper-0.3.9/tests/parser/exceptions/test_type_mismatch_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/exceptions/test_undeclared_definition.py` & `vyper-0.3.9/tests/parser/exceptions/test_undeclared_definition.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/exceptions/test_variable_declaration_exception.py` & `vyper-0.3.9/tests/parser/exceptions/test_variable_declaration_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/exceptions/test_vyper_exception_pos.py` & `vyper-0.3.9/tests/parser/exceptions/test_vyper_exception_pos.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/arithmetic/test_division.py` & `vyper-0.3.9/tests/parser/features/arithmetic/test_division.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/arithmetic/test_modulo.py` & `vyper-0.3.9/tests/parser/features/arithmetic/test_modulo.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/decorators/test_nonreentrant.py` & `vyper-0.3.9/tests/parser/features/decorators/test_nonreentrant.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/decorators/test_payable.py` & `vyper-0.3.9/tests/parser/features/decorators/test_payable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/decorators/test_private.py` & `vyper-0.3.9/tests/parser/features/decorators/test_private.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/decorators/test_public.py` & `vyper-0.3.9/tests/parser/features/decorators/test_public.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/decorators/test_pure.py` & `vyper-0.3.9/tests/parser/features/decorators/test_pure.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/decorators/test_view.py` & `vyper-0.3.9/tests/parser/features/decorators/test_view.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/external_contracts/test_erc20_abi.py` & `vyper-0.3.9/tests/parser/features/external_contracts/test_erc20_abi.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/external_contracts/test_external_contract_calls.py` & `vyper-0.3.9/tests/parser/features/external_contracts/test_external_contract_calls.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/external_contracts/test_modifiable_external_contract_calls.py` & `vyper-0.3.9/tests/parser/features/external_contracts/test_modifiable_external_contract_calls.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/external_contracts/test_self_call_struct.py` & `vyper-0.3.9/tests/parser/features/external_contracts/test_self_call_struct.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/iteration/test_break.py` & `vyper-0.3.9/tests/parser/features/iteration/test_break.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/iteration/test_continue.py` & `vyper-0.3.9/tests/parser/features/iteration/test_continue.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/iteration/test_for_in_list.py` & `vyper-0.3.9/tests/parser/features/iteration/test_for_in_list.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/iteration/test_for_range.py` & `vyper-0.3.9/tests/parser/features/iteration/test_for_range.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/iteration/test_range_in.py` & `vyper-0.3.9/tests/parser/features/iteration/test_range_in.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/test_assert.py` & `vyper-0.3.9/tests/parser/features/test_assert.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/test_assert_unreachable.py` & `vyper-0.3.9/tests/parser/features/test_assert_unreachable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/test_assignment.py` & `vyper-0.3.9/tests/parser/features/test_assignment.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/test_bytes_map_keys.py` & `vyper-0.3.9/tests/parser/features/test_bytes_map_keys.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/test_clampers.py` & `vyper-0.3.9/tests/parser/features/test_clampers.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/test_comparison.py` & `vyper-0.3.9/tests/parser/features/test_comparison.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/test_conditionals.py` & `vyper-0.3.9/tests/parser/features/test_conditionals.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/test_constructor.py` & `vyper-0.3.9/tests/parser/features/test_constructor.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/test_immutable.py` & `vyper-0.3.9/tests/parser/features/test_immutable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/test_init.py` & `vyper-0.3.9/tests/parser/features/test_init.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/test_internal_call.py` & `vyper-0.3.9/tests/parser/features/test_internal_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/test_logging.py` & `vyper-0.3.9/tests/parser/features/test_logging.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/test_logging_bytes_extended.py` & `vyper-0.3.9/tests/parser/features/test_logging_bytes_extended.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/test_logging_from_call.py` & `vyper-0.3.9/tests/parser/features/test_logging_from_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/test_memory_dealloc.py` & `vyper-0.3.9/tests/parser/features/test_memory_dealloc.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/test_packing.py` & `vyper-0.3.9/tests/parser/features/test_packing.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/test_reverting.py` & `vyper-0.3.9/tests/parser/features/test_reverting.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/test_short_circuiting.py` & `vyper-0.3.9/tests/parser/features/test_short_circuiting.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/test_string_map_keys.py` & `vyper-0.3.9/tests/parser/features/test_string_map_keys.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/test_ternary.py` & `vyper-0.3.9/tests/parser/features/test_ternary.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/features/test_transient.py` & `vyper-0.3.9/tests/parser/features/test_transient.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_abi.py` & `vyper-0.3.9/tests/parser/functions/test_abi.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_abi_decode.py` & `vyper-0.3.9/tests/parser/functions/test_abi_decode.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_abi_encode.py` & `vyper-0.3.9/tests/parser/functions/test_abi_encode.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_addmod.py` & `vyper-0.3.9/tests/parser/functions/test_addmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_as_wei_value.py` & `vyper-0.3.9/tests/parser/functions/test_as_wei_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_bitwise.py` & `vyper-0.3.9/tests/parser/functions/test_bitwise.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_block.py` & `vyper-0.3.9/tests/parser/functions/test_block.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_ceil.py` & `vyper-0.3.9/tests/parser/functions/test_ceil.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_concat.py` & `vyper-0.3.9/tests/parser/functions/test_concat.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_convert.py` & `vyper-0.3.9/tests/parser/functions/test_convert.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_create_functions.py` & `vyper-0.3.9/tests/parser/functions/test_create_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import pytest
 import rlp
 from eth.codecs import abi
 from hexbytes import HexBytes
 
+import vyper.ir.compile_ir as compile_ir
+from vyper.codegen.ir_node import IRnode
 from vyper.utils import EIP_170_LIMIT, checksum_encode, keccak256
 
 
 # initcode used by create_minimal_proxy_to
 def eip1167_initcode(_addr):
     addr = HexBytes(_addr)
     pre = HexBytes("0x602D3D8160093D39F3363d3d373d3d3d363d73")
@@ -220,23 +222,31 @@
     BLUEPRINT = blueprint_address
 
 @external
 def test(code_ofst: uint256) -> address:
     return create_from_blueprint(BLUEPRINT, code_offset=code_ofst)
     """
 
-    # use a bunch of JUMPDEST + STOP instructions as blueprint code
-    # (as any STOP instruction returns valid code, split up with
-    # jumpdests as optimization fence)
     initcode_len = 100
-    f = get_contract_from_ir(["deploy", 0, ["seq"] + ["jumpdest", "stop"] * (initcode_len // 2), 0])
-    blueprint_code = w3.eth.get_code(f.address)
-    print(blueprint_code)
 
-    d = get_contract(deployer_code, f.address)
+    # deploy a blueprint contract whose contained initcode contains only
+    # zeroes (so no matter which offset, create_from_blueprint will
+    # return empty code)
+    ir = IRnode.from_list(["deploy", 0, ["seq"] + ["stop"] * initcode_len, 0])
+    bytecode, _ = compile_ir.assembly_to_evm(compile_ir.compile_to_assembly(ir, no_optimize=True))
+    # manually deploy the bytecode
+    c = w3.eth.contract(abi=[], bytecode=bytecode)
+    deploy_transaction = c.constructor()
+    tx_info = {"from": w3.eth.accounts[0], "value": 0, "gasPrice": 0}
+    tx_hash = deploy_transaction.transact(tx_info)
+    blueprint_address = w3.eth.get_transaction_receipt(tx_hash)["contractAddress"]
+    blueprint_code = w3.eth.get_code(blueprint_address)
+    print("BLUEPRINT CODE:", blueprint_code)
+
+    d = get_contract(deployer_code, blueprint_address)
 
     # deploy with code_ofst=0 fine
     d.test(0)
 
     # deploy with code_ofst=len(blueprint) - 1 fine
     d.test(initcode_len - 1)
```

### Comparing `vyper-0.3.8/tests/parser/functions/test_default_function.py` & `vyper-0.3.9/tests/parser/functions/test_default_function.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_default_parameters.py` & `vyper-0.3.9/tests/parser/functions/test_default_parameters.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_ec.py` & `vyper-0.3.9/tests/parser/functions/test_ec.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_ecrecover.py` & `vyper-0.3.9/tests/parser/functions/test_ecrecover.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_empty.py` & `vyper-0.3.9/tests/parser/functions/test_empty.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_extract32.py` & `vyper-0.3.9/tests/parser/functions/test_extract32.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_floor.py` & `vyper-0.3.9/tests/parser/functions/test_floor.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_interfaces.py` & `vyper-0.3.9/tests/parser/functions/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_is_contract.py` & `vyper-0.3.9/tests/parser/functions/test_is_contract.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_keccak256.py` & `vyper-0.3.9/tests/parser/functions/test_keccak256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_length.py` & `vyper-0.3.9/tests/parser/functions/test_length.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_method_id.py` & `vyper-0.3.9/tests/parser/functions/test_method_id.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_minmax.py` & `vyper-0.3.9/tests/parser/functions/test_minmax.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_minmax_value.py` & `vyper-0.3.9/tests/parser/functions/test_minmax_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_mkstr.py` & `vyper-0.3.9/tests/parser/functions/test_mkstr.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_mulmod.py` & `vyper-0.3.9/tests/parser/functions/test_mulmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_raw_call.py` & `vyper-0.3.9/tests/parser/functions/test_raw_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_return.py` & `vyper-0.3.9/tests/parser/functions/test_return.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_return_struct.py` & `vyper-0.3.9/tests/parser/functions/test_return_struct.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_return_tuple.py` & `vyper-0.3.9/tests/parser/functions/test_return_tuple.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_send.py` & `vyper-0.3.9/tests/parser/functions/test_send.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_sha256.py` & `vyper-0.3.9/tests/parser/functions/test_sha256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_slice.py` & `vyper-0.3.9/tests/parser/functions/test_slice.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_unary.py` & `vyper-0.3.9/tests/parser/functions/test_unary.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/functions/test_unsafe_math.py` & `vyper-0.3.9/tests/parser/functions/test_unsafe_math.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/globals/test_getters.py` & `vyper-0.3.9/tests/parser/globals/test_getters.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/globals/test_globals.py` & `vyper-0.3.9/tests/parser/globals/test_globals.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/globals/test_setters.py` & `vyper-0.3.9/tests/parser/globals/test_setters.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/integration/test_crowdfund.py` & `vyper-0.3.9/tests/parser/integration/test_crowdfund.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/integration/test_escrow.py` & `vyper-0.3.9/tests/parser/integration/test_escrow.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/parser_utils/test_annotate_and_optimize_ast.py` & `vyper-0.3.9/tests/parser/parser_utils/test_annotate_and_optimize_ast.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_abi_encode.py` & `vyper-0.3.9/tests/parser/syntax/test_abi_encode.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_address_code.py` & `vyper-0.3.9/tests/parser/syntax/test_address_code.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_ann_assign.py` & `vyper-0.3.9/tests/parser/syntax/test_ann_assign.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_as_uint256.py` & `vyper-0.3.9/tests/parser/syntax/test_as_uint256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_as_wei_value.py` & `vyper-0.3.9/tests/parser/syntax/test_as_wei_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_block.py` & `vyper-0.3.9/tests/parser/syntax/test_block.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_blockscope.py` & `vyper-0.3.9/tests/parser/syntax/test_blockscope.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_bool.py` & `vyper-0.3.9/tests/parser/syntax/test_bool.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_bool_ops.py` & `vyper-0.3.9/tests/parser/syntax/test_bool_ops.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_bytes.py` & `vyper-0.3.9/tests/parser/syntax/test_bytes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_chainid.py` & `vyper-0.3.9/tests/parser/syntax/test_chainid.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_code_size.py` & `vyper-0.3.9/tests/parser/syntax/test_code_size.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_codehash.py` & `vyper-0.3.9/tests/parser/syntax/test_codehash.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_concat.py` & `vyper-0.3.9/tests/parser/syntax/test_concat.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_constants.py` & `vyper-0.3.9/tests/parser/syntax/test_constants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_create_with_code_of.py` & `vyper-0.3.9/tests/parser/syntax/test_create_with_code_of.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_dynamic_array.py` & `vyper-0.3.9/tests/parser/syntax/test_dynamic_array.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_enum.py` & `vyper-0.3.9/tests/parser/syntax/test_enum.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_extract32.py` & `vyper-0.3.9/tests/parser/syntax/test_extract32.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_for_range.py` & `vyper-0.3.9/tests/parser/syntax/test_for_range.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_functions_call.py` & `vyper-0.3.9/tests/parser/syntax/test_functions_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_immutables.py` & `vyper-0.3.9/tests/parser/syntax/test_immutables.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_interfaces.py` & `vyper-0.3.9/tests/parser/syntax/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_invalids.py` & `vyper-0.3.9/tests/parser/syntax/test_invalids.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_keccak256.py` & `vyper-0.3.9/tests/parser/syntax/test_keccak256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_len.py` & `vyper-0.3.9/tests/parser/syntax/test_len.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_list.py` & `vyper-0.3.9/tests/parser/syntax/test_list.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_logging.py` & `vyper-0.3.9/tests/parser/syntax/test_logging.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_minmax.py` & `vyper-0.3.9/tests/parser/syntax/test_minmax.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_msg_data.py` & `vyper-0.3.9/tests/parser/syntax/test_msg_data.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_nested_list.py` & `vyper-0.3.9/tests/parser/syntax/test_nested_list.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_no_none.py` & `vyper-0.3.9/tests/parser/syntax/test_no_none.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_print.py` & `vyper-0.3.9/tests/parser/syntax/test_print.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_public.py` & `vyper-0.3.9/tests/parser/syntax/test_public.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_raw_call.py` & `vyper-0.3.9/tests/parser/syntax/test_raw_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_return_tuple.py` & `vyper-0.3.9/tests/parser/syntax/test_return_tuple.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_self_balance.py` & `vyper-0.3.9/tests/parser/syntax/test_self_balance.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_selfdestruct.py` & `vyper-0.3.9/tests/parser/syntax/test_selfdestruct.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_send.py` & `vyper-0.3.9/tests/parser/syntax/test_send.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_slice.py` & `vyper-0.3.9/tests/parser/syntax/test_slice.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_string.py` & `vyper-0.3.9/tests/parser/syntax/test_string.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_structs.py` & `vyper-0.3.9/tests/parser/syntax/test_structs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_ternary.py` & `vyper-0.3.9/tests/parser/syntax/test_ternary.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_tuple_assign.py` & `vyper-0.3.9/tests/parser/syntax/test_tuple_assign.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/test_unbalanced_return.py` & `vyper-0.3.9/tests/parser/syntax/test_unbalanced_return.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/utils/test_event_names.py` & `vyper-0.3.9/tests/parser/syntax/utils/test_event_names.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/utils/test_function_names.py` & `vyper-0.3.9/tests/parser/syntax/utils/test_function_names.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/syntax/utils/test_variable_names.py` & `vyper-0.3.9/tests/parser/syntax/utils/test_variable_names.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/test_call_graph_stability.py` & `vyper-0.3.9/tests/parser/test_call_graph_stability.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/types/numbers/test_constants.py` & `vyper-0.3.9/tests/parser/types/numbers/test_constants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/types/numbers/test_decimals.py` & `vyper-0.3.9/tests/parser/types/numbers/test_decimals.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/types/numbers/test_isqrt.py` & `vyper-0.3.9/tests/parser/types/numbers/test_isqrt.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/types/numbers/test_signed_ints.py` & `vyper-0.3.9/tests/parser/types/numbers/test_signed_ints.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/types/numbers/test_sqrt.py` & `vyper-0.3.9/tests/parser/types/numbers/test_sqrt.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/types/numbers/test_unsigned_ints.py` & `vyper-0.3.9/tests/parser/types/numbers/test_unsigned_ints.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/types/test_bytes.py` & `vyper-0.3.9/tests/parser/types/test_bytes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/types/test_bytes_literal.py` & `vyper-0.3.9/tests/parser/types/test_bytes_literal.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/types/test_bytes_zero_padding.py` & `vyper-0.3.9/tests/parser/types/test_bytes_zero_padding.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/types/test_dynamic_array.py` & `vyper-0.3.9/tests/parser/types/test_dynamic_array.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/types/test_enum.py` & `vyper-0.3.9/tests/parser/types/test_enum.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/types/test_identifier_naming.py` & `vyper-0.3.9/tests/parser/types/test_identifier_naming.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/types/test_lists.py` & `vyper-0.3.9/tests/parser/types/test_lists.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/types/test_node_types.py` & `vyper-0.3.9/tests/parser/types/test_node_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/types/test_string.py` & `vyper-0.3.9/tests/parser/types/test_string.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/types/test_string_literal.py` & `vyper-0.3.9/tests/parser/types/test_string_literal.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/parser/types/value/test_as_wei_value.py` & `vyper-0.3.9/tests/parser/types/value/test_as_wei_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/signatures/test_method_id_conflicts.py` & `vyper-0.3.9/tests/signatures/test_method_id_conflicts.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tests/test_utils.py` & `vyper-0.3.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/tox.ini` & `vyper-0.3.9/tox.ini`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/__init__.py` & `vyper-0.3.9/vyper/__init__.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/__main__.py` & `vyper-0.3.9/vyper/__main__.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/abi_types.py` & `vyper-0.3.9/vyper/abi_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/ast/README.md` & `vyper-0.3.9/vyper/ast/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/ast/annotation.py` & `vyper-0.3.9/vyper/ast/annotation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/ast/expansion.py` & `vyper-0.3.9/vyper/ast/expansion.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/ast/folding.py` & `vyper-0.3.9/vyper/ast/folding.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/ast/grammar.lark` & `vyper-0.3.9/vyper/ast/grammar.lark`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/ast/grammar.py` & `vyper-0.3.9/vyper/ast/grammar.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/ast/metadata.py` & `vyper-0.3.9/vyper/ast/metadata.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/ast/natspec.py` & `vyper-0.3.9/vyper/ast/natspec.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/ast/nodes.py` & `vyper-0.3.9/vyper/ast/nodes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/ast/nodes.pyi` & `vyper-0.3.9/vyper/ast/nodes.pyi`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/ast/pre_parser.py` & `vyper-0.3.9/vyper/ast/pre_parser.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/ast/utils.py` & `vyper-0.3.9/vyper/ast/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/ast/validation.py` & `vyper-0.3.9/vyper/ast/validation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/builtins/_convert.py` & `vyper-0.3.9/vyper/builtins/_convert.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/builtins/_signatures.py` & `vyper-0.3.9/vyper/builtins/_signatures.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/builtins/_utils.py` & `vyper-0.3.9/vyper/builtins/_utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/builtins/functions.py` & `vyper-0.3.9/vyper/builtins/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1243,15 +1243,17 @@
     _return_type = None
 
     @process_inputs
     def build_IR(self, expr, args, kwargs, context):
         to, value = args
         gas = kwargs["gas"]
         context.check_is_not_constant("send ether", expr)
-        return IRnode.from_list(["assert", ["call", gas, to, value, 0, 0, 0, 0]])
+        return IRnode.from_list(
+            ["assert", ["call", gas, to, value, 0, 0, 0, 0]], error_msg="send failed"
+        )
 
 
 class SelfDestruct(BuiltinFunction):
     _id = "selfdestruct"
     _inputs = [("to", AddressT())]
     _return_type = None
     _is_terminus = True
```

### Comparing `vyper-0.3.8/vyper/builtins/interfaces/ERC20.py` & `vyper-0.3.9/vyper/builtins/interfaces/ERC20.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/builtins/interfaces/ERC4626.py` & `vyper-0.3.9/vyper/builtins/interfaces/ERC4626.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/builtins/interfaces/ERC721.py` & `vyper-0.3.9/vyper/builtins/interfaces/ERC721.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/cli/utils.py` & `vyper-0.3.9/vyper/cli/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/cli/vyper_compile.py` & `vyper-0.3.9/vyper/cli/vyper_compile.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/cli/vyper_ir.py` & `vyper-0.3.9/vyper/cli/vyper_ir.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/cli/vyper_json.py` & `vyper-0.3.9/vyper/cli/vyper_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -425,15 +425,15 @@
             if "bytecode_runtime" in data:
                 evm["object"] = data["bytecode_runtime"]
             if "opcodes_runtime" in data:
                 evm["opcodes"] = data["opcodes_runtime"]
             if "source_map" in data:
                 evm["sourceMap"] = data["source_map"]["pc_pos_map_compressed"]
             if "source_map_full" in data:
-                evm["sourceMapFull"] = data["source_map"]
+                evm["sourceMapFull"] = data["source_map_full"]
 
     return output_dict
 
 
 # https://stackoverflow.com/a/49518779
 def _raise_on_duplicate_keys(ordered_pairs: List[Tuple[Hashable, Any]]) -> Dict:
     """
```

### Comparing `vyper-0.3.8/vyper/cli/vyper_serve.py` & `vyper-0.3.9/vyper/cli/vyper_serve.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/codegen/abi_encoder.py` & `vyper-0.3.9/vyper/codegen/abi_encoder.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/codegen/arithmetic.py` & `vyper-0.3.9/vyper/codegen/arithmetic.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/codegen/context.py` & `vyper-0.3.9/vyper/codegen/context.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/codegen/core.py` & `vyper-0.3.9/vyper/codegen/core.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/codegen/events.py` & `vyper-0.3.9/vyper/codegen/events.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/codegen/expr.py` & `vyper-0.3.9/vyper/codegen/expr.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/codegen/external_call.py` & `vyper-0.3.9/vyper/codegen/external_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/codegen/function_definitions/common.py` & `vyper-0.3.9/vyper/codegen/function_definitions/common.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/codegen/function_definitions/external_function.py` & `vyper-0.3.9/vyper/codegen/function_definitions/external_function.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,16 +85,15 @@
         ret = ["seq"]
 
         # ensure calldata is at least of minimum length
         args_abi_t = calldata_args_t.abi_type
         calldata_min_size = args_abi_t.min_size() + 4
 
         # note we don't need the check if calldata_min_size == 4,
-        # because the selector checks later in this routine ensure
-        # that calldatasize >= 4.
+        # because the global calldatasize check ensures that already.
         if calldata_min_size > 4:
             ret.append(["assert", ["ge", "calldatasize", calldata_min_size]])
 
         # TODO optimize make_setter by using
         # TupleT(list(arg.typ for arg in calldata_kwargs + default_kwargs))
         # (must ensure memory area is contiguous)
 
@@ -121,36 +120,14 @@
             copy_arg = make_setter(lhs, rhs)
             copy_arg.source_pos = getpos(x.ast_source)
             ret.append(copy_arg)
 
         ret.append(["goto", func_t._ir_info.external_function_base_entry_label])
 
         method_id_check = ["eq", "_calldata_method_id", method_id]
-
-        # if there is a function whose selector is 0 or has trailing 0s, it
-        # might not be distinguished from the case where insufficient calldata
-        # is supplied, b/c calldataload loads 0s past the end of physical
-        # calldata (cf. yellow paper).
-        # since the expected behavior of supplying insufficient calldata
-        # is to trigger the fallback fn, we add to the selector check that
-        # calldatasize >= 4, which distinguishes any selector with trailing
-        # 0 bytes from the fallback function "selector" (equiv. to "all
-        # selectors not in the selector table").
-        #
-        # note that the inclusion of this check means that, we are always
-        # guaranteed that the calldata is at least 4 bytes - either we have
-        # the explicit `calldatasize >= 4` condition in the selector check,
-        # or there are no trailing zeroes in the selector, (so the selector
-        # is impossible to match without calldatasize being at least 4).
-        method_id_bytes = util.method_id(abi_sig)
-        assert len(method_id_bytes) == 4
-        has_trailing_zeroes = method_id_bytes.endswith(b"\x00")
-        if has_trailing_zeroes:
-            method_id_check = ["and", ["ge", "calldatasize", 4], method_id_check]
-
         ret = ["if", method_id_check, ret]
         return ret
 
     ret = ["seq"]
 
     keyword_args = func_t.keyword_args
 
@@ -196,15 +173,18 @@
     # once optional args have been handled,
     # generate the main body of the function
     body += handle_base_args
 
     if not func_t.is_payable and not skip_nonpayable_check:
         # if the contract contains payable functions, but this is not one of them
         # add an assertion that the value of the call is zero
-        body += [["assert", ["iszero", "callvalue"]]]
+        nonpayable_check = IRnode.from_list(
+            ["assert", ["iszero", "callvalue"]], error_msg="nonpayable check"
+        )
+        body.append(nonpayable_check)
 
     body += nonreentrant_pre
 
     body += [parse_body(code.body, context, ensure_terminated=True)]
 
     # wrap the body in labeled block
     body = ["label", func_t._ir_info.external_function_base_entry_label, ["var_list"], body]
```

### Comparing `vyper-0.3.8/vyper/codegen/function_definitions/internal_function.py` & `vyper-0.3.9/vyper/codegen/function_definitions/internal_function.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/codegen/function_definitions/utils.py` & `vyper-0.3.9/vyper/codegen/function_definitions/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/codegen/global_context.py` & `vyper-0.3.9/vyper/codegen/global_context.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/codegen/ir_node.py` & `vyper-0.3.9/vyper/codegen/ir_node.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/codegen/keccak256_helper.py` & `vyper-0.3.9/vyper/codegen/keccak256_helper.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/codegen/memory_allocator.py` & `vyper-0.3.9/vyper/codegen/memory_allocator.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/codegen/module.py` & `vyper-0.3.9/vyper/codegen/module.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,41 +93,48 @@
     selector_section = ["seq"]
 
     for func_ast in payables:
         func_ir = generate_ir_for_function(func_ast, global_ctx, False)
         selector_section.append(func_ir)
 
     if batch_payable_check:
-        selector_section.append(["assert", ["iszero", "callvalue"]])
+        nonpayable_check = IRnode.from_list(
+            ["assert", ["iszero", "callvalue"]], error_msg="nonpayable check"
+        )
+        selector_section.append(nonpayable_check)
 
     for func_ast in nonpayables:
         func_ir = generate_ir_for_function(func_ast, global_ctx, skip_nonpayable_check)
         selector_section.append(func_ir)
 
     if default_function:
-        fallback_ir = generate_ir_for_function(default_function, global_ctx, skip_nonpayable_check)
+        fallback_ir = generate_ir_for_function(
+            default_function, global_ctx, skip_nonpayable_check=False
+        )
     else:
         fallback_ir = IRnode.from_list(
             ["revert", 0, 0], annotation="Default function", error_msg="fallback function"
         )
 
     # ensure the external jumptable section gets closed out
     # (for basic block hygiene and also for zksync interpreter)
     # NOTE: this jump gets optimized out in assembly since the
     # fallback label is the immediate next instruction,
     close_selector_section = ["goto", "fallback"]
 
+    global_calldatasize_check = ["if", ["lt", "calldatasize", 4], ["goto", "fallback"]]
+
     runtime = [
         "seq",
+        global_calldatasize_check,
         ["with", "_calldata_method_id", shr(224, ["calldataload", 0]), selector_section],
         close_selector_section,
         ["label", "fallback", ["var_list"], fallback_ir],
     ]
 
-    # note: dead code eliminator will clean dead functions
     runtime.extend(internal_functions_ir)
 
     return runtime
 
 
 # take a GlobalContext, and generate the runtime and deploy IR
 def generate_ir_for_module(global_ctx: GlobalContext) -> tuple[IRnode, IRnode]:
@@ -174,18 +181,22 @@
         deploy_code.append(init_func_ir)
 
         deploy_code.append(["deploy", init_mem_used, runtime, immutables_len])
 
         # internal functions come after everything else
         internal_functions = [f for f in runtime_functions if _is_internal(f)]
         for f in internal_functions:
+            init_func_t = init_function._metadata["type"]
+            if f.name not in init_func_t.recursive_calls:
+                # unreachable
+                continue
+
             func_ir = generate_ir_for_function(
                 f, global_ctx, skip_nonpayable_check=False, is_ctor_context=True
             )
-            # note: we depend on dead code eliminator to clean dead function defs
             deploy_code.append(func_ir)
 
     else:
         if immutables_len != 0:
             raise CompilerPanic("unreachable")
         deploy_code.append(["deploy", 0, runtime, 0])
```

### Comparing `vyper-0.3.8/vyper/codegen/return_.py` & `vyper-0.3.9/vyper/codegen/return_.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/codegen/self_call.py` & `vyper-0.3.9/vyper/codegen/self_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/codegen/stmt.py` & `vyper-0.3.9/vyper/codegen/stmt.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/compiler/README.md` & `vyper-0.3.9/vyper/compiler/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/compiler/__init__.py` & `vyper-0.3.9/vyper/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/compiler/output.py` & `vyper-0.3.9/vyper/compiler/output.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/compiler/phases.py` & `vyper-0.3.9/vyper/compiler/phases.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/compiler/utils.py` & `vyper-0.3.9/vyper/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/evm/address_space.py` & `vyper-0.3.9/vyper/evm/address_space.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/evm/opcodes.py` & `vyper-0.3.9/vyper/evm/opcodes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/exceptions.py` & `vyper-0.3.9/vyper/exceptions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/ir/README.md` & `vyper-0.3.9/vyper/ir/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/ir/compile_ir.py` & `vyper-0.3.9/vyper/ir/compile_ir.py`

 * *Files 0% similar despite different names*

```diff
@@ -754,25 +754,32 @@
         if item.pc_debugger:
             line_number_map["pc_breakpoints"].add(pos)
         # Create line number breakpoint.
         else:
             line_number_map["breakpoints"].add(item.lineno + 1)
 
 
+_TERMINAL_OPS = ("JUMP", "RETURN", "REVERT", "STOP", "INVALID")
+
+
 def _prune_unreachable_code(assembly):
     # In converting IR to assembly we sometimes end up with unreachable
     # instructions - POPing to clear the stack or STOPing execution at the
     # end of a function that has already returned or reverted. This should
     # be addressed in the IR, but for now we do a final sanity check here
     # to avoid unnecessary bytecode bloat.
     changed = False
     i = 0
-    while i < len(assembly) - 1:
-        if assembly[i] in ("JUMP", "RETURN", "REVERT", "STOP") and not (
-            is_symbol(assembly[i + 1]) or assembly[i + 1] == "JUMPDEST"
+    while i < len(assembly) - 2:
+        instr = assembly[i]
+        if isinstance(instr, list):
+            instr = assembly[i][-1]
+
+        if assembly[i] in _TERMINAL_OPS and not (
+            is_symbol(assembly[i + 1]) and assembly[i + 2] in ("JUMPDEST", "BLANK")
         ):
             changed = True
             del assembly[i + 1]
         else:
             i += 1
 
     return changed
```

### Comparing `vyper-0.3.8/vyper/ir/optimizer.py` & `vyper-0.3.9/vyper/ir/optimizer.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/ir/s_expressions.py` & `vyper-0.3.9/vyper/ir/s_expressions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/semantics/README.md` & `vyper-0.3.9/vyper/semantics/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/semantics/analysis/annotation.py` & `vyper-0.3.9/vyper/semantics/analysis/annotation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/semantics/analysis/base.py` & `vyper-0.3.9/vyper/semantics/analysis/base.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/semantics/analysis/common.py` & `vyper-0.3.9/vyper/semantics/analysis/common.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/semantics/analysis/data_positions.py` & `vyper-0.3.9/vyper/semantics/analysis/data_positions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/semantics/analysis/levenshtein_utils.py` & `vyper-0.3.9/vyper/semantics/analysis/levenshtein_utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/semantics/analysis/local.py` & `vyper-0.3.9/vyper/semantics/analysis/local.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/semantics/analysis/module.py` & `vyper-0.3.9/vyper/semantics/analysis/module.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/semantics/analysis/utils.py` & `vyper-0.3.9/vyper/semantics/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/semantics/environment.py` & `vyper-0.3.9/vyper/semantics/environment.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/semantics/namespace.py` & `vyper-0.3.9/vyper/semantics/namespace.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/semantics/types/__init__.py` & `vyper-0.3.9/vyper/semantics/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/semantics/types/base.py` & `vyper-0.3.9/vyper/semantics/types/base.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/semantics/types/bytestrings.py` & `vyper-0.3.9/vyper/semantics/types/bytestrings.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/semantics/types/function.py` & `vyper-0.3.9/vyper/semantics/types/function.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/semantics/types/primitives.py` & `vyper-0.3.9/vyper/semantics/types/primitives.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/semantics/types/subscriptable.py` & `vyper-0.3.9/vyper/semantics/types/subscriptable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/semantics/types/user.py` & `vyper-0.3.9/vyper/semantics/types/user.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/semantics/types/utils.py` & `vyper-0.3.9/vyper/semantics/types/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/typing.py` & `vyper-0.3.9/vyper/typing.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper/utils.py` & `vyper-0.3.9/vyper/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper.egg-info/PKG-INFO` & `vyper-0.3.9/vyper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vyper
-Version: 0.3.8
+Version: 0.3.9
 Summary: Vyper: the Pythonic Programming Language for the EVM
 Home-page: https://github.com/vyperlang/vyper
 Author: Vyper Team
 Author-email: 
 License: Apache License 2.0
 Keywords: ethereum evm smart contract language
 Classifier: Intended Audience :: Developers
```

### Comparing `vyper-0.3.8/vyper.egg-info/SOURCES.txt` & `vyper-0.3.9/vyper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vyper-0.3.8/vyper.egg-info/requires.txt` & `vyper-0.3.9/vyper.egg-info/requires.txt`

 * *Files identical despite different names*

