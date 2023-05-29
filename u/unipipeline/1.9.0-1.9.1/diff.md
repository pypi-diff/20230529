# Comparing `tmp/unipipeline-1.9.0.tar.gz` & `tmp/unipipeline-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unipipeline-1.9.0.tar", last modified: Sat Apr 29 18:20:25 2023, max compression
+gzip compressed data, was "unipipeline-1.9.1.tar", last modified: Mon May 29 10:18:16 2023, max compression
```

## Comparing `unipipeline-1.9.0.tar` & `unipipeline-1.9.1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/
--rwxrwxr-x   0 master    (1000) master    (1000)     1063 2022-08-17 09:07:38.000000 unipipeline-1.9.0/LICENSE
--rw-rw-r--   0 master    (1000) master    (1000)    11100 2023-04-29 18:20:25.683588 unipipeline-1.9.0/PKG-INFO
--rwxrwxr-x   0 master    (1000) master    (1000)    10229 2022-08-17 09:07:38.000000 unipipeline-1.9.0/README.md
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.679588 unipipeline-1.9.0/example/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-13 18:33:01.000000 unipipeline-1.9.0/example/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)     1811 2022-06-22 10:47:54.000000 unipipeline-1.9.0/example/args.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.679588 unipipeline-1.9.0/example/brokers/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-05 14:14:23.000000 unipipeline-1.9.0/example/brokers/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      294 2022-06-06 14:43:02.000000 unipipeline-1.9.0/example/brokers/kafka_broker.py
--rw-rw-r--   0 master    (1000) master    (1000)      213 2022-06-06 14:43:02.000000 unipipeline-1.9.0/example/brokers/rmq_broker.py
--rw-rw-r--   0 master    (1000) master    (1000)       86 2021-11-22 19:50:31.000000 unipipeline-1.9.0/example/brokers/uni_log_broker.py
--rw-rw-r--   0 master    (1000) master    (1000)      299 2022-06-06 14:43:02.000000 unipipeline-1.9.0/example/example_consumer.py
--rw-rw-r--   0 master    (1000) master    (1000)      295 2022-06-07 10:55:34.000000 unipipeline-1.9.0/example/example_cron_producer.py
--rw-rw-r--   0 master    (1000) master    (1000)      281 2021-11-22 19:50:31.000000 unipipeline-1.9.0/example/example_csi.py
--rw-rw-r--   0 master    (1000) master    (1000)      776 2022-08-17 09:07:38.000000 unipipeline-1.9.0/example/example_producer.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/example/messages/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-05 14:14:23.000000 unipipeline-1.9.0/example/messages/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      115 2021-11-22 19:50:31.000000 unipipeline-1.9.0/example/messages/ender_after_answer_message.py
--rw-rw-r--   0 master    (1000) master    (1000)      135 2022-06-13 15:46:45.000000 unipipeline-1.9.0/example/messages/ender_after_cron_answer_message.py
--rw-rw-r--   0 master    (1000) master    (1000)      133 2022-06-13 15:46:17.000000 unipipeline-1.9.0/example/messages/ender_after_cron_input_message.py
--rw-rw-r--   0 master    (1000) master    (1000)      114 2021-11-22 19:50:31.000000 unipipeline-1.9.0/example/messages/ender_after_input_message.py
--rw-rw-r--   0 master    (1000) master    (1000)      118 2022-06-06 14:43:02.000000 unipipeline-1.9.0/example/messages/input_message.py
--rw-rw-r--   0 master    (1000) master    (1000)      111 2021-11-22 19:50:31.000000 unipipeline-1.9.0/example/messages/some_external_message.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/example/waitings/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-05 14:14:23.000000 unipipeline-1.9.0/example/waitings/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      142 2021-11-22 19:50:31.000000 unipipeline-1.9.0/example/waitings/common_db_wating.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/example/workers/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-24 20:36:10.000000 unipipeline-1.9.0/example/workers/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      407 2023-02-23 10:59:56.000000 unipipeline-1.9.0/example/workers/auto_retry_worker.py
--rw-rw-r--   0 master    (1000) master    (1000)      682 2022-06-13 15:46:56.000000 unipipeline-1.9.0/example/workers/ender_after_cron_worker.py
--rw-rw-r--   0 master    (1000) master    (1000)      672 2022-06-21 08:44:39.000000 unipipeline-1.9.0/example/workers/ender_after_input_worker.py
--rw-rw-r--   0 master    (1000) master    (1000)     1544 2023-04-29 16:22:20.000000 unipipeline-1.9.0/example/workers/input_worker.py
--rw-rw-r--   0 master    (1000) master    (1000)     1028 2022-06-13 15:49:23.000000 unipipeline-1.9.0/example/workers/my_super_cron_worker.py
--rw-rw-r--   0 master    (1000) master    (1000)       38 2023-04-29 18:20:25.683588 unipipeline-1.9.0/setup.cfg
--rwxrwxr-x   0 master    (1000) master    (1000)     1767 2023-04-29 18:20:06.000000 unipipeline-1.9.0/setup.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/unipipeline/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-11-22 19:50:31.000000 unipipeline-1.9.0/unipipeline/__init__.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/unipipeline/answer/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 21:16:22.000000 unipipeline-1.9.0/unipipeline/answer/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)     1503 2022-06-07 15:42:31.000000 unipipeline-1.9.0/unipipeline/answer/uni_answer_message.py
--rw-rw-r--   0 master    (1000) master    (1000)      210 2022-06-24 18:50:54.000000 unipipeline-1.9.0/unipipeline/answer/uni_answer_params.py
--rw-rw-r--   0 master    (1000) master    (1000)     5142 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/args.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/unipipeline/brokers/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-09 18:57:22.000000 unipipeline-1.9.0/unipipeline/brokers/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)    16198 2022-06-24 21:52:15.000000 unipipeline-1.9.0/unipipeline/brokers/uni_amqp_pika_broker.py
--rw-rw-r--   0 master    (1000) master    (1000)    26095 2023-04-29 15:19:17.000000 unipipeline-1.9.0/unipipeline/brokers/uni_amqp_py_broker.py
--rw-rw-r--   0 master    (1000) master    (1000)     4031 2022-06-24 18:01:25.000000 unipipeline-1.9.0/unipipeline/brokers/uni_broker.py
--rw-rw-r--   0 master    (1000) master    (1000)      306 2022-06-24 20:56:59.000000 unipipeline-1.9.0/unipipeline/brokers/uni_broker_consumer.py
--rw-rw-r--   0 master    (1000) master    (1000)     6894 2023-04-29 16:21:17.000000 unipipeline-1.9.0/unipipeline/brokers/uni_kafka_broker.py
--rw-rw-r--   0 master    (1000) master    (1000)     1915 2022-06-06 14:43:02.000000 unipipeline-1.9.0/unipipeline/brokers/uni_log_broker.py
--rw-rw-r--   0 master    (1000) master    (1000)     7198 2022-06-24 21:10:13.000000 unipipeline-1.9.0/unipipeline/brokers/uni_memory_broker.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/unipipeline/config/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 21:04:47.000000 unipipeline-1.9.0/unipipeline/config/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)    21472 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/config/uni_config.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/unipipeline/definitions/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 21:12:24.000000 unipipeline-1.9.0/unipipeline/definitions/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      511 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/definitions/uni_broker_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)      276 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/definitions/uni_codec_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)     1243 2023-01-18 14:06:03.000000 unipipeline-1.9.0/unipipeline/definitions/uni_cron_task_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)      697 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/definitions/uni_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)      179 2022-06-06 16:36:07.000000 unipipeline-1.9.0/unipipeline/definitions/uni_dynamic_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)      161 2021-07-22 21:12:30.000000 unipipeline-1.9.0/unipipeline/definitions/uni_external_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)      232 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/definitions/uni_message_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)     5911 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/definitions/uni_module_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)      158 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/definitions/uni_service_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)     1128 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/definitions/uni_waiting_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)     1127 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/definitions/uni_worker_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)      846 2023-04-29 18:15:03.000000 unipipeline-1.9.0/unipipeline/errors.py
--rw-rw-r--   0 master    (1000) master    (1000)      132 2021-07-22 20:24:04.000000 unipipeline-1.9.0/unipipeline/main.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/unipipeline/message/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-24 21:16:55.000000 unipipeline-1.9.0/unipipeline/message/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      110 2021-07-22 21:11:39.000000 unipipeline-1.9.0/unipipeline/message/uni_cron_message.py
--rw-rw-r--   0 master    (1000) master    (1000)      116 2022-06-06 16:35:13.000000 unipipeline-1.9.0/unipipeline/message/uni_message.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/unipipeline/message_meta/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-24 21:16:55.000000 unipipeline-1.9.0/unipipeline/message_meta/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)     2794 2022-06-24 18:03:59.000000 unipipeline-1.9.0/unipipeline/message_meta/uni_message_meta.py
--rw-rw-r--   0 master    (1000) master    (1000)      340 2022-06-06 16:36:31.000000 unipipeline-1.9.0/unipipeline/message_meta/uni_message_meta_err.py
--rw-rw-r--   0 master    (1000) master    (1000)      328 2023-04-29 18:17:11.000000 unipipeline-1.9.0/unipipeline/message_meta/uni_message_meta_error_topic.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/unipipeline/modules/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-13 18:33:01.000000 unipipeline-1.9.0/unipipeline/modules/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      416 2021-11-17 17:34:03.000000 unipipeline-1.9.0/unipipeline/modules/test_uni_util.py
--rw-rw-r--   0 master    (1000) master    (1000)     5102 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/modules/uni.py
--rw-rw-r--   0 master    (1000) master    (1000)     2160 2022-06-22 14:13:58.000000 unipipeline-1.9.0/unipipeline/modules/uni_cron_job.py
--rw-rw-r--   0 master    (1000) master    (1000)    21881 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/modules/uni_mediator.py
--rw-rw-r--   0 master    (1000) master    (1000)        0 2022-07-25 03:22:44.000000 unipipeline-1.9.0/unipipeline/py.typed
--rw-rw-r--   0 master    (1000) master    (1000)     1515 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/run.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/unipipeline/utils/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-09 18:57:22.000000 unipipeline-1.9.0/unipipeline/utils/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      600 2021-07-22 20:24:04.000000 unipipeline-1.9.0/unipipeline/utils/complex_serializer.py
--rw-rw-r--   0 master    (1000) master    (1000)      111 2023-01-18 10:00:59.000000 unipipeline-1.9.0/unipipeline/utils/filter_camel.py
--rw-rw-r--   0 master    (1000) master    (1000)     2780 2022-06-07 15:42:12.000000 unipipeline-1.9.0/unipipeline/utils/sig.py
--rw-rw-r--   0 master    (1000) master    (1000)     2902 2021-07-22 21:03:59.000000 unipipeline-1.9.0/unipipeline/utils/uni_echo.py
--rw-rw-r--   0 master    (1000) master    (1000)      418 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/utils/uni_util.py
--rw-rw-r--   0 master    (1000) master    (1000)      737 2021-07-22 20:24:04.000000 unipipeline-1.9.0/unipipeline/utils/uni_util_color.py
--rw-rw-r--   0 master    (1000) master    (1000)      798 2021-07-22 20:24:04.000000 unipipeline-1.9.0/unipipeline/utils/uni_util_template.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/unipipeline/waiting/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 20:24:04.000000 unipipeline-1.9.0/unipipeline/waiting/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      780 2022-06-06 15:35:18.000000 unipipeline-1.9.0/unipipeline/waiting/uni_postgres_waiting.py
--rw-rw-r--   0 master    (1000) master    (1000)      133 2021-06-09 18:57:22.000000 unipipeline-1.9.0/unipipeline/waiting/uni_wating.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/unipipeline/worker/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 21:17:42.000000 unipipeline-1.9.0/unipipeline/worker/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      899 2022-06-24 18:49:23.000000 unipipeline-1.9.0/unipipeline/worker/uni_msg_params.py
--rw-rw-r--   0 master    (1000) master    (1000)      910 2022-06-06 14:43:02.000000 unipipeline-1.9.0/unipipeline/worker/uni_worker.py
--rw-rw-r--   0 master    (1000) master    (1000)     5272 2023-04-29 18:19:32.000000 unipipeline-1.9.0/unipipeline/worker/uni_worker_consumer.py
--rw-rw-r--   0 master    (1000) master    (1000)     1786 2023-04-29 18:05:31.000000 unipipeline-1.9.0/unipipeline/worker/uni_worker_consumer_manager.py
--rw-rw-r--   0 master    (1000) master    (1000)     1618 2023-04-29 18:10:58.000000 unipipeline-1.9.0/unipipeline/worker/uni_worker_consumer_message.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/unipipeline.egg-info/
--rw-rw-r--   0 master    (1000) master    (1000)    11100 2023-04-29 18:20:25.000000 unipipeline-1.9.0/unipipeline.egg-info/PKG-INFO
--rw-rw-r--   0 master    (1000) master    (1000)     3407 2023-04-29 18:20:25.000000 unipipeline-1.9.0/unipipeline.egg-info/SOURCES.txt
--rw-rw-r--   0 master    (1000) master    (1000)        1 2023-04-29 18:20:25.000000 unipipeline-1.9.0/unipipeline.egg-info/dependency_links.txt
--rw-rw-r--   0 master    (1000) master    (1000)       54 2023-04-29 18:20:25.000000 unipipeline-1.9.0/unipipeline.egg-info/entry_points.txt
--rw-rw-r--   0 master    (1000) master    (1000)        1 2022-07-25 03:30:28.000000 unipipeline-1.9.0/unipipeline.egg-info/not-zip-safe
--rw-rw-r--   0 master    (1000) master    (1000)      143 2023-04-29 18:20:25.000000 unipipeline-1.9.0/unipipeline.egg-info/requires.txt
--rw-rw-r--   0 master    (1000) master    (1000)       20 2023-04-29 18:20:25.000000 unipipeline-1.9.0/unipipeline.egg-info/top_level.txt
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-05-29 10:18:16.569828 unipipeline-1.9.1/
+-rwxrwxr-x   0 master    (1000) master    (1000)     1063 2022-08-17 09:07:38.000000 unipipeline-1.9.1/LICENSE
+-rw-rw-r--   0 master    (1000) master    (1000)    11100 2023-05-29 10:18:16.569828 unipipeline-1.9.1/PKG-INFO
+-rwxrwxr-x   0 master    (1000) master    (1000)    10229 2022-08-17 09:07:38.000000 unipipeline-1.9.1/README.md
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-05-29 10:18:16.565828 unipipeline-1.9.1/example/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-13 18:33:01.000000 unipipeline-1.9.1/example/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1811 2022-06-22 10:47:54.000000 unipipeline-1.9.1/example/args.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-05-29 10:18:16.565828 unipipeline-1.9.1/example/brokers/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-05 14:14:23.000000 unipipeline-1.9.1/example/brokers/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      294 2022-06-06 14:43:02.000000 unipipeline-1.9.1/example/brokers/kafka_broker.py
+-rw-rw-r--   0 master    (1000) master    (1000)      213 2022-06-06 14:43:02.000000 unipipeline-1.9.1/example/brokers/rmq_broker.py
+-rw-rw-r--   0 master    (1000) master    (1000)       86 2021-11-22 19:50:31.000000 unipipeline-1.9.1/example/brokers/uni_log_broker.py
+-rw-rw-r--   0 master    (1000) master    (1000)      299 2022-06-06 14:43:02.000000 unipipeline-1.9.1/example/example_consumer.py
+-rw-rw-r--   0 master    (1000) master    (1000)      295 2022-06-07 10:55:34.000000 unipipeline-1.9.1/example/example_cron_producer.py
+-rw-rw-r--   0 master    (1000) master    (1000)      281 2021-11-22 19:50:31.000000 unipipeline-1.9.1/example/example_csi.py
+-rw-rw-r--   0 master    (1000) master    (1000)      776 2022-08-17 09:07:38.000000 unipipeline-1.9.1/example/example_producer.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-05-29 10:18:16.565828 unipipeline-1.9.1/example/messages/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-05 14:14:23.000000 unipipeline-1.9.1/example/messages/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      115 2021-11-22 19:50:31.000000 unipipeline-1.9.1/example/messages/ender_after_answer_message.py
+-rw-rw-r--   0 master    (1000) master    (1000)      135 2022-06-13 15:46:45.000000 unipipeline-1.9.1/example/messages/ender_after_cron_answer_message.py
+-rw-rw-r--   0 master    (1000) master    (1000)      133 2022-06-13 15:46:17.000000 unipipeline-1.9.1/example/messages/ender_after_cron_input_message.py
+-rw-rw-r--   0 master    (1000) master    (1000)      114 2021-11-22 19:50:31.000000 unipipeline-1.9.1/example/messages/ender_after_input_message.py
+-rw-rw-r--   0 master    (1000) master    (1000)      118 2022-06-06 14:43:02.000000 unipipeline-1.9.1/example/messages/input_message.py
+-rw-rw-r--   0 master    (1000) master    (1000)      111 2021-11-22 19:50:31.000000 unipipeline-1.9.1/example/messages/some_external_message.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-05-29 10:18:16.565828 unipipeline-1.9.1/example/waitings/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-05 14:14:23.000000 unipipeline-1.9.1/example/waitings/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      142 2021-11-22 19:50:31.000000 unipipeline-1.9.1/example/waitings/common_db_wating.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-05-29 10:18:16.565828 unipipeline-1.9.1/example/workers/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-24 20:36:10.000000 unipipeline-1.9.1/example/workers/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      407 2023-02-23 10:59:56.000000 unipipeline-1.9.1/example/workers/auto_retry_worker.py
+-rw-rw-r--   0 master    (1000) master    (1000)      682 2022-06-13 15:46:56.000000 unipipeline-1.9.1/example/workers/ender_after_cron_worker.py
+-rw-rw-r--   0 master    (1000) master    (1000)      840 2023-05-23 11:30:33.000000 unipipeline-1.9.1/example/workers/ender_after_input_worker.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1544 2023-04-29 16:22:20.000000 unipipeline-1.9.1/example/workers/input_worker.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1028 2022-06-13 15:49:23.000000 unipipeline-1.9.1/example/workers/my_super_cron_worker.py
+-rw-rw-r--   0 master    (1000) master    (1000)       38 2023-05-29 10:18:16.569828 unipipeline-1.9.1/setup.cfg
+-rwxrwxr-x   0 master    (1000) master    (1000)     1767 2023-05-29 10:17:57.000000 unipipeline-1.9.1/setup.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-05-29 10:18:16.565828 unipipeline-1.9.1/unipipeline/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-11-22 19:50:31.000000 unipipeline-1.9.1/unipipeline/__init__.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-05-29 10:18:16.565828 unipipeline-1.9.1/unipipeline/answer/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 21:16:22.000000 unipipeline-1.9.1/unipipeline/answer/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1503 2022-06-07 15:42:31.000000 unipipeline-1.9.1/unipipeline/answer/uni_answer_message.py
+-rw-rw-r--   0 master    (1000) master    (1000)      210 2022-06-24 18:50:54.000000 unipipeline-1.9.1/unipipeline/answer/uni_answer_params.py
+-rw-rw-r--   0 master    (1000) master    (1000)     5142 2023-02-22 10:34:17.000000 unipipeline-1.9.1/unipipeline/args.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-05-29 10:18:16.565828 unipipeline-1.9.1/unipipeline/brokers/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-09 18:57:22.000000 unipipeline-1.9.1/unipipeline/brokers/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)    16198 2022-06-24 21:52:15.000000 unipipeline-1.9.1/unipipeline/brokers/uni_amqp_pika_broker.py
+-rw-rw-r--   0 master    (1000) master    (1000)    26758 2023-05-24 09:41:45.000000 unipipeline-1.9.1/unipipeline/brokers/uni_amqp_py_broker.py
+-rw-rw-r--   0 master    (1000) master    (1000)     4031 2022-06-24 18:01:25.000000 unipipeline-1.9.1/unipipeline/brokers/uni_broker.py
+-rw-rw-r--   0 master    (1000) master    (1000)      306 2022-06-24 20:56:59.000000 unipipeline-1.9.1/unipipeline/brokers/uni_broker_consumer.py
+-rw-rw-r--   0 master    (1000) master    (1000)     6894 2023-04-29 16:21:17.000000 unipipeline-1.9.1/unipipeline/brokers/uni_kafka_broker.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1915 2022-06-06 14:43:02.000000 unipipeline-1.9.1/unipipeline/brokers/uni_log_broker.py
+-rw-rw-r--   0 master    (1000) master    (1000)     7198 2022-06-24 21:10:13.000000 unipipeline-1.9.1/unipipeline/brokers/uni_memory_broker.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-05-29 10:18:16.565828 unipipeline-1.9.1/unipipeline/config/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 21:04:47.000000 unipipeline-1.9.1/unipipeline/config/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)    21472 2023-02-22 10:34:17.000000 unipipeline-1.9.1/unipipeline/config/uni_config.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-05-29 10:18:16.565828 unipipeline-1.9.1/unipipeline/definitions/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 21:12:24.000000 unipipeline-1.9.1/unipipeline/definitions/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      511 2023-02-22 10:34:17.000000 unipipeline-1.9.1/unipipeline/definitions/uni_broker_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)      276 2023-02-22 10:34:17.000000 unipipeline-1.9.1/unipipeline/definitions/uni_codec_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1243 2023-01-18 14:06:03.000000 unipipeline-1.9.1/unipipeline/definitions/uni_cron_task_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)      697 2023-02-22 10:34:17.000000 unipipeline-1.9.1/unipipeline/definitions/uni_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)      179 2022-06-06 16:36:07.000000 unipipeline-1.9.1/unipipeline/definitions/uni_dynamic_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)      161 2021-07-22 21:12:30.000000 unipipeline-1.9.1/unipipeline/definitions/uni_external_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)      232 2023-02-22 10:34:17.000000 unipipeline-1.9.1/unipipeline/definitions/uni_message_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)     5911 2023-02-22 10:34:17.000000 unipipeline-1.9.1/unipipeline/definitions/uni_module_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)      158 2023-02-22 10:34:17.000000 unipipeline-1.9.1/unipipeline/definitions/uni_service_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1128 2023-02-22 10:34:17.000000 unipipeline-1.9.1/unipipeline/definitions/uni_waiting_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1127 2023-02-22 10:34:17.000000 unipipeline-1.9.1/unipipeline/definitions/uni_worker_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)      846 2023-04-29 18:15:03.000000 unipipeline-1.9.1/unipipeline/errors.py
+-rw-rw-r--   0 master    (1000) master    (1000)      132 2021-07-22 20:24:04.000000 unipipeline-1.9.1/unipipeline/main.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-05-29 10:18:16.565828 unipipeline-1.9.1/unipipeline/message/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-24 21:16:55.000000 unipipeline-1.9.1/unipipeline/message/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      110 2021-07-22 21:11:39.000000 unipipeline-1.9.1/unipipeline/message/uni_cron_message.py
+-rw-rw-r--   0 master    (1000) master    (1000)      116 2022-06-06 16:35:13.000000 unipipeline-1.9.1/unipipeline/message/uni_message.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-05-29 10:18:16.565828 unipipeline-1.9.1/unipipeline/message_meta/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-24 21:16:55.000000 unipipeline-1.9.1/unipipeline/message_meta/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)     2794 2022-06-24 18:03:59.000000 unipipeline-1.9.1/unipipeline/message_meta/uni_message_meta.py
+-rw-rw-r--   0 master    (1000) master    (1000)      340 2022-06-06 16:36:31.000000 unipipeline-1.9.1/unipipeline/message_meta/uni_message_meta_err.py
+-rw-rw-r--   0 master    (1000) master    (1000)      328 2023-04-29 18:17:11.000000 unipipeline-1.9.1/unipipeline/message_meta/uni_message_meta_error_topic.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-05-29 10:18:16.565828 unipipeline-1.9.1/unipipeline/modules/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-13 18:33:01.000000 unipipeline-1.9.1/unipipeline/modules/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      416 2021-11-17 17:34:03.000000 unipipeline-1.9.1/unipipeline/modules/test_uni_util.py
+-rw-rw-r--   0 master    (1000) master    (1000)     5102 2023-02-22 10:34:17.000000 unipipeline-1.9.1/unipipeline/modules/uni.py
+-rw-rw-r--   0 master    (1000) master    (1000)     2160 2022-06-22 14:13:58.000000 unipipeline-1.9.1/unipipeline/modules/uni_cron_job.py
+-rw-rw-r--   0 master    (1000) master    (1000)    21967 2023-05-23 10:35:54.000000 unipipeline-1.9.1/unipipeline/modules/uni_mediator.py
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2022-07-25 03:22:44.000000 unipipeline-1.9.1/unipipeline/py.typed
+-rw-rw-r--   0 master    (1000) master    (1000)     1515 2023-02-22 10:34:17.000000 unipipeline-1.9.1/unipipeline/run.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-05-29 10:18:16.569828 unipipeline-1.9.1/unipipeline/utils/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-09 18:57:22.000000 unipipeline-1.9.1/unipipeline/utils/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      600 2021-07-22 20:24:04.000000 unipipeline-1.9.1/unipipeline/utils/complex_serializer.py
+-rw-rw-r--   0 master    (1000) master    (1000)      111 2023-01-18 10:00:59.000000 unipipeline-1.9.1/unipipeline/utils/filter_camel.py
+-rw-rw-r--   0 master    (1000) master    (1000)     2780 2022-06-07 15:42:12.000000 unipipeline-1.9.1/unipipeline/utils/sig.py
+-rw-rw-r--   0 master    (1000) master    (1000)     2902 2021-07-22 21:03:59.000000 unipipeline-1.9.1/unipipeline/utils/uni_echo.py
+-rw-rw-r--   0 master    (1000) master    (1000)      418 2023-02-22 10:34:17.000000 unipipeline-1.9.1/unipipeline/utils/uni_util.py
+-rw-rw-r--   0 master    (1000) master    (1000)      737 2021-07-22 20:24:04.000000 unipipeline-1.9.1/unipipeline/utils/uni_util_color.py
+-rw-rw-r--   0 master    (1000) master    (1000)      798 2021-07-22 20:24:04.000000 unipipeline-1.9.1/unipipeline/utils/uni_util_template.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-05-29 10:18:16.569828 unipipeline-1.9.1/unipipeline/waiting/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 20:24:04.000000 unipipeline-1.9.1/unipipeline/waiting/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      780 2022-06-06 15:35:18.000000 unipipeline-1.9.1/unipipeline/waiting/uni_postgres_waiting.py
+-rw-rw-r--   0 master    (1000) master    (1000)      133 2021-06-09 18:57:22.000000 unipipeline-1.9.1/unipipeline/waiting/uni_wating.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-05-29 10:18:16.569828 unipipeline-1.9.1/unipipeline/worker/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 21:17:42.000000 unipipeline-1.9.1/unipipeline/worker/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      899 2022-06-24 18:49:23.000000 unipipeline-1.9.1/unipipeline/worker/uni_msg_params.py
+-rw-rw-r--   0 master    (1000) master    (1000)      910 2022-06-06 14:43:02.000000 unipipeline-1.9.1/unipipeline/worker/uni_worker.py
+-rw-rw-r--   0 master    (1000) master    (1000)     5375 2023-05-23 11:12:41.000000 unipipeline-1.9.1/unipipeline/worker/uni_worker_consumer.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1786 2023-04-29 18:05:31.000000 unipipeline-1.9.1/unipipeline/worker/uni_worker_consumer_manager.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1618 2023-04-29 18:10:58.000000 unipipeline-1.9.1/unipipeline/worker/uni_worker_consumer_message.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-05-29 10:18:16.565828 unipipeline-1.9.1/unipipeline.egg-info/
+-rw-rw-r--   0 master    (1000) master    (1000)    11100 2023-05-29 10:18:16.000000 unipipeline-1.9.1/unipipeline.egg-info/PKG-INFO
+-rw-rw-r--   0 master    (1000) master    (1000)     3407 2023-05-29 10:18:16.000000 unipipeline-1.9.1/unipipeline.egg-info/SOURCES.txt
+-rw-rw-r--   0 master    (1000) master    (1000)        1 2023-05-29 10:18:16.000000 unipipeline-1.9.1/unipipeline.egg-info/dependency_links.txt
+-rw-rw-r--   0 master    (1000) master    (1000)       54 2023-05-29 10:18:16.000000 unipipeline-1.9.1/unipipeline.egg-info/entry_points.txt
+-rw-rw-r--   0 master    (1000) master    (1000)        1 2022-07-25 03:30:28.000000 unipipeline-1.9.1/unipipeline.egg-info/not-zip-safe
+-rw-rw-r--   0 master    (1000) master    (1000)      143 2023-05-29 10:18:16.000000 unipipeline-1.9.1/unipipeline.egg-info/requires.txt
+-rw-rw-r--   0 master    (1000) master    (1000)       20 2023-05-29 10:18:16.000000 unipipeline-1.9.1/unipipeline.egg-info/top_level.txt
```

### Comparing `unipipeline-1.9.0/LICENSE` & `unipipeline-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/PKG-INFO` & `unipipeline-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unipipeline
-Version: 1.9.0
+Version: 1.9.1
 Summary: simple way to build the declarative and distributed data pipelines with python. it supports rabbitmq or kafka as a broker
 Home-page: https://github.com/aliaksandr-master/unipipeline
 Author: Aliaksandr Master
 Author-email: alxe.master@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `unipipeline-1.9.0/README.md` & `unipipeline-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/example/args.py` & `unipipeline-1.9.1/example/args.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/example/example_producer.py` & `unipipeline-1.9.1/example/example_producer.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/example/workers/ender_after_cron_worker.py` & `unipipeline-1.9.1/example/workers/ender_after_cron_worker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/example/workers/input_worker.py` & `unipipeline-1.9.1/example/workers/input_worker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/example/workers/my_super_cron_worker.py` & `unipipeline-1.9.1/example/workers/my_super_cron_worker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/setup.py` & `unipipeline-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="unipipeline",
-    version="1.9.0",
+    version="1.9.1",
     description="simple way to build the declarative and distributed data pipelines with python. it supports rabbitmq or kafka as a broker",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aliaksandr-master/unipipeline",
     author="Aliaksandr Master",
     author_email="alxe.master@gmail.com",
     license="MIT",
```

