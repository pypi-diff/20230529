# Comparing `tmp/propan-0.1.2.3.tar.gz` & `tmp/propan-0.1.2.4.tar.gz`

## Comparing `propan-0.1.2.3.tar` & `propan-0.1.2.4.tar`

### file list

```diff
@@ -1,142 +1,142 @@
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.2.3/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.2.3/SECURITY.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 propan-0.1.2.3/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.2.3/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.2.3/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 propan-0.1.2.3/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/kafka/1_direct.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/nats/1_basic.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/redis/pattern.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/sqs/1_basic.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/__about__.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/__main__.py
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/py.typed
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/__init__.py
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/_model/__init__.py
--rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/_model/broker_usecase.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/_model/schemas.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/_model/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/kafka/__init__.py
--rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/kafka/kafka_broker.py
--rw-r--r--   0        0        0     7406 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/kafka/kafka_broker.pyi
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/kafka/schemas.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0    11041 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/sqs/__init__.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/sqs/schema.py
--rw-r--r--   0        0        0    10585 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/sqs/sqs_broker.py
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/sqs/sqs_broker.pyi
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/__init__.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/app.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/main.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/async_app/kafka.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/async_app/sqs.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/kafka/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/kafka/router.py
--rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/kafka/router.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/nats/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/nats/router.py
--rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/nats/router.pyi
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/sqs/__init__.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/sqs/router.py
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/sqs/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/log/__init__.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/log/formatter.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/log/logging.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/test/__init__.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/test/kafka.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/test/nats.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/test/rabbit.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/test/redis.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/test/sqs.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/test/utils.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/utils/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/utils/classes.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/utils/functions.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/utils/context/main.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.2.3/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.2.3/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.2.3/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.2.3/scripts/test.sh
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 propan-0.1.2.3/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.2.3/LICENSE
--rw-r--r--   0        0        0    12356 2020-02-02 00:00:00.000000 propan-0.1.2.3/README.md
--rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 propan-0.1.2.3/pyproject.toml
--rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 propan-0.1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.2.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.2.4/SECURITY.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 propan-0.1.2.4/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.2.4/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.2.4/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 propan-0.1.2.4/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/kafka/1_direct.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/nats/1_basic.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/redis/pattern.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/sqs/1_basic.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/__about__.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/__main__.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/py.typed
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/__init__.py
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/_model/__init__.py
+-rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/_model/broker_usecase.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/_model/schemas.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/_model/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/kafka/__init__.py
+-rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     7406 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/kafka/kafka_broker.pyi
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/kafka/schemas.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0    11041 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/sqs/__init__.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/sqs/schema.py
+-rw-r--r--   0        0        0    10585 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/sqs/sqs_broker.py
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/sqs/sqs_broker.pyi
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/__init__.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/app.py
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/main.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/async_app/kafka.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/async_app/sqs.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/kafka/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/kafka/router.py
+-rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/kafka/router.pyi
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/nats/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/nats/router.py
+-rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/nats/router.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/sqs/__init__.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/sqs/router.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/sqs/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/log/__init__.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/log/formatter.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/log/logging.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/test/__init__.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/test/kafka.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/test/nats.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/test/redis.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/test/sqs.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/test/utils.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/utils/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/utils/classes.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/utils/functions.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/utils/context/main.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.2.4/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.2.4/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.2.4/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.2.4/scripts/test.sh
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 propan-0.1.2.4/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.2.4/LICENSE
+-rw-r--r--   0        0        0    12542 2020-02-02 00:00:00.000000 propan-0.1.2.4/README.md
+-rw-r--r--   0        0        0     5494 2020-02-02 00:00:00.000000 propan-0.1.2.4/pyproject.toml
+-rw-r--r--   0        0        0    16147 2020-02-02 00:00:00.000000 propan-0.1.2.4/PKG-INFO
```

### Comparing `propan-0.1.2.3/CONTRIBUTING.md` & `propan-0.1.2.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/SECURITY.md` & `propan-0.1.2.4/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/.github/workflows/documentation.yml` & `propan-0.1.2.4/.github/workflows/documentation.yml`

 * *Files 2% similar despite different names*

```diff
@@ -18,10 +18,10 @@
       - uses: actions/setup-python@v4
         with:
           python-version: 3.x
       - uses: actions/cache@v2
         with:
           key: ${{ github.ref }}
           path: .cache
-      - run: pip install mkdocs-material mkdocs-static-i18n mdx-include mkdocs-markdownextradata-plugin
+      - run: pip install mkdocs-material mkdocs-static-i18n mdx-include mkdocs-macros-plugin
       - working-directory: ./docs
         run: mkdocs gh-deploy --force
```

