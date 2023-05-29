# Comparing `tmp/gurux_dlms-1.0.98.tar.gz` & `tmp/gurux_dlms-1.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gurux_dlms-1.0.98.tar", last modified: Thu Jan 28 06:54:34 2021, max compression
+gzip compressed data, was "dist\gurux_dlms-1.0.99.tar", last modified: Fri Feb 12 06:52:42 2021, max compression
```

## Comparing `gurux_dlms-1.0.98.tar` & `gurux_dlms-1.0.99.tar`

### file list

```diff
@@ -1,318 +1,318 @@
-drwxrwxrwx   0        0        0        0 2021-01-28 06:54:34.000000 gurux_dlms-1.0.98/
--rw-rw-rw-   0        0        0     7195 2021-01-28 06:54:34.000000 gurux_dlms-1.0.98/PKG-INFO
--rw-rw-rw-   0        0        0     5236 2020-07-13 08:30:48.000000 gurux_dlms-1.0.98/README.md
-drwxrwxrwx   0        0        0        0 2021-01-28 06:54:33.000000 gurux_dlms-1.0.98/gurux_dlms/
--rw-rw-rw-   0        0        0     1611 2020-05-26 09:00:26.000000 gurux_dlms-1.0.98/gurux_dlms/ActionRequestType.py
--rw-rw-rw-   0        0        0     1510 2020-05-26 08:57:45.000000 gurux_dlms-1.0.98/gurux_dlms/ActionResponseType.py
--rw-rw-rw-   0        0        0     2909 2020-02-11 09:20:20.000000 gurux_dlms-1.0.98/gurux_dlms/AesGcmParameter.py
--rw-rw-rw-   0        0        0     1447 2020-05-26 08:50:46.000000 gurux_dlms-1.0.98/gurux_dlms/ConfirmedServiceError.py
--rw-rw-rw-   0        0        0     1502 2020-05-26 13:31:22.000000 gurux_dlms-1.0.98/gurux_dlms/ConnectionState.py
--rw-rw-rw-   0        0        0     1462 2020-05-26 08:58:04.000000 gurux_dlms-1.0.98/gurux_dlms/CountType.py
--rw-rw-rw-   0        0        0     1266 2019-09-09 12:45:06.000000 gurux_dlms-1.0.98/gurux_dlms/GXArray.py
--rw-rw-rw-   0        0        0     3075 2020-05-26 13:46:02.000000 gurux_dlms-1.0.98/gurux_dlms/GXBitString.py
--rw-rw-rw-   0        0        0    19670 2020-05-25 08:11:23.000000 gurux_dlms-1.0.98/gurux_dlms/GXByteBuffer.py
--rw-rw-rw-   0        0        0     6999 2020-08-10 11:39:46.000000 gurux_dlms-1.0.98/gurux_dlms/GXCiphering.py
--rw-rw-rw-   0        0        0    95719 2021-01-27 11:22:25.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMS.py
--rw-rw-rw-   0        0        0     1994 2019-08-15 11:02:48.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMSAccessItem.py
--rw-rw-rw-   0        0        0    11611 2021-01-28 06:41:03.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMSChippering.py
--rw-rw-rw-   0        0        0    44103 2019-10-29 14:09:39.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMSChipperingStream.py
--rw-rw-rw-   0        0        0    52375 2020-10-15 17:52:53.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMSClient.py
--rw-rw-rw-   0        0        0     4670 2019-08-16 12:46:43.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMSConfirmedServiceError.py
--rw-rw-rw-   0        0        0     1316 2019-08-15 11:02:48.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMSConnectionEventArgs.py
--rw-rw-rw-   0        0        0    21745 2020-05-27 09:31:27.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMSConverter.py
--rw-rw-rw-   0        0        0     5527 2020-08-04 13:49:25.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMSException.py
--rw-rw-rw-   0        0        0     2900 2020-08-04 12:25:24.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMSExceptionResponse.py
--rw-rw-rw-   0        0        0     1513 2019-08-15 11:02:48.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMSGateway.py
--rw-rw-rw-   0        0        0    37003 2020-05-14 13:04:32.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMSLNCommandHandler.py
--rw-rw-rw-   0        0        0     2945 2020-03-10 09:29:08.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMSLNParameters.py
--rw-rw-rw-   0        0        0     1754 2019-08-15 11:02:48.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMSLimits.py
--rw-rw-rw-   0        0        0     1792 2019-08-15 11:02:49.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMSLongTransaction.py
--rw-rw-rw-   0        0        0     9738 2020-05-13 12:18:39.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMSNotify.py
--rw-rw-rw-   0        0        0    22711 2021-01-28 06:43:59.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMSSNCommandHandler.py
--rw-rw-rw-   0        0        0     2399 2019-08-15 11:02:48.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMSSNParameters.py
--rw-rw-rw-   0        0        0    39149 2021-01-28 06:46:17.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMSServer.py
--rw-rw-rw-   0        0        0    13106 2020-08-25 11:37:56.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMSSettings.py
--rw-rw-rw-   0        0        0    87699 2021-01-28 06:44:30.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMSTranslator.py
--rw-rw-rw-   0        0        0     7632 2019-09-04 09:24:08.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMSTranslatorStructure.py
--rw-rw-rw-   0        0        0    12691 2020-05-13 12:19:35.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMSXmlClient.py
--rw-rw-rw-   0        0        0     5119 2019-08-16 11:46:15.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMSXmlPdu.py
--rw-rw-rw-   0        0        0     3622 2019-08-16 12:09:06.000000 gurux_dlms-1.0.98/gurux_dlms/GXDLMSXmlSettings.py
--rw-rw-rw-   0        0        0     2377 2020-05-13 08:42:31.000000 gurux_dlms-1.0.98/gurux_dlms/GXDate.py
--rw-rw-rw-   0        0        0    23358 2020-11-26 10:24:27.000000 gurux_dlms-1.0.98/gurux_dlms/GXDateTime.py
--rw-rw-rw-   0        0        0     1233 2020-03-24 13:04:34.000000 gurux_dlms-1.0.98/gurux_dlms/GXEnum.py
--rw-rw-rw-   0        0        0     1241 2020-05-22 06:23:32.000000 gurux_dlms-1.0.98/gurux_dlms/GXFloat32.py
--rw-rw-rw-   0        0        0     1243 2020-05-22 06:23:58.000000 gurux_dlms-1.0.98/gurux_dlms/GXFloat64.py
--rw-rw-rw-   0        0        0     5213 2019-08-16 11:45:19.000000 gurux_dlms-1.0.98/gurux_dlms/GXICipher.py
--rw-rw-rw-   0        0        0     1235 2020-03-26 13:25:03.000000 gurux_dlms-1.0.98/gurux_dlms/GXInt16.py
--rw-rw-rw-   0        0        0     1235 2020-03-26 13:28:49.000000 gurux_dlms-1.0.98/gurux_dlms/GXInt32.py
--rw-rw-rw-   0        0        0     1235 2020-03-26 13:28:26.000000 gurux_dlms-1.0.98/gurux_dlms/GXInt64.py
--rw-rw-rw-   0        0        0     1233 2020-03-26 13:24:26.000000 gurux_dlms-1.0.98/gurux_dlms/GXInt8.py
--rw-rw-rw-   0        0        0     1388 2020-05-26 13:46:37.000000 gurux_dlms-1.0.98/gurux_dlms/GXIntEnum.py
--rw-rw-rw-   0        0        0     1398 2020-05-26 13:46:43.000000 gurux_dlms-1.0.98/gurux_dlms/GXIntFlag.py
--rw-rw-rw-   0        0        0     6250 2020-03-24 08:27:15.000000 gurux_dlms-1.0.98/gurux_dlms/GXReplyData.py
--rw-rw-rw-   0        0        0     1656 2019-08-16 11:49:03.000000 gurux_dlms-1.0.98/gurux_dlms/GXSNInfo.py
--rw-rw-rw-   0        0        0     5000 2020-05-14 12:19:14.000000 gurux_dlms-1.0.98/gurux_dlms/GXSecure.py
--rw-rw-rw-   0        0        0     1751 2019-08-16 11:41:05.000000 gurux_dlms-1.0.98/gurux_dlms/GXServerReply.py
--rw-rw-rw-   0        0        0     2094 2020-03-23 09:10:46.000000 gurux_dlms-1.0.98/gurux_dlms/GXStandardObisCode.py
--rw-rw-rw-   0        0        0    15758 2020-08-04 12:07:39.000000 gurux_dlms-1.0.98/gurux_dlms/GXStandardObisCodeCollection.py
--rw-rw-rw-   0        0        0     1270 2019-09-09 12:45:27.000000 gurux_dlms-1.0.98/gurux_dlms/GXStructure.py
--rw-rw-rw-   0        0        0     2180 2020-05-13 08:42:36.000000 gurux_dlms-1.0.98/gurux_dlms/GXTime.py
--rw-rw-rw-   0        0        0     2101 2020-05-13 13:10:30.000000 gurux_dlms-1.0.98/gurux_dlms/GXTimeZone.py
--rw-rw-rw-   0        0        0     1237 2020-03-26 13:12:32.000000 gurux_dlms-1.0.98/gurux_dlms/GXUInt16.py
--rw-rw-rw-   0        0        0     1331 2020-05-14 14:35:21.000000 gurux_dlms-1.0.98/gurux_dlms/GXUInt32.py
--rw-rw-rw-   0        0        0     1237 2020-03-26 13:13:06.000000 gurux_dlms-1.0.98/gurux_dlms/GXUInt64.py
--rw-rw-rw-   0        0        0     1235 2020-03-26 13:12:41.000000 gurux_dlms-1.0.98/gurux_dlms/GXUInt8.py
--rw-rw-rw-   0        0        0     1901 2019-08-16 11:40:56.000000 gurux_dlms-1.0.98/gurux_dlms/GXWriteItem.py
--rw-rw-rw-   0        0        0     1394 2019-08-15 11:02:48.000000 gurux_dlms-1.0.98/gurux_dlms/GXXmlLoadSettings.py
--rw-rw-rw-   0        0        0     1465 2020-05-26 09:08:30.000000 gurux_dlms-1.0.98/gurux_dlms/GetCommandType.py
--rw-rw-rw-   0        0        0     1376 2020-05-26 09:08:32.000000 gurux_dlms-1.0.98/gurux_dlms/HdlcControlFrame.py
--rw-rw-rw-   0        0        0     8823 2020-05-15 10:31:22.000000 gurux_dlms-1.0.98/gurux_dlms/India.txt
--rw-rw-rw-   0        0        0     7960 2019-08-15 11:02:47.000000 gurux_dlms-1.0.98/gurux_dlms/Italy.txt
--rw-rw-rw-   0        0        0     1336 2020-05-26 09:07:44.000000 gurux_dlms-1.0.98/gurux_dlms/MBusCommand.py
--rw-rw-rw-   0        0        0     1832 2020-05-26 09:07:50.000000 gurux_dlms-1.0.98/gurux_dlms/MBusControlInfo.py
--rw-rw-rw-   0        0        0     1816 2020-05-26 09:07:54.000000 gurux_dlms-1.0.98/gurux_dlms/MBusEncryptionMode.py
--rw-rw-rw-   0        0        0     1474 2020-05-26 09:07:57.000000 gurux_dlms-1.0.98/gurux_dlms/MBusMeterType.py
--rw-rw-rw-   0        0        0   172620 2020-11-12 13:51:44.000000 gurux_dlms-1.0.98/gurux_dlms/OBISCodes.txt
--rw-rw-rw-   0        0        0     1589 2020-05-26 09:13:46.000000 gurux_dlms-1.0.98/gurux_dlms/ReleaseRequestReason.py
--rw-rw-rw-   0        0        0     1593 2020-05-26 09:13:46.000000 gurux_dlms-1.0.98/gurux_dlms/ReleaseResponseReason.py
--rw-rw-rw-   0        0        0     5141 2019-08-15 11:02:48.000000 gurux_dlms-1.0.98/gurux_dlms/SaudiArabia.txt
--rw-rw-rw-   0        0        0     3575 2020-05-14 12:28:17.000000 gurux_dlms-1.0.98/gurux_dlms/SerialnumberCounter.py
--rw-rw-rw-   0        0        0     1829 2020-05-26 09:13:45.000000 gurux_dlms-1.0.98/gurux_dlms/ServiceError.py
--rw-rw-rw-   0        0        0     1583 2020-05-26 09:13:45.000000 gurux_dlms-1.0.98/gurux_dlms/SetRequestType.py
--rw-rw-rw-   0        0        0     1676 2020-05-26 09:14:24.000000 gurux_dlms-1.0.98/gurux_dlms/SetResponseType.py
--rw-rw-rw-   0        0        0     1574 2020-05-26 09:13:32.000000 gurux_dlms-1.0.98/gurux_dlms/SingleReadResponse.py
--rw-rw-rw-   0        0        0     1552 2020-05-26 09:13:30.000000 gurux_dlms-1.0.98/gurux_dlms/SingleWriteResponse.py
--rw-rw-rw-   0        0        0     2247 2020-05-26 09:13:27.000000 gurux_dlms-1.0.98/gurux_dlms/TranslatorGeneralTags.py
--rw-rw-rw-   0        0        0     1395 2020-05-26 09:14:21.000000 gurux_dlms-1.0.98/gurux_dlms/TranslatorOutputType.py
--rw-rw-rw-   0        0        0    40626 2020-08-25 14:18:12.000000 gurux_dlms-1.0.98/gurux_dlms/TranslatorSimpleTags.py
--rw-rw-rw-   0        0        0    41782 2020-08-25 14:18:32.000000 gurux_dlms-1.0.98/gurux_dlms/TranslatorStandardTags.py
--rw-rw-rw-   0        0        0     4026 2020-08-04 13:00:37.000000 gurux_dlms-1.0.98/gurux_dlms/TranslatorTags.py
--rw-rw-rw-   0        0        0     3219 2019-08-16 11:41:43.000000 gurux_dlms-1.0.98/gurux_dlms/ValueEventArgs.py
--rw-rw-rw-   0        0        0     1705 2020-05-26 09:14:16.000000 gurux_dlms-1.0.98/gurux_dlms/VariableAccessSpecification.py
--rw-rw-rw-   0        0        0    50521 2020-11-26 10:26:51.000000 gurux_dlms-1.0.98/gurux_dlms/_GXAPDU.py
--rw-rw-rw-   0        0        0     4531 2019-08-15 11:02:48.000000 gurux_dlms-1.0.98/gurux_dlms/_GXFCS16.py
--rw-rw-rw-   0        0        0    10186 2020-04-15 08:39:06.000000 gurux_dlms-1.0.98/gurux_dlms/_GXObjectFactory.py
--rw-rw-rw-   0        0        0     1474 2019-08-16 11:50:24.000000 gurux_dlms-1.0.98/gurux_dlms/_HDLCInfo.py
--rw-rw-rw-   0        0        0     5018 2020-08-04 13:52:18.000000 gurux_dlms-1.0.98/gurux_dlms/__init__.py
-drwxrwxrwx   0        0        0        0 2021-01-28 06:54:33.000000 gurux_dlms-1.0.98/gurux_dlms/enums/
--rw-rw-rw-   0        0        0     1497 2020-05-26 08:51:49.000000 gurux_dlms-1.0.98/gurux_dlms/enums/Access.py
--rw-rw-rw-   0        0        0     1715 2020-05-26 08:52:14.000000 gurux_dlms-1.0.98/gurux_dlms/enums/AccessMode.py
--rw-rw-rw-   0        0        0     1501 2020-05-26 08:55:17.000000 gurux_dlms-1.0.98/gurux_dlms/enums/AccessServiceCommandType.py
--rw-rw-rw-   0        0        0     1422 2020-11-26 10:30:28.000000 gurux_dlms-1.0.98/gurux_dlms/enums/AcseServiceProvider.py
--rw-rw-rw-   0        0        0     1830 2020-05-26 09:00:06.000000 gurux_dlms-1.0.98/gurux_dlms/enums/ApplicationReference.py
--rw-rw-rw-   0        0        0     1654 2020-05-26 09:14:10.000000 gurux_dlms-1.0.98/gurux_dlms/enums/AssociationResult.py
--rw-rw-rw-   0        0        0     2642 2020-05-26 09:00:02.000000 gurux_dlms-1.0.98/gurux_dlms/enums/Authentication.py
--rw-rw-rw-   0        0        0     2682 2020-05-26 08:59:58.000000 gurux_dlms-1.0.98/gurux_dlms/enums/BerType.py
--rw-rw-rw-   0        0        0     1821 2020-05-26 08:59:54.000000 gurux_dlms-1.0.98/gurux_dlms/enums/ClockStatus.py
--rw-rw-rw-   0        0        0    15585 2020-08-25 15:07:14.000000 gurux_dlms-1.0.98/gurux_dlms/enums/Command.py
--rw-rw-rw-   0        0        0     7330 2020-05-26 11:52:13.000000 gurux_dlms-1.0.98/gurux_dlms/enums/Conformance.py
--rw-rw-rw-   0        0        0     2566 2020-05-26 09:02:23.000000 gurux_dlms-1.0.98/gurux_dlms/enums/DataType.py
--rw-rw-rw-   0        0        0     1560 2020-05-26 13:35:39.000000 gurux_dlms-1.0.98/gurux_dlms/enums/DateTimeExtraInfo.py
--rw-rw-rw-   0        0        0     2020 2020-05-26 13:35:28.000000 gurux_dlms-1.0.98/gurux_dlms/enums/DateTimeSkips.py
--rw-rw-rw-   0        0        0     1476 2020-05-26 08:59:42.000000 gurux_dlms-1.0.98/gurux_dlms/enums/Definition.py
--rw-rw-rw-   0        0        0     2014 2020-05-26 08:59:36.000000 gurux_dlms-1.0.98/gurux_dlms/enums/ErrorCode.py
--rw-rw-rw-   0        0        0     1673 2020-08-04 12:26:06.000000 gurux_dlms-1.0.98/gurux_dlms/enums/ExceptionServiceError.py
--rw-rw-rw-   0        0        0     1512 2020-05-26 09:00:37.000000 gurux_dlms-1.0.98/gurux_dlms/enums/HardwareResource.py
--rw-rw-rw-   0        0        0     1387 2020-05-26 09:00:47.000000 gurux_dlms-1.0.98/gurux_dlms/enums/HdlcFrameType.py
--rw-rw-rw-   0        0        0     1484 2020-05-26 09:02:42.000000 gurux_dlms-1.0.98/gurux_dlms/enums/Initiate.py
--rw-rw-rw-   0        0        0     1455 2020-05-26 09:00:57.000000 gurux_dlms-1.0.98/gurux_dlms/enums/InterfaceType.py
--rw-rw-rw-   0        0        0     1616 2020-05-26 09:01:06.000000 gurux_dlms-1.0.98/gurux_dlms/enums/KeyAgreement.py
--rw-rw-rw-   0        0        0     1785 2020-05-26 09:02:51.000000 gurux_dlms-1.0.98/gurux_dlms/enums/LoadDataSet.py
--rw-rw-rw-   0        0        0     1466 2020-05-26 09:01:16.000000 gurux_dlms-1.0.98/gurux_dlms/enums/MethodAccessMode.py
--rw-rw-rw-   0        0        0    12599 2020-05-26 09:01:26.000000 gurux_dlms-1.0.98/gurux_dlms/enums/ObjectType.py
--rw-rw-rw-   0        0        0     2531 2020-05-26 09:03:02.000000 gurux_dlms-1.0.98/gurux_dlms/enums/PduType.py
--rw-rw-rw-   0        0        0     1358 2020-05-26 09:01:35.000000 gurux_dlms-1.0.98/gurux_dlms/enums/Priority.py
--rw-rw-rw-   0        0        0     1437 2020-07-06 13:16:03.000000 gurux_dlms-1.0.98/gurux_dlms/enums/RequestTypes.py
--rw-rw-rw-   0        0        0     1605 2020-05-26 09:03:14.000000 gurux_dlms-1.0.98/gurux_dlms/enums/Security.py
--rw-rw-rw-   0        0        0     1555 2020-05-26 09:03:26.000000 gurux_dlms-1.0.98/gurux_dlms/enums/Service.py
--rw-rw-rw-   0        0        0     1372 2020-05-26 13:32:51.000000 gurux_dlms-1.0.98/gurux_dlms/enums/ServiceClass.py
--rw-rw-rw-   0        0        0     1412 2020-05-26 09:08:55.000000 gurux_dlms-1.0.98/gurux_dlms/enums/ServiceError.py
--rw-rw-rw-   0        0        0     2043 2020-05-26 09:08:49.000000 gurux_dlms-1.0.98/gurux_dlms/enums/SourceDiagnostic.py
--rw-rw-rw-   0        0        0     1745 2020-05-26 09:08:47.000000 gurux_dlms-1.0.98/gurux_dlms/enums/Standard.py
--rw-rw-rw-   0        0        0     1375 2020-05-26 09:08:44.000000 gurux_dlms-1.0.98/gurux_dlms/enums/StateError.py
--rw-rw-rw-   0        0        0     1453 2020-05-26 09:08:42.000000 gurux_dlms-1.0.98/gurux_dlms/enums/Task.py
--rw-rw-rw-   0        0        0     3988 2020-05-26 09:08:39.000000 gurux_dlms-1.0.98/gurux_dlms/enums/Unit.py
--rw-rw-rw-   0        0        0     1487 2020-05-26 09:08:37.000000 gurux_dlms-1.0.98/gurux_dlms/enums/VdeStateError.py
--rw-rw-rw-   0        0        0     2669 2020-11-26 10:29:49.000000 gurux_dlms-1.0.98/gurux_dlms/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2021-01-28 06:54:33.000000 gurux_dlms-1.0.98/gurux_dlms/internal/
--rw-rw-rw-   0        0        0    64702 2020-08-19 06:09:03.000000 gurux_dlms-1.0.98/gurux_dlms/internal/_GXCommon.py
--rw-rw-rw-   0        0        0     1816 2019-08-15 12:07:47.000000 gurux_dlms-1.0.98/gurux_dlms/internal/_GXDataInfo.py
--rw-rw-rw-   0        0        0     1229 2019-08-15 11:02:48.000000 gurux_dlms-1.0.98/gurux_dlms/internal/__init__.py
-drwxrwxrwx   0        0        0        0 2021-01-28 06:54:33.000000 gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/
--rw-rw-rw-   0        0        0     1867 2019-11-08 09:01:33.000000 gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/GXAttributeCollection.py
--rw-rw-rw-   0        0        0     1766 2019-08-15 11:02:48.000000 gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/GXAuthentication.py
--rw-rw-rw-   0        0        0     1778 2019-08-16 12:37:42.000000 gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/GXDLMSAttribute.py
--rw-rw-rw-   0        0        0     2177 2019-08-16 08:46:08.000000 gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/GXDLMSAttributeSettings.py
--rw-rw-rw-   0        0        0     2485 2019-08-15 11:02:48.000000 gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/GXManufacturer.py
--rw-rw-rw-   0        0        0     9221 2019-08-16 13:58:57.000000 gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/GXManufacturerCollection.py
--rw-rw-rw-   0        0        0     1855 2020-03-24 14:31:21.000000 gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/GXObisCode.py
--rw-rw-rw-   0        0        0     1473 2019-08-15 11:02:48.000000 gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/GXObisCodeCollection.py
--rw-rw-rw-   0        0        0     1502 2019-08-15 11:02:48.000000 gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/GXObisValueItem.py
--rw-rw-rw-   0        0        0     1866 2019-08-16 12:37:57.000000 gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/GXObisValueItemCollection.py
--rw-rw-rw-   0        0        0     1649 2019-08-15 11:02:48.000000 gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/GXServerAddress.py
--rw-rw-rw-   0        0        0     1348 2020-05-26 09:08:16.000000 gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/HDLCAddressType.py
--rw-rw-rw-   0        0        0     1513 2020-05-26 09:08:13.000000 gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/InactivityMode.py
--rw-rw-rw-   0        0        0     1469 2020-05-26 09:08:10.000000 gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/StartProtocolType.py
--rw-rw-rw-   0        0        0      482 2019-08-15 11:02:48.000000 gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/__init__.py
-drwxrwxrwx   0        0        0        0 2021-01-28 06:54:34.000000 gurux_dlms-1.0.98/gurux_dlms/objects/
--rw-rw-rw-   0        0        0     1474 2019-08-16 08:59:10.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXAdjacentCell.py
--rw-rw-rw-   0        0        0     1983 2019-08-16 08:42:12.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXApplicationContextName.py
--rw-rw-rw-   0        0        0     1996 2019-08-16 09:27:26.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXAuthenticationMechanismName.py
--rw-rw-rw-   0        0        0     1599 2019-08-16 13:03:06.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXChargePerUnitScaling.py
--rw-rw-rw-   0        0        0     1528 2019-08-16 09:31:32.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXChargeTable.py
--rw-rw-rw-   0        0        0     1580 2019-08-15 13:16:33.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXCommodity.py
--rw-rw-rw-   0        0        0     1656 2019-08-15 13:20:30.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXCreditChargeConfiguration.py
--rw-rw-rw-   0        0        0     1782 2019-08-16 08:34:48.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXCurrency.py
--rw-rw-rw-   0        0        0    22795 2020-09-08 06:15:54.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSAccount.py
--rw-rw-rw-   0        0        0     1534 2019-08-16 09:28:09.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSActionItem.py
--rw-rw-rw-   0        0        0     8620 2020-05-27 08:16:51.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSActionSchedule.py
--rw-rw-rw-   0        0        0     1501 2019-08-16 09:07:30.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSActionSet.py
--rw-rw-rw-   0        0        0    20076 2020-08-26 12:59:51.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSActivityCalendar.py
--rw-rw-rw-   0        0        0    32168 2020-06-03 10:59:11.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSAssociationLogicalName.py
--rw-rw-rw-   0        0        0    10529 2020-05-14 12:07:49.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSAssociationShortName.py
--rw-rw-rw-   0        0        0     8616 2020-05-14 13:12:47.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSAutoAnswer.py
--rw-rw-rw-   0        0        0     8557 2020-05-14 13:13:07.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSAutoConnect.py
--rw-rw-rw-   0        0        0     1522 2019-08-16 08:37:07.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSCaptureObject.py
--rw-rw-rw-   0        0        0     1653 2019-08-16 08:28:06.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSCertificateInfo.py
--rw-rw-rw-   0        0        0    13422 2020-05-27 06:43:30.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSCharge.py
--rw-rw-rw-   0        0        0    10000 2020-05-14 13:13:54.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSClock.py
--rw-rw-rw-   0        0        0     9667 2020-11-26 10:25:22.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSCredit.py
--rw-rw-rw-   0        0        0     3721 2020-03-26 14:20:36.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSData.py
--rw-rw-rw-   0        0        0     1801 2019-08-15 13:20:05.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSDayProfile.py
--rw-rw-rw-   0        0        0     1852 2019-08-15 13:46:23.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSDayProfileAction.py
--rw-rw-rw-   0        0        0    11377 2020-05-27 06:44:03.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSDemandRegister.py
--rw-rw-rw-   0        0        0     5471 2020-03-23 08:05:49.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSDisconnectControl.py
--rw-rw-rw-   0        0        0     1584 2019-08-16 08:40:21.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSEmergencyProfile.py
--rw-rw-rw-   0        0        0     7653 2020-05-27 06:44:27.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSExtendedRegister.py
--rw-rw-rw-   0        0        0     1589 2019-08-16 09:31:50.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSGSMCellInfo.py
--rw-rw-rw-   0        0        0    11616 2020-05-27 06:25:25.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSGSMDiagnostic.py
--rw-rw-rw-   0        0        0     9679 2020-05-14 13:14:26.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSGprsSetup.py
--rw-rw-rw-   0        0        0     8108 2020-03-24 08:05:35.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSHdlcSetup.py
--rw-rw-rw-   0        0        0     7922 2020-05-14 13:14:45.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSIECLocalPortSetup.py
--rw-rw-rw-   0        0        0     5540 2019-08-16 13:02:13.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSIecTwistedPairSetup.py
--rw-rw-rw-   0        0        0     2158 2019-08-16 09:02:40.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSImageActivateInfo.py
--rw-rw-rw-   0        0        0    13230 2020-05-14 11:37:06.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSImageTransfer.py
--rw-rw-rw-   0        0        0    11925 2020-05-13 13:20:58.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSIp4Setup.py
--rw-rw-rw-   0        0        0     1431 2019-08-16 08:59:33.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSIp4SetupIpOption.py
--rw-rw-rw-   0        0        0    14170 2020-05-27 07:54:03.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSIp6Setup.py
--rw-rw-rw-   0        0        0    15527 2020-05-14 13:51:57.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSLimiter.py
--rw-rw-rw-   0        0        0     4728 2020-04-15 08:57:01.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSLlcSscsSetup.py
--rw-rw-rw-   0        0        0    12445 2020-05-14 13:15:10.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSMBusClient.py
--rw-rw-rw-   0        0        0     3672 2020-05-27 06:51:27.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSMBusMasterPortSetup.py
--rw-rw-rw-   0        0        0     6196 2020-03-26 14:33:32.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSMBusSlavePortSetup.py
--rw-rw-rw-   0        0        0     3982 2019-08-16 13:05:44.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSMacAddressSetup.py
--rw-rw-rw-   0        0        0     7902 2020-05-27 06:52:48.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSModemConfiguration.py
--rw-rw-rw-   0        0        0     1552 2019-08-16 08:29:04.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSModemInitialisation.py
--rw-rw-rw-   0        0        0     1793 2019-08-16 08:36:52.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSMonitoredValue.py
--rw-rw-rw-   0        0        0     8528 2020-11-09 07:33:57.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSObject.py
--rw-rw-rw-   0        0        0     5792 2020-05-27 09:32:22.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSObjectCollection.py
--rw-rw-rw-   0        0        0     1550 2019-08-16 08:37:52.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSObjectDefinition.py
--rw-rw-rw-   0        0        0    12722 2020-05-14 13:15:19.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSParameterMonitor.py
--rw-rw-rw-   0        0        0    10040 2020-05-13 12:14:37.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSPppSetup.py
--rw-rw-rw-   0        0        0     1462 2019-08-16 08:40:47.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSPppSetupIPCPOption.py
--rw-rw-rw-   0        0        0     1527 2019-08-16 08:41:02.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSPppSetupLcpOption.py
--rw-rw-rw-   0        0        0     5197 2020-08-25 15:10:40.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSPrimeNbOfdmPlcApplicationsIdentification.py
--rw-rw-rw-   0        0        0     7195 2020-04-15 11:37:00.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSPrimeNbOfdmPlcMacCounters.py
--rw-rw-rw-   0        0        0    10411 2020-05-27 06:26:30.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSPrimeNbOfdmPlcMacFunctionalParameters.py
--rw-rw-rw-   0        0        0    19391 2020-05-27 06:35:00.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSPrimeNbOfdmPlcMacNetworkAdministrationData.py
--rw-rw-rw-   0        0        0     7106 2020-04-15 12:03:38.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSPrimeNbOfdmPlcMacSetup.py
--rw-rw-rw-   0        0        0     6100 2020-04-15 10:47:54.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSPrimeNbOfdmPlcPhysicalLayerCounters.py
--rw-rw-rw-   0        0        0    23426 2020-11-09 07:29:46.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSProfileGeneric.py
--rw-rw-rw-   0        0        0    11845 2020-05-27 07:02:46.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSPushSetup.py
--rw-rw-rw-   0        0        0     1531 2019-08-16 09:29:29.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSQualityOfService.py
--rw-rw-rw-   0        0        0     6007 2020-11-09 07:56:39.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSRegister.py
--rw-rw-rw-   0        0        0     8017 2020-05-13 12:14:37.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSRegisterActivation.py
--rw-rw-rw-   0        0        0     9772 2020-05-27 08:05:40.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSRegisterMonitor.py
--rw-rw-rw-   0        0        0     5370 2020-05-14 13:15:35.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSSapAssignment.py
--rw-rw-rw-   0        0        0    10429 2021-01-27 13:24:26.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSSchedule.py
--rw-rw-rw-   0        0        0     2290 2019-08-16 08:33:06.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSScheduleEntry.py
--rw-rw-rw-   0        0        0     1531 2019-08-16 08:37:28.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSScript.py
--rw-rw-rw-   0        0        0     2294 2020-05-14 11:58:39.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSScriptAction.py
--rw-rw-rw-   0        0        0    10359 2020-05-27 08:01:32.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSScriptTable.py
--rw-rw-rw-   0        0        0     1912 2020-03-19 12:02:21.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSSeasonProfile.py
--rw-rw-rw-   0        0        0    19569 2020-05-26 13:42:48.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSSecuritySetup.py
--rw-rw-rw-   0        0        0     1518 2019-09-18 06:59:18.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSSpecialDay.py
--rw-rw-rw-   0        0        0     7467 2020-08-18 13:50:59.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSSpecialDaysTable.py
--rw-rw-rw-   0        0        0     1634 2019-08-16 08:42:33.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSTarget.py
--rw-rw-rw-   0        0        0     6670 2019-08-16 13:11:58.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSTcpUdpSetup.py
--rw-rw-rw-   0        0        0     7611 2020-05-14 13:16:08.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSTokenGateway.py
--rw-rw-rw-   0        0        0     4701 2020-04-21 06:56:57.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSUtilityTables.py
--rw-rw-rw-   0        0        0     1728 2020-03-10 07:32:34.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSWeekProfile.py
--rw-rw-rw-   0        0        0     1721 2020-04-15 11:46:04.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXMacAvailableSwitch.py
--rw-rw-rw-   0        0        0     2041 2020-04-15 11:44:28.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXMacDirectTable.py
--rw-rw-rw-   0        0        0     1480 2020-04-15 11:42:33.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXMacMulticastEntry.py
--rw-rw-rw-   0        0        0     2217 2020-04-21 06:57:57.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXMacPhyCommunication.py
--rw-rw-rw-   0        0        0     1671 2019-08-16 08:41:53.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXNeighborDiscoverySetup.py
--rw-rw-rw-   0        0        0     1599 2019-08-16 08:58:58.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXTokenGatewayConfiguration.py
--rw-rw-rw-   0        0        0     1907 2019-08-16 08:59:52.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXUnitCharge.py
--rw-rw-rw-   0        0        0     6626 2020-05-13 08:40:48.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXXmlReader.py
--rw-rw-rw-   0        0        0     6679 2020-05-27 07:58:18.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXXmlWriter.py
--rw-rw-rw-   0        0        0     1471 2019-08-16 10:23:04.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXXmlWriterSettings.py
--rw-rw-rw-   0        0        0     3867 2019-08-16 10:20:20.000000 gurux_dlms-1.0.98/gurux_dlms/objects/GXxDLMSContextType.py
--rw-rw-rw-   0        0        0     3313 2019-08-15 12:57:54.000000 gurux_dlms-1.0.98/gurux_dlms/objects/IGXDLMSBase.py
--rw-rw-rw-   0        0        0     6463 2020-05-27 07:03:16.000000 gurux_dlms-1.0.98/gurux_dlms/objects/__init__.py
-drwxrwxrwx   0        0        0        0 2021-01-28 06:54:34.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/
--rw-rw-rw-   0        0        0     1990 2020-05-26 13:33:57.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/AccountCreditStatus.py
--rw-rw-rw-   0        0        0     1614 2020-05-26 09:08:01.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/AccountStatus.py
--rw-rw-rw-   0        0        0     1578 2020-05-26 09:07:39.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/AddressConfigMode.py
--rw-rw-rw-   0        0        0     1599 2020-05-26 09:07:15.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/AddressState.py
--rw-rw-rw-   0        0        0     1650 2020-05-26 09:14:46.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/ApplicationContextName.py
--rw-rw-rw-   0        0        0     1620 2020-05-26 09:14:59.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/AssociationStatus.py
--rw-rw-rw-   0        0        0     1933 2020-05-26 09:06:51.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/AutoAnswerMode.py
--rw-rw-rw-   0        0        0     1356 2020-05-26 09:06:55.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/AutoAnswerStatus.py
--rw-rw-rw-   0        0        0     2915 2020-05-26 09:07:00.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/AutoConnectMode.py
--rw-rw-rw-   0        0        0     1987 2020-05-26 09:06:47.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/BaudRate.py
--rw-rw-rw-   0        0        0     1645 2020-05-26 09:06:23.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/CertificateEntity.py
--rw-rw-rw-   0        0        0     1632 2020-05-26 09:06:16.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/CertificateIdentificationType.py
--rw-rw-rw-   0        0        0     1632 2020-05-26 09:11:37.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/CertificateType.py
--rw-rw-rw-   0        0        0     1456 2020-05-26 13:47:49.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/ChargeConfiguration.py
--rw-rw-rw-   0        0        0     1687 2020-05-26 09:11:35.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/ChargeType.py
--rw-rw-rw-   0        0        0     1708 2020-05-26 09:11:32.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/ClockBase.py
--rw-rw-rw-   0        0        0     2326 2020-05-26 09:11:30.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/ControlMode.py
--rw-rw-rw-   0        0        0     1714 2020-05-26 09:11:27.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/ControlState.py
--rw-rw-rw-   0        0        0     1674 2020-05-26 12:08:59.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/CreditCollectionConfiguration.py
--rw-rw-rw-   0        0        0     1886 2020-05-26 13:34:27.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/CreditConfiguration.py
--rw-rw-rw-   0        0        0     1705 2020-05-26 09:11:25.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/CreditStatus.py
--rw-rw-rw-   0        0        0     1712 2020-05-26 09:11:22.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/CreditType.py
--rw-rw-rw-   0        0        0     1560 2020-05-26 09:11:20.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/Currency.py
--rw-rw-rw-   0        0        0     1765 2020-05-26 09:11:17.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/GlobalKeyType.py
--rw-rw-rw-   0        0        0     1514 2020-05-26 09:11:15.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/GsmCircuitSwitchStatus.py
--rw-rw-rw-   0        0        0     1657 2020-05-26 09:11:11.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/GsmPacketSwitchStatus.py
--rw-rw-rw-   0        0        0     1597 2020-05-26 09:11:07.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/GsmStatus.py
--rw-rw-rw-   0        0        0     1500 2020-05-26 09:11:04.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/IecTwistedPairSetupMode.py
--rw-rw-rw-   0        0        0     1668 2020-05-26 09:10:59.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/ImageTransferStatus.py
--rw-rw-rw-   0        0        0     1538 2020-05-26 09:11:02.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/ImageTransferredBlocksStatus.py
--rw-rw-rw-   0        0        0     3311 2020-05-26 09:10:56.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/Ip4SetupIpOptionType.py
--rw-rw-rw-   0        0        0     1710 2020-05-26 09:10:53.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/KeyUsage.py
--rw-rw-rw-   0        0        0     1608 2020-05-26 09:10:50.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/LocalPortResponseTime.py
--rw-rw-rw-   0        0        0     1546 2020-05-26 09:10:45.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/MBusEncryptionKeyStatus.py
--rw-rw-rw-   0        0        0     1491 2020-05-26 09:10:48.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/MacState.py
--rw-rw-rw-   0        0        0     1425 2020-05-26 09:10:42.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/MessageType.py
--rw-rw-rw-   0        0        0     1856 2020-05-26 09:13:46.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/OpticalProtocolMode.py
--rw-rw-rw-   0        0        0     1526 2020-05-26 09:13:46.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/PaymentMode.py
--rw-rw-rw-   0        0        0     1517 2020-05-26 09:13:46.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/PppAuthenticationType.py
--rw-rw-rw-   0        0        0     1418 2020-05-26 09:13:46.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/PppSetupIPCPOptionType.py
--rw-rw-rw-   0        0        0     1527 2020-05-26 09:13:46.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/PppSetupLcpOptionType.py
--rw-rw-rw-   0        0        0     1478 2020-05-26 09:13:46.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/ScriptActionType.py
--rw-rw-rw-   0        0        0     2019 2020-05-26 13:41:22.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/SecurityPolicy.py
--rw-rw-rw-   0        0        0     1780 2020-05-26 09:13:46.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/SecurityPolicy0.py
--rw-rw-rw-   0        0        0     1803 2020-05-26 09:13:46.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/SecuritySuite.py
--rw-rw-rw-   0        0        0     1897 2020-05-26 09:13:46.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/ServiceType.py
--rw-rw-rw-   0        0        0     2042 2020-05-26 09:13:46.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/SingleActionScheduleType.py
--rw-rw-rw-   0        0        0     1813 2020-05-26 09:13:46.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/SortMethod.py
--rw-rw-rw-   0        0        0     1621 2020-05-26 09:13:46.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/TokenDelivery.py
--rw-rw-rw-   0        0        0     2121 2020-05-26 09:13:46.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/TokenStatusCode.py
--rw-rw-rw-   0        0        0     1816 2020-05-26 12:44:38.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/Weekdays.py
--rw-rw-rw-   0        0        0     3583 2020-05-26 12:18:37.000000 gurux_dlms-1.0.98/gurux_dlms/objects/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2021-01-28 06:54:34.000000 gurux_dlms-1.0.98/gurux_dlms/secure/
--rw-rw-rw-   0        0        0     4257 2020-03-12 09:21:59.000000 gurux_dlms-1.0.98/gurux_dlms/secure/GXDLMSSecureClient.py
--rw-rw-rw-   0        0        0     2157 2019-08-15 11:02:46.000000 gurux_dlms-1.0.98/gurux_dlms/secure/GXDLMSSecureNotify.py
--rw-rw-rw-   0        0        0     6594 2019-08-15 11:02:46.000000 gurux_dlms-1.0.98/gurux_dlms/secure/GXDLMSSecureServer.py
--rw-rw-rw-   0        0        0     1279 2019-08-15 11:02:46.000000 gurux_dlms-1.0.98/gurux_dlms/secure/__init__.py
-drwxrwxrwx   0        0        0        0 2021-01-28 06:54:33.000000 gurux_dlms-1.0.98/gurux_dlms.egg-info/
--rw-rw-rw-   0        0        0     7195 2021-01-28 06:54:32.000000 gurux_dlms-1.0.98/gurux_dlms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11548 2021-01-28 06:54:32.000000 gurux_dlms-1.0.98/gurux_dlms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-01-28 06:54:32.000000 gurux_dlms-1.0.98/gurux_dlms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2021-01-28 06:54:32.000000 gurux_dlms-1.0.98/gurux_dlms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-01-28 06:54:34.000000 gurux_dlms-1.0.98/setup.cfg
--rw-rw-rw-   0        0        0     2286 2021-01-28 06:47:44.000000 gurux_dlms-1.0.98/setup.py
+drwxrwxrwx   0        0        0        0 2021-02-12 06:52:42.000000 gurux_dlms-1.0.99/
+-rw-rw-rw-   0        0        0     7195 2021-02-12 06:52:42.000000 gurux_dlms-1.0.99/PKG-INFO
+-rw-rw-rw-   0        0        0     5236 2020-07-13 08:30:48.000000 gurux_dlms-1.0.99/README.md
+drwxrwxrwx   0        0        0        0 2021-02-12 06:52:41.000000 gurux_dlms-1.0.99/gurux_dlms/
+-rw-rw-rw-   0        0        0     1611 2020-05-26 09:00:26.000000 gurux_dlms-1.0.99/gurux_dlms/ActionRequestType.py
+-rw-rw-rw-   0        0        0     1510 2020-05-26 08:57:45.000000 gurux_dlms-1.0.99/gurux_dlms/ActionResponseType.py
+-rw-rw-rw-   0        0        0     2909 2020-02-11 09:20:20.000000 gurux_dlms-1.0.99/gurux_dlms/AesGcmParameter.py
+-rw-rw-rw-   0        0        0     1447 2020-05-26 08:50:46.000000 gurux_dlms-1.0.99/gurux_dlms/ConfirmedServiceError.py
+-rw-rw-rw-   0        0        0     1502 2020-05-26 13:31:22.000000 gurux_dlms-1.0.99/gurux_dlms/ConnectionState.py
+-rw-rw-rw-   0        0        0     1462 2020-05-26 08:58:04.000000 gurux_dlms-1.0.99/gurux_dlms/CountType.py
+-rw-rw-rw-   0        0        0     1266 2019-09-09 12:45:06.000000 gurux_dlms-1.0.99/gurux_dlms/GXArray.py
+-rw-rw-rw-   0        0        0     3075 2020-05-26 13:46:02.000000 gurux_dlms-1.0.99/gurux_dlms/GXBitString.py
+-rw-rw-rw-   0        0        0    19670 2020-05-25 08:11:23.000000 gurux_dlms-1.0.99/gurux_dlms/GXByteBuffer.py
+-rw-rw-rw-   0        0        0     6999 2020-08-10 11:39:46.000000 gurux_dlms-1.0.99/gurux_dlms/GXCiphering.py
+-rw-rw-rw-   0        0        0    95693 2021-02-12 06:44:09.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMS.py
+-rw-rw-rw-   0        0        0     1994 2019-08-15 11:02:48.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMSAccessItem.py
+-rw-rw-rw-   0        0        0    11611 2021-01-28 06:41:03.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMSChippering.py
+-rw-rw-rw-   0        0        0    44103 2019-10-29 14:09:39.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMSChipperingStream.py
+-rw-rw-rw-   0        0        0    52375 2020-10-15 17:52:53.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMSClient.py
+-rw-rw-rw-   0        0        0     4670 2019-08-16 12:46:43.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMSConfirmedServiceError.py
+-rw-rw-rw-   0        0        0     1316 2019-08-15 11:02:48.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMSConnectionEventArgs.py
+-rw-rw-rw-   0        0        0    21745 2020-05-27 09:31:27.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMSConverter.py
+-rw-rw-rw-   0        0        0     5527 2020-08-04 13:49:25.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMSException.py
+-rw-rw-rw-   0        0        0     2900 2020-08-04 12:25:24.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMSExceptionResponse.py
+-rw-rw-rw-   0        0        0     1513 2019-08-15 11:02:48.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMSGateway.py
+-rw-rw-rw-   0        0        0    37003 2020-05-14 13:04:32.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMSLNCommandHandler.py
+-rw-rw-rw-   0        0        0     2945 2020-03-10 09:29:08.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMSLNParameters.py
+-rw-rw-rw-   0        0        0     1754 2019-08-15 11:02:48.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMSLimits.py
+-rw-rw-rw-   0        0        0     1792 2019-08-15 11:02:49.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMSLongTransaction.py
+-rw-rw-rw-   0        0        0     9738 2020-05-13 12:18:39.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMSNotify.py
+-rw-rw-rw-   0        0        0    22711 2021-01-28 06:43:59.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMSSNCommandHandler.py
+-rw-rw-rw-   0        0        0     2399 2019-08-15 11:02:48.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMSSNParameters.py
+-rw-rw-rw-   0        0        0    39149 2021-01-28 06:46:17.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMSServer.py
+-rw-rw-rw-   0        0        0    13106 2020-08-25 11:37:56.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMSSettings.py
+-rw-rw-rw-   0        0        0    87740 2021-02-12 06:49:05.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMSTranslator.py
+-rw-rw-rw-   0        0        0     7632 2019-09-04 09:24:08.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMSTranslatorStructure.py
+-rw-rw-rw-   0        0        0    12691 2020-05-13 12:19:35.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMSXmlClient.py
+-rw-rw-rw-   0        0        0     5119 2019-08-16 11:46:15.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMSXmlPdu.py
+-rw-rw-rw-   0        0        0     3622 2019-08-16 12:09:06.000000 gurux_dlms-1.0.99/gurux_dlms/GXDLMSXmlSettings.py
+-rw-rw-rw-   0        0        0     2377 2020-05-13 08:42:31.000000 gurux_dlms-1.0.99/gurux_dlms/GXDate.py
+-rw-rw-rw-   0        0        0    23358 2020-11-26 10:24:27.000000 gurux_dlms-1.0.99/gurux_dlms/GXDateTime.py
+-rw-rw-rw-   0        0        0     1233 2020-03-24 13:04:34.000000 gurux_dlms-1.0.99/gurux_dlms/GXEnum.py
+-rw-rw-rw-   0        0        0     1241 2020-05-22 06:23:32.000000 gurux_dlms-1.0.99/gurux_dlms/GXFloat32.py
+-rw-rw-rw-   0        0        0     1243 2020-05-22 06:23:58.000000 gurux_dlms-1.0.99/gurux_dlms/GXFloat64.py
+-rw-rw-rw-   0        0        0     5213 2019-08-16 11:45:19.000000 gurux_dlms-1.0.99/gurux_dlms/GXICipher.py
+-rw-rw-rw-   0        0        0     1235 2020-03-26 13:25:03.000000 gurux_dlms-1.0.99/gurux_dlms/GXInt16.py
+-rw-rw-rw-   0        0        0     1235 2020-03-26 13:28:49.000000 gurux_dlms-1.0.99/gurux_dlms/GXInt32.py
+-rw-rw-rw-   0        0        0     1235 2020-03-26 13:28:26.000000 gurux_dlms-1.0.99/gurux_dlms/GXInt64.py
+-rw-rw-rw-   0        0        0     1233 2020-03-26 13:24:26.000000 gurux_dlms-1.0.99/gurux_dlms/GXInt8.py
+-rw-rw-rw-   0        0        0     1388 2020-05-26 13:46:37.000000 gurux_dlms-1.0.99/gurux_dlms/GXIntEnum.py
+-rw-rw-rw-   0        0        0     1398 2020-05-26 13:46:43.000000 gurux_dlms-1.0.99/gurux_dlms/GXIntFlag.py
+-rw-rw-rw-   0        0        0     6250 2020-03-24 08:27:15.000000 gurux_dlms-1.0.99/gurux_dlms/GXReplyData.py
+-rw-rw-rw-   0        0        0     1656 2019-08-16 11:49:03.000000 gurux_dlms-1.0.99/gurux_dlms/GXSNInfo.py
+-rw-rw-rw-   0        0        0     5000 2020-05-14 12:19:14.000000 gurux_dlms-1.0.99/gurux_dlms/GXSecure.py
+-rw-rw-rw-   0        0        0     1751 2019-08-16 11:41:05.000000 gurux_dlms-1.0.99/gurux_dlms/GXServerReply.py
+-rw-rw-rw-   0        0        0     2094 2020-03-23 09:10:46.000000 gurux_dlms-1.0.99/gurux_dlms/GXStandardObisCode.py
+-rw-rw-rw-   0        0        0    15758 2020-08-04 12:07:39.000000 gurux_dlms-1.0.99/gurux_dlms/GXStandardObisCodeCollection.py
+-rw-rw-rw-   0        0        0     1270 2019-09-09 12:45:27.000000 gurux_dlms-1.0.99/gurux_dlms/GXStructure.py
+-rw-rw-rw-   0        0        0     2180 2020-05-13 08:42:36.000000 gurux_dlms-1.0.99/gurux_dlms/GXTime.py
+-rw-rw-rw-   0        0        0     2101 2020-05-13 13:10:30.000000 gurux_dlms-1.0.99/gurux_dlms/GXTimeZone.py
+-rw-rw-rw-   0        0        0     1237 2020-03-26 13:12:32.000000 gurux_dlms-1.0.99/gurux_dlms/GXUInt16.py
+-rw-rw-rw-   0        0        0     1331 2020-05-14 14:35:21.000000 gurux_dlms-1.0.99/gurux_dlms/GXUInt32.py
+-rw-rw-rw-   0        0        0     1237 2020-03-26 13:13:06.000000 gurux_dlms-1.0.99/gurux_dlms/GXUInt64.py
+-rw-rw-rw-   0        0        0     1235 2020-03-26 13:12:41.000000 gurux_dlms-1.0.99/gurux_dlms/GXUInt8.py
+-rw-rw-rw-   0        0        0     1901 2019-08-16 11:40:56.000000 gurux_dlms-1.0.99/gurux_dlms/GXWriteItem.py
+-rw-rw-rw-   0        0        0     1394 2019-08-15 11:02:48.000000 gurux_dlms-1.0.99/gurux_dlms/GXXmlLoadSettings.py
+-rw-rw-rw-   0        0        0     1465 2020-05-26 09:08:30.000000 gurux_dlms-1.0.99/gurux_dlms/GetCommandType.py
+-rw-rw-rw-   0        0        0     1376 2020-05-26 09:08:32.000000 gurux_dlms-1.0.99/gurux_dlms/HdlcControlFrame.py
+-rw-rw-rw-   0        0        0     8823 2020-05-15 10:31:22.000000 gurux_dlms-1.0.99/gurux_dlms/India.txt
+-rw-rw-rw-   0        0        0     7960 2019-08-15 11:02:47.000000 gurux_dlms-1.0.99/gurux_dlms/Italy.txt
+-rw-rw-rw-   0        0        0     1336 2020-05-26 09:07:44.000000 gurux_dlms-1.0.99/gurux_dlms/MBusCommand.py
+-rw-rw-rw-   0        0        0     1832 2020-05-26 09:07:50.000000 gurux_dlms-1.0.99/gurux_dlms/MBusControlInfo.py
+-rw-rw-rw-   0        0        0     1816 2020-05-26 09:07:54.000000 gurux_dlms-1.0.99/gurux_dlms/MBusEncryptionMode.py
+-rw-rw-rw-   0        0        0     1474 2020-05-26 09:07:57.000000 gurux_dlms-1.0.99/gurux_dlms/MBusMeterType.py
+-rw-rw-rw-   0        0        0   172620 2020-11-12 13:51:44.000000 gurux_dlms-1.0.99/gurux_dlms/OBISCodes.txt
+-rw-rw-rw-   0        0        0     1589 2020-05-26 09:13:46.000000 gurux_dlms-1.0.99/gurux_dlms/ReleaseRequestReason.py
+-rw-rw-rw-   0        0        0     1593 2020-05-26 09:13:46.000000 gurux_dlms-1.0.99/gurux_dlms/ReleaseResponseReason.py
+-rw-rw-rw-   0        0        0     5141 2019-08-15 11:02:48.000000 gurux_dlms-1.0.99/gurux_dlms/SaudiArabia.txt
+-rw-rw-rw-   0        0        0     3575 2020-05-14 12:28:17.000000 gurux_dlms-1.0.99/gurux_dlms/SerialnumberCounter.py
+-rw-rw-rw-   0        0        0     1829 2020-05-26 09:13:45.000000 gurux_dlms-1.0.99/gurux_dlms/ServiceError.py
+-rw-rw-rw-   0        0        0     1583 2020-05-26 09:13:45.000000 gurux_dlms-1.0.99/gurux_dlms/SetRequestType.py
+-rw-rw-rw-   0        0        0     1676 2020-05-26 09:14:24.000000 gurux_dlms-1.0.99/gurux_dlms/SetResponseType.py
+-rw-rw-rw-   0        0        0     1574 2020-05-26 09:13:32.000000 gurux_dlms-1.0.99/gurux_dlms/SingleReadResponse.py
+-rw-rw-rw-   0        0        0     1552 2020-05-26 09:13:30.000000 gurux_dlms-1.0.99/gurux_dlms/SingleWriteResponse.py
+-rw-rw-rw-   0        0        0     2247 2020-05-26 09:13:27.000000 gurux_dlms-1.0.99/gurux_dlms/TranslatorGeneralTags.py
+-rw-rw-rw-   0        0        0     1395 2020-05-26 09:14:21.000000 gurux_dlms-1.0.99/gurux_dlms/TranslatorOutputType.py
+-rw-rw-rw-   0        0        0    40626 2020-08-25 14:18:12.000000 gurux_dlms-1.0.99/gurux_dlms/TranslatorSimpleTags.py
+-rw-rw-rw-   0        0        0    41782 2020-08-25 14:18:32.000000 gurux_dlms-1.0.99/gurux_dlms/TranslatorStandardTags.py
+-rw-rw-rw-   0        0        0     4026 2020-08-04 13:00:37.000000 gurux_dlms-1.0.99/gurux_dlms/TranslatorTags.py
+-rw-rw-rw-   0        0        0     3219 2019-08-16 11:41:43.000000 gurux_dlms-1.0.99/gurux_dlms/ValueEventArgs.py
+-rw-rw-rw-   0        0        0     1705 2020-05-26 09:14:16.000000 gurux_dlms-1.0.99/gurux_dlms/VariableAccessSpecification.py
+-rw-rw-rw-   0        0        0    50521 2020-11-26 10:26:51.000000 gurux_dlms-1.0.99/gurux_dlms/_GXAPDU.py
+-rw-rw-rw-   0        0        0     4531 2019-08-15 11:02:48.000000 gurux_dlms-1.0.99/gurux_dlms/_GXFCS16.py
+-rw-rw-rw-   0        0        0    10186 2020-04-15 08:39:06.000000 gurux_dlms-1.0.99/gurux_dlms/_GXObjectFactory.py
+-rw-rw-rw-   0        0        0     1474 2019-08-16 11:50:24.000000 gurux_dlms-1.0.99/gurux_dlms/_HDLCInfo.py
+-rw-rw-rw-   0        0        0     5018 2020-08-04 13:52:18.000000 gurux_dlms-1.0.99/gurux_dlms/__init__.py
+drwxrwxrwx   0        0        0        0 2021-02-12 06:52:41.000000 gurux_dlms-1.0.99/gurux_dlms/enums/
+-rw-rw-rw-   0        0        0     1497 2020-05-26 08:51:49.000000 gurux_dlms-1.0.99/gurux_dlms/enums/Access.py
+-rw-rw-rw-   0        0        0     1715 2020-05-26 08:52:14.000000 gurux_dlms-1.0.99/gurux_dlms/enums/AccessMode.py
+-rw-rw-rw-   0        0        0     1501 2020-05-26 08:55:17.000000 gurux_dlms-1.0.99/gurux_dlms/enums/AccessServiceCommandType.py
+-rw-rw-rw-   0        0        0     1422 2020-11-26 10:30:28.000000 gurux_dlms-1.0.99/gurux_dlms/enums/AcseServiceProvider.py
+-rw-rw-rw-   0        0        0     1830 2020-05-26 09:00:06.000000 gurux_dlms-1.0.99/gurux_dlms/enums/ApplicationReference.py
+-rw-rw-rw-   0        0        0     1654 2020-05-26 09:14:10.000000 gurux_dlms-1.0.99/gurux_dlms/enums/AssociationResult.py
+-rw-rw-rw-   0        0        0     2642 2020-05-26 09:00:02.000000 gurux_dlms-1.0.99/gurux_dlms/enums/Authentication.py
+-rw-rw-rw-   0        0        0     2682 2020-05-26 08:59:58.000000 gurux_dlms-1.0.99/gurux_dlms/enums/BerType.py
+-rw-rw-rw-   0        0        0     1821 2020-05-26 08:59:54.000000 gurux_dlms-1.0.99/gurux_dlms/enums/ClockStatus.py
+-rw-rw-rw-   0        0        0    15585 2020-08-25 15:07:14.000000 gurux_dlms-1.0.99/gurux_dlms/enums/Command.py
+-rw-rw-rw-   0        0        0     7330 2020-05-26 11:52:13.000000 gurux_dlms-1.0.99/gurux_dlms/enums/Conformance.py
+-rw-rw-rw-   0        0        0     2566 2020-05-26 09:02:23.000000 gurux_dlms-1.0.99/gurux_dlms/enums/DataType.py
+-rw-rw-rw-   0        0        0     1560 2020-05-26 13:35:39.000000 gurux_dlms-1.0.99/gurux_dlms/enums/DateTimeExtraInfo.py
+-rw-rw-rw-   0        0        0     2020 2020-05-26 13:35:28.000000 gurux_dlms-1.0.99/gurux_dlms/enums/DateTimeSkips.py
+-rw-rw-rw-   0        0        0     1476 2020-05-26 08:59:42.000000 gurux_dlms-1.0.99/gurux_dlms/enums/Definition.py
+-rw-rw-rw-   0        0        0     2014 2020-05-26 08:59:36.000000 gurux_dlms-1.0.99/gurux_dlms/enums/ErrorCode.py
+-rw-rw-rw-   0        0        0     1673 2020-08-04 12:26:06.000000 gurux_dlms-1.0.99/gurux_dlms/enums/ExceptionServiceError.py
+-rw-rw-rw-   0        0        0     1512 2020-05-26 09:00:37.000000 gurux_dlms-1.0.99/gurux_dlms/enums/HardwareResource.py
+-rw-rw-rw-   0        0        0     1387 2020-05-26 09:00:47.000000 gurux_dlms-1.0.99/gurux_dlms/enums/HdlcFrameType.py
+-rw-rw-rw-   0        0        0     1484 2020-05-26 09:02:42.000000 gurux_dlms-1.0.99/gurux_dlms/enums/Initiate.py
+-rw-rw-rw-   0        0        0     1455 2020-05-26 09:00:57.000000 gurux_dlms-1.0.99/gurux_dlms/enums/InterfaceType.py
+-rw-rw-rw-   0        0        0     1616 2020-05-26 09:01:06.000000 gurux_dlms-1.0.99/gurux_dlms/enums/KeyAgreement.py
+-rw-rw-rw-   0        0        0     1785 2020-05-26 09:02:51.000000 gurux_dlms-1.0.99/gurux_dlms/enums/LoadDataSet.py
+-rw-rw-rw-   0        0        0     1466 2020-05-26 09:01:16.000000 gurux_dlms-1.0.99/gurux_dlms/enums/MethodAccessMode.py
+-rw-rw-rw-   0        0        0    12599 2020-05-26 09:01:26.000000 gurux_dlms-1.0.99/gurux_dlms/enums/ObjectType.py
+-rw-rw-rw-   0        0        0     2531 2020-05-26 09:03:02.000000 gurux_dlms-1.0.99/gurux_dlms/enums/PduType.py
+-rw-rw-rw-   0        0        0     1358 2020-05-26 09:01:35.000000 gurux_dlms-1.0.99/gurux_dlms/enums/Priority.py
+-rw-rw-rw-   0        0        0     1437 2020-07-06 13:16:03.000000 gurux_dlms-1.0.99/gurux_dlms/enums/RequestTypes.py
+-rw-rw-rw-   0        0        0     1605 2020-05-26 09:03:14.000000 gurux_dlms-1.0.99/gurux_dlms/enums/Security.py
+-rw-rw-rw-   0        0        0     1555 2020-05-26 09:03:26.000000 gurux_dlms-1.0.99/gurux_dlms/enums/Service.py
+-rw-rw-rw-   0        0        0     1372 2020-05-26 13:32:51.000000 gurux_dlms-1.0.99/gurux_dlms/enums/ServiceClass.py
+-rw-rw-rw-   0        0        0     1412 2020-05-26 09:08:55.000000 gurux_dlms-1.0.99/gurux_dlms/enums/ServiceError.py
+-rw-rw-rw-   0        0        0     2043 2020-05-26 09:08:49.000000 gurux_dlms-1.0.99/gurux_dlms/enums/SourceDiagnostic.py
+-rw-rw-rw-   0        0        0     1745 2020-05-26 09:08:47.000000 gurux_dlms-1.0.99/gurux_dlms/enums/Standard.py
+-rw-rw-rw-   0        0        0     1375 2020-05-26 09:08:44.000000 gurux_dlms-1.0.99/gurux_dlms/enums/StateError.py
+-rw-rw-rw-   0        0        0     1453 2020-05-26 09:08:42.000000 gurux_dlms-1.0.99/gurux_dlms/enums/Task.py
+-rw-rw-rw-   0        0        0     3988 2020-05-26 09:08:39.000000 gurux_dlms-1.0.99/gurux_dlms/enums/Unit.py
+-rw-rw-rw-   0        0        0     1487 2020-05-26 09:08:37.000000 gurux_dlms-1.0.99/gurux_dlms/enums/VdeStateError.py
+-rw-rw-rw-   0        0        0     2669 2020-11-26 10:29:49.000000 gurux_dlms-1.0.99/gurux_dlms/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2021-02-12 06:52:41.000000 gurux_dlms-1.0.99/gurux_dlms/internal/
+-rw-rw-rw-   0        0        0    64702 2020-08-19 06:09:03.000000 gurux_dlms-1.0.99/gurux_dlms/internal/_GXCommon.py
+-rw-rw-rw-   0        0        0     1816 2019-08-15 12:07:47.000000 gurux_dlms-1.0.99/gurux_dlms/internal/_GXDataInfo.py
+-rw-rw-rw-   0        0        0     1229 2019-08-15 11:02:48.000000 gurux_dlms-1.0.99/gurux_dlms/internal/__init__.py
+drwxrwxrwx   0        0        0        0 2021-02-12 06:52:41.000000 gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/
+-rw-rw-rw-   0        0        0     1867 2019-11-08 09:01:33.000000 gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/GXAttributeCollection.py
+-rw-rw-rw-   0        0        0     1766 2019-08-15 11:02:48.000000 gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/GXAuthentication.py
+-rw-rw-rw-   0        0        0     1778 2019-08-16 12:37:42.000000 gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/GXDLMSAttribute.py
+-rw-rw-rw-   0        0        0     2177 2019-08-16 08:46:08.000000 gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/GXDLMSAttributeSettings.py
+-rw-rw-rw-   0        0        0     2485 2019-08-15 11:02:48.000000 gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/GXManufacturer.py
+-rw-rw-rw-   0        0        0     9221 2019-08-16 13:58:57.000000 gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/GXManufacturerCollection.py
+-rw-rw-rw-   0        0        0     1855 2020-03-24 14:31:21.000000 gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/GXObisCode.py
+-rw-rw-rw-   0        0        0     1473 2019-08-15 11:02:48.000000 gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/GXObisCodeCollection.py
+-rw-rw-rw-   0        0        0     1502 2019-08-15 11:02:48.000000 gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/GXObisValueItem.py
+-rw-rw-rw-   0        0        0     1866 2019-08-16 12:37:57.000000 gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/GXObisValueItemCollection.py
+-rw-rw-rw-   0        0        0     1649 2019-08-15 11:02:48.000000 gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/GXServerAddress.py
+-rw-rw-rw-   0        0        0     1348 2020-05-26 09:08:16.000000 gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/HDLCAddressType.py
+-rw-rw-rw-   0        0        0     1513 2020-05-26 09:08:13.000000 gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/InactivityMode.py
+-rw-rw-rw-   0        0        0     1469 2020-05-26 09:08:10.000000 gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/StartProtocolType.py
+-rw-rw-rw-   0        0        0      482 2019-08-15 11:02:48.000000 gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/__init__.py
+drwxrwxrwx   0        0        0        0 2021-02-12 06:52:42.000000 gurux_dlms-1.0.99/gurux_dlms/objects/
+-rw-rw-rw-   0        0        0     1474 2019-08-16 08:59:10.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXAdjacentCell.py
+-rw-rw-rw-   0        0        0     1983 2019-08-16 08:42:12.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXApplicationContextName.py
+-rw-rw-rw-   0        0        0     1996 2019-08-16 09:27:26.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXAuthenticationMechanismName.py
+-rw-rw-rw-   0        0        0     1599 2019-08-16 13:03:06.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXChargePerUnitScaling.py
+-rw-rw-rw-   0        0        0     1528 2019-08-16 09:31:32.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXChargeTable.py
+-rw-rw-rw-   0        0        0     1580 2019-08-15 13:16:33.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXCommodity.py
+-rw-rw-rw-   0        0        0     1656 2019-08-15 13:20:30.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXCreditChargeConfiguration.py
+-rw-rw-rw-   0        0        0     1782 2019-08-16 08:34:48.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXCurrency.py
+-rw-rw-rw-   0        0        0    22795 2020-09-08 06:15:54.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSAccount.py
+-rw-rw-rw-   0        0        0     1534 2019-08-16 09:28:09.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSActionItem.py
+-rw-rw-rw-   0        0        0     8620 2020-05-27 08:16:51.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSActionSchedule.py
+-rw-rw-rw-   0        0        0     1501 2019-08-16 09:07:30.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSActionSet.py
+-rw-rw-rw-   0        0        0    20076 2020-08-26 12:59:51.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSActivityCalendar.py
+-rw-rw-rw-   0        0        0    32168 2020-06-03 10:59:11.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSAssociationLogicalName.py
+-rw-rw-rw-   0        0        0    10529 2020-05-14 12:07:49.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSAssociationShortName.py
+-rw-rw-rw-   0        0        0     8616 2020-05-14 13:12:47.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSAutoAnswer.py
+-rw-rw-rw-   0        0        0     8557 2020-05-14 13:13:07.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSAutoConnect.py
+-rw-rw-rw-   0        0        0     1522 2019-08-16 08:37:07.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSCaptureObject.py
+-rw-rw-rw-   0        0        0     1653 2019-08-16 08:28:06.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSCertificateInfo.py
+-rw-rw-rw-   0        0        0    13422 2020-05-27 06:43:30.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSCharge.py
+-rw-rw-rw-   0        0        0    10000 2020-05-14 13:13:54.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSClock.py
+-rw-rw-rw-   0        0        0     9667 2020-11-26 10:25:22.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSCredit.py
+-rw-rw-rw-   0        0        0     3721 2020-03-26 14:20:36.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSData.py
+-rw-rw-rw-   0        0        0     1801 2019-08-15 13:20:05.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSDayProfile.py
+-rw-rw-rw-   0        0        0     1852 2019-08-15 13:46:23.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSDayProfileAction.py
+-rw-rw-rw-   0        0        0    11377 2020-05-27 06:44:03.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSDemandRegister.py
+-rw-rw-rw-   0        0        0     5471 2020-03-23 08:05:49.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSDisconnectControl.py
+-rw-rw-rw-   0        0        0     1584 2019-08-16 08:40:21.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSEmergencyProfile.py
+-rw-rw-rw-   0        0        0     7653 2020-05-27 06:44:27.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSExtendedRegister.py
+-rw-rw-rw-   0        0        0     1589 2019-08-16 09:31:50.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSGSMCellInfo.py
+-rw-rw-rw-   0        0        0    11616 2020-05-27 06:25:25.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSGSMDiagnostic.py
+-rw-rw-rw-   0        0        0     9679 2020-05-14 13:14:26.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSGprsSetup.py
+-rw-rw-rw-   0        0        0     8108 2020-03-24 08:05:35.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSHdlcSetup.py
+-rw-rw-rw-   0        0        0     7922 2020-05-14 13:14:45.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSIECLocalPortSetup.py
+-rw-rw-rw-   0        0        0     5540 2019-08-16 13:02:13.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSIecTwistedPairSetup.py
+-rw-rw-rw-   0        0        0     2158 2019-08-16 09:02:40.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSImageActivateInfo.py
+-rw-rw-rw-   0        0        0    13230 2020-05-14 11:37:06.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSImageTransfer.py
+-rw-rw-rw-   0        0        0    11925 2020-05-13 13:20:58.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSIp4Setup.py
+-rw-rw-rw-   0        0        0     1431 2019-08-16 08:59:33.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSIp4SetupIpOption.py
+-rw-rw-rw-   0        0        0    14170 2020-05-27 07:54:03.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSIp6Setup.py
+-rw-rw-rw-   0        0        0    15527 2020-05-14 13:51:57.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSLimiter.py
+-rw-rw-rw-   0        0        0     4728 2020-04-15 08:57:01.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSLlcSscsSetup.py
+-rw-rw-rw-   0        0        0    12445 2020-05-14 13:15:10.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSMBusClient.py
+-rw-rw-rw-   0        0        0     3672 2020-05-27 06:51:27.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSMBusMasterPortSetup.py
+-rw-rw-rw-   0        0        0     6196 2020-03-26 14:33:32.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSMBusSlavePortSetup.py
+-rw-rw-rw-   0        0        0     3982 2019-08-16 13:05:44.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSMacAddressSetup.py
+-rw-rw-rw-   0        0        0     7902 2020-05-27 06:52:48.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSModemConfiguration.py
+-rw-rw-rw-   0        0        0     1552 2019-08-16 08:29:04.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSModemInitialisation.py
+-rw-rw-rw-   0        0        0     1793 2019-08-16 08:36:52.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSMonitoredValue.py
+-rw-rw-rw-   0        0        0     8528 2020-11-09 07:33:57.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSObject.py
+-rw-rw-rw-   0        0        0     5792 2020-05-27 09:32:22.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSObjectCollection.py
+-rw-rw-rw-   0        0        0     1550 2019-08-16 08:37:52.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSObjectDefinition.py
+-rw-rw-rw-   0        0        0    12722 2020-05-14 13:15:19.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSParameterMonitor.py
+-rw-rw-rw-   0        0        0    10040 2020-05-13 12:14:37.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSPppSetup.py
+-rw-rw-rw-   0        0        0     1462 2019-08-16 08:40:47.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSPppSetupIPCPOption.py
+-rw-rw-rw-   0        0        0     1527 2019-08-16 08:41:02.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSPppSetupLcpOption.py
+-rw-rw-rw-   0        0        0     5197 2020-08-25 15:10:40.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSPrimeNbOfdmPlcApplicationsIdentification.py
+-rw-rw-rw-   0        0        0     7195 2020-04-15 11:37:00.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSPrimeNbOfdmPlcMacCounters.py
+-rw-rw-rw-   0        0        0    10411 2020-05-27 06:26:30.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSPrimeNbOfdmPlcMacFunctionalParameters.py
+-rw-rw-rw-   0        0        0    19391 2020-05-27 06:35:00.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSPrimeNbOfdmPlcMacNetworkAdministrationData.py
+-rw-rw-rw-   0        0        0     7106 2020-04-15 12:03:38.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSPrimeNbOfdmPlcMacSetup.py
+-rw-rw-rw-   0        0        0     6100 2020-04-15 10:47:54.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSPrimeNbOfdmPlcPhysicalLayerCounters.py
+-rw-rw-rw-   0        0        0    23426 2020-11-09 07:29:46.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSProfileGeneric.py
+-rw-rw-rw-   0        0        0    11845 2020-05-27 07:02:46.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSPushSetup.py
+-rw-rw-rw-   0        0        0     1531 2019-08-16 09:29:29.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSQualityOfService.py
+-rw-rw-rw-   0        0        0     6007 2020-11-09 07:56:39.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSRegister.py
+-rw-rw-rw-   0        0        0     8017 2020-05-13 12:14:37.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSRegisterActivation.py
+-rw-rw-rw-   0        0        0     9772 2020-05-27 08:05:40.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSRegisterMonitor.py
+-rw-rw-rw-   0        0        0     5370 2020-05-14 13:15:35.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSSapAssignment.py
+-rw-rw-rw-   0        0        0    10429 2021-01-27 13:24:26.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSSchedule.py
+-rw-rw-rw-   0        0        0     2290 2019-08-16 08:33:06.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSScheduleEntry.py
+-rw-rw-rw-   0        0        0     1531 2019-08-16 08:37:28.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSScript.py
+-rw-rw-rw-   0        0        0     2294 2020-05-14 11:58:39.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSScriptAction.py
+-rw-rw-rw-   0        0        0    10359 2020-05-27 08:01:32.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSScriptTable.py
+-rw-rw-rw-   0        0        0     1912 2020-03-19 12:02:21.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSSeasonProfile.py
+-rw-rw-rw-   0        0        0    19569 2020-05-26 13:42:48.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSSecuritySetup.py
+-rw-rw-rw-   0        0        0     1518 2019-09-18 06:59:18.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSSpecialDay.py
+-rw-rw-rw-   0        0        0     7467 2020-08-18 13:50:59.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSSpecialDaysTable.py
+-rw-rw-rw-   0        0        0     1634 2019-08-16 08:42:33.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSTarget.py
+-rw-rw-rw-   0        0        0     6670 2019-08-16 13:11:58.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSTcpUdpSetup.py
+-rw-rw-rw-   0        0        0     7611 2020-05-14 13:16:08.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSTokenGateway.py
+-rw-rw-rw-   0        0        0     4701 2020-04-21 06:56:57.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSUtilityTables.py
+-rw-rw-rw-   0        0        0     1728 2020-03-10 07:32:34.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSWeekProfile.py
+-rw-rw-rw-   0        0        0     1721 2020-04-15 11:46:04.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXMacAvailableSwitch.py
+-rw-rw-rw-   0        0        0     2041 2020-04-15 11:44:28.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXMacDirectTable.py
+-rw-rw-rw-   0        0        0     1480 2020-04-15 11:42:33.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXMacMulticastEntry.py
+-rw-rw-rw-   0        0        0     2217 2020-04-21 06:57:57.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXMacPhyCommunication.py
+-rw-rw-rw-   0        0        0     1671 2019-08-16 08:41:53.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXNeighborDiscoverySetup.py
+-rw-rw-rw-   0        0        0     1599 2019-08-16 08:58:58.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXTokenGatewayConfiguration.py
+-rw-rw-rw-   0        0        0     1907 2019-08-16 08:59:52.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXUnitCharge.py
+-rw-rw-rw-   0        0        0     6626 2020-05-13 08:40:48.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXXmlReader.py
+-rw-rw-rw-   0        0        0     6679 2020-05-27 07:58:18.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXXmlWriter.py
+-rw-rw-rw-   0        0        0     1471 2019-08-16 10:23:04.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXXmlWriterSettings.py
+-rw-rw-rw-   0        0        0     3867 2019-08-16 10:20:20.000000 gurux_dlms-1.0.99/gurux_dlms/objects/GXxDLMSContextType.py
+-rw-rw-rw-   0        0        0     3313 2019-08-15 12:57:54.000000 gurux_dlms-1.0.99/gurux_dlms/objects/IGXDLMSBase.py
+-rw-rw-rw-   0        0        0     6463 2020-05-27 07:03:16.000000 gurux_dlms-1.0.99/gurux_dlms/objects/__init__.py
+drwxrwxrwx   0        0        0        0 2021-02-12 06:52:42.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/
+-rw-rw-rw-   0        0        0     1990 2020-05-26 13:33:57.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/AccountCreditStatus.py
+-rw-rw-rw-   0        0        0     1614 2020-05-26 09:08:01.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/AccountStatus.py
+-rw-rw-rw-   0        0        0     1578 2020-05-26 09:07:39.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/AddressConfigMode.py
+-rw-rw-rw-   0        0        0     1599 2020-05-26 09:07:15.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/AddressState.py
+-rw-rw-rw-   0        0        0     1650 2020-05-26 09:14:46.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/ApplicationContextName.py
+-rw-rw-rw-   0        0        0     1620 2020-05-26 09:14:59.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/AssociationStatus.py
+-rw-rw-rw-   0        0        0     1933 2020-05-26 09:06:51.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/AutoAnswerMode.py
+-rw-rw-rw-   0        0        0     1356 2020-05-26 09:06:55.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/AutoAnswerStatus.py
+-rw-rw-rw-   0        0        0     2915 2020-05-26 09:07:00.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/AutoConnectMode.py
+-rw-rw-rw-   0        0        0     1987 2020-05-26 09:06:47.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/BaudRate.py
+-rw-rw-rw-   0        0        0     1645 2020-05-26 09:06:23.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/CertificateEntity.py
+-rw-rw-rw-   0        0        0     1632 2020-05-26 09:06:16.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/CertificateIdentificationType.py
+-rw-rw-rw-   0        0        0     1632 2020-05-26 09:11:37.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/CertificateType.py
+-rw-rw-rw-   0        0        0     1456 2020-05-26 13:47:49.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/ChargeConfiguration.py
+-rw-rw-rw-   0        0        0     1687 2020-05-26 09:11:35.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/ChargeType.py
+-rw-rw-rw-   0        0        0     1708 2020-05-26 09:11:32.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/ClockBase.py
+-rw-rw-rw-   0        0        0     2326 2020-05-26 09:11:30.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/ControlMode.py
+-rw-rw-rw-   0        0        0     1714 2020-05-26 09:11:27.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/ControlState.py
+-rw-rw-rw-   0        0        0     1674 2020-05-26 12:08:59.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/CreditCollectionConfiguration.py
+-rw-rw-rw-   0        0        0     1886 2020-05-26 13:34:27.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/CreditConfiguration.py
+-rw-rw-rw-   0        0        0     1705 2020-05-26 09:11:25.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/CreditStatus.py
+-rw-rw-rw-   0        0        0     1712 2020-05-26 09:11:22.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/CreditType.py
+-rw-rw-rw-   0        0        0     1560 2020-05-26 09:11:20.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/Currency.py
+-rw-rw-rw-   0        0        0     1765 2020-05-26 09:11:17.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/GlobalKeyType.py
+-rw-rw-rw-   0        0        0     1514 2020-05-26 09:11:15.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/GsmCircuitSwitchStatus.py
+-rw-rw-rw-   0        0        0     1657 2020-05-26 09:11:11.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/GsmPacketSwitchStatus.py
+-rw-rw-rw-   0        0        0     1597 2020-05-26 09:11:07.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/GsmStatus.py
+-rw-rw-rw-   0        0        0     1500 2020-05-26 09:11:04.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/IecTwistedPairSetupMode.py
+-rw-rw-rw-   0        0        0     1668 2020-05-26 09:10:59.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/ImageTransferStatus.py
+-rw-rw-rw-   0        0        0     1538 2020-05-26 09:11:02.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/ImageTransferredBlocksStatus.py
+-rw-rw-rw-   0        0        0     3311 2020-05-26 09:10:56.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/Ip4SetupIpOptionType.py
+-rw-rw-rw-   0        0        0     1710 2020-05-26 09:10:53.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/KeyUsage.py
+-rw-rw-rw-   0        0        0     1608 2020-05-26 09:10:50.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/LocalPortResponseTime.py
+-rw-rw-rw-   0        0        0     1546 2020-05-26 09:10:45.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/MBusEncryptionKeyStatus.py
+-rw-rw-rw-   0        0        0     1491 2020-05-26 09:10:48.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/MacState.py
+-rw-rw-rw-   0        0        0     1425 2020-05-26 09:10:42.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/MessageType.py
+-rw-rw-rw-   0        0        0     1856 2020-05-26 09:13:46.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/OpticalProtocolMode.py
+-rw-rw-rw-   0        0        0     1526 2020-05-26 09:13:46.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/PaymentMode.py
+-rw-rw-rw-   0        0        0     1517 2020-05-26 09:13:46.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/PppAuthenticationType.py
+-rw-rw-rw-   0        0        0     1418 2020-05-26 09:13:46.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/PppSetupIPCPOptionType.py
+-rw-rw-rw-   0        0        0     1527 2020-05-26 09:13:46.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/PppSetupLcpOptionType.py
+-rw-rw-rw-   0        0        0     1478 2020-05-26 09:13:46.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/ScriptActionType.py
+-rw-rw-rw-   0        0        0     2019 2020-05-26 13:41:22.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/SecurityPolicy.py
+-rw-rw-rw-   0        0        0     1780 2020-05-26 09:13:46.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/SecurityPolicy0.py
+-rw-rw-rw-   0        0        0     1803 2020-05-26 09:13:46.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/SecuritySuite.py
+-rw-rw-rw-   0        0        0     1897 2020-05-26 09:13:46.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/ServiceType.py
+-rw-rw-rw-   0        0        0     2042 2020-05-26 09:13:46.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/SingleActionScheduleType.py
+-rw-rw-rw-   0        0        0     1813 2020-05-26 09:13:46.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/SortMethod.py
+-rw-rw-rw-   0        0        0     1621 2020-05-26 09:13:46.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/TokenDelivery.py
+-rw-rw-rw-   0        0        0     2121 2020-05-26 09:13:46.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/TokenStatusCode.py
+-rw-rw-rw-   0        0        0     1816 2020-05-26 12:44:38.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/Weekdays.py
+-rw-rw-rw-   0        0        0     3583 2020-05-26 12:18:37.000000 gurux_dlms-1.0.99/gurux_dlms/objects/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2021-02-12 06:52:42.000000 gurux_dlms-1.0.99/gurux_dlms/secure/
+-rw-rw-rw-   0        0        0     4257 2020-03-12 09:21:59.000000 gurux_dlms-1.0.99/gurux_dlms/secure/GXDLMSSecureClient.py
+-rw-rw-rw-   0        0        0     2157 2019-08-15 11:02:46.000000 gurux_dlms-1.0.99/gurux_dlms/secure/GXDLMSSecureNotify.py
+-rw-rw-rw-   0        0        0     6594 2019-08-15 11:02:46.000000 gurux_dlms-1.0.99/gurux_dlms/secure/GXDLMSSecureServer.py
+-rw-rw-rw-   0        0        0     1279 2019-08-15 11:02:46.000000 gurux_dlms-1.0.99/gurux_dlms/secure/__init__.py
+drwxrwxrwx   0        0        0        0 2021-02-12 06:52:41.000000 gurux_dlms-1.0.99/gurux_dlms.egg-info/
+-rw-rw-rw-   0        0        0     7195 2021-02-12 06:52:40.000000 gurux_dlms-1.0.99/gurux_dlms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11548 2021-02-12 06:52:40.000000 gurux_dlms-1.0.99/gurux_dlms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-02-12 06:52:40.000000 gurux_dlms-1.0.99/gurux_dlms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2021-02-12 06:52:40.000000 gurux_dlms-1.0.99/gurux_dlms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-02-12 06:52:42.000000 gurux_dlms-1.0.99/setup.cfg
+-rw-rw-rw-   0        0        0     2286 2021-02-12 06:47:24.000000 gurux_dlms-1.0.99/setup.py
```

### Comparing `gurux_dlms-1.0.98/PKG-INFO` & `gurux_dlms-1.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gurux_dlms
-Version: 1.0.98
+Version: 1.0.99
 Summary: Gurux DLMS library for Python.
 Home-page: https://github.com/gurux/gurux.dlms.python
 Author: Gurux Ltd
 Author-email: gurux@gurux.fi
 License: GPLv2
 Description: See An [Gurux](http://www.gurux.org/ "Gurux") for an overview.
```

### Comparing `gurux_dlms-1.0.98/README.md` & `gurux_dlms-1.0.99/README.md`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/ActionRequestType.py` & `gurux_dlms-1.0.99/gurux_dlms/ActionRequestType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/ActionResponseType.py` & `gurux_dlms-1.0.99/gurux_dlms/ActionResponseType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/AesGcmParameter.py` & `gurux_dlms-1.0.99/gurux_dlms/AesGcmParameter.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/ConfirmedServiceError.py` & `gurux_dlms-1.0.99/gurux_dlms/ConfirmedServiceError.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/ConnectionState.py` & `gurux_dlms-1.0.99/gurux_dlms/ConnectionState.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/CountType.py` & `gurux_dlms-1.0.99/gurux_dlms/CountType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXArray.py` & `gurux_dlms-1.0.99/gurux_dlms/GXArray.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXBitString.py` & `gurux_dlms-1.0.99/gurux_dlms/GXBitString.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXByteBuffer.py` & `gurux_dlms-1.0.99/gurux_dlms/GXByteBuffer.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXCiphering.py` & `gurux_dlms-1.0.99/gurux_dlms/GXCiphering.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMS.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMS.py`

 * *Files 0% similar despite different names*

```diff
@@ -1664,19 +1664,18 @@
                 pass
             elif cmd == Command.GENERAL_CIPHERING:
                 cls.handleGeneralCiphering(settings, data)
             elif cmd == Command.GATEWAY_REQUEST:
                 pass
             elif cmd == Command.GATEWAY_RESPONSE:
                 data.data.getUInt8()
-                len_ = _GXCommon.getObjectCount(data.data)
-                pda = bytearray(len_)
+                pda = bytearray(_GXCommon.getObjectCount(data.data))
                 data.data.get(pda)
-                cls.getDataFromBlock(data, index)
-                data.command = (Command.NONE)
+                cls.getDataFromBlock(data.data, index)
+                data.command = Command.NONE
                 cls.getPdu(settings, data)
             else:
                 raise ValueError("Invalid Command.")
         elif (data.moreData & RequestTypes.FRAME) == 0:
             if not data.peek and data.moreData == RequestTypes.NONE:
                 if data.command == Command.AARE or data.command == Command.AARQ:
                     data.data.position = 0
```

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMSAccessItem.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMSAccessItem.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMSChippering.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMSChippering.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMSChipperingStream.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMSChipperingStream.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMSClient.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMSClient.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMSConfirmedServiceError.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMSConfirmedServiceError.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMSConnectionEventArgs.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMSConnectionEventArgs.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMSConverter.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMSConverter.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMSException.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMSException.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMSExceptionResponse.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMSExceptionResponse.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMSGateway.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMSGateway.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMSLNCommandHandler.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMSLNCommandHandler.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMSLNParameters.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMSLNParameters.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMSLimits.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMSLimits.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMSLongTransaction.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMSLongTransaction.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMSNotify.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMSNotify.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMSSNCommandHandler.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMSSNCommandHandler.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMSSNParameters.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMSSNParameters.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMSServer.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMSServer.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMSSettings.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMSSettings.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMSTranslator.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMSTranslator.py`

 * *Files 0% similar despite different names*

```diff
@@ -513,15 +513,16 @@
     def isCiphered(cls, cmd):
         return cmd in (Command.GENERAL_GLO_CIPHERING, Command.GENERAL_DED_CIPHERING,\
             Command.GLO_READ_REQUEST, Command.GLO_WRITE_REQUEST, Command.GLO_GET_REQUEST,\
             Command.GLO_SET_REQUEST, Command.GLO_READ_RESPONSE, Command.GLO_WRITE_RESPONSE,\
             Command.GLO_GET_RESPONSE, Command.GLO_SET_RESPONSE, Command.GLO_METHOD_REQUEST,\
             Command.GLO_METHOD_RESPONSE, Command.DED_GET_REQUEST, Command.DED_SET_REQUEST,\
             Command.DED_READ_RESPONSE, Command.DED_GET_RESPONSE, Command.DED_SET_RESPONSE,\
-            Command.DED_METHOD_REQUEST, Command.DED_METHOD_RESPONSE, Command.GLO_CONFIRMED_SERVICE_ERROR, Command.DED_CONFIRMED_SERVICE_ERROR)
+            Command.DED_METHOD_REQUEST, Command.DED_METHOD_RESPONSE, Command.GLO_CONFIRMED_SERVICE_ERROR,\
+            Command.DED_CONFIRMED_SERVICE_ERROR, Command.GENERAL_CIPHERING)
 
     #
     # Convert bytes to XML.
     #
     # @param value
     #            Bytes to convert.
     # Converted XML.