### Comparing `unipipeline-1.9.0/unipipeline/answer/uni_answer_message.py` & `unipipeline-1.9.1/unipipeline/answer/uni_answer_message.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/args.py` & `unipipeline-1.9.1/unipipeline/args.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/brokers/uni_amqp_pika_broker.py` & `unipipeline-1.9.1/unipipeline/brokers/uni_amqp_pika_broker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/brokers/uni_amqp_py_broker.py` & `unipipeline-1.9.1/unipipeline/brokers/uni_amqp_py_broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
     def _get_topic_approximate_messages_count(self, ch: amqp.Channel, topic: str) -> int:
         result = ch.queue_declare(queue=topic, passive=True)
         self.echo.log_debug(f'topic "{topic}" has messages={result.message_count}, consumers={result.consumer_count}')
         return int(result.message_count)
 
     def get_topic_approximate_messages_count(self, topic: str) -> int:
-        with self._channel() as get_ch:
+        with self._everytime_new_channel(close=True) as get_ch:
             return self._retry_net_interaction(
                 'get_topic_approximate_messages_count',
                 lambda has_error: self._get_topic_approximate_messages_count(get_ch(has_error), topic),
                 retryable_errors=PUBLISHING_RETRYABLE_ERRORS,
             )
 
     @classmethod