### Comparing `propan-0.1.2.3/.github/workflows/publish_coverage.yml` & `propan-0.1.2.4/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/.github/workflows/publish_pypi.yml` & `propan-0.1.2.4/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/.github/workflows/tests.yml` & `propan-0.1.2.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/examples/3_lifespan_events.py` & `propan-0.1.2.4/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/examples/4_cli_attributes_promotion.py` & `propan-0.1.2.4/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/examples/5_publishing.py` & `propan-0.1.2.4/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/examples/6_arguments_casting.py` & `propan-0.1.2.4/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/examples/7_handler_errors_processing.py` & `propan-0.1.2.4/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/examples/dependencies/1_dependency_injection.py` & `propan-0.1.2.4/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.2.4/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.2.4/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.2.4/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.2.4/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/examples/dependencies/7_annotated.py` & `propan-0.1.2.4/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.2.4/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.2.4/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.2.4/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.2.4/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/examples/http_frameworks_integrations/quart.py` & `propan-0.1.2.4/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.2.4/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.2.4/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/examples/rabbit/direct.py` & `propan-0.1.2.4/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/examples/rabbit/fanout.py` & `propan-0.1.2.4/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/examples/rabbit/header.py` & `propan-0.1.2.4/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/examples/rabbit/topic.py` & `propan-0.1.2.4/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/examples/redis/direct.py` & `propan-0.1.2.4/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/examples/redis/pattern.py` & `propan-0.1.2.4/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/__init__.py` & `propan-0.1.2.4/propan/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/annotations.py` & `propan-0.1.2.4/propan/annotations.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/types.py` & `propan-0.1.2.4/propan/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/brokers/push_back_watcher.py` & `propan-0.1.2.4/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/brokers/_model/broker_usecase.py` & `propan-0.1.2.4/propan/brokers/_model/broker_usecase.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/brokers/_model/schemas.py` & `propan-0.1.2.4/propan/brokers/_model/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/brokers/_model/utils.py` & `propan-0.1.2.4/propan/brokers/_model/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/brokers/kafka/kafka_broker.py` & `propan-0.1.2.4/propan/brokers/kafka/kafka_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/brokers/kafka/kafka_broker.pyi` & `propan-0.1.2.4/propan/brokers/kafka/kafka_broker.pyi`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     handlers: List[Handler]
 
     def __init__(
         self,
         bootstrap_servers: Union[str, List[str]] = "localhost",
         *,
         # both
-        loop: Optional[AbstractEventLoop] = None,
         client_id: str = "propan-" + __version__,
         request_timeout_ms: int = 40 * 1000,
         retry_backoff_ms: int = 100,
         metadata_max_age_ms: int = 5 * 60 * 1000,
         security_protocol: Literal[
             "SSL",
             "PLAINTEXT",
@@ -70,14 +69,15 @@
         max_request_size: int = 1048576,
         linger_ms: int = 0,
         send_backoff_ms: int = 100,
         ssl_context: Optional[SSLContext] = None,
         enable_idempotence: bool = False,
         transactional_id: Optional[str] = None,
         transaction_timeout_ms: int = 60000,
+        loop: Optional[AbstractEventLoop] = None,
         # broker
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
     ) -> None: ...
     async def connect(
```

### Comparing `propan-0.1.2.3/propan/brokers/nats/nats_broker.py` & `propan-0.1.2.4/propan/brokers/nats/nats_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.2.4/propan/brokers/nats/nats_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.2.4/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/brokers/nats/schemas.py` & `propan-0.1.2.4/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.2.4/propan/brokers/rabbit/rabbit_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.2.4/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/brokers/rabbit/schemas.py` & `propan-0.1.2.4/propan/brokers/rabbit/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/brokers/redis/redis_broker.py` & `propan-0.1.2.4/propan/brokers/redis/redis_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/brokers/redis/redis_broker.pyi` & `propan-0.1.2.4/propan/brokers/redis/redis_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/brokers/redis/schemas.py` & `propan-0.1.2.4/propan/brokers/redis/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/brokers/sqs/schema.py` & `propan-0.1.2.4/propan/brokers/sqs/schema.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/brokers/sqs/sqs_broker.py` & `propan-0.1.2.4/propan/brokers/sqs/sqs_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/brokers/sqs/sqs_broker.pyi` & `propan-0.1.2.4/propan/brokers/sqs/sqs_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/cli/app.py` & `propan-0.1.2.4/propan/cli/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/cli/main.py` & `propan-0.1.2.4/propan/cli/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/cli/startproject/core.py` & `propan-0.1.2.4/propan/cli/startproject/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/cli/startproject/async_app/app.py` & `propan-0.1.2.4/propan/cli/startproject/async_app/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/cli/startproject/async_app/core.py` & `propan-0.1.2.4/propan/cli/startproject/async_app/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/cli/startproject/async_app/kafka.py` & `propan-0.1.2.4/propan/cli/startproject/async_app/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/cli/startproject/async_app/nats.py` & `propan-0.1.2.4/propan/cli/startproject/async_app/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.2.4/propan/cli/startproject/async_app/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/cli/startproject/async_app/redis.py` & `propan-0.1.2.4/propan/cli/startproject/async_app/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/cli/startproject/async_app/sqs.py` & `propan-0.1.2.4/propan/cli/startproject/async_app/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/cli/supervisors/basereload.py` & `propan-0.1.2.4/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/cli/supervisors/multiprocess.py` & `propan-0.1.2.4/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/cli/supervisors/utils.py` & `propan-0.1.2.4/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/cli/supervisors/watchfiles.py` & `propan-0.1.2.4/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/cli/utils/imports.py` & `propan-0.1.2.4/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/cli/utils/logs.py` & `propan-0.1.2.4/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/cli/utils/parser.py` & `propan-0.1.2.4/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/fastapi/__init__.py` & `propan-0.1.2.4/propan/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/fastapi/core/route.py` & `propan-0.1.2.4/propan/fastapi/core/route.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/fastapi/core/router.py` & `propan-0.1.2.4/propan/fastapi/core/router.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/fastapi/kafka/router.pyi` & `propan-0.1.2.4/propan/fastapi/kafka/router.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,30 @@
 from kafka.coordinator.assignors.roundrobin import RoundRobinPartitionAssignor
 from kafka.partitioner.default import DefaultPartitioner
 from starlette import routing
 from starlette.responses import JSONResponse, Response
 from starlette.types import ASGIApp
 from typing_extensions import Literal, TypeVar
 
+from propan import KafkaBroker
 from propan.__about__ import __version__
 from propan.fastapi.core import PropanRouter
 from propan.log import access_logger
 from propan.types import AnyCallable
 
 Partition = TypeVar("Partition")
 
 class KafkaRouter(PropanRouter):
+    broker: KafkaBroker
+
     def __init__(
         self,
         bootstrap_servers: Union[str, List[str]] = "localhost",
         *,
         # both
-        loop: Optional[AbstractEventLoop] = None,
         client_id: str = "propan-" + __version__,
         request_timeout_ms: int = 40 * 1000,
         retry_backoff_ms: int = 100,
         metadata_max_age_ms: int = 5 * 60 * 1000,
         security_protocol: Literal[
             "SSL",
             "PLAINTEXT",
@@ -86,14 +88,15 @@
         on_startup: Optional[Sequence[Callable[[], Any]]] = None,
         on_shutdown: Optional[Sequence[Callable[[], Any]]] = None,
         deprecated: Optional[bool] = None,
         include_in_schema: bool = True,
         generate_unique_id_function: Callable[[APIRoute], str] = Default(
             generate_unique_id
         ),
+        loop: Optional[AbstractEventLoop] = None,
         # Broker kwargs
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
     ) -> None:
         pass
```

### Comparing `propan-0.1.2.3/propan/fastapi/nats/router.pyi` & `propan-0.1.2.4/propan/fastapi/nats/router.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -23,19 +23,22 @@
     JWTCallback,
     SignatureCallback,
 )
 from starlette import routing
 from starlette.responses import JSONResponse, Response
 from starlette.types import ASGIApp
 
+from propan import NatsBroker
 from propan.fastapi.core.router import PropanRouter
 from propan.log import access_logger
 from propan.types import AnyCallable
 
 class NatsRouter(PropanRouter):
+    broker: NatsBroker
+
     def __init__(
         self,
         servers: Union[str, List[str]] = ["nats://localhost:4222"],  # noqa: B006
         error_cb: Optional[ErrorCallback] = None,
         disconnected_cb: Optional[Callback] = None,
         closed_cb: Optional[Callback] = None,
         discovered_server_cb: Optional[Callback] = None,
```

### Comparing `propan-0.1.2.3/propan/fastapi/rabbit/router.pyi` & `propan-0.1.2.4/propan/fastapi/rabbit/router.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,23 @@
 from fastapi.routing import APIRoute
 from fastapi.utils import generate_unique_id
 from pamqp.common import FieldTable
 from starlette import routing
 from starlette.responses import JSONResponse, Response
 from starlette.types import ASGIApp
 
+from propan import RabbitBroker
 from propan.brokers.rabbit import RabbitExchange, RabbitQueue
 from propan.fastapi.core import PropanRouter
 from propan.log import access_logger
 from propan.types import AnyCallable
 
 class RabbitRouter(PropanRouter):
+    broker: RabbitBroker
+
     def __init__(
         self,
         host: str = "localhost",
         port: int = 5672,
         login: str = "guest",
         password: str = "guest",
         virtualhost: str = "/",
```

### Comparing `propan-0.1.2.3/propan/fastapi/redis/router.pyi` & `propan-0.1.2.4/propan/fastapi/redis/router.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,22 @@
 from fastapi.routing import APIRoute
 from fastapi.utils import generate_unique_id
 from redis.asyncio.connection import BaseParser, DefaultParser, Encoder
 from starlette import routing
 from starlette.responses import JSONResponse, Response
 from starlette.types import ASGIApp
 
+from propan import RedisBroker
 from propan.fastapi.core.router import PropanRouter
 from propan.log import access_logger
 from propan.types import AnyCallable
 
 class RedisRouter(PropanRouter):
+    broker: RedisBroker
+
     def __init__(
         self,
         url: str = "redis://localhost:6379",
         polling_interval: float = 1.0,
         host: str = "localhost",
         port: Union[str, int] = 6379,
         db: Union[str, int] = 0,
```

### Comparing `propan-0.1.2.3/propan/fastapi/sqs/router.pyi` & `propan-0.1.2.4/propan/fastapi/sqs/router.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -7,20 +7,23 @@
 from fastapi.datastructures import Default
 from fastapi.routing import APIRoute
 from fastapi.utils import generate_unique_id
 from starlette import routing
 from starlette.responses import JSONResponse, Response
 from starlette.types import ASGIApp
 
+from propan import SQSBroker
 from propan.brokers.sqs.schema import SQSQueue
 from propan.fastapi.core.router import PropanRouter
 from propan.log import access_logger
 from propan.types import AnyCallable
 
 class SQSRouter(PropanRouter):
+    broker: SQSBroker
+
     def __init__(
         self,
         url: str = "http://localhost:9324/",
         *,
         region_name: Optional[str] = None,
         api_version: Optional[str] = None,
         use_ssl: bool = True,
```

### Comparing `propan-0.1.2.3/propan/log/formatter.py` & `propan-0.1.2.4/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/log/logging.py` & `propan-0.1.2.4/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/test/__init__.py` & `propan-0.1.2.4/propan/test/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/test/kafka.py` & `propan-0.1.2.4/propan/test/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/test/nats.py` & `propan-0.1.2.4/propan/test/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/test/rabbit.py` & `propan-0.1.2.4/propan/test/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/test/redis.py` & `propan-0.1.2.4/propan/test/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/test/sqs.py` & `propan-0.1.2.4/propan/test/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/test/utils.py` & `propan-0.1.2.4/propan/test/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/utils/functions.py` & `propan-0.1.2.4/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/utils/context/main.py` & `propan-0.1.2.4/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/propan/utils/context/types.py` & `propan-0.1.2.4/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/LICENSE` & `propan-0.1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.3/README.md` & `propan-0.1.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 # Propan
 
 **Propan** - just *~~an another one HTTP~~* a **declarative Python MQ framework**. It's following by <a href="https://fastapi.tiangolo.com/ru/" target="_blank">*fastapi*</a>, simplify Message Brokers around code writing and provides a helpful development toolkit, which existed only in HTTP-frameworks world until now.
 
 It's designed to create reactive microservices around <a href="https://microservices.io/patterns/communication-style/messaging.html" target="_blank">Messaging Architecture</a>.
 
-It is a modern, high-level framework on top of popular specific Python brokers libraries, based on <a href="https://docs.pydantic.dev/" target="_blank">*pydantic*</a> and <a href="https://fastapi.tiangolo.com/ru/" target="_blank">*fastapi*</a>, <a href="https://docs.pytest.org/en/7.3.x/" target="_blank">*pytest*</a> concepts.
+It is a modern, high-level framework on top of popular specific Python brokers libraries, based on <a href="https://docs.pydantic.dev/" target="_blank">*pydantic*</a> and <a href="https://fastapi.tiangolo.com/ru/" target="_blank">*fastapi*</a>, <a href="https://docs.pytest.org/en/latest/" target="_blank">*pytest*</a> concepts.
 
 ---
 
 **Documentation**: <a href="https://lancetnik.github.io/Propan/" target="_blank">https://lancetnik.github.io/Propan/</a>
 
 ---
 
@@ -46,14 +46,15 @@
 * **Intuitive**: Great editor support. Autocompletion everywhere.
 * [**Dependencies management**](#dependencies): Minimization of code duplication. Access to dependencies at any level of the call stack.
 * [**Integrations**](#http-frameworks-integrations): **Propan** is fully compatible with <a href="https://lancetnik.github.io/Propan/integrations/1_integrations-index/" target="_blank">any HTTP framework</a> you want
 * **MQ independent**: Single interface to popular MQ:
   * **Redis** (based on <a href="https://redis.readthedocs.io/en/stable/index.html" target="_blank">redis-py</a>)
   * **RabbitMQ** (based on <a href="https://aio-pika.readthedocs.io/en/latest/" target="_blank">aio-pika</a>)
   * **Kafka** (based on <a href="https://aiokafka.readthedocs.io/en/stable/" target="_blank">aiokafka</a>)
+  * **SQS** (based on <a href="https://aiobotocore.readthedocs.io/en/latest/" target="_blank">aiobotocore</a>)
   * **Nats** (based on <a href="https://github.com/nats-io/nats.py" target="_blank">nats-py</a>)
 * <a href="https://lancetnik.github.io/Propan/getting_started/4_broker/5_rpc/" target="_blank">**RPC**</a>: The framework supports RPC requests over MQ, which will allow performing long operations on remote services asynchronously.
 * [**Great to develop**](#cli-power): CLI tool provides great development experience:
   * framework-independent way to manage the project environment
   * application code *hot reload*
   * robust application templates
 * <a href="https://lancetnik.github.io/Propan/getting_started/7_testing" target="_blank">**Testability**</a>: **Propan** allows you to test your app without external dependencies: you do not have to set up a Message Broker, you can use a virtual one!
@@ -154,19 +155,21 @@
 
 ```python
 from propan import PropanApp
 from propan import RabbitBroker
 # from propan import RedisBroker
 # from propan import NatsBroker
 # from propan import SQSBroker
+# from propan import KafkaBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 # broker = NatsBroker("nats://localhost:4222")
 # broker = RedisBroker("redis://localhost:6379")
 # broker = SQSBroker("http://localhost:9324", ...)
+# broker = KafkaBroker("localhost:9092")
 
 app = PropanApp(broker)
 
 @broker.handle("test")
 async def base_handler(body):
     '''Handle all default exchange messages with `test` routing key'''
     print(body)
```

#### html2text {}

```diff
@@ -11,64 +11,66 @@
 -- ### The key features are * **Simple**: Designed to be easy to use and learn.
 * **Intuitive**: Great editor support. Autocompletion everywhere. *
 [**Dependencies management**](#dependencies): Minimization of code duplication.
 Access to dependencies at any level of the call stack. * [**Integrations**]
 (#http-frameworks-integrations): **Propan** is fully compatible with any_HTTP
 framework you want * **MQ independent**: Single interface to popular MQ: *
 **Redis** (based on redis-py) * **RabbitMQ** (based on aio-pika) * **Kafka**
-(based on aiokafka) * **Nats** (based on nats-py) * **RPC**: The framework
-supports RPC requests over MQ, which will allow performing long operations on
-remote services asynchronously. * [**Great to develop**](#cli-power): CLI tool
-provides great development experience: * framework-independent way to manage
-the project environment * application code *hot reload* * robust application
-templates * **Testability**: **Propan** allows you to test your app without
-external dependencies: you do not have to set up a Message Broker, you can use
-a virtual one! ### Supported MQ brokers | | async | sync | |-------------------
-|:-------------------------------------------------------:|:-------------------
--:| | **RabbitMQ** | :heavy_check_mark: **stable** :heavy_check_mark: | :mag:
-planning :mag: | | **Redis** | :heavy_check_mark: **stable** :heavy_check_mark:
-| :mag: planning :mag: | | **Nats** | :heavy_check_mark: **stable** :
-heavy_check_mark: | :mag: planning :mag: | | **Kafka** | :warning: **beta** :
-warning: | :mag: planning :mag: | | **SQS** | :warning: **beta** :warning: | :
-mag: planning :mag: | | **NatsJS** | :hammer_and_wrench: **in progress** :
-hammer_and_wrench: | :mag: planning :mag: | | **MQTT** | :mag: planning :mag: |
-:mag: planning :mag: | | **Redis Streams** | :mag: planning :mag: | :mag:
-planning :mag: | | **Pulsar** | :mag: planning :mag: | :mag: planning :mag: |
-### Community If you are interested in this project, please give me feedback by
-star or/and watch repository. If you have any questions or ideas about features
-to implement, welcome to [discussions](https://github.com/Lancetnik/Propan/
-discussions). --- ## Declarative? With declarative tools you can define **what
-you need to get**. With traditional imperative tools you must write **what you
-need to do**. Take a look at classic imperative tools, such as aio-pika, pika,
-redis-py, nats-py, etc. This is the **Quickstart** with the *aio-pika*:
-```python import asyncio import aio_pika async def main(): connection = await
-aio_pika.connect_robust( "amqp://guest:guest@127.0.0.1/" ) queue_name =
-"test_queue" async with connection: channel = await connection.channel() queue
-= await channel.declare_queue(queue_name) async with queue.iterator() as
-queue_iter: async for message in queue_iter: async with message.process():
-print(message.body) asyncio.run(main()) ``` **aio-pika** is a great tool with a
+(based on aiokafka) * **SQS** (based on aiobotocore) * **Nats** (based on nats-
+py) * **RPC**: The framework supports RPC requests over MQ, which will allow
+performing long operations on remote services asynchronously. * [**Great to
+develop**](#cli-power): CLI tool provides great development experience: *
+framework-independent way to manage the project environment * application code
+*hot reload* * robust application templates * **Testability**: **Propan**
+allows you to test your app without external dependencies: you do not have to
+set up a Message Broker, you can use a virtual one! ### Supported MQ brokers |
+| async | sync | |-------------------|:----------------------------------------
+---------------:|:--------------------:| | **RabbitMQ** | :heavy_check_mark:
+**stable** :heavy_check_mark: | :mag: planning :mag: | | **Redis** | :
+heavy_check_mark: **stable** :heavy_check_mark: | :mag: planning :mag: | |
+**Nats** | :heavy_check_mark: **stable** :heavy_check_mark: | :mag: planning :
+mag: | | **Kafka** | :warning: **beta** :warning: | :mag: planning :mag: | |
+**SQS** | :warning: **beta** :warning: | :mag: planning :mag: | | **NatsJS** |
+:hammer_and_wrench: **in progress** :hammer_and_wrench: | :mag: planning :mag:
+| | **MQTT** | :mag: planning :mag: | :mag: planning :mag: | | **Redis
+Streams** | :mag: planning :mag: | :mag: planning :mag: | | **Pulsar** | :mag:
+planning :mag: | :mag: planning :mag: | ### Community If you are interested in
+this project, please give me feedback by star or/and watch repository. If you
+have any questions or ideas about features to implement, welcome to
+[discussions](https://github.com/Lancetnik/Propan/discussions). --- ##
+Declarative? With declarative tools you can define **what you need to get**.
+With traditional imperative tools you must write **what you need to do**. Take
+a look at classic imperative tools, such as aio-pika, pika, redis-py, nats-py,
+etc. This is the **Quickstart** with the *aio-pika*: ```python import asyncio
+import aio_pika async def main(): connection = await aio_pika.connect_robust
+( "amqp://guest:guest@127.0.0.1/" ) queue_name = "test_queue" async with
+connection: channel = await connection.channel() queue = await
+channel.declare_queue(queue_name) async with queue.iterator() as queue_iter:
+async for message in queue_iter: async with message.process(): print
+(message.body) asyncio.run(main()) ``` **aio-pika** is a great tool with a
 really easy learning curve. But it's still imperative. You need to *connect*,
 declare *channel*, *queues*, *exchanges* by yourself. Also, you need to manage
 *connection*, *message*, *queue* context to avoid any troubles. It is not a bad
 way, but it can be much easier. ```python from propan import PropanApp,
 RabbitBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
 PropanApp(broker) @broker.handle("test_queue") async def base_handler(body):
 print(body) ``` This is the **Propan** declarative way to write the same code.
 That is so much easier, isn't it? --- ## Quickstart Install using `pip`:
 ```shell pip install "propan[async-rabbit]" # or pip install "propan[async-
 nats]" # or pip install "propan[async-redis]" # or pip install "propan[async-
 kafka]" # or pip install "propan[async-sqs]" ``` ### Basic usage Create an
 application with the following code at `serve.py`: ```python from propan import
 PropanApp from propan import RabbitBroker # from propan import RedisBroker #
-from propan import NatsBroker # from propan import SQSBroker broker =
-RabbitBroker("amqp://guest:guest@localhost:5672/") # broker = NatsBroker("nats:
-//localhost:4222") # broker = RedisBroker("redis://localhost:6379") # broker =
-SQSBroker("http://localhost:9324", ...) app = PropanApp(broker) @broker.handle
-("test") async def base_handler(body): '''Handle all default exchange messages
-with `test` routing key''' print(body) ``` And just run it: ```shell propan run
+from propan import NatsBroker # from propan import SQSBroker # from propan
+import KafkaBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
+# broker = NatsBroker("nats://localhost:4222") # broker = RedisBroker("redis://
+localhost:6379") # broker = SQSBroker("http://localhost:9324", ...) # broker =
+KafkaBroker("localhost:9092") app = PropanApp(broker) @broker.handle("test")
+async def base_handler(body): '''Handle all default exchange messages with
+`test` routing key''' print(body) ``` And just run it: ```shell propan run
 serve:app ``` --- ## Type casting Propan uses `pydantic` to cast incoming
 function arguments to types according to their annotation. ```python from
 pydantic import BaseModel from propan import PropanApp, Context, RabbitBroker
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp
 (broker) class SimpleMessage(BaseModel): key: int @broker.handle("test2") async
 def second_handler(body: SimpleMessage): assert isinstance(body.key, int) ``` -
 -- ## Dependencies **Propan** a has dependencies management policy close to
```

### Comparing `propan-0.1.2.3/pyproject.toml` & `propan-0.1.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     "asyncmock; python_version < '3.8'",
 ]
 
 doc = [
     "mkdocs-material >=8.1.4,<9.0.0",
     "mkdocs-static-i18n",
     "mdx-include >=1.4.1,<2.0.0",
-    "mkdocs-markdownextradata-plugin >=0.1.7,<0.3.0",
+    "mkdocs-macros-plugin",
 
     "typer[all]",
 ]
 
 dev = [
     "propan[test]",
     "propan[doc]",
```

### Comparing `propan-0.1.2.3/PKG-INFO` & `propan-0.1.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.2.3
+Version: 0.1.2.4
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
@@ -56,15 +56,15 @@
 Requires-Dist: propan[doc]; extra == 'dev'
 Requires-Dist: propan[test]; extra == 'dev'
 Requires-Dist: ruff==0.0.261; extra == 'dev'
 Requires-Dist: typer[all]; extra == 'dev'
 Requires-Dist: types-redis; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: mdx-include<2.0.0,>=1.4.1; extra == 'doc'
-Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7; extra == 'doc'
+Requires-Dist: mkdocs-macros-plugin; extra == 'doc'
 Requires-Dist: mkdocs-material<9.0.0,>=8.1.4; extra == 'doc'
 Requires-Dist: mkdocs-static-i18n; extra == 'doc'
 Requires-Dist: typer[all]; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: asyncmock; python_version < '3.8' and extra == 'test'
 Requires-Dist: coverage[toml]>=7.2; extra == 'test'
 Requires-Dist: fastapi; extra == 'test'
@@ -107,15 +107,15 @@
 
 # Propan
 
 **Propan** - just *~~an another one HTTP~~* a **declarative Python MQ framework**. It's following by <a href="https://fastapi.tiangolo.com/ru/" target="_blank">*fastapi*</a>, simplify Message Brokers around code writing and provides a helpful development toolkit, which existed only in HTTP-frameworks world until now.
 
 It's designed to create reactive microservices around <a href="https://microservices.io/patterns/communication-style/messaging.html" target="_blank">Messaging Architecture</a>.
 
-It is a modern, high-level framework on top of popular specific Python brokers libraries, based on <a href="https://docs.pydantic.dev/" target="_blank">*pydantic*</a> and <a href="https://fastapi.tiangolo.com/ru/" target="_blank">*fastapi*</a>, <a href="https://docs.pytest.org/en/7.3.x/" target="_blank">*pytest*</a> concepts.
+It is a modern, high-level framework on top of popular specific Python brokers libraries, based on <a href="https://docs.pydantic.dev/" target="_blank">*pydantic*</a> and <a href="https://fastapi.tiangolo.com/ru/" target="_blank">*fastapi*</a>, <a href="https://docs.pytest.org/en/latest/" target="_blank">*pytest*</a> concepts.
 
 ---
 
 **Documentation**: <a href="https://lancetnik.github.io/Propan/" target="_blank">https://lancetnik.github.io/Propan/</a>
 
 ---
 
@@ -125,14 +125,15 @@
 * **Intuitive**: Great editor support. Autocompletion everywhere.
 * [**Dependencies management**](#dependencies): Minimization of code duplication. Access to dependencies at any level of the call stack.
 * [**Integrations**](#http-frameworks-integrations): **Propan** is fully compatible with <a href="https://lancetnik.github.io/Propan/integrations/1_integrations-index/" target="_blank">any HTTP framework</a> you want
 * **MQ independent**: Single interface to popular MQ:
   * **Redis** (based on <a href="https://redis.readthedocs.io/en/stable/index.html" target="_blank">redis-py</a>)
   * **RabbitMQ** (based on <a href="https://aio-pika.readthedocs.io/en/latest/" target="_blank">aio-pika</a>)
   * **Kafka** (based on <a href="https://aiokafka.readthedocs.io/en/stable/" target="_blank">aiokafka</a>)
+  * **SQS** (based on <a href="https://aiobotocore.readthedocs.io/en/latest/" target="_blank">aiobotocore</a>)
   * **Nats** (based on <a href="https://github.com/nats-io/nats.py" target="_blank">nats-py</a>)
 * <a href="https://lancetnik.github.io/Propan/getting_started/4_broker/5_rpc/" target="_blank">**RPC**</a>: The framework supports RPC requests over MQ, which will allow performing long operations on remote services asynchronously.
 * [**Great to develop**](#cli-power): CLI tool provides great development experience:
   * framework-independent way to manage the project environment
   * application code *hot reload*
   * robust application templates
 * <a href="https://lancetnik.github.io/Propan/getting_started/7_testing" target="_blank">**Testability**</a>: **Propan** allows you to test your app without external dependencies: you do not have to set up a Message Broker, you can use a virtual one!
@@ -233,19 +234,21 @@
 
 ```python
 from propan import PropanApp
 from propan import RabbitBroker
 # from propan import RedisBroker
 # from propan import NatsBroker
 # from propan import SQSBroker
+# from propan import KafkaBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 # broker = NatsBroker("nats://localhost:4222")
 # broker = RedisBroker("redis://localhost:6379")
 # broker = SQSBroker("http://localhost:9324", ...)
+# broker = KafkaBroker("localhost:9092")
 
 app = PropanApp(broker)
 
 @broker.handle("test")
 async def base_handler(body):
     '''Handle all default exchange messages with `test` routing key'''
     print(body)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propan Version: 0.1.2.3 Summary: Propan framework:
+Metadata-Version: 2.1 Name: propan Version: 0.1.2.4 Summary: Propan framework:
 the simplest way to work with a messaging queues Project-URL: Homepage, https:/
 /lancetnik.github.io/Propan/ Project-URL: Documentation, https://
 lancetnik.github.io/Propan/ Project-URL: Tracker, https://github.com/Lancetnik/
 Propan/issues Project-URL: Source, https://github.com/Lancetnik/Propan Author-
 email: Pastukhov Nikita
 yandex.ru> License-File: LICENSE Keywords: framework,message brokers,rabbitmq
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
@@ -31,25 +31,25 @@
 redis>=4.2.0rc1; extra == 'async-redis' Provides-Extra: async-sqs Requires-
 Dist: aiobotocore; extra == 'async-sqs' Provides-Extra: dev Requires-Dist:
 black==23.3.0; extra == 'dev' Requires-Dist: isort>=5; extra == 'dev' Requires-
 Dist: mypy==1.1.1; extra == 'dev' Requires-Dist: propan[doc]; extra == 'dev'
 Requires-Dist: propan[test]; extra == 'dev' Requires-Dist: ruff==0.0.261; extra
 == 'dev' Requires-Dist: typer[all]; extra == 'dev' Requires-Dist: types-redis;
 extra == 'dev' Provides-Extra: doc Requires-Dist: mdx-include<2.0.0,>=1.4.1;
-extra == 'doc' Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7;
-extra == 'doc' Requires-Dist: mkdocs-material<9.0.0,>=8.1.4; extra == 'doc'
-Requires-Dist: mkdocs-static-i18n; extra == 'doc' Requires-Dist: typer[all];
-extra == 'doc' Provides-Extra: test Requires-Dist: asyncmock; python_version <
-'3.8' and extra == 'test' Requires-Dist: coverage[toml]>=7.2; extra == 'test'
-Requires-Dist: fastapi; extra == 'test' Requires-Dist: propan[async-kafka];
-extra == 'test' Requires-Dist: propan[async-nats]; extra == 'test' Requires-
-Dist: propan[async-rabbit]; extra == 'test' Requires-Dist: propan[async-redis];
-extra == 'test' Requires-Dist: propan[async-sqs]; extra == 'test' Requires-
-Dist: pytest-asyncio>=0.21; extra == 'test' Requires-Dist: pytest>=7; extra ==
-'test' Description-Content-Type: text/markdown
+extra == 'doc' Requires-Dist: mkdocs-macros-plugin; extra == 'doc' Requires-
+Dist: mkdocs-material<9.0.0,>=8.1.4; extra == 'doc' Requires-Dist: mkdocs-
+static-i18n; extra == 'doc' Requires-Dist: typer[all]; extra == 'doc' Provides-
+Extra: test Requires-Dist: asyncmock; python_version < '3.8' and extra ==
+'test' Requires-Dist: coverage[toml]>=7.2; extra == 'test' Requires-Dist:
+fastapi; extra == 'test' Requires-Dist: propan[async-kafka]; extra == 'test'
+Requires-Dist: propan[async-nats]; extra == 'test' Requires-Dist: propan[async-
+rabbit]; extra == 'test' Requires-Dist: propan[async-redis]; extra == 'test'
+Requires-Dist: propan[async-sqs]; extra == 'test' Requires-Dist: pytest-
+asyncio>=0.21; extra == 'test' Requires-Dist: pytest>=7; extra == 'test'
+Description-Content-Type: text/markdown
                                  [Propan_logo]
           [Tests_coverage] [Coverage] [Package_version] [downloads]
                      [Supported_Python_versions] [GitHub]
 # Propan **Propan** - just *~~an another one HTTP~~* a **declarative Python MQ
 framework**. It's following by *fastapi*, simplify Message Brokers around code
 writing and provides a helpful development toolkit, which existed only in HTTP-
 frameworks world until now. It's designed to create reactive microservices
@@ -59,64 +59,66 @@
 -- ### The key features are * **Simple**: Designed to be easy to use and learn.
 * **Intuitive**: Great editor support. Autocompletion everywhere. *
 [**Dependencies management**](#dependencies): Minimization of code duplication.
 Access to dependencies at any level of the call stack. * [**Integrations**]
 (#http-frameworks-integrations): **Propan** is fully compatible with any_HTTP
 framework you want * **MQ independent**: Single interface to popular MQ: *
 **Redis** (based on redis-py) * **RabbitMQ** (based on aio-pika) * **Kafka**
-(based on aiokafka) * **Nats** (based on nats-py) * **RPC**: The framework
-supports RPC requests over MQ, which will allow performing long operations on
-remote services asynchronously. * [**Great to develop**](#cli-power): CLI tool
-provides great development experience: * framework-independent way to manage
-the project environment * application code *hot reload* * robust application
-templates * **Testability**: **Propan** allows you to test your app without
-external dependencies: you do not have to set up a Message Broker, you can use
-a virtual one! ### Supported MQ brokers | | async | sync | |-------------------
-|:-------------------------------------------------------:|:-------------------
--:| | **RabbitMQ** | :heavy_check_mark: **stable** :heavy_check_mark: | :mag:
-planning :mag: | | **Redis** | :heavy_check_mark: **stable** :heavy_check_mark:
-| :mag: planning :mag: | | **Nats** | :heavy_check_mark: **stable** :
-heavy_check_mark: | :mag: planning :mag: | | **Kafka** | :warning: **beta** :
-warning: | :mag: planning :mag: | | **SQS** | :warning: **beta** :warning: | :
-mag: planning :mag: | | **NatsJS** | :hammer_and_wrench: **in progress** :
-hammer_and_wrench: | :mag: planning :mag: | | **MQTT** | :mag: planning :mag: |
-:mag: planning :mag: | | **Redis Streams** | :mag: planning :mag: | :mag:
-planning :mag: | | **Pulsar** | :mag: planning :mag: | :mag: planning :mag: |
-### Community If you are interested in this project, please give me feedback by
-star or/and watch repository. If you have any questions or ideas about features
-to implement, welcome to [discussions](https://github.com/Lancetnik/Propan/
-discussions). --- ## Declarative? With declarative tools you can define **what
-you need to get**. With traditional imperative tools you must write **what you
-need to do**. Take a look at classic imperative tools, such as aio-pika, pika,
-redis-py, nats-py, etc. This is the **Quickstart** with the *aio-pika*:
-```python import asyncio import aio_pika async def main(): connection = await
-aio_pika.connect_robust( "amqp://guest:guest@127.0.0.1/" ) queue_name =
-"test_queue" async with connection: channel = await connection.channel() queue
-= await channel.declare_queue(queue_name) async with queue.iterator() as
-queue_iter: async for message in queue_iter: async with message.process():
-print(message.body) asyncio.run(main()) ``` **aio-pika** is a great tool with a
+(based on aiokafka) * **SQS** (based on aiobotocore) * **Nats** (based on nats-
+py) * **RPC**: The framework supports RPC requests over MQ, which will allow
+performing long operations on remote services asynchronously. * [**Great to
+develop**](#cli-power): CLI tool provides great development experience: *
+framework-independent way to manage the project environment * application code
+*hot reload* * robust application templates * **Testability**: **Propan**
+allows you to test your app without external dependencies: you do not have to
+set up a Message Broker, you can use a virtual one! ### Supported MQ brokers |
+| async | sync | |-------------------|:----------------------------------------
+---------------:|:--------------------:| | **RabbitMQ** | :heavy_check_mark:
+**stable** :heavy_check_mark: | :mag: planning :mag: | | **Redis** | :
+heavy_check_mark: **stable** :heavy_check_mark: | :mag: planning :mag: | |
+**Nats** | :heavy_check_mark: **stable** :heavy_check_mark: | :mag: planning :
+mag: | | **Kafka** | :warning: **beta** :warning: | :mag: planning :mag: | |
+**SQS** | :warning: **beta** :warning: | :mag: planning :mag: | | **NatsJS** |
+:hammer_and_wrench: **in progress** :hammer_and_wrench: | :mag: planning :mag:
+| | **MQTT** | :mag: planning :mag: | :mag: planning :mag: | | **Redis
+Streams** | :mag: planning :mag: | :mag: planning :mag: | | **Pulsar** | :mag:
+planning :mag: | :mag: planning :mag: | ### Community If you are interested in
+this project, please give me feedback by star or/and watch repository. If you
+have any questions or ideas about features to implement, welcome to
+[discussions](https://github.com/Lancetnik/Propan/discussions). --- ##
+Declarative? With declarative tools you can define **what you need to get**.
+With traditional imperative tools you must write **what you need to do**. Take
+a look at classic imperative tools, such as aio-pika, pika, redis-py, nats-py,
+etc. This is the **Quickstart** with the *aio-pika*: ```python import asyncio
+import aio_pika async def main(): connection = await aio_pika.connect_robust
+( "amqp://guest:guest@127.0.0.1/" ) queue_name = "test_queue" async with
+connection: channel = await connection.channel() queue = await
+channel.declare_queue(queue_name) async with queue.iterator() as queue_iter:
+async for message in queue_iter: async with message.process(): print
+(message.body) asyncio.run(main()) ``` **aio-pika** is a great tool with a
 really easy learning curve. But it's still imperative. You need to *connect*,
 declare *channel*, *queues*, *exchanges* by yourself. Also, you need to manage
 *connection*, *message*, *queue* context to avoid any troubles. It is not a bad
 way, but it can be much easier. ```python from propan import PropanApp,
 RabbitBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
 PropanApp(broker) @broker.handle("test_queue") async def base_handler(body):
 print(body) ``` This is the **Propan** declarative way to write the same code.
 That is so much easier, isn't it? --- ## Quickstart Install using `pip`:
 ```shell pip install "propan[async-rabbit]" # or pip install "propan[async-
 nats]" # or pip install "propan[async-redis]" # or pip install "propan[async-
 kafka]" # or pip install "propan[async-sqs]" ``` ### Basic usage Create an
 application with the following code at `serve.py`: ```python from propan import
 PropanApp from propan import RabbitBroker # from propan import RedisBroker #
-from propan import NatsBroker # from propan import SQSBroker broker =
-RabbitBroker("amqp://guest:guest@localhost:5672/") # broker = NatsBroker("nats:
-//localhost:4222") # broker = RedisBroker("redis://localhost:6379") # broker =
-SQSBroker("http://localhost:9324", ...) app = PropanApp(broker) @broker.handle
-("test") async def base_handler(body): '''Handle all default exchange messages
-with `test` routing key''' print(body) ``` And just run it: ```shell propan run
+from propan import NatsBroker # from propan import SQSBroker # from propan
+import KafkaBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
+# broker = NatsBroker("nats://localhost:4222") # broker = RedisBroker("redis://
+localhost:6379") # broker = SQSBroker("http://localhost:9324", ...) # broker =
+KafkaBroker("localhost:9092") app = PropanApp(broker) @broker.handle("test")
+async def base_handler(body): '''Handle all default exchange messages with
+`test` routing key''' print(body) ``` And just run it: ```shell propan run
 serve:app ``` --- ## Type casting Propan uses `pydantic` to cast incoming
 function arguments to types according to their annotation. ```python from
 pydantic import BaseModel from propan import PropanApp, Context, RabbitBroker
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp
 (broker) class SimpleMessage(BaseModel): key: int @broker.handle("test2") async
 def second_handler(body: SimpleMessage): assert isinstance(body.key, int) ``` -
 -- ## Dependencies **Propan** a has dependencies management policy close to
```

