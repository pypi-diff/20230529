# Comparing `tmp/aos_prov-4.0.2b3-py3-none-any.whl.zip` & `tmp/aos_prov-4.1.0b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,58 +1,38 @@
-Zip file size: 64410 bytes, number of entries: 56
+Zip file size: 32473 bytes, number of entries: 36
 -rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/__init__.py
 -rw-rw-r--  2.0 unx     2842 b- defN 23-Apr-04 10:59 aos_prov/actions.py
--rw-rw-r--  2.0 unx     7325 b- defN 23-May-23 08:08 aos_prov/main.py
+-rw-rw-r--  2.0 unx     7314 b- defN 23-May-25 16:51 aos_prov/main.py
 -rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/commands/__init__.py
--rw-rw-r--  2.0 unx     7501 b- defN 23-Apr-04 10:59 aos_prov/commands/command_provision.py
+-rw-rw-r--  2.0 unx     5861 b- defN 23-May-25 16:52 aos_prov/commands/command_provision.py
 -rw-rw-r--  2.0 unx     9689 b- defN 23-Apr-04 10:59 aos_prov/commands/command_vm_multi_node_manage.py
 -rw-rw-r--  2.0 unx     3799 b- defN 23-Apr-04 10:59 aos_prov/commands/download.py
 -rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/communication/__init__.py
 -rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/communication/cloud/__init__.py
--rw-rw-r--  2.0 unx     8552 b- defN 23-Apr-04 10:59 aos_prov/communication/cloud/cloud_api.py
+-rw-rw-r--  2.0 unx     8549 b- defN 23-May-25 16:53 aos_prov/communication/cloud/cloud_api.py
 -rw-rw-r--  2.0 unx       89 b- defN 22-Apr-10 14:06 aos_prov/communication/unit/__init__.py
 -rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v0/__init__.py
--rw-rw-r--  2.0 unx     5222 b- defN 23-Apr-04 10:59 aos_prov/communication/unit/v0/unit_communication.py
--rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v0/generated/__init__.py
--rw-rw-r--  2.0 unx    28704 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2.py
--rw-rw-r--  2.0 unx    20182 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2_grpc.py
 -rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v1/__init__.py
--rw-rw-r--  2.0 unx     6382 b- defN 23-Apr-04 10:59 aos_prov/communication/unit/v1/unit_communication_v1.py
--rw-rw-r--  2.0 unx       89 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v1/generated/__init__.py
--rw-rw-r--  2.0 unx     5409 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v1/generated/iamanagercommon_pb2.py
--rw-rw-r--  2.0 unx      159 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v1/generated/iamanagercommon_pb2_grpc.py
--rw-rw-r--  2.0 unx    31002 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v1/generated/iamanagerprotected_pb2.py
--rw-rw-r--  2.0 unx    19810 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v1/generated/iamanagerprotected_pb2_grpc.py
--rw-rw-r--  2.0 unx     9075 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2.py
--rw-rw-r--  2.0 unx     7934 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2_grpc.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v2/__init__.py
--rw-rw-r--  2.0 unx     6713 b- defN 23-Apr-04 10:59 aos_prov/communication/unit/v2/unit_communication_v2.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v2/generated/__init__.py
--rw-rw-r--  2.0 unx     5409 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v2/generated/iamanagercommon_pb2.py
--rw-rw-r--  2.0 unx      159 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v2/generated/iamanagercommon_pb2_grpc.py
--rw-rw-r--  2.0 unx    24470 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2.py
--rw-rw-r--  2.0 unx    16454 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2_grpc.py
--rw-rw-r--  2.0 unx    17266 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2.py
--rw-rw-r--  2.0 unx    12904 b- defN 22-Nov-13 13:27 aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2_grpc.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Dec-01 17:44 aos_prov/communication/unit/v4/__init__.py
--rw-rw-r--  2.0 unx     9592 b- defN 23-Apr-04 10:59 aos_prov/communication/unit/v4/unit_communication_v4.py
+-rw-rw-r--  2.0 unx     9583 b- defN 23-May-25 17:01 aos_prov/communication/unit/v4/unit_communication_v4.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Dec-01 17:44 aos_prov/communication/unit/v4/generated/__init__.py
 -rw-rw-r--  2.0 unx    18433 b- defN 22-Dec-01 17:44 aos_prov/communication/unit/v4/generated/iamanager_pb2.py
 -rw-rw-r--  2.0 unx    33405 b- defN 22-Dec-01 17:44 aos_prov/communication/unit/v4/generated/iamanager_pb2_grpc.py
 -rw-rw-r--  2.0 unx     2705 b- defN 22-Apr-10 14:06 aos_prov/files/1rootCA.crt
 -rw-rw-r--  2.0 unx      748 b- defN 22-Nov-13 13:27 aos_prov/utils/__init__.py
 -rw-rw-r--  2.0 unx     1649 b- defN 23-Apr-04 10:59 aos_prov/utils/common.py