@@ -181,15 +181,30 @@
             ch = self.connected_connection.channel()
 
         self.echo.log_debug(f'channel {ch.channel_id} :: new')
 
         return now + float(self.config.heartbeat), ch
 
     @contextlib.contextmanager
-    def _channel(self, *, close: bool = False) -> Generator[Callable[[bool], amqp.Channel], Any, Any]:
+    def _everytime_new_channel(self, *, close: bool) -> Generator[Callable[[bool], amqp.Channel], Any, Any]:
+        c_to_close = []
+
+        def get_ch(force_new: bool) -> amqp.Channel:
+            current_c = self._get_or_create_or_del_free_channel()
+            c_to_close.append(current_c)
+            return current_c[1]
+
+        try:
+            yield get_ch
+        finally:
+            for c in c_to_close:
+                self._close_ch(c[1])
+
+    @contextlib.contextmanager
+    def _channel(self, *, close: bool) -> Generator[Callable[[bool], amqp.Channel], Any, Any]:
         c_to_close = []
         current_c = None
 
         def get_ch(force_new: bool) -> amqp.Channel:
             nonlocal current_c
             if force_new or current_c is None:
                 current_c = self._get_or_create_or_del_free_channel()
@@ -352,32 +367,31 @@
 
         def consumer_wrapper(ch: amqp.Channel, message: amqp.Message) -> None:
             key = f'consumer "{consumer.id}" :: channel "{ch.channel_id}" :: message "{message.delivery_tag}"'
             self._interacted()
             self._consumer_in_processing = True
             self.echo.log_debug(f'{key} :: received')
 