```

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMSTranslatorStructure.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMSTranslatorStructure.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMSXmlClient.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMSXmlClient.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMSXmlPdu.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMSXmlPdu.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDLMSXmlSettings.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDLMSXmlSettings.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDate.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDate.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXDateTime.py` & `gurux_dlms-1.0.99/gurux_dlms/GXDateTime.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXEnum.py` & `gurux_dlms-1.0.99/gurux_dlms/GXEnum.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXFloat32.py` & `gurux_dlms-1.0.99/gurux_dlms/GXFloat32.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXFloat64.py` & `gurux_dlms-1.0.99/gurux_dlms/GXFloat64.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXICipher.py` & `gurux_dlms-1.0.99/gurux_dlms/GXICipher.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXInt16.py` & `gurux_dlms-1.0.99/gurux_dlms/GXInt16.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXInt32.py` & `gurux_dlms-1.0.99/gurux_dlms/GXInt32.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXInt64.py` & `gurux_dlms-1.0.99/gurux_dlms/GXInt64.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXInt8.py` & `gurux_dlms-1.0.99/gurux_dlms/GXInt8.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXIntEnum.py` & `gurux_dlms-1.0.99/gurux_dlms/GXIntEnum.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXIntFlag.py` & `gurux_dlms-1.0.99/gurux_dlms/GXIntFlag.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXReplyData.py` & `gurux_dlms-1.0.99/gurux_dlms/GXReplyData.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXSNInfo.py` & `gurux_dlms-1.0.99/gurux_dlms/GXSNInfo.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXSecure.py` & `gurux_dlms-1.0.99/gurux_dlms/GXSecure.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXServerReply.py` & `gurux_dlms-1.0.99/gurux_dlms/GXServerReply.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXStandardObisCode.py` & `gurux_dlms-1.0.99/gurux_dlms/GXStandardObisCode.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXStandardObisCodeCollection.py` & `gurux_dlms-1.0.99/gurux_dlms/GXStandardObisCodeCollection.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXStructure.py` & `gurux_dlms-1.0.99/gurux_dlms/GXStructure.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXTime.py` & `gurux_dlms-1.0.99/gurux_dlms/GXTime.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXTimeZone.py` & `gurux_dlms-1.0.99/gurux_dlms/GXTimeZone.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXUInt16.py` & `gurux_dlms-1.0.99/gurux_dlms/GXUInt16.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXUInt32.py` & `gurux_dlms-1.0.99/gurux_dlms/GXUInt32.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXUInt64.py` & `gurux_dlms-1.0.99/gurux_dlms/GXUInt64.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXUInt8.py` & `gurux_dlms-1.0.99/gurux_dlms/GXUInt8.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXWriteItem.py` & `gurux_dlms-1.0.99/gurux_dlms/GXWriteItem.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GXXmlLoadSettings.py` & `gurux_dlms-1.0.99/gurux_dlms/GXXmlLoadSettings.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/GetCommandType.py` & `gurux_dlms-1.0.99/gurux_dlms/GetCommandType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/HdlcControlFrame.py` & `gurux_dlms-1.0.99/gurux_dlms/HdlcControlFrame.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/India.txt` & `gurux_dlms-1.0.99/gurux_dlms/India.txt`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/Italy.txt` & `gurux_dlms-1.0.99/gurux_dlms/Italy.txt`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/MBusCommand.py` & `gurux_dlms-1.0.99/gurux_dlms/MBusCommand.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/MBusControlInfo.py` & `gurux_dlms-1.0.99/gurux_dlms/MBusControlInfo.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/MBusEncryptionMode.py` & `gurux_dlms-1.0.99/gurux_dlms/MBusEncryptionMode.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/MBusMeterType.py` & `gurux_dlms-1.0.99/gurux_dlms/MBusMeterType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/OBISCodes.txt` & `gurux_dlms-1.0.99/gurux_dlms/OBISCodes.txt`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/ReleaseRequestReason.py` & `gurux_dlms-1.0.99/gurux_dlms/ReleaseRequestReason.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/ReleaseResponseReason.py` & `gurux_dlms-1.0.99/gurux_dlms/ReleaseResponseReason.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/SaudiArabia.txt` & `gurux_dlms-1.0.99/gurux_dlms/SaudiArabia.txt`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/SerialnumberCounter.py` & `gurux_dlms-1.0.99/gurux_dlms/SerialnumberCounter.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/ServiceError.py` & `gurux_dlms-1.0.99/gurux_dlms/ServiceError.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/SetRequestType.py` & `gurux_dlms-1.0.99/gurux_dlms/SetRequestType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/SetResponseType.py` & `gurux_dlms-1.0.99/gurux_dlms/SetResponseType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/SingleReadResponse.py` & `gurux_dlms-1.0.99/gurux_dlms/SingleReadResponse.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/SingleWriteResponse.py` & `gurux_dlms-1.0.99/gurux_dlms/SingleWriteResponse.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/TranslatorGeneralTags.py` & `gurux_dlms-1.0.99/gurux_dlms/TranslatorGeneralTags.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/TranslatorOutputType.py` & `gurux_dlms-1.0.99/gurux_dlms/TranslatorOutputType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/TranslatorSimpleTags.py` & `gurux_dlms-1.0.99/gurux_dlms/TranslatorSimpleTags.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/TranslatorStandardTags.py` & `gurux_dlms-1.0.99/gurux_dlms/TranslatorStandardTags.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/TranslatorTags.py` & `gurux_dlms-1.0.99/gurux_dlms/TranslatorTags.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/ValueEventArgs.py` & `gurux_dlms-1.0.99/gurux_dlms/ValueEventArgs.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/VariableAccessSpecification.py` & `gurux_dlms-1.0.99/gurux_dlms/VariableAccessSpecification.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/_GXAPDU.py` & `gurux_dlms-1.0.99/gurux_dlms/_GXAPDU.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/_GXFCS16.py` & `gurux_dlms-1.0.99/gurux_dlms/_GXFCS16.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/_GXObjectFactory.py` & `gurux_dlms-1.0.99/gurux_dlms/_GXObjectFactory.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/_HDLCInfo.py` & `gurux_dlms-1.0.99/gurux_dlms/_HDLCInfo.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/__init__.py` & `gurux_dlms-1.0.99/gurux_dlms/__init__.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/Access.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/Access.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/AccessMode.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/AccessMode.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/AccessServiceCommandType.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/AccessServiceCommandType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/AcseServiceProvider.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/AcseServiceProvider.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/ApplicationReference.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/ApplicationReference.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/AssociationResult.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/AssociationResult.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/Authentication.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/Authentication.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/BerType.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/BerType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/ClockStatus.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/ClockStatus.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/Command.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/Command.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/Conformance.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/Conformance.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/DataType.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/DataType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/DateTimeExtraInfo.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/DateTimeExtraInfo.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/DateTimeSkips.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/DateTimeSkips.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/Definition.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/Definition.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/ErrorCode.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/ExceptionServiceError.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/ExceptionServiceError.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/HardwareResource.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/HardwareResource.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/HdlcFrameType.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/HdlcFrameType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/Initiate.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/Initiate.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/InterfaceType.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/InterfaceType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/KeyAgreement.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/KeyAgreement.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/LoadDataSet.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/LoadDataSet.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/MethodAccessMode.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/MethodAccessMode.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/ObjectType.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/ObjectType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/PduType.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/PduType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/Priority.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/Priority.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/RequestTypes.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/RequestTypes.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/Security.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/Security.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/Service.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/Service.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/ServiceClass.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/ServiceClass.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/ServiceError.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/ServiceError.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/SourceDiagnostic.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/SourceDiagnostic.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/Standard.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/Standard.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/StateError.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/StateError.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/Task.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/Task.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/Unit.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/Unit.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/VdeStateError.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/VdeStateError.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/enums/__init__.py` & `gurux_dlms-1.0.99/gurux_dlms/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/internal/_GXCommon.py` & `gurux_dlms-1.0.99/gurux_dlms/internal/_GXCommon.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/internal/_GXDataInfo.py` & `gurux_dlms-1.0.99/gurux_dlms/internal/_GXDataInfo.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/internal/__init__.py` & `gurux_dlms-1.0.99/gurux_dlms/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/GXAttributeCollection.py` & `gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/GXAttributeCollection.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/GXAuthentication.py` & `gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/GXAuthentication.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/GXDLMSAttribute.py` & `gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/GXDLMSAttribute.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/GXDLMSAttributeSettings.py` & `gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/GXDLMSAttributeSettings.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/GXManufacturer.py` & `gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/GXManufacturer.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/GXManufacturerCollection.py` & `gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/GXManufacturerCollection.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/GXObisCode.py` & `gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/GXObisCode.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/GXObisCodeCollection.py` & `gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/GXObisCodeCollection.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/GXObisValueItem.py` & `gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/GXObisValueItem.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/GXObisValueItemCollection.py` & `gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/GXObisValueItemCollection.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/GXServerAddress.py` & `gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/GXServerAddress.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/HDLCAddressType.py` & `gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/HDLCAddressType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/InactivityMode.py` & `gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/InactivityMode.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/manufacturersettings/StartProtocolType.py` & `gurux_dlms-1.0.99/gurux_dlms/manufacturersettings/StartProtocolType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXAdjacentCell.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXAdjacentCell.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXApplicationContextName.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXApplicationContextName.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXAuthenticationMechanismName.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXAuthenticationMechanismName.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXChargePerUnitScaling.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXChargePerUnitScaling.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXChargeTable.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXChargeTable.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXCommodity.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXCommodity.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXCreditChargeConfiguration.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXCreditChargeConfiguration.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXCurrency.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXCurrency.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSAccount.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSAccount.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSActionItem.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSActionItem.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSActionSchedule.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSActionSchedule.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSActionSet.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSActionSet.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSActivityCalendar.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSActivityCalendar.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSAssociationLogicalName.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSAssociationLogicalName.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSAssociationShortName.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSAssociationShortName.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSAutoAnswer.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSAutoAnswer.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSAutoConnect.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSAutoConnect.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSCaptureObject.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSCaptureObject.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSCertificateInfo.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSCertificateInfo.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSCharge.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSCharge.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSClock.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSClock.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSCredit.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSCredit.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSData.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSData.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSDayProfile.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSDayProfile.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSDayProfileAction.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSDayProfileAction.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSDemandRegister.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSDemandRegister.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSDisconnectControl.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSDisconnectControl.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSEmergencyProfile.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSEmergencyProfile.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSExtendedRegister.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSExtendedRegister.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSGSMCellInfo.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSGSMCellInfo.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSGSMDiagnostic.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSGSMDiagnostic.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSGprsSetup.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSGprsSetup.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSHdlcSetup.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSHdlcSetup.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSIECLocalPortSetup.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSIECLocalPortSetup.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSIecTwistedPairSetup.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSIecTwistedPairSetup.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSImageActivateInfo.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSImageActivateInfo.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSImageTransfer.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSImageTransfer.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSIp4Setup.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSIp4Setup.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSIp4SetupIpOption.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSIp4SetupIpOption.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSIp6Setup.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSIp6Setup.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSLimiter.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSLimiter.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSLlcSscsSetup.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSLlcSscsSetup.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSMBusClient.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSMBusClient.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSMBusMasterPortSetup.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSMBusMasterPortSetup.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSMBusSlavePortSetup.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSMBusSlavePortSetup.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSMacAddressSetup.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSMacAddressSetup.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSModemConfiguration.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSModemConfiguration.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSModemInitialisation.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSModemInitialisation.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSMonitoredValue.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSMonitoredValue.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSObject.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSObject.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSObjectCollection.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSObjectCollection.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSObjectDefinition.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSObjectDefinition.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSParameterMonitor.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSParameterMonitor.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSPppSetup.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSPppSetup.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSPppSetupIPCPOption.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSPppSetupIPCPOption.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSPppSetupLcpOption.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSPppSetupLcpOption.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSPrimeNbOfdmPlcApplicationsIdentification.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSPrimeNbOfdmPlcApplicationsIdentification.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSPrimeNbOfdmPlcMacCounters.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSPrimeNbOfdmPlcMacCounters.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSPrimeNbOfdmPlcMacFunctionalParameters.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSPrimeNbOfdmPlcMacFunctionalParameters.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSPrimeNbOfdmPlcMacNetworkAdministrationData.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSPrimeNbOfdmPlcMacNetworkAdministrationData.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSPrimeNbOfdmPlcMacSetup.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSPrimeNbOfdmPlcMacSetup.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSPrimeNbOfdmPlcPhysicalLayerCounters.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSPrimeNbOfdmPlcPhysicalLayerCounters.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSProfileGeneric.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSProfileGeneric.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSPushSetup.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSPushSetup.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSQualityOfService.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSQualityOfService.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSRegister.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSRegister.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSRegisterActivation.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSRegisterActivation.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSRegisterMonitor.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSRegisterMonitor.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSSapAssignment.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSSapAssignment.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSSchedule.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSSchedule.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSScheduleEntry.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSScheduleEntry.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSScript.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSScript.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSScriptAction.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSScriptAction.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSScriptTable.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSScriptTable.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSSeasonProfile.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSSeasonProfile.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSSecuritySetup.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSSecuritySetup.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSSpecialDay.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSSpecialDay.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSSpecialDaysTable.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSSpecialDaysTable.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSTarget.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSTarget.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSTcpUdpSetup.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSTcpUdpSetup.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSTokenGateway.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSTokenGateway.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSUtilityTables.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSUtilityTables.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXDLMSWeekProfile.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXDLMSWeekProfile.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXMacAvailableSwitch.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXMacAvailableSwitch.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXMacDirectTable.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXMacDirectTable.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXMacMulticastEntry.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXMacMulticastEntry.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXMacPhyCommunication.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXMacPhyCommunication.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXNeighborDiscoverySetup.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXNeighborDiscoverySetup.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXTokenGatewayConfiguration.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXTokenGatewayConfiguration.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXUnitCharge.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXUnitCharge.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXXmlReader.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXXmlReader.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXXmlWriter.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXXmlWriter.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXXmlWriterSettings.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXXmlWriterSettings.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/GXxDLMSContextType.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/GXxDLMSContextType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/IGXDLMSBase.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/IGXDLMSBase.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/__init__.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/AccountCreditStatus.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/AccountCreditStatus.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/AccountStatus.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/AccountStatus.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/AddressConfigMode.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/AddressConfigMode.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/AddressState.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/AddressState.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/ApplicationContextName.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/ApplicationContextName.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/AssociationStatus.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/AssociationStatus.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/AutoAnswerMode.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/AutoAnswerMode.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/AutoAnswerStatus.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/AutoAnswerStatus.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/AutoConnectMode.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/AutoConnectMode.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/BaudRate.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/BaudRate.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/CertificateEntity.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/CertificateEntity.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/CertificateIdentificationType.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/CertificateIdentificationType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/CertificateType.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/CertificateType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/ChargeConfiguration.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/ChargeConfiguration.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/ChargeType.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/ChargeType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/ClockBase.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/ClockBase.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/ControlMode.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/ControlMode.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/ControlState.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/ControlState.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/CreditCollectionConfiguration.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/CreditCollectionConfiguration.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/CreditConfiguration.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/CreditConfiguration.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/CreditStatus.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/CreditStatus.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/CreditType.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/CreditType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/Currency.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/Currency.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/GlobalKeyType.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/GlobalKeyType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/GsmCircuitSwitchStatus.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/GsmCircuitSwitchStatus.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/GsmPacketSwitchStatus.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/GsmPacketSwitchStatus.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/GsmStatus.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/GsmStatus.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/IecTwistedPairSetupMode.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/IecTwistedPairSetupMode.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/ImageTransferStatus.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/ImageTransferStatus.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/ImageTransferredBlocksStatus.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/ImageTransferredBlocksStatus.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/Ip4SetupIpOptionType.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/Ip4SetupIpOptionType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/KeyUsage.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/KeyUsage.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/LocalPortResponseTime.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/LocalPortResponseTime.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/MBusEncryptionKeyStatus.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/MBusEncryptionKeyStatus.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/MacState.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/MacState.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/MessageType.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/MessageType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/OpticalProtocolMode.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/OpticalProtocolMode.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/PaymentMode.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/PaymentMode.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/PppAuthenticationType.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/PppAuthenticationType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/PppSetupIPCPOptionType.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/PppSetupIPCPOptionType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/PppSetupLcpOptionType.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/PppSetupLcpOptionType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/ScriptActionType.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/ScriptActionType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/SecurityPolicy.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/SecurityPolicy.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/SecurityPolicy0.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/SecurityPolicy0.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/SecuritySuite.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/SecuritySuite.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/ServiceType.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/ServiceType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/SingleActionScheduleType.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/SingleActionScheduleType.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/SortMethod.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/SortMethod.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/TokenDelivery.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/TokenDelivery.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/TokenStatusCode.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/TokenStatusCode.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/Weekdays.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/Weekdays.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/objects/enums/__init__.py` & `gurux_dlms-1.0.99/gurux_dlms/objects/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/secure/GXDLMSSecureClient.py` & `gurux_dlms-1.0.99/gurux_dlms/secure/GXDLMSSecureClient.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/secure/GXDLMSSecureNotify.py` & `gurux_dlms-1.0.99/gurux_dlms/secure/GXDLMSSecureNotify.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/secure/GXDLMSSecureServer.py` & `gurux_dlms-1.0.99/gurux_dlms/secure/GXDLMSSecureServer.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms/secure/__init__.py` & `gurux_dlms-1.0.99/gurux_dlms/secure/__init__.py`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/gurux_dlms.egg-info/PKG-INFO` & `gurux_dlms-1.0.99/gurux_dlms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gurux-dlms
-Version: 1.0.98
+Version: 1.0.99
 Summary: Gurux DLMS library for Python.
 Home-page: https://github.com/gurux/gurux.dlms.python
 Author: Gurux Ltd
 Author-email: gurux@gurux.fi
 License: GPLv2
 Description: See An [Gurux](http://www.gurux.org/ "Gurux") for an overview.
```

### Comparing `gurux_dlms-1.0.98/gurux_dlms.egg-info/SOURCES.txt` & `gurux_dlms-1.0.99/gurux_dlms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gurux_dlms-1.0.98/setup.py` & `gurux_dlms-1.0.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gurux_dlms",
-    version="1.0.98",
+    version="1.0.99",
     author="Gurux Ltd",
     author_email="gurux@gurux.fi",
     description="Gurux DLMS library for Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gurux/gurux.dlms.python",
     packages=setuptools.find_packages(),
```