--rw-rw-r--  2.0 unx     2591 b- defN 22-Dec-01 17:44 aos_prov/utils/config.py
--rw-rw-r--  2.0 unx      501 b- defN 22-Nov-13 13:27 aos_prov/utils/errors.py
+-rw-rw-r--  2.0 unx     2579 b- defN 23-May-25 16:54 aos_prov/utils/config.py
+-rw-rw-r--  2.0 unx      468 b- defN 23-May-25 16:47 aos_prov/utils/errors.py
 -rw-rw-r--  2.0 unx     1176 b- defN 22-Dec-01 17:44 aos_prov/utils/unit_certificate.py
 -rw-rw-r--  2.0 unx     7475 b- defN 23-Apr-04 10:59 aos_prov/utils/user_credentials.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-13 13:27 test/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-13 13:27 test/utils/__init__.py
 -rw-rw-r--  2.0 unx      642 b- defN 22-Dec-01 17:44 test/utils/test_config.py
 -rw-rw-r--  2.0 unx      632 b- defN 22-Dec-01 17:44 test/utils/test_unit_certificate.py
 -rw-rw-r--  2.0 unx      439 b- defN 22-Nov-13 13:27 test/utils/test_user_credentials.py
--rw-rw-r--  2.0 unx     2484 b- defN 23-May-23 16:49 aos_prov-4.0.2b3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-23 16:49 aos_prov-4.0.2b3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       48 b- defN 23-May-23 16:49 aos_prov-4.0.2b3.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       14 b- defN 23-May-23 16:49 aos_prov-4.0.2b3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5618 b- defN 23-May-23 16:49 aos_prov-4.0.2b3.dist-info/RECORD
-56 files, 346007 bytes uncompressed, 55094 bytes compressed:  84.1%
+-rw-rw-r--  2.0 unx     2484 b- defN 23-May-29 17:22 aos_prov-4.1.0b1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-29 17:22 aos_prov-4.1.0b1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       48 b- defN 23-May-29 17:22 aos_prov-4.1.0b1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       14 b- defN 23-May-29 17:22 aos_prov-4.1.0b1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3216 b- defN 23-May-29 17:22 aos_prov-4.1.0b1.dist-info/RECORD
+36 files, 124465 bytes uncompressed, 27203 bytes compressed:  78.1%
```

## zipnote {}

```diff
@@ -30,80 +30,20 @@
 
 Filename: aos_prov/communication/unit/__init__.py
 Comment: 
 
 Filename: aos_prov/communication/unit/v0/__init__.py
 Comment: 
 
-Filename: aos_prov/communication/unit/v0/unit_communication.py
-Comment: 
-
-Filename: aos_prov/communication/unit/v0/generated/__init__.py
-Comment: 
-
-Filename: aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2.py
-Comment: 
-
-Filename: aos_prov/communication/unit/v0/generated/api_iamanager_iamanager_pb2_grpc.py
-Comment: 
-
 Filename: aos_prov/communication/unit/v1/__init__.py
 Comment: 
 