-            rejected = False
+            rejected = True
             try:
                 get_meta = functools.partial(
                     self.parse_message_body,
                     content=message.body,
                     compression=message.headers.get(BASIC_PROPERTIES__HEADER__COMPRESSION_KEY, None),
                     content_type=message.content_type,
                     unwrapped=consumer.unwrapped,
                 )
                 consumer.message_handler(get_meta)
+                rejected = False
             except UniMessageRejectError:
-                rejected = True
                 self.echo.log_debug(f'{key} :: reject :: started')
                 with self._interaction():
                     ch.basic_reject(delivery_tag=message.delivery_tag, requeue=True)
                 self.echo.log_debug(f'{key} :: reject :: done')
             except Exception as e: # noqa
-                rejected = True
                 traceback.print_exc()
                 self.echo.log_error(f'{key} :: {str(e)}')
                 raise
 
             if not rejected:
                 self.echo.log_debug(f'{key} :: ack :: started')
                 with self._interaction():
@@ -404,31 +418,32 @@
         if not self._heartbeat_enabled:
             return
         self._heartbeat_enabled = False
         if self._heartbeat_thread is not None:
             self.echo.log_debug('heartbeat :: disable')
             if self._heartbeat_thread.is_alive():
                 self._heartbeat_thread.join()
