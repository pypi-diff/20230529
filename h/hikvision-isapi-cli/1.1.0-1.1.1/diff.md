# Comparing `tmp/hikvision_isapi_cli-1.1.0.tar.gz` & `tmp/hikvision_isapi_cli-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikvision_isapi_cli-1.1.0.tar", max compression
+gzip compressed data, was "hikvision_isapi_cli-1.1.1.tar", max compression
```

## Comparing `hikvision_isapi_cli-1.1.0.tar` & `hikvision_isapi_cli-1.1.1.tar`

### file list

```diff
@@ -1,246 +1,246 @@
--rw-r--r--   0        0        0        0 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     4035 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/README.md
--rw-r--r--   0        0        0       24 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/docs/API.md
--rw-r--r--   0        0        0      102 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/__init__.py
--rw-r--r--   0        0        0       47 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/default/__init__.py
--rw-r--r--   0        0        0     3809 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/default/get_isapi_system_network_interfaces.py
--rw-r--r--   0        0        0    13745 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/default/put_isapi_system_device_info.py
--rw-r--r--   0        0        0     4919 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/default/put_isapi_system_two_way_audio_channels_channel_id_audio_data.py
--rw-r--r--   0        0        0     3682 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/default/session_heartbeat.py
--rw-r--r--   0        0        0     7421 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/default/session_login.py
--rw-r--r--   0        0        0     4608 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/default/session_login_capabilities.py
--rw-r--r--   0        0        0        0 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/__init__.py
--rw-r--r--   0        0        0     4318 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/callstatus.py
--rw-r--r--   0        0        0     4624 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/callstatus_capabilities_format_json.py
--rw-r--r--   0        0        0     4330 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/capabilities.py
--rw-r--r--   0        0        0     2296 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/capabilities1.py
--rw-r--r--   0        0        0     2285 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/capabilties.py
--rw-r--r--   0        0        0     4379 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/channels.py
--rw-r--r--   0        0        0     2271 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/channels2.py
--rw-r--r--   0        0        0     5421 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/channels_1_audiodata.py
--rw-r--r--   0        0        0     2578 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/channels_1_capabilities.py
--rw-r--r--   0        0        0     4105 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/channels_1_close.py
--rw-r--r--   0        0        0     4150 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/channels_1_open.py
--rw-r--r--   0        0        0     2553 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/channels_1_picture.py
--rw-r--r--   0        0        0     2902 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/devicecommunication_format_json.py
--rw-r--r--   0        0        0     2276 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/deviceid.py
--rw-r--r--   0        0        0     2341 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/deviceid_capabilities.py
--rw-r--r--   0        0        0     4226 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/deviceinfo.py
--rw-r--r--   0        0        0     5497 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/door.py
--rw-r--r--   0        0        0     4442 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/door_capabilities.py
--rw-r--r--   0        0        0     2853 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/encryption_format_json.py
--rw-r--r--   0        0        0     4018 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/get_isapi_streaming_channels.py
--rw-r--r--   0        0        0     2257 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/index1.py
--rw-r--r--   0        0        0     4422 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/inputs_channels.py
--rw-r--r--   0        0        0     2262 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/status.py
--rw-r--r--   0        0        0     3554 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/usercheck.py
--rw-r--r--   0        0        0     2506 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/userpermission1.py
--rw-r--r--   0        0        0     2256 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/users.py
--rw-r--r--   0        0        0     2438 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/client.py
--rw-r--r--   0        0        0      282 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/errors.py
--rw-r--r--   0        0        0    43634 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/__init__.py
--rw-r--r--   0        0        0     2319 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_call_status.py
--rw-r--r--   0        0        0     1578 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_call_status_call_status.py
--rw-r--r--   0        0        0     2477 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_json_cap_call_status.py
--rw-r--r--   0        0        0     2388 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_json_cap_call_status_call_status.py
--rw-r--r--   0        0        0     1749 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_json_cap_call_status_call_status_status.py
--rw-r--r--   0        0        0     4019 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_json_response_status.py
--rw-r--r--   0        0        0     6780 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control.py
--rw-r--r--   0        0        0   165585 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control.py
--rw-r--r--   0        0        0     5642 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info.py
--rw-r--r--   0        0        0     1763 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info_character_type.py
--rw-r--r--   0        0        0     1980 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info_employee_no.py
--rw-r--r--   0        0        0     1526 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info_is_support_compress.py
--rw-r--r--   0        0        0     3004 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_factory_reset.py
--rw-r--r--   0        0        0     1702 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_factory_reset_mode.py
--rw-r--r--   0        0        0     1416 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_cfg.py
--rw-r--r--   0        0        0     1426 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_event.py
--rw-r--r--   0        0        0     1472 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_event_total_num.py
--rw-r--r--   0        0        0     1454 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_work_status.py
--rw-r--r--   0        0        0     1449 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_anti_sneak_cfg.py
--rw-r--r--   0        0        0     1523 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_holiday_group.py
--rw-r--r--   0        0        0     1494 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_holiday_plan.py
--rw-r--r--   0        0        0     1456 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_rule.py
--rw-r--r--   0        0        0     1531 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_status_mode_cfg.py
--rw-r--r--   0        0        0     1531 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_status_rule_cfg.py
--rw-r--r--   0        0        0     1449 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_auth_code_info.py
--rw-r--r--   0        0        0     1464 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_card_info.py
--rw-r--r--   0        0        0     1441 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_face.py
--rw-r--r--   0        0        0     1479 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_finger_print.py
--rw-r--r--   0        0        0     1454 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_id_info.py
--rw-r--r--   0        0        0     1484 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_infrared_face.py
--rw-r--r--   0        0        0     1479 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_preset_param.py
--rw-r--r--   0        0        0     1441 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_rule.py
--rw-r--r--   0        0        0     1456 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_operations.py
--rw-r--r--   0        0        0     1529 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_reader_anti_sneak_cfg.py
--rw-r--r--   0        0        0     1454 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_reader_cfg.py
--rw-r--r--   0        0        0     1459 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_reader_plan.py
--rw-r--r--   0        0        0     1534 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_right_holiday_plan_cfg.py
--rw-r--r--   0        0        0     1519 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_right_week_plan_cfg.py
--rw-r--r--   0        0        0     1561 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_alarm_linkage.py
--rw-r--r--   0        0        0     1541 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_alarm_out.py
--rw-r--r--   0        0        0     1579 2023-05-18 21:29:55.671886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_alarm_out_control.py
--rw-r--r--   0        0        0     1489 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_cfg.py
--rw-r--r--   0        0        0     1536 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_type_cfg.py
--rw-r--r--   0        0        0     1459 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_anti_sneak.py
--rw-r--r--   0        0        0     1477 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_anti_sneak_cfg.py
--rw-r--r--   0        0        0     1464 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_card_record.py
--rw-r--r--   0        0        0     1539 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_event_card_linkage_cfg.py
--rw-r--r--   0        0        0     1454 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_group_cfg.py
--rw-r--r--   0        0        0     1454 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_plans_cfg.py
--rw-r--r--   0        0        0     1479 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_submarine_back.py
--rw-r--r--   0        0        0     1461 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_department_param.py
--rw-r--r--   0        0        0     1459 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_deploy_info_item.py
--rw-r--r--   0        0        0     1421 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_cfg.py
--rw-r--r--   0        0        0     1544 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_holiday_group_cfg.py
--rw-r--r--   0        0        0     1539 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_holiday_plan_cfg.py
--rw-r--r--   0        0        0     1459 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_plan.py
--rw-r--r--   0        0        0     1526 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_plan_template.py
--rw-r--r--   0        0        0     1524 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_week_plan_cfg.py
--rw-r--r--   0        0        0     1487 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_event_card_linkage_cfg.py
--rw-r--r--   0        0        0     1467 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_event_card_no_list.py
--rw-r--r--   0        0        0     1489 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_event_optimization_cfg.py
--rw-r--r--   0        0        0     1474 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_face_recognize_mode.py
--rw-r--r--   0        0        0     1459 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_finger_print_cfg.py
--rw-r--r--   0        0        0     1474 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_finger_print_delete.py
--rw-r--r--   0        0        0     1467 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_dial_and_info.py
--rw-r--r--   0        0        0     1449 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_ir_status.py
--rw-r--r--   0        0        0     1526 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_related_parts_status.py
--rw-r--r--   0        0        0     1436 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_status.py
--rw-r--r--   0        0        0     1426 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_group_cfg.py
--rw-r--r--   0        0        0     1466 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_identity_terminal.py
--rw-r--r--   0        0        0     1479 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_ladder_control_relay.py
--rw-r--r--   0        0        0     1439 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_log_mode_cfg.py
--rw-r--r--   0        0        0     1472 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_m1_card_encrypt_cfg.py
--rw-r--r--   0        0        0     1446 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_module_status.py
--rw-r--r--   0        0        0     1449 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_multi_card_cfg.py
--rw-r--r--   0        0        0     1524 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_multi_door_inter_lock_cfg.py
--rw-r--r--   0        0        0     1456 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_offline_capture.py
--rw-r--r--   0        0        0     1451 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_ordinary_class.py
--rw-r--r--   0        0        0     1436 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_osdp_modify.py
--rw-r--r--   0        0        0     1436 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_osdp_status.py
--rw-r--r--   0        0        0     1477 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_phone_door_right_cfg.py
--rw-r--r--   0        0        0     1469 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_reader_across_host.py
--rw-r--r--   0        0        0     1484 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_buzzer.py
--rw-r--r--   0        0        0     1474 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_door.py
--rw-r--r--   0        0        0     1482 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_pw_cfg.py
--rw-r--r--   0        0        0     1492 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_pw_chcek.py
--rw-r--r--   0        0        0     1489 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_right_controller_audio.py
--rw-r--r--   0        0        0     1446 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_schedule_plan.py
--rw-r--r--   0        0        0     1446 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_server_device.py
--rw-r--r--   0        0        0     1469 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_sms_relative_param.py
--rw-r--r--   0        0        0     1436 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_snap_config.py
--rw-r--r--   0        0        0     1464 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_start_reader_info.py
--rw-r--r--   0        0        0     1451 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back.py
--rw-r--r--   0        0        0     1521 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back_host_info.py
--rw-r--r--   0        0        0     1474 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back_mode.py
--rw-r--r--   0        0        0     1484 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back_reader.py
--rw-r--r--   0        0        0     1431 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_usb_manage.py
--rw-r--r--   0        0        0     1539 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_user_right_holiday_group_cfg.py
--rw-r--r--   0        0        0     1521 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_user_right_plan_template.py
--rw-r--r--   0        0        0     1521 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_holiday_group_cfg.py
--rw-r--r--   0        0        0     1492 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_holiday_plan_cfg.py
--rw-r--r--   0        0        0     1479 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_plan_template.py
--rw-r--r--   0        0        0     1477 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_week_plan_cfg.py
--rw-r--r--   0        0        0     1436 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_wiegand_cfg.py
--rw-r--r--   0        0        0     1459 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_wiegand_rule_cfg.py
--rw-r--r--   0        0        0     1446 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_working_class.py
--rw-r--r--   0        0        0     5455 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_local_controller.py
--rw-r--r--   0        0        0     1604 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_local_controller_is_support_local_controller_control.py
--rw-r--r--   0        0        0     1599 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_local_controller_is_support_local_controller_manage.py
--rw-r--r--   0        0        0     3009 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door.py
--rw-r--r--   0        0        0     5227 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door.py
--rw-r--r--   0        0        0     1677 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door_cmd.py
--rw-r--r--   0        0        0     1927 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door_door_no.py
--rw-r--r--   0        0        0     1934 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door_password.py
--rw-r--r--   0        0        0     4548 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info.py
--rw-r--r--   0        0        0    31772 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info.py
--rw-r--r--   0        0        0    12689 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status.py
--rw-r--r--   0        0        0     1466 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_ethernet_broken.py
--rw-r--r--   0        0        0     1464 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_hard_disk_error.py
--rw-r--r--   0        0        0     1459 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_hard_disk_full.py
--rw-r--r--   0        0        0     1461 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_illegal_access.py
--rw-r--r--   0        0        0     1466 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_ipaddr_conflict.py
--rw-r--r--   0        0        0     1492 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_raid_logic_disk_error.py
--rw-r--r--   0        0        0     1451 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_record_error.py
--rw-r--r--   0        0        0     1526 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_spare_work_device_error.py
--rw-r--r--   0        0        0     3040 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_dock_station.py
--rw-r--r--   0        0        0     2645 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_dock_station_platform.py
--rw-r--r--   0        0        0     1695 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_is_reset_device_language.py
--rw-r--r--   0        0        0     1848 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_r3_version.py
--rw-r--r--   0        0        0     1848 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_rx_version.py
--rw-r--r--   0        0        0     1706 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_uid_lamp_recognition.py
--rw-r--r--   0        0        0     1871 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_zig_bee_version.py
--rw-r--r--   0        0        0     3132 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_network_interface.py
--rw-r--r--   0        0        0     2953 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_network_interface_list.py
--rw-r--r--   0        0        0     3208 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_network_interface_list_network_interface_list.py
--rw-r--r--   0        0        0     7425 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface.py
--rw-r--r--   0        0        0     4767 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_active_multicast.py
--rw-r--r--   0        0        0     1961 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_active_multicast_port.py
--rw-r--r--   0        0        0     1752 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_active_multicast_stream_id.py
--rw-r--r--   0        0        0     3140 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_ethernet_port_list.py
--rw-r--r--   0        0        0     2544 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_ethernet_port_list_ethernet_port.py
--rw-r--r--   0        0        0     1913 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_mac_address.py
--rw-r--r--   0        0        0     2803 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_remote_control_door.py
--rw-r--r--   0        0        0     2400 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_remote_control_door_remote_control_door.py
--rw-r--r--   0        0        0     2690 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_response_status.py
--rw-r--r--   0        0        0     2997 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_response_status_authentication_failed.py
--rw-r--r--   0        0        0     4161 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_response_status_authentication_failed_response_status.py
--rw-r--r--   0        0        0     3141 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_response_status_response_status.py
--rw-r--r--   0        0        0     2719 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_session_login.py
--rw-r--r--   0        0        0     2958 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_session_login_cap.py
--rw-r--r--   0        0        0     3693 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_session_login_cap_session_login_cap.py
--rw-r--r--   0        0        0     2746 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_session_login_response.py
--rw-r--r--   0        0        0     3581 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_session_login_response_session_login.py
--rw-r--r--   0        0        0     3971 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_session_login_session_login.py
--rw-r--r--   0        0        0     5608 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel.py
--rw-r--r--   0        0        0     2441 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_audio.py
--rw-r--r--   0        0        0     2953 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_list.py
--rw-r--r--   0        0        0     3208 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_list_streaming_channel_list.py
--rw-r--r--   0        0        0     3830 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_transport.py
--rw-r--r--   0        0        0     3189 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_transport_control_protocol_list.py
--rw-r--r--   0        0        0     1991 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_transport_control_protocol_list_control_protocol_item.py
--rw-r--r--   0        0        0     1672 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_transport_security.py
--rw-r--r--   0        0        0     6719 2023-05-18 21:29:55.675886 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_video.py
--rw-r--r--   0        0        0     3211 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel.py
--rw-r--r--   0        0        0     3083 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_list.py
--rw-r--r--   0        0        0     3354 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_list_two_way_audio_channel_list.py
--rw-r--r--   0        0        0    18177 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel.py
--rw-r--r--   0        0        0     4669 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs.py
--rw-r--r--   0        0        0     1544 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs_enabled.py
--rw-r--r--   0        0        0     3644 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs_video_input_channel_list.py
--rw-r--r--   0        0        0     1765 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs_video_input_channel_list_video_input_channel_id.py
--rw-r--r--   0        0        0     1442 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_bit_rate.py
--rw-r--r--   0        0        0     1482 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_compression_type.py
--rw-r--r--   0        0        0     1544 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_inbound_compression_type.py
--rw-r--r--   0        0        0     1452 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_input_type.py
--rw-r--r--   0        0        0     1411 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_enabled.py
--rw-r--r--   0        0        0     1386 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_id.py
--rw-r--r--   0        0        0     1462 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_line_out_forbidden.py
--rw-r--r--   0        0        0     1452 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_mic_in_forbidden.py
--rw-r--r--   0        0        0     1459 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_microphone_volume.py
--rw-r--r--   0        0        0     1431 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_noisereduce.py
--rw-r--r--   0        0        0     1444 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_speaker_volume.py
--rw-r--r--   0        0        0     2845 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_session.py
--rw-r--r--   0        0        0     2224 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_session_two_way_audio_session.py
--rw-r--r--   0        0        0     2558 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_user_check.py
--rw-r--r--   0        0        0     4455 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_user_check_user_check.py
--rw-r--r--   0        0        0     2890 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel.py
--rw-r--r--   0        0        0     3020 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_list.py
--rw-r--r--   0        0        0     3281 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_list_video_input_channel_list.py
--rw-r--r--   0        0        0     9938 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel.py
--rw-r--r--   0        0        0     1370 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_id.py
--rw-r--r--   0        0        0     1408 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_input_port.py
--rw-r--r--   0        0        0     1380 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_name.py
--rw-r--r--   0        0        0     1403 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_port_type.py
--rw-r--r--   0        0        0     1398 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_res_desc.py
--rw-r--r--   0        0        0     1418 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_video_format.py
--rw-r--r--   0        0        0     1451 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_video_input_enabled.py
--rw-r--r--   0        0        0       25 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/py.typed
--rw-r--r--   0        0        0      974 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/types.py
--rw-r--r--   0        0        0      154 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_sk/__init__.py
--rw-r--r--   0        0        0     3810 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_sk/session.py
--rw-r--r--   0        0        0     1309 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/hikvision_isapi_sk/snap.py
--rw-r--r--   0        0        0     1139 2023-05-18 21:29:55.679885 hikvision_isapi_cli-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4978 1970-01-01 00:00:00.000000 hikvision_isapi_cli-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     4035 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/README.md
+-rw-r--r--   0        0        0       24 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/docs/API.md
+-rw-r--r--   0        0        0      102 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/default/__init__.py
+-rw-r--r--   0        0        0     3809 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/default/get_isapi_system_network_interfaces.py
+-rw-r--r--   0        0        0    13745 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/default/put_isapi_system_device_info.py
+-rw-r--r--   0        0        0     4919 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/default/put_isapi_system_two_way_audio_channels_channel_id_audio_data.py
+-rw-r--r--   0        0        0     3682 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/default/session_heartbeat.py
+-rw-r--r--   0        0        0     7421 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/default/session_login.py
+-rw-r--r--   0        0        0     4608 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/default/session_login_capabilities.py
+-rw-r--r--   0        0        0        0 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/__init__.py
+-rw-r--r--   0        0        0     4318 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/callstatus.py
+-rw-r--r--   0        0        0     4624 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/callstatus_capabilities_format_json.py
+-rw-r--r--   0        0        0     4330 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/capabilities.py
+-rw-r--r--   0        0        0     2296 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/capabilities1.py
+-rw-r--r--   0        0        0     2285 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/capabilties.py
+-rw-r--r--   0        0        0     4379 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/channels.py
+-rw-r--r--   0        0        0     2271 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/channels2.py
+-rw-r--r--   0        0        0     5421 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/channels_1_audiodata.py
+-rw-r--r--   0        0        0     2578 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/channels_1_capabilities.py
+-rw-r--r--   0        0        0     4105 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/channels_1_close.py
+-rw-r--r--   0        0        0     4150 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/channels_1_open.py
+-rw-r--r--   0        0        0     2553 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/channels_1_picture.py
+-rw-r--r--   0        0        0     2902 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/devicecommunication_format_json.py
+-rw-r--r--   0        0        0     2276 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/deviceid.py
+-rw-r--r--   0        0        0     2341 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/deviceid_capabilities.py
+-rw-r--r--   0        0        0     4226 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/deviceinfo.py
+-rw-r--r--   0        0        0     5497 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/door.py
+-rw-r--r--   0        0        0     4442 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/door_capabilities.py
+-rw-r--r--   0        0        0     2853 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/encryption_format_json.py
+-rw-r--r--   0        0        0     4018 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/get_isapi_streaming_channels.py
+-rw-r--r--   0        0        0     2257 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/index1.py
+-rw-r--r--   0        0        0     4422 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/inputs_channels.py
+-rw-r--r--   0        0        0     2262 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/status.py
+-rw-r--r--   0        0        0     3554 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/usercheck.py
+-rw-r--r--   0        0        0     2506 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/userpermission1.py
+-rw-r--r--   0        0        0     2256 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/users.py
+-rw-r--r--   0        0        0     2438 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/client.py
+-rw-r--r--   0        0        0      282 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/errors.py
+-rw-r--r--   0        0        0    43634 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/__init__.py
+-rw-r--r--   0        0        0     2319 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_call_status.py
+-rw-r--r--   0        0        0     1578 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_call_status_call_status.py
+-rw-r--r--   0        0        0     2477 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_json_cap_call_status.py
+-rw-r--r--   0        0        0     2388 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_json_cap_call_status_call_status.py
+-rw-r--r--   0        0        0     1749 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_json_cap_call_status_call_status_status.py
+-rw-r--r--   0        0        0     4019 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_json_response_status.py
+-rw-r--r--   0        0        0     6780 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control.py
+-rw-r--r--   0        0        0   165585 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control.py
+-rw-r--r--   0        0        0     5642 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info.py
+-rw-r--r--   0        0        0     1763 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info_character_type.py
+-rw-r--r--   0        0        0     1980 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info_employee_no.py
+-rw-r--r--   0        0        0     1526 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info_is_support_compress.py
+-rw-r--r--   0        0        0     3004 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_factory_reset.py
+-rw-r--r--   0        0        0     1702 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_factory_reset_mode.py
+-rw-r--r--   0        0        0     1416 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_cfg.py
+-rw-r--r--   0        0        0     1426 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_event.py
+-rw-r--r--   0        0        0     1472 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_event_total_num.py
+-rw-r--r--   0        0        0     1454 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_work_status.py
+-rw-r--r--   0        0        0     1449 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_anti_sneak_cfg.py
+-rw-r--r--   0        0        0     1523 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_holiday_group.py
+-rw-r--r--   0        0        0     1494 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_holiday_plan.py
+-rw-r--r--   0        0        0     1456 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_rule.py
+-rw-r--r--   0        0        0     1531 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_status_mode_cfg.py
+-rw-r--r--   0        0        0     1531 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_status_rule_cfg.py
+-rw-r--r--   0        0        0     1449 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_auth_code_info.py
+-rw-r--r--   0        0        0     1464 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_card_info.py
+-rw-r--r--   0        0        0     1441 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_face.py
+-rw-r--r--   0        0        0     1479 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_finger_print.py
+-rw-r--r--   0        0        0     1454 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_id_info.py
+-rw-r--r--   0        0        0     1484 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_infrared_face.py
+-rw-r--r--   0        0        0     1479 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_preset_param.py
+-rw-r--r--   0        0        0     1441 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_rule.py
+-rw-r--r--   0        0        0     1456 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_operations.py
+-rw-r--r--   0        0        0     1529 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_reader_anti_sneak_cfg.py
+-rw-r--r--   0        0        0     1454 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_reader_cfg.py
+-rw-r--r--   0        0        0     1459 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_reader_plan.py
+-rw-r--r--   0        0        0     1534 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_right_holiday_plan_cfg.py
+-rw-r--r--   0        0        0     1519 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_right_week_plan_cfg.py
+-rw-r--r--   0        0        0     1561 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_alarm_linkage.py
+-rw-r--r--   0        0        0     1541 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_alarm_out.py
+-rw-r--r--   0        0        0     1579 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_alarm_out_control.py
+-rw-r--r--   0        0        0     1489 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_cfg.py
+-rw-r--r--   0        0        0     1536 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_type_cfg.py
+-rw-r--r--   0        0        0     1459 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_anti_sneak.py
+-rw-r--r--   0        0        0     1477 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_anti_sneak_cfg.py
+-rw-r--r--   0        0        0     1464 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_card_record.py
+-rw-r--r--   0        0        0     1539 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_event_card_linkage_cfg.py
+-rw-r--r--   0        0        0     1454 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_group_cfg.py
+-rw-r--r--   0        0        0     1454 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_plans_cfg.py
+-rw-r--r--   0        0        0     1479 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_submarine_back.py
+-rw-r--r--   0        0        0     1461 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_department_param.py
+-rw-r--r--   0        0        0     1459 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_deploy_info_item.py
+-rw-r--r--   0        0        0     1421 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_cfg.py
+-rw-r--r--   0        0        0     1544 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_holiday_group_cfg.py
+-rw-r--r--   0        0        0     1539 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_holiday_plan_cfg.py
+-rw-r--r--   0        0        0     1459 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_plan.py
+-rw-r--r--   0        0        0     1526 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_plan_template.py
+-rw-r--r--   0        0        0     1524 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_week_plan_cfg.py
+-rw-r--r--   0        0        0     1487 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_event_card_linkage_cfg.py
+-rw-r--r--   0        0        0     1467 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_event_card_no_list.py
+-rw-r--r--   0        0        0     1489 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_event_optimization_cfg.py
+-rw-r--r--   0        0        0     1474 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_face_recognize_mode.py
+-rw-r--r--   0        0        0     1459 2023-05-29 20:36:25.903931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_finger_print_cfg.py
+-rw-r--r--   0        0        0     1474 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_finger_print_delete.py
+-rw-r--r--   0        0        0     1467 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_dial_and_info.py
+-rw-r--r--   0        0        0     1449 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_ir_status.py
+-rw-r--r--   0        0        0     1526 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_related_parts_status.py
+-rw-r--r--   0        0        0     1436 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_status.py
+-rw-r--r--   0        0        0     1426 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_group_cfg.py
+-rw-r--r--   0        0        0     1466 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_identity_terminal.py
+-rw-r--r--   0        0        0     1479 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_ladder_control_relay.py
+-rw-r--r--   0        0        0     1439 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_log_mode_cfg.py
+-rw-r--r--   0        0        0     1472 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_m1_card_encrypt_cfg.py
+-rw-r--r--   0        0        0     1446 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_module_status.py
+-rw-r--r--   0        0        0     1449 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_multi_card_cfg.py
+-rw-r--r--   0        0        0     1524 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_multi_door_inter_lock_cfg.py
+-rw-r--r--   0        0        0     1456 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_offline_capture.py
+-rw-r--r--   0        0        0     1451 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_ordinary_class.py
+-rw-r--r--   0        0        0     1436 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_osdp_modify.py
+-rw-r--r--   0        0        0     1436 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_osdp_status.py
+-rw-r--r--   0        0        0     1477 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_phone_door_right_cfg.py
+-rw-r--r--   0        0        0     1469 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_reader_across_host.py
+-rw-r--r--   0        0        0     1484 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_buzzer.py
+-rw-r--r--   0        0        0     1474 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_door.py
+-rw-r--r--   0        0        0     1482 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_pw_cfg.py
+-rw-r--r--   0        0        0     1492 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_pw_chcek.py
+-rw-r--r--   0        0        0     1489 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_right_controller_audio.py
+-rw-r--r--   0        0        0     1446 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_schedule_plan.py
+-rw-r--r--   0        0        0     1446 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_server_device.py
+-rw-r--r--   0        0        0     1469 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_sms_relative_param.py
+-rw-r--r--   0        0        0     1436 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_snap_config.py
+-rw-r--r--   0        0        0     1464 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_start_reader_info.py
+-rw-r--r--   0        0        0     1451 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back.py
+-rw-r--r--   0        0        0     1521 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back_host_info.py
+-rw-r--r--   0        0        0     1474 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back_mode.py
+-rw-r--r--   0        0        0     1484 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back_reader.py
+-rw-r--r--   0        0        0     1431 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_usb_manage.py
+-rw-r--r--   0        0        0     1539 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_user_right_holiday_group_cfg.py
+-rw-r--r--   0        0        0     1521 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_user_right_plan_template.py
+-rw-r--r--   0        0        0     1521 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_holiday_group_cfg.py
+-rw-r--r--   0        0        0     1492 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_holiday_plan_cfg.py
+-rw-r--r--   0        0        0     1479 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_plan_template.py
+-rw-r--r--   0        0        0     1477 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_week_plan_cfg.py
+-rw-r--r--   0        0        0     1436 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_wiegand_cfg.py
+-rw-r--r--   0        0        0     1459 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_wiegand_rule_cfg.py
+-rw-r--r--   0        0        0     1446 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_working_class.py
+-rw-r--r--   0        0        0     5455 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_local_controller.py
+-rw-r--r--   0        0        0     1604 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_local_controller_is_support_local_controller_control.py
+-rw-r--r--   0        0        0     1599 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_local_controller_is_support_local_controller_manage.py
+-rw-r--r--   0        0        0     3009 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door.py
+-rw-r--r--   0        0        0     5227 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door.py
+-rw-r--r--   0        0        0     1677 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door_cmd.py
+-rw-r--r--   0        0        0     1927 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door_door_no.py
+-rw-r--r--   0        0        0     1934 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door_password.py
+-rw-r--r--   0        0        0     4548 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info.py
+-rw-r--r--   0        0        0    31772 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info.py
+-rw-r--r--   0        0        0    12689 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status.py
+-rw-r--r--   0        0        0     1466 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_ethernet_broken.py
+-rw-r--r--   0        0        0     1464 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_hard_disk_error.py
+-rw-r--r--   0        0        0     1459 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_hard_disk_full.py
+-rw-r--r--   0        0        0     1461 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_illegal_access.py
+-rw-r--r--   0        0        0     1466 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_ipaddr_conflict.py
+-rw-r--r--   0        0        0     1492 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_raid_logic_disk_error.py
+-rw-r--r--   0        0        0     1451 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_record_error.py
+-rw-r--r--   0        0        0     1526 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_spare_work_device_error.py
+-rw-r--r--   0        0        0     3040 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_dock_station.py
+-rw-r--r--   0        0        0     2645 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_dock_station_platform.py
+-rw-r--r--   0        0        0     1695 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_is_reset_device_language.py
+-rw-r--r--   0        0        0     1848 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_r3_version.py
+-rw-r--r--   0        0        0     1848 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_rx_version.py
+-rw-r--r--   0        0        0     1706 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_uid_lamp_recognition.py
+-rw-r--r--   0        0        0     1871 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_zig_bee_version.py
+-rw-r--r--   0        0        0     3132 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_network_interface.py
+-rw-r--r--   0        0        0     2953 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_network_interface_list.py
+-rw-r--r--   0        0        0     3208 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_network_interface_list_network_interface_list.py
+-rw-r--r--   0        0        0     7425 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface.py
+-rw-r--r--   0        0        0     4767 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_active_multicast.py
+-rw-r--r--   0        0        0     1961 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_active_multicast_port.py
+-rw-r--r--   0        0        0     1752 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_active_multicast_stream_id.py
+-rw-r--r--   0        0        0     3140 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_ethernet_port_list.py
+-rw-r--r--   0        0        0     2544 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_ethernet_port_list_ethernet_port.py
+-rw-r--r--   0        0        0     1913 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_mac_address.py
+-rw-r--r--   0        0        0     2803 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_remote_control_door.py
+-rw-r--r--   0        0        0     2400 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_remote_control_door_remote_control_door.py
+-rw-r--r--   0        0        0     2690 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_response_status.py
+-rw-r--r--   0        0        0     2997 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_response_status_authentication_failed.py
+-rw-r--r--   0        0        0     4161 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_response_status_authentication_failed_response_status.py
+-rw-r--r--   0        0        0     3141 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_response_status_response_status.py
+-rw-r--r--   0        0        0     2719 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_session_login.py
+-rw-r--r--   0        0        0     2958 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_session_login_cap.py
+-rw-r--r--   0        0        0     3693 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_session_login_cap_session_login_cap.py
+-rw-r--r--   0        0        0     2746 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_session_login_response.py
+-rw-r--r--   0        0        0     3581 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_session_login_response_session_login.py
+-rw-r--r--   0        0        0     3971 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_session_login_session_login.py
+-rw-r--r--   0        0        0     5608 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel.py
+-rw-r--r--   0        0        0     2441 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_audio.py
+-rw-r--r--   0        0        0     2953 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_list.py
+-rw-r--r--   0        0        0     3208 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_list_streaming_channel_list.py
+-rw-r--r--   0        0        0     3830 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_transport.py
+-rw-r--r--   0        0        0     3189 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_transport_control_protocol_list.py
+-rw-r--r--   0        0        0     1991 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_transport_control_protocol_list_control_protocol_item.py
+-rw-r--r--   0        0        0     1672 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_transport_security.py
+-rw-r--r--   0        0        0     6719 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_video.py
+-rw-r--r--   0        0        0     3211 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel.py
+-rw-r--r--   0        0        0     3083 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_list.py
+-rw-r--r--   0        0        0     3354 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_list_two_way_audio_channel_list.py
+-rw-r--r--   0        0        0    18177 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel.py
+-rw-r--r--   0        0        0     4669 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs.py
+-rw-r--r--   0        0        0     1544 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs_enabled.py
+-rw-r--r--   0        0        0     3644 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs_video_input_channel_list.py
+-rw-r--r--   0        0        0     1765 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs_video_input_channel_list_video_input_channel_id.py
+-rw-r--r--   0        0        0     1442 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_bit_rate.py
+-rw-r--r--   0        0        0     1482 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_compression_type.py
+-rw-r--r--   0        0        0     1544 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_inbound_compression_type.py
+-rw-r--r--   0        0        0     1452 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_input_type.py
+-rw-r--r--   0        0        0     1411 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_enabled.py
+-rw-r--r--   0        0        0     1386 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_id.py
+-rw-r--r--   0        0        0     1462 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_line_out_forbidden.py
+-rw-r--r--   0        0        0     1452 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_mic_in_forbidden.py
+-rw-r--r--   0        0        0     1459 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_microphone_volume.py
+-rw-r--r--   0        0        0     1431 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_noisereduce.py
+-rw-r--r--   0        0        0     1444 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_speaker_volume.py
+-rw-r--r--   0        0        0     2845 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_session.py
+-rw-r--r--   0        0        0     2224 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_session_two_way_audio_session.py
+-rw-r--r--   0        0        0     2558 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_user_check.py
+-rw-r--r--   0        0        0     4455 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_user_check_user_check.py
+-rw-r--r--   0        0        0     2890 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel.py
+-rw-r--r--   0        0        0     3020 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_list.py
+-rw-r--r--   0        0        0     3281 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_list_video_input_channel_list.py
+-rw-r--r--   0        0        0     9938 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel.py
+-rw-r--r--   0        0        0     1370 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_id.py
+-rw-r--r--   0        0        0     1408 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_input_port.py
+-rw-r--r--   0        0        0     1380 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_name.py
+-rw-r--r--   0        0        0     1403 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_port_type.py
+-rw-r--r--   0        0        0     1398 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_res_desc.py
+-rw-r--r--   0        0        0     1418 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_video_format.py
+-rw-r--r--   0        0        0     1451 2023-05-29 20:36:25.907931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_video_input_enabled.py
+-rw-r--r--   0        0        0       25 2023-05-29 20:36:25.911931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/py.typed
+-rw-r--r--   0        0        0      974 2023-05-29 20:36:25.911931 hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/types.py
+-rw-r--r--   0        0        0      154 2023-05-29 20:36:25.911931 hikvision_isapi_cli-1.1.1/hikvision_isapi_sk/__init__.py
+-rw-r--r--   0        0        0     3810 2023-05-29 20:36:25.911931 hikvision_isapi_cli-1.1.1/hikvision_isapi_sk/session.py
+-rw-r--r--   0        0        0     1309 2023-05-29 20:36:25.911931 hikvision_isapi_cli-1.1.1/hikvision_isapi_sk/snap.py
+-rw-r--r--   0        0        0     1138 2023-05-29 20:36:25.911931 hikvision_isapi_cli-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4978 1970-01-01 00:00:00.000000 hikvision_isapi_cli-1.1.1/PKG-INFO
```

### Comparing `hikvision_isapi_cli-1.1.0/README.md` & `hikvision_isapi_cli-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/default/get_isapi_system_network_interfaces.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/default/get_isapi_system_network_interfaces.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/default/put_isapi_system_device_info.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/default/put_isapi_system_device_info.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/default/put_isapi_system_two_way_audio_channels_channel_id_audio_data.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/default/put_isapi_system_two_way_audio_channels_channel_id_audio_data.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/default/session_heartbeat.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/default/session_heartbeat.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/default/session_login.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/default/session_login.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/default/session_login_capabilities.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/default/session_login_capabilities.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/callstatus.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/callstatus.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/callstatus_capabilities_format_json.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/callstatus_capabilities_format_json.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/capabilities.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/capabilities.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/capabilities1.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/capabilities1.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/capabilties.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/capabilties.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/channels.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/channels.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/channels2.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/channels2.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/channels_1_audiodata.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/channels_1_audiodata.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/channels_1_capabilities.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/channels_1_capabilities.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/channels_1_close.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/channels_1_close.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/channels_1_open.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/channels_1_open.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/channels_1_picture.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/channels_1_picture.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/devicecommunication_format_json.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/devicecommunication_format_json.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/deviceid.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/deviceid.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/deviceid_capabilities.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/deviceid_capabilities.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/deviceinfo.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/deviceinfo.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/door.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/door.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/door_capabilities.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/door_capabilities.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/encryption_format_json.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/encryption_format_json.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/get_isapi_streaming_channels.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/get_isapi_streaming_channels.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/index1.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/index1.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/inputs_channels.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/inputs_channels.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/status.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/usercheck.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/usercheck.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/userpermission1.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/userpermission1.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/api/isapi/users.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/api/isapi/users.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/client.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/client.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/__init__.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_call_status.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_call_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_call_status_call_status.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_call_status_call_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_json_cap_call_status.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_json_cap_call_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_json_cap_call_status_call_status.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_json_cap_call_status_call_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_json_cap_call_status_call_status_status.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_json_cap_call_status_call_status_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_json_response_status.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_json_response_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info_character_type.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info_character_type.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info_employee_no.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info_employee_no.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info_is_support_compress.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_employee_no_info_is_support_compress.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_factory_reset.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_factory_reset.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_factory_reset_mode.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_factory_reset_mode.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_event.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_event.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_event_total_num.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_event_total_num.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_work_status.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_acs_work_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_anti_sneak_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_anti_sneak_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_holiday_group.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_holiday_group.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_holiday_plan.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_holiday_plan.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_rule.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_rule.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_status_mode_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_status_mode_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_status_rule_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_attendance_status_rule_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_auth_code_info.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_auth_code_info.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_card_info.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_card_info.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_face.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_face.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_finger_print.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_finger_print.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_id_info.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_id_info.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_infrared_face.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_infrared_face.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_preset_param.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_preset_param.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_rule.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_capture_rule.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_operations.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_operations.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_reader_anti_sneak_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_reader_anti_sneak_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_reader_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_reader_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_reader_plan.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_reader_plan.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_right_holiday_plan_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_right_holiday_plan_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_right_week_plan_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_card_right_week_plan_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_alarm_linkage.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_alarm_linkage.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_alarm_out.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_alarm_out.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_alarm_out_control.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_alarm_out_control.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_type_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_channel_controller_type_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_anti_sneak.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_anti_sneak.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_anti_sneak_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_anti_sneak_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_card_record.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_card_record.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_event_card_linkage_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_event_card_linkage_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_group_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_group_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_plans_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_plans_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_submarine_back.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_clear_submarine_back.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_department_param.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_department_param.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_deploy_info_item.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_deploy_info_item.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_holiday_group_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_holiday_group_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_holiday_plan_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_holiday_plan_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_plan.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_plan.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_plan_template.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_plan_template.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_week_plan_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_door_status_week_plan_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_event_card_linkage_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_event_card_linkage_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_event_card_no_list.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_event_card_no_list.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_event_optimization_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_event_optimization_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_face_recognize_mode.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_face_recognize_mode.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_finger_print_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_finger_print_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_finger_print_delete.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_finger_print_delete.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_dial_and_info.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_dial_and_info.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_ir_status.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_ir_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_related_parts_status.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_related_parts_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_status.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_gate_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_group_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_group_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_identity_terminal.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_identity_terminal.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_ladder_control_relay.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_ladder_control_relay.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_log_mode_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_log_mode_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_m1_card_encrypt_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_m1_card_encrypt_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_module_status.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_module_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_multi_card_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_multi_card_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_multi_door_inter_lock_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_multi_door_inter_lock_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_offline_capture.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_offline_capture.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_ordinary_class.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_ordinary_class.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_osdp_modify.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_osdp_modify.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_osdp_status.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_osdp_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_phone_door_right_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_phone_door_right_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_reader_across_host.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_reader_across_host.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_buzzer.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_buzzer.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_door.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_door.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_pw_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_pw_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_pw_chcek.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_remote_control_pw_chcek.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_right_controller_audio.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_right_controller_audio.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_schedule_plan.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_schedule_plan.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_server_device.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_server_device.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_sms_relative_param.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_sms_relative_param.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_snap_config.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_snap_config.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_start_reader_info.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_start_reader_info.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back_host_info.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back_host_info.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back_mode.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back_mode.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back_reader.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_submarine_back_reader.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_usb_manage.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_usb_manage.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_user_right_holiday_group_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_user_right_holiday_group_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_user_right_plan_template.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_user_right_plan_template.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_holiday_group_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_holiday_group_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_holiday_plan_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_holiday_plan_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_plan_template.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_plan_template.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_week_plan_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_verify_week_plan_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_wiegand_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_wiegand_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_wiegand_rule_cfg.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_wiegand_rule_cfg.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_working_class.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_is_support_working_class.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_local_controller.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_local_controller.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_local_controller_is_support_local_controller_control.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_local_controller_is_support_local_controller_control.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_local_controller_is_support_local_controller_manage.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_access_control_access_control_local_controller_is_support_local_controller_manage.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door_cmd.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door_cmd.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door_door_no.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door_door_no.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door_password.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_cap_remote_control_door_remote_control_door_password.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_ethernet_broken.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_ethernet_broken.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_hard_disk_error.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_hard_disk_error.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_hard_disk_full.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_hard_disk_full.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_illegal_access.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_illegal_access.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_ipaddr_conflict.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_ipaddr_conflict.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_raid_logic_disk_error.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_raid_logic_disk_error.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_record_error.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_record_error.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_spare_work_device_error.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_detail_abnormal_status_spare_work_device_error.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_dock_station.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_dock_station.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_dock_station_platform.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_dock_station_platform.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_is_reset_device_language.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_is_reset_device_language.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_r3_version.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_r3_version.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_rx_version.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_rx_version.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_uid_lamp_recognition.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_uid_lamp_recognition.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_zig_bee_version.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_device_info_device_info_zig_bee_version.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_network_interface.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_network_interface.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_network_interface_list.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_network_interface_list.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_network_interface_list_network_interface_list.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_network_interface_list_network_interface_list.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_active_multicast.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_active_multicast.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_active_multicast_port.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_active_multicast_port.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_active_multicast_stream_id.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_active_multicast_stream_id.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_ethernet_port_list.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_ethernet_port_list.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_ethernet_port_list_ethernet_port.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_ethernet_port_list_ethernet_port.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_mac_address.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_network_interface_network_interface_mac_address.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_remote_control_door.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_remote_control_door.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_remote_control_door_remote_control_door.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_remote_control_door_remote_control_door.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_response_status.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_response_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_response_status_authentication_failed.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_response_status_authentication_failed.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_response_status_authentication_failed_response_status.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_response_status_authentication_failed_response_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_response_status_response_status.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_response_status_response_status.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_session_login.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_session_login.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_session_login_cap.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_session_login_cap.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_session_login_cap_session_login_cap.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_session_login_cap_session_login_cap.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_session_login_response.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_session_login_response.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_session_login_response_session_login.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_session_login_response_session_login.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_session_login_session_login.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_session_login_session_login.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_audio.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_audio.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_list.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_list.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_list_streaming_channel_list.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_list_streaming_channel_list.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_transport.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_transport.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_transport_control_protocol_list.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_transport_control_protocol_list.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_transport_control_protocol_list_control_protocol_item.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_transport_control_protocol_list_control_protocol_item.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_transport_security.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_transport_security.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_video.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_streaming_channel_video.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_list.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_list.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_list_two_way_audio_channel_list.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_list_two_way_audio_channel_list.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs_enabled.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs_enabled.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs_video_input_channel_list.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs_video_input_channel_list.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs_video_input_channel_list_video_input_channel_id.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_associate_video_inputs_video_input_channel_list_video_input_channel_id.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_bit_rate.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_bit_rate.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_compression_type.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_compression_type.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_inbound_compression_type.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_inbound_compression_type.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_input_type.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_audio_input_type.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_enabled.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_enabled.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_id.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_id.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_line_out_forbidden.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_line_out_forbidden.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_mic_in_forbidden.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_mic_in_forbidden.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_microphone_volume.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_microphone_volume.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_noisereduce.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_noisereduce.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_speaker_volume.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_channel_two_way_audio_channel_speaker_volume.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_session.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_session.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_session_two_way_audio_session.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_two_way_audio_session_two_way_audio_session.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_user_check.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_user_check.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_user_check_user_check.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_user_check_user_check.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_list.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_list.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_list_video_input_channel_list.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_list_video_input_channel_list.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_id.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_id.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_input_port.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_input_port.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_name.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_name.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_port_type.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_port_type.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_res_desc.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_res_desc.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_video_format.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_video_format.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_video_input_enabled.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/models/root_type_for_xml_video_input_channel_video_input_channel_video_input_enabled.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_cli/types.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_cli/types.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_sk/session.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_sk/session.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/hikvision_isapi_sk/snap.py` & `hikvision_isapi_cli-1.1.1/hikvision_isapi_sk/snap.py`

 * *Files identical despite different names*

### Comparing `hikvision_isapi_cli-1.1.0/pyproject.toml` & `hikvision_isapi_cli-1.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "hikvision-isapi-cli"
-version = "1.1.0"
+version = "1.1.1"
 description = "A client library for accessing Hikvision ISAPI and more"
 
 authors = ["mmascia"]
 
 readme = "README.md"
 packages = [
     {include = "hikvision_isapi_cli"},
     {include = "hikvision_isapi_sk"},
 ]
 include = ["CHANGELOG.md", "hikvision_isapi_cli/py.typed", "docs"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-httpx = "==0.24.0"
+httpx = "==0.24.1"
 python-dateutil = "==2.8.2"
-xmltodict = "==0.13.0"
+xmltodict = "=0.13.0"
 pytest-asyncio = "==0.20.3"
 pytest-aiohttp = "==1.0.4"
 pytest-cov = "==3.0.0"
 pytest-freezer = "==0.4.6"
 pytest-socket = "==0.5.1"
 pytest-test-groups = "==1.0.3"
 pytest-sugar = "==0.9.6"
```

### Comparing `hikvision_isapi_cli-1.1.0/PKG-INFO` & `hikvision_isapi_cli-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: hikvision-isapi-cli
-Version: 1.1.0
+Version: 1.1.1
 Summary: A client library for accessing Hikvision ISAPI and more
 Author: mmascia
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: httpx (==0.24.0)
+Requires-Dist: httpx (==0.24.1)
 Requires-Dist: pytest (==7.3.1)
 Requires-Dist: pytest-aiohttp (==1.0.4)
 Requires-Dist: pytest-asyncio (==0.20.3)
 Requires-Dist: pytest-cov (==3.0.0)
 Requires-Dist: pytest-freezer (==0.4.6)
 Requires-Dist: pytest-picked (==0.4.6)
 Requires-Dist: pytest-socket (==0.5.1)
```