-Filename: aos_prov/communication/unit/v1/unit_communication_v1.py
-Comment: 
-
-Filename: aos_prov/communication/unit/v1/generated/__init__.py
-Comment: 
-
-Filename: aos_prov/communication/unit/v1/generated/iamanagercommon_pb2.py
-Comment: 
-
-Filename: aos_prov/communication/unit/v1/generated/iamanagercommon_pb2_grpc.py
-Comment: 
-
-Filename: aos_prov/communication/unit/v1/generated/iamanagerprotected_pb2.py
-Comment: 
-
-Filename: aos_prov/communication/unit/v1/generated/iamanagerprotected_pb2_grpc.py
-Comment: 
-
-Filename: aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2.py
-Comment: 
-
-Filename: aos_prov/communication/unit/v1/generated/iamanagerpublic_pb2_grpc.py
-Comment: 
-
 Filename: aos_prov/communication/unit/v2/__init__.py
 Comment: 
 
-Filename: aos_prov/communication/unit/v2/unit_communication_v2.py
-Comment: 
-
-Filename: aos_prov/communication/unit/v2/generated/__init__.py
-Comment: 
-
-Filename: aos_prov/communication/unit/v2/generated/iamanagercommon_pb2.py
-Comment: 
-
-Filename: aos_prov/communication/unit/v2/generated/iamanagercommon_pb2_grpc.py
-Comment: 
-
-Filename: aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2.py
-Comment: 
-
-Filename: aos_prov/communication/unit/v2/generated/iamanagerprotected_pb2_grpc.py
-Comment: 
-
-Filename: aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2.py
-Comment: 
-
-Filename: aos_prov/communication/unit/v2/generated/iamanagerpublic_pb2_grpc.py
-Comment: 
-
 Filename: aos_prov/communication/unit/v4/__init__.py
 Comment: 
 
 Filename: aos_prov/communication/unit/v4/unit_communication_v4.py
 Comment: 
 
 Filename: aos_prov/communication/unit/v4/generated/__init__.py
@@ -147,23 +87,23 @@
 
 Filename: test/utils/test_unit_certificate.py
 Comment: 
 
 Filename: test/utils/test_user_credentials.py
 Comment: 
 
-Filename: aos_prov-4.0.2b3.dist-info/METADATA
+Filename: aos_prov-4.1.0b1.dist-info/METADATA
 Comment: 
 
-Filename: aos_prov-4.0.2b3.dist-info/WHEEL
+Filename: aos_prov-4.1.0b1.dist-info/WHEEL
 Comment: 
 
-Filename: aos_prov-4.0.2b3.dist-info/entry_points.txt
+Filename: aos_prov-4.1.0b1.dist-info/entry_points.txt
 Comment: 
 
-Filename: aos_prov-4.0.2b3.dist-info/top_level.txt
+Filename: aos_prov-4.1.0b1.dist-info/top_level.txt
 Comment: 
 
-Filename: aos_prov-4.0.2b3.dist-info/RECORD
+Filename: aos_prov-4.1.0b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aos_prov/main.py