+                self.echo.log_debug('heartbeat :: thread joined')
             self._heartbeat_thread = None
         self.echo.log_debug('heartbeat :: disabled')
 
     def _start_heartbeat_tick(self) -> None:
         self._stop_heartbeat_tick()
         if self._heartbeat_enabled:
             return
         self._heartbeat_enabled = self._heartbeat_delay > 0
 
         if not self._heartbeat_enabled:
             return
 
         if self._heartbeat_thread is None:
             self._heartbeat_thread = threading.Thread(
-                name=f'broker-{self.definition.name}-system',
+                name=f'broker-{self.definition.name}-heartbeat',
                 target=self._heartbeat_loop_tick,
-                daemon=False,
+                daemon=True,
                 kwargs=dict(
                     delay_s=self._heartbeat_delay,
                     heartbeat_delay_threshold=self._heartbeat_delay,
                 ),
             )
 
         if not self._heartbeat_thread.is_alive():
@@ -447,15 +462,16 @@
             sum_steps = 0
             with self._lock_interaction:
                 current_delay = time.time() - self._last_interaction
 
             if current_delay < heartbeat_delay_threshold:
                 self.echo.log_debug(f'heartbeat :: skipped ({current_delay:0.2f}s > {heartbeat_delay_threshold:0.2f}s)')
                 continue