```diff
@@ -8,15 +8,15 @@
 import sys
 from pathlib import Path
 
 from aos_prov.actions import create_new_unit, download_image, provision_unit, start_vm
 from aos_prov.communication.cloud.cloud_api import DEFAULT_REGISTER_PORT, CloudAPI
 from aos_prov.utils import DEFAULT_USER_CERT_PATH, DEFAULT_USER_KEY_PATH
 from aos_prov.utils.common import DISK_IMAGE_DOWNLOAD_URL, AOS_DISKS_PATH, print_error
-from aos_prov.utils.errors import CloudAccessError, BoardError, DeviceRegisterError, OnBoardingError
+from aos_prov.utils.errors import CloudAccessError, UnitError, DeviceRegisterError, OnUnitError
 from aos_prov.utils.user_credentials import UserCredentials
 
 try:
     from importlib.metadata import version  # noqa: WPS433
 except ImportError:
     import importlib_metadata as version  # noqa: WPS433
 
@@ -33,15 +33,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 def _parse_args():
     parser = argparse.ArgumentParser(
         prog='aos-prov',
-        description="The board provisioning tool using gRPC protocol",
+        description="The unit provisioning tool using gRPC protocol",
         epilog="Run 'aos-prov --help' for more information about commands, "
                "or 'aos-prov COMMAND --help' to see info about command about desired command")
 
     parser.add_argument(
         '-u',
         '--unit',
         required=False,
@@ -233,18 +233,18 @@
 
     except CloudAccessError as e:
         print_error(f"Failed during communication with the AosCloud with error: {str(e)}")
         status = 1
     except DeviceRegisterError as e:
         print_error(f"FAILED with error: {str(e)}")
         status = 1
-    except BoardError as e:
+    except UnitError as e:
         print_error(f'Failed during communication with device with error: \n {str(e)}')
         status = 1
-    except OnBoardingError as e:
+    except OnUnitError as e:
         print_error('Failed to execute the command!')
         print_error(f'Error: {str(e)} ')
         status = 1
     except (AssertionError, KeyboardInterrupt):
         print_error('Stopped by keyboard...')
         status = 1
```

## aos_prov/commands/command_provision.py

```diff
@@ -3,21 +3,18 @@
 #  Copyright (c) 2018-2022 EPAM Systems Inc.
 #
 """Provision unit."""
 
 import time
 
 from aos_prov.communication.cloud.cloud_api import CloudAPI
-from aos_prov.communication.unit.v0.unit_communication import UnitCommunication
-from aos_prov.communication.unit.v1.unit_communication_v1 import UnitCommunicationV1
-from aos_prov.communication.unit.v2.unit_communication_v2 import UnitCommunicationV2
 from aos_prov.communication.unit.v4.unit_communication_v4 import UnitCommunicationV4
 from aos_prov.utils.common import generate_random_password, print_message
 from aos_prov.utils.config import Config
-from aos_prov.utils.errors import GrpcUnimplemented, BoardError
+from aos_prov.utils.errors import GrpcUnimplemented, UnitError
 
 COMMAND_TO_DECRYPT = 'diskencryption'
 
 
 def run_provision(unit_address: str, cloud_api: CloudAPI, reconnect_times: int = 1):
     """
     Provision Unit. This function will try to provision starting from the newest to the oldest.
@@ -31,49 +28,30 @@
         AosProvError: If provision fails.
     """
     config = Config()
     uc = UnitCommunicationV4(unit_address)
     model_name = ''
     for retry in range(reconnect_times):
         try:
-            print_message('Starting provisioning using protocol v4....')
+            print_message('Starting provisioning...')
             config.system_id, model_name = uc.get_system_info()
             config.protocol_version = uc.get_protocol_version()
             break
-        except GrpcUnimplemented:
-            try:
-                print_message('v4 is not supported. Starting provisioning using protocol v2...')
-                uc = UnitCommunicationV2(unit_address)
-                if uc.get_protocol_version() == 3:
-                    uc.need_set_users = False
-                config.system_id, model_name = uc.get_system_info()
-                config.protocol_version = uc.get_protocol_version()
-                break
-            except GrpcUnimplemented:
-                try:
-                    print_message('v2 is not supported. Using protocol v1')
-                    uc = UnitCommunicationV1(unit_address)
-                    config.system_id, model_name = uc.get_system_info()
-                    config.protocol_version = uc.get_protocol_version()
-                    break
-                except GrpcUnimplemented:
-                    print_message('v1 is not supported. Using protocol v0')
-                    uc = UnitCommunication(unit_address)
-                    config.system_id, model_name = uc.get_system_info()
-                    config.protocol_version = uc.get_protocol_version()
-                    break
-        except BoardError as be:
+        except GrpcUnimplemented as gu:
+            print_message(f'[red]Grpc protocol error: {gu}.')
+            raise gu
+        except UnitError as be:
             print_message('[yellow]Connection failed')
             if retry + 1 < reconnect_times:
                 time.sleep(5)
             else:
                 raise be
 
     if config.system_id is None:
-        raise BoardError('Cannot read system_id')
+        raise UnitError('Cannot read system_id')
 
     config.set_model(model_name)
     cloud_api.check_unit_is_not_provisioned(config.system_id)
     if config.protocol_version >= 4:  # support of multi domains
         config.node_ids = uc.get_all_node_ids()
         for node_id in config.node_ids:
             config.supported_cert_types = uc.get_cert_types(node_id)
@@ -116,27 +94,20 @@
 
         for cert_type in config.supported_cert_types:
             config.unit_certificates.append(uc.create_keys(cert_type, password))
 
     register_payload = {
         'hardware_id': config.system_id,
         'system_uid': config.system_id,
-        'board_model_name': config.model_name,
-        'board_model_version': config.model_version,
+        'model_name': config.model_name,
+        'model_version': config.model_version,
         'provisioning_software': "aos-provisioning:{version}".format(version=3.1),
         'additional_csrs': []
     }
 
-    if cloud_api.use_model_name_param():
-        register_payload['model_name'] = config.model_name
-        register_payload['model_version'] = config.model_version
-    else:
-        register_payload['board_model_name'] = config.model_name
-        register_payload['board_model_version'] = config.model_version
-
     for cert in config.unit_certificates:
         if cert.cert_type == 'online':
             register_payload['online_public_csr'] = cert.csr
             if cert.node_id:
                 register_payload['online_public_node_id'] = cert.node_id
         elif cert.cert_type == 'offline':
             register_payload['offline_public_csr'] = cert.csr
```