-
+            if not self._heartbeat_enabled:
+                break
             self.connected_connection.send_heartbeat()
             self.echo.log_debug(f'heartbeat :: tick (since last interaction {current_delay:0.2f}s)')
 
     def _consuming(self) -> None:
         if not self._consuming_enabled or len(self._consumers) == 0:
             self.echo.log_warning('start_consuming :: has no consumers to start consuming')
             self.stop_consuming()
@@ -533,15 +549,15 @@
             content_encoding='utf-8',
             delivery_mode=2 if self.config.persistent_message else 0,
             application_headers=headers,
             expiration=expiration,
         )
 
     def publish(self, topic: str, meta_list: List[UniMessageMeta], alone: bool = False) -> None:
-        with self._channel() as get_ch:
+        with self._everytime_new_channel(close=True) as get_ch:
             exchange, topic = self._retry_net_interaction(
                 'publish._init_topic',
                 lambda has_error: self._init_topic(get_ch(has_error), topic),
                 retryable_errors=PUBLISHING_RETRYABLE_ERRORS,
             )
 
             if self._retry_net_interaction(
@@ -556,15 +572,15 @@
                 self._retry_net_interaction(
                     'publish._publish_ch',
                     lambda has_error: self._publish_ch('publish', get_ch(has_error), exchange, topic, meta, props),
                     retryable_errors=PUBLISHING_RETRYABLE_ERRORS,
                 )
 
     def rpc_call(self, topic: str, meta: UniMessageMeta, *, alone: bool = False, max_delay_s: int = 1, unwrapped: bool = False) -> Optional[UniMessageMeta]:
-        with self._channel(close=True) as get_ch:
+        with self._everytime_new_channel(close=True) as get_ch:
             return self._retry_net_interaction(
                 'rpc_call',
                 lambda has_error: self._rpc_call(get_ch(has_error), topic, meta, alone=alone, max_delay_s=max_delay_s, unwrapped=unwrapped),
                 retryable_errors=PUBLISHING_RETRYABLE_ERRORS,
             )
 
     def _rpc_call(self, ch: amqp.Channel, topic: str, meta: UniMessageMeta, *, alone: bool = False, max_delay_s: int = 1, unwrapped: bool = False) -> Optional[UniMessageMeta]:
@@ -610,15 +626,15 @@
             content_type=self.definition.content_type,
             content_encoding='utf-8',
             delivery_mode=1,
             application_headers=headers,
             expiration=str(ttl_s * 1000) if ttl_s is not None else None,
         )
 
-        with self._channel() as get_ch:
+        with self._everytime_new_channel(close=True) as get_ch:
             self._retry_net_interaction(
                 'publish_answer._publish_ch',
                 lambda has_error: self._publish_ch('answer :: publish', get_ch(has_error), self.config.answer_exchange_name, self._mk_answer_topic(answer_params), meta, props),
                 retryable_errors=PUBLISHING_RETRYABLE_ERRORS,
             )
 
     def _mk_answer_topic(self, answer_params: UniAnswerParams) -> str:
```

### Comparing `unipipeline-1.9.0/unipipeline/brokers/uni_broker.py` & `unipipeline-1.9.1/unipipeline/brokers/uni_broker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/brokers/uni_kafka_broker.py` & `unipipeline-1.9.1/unipipeline/brokers/uni_kafka_broker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/brokers/uni_log_broker.py` & `unipipeline-1.9.1/unipipeline/brokers/uni_log_broker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/brokers/uni_memory_broker.py` & `unipipeline-1.9.1/unipipeline/brokers/uni_memory_broker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/config/uni_config.py` & `unipipeline-1.9.1/unipipeline/config/uni_config.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/definitions/uni_cron_task_definition.py` & `unipipeline-1.9.1/unipipeline/definitions/uni_cron_task_definition.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/definitions/uni_definition.py` & `unipipeline-1.9.1/unipipeline/definitions/uni_definition.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/definitions/uni_module_definition.py` & `unipipeline-1.9.1/unipipeline/definitions/uni_module_definition.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/definitions/uni_waiting_definition.py` & `unipipeline-1.9.1/unipipeline/definitions/uni_waiting_definition.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/definitions/uni_worker_definition.py` & `unipipeline-1.9.1/unipipeline/definitions/uni_worker_definition.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/errors.py` & `unipipeline-1.9.1/unipipeline/errors.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/message_meta/uni_message_meta.py` & `unipipeline-1.9.1/unipipeline/message_meta/uni_message_meta.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/modules/uni.py` & `unipipeline-1.9.1/unipipeline/modules/uni.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/modules/uni_cron_job.py` & `unipipeline-1.9.1/unipipeline/modules/uni_cron_job.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/modules/uni_mediator.py` & `unipipeline-1.9.1/unipipeline/modules/uni_mediator.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         self._echo.log_error(str(err))
         meta = meta.create_error_child(err_topic, err)
         br = self.get_broker(wd.broker.name)
         error_topic = wd.error_topic
         if error_topic == UniMessageMetaErrTopic.MESSAGE_PAYLOAD_ERR.value:
             error_topic = wd.error_payload_topic
         br.publish(error_topic, [meta])