## aos_prov/communication/cloud/cloud_api.py

```diff
@@ -79,15 +79,15 @@
     def register_device(self, payload):
         """Registers device in cloud. Returns registered metadata.
         :param: str - end_point for registering
         :param: str - path to server pem that contains certs and a private one
         :param: dict
         :return: dict
         """
-        logger.info('Registering the board ...')
+        logger.info('Registering the unit ...')
         end_point = self.__REGISTER_URI_TPL.format(self._cloud_api_host, self._cloud_api_port)
 
         try:
             logger.debug('Sending to %s payload: %s', end_point, payload)
             server_certificate = pkg_resources.files(self.__FILES_DIR) / self.__ROOT_CA_CERT_FILENAME
             with pkg_resources.as_file(server_certificate) as server_certificate_path:
                 with self._user_credentials.user_credentials as temp_creds:
@@ -110,15 +110,15 @@
                         logger.debug('Cloud response: {}'.format(resp_content))
                     ret.raise_for_status()
                     response = ret.json()
         except (requests.exceptions.RequestException,
                 ValueError, OSError, OpenSSL.SSL.Error) as e:
             logger.debug(e)
             print(e)
-            raise DeviceRegisterError('Failed to register board.')
+            raise DeviceRegisterError('Failed to register unit.')
 
         return response
 
     def check_unit_is_not_provisioned(self, system_uid):
         print('Getting unit\'s status on the cloud ...')
         try:
             end_point = self.__UNIT_STATUS_URL.format(
@@ -139,15 +139,15 @@
 
         response_json = response.json()
 
         if 'results' not in response_json or 'count' not in response_json:
             raise DeviceRegisterError('Invalid answer from the cloud. Please update current library')
 
         if response_json['count'] == 0:
-            # There is no such board on the cloud
+            # There is no such unit on the cloud
             return
 
         status = response_json.get('results', [{}])[0].get('status')
         if status is None:
             return
 
         if status != 'new':
```

## aos_prov/communication/unit/v4/unit_communication_v4.py