+        self._echo.log_info(f'successfully moved message "{meta.id}" to error topic')
 
     def add_worker_to_consume_list(self, name: str) -> None:
         wd = self._config.workers[name]
         if wd.marked_as_external:
             raise OverflowError(f'your could not use worker "{name}" as consumer. it marked as external "{wd.external}"')
         self._consumers_list.add(name)
         self.echo.log_info(f'added consumer {name}')
```

### Comparing `unipipeline-1.9.0/unipipeline/run.py` & `unipipeline-1.9.1/unipipeline/run.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/utils/complex_serializer.py` & `unipipeline-1.9.1/unipipeline/utils/complex_serializer.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/utils/sig.py` & `unipipeline-1.9.1/unipipeline/utils/sig.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/utils/uni_echo.py` & `unipipeline-1.9.1/unipipeline/utils/uni_echo.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/utils/uni_util_color.py` & `unipipeline-1.9.1/unipipeline/utils/uni_util_color.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/utils/uni_util_template.py` & `unipipeline-1.9.1/unipipeline/utils/uni_util_template.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/waiting/uni_postgres_waiting.py` & `unipipeline-1.9.1/unipipeline/waiting/uni_postgres_waiting.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/worker/uni_msg_params.py` & `unipipeline-1.9.1/unipipeline/worker/uni_msg_params.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/worker/uni_worker.py` & `unipipeline-1.9.1/unipipeline/worker/uni_worker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/worker/uni_worker_consumer.py` & `unipipeline-1.9.1/unipipeline/worker/uni_worker_consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,16 +90,19 @@
             self._current_meta = None
             return
 
         except UniMessageRejectError as e:
             self._uni_echo.log_warning(f'rejected message {meta.id}')
             if e.rejection_exception is not None:
                 self._mediator.move_to_error_topic(self._definition, meta, UniMessageMetaErrTopic.USER_ERROR, e.rejection_exception)
-            self._current_meta = None
-            raise
+                self._current_meta = None
+                return  # JUST ACK
+            else:
+                self._current_meta = None
+                raise
 
         self._uni_echo.log_debug(f'processing successfully done {meta.id}')
         if meta.need_answer and self._definition.need_answer:
             try:
                 self._mediator.answer_to(self._definition.name, meta, result, unwrapped=self._definition.answer_unwrapped)
             except UniSendingToUndefinedWorkerError:
                 pass
```

### Comparing `unipipeline-1.9.0/unipipeline/worker/uni_worker_consumer_manager.py` & `unipipeline-1.9.1/unipipeline/worker/uni_worker_consumer_manager.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline/worker/uni_worker_consumer_message.py` & `unipipeline-1.9.1/unipipeline/worker/uni_worker_consumer_message.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.9.0/unipipeline.egg-info/PKG-INFO` & `unipipeline-1.9.1/unipipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unipipeline
-Version: 1.9.0
+Version: 1.9.1
 Summary: simple way to build the declarative and distributed data pipelines with python. it supports rabbitmq or kafka as a broker
 Home-page: https://github.com/aliaksandr-master/unipipeline
 Author: Aliaksandr Master
 Author-email: alxe.master@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `unipipeline-1.9.0/unipipeline.egg-info/SOURCES.txt` & `unipipeline-1.9.1/unipipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