```diff
@@ -6,15 +6,15 @@
 
 import grpc
 from google.protobuf import empty_pb2
 
 from aos_prov.communication.unit.v4.generated import iamanager_pb2 as iam_manager
 from aos_prov.communication.unit.v4.generated import iamanager_pb2_grpc as iam_manager_grpc
 from aos_prov.utils.common import print_message, print_done, print_left, print_success
-from aos_prov.utils.errors import BoardError, GrpcUnimplemented
+from aos_prov.utils.errors import UnitError, GrpcUnimplemented
 from aos_prov.utils.unit_certificate import UnitCertificate
 
 UNIT_DEFAULT_PORT = 8089
 
 
 class UnitCommunicationV4:
     def __init__(self, address: str = 'localhost:8089'):
@@ -23,17 +23,17 @@
         if address is None:
             address = 'localhost:8089'
         parts = address.split(':')
         if len(parts) == 2:
             try:
                 port = int(parts[1])
                 if not 1 <= port <= 65535:
-                    raise BoardError('Unit port is invalid')
+                    raise UnitError('Unit port is invalid')
             except ValueError:
-                raise BoardError('Unit port is invalid')
+                raise UnitError('Unit port is invalid')
         else:
             address = address + ':' + str(UNIT_DEFAULT_PORT)
         self.__unit_address = address
         print_message(f'Will search unit on address: [green]{self.__unit_address}')
 
     @property
     def need_set_users(self):
@@ -58,15 +58,15 @@
 
         except grpc.RpcError as e:
             if catch_inactive and \
                     not (e.code() == grpc.StatusCode.UNAVAILABLE.value and e.details() == 'Socket closed'):
                 return
             elif wait_for_close and (e.code() == grpc.StatusCode.UNKNOWN.value and e.details() == 'Stream removed'):
                 return
-            raise BoardError(f"FAILED! Error occurred: \n{e.code()}: {e.details()}")
+            raise UnitError(f"FAILED! Error occurred: \n{e.code()}: {e.details()}")
 
     @contextmanager
     def unit_stub(self, catch_inactive=False, wait_for_close=False):
         try:
             with grpc.insecure_channel(self.__unit_address) as channel:
                 stub = iam_manager_grpc.IAMPublicServiceStub(channel)
                 if wait_for_close:
@@ -79,28 +79,28 @@
 
         except grpc.RpcError as e:
             if catch_inactive and \
                     not (e.code() == grpc.StatusCode.UNAVAILABLE.value and e.details() == 'Socket closed'):
                 return
             elif wait_for_close and (e.code() == grpc.StatusCode.UNKNOWN.value and e.details() == 'Stream removed'):
                 return
-            raise BoardError(f"FAILED! Error occurred: \n{e.code()}: {e.details()}")
+            raise UnitError(f"FAILED! Error occurred: \n{e.code()}: {e.details()}")
 
     @contextmanager
     def unit_identify_stub(self):
         try:
             with grpc.insecure_channel(self.__unit_address) as channel:
                 stub = iam_manager_grpc.IAMPublicIdentityServiceStub(channel)
                 yield stub
 
         except grpc.RpcError as e:
             if e.code().value == grpc.StatusCode.UNIMPLEMENTED.value:
                 raise GrpcUnimplemented(f'Protocol V4 is not supported: \n{e.code()}: {e.details()}')
             else:
-                raise BoardError(f"FAILED! Error occurred: \n{e.code()}: {e.details()}")
+                raise UnitError(f"FAILED! Error occurred: \n{e.code()}: {e.details()}")
 
     @contextmanager
     def unit_provisioning_stub(self, catch_inactive=False, wait_for_close=False):
         try:
             with grpc.insecure_channel(self.__unit_address) as channel:
                 stub = iam_manager_grpc.IAMProvisioningServiceStub(channel)
                 if wait_for_close:
@@ -113,28 +113,28 @@
 
         except grpc.RpcError as e:
             if catch_inactive and \
                     not (e.code() == grpc.StatusCode.UNAVAILABLE.value and e.details() == 'Socket closed'):
                 return
             elif wait_for_close and (e.code() == grpc.StatusCode.UNKNOWN.value and e.details() == 'Stream removed'):
                 return
-            raise BoardError(f"Error occurred: \n{e.code()}: {e.details()}")
+            raise UnitError(f"Error occurred: \n{e.code()}: {e.details()}")
 
     @contextmanager
     def unit_public_stub(self):
         try:
             with grpc.insecure_channel(self.__unit_address) as channel:
                 stub = iam_manager_grpc.IAMPublicServiceStub(channel)
                 yield stub
 
         except grpc.RpcError as e:
             if e.code().value == grpc.StatusCode.UNIMPLEMENTED.value:
                 raise GrpcUnimplemented(f'Protocol V4 is not supported: \n{e.code()}: {e.details()}')
             else:
-                raise BoardError(f"Error occurred: \n{e.code()}: {e.details()}")
+                raise UnitError(f"Error occurred: \n{e.code()}: {e.details()}")
 
     def get_protocol_version(self) -> int:
         with self.unit_public_stub() as stub:
             print_left('Getting protocol version...')
             response = stub.GetAPIVersion(empty_pb2.Empty())
             print_success(str(response.version))
             return int(response.version)
@@ -206,15 +206,15 @@
 
     def encrypt_disk(self, password: str, node_id: str):
         print_left(f'Starting disk encryption on node {node_id}...')
         try:
             with self.unit_provisioning_stub(wait_for_close=False) as stub:
                 stub.EncryptDisk(iam_manager.EncryptDiskRequest(password=password, node_id=node_id))
                 print_done()
-        except BoardError as be:
+        except UnitError as be:
             print_message(f'[red] Error.')
             print_message(be)
 
     def finish_provisioning(self):
         with self.unit_provisioning_stub(True) as stub:
             print_left('Finishing provisioning...')
             stub.FinishProvisioning(empty_pb2.Empty())
```

## aos_prov/utils/config.py

```diff
@@ -26,20 +26,20 @@
 
     @system_id.setter
     def system_id(self, sys_id):
         self._system_id = sys_id
 
     @property
     def model_name(self) -> str:
-        """Return Model/Board Name of the Unit. It is defined by the manufacturer."""
+        """Return Model Name of the Unit. It is defined by the manufacturer."""
         return self._model_name
 
     @property
     def model_version(self) -> str:
-        """Return Model/Board Version or Revision of the Unit. It is defined by the manufacturer."""
+        """Return Model Version or Revision of the Unit. It is defined by the manufacturer."""
         return self._model_version
 
     @property
     def supported_cert_types(self) -> [str]:
         """Return list of certificate names to be set on the Unit."""
         return self._supported_cert_types
```

## aos_prov/utils/errors.py

```diff
@@ -1,36 +1,36 @@
 #
 #  Copyright (c) 2018-2022 Renesas Inc.
 #  Copyright (c) 2018-2022 EPAM Systems Inc.
 #
 
 
-class OnBoardingError(Exception):
+class OnUnitError(Exception):
     pass
 
 
-class UserCredentialsError(OnBoardingError):
+class UserCredentialsError(OnUnitError):
     pass
 
 
-class DeviceRegisterError(OnBoardingError):
+class DeviceRegisterError(OnUnitError):
     pass
 
 
-class DeviceDeregisterError(OnBoardingError):
+class DeviceDeregisterError(OnUnitError):
     pass
 
 
-class BoardError(OnBoardingError):
+class UnitError(OnUnitError):
     pass
 
 
-class GrpcUnimplemented(OnBoardingError):
+class GrpcUnimplemented(OnUnitError):
     pass
 
 
-class CloudAccessError(OnBoardingError):
+class CloudAccessError(OnUnitError):
     pass
 
 
-class AosProvError(OnBoardingError):
+class AosProvError(OnUnitError):
     pass
```

## Comparing `aos_prov-4.0.2b3.dist-info/METADATA` & `aos_prov-4.1.0b1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aos-prov
-Version: 4.0.2b3
+Version: 4.1.0b1
 Summary: AosEdge Unit provisioning tool
 Author: EPAM Systems
 Author-email: support@aoscloud.io
 License: Apache License 2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

