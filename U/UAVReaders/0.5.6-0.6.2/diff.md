# Comparing `tmp/UAVReaders-0.5.6.tar.gz` & `tmp/UAVReaders-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UAVReaders-0.5.6.tar", last modified: Thu May  4 22:16:10 2023, max compression
+gzip compressed data, was "UAVReaders-0.6.2.tar", last modified: Fri Jul 14 23:59:48 2023, max compression
```

## Comparing `UAVReaders-0.5.6.tar` & `UAVReaders-0.6.2.tar`

### file list

```diff
@@ -1,457 +1,458 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.855582 UAVReaders-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-04 22:15:35.000000 UAVReaders-0.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-04 22:16:10.855582 UAVReaders-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-04 22:15:35.000000 UAVReaders-0.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.775581 UAVReaders-0.5.6/UAVReaders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-04 22:16:10.000000 UAVReaders-0.5.6/UAVReaders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-05-04 22:16:10.000000 UAVReaders-0.5.6/UAVReaders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 22:16:10.000000 UAVReaders-0.5.6/UAVReaders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 22:16:10.000000 UAVReaders-0.5.6/UAVReaders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-04 22:15:35.000000 UAVReaders-0.5.6/c_introspect.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-04 22:15:35.000000 UAVReaders-0.5.6/c_introspect.h
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-04 22:15:35.000000 UAVReaders-0.5.6/dataflash.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-04 22:15:35.000000 UAVReaders-0.5.6/dataflash.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.775581 UAVReaders-0.5.6/mavlink/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.779581 UAVReaders-0.5.6/mavlink/ASLUAV/
--rw-r--r--   0 runner    (1001) docker     (123)    25766 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/ASLUAV.h
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)    15283 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_asl_obctrl.h
--rw-r--r--   0 runner    (1001) docker     (123)    32302 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_aslctrl_data.h
--rw-r--r--   0 runner    (1001) docker     (123)    17208 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_aslctrl_debug.h
--rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_asluav_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    26694 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_command_int_stamped.h
--rw-r--r--   0 runner    (1001) docker     (123)    25076 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_command_long_stamped.h
--rw-r--r--   0 runner    (1001) docker     (123)    14130 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_ekf_ext.h
--rw-r--r--   0 runner    (1001) docker     (123)    37305 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_fw_soaring_data.h
--rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_gsm_link_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    18821 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_satcom_link_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sens_atmos.h
--rw-r--r--   0 runner    (1001) docker     (123)    26167 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sens_batmon.h
--rw-r--r--   0 runner    (1001) docker     (123)    21554 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sens_mppt.h
--rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sens_power.h
--rw-r--r--   0 runner    (1001) docker     (123)    24857 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sens_power_board.h
--rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sensor_airflow_angles.h
--rw-r--r--   0 runner    (1001) docker     (123)    18334 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sensorpod_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    66439 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.783581 UAVReaders-0.5.6/mavlink/AVSSUAS/
--rw-r--r--   0 runner    (1001) docker     (123)    25408 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/AVSSUAS/AVSSUAS.h
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/AVSSUAS/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)    18968 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/AVSSUAS/mavlink_msg_avss_drone_imu.h
--rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/AVSSUAS/mavlink_msg_avss_drone_operation_mode.h
--rw-r--r--   0 runner    (1001) docker     (123)    15511 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/AVSSUAS/mavlink_msg_avss_drone_position.h
--rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/AVSSUAS/mavlink_msg_avss_prs_sys_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    14399 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/AVSSUAS/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/AVSSUAS/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.783581 UAVReaders-0.5.6/mavlink/all/
--rw-r--r--   0 runner    (1001) docker     (123)    35975 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/all/all.h
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/all/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/all/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/all/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.795581 UAVReaders-0.5.6/mavlink/ardupilotmega/
--rw-r--r--   0 runner    (1001) docker     (123)   146469 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/ardupilotmega.h
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)    20361 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_adap_tuning.h
--rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_ahrs.h
--rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_ahrs2.h
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_ahrs3.h
--rw-r--r--   0 runner    (1001) docker     (123)    19616 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_airspeed_autocal.h
--rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_aoa_ssa.h
--rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_ap_adc.h
--rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_autopilot_version_request.h
--rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_battery2.h
--rw-r--r--   0 runner    (1001) docker     (123)    23445 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_camera_feedback.h
--rw-r--r--   0 runner    (1001) docker     (123)    17589 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_camera_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    14750 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_compassmot_status.h
--rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_data16.h
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_data32.h
--rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_data64.h
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_data96.h
--rw-r--r--   0 runner    (1001) docker     (123)    19561 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_deepstall.h
--rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_device_op_read.h
--rw-r--r--   0 runner    (1001) docker     (123)    14869 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_device_op_read_reply.h
--rw-r--r--   0 runner    (1001) docker     (123)    20176 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_device_op_write.h
--rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_device_op_write_reply.h
--rw-r--r--   0 runner    (1001) docker     (123)    22964 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_digicam_configure.h
--rw-r--r--   0 runner    (1001) docker     (123)    20889 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_digicam_control.h
--rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_ekf_status_report.h
--rw-r--r--   0 runner    (1001) docker     (123)    16696 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_esc_telemetry_1_to_4.h
--rw-r--r--   0 runner    (1001) docker     (123)    16696 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_esc_telemetry_5_to_8.h
--rw-r--r--   0 runner    (1001) docker     (123)    16842 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_esc_telemetry_9_to_12.h
--rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_fence_fetch_point.h
--rw-r--r--   0 runner    (1001) docker     (123)    13532 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_fence_point.h
--rw-r--r--   0 runner    (1001) docker     (123)    13840 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gimbal_control.h
--rw-r--r--   0 runner    (1001) docker     (123)    21961 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gimbal_report.h
--rw-r--r--   0 runner    (1001) docker     (123)    14917 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gimbal_torque_cmd_report.h
--rw-r--r--   0 runner    (1001) docker     (123)    11044 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gopro_get_request.h
--rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gopro_get_response.h
--rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gopro_heartbeat.h
--rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gopro_set_request.h
--rw-r--r--   0 runner    (1001) docker     (123)     9542 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gopro_set_response.h
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_hwstatus.h
--rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_led_control.h
--rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_limits_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    19419 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_mag_cal_progress.h
--rw-r--r--   0 runner    (1001) docker     (123)    12861 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_mcu_status.h
--rw-r--r--   0 runner    (1001) docker     (123)     9642 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_meminfo.h
--rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_mount_configure.h
--rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_mount_control.h
--rw-r--r--   0 runner    (1001) docker     (123)    14081 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_mount_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    19293 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_obstacle_distance_3d.h
--rw-r--r--   0 runner    (1001) docker     (123)    21041 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_osd_param_config.h
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_osd_param_config_reply.h
--rw-r--r--   0 runner    (1001) docker     (123)    14313 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_osd_param_show_config.h
--rw-r--r--   0 runner    (1001) docker     (123)    18684 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_osd_param_show_config_reply.h
--rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_pid_tuning.h
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_radio.h
--rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_rally_fetch_point.h
--rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_rally_point.h
--rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_rangefinder.h
--rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_remote_log_block_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_remote_log_data_block.h
--rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_rpm.h
--rw-r--r--   0 runner    (1001) docker     (123)    21565 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_sensor_offsets.h
--rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_set_mag_offsets.h
--rw-r--r--   0 runner    (1001) docker     (123)    17127 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_simstate.h
--rw-r--r--   0 runner    (1001) docker     (123)    16395 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_vision_position_delta.h
--rw-r--r--   0 runner    (1001) docker     (123)    18313 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_water_depth.h
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_wind.h
--rw-r--r--   0 runner    (1001) docker     (123)   219339 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/version.h
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/checksum.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.839582 UAVReaders-0.5.6/mavlink/common/
--rw-r--r--   0 runner    (1001) docker     (123)   164519 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/common.h
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)    15007 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_actuator_control_target.h
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_actuator_output_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    22225 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_adsb_vehicle.h
--rw-r--r--   0 runner    (1001) docker     (123)    27216 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_ais_vessel.h
--rw-r--r--   0 runner    (1001) docker     (123)    22867 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_altitude.h
--rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_att_pos_mocap.h
--rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_attitude.h
--rw-r--r--   0 runner    (1001) docker     (123)    21250 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_attitude_quaternion.h
--rw-r--r--   0 runner    (1001) docker     (123)    17834 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_attitude_quaternion_cov.h
--rw-r--r--   0 runner    (1001) docker     (123)    16735 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_attitude_target.h
--rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_auth_key.h
--rw-r--r--   0 runner    (1001) docker     (123)    30727 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_autopilot_state_for_gimbal_device.h
--rw-r--r--   0 runner    (1001) docker     (123)    29075 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_autopilot_version.h
--rw-r--r--   0 runner    (1001) docker     (123)    32779 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_battery_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    10853 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_button_change.h
--rw-r--r--   0 runner    (1001) docker     (123)    19444 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_capture_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    21741 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_fov_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    23640 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_image_captured.h
--rw-r--r--   0 runner    (1001) docker     (123)    28706 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_information.h
--rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_settings.h
--rw-r--r--   0 runner    (1001) docker     (123)    24575 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_tracking_geo_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    25202 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_tracking_image_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_trigger.h
--rw-r--r--   0 runner    (1001) docker     (123)    14952 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_can_filter_modify.h
--rw-r--r--   0 runner    (1001) docker     (123)    12988 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_can_frame.h
--rw-r--r--   0 runner    (1001) docker     (123)    13283 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_canfd_frame.h
--rw-r--r--   0 runner    (1001) docker     (123)    20341 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_cellular_config.h
--rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_cellular_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_change_operator_control.h
--rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_change_operator_control_ack.h
--rw-r--r--   0 runner    (1001) docker     (123)    16191 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_collision.h
--rw-r--r--   0 runner    (1001) docker     (123)    16633 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_command_ack.h
--rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_command_cancel.h
--rw-r--r--   0 runner    (1001) docker     (123)    21732 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_command_int.h
--rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_command_long.h
--rw-r--r--   0 runner    (1001) docker     (123)    20305 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_component_information.h
--rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_component_metadata.h
--rw-r--r--   0 runner    (1001) docker     (123)    29561 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_control_system_state.h
--rw-r--r--   0 runner    (1001) docker     (123)    10060 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_current_event_sequence.h
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_data_stream.h
--rw-r--r--   0 runner    (1001) docker     (123)    17663 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_data_transmission_handshake.h
--rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_debug.h
--rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_debug_float_array.h
--rw-r--r--   0 runner    (1001) docker     (123)    12155 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_debug_vect.h
--rw-r--r--   0 runner    (1001) docker     (123)    27666 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_distance_sensor.h
--rw-r--r--   0 runner    (1001) docker     (123)    32838 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_efi_status.h
--rw-r--r--   0 runner    (1001) docker     (123)     9942 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_encapsulated_data.h
--rw-r--r--   0 runner    (1001) docker     (123)    20131 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_esc_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    14316 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_esc_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    21732 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_estimator_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_event.h
--rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_extended_sys_state.h
--rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_fence_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_file_transfer_protocol.h
--rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_flight_information.h
--rw-r--r--   0 runner    (1001) docker     (123)    21332 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_follow_target.h
--rw-r--r--   0 runner    (1001) docker     (123)    26488 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_generator_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    27546 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_device_attitude_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    32438 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_device_information.h
--rw-r--r--   0 runner    (1001) docker     (123)    20454 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_device_set_attitude.h
--rw-r--r--   0 runner    (1001) docker     (123)    21643 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_manager_information.h
--rw-r--r--   0 runner    (1001) docker     (123)    22236 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_manager_set_attitude.h
--rw-r--r--   0 runner    (1001) docker     (123)    21708 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_manager_set_manual_control.h
--rw-r--r--   0 runner    (1001) docker     (123)    20581 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_manager_set_pitchyaw.h
--rw-r--r--   0 runner    (1001) docker     (123)    19605 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_manager_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_global_position_int.h
--rw-r--r--   0 runner    (1001) docker     (123)    22136 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_global_position_int_cov.h
--rw-r--r--   0 runner    (1001) docker     (123)    22008 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_global_vision_position_estimate.h
--rw-r--r--   0 runner    (1001) docker     (123)    29060 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps2_raw.h
--rw-r--r--   0 runner    (1001) docker     (123)    23748 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps2_rtk.h
--rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_global_origin.h
--rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_inject_data.h
--rw-r--r--   0 runner    (1001) docker     (123)    30409 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_input.h
--rw-r--r--   0 runner    (1001) docker     (123)    28204 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_raw_int.h
--rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_rtcm_data.h
--rw-r--r--   0 runner    (1001) docker     (123)    23541 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_rtk.h
--rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    36773 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_high_latency.h
--rw-r--r--   0 runner    (1001) docker     (123)    40352 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_high_latency2.h
--rw-r--r--   0 runner    (1001) docker     (123)    25647 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_highres_imu.h
--rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_actuator_controls.h
--rw-r--r--   0 runner    (1001) docker     (123)    19626 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_controls.h
--rw-r--r--   0 runner    (1001) docker     (123)    25408 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_gps.h
--rw-r--r--   0 runner    (1001) docker     (123)    26914 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_optical_flow.h
--rw-r--r--   0 runner    (1001) docker     (123)    25694 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_rc_inputs_raw.h
--rw-r--r--   0 runner    (1001) docker     (123)    25462 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_sensor.h
--rw-r--r--   0 runner    (1001) docker     (123)    23587 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_state.h
--rw-r--r--   0 runner    (1001) docker     (123)    28077 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_state_quaternion.h
--rw-r--r--   0 runner    (1001) docker     (123)    26362 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_home_position.h
--rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_hygrometer_sensor.h
--rw-r--r--   0 runner    (1001) docker     (123)    21373 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_isbd_link_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    25433 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_landing_target.h
--rw-r--r--   0 runner    (1001) docker     (123)    22275 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_link_node_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    14315 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_local_position_ned.h
--rw-r--r--   0 runner    (1001) docker     (123)    23152 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_local_position_ned_cov.h
--rw-r--r--   0 runner    (1001) docker     (123)    17627 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_local_position_ned_system_global_offset.h
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_log_data.h
--rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_log_entry.h
--rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_log_erase.h
--rw-r--r--   0 runner    (1001) docker     (123)    13013 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_log_request_data.h
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_log_request_end.h
--rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_log_request_list.h
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_logging_ack.h
--rw-r--r--   0 runner    (1001) docker     (123)    15228 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_logging_data.h
--rw-r--r--   0 runner    (1001) docker     (123)    16084 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_logging_data_acked.h
--rw-r--r--   0 runner    (1001) docker     (123)    28867 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mag_cal_report.h
--rw-r--r--   0 runner    (1001) docker     (123)    25464 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_manual_control.h
--rw-r--r--   0 runner    (1001) docker     (123)    15766 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_manual_setpoint.h
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_memory_vect.h
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_message_interval.h
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_ack.h
--rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_clear_all.h
--rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_count.h
--rw-r--r--   0 runner    (1001) docker     (123)    13767 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_current.h
--rw-r--r--   0 runner    (1001) docker     (123)    24141 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_item.h
--rw-r--r--   0 runner    (1001) docker     (123)    26048 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_item_int.h
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_item_reached.h
--rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_request.h
--rw-r--r--   0 runner    (1001) docker     (123)    12438 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_request_int.h
--rw-r--r--   0 runner    (1001) docker     (123)    11572 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_request_list.h
--rw-r--r--   0 runner    (1001) docker     (123)    15394 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_request_partial_list.h
--rw-r--r--   0 runner    (1001) docker     (123)    11164 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_set_current.h
--rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_write_partial_list.h
--rw-r--r--   0 runner    (1001) docker     (123)    13896 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mount_orientation.h
--rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_named_value_float.h
--rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_named_value_int.h
--rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_nav_controller_output.h
--rw-r--r--   0 runner    (1001) docker     (123)    24972 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_obstacle_distance.h
--rw-r--r--   0 runner    (1001) docker     (123)    32455 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_odometry.h
--rw-r--r--   0 runner    (1001) docker     (123)    48490 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_onboard_computer_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_arm_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    25685 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_authentication.h
--rw-r--r--   0 runner    (1001) docker     (123)    17580 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_basic_id.h
--rw-r--r--   0 runner    (1001) docker     (123)    40771 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_location.h
--rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_message_pack.h
--rw-r--r--   0 runner    (1001) docker     (123)    16940 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_operator_id.h
--rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_self_id.h
--rw-r--r--   0 runner    (1001) docker     (123)    32622 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_system.h
--rw-r--r--   0 runner    (1001) docker     (123)    18204 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_system_update.h
--rw-r--r--   0 runner    (1001) docker     (123)    20576 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_optical_flow.h
--rw-r--r--   0 runner    (1001) docker     (123)    26804 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_optical_flow_rad.h
--rw-r--r--   0 runner    (1001) docker     (123)    17116 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_orbit_execution_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_ext_ack.h
--rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_ext_request_list.h
--rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_ext_request_read.h
--rw-r--r--   0 runner    (1001) docker     (123)    14708 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_ext_set.h
--rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_ext_value.h
--rw-r--r--   0 runner    (1001) docker     (123)    22140 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_map_rc.h
--rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_request_list.h
--rw-r--r--   0 runner    (1001) docker     (123)    14316 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_request_read.h
--rw-r--r--   0 runner    (1001) docker     (123)    13957 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_set.h
--rw-r--r--   0 runner    (1001) docker     (123)    14254 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_value.h
--rw-r--r--   0 runner    (1001) docker     (123)    12766 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_ping.h
--rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_play_tune.h
--rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_play_tune_v2.h
--rw-r--r--   0 runner    (1001) docker     (123)    27839 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_position_target_global_int.h
--rw-r--r--   0 runner    (1001) docker     (123)    26159 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_position_target_local_ned.h
--rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_power_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    17212 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_radio_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    20265 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_raw_imu.h
--rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_raw_pressure.h
--rw-r--r--   0 runner    (1001) docker     (123)     8597 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_raw_rpm.h
--rw-r--r--   0 runner    (1001) docker     (123)    33163 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_rc_channels.h
--rw-r--r--   0 runner    (1001) docker     (123)    44394 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_rc_channels_override.h
--rw-r--r--   0 runner    (1001) docker     (123)    21192 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_rc_channels_raw.h
--rw-r--r--   0 runner    (1001) docker     (123)    22513 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_rc_channels_scaled.h
--rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_request_data_stream.h
--rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_request_event.h
--rw-r--r--   0 runner    (1001) docker     (123)    15666 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_resource_request.h
--rw-r--r--   0 runner    (1001) docker     (123)    14641 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_response_event_error.h
--rw-r--r--   0 runner    (1001) docker     (123)    15336 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_safety_allowed_area.h
--rw-r--r--   0 runner    (1001) docker     (123)    18702 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_safety_set_allowed_area.h
--rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_scaled_imu.h
--rw-r--r--   0 runner    (1001) docker     (123)    19078 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_scaled_imu2.h
--rw-r--r--   0 runner    (1001) docker     (123)    19078 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_scaled_imu3.h
--rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_scaled_pressure.h
--rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_scaled_pressure2.h
--rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_scaled_pressure3.h
--rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_serial_control.h
--rw-r--r--   0 runner    (1001) docker     (123)    31142 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_servo_output_raw.h
--rw-r--r--   0 runner    (1001) docker     (123)    18303 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_actuator_control_target.h
--rw-r--r--   0 runner    (1001) docker     (123)    21827 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_attitude_target.h
--rw-r--r--   0 runner    (1001) docker     (123)    14839 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_gps_global_origin.h
--rw-r--r--   0 runner    (1001) docker     (123)    28389 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_home_position.h
--rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_mode.h
--rw-r--r--   0 runner    (1001) docker     (123)    31542 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_position_target_global_int.h
--rw-r--r--   0 runner    (1001) docker     (123)    29883 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_position_target_local_ned.h
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_setup_signing.h
--rw-r--r--   0 runner    (1001) docker     (123)    33189 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_sim_state.h
--rw-r--r--   0 runner    (1001) docker     (123)    37137 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_smart_battery_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    13245 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_statustext.h
--rw-r--r--   0 runner    (1001) docker     (123)    27262 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_storage_information.h
--rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_supported_tunes.h
--rw-r--r--   0 runner    (1001) docker     (123)    36382 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_sys_status.h
--rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_system_time.h
--rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_terrain_check.h
--rw-r--r--   0 runner    (1001) docker     (123)    12755 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_terrain_data.h
--rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_terrain_report.h
--rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_terrain_request.h
--rw-r--r--   0 runner    (1001) docker     (123)    17785 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_time_estimate_to_target.h
--rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_timesync.h
--rw-r--r--   0 runner    (1001) docker     (123)    21152 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_trajectory_representation_bezier.h
--rw-r--r--   0 runner    (1001) docker     (123)    33591 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_trajectory_representation_waypoints.h
--rw-r--r--   0 runner    (1001) docker     (123)    15996 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_tunnel.h
--rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_uavcan_node_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_uavcan_node_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    29856 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_utm_global_position.h
--rw-r--r--   0 runner    (1001) docker     (123)    19231 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_v2_extension.h
--rw-r--r--   0 runner    (1001) docker     (123)    13981 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_vfr_hud.h
--rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_vibration.h
--rw-r--r--   0 runner    (1001) docker     (123)    18003 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_vicon_position_estimate.h
--rw-r--r--   0 runner    (1001) docker     (123)    23764 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_video_stream_information.h
--rw-r--r--   0 runner    (1001) docker     (123)    17441 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_video_stream_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    20723 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_vision_position_estimate.h
--rw-r--r--   0 runner    (1001) docker     (123)    16707 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_vision_speed_estimate.h
--rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_wheel_distance.h
--rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_wifi_config_ap.h
--rw-r--r--   0 runner    (1001) docker     (123)    17186 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_winch_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    19004 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_wind_cov.h
--rw-r--r--   0 runner    (1001) docker     (123)   809444 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.839582 UAVReaders-0.5.6/mavlink/cubepilot/
--rw-r--r--   0 runner    (1001) docker     (123)    23605 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/cubepilot/cubepilot.h
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/cubepilot/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/cubepilot/mavlink_msg_cubepilot_firmware_update_resp.h
--rw-r--r--   0 runner    (1001) docker     (123)    13725 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/cubepilot/mavlink_msg_cubepilot_firmware_update_start.h
--rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/cubepilot/mavlink_msg_cubepilot_raw_rc.h
--rw-r--r--   0 runner    (1001) docker     (123)    14173 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/cubepilot/mavlink_msg_herelink_telem.h
--rw-r--r--   0 runner    (1001) docker     (123)    20451 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/cubepilot/mavlink_msg_herelink_video_stream_information.h
--rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/cubepilot/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/cubepilot/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.843582 UAVReaders-0.5.6/mavlink/development/
--rw-r--r--   0 runner    (1001) docker     (123)    38436 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/development.h
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_airspeed.h
--rw-r--r--   0 runner    (1001) docker     (123)    15694 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_available_modes.h
--rw-r--r--   0 runner    (1001) docker     (123)    20885 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_battery_status_v2.h
--rw-r--r--   0 runner    (1001) docker     (123)    22951 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_component_information_basic.h
--rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_current_mode.h
--rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_figure_eight_execution_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    11639 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_group_end.h
--rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_group_start.h
--rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_mission_checksum.h
--rw-r--r--   0 runner    (1001) docker     (123)    17317 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_param_ack_transaction.h
--rw-r--r--   0 runner    (1001) docker     (123)    25425 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_target_absolute.h
--rw-r--r--   0 runner    (1001) docker     (123)    21946 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_target_relative.h
--rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_wifi_network_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    45228 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.843582 UAVReaders-0.5.6/mavlink/icarous/
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/icarous/icarous.h
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/icarous/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/icarous/mavlink_msg_icarous_heartbeat.h
--rw-r--r--   0 runner    (1001) docker     (123)    25956 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/icarous/mavlink_msg_icarous_kinematic_bands.h
--rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/icarous/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/icarous/version.h
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/mavlink_conversions.h
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/mavlink_get_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    37370 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/mavlink_helpers.h
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/mavlink_sha256.h
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/mavlink_types.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.847582 UAVReaders-0.5.6/mavlink/minimal/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/minimal/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/minimal/mavlink_msg_heartbeat.h
--rw-r--r--   0 runner    (1001) docker     (123)    15671 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/minimal/mavlink_msg_protocol_version.h
--rw-r--r--   0 runner    (1001) docker     (123)    30758 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/minimal/minimal.h
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/minimal/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/minimal/version.h
--rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/protocol.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.847582 UAVReaders-0.5.6/mavlink/python_array_test/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/python_array_test/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_0.h
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_1.h
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_3.h
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_4.h
--rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_5.h
--rw-r--r--   0 runner    (1001) docker     (123)    21106 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_6.h
--rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_7.h
--rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_8.h
--rw-r--r--   0 runner    (1001) docker     (123)    23871 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/python_array_test/python_array_test.h
--rw-r--r--   0 runner    (1001) docker     (123)    26161 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/python_array_test/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/python_array_test/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.847582 UAVReaders-0.5.6/mavlink/standard/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/standard/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/standard/standard.h
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/standard/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/standard/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.851582 UAVReaders-0.5.6/mavlink/storm32/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_frsky_passthrough_array.h
--rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_param_value_array.h
--rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_qshot_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    28610 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_radio_link_stats.h
--rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_radio_rc_channels.h
--rw-r--r--   0 runner    (1001) docker     (123)    26585 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_control.h
--rw-r--r--   0 runner    (1001) docker     (123)    26558 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_control_pitchyaw.h
--rw-r--r--   0 runner    (1001) docker     (123)    16806 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_correct_roll.h
--rw-r--r--   0 runner    (1001) docker     (123)    24582 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_information.h
--rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    41670 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/storm32.h
--rw-r--r--   0 runner    (1001) docker     (123)    39288 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.851582 UAVReaders-0.5.6/mavlink/test/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/test/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)    31221 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/test/mavlink_msg_test_types.h
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/test/test.h
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/test/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/test/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.851582 UAVReaders-0.5.6/mavlink/uAvionix/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/uAvionix/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)    19675 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/uAvionix/mavlink_msg_uavionix_adsb_out_cfg.h
--rw-r--r--   0 runner    (1001) docker     (123)    31688 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/uAvionix/mavlink_msg_uavionix_adsb_out_dynamic.h
--rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/uAvionix/mavlink_msg_uavionix_adsb_transceiver_health_report.h
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/uAvionix/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)    28686 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/uAvionix/uAvionix.h
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/uAvionix/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.855582 UAVReaders-0.5.6/mavlink/ualberta/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/ualberta/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)    14284 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/ualberta/mavlink_msg_nav_filter_bias.h
--rw-r--r--   0 runner    (1001) docker     (123)    16639 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/ualberta/mavlink_msg_radio_calibration.h
--rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/ualberta/mavlink_msg_ualberta_sys_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/ualberta/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)    24428 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/ualberta/ualberta.h
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/ualberta/version.h
--rw-r--r--   0 runner    (1001) docker     (123)   708323 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink_introspect_gen.c
--rw-r--r--   0 runner    (1001) docker     (123)    24009 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink_introspect_gen.h
--rw-r--r--   0 runner    (1001) docker     (123)  1117162 2023-05-04 22:15:56.000000 UAVReaders-0.5.6/pyinterop.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-04 22:15:35.000000 UAVReaders-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-04 22:15:35.000000 UAVReaders-0.5.6/readers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-04 22:15:35.000000 UAVReaders-0.5.6/readers.h
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 22:16:10.855582 UAVReaders-0.5.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      686 2023-05-04 22:15:35.000000 UAVReaders-0.5.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-04 22:15:35.000000 UAVReaders-0.5.6/table.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:59:48.306499 UAVReaders-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-14 23:59:16.000000 UAVReaders-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-14 23:59:16.000000 UAVReaders-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-14 23:59:48.306499 UAVReaders-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-14 23:59:16.000000 UAVReaders-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:59:48.226499 UAVReaders-0.6.2/UAVReaders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-14 23:59:48.000000 UAVReaders-0.6.2/UAVReaders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19106 2023-07-14 23:59:48.000000 UAVReaders-0.6.2/UAVReaders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:59:48.000000 UAVReaders-0.6.2/UAVReaders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 23:59:48.000000 UAVReaders-0.6.2/UAVReaders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-14 23:59:16.000000 UAVReaders-0.6.2/c_introspect.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-14 23:59:16.000000 UAVReaders-0.6.2/c_introspect.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-07-14 23:59:16.000000 UAVReaders-0.6.2/dataflash.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-14 23:59:16.000000 UAVReaders-0.6.2/dataflash.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:59:48.230499 UAVReaders-0.6.2/mavlink/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:59:48.234499 UAVReaders-0.6.2/mavlink/ASLUAV/
+-rw-r--r--   0 runner    (1001) docker     (123)    25765 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ASLUAV/ASLUAV.h
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ASLUAV/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15283 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_asl_obctrl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32302 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_aslctrl_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17208 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_aslctrl_debug.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_asluav_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26694 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_command_int_stamped.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25076 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_command_long_stamped.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14130 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_ekf_ext.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37305 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_fw_soaring_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_gsm_link_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18821 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_satcom_link_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_sens_atmos.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26167 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_sens_batmon.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21554 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_sens_mppt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_sens_power.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24857 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_sens_power_board.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_sensor_airflow_angles.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18334 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_sensorpod_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    66439 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ASLUAV/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ASLUAV/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:59:48.234499 UAVReaders-0.6.2/mavlink/AVSSUAS/
+-rw-r--r--   0 runner    (1001) docker     (123)    25409 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/AVSSUAS/AVSSUAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/AVSSUAS/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18968 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/AVSSUAS/mavlink_msg_avss_drone_imu.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/AVSSUAS/mavlink_msg_avss_drone_operation_mode.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15511 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/AVSSUAS/mavlink_msg_avss_drone_position.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/AVSSUAS/mavlink_msg_avss_prs_sys_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14399 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/AVSSUAS/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/AVSSUAS/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:59:48.234499 UAVReaders-0.6.2/mavlink/all/
+-rw-r--r--   0 runner    (1001) docker     (123)    35977 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/all/all.h
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-14 23:59:32.000000 UAVReaders-0.6.2/mavlink/all/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/all/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-14 23:59:32.000000 UAVReaders-0.6.2/mavlink/all/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:59:48.246499 UAVReaders-0.6.2/mavlink/ardupilotmega/
+-rw-r--r--   0 runner    (1001) docker     (123)   146468 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/ardupilotmega.h
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20361 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_adap_tuning.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_ahrs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_ahrs2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_ahrs3.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19616 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_airspeed_autocal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_aoa_ssa.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_ap_adc.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_autopilot_version_request.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_battery2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23445 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_camera_feedback.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17589 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_camera_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14750 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_compassmot_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_data16.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_data32.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_data64.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_data96.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19561 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_deepstall.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_device_op_read.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14869 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_device_op_read_reply.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20176 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_device_op_write.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_device_op_write_reply.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22964 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_digicam_configure.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20889 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_digicam_control.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_ekf_status_report.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16696 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_esc_telemetry_1_to_4.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16696 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_esc_telemetry_5_to_8.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16842 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_esc_telemetry_9_to_12.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_fence_fetch_point.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13532 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_fence_point.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13840 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_gimbal_control.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21961 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_gimbal_report.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14917 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_gimbal_torque_cmd_report.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11044 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_gopro_get_request.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_gopro_get_response.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_gopro_heartbeat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_gopro_set_request.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9542 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_gopro_set_response.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_hwstatus.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_led_control.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_limits_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19419 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_mag_cal_progress.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12861 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_mcu_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9642 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_meminfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_mount_configure.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_mount_control.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14081 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_mount_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19293 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_obstacle_distance_3d.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21041 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_osd_param_config.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_osd_param_config_reply.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14313 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_osd_param_show_config.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18684 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_osd_param_show_config_reply.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_pid_tuning.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_radio.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_rally_fetch_point.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_rally_point.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_rangefinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_remote_log_block_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_remote_log_data_block.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_rpm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21565 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_sensor_offsets.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_set_mag_offsets.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17127 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_simstate.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16395 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_vision_position_delta.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18313 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_water_depth.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_wind.h
+-rw-r--r--   0 runner    (1001) docker     (123)   219339 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ardupilotmega/version.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/checksum.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:59:48.290499 UAVReaders-0.6.2/mavlink/common/
+-rw-r--r--   0 runner    (1001) docker     (123)   164520 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15007 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_actuator_control_target.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_actuator_output_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22225 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_adsb_vehicle.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27216 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_ais_vessel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22867 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_altitude.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_att_pos_mocap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_attitude.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21250 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_attitude_quaternion.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17834 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_attitude_quaternion_cov.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16735 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_attitude_target.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_auth_key.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30727 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_autopilot_state_for_gimbal_device.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29075 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_autopilot_version.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32779 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_battery_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10853 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_button_change.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19444 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_camera_capture_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21741 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_camera_fov_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23640 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_camera_image_captured.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28706 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_camera_information.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_camera_settings.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24575 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_camera_tracking_geo_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25202 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_camera_tracking_image_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_camera_trigger.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14952 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_can_filter_modify.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12988 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_can_frame.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13283 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_canfd_frame.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20341 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_cellular_config.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_cellular_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_change_operator_control.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_change_operator_control_ack.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16191 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_collision.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16633 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_command_ack.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_command_cancel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21732 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_command_int.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_command_long.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20305 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_component_information.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_component_metadata.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29561 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_control_system_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10060 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_current_event_sequence.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_data_stream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17663 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_data_transmission_handshake.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_debug.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_debug_float_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12155 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_debug_vect.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27666 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_distance_sensor.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32838 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_efi_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9942 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_encapsulated_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20131 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_esc_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14316 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_esc_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21732 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_estimator_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_event.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_extended_sys_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_fence_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_file_transfer_protocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_flight_information.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21332 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_follow_target.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26488 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_generator_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27546 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_gimbal_device_attitude_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32438 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_gimbal_device_information.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20454 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_gimbal_device_set_attitude.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21643 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_gimbal_manager_information.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22236 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_gimbal_manager_set_attitude.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21708 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_gimbal_manager_set_manual_control.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20581 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_gimbal_manager_set_pitchyaw.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19605 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_gimbal_manager_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_global_position_int.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22136 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_global_position_int_cov.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22008 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_global_vision_position_estimate.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29060 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_gps2_raw.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23748 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_gps2_rtk.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_gps_global_origin.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_gps_inject_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30409 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_gps_input.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28204 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_gps_raw_int.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_gps_rtcm_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23541 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_gps_rtk.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_gps_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36773 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_high_latency.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40352 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_high_latency2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25647 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_highres_imu.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_hil_actuator_controls.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19626 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_hil_controls.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25408 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_hil_gps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26914 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_hil_optical_flow.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25694 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_hil_rc_inputs_raw.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25462 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_hil_sensor.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23587 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_hil_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28077 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_hil_state_quaternion.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26362 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_home_position.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_hygrometer_sensor.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21373 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_isbd_link_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25433 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_landing_target.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22275 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_link_node_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14315 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_local_position_ned.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23152 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_local_position_ned_cov.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17627 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_local_position_ned_system_global_offset.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_log_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_log_entry.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_log_erase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13013 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_log_request_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_log_request_end.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_log_request_list.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_logging_ack.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15228 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_logging_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16084 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_logging_data_acked.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28867 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_mag_cal_report.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25464 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_manual_control.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15766 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_manual_setpoint.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_memory_vect.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_message_interval.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_ack.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_clear_all.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_count.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13767 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_current.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24141 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_item.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26048 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_item_int.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_item_reached.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_request.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12438 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_request_int.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11572 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_request_list.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15394 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_request_partial_list.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11164 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_set_current.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_write_partial_list.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13896 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_mount_orientation.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_named_value_float.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_named_value_int.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_nav_controller_output.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24972 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_obstacle_distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32455 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_odometry.h
+-rw-r--r--   0 runner    (1001) docker     (123)    48490 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_onboard_computer_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_open_drone_id_arm_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25685 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_open_drone_id_authentication.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17580 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_open_drone_id_basic_id.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40771 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_open_drone_id_location.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_open_drone_id_message_pack.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16940 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_open_drone_id_operator_id.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_open_drone_id_self_id.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32622 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_open_drone_id_system.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18204 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_open_drone_id_system_update.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20576 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_optical_flow.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26804 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_optical_flow_rad.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17116 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_orbit_execution_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_param_ext_ack.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_param_ext_request_list.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_param_ext_request_read.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14708 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_param_ext_set.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_param_ext_value.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22140 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_param_map_rc.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_param_request_list.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14316 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_param_request_read.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13957 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_param_set.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14254 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_param_value.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12766 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_ping.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_play_tune.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_play_tune_v2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27839 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_position_target_global_int.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26159 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_position_target_local_ned.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_power_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17212 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_radio_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20265 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_raw_imu.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_raw_pressure.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8597 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_raw_rpm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    33163 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_rc_channels.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44394 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_rc_channels_override.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21192 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_rc_channels_raw.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22513 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_rc_channels_scaled.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_request_data_stream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_request_event.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15666 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_resource_request.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14641 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_response_event_error.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15336 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_safety_allowed_area.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18702 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_safety_set_allowed_area.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_scaled_imu.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19078 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_scaled_imu2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19078 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_scaled_imu3.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_scaled_pressure.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_scaled_pressure2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_scaled_pressure3.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_serial_control.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31142 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_servo_output_raw.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18303 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_set_actuator_control_target.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21827 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_set_attitude_target.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14839 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_set_gps_global_origin.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28389 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_set_home_position.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_set_mode.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31542 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_set_position_target_global_int.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29883 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_set_position_target_local_ned.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_setup_signing.h
+-rw-r--r--   0 runner    (1001) docker     (123)    33189 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_sim_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37137 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_smart_battery_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13245 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_statustext.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27262 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_storage_information.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_supported_tunes.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36382 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_sys_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_system_time.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_terrain_check.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12755 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_terrain_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_terrain_report.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_terrain_request.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17785 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_time_estimate_to_target.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_timesync.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21152 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_trajectory_representation_bezier.h
+-rw-r--r--   0 runner    (1001) docker     (123)    33591 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_trajectory_representation_waypoints.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15996 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_tunnel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_uavcan_node_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_uavcan_node_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29856 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_utm_global_position.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19231 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_v2_extension.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13981 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_vfr_hud.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_vibration.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18003 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_vicon_position_estimate.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23764 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_video_stream_information.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17441 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_video_stream_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20723 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_vision_position_estimate.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16707 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_vision_speed_estimate.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_wheel_distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_wifi_config_ap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17186 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_winch_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19004 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/mavlink_msg_wind_cov.h
+-rw-r--r--   0 runner    (1001) docker     (123)   809444 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/common/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:59:48.290499 UAVReaders-0.6.2/mavlink/cubepilot/
+-rw-r--r--   0 runner    (1001) docker     (123)    23605 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/cubepilot/cubepilot.h
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/cubepilot/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/cubepilot/mavlink_msg_cubepilot_firmware_update_resp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13725 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/cubepilot/mavlink_msg_cubepilot_firmware_update_start.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/cubepilot/mavlink_msg_cubepilot_raw_rc.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14173 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/cubepilot/mavlink_msg_herelink_telem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20451 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/cubepilot/mavlink_msg_herelink_video_stream_information.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/cubepilot/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/cubepilot/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:59:48.294499 UAVReaders-0.6.2/mavlink/development/
+-rw-r--r--   0 runner    (1001) docker     (123)    38436 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/development/development.h
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/development/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/development/mavlink_msg_airspeed.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15694 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/development/mavlink_msg_available_modes.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20885 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/development/mavlink_msg_battery_status_v2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22951 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/development/mavlink_msg_component_information_basic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/development/mavlink_msg_current_mode.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/development/mavlink_msg_figure_eight_execution_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11639 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/development/mavlink_msg_group_end.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/development/mavlink_msg_group_start.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/development/mavlink_msg_mission_checksum.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17317 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/development/mavlink_msg_param_ack_transaction.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25425 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/development/mavlink_msg_target_absolute.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21946 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/development/mavlink_msg_target_relative.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/development/mavlink_msg_wifi_network_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45228 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/development/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/development/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:59:48.294499 UAVReaders-0.6.2/mavlink/icarous/
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/icarous/icarous.h
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/icarous/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/icarous/mavlink_msg_icarous_heartbeat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25956 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/icarous/mavlink_msg_icarous_kinematic_bands.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/icarous/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/icarous/version.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/mavlink_conversions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/mavlink_get_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37370 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/mavlink_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/mavlink_sha256.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/mavlink_types.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:59:48.298499 UAVReaders-0.6.2/mavlink/minimal/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/minimal/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/minimal/mavlink_msg_heartbeat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15671 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/minimal/mavlink_msg_protocol_version.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30757 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/minimal/minimal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/minimal/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/minimal/version.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/protocol.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:59:48.298499 UAVReaders-0.6.2/mavlink/python_array_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/python_array_test/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/python_array_test/mavlink_msg_array_test_0.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/python_array_test/mavlink_msg_array_test_1.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/python_array_test/mavlink_msg_array_test_3.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/python_array_test/mavlink_msg_array_test_4.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/python_array_test/mavlink_msg_array_test_5.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21106 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/python_array_test/mavlink_msg_array_test_6.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/python_array_test/mavlink_msg_array_test_7.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/python_array_test/mavlink_msg_array_test_8.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23872 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/python_array_test/python_array_test.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26161 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/python_array_test/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/python_array_test/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:59:48.298499 UAVReaders-0.6.2/mavlink/standard/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/standard/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/standard/standard.h
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/standard/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/standard/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:59:48.302499 UAVReaders-0.6.2/mavlink/storm32/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/storm32/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/storm32/mavlink_msg_frsky_passthrough_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/storm32/mavlink_msg_param_value_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/storm32/mavlink_msg_qshot_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28610 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/storm32/mavlink_msg_radio_link_stats.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/storm32/mavlink_msg_radio_rc_channels.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26585 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_control.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26558 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_control_pitchyaw.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16806 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_correct_roll.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24582 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_information.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    41670 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/storm32/storm32.h
+-rw-r--r--   0 runner    (1001) docker     (123)    39288 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/storm32/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/storm32/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:59:48.302499 UAVReaders-0.6.2/mavlink/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/test/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31221 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/test/mavlink_msg_test_types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/test/test.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/test/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/test/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:59:48.302499 UAVReaders-0.6.2/mavlink/uAvionix/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/uAvionix/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19675 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/uAvionix/mavlink_msg_uavionix_adsb_out_cfg.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31688 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/uAvionix/mavlink_msg_uavionix_adsb_out_dynamic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/uAvionix/mavlink_msg_uavionix_adsb_transceiver_health_report.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/uAvionix/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28685 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/uAvionix/uAvionix.h
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/uAvionix/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:59:48.306499 UAVReaders-0.6.2/mavlink/ualberta/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ualberta/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14284 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ualberta/mavlink_msg_nav_filter_bias.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16639 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ualberta/mavlink_msg_radio_calibration.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ualberta/mavlink_msg_ualberta_sys_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ualberta/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24427 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ualberta/ualberta.h
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink/ualberta/version.h
+-rw-r--r--   0 runner    (1001) docker     (123)   708323 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink_introspect_gen.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24009 2023-07-14 23:59:33.000000 UAVReaders-0.6.2/mavlink_introspect_gen.h
+-rw-r--r--   0 runner    (1001) docker     (123)  1119160 2023-07-14 23:59:35.000000 UAVReaders-0.6.2/pyinterop.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-14 23:59:16.000000 UAVReaders-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-14 23:59:16.000000 UAVReaders-0.6.2/readers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-14 23:59:16.000000 UAVReaders-0.6.2/readers.h
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 23:59:48.306499 UAVReaders-0.6.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      686 2023-07-14 23:59:16.000000 UAVReaders-0.6.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-14 23:59:16.000000 UAVReaders-0.6.2/table.h
```

### Comparing `UAVReaders-0.5.6/PKG-INFO` & `UAVReaders-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: UAVReaders
-Version: 0.5.6
+Version: 0.6.2
 Summary: Parsers for UAV/Aerial Drone-related formats like MavLink and DataFlash
 Author: Christian Clifford
 Author-email: Christian Clifford <cjclifford@alaska.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 [![Test UAVReaders](https://github.com/UA-ACUASI-Engineering/UAVReaders/actions/workflows/test_uavreaders.yml/badge.svg)](https://github.com/UA-ACUASI-Engineering/UAVReaders/actions/workflows/test_uavreaders.yml)
 
 # UAVReaders
 Parsers for UAV-related formats like DataFlash and Mavlink
 
 ## Installation and Usage
```

### Comparing `UAVReaders-0.5.6/README.md` & `UAVReaders-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/UAVReaders.egg-info/PKG-INFO` & `UAVReaders-0.6.2/UAVReaders.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: UAVReaders
-Version: 0.5.6
+Version: 0.6.2
 Summary: Parsers for UAV/Aerial Drone-related formats like MavLink and DataFlash
 Author: Christian Clifford
 Author-email: Christian Clifford <cjclifford@alaska.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 [![Test UAVReaders](https://github.com/UA-ACUASI-Engineering/UAVReaders/actions/workflows/test_uavreaders.yml/badge.svg)](https://github.com/UA-ACUASI-Engineering/UAVReaders/actions/workflows/test_uavreaders.yml)
 
 # UAVReaders
 Parsers for UAV-related formats like DataFlash and Mavlink
 
 ## Installation and Usage
```

### Comparing `UAVReaders-0.5.6/UAVReaders.egg-info/SOURCES.txt` & `UAVReaders-0.6.2/UAVReaders.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 c_introspect.h
 dataflash.h
 mavlink_introspect_gen.h
 pyinterop.cpp
 pyproject.toml
```

### Comparing `UAVReaders-0.5.6/c_introspect.h` & `UAVReaders-0.6.2/c_introspect.h`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 #include <sstream>
 #include <stddef.h>
 #include <string>
 #include <cstring>
 #include <type_traits>
 #include <vector>
 #include <map>
-#include <any>
 
 #include <iostream>
 
 
 extern "C" {
 #include "table.h"
 }
@@ -35,14 +34,15 @@
 
 namespace introspect {
 
 	class abstractToJson {
 		/* Interface for things that can be turned into json */
 	public:
 		virtual std::string to_json() = 0;
+		virtual ~abstractToJson() {};
 	};
 
 	class abstractStructMember: public abstractToJson {
 		/* Interface for members of Structs */
 	public:
 		virtual std::string& getName() = 0;
 		virtual size_t getNumElements() = 0;
@@ -57,15 +57,14 @@
 		std::string name;
 		T* elements;
 		size_t count;
 		cType typeEnum;
 	public:
 		using type = T;
 		structMember(const cMember member):
-			abstractStructMember(),
 			name(member.name),
 			elements(),
 			count(member.elements),
 			typeEnum(member.type){
 			this->count = member.elements;
 			this->elements = new T[this->count];
 			std::memcpy(elements, member.value, sizeof(T)*this->count);
@@ -85,15 +84,15 @@
 	
 	class Struct: public abstractToJson{
 		std::string name;
 		std::vector<abstractStructMember*> elements;
 		int mavType;
 	public:
 		int getNumChildren() {return elements.size();}
-		int getType() {return mavType;}
+		uint8_t getType() {return mavType;}
 		std::string& getName() {return this->name;}
 		auto begin() {return this->elements.begin();}
 		auto end() {return this->elements.end();}
 		auto innerVector() {return elements;}
 		Struct(const cStruct * s):
 			name(s->name),
 			elements(),
```

### Comparing `UAVReaders-0.5.6/dataflash.cpp` & `UAVReaders-0.6.2/dataflash.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #include <ostream>
 #include <string>
+#include <cstdint>
 #include "dataflash.h"
 #include "table.h"
 
 #include <iostream>
 #include <iomanip>
 
 namespace DataFlash{
@@ -18,37 +19,37 @@
 		}
 		this->copy = packet;
 		this->current = description;
 		this->current.members = new cMember[description.numMembers];
 		for (int i = 0; i < current.numMembers; i++){
 			current.members[i] = description.members[i];
 			//bleh
-			long index = (long)description.members[i].value;
+			uint64_t index = (uintptr_t)description.members[i].value;
 			uint8_t * mem = copy.rest;
 			current.members[i].value = (void*)(mem + index);
 			/*				std::cerr << index
 							<< std::endl
 							<< &copy.rest
 							<< std::endl
 							<< current.members[i].value
 							<< std::endl<<std::endl;
-			*/
+			//*/
 			std::cerr.flush();
 		}
 			
 		return current;
 	}
 	void DFFormatDescription::releaseFormat() {
 		delete[] current.members;
 	}
 
 	bool DFFormatDescription::initialized = false;
 	cMember DFFormatDescription::dfMemberTypes[256] = {cMember{0,0,0,NONE}};
 	void DFFormatDescription::initialize() {
-		if (not DFFormatDescription::initialized){
+		if (! DFFormatDescription::initialized){
 			DFFormatDescription::initialized = true;
 			DFFormatDescription::dfMemberTypes['B'] = cMember{0, 0, 1, UINT8_T};
 			DFFormatDescription::dfMemberTypes['C'] = cMember{0, 0, 100, UINT16_T};
 			DFFormatDescription::dfMemberTypes['E'] = cMember{0, 0, 100, UINT32_T};
 			DFFormatDescription::dfMemberTypes['H'] = cMember{0, 0, 1, UINT16_T};
 			DFFormatDescription::dfMemberTypes['I'] = cMember{0, 0, 1, UINT32_T};
 			DFFormatDescription::dfMemberTypes['L'] = cMember{0, 0, 1, INT32_T};
@@ -79,25 +80,25 @@
 		if (this->formats[type] != nullptr) 
 			delete formats[type];
 		this->formats[type] = new DFFormatDescription(packet);
 		this->packetLengths[packet.type] = packet.len;
 	}
 	
 	bool DFParser::parseDataFlash(const uint8_t byte, DFPacket& packet) {
-		if (this->consumedCount == 0 and byte == DFParser::headerByte1) {
+		if (this->consumedCount == 0 && byte == DFParser::headerByte1) {
 			this->consumedCount = 1;
 			goto out;
 		}
 
-		else if (this->consumedCount == 1 and byte == DFParser::headerByte2){
+		else if (this->consumedCount == 1 && byte == DFParser::headerByte2){
 			this->consumedCount = 2;
 			goto out;
 		}
 
-		else if (this->consumedCount == 2 and byte == DFParser::idDescriptorPacketByte) {
+		else if (this->consumedCount == 2 && byte == DFParser::idDescriptorPacketByte) {
 			// the packet is a format descriptor
 			this->totalSize = DFParser::idDescriptorPacketLen;
 			this->consumedCount = 3;
 			this->isDescriptor = true;
 			packet.packet_type = DFParser::idDescriptorPacketByte;
 			goto out;
 		}
@@ -106,41 +107,41 @@
 			// some other packet type
 			this->consumedCount = 3;
 			packet.packet_type = byte;
 			this->totalSize = this->packetLengths[byte];
 			goto out;
 		}
 
-		else if (this->consumedCount >= 3 and this->consumedCount < (this->totalSize-1)) {
+		else if (this->consumedCount >= 3 && this->consumedCount < (this->totalSize-1)) {
 			// Bytes of the packet body
 			packet.rest[this->consumedCount - 3] = byte;
 			this->consumedCount++;
 			goto out;
 		}
 
-		else if (this->consumedCount >= 3 and this->consumedCount == (this->totalSize-1)) {
+		else if (this->consumedCount >= 3 && this->consumedCount == (this->totalSize-1)) {
 			/// Last byte in the packet
-			if (not this->isDescriptor) {
+			if (! this->isDescriptor) {
 				packet.rest[this->consumedCount - 3] = byte;
 				this->zero();
 				return true;
 			}
 
 			// The parser does not emit format packets, just keeps them for itself.
-			else { 
+			else {
 				packet.rest[this->consumedCount - 3] = byte;
 				const DFDescriptionPacket format = reinterpret_cast<DFDescriptionPacket&>(packet);
 				this->newFormat(format);
-				/*				std::cerr << "defined packet 0x"
+				/*std::cerr << "defined packet 0x"
 						  << std::setfill('0')
 						  << std::setw(2)
 						  << std::hex
 						  <<(int)this->formats[format.type]->packet_type
-						  << std::endl;*/
-									
+						  << std::endl;
+				*/					
 			}
 		}
 		
 		this->zero();
 	out:
 		return false;
 	}
```

### Comparing `UAVReaders-0.5.6/dataflash.h` & `UAVReaders-0.6.2/dataflash.h`

 * *Files 3% similar despite different names*

```diff
@@ -7,42 +7,45 @@
  *************************************************/
 
 #pragma once
 
 #include <cstdint>
 #include <queue>
 #include <cstring>
+#include <iostream>
 
 extern "C"{
 #include "table.h"
 }
 
 #define LEN_NAME 4
 #define LEN_FMT_STR 16
 #define LEN_LABELS 64
 
 namespace DataFlash{
 
+#pragma pack(push, 1)
 	extern "C"{
-		struct __attribute__((packed)) DFPacket {
+		struct DFPacket {
 			uint16_t begin;
 			uint8_t packet_type;
 			uint8_t rest[253];
 		};
 
-		struct __attribute__((packed)) DFDescriptionPacket{
+		struct DFDescriptionPacket{
 			uint16_t begin;
 			uint8_t packet_type;
 			uint8_t type;
 			uint8_t len;
 			char name[LEN_NAME];
 			char fmt_string[LEN_FMT_STR];
 			char labels[LEN_LABELS];
 		};
 	}
+#pragma pack(pop)
 
 	class DFFormatDescription {
 		static bool initialized;
 		static void initialize();
 		static cMember dfMemberTypes[256];
 		char name[LEN_NAME + 1];
 		char fields[LEN_LABELS + 1];
@@ -68,25 +71,26 @@
 			name[LEN_NAME] = 0;
 			fields[LEN_LABELS] = 0;
 			std::memcpy(name, format.name, LEN_NAME * sizeof(char));
 			std::memcpy(fields, format.labels, LEN_LABELS * sizeof(char));
 
 			std::queue<char*> fieldNames;
 			fieldNames.push(fields);
-			for (int i = 0; i < LEN_LABELS and fields[i] != 0; i++) {
+			for (int i = 0; i < LEN_LABELS && fields[i] != 0; i++) {
 				if (fields[i] == ',') {
 					fields[i] = 0;
 					fieldNames.push(fields + i + 1);
 				}
 			}
  
 			description.numMembers = 0;
 			description.name = name;
+			std::cerr << name << " ->\n";
 			/* intentionally empty */
-			for (; description.numMembers < LEN_FMT_STR and
+			for (; description.numMembers < LEN_FMT_STR &&
 					 format.fmt_string[description.numMembers] != 0;
 				 description.numMembers++);
 			description.members = new cMember[description.numMembers];
 
 			long offset = 0;
 			for (int i = 0; i < description.numMembers; i++) {
 				char format_type = format.fmt_string[i];
```

### Comparing `UAVReaders-0.5.6/mavlink/ASLUAV/ASLUAV.h` & `UAVReaders-0.6.2/mavlink/ASLUAV/ASLUAV.h`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_ASLUAV_H
 #define MAVLINK_ASLUAV_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_ASLUAV.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_ASLUAV_XML_HASH -6921207667047634836
+#define MAVLINK_ASLUAV_XML_HASH -346159300409528103
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink.h` & `UAVReaders-0.6.2/mavlink/AVSSUAS/mavlink.h`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 /** @file
- *  @brief MAVLink comm protocol built from ASLUAV.xml
+ *  @brief MAVLink comm protocol built from AVSSUAS.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH -6921207667047634836
+#define MAVLINK_PRIMARY_XML_HASH -3996619319064959883
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
@@ -25,10 +25,10 @@
 #endif
 
 #ifndef MAVLINK_COMMAND_24BIT
 #define MAVLINK_COMMAND_24BIT 1
 #endif
 
 #include "version.h"
-#include "ASLUAV.h"
+#include "AVSSUAS.h"
 
 #endif // MAVLINK_H
```

### Comparing `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_asl_obctrl.h` & `UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_asl_obctrl.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_aslctrl_data.h` & `UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_aslctrl_data.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_aslctrl_debug.h` & `UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_aslctrl_debug.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_asluav_status.h` & `UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_asluav_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_command_int_stamped.h` & `UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_command_int_stamped.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_command_long_stamped.h` & `UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_command_long_stamped.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_ekf_ext.h` & `UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_ekf_ext.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_fw_soaring_data.h` & `UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_fw_soaring_data.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_gsm_link_status.h` & `UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_gsm_link_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_satcom_link_status.h` & `UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_satcom_link_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sens_atmos.h` & `UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_sens_atmos.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sens_batmon.h` & `UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_sens_batmon.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sens_mppt.h` & `UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_sens_mppt.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sens_power.h` & `UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_sens_power.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sens_power_board.h` & `UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_sens_power_board.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sensor_airflow_angles.h` & `UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_sensor_airflow_angles.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sensorpod_status.h` & `UAVReaders-0.6.2/mavlink/ASLUAV/mavlink_msg_sensorpod_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ASLUAV/testsuite.h` & `UAVReaders-0.6.2/mavlink/ASLUAV/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/AVSSUAS/AVSSUAS.h` & `UAVReaders-0.6.2/mavlink/AVSSUAS/AVSSUAS.h`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_AVSSUAS_H
 #define MAVLINK_AVSSUAS_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_AVSSUAS.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_AVSSUAS_XML_HASH 2697101801489672959
+#define MAVLINK_AVSSUAS_XML_HASH -3996619319064959883
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.6/mavlink/AVSSUAS/mavlink.h` & `UAVReaders-0.6.2/mavlink/ASLUAV/mavlink.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 /** @file
- *  @brief MAVLink comm protocol built from AVSSUAS.xml
+ *  @brief MAVLink comm protocol built from ASLUAV.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH 2697101801489672959
+#define MAVLINK_PRIMARY_XML_HASH -346159300409528103
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
@@ -25,10 +25,10 @@
 #endif
 
 #ifndef MAVLINK_COMMAND_24BIT
 #define MAVLINK_COMMAND_24BIT 1
 #endif
 
 #include "version.h"
-#include "AVSSUAS.h"
+#include "ASLUAV.h"
 
 #endif // MAVLINK_H
```

### Comparing `UAVReaders-0.5.6/mavlink/AVSSUAS/mavlink_msg_avss_drone_imu.h` & `UAVReaders-0.6.2/mavlink/AVSSUAS/mavlink_msg_avss_drone_imu.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/AVSSUAS/mavlink_msg_avss_drone_operation_mode.h` & `UAVReaders-0.6.2/mavlink/AVSSUAS/mavlink_msg_avss_drone_operation_mode.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/AVSSUAS/mavlink_msg_avss_drone_position.h` & `UAVReaders-0.6.2/mavlink/AVSSUAS/mavlink_msg_avss_drone_position.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/AVSSUAS/mavlink_msg_avss_prs_sys_status.h` & `UAVReaders-0.6.2/mavlink/AVSSUAS/mavlink_msg_avss_prs_sys_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/AVSSUAS/testsuite.h` & `UAVReaders-0.6.2/mavlink/AVSSUAS/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/all/all.h` & `UAVReaders-0.6.2/mavlink/all/all.h`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_ALL_H
 #define MAVLINK_ALL_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_ALL.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_ALL_XML_HASH 176630288810012530
+#define MAVLINK_ALL_XML_HASH -2541766989881147069
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.6/mavlink/all/mavlink.h` & `UAVReaders-0.6.2/mavlink/development/mavlink.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 /** @file
- *  @brief MAVLink comm protocol built from all.xml
+ *  @brief MAVLink comm protocol built from development.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH 176630288810012530
+#define MAVLINK_PRIMARY_XML_HASH -7096509658459095623
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
@@ -25,10 +25,10 @@
 #endif
 
 #ifndef MAVLINK_COMMAND_24BIT
 #define MAVLINK_COMMAND_24BIT 1
 #endif
 
 #include "version.h"
-#include "all.h"
+#include "development.h"
 
 #endif // MAVLINK_H
```

### Comparing `UAVReaders-0.5.6/mavlink/all/testsuite.h` & `UAVReaders-0.6.2/mavlink/all/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/ardupilotmega.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/ardupilotmega.h`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_ARDUPILOTMEGA_H
 #define MAVLINK_ARDUPILOTMEGA_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_ARDUPILOTMEGA.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_ARDUPILOTMEGA_XML_HASH -6398486276474170115
+#define MAVLINK_ARDUPILOTMEGA_XML_HASH 3954163363249922604
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink.h` & `UAVReaders-0.6.2/mavlink/all/mavlink.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 /** @file
- *  @brief MAVLink comm protocol built from ardupilotmega.xml
+ *  @brief MAVLink comm protocol built from all.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH -6398486276474170115
+#define MAVLINK_PRIMARY_XML_HASH -2541766989881147069
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
@@ -25,10 +25,10 @@
 #endif
 
 #ifndef MAVLINK_COMMAND_24BIT
 #define MAVLINK_COMMAND_24BIT 1
 #endif
 
 #include "version.h"
-#include "ardupilotmega.h"
+#include "all.h"
 
 #endif // MAVLINK_H
```

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_adap_tuning.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_adap_tuning.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_ahrs.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_ahrs.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_ahrs2.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_ahrs2.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_ahrs3.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_ahrs3.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_airspeed_autocal.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_airspeed_autocal.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_aoa_ssa.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_aoa_ssa.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_ap_adc.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_ap_adc.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_autopilot_version_request.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_autopilot_version_request.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_battery2.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_battery2.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_camera_feedback.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_camera_feedback.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_camera_status.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_camera_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_compassmot_status.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_compassmot_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_data16.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_data16.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_data32.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_data32.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_data64.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_data64.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_data96.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_data96.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_deepstall.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_deepstall.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_device_op_read.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_device_op_read.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_device_op_read_reply.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_device_op_read_reply.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_device_op_write.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_device_op_write.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_device_op_write_reply.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_device_op_write_reply.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_digicam_configure.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_digicam_configure.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_digicam_control.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_digicam_control.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_ekf_status_report.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_ekf_status_report.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_esc_telemetry_1_to_4.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_esc_telemetry_1_to_4.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_esc_telemetry_5_to_8.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_esc_telemetry_5_to_8.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_esc_telemetry_9_to_12.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_esc_telemetry_9_to_12.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_fence_fetch_point.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_fence_fetch_point.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_fence_point.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_fence_point.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gimbal_control.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_gimbal_control.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gimbal_report.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_gimbal_report.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gimbal_torque_cmd_report.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_gimbal_torque_cmd_report.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gopro_get_request.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_gopro_get_request.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gopro_get_response.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_gopro_get_response.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gopro_heartbeat.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_gopro_heartbeat.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gopro_set_request.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_gopro_set_request.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gopro_set_response.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_gopro_set_response.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_hwstatus.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_hwstatus.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_led_control.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_led_control.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_limits_status.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_limits_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_mag_cal_progress.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_mag_cal_progress.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_mcu_status.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_mcu_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_meminfo.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_meminfo.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_mount_configure.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_mount_configure.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_mount_control.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_mount_control.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_mount_status.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_mount_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_obstacle_distance_3d.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_obstacle_distance_3d.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_osd_param_config.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_osd_param_config.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_osd_param_config_reply.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_osd_param_config_reply.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_osd_param_show_config.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_osd_param_show_config.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_osd_param_show_config_reply.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_osd_param_show_config_reply.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_pid_tuning.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_pid_tuning.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_radio.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_radio.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_rally_fetch_point.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_rally_fetch_point.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_rally_point.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_rally_point.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_rangefinder.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_rangefinder.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_remote_log_block_status.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_remote_log_block_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_remote_log_data_block.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_remote_log_data_block.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_rpm.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_rpm.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_sensor_offsets.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_sensor_offsets.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_set_mag_offsets.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_set_mag_offsets.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_simstate.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_simstate.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_vision_position_delta.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_vision_position_delta.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_water_depth.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_water_depth.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_wind.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink_msg_wind.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ardupilotmega/testsuite.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/checksum.h` & `UAVReaders-0.6.2/mavlink/checksum.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/common.h` & `UAVReaders-0.6.2/mavlink/common/common.h`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_COMMON_H
 #define MAVLINK_COMMON_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_COMMON.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_COMMON_XML_HASH 5515211591480474682
+#define MAVLINK_COMMON_XML_HASH -2648244614670464807
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink.h` & `UAVReaders-0.6.2/mavlink/icarous/mavlink.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 /** @file
- *  @brief MAVLink comm protocol built from common.xml
+ *  @brief MAVLink comm protocol built from icarous.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH 5515211591480474682
+#define MAVLINK_PRIMARY_XML_HASH -2439300828852534093
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
@@ -25,10 +25,10 @@
 #endif
 
 #ifndef MAVLINK_COMMAND_24BIT
 #define MAVLINK_COMMAND_24BIT 1
 #endif
 
 #include "version.h"
-#include "common.h"
+#include "icarous.h"
 
 #endif // MAVLINK_H
```

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_actuator_control_target.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_actuator_control_target.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_actuator_output_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_actuator_output_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_adsb_vehicle.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_adsb_vehicle.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_ais_vessel.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_ais_vessel.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_altitude.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_altitude.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_att_pos_mocap.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_att_pos_mocap.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_attitude.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_attitude.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_attitude_quaternion.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_attitude_quaternion.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_attitude_quaternion_cov.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_attitude_quaternion_cov.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_attitude_target.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_attitude_target.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_auth_key.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_auth_key.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_autopilot_state_for_gimbal_device.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_autopilot_state_for_gimbal_device.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_autopilot_version.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_autopilot_version.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_battery_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_battery_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_button_change.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_button_change.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_capture_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_camera_capture_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_fov_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_camera_fov_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_image_captured.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_camera_image_captured.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_information.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_camera_information.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_settings.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_camera_settings.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_tracking_geo_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_camera_tracking_geo_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_tracking_image_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_camera_tracking_image_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_trigger.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_camera_trigger.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_can_filter_modify.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_can_filter_modify.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_can_frame.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_can_frame.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_canfd_frame.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_canfd_frame.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_cellular_config.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_cellular_config.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_cellular_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_cellular_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_change_operator_control.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_change_operator_control.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_change_operator_control_ack.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_change_operator_control_ack.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_collision.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_collision.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_command_ack.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_command_ack.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_command_cancel.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_command_cancel.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_command_int.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_command_int.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_command_long.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_command_long.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_component_information.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_component_information.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_component_metadata.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_component_metadata.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_control_system_state.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_control_system_state.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_current_event_sequence.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_current_event_sequence.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_data_stream.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_data_stream.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_data_transmission_handshake.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_data_transmission_handshake.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_debug.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_debug.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_debug_float_array.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_debug_float_array.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_debug_vect.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_debug_vect.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_distance_sensor.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_distance_sensor.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_efi_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_efi_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_encapsulated_data.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_encapsulated_data.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_esc_info.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_esc_info.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_esc_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_esc_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_estimator_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_estimator_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_event.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_event.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_extended_sys_state.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_extended_sys_state.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_fence_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_fence_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_file_transfer_protocol.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_file_transfer_protocol.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_flight_information.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_flight_information.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_follow_target.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_follow_target.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_generator_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_generator_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_device_attitude_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_gimbal_device_attitude_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_device_information.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_gimbal_device_information.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_device_set_attitude.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_gimbal_device_set_attitude.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_manager_information.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_gimbal_manager_information.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_manager_set_attitude.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_gimbal_manager_set_attitude.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_manager_set_manual_control.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_gimbal_manager_set_manual_control.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_manager_set_pitchyaw.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_gimbal_manager_set_pitchyaw.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_manager_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_gimbal_manager_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_global_position_int.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_global_position_int.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_global_position_int_cov.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_global_position_int_cov.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_global_vision_position_estimate.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_global_vision_position_estimate.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps2_raw.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_gps2_raw.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps2_rtk.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_gps2_rtk.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_global_origin.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_gps_global_origin.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_inject_data.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_gps_inject_data.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_input.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_gps_input.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_raw_int.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_gps_raw_int.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_rtcm_data.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_gps_rtcm_data.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_rtk.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_gps_rtk.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_gps_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_high_latency.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_high_latency.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_high_latency2.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_high_latency2.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_highres_imu.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_highres_imu.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_actuator_controls.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_hil_actuator_controls.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_controls.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_hil_controls.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_gps.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_hil_gps.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_optical_flow.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_hil_optical_flow.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_rc_inputs_raw.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_hil_rc_inputs_raw.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_sensor.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_hil_sensor.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_state.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_hil_state.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_state_quaternion.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_hil_state_quaternion.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_home_position.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_home_position.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_hygrometer_sensor.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_hygrometer_sensor.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_isbd_link_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_isbd_link_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_landing_target.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_landing_target.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_link_node_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_link_node_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_local_position_ned.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_local_position_ned.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_local_position_ned_cov.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_local_position_ned_cov.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_local_position_ned_system_global_offset.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_local_position_ned_system_global_offset.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_log_data.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_log_data.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_log_entry.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_log_entry.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_log_erase.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_log_erase.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_log_request_data.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_log_request_data.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_log_request_end.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_log_request_end.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_log_request_list.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_log_request_list.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_logging_ack.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_logging_ack.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_logging_data.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_logging_data.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_logging_data_acked.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_logging_data_acked.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mag_cal_report.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_mag_cal_report.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_manual_control.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_manual_control.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_manual_setpoint.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_manual_setpoint.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_memory_vect.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_memory_vect.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_message_interval.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_message_interval.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_ack.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_ack.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_clear_all.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_clear_all.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_count.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_count.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_current.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_current.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_item.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_item.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_item_int.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_item_int.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_item_reached.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_item_reached.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_request.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_request.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_request_int.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_request_int.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_request_list.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_request_list.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_request_partial_list.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_request_partial_list.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_set_current.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_set_current.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_write_partial_list.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_mission_write_partial_list.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mount_orientation.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_mount_orientation.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_named_value_float.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_named_value_float.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_named_value_int.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_named_value_int.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_nav_controller_output.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_nav_controller_output.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_obstacle_distance.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_obstacle_distance.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_odometry.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_odometry.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_onboard_computer_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_onboard_computer_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_arm_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_open_drone_id_arm_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_authentication.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_open_drone_id_authentication.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_basic_id.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_open_drone_id_basic_id.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_location.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_open_drone_id_location.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_message_pack.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_open_drone_id_message_pack.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_operator_id.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_open_drone_id_operator_id.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_self_id.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_open_drone_id_self_id.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_system.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_open_drone_id_system.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_system_update.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_open_drone_id_system_update.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_optical_flow.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_optical_flow.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_optical_flow_rad.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_optical_flow_rad.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_orbit_execution_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_orbit_execution_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_ext_ack.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_param_ext_ack.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_ext_request_list.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_param_ext_request_list.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_ext_request_read.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_param_ext_request_read.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_ext_set.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_param_ext_set.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_ext_value.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_param_ext_value.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_map_rc.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_param_map_rc.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_request_list.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_param_request_list.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_request_read.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_param_request_read.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_set.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_param_set.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_value.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_param_value.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_ping.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_ping.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_play_tune.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_play_tune.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_play_tune_v2.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_play_tune_v2.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_position_target_global_int.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_position_target_global_int.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_position_target_local_ned.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_position_target_local_ned.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_power_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_power_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_radio_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_radio_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_raw_imu.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_raw_imu.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_raw_pressure.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_raw_pressure.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_raw_rpm.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_raw_rpm.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_rc_channels.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_rc_channels.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_rc_channels_override.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_rc_channels_override.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_rc_channels_raw.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_rc_channels_raw.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_rc_channels_scaled.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_rc_channels_scaled.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_request_data_stream.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_request_data_stream.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_request_event.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_request_event.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_resource_request.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_resource_request.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_response_event_error.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_response_event_error.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_safety_allowed_area.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_safety_allowed_area.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_safety_set_allowed_area.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_safety_set_allowed_area.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_scaled_imu.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_scaled_imu.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_scaled_imu2.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_scaled_imu2.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_scaled_imu3.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_scaled_imu3.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_scaled_pressure.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_scaled_pressure.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_scaled_pressure2.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_scaled_pressure2.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_scaled_pressure3.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_scaled_pressure3.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_serial_control.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_serial_control.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_servo_output_raw.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_servo_output_raw.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_actuator_control_target.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_set_actuator_control_target.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_attitude_target.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_set_attitude_target.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_gps_global_origin.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_set_gps_global_origin.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_home_position.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_set_home_position.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_mode.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_set_mode.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_position_target_global_int.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_set_position_target_global_int.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_position_target_local_ned.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_set_position_target_local_ned.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_setup_signing.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_setup_signing.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_sim_state.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_sim_state.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_smart_battery_info.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_smart_battery_info.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_statustext.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_statustext.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_storage_information.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_storage_information.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_supported_tunes.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_supported_tunes.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_sys_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_sys_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_system_time.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_system_time.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_terrain_check.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_terrain_check.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_terrain_data.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_terrain_data.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_terrain_report.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_terrain_report.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_terrain_request.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_terrain_request.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_time_estimate_to_target.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_time_estimate_to_target.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_timesync.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_timesync.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_trajectory_representation_bezier.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_trajectory_representation_bezier.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_trajectory_representation_waypoints.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_trajectory_representation_waypoints.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_tunnel.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_tunnel.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_uavcan_node_info.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_uavcan_node_info.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_uavcan_node_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_uavcan_node_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_utm_global_position.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_utm_global_position.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_v2_extension.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_v2_extension.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_vfr_hud.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_vfr_hud.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_vibration.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_vibration.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_vicon_position_estimate.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_vicon_position_estimate.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_video_stream_information.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_video_stream_information.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_video_stream_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_video_stream_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_vision_position_estimate.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_vision_position_estimate.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_vision_speed_estimate.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_vision_speed_estimate.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_wheel_distance.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_wheel_distance.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_wifi_config_ap.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_wifi_config_ap.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_winch_status.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_winch_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/mavlink_msg_wind_cov.h` & `UAVReaders-0.6.2/mavlink/common/mavlink_msg_wind_cov.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/common/testsuite.h` & `UAVReaders-0.6.2/mavlink/common/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/cubepilot/cubepilot.h` & `UAVReaders-0.6.2/mavlink/cubepilot/cubepilot.h`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_CUBEPILOT_H
 #define MAVLINK_CUBEPILOT_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_CUBEPILOT.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_CUBEPILOT_XML_HASH 4348068059622669928
+#define MAVLINK_CUBEPILOT_XML_HASH 1462442922816866458
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.6/mavlink/cubepilot/mavlink.h` & `UAVReaders-0.6.2/mavlink/cubepilot/mavlink.h`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  *  @brief MAVLink comm protocol built from cubepilot.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH 4348068059622669928
+#define MAVLINK_PRIMARY_XML_HASH 1462442922816866458
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
```

### Comparing `UAVReaders-0.5.6/mavlink/cubepilot/mavlink_msg_cubepilot_firmware_update_resp.h` & `UAVReaders-0.6.2/mavlink/cubepilot/mavlink_msg_cubepilot_firmware_update_resp.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/cubepilot/mavlink_msg_cubepilot_firmware_update_start.h` & `UAVReaders-0.6.2/mavlink/cubepilot/mavlink_msg_cubepilot_firmware_update_start.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/cubepilot/mavlink_msg_cubepilot_raw_rc.h` & `UAVReaders-0.6.2/mavlink/cubepilot/mavlink_msg_cubepilot_raw_rc.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/cubepilot/mavlink_msg_herelink_telem.h` & `UAVReaders-0.6.2/mavlink/cubepilot/mavlink_msg_herelink_telem.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/cubepilot/mavlink_msg_herelink_video_stream_information.h` & `UAVReaders-0.6.2/mavlink/cubepilot/mavlink_msg_herelink_video_stream_information.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/cubepilot/testsuite.h` & `UAVReaders-0.6.2/mavlink/cubepilot/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/development/development.h` & `UAVReaders-0.6.2/mavlink/development/development.h`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_DEVELOPMENT_H
 #define MAVLINK_DEVELOPMENT_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_DEVELOPMENT.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_DEVELOPMENT_XML_HASH -4303497761705237489
+#define MAVLINK_DEVELOPMENT_XML_HASH -7096509658459095623
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.6/mavlink/development/mavlink.h` & `UAVReaders-0.6.2/mavlink/common/mavlink.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 /** @file
- *  @brief MAVLink comm protocol built from development.xml
+ *  @brief MAVLink comm protocol built from common.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH -4303497761705237489
+#define MAVLINK_PRIMARY_XML_HASH -2648244614670464807
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
@@ -25,10 +25,10 @@
 #endif
 
 #ifndef MAVLINK_COMMAND_24BIT
 #define MAVLINK_COMMAND_24BIT 1
 #endif
 
 #include "version.h"
-#include "development.h"
+#include "common.h"
 
 #endif // MAVLINK_H
```

### Comparing `UAVReaders-0.5.6/mavlink/development/mavlink_msg_airspeed.h` & `UAVReaders-0.6.2/mavlink/development/mavlink_msg_airspeed.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/development/mavlink_msg_available_modes.h` & `UAVReaders-0.6.2/mavlink/development/mavlink_msg_available_modes.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/development/mavlink_msg_battery_status_v2.h` & `UAVReaders-0.6.2/mavlink/development/mavlink_msg_battery_status_v2.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/development/mavlink_msg_component_information_basic.h` & `UAVReaders-0.6.2/mavlink/development/mavlink_msg_component_information_basic.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/development/mavlink_msg_current_mode.h` & `UAVReaders-0.6.2/mavlink/development/mavlink_msg_current_mode.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/development/mavlink_msg_figure_eight_execution_status.h` & `UAVReaders-0.6.2/mavlink/development/mavlink_msg_figure_eight_execution_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/development/mavlink_msg_group_end.h` & `UAVReaders-0.6.2/mavlink/development/mavlink_msg_group_end.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/development/mavlink_msg_group_start.h` & `UAVReaders-0.6.2/mavlink/development/mavlink_msg_group_start.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/development/mavlink_msg_mission_checksum.h` & `UAVReaders-0.6.2/mavlink/development/mavlink_msg_mission_checksum.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/development/mavlink_msg_param_ack_transaction.h` & `UAVReaders-0.6.2/mavlink/development/mavlink_msg_param_ack_transaction.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/development/mavlink_msg_target_absolute.h` & `UAVReaders-0.6.2/mavlink/development/mavlink_msg_target_absolute.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/development/mavlink_msg_target_relative.h` & `UAVReaders-0.6.2/mavlink/development/mavlink_msg_target_relative.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/development/mavlink_msg_wifi_network_info.h` & `UAVReaders-0.6.2/mavlink/development/mavlink_msg_wifi_network_info.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/development/testsuite.h` & `UAVReaders-0.6.2/mavlink/development/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/icarous/icarous.h` & `UAVReaders-0.6.2/mavlink/icarous/icarous.h`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_ICAROUS_H
 #define MAVLINK_ICAROUS_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_ICAROUS.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_ICAROUS_XML_HASH 2245595000028289331
+#define MAVLINK_ICAROUS_XML_HASH -2439300828852534093
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.6/mavlink/icarous/mavlink.h` & `UAVReaders-0.6.2/mavlink/storm32/mavlink.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 /** @file
- *  @brief MAVLink comm protocol built from icarous.xml
+ *  @brief MAVLink comm protocol built from storm32.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH 2245595000028289331
+#define MAVLINK_PRIMARY_XML_HASH -7966875315739443268
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
@@ -25,10 +25,10 @@
 #endif
 
 #ifndef MAVLINK_COMMAND_24BIT
 #define MAVLINK_COMMAND_24BIT 1
 #endif
 
 #include "version.h"
-#include "icarous.h"
+#include "storm32.h"
 
 #endif // MAVLINK_H
```

### Comparing `UAVReaders-0.5.6/mavlink/icarous/mavlink_msg_icarous_heartbeat.h` & `UAVReaders-0.6.2/mavlink/icarous/mavlink_msg_icarous_heartbeat.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/icarous/mavlink_msg_icarous_kinematic_bands.h` & `UAVReaders-0.6.2/mavlink/icarous/mavlink_msg_icarous_kinematic_bands.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/icarous/testsuite.h` & `UAVReaders-0.6.2/mavlink/icarous/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/mavlink_conversions.h` & `UAVReaders-0.6.2/mavlink/mavlink_conversions.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/mavlink_get_info.h` & `UAVReaders-0.6.2/mavlink/mavlink_get_info.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/mavlink_helpers.h` & `UAVReaders-0.6.2/mavlink/mavlink_helpers.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/mavlink_sha256.h` & `UAVReaders-0.6.2/mavlink/mavlink_sha256.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/mavlink_types.h` & `UAVReaders-0.6.2/mavlink/mavlink_types.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/minimal/mavlink.h` & `UAVReaders-0.6.2/mavlink/minimal/mavlink.h`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  *  @brief MAVLink comm protocol built from minimal.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH -8787493283418306967
+#define MAVLINK_PRIMARY_XML_HASH -953340554165526151
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
```

### Comparing `UAVReaders-0.5.6/mavlink/minimal/mavlink_msg_heartbeat.h` & `UAVReaders-0.6.2/mavlink/minimal/mavlink_msg_heartbeat.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/minimal/mavlink_msg_protocol_version.h` & `UAVReaders-0.6.2/mavlink/minimal/mavlink_msg_protocol_version.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/minimal/minimal.h` & `UAVReaders-0.6.2/mavlink/minimal/minimal.h`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_MINIMAL_H
 #define MAVLINK_MINIMAL_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_MINIMAL.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_MINIMAL_XML_HASH -8787493283418306967
+#define MAVLINK_MINIMAL_XML_HASH -953340554165526151
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.6/mavlink/minimal/testsuite.h` & `UAVReaders-0.6.2/mavlink/minimal/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/protocol.h` & `UAVReaders-0.6.2/mavlink/protocol.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/python_array_test/mavlink.h` & `UAVReaders-0.6.2/mavlink/python_array_test/mavlink.h`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  *  @brief MAVLink comm protocol built from python_array_test.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH 1341603429249984703
+#define MAVLINK_PRIMARY_XML_HASH -8662182371111149576
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
```

### Comparing `UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_0.h` & `UAVReaders-0.6.2/mavlink/python_array_test/mavlink_msg_array_test_0.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_1.h` & `UAVReaders-0.6.2/mavlink/python_array_test/mavlink_msg_array_test_1.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_3.h` & `UAVReaders-0.6.2/mavlink/python_array_test/mavlink_msg_array_test_3.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_4.h` & `UAVReaders-0.6.2/mavlink/python_array_test/mavlink_msg_array_test_4.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_5.h` & `UAVReaders-0.6.2/mavlink/python_array_test/mavlink_msg_array_test_5.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_6.h` & `UAVReaders-0.6.2/mavlink/python_array_test/mavlink_msg_array_test_6.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_7.h` & `UAVReaders-0.6.2/mavlink/python_array_test/mavlink_msg_array_test_7.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_8.h` & `UAVReaders-0.6.2/mavlink/python_array_test/mavlink_msg_array_test_8.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/python_array_test/python_array_test.h` & `UAVReaders-0.6.2/mavlink/python_array_test/python_array_test.h`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_PYTHON_ARRAY_TEST_H
 #define MAVLINK_PYTHON_ARRAY_TEST_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_PYTHON_ARRAY_TEST.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_PYTHON_ARRAY_TEST_XML_HASH 1341603429249984703
+#define MAVLINK_PYTHON_ARRAY_TEST_XML_HASH -8662182371111149576
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.6/mavlink/python_array_test/testsuite.h` & `UAVReaders-0.6.2/mavlink/python_array_test/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/standard/mavlink.h` & `UAVReaders-0.6.2/mavlink/standard/mavlink.h`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  *  @brief MAVLink comm protocol built from standard.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH -8068599972875758283
+#define MAVLINK_PRIMARY_XML_HASH -581617275612289036
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
```

### Comparing `UAVReaders-0.5.6/mavlink/standard/standard.h` & `UAVReaders-0.6.2/mavlink/standard/standard.h`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_STANDARD_H
 #define MAVLINK_STANDARD_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_STANDARD.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_STANDARD_XML_HASH -8068599972875758283
+#define MAVLINK_STANDARD_XML_HASH -581617275612289036
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.6/mavlink/standard/testsuite.h` & `UAVReaders-0.6.2/mavlink/standard/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/storm32/mavlink.h` & `UAVReaders-0.6.2/mavlink/ualberta/mavlink.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 /** @file
- *  @brief MAVLink comm protocol built from storm32.xml
+ *  @brief MAVLink comm protocol built from ualberta.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH -4905212276485218532
+#define MAVLINK_PRIMARY_XML_HASH 4100829363721598037
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
@@ -25,10 +25,10 @@
 #endif
 
 #ifndef MAVLINK_COMMAND_24BIT
 #define MAVLINK_COMMAND_24BIT 1
 #endif
 
 #include "version.h"
-#include "storm32.h"
+#include "ualberta.h"
 
 #endif // MAVLINK_H
```

### Comparing `UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_frsky_passthrough_array.h` & `UAVReaders-0.6.2/mavlink/storm32/mavlink_msg_frsky_passthrough_array.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_param_value_array.h` & `UAVReaders-0.6.2/mavlink/storm32/mavlink_msg_param_value_array.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_qshot_status.h` & `UAVReaders-0.6.2/mavlink/storm32/mavlink_msg_qshot_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_radio_link_stats.h` & `UAVReaders-0.6.2/mavlink/storm32/mavlink_msg_radio_link_stats.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_radio_rc_channels.h` & `UAVReaders-0.6.2/mavlink/storm32/mavlink_msg_radio_rc_channels.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_control.h` & `UAVReaders-0.6.2/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_control.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_control_pitchyaw.h` & `UAVReaders-0.6.2/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_control_pitchyaw.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_correct_roll.h` & `UAVReaders-0.6.2/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_correct_roll.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_information.h` & `UAVReaders-0.6.2/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_information.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_status.h` & `UAVReaders-0.6.2/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/storm32/storm32.h` & `UAVReaders-0.6.2/mavlink/storm32/storm32.h`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_STORM32_H
 #define MAVLINK_STORM32_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_STORM32.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_STORM32_XML_HASH -4905212276485218532
+#define MAVLINK_STORM32_XML_HASH -7966875315739443268
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.6/mavlink/storm32/testsuite.h` & `UAVReaders-0.6.2/mavlink/storm32/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/test/mavlink.h` & `UAVReaders-0.6.2/mavlink/test/mavlink.h`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  *  @brief MAVLink comm protocol built from test.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH -5416981559095984788
+#define MAVLINK_PRIMARY_XML_HASH 4927255601471392237
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
```

### Comparing `UAVReaders-0.5.6/mavlink/test/mavlink_msg_test_types.h` & `UAVReaders-0.6.2/mavlink/test/mavlink_msg_test_types.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/test/test.h` & `UAVReaders-0.6.2/mavlink/test/test.h`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_TEST_H
 #define MAVLINK_TEST_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_TEST.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_TEST_XML_HASH -5416981559095984788
+#define MAVLINK_TEST_XML_HASH 4927255601471392237
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.6/mavlink/test/testsuite.h` & `UAVReaders-0.6.2/mavlink/test/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/uAvionix/mavlink.h` & `UAVReaders-0.6.2/mavlink/ardupilotmega/mavlink.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 /** @file
- *  @brief MAVLink comm protocol built from uAvionix.xml
+ *  @brief MAVLink comm protocol built from ardupilotmega.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH -7924362279646143647
+#define MAVLINK_PRIMARY_XML_HASH 3954163363249922604
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
@@ -25,10 +25,10 @@
 #endif
 
 #ifndef MAVLINK_COMMAND_24BIT
 #define MAVLINK_COMMAND_24BIT 1
 #endif
 
 #include "version.h"
-#include "uAvionix.h"
+#include "ardupilotmega.h"
 
 #endif // MAVLINK_H
```

### Comparing `UAVReaders-0.5.6/mavlink/uAvionix/mavlink_msg_uavionix_adsb_out_cfg.h` & `UAVReaders-0.6.2/mavlink/uAvionix/mavlink_msg_uavionix_adsb_out_cfg.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/uAvionix/mavlink_msg_uavionix_adsb_out_dynamic.h` & `UAVReaders-0.6.2/mavlink/uAvionix/mavlink_msg_uavionix_adsb_out_dynamic.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/uAvionix/mavlink_msg_uavionix_adsb_transceiver_health_report.h` & `UAVReaders-0.6.2/mavlink/uAvionix/mavlink_msg_uavionix_adsb_transceiver_health_report.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/uAvionix/testsuite.h` & `UAVReaders-0.6.2/mavlink/uAvionix/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/uAvionix/uAvionix.h` & `UAVReaders-0.6.2/mavlink/uAvionix/uAvionix.h`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_UAVIONIX_H
 #define MAVLINK_UAVIONIX_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_UAVIONIX.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_UAVIONIX_XML_HASH -7924362279646143647
+#define MAVLINK_UAVIONIX_XML_HASH 4025664085865078695
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.6/mavlink/ualberta/mavlink.h` & `UAVReaders-0.6.2/mavlink/uAvionix/mavlink.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 /** @file
- *  @brief MAVLink comm protocol built from ualberta.xml
+ *  @brief MAVLink comm protocol built from uAvionix.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH -8458791220127004858
+#define MAVLINK_PRIMARY_XML_HASH 4025664085865078695
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
@@ -25,10 +25,10 @@
 #endif
 
 #ifndef MAVLINK_COMMAND_24BIT
 #define MAVLINK_COMMAND_24BIT 1
 #endif
 
 #include "version.h"
-#include "ualberta.h"
+#include "uAvionix.h"
 
 #endif // MAVLINK_H
```

### Comparing `UAVReaders-0.5.6/mavlink/ualberta/mavlink_msg_nav_filter_bias.h` & `UAVReaders-0.6.2/mavlink/ualberta/mavlink_msg_nav_filter_bias.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ualberta/mavlink_msg_radio_calibration.h` & `UAVReaders-0.6.2/mavlink/ualberta/mavlink_msg_radio_calibration.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ualberta/mavlink_msg_ualberta_sys_status.h` & `UAVReaders-0.6.2/mavlink/ualberta/mavlink_msg_ualberta_sys_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ualberta/testsuite.h` & `UAVReaders-0.6.2/mavlink/ualberta/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/mavlink/ualberta/ualberta.h` & `UAVReaders-0.6.2/mavlink/ualberta/ualberta.h`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_UALBERTA_H
 #define MAVLINK_UALBERTA_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_UALBERTA.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_UALBERTA_XML_HASH -8458791220127004858
+#define MAVLINK_UALBERTA_XML_HASH 4100829363721598037
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.6/mavlink_introspect_gen.c` & `UAVReaders-0.6.2/mavlink_introspect_gen.c`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,3022 +1,3181 @@
-#include "mavlink/ualberta/mavlink.h"
-#include "mavlink/development/mavlink.h"
-#include "mavlink/storm32/mavlink.h"
-#include "mavlink/icarous/mavlink.h"
-#include "mavlink/minimal/mavlink.h"
-#include "mavlink/ardupilotmega/mavlink.h"
-#include "mavlink/uAvionix/mavlink.h"
-#include "mavlink/AVSSUAS/mavlink.h"
-#include "mavlink/python_array_test/mavlink.h"
-#include "mavlink/ASLUAV/mavlink.h"
 #include "mavlink/common/mavlink.h"
+#include "mavlink/uAvionix/mavlink.h"
 #include "mavlink/cubepilot/mavlink.h"
+#include "mavlink/python_array_test/mavlink.h"
+#include "mavlink/ardupilotmega/mavlink.h"
+#include "mavlink/AVSSUAS/mavlink.h"
 #include "mavlink/test/mavlink.h"
-#include "mavlink/development/mavlink_msg_wifi_network_info.h"
-#include "mavlink/development/mavlink_msg_target_absolute.h"
-#include "mavlink/development/mavlink_msg_current_mode.h"
-#include "mavlink/development/mavlink_msg_battery_status_v2.h"
-#include "mavlink/development/mavlink_msg_group_start.h"
-#include "mavlink/development/mavlink_msg_figure_eight_execution_status.h"
-#include "mavlink/development/mavlink_msg_group_end.h"
-#include "mavlink/development/mavlink_msg_mission_checksum.h"
-#include "mavlink/development/mavlink_msg_target_relative.h"
-#include "mavlink/development/mavlink_msg_airspeed.h"
-#include "mavlink/development/mavlink_msg_param_ack_transaction.h"
-#include "mavlink/development/mavlink_msg_available_modes.h"
-#include "mavlink/development/mavlink_msg_component_information_basic.h"
-#include "mavlink/icarous/mavlink_msg_icarous_kinematic_bands.h"
-#include "mavlink/icarous/mavlink_msg_icarous_heartbeat.h"
-#include "mavlink/ASLUAV/mavlink_msg_sensor_airflow_angles.h"
-#include "mavlink/ASLUAV/mavlink_msg_aslctrl_debug.h"
-#include "mavlink/ASLUAV/mavlink_msg_sens_batmon.h"
-#include "mavlink/ASLUAV/mavlink_msg_asluav_status.h"
-#include "mavlink/ASLUAV/mavlink_msg_sens_power.h"
-#include "mavlink/ASLUAV/mavlink_msg_command_long_stamped.h"
+#include "mavlink/development/mavlink.h"
+#include "mavlink/minimal/mavlink.h"
+#include "mavlink/ASLUAV/mavlink.h"
+#include "mavlink/storm32/mavlink.h"
+#include "mavlink/icarous/mavlink.h"
+#include "mavlink/ualberta/mavlink.h"
+#include "mavlink/common/mavlink_msg_local_position_ned_system_global_offset.h"
+#include "mavlink/common/mavlink_msg_hil_actuator_controls.h"
+#include "mavlink/common/mavlink_msg_vision_speed_estimate.h"
+#include "mavlink/common/mavlink_msg_hil_rc_inputs_raw.h"
+#include "mavlink/common/mavlink_msg_log_request_data.h"
+#include "mavlink/common/mavlink_msg_hil_optical_flow.h"
+#include "mavlink/common/mavlink_msg_open_drone_id_message_pack.h"
+#include "mavlink/common/mavlink_msg_safety_set_allowed_area.h"
+#include "mavlink/common/mavlink_msg_play_tune_v2.h"
+#include "mavlink/common/mavlink_msg_follow_target.h"
+#include "mavlink/common/mavlink_msg_odometry.h"
+#include "mavlink/common/mavlink_msg_gps_rtk.h"
+#include "mavlink/common/mavlink_msg_winch_status.h"
+#include "mavlink/common/mavlink_msg_trajectory_representation_bezier.h"
+#include "mavlink/common/mavlink_msg_param_set.h"
+#include "mavlink/common/mavlink_msg_hil_gps.h"
+#include "mavlink/common/mavlink_msg_wifi_config_ap.h"
+#include "mavlink/common/mavlink_msg_vision_position_estimate.h"
+#include "mavlink/common/mavlink_msg_rc_channels.h"
+#include "mavlink/common/mavlink_msg_highres_imu.h"
+#include "mavlink/common/mavlink_msg_gimbal_device_attitude_status.h"
+#include "mavlink/common/mavlink_msg_autopilot_state_for_gimbal_device.h"
+#include "mavlink/common/mavlink_msg_fence_status.h"
+#include "mavlink/common/mavlink_msg_extended_sys_state.h"
+#include "mavlink/common/mavlink_msg_open_drone_id_operator_id.h"
+#include "mavlink/common/mavlink_msg_named_value_int.h"
+#include "mavlink/common/mavlink_msg_message_interval.h"
+#include "mavlink/common/mavlink_msg_param_ext_ack.h"
+#include "mavlink/common/mavlink_msg_param_ext_set.h"
+#include "mavlink/common/mavlink_msg_mag_cal_report.h"
+#include "mavlink/common/mavlink_msg_current_event_sequence.h"
+#include "mavlink/common/mavlink_msg_terrain_data.h"
+#include "mavlink/common/mavlink_msg_request_event.h"
+#include "mavlink/common/mavlink_msg_component_metadata.h"
+#include "mavlink/common/mavlink_msg_actuator_control_target.h"
+#include "mavlink/common/mavlink_msg_scaled_imu2.h"
+#include "mavlink/common/mavlink_msg_data_transmission_handshake.h"
+#include "mavlink/common/mavlink_msg_uavcan_node_info.h"
+#include "mavlink/common/mavlink_msg_param_ext_value.h"
+#include "mavlink/common/mavlink_msg_play_tune.h"
+#include "mavlink/common/mavlink_msg_cellular_status.h"
+#include "mavlink/common/mavlink_msg_logging_data_acked.h"
+#include "mavlink/common/mavlink_msg_gps2_raw.h"
+#include "mavlink/common/mavlink_msg_isbd_link_status.h"
+#include "mavlink/common/mavlink_msg_gimbal_manager_set_manual_control.h"
+#include "mavlink/common/mavlink_msg_camera_image_captured.h"
+#include "mavlink/common/mavlink_msg_component_information.h"
+#include "mavlink/common/mavlink_msg_control_system_state.h"
+#include "mavlink/common/mavlink_msg_cellular_config.h"
+#include "mavlink/common/mavlink_msg_uavcan_node_status.h"
+#include "mavlink/common/mavlink_msg_distance_sensor.h"
+#include "mavlink/common/mavlink_msg_param_ext_request_list.h"
+#include "mavlink/common/mavlink_msg_file_transfer_protocol.h"
+#include "mavlink/common/mavlink_msg_gimbal_manager_information.h"
+#include "mavlink/common/mavlink_msg_manual_control.h"
+#include "mavlink/common/mavlink_msg_setup_signing.h"
+#include "mavlink/common/mavlink_msg_statustext.h"
+#include "mavlink/common/mavlink_msg_command_cancel.h"
+#include "mavlink/common/mavlink_msg_esc_info.h"
+#include "mavlink/common/mavlink_msg_mission_set_current.h"
+#include "mavlink/common/mavlink_msg_utm_global_position.h"
+#include "mavlink/common/mavlink_msg_gimbal_manager_set_pitchyaw.h"
+#include "mavlink/common/mavlink_msg_power_status.h"
+#include "mavlink/common/mavlink_msg_param_request_read.h"
+#include "mavlink/common/mavlink_msg_camera_fov_status.h"
+#include "mavlink/common/mavlink_msg_mission_current.h"
+#include "mavlink/common/mavlink_msg_mount_orientation.h"
+#include "mavlink/common/mavlink_msg_attitude.h"
+#include "mavlink/common/mavlink_msg_hygrometer_sensor.h"
+#include "mavlink/common/mavlink_msg_terrain_report.h"
+#include "mavlink/common/mavlink_msg_hil_sensor.h"
+#include "mavlink/common/mavlink_msg_vibration.h"
+#include "mavlink/common/mavlink_msg_scaled_pressure3.h"
+#include "mavlink/common/mavlink_msg_change_operator_control_ack.h"
+#include "mavlink/common/mavlink_msg_v2_extension.h"
+#include "mavlink/common/mavlink_msg_event.h"
+#include "mavlink/common/mavlink_msg_video_stream_status.h"
+#include "mavlink/common/mavlink_msg_log_request_end.h"
+#include "mavlink/common/mavlink_msg_actuator_output_status.h"
+#include "mavlink/common/mavlink_msg_esc_status.h"
+#include "mavlink/common/mavlink_msg_scaled_pressure2.h"
+#include "mavlink/common/mavlink_msg_set_mode.h"
+#include "mavlink/common/mavlink_msg_global_position_int.h"
+#include "mavlink/common/mavlink_msg_canfd_frame.h"
+#include "mavlink/common/mavlink_msg_optical_flow_rad.h"
+#include "mavlink/common/mavlink_msg_gps_global_origin.h"
+#include "mavlink/common/mavlink_msg_high_latency.h"
+#include "mavlink/common/mavlink_msg_param_value.h"
+#include "mavlink/common/mavlink_msg_attitude_target.h"
+#include "mavlink/common/mavlink_msg_time_estimate_to_target.h"
+#include "mavlink/common/mavlink_msg_camera_trigger.h"
+#include "mavlink/common/mavlink_msg_system_time.h"
+#include "mavlink/common/mavlink_msg_mission_item_reached.h"
+#include "mavlink/common/mavlink_msg_log_entry.h"
+#include "mavlink/common/mavlink_msg_link_node_status.h"
+#include "mavlink/common/mavlink_msg_command_int.h"
+#include "mavlink/common/mavlink_msg_position_target_local_ned.h"
+#include "mavlink/common/mavlink_msg_rc_channels_override.h"
+#include "mavlink/common/mavlink_msg_local_position_ned_cov.h"
+#include "mavlink/common/mavlink_msg_raw_pressure.h"
+#include "mavlink/common/mavlink_msg_home_position.h"
+#include "mavlink/common/mavlink_msg_autopilot_version.h"
+#include "mavlink/common/mavlink_msg_change_operator_control.h"
+#include "mavlink/common/mavlink_msg_manual_setpoint.h"
+#include "mavlink/common/mavlink_msg_scaled_imu.h"
+#include "mavlink/common/mavlink_msg_wind_cov.h"
+#include "mavlink/common/mavlink_msg_debug_vect.h"
+#include "mavlink/common/mavlink_msg_gps_status.h"
+#include "mavlink/common/mavlink_msg_flight_information.h"
+#include "mavlink/common/mavlink_msg_scaled_pressure.h"
+#include "mavlink/common/mavlink_msg_set_attitude_target.h"
+#include "mavlink/common/mavlink_msg_ais_vessel.h"
+#include "mavlink/common/mavlink_msg_att_pos_mocap.h"
+#include "mavlink/common/mavlink_msg_hil_state_quaternion.h"
+#include "mavlink/common/mavlink_msg_landing_target.h"
+#include "mavlink/common/mavlink_msg_param_ext_request_read.h"
+#include "mavlink/common/mavlink_msg_button_change.h"
+#include "mavlink/common/mavlink_msg_attitude_quaternion_cov.h"
+#include "mavlink/common/mavlink_msg_open_drone_id_system_update.h"
+#include "mavlink/common/mavlink_msg_gimbal_manager_set_attitude.h"
+#include "mavlink/common/mavlink_msg_mission_ack.h"
+#include "mavlink/common/mavlink_msg_global_vision_position_estimate.h"
+#include "mavlink/common/mavlink_msg_local_position_ned.h"
+#include "mavlink/common/mavlink_msg_encapsulated_data.h"
+#include "mavlink/common/mavlink_msg_set_position_target_local_ned.h"
+#include "mavlink/common/mavlink_msg_open_drone_id_self_id.h"
+#include "mavlink/common/mavlink_msg_efi_status.h"
+#include "mavlink/common/mavlink_msg_mission_clear_all.h"
+#include "mavlink/common/mavlink_msg_sys_status.h"
+#include "mavlink/common/mavlink_msg_estimator_status.h"
+#include "mavlink/common/mavlink_msg_set_position_target_global_int.h"
+#include "mavlink/common/mavlink_msg_data_stream.h"
+#include "mavlink/common/mavlink_msg_timesync.h"
+#include "mavlink/common/mavlink_msg_camera_tracking_geo_status.h"
+#include "mavlink/common/mavlink_msg_gps_rtcm_data.h"
+#include "mavlink/common/mavlink_msg_camera_settings.h"
+#include "mavlink/common/mavlink_msg_video_stream_information.h"
+#include "mavlink/common/mavlink_msg_resource_request.h"
+#include "mavlink/common/mavlink_msg_request_data_stream.h"
+#include "mavlink/common/mavlink_msg_open_drone_id_system.h"
+#include "mavlink/common/mavlink_msg_set_gps_global_origin.h"
+#include "mavlink/common/mavlink_msg_param_request_list.h"
+#include "mavlink/common/mavlink_msg_serial_control.h"
+#include "mavlink/common/mavlink_msg_nav_controller_output.h"
+#include "mavlink/common/mavlink_msg_raw_rpm.h"
+#include "mavlink/common/mavlink_msg_log_erase.h"
+#include "mavlink/common/mavlink_msg_high_latency2.h"
+#include "mavlink/common/mavlink_msg_storage_information.h"
+#include "mavlink/common/mavlink_msg_ping.h"
+#include "mavlink/common/mavlink_msg_rc_channels_scaled.h"
+#include "mavlink/common/mavlink_msg_orbit_execution_status.h"
+#include "mavlink/common/mavlink_msg_debug_float_array.h"
+#include "mavlink/common/mavlink_msg_command_ack.h"
+#include "mavlink/common/mavlink_msg_supported_tunes.h"
+#include "mavlink/common/mavlink_msg_adsb_vehicle.h"
+#include "mavlink/common/mavlink_msg_set_home_position.h"
+#include "mavlink/common/mavlink_msg_gps_raw_int.h"
+#include "mavlink/common/mavlink_msg_mission_request_list.h"
+#include "mavlink/common/mavlink_msg_servo_output_raw.h"
+#include "mavlink/common/mavlink_msg_logging_ack.h"
+#include "mavlink/common/mavlink_msg_can_frame.h"
+#include "mavlink/common/mavlink_msg_debug.h"
+#include "mavlink/common/mavlink_msg_radio_status.h"
+#include "mavlink/common/mavlink_msg_gimbal_device_set_attitude.h"
+#include "mavlink/common/mavlink_msg_optical_flow.h"
+#include "mavlink/common/mavlink_msg_collision.h"
+#include "mavlink/common/mavlink_msg_mission_request_int.h"
+#include "mavlink/common/mavlink_msg_open_drone_id_authentication.h"
+#include "mavlink/common/mavlink_msg_generator_status.h"
+#include "mavlink/common/mavlink_msg_camera_capture_status.h"
+#include "mavlink/common/mavlink_msg_mission_request.h"
+#include "mavlink/common/mavlink_msg_attitude_quaternion.h"
+#include "mavlink/common/mavlink_msg_obstacle_distance.h"
+#include "mavlink/common/mavlink_msg_hil_state.h"
+#include "mavlink/common/mavlink_msg_gimbal_manager_status.h"
+#include "mavlink/common/mavlink_msg_trajectory_representation_waypoints.h"
+#include "mavlink/common/mavlink_msg_auth_key.h"
+#include "mavlink/common/mavlink_msg_terrain_check.h"
+#include "mavlink/common/mavlink_msg_gps_inject_data.h"
+#include "mavlink/common/mavlink_msg_scaled_imu3.h"
+#include "mavlink/common/mavlink_msg_battery_status.h"
+#include "mavlink/common/mavlink_msg_open_drone_id_basic_id.h"
+#include "mavlink/common/mavlink_msg_param_map_rc.h"
+#include "mavlink/common/mavlink_msg_hil_controls.h"
+#include "mavlink/common/mavlink_msg_gps_input.h"
+#include "mavlink/common/mavlink_msg_gps2_rtk.h"
+#include "mavlink/common/mavlink_msg_set_actuator_control_target.h"
+#include "mavlink/common/mavlink_msg_named_value_float.h"
+#include "mavlink/common/mavlink_msg_wheel_distance.h"
+#include "mavlink/common/mavlink_msg_onboard_computer_status.h"
+#include "mavlink/common/mavlink_msg_rc_channels_raw.h"
+#include "mavlink/common/mavlink_msg_mission_item_int.h"
+#include "mavlink/common/mavlink_msg_log_request_list.h"
+#include "mavlink/common/mavlink_msg_safety_allowed_area.h"
+#include "mavlink/common/mavlink_msg_tunnel.h"
+#include "mavlink/common/mavlink_msg_global_position_int_cov.h"
+#include "mavlink/common/mavlink_msg_camera_information.h"
+#include "mavlink/common/mavlink_msg_gimbal_device_information.h"
+#include "mavlink/common/mavlink_msg_terrain_request.h"
+#include "mavlink/common/mavlink_msg_command_long.h"
+#include "mavlink/common/mavlink_msg_camera_tracking_image_status.h"
+#include "mavlink/common/mavlink_msg_vfr_hud.h"
+#include "mavlink/common/mavlink_msg_log_data.h"
+#include "mavlink/common/mavlink_msg_can_filter_modify.h"
+#include "mavlink/common/mavlink_msg_vicon_position_estimate.h"
+#include "mavlink/common/mavlink_msg_mission_request_partial_list.h"
+#include "mavlink/common/mavlink_msg_logging_data.h"
+#include "mavlink/common/mavlink_msg_raw_imu.h"
+#include "mavlink/common/mavlink_msg_open_drone_id_arm_status.h"
+#include "mavlink/common/mavlink_msg_mission_item.h"
+#include "mavlink/common/mavlink_msg_open_drone_id_location.h"
+#include "mavlink/common/mavlink_msg_response_event_error.h"
+#include "mavlink/common/mavlink_msg_smart_battery_info.h"
+#include "mavlink/common/mavlink_msg_mission_write_partial_list.h"
+#include "mavlink/common/mavlink_msg_sim_state.h"
+#include "mavlink/common/mavlink_msg_mission_count.h"
+#include "mavlink/common/mavlink_msg_memory_vect.h"
+#include "mavlink/common/mavlink_msg_position_target_global_int.h"
+#include "mavlink/common/mavlink_msg_altitude.h"
+#include "mavlink/ASLUAV/mavlink_msg_sens_mppt.h"
 #include "mavlink/ASLUAV/mavlink_msg_command_int_stamped.h"
+#include "mavlink/ASLUAV/mavlink_msg_sens_batmon.h"
+#include "mavlink/ASLUAV/mavlink_msg_aslctrl_debug.h"
 #include "mavlink/ASLUAV/mavlink_msg_sens_atmos.h"
-#include "mavlink/ASLUAV/mavlink_msg_gsm_link_status.h"
 #include "mavlink/ASLUAV/mavlink_msg_satcom_link_status.h"
-#include "mavlink/ASLUAV/mavlink_msg_sens_power_board.h"
-#include "mavlink/ASLUAV/mavlink_msg_sens_mppt.h"
-#include "mavlink/ASLUAV/mavlink_msg_asl_obctrl.h"
-#include "mavlink/ASLUAV/mavlink_msg_sensorpod_status.h"
+#include "mavlink/ASLUAV/mavlink_msg_fw_soaring_data.h"
 #include "mavlink/ASLUAV/mavlink_msg_aslctrl_data.h"
+#include "mavlink/ASLUAV/mavlink_msg_asluav_status.h"
+#include "mavlink/ASLUAV/mavlink_msg_sens_power_board.h"
+#include "mavlink/ASLUAV/mavlink_msg_gsm_link_status.h"
+#include "mavlink/ASLUAV/mavlink_msg_command_long_stamped.h"
+#include "mavlink/ASLUAV/mavlink_msg_sensor_airflow_angles.h"
 #include "mavlink/ASLUAV/mavlink_msg_ekf_ext.h"
-#include "mavlink/ASLUAV/mavlink_msg_fw_soaring_data.h"
-#include "mavlink/AVSSUAS/mavlink_msg_avss_drone_operation_mode.h"
-#include "mavlink/AVSSUAS/mavlink_msg_avss_drone_imu.h"
-#include "mavlink/AVSSUAS/mavlink_msg_avss_prs_sys_status.h"
-#include "mavlink/AVSSUAS/mavlink_msg_avss_drone_position.h"
-#include "mavlink/ardupilotmega/mavlink_msg_osd_param_show_config_reply.h"
+#include "mavlink/ASLUAV/mavlink_msg_sensorpod_status.h"
+#include "mavlink/ASLUAV/mavlink_msg_sens_power.h"
+#include "mavlink/ASLUAV/mavlink_msg_asl_obctrl.h"
 #include "mavlink/ardupilotmega/mavlink_msg_mag_cal_progress.h"
-#include "mavlink/ardupilotmega/mavlink_msg_gopro_get_response.h"
-#include "mavlink/ardupilotmega/mavlink_msg_data32.h"
-#include "mavlink/ardupilotmega/mavlink_msg_rangefinder.h"
-#include "mavlink/ardupilotmega/mavlink_msg_water_depth.h"
-#include "mavlink/ardupilotmega/mavlink_msg_airspeed_autocal.h"
-#include "mavlink/ardupilotmega/mavlink_msg_data96.h"
-#include "mavlink/ardupilotmega/mavlink_msg_remote_log_data_block.h"
+#include "mavlink/ardupilotmega/mavlink_msg_ahrs.h"
+#include "mavlink/ardupilotmega/mavlink_msg_wind.h"
+#include "mavlink/ardupilotmega/mavlink_msg_gopro_get_request.h"
+#include "mavlink/ardupilotmega/mavlink_msg_rpm.h"
+#include "mavlink/ardupilotmega/mavlink_msg_obstacle_distance_3d.h"
+#include "mavlink/ardupilotmega/mavlink_msg_device_op_write_reply.h"
+#include "mavlink/ardupilotmega/mavlink_msg_camera_feedback.h"
+#include "mavlink/ardupilotmega/mavlink_msg_meminfo.h"
+#include "mavlink/ardupilotmega/mavlink_msg_gopro_set_response.h"
+#include "mavlink/ardupilotmega/mavlink_msg_device_op_read_reply.h"
+#include "mavlink/ardupilotmega/mavlink_msg_camera_status.h"
+#include "mavlink/ardupilotmega/mavlink_msg_pid_tuning.h"
 #include "mavlink/ardupilotmega/mavlink_msg_set_mag_offsets.h"
-#include "mavlink/ardupilotmega/mavlink_msg_gimbal_report.h"
+#include "mavlink/ardupilotmega/mavlink_msg_rangefinder.h"
+#include "mavlink/ardupilotmega/mavlink_msg_mount_control.h"
 #include "mavlink/ardupilotmega/mavlink_msg_gimbal_torque_cmd_report.h"
-#include "mavlink/ardupilotmega/mavlink_msg_simstate.h"
-#include "mavlink/ardupilotmega/mavlink_msg_autopilot_version_request.h"
-#include "mavlink/ardupilotmega/mavlink_msg_esc_telemetry_5_to_8.h"
-#include "mavlink/ardupilotmega/mavlink_msg_vision_position_delta.h"
-#include "mavlink/ardupilotmega/mavlink_msg_device_op_read_reply.h"
-#include "mavlink/ardupilotmega/mavlink_msg_device_op_read.h"
 #include "mavlink/ardupilotmega/mavlink_msg_fence_fetch_point.h"
-#include "mavlink/ardupilotmega/mavlink_msg_device_op_write.h"
-#include "mavlink/ardupilotmega/mavlink_msg_ahrs.h"
-#include "mavlink/ardupilotmega/mavlink_msg_mount_control.h"
 #include "mavlink/ardupilotmega/mavlink_msg_ekf_status_report.h"
-#include "mavlink/ardupilotmega/mavlink_msg_camera_feedback.h"
+#include "mavlink/ardupilotmega/mavlink_msg_data96.h"
+#include "mavlink/ardupilotmega/mavlink_msg_osd_param_show_config.h"
+#include "mavlink/ardupilotmega/mavlink_msg_ahrs3.h"
+#include "mavlink/ardupilotmega/mavlink_msg_limits_status.h"
 #include "mavlink/ardupilotmega/mavlink_msg_gopro_set_request.h"
-#include "mavlink/ardupilotmega/mavlink_msg_mount_status.h"
-#include "mavlink/ardupilotmega/mavlink_msg_gopro_heartbeat.h"
+#include "mavlink/ardupilotmega/mavlink_msg_sensor_offsets.h"
+#include "mavlink/ardupilotmega/mavlink_msg_ahrs2.h"
+#include "mavlink/ardupilotmega/mavlink_msg_data32.h"
+#include "mavlink/ardupilotmega/mavlink_msg_gimbal_report.h"
+#include "mavlink/ardupilotmega/mavlink_msg_hwstatus.h"
+#include "mavlink/ardupilotmega/mavlink_msg_vision_position_delta.h"
+#include "mavlink/ardupilotmega/mavlink_msg_osd_param_config.h"
+#include "mavlink/ardupilotmega/mavlink_msg_led_control.h"
 #include "mavlink/ardupilotmega/mavlink_msg_data64.h"
-#include "mavlink/ardupilotmega/mavlink_msg_gimbal_control.h"
-#include "mavlink/ardupilotmega/mavlink_msg_mcu_status.h"
-#include "mavlink/ardupilotmega/mavlink_msg_aoa_ssa.h"
-#include "mavlink/ardupilotmega/mavlink_msg_rpm.h"
+#include "mavlink/ardupilotmega/mavlink_msg_battery2.h"
 #include "mavlink/ardupilotmega/mavlink_msg_rally_point.h"
-#include "mavlink/ardupilotmega/mavlink_msg_data16.h"
-#include "mavlink/ardupilotmega/mavlink_msg_limits_status.h"
-#include "mavlink/ardupilotmega/mavlink_msg_pid_tuning.h"
-#include "mavlink/ardupilotmega/mavlink_msg_digicam_control.h"
-#include "mavlink/ardupilotmega/mavlink_msg_wind.h"
-#include "mavlink/ardupilotmega/mavlink_msg_gopro_set_response.h"
-#include "mavlink/ardupilotmega/mavlink_msg_compassmot_status.h"
-#include "mavlink/ardupilotmega/mavlink_msg_ahrs3.h"
-#include "mavlink/ardupilotmega/mavlink_msg_remote_log_block_status.h"
-#include "mavlink/ardupilotmega/mavlink_msg_rally_fetch_point.h"
-#include "mavlink/ardupilotmega/mavlink_msg_ahrs2.h"
-#include "mavlink/ardupilotmega/mavlink_msg_osd_param_show_config.h"
+#include "mavlink/ardupilotmega/mavlink_msg_aoa_ssa.h"
 #include "mavlink/ardupilotmega/mavlink_msg_deepstall.h"
-#include "mavlink/ardupilotmega/mavlink_msg_device_op_write_reply.h"
-#include "mavlink/ardupilotmega/mavlink_msg_osd_param_config_reply.h"
-#include "mavlink/ardupilotmega/mavlink_msg_camera_status.h"
+#include "mavlink/ardupilotmega/mavlink_msg_digicam_configure.h"
+#include "mavlink/ardupilotmega/mavlink_msg_remote_log_block_status.h"
+#include "mavlink/ardupilotmega/mavlink_msg_data16.h"
+#include "mavlink/ardupilotmega/mavlink_msg_autopilot_version_request.h"
+#include "mavlink/ardupilotmega/mavlink_msg_esc_telemetry_9_to_12.h"
 #include "mavlink/ardupilotmega/mavlink_msg_fence_point.h"
+#include "mavlink/ardupilotmega/mavlink_msg_compassmot_status.h"
+#include "mavlink/ardupilotmega/mavlink_msg_gopro_get_response.h"
+#include "mavlink/ardupilotmega/mavlink_msg_mount_status.h"
 #include "mavlink/ardupilotmega/mavlink_msg_radio.h"
-#include "mavlink/ardupilotmega/mavlink_msg_obstacle_distance_3d.h"
-#include "mavlink/ardupilotmega/mavlink_msg_meminfo.h"
+#include "mavlink/ardupilotmega/mavlink_msg_osd_param_config_reply.h"
+#include "mavlink/ardupilotmega/mavlink_msg_remote_log_data_block.h"
+#include "mavlink/ardupilotmega/mavlink_msg_digicam_control.h"
+#include "mavlink/ardupilotmega/mavlink_msg_water_depth.h"
 #include "mavlink/ardupilotmega/mavlink_msg_mount_configure.h"
-#include "mavlink/ardupilotmega/mavlink_msg_led_control.h"
-#include "mavlink/ardupilotmega/mavlink_msg_adap_tuning.h"
-#include "mavlink/ardupilotmega/mavlink_msg_battery2.h"
-#include "mavlink/ardupilotmega/mavlink_msg_osd_param_config.h"
+#include "mavlink/ardupilotmega/mavlink_msg_esc_telemetry_5_to_8.h"
+#include "mavlink/ardupilotmega/mavlink_msg_device_op_write.h"
 #include "mavlink/ardupilotmega/mavlink_msg_ap_adc.h"
-#include "mavlink/ardupilotmega/mavlink_msg_sensor_offsets.h"
-#include "mavlink/ardupilotmega/mavlink_msg_digicam_configure.h"
+#include "mavlink/ardupilotmega/mavlink_msg_device_op_read.h"
+#include "mavlink/ardupilotmega/mavlink_msg_simstate.h"
+#include "mavlink/ardupilotmega/mavlink_msg_rally_fetch_point.h"
 #include "mavlink/ardupilotmega/mavlink_msg_esc_telemetry_1_to_4.h"
-#include "mavlink/ardupilotmega/mavlink_msg_esc_telemetry_9_to_12.h"
-#include "mavlink/ardupilotmega/mavlink_msg_hwstatus.h"
-#include "mavlink/ardupilotmega/mavlink_msg_gopro_get_request.h"
-#include "mavlink/storm32/mavlink_msg_storm32_gimbal_manager_correct_roll.h"
-#include "mavlink/storm32/mavlink_msg_radio_rc_channels.h"
-#include "mavlink/storm32/mavlink_msg_param_value_array.h"
-#include "mavlink/storm32/mavlink_msg_storm32_gimbal_manager_information.h"
-#include "mavlink/storm32/mavlink_msg_radio_link_stats.h"
-#include "mavlink/storm32/mavlink_msg_frsky_passthrough_array.h"
-#include "mavlink/storm32/mavlink_msg_storm32_gimbal_manager_control.h"
-#include "mavlink/storm32/mavlink_msg_storm32_gimbal_manager_control_pitchyaw.h"
-#include "mavlink/storm32/mavlink_msg_storm32_gimbal_manager_status.h"
-#include "mavlink/storm32/mavlink_msg_qshot_status.h"
-#include "mavlink/cubepilot/mavlink_msg_cubepilot_raw_rc.h"
+#include "mavlink/ardupilotmega/mavlink_msg_adap_tuning.h"
+#include "mavlink/ardupilotmega/mavlink_msg_gopro_heartbeat.h"
+#include "mavlink/ardupilotmega/mavlink_msg_airspeed_autocal.h"
+#include "mavlink/ardupilotmega/mavlink_msg_osd_param_show_config_reply.h"
+#include "mavlink/ardupilotmega/mavlink_msg_gimbal_control.h"
+#include "mavlink/ardupilotmega/mavlink_msg_mcu_status.h"
 #include "mavlink/cubepilot/mavlink_msg_cubepilot_firmware_update_resp.h"
+#include "mavlink/cubepilot/mavlink_msg_cubepilot_raw_rc.h"
 #include "mavlink/cubepilot/mavlink_msg_herelink_video_stream_information.h"
 #include "mavlink/cubepilot/mavlink_msg_herelink_telem.h"
 #include "mavlink/cubepilot/mavlink_msg_cubepilot_firmware_update_start.h"
-#include "mavlink/uAvionix/mavlink_msg_uavionix_adsb_out_dynamic.h"
+#include "mavlink/ualberta/mavlink_msg_nav_filter_bias.h"
+#include "mavlink/ualberta/mavlink_msg_ualberta_sys_status.h"
+#include "mavlink/ualberta/mavlink_msg_radio_calibration.h"
+#include "mavlink/icarous/mavlink_msg_icarous_heartbeat.h"
+#include "mavlink/icarous/mavlink_msg_icarous_kinematic_bands.h"
+#include "mavlink/storm32/mavlink_msg_storm32_gimbal_manager_correct_roll.h"
+#include "mavlink/storm32/mavlink_msg_frsky_passthrough_array.h"
+#include "mavlink/storm32/mavlink_msg_storm32_gimbal_manager_information.h"
+#include "mavlink/storm32/mavlink_msg_param_value_array.h"
+#include "mavlink/storm32/mavlink_msg_qshot_status.h"
+#include "mavlink/storm32/mavlink_msg_radio_rc_channels.h"
+#include "mavlink/storm32/mavlink_msg_storm32_gimbal_manager_control_pitchyaw.h"
+#include "mavlink/storm32/mavlink_msg_storm32_gimbal_manager_status.h"
+#include "mavlink/storm32/mavlink_msg_radio_link_stats.h"
+#include "mavlink/storm32/mavlink_msg_storm32_gimbal_manager_control.h"
+#include "mavlink/development/mavlink_msg_figure_eight_execution_status.h"
+#include "mavlink/development/mavlink_msg_target_absolute.h"
+#include "mavlink/development/mavlink_msg_wifi_network_info.h"
+#include "mavlink/development/mavlink_msg_mission_checksum.h"
+#include "mavlink/development/mavlink_msg_target_relative.h"
+#include "mavlink/development/mavlink_msg_available_modes.h"
+#include "mavlink/development/mavlink_msg_airspeed.h"
+#include "mavlink/development/mavlink_msg_component_information_basic.h"
+#include "mavlink/development/mavlink_msg_param_ack_transaction.h"
+#include "mavlink/development/mavlink_msg_group_end.h"
+#include "mavlink/development/mavlink_msg_current_mode.h"
+#include "mavlink/development/mavlink_msg_battery_status_v2.h"
+#include "mavlink/development/mavlink_msg_group_start.h"
+#include "mavlink/minimal/mavlink_msg_protocol_version.h"
+#include "mavlink/minimal/mavlink_msg_heartbeat.h"
 #include "mavlink/uAvionix/mavlink_msg_uavionix_adsb_transceiver_health_report.h"
+#include "mavlink/uAvionix/mavlink_msg_uavionix_adsb_out_dynamic.h"
 #include "mavlink/uAvionix/mavlink_msg_uavionix_adsb_out_cfg.h"
-#include "mavlink/python_array_test/mavlink_msg_array_test_6.h"
 #include "mavlink/python_array_test/mavlink_msg_array_test_1.h"
-#include "mavlink/python_array_test/mavlink_msg_array_test_3.h"
-#include "mavlink/python_array_test/mavlink_msg_array_test_8.h"
 #include "mavlink/python_array_test/mavlink_msg_array_test_7.h"
-#include "mavlink/python_array_test/mavlink_msg_array_test_0.h"
-#include "mavlink/python_array_test/mavlink_msg_array_test_5.h"
 #include "mavlink/python_array_test/mavlink_msg_array_test_4.h"
-#include "mavlink/minimal/mavlink_msg_protocol_version.h"
-#include "mavlink/minimal/mavlink_msg_heartbeat.h"
+#include "mavlink/python_array_test/mavlink_msg_array_test_5.h"
+#include "mavlink/python_array_test/mavlink_msg_array_test_8.h"
+#include "mavlink/python_array_test/mavlink_msg_array_test_6.h"
+#include "mavlink/python_array_test/mavlink_msg_array_test_0.h"
+#include "mavlink/python_array_test/mavlink_msg_array_test_3.h"
+#include "mavlink/AVSSUAS/mavlink_msg_avss_drone_position.h"
+#include "mavlink/AVSSUAS/mavlink_msg_avss_drone_operation_mode.h"
+#include "mavlink/AVSSUAS/mavlink_msg_avss_drone_imu.h"
+#include "mavlink/AVSSUAS/mavlink_msg_avss_prs_sys_status.h"
 #include "mavlink/test/mavlink_msg_test_types.h"
-#include "mavlink/ualberta/mavlink_msg_radio_calibration.h"
-#include "mavlink/ualberta/mavlink_msg_ualberta_sys_status.h"
-#include "mavlink/ualberta/mavlink_msg_nav_filter_bias.h"
-#include "mavlink/common/mavlink_msg_hygrometer_sensor.h"
-#include "mavlink/common/mavlink_msg_local_position_ned.h"
-#include "mavlink/common/mavlink_msg_ais_vessel.h"
-#include "mavlink/common/mavlink_msg_gimbal_device_attitude_status.h"
-#include "mavlink/common/mavlink_msg_mission_write_partial_list.h"
-#include "mavlink/common/mavlink_msg_scaled_imu2.h"
-#include "mavlink/common/mavlink_msg_vision_speed_estimate.h"
-#include "mavlink/common/mavlink_msg_serial_control.h"
-#include "mavlink/common/mavlink_msg_mission_set_current.h"
-#include "mavlink/common/mavlink_msg_landing_target.h"
-#include "mavlink/common/mavlink_msg_rc_channels.h"
-#include "mavlink/common/mavlink_msg_command_ack.h"
-#include "mavlink/common/mavlink_msg_autopilot_version.h"
-#include "mavlink/common/mavlink_msg_safety_set_allowed_area.h"
-#include "mavlink/common/mavlink_msg_memory_vect.h"
-#include "mavlink/common/mavlink_msg_request_event.h"
-#include "mavlink/common/mavlink_msg_rc_channels_scaled.h"
-#include "mavlink/common/mavlink_msg_isbd_link_status.h"
-#include "mavlink/common/mavlink_msg_gps_inject_data.h"
-#include "mavlink/common/mavlink_msg_mission_item_int.h"
-#include "mavlink/common/mavlink_msg_gimbal_device_information.h"
-#include "mavlink/common/mavlink_msg_scaled_imu3.h"
-#include "mavlink/common/mavlink_msg_manual_setpoint.h"
-#include "mavlink/common/mavlink_msg_safety_allowed_area.h"
-#include "mavlink/common/mavlink_msg_follow_target.h"
-#include "mavlink/common/mavlink_msg_gps_rtcm_data.h"
-#include "mavlink/common/mavlink_msg_rc_channels_raw.h"
-#include "mavlink/common/mavlink_msg_hil_gps.h"
-#include "mavlink/common/mavlink_msg_attitude.h"
-#include "mavlink/common/mavlink_msg_component_metadata.h"
-#include "mavlink/common/mavlink_msg_gps_raw_int.h"
-#include "mavlink/common/mavlink_msg_mission_clear_all.h"
-#include "mavlink/common/mavlink_msg_position_target_global_int.h"
-#include "mavlink/common/mavlink_msg_manual_control.h"
-#include "mavlink/common/mavlink_msg_camera_tracking_image_status.h"
-#include "mavlink/common/mavlink_msg_debug.h"
-#include "mavlink/common/mavlink_msg_video_stream_information.h"
-#include "mavlink/common/mavlink_msg_mission_request_partial_list.h"
-#include "mavlink/common/mavlink_msg_open_drone_id_arm_status.h"
-#include "mavlink/common/mavlink_msg_param_set.h"
-#include "mavlink/common/mavlink_msg_open_drone_id_authentication.h"
-#include "mavlink/common/mavlink_msg_event.h"
-#include "mavlink/common/mavlink_msg_set_attitude_target.h"
-#include "mavlink/common/mavlink_msg_change_operator_control.h"
-#include "mavlink/common/mavlink_msg_link_node_status.h"
-#include "mavlink/common/mavlink_msg_v2_extension.h"
-#include "mavlink/common/mavlink_msg_camera_information.h"
-#include "mavlink/common/mavlink_msg_attitude_quaternion_cov.h"
-#include "mavlink/common/mavlink_msg_collision.h"
-#include "mavlink/common/mavlink_msg_hil_controls.h"
-#include "mavlink/common/mavlink_msg_scaled_pressure2.h"
-#include "mavlink/common/mavlink_msg_gimbal_device_set_attitude.h"
-#include "mavlink/common/mavlink_msg_terrain_data.h"
-#include "mavlink/common/mavlink_msg_supported_tunes.h"
-#include "mavlink/common/mavlink_msg_can_filter_modify.h"
-#include "mavlink/common/mavlink_msg_distance_sensor.h"
-#include "mavlink/common/mavlink_msg_hil_state.h"
-#include "mavlink/common/mavlink_msg_camera_capture_status.h"
-#include "mavlink/common/mavlink_msg_canfd_frame.h"
-#include "mavlink/common/mavlink_msg_flight_information.h"
-#include "mavlink/common/mavlink_msg_logging_data_acked.h"
-#include "mavlink/common/mavlink_msg_optical_flow.h"
-#include "mavlink/common/mavlink_msg_command_cancel.h"
-#include "mavlink/common/mavlink_msg_camera_image_captured.h"
-#include "mavlink/common/mavlink_msg_set_position_target_global_int.h"
-#include "mavlink/common/mavlink_msg_set_gps_global_origin.h"
-#include "mavlink/common/mavlink_msg_statustext.h"
-#include "mavlink/common/mavlink_msg_param_request_read.h"
-#include "mavlink/common/mavlink_msg_adsb_vehicle.h"
-#include "mavlink/common/mavlink_msg_high_latency.h"
-#include "mavlink/common/mavlink_msg_wheel_distance.h"
-#include "mavlink/common/mavlink_msg_extended_sys_state.h"
-#include "mavlink/common/mavlink_msg_vibration.h"
-#include "mavlink/common/mavlink_msg_obstacle_distance.h"
-#include "mavlink/common/mavlink_msg_log_entry.h"
-#include "mavlink/common/mavlink_msg_request_data_stream.h"
-#include "mavlink/common/mavlink_msg_autopilot_state_for_gimbal_device.h"
-#include "mavlink/common/mavlink_msg_open_drone_id_basic_id.h"
-#include "mavlink/common/mavlink_msg_command_long.h"
-#include "mavlink/common/mavlink_msg_named_value_int.h"
-#include "mavlink/common/mavlink_msg_mission_item.h"
-#include "mavlink/common/mavlink_msg_actuator_control_target.h"
-#include "mavlink/common/mavlink_msg_storage_information.h"
-#include "mavlink/common/mavlink_msg_time_estimate_to_target.h"
-#include "mavlink/common/mavlink_msg_mission_ack.h"
-#include "mavlink/common/mavlink_msg_position_target_local_ned.h"
-#include "mavlink/common/mavlink_msg_trajectory_representation_waypoints.h"
-#include "mavlink/common/mavlink_msg_local_position_ned_cov.h"
-#include "mavlink/common/mavlink_msg_control_system_state.h"
-#include "mavlink/common/mavlink_msg_orbit_execution_status.h"
-#include "mavlink/common/mavlink_msg_efi_status.h"
-#include "mavlink/common/mavlink_msg_debug_float_array.h"
-#include "mavlink/common/mavlink_msg_response_event_error.h"
-#include "mavlink/common/mavlink_msg_can_frame.h"
-#include "mavlink/common/mavlink_msg_camera_settings.h"
-#include "mavlink/common/mavlink_msg_nav_controller_output.h"
-#include "mavlink/common/mavlink_msg_utm_global_position.h"
-#include "mavlink/common/mavlink_msg_raw_imu.h"
-#include "mavlink/common/mavlink_msg_camera_fov_status.h"
-#include "mavlink/common/mavlink_msg_hil_rc_inputs_raw.h"
-#include "mavlink/common/mavlink_msg_logging_ack.h"
-#include "mavlink/common/mavlink_msg_timesync.h"
-#include "mavlink/common/mavlink_msg_gps_global_origin.h"
-#include "mavlink/common/mavlink_msg_debug_vect.h"
-#include "mavlink/common/mavlink_msg_gimbal_manager_status.h"
-#include "mavlink/common/mavlink_msg_actuator_output_status.h"
-#include "mavlink/common/mavlink_msg_open_drone_id_system.h"
-#include "mavlink/common/mavlink_msg_altitude.h"
-#include "mavlink/common/mavlink_msg_vfr_hud.h"
-#include "mavlink/common/mavlink_msg_terrain_report.h"
-#include "mavlink/common/mavlink_msg_gimbal_manager_information.h"
-#include "mavlink/common/mavlink_msg_cellular_status.h"
-#include "mavlink/common/mavlink_msg_mag_cal_report.h"
-#include "mavlink/common/mavlink_msg_raw_rpm.h"
-#include "mavlink/common/mavlink_msg_param_value.h"
-#include "mavlink/common/mavlink_msg_highres_imu.h"
-#include "mavlink/common/mavlink_msg_hil_sensor.h"
-#include "mavlink/common/mavlink_msg_rc_channels_override.h"
-#include "mavlink/common/mavlink_msg_cellular_config.h"
-#include "mavlink/common/mavlink_msg_gps2_rtk.h"
-#include "mavlink/common/mavlink_msg_trajectory_representation_bezier.h"
-#include "mavlink/common/mavlink_msg_log_request_end.h"
-#include "mavlink/common/mavlink_msg_mission_request_int.h"
-#include "mavlink/common/mavlink_msg_sys_status.h"
-#include "mavlink/common/mavlink_msg_global_position_int_cov.h"
-#include "mavlink/common/mavlink_msg_param_ext_request_list.h"
-#include "mavlink/common/mavlink_msg_sim_state.h"
-#include "mavlink/common/mavlink_msg_param_ext_set.h"
-#include "mavlink/common/mavlink_msg_scaled_pressure.h"
-#include "mavlink/common/mavlink_msg_terrain_request.h"
-#include "mavlink/common/mavlink_msg_named_value_float.h"
-#include "mavlink/common/mavlink_msg_radio_status.h"
-#include "mavlink/common/mavlink_msg_wind_cov.h"
-#include "mavlink/common/mavlink_msg_log_request_data.h"
-#include "mavlink/common/mavlink_msg_param_ext_request_read.h"
-#include "mavlink/common/mavlink_msg_system_time.h"
-#include "mavlink/common/mavlink_msg_component_information.h"
-#include "mavlink/common/mavlink_msg_global_vision_position_estimate.h"
-#include "mavlink/common/mavlink_msg_open_drone_id_message_pack.h"
-#include "mavlink/common/mavlink_msg_generator_status.h"
-#include "mavlink/common/mavlink_msg_smart_battery_info.h"
-#include "mavlink/common/mavlink_msg_esc_status.h"
-#include "mavlink/common/mavlink_msg_battery_status.h"
-#include "mavlink/common/mavlink_msg_ping.h"
-#include "mavlink/common/mavlink_msg_estimator_status.h"
-#include "mavlink/common/mavlink_msg_log_erase.h"
-#include "mavlink/common/mavlink_msg_button_change.h"
-#include "mavlink/common/mavlink_msg_data_stream.h"
-#include "mavlink/common/mavlink_msg_set_mode.h"
-#include "mavlink/common/mavlink_msg_gps_status.h"
-#include "mavlink/common/mavlink_msg_attitude_quaternion.h"
-#include "mavlink/common/mavlink_msg_current_event_sequence.h"
-#include "mavlink/common/mavlink_msg_open_drone_id_self_id.h"
-#include "mavlink/common/mavlink_msg_set_home_position.h"
-#include "mavlink/common/mavlink_msg_gps_input.h"
-#include "mavlink/common/mavlink_msg_hil_state_quaternion.h"
-#include "mavlink/common/mavlink_msg_open_drone_id_location.h"
-#include "mavlink/common/mavlink_msg_mission_request_list.h"
-#include "mavlink/common/mavlink_msg_gimbal_manager_set_pitchyaw.h"
-#include "mavlink/common/mavlink_msg_power_status.h"
-#include "mavlink/common/mavlink_msg_hil_optical_flow.h"
-#include "mavlink/common/mavlink_msg_resource_request.h"
-#include "mavlink/common/mavlink_msg_gimbal_manager_set_attitude.h"
-#include "mavlink/common/mavlink_msg_vicon_position_estimate.h"
-#include "mavlink/common/mavlink_msg_set_actuator_control_target.h"
-#include "mavlink/common/mavlink_msg_message_interval.h"
-#include "mavlink/common/mavlink_msg_mission_current.h"
-#include "mavlink/common/mavlink_msg_scaled_imu.h"
-#include "mavlink/common/mavlink_msg_set_position_target_local_ned.h"
-#include "mavlink/common/mavlink_msg_hil_actuator_controls.h"
-#include "mavlink/common/mavlink_msg_command_int.h"
-#include "mavlink/common/mavlink_msg_play_tune_v2.h"
-#include "mavlink/common/mavlink_msg_mount_orientation.h"
-#include "mavlink/common/mavlink_msg_global_position_int.h"
-#include "mavlink/common/mavlink_msg_gps_rtk.h"
-#include "mavlink/common/mavlink_msg_setup_signing.h"
-#include "mavlink/common/mavlink_msg_param_ext_ack.h"
-#include "mavlink/common/mavlink_msg_winch_status.h"
-#include "mavlink/common/mavlink_msg_fence_status.h"
-#include "mavlink/common/mavlink_msg_auth_key.h"
-#include "mavlink/common/mavlink_msg_tunnel.h"
-#include "mavlink/common/mavlink_msg_optical_flow_rad.h"
-#include "mavlink/common/mavlink_msg_local_position_ned_system_global_offset.h"
-#include "mavlink/common/mavlink_msg_param_map_rc.h"
-#include "mavlink/common/mavlink_msg_log_data.h"
-#include "mavlink/common/mavlink_msg_file_transfer_protocol.h"
-#include "mavlink/common/mavlink_msg_encapsulated_data.h"
-#include "mavlink/common/mavlink_msg_param_ext_value.h"
-#include "mavlink/common/mavlink_msg_mission_request.h"
-#include "mavlink/common/mavlink_msg_terrain_check.h"
-#include "mavlink/common/mavlink_msg_uavcan_node_status.h"
-#include "mavlink/common/mavlink_msg_camera_tracking_geo_status.h"
-#include "mavlink/common/mavlink_msg_uavcan_node_info.h"
-#include "mavlink/common/mavlink_msg_data_transmission_handshake.h"
-#include "mavlink/common/mavlink_msg_mission_item_reached.h"
-#include "mavlink/common/mavlink_msg_gps2_raw.h"
-#include "mavlink/common/mavlink_msg_scaled_pressure3.h"
-#include "mavlink/common/mavlink_msg_att_pos_mocap.h"
-#include "mavlink/common/mavlink_msg_raw_pressure.h"
-#include "mavlink/common/mavlink_msg_play_tune.h"
-#include "mavlink/common/mavlink_msg_high_latency2.h"
-#include "mavlink/common/mavlink_msg_camera_trigger.h"
-#include "mavlink/common/mavlink_msg_gimbal_manager_set_manual_control.h"
-#include "mavlink/common/mavlink_msg_log_request_list.h"
-#include "mavlink/common/mavlink_msg_attitude_target.h"
-#include "mavlink/common/mavlink_msg_change_operator_control_ack.h"
-#include "mavlink/common/mavlink_msg_wifi_config_ap.h"
-#include "mavlink/common/mavlink_msg_mission_count.h"
-#include "mavlink/common/mavlink_msg_esc_info.h"
-#include "mavlink/common/mavlink_msg_param_request_list.h"
-#include "mavlink/common/mavlink_msg_onboard_computer_status.h"
-#include "mavlink/common/mavlink_msg_home_position.h"
-#include "mavlink/common/mavlink_msg_open_drone_id_system_update.h"
-#include "mavlink/common/mavlink_msg_vision_position_estimate.h"
-#include "mavlink/common/mavlink_msg_video_stream_status.h"
-#include "mavlink/common/mavlink_msg_logging_data.h"
-#include "mavlink/common/mavlink_msg_odometry.h"
-#include "mavlink/common/mavlink_msg_servo_output_raw.h"
-#include "mavlink/common/mavlink_msg_open_drone_id_operator_id.h"
 #include "mavlink_introspect_gen.h"
 
-cStruct* unbox_wifi_network_info(const mavlink_message_t* message)
+cStruct* unbox_local_position_ned_system_global_offset(const mavlink_message_t* message)
 {
-    static mavlink_wifi_network_info_t parsed;
+    static mavlink_local_position_ned_system_global_offset_t parsed;
 
     static cMember members[] = {
-        { "data_rate", &(parsed.data_rate), 1, UINT16_T},
-        { "ssid", &(parsed.ssid), 32, CHAR},
-        { "channel_id", &(parsed.channel_id), 1, UINT8_T},
-        { "signal_quality", &(parsed.signal_quality), 1, UINT8_T},
-        { "security", &(parsed.security), 1, UINT8_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "x", &(parsed.x), 1, FLOAT},
+        { "y", &(parsed.y), 1, FLOAT},
+        { "z", &(parsed.z), 1, FLOAT},
+        { "roll", &(parsed.roll), 1, FLOAT},
+        { "pitch", &(parsed.pitch), 1, FLOAT},
+        { "yaw", &(parsed.yaw), 1, FLOAT}
     };
-    static cStruct record = {"wifi_network_info", members, 5, 298};
+    static cStruct record = {"local_position_ned_system_global_offset", members, 7, 89};
 
-    mavlink_msg_wifi_network_info_decode(message, &parsed);
+    mavlink_msg_local_position_ned_system_global_offset_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_target_absolute(const mavlink_message_t* message)
+cStruct* unbox_hil_actuator_controls(const mavlink_message_t* message)
 {
-    static mavlink_target_absolute_t parsed;
+    static mavlink_hil_actuator_controls_t parsed;
 
     static cMember members[] = {
-        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
-        { "lat", &(parsed.lat), 1, INT32_T},
-        { "lon", &(parsed.lon), 1, INT32_T},
-        { "alt", &(parsed.alt), 1, FLOAT},
-        { "vel", &(parsed.vel), 3, FLOAT},
-        { "acc", &(parsed.acc), 3, FLOAT},
-        { "q_target", &(parsed.q_target), 4, FLOAT},
-        { "rates", &(parsed.rates), 3, FLOAT},
-        { "position_std", &(parsed.position_std), 2, FLOAT},
-        { "vel_std", &(parsed.vel_std), 3, FLOAT},
-        { "acc_std", &(parsed.acc_std), 3, FLOAT},
-        { "id", &(parsed.id), 1, UINT8_T},
-        { "sensor_capabilities", &(parsed.sensor_capabilities), 1, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "flags", &(parsed.flags), 1, UINT64_T},
+        { "controls", &(parsed.controls), 16, FLOAT},
+        { "mode", &(parsed.mode), 1, UINT8_T}
     };
-    static cStruct record = {"target_absolute", members, 13, 510};
+    static cStruct record = {"hil_actuator_controls", members, 4, 93};
 
-    mavlink_msg_target_absolute_decode(message, &parsed);
+    mavlink_msg_hil_actuator_controls_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_current_mode(const mavlink_message_t* message)
+cStruct* unbox_vision_speed_estimate(const mavlink_message_t* message)
 {
-    static mavlink_current_mode_t parsed;
+    static mavlink_vision_speed_estimate_t parsed;
 
     static cMember members[] = {
-        { "custom_mode", &(parsed.custom_mode), 1, UINT32_T},
-        { "standard_mode", &(parsed.standard_mode), 1, UINT8_T},
-        { "base_mode", &(parsed.base_mode), 1, UINT8_T}
+        { "usec", &(parsed.usec), 1, UINT64_T},
+        { "x", &(parsed.x), 1, FLOAT},
+        { "y", &(parsed.y), 1, FLOAT},
+        { "z", &(parsed.z), 1, FLOAT},
+        { "covariance", &(parsed.covariance), 9, FLOAT},
+        { "reset_counter", &(parsed.reset_counter), 1, UINT8_T}
     };
-    static cStruct record = {"current_mode", members, 3, 436};
+    static cStruct record = {"vision_speed_estimate", members, 6, 103};
 
-    mavlink_msg_current_mode_decode(message, &parsed);
+    mavlink_msg_vision_speed_estimate_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_battery_status_v2(const mavlink_message_t* message)
+cStruct* unbox_hil_rc_inputs_raw(const mavlink_message_t* message)
 {
-    static mavlink_battery_status_v2_t parsed;
+    static mavlink_hil_rc_inputs_raw_t parsed;
 
     static cMember members[] = {
-        { "voltage", &(parsed.voltage), 1, FLOAT},
-        { "current", &(parsed.current), 1, FLOAT},
-        { "capacity_consumed", &(parsed.capacity_consumed), 1, FLOAT},
-        { "capacity_remaining", &(parsed.capacity_remaining), 1, FLOAT},
-        { "status_flags", &(parsed.status_flags), 1, UINT32_T},
-        { "temperature", &(parsed.temperature), 1, INT16_T},
-        { "id", &(parsed.id), 1, UINT8_T},
-        { "percent_remaining", &(parsed.percent_remaining), 1, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "chan1_raw", &(parsed.chan1_raw), 1, UINT16_T},
+        { "chan2_raw", &(parsed.chan2_raw), 1, UINT16_T},
+        { "chan3_raw", &(parsed.chan3_raw), 1, UINT16_T},
+        { "chan4_raw", &(parsed.chan4_raw), 1, UINT16_T},
+        { "chan5_raw", &(parsed.chan5_raw), 1, UINT16_T},
+        { "chan6_raw", &(parsed.chan6_raw), 1, UINT16_T},
+        { "chan7_raw", &(parsed.chan7_raw), 1, UINT16_T},
+        { "chan8_raw", &(parsed.chan8_raw), 1, UINT16_T},
+        { "chan9_raw", &(parsed.chan9_raw), 1, UINT16_T},
+        { "chan10_raw", &(parsed.chan10_raw), 1, UINT16_T},
+        { "chan11_raw", &(parsed.chan11_raw), 1, UINT16_T},
+        { "chan12_raw", &(parsed.chan12_raw), 1, UINT16_T},
+        { "rssi", &(parsed.rssi), 1, UINT8_T}
     };
-    static cStruct record = {"battery_status_v2", members, 8, 369};
+    static cStruct record = {"hil_rc_inputs_raw", members, 14, 92};
 
-    mavlink_msg_battery_status_v2_decode(message, &parsed);
+    mavlink_msg_hil_rc_inputs_raw_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_group_start(const mavlink_message_t* message)
+cStruct* unbox_log_request_data(const mavlink_message_t* message)
 {
-    static mavlink_group_start_t parsed;
+    static mavlink_log_request_data_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "group_id", &(parsed.group_id), 1, UINT32_T},
-        { "mission_checksum", &(parsed.mission_checksum), 1, UINT32_T}
+        { "ofs", &(parsed.ofs), 1, UINT32_T},
+        { "count", &(parsed.count), 1, UINT32_T},
+        { "id", &(parsed.id), 1, UINT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T}
     };
-    static cStruct record = {"group_start", members, 3, 414};
+    static cStruct record = {"log_request_data", members, 5, 119};
 
-    mavlink_msg_group_start_decode(message, &parsed);
+    mavlink_msg_log_request_data_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_figure_eight_execution_status(const mavlink_message_t* message)
+cStruct* unbox_hil_optical_flow(const mavlink_message_t* message)
 {
-    static mavlink_figure_eight_execution_status_t parsed;
+    static mavlink_hil_optical_flow_t parsed;
 
     static cMember members[] = {
         { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "major_radius", &(parsed.major_radius), 1, FLOAT},
-        { "minor_radius", &(parsed.minor_radius), 1, FLOAT},
-        { "orientation", &(parsed.orientation), 1, FLOAT},
-        { "x", &(parsed.x), 1, INT32_T},
-        { "y", &(parsed.y), 1, INT32_T},
-        { "z", &(parsed.z), 1, FLOAT},
-        { "frame", &(parsed.frame), 1, UINT8_T}
+        { "integration_time_us", &(parsed.integration_time_us), 1, UINT32_T},
+        { "integrated_x", &(parsed.integrated_x), 1, FLOAT},
+        { "integrated_y", &(parsed.integrated_y), 1, FLOAT},
+        { "integrated_xgyro", &(parsed.integrated_xgyro), 1, FLOAT},
+        { "integrated_ygyro", &(parsed.integrated_ygyro), 1, FLOAT},
+        { "integrated_zgyro", &(parsed.integrated_zgyro), 1, FLOAT},
+        { "time_delta_distance_us", &(parsed.time_delta_distance_us), 1, UINT32_T},
+        { "distance", &(parsed.distance), 1, FLOAT},
+        { "temperature", &(parsed.temperature), 1, INT16_T},
+        { "sensor_id", &(parsed.sensor_id), 1, UINT8_T},
+        { "quality", &(parsed.quality), 1, UINT8_T}
     };
-    static cStruct record = {"figure_eight_execution_status", members, 8, 361};
+    static cStruct record = {"hil_optical_flow", members, 12, 114};
 
-    mavlink_msg_figure_eight_execution_status_decode(message, &parsed);
+    mavlink_msg_hil_optical_flow_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_group_end(const mavlink_message_t* message)
+cStruct* unbox_open_drone_id_message_pack(const mavlink_message_t* message)
 {
-    static mavlink_group_end_t parsed;
+    static mavlink_open_drone_id_message_pack_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "group_id", &(parsed.group_id), 1, UINT32_T},
-        { "mission_checksum", &(parsed.mission_checksum), 1, UINT32_T}
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "id_or_mac", &(parsed.id_or_mac), 20, UINT8_T},
+        { "single_message_size", &(parsed.single_message_size), 1, UINT8_T},
+        { "msg_pack_size", &(parsed.msg_pack_size), 1, UINT8_T},
+        { "messages", &(parsed.messages), 225, UINT8_T}
     };
-    static cStruct record = {"group_end", members, 3, 415};
+    static cStruct record = {"open_drone_id_message_pack", members, 6, 12915};
 
-    mavlink_msg_group_end_decode(message, &parsed);
+    mavlink_msg_open_drone_id_message_pack_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_mission_checksum(const mavlink_message_t* message)
+cStruct* unbox_safety_set_allowed_area(const mavlink_message_t* message)
 {
-    static mavlink_mission_checksum_t parsed;
+    static mavlink_safety_set_allowed_area_t parsed;
 
     static cMember members[] = {
-        { "checksum", &(parsed.checksum), 1, UINT32_T},
-        { "mission_type", &(parsed.mission_type), 1, UINT8_T}
+        { "p1x", &(parsed.p1x), 1, FLOAT},
+        { "p1y", &(parsed.p1y), 1, FLOAT},
+        { "p1z", &(parsed.p1z), 1, FLOAT},
+        { "p2x", &(parsed.p2x), 1, FLOAT},
+        { "p2y", &(parsed.p2y), 1, FLOAT},
+        { "p2z", &(parsed.p2z), 1, FLOAT},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "frame", &(parsed.frame), 1, UINT8_T}
     };
-    static cStruct record = {"mission_checksum", members, 2, 53};
+    static cStruct record = {"safety_set_allowed_area", members, 9, 54};
 
-    mavlink_msg_mission_checksum_decode(message, &parsed);
+    mavlink_msg_safety_set_allowed_area_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_target_relative(const mavlink_message_t* message)
+cStruct* unbox_play_tune_v2(const mavlink_message_t* message)
 {
-    static mavlink_target_relative_t parsed;
+    static mavlink_play_tune_v2_t parsed;
 
     static cMember members[] = {
-        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
-        { "x", &(parsed.x), 1, FLOAT},
-        { "y", &(parsed.y), 1, FLOAT},
-        { "z", &(parsed.z), 1, FLOAT},
-        { "pos_std", &(parsed.pos_std), 3, FLOAT},
-        { "yaw_std", &(parsed.yaw_std), 1, FLOAT},
-        { "q_target", &(parsed.q_target), 4, FLOAT},
-        { "q_sensor", &(parsed.q_sensor), 4, FLOAT},
-        { "id", &(parsed.id), 1, UINT8_T},
-        { "frame", &(parsed.frame), 1, UINT8_T},
-        { "type", &(parsed.type), 1, UINT8_T}
+        { "format", &(parsed.format), 1, UINT32_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "tune", &(parsed.tune), 248, CHAR}
     };
-    static cStruct record = {"target_relative", members, 11, 511};
+    static cStruct record = {"play_tune_v2", members, 4, 400};
 
-    mavlink_msg_target_relative_decode(message, &parsed);
+    mavlink_msg_play_tune_v2_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_airspeed(const mavlink_message_t* message)
+cStruct* unbox_follow_target(const mavlink_message_t* message)
 {
-    static mavlink_airspeed_t parsed;
+    static mavlink_follow_target_t parsed;
 
     static cMember members[] = {
-        { "airspeed", &(parsed.airspeed), 1, FLOAT},
-        { "raw_press", &(parsed.raw_press), 1, FLOAT},
-        { "temperature", &(parsed.temperature), 1, INT16_T},
-        { "id", &(parsed.id), 1, UINT8_T},
-        { "flags", &(parsed.flags), 1, UINT8_T}
+        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
+        { "custom_state", &(parsed.custom_state), 1, UINT64_T},
+        { "lat", &(parsed.lat), 1, INT32_T},
+        { "lon", &(parsed.lon), 1, INT32_T},
+        { "alt", &(parsed.alt), 1, FLOAT},
+        { "vel", &(parsed.vel), 3, FLOAT},
+        { "acc", &(parsed.acc), 3, FLOAT},
+        { "attitude_q", &(parsed.attitude_q), 4, FLOAT},
+        { "rates", &(parsed.rates), 3, FLOAT},
+        { "position_cov", &(parsed.position_cov), 3, FLOAT},
+        { "est_capabilities", &(parsed.est_capabilities), 1, UINT8_T}
     };
-    static cStruct record = {"airspeed", members, 5, 295};
+    static cStruct record = {"follow_target", members, 11, 144};
 
-    mavlink_msg_airspeed_decode(message, &parsed);
+    mavlink_msg_follow_target_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_param_ack_transaction(const mavlink_message_t* message)
+cStruct* unbox_odometry(const mavlink_message_t* message)
 {
-    static mavlink_param_ack_transaction_t parsed;
+    static mavlink_odometry_t parsed;
 
     static cMember members[] = {
-        { "param_value", &(parsed.param_value), 1, FLOAT},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "param_id", &(parsed.param_id), 16, CHAR},
-        { "param_type", &(parsed.param_type), 1, UINT8_T},
-        { "param_result", &(parsed.param_result), 1, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "x", &(parsed.x), 1, FLOAT},
+        { "y", &(parsed.y), 1, FLOAT},
+        { "z", &(parsed.z), 1, FLOAT},
+        { "q", &(parsed.q), 4, FLOAT},
+        { "vx", &(parsed.vx), 1, FLOAT},
+        { "vy", &(parsed.vy), 1, FLOAT},
+        { "vz", &(parsed.vz), 1, FLOAT},
+        { "rollspeed", &(parsed.rollspeed), 1, FLOAT},
+        { "pitchspeed", &(parsed.pitchspeed), 1, FLOAT},
+        { "yawspeed", &(parsed.yawspeed), 1, FLOAT},
+        { "pose_covariance", &(parsed.pose_covariance), 21, FLOAT},
+        { "velocity_covariance", &(parsed.velocity_covariance), 21, FLOAT},
+        { "frame_id", &(parsed.frame_id), 1, UINT8_T},
+        { "child_frame_id", &(parsed.child_frame_id), 1, UINT8_T},
+        { "reset_counter", &(parsed.reset_counter), 1, UINT8_T},
+        { "estimator_type", &(parsed.estimator_type), 1, UINT8_T},
+        { "quality", &(parsed.quality), 1, INT8_T}
     };
-    static cStruct record = {"param_ack_transaction", members, 6, 19};
+    static cStruct record = {"odometry", members, 18, 331};
 
-    mavlink_msg_param_ack_transaction_decode(message, &parsed);
+    mavlink_msg_odometry_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_available_modes(const mavlink_message_t* message)
+cStruct* unbox_gps_rtk(const mavlink_message_t* message)
 {
-    static mavlink_available_modes_t parsed;
+    static mavlink_gps_rtk_t parsed;
 
     static cMember members[] = {
-        { "custom_mode", &(parsed.custom_mode), 1, UINT32_T},
-        { "number_modes", &(parsed.number_modes), 1, UINT8_T},
-        { "mode_index", &(parsed.mode_index), 1, UINT8_T},
-        { "standard_mode", &(parsed.standard_mode), 1, UINT8_T},
-        { "base_mode", &(parsed.base_mode), 1, UINT8_T},
-        { "mode_name", &(parsed.mode_name), 50, CHAR}
+        { "time_last_baseline_ms", &(parsed.time_last_baseline_ms), 1, UINT32_T},
+        { "tow", &(parsed.tow), 1, UINT32_T},
+        { "baseline_a_mm", &(parsed.baseline_a_mm), 1, INT32_T},
+        { "baseline_b_mm", &(parsed.baseline_b_mm), 1, INT32_T},
+        { "baseline_c_mm", &(parsed.baseline_c_mm), 1, INT32_T},
+        { "accuracy", &(parsed.accuracy), 1, UINT32_T},
+        { "iar_num_hypotheses", &(parsed.iar_num_hypotheses), 1, INT32_T},
+        { "wn", &(parsed.wn), 1, UINT16_T},
+        { "rtk_receiver_id", &(parsed.rtk_receiver_id), 1, UINT8_T},
+        { "rtk_health", &(parsed.rtk_health), 1, UINT8_T},
+        { "rtk_rate", &(parsed.rtk_rate), 1, UINT8_T},
+        { "nsats", &(parsed.nsats), 1, UINT8_T},
+        { "baseline_coords_type", &(parsed.baseline_coords_type), 1, UINT8_T}
     };
-    static cStruct record = {"available_modes", members, 6, 435};
+    static cStruct record = {"gps_rtk", members, 13, 127};
 
-    mavlink_msg_available_modes_decode(message, &parsed);
+    mavlink_msg_gps_rtk_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_component_information_basic(const mavlink_message_t* message)
+cStruct* unbox_winch_status(const mavlink_message_t* message)
 {
-    static mavlink_component_information_basic_t parsed;
+    static mavlink_winch_status_t parsed;
 
     static cMember members[] = {
-        { "capabilities", &(parsed.capabilities), 1, UINT64_T},
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "vendor_name", &(parsed.vendor_name), 32, CHAR},
-        { "model_name", &(parsed.model_name), 32, CHAR},
-        { "software_version", &(parsed.software_version), 24, CHAR},
-        { "hardware_version", &(parsed.hardware_version), 24, CHAR},
-        { "serial_number", &(parsed.serial_number), 32, CHAR}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "line_length", &(parsed.line_length), 1, FLOAT},
+        { "speed", &(parsed.speed), 1, FLOAT},
+        { "tension", &(parsed.tension), 1, FLOAT},
+        { "voltage", &(parsed.voltage), 1, FLOAT},
+        { "current", &(parsed.current), 1, FLOAT},
+        { "status", &(parsed.status), 1, UINT32_T},
+        { "temperature", &(parsed.temperature), 1, INT16_T}
     };
-    static cStruct record = {"component_information_basic", members, 7, 396};
+    static cStruct record = {"winch_status", members, 8, 9005};
 
-    mavlink_msg_component_information_basic_decode(message, &parsed);
+    mavlink_msg_winch_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_icarous_kinematic_bands(const mavlink_message_t* message)
+cStruct* unbox_trajectory_representation_bezier(const mavlink_message_t* message)
 {
-    static mavlink_icarous_kinematic_bands_t parsed;
+    static mavlink_trajectory_representation_bezier_t parsed;
 
     static cMember members[] = {
-        { "min1", &(parsed.min1), 1, FLOAT},
-        { "max1", &(parsed.max1), 1, FLOAT},
-        { "min2", &(parsed.min2), 1, FLOAT},
-        { "max2", &(parsed.max2), 1, FLOAT},
-        { "min3", &(parsed.min3), 1, FLOAT},
-        { "max3", &(parsed.max3), 1, FLOAT},
-        { "min4", &(parsed.min4), 1, FLOAT},
-        { "max4", &(parsed.max4), 1, FLOAT},
-        { "min5", &(parsed.min5), 1, FLOAT},
-        { "max5", &(parsed.max5), 1, FLOAT},
-        { "numBands", &(parsed.numBands), 1, INT8_T},
-        { "type1", &(parsed.type1), 1, UINT8_T},
-        { "type2", &(parsed.type2), 1, UINT8_T},
-        { "type3", &(parsed.type3), 1, UINT8_T},
-        { "type4", &(parsed.type4), 1, UINT8_T},
-        { "type5", &(parsed.type5), 1, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "pos_x", &(parsed.pos_x), 5, FLOAT},
+        { "pos_y", &(parsed.pos_y), 5, FLOAT},
+        { "pos_z", &(parsed.pos_z), 5, FLOAT},
+        { "delta", &(parsed.delta), 5, FLOAT},
+        { "pos_yaw", &(parsed.pos_yaw), 5, FLOAT},
+        { "valid_points", &(parsed.valid_points), 1, UINT8_T}
     };
-    static cStruct record = {"icarous_kinematic_bands", members, 16, 42001};
+    static cStruct record = {"trajectory_representation_bezier", members, 7, 333};
 
-    mavlink_msg_icarous_kinematic_bands_decode(message, &parsed);
+    mavlink_msg_trajectory_representation_bezier_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_icarous_heartbeat(const mavlink_message_t* message)
+cStruct* unbox_param_set(const mavlink_message_t* message)
 {
-    static mavlink_icarous_heartbeat_t parsed;
+    static mavlink_param_set_t parsed;
 
     static cMember members[] = {
-        { "status", &(parsed.status), 1, UINT8_T}
+        { "param_value", &(parsed.param_value), 1, FLOAT},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "param_id", &(parsed.param_id), 16, CHAR},
+        { "param_type", &(parsed.param_type), 1, UINT8_T}
     };
-    static cStruct record = {"icarous_heartbeat", members, 1, 42000};
+    static cStruct record = {"param_set", members, 5, 23};
 
-    mavlink_msg_icarous_heartbeat_decode(message, &parsed);
+    mavlink_msg_param_set_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_sensor_airflow_angles(const mavlink_message_t* message)
+cStruct* unbox_hil_gps(const mavlink_message_t* message)
 {
-    static mavlink_sensor_airflow_angles_t parsed;
+    static mavlink_hil_gps_t parsed;
 
     static cMember members[] = {
-        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
-        { "angleofattack", &(parsed.angleofattack), 1, FLOAT},
-        { "sideslip", &(parsed.sideslip), 1, FLOAT},
-        { "angleofattack_valid", &(parsed.angleofattack_valid), 1, UINT8_T},
-        { "sideslip_valid", &(parsed.sideslip_valid), 1, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "lat", &(parsed.lat), 1, INT32_T},
+        { "lon", &(parsed.lon), 1, INT32_T},
+        { "alt", &(parsed.alt), 1, INT32_T},
+        { "eph", &(parsed.eph), 1, UINT16_T},
+        { "epv", &(parsed.epv), 1, UINT16_T},
+        { "vel", &(parsed.vel), 1, UINT16_T},
+        { "vn", &(parsed.vn), 1, INT16_T},
+        { "ve", &(parsed.ve), 1, INT16_T},
+        { "vd", &(parsed.vd), 1, INT16_T},
+        { "cog", &(parsed.cog), 1, UINT16_T},
+        { "fix_type", &(parsed.fix_type), 1, UINT8_T},
+        { "satellites_visible", &(parsed.satellites_visible), 1, UINT8_T},
+        { "id", &(parsed.id), 1, UINT8_T},
+        { "yaw", &(parsed.yaw), 1, UINT16_T}
     };
-    static cStruct record = {"sensor_airflow_angles", members, 5, 8016};
+    static cStruct record = {"hil_gps", members, 15, 113};
 
-    mavlink_msg_sensor_airflow_angles_decode(message, &parsed);
+    mavlink_msg_hil_gps_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_aslctrl_debug(const mavlink_message_t* message)
+cStruct* unbox_wifi_config_ap(const mavlink_message_t* message)
 {
-    static mavlink_aslctrl_debug_t parsed;
+    static mavlink_wifi_config_ap_t parsed;
 
     static cMember members[] = {
-        { "i32_1", &(parsed.i32_1), 1, UINT32_T},
-        { "f_1", &(parsed.f_1), 1, FLOAT},
-        { "f_2", &(parsed.f_2), 1, FLOAT},
-        { "f_3", &(parsed.f_3), 1, FLOAT},
-        { "f_4", &(parsed.f_4), 1, FLOAT},
-        { "f_5", &(parsed.f_5), 1, FLOAT},
-        { "f_6", &(parsed.f_6), 1, FLOAT},
-        { "f_7", &(parsed.f_7), 1, FLOAT},
-        { "f_8", &(parsed.f_8), 1, FLOAT},
-        { "i8_1", &(parsed.i8_1), 1, UINT8_T},
-        { "i8_2", &(parsed.i8_2), 1, UINT8_T}
+        { "ssid", &(parsed.ssid), 32, CHAR},
+        { "password", &(parsed.password), 64, CHAR},
+        { "mode", &(parsed.mode), 1, INT8_T},
+        { "response", &(parsed.response), 1, INT8_T}
     };
-    static cStruct record = {"aslctrl_debug", members, 11, 8005};
+    static cStruct record = {"wifi_config_ap", members, 4, 299};
 
-    mavlink_msg_aslctrl_debug_decode(message, &parsed);
+    mavlink_msg_wifi_config_ap_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_sens_batmon(const mavlink_message_t* message)
+cStruct* unbox_vision_position_estimate(const mavlink_message_t* message)
 {
-    static mavlink_sens_batmon_t parsed;
+    static mavlink_vision_position_estimate_t parsed;
 
     static cMember members[] = {
-        { "batmon_timestamp", &(parsed.batmon_timestamp), 1, UINT64_T},
-        { "temperature", &(parsed.temperature), 1, FLOAT},
-        { "safetystatus", &(parsed.safetystatus), 1, UINT32_T},
-        { "operationstatus", &(parsed.operationstatus), 1, UINT32_T},
-        { "voltage", &(parsed.voltage), 1, UINT16_T},
-        { "current", &(parsed.current), 1, INT16_T},
-        { "batterystatus", &(parsed.batterystatus), 1, UINT16_T},
-        { "serialnumber", &(parsed.serialnumber), 1, UINT16_T},
-        { "cellvoltage1", &(parsed.cellvoltage1), 1, UINT16_T},
-        { "cellvoltage2", &(parsed.cellvoltage2), 1, UINT16_T},
-        { "cellvoltage3", &(parsed.cellvoltage3), 1, UINT16_T},
-        { "cellvoltage4", &(parsed.cellvoltage4), 1, UINT16_T},
-        { "cellvoltage5", &(parsed.cellvoltage5), 1, UINT16_T},
-        { "cellvoltage6", &(parsed.cellvoltage6), 1, UINT16_T},
-        { "SoC", &(parsed.SoC), 1, UINT8_T}
+        { "usec", &(parsed.usec), 1, UINT64_T},
+        { "x", &(parsed.x), 1, FLOAT},
+        { "y", &(parsed.y), 1, FLOAT},
+        { "z", &(parsed.z), 1, FLOAT},
+        { "roll", &(parsed.roll), 1, FLOAT},
+        { "pitch", &(parsed.pitch), 1, FLOAT},
+        { "yaw", &(parsed.yaw), 1, FLOAT},
+        { "covariance", &(parsed.covariance), 21, FLOAT},
+        { "reset_counter", &(parsed.reset_counter), 1, UINT8_T}
     };
-    static cStruct record = {"sens_batmon", members, 15, 8010};
+    static cStruct record = {"vision_position_estimate", members, 9, 102};
 
-    mavlink_msg_sens_batmon_decode(message, &parsed);
+    mavlink_msg_vision_position_estimate_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_asluav_status(const mavlink_message_t* message)
+cStruct* unbox_rc_channels(const mavlink_message_t* message)
 {
-    static mavlink_asluav_status_t parsed;
+    static mavlink_rc_channels_t parsed;
 
     static cMember members[] = {
-        { "Motor_rpm", &(parsed.Motor_rpm), 1, FLOAT},
-        { "LED_status", &(parsed.LED_status), 1, UINT8_T},
-        { "SATCOM_status", &(parsed.SATCOM_status), 1, UINT8_T},
-        { "Servo_status", &(parsed.Servo_status), 8, UINT8_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "chan1_raw", &(parsed.chan1_raw), 1, UINT16_T},
+        { "chan2_raw", &(parsed.chan2_raw), 1, UINT16_T},
+        { "chan3_raw", &(parsed.chan3_raw), 1, UINT16_T},
+        { "chan4_raw", &(parsed.chan4_raw), 1, UINT16_T},
+        { "chan5_raw", &(parsed.chan5_raw), 1, UINT16_T},
+        { "chan6_raw", &(parsed.chan6_raw), 1, UINT16_T},
+        { "chan7_raw", &(parsed.chan7_raw), 1, UINT16_T},
+        { "chan8_raw", &(parsed.chan8_raw), 1, UINT16_T},
+        { "chan9_raw", &(parsed.chan9_raw), 1, UINT16_T},
+        { "chan10_raw", &(parsed.chan10_raw), 1, UINT16_T},
+        { "chan11_raw", &(parsed.chan11_raw), 1, UINT16_T},
+        { "chan12_raw", &(parsed.chan12_raw), 1, UINT16_T},
+        { "chan13_raw", &(parsed.chan13_raw), 1, UINT16_T},
+        { "chan14_raw", &(parsed.chan14_raw), 1, UINT16_T},
+        { "chan15_raw", &(parsed.chan15_raw), 1, UINT16_T},
+        { "chan16_raw", &(parsed.chan16_raw), 1, UINT16_T},
+        { "chan17_raw", &(parsed.chan17_raw), 1, UINT16_T},
+        { "chan18_raw", &(parsed.chan18_raw), 1, UINT16_T},
+        { "chancount", &(parsed.chancount), 1, UINT8_T},
+        { "rssi", &(parsed.rssi), 1, UINT8_T}
     };
-    static cStruct record = {"asluav_status", members, 4, 8006};
+    static cStruct record = {"rc_channels", members, 21, 65};
 
-    mavlink_msg_asluav_status_decode(message, &parsed);
+    mavlink_msg_rc_channels_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_sens_power(const mavlink_message_t* message)
+cStruct* unbox_highres_imu(const mavlink_message_t* message)
 {
-    static mavlink_sens_power_t parsed;
+    static mavlink_highres_imu_t parsed;
 
     static cMember members[] = {
-        { "adc121_vspb_volt", &(parsed.adc121_vspb_volt), 1, FLOAT},
-        { "adc121_cspb_amp", &(parsed.adc121_cspb_amp), 1, FLOAT},
-        { "adc121_cs1_amp", &(parsed.adc121_cs1_amp), 1, FLOAT},
-        { "adc121_cs2_amp", &(parsed.adc121_cs2_amp), 1, FLOAT}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "xacc", &(parsed.xacc), 1, FLOAT},
+        { "yacc", &(parsed.yacc), 1, FLOAT},
+        { "zacc", &(parsed.zacc), 1, FLOAT},
+        { "xgyro", &(parsed.xgyro), 1, FLOAT},
+        { "ygyro", &(parsed.ygyro), 1, FLOAT},
+        { "zgyro", &(parsed.zgyro), 1, FLOAT},
+        { "xmag", &(parsed.xmag), 1, FLOAT},
+        { "ymag", &(parsed.ymag), 1, FLOAT},
+        { "zmag", &(parsed.zmag), 1, FLOAT},
+        { "abs_pressure", &(parsed.abs_pressure), 1, FLOAT},
+        { "diff_pressure", &(parsed.diff_pressure), 1, FLOAT},
+        { "pressure_alt", &(parsed.pressure_alt), 1, FLOAT},
+        { "temperature", &(parsed.temperature), 1, FLOAT},
+        { "fields_updated", &(parsed.fields_updated), 1, UINT16_T},
+        { "id", &(parsed.id), 1, UINT8_T}
     };
-    static cStruct record = {"sens_power", members, 4, 8002};
+    static cStruct record = {"highres_imu", members, 16, 105};
 
-    mavlink_msg_sens_power_decode(message, &parsed);
+    mavlink_msg_highres_imu_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_command_long_stamped(const mavlink_message_t* message)
+cStruct* unbox_gimbal_device_attitude_status(const mavlink_message_t* message)
 {
-    static mavlink_command_long_stamped_t parsed;
+    static mavlink_gimbal_device_attitude_status_t parsed;
 
     static cMember members[] = {
-        { "vehicle_timestamp", &(parsed.vehicle_timestamp), 1, UINT64_T},
-        { "utc_time", &(parsed.utc_time), 1, UINT32_T},
-        { "param1", &(parsed.param1), 1, FLOAT},
-        { "param2", &(parsed.param2), 1, FLOAT},
-        { "param3", &(parsed.param3), 1, FLOAT},
-        { "param4", &(parsed.param4), 1, FLOAT},
-        { "param5", &(parsed.param5), 1, FLOAT},
-        { "param6", &(parsed.param6), 1, FLOAT},
-        { "param7", &(parsed.param7), 1, FLOAT},
-        { "command", &(parsed.command), 1, UINT16_T},
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "q", &(parsed.q), 4, FLOAT},
+        { "angular_velocity_x", &(parsed.angular_velocity_x), 1, FLOAT},
+        { "angular_velocity_y", &(parsed.angular_velocity_y), 1, FLOAT},
+        { "angular_velocity_z", &(parsed.angular_velocity_z), 1, FLOAT},
+        { "failure_flags", &(parsed.failure_flags), 1, UINT32_T},
+        { "flags", &(parsed.flags), 1, UINT16_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "confirmation", &(parsed.confirmation), 1, UINT8_T}
+        { "delta_yaw", &(parsed.delta_yaw), 1, FLOAT},
+        { "delta_yaw_velocity", &(parsed.delta_yaw_velocity), 1, FLOAT}
     };
-    static cStruct record = {"command_long_stamped", members, 13, 224};
+    static cStruct record = {"gimbal_device_attitude_status", members, 11, 285};
 
-    mavlink_msg_command_long_stamped_decode(message, &parsed);
+    mavlink_msg_gimbal_device_attitude_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_command_int_stamped(const mavlink_message_t* message)
+cStruct* unbox_autopilot_state_for_gimbal_device(const mavlink_message_t* message)
 {
-    static mavlink_command_int_stamped_t parsed;
+    static mavlink_autopilot_state_for_gimbal_device_t parsed;
 
     static cMember members[] = {
-        { "vehicle_timestamp", &(parsed.vehicle_timestamp), 1, UINT64_T},
-        { "utc_time", &(parsed.utc_time), 1, UINT32_T},
-        { "param1", &(parsed.param1), 1, FLOAT},
-        { "param2", &(parsed.param2), 1, FLOAT},
-        { "param3", &(parsed.param3), 1, FLOAT},
-        { "param4", &(parsed.param4), 1, FLOAT},
-        { "x", &(parsed.x), 1, INT32_T},
-        { "y", &(parsed.y), 1, INT32_T},
-        { "z", &(parsed.z), 1, FLOAT},
-        { "command", &(parsed.command), 1, UINT16_T},
+        { "time_boot_us", &(parsed.time_boot_us), 1, UINT64_T},
+        { "q", &(parsed.q), 4, FLOAT},
+        { "q_estimated_delay_us", &(parsed.q_estimated_delay_us), 1, UINT32_T},
+        { "vx", &(parsed.vx), 1, FLOAT},
+        { "vy", &(parsed.vy), 1, FLOAT},
+        { "vz", &(parsed.vz), 1, FLOAT},
+        { "v_estimated_delay_us", &(parsed.v_estimated_delay_us), 1, UINT32_T},
+        { "feed_forward_angular_velocity_z", &(parsed.feed_forward_angular_velocity_z), 1, FLOAT},
+        { "estimator_status", &(parsed.estimator_status), 1, UINT16_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "frame", &(parsed.frame), 1, UINT8_T},
-        { "current", &(parsed.current), 1, UINT8_T},
-        { "autocontinue", &(parsed.autocontinue), 1, UINT8_T}
+        { "landed_state", &(parsed.landed_state), 1, UINT8_T},
+        { "angular_velocity_z", &(parsed.angular_velocity_z), 1, FLOAT}
     };
-    static cStruct record = {"command_int_stamped", members, 15, 223};
+    static cStruct record = {"autopilot_state_for_gimbal_device", members, 13, 286};
 
-    mavlink_msg_command_int_stamped_decode(message, &parsed);
+    mavlink_msg_autopilot_state_for_gimbal_device_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_sens_atmos(const mavlink_message_t* message)
+cStruct* unbox_fence_status(const mavlink_message_t* message)
 {
-    static mavlink_sens_atmos_t parsed;
+    static mavlink_fence_status_t parsed;
 
     static cMember members[] = {
-        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
-        { "TempAmbient", &(parsed.TempAmbient), 1, FLOAT},
-        { "Humidity", &(parsed.Humidity), 1, FLOAT}
+        { "breach_time", &(parsed.breach_time), 1, UINT32_T},
+        { "breach_count", &(parsed.breach_count), 1, UINT16_T},
+        { "breach_status", &(parsed.breach_status), 1, UINT8_T},
+        { "breach_type", &(parsed.breach_type), 1, UINT8_T},
+        { "breach_mitigation", &(parsed.breach_mitigation), 1, UINT8_T}
     };
-    static cStruct record = {"sens_atmos", members, 3, 8009};
+    static cStruct record = {"fence_status", members, 5, 162};
 
-    mavlink_msg_sens_atmos_decode(message, &parsed);
+    mavlink_msg_fence_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_gsm_link_status(const mavlink_message_t* message)
+cStruct* unbox_extended_sys_state(const mavlink_message_t* message)
 {
-    static mavlink_gsm_link_status_t parsed;
+    static mavlink_extended_sys_state_t parsed;
 
     static cMember members[] = {
-        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
-        { "gsm_modem_type", &(parsed.gsm_modem_type), 1, UINT8_T},
-        { "gsm_link_type", &(parsed.gsm_link_type), 1, UINT8_T},
-        { "rssi", &(parsed.rssi), 1, UINT8_T},
-        { "rsrp_rscp", &(parsed.rsrp_rscp), 1, UINT8_T},
-        { "sinr_ecio", &(parsed.sinr_ecio), 1, UINT8_T},
-        { "rsrq", &(parsed.rsrq), 1, UINT8_T}
+        { "vtol_state", &(parsed.vtol_state), 1, UINT8_T},
+        { "landed_state", &(parsed.landed_state), 1, UINT8_T}
     };
-    static cStruct record = {"gsm_link_status", members, 7, 8014};
+    static cStruct record = {"extended_sys_state", members, 2, 245};
 
-    mavlink_msg_gsm_link_status_decode(message, &parsed);
+    mavlink_msg_extended_sys_state_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_satcom_link_status(const mavlink_message_t* message)
+cStruct* unbox_open_drone_id_operator_id(const mavlink_message_t* message)
 {
-    static mavlink_satcom_link_status_t parsed;
+    static mavlink_open_drone_id_operator_id_t parsed;
 
     static cMember members[] = {
-        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
-        { "last_heartbeat", &(parsed.last_heartbeat), 1, UINT64_T},
-        { "failed_sessions", &(parsed.failed_sessions), 1, UINT16_T},
-        { "successful_sessions", &(parsed.successful_sessions), 1, UINT16_T},
-        { "signal_quality", &(parsed.signal_quality), 1, UINT8_T},
-        { "ring_pending", &(parsed.ring_pending), 1, UINT8_T},
-        { "tx_session_pending", &(parsed.tx_session_pending), 1, UINT8_T},
-        { "rx_session_pending", &(parsed.rx_session_pending), 1, UINT8_T}
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "id_or_mac", &(parsed.id_or_mac), 20, UINT8_T},
+        { "operator_id_type", &(parsed.operator_id_type), 1, UINT8_T},
+        { "operator_id", &(parsed.operator_id), 20, CHAR}
     };
-    static cStruct record = {"satcom_link_status", members, 8, 8015};
+    static cStruct record = {"open_drone_id_operator_id", members, 5, 12905};
 
-    mavlink_msg_satcom_link_status_decode(message, &parsed);
+    mavlink_msg_open_drone_id_operator_id_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_sens_power_board(const mavlink_message_t* message)
+cStruct* unbox_named_value_int(const mavlink_message_t* message)
 {
-    static mavlink_sens_power_board_t parsed;
+    static mavlink_named_value_int_t parsed;
 
     static cMember members[] = {
-        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
-        { "pwr_brd_system_volt", &(parsed.pwr_brd_system_volt), 1, FLOAT},
-        { "pwr_brd_servo_volt", &(parsed.pwr_brd_servo_volt), 1, FLOAT},
-        { "pwr_brd_digital_volt", &(parsed.pwr_brd_digital_volt), 1, FLOAT},
-        { "pwr_brd_mot_l_amp", &(parsed.pwr_brd_mot_l_amp), 1, FLOAT},
-        { "pwr_brd_mot_r_amp", &(parsed.pwr_brd_mot_r_amp), 1, FLOAT},
-        { "pwr_brd_analog_amp", &(parsed.pwr_brd_analog_amp), 1, FLOAT},
-        { "pwr_brd_digital_amp", &(parsed.pwr_brd_digital_amp), 1, FLOAT},
-        { "pwr_brd_ext_amp", &(parsed.pwr_brd_ext_amp), 1, FLOAT},
-        { "pwr_brd_aux_amp", &(parsed.pwr_brd_aux_amp), 1, FLOAT},
-        { "pwr_brd_status", &(parsed.pwr_brd_status), 1, UINT8_T},
-        { "pwr_brd_led_status", &(parsed.pwr_brd_led_status), 1, UINT8_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "value", &(parsed.value), 1, INT32_T},
+        { "name", &(parsed.name), 10, CHAR}
     };
-    static cStruct record = {"sens_power_board", members, 12, 8013};
+    static cStruct record = {"named_value_int", members, 3, 252};
 
-    mavlink_msg_sens_power_board_decode(message, &parsed);
+    mavlink_msg_named_value_int_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_sens_mppt(const mavlink_message_t* message)
+cStruct* unbox_message_interval(const mavlink_message_t* message)
 {
-    static mavlink_sens_mppt_t parsed;
+    static mavlink_message_interval_t parsed;
 
     static cMember members[] = {
-        { "mppt_timestamp", &(parsed.mppt_timestamp), 1, UINT64_T},
-        { "mppt1_volt", &(parsed.mppt1_volt), 1, FLOAT},
-        { "mppt1_amp", &(parsed.mppt1_amp), 1, FLOAT},
-        { "mppt2_volt", &(parsed.mppt2_volt), 1, FLOAT},
-        { "mppt2_amp", &(parsed.mppt2_amp), 1, FLOAT},
-        { "mppt3_volt", &(parsed.mppt3_volt), 1, FLOAT},
-        { "mppt3_amp", &(parsed.mppt3_amp), 1, FLOAT},
-        { "mppt1_pwm", &(parsed.mppt1_pwm), 1, UINT16_T},
-        { "mppt2_pwm", &(parsed.mppt2_pwm), 1, UINT16_T},
-        { "mppt3_pwm", &(parsed.mppt3_pwm), 1, UINT16_T},
-        { "mppt1_status", &(parsed.mppt1_status), 1, UINT8_T},
-        { "mppt2_status", &(parsed.mppt2_status), 1, UINT8_T},
-        { "mppt3_status", &(parsed.mppt3_status), 1, UINT8_T}
+        { "interval_us", &(parsed.interval_us), 1, INT32_T},
+        { "message_id", &(parsed.message_id), 1, UINT16_T}
     };
-    static cStruct record = {"sens_mppt", members, 13, 8003};
+    static cStruct record = {"message_interval", members, 2, 244};
 
-    mavlink_msg_sens_mppt_decode(message, &parsed);
+    mavlink_msg_message_interval_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_asl_obctrl(const mavlink_message_t* message)
+cStruct* unbox_param_ext_ack(const mavlink_message_t* message)
 {
-    static mavlink_asl_obctrl_t parsed;
+    static mavlink_param_ext_ack_t parsed;
 
     static cMember members[] = {
-        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
-        { "uElev", &(parsed.uElev), 1, FLOAT},
-        { "uThrot", &(parsed.uThrot), 1, FLOAT},
-        { "uThrot2", &(parsed.uThrot2), 1, FLOAT},
-        { "uAilL", &(parsed.uAilL), 1, FLOAT},
-        { "uAilR", &(parsed.uAilR), 1, FLOAT},
-        { "uRud", &(parsed.uRud), 1, FLOAT},
-        { "obctrl_status", &(parsed.obctrl_status), 1, UINT8_T}
+        { "param_id", &(parsed.param_id), 16, CHAR},
+        { "param_value", &(parsed.param_value), 128, CHAR},
+        { "param_type", &(parsed.param_type), 1, UINT8_T},
+        { "param_result", &(parsed.param_result), 1, UINT8_T}
     };
-    static cStruct record = {"asl_obctrl", members, 8, 8008};
+    static cStruct record = {"param_ext_ack", members, 4, 324};
 
-    mavlink_msg_asl_obctrl_decode(message, &parsed);
+    mavlink_msg_param_ext_ack_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_sensorpod_status(const mavlink_message_t* message)
+cStruct* unbox_param_ext_set(const mavlink_message_t* message)
 {
-    static mavlink_sensorpod_status_t parsed;
+    static mavlink_param_ext_set_t parsed;
 
     static cMember members[] = {
-        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
-        { "free_space", &(parsed.free_space), 1, UINT16_T},
-        { "visensor_rate_1", &(parsed.visensor_rate_1), 1, UINT8_T},
-        { "visensor_rate_2", &(parsed.visensor_rate_2), 1, UINT8_T},
-        { "visensor_rate_3", &(parsed.visensor_rate_3), 1, UINT8_T},
-        { "visensor_rate_4", &(parsed.visensor_rate_4), 1, UINT8_T},
-        { "recording_nodes_count", &(parsed.recording_nodes_count), 1, UINT8_T},
-        { "cpu_temp", &(parsed.cpu_temp), 1, UINT8_T}
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "param_id", &(parsed.param_id), 16, CHAR},
+        { "param_value", &(parsed.param_value), 128, CHAR},
+        { "param_type", &(parsed.param_type), 1, UINT8_T}
     };
-    static cStruct record = {"sensorpod_status", members, 8, 8012};
+    static cStruct record = {"param_ext_set", members, 5, 323};
 
-    mavlink_msg_sensorpod_status_decode(message, &parsed);
+    mavlink_msg_param_ext_set_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_aslctrl_data(const mavlink_message_t* message)
+cStruct* unbox_mag_cal_report(const mavlink_message_t* message)
 {
-    static mavlink_aslctrl_data_t parsed;
+    static mavlink_mag_cal_report_t parsed;
 
     static cMember members[] = {
-        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
-        { "h", &(parsed.h), 1, FLOAT},
-        { "hRef", &(parsed.hRef), 1, FLOAT},
-        { "hRef_t", &(parsed.hRef_t), 1, FLOAT},
-        { "PitchAngle", &(parsed.PitchAngle), 1, FLOAT},
-        { "PitchAngleRef", &(parsed.PitchAngleRef), 1, FLOAT},
-        { "q", &(parsed.q), 1, FLOAT},
-        { "qRef", &(parsed.qRef), 1, FLOAT},
-        { "uElev", &(parsed.uElev), 1, FLOAT},
-        { "uThrot", &(parsed.uThrot), 1, FLOAT},
-        { "uThrot2", &(parsed.uThrot2), 1, FLOAT},
-        { "nZ", &(parsed.nZ), 1, FLOAT},
-        { "AirspeedRef", &(parsed.AirspeedRef), 1, FLOAT},
-        { "YawAngle", &(parsed.YawAngle), 1, FLOAT},
-        { "YawAngleRef", &(parsed.YawAngleRef), 1, FLOAT},
-        { "RollAngle", &(parsed.RollAngle), 1, FLOAT},
-        { "RollAngleRef", &(parsed.RollAngleRef), 1, FLOAT},
-        { "p", &(parsed.p), 1, FLOAT},
-        { "pRef", &(parsed.pRef), 1, FLOAT},
-        { "r", &(parsed.r), 1, FLOAT},
-        { "rRef", &(parsed.rRef), 1, FLOAT},
-        { "uAil", &(parsed.uAil), 1, FLOAT},
-        { "uRud", &(parsed.uRud), 1, FLOAT},
-        { "aslctrl_mode", &(parsed.aslctrl_mode), 1, UINT8_T},
-        { "SpoilersEngaged", &(parsed.SpoilersEngaged), 1, UINT8_T}
+        { "fitness", &(parsed.fitness), 1, FLOAT},
+        { "ofs_x", &(parsed.ofs_x), 1, FLOAT},
+        { "ofs_y", &(parsed.ofs_y), 1, FLOAT},
+        { "ofs_z", &(parsed.ofs_z), 1, FLOAT},
+        { "diag_x", &(parsed.diag_x), 1, FLOAT},
+        { "diag_y", &(parsed.diag_y), 1, FLOAT},
+        { "diag_z", &(parsed.diag_z), 1, FLOAT},
+        { "offdiag_x", &(parsed.offdiag_x), 1, FLOAT},
+        { "offdiag_y", &(parsed.offdiag_y), 1, FLOAT},
+        { "offdiag_z", &(parsed.offdiag_z), 1, FLOAT},
+        { "compass_id", &(parsed.compass_id), 1, UINT8_T},
+        { "cal_mask", &(parsed.cal_mask), 1, UINT8_T},
+        { "cal_status", &(parsed.cal_status), 1, UINT8_T},
+        { "autosaved", &(parsed.autosaved), 1, UINT8_T},
+        { "orientation_confidence", &(parsed.orientation_confidence), 1, FLOAT},
+        { "old_orientation", &(parsed.old_orientation), 1, UINT8_T},
+        { "new_orientation", &(parsed.new_orientation), 1, UINT8_T},
+        { "scale_factor", &(parsed.scale_factor), 1, FLOAT}
     };
-    static cStruct record = {"aslctrl_data", members, 25, 8004};
+    static cStruct record = {"mag_cal_report", members, 18, 192};
 
-    mavlink_msg_aslctrl_data_decode(message, &parsed);
+    mavlink_msg_mag_cal_report_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_ekf_ext(const mavlink_message_t* message)
+cStruct* unbox_current_event_sequence(const mavlink_message_t* message)
 {
-    static mavlink_ekf_ext_t parsed;
+    static mavlink_current_event_sequence_t parsed;
 
     static cMember members[] = {
-        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
-        { "Windspeed", &(parsed.Windspeed), 1, FLOAT},
-        { "WindDir", &(parsed.WindDir), 1, FLOAT},
-        { "WindZ", &(parsed.WindZ), 1, FLOAT},
-        { "Airspeed", &(parsed.Airspeed), 1, FLOAT},
-        { "beta", &(parsed.beta), 1, FLOAT},
-        { "alpha", &(parsed.alpha), 1, FLOAT}
+        { "sequence", &(parsed.sequence), 1, UINT16_T},
+        { "flags", &(parsed.flags), 1, UINT8_T}
     };
-    static cStruct record = {"ekf_ext", members, 7, 8007};
+    static cStruct record = {"current_event_sequence", members, 2, 411};
 
-    mavlink_msg_ekf_ext_decode(message, &parsed);
+    mavlink_msg_current_event_sequence_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_fw_soaring_data(const mavlink_message_t* message)
+cStruct* unbox_terrain_data(const mavlink_message_t* message)
 {
-    static mavlink_fw_soaring_data_t parsed;
+    static mavlink_terrain_data_t parsed;
 
     static cMember members[] = {
-        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
-        { "timestampModeChanged", &(parsed.timestampModeChanged), 1, UINT64_T},
-        { "xW", &(parsed.xW), 1, FLOAT},
-        { "xR", &(parsed.xR), 1, FLOAT},
-        { "xLat", &(parsed.xLat), 1, FLOAT},
-        { "xLon", &(parsed.xLon), 1, FLOAT},
-        { "VarW", &(parsed.VarW), 1, FLOAT},
-        { "VarR", &(parsed.VarR), 1, FLOAT},
-        { "VarLat", &(parsed.VarLat), 1, FLOAT},
-        { "VarLon", &(parsed.VarLon), 1, FLOAT},
-        { "LoiterRadius", &(parsed.LoiterRadius), 1, FLOAT},
-        { "LoiterDirection", &(parsed.LoiterDirection), 1, FLOAT},
-        { "DistToSoarPoint", &(parsed.DistToSoarPoint), 1, FLOAT},
-        { "vSinkExp", &(parsed.vSinkExp), 1, FLOAT},
-        { "z1_LocalUpdraftSpeed", &(parsed.z1_LocalUpdraftSpeed), 1, FLOAT},
-        { "z2_DeltaRoll", &(parsed.z2_DeltaRoll), 1, FLOAT},
-        { "z1_exp", &(parsed.z1_exp), 1, FLOAT},
-        { "z2_exp", &(parsed.z2_exp), 1, FLOAT},
-        { "ThermalGSNorth", &(parsed.ThermalGSNorth), 1, FLOAT},
-        { "ThermalGSEast", &(parsed.ThermalGSEast), 1, FLOAT},
-        { "TSE_dot", &(parsed.TSE_dot), 1, FLOAT},
-        { "DebugVar1", &(parsed.DebugVar1), 1, FLOAT},
-        { "DebugVar2", &(parsed.DebugVar2), 1, FLOAT},
-        { "ControlMode", &(parsed.ControlMode), 1, UINT8_T},
-        { "valid", &(parsed.valid), 1, UINT8_T}
+        { "lat", &(parsed.lat), 1, INT32_T},
+        { "lon", &(parsed.lon), 1, INT32_T},
+        { "grid_spacing", &(parsed.grid_spacing), 1, UINT16_T},
+        { "data", &(parsed.data), 16, INT16_T},
+        { "gridbit", &(parsed.gridbit), 1, UINT8_T}
     };
-    static cStruct record = {"fw_soaring_data", members, 25, 8011};
+    static cStruct record = {"terrain_data", members, 5, 134};
 
-    mavlink_msg_fw_soaring_data_decode(message, &parsed);
+    mavlink_msg_terrain_data_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_avss_drone_operation_mode(const mavlink_message_t* message)
+cStruct* unbox_request_event(const mavlink_message_t* message)
 {
-    static mavlink_avss_drone_operation_mode_t parsed;
+    static mavlink_request_event_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "M300_operation_mode", &(parsed.M300_operation_mode), 1, UINT8_T},
-        { "horsefly_operation_mode", &(parsed.horsefly_operation_mode), 1, UINT8_T}
+        { "first_sequence", &(parsed.first_sequence), 1, UINT16_T},
+        { "last_sequence", &(parsed.last_sequence), 1, UINT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T}
     };
-    static cStruct record = {"avss_drone_operation_mode", members, 3, 60053};
+    static cStruct record = {"request_event", members, 4, 412};
 
-    mavlink_msg_avss_drone_operation_mode_decode(message, &parsed);
+    mavlink_msg_request_event_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_avss_drone_imu(const mavlink_message_t* message)
+cStruct* unbox_component_metadata(const mavlink_message_t* message)
 {
-    static mavlink_avss_drone_imu_t parsed;
+    static mavlink_component_metadata_t parsed;
 
     static cMember members[] = {
         { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "q1", &(parsed.q1), 1, FLOAT},
-        { "q2", &(parsed.q2), 1, FLOAT},
-        { "q3", &(parsed.q3), 1, FLOAT},
-        { "q4", &(parsed.q4), 1, FLOAT},
-        { "xacc", &(parsed.xacc), 1, FLOAT},
-        { "yacc", &(parsed.yacc), 1, FLOAT},
-        { "zacc", &(parsed.zacc), 1, FLOAT},
-        { "xgyro", &(parsed.xgyro), 1, FLOAT},
-        { "ygyro", &(parsed.ygyro), 1, FLOAT},
-        { "zgyro", &(parsed.zgyro), 1, FLOAT}
+        { "file_crc", &(parsed.file_crc), 1, UINT32_T},
+        { "uri", &(parsed.uri), 100, CHAR}
     };
-    static cStruct record = {"avss_drone_imu", members, 11, 60052};
+    static cStruct record = {"component_metadata", members, 3, 397};
 
-    mavlink_msg_avss_drone_imu_decode(message, &parsed);
+    mavlink_msg_component_metadata_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_avss_prs_sys_status(const mavlink_message_t* message)
+cStruct* unbox_actuator_control_target(const mavlink_message_t* message)
 {
-    static mavlink_avss_prs_sys_status_t parsed;
+    static mavlink_actuator_control_target_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "error_status", &(parsed.error_status), 1, UINT32_T},
-        { "battery_status", &(parsed.battery_status), 1, UINT32_T},
-        { "arm_status", &(parsed.arm_status), 1, UINT8_T},
-        { "charge_status", &(parsed.charge_status), 1, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "controls", &(parsed.controls), 8, FLOAT},
+        { "group_mlx", &(parsed.group_mlx), 1, UINT8_T}
     };
-    static cStruct record = {"avss_prs_sys_status", members, 5, 60050};
+    static cStruct record = {"actuator_control_target", members, 3, 140};
 
-    mavlink_msg_avss_prs_sys_status_decode(message, &parsed);
+    mavlink_msg_actuator_control_target_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_avss_drone_position(const mavlink_message_t* message)
+cStruct* unbox_scaled_imu2(const mavlink_message_t* message)
 {
-    static mavlink_avss_drone_position_t parsed;
+    static mavlink_scaled_imu2_t parsed;
 
     static cMember members[] = {
         { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "lat", &(parsed.lat), 1, INT32_T},
-        { "lon", &(parsed.lon), 1, INT32_T},
-        { "alt", &(parsed.alt), 1, INT32_T},
-        { "ground_alt", &(parsed.ground_alt), 1, FLOAT},
-        { "barometer_alt", &(parsed.barometer_alt), 1, FLOAT}
+        { "xacc", &(parsed.xacc), 1, INT16_T},
+        { "yacc", &(parsed.yacc), 1, INT16_T},
+        { "zacc", &(parsed.zacc), 1, INT16_T},
+        { "xgyro", &(parsed.xgyro), 1, INT16_T},
+        { "ygyro", &(parsed.ygyro), 1, INT16_T},
+        { "zgyro", &(parsed.zgyro), 1, INT16_T},
+        { "xmag", &(parsed.xmag), 1, INT16_T},
+        { "ymag", &(parsed.ymag), 1, INT16_T},
+        { "zmag", &(parsed.zmag), 1, INT16_T},
+        { "temperature", &(parsed.temperature), 1, INT16_T}
     };
-    static cStruct record = {"avss_drone_position", members, 6, 60051};
+    static cStruct record = {"scaled_imu2", members, 11, 116};
 
-    mavlink_msg_avss_drone_position_decode(message, &parsed);
+    mavlink_msg_scaled_imu2_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_osd_param_show_config_reply(const mavlink_message_t* message)
+cStruct* unbox_data_transmission_handshake(const mavlink_message_t* message)
 {
-    static mavlink_osd_param_show_config_reply_t parsed;
+    static mavlink_data_transmission_handshake_t parsed;
 
     static cMember members[] = {
-        { "request_id", &(parsed.request_id), 1, UINT32_T},
-        { "min_value", &(parsed.min_value), 1, FLOAT},
-        { "max_value", &(parsed.max_value), 1, FLOAT},
-        { "increment", &(parsed.increment), 1, FLOAT},
-        { "result", &(parsed.result), 1, UINT8_T},
-        { "param_id", &(parsed.param_id), 16, CHAR},
-        { "config_type", &(parsed.config_type), 1, UINT8_T}
+        { "size", &(parsed.size), 1, UINT32_T},
+        { "width", &(parsed.width), 1, UINT16_T},
+        { "height", &(parsed.height), 1, UINT16_T},
+        { "packets", &(parsed.packets), 1, UINT16_T},
+        { "type", &(parsed.type), 1, UINT8_T},
+        { "payload", &(parsed.payload), 1, UINT8_T},
+        { "jpg_quality", &(parsed.jpg_quality), 1, UINT8_T}
     };
-    static cStruct record = {"osd_param_show_config_reply", members, 7, 11036};
+    static cStruct record = {"data_transmission_handshake", members, 7, 130};
 
-    mavlink_msg_osd_param_show_config_reply_decode(message, &parsed);
+    mavlink_msg_data_transmission_handshake_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_mag_cal_progress(const mavlink_message_t* message)
+cStruct* unbox_uavcan_node_info(const mavlink_message_t* message)
 {
-    static mavlink_mag_cal_progress_t parsed;
+    static mavlink_uavcan_node_info_t parsed;
 
     static cMember members[] = {
-        { "direction_x", &(parsed.direction_x), 1, FLOAT},
-        { "direction_y", &(parsed.direction_y), 1, FLOAT},
-        { "direction_z", &(parsed.direction_z), 1, FLOAT},
-        { "compass_id", &(parsed.compass_id), 1, UINT8_T},
-        { "cal_mask", &(parsed.cal_mask), 1, UINT8_T},
-        { "cal_status", &(parsed.cal_status), 1, UINT8_T},
-        { "attempt", &(parsed.attempt), 1, UINT8_T},
-        { "completion_pct", &(parsed.completion_pct), 1, UINT8_T},
-        { "completion_mask", &(parsed.completion_mask), 10, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "uptime_sec", &(parsed.uptime_sec), 1, UINT32_T},
+        { "sw_vcs_commit", &(parsed.sw_vcs_commit), 1, UINT32_T},
+        { "name", &(parsed.name), 80, CHAR},
+        { "hw_version_major", &(parsed.hw_version_major), 1, UINT8_T},
+        { "hw_version_minor", &(parsed.hw_version_minor), 1, UINT8_T},
+        { "hw_unique_id", &(parsed.hw_unique_id), 16, UINT8_T},
+        { "sw_version_major", &(parsed.sw_version_major), 1, UINT8_T},
+        { "sw_version_minor", &(parsed.sw_version_minor), 1, UINT8_T}
     };
-    static cStruct record = {"mag_cal_progress", members, 9, 191};
+    static cStruct record = {"uavcan_node_info", members, 9, 311};
 
-    mavlink_msg_mag_cal_progress_decode(message, &parsed);
+    mavlink_msg_uavcan_node_info_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_gopro_get_response(const mavlink_message_t* message)
+cStruct* unbox_param_ext_value(const mavlink_message_t* message)
 {
-    static mavlink_gopro_get_response_t parsed;
+    static mavlink_param_ext_value_t parsed;
 
     static cMember members[] = {
-        { "cmd_id", &(parsed.cmd_id), 1, UINT8_T},
-        { "status", &(parsed.status), 1, UINT8_T},
-        { "value", &(parsed.value), 4, UINT8_T}
+        { "param_count", &(parsed.param_count), 1, UINT16_T},
+        { "param_index", &(parsed.param_index), 1, UINT16_T},
+        { "param_id", &(parsed.param_id), 16, CHAR},
+        { "param_value", &(parsed.param_value), 128, CHAR},
+        { "param_type", &(parsed.param_type), 1, UINT8_T}
     };
-    static cStruct record = {"gopro_get_response", members, 3, 217};
+    static cStruct record = {"param_ext_value", members, 5, 322};
 
-    mavlink_msg_gopro_get_response_decode(message, &parsed);
+    mavlink_msg_param_ext_value_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_data32(const mavlink_message_t* message)
+cStruct* unbox_play_tune(const mavlink_message_t* message)
 {
-    static mavlink_data32_t parsed;
+    static mavlink_play_tune_t parsed;
 
     static cMember members[] = {
-        { "type", &(parsed.type), 1, UINT8_T},
-        { "len", &(parsed.len), 1, UINT8_T},
-        { "data", &(parsed.data), 32, UINT8_T}
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "tune", &(parsed.tune), 30, CHAR},
+        { "tune2", &(parsed.tune2), 200, CHAR}
     };
-    static cStruct record = {"data32", members, 3, 170};
+    static cStruct record = {"play_tune", members, 4, 258};
 
-    mavlink_msg_data32_decode(message, &parsed);
+    mavlink_msg_play_tune_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_rangefinder(const mavlink_message_t* message)
+cStruct* unbox_cellular_status(const mavlink_message_t* message)
 {
-    static mavlink_rangefinder_t parsed;
+    static mavlink_cellular_status_t parsed;
 
     static cMember members[] = {
-        { "distance", &(parsed.distance), 1, FLOAT},
-        { "voltage", &(parsed.voltage), 1, FLOAT}
+        { "mcc", &(parsed.mcc), 1, UINT16_T},
+        { "mnc", &(parsed.mnc), 1, UINT16_T},
+        { "lac", &(parsed.lac), 1, UINT16_T},
+        { "status", &(parsed.status), 1, UINT8_T},
+        { "failure_reason", &(parsed.failure_reason), 1, UINT8_T},
+        { "type", &(parsed.type), 1, UINT8_T},
+        { "quality", &(parsed.quality), 1, UINT8_T}
     };
-    static cStruct record = {"rangefinder", members, 2, 173};
+    static cStruct record = {"cellular_status", members, 7, 334};
 
-    mavlink_msg_rangefinder_decode(message, &parsed);
+    mavlink_msg_cellular_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_water_depth(const mavlink_message_t* message)
+cStruct* unbox_logging_data_acked(const mavlink_message_t* message)
 {
-    static mavlink_water_depth_t parsed;
+    static mavlink_logging_data_acked_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "lat", &(parsed.lat), 1, INT32_T},
-        { "lng", &(parsed.lng), 1, INT32_T},
-        { "alt", &(parsed.alt), 1, FLOAT},
-        { "roll", &(parsed.roll), 1, FLOAT},
-        { "pitch", &(parsed.pitch), 1, FLOAT},
-        { "yaw", &(parsed.yaw), 1, FLOAT},
-        { "distance", &(parsed.distance), 1, FLOAT},
-        { "temperature", &(parsed.temperature), 1, FLOAT},
-        { "id", &(parsed.id), 1, UINT8_T},
-        { "healthy", &(parsed.healthy), 1, UINT8_T}
+        { "sequence", &(parsed.sequence), 1, UINT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "length", &(parsed.length), 1, UINT8_T},
+        { "first_message_offset", &(parsed.first_message_offset), 1, UINT8_T},
+        { "data", &(parsed.data), 249, UINT8_T}
     };
-    static cStruct record = {"water_depth", members, 11, 11038};
+    static cStruct record = {"logging_data_acked", members, 6, 267};
 
-    mavlink_msg_water_depth_decode(message, &parsed);
+    mavlink_msg_logging_data_acked_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_airspeed_autocal(const mavlink_message_t* message)
+cStruct* unbox_gps2_raw(const mavlink_message_t* message)
 {
-    static mavlink_airspeed_autocal_t parsed;
+    static mavlink_gps2_raw_t parsed;
 
     static cMember members[] = {
-        { "vx", &(parsed.vx), 1, FLOAT},
-        { "vy", &(parsed.vy), 1, FLOAT},
-        { "vz", &(parsed.vz), 1, FLOAT},
-        { "diff_pressure", &(parsed.diff_pressure), 1, FLOAT},
-        { "EAS2TAS", &(parsed.EAS2TAS), 1, FLOAT},
-        { "ratio", &(parsed.ratio), 1, FLOAT},
-        { "state_x", &(parsed.state_x), 1, FLOAT},
-        { "state_y", &(parsed.state_y), 1, FLOAT},
-        { "state_z", &(parsed.state_z), 1, FLOAT},
-        { "Pax", &(parsed.Pax), 1, FLOAT},
-        { "Pby", &(parsed.Pby), 1, FLOAT},
-        { "Pcz", &(parsed.Pcz), 1, FLOAT}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "lat", &(parsed.lat), 1, INT32_T},
+        { "lon", &(parsed.lon), 1, INT32_T},
+        { "alt", &(parsed.alt), 1, INT32_T},
+        { "dgps_age", &(parsed.dgps_age), 1, UINT32_T},
+        { "eph", &(parsed.eph), 1, UINT16_T},
+        { "epv", &(parsed.epv), 1, UINT16_T},
+        { "vel", &(parsed.vel), 1, UINT16_T},
+        { "cog", &(parsed.cog), 1, UINT16_T},
+        { "fix_type", &(parsed.fix_type), 1, UINT8_T},
+        { "satellites_visible", &(parsed.satellites_visible), 1, UINT8_T},
+        { "dgps_numch", &(parsed.dgps_numch), 1, UINT8_T},
+        { "yaw", &(parsed.yaw), 1, UINT16_T},
+        { "alt_ellipsoid", &(parsed.alt_ellipsoid), 1, INT32_T},
+        { "h_acc", &(parsed.h_acc), 1, UINT32_T},
+        { "v_acc", &(parsed.v_acc), 1, UINT32_T},
+        { "vel_acc", &(parsed.vel_acc), 1, UINT32_T},
+        { "hdg_acc", &(parsed.hdg_acc), 1, UINT32_T}
     };
-    static cStruct record = {"airspeed_autocal", members, 12, 174};
+    static cStruct record = {"gps2_raw", members, 18, 124};
 
-    mavlink_msg_airspeed_autocal_decode(message, &parsed);
+    mavlink_msg_gps2_raw_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_data96(const mavlink_message_t* message)
+cStruct* unbox_isbd_link_status(const mavlink_message_t* message)
 {
-    static mavlink_data96_t parsed;
+    static mavlink_isbd_link_status_t parsed;
 
     static cMember members[] = {
-        { "type", &(parsed.type), 1, UINT8_T},
-        { "len", &(parsed.len), 1, UINT8_T},
-        { "data", &(parsed.data), 96, UINT8_T}
+        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
+        { "last_heartbeat", &(parsed.last_heartbeat), 1, UINT64_T},
+        { "failed_sessions", &(parsed.failed_sessions), 1, UINT16_T},
+        { "successful_sessions", &(parsed.successful_sessions), 1, UINT16_T},
+        { "signal_quality", &(parsed.signal_quality), 1, UINT8_T},
+        { "ring_pending", &(parsed.ring_pending), 1, UINT8_T},
+        { "tx_session_pending", &(parsed.tx_session_pending), 1, UINT8_T},
+        { "rx_session_pending", &(parsed.rx_session_pending), 1, UINT8_T}
     };
-    static cStruct record = {"data96", members, 3, 172};
+    static cStruct record = {"isbd_link_status", members, 8, 335};
 
-    mavlink_msg_data96_decode(message, &parsed);
+    mavlink_msg_isbd_link_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_remote_log_data_block(const mavlink_message_t* message)
+cStruct* unbox_gimbal_manager_set_manual_control(const mavlink_message_t* message)
 {
-    static mavlink_remote_log_data_block_t parsed;
+    static mavlink_gimbal_manager_set_manual_control_t parsed;
 
     static cMember members[] = {
-        { "seqno", &(parsed.seqno), 1, UINT32_T},
+        { "flags", &(parsed.flags), 1, UINT32_T},
+        { "pitch", &(parsed.pitch), 1, FLOAT},
+        { "yaw", &(parsed.yaw), 1, FLOAT},
+        { "pitch_rate", &(parsed.pitch_rate), 1, FLOAT},
+        { "yaw_rate", &(parsed.yaw_rate), 1, FLOAT},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "data", &(parsed.data), 200, UINT8_T}
+        { "gimbal_device_id", &(parsed.gimbal_device_id), 1, UINT8_T}
     };
-    static cStruct record = {"remote_log_data_block", members, 4, 184};
+    static cStruct record = {"gimbal_manager_set_manual_control", members, 8, 288};
 
-    mavlink_msg_remote_log_data_block_decode(message, &parsed);
+    mavlink_msg_gimbal_manager_set_manual_control_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_set_mag_offsets(const mavlink_message_t* message)
+cStruct* unbox_camera_image_captured(const mavlink_message_t* message)
 {
-    static mavlink_set_mag_offsets_t parsed;
+    static mavlink_camera_image_captured_t parsed;
 
     static cMember members[] = {
-        { "mag_ofs_x", &(parsed.mag_ofs_x), 1, INT16_T},
-        { "mag_ofs_y", &(parsed.mag_ofs_y), 1, INT16_T},
-        { "mag_ofs_z", &(parsed.mag_ofs_z), 1, INT16_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T}
+        { "time_utc", &(parsed.time_utc), 1, UINT64_T},
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "lat", &(parsed.lat), 1, INT32_T},
+        { "lon", &(parsed.lon), 1, INT32_T},
+        { "alt", &(parsed.alt), 1, INT32_T},
+        { "relative_alt", &(parsed.relative_alt), 1, INT32_T},
+        { "q", &(parsed.q), 4, FLOAT},
+        { "image_index", &(parsed.image_index), 1, INT32_T},
+        { "camera_id", &(parsed.camera_id), 1, UINT8_T},
+        { "capture_result", &(parsed.capture_result), 1, INT8_T},
+        { "file_url", &(parsed.file_url), 205, CHAR}
     };
-    static cStruct record = {"set_mag_offsets", members, 5, 151};
+    static cStruct record = {"camera_image_captured", members, 11, 263};
 
-    mavlink_msg_set_mag_offsets_decode(message, &parsed);
+    mavlink_msg_camera_image_captured_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_gimbal_report(const mavlink_message_t* message)
+cStruct* unbox_component_information(const mavlink_message_t* message)
 {
-    static mavlink_gimbal_report_t parsed;
+    static mavlink_component_information_t parsed;
 
     static cMember members[] = {
-        { "delta_time", &(parsed.delta_time), 1, FLOAT},
-        { "delta_angle_x", &(parsed.delta_angle_x), 1, FLOAT},
-        { "delta_angle_y", &(parsed.delta_angle_y), 1, FLOAT},
-        { "delta_angle_z", &(parsed.delta_angle_z), 1, FLOAT},
-        { "delta_velocity_x", &(parsed.delta_velocity_x), 1, FLOAT},
-        { "delta_velocity_y", &(parsed.delta_velocity_y), 1, FLOAT},
-        { "delta_velocity_z", &(parsed.delta_velocity_z), 1, FLOAT},
-        { "joint_roll", &(parsed.joint_roll), 1, FLOAT},
-        { "joint_el", &(parsed.joint_el), 1, FLOAT},
-        { "joint_az", &(parsed.joint_az), 1, FLOAT},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "general_metadata_file_crc", &(parsed.general_metadata_file_crc), 1, UINT32_T},
+        { "peripherals_metadata_file_crc", &(parsed.peripherals_metadata_file_crc), 1, UINT32_T},
+        { "general_metadata_uri", &(parsed.general_metadata_uri), 100, CHAR},
+        { "peripherals_metadata_uri", &(parsed.peripherals_metadata_uri), 100, CHAR}
     };
-    static cStruct record = {"gimbal_report", members, 12, 200};
+    static cStruct record = {"component_information", members, 5, 395};
 
-    mavlink_msg_gimbal_report_decode(message, &parsed);
+    mavlink_msg_component_information_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_gimbal_torque_cmd_report(const mavlink_message_t* message)
+cStruct* unbox_control_system_state(const mavlink_message_t* message)
 {
-    static mavlink_gimbal_torque_cmd_report_t parsed;
+    static mavlink_control_system_state_t parsed;
 
     static cMember members[] = {
-        { "rl_torque_cmd", &(parsed.rl_torque_cmd), 1, INT16_T},
-        { "el_torque_cmd", &(parsed.el_torque_cmd), 1, INT16_T},
-        { "az_torque_cmd", &(parsed.az_torque_cmd), 1, INT16_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "x_acc", &(parsed.x_acc), 1, FLOAT},
+        { "y_acc", &(parsed.y_acc), 1, FLOAT},
+        { "z_acc", &(parsed.z_acc), 1, FLOAT},
+        { "x_vel", &(parsed.x_vel), 1, FLOAT},
+        { "y_vel", &(parsed.y_vel), 1, FLOAT},
+        { "z_vel", &(parsed.z_vel), 1, FLOAT},
+        { "x_pos", &(parsed.x_pos), 1, FLOAT},
+        { "y_pos", &(parsed.y_pos), 1, FLOAT},
+        { "z_pos", &(parsed.z_pos), 1, FLOAT},
+        { "airspeed", &(parsed.airspeed), 1, FLOAT},
+        { "vel_variance", &(parsed.vel_variance), 3, FLOAT},
+        { "pos_variance", &(parsed.pos_variance), 3, FLOAT},
+        { "q", &(parsed.q), 4, FLOAT},
+        { "roll_rate", &(parsed.roll_rate), 1, FLOAT},
+        { "pitch_rate", &(parsed.pitch_rate), 1, FLOAT},
+        { "yaw_rate", &(parsed.yaw_rate), 1, FLOAT}
     };
-    static cStruct record = {"gimbal_torque_cmd_report", members, 5, 214};
+    static cStruct record = {"control_system_state", members, 17, 146};
 
-    mavlink_msg_gimbal_torque_cmd_report_decode(message, &parsed);
+    mavlink_msg_control_system_state_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_simstate(const mavlink_message_t* message)
+cStruct* unbox_cellular_config(const mavlink_message_t* message)
 {
-    static mavlink_simstate_t parsed;
+    static mavlink_cellular_config_t parsed;
 
     static cMember members[] = {
-        { "roll", &(parsed.roll), 1, FLOAT},
-        { "pitch", &(parsed.pitch), 1, FLOAT},
-        { "yaw", &(parsed.yaw), 1, FLOAT},
-        { "xacc", &(parsed.xacc), 1, FLOAT},
-        { "yacc", &(parsed.yacc), 1, FLOAT},
-        { "zacc", &(parsed.zacc), 1, FLOAT},
-        { "xgyro", &(parsed.xgyro), 1, FLOAT},
-        { "ygyro", &(parsed.ygyro), 1, FLOAT},
-        { "zgyro", &(parsed.zgyro), 1, FLOAT},
-        { "lat", &(parsed.lat), 1, INT32_T},
-        { "lng", &(parsed.lng), 1, INT32_T}
+        { "enable_lte", &(parsed.enable_lte), 1, UINT8_T},
+        { "enable_pin", &(parsed.enable_pin), 1, UINT8_T},
+        { "pin", &(parsed.pin), 16, CHAR},
+        { "new_pin", &(parsed.new_pin), 16, CHAR},
+        { "apn", &(parsed.apn), 32, CHAR},
+        { "puk", &(parsed.puk), 16, CHAR},
+        { "roaming", &(parsed.roaming), 1, UINT8_T},
+        { "response", &(parsed.response), 1, UINT8_T}
     };
-    static cStruct record = {"simstate", members, 11, 164};
+    static cStruct record = {"cellular_config", members, 8, 336};
 
-    mavlink_msg_simstate_decode(message, &parsed);
+    mavlink_msg_cellular_config_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_autopilot_version_request(const mavlink_message_t* message)
+cStruct* unbox_uavcan_node_status(const mavlink_message_t* message)
 {
-    static mavlink_autopilot_version_request_t parsed;
+    static mavlink_uavcan_node_status_t parsed;
+
+    static cMember members[] = {
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "uptime_sec", &(parsed.uptime_sec), 1, UINT32_T},
+        { "vendor_specific_status_code", &(parsed.vendor_specific_status_code), 1, UINT16_T},
+        { "health", &(parsed.health), 1, UINT8_T},
+        { "mode", &(parsed.mode), 1, UINT8_T},
+        { "sub_mode", &(parsed.sub_mode), 1, UINT8_T}
+    };
+    static cStruct record = {"uavcan_node_status", members, 6, 310};
+
+    mavlink_msg_uavcan_node_status_decode(message, &parsed);
+    return &record;
+}
+
+cStruct* unbox_distance_sensor(const mavlink_message_t* message)
+{
+    static mavlink_distance_sensor_t parsed;
+
+    static cMember members[] = {
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "min_distance", &(parsed.min_distance), 1, UINT16_T},
+        { "max_distance", &(parsed.max_distance), 1, UINT16_T},
+        { "current_distance", &(parsed.current_distance), 1, UINT16_T},
+        { "type", &(parsed.type), 1, UINT8_T},
+        { "id", &(parsed.id), 1, UINT8_T},
+        { "orientation", &(parsed.orientation), 1, UINT8_T},
+        { "covariance", &(parsed.covariance), 1, UINT8_T},
+        { "horizontal_fov", &(parsed.horizontal_fov), 1, FLOAT},
+        { "vertical_fov", &(parsed.vertical_fov), 1, FLOAT},
+        { "quaternion", &(parsed.quaternion), 4, FLOAT},
+        { "signal_quality", &(parsed.signal_quality), 1, UINT8_T}
+    };
+    static cStruct record = {"distance_sensor", members, 12, 132};
+
+    mavlink_msg_distance_sensor_decode(message, &parsed);
+    return &record;
+}
+
+cStruct* unbox_param_ext_request_list(const mavlink_message_t* message)
+{
+    static mavlink_param_ext_request_list_t parsed;
 
     static cMember members[] = {
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T}
     };
-    static cStruct record = {"autopilot_version_request", members, 2, 183};
+    static cStruct record = {"param_ext_request_list", members, 2, 321};
 
-    mavlink_msg_autopilot_version_request_decode(message, &parsed);
+    mavlink_msg_param_ext_request_list_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_esc_telemetry_5_to_8(const mavlink_message_t* message)
+cStruct* unbox_file_transfer_protocol(const mavlink_message_t* message)
 {
-    static mavlink_esc_telemetry_5_to_8_t parsed;
+    static mavlink_file_transfer_protocol_t parsed;
 
     static cMember members[] = {
-        { "voltage", &(parsed.voltage), 4, UINT16_T},
-        { "current", &(parsed.current), 4, UINT16_T},
-        { "totalcurrent", &(parsed.totalcurrent), 4, UINT16_T},
-        { "rpm", &(parsed.rpm), 4, UINT16_T},
-        { "count", &(parsed.count), 4, UINT16_T},
-        { "temperature", &(parsed.temperature), 4, UINT8_T}
+        { "target_network", &(parsed.target_network), 1, UINT8_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "payload", &(parsed.payload), 251, UINT8_T}
     };
-    static cStruct record = {"esc_telemetry_5_to_8", members, 6, 11031};
+    static cStruct record = {"file_transfer_protocol", members, 4, 110};
 
-    mavlink_msg_esc_telemetry_5_to_8_decode(message, &parsed);
+    mavlink_msg_file_transfer_protocol_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_vision_position_delta(const mavlink_message_t* message)
+cStruct* unbox_gimbal_manager_information(const mavlink_message_t* message)
 {
-    static mavlink_vision_position_delta_t parsed;
+    static mavlink_gimbal_manager_information_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "time_delta_usec", &(parsed.time_delta_usec), 1, UINT64_T},
-        { "angle_delta", &(parsed.angle_delta), 3, FLOAT},
-        { "position_delta", &(parsed.position_delta), 3, FLOAT},
-        { "confidence", &(parsed.confidence), 1, FLOAT}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "cap_flags", &(parsed.cap_flags), 1, UINT32_T},
+        { "roll_min", &(parsed.roll_min), 1, FLOAT},
+        { "roll_max", &(parsed.roll_max), 1, FLOAT},
+        { "pitch_min", &(parsed.pitch_min), 1, FLOAT},
+        { "pitch_max", &(parsed.pitch_max), 1, FLOAT},
+        { "yaw_min", &(parsed.yaw_min), 1, FLOAT},
+        { "yaw_max", &(parsed.yaw_max), 1, FLOAT},
+        { "gimbal_device_id", &(parsed.gimbal_device_id), 1, UINT8_T}
     };
-    static cStruct record = {"vision_position_delta", members, 5, 11011};
+    static cStruct record = {"gimbal_manager_information", members, 9, 280};
 
-    mavlink_msg_vision_position_delta_decode(message, &parsed);
+    mavlink_msg_gimbal_manager_information_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_device_op_read_reply(const mavlink_message_t* message)
+cStruct* unbox_manual_control(const mavlink_message_t* message)
 {
-    static mavlink_device_op_read_reply_t parsed;
+    static mavlink_manual_control_t parsed;
 
     static cMember members[] = {
-        { "request_id", &(parsed.request_id), 1, UINT32_T},
-        { "result", &(parsed.result), 1, UINT8_T},
-        { "regstart", &(parsed.regstart), 1, UINT8_T},
-        { "count", &(parsed.count), 1, UINT8_T},
-        { "data", &(parsed.data), 128, UINT8_T},
-        { "bank", &(parsed.bank), 1, UINT8_T}
+        { "x", &(parsed.x), 1, INT16_T},
+        { "y", &(parsed.y), 1, INT16_T},
+        { "z", &(parsed.z), 1, INT16_T},
+        { "r", &(parsed.r), 1, INT16_T},
+        { "buttons", &(parsed.buttons), 1, UINT16_T},
+        { "target", &(parsed.target), 1, UINT8_T},
+        { "buttons2", &(parsed.buttons2), 1, UINT16_T},
+        { "enabled_extensions", &(parsed.enabled_extensions), 1, UINT8_T},
+        { "s", &(parsed.s), 1, INT16_T},
+        { "t", &(parsed.t), 1, INT16_T}
     };
-    static cStruct record = {"device_op_read_reply", members, 6, 11001};
+    static cStruct record = {"manual_control", members, 10, 69};
 
-    mavlink_msg_device_op_read_reply_decode(message, &parsed);
+    mavlink_msg_manual_control_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_device_op_read(const mavlink_message_t* message)
+cStruct* unbox_setup_signing(const mavlink_message_t* message)
 {
-    static mavlink_device_op_read_t parsed;
+    static mavlink_setup_signing_t parsed;
 
     static cMember members[] = {
-        { "request_id", &(parsed.request_id), 1, UINT32_T},
+        { "initial_timestamp", &(parsed.initial_timestamp), 1, UINT64_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "bustype", &(parsed.bustype), 1, UINT8_T},
-        { "bus", &(parsed.bus), 1, UINT8_T},
-        { "address", &(parsed.address), 1, UINT8_T},
-        { "busname", &(parsed.busname), 40, CHAR},
-        { "regstart", &(parsed.regstart), 1, UINT8_T},
-        { "count", &(parsed.count), 1, UINT8_T},
-        { "bank", &(parsed.bank), 1, UINT8_T}
+        { "secret_key", &(parsed.secret_key), 32, UINT8_T}
     };
-    static cStruct record = {"device_op_read", members, 10, 11000};
+    static cStruct record = {"setup_signing", members, 4, 256};
 
-    mavlink_msg_device_op_read_decode(message, &parsed);
+    mavlink_msg_setup_signing_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_fence_fetch_point(const mavlink_message_t* message)
+cStruct* unbox_statustext(const mavlink_message_t* message)
 {
-    static mavlink_fence_fetch_point_t parsed;
+    static mavlink_statustext_t parsed;
 
     static cMember members[] = {
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "idx", &(parsed.idx), 1, UINT8_T}
+        { "severity", &(parsed.severity), 1, UINT8_T},
+        { "text", &(parsed.text), 50, CHAR},
+        { "id", &(parsed.id), 1, UINT16_T},
+        { "chunk_seq", &(parsed.chunk_seq), 1, UINT8_T}
     };
-    static cStruct record = {"fence_fetch_point", members, 3, 161};
+    static cStruct record = {"statustext", members, 4, 253};
 
-    mavlink_msg_fence_fetch_point_decode(message, &parsed);
+    mavlink_msg_statustext_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_device_op_write(const mavlink_message_t* message)
+cStruct* unbox_command_cancel(const mavlink_message_t* message)
 {
-    static mavlink_device_op_write_t parsed;
+    static mavlink_command_cancel_t parsed;
 
     static cMember members[] = {
-        { "request_id", &(parsed.request_id), 1, UINT32_T},
+        { "command", &(parsed.command), 1, UINT16_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "bustype", &(parsed.bustype), 1, UINT8_T},
-        { "bus", &(parsed.bus), 1, UINT8_T},
-        { "address", &(parsed.address), 1, UINT8_T},
-        { "busname", &(parsed.busname), 40, CHAR},
-        { "regstart", &(parsed.regstart), 1, UINT8_T},
-        { "count", &(parsed.count), 1, UINT8_T},
-        { "data", &(parsed.data), 128, UINT8_T},
-        { "bank", &(parsed.bank), 1, UINT8_T}
+        { "target_component", &(parsed.target_component), 1, UINT8_T}
     };
-    static cStruct record = {"device_op_write", members, 11, 11002};
+    static cStruct record = {"command_cancel", members, 3, 80};
 
-    mavlink_msg_device_op_write_decode(message, &parsed);
+    mavlink_msg_command_cancel_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_ahrs(const mavlink_message_t* message)
+cStruct* unbox_esc_info(const mavlink_message_t* message)
 {
-    static mavlink_ahrs_t parsed;
+    static mavlink_esc_info_t parsed;
 
     static cMember members[] = {
-        { "omegaIx", &(parsed.omegaIx), 1, FLOAT},
-        { "omegaIy", &(parsed.omegaIy), 1, FLOAT},
-        { "omegaIz", &(parsed.omegaIz), 1, FLOAT},
-        { "accel_weight", &(parsed.accel_weight), 1, FLOAT},
-        { "renorm_val", &(parsed.renorm_val), 1, FLOAT},
-        { "error_rp", &(parsed.error_rp), 1, FLOAT},
-        { "error_yaw", &(parsed.error_yaw), 1, FLOAT}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "error_count", &(parsed.error_count), 4, UINT32_T},
+        { "counter", &(parsed.counter), 1, UINT16_T},
+        { "failure_flags", &(parsed.failure_flags), 4, UINT16_T},
+        { "temperature", &(parsed.temperature), 4, INT16_T},
+        { "index", &(parsed.index), 1, UINT8_T},
+        { "count", &(parsed.count), 1, UINT8_T},
+        { "connection_type", &(parsed.connection_type), 1, UINT8_T},
+        { "info", &(parsed.info), 1, UINT8_T}
     };
-    static cStruct record = {"ahrs", members, 7, 163};
+    static cStruct record = {"esc_info", members, 9, 290};
 
-    mavlink_msg_ahrs_decode(message, &parsed);
+    mavlink_msg_esc_info_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_mount_control(const mavlink_message_t* message)
+cStruct* unbox_mission_set_current(const mavlink_message_t* message)
 {
-    static mavlink_mount_control_t parsed;
+    static mavlink_mission_set_current_t parsed;
 
     static cMember members[] = {
-        { "input_a", &(parsed.input_a), 1, INT32_T},
-        { "input_b", &(parsed.input_b), 1, INT32_T},
-        { "input_c", &(parsed.input_c), 1, INT32_T},
+        { "seq", &(parsed.seq), 1, UINT16_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "save_position", &(parsed.save_position), 1, UINT8_T}
+        { "target_component", &(parsed.target_component), 1, UINT8_T}
     };
-    static cStruct record = {"mount_control", members, 6, 157};
+    static cStruct record = {"mission_set_current", members, 3, 41};
 
-    mavlink_msg_mount_control_decode(message, &parsed);
+    mavlink_msg_mission_set_current_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_ekf_status_report(const mavlink_message_t* message)
+cStruct* unbox_utm_global_position(const mavlink_message_t* message)
 {
-    static mavlink_ekf_status_report_t parsed;
+    static mavlink_utm_global_position_t parsed;
 
     static cMember members[] = {
-        { "velocity_variance", &(parsed.velocity_variance), 1, FLOAT},
-        { "pos_horiz_variance", &(parsed.pos_horiz_variance), 1, FLOAT},
-        { "pos_vert_variance", &(parsed.pos_vert_variance), 1, FLOAT},
-        { "compass_variance", &(parsed.compass_variance), 1, FLOAT},
-        { "terrain_alt_variance", &(parsed.terrain_alt_variance), 1, FLOAT},
-        { "flags", &(parsed.flags), 1, UINT16_T},
-        { "airspeed_variance", &(parsed.airspeed_variance), 1, FLOAT}
+        { "time", &(parsed.time), 1, UINT64_T},
+        { "lat", &(parsed.lat), 1, INT32_T},
+        { "lon", &(parsed.lon), 1, INT32_T},
+        { "alt", &(parsed.alt), 1, INT32_T},
+        { "relative_alt", &(parsed.relative_alt), 1, INT32_T},
+        { "next_lat", &(parsed.next_lat), 1, INT32_T},
+        { "next_lon", &(parsed.next_lon), 1, INT32_T},
+        { "next_alt", &(parsed.next_alt), 1, INT32_T},
+        { "vx", &(parsed.vx), 1, INT16_T},
+        { "vy", &(parsed.vy), 1, INT16_T},
+        { "vz", &(parsed.vz), 1, INT16_T},
+        { "h_acc", &(parsed.h_acc), 1, UINT16_T},
+        { "v_acc", &(parsed.v_acc), 1, UINT16_T},
+        { "vel_acc", &(parsed.vel_acc), 1, UINT16_T},
+        { "update_rate", &(parsed.update_rate), 1, UINT16_T},
+        { "uas_id", &(parsed.uas_id), 18, UINT8_T},
+        { "flight_state", &(parsed.flight_state), 1, UINT8_T},
+        { "flags", &(parsed.flags), 1, UINT8_T}
     };
-    static cStruct record = {"ekf_status_report", members, 7, 193};
+    static cStruct record = {"utm_global_position", members, 18, 340};
 
-    mavlink_msg_ekf_status_report_decode(message, &parsed);
+    mavlink_msg_utm_global_position_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_camera_feedback(const mavlink_message_t* message)
+cStruct* unbox_gimbal_manager_set_pitchyaw(const mavlink_message_t* message)
 {
-    static mavlink_camera_feedback_t parsed;
+    static mavlink_gimbal_manager_set_pitchyaw_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "lat", &(parsed.lat), 1, INT32_T},
-        { "lng", &(parsed.lng), 1, INT32_T},
-        { "alt_msl", &(parsed.alt_msl), 1, FLOAT},
-        { "alt_rel", &(parsed.alt_rel), 1, FLOAT},
-        { "roll", &(parsed.roll), 1, FLOAT},
+        { "flags", &(parsed.flags), 1, UINT32_T},
         { "pitch", &(parsed.pitch), 1, FLOAT},
         { "yaw", &(parsed.yaw), 1, FLOAT},
-        { "foc_len", &(parsed.foc_len), 1, FLOAT},
-        { "img_idx", &(parsed.img_idx), 1, UINT16_T},
+        { "pitch_rate", &(parsed.pitch_rate), 1, FLOAT},
+        { "yaw_rate", &(parsed.yaw_rate), 1, FLOAT},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "cam_idx", &(parsed.cam_idx), 1, UINT8_T},
-        { "flags", &(parsed.flags), 1, UINT8_T},
-        { "completed_captures", &(parsed.completed_captures), 1, UINT16_T}
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "gimbal_device_id", &(parsed.gimbal_device_id), 1, UINT8_T}
     };
-    static cStruct record = {"camera_feedback", members, 14, 180};
+    static cStruct record = {"gimbal_manager_set_pitchyaw", members, 8, 287};
 
-    mavlink_msg_camera_feedback_decode(message, &parsed);
+    mavlink_msg_gimbal_manager_set_pitchyaw_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_gopro_set_request(const mavlink_message_t* message)
+cStruct* unbox_power_status(const mavlink_message_t* message)
 {
-    static mavlink_gopro_set_request_t parsed;
+    static mavlink_power_status_t parsed;
 
     static cMember members[] = {
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "cmd_id", &(parsed.cmd_id), 1, UINT8_T},
-        { "value", &(parsed.value), 4, UINT8_T}
+        { "Vcc", &(parsed.Vcc), 1, UINT16_T},
+        { "Vservo", &(parsed.Vservo), 1, UINT16_T},
+        { "flags", &(parsed.flags), 1, UINT16_T}
     };
-    static cStruct record = {"gopro_set_request", members, 4, 218};
+    static cStruct record = {"power_status", members, 3, 125};
 
-    mavlink_msg_gopro_set_request_decode(message, &parsed);
+    mavlink_msg_power_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_mount_status(const mavlink_message_t* message)
+cStruct* unbox_param_request_read(const mavlink_message_t* message)
 {
-    static mavlink_mount_status_t parsed;
+    static mavlink_param_request_read_t parsed;
 
     static cMember members[] = {
-        { "pointing_a", &(parsed.pointing_a), 1, INT32_T},
-        { "pointing_b", &(parsed.pointing_b), 1, INT32_T},
-        { "pointing_c", &(parsed.pointing_c), 1, INT32_T},
+        { "param_index", &(parsed.param_index), 1, INT16_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "mount_mode", &(parsed.mount_mode), 1, UINT8_T}
+        { "param_id", &(parsed.param_id), 16, CHAR}
     };
-    static cStruct record = {"mount_status", members, 6, 158};
+    static cStruct record = {"param_request_read", members, 4, 20};
 
-    mavlink_msg_mount_status_decode(message, &parsed);
+    mavlink_msg_param_request_read_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_gopro_heartbeat(const mavlink_message_t* message)
+cStruct* unbox_camera_fov_status(const mavlink_message_t* message)
 {
-    static mavlink_gopro_heartbeat_t parsed;
+    static mavlink_camera_fov_status_t parsed;
 
     static cMember members[] = {
-        { "status", &(parsed.status), 1, UINT8_T},
-        { "capture_mode", &(parsed.capture_mode), 1, UINT8_T},
-        { "flags", &(parsed.flags), 1, UINT8_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "lat_camera", &(parsed.lat_camera), 1, INT32_T},
+        { "lon_camera", &(parsed.lon_camera), 1, INT32_T},
+        { "alt_camera", &(parsed.alt_camera), 1, INT32_T},
+        { "lat_image", &(parsed.lat_image), 1, INT32_T},
+        { "lon_image", &(parsed.lon_image), 1, INT32_T},
+        { "alt_image", &(parsed.alt_image), 1, INT32_T},
+        { "q", &(parsed.q), 4, FLOAT},
+        { "hfov", &(parsed.hfov), 1, FLOAT},
+        { "vfov", &(parsed.vfov), 1, FLOAT}
     };
-    static cStruct record = {"gopro_heartbeat", members, 3, 215};
+    static cStruct record = {"camera_fov_status", members, 10, 271};
 
-    mavlink_msg_gopro_heartbeat_decode(message, &parsed);
+    mavlink_msg_camera_fov_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_data64(const mavlink_message_t* message)
+cStruct* unbox_mission_current(const mavlink_message_t* message)
 {
-    static mavlink_data64_t parsed;
+    static mavlink_mission_current_t parsed;
 
     static cMember members[] = {
-        { "type", &(parsed.type), 1, UINT8_T},
-        { "len", &(parsed.len), 1, UINT8_T},
-        { "data", &(parsed.data), 64, UINT8_T}
+        { "seq", &(parsed.seq), 1, UINT16_T},
+        { "total", &(parsed.total), 1, UINT16_T},
+        { "mission_state", &(parsed.mission_state), 1, UINT8_T},
+        { "mission_mode", &(parsed.mission_mode), 1, UINT8_T}
     };
-    static cStruct record = {"data64", members, 3, 171};
+    static cStruct record = {"mission_current", members, 4, 42};
 
-    mavlink_msg_data64_decode(message, &parsed);
+    mavlink_msg_mission_current_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_gimbal_control(const mavlink_message_t* message)
+cStruct* unbox_mount_orientation(const mavlink_message_t* message)
 {
-    static mavlink_gimbal_control_t parsed;
+    static mavlink_mount_orientation_t parsed;
 
     static cMember members[] = {
-        { "demanded_rate_x", &(parsed.demanded_rate_x), 1, FLOAT},
-        { "demanded_rate_y", &(parsed.demanded_rate_y), 1, FLOAT},
-        { "demanded_rate_z", &(parsed.demanded_rate_z), 1, FLOAT},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "roll", &(parsed.roll), 1, FLOAT},
+        { "pitch", &(parsed.pitch), 1, FLOAT},
+        { "yaw", &(parsed.yaw), 1, FLOAT},
+        { "yaw_absolute", &(parsed.yaw_absolute), 1, FLOAT}
     };
-    static cStruct record = {"gimbal_control", members, 5, 201};
+    static cStruct record = {"mount_orientation", members, 5, 265};
 
-    mavlink_msg_gimbal_control_decode(message, &parsed);
+    mavlink_msg_mount_orientation_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_mcu_status(const mavlink_message_t* message)
+cStruct* unbox_attitude(const mavlink_message_t* message)
 {
-    static mavlink_mcu_status_t parsed;
+    static mavlink_attitude_t parsed;
 
     static cMember members[] = {
-        { "MCU_temperature", &(parsed.MCU_temperature), 1, INT16_T},
-        { "MCU_voltage", &(parsed.MCU_voltage), 1, UINT16_T},
-        { "MCU_voltage_min", &(parsed.MCU_voltage_min), 1, UINT16_T},
-        { "MCU_voltage_max", &(parsed.MCU_voltage_max), 1, UINT16_T},
-        { "id", &(parsed.id), 1, UINT8_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "roll", &(parsed.roll), 1, FLOAT},
+        { "pitch", &(parsed.pitch), 1, FLOAT},
+        { "yaw", &(parsed.yaw), 1, FLOAT},
+        { "rollspeed", &(parsed.rollspeed), 1, FLOAT},
+        { "pitchspeed", &(parsed.pitchspeed), 1, FLOAT},
+        { "yawspeed", &(parsed.yawspeed), 1, FLOAT}
     };
-    static cStruct record = {"mcu_status", members, 5, 11039};
+    static cStruct record = {"attitude", members, 7, 30};
 
-    mavlink_msg_mcu_status_decode(message, &parsed);
+    mavlink_msg_attitude_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_aoa_ssa(const mavlink_message_t* message)
+cStruct* unbox_hygrometer_sensor(const mavlink_message_t* message)
 {
-    static mavlink_aoa_ssa_t parsed;
+    static mavlink_hygrometer_sensor_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "AOA", &(parsed.AOA), 1, FLOAT},
-        { "SSA", &(parsed.SSA), 1, FLOAT}
+        { "temperature", &(parsed.temperature), 1, INT16_T},
+        { "humidity", &(parsed.humidity), 1, UINT16_T},
+        { "id", &(parsed.id), 1, UINT8_T}
     };
-    static cStruct record = {"aoa_ssa", members, 3, 11020};
+    static cStruct record = {"hygrometer_sensor", members, 3, 12920};
 
-    mavlink_msg_aoa_ssa_decode(message, &parsed);
+    mavlink_msg_hygrometer_sensor_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_rpm(const mavlink_message_t* message)
+cStruct* unbox_terrain_report(const mavlink_message_t* message)
 {
-    static mavlink_rpm_t parsed;
+    static mavlink_terrain_report_t parsed;
 
     static cMember members[] = {
-        { "rpm1", &(parsed.rpm1), 1, FLOAT},
-        { "rpm2", &(parsed.rpm2), 1, FLOAT}
+        { "lat", &(parsed.lat), 1, INT32_T},
+        { "lon", &(parsed.lon), 1, INT32_T},
+        { "terrain_height", &(parsed.terrain_height), 1, FLOAT},
+        { "current_height", &(parsed.current_height), 1, FLOAT},
+        { "spacing", &(parsed.spacing), 1, UINT16_T},
+        { "pending", &(parsed.pending), 1, UINT16_T},
+        { "loaded", &(parsed.loaded), 1, UINT16_T}
     };
-    static cStruct record = {"rpm", members, 2, 226};
+    static cStruct record = {"terrain_report", members, 7, 136};
 
-    mavlink_msg_rpm_decode(message, &parsed);
+    mavlink_msg_terrain_report_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_rally_point(const mavlink_message_t* message)
+cStruct* unbox_hil_sensor(const mavlink_message_t* message)
 {
-    static mavlink_rally_point_t parsed;
+    static mavlink_hil_sensor_t parsed;
 
     static cMember members[] = {
-        { "lat", &(parsed.lat), 1, INT32_T},
-        { "lng", &(parsed.lng), 1, INT32_T},
-        { "alt", &(parsed.alt), 1, INT16_T},
-        { "break_alt", &(parsed.break_alt), 1, INT16_T},
-        { "land_dir", &(parsed.land_dir), 1, UINT16_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "idx", &(parsed.idx), 1, UINT8_T},
-        { "count", &(parsed.count), 1, UINT8_T},
-        { "flags", &(parsed.flags), 1, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "xacc", &(parsed.xacc), 1, FLOAT},
+        { "yacc", &(parsed.yacc), 1, FLOAT},
+        { "zacc", &(parsed.zacc), 1, FLOAT},
+        { "xgyro", &(parsed.xgyro), 1, FLOAT},
+        { "ygyro", &(parsed.ygyro), 1, FLOAT},
+        { "zgyro", &(parsed.zgyro), 1, FLOAT},
+        { "xmag", &(parsed.xmag), 1, FLOAT},
+        { "ymag", &(parsed.ymag), 1, FLOAT},
+        { "zmag", &(parsed.zmag), 1, FLOAT},
+        { "abs_pressure", &(parsed.abs_pressure), 1, FLOAT},
+        { "diff_pressure", &(parsed.diff_pressure), 1, FLOAT},
+        { "pressure_alt", &(parsed.pressure_alt), 1, FLOAT},
+        { "temperature", &(parsed.temperature), 1, FLOAT},
+        { "fields_updated", &(parsed.fields_updated), 1, UINT32_T},
+        { "id", &(parsed.id), 1, UINT8_T}
     };
-    static cStruct record = {"rally_point", members, 10, 175};
+    static cStruct record = {"hil_sensor", members, 16, 107};
 
-    mavlink_msg_rally_point_decode(message, &parsed);
+    mavlink_msg_hil_sensor_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_data16(const mavlink_message_t* message)
+cStruct* unbox_vibration(const mavlink_message_t* message)
 {
-    static mavlink_data16_t parsed;
+    static mavlink_vibration_t parsed;
 
     static cMember members[] = {
-        { "type", &(parsed.type), 1, UINT8_T},
-        { "len", &(parsed.len), 1, UINT8_T},
-        { "data", &(parsed.data), 16, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "vibration_x", &(parsed.vibration_x), 1, FLOAT},
+        { "vibration_y", &(parsed.vibration_y), 1, FLOAT},
+        { "vibration_z", &(parsed.vibration_z), 1, FLOAT},
+        { "clipping_0", &(parsed.clipping_0), 1, UINT32_T},
+        { "clipping_1", &(parsed.clipping_1), 1, UINT32_T},
+        { "clipping_2", &(parsed.clipping_2), 1, UINT32_T}
     };
-    static cStruct record = {"data16", members, 3, 169};
+    static cStruct record = {"vibration", members, 7, 241};
 
-    mavlink_msg_data16_decode(message, &parsed);
+    mavlink_msg_vibration_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_limits_status(const mavlink_message_t* message)
+cStruct* unbox_scaled_pressure3(const mavlink_message_t* message)
 {
-    static mavlink_limits_status_t parsed;
+    static mavlink_scaled_pressure3_t parsed;
 
     static cMember members[] = {
-        { "last_trigger", &(parsed.last_trigger), 1, UINT32_T},
-        { "last_action", &(parsed.last_action), 1, UINT32_T},
-        { "last_recovery", &(parsed.last_recovery), 1, UINT32_T},
-        { "last_clear", &(parsed.last_clear), 1, UINT32_T},
-        { "breach_count", &(parsed.breach_count), 1, UINT16_T},
-        { "limits_state", &(parsed.limits_state), 1, UINT8_T},
-        { "mods_enabled", &(parsed.mods_enabled), 1, UINT8_T},
-        { "mods_required", &(parsed.mods_required), 1, UINT8_T},
-        { "mods_triggered", &(parsed.mods_triggered), 1, UINT8_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "press_abs", &(parsed.press_abs), 1, FLOAT},
+        { "press_diff", &(parsed.press_diff), 1, FLOAT},
+        { "temperature", &(parsed.temperature), 1, INT16_T},
+        { "temperature_press_diff", &(parsed.temperature_press_diff), 1, INT16_T}
     };
-    static cStruct record = {"limits_status", members, 9, 167};
+    static cStruct record = {"scaled_pressure3", members, 5, 143};
 
-    mavlink_msg_limits_status_decode(message, &parsed);
+    mavlink_msg_scaled_pressure3_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_pid_tuning(const mavlink_message_t* message)
+cStruct* unbox_change_operator_control_ack(const mavlink_message_t* message)
 {
-    static mavlink_pid_tuning_t parsed;
+    static mavlink_change_operator_control_ack_t parsed;
 
     static cMember members[] = {
-        { "desired", &(parsed.desired), 1, FLOAT},
-        { "achieved", &(parsed.achieved), 1, FLOAT},
-        { "FF", &(parsed.FF), 1, FLOAT},
-        { "P", &(parsed.P), 1, FLOAT},
-        { "I", &(parsed.I), 1, FLOAT},
-        { "D", &(parsed.D), 1, FLOAT},
-        { "axis", &(parsed.axis), 1, UINT8_T},
-        { "SRate", &(parsed.SRate), 1, FLOAT},
-        { "PDmod", &(parsed.PDmod), 1, FLOAT}
+        { "gcs_system_id", &(parsed.gcs_system_id), 1, UINT8_T},
+        { "control_request", &(parsed.control_request), 1, UINT8_T},
+        { "ack", &(parsed.ack), 1, UINT8_T}
     };
-    static cStruct record = {"pid_tuning", members, 9, 194};
+    static cStruct record = {"change_operator_control_ack", members, 3, 6};
 
-    mavlink_msg_pid_tuning_decode(message, &parsed);
+    mavlink_msg_change_operator_control_ack_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_digicam_control(const mavlink_message_t* message)
+cStruct* unbox_v2_extension(const mavlink_message_t* message)
 {
-    static mavlink_digicam_control_t parsed;
+    static mavlink_v2_extension_t parsed;
 
     static cMember members[] = {
-        { "extra_value", &(parsed.extra_value), 1, FLOAT},
+        { "message_type", &(parsed.message_type), 1, UINT16_T},
+        { "target_network", &(parsed.target_network), 1, UINT8_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "session", &(parsed.session), 1, UINT8_T},
-        { "zoom_pos", &(parsed.zoom_pos), 1, UINT8_T},
-        { "zoom_step", &(parsed.zoom_step), 1, INT8_T},
-        { "focus_lock", &(parsed.focus_lock), 1, UINT8_T},
-        { "shot", &(parsed.shot), 1, UINT8_T},
-        { "command_id", &(parsed.command_id), 1, UINT8_T},
-        { "extra_param", &(parsed.extra_param), 1, UINT8_T}
+        { "payload", &(parsed.payload), 249, UINT8_T}
     };
-    static cStruct record = {"digicam_control", members, 10, 155};
+    static cStruct record = {"v2_extension", members, 5, 248};
 
-    mavlink_msg_digicam_control_decode(message, &parsed);
+    mavlink_msg_v2_extension_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_wind(const mavlink_message_t* message)
+cStruct* unbox_event(const mavlink_message_t* message)
 {
-    static mavlink_wind_t parsed;
+    static mavlink_event_t parsed;
 
     static cMember members[] = {
-        { "direction", &(parsed.direction), 1, FLOAT},
-        { "speed", &(parsed.speed), 1, FLOAT},
-        { "speed_z", &(parsed.speed_z), 1, FLOAT}
+        { "id", &(parsed.id), 1, UINT32_T},
+        { "event_time_boot_ms", &(parsed.event_time_boot_ms), 1, UINT32_T},
+        { "sequence", &(parsed.sequence), 1, UINT16_T},
+        { "destination_component", &(parsed.destination_component), 1, UINT8_T},
+        { "destination_system", &(parsed.destination_system), 1, UINT8_T},
+        { "log_levels", &(parsed.log_levels), 1, UINT8_T},
+        { "arguments", &(parsed.arguments), 40, UINT8_T}
     };
-    static cStruct record = {"wind", members, 3, 168};
+    static cStruct record = {"event", members, 7, 410};
 
-    mavlink_msg_wind_decode(message, &parsed);
+    mavlink_msg_event_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_gopro_set_response(const mavlink_message_t* message)
+cStruct* unbox_video_stream_status(const mavlink_message_t* message)
 {
-    static mavlink_gopro_set_response_t parsed;
+    static mavlink_video_stream_status_t parsed;
 
     static cMember members[] = {
-        { "cmd_id", &(parsed.cmd_id), 1, UINT8_T},
-        { "status", &(parsed.status), 1, UINT8_T}
+        { "framerate", &(parsed.framerate), 1, FLOAT},
+        { "bitrate", &(parsed.bitrate), 1, UINT32_T},
+        { "flags", &(parsed.flags), 1, UINT16_T},
+        { "resolution_h", &(parsed.resolution_h), 1, UINT16_T},
+        { "resolution_v", &(parsed.resolution_v), 1, UINT16_T},
+        { "rotation", &(parsed.rotation), 1, UINT16_T},
+        { "hfov", &(parsed.hfov), 1, UINT16_T},
+        { "stream_id", &(parsed.stream_id), 1, UINT8_T}
     };
-    static cStruct record = {"gopro_set_response", members, 2, 219};
+    static cStruct record = {"video_stream_status", members, 8, 270};
 
-    mavlink_msg_gopro_set_response_decode(message, &parsed);
+    mavlink_msg_video_stream_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_compassmot_status(const mavlink_message_t* message)
+cStruct* unbox_log_request_end(const mavlink_message_t* message)
 {
-    static mavlink_compassmot_status_t parsed;
+    static mavlink_log_request_end_t parsed;
 
     static cMember members[] = {
-        { "current", &(parsed.current), 1, FLOAT},
-        { "CompensationX", &(parsed.CompensationX), 1, FLOAT},
-        { "CompensationY", &(parsed.CompensationY), 1, FLOAT},
-        { "CompensationZ", &(parsed.CompensationZ), 1, FLOAT},
-        { "throttle", &(parsed.throttle), 1, UINT16_T},
-        { "interference", &(parsed.interference), 1, UINT16_T}
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T}
     };
-    static cStruct record = {"compassmot_status", members, 6, 177};
+    static cStruct record = {"log_request_end", members, 2, 122};
 
-    mavlink_msg_compassmot_status_decode(message, &parsed);
+    mavlink_msg_log_request_end_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_ahrs3(const mavlink_message_t* message)
+cStruct* unbox_actuator_output_status(const mavlink_message_t* message)
 {
-    static mavlink_ahrs3_t parsed;
+    static mavlink_actuator_output_status_t parsed;
 
     static cMember members[] = {
-        { "roll", &(parsed.roll), 1, FLOAT},
-        { "pitch", &(parsed.pitch), 1, FLOAT},
-        { "yaw", &(parsed.yaw), 1, FLOAT},
-        { "altitude", &(parsed.altitude), 1, FLOAT},
-        { "lat", &(parsed.lat), 1, INT32_T},
-        { "lng", &(parsed.lng), 1, INT32_T},
-        { "v1", &(parsed.v1), 1, FLOAT},
-        { "v2", &(parsed.v2), 1, FLOAT},
-        { "v3", &(parsed.v3), 1, FLOAT},
-        { "v4", &(parsed.v4), 1, FLOAT}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "active", &(parsed.active), 1, UINT32_T},
+        { "actuator", &(parsed.actuator), 32, FLOAT}
     };
-    static cStruct record = {"ahrs3", members, 10, 182};
+    static cStruct record = {"actuator_output_status", members, 3, 375};
 
-    mavlink_msg_ahrs3_decode(message, &parsed);
+    mavlink_msg_actuator_output_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_remote_log_block_status(const mavlink_message_t* message)
+cStruct* unbox_esc_status(const mavlink_message_t* message)
 {
-    static mavlink_remote_log_block_status_t parsed;
+    static mavlink_esc_status_t parsed;
 
     static cMember members[] = {
-        { "seqno", &(parsed.seqno), 1, UINT32_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "status", &(parsed.status), 1, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "rpm", &(parsed.rpm), 4, INT32_T},
+        { "voltage", &(parsed.voltage), 4, FLOAT},
+        { "current", &(parsed.current), 4, FLOAT},
+        { "index", &(parsed.index), 1, UINT8_T}
     };
-    static cStruct record = {"remote_log_block_status", members, 4, 185};
+    static cStruct record = {"esc_status", members, 5, 291};
 
-    mavlink_msg_remote_log_block_status_decode(message, &parsed);
+    mavlink_msg_esc_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_rally_fetch_point(const mavlink_message_t* message)
+cStruct* unbox_scaled_pressure2(const mavlink_message_t* message)
 {
-    static mavlink_rally_fetch_point_t parsed;
+    static mavlink_scaled_pressure2_t parsed;
 
     static cMember members[] = {
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "idx", &(parsed.idx), 1, UINT8_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "press_abs", &(parsed.press_abs), 1, FLOAT},
+        { "press_diff", &(parsed.press_diff), 1, FLOAT},
+        { "temperature", &(parsed.temperature), 1, INT16_T},
+        { "temperature_press_diff", &(parsed.temperature_press_diff), 1, INT16_T}
     };
-    static cStruct record = {"rally_fetch_point", members, 3, 176};
+    static cStruct record = {"scaled_pressure2", members, 5, 137};
 
-    mavlink_msg_rally_fetch_point_decode(message, &parsed);
+    mavlink_msg_scaled_pressure2_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_ahrs2(const mavlink_message_t* message)
+cStruct* unbox_set_mode(const mavlink_message_t* message)
 {
-    static mavlink_ahrs2_t parsed;
+    static mavlink_set_mode_t parsed;
 
     static cMember members[] = {
-        { "roll", &(parsed.roll), 1, FLOAT},
-        { "pitch", &(parsed.pitch), 1, FLOAT},
-        { "yaw", &(parsed.yaw), 1, FLOAT},
-        { "altitude", &(parsed.altitude), 1, FLOAT},
-        { "lat", &(parsed.lat), 1, INT32_T},
-        { "lng", &(parsed.lng), 1, INT32_T}
+        { "custom_mode", &(parsed.custom_mode), 1, UINT32_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "base_mode", &(parsed.base_mode), 1, UINT8_T}
     };
-    static cStruct record = {"ahrs2", members, 6, 178};
+    static cStruct record = {"set_mode", members, 3, 11};
 
-    mavlink_msg_ahrs2_decode(message, &parsed);
+    mavlink_msg_set_mode_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_osd_param_show_config(const mavlink_message_t* message)
+cStruct* unbox_global_position_int(const mavlink_message_t* message)
 {
-    static mavlink_osd_param_show_config_t parsed;
+    static mavlink_global_position_int_t parsed;
 
     static cMember members[] = {
-        { "request_id", &(parsed.request_id), 1, UINT32_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "osd_screen", &(parsed.osd_screen), 1, UINT8_T},
-        { "osd_index", &(parsed.osd_index), 1, UINT8_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "lat", &(parsed.lat), 1, INT32_T},
+        { "lon", &(parsed.lon), 1, INT32_T},
+        { "alt", &(parsed.alt), 1, INT32_T},
+        { "relative_alt", &(parsed.relative_alt), 1, INT32_T},
+        { "vx", &(parsed.vx), 1, INT16_T},
+        { "vy", &(parsed.vy), 1, INT16_T},
+        { "vz", &(parsed.vz), 1, INT16_T},
+        { "hdg", &(parsed.hdg), 1, UINT16_T}
     };
-    static cStruct record = {"osd_param_show_config", members, 5, 11035};
+    static cStruct record = {"global_position_int", members, 9, 33};
 
-    mavlink_msg_osd_param_show_config_decode(message, &parsed);
+    mavlink_msg_global_position_int_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_deepstall(const mavlink_message_t* message)
+cStruct* unbox_canfd_frame(const mavlink_message_t* message)
 {
-    static mavlink_deepstall_t parsed;
+    static mavlink_canfd_frame_t parsed;
 
     static cMember members[] = {
-        { "landing_lat", &(parsed.landing_lat), 1, INT32_T},
-        { "landing_lon", &(parsed.landing_lon), 1, INT32_T},
-        { "path_lat", &(parsed.path_lat), 1, INT32_T},
-        { "path_lon", &(parsed.path_lon), 1, INT32_T},
-        { "arc_entry_lat", &(parsed.arc_entry_lat), 1, INT32_T},
-        { "arc_entry_lon", &(parsed.arc_entry_lon), 1, INT32_T},
-        { "altitude", &(parsed.altitude), 1, FLOAT},
-        { "expected_travel_distance", &(parsed.expected_travel_distance), 1, FLOAT},
-        { "cross_track_error", &(parsed.cross_track_error), 1, FLOAT},
-        { "stage", &(parsed.stage), 1, UINT8_T}
+        { "id", &(parsed.id), 1, UINT32_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "bus", &(parsed.bus), 1, UINT8_T},
+        { "len", &(parsed.len), 1, UINT8_T},
+        { "data", &(parsed.data), 64, UINT8_T}
     };
-    static cStruct record = {"deepstall", members, 10, 195};
+    static cStruct record = {"canfd_frame", members, 6, 387};
 
-    mavlink_msg_deepstall_decode(message, &parsed);
+    mavlink_msg_canfd_frame_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_device_op_write_reply(const mavlink_message_t* message)
+cStruct* unbox_optical_flow_rad(const mavlink_message_t* message)
 {
-    static mavlink_device_op_write_reply_t parsed;
+    static mavlink_optical_flow_rad_t parsed;
 
     static cMember members[] = {
-        { "request_id", &(parsed.request_id), 1, UINT32_T},
-        { "result", &(parsed.result), 1, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "integration_time_us", &(parsed.integration_time_us), 1, UINT32_T},
+        { "integrated_x", &(parsed.integrated_x), 1, FLOAT},
+        { "integrated_y", &(parsed.integrated_y), 1, FLOAT},
+        { "integrated_xgyro", &(parsed.integrated_xgyro), 1, FLOAT},
+        { "integrated_ygyro", &(parsed.integrated_ygyro), 1, FLOAT},
+        { "integrated_zgyro", &(parsed.integrated_zgyro), 1, FLOAT},
+        { "time_delta_distance_us", &(parsed.time_delta_distance_us), 1, UINT32_T},
+        { "distance", &(parsed.distance), 1, FLOAT},
+        { "temperature", &(parsed.temperature), 1, INT16_T},
+        { "sensor_id", &(parsed.sensor_id), 1, UINT8_T},
+        { "quality", &(parsed.quality), 1, UINT8_T}
     };
-    static cStruct record = {"device_op_write_reply", members, 2, 11003};
+    static cStruct record = {"optical_flow_rad", members, 12, 106};
 
-    mavlink_msg_device_op_write_reply_decode(message, &parsed);
+    mavlink_msg_optical_flow_rad_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_osd_param_config_reply(const mavlink_message_t* message)
+cStruct* unbox_gps_global_origin(const mavlink_message_t* message)
 {
-    static mavlink_osd_param_config_reply_t parsed;
+    static mavlink_gps_global_origin_t parsed;
 
     static cMember members[] = {
-        { "request_id", &(parsed.request_id), 1, UINT32_T},
-        { "result", &(parsed.result), 1, UINT8_T}
+        { "latitude", &(parsed.latitude), 1, INT32_T},
+        { "longitude", &(parsed.longitude), 1, INT32_T},
+        { "altitude", &(parsed.altitude), 1, INT32_T},
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T}
     };
-    static cStruct record = {"osd_param_config_reply", members, 2, 11034};
+    static cStruct record = {"gps_global_origin", members, 4, 49};
 
-    mavlink_msg_osd_param_config_reply_decode(message, &parsed);
+    mavlink_msg_gps_global_origin_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_camera_status(const mavlink_message_t* message)
+cStruct* unbox_high_latency(const mavlink_message_t* message)
 {
-    static mavlink_camera_status_t parsed;
+    static mavlink_high_latency_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "p1", &(parsed.p1), 1, FLOAT},
-        { "p2", &(parsed.p2), 1, FLOAT},
-        { "p3", &(parsed.p3), 1, FLOAT},
-        { "p4", &(parsed.p4), 1, FLOAT},
-        { "img_idx", &(parsed.img_idx), 1, UINT16_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "cam_idx", &(parsed.cam_idx), 1, UINT8_T},
-        { "event_id", &(parsed.event_id), 1, UINT8_T}
+        { "custom_mode", &(parsed.custom_mode), 1, UINT32_T},
+        { "latitude", &(parsed.latitude), 1, INT32_T},
+        { "longitude", &(parsed.longitude), 1, INT32_T},
+        { "roll", &(parsed.roll), 1, INT16_T},
+        { "pitch", &(parsed.pitch), 1, INT16_T},
+        { "heading", &(parsed.heading), 1, UINT16_T},
+        { "heading_sp", &(parsed.heading_sp), 1, INT16_T},
+        { "altitude_amsl", &(parsed.altitude_amsl), 1, INT16_T},
+        { "altitude_sp", &(parsed.altitude_sp), 1, INT16_T},
+        { "wp_distance", &(parsed.wp_distance), 1, UINT16_T},
+        { "base_mode", &(parsed.base_mode), 1, UINT8_T},
+        { "landed_state", &(parsed.landed_state), 1, UINT8_T},
+        { "throttle", &(parsed.throttle), 1, INT8_T},
+        { "airspeed", &(parsed.airspeed), 1, UINT8_T},
+        { "airspeed_sp", &(parsed.airspeed_sp), 1, UINT8_T},
+        { "groundspeed", &(parsed.groundspeed), 1, UINT8_T},
+        { "climb_rate", &(parsed.climb_rate), 1, INT8_T},
+        { "gps_nsat", &(parsed.gps_nsat), 1, UINT8_T},
+        { "gps_fix_type", &(parsed.gps_fix_type), 1, UINT8_T},
+        { "battery_remaining", &(parsed.battery_remaining), 1, UINT8_T},
+        { "temperature", &(parsed.temperature), 1, INT8_T},
+        { "temperature_air", &(parsed.temperature_air), 1, INT8_T},
+        { "failsafe", &(parsed.failsafe), 1, UINT8_T},
+        { "wp_num", &(parsed.wp_num), 1, UINT8_T}
     };
-    static cStruct record = {"camera_status", members, 9, 179};
+    static cStruct record = {"high_latency", members, 24, 234};
 
-    mavlink_msg_camera_status_decode(message, &parsed);
+    mavlink_msg_high_latency_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_fence_point(const mavlink_message_t* message)
+cStruct* unbox_param_value(const mavlink_message_t* message)
 {
-    static mavlink_fence_point_t parsed;
+    static mavlink_param_value_t parsed;
 
     static cMember members[] = {
-        { "lat", &(parsed.lat), 1, FLOAT},
-        { "lng", &(parsed.lng), 1, FLOAT},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "idx", &(parsed.idx), 1, UINT8_T},
-        { "count", &(parsed.count), 1, UINT8_T}
+        { "param_value", &(parsed.param_value), 1, FLOAT},
+        { "param_count", &(parsed.param_count), 1, UINT16_T},
+        { "param_index", &(parsed.param_index), 1, UINT16_T},
+        { "param_id", &(parsed.param_id), 16, CHAR},
+        { "param_type", &(parsed.param_type), 1, UINT8_T}
     };
-    static cStruct record = {"fence_point", members, 6, 160};
+    static cStruct record = {"param_value", members, 5, 22};
 
-    mavlink_msg_fence_point_decode(message, &parsed);
+    mavlink_msg_param_value_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_radio(const mavlink_message_t* message)
+cStruct* unbox_attitude_target(const mavlink_message_t* message)
 {
-    static mavlink_radio_t parsed;
+    static mavlink_attitude_target_t parsed;
 
     static cMember members[] = {
-        { "rxerrors", &(parsed.rxerrors), 1, UINT16_T},
-        { "fixed", &(parsed.fixed), 1, UINT16_T},
-        { "rssi", &(parsed.rssi), 1, UINT8_T},
-        { "remrssi", &(parsed.remrssi), 1, UINT8_T},
-        { "txbuf", &(parsed.txbuf), 1, UINT8_T},
-        { "noise", &(parsed.noise), 1, UINT8_T},
-        { "remnoise", &(parsed.remnoise), 1, UINT8_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "q", &(parsed.q), 4, FLOAT},
+        { "body_roll_rate", &(parsed.body_roll_rate), 1, FLOAT},
+        { "body_pitch_rate", &(parsed.body_pitch_rate), 1, FLOAT},
+        { "body_yaw_rate", &(parsed.body_yaw_rate), 1, FLOAT},
+        { "thrust", &(parsed.thrust), 1, FLOAT},
+        { "type_mask", &(parsed.type_mask), 1, UINT8_T}
     };
-    static cStruct record = {"radio", members, 7, 166};
+    static cStruct record = {"attitude_target", members, 7, 83};
 
-    mavlink_msg_radio_decode(message, &parsed);
+    mavlink_msg_attitude_target_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_obstacle_distance_3d(const mavlink_message_t* message)
+cStruct* unbox_time_estimate_to_target(const mavlink_message_t* message)
 {
-    static mavlink_obstacle_distance_3d_t parsed;
+    static mavlink_time_estimate_to_target_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "x", &(parsed.x), 1, FLOAT},
-        { "y", &(parsed.y), 1, FLOAT},
-        { "z", &(parsed.z), 1, FLOAT},
-        { "min_distance", &(parsed.min_distance), 1, FLOAT},
-        { "max_distance", &(parsed.max_distance), 1, FLOAT},
-        { "obstacle_id", &(parsed.obstacle_id), 1, UINT16_T},
-        { "sensor_type", &(parsed.sensor_type), 1, UINT8_T},
-        { "frame", &(parsed.frame), 1, UINT8_T}
+        { "safe_return", &(parsed.safe_return), 1, INT32_T},
+        { "land", &(parsed.land), 1, INT32_T},
+        { "mission_next_item", &(parsed.mission_next_item), 1, INT32_T},
+        { "mission_end", &(parsed.mission_end), 1, INT32_T},
+        { "commanded_action", &(parsed.commanded_action), 1, INT32_T}
     };
-    static cStruct record = {"obstacle_distance_3d", members, 9, 11037};
+    static cStruct record = {"time_estimate_to_target", members, 5, 380};
 
-    mavlink_msg_obstacle_distance_3d_decode(message, &parsed);
+    mavlink_msg_time_estimate_to_target_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_meminfo(const mavlink_message_t* message)
+cStruct* unbox_camera_trigger(const mavlink_message_t* message)
 {
-    static mavlink_meminfo_t parsed;
+    static mavlink_camera_trigger_t parsed;
 
     static cMember members[] = {
-        { "brkval", &(parsed.brkval), 1, UINT16_T},
-        { "freemem", &(parsed.freemem), 1, UINT16_T},
-        { "freemem32", &(parsed.freemem32), 1, UINT32_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "seq", &(parsed.seq), 1, UINT32_T}
     };
-    static cStruct record = {"meminfo", members, 3, 152};
+    static cStruct record = {"camera_trigger", members, 2, 112};
 
-    mavlink_msg_meminfo_decode(message, &parsed);
+    mavlink_msg_camera_trigger_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_mount_configure(const mavlink_message_t* message)
+cStruct* unbox_system_time(const mavlink_message_t* message)
 {
-    static mavlink_mount_configure_t parsed;
+    static mavlink_system_time_t parsed;
 
     static cMember members[] = {
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "mount_mode", &(parsed.mount_mode), 1, UINT8_T},
-        { "stab_roll", &(parsed.stab_roll), 1, UINT8_T},
-        { "stab_pitch", &(parsed.stab_pitch), 1, UINT8_T},
-        { "stab_yaw", &(parsed.stab_yaw), 1, UINT8_T}
+        { "time_unix_usec", &(parsed.time_unix_usec), 1, UINT64_T},
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T}
     };
-    static cStruct record = {"mount_configure", members, 6, 156};
+    static cStruct record = {"system_time", members, 2, 2};
 
-    mavlink_msg_mount_configure_decode(message, &parsed);
+    mavlink_msg_system_time_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_led_control(const mavlink_message_t* message)
+cStruct* unbox_mission_item_reached(const mavlink_message_t* message)
 {
-    static mavlink_led_control_t parsed;
+    static mavlink_mission_item_reached_t parsed;
 
     static cMember members[] = {
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "instance", &(parsed.instance), 1, UINT8_T},
-        { "pattern", &(parsed.pattern), 1, UINT8_T},
-        { "custom_len", &(parsed.custom_len), 1, UINT8_T},
-        { "custom_bytes", &(parsed.custom_bytes), 24, UINT8_T}
+        { "seq", &(parsed.seq), 1, UINT16_T}
     };
-    static cStruct record = {"led_control", members, 6, 186};
+    static cStruct record = {"mission_item_reached", members, 1, 46};
 
-    mavlink_msg_led_control_decode(message, &parsed);
+    mavlink_msg_mission_item_reached_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_adap_tuning(const mavlink_message_t* message)
+cStruct* unbox_log_entry(const mavlink_message_t* message)
 {
-    static mavlink_adap_tuning_t parsed;
+    static mavlink_log_entry_t parsed;
 
     static cMember members[] = {
-        { "desired", &(parsed.desired), 1, FLOAT},
-        { "achieved", &(parsed.achieved), 1, FLOAT},
-        { "error", &(parsed.error), 1, FLOAT},
-        { "theta", &(parsed.theta), 1, FLOAT},
-        { "omega", &(parsed.omega), 1, FLOAT},
-        { "sigma", &(parsed.sigma), 1, FLOAT},
-        { "theta_dot", &(parsed.theta_dot), 1, FLOAT},
-        { "omega_dot", &(parsed.omega_dot), 1, FLOAT},
-        { "sigma_dot", &(parsed.sigma_dot), 1, FLOAT},
-        { "f", &(parsed.f), 1, FLOAT},
-        { "f_dot", &(parsed.f_dot), 1, FLOAT},
-        { "u", &(parsed.u), 1, FLOAT},
-        { "axis", &(parsed.axis), 1, UINT8_T}
+        { "time_utc", &(parsed.time_utc), 1, UINT32_T},
+        { "size", &(parsed.size), 1, UINT32_T},
+        { "id", &(parsed.id), 1, UINT16_T},
+        { "num_logs", &(parsed.num_logs), 1, UINT16_T},
+        { "last_log_num", &(parsed.last_log_num), 1, UINT16_T}
     };
-    static cStruct record = {"adap_tuning", members, 13, 11010};
+    static cStruct record = {"log_entry", members, 5, 118};
 
-    mavlink_msg_adap_tuning_decode(message, &parsed);
+    mavlink_msg_log_entry_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_battery2(const mavlink_message_t* message)
+cStruct* unbox_link_node_status(const mavlink_message_t* message)
 {
-    static mavlink_battery2_t parsed;
+    static mavlink_link_node_status_t parsed;
 
     static cMember members[] = {
-        { "voltage", &(parsed.voltage), 1, UINT16_T},
-        { "current_battery", &(parsed.current_battery), 1, INT16_T}
+        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
+        { "tx_rate", &(parsed.tx_rate), 1, UINT32_T},
+        { "rx_rate", &(parsed.rx_rate), 1, UINT32_T},
+        { "messages_sent", &(parsed.messages_sent), 1, UINT32_T},
+        { "messages_received", &(parsed.messages_received), 1, UINT32_T},
+        { "messages_lost", &(parsed.messages_lost), 1, UINT32_T},
+        { "rx_parse_err", &(parsed.rx_parse_err), 1, UINT16_T},
+        { "tx_overflows", &(parsed.tx_overflows), 1, UINT16_T},
+        { "rx_overflows", &(parsed.rx_overflows), 1, UINT16_T},
+        { "tx_buf", &(parsed.tx_buf), 1, UINT8_T},
+        { "rx_buf", &(parsed.rx_buf), 1, UINT8_T}
     };
-    static cStruct record = {"battery2", members, 2, 181};
+    static cStruct record = {"link_node_status", members, 11, 8};
 
-    mavlink_msg_battery2_decode(message, &parsed);
+    mavlink_msg_link_node_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_osd_param_config(const mavlink_message_t* message)
+cStruct* unbox_command_int(const mavlink_message_t* message)
 {
-    static mavlink_osd_param_config_t parsed;
+    static mavlink_command_int_t parsed;
 
     static cMember members[] = {
-        { "request_id", &(parsed.request_id), 1, UINT32_T},
-        { "min_value", &(parsed.min_value), 1, FLOAT},
-        { "max_value", &(parsed.max_value), 1, FLOAT},
-        { "increment", &(parsed.increment), 1, FLOAT},
+        { "param1", &(parsed.param1), 1, FLOAT},
+        { "param2", &(parsed.param2), 1, FLOAT},
+        { "param3", &(parsed.param3), 1, FLOAT},
+        { "param4", &(parsed.param4), 1, FLOAT},
+        { "x", &(parsed.x), 1, INT32_T},
+        { "y", &(parsed.y), 1, INT32_T},
+        { "z", &(parsed.z), 1, FLOAT},
+        { "command", &(parsed.command), 1, UINT16_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "osd_screen", &(parsed.osd_screen), 1, UINT8_T},
-        { "osd_index", &(parsed.osd_index), 1, UINT8_T},
-        { "param_id", &(parsed.param_id), 16, CHAR},
-        { "config_type", &(parsed.config_type), 1, UINT8_T}
+        { "frame", &(parsed.frame), 1, UINT8_T},
+        { "current", &(parsed.current), 1, UINT8_T},
+        { "autocontinue", &(parsed.autocontinue), 1, UINT8_T}
     };
-    static cStruct record = {"osd_param_config", members, 10, 11033};
+    static cStruct record = {"command_int", members, 13, 75};
 
-    mavlink_msg_osd_param_config_decode(message, &parsed);
+    mavlink_msg_command_int_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_ap_adc(const mavlink_message_t* message)
+cStruct* unbox_position_target_local_ned(const mavlink_message_t* message)
 {
-    static mavlink_ap_adc_t parsed;
+    static mavlink_position_target_local_ned_t parsed;
 
     static cMember members[] = {
-        { "adc1", &(parsed.adc1), 1, UINT16_T},
-        { "adc2", &(parsed.adc2), 1, UINT16_T},
-        { "adc3", &(parsed.adc3), 1, UINT16_T},
-        { "adc4", &(parsed.adc4), 1, UINT16_T},
-        { "adc5", &(parsed.adc5), 1, UINT16_T},
-        { "adc6", &(parsed.adc6), 1, UINT16_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "x", &(parsed.x), 1, FLOAT},
+        { "y", &(parsed.y), 1, FLOAT},
+        { "z", &(parsed.z), 1, FLOAT},
+        { "vx", &(parsed.vx), 1, FLOAT},
+        { "vy", &(parsed.vy), 1, FLOAT},
+        { "vz", &(parsed.vz), 1, FLOAT},
+        { "afx", &(parsed.afx), 1, FLOAT},
+        { "afy", &(parsed.afy), 1, FLOAT},
+        { "afz", &(parsed.afz), 1, FLOAT},
+        { "yaw", &(parsed.yaw), 1, FLOAT},
+        { "yaw_rate", &(parsed.yaw_rate), 1, FLOAT},
+        { "type_mask", &(parsed.type_mask), 1, UINT16_T},
+        { "coordinate_frame", &(parsed.coordinate_frame), 1, UINT8_T}
     };
-    static cStruct record = {"ap_adc", members, 6, 153};
+    static cStruct record = {"position_target_local_ned", members, 14, 85};
 
-    mavlink_msg_ap_adc_decode(message, &parsed);
+    mavlink_msg_position_target_local_ned_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_sensor_offsets(const mavlink_message_t* message)
+cStruct* unbox_rc_channels_override(const mavlink_message_t* message)
 {
-    static mavlink_sensor_offsets_t parsed;
+    static mavlink_rc_channels_override_t parsed;
 
     static cMember members[] = {
-        { "mag_declination", &(parsed.mag_declination), 1, FLOAT},
-        { "raw_press", &(parsed.raw_press), 1, INT32_T},
-        { "raw_temp", &(parsed.raw_temp), 1, INT32_T},
-        { "gyro_cal_x", &(parsed.gyro_cal_x), 1, FLOAT},
-        { "gyro_cal_y", &(parsed.gyro_cal_y), 1, FLOAT},
-        { "gyro_cal_z", &(parsed.gyro_cal_z), 1, FLOAT},
-        { "accel_cal_x", &(parsed.accel_cal_x), 1, FLOAT},
-        { "accel_cal_y", &(parsed.accel_cal_y), 1, FLOAT},
-        { "accel_cal_z", &(parsed.accel_cal_z), 1, FLOAT},
-        { "mag_ofs_x", &(parsed.mag_ofs_x), 1, INT16_T},
-        { "mag_ofs_y", &(parsed.mag_ofs_y), 1, INT16_T},
-        { "mag_ofs_z", &(parsed.mag_ofs_z), 1, INT16_T}
+        { "chan1_raw", &(parsed.chan1_raw), 1, UINT16_T},
+        { "chan2_raw", &(parsed.chan2_raw), 1, UINT16_T},
+        { "chan3_raw", &(parsed.chan3_raw), 1, UINT16_T},
+        { "chan4_raw", &(parsed.chan4_raw), 1, UINT16_T},
+        { "chan5_raw", &(parsed.chan5_raw), 1, UINT16_T},
+        { "chan6_raw", &(parsed.chan6_raw), 1, UINT16_T},
+        { "chan7_raw", &(parsed.chan7_raw), 1, UINT16_T},
+        { "chan8_raw", &(parsed.chan8_raw), 1, UINT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "chan9_raw", &(parsed.chan9_raw), 1, UINT16_T},
+        { "chan10_raw", &(parsed.chan10_raw), 1, UINT16_T},
+        { "chan11_raw", &(parsed.chan11_raw), 1, UINT16_T},
+        { "chan12_raw", &(parsed.chan12_raw), 1, UINT16_T},
+        { "chan13_raw", &(parsed.chan13_raw), 1, UINT16_T},
+        { "chan14_raw", &(parsed.chan14_raw), 1, UINT16_T},
+        { "chan15_raw", &(parsed.chan15_raw), 1, UINT16_T},
+        { "chan16_raw", &(parsed.chan16_raw), 1, UINT16_T},
+        { "chan17_raw", &(parsed.chan17_raw), 1, UINT16_T},
+        { "chan18_raw", &(parsed.chan18_raw), 1, UINT16_T}
     };
-    static cStruct record = {"sensor_offsets", members, 12, 150};
+    static cStruct record = {"rc_channels_override", members, 20, 70};
 
-    mavlink_msg_sensor_offsets_decode(message, &parsed);
+    mavlink_msg_rc_channels_override_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_digicam_configure(const mavlink_message_t* message)
+cStruct* unbox_local_position_ned_cov(const mavlink_message_t* message)
 {
-    static mavlink_digicam_configure_t parsed;
+    static mavlink_local_position_ned_cov_t parsed;
 
     static cMember members[] = {
-        { "extra_value", &(parsed.extra_value), 1, FLOAT},
-        { "shutter_speed", &(parsed.shutter_speed), 1, UINT16_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "mode", &(parsed.mode), 1, UINT8_T},
-        { "aperture", &(parsed.aperture), 1, UINT8_T},
-        { "iso", &(parsed.iso), 1, UINT8_T},
-        { "exposure_type", &(parsed.exposure_type), 1, UINT8_T},
-        { "command_id", &(parsed.command_id), 1, UINT8_T},
-        { "engine_cut_off", &(parsed.engine_cut_off), 1, UINT8_T},
-        { "extra_param", &(parsed.extra_param), 1, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "x", &(parsed.x), 1, FLOAT},
+        { "y", &(parsed.y), 1, FLOAT},
+        { "z", &(parsed.z), 1, FLOAT},
+        { "vx", &(parsed.vx), 1, FLOAT},
+        { "vy", &(parsed.vy), 1, FLOAT},
+        { "vz", &(parsed.vz), 1, FLOAT},
+        { "ax", &(parsed.ax), 1, FLOAT},
+        { "ay", &(parsed.ay), 1, FLOAT},
+        { "az", &(parsed.az), 1, FLOAT},
+        { "covariance", &(parsed.covariance), 45, FLOAT},
+        { "estimator_type", &(parsed.estimator_type), 1, UINT8_T}
     };
-    static cStruct record = {"digicam_configure", members, 11, 154};
+    static cStruct record = {"local_position_ned_cov", members, 12, 64};
 
-    mavlink_msg_digicam_configure_decode(message, &parsed);
+    mavlink_msg_local_position_ned_cov_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_esc_telemetry_1_to_4(const mavlink_message_t* message)
+cStruct* unbox_raw_pressure(const mavlink_message_t* message)
 {
-    static mavlink_esc_telemetry_1_to_4_t parsed;
+    static mavlink_raw_pressure_t parsed;
 
     static cMember members[] = {
-        { "voltage", &(parsed.voltage), 4, UINT16_T},
-        { "current", &(parsed.current), 4, UINT16_T},
-        { "totalcurrent", &(parsed.totalcurrent), 4, UINT16_T},
-        { "rpm", &(parsed.rpm), 4, UINT16_T},
-        { "count", &(parsed.count), 4, UINT16_T},
-        { "temperature", &(parsed.temperature), 4, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "press_abs", &(parsed.press_abs), 1, INT16_T},
+        { "press_diff1", &(parsed.press_diff1), 1, INT16_T},
+        { "press_diff2", &(parsed.press_diff2), 1, INT16_T},
+        { "temperature", &(parsed.temperature), 1, INT16_T}
     };
-    static cStruct record = {"esc_telemetry_1_to_4", members, 6, 11030};
+    static cStruct record = {"raw_pressure", members, 5, 28};
 
-    mavlink_msg_esc_telemetry_1_to_4_decode(message, &parsed);
+    mavlink_msg_raw_pressure_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_esc_telemetry_9_to_12(const mavlink_message_t* message)
+cStruct* unbox_home_position(const mavlink_message_t* message)
 {
-    static mavlink_esc_telemetry_9_to_12_t parsed;
+    static mavlink_home_position_t parsed;
 
     static cMember members[] = {
-        { "voltage", &(parsed.voltage), 4, UINT16_T},
-        { "current", &(parsed.current), 4, UINT16_T},
-        { "totalcurrent", &(parsed.totalcurrent), 4, UINT16_T},
-        { "rpm", &(parsed.rpm), 4, UINT16_T},
-        { "count", &(parsed.count), 4, UINT16_T},
-        { "temperature", &(parsed.temperature), 4, UINT8_T}
+        { "latitude", &(parsed.latitude), 1, INT32_T},
+        { "longitude", &(parsed.longitude), 1, INT32_T},
+        { "altitude", &(parsed.altitude), 1, INT32_T},
+        { "x", &(parsed.x), 1, FLOAT},
+        { "y", &(parsed.y), 1, FLOAT},
+        { "z", &(parsed.z), 1, FLOAT},
+        { "q", &(parsed.q), 4, FLOAT},
+        { "approach_x", &(parsed.approach_x), 1, FLOAT},
+        { "approach_y", &(parsed.approach_y), 1, FLOAT},
+        { "approach_z", &(parsed.approach_z), 1, FLOAT},
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T}
     };
-    static cStruct record = {"esc_telemetry_9_to_12", members, 6, 11032};
+    static cStruct record = {"home_position", members, 11, 242};
 
-    mavlink_msg_esc_telemetry_9_to_12_decode(message, &parsed);
+    mavlink_msg_home_position_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_hwstatus(const mavlink_message_t* message)
+cStruct* unbox_autopilot_version(const mavlink_message_t* message)
 {
-    static mavlink_hwstatus_t parsed;
+    static mavlink_autopilot_version_t parsed;
 
     static cMember members[] = {
-        { "Vcc", &(parsed.Vcc), 1, UINT16_T},
-        { "I2Cerr", &(parsed.I2Cerr), 1, UINT8_T}
+        { "capabilities", &(parsed.capabilities), 1, UINT64_T},
+        { "uid", &(parsed.uid), 1, UINT64_T},
+        { "flight_sw_version", &(parsed.flight_sw_version), 1, UINT32_T},
+        { "middleware_sw_version", &(parsed.middleware_sw_version), 1, UINT32_T},
+        { "os_sw_version", &(parsed.os_sw_version), 1, UINT32_T},
+        { "board_version", &(parsed.board_version), 1, UINT32_T},
+        { "vendor_id", &(parsed.vendor_id), 1, UINT16_T},
+        { "product_id", &(parsed.product_id), 1, UINT16_T},
+        { "flight_custom_version", &(parsed.flight_custom_version), 8, UINT8_T},
+        { "middleware_custom_version", &(parsed.middleware_custom_version), 8, UINT8_T},
+        { "os_custom_version", &(parsed.os_custom_version), 8, UINT8_T},
+        { "uid2", &(parsed.uid2), 18, UINT8_T}
     };
-    static cStruct record = {"hwstatus", members, 2, 165};
+    static cStruct record = {"autopilot_version", members, 12, 148};
 
-    mavlink_msg_hwstatus_decode(message, &parsed);
+    mavlink_msg_autopilot_version_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_gopro_get_request(const mavlink_message_t* message)
+cStruct* unbox_change_operator_control(const mavlink_message_t* message)
 {
-    static mavlink_gopro_get_request_t parsed;
+    static mavlink_change_operator_control_t parsed;
 
     static cMember members[] = {
         { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "cmd_id", &(parsed.cmd_id), 1, UINT8_T}
+        { "control_request", &(parsed.control_request), 1, UINT8_T},
+        { "version", &(parsed.version), 1, UINT8_T},
+        { "passkey", &(parsed.passkey), 25, CHAR}
     };
-    static cStruct record = {"gopro_get_request", members, 3, 216};
+    static cStruct record = {"change_operator_control", members, 4, 5};
 
-    mavlink_msg_gopro_get_request_decode(message, &parsed);
+    mavlink_msg_change_operator_control_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_storm32_gimbal_manager_correct_roll(const mavlink_message_t* message)
+cStruct* unbox_manual_setpoint(const mavlink_message_t* message)
 {
-    static mavlink_storm32_gimbal_manager_correct_roll_t parsed;
+    static mavlink_manual_setpoint_t parsed;
 
     static cMember members[] = {
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
         { "roll", &(parsed.roll), 1, FLOAT},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "gimbal_id", &(parsed.gimbal_id), 1, UINT8_T},
-        { "client", &(parsed.client), 1, UINT8_T}
+        { "pitch", &(parsed.pitch), 1, FLOAT},
+        { "yaw", &(parsed.yaw), 1, FLOAT},
+        { "thrust", &(parsed.thrust), 1, FLOAT},
+        { "mode_switch", &(parsed.mode_switch), 1, UINT8_T},
+        { "manual_override_switch", &(parsed.manual_override_switch), 1, UINT8_T}
     };
-    static cStruct record = {"storm32_gimbal_manager_correct_roll", members, 5, 60014};
+    static cStruct record = {"manual_setpoint", members, 7, 81};
 
-    mavlink_msg_storm32_gimbal_manager_correct_roll_decode(message, &parsed);
+    mavlink_msg_manual_setpoint_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_radio_rc_channels(const mavlink_message_t* message)
+cStruct* unbox_scaled_imu(const mavlink_message_t* message)
 {
-    static mavlink_radio_rc_channels_t parsed;
+    static mavlink_scaled_imu_t parsed;
 
     static cMember members[] = {
-        { "count", &(parsed.count), 1, UINT8_T},
-        { "flags", &(parsed.flags), 1, UINT8_T},
-        { "channels", &(parsed.channels), 24, INT16_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "xacc", &(parsed.xacc), 1, INT16_T},
+        { "yacc", &(parsed.yacc), 1, INT16_T},
+        { "zacc", &(parsed.zacc), 1, INT16_T},
+        { "xgyro", &(parsed.xgyro), 1, INT16_T},
+        { "ygyro", &(parsed.ygyro), 1, INT16_T},
+        { "zgyro", &(parsed.zgyro), 1, INT16_T},
+        { "xmag", &(parsed.xmag), 1, INT16_T},
+        { "ymag", &(parsed.ymag), 1, INT16_T},
+        { "zmag", &(parsed.zmag), 1, INT16_T},
+        { "temperature", &(parsed.temperature), 1, INT16_T}
     };
-    static cStruct record = {"radio_rc_channels", members, 3, 60045};
+    static cStruct record = {"scaled_imu", members, 11, 26};
 
-    mavlink_msg_radio_rc_channels_decode(message, &parsed);
+    mavlink_msg_scaled_imu_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_param_value_array(const mavlink_message_t* message)
+cStruct* unbox_wind_cov(const mavlink_message_t* message)
 {
-    static mavlink_param_value_array_t parsed;
+    static mavlink_wind_cov_t parsed;
 
     static cMember members[] = {
-        { "param_count", &(parsed.param_count), 1, UINT16_T},
-        { "param_index_first", &(parsed.param_index_first), 1, UINT16_T},
-        { "flags", &(parsed.flags), 1, UINT16_T},
-        { "param_array_len", &(parsed.param_array_len), 1, UINT8_T},
-        { "packet_buf", &(parsed.packet_buf), 248, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "wind_x", &(parsed.wind_x), 1, FLOAT},
+        { "wind_y", &(parsed.wind_y), 1, FLOAT},
+        { "wind_z", &(parsed.wind_z), 1, FLOAT},
+        { "var_horiz", &(parsed.var_horiz), 1, FLOAT},
+        { "var_vert", &(parsed.var_vert), 1, FLOAT},
+        { "wind_alt", &(parsed.wind_alt), 1, FLOAT},
+        { "horiz_accuracy", &(parsed.horiz_accuracy), 1, FLOAT},
+        { "vert_accuracy", &(parsed.vert_accuracy), 1, FLOAT}
     };
-    static cStruct record = {"param_value_array", members, 5, 60041};
+    static cStruct record = {"wind_cov", members, 9, 231};
 
-    mavlink_msg_param_value_array_decode(message, &parsed);
+    mavlink_msg_wind_cov_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_storm32_gimbal_manager_information(const mavlink_message_t* message)
+cStruct* unbox_debug_vect(const mavlink_message_t* message)
 {
-    static mavlink_storm32_gimbal_manager_information_t parsed;
+    static mavlink_debug_vect_t parsed;
 
     static cMember members[] = {
-        { "device_cap_flags", &(parsed.device_cap_flags), 1, UINT32_T},
-        { "manager_cap_flags", &(parsed.manager_cap_flags), 1, UINT32_T},
-        { "roll_min", &(parsed.roll_min), 1, FLOAT},
-        { "roll_max", &(parsed.roll_max), 1, FLOAT},
-        { "pitch_min", &(parsed.pitch_min), 1, FLOAT},
-        { "pitch_max", &(parsed.pitch_max), 1, FLOAT},
-        { "yaw_min", &(parsed.yaw_min), 1, FLOAT},
-        { "yaw_max", &(parsed.yaw_max), 1, FLOAT},
-        { "gimbal_id", &(parsed.gimbal_id), 1, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "x", &(parsed.x), 1, FLOAT},
+        { "y", &(parsed.y), 1, FLOAT},
+        { "z", &(parsed.z), 1, FLOAT},
+        { "name", &(parsed.name), 10, CHAR}
     };
-    static cStruct record = {"storm32_gimbal_manager_information", members, 9, 60010};
+    static cStruct record = {"debug_vect", members, 5, 250};
 
-    mavlink_msg_storm32_gimbal_manager_information_decode(message, &parsed);
+    mavlink_msg_debug_vect_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_radio_link_stats(const mavlink_message_t* message)
+cStruct* unbox_gps_status(const mavlink_message_t* message)
 {
-    static mavlink_radio_link_stats_t parsed;
+    static mavlink_gps_status_t parsed;
 
     static cMember members[] = {
-        { "flags", &(parsed.flags), 1, UINT8_T},
-        { "rx_LQ", &(parsed.rx_LQ), 1, UINT8_T},
-        { "rx_rssi1", &(parsed.rx_rssi1), 1, UINT8_T},
-        { "rx_snr1", &(parsed.rx_snr1), 1, INT8_T},
-        { "rx_rssi2", &(parsed.rx_rssi2), 1, UINT8_T},
-        { "rx_snr2", &(parsed.rx_snr2), 1, INT8_T},
-        { "rx_receive_antenna", &(parsed.rx_receive_antenna), 1, UINT8_T},
-        { "rx_transmit_antenna", &(parsed.rx_transmit_antenna), 1, UINT8_T},
-        { "tx_LQ", &(parsed.tx_LQ), 1, UINT8_T},
-        { "tx_rssi1", &(parsed.tx_rssi1), 1, UINT8_T},
-        { "tx_snr1", &(parsed.tx_snr1), 1, INT8_T},
-        { "tx_rssi2", &(parsed.tx_rssi2), 1, UINT8_T},
-        { "tx_snr2", &(parsed.tx_snr2), 1, INT8_T},
-        { "tx_receive_antenna", &(parsed.tx_receive_antenna), 1, UINT8_T},
-        { "tx_transmit_antenna", &(parsed.tx_transmit_antenna), 1, UINT8_T}
+        { "satellites_visible", &(parsed.satellites_visible), 1, UINT8_T},
+        { "satellite_prn", &(parsed.satellite_prn), 20, UINT8_T},
+        { "satellite_used", &(parsed.satellite_used), 20, UINT8_T},
+        { "satellite_elevation", &(parsed.satellite_elevation), 20, UINT8_T},
+        { "satellite_azimuth", &(parsed.satellite_azimuth), 20, UINT8_T},
+        { "satellite_snr", &(parsed.satellite_snr), 20, UINT8_T}
     };
-    static cStruct record = {"radio_link_stats", members, 15, 60046};
+    static cStruct record = {"gps_status", members, 6, 25};
 
-    mavlink_msg_radio_link_stats_decode(message, &parsed);
+    mavlink_msg_gps_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_frsky_passthrough_array(const mavlink_message_t* message)
+cStruct* unbox_flight_information(const mavlink_message_t* message)
 {
-    static mavlink_frsky_passthrough_array_t parsed;
+    static mavlink_flight_information_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "count", &(parsed.count), 1, UINT8_T},
-        { "packet_buf", &(parsed.packet_buf), 240, UINT8_T}
+        { "arming_time_utc", &(parsed.arming_time_utc), 1, UINT64_T},
+        { "takeoff_time_utc", &(parsed.takeoff_time_utc), 1, UINT64_T},
+        { "flight_uuid", &(parsed.flight_uuid), 1, UINT64_T},
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T}
     };
-    static cStruct record = {"frsky_passthrough_array", members, 3, 60040};
+    static cStruct record = {"flight_information", members, 4, 264};
 
-    mavlink_msg_frsky_passthrough_array_decode(message, &parsed);
+    mavlink_msg_flight_information_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_storm32_gimbal_manager_control(const mavlink_message_t* message)
+cStruct* unbox_scaled_pressure(const mavlink_message_t* message)
 {
-    static mavlink_storm32_gimbal_manager_control_t parsed;
+    static mavlink_scaled_pressure_t parsed;
 
     static cMember members[] = {
-        { "q", &(parsed.q), 4, FLOAT},
-        { "angular_velocity_x", &(parsed.angular_velocity_x), 1, FLOAT},
-        { "angular_velocity_y", &(parsed.angular_velocity_y), 1, FLOAT},
-        { "angular_velocity_z", &(parsed.angular_velocity_z), 1, FLOAT},
-        { "device_flags", &(parsed.device_flags), 1, UINT16_T},
-        { "manager_flags", &(parsed.manager_flags), 1, UINT16_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "gimbal_id", &(parsed.gimbal_id), 1, UINT8_T},
-        { "client", &(parsed.client), 1, UINT8_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "press_abs", &(parsed.press_abs), 1, FLOAT},
+        { "press_diff", &(parsed.press_diff), 1, FLOAT},
+        { "temperature", &(parsed.temperature), 1, INT16_T},
+        { "temperature_press_diff", &(parsed.temperature_press_diff), 1, INT16_T}
     };
-    static cStruct record = {"storm32_gimbal_manager_control", members, 10, 60012};
+    static cStruct record = {"scaled_pressure", members, 5, 29};
 
-    mavlink_msg_storm32_gimbal_manager_control_decode(message, &parsed);
+    mavlink_msg_scaled_pressure_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_storm32_gimbal_manager_control_pitchyaw(const mavlink_message_t* message)
+cStruct* unbox_set_attitude_target(const mavlink_message_t* message)
 {
-    static mavlink_storm32_gimbal_manager_control_pitchyaw_t parsed;
+    static mavlink_set_attitude_target_t parsed;
 
     static cMember members[] = {
-        { "pitch", &(parsed.pitch), 1, FLOAT},
-        { "yaw", &(parsed.yaw), 1, FLOAT},
-        { "pitch_rate", &(parsed.pitch_rate), 1, FLOAT},
-        { "yaw_rate", &(parsed.yaw_rate), 1, FLOAT},
-        { "device_flags", &(parsed.device_flags), 1, UINT16_T},
-        { "manager_flags", &(parsed.manager_flags), 1, UINT16_T},
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "q", &(parsed.q), 4, FLOAT},
+        { "body_roll_rate", &(parsed.body_roll_rate), 1, FLOAT},
+        { "body_pitch_rate", &(parsed.body_pitch_rate), 1, FLOAT},
+        { "body_yaw_rate", &(parsed.body_yaw_rate), 1, FLOAT},
+        { "thrust", &(parsed.thrust), 1, FLOAT},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "gimbal_id", &(parsed.gimbal_id), 1, UINT8_T},
-        { "client", &(parsed.client), 1, UINT8_T}
+        { "type_mask", &(parsed.type_mask), 1, UINT8_T},
+        { "thrust_body", &(parsed.thrust_body), 3, FLOAT}
     };
-    static cStruct record = {"storm32_gimbal_manager_control_pitchyaw", members, 10, 60013};
+    static cStruct record = {"set_attitude_target", members, 10, 82};
 
-    mavlink_msg_storm32_gimbal_manager_control_pitchyaw_decode(message, &parsed);
+    mavlink_msg_set_attitude_target_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_storm32_gimbal_manager_status(const mavlink_message_t* message)
+cStruct* unbox_ais_vessel(const mavlink_message_t* message)
 {
-    static mavlink_storm32_gimbal_manager_status_t parsed;
+    static mavlink_ais_vessel_t parsed;
 
     static cMember members[] = {
-        { "device_flags", &(parsed.device_flags), 1, UINT16_T},
-        { "manager_flags", &(parsed.manager_flags), 1, UINT16_T},
-        { "gimbal_id", &(parsed.gimbal_id), 1, UINT8_T},
-        { "supervisor", &(parsed.supervisor), 1, UINT8_T},
-        { "profile", &(parsed.profile), 1, UINT8_T}
+        { "MMSI", &(parsed.MMSI), 1, UINT32_T},
+        { "lat", &(parsed.lat), 1, INT32_T},
+        { "lon", &(parsed.lon), 1, INT32_T},
+        { "COG", &(parsed.COG), 1, UINT16_T},
+        { "heading", &(parsed.heading), 1, UINT16_T},
+        { "velocity", &(parsed.velocity), 1, UINT16_T},
+        { "dimension_bow", &(parsed.dimension_bow), 1, UINT16_T},
+        { "dimension_stern", &(parsed.dimension_stern), 1, UINT16_T},
+        { "tslc", &(parsed.tslc), 1, UINT16_T},
+        { "flags", &(parsed.flags), 1, UINT16_T},
+        { "turn_rate", &(parsed.turn_rate), 1, INT8_T},
+        { "navigational_status", &(parsed.navigational_status), 1, UINT8_T},
+        { "type", &(parsed.type), 1, UINT8_T},
+        { "dimension_port", &(parsed.dimension_port), 1, UINT8_T},
+        { "dimension_starboard", &(parsed.dimension_starboard), 1, UINT8_T},
+        { "callsign", &(parsed.callsign), 7, CHAR},
+        { "name", &(parsed.name), 20, CHAR}
     };
-    static cStruct record = {"storm32_gimbal_manager_status", members, 5, 60011};
+    static cStruct record = {"ais_vessel", members, 17, 301};
 
-    mavlink_msg_storm32_gimbal_manager_status_decode(message, &parsed);
+    mavlink_msg_ais_vessel_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_qshot_status(const mavlink_message_t* message)
+cStruct* unbox_att_pos_mocap(const mavlink_message_t* message)
 {
-    static mavlink_qshot_status_t parsed;
+    static mavlink_att_pos_mocap_t parsed;
 
     static cMember members[] = {
-        { "mode", &(parsed.mode), 1, UINT16_T},
-        { "shot_state", &(parsed.shot_state), 1, UINT16_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "q", &(parsed.q), 4, FLOAT},
+        { "x", &(parsed.x), 1, FLOAT},
+        { "y", &(parsed.y), 1, FLOAT},
+        { "z", &(parsed.z), 1, FLOAT},
+        { "covariance", &(parsed.covariance), 21, FLOAT}
     };
-    static cStruct record = {"qshot_status", members, 2, 60020};
+    static cStruct record = {"att_pos_mocap", members, 6, 138};
 
-    mavlink_msg_qshot_status_decode(message, &parsed);
+    mavlink_msg_att_pos_mocap_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_cubepilot_raw_rc(const mavlink_message_t* message)
+cStruct* unbox_hil_state_quaternion(const mavlink_message_t* message)
 {
-    static mavlink_cubepilot_raw_rc_t parsed;
+    static mavlink_hil_state_quaternion_t parsed;
 
     static cMember members[] = {
-        { "rc_raw", &(parsed.rc_raw), 32, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "attitude_quaternion", &(parsed.attitude_quaternion), 4, FLOAT},
+        { "rollspeed", &(parsed.rollspeed), 1, FLOAT},
+        { "pitchspeed", &(parsed.pitchspeed), 1, FLOAT},
+        { "yawspeed", &(parsed.yawspeed), 1, FLOAT},
+        { "lat", &(parsed.lat), 1, INT32_T},
+        { "lon", &(parsed.lon), 1, INT32_T},
+        { "alt", &(parsed.alt), 1, INT32_T},
+        { "vx", &(parsed.vx), 1, INT16_T},
+        { "vy", &(parsed.vy), 1, INT16_T},
+        { "vz", &(parsed.vz), 1, INT16_T},
+        { "ind_airspeed", &(parsed.ind_airspeed), 1, UINT16_T},
+        { "true_airspeed", &(parsed.true_airspeed), 1, UINT16_T},
+        { "xacc", &(parsed.xacc), 1, INT16_T},
+        { "yacc", &(parsed.yacc), 1, INT16_T},
+        { "zacc", &(parsed.zacc), 1, INT16_T}
     };
-    static cStruct record = {"cubepilot_raw_rc", members, 1, 50001};
+    static cStruct record = {"hil_state_quaternion", members, 16, 115};
 
-    mavlink_msg_cubepilot_raw_rc_decode(message, &parsed);
+    mavlink_msg_hil_state_quaternion_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_cubepilot_firmware_update_resp(const mavlink_message_t* message)
+cStruct* unbox_landing_target(const mavlink_message_t* message)
 {
-    static mavlink_cubepilot_firmware_update_resp_t parsed;
+    static mavlink_landing_target_t parsed;
 
     static cMember members[] = {
-        { "offset", &(parsed.offset), 1, UINT32_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "angle_x", &(parsed.angle_x), 1, FLOAT},
+        { "angle_y", &(parsed.angle_y), 1, FLOAT},
+        { "distance", &(parsed.distance), 1, FLOAT},
+        { "size_x", &(parsed.size_x), 1, FLOAT},
+        { "size_y", &(parsed.size_y), 1, FLOAT},
+        { "target_num", &(parsed.target_num), 1, UINT8_T},
+        { "frame", &(parsed.frame), 1, UINT8_T},
+        { "x", &(parsed.x), 1, FLOAT},
+        { "y", &(parsed.y), 1, FLOAT},
+        { "z", &(parsed.z), 1, FLOAT},
+        { "q", &(parsed.q), 4, FLOAT},
+        { "type", &(parsed.type), 1, UINT8_T},
+        { "position_valid", &(parsed.position_valid), 1, UINT8_T}
     };
-    static cStruct record = {"cubepilot_firmware_update_resp", members, 3, 50005};
+    static cStruct record = {"landing_target", members, 14, 149};
 
-    mavlink_msg_cubepilot_firmware_update_resp_decode(message, &parsed);
+    mavlink_msg_landing_target_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_herelink_video_stream_information(const mavlink_message_t* message)
+cStruct* unbox_param_ext_request_read(const mavlink_message_t* message)
 {
-    static mavlink_herelink_video_stream_information_t parsed;
+    static mavlink_param_ext_request_read_t parsed;
 
     static cMember members[] = {
-        { "framerate", &(parsed.framerate), 1, FLOAT},
-        { "bitrate", &(parsed.bitrate), 1, UINT32_T},
-        { "resolution_h", &(parsed.resolution_h), 1, UINT16_T},
-        { "resolution_v", &(parsed.resolution_v), 1, UINT16_T},
-        { "rotation", &(parsed.rotation), 1, UINT16_T},
-        { "camera_id", &(parsed.camera_id), 1, UINT8_T},
-        { "status", &(parsed.status), 1, UINT8_T},
-        { "uri", &(parsed.uri), 230, CHAR}
+        { "param_index", &(parsed.param_index), 1, INT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "param_id", &(parsed.param_id), 16, CHAR}
     };
-    static cStruct record = {"herelink_video_stream_information", members, 8, 50002};
+    static cStruct record = {"param_ext_request_read", members, 4, 320};
 
-    mavlink_msg_herelink_video_stream_information_decode(message, &parsed);
+    mavlink_msg_param_ext_request_read_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_herelink_telem(const mavlink_message_t* message)
+cStruct* unbox_button_change(const mavlink_message_t* message)
 {
-    static mavlink_herelink_telem_t parsed;
+    static mavlink_button_change_t parsed;
 
     static cMember members[] = {
-        { "rf_freq", &(parsed.rf_freq), 1, UINT32_T},
-        { "link_bw", &(parsed.link_bw), 1, UINT32_T},
-        { "link_rate", &(parsed.link_rate), 1, UINT32_T},
-        { "snr", &(parsed.snr), 1, INT16_T},
-        { "cpu_temp", &(parsed.cpu_temp), 1, INT16_T},
-        { "board_temp", &(parsed.board_temp), 1, INT16_T},
-        { "rssi", &(parsed.rssi), 1, UINT8_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "last_change_ms", &(parsed.last_change_ms), 1, UINT32_T},
+        { "state", &(parsed.state), 1, UINT8_T}
     };
-    static cStruct record = {"herelink_telem", members, 7, 50003};
+    static cStruct record = {"button_change", members, 3, 257};
 
-    mavlink_msg_herelink_telem_decode(message, &parsed);
+    mavlink_msg_button_change_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_cubepilot_firmware_update_start(const mavlink_message_t* message)
+cStruct* unbox_attitude_quaternion_cov(const mavlink_message_t* message)
 {
-    static mavlink_cubepilot_firmware_update_start_t parsed;
+    static mavlink_attitude_quaternion_cov_t parsed;
 
     static cMember members[] = {
-        { "size", &(parsed.size), 1, UINT32_T},
-        { "crc", &(parsed.crc), 1, UINT32_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "q", &(parsed.q), 4, FLOAT},
+        { "rollspeed", &(parsed.rollspeed), 1, FLOAT},
+        { "pitchspeed", &(parsed.pitchspeed), 1, FLOAT},
+        { "yawspeed", &(parsed.yawspeed), 1, FLOAT},
+        { "covariance", &(parsed.covariance), 9, FLOAT}
     };
-    static cStruct record = {"cubepilot_firmware_update_start", members, 4, 50004};
+    static cStruct record = {"attitude_quaternion_cov", members, 6, 61};
 
-    mavlink_msg_cubepilot_firmware_update_start_decode(message, &parsed);
+    mavlink_msg_attitude_quaternion_cov_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_uavionix_adsb_out_dynamic(const mavlink_message_t* message)
+cStruct* unbox_open_drone_id_system_update(const mavlink_message_t* message)
 {
-    static mavlink_uavionix_adsb_out_dynamic_t parsed;
+    static mavlink_open_drone_id_system_update_t parsed;
 
     static cMember members[] = {
-        { "utcTime", &(parsed.utcTime), 1, UINT32_T},
-        { "gpsLat", &(parsed.gpsLat), 1, INT32_T},
-        { "gpsLon", &(parsed.gpsLon), 1, INT32_T},
-        { "gpsAlt", &(parsed.gpsAlt), 1, INT32_T},
-        { "baroAltMSL", &(parsed.baroAltMSL), 1, INT32_T},
-        { "accuracyHor", &(parsed.accuracyHor), 1, UINT32_T},
-        { "accuracyVert", &(parsed.accuracyVert), 1, UINT16_T},
-        { "accuracyVel", &(parsed.accuracyVel), 1, UINT16_T},
-        { "velVert", &(parsed.velVert), 1, INT16_T},
-        { "velNS", &(parsed.velNS), 1, INT16_T},
-        { "VelEW", &(parsed.VelEW), 1, INT16_T},
-        { "state", &(parsed.state), 1, UINT16_T},
-        { "squawk", &(parsed.squawk), 1, UINT16_T},
-        { "gpsFix", &(parsed.gpsFix), 1, UINT8_T},
-        { "numSats", &(parsed.numSats), 1, UINT8_T},
-        { "emergencyStatus", &(parsed.emergencyStatus), 1, UINT8_T}
+        { "operator_latitude", &(parsed.operator_latitude), 1, INT32_T},
+        { "operator_longitude", &(parsed.operator_longitude), 1, INT32_T},
+        { "operator_altitude_geo", &(parsed.operator_altitude_geo), 1, FLOAT},
+        { "timestamp", &(parsed.timestamp), 1, UINT32_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T}
     };
-    static cStruct record = {"uavionix_adsb_out_dynamic", members, 16, 10002};
+    static cStruct record = {"open_drone_id_system_update", members, 6, 12919};
 
-    mavlink_msg_uavionix_adsb_out_dynamic_decode(message, &parsed);
+    mavlink_msg_open_drone_id_system_update_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_uavionix_adsb_transceiver_health_report(const mavlink_message_t* message)
+cStruct* unbox_gimbal_manager_set_attitude(const mavlink_message_t* message)
 {
-    static mavlink_uavionix_adsb_transceiver_health_report_t parsed;
+    static mavlink_gimbal_manager_set_attitude_t parsed;
 
     static cMember members[] = {
-        { "rfHealth", &(parsed.rfHealth), 1, UINT8_T}
+        { "flags", &(parsed.flags), 1, UINT32_T},
+        { "q", &(parsed.q), 4, FLOAT},
+        { "angular_velocity_x", &(parsed.angular_velocity_x), 1, FLOAT},
+        { "angular_velocity_y", &(parsed.angular_velocity_y), 1, FLOAT},
+        { "angular_velocity_z", &(parsed.angular_velocity_z), 1, FLOAT},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "gimbal_device_id", &(parsed.gimbal_device_id), 1, UINT8_T}
     };
-    static cStruct record = {"uavionix_adsb_transceiver_health_report", members, 1, 10003};
+    static cStruct record = {"gimbal_manager_set_attitude", members, 8, 282};
 
-    mavlink_msg_uavionix_adsb_transceiver_health_report_decode(message, &parsed);
+    mavlink_msg_gimbal_manager_set_attitude_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_uavionix_adsb_out_cfg(const mavlink_message_t* message)
+cStruct* unbox_mission_ack(const mavlink_message_t* message)
 {
-    static mavlink_uavionix_adsb_out_cfg_t parsed;
+    static mavlink_mission_ack_t parsed;
 
     static cMember members[] = {
-        { "ICAO", &(parsed.ICAO), 1, UINT32_T},
-        { "stallSpeed", &(parsed.stallSpeed), 1, UINT16_T},
-        { "callsign", &(parsed.callsign), 9, CHAR},
-        { "emitterType", &(parsed.emitterType), 1, UINT8_T},
-        { "aircraftSize", &(parsed.aircraftSize), 1, UINT8_T},
-        { "gpsOffsetLat", &(parsed.gpsOffsetLat), 1, UINT8_T},
-        { "gpsOffsetLon", &(parsed.gpsOffsetLon), 1, UINT8_T},
-        { "rfSelect", &(parsed.rfSelect), 1, UINT8_T}
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "type", &(parsed.type), 1, UINT8_T},
+        { "mission_type", &(parsed.mission_type), 1, UINT8_T}
     };
-    static cStruct record = {"uavionix_adsb_out_cfg", members, 8, 10001};
+    static cStruct record = {"mission_ack", members, 4, 47};
 
-    mavlink_msg_uavionix_adsb_out_cfg_decode(message, &parsed);
+    mavlink_msg_mission_ack_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_array_test_6(const mavlink_message_t* message)
+cStruct* unbox_global_vision_position_estimate(const mavlink_message_t* message)
 {
-    static mavlink_array_test_6_t parsed;
+    static mavlink_global_vision_position_estimate_t parsed;
 
     static cMember members[] = {
-        { "ar_d", &(parsed.ar_d), 2, DOUBLE},
-        { "v3", &(parsed.v3), 1, UINT32_T},
-        { "ar_u32", &(parsed.ar_u32), 2, UINT32_T},
-        { "ar_i32", &(parsed.ar_i32), 2, INT32_T},
-        { "ar_f", &(parsed.ar_f), 2, FLOAT},
-        { "v2", &(parsed.v2), 1, UINT16_T},
-        { "ar_u16", &(parsed.ar_u16), 2, UINT16_T},
-        { "ar_i16", &(parsed.ar_i16), 2, INT16_T},
-        { "v1", &(parsed.v1), 1, UINT8_T},
-        { "ar_u8", &(parsed.ar_u8), 2, UINT8_T},
-        { "ar_i8", &(parsed.ar_i8), 2, INT8_T},
-        { "ar_c", &(parsed.ar_c), 32, CHAR}
+        { "usec", &(parsed.usec), 1, UINT64_T},
+        { "x", &(parsed.x), 1, FLOAT},
+        { "y", &(parsed.y), 1, FLOAT},
+        { "z", &(parsed.z), 1, FLOAT},
+        { "roll", &(parsed.roll), 1, FLOAT},
+        { "pitch", &(parsed.pitch), 1, FLOAT},
+        { "yaw", &(parsed.yaw), 1, FLOAT},
+        { "covariance", &(parsed.covariance), 21, FLOAT},
+        { "reset_counter", &(parsed.reset_counter), 1, UINT8_T}
     };
-    static cStruct record = {"array_test_6", members, 12, 17156};
+    static cStruct record = {"global_vision_position_estimate", members, 9, 101};
 
-    mavlink_msg_array_test_6_decode(message, &parsed);
+    mavlink_msg_global_vision_position_estimate_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_array_test_1(const mavlink_message_t* message)
+cStruct* unbox_local_position_ned(const mavlink_message_t* message)
 {
-    static mavlink_array_test_1_t parsed;
+    static mavlink_local_position_ned_t parsed;
 
     static cMember members[] = {
-        { "ar_u32", &(parsed.ar_u32), 4, UINT32_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "x", &(parsed.x), 1, FLOAT},
+        { "y", &(parsed.y), 1, FLOAT},
+        { "z", &(parsed.z), 1, FLOAT},
+        { "vx", &(parsed.vx), 1, FLOAT},
+        { "vy", &(parsed.vy), 1, FLOAT},
+        { "vz", &(parsed.vz), 1, FLOAT}
     };
-    static cStruct record = {"array_test_1", members, 1, 17151};
+    static cStruct record = {"local_position_ned", members, 7, 32};
 
-    mavlink_msg_array_test_1_decode(message, &parsed);
+    mavlink_msg_local_position_ned_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_array_test_3(const mavlink_message_t* message)
+cStruct* unbox_encapsulated_data(const mavlink_message_t* message)
 {
-    static mavlink_array_test_3_t parsed;
+    static mavlink_encapsulated_data_t parsed;
 
     static cMember members[] = {
-        { "ar_u32", &(parsed.ar_u32), 4, UINT32_T},
-        { "v", &(parsed.v), 1, UINT8_T}
+        { "seqnr", &(parsed.seqnr), 1, UINT16_T},
+        { "data", &(parsed.data), 253, UINT8_T}
     };
-    static cStruct record = {"array_test_3", members, 2, 17153};
+    static cStruct record = {"encapsulated_data", members, 2, 131};
 
-    mavlink_msg_array_test_3_decode(message, &parsed);
+    mavlink_msg_encapsulated_data_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_array_test_8(const mavlink_message_t* message)
+cStruct* unbox_set_position_target_local_ned(const mavlink_message_t* message)
 {
-    static mavlink_array_test_8_t parsed;
+    static mavlink_set_position_target_local_ned_t parsed;
 
     static cMember members[] = {
-        { "ar_d", &(parsed.ar_d), 2, DOUBLE},
-        { "v3", &(parsed.v3), 1, UINT32_T},
-        { "ar_u16", &(parsed.ar_u16), 2, UINT16_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "x", &(parsed.x), 1, FLOAT},
+        { "y", &(parsed.y), 1, FLOAT},
+        { "z", &(parsed.z), 1, FLOAT},
+        { "vx", &(parsed.vx), 1, FLOAT},
+        { "vy", &(parsed.vy), 1, FLOAT},
+        { "vz", &(parsed.vz), 1, FLOAT},
+        { "afx", &(parsed.afx), 1, FLOAT},
+        { "afy", &(parsed.afy), 1, FLOAT},
+        { "afz", &(parsed.afz), 1, FLOAT},
+        { "yaw", &(parsed.yaw), 1, FLOAT},
+        { "yaw_rate", &(parsed.yaw_rate), 1, FLOAT},
+        { "type_mask", &(parsed.type_mask), 1, UINT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "coordinate_frame", &(parsed.coordinate_frame), 1, UINT8_T}
     };
-    static cStruct record = {"array_test_8", members, 3, 17158};
+    static cStruct record = {"set_position_target_local_ned", members, 16, 84};
 
-    mavlink_msg_array_test_8_decode(message, &parsed);
+    mavlink_msg_set_position_target_local_ned_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_array_test_7(const mavlink_message_t* message)
+cStruct* unbox_open_drone_id_self_id(const mavlink_message_t* message)
 {
-    static mavlink_array_test_7_t parsed;
+    static mavlink_open_drone_id_self_id_t parsed;
 
     static cMember members[] = {
-        { "ar_d", &(parsed.ar_d), 2, DOUBLE},
-        { "ar_f", &(parsed.ar_f), 2, FLOAT},
-        { "ar_u32", &(parsed.ar_u32), 2, UINT32_T},
-        { "ar_i32", &(parsed.ar_i32), 2, INT32_T},
-        { "ar_u16", &(parsed.ar_u16), 2, UINT16_T},
-        { "ar_i16", &(parsed.ar_i16), 2, INT16_T},
-        { "ar_u8", &(parsed.ar_u8), 2, UINT8_T},
-        { "ar_i8", &(parsed.ar_i8), 2, INT8_T},
-        { "ar_c", &(parsed.ar_c), 32, CHAR}
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "id_or_mac", &(parsed.id_or_mac), 20, UINT8_T},
+        { "description_type", &(parsed.description_type), 1, UINT8_T},
+        { "description", &(parsed.description), 23, CHAR}
     };
-    static cStruct record = {"array_test_7", members, 9, 17157};
+    static cStruct record = {"open_drone_id_self_id", members, 5, 12903};
 
-    mavlink_msg_array_test_7_decode(message, &parsed);
+    mavlink_msg_open_drone_id_self_id_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_array_test_0(const mavlink_message_t* message)
+cStruct* unbox_efi_status(const mavlink_message_t* message)
 {
-    static mavlink_array_test_0_t parsed;
+    static mavlink_efi_status_t parsed;
 
     static cMember members[] = {
-        { "ar_u32", &(parsed.ar_u32), 4, UINT32_T},
-        { "ar_u16", &(parsed.ar_u16), 4, UINT16_T},
-        { "v1", &(parsed.v1), 1, UINT8_T},
-        { "ar_i8", &(parsed.ar_i8), 4, INT8_T},
-        { "ar_u8", &(parsed.ar_u8), 4, UINT8_T}
+        { "ecu_index", &(parsed.ecu_index), 1, FLOAT},
+        { "rpm", &(parsed.rpm), 1, FLOAT},
+        { "fuel_consumed", &(parsed.fuel_consumed), 1, FLOAT},
+        { "fuel_flow", &(parsed.fuel_flow), 1, FLOAT},
+        { "engine_load", &(parsed.engine_load), 1, FLOAT},
+        { "throttle_position", &(parsed.throttle_position), 1, FLOAT},
+        { "spark_dwell_time", &(parsed.spark_dwell_time), 1, FLOAT},
+        { "barometric_pressure", &(parsed.barometric_pressure), 1, FLOAT},
+        { "intake_manifold_pressure", &(parsed.intake_manifold_pressure), 1, FLOAT},
+        { "intake_manifold_temperature", &(parsed.intake_manifold_temperature), 1, FLOAT},
+        { "cylinder_head_temperature", &(parsed.cylinder_head_temperature), 1, FLOAT},
+        { "ignition_timing", &(parsed.ignition_timing), 1, FLOAT},
+        { "injection_time", &(parsed.injection_time), 1, FLOAT},
+        { "exhaust_gas_temperature", &(parsed.exhaust_gas_temperature), 1, FLOAT},
+        { "throttle_out", &(parsed.throttle_out), 1, FLOAT},
+        { "pt_compensation", &(parsed.pt_compensation), 1, FLOAT},
+        { "health", &(parsed.health), 1, UINT8_T},
+        { "ignition_voltage", &(parsed.ignition_voltage), 1, FLOAT},
+        { "fuel_pressure", &(parsed.fuel_pressure), 1, FLOAT}
     };
-    static cStruct record = {"array_test_0", members, 5, 17150};
+    static cStruct record = {"efi_status", members, 19, 225};
 
-    mavlink_msg_array_test_0_decode(message, &parsed);
+    mavlink_msg_efi_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_array_test_5(const mavlink_message_t* message)
+cStruct* unbox_mission_clear_all(const mavlink_message_t* message)
 {
-    static mavlink_array_test_5_t parsed;
+    static mavlink_mission_clear_all_t parsed;
 
     static cMember members[] = {
-        { "c1", &(parsed.c1), 5, CHAR},
-        { "c2", &(parsed.c2), 5, CHAR}
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "mission_type", &(parsed.mission_type), 1, UINT8_T}
     };
-    static cStruct record = {"array_test_5", members, 2, 17155};
+    static cStruct record = {"mission_clear_all", members, 3, 45};
 
-    mavlink_msg_array_test_5_decode(message, &parsed);
+    mavlink_msg_mission_clear_all_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_array_test_4(const mavlink_message_t* message)
+cStruct* unbox_sys_status(const mavlink_message_t* message)
 {
-    static mavlink_array_test_4_t parsed;
+    static mavlink_sys_status_t parsed;
 
     static cMember members[] = {
-        { "ar_u32", &(parsed.ar_u32), 4, UINT32_T},
-        { "v", &(parsed.v), 1, UINT8_T}
+        { "onboard_control_sensors_present", &(parsed.onboard_control_sensors_present), 1, UINT32_T},
+        { "onboard_control_sensors_enabled", &(parsed.onboard_control_sensors_enabled), 1, UINT32_T},
+        { "onboard_control_sensors_health", &(parsed.onboard_control_sensors_health), 1, UINT32_T},
+        { "load", &(parsed.load), 1, UINT16_T},
+        { "voltage_battery", &(parsed.voltage_battery), 1, UINT16_T},
+        { "current_battery", &(parsed.current_battery), 1, INT16_T},
+        { "drop_rate_comm", &(parsed.drop_rate_comm), 1, UINT16_T},
+        { "errors_comm", &(parsed.errors_comm), 1, UINT16_T},
+        { "errors_count1", &(parsed.errors_count1), 1, UINT16_T},
+        { "errors_count2", &(parsed.errors_count2), 1, UINT16_T},
+        { "errors_count3", &(parsed.errors_count3), 1, UINT16_T},
+        { "errors_count4", &(parsed.errors_count4), 1, UINT16_T},
+        { "battery_remaining", &(parsed.battery_remaining), 1, INT8_T},
+        { "onboard_control_sensors_present_extended", &(parsed.onboard_control_sensors_present_extended), 1, UINT32_T},
+        { "onboard_control_sensors_enabled_extended", &(parsed.onboard_control_sensors_enabled_extended), 1, UINT32_T},
+        { "onboard_control_sensors_health_extended", &(parsed.onboard_control_sensors_health_extended), 1, UINT32_T}
     };
-    static cStruct record = {"array_test_4", members, 2, 17154};
+    static cStruct record = {"sys_status", members, 16, 1};
 
-    mavlink_msg_array_test_4_decode(message, &parsed);
+    mavlink_msg_sys_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_protocol_version(const mavlink_message_t* message)
+cStruct* unbox_estimator_status(const mavlink_message_t* message)
 {
-    static mavlink_protocol_version_t parsed;
+    static mavlink_estimator_status_t parsed;
 
     static cMember members[] = {
-        { "version", &(parsed.version), 1, UINT16_T},
-        { "min_version", &(parsed.min_version), 1, UINT16_T},
-        { "max_version", &(parsed.max_version), 1, UINT16_T},
-        { "spec_version_hash", &(parsed.spec_version_hash), 8, UINT8_T},
-        { "library_version_hash", &(parsed.library_version_hash), 8, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "vel_ratio", &(parsed.vel_ratio), 1, FLOAT},
+        { "pos_horiz_ratio", &(parsed.pos_horiz_ratio), 1, FLOAT},
+        { "pos_vert_ratio", &(parsed.pos_vert_ratio), 1, FLOAT},
+        { "mag_ratio", &(parsed.mag_ratio), 1, FLOAT},
+        { "hagl_ratio", &(parsed.hagl_ratio), 1, FLOAT},
+        { "tas_ratio", &(parsed.tas_ratio), 1, FLOAT},
+        { "pos_horiz_accuracy", &(parsed.pos_horiz_accuracy), 1, FLOAT},
+        { "pos_vert_accuracy", &(parsed.pos_vert_accuracy), 1, FLOAT},
+        { "flags", &(parsed.flags), 1, UINT16_T}
     };
-    static cStruct record = {"protocol_version", members, 5, 300};
+    static cStruct record = {"estimator_status", members, 10, 230};
 
-    mavlink_msg_protocol_version_decode(message, &parsed);
+    mavlink_msg_estimator_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_heartbeat(const mavlink_message_t* message)
+cStruct* unbox_set_position_target_global_int(const mavlink_message_t* message)
 {
-    static mavlink_heartbeat_t parsed;
+    static mavlink_set_position_target_global_int_t parsed;
 
     static cMember members[] = {
-        { "custom_mode", &(parsed.custom_mode), 1, UINT32_T},
-        { "type", &(parsed.type), 1, UINT8_T},
-        { "autopilot", &(parsed.autopilot), 1, UINT8_T},
-        { "base_mode", &(parsed.base_mode), 1, UINT8_T},
-        { "system_status", &(parsed.system_status), 1, UINT8_T},
-        { "mavlink_version", &(parsed.mavlink_version), 1, UINT8_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "lat_int", &(parsed.lat_int), 1, INT32_T},
+        { "lon_int", &(parsed.lon_int), 1, INT32_T},
+        { "alt", &(parsed.alt), 1, FLOAT},
+        { "vx", &(parsed.vx), 1, FLOAT},
+        { "vy", &(parsed.vy), 1, FLOAT},
+        { "vz", &(parsed.vz), 1, FLOAT},
+        { "afx", &(parsed.afx), 1, FLOAT},
+        { "afy", &(parsed.afy), 1, FLOAT},
+        { "afz", &(parsed.afz), 1, FLOAT},
+        { "yaw", &(parsed.yaw), 1, FLOAT},
+        { "yaw_rate", &(parsed.yaw_rate), 1, FLOAT},
+        { "type_mask", &(parsed.type_mask), 1, UINT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "coordinate_frame", &(parsed.coordinate_frame), 1, UINT8_T}
     };
-    static cStruct record = {"heartbeat", members, 6, 0};
+    static cStruct record = {"set_position_target_global_int", members, 16, 86};
 
-    mavlink_msg_heartbeat_decode(message, &parsed);
+    mavlink_msg_set_position_target_global_int_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_test_types(const mavlink_message_t* message)
+cStruct* unbox_data_stream(const mavlink_message_t* message)
 {
-    static mavlink_test_types_t parsed;
+    static mavlink_data_stream_t parsed;
 
     static cMember members[] = {
-        { "u64", &(parsed.u64), 1, UINT64_T},
-        { "s64", &(parsed.s64), 1, INT64_T},
-        { "d", &(parsed.d), 1, DOUBLE},
-        { "u64_array", &(parsed.u64_array), 3, UINT64_T},
-        { "s64_array", &(parsed.s64_array), 3, INT64_T},
-        { "d_array", &(parsed.d_array), 3, DOUBLE},
-        { "u32", &(parsed.u32), 1, UINT32_T},
-        { "s32", &(parsed.s32), 1, INT32_T},
-        { "f", &(parsed.f), 1, FLOAT},
-        { "u32_array", &(parsed.u32_array), 3, UINT32_T},
-        { "s32_array", &(parsed.s32_array), 3, INT32_T},
-        { "f_array", &(parsed.f_array), 3, FLOAT},
-        { "u16", &(parsed.u16), 1, UINT16_T},
-        { "s16", &(parsed.s16), 1, INT16_T},
-        { "u16_array", &(parsed.u16_array), 3, UINT16_T},
-        { "s16_array", &(parsed.s16_array), 3, INT16_T},
-        { "c", &(parsed.c), 1, CHAR},
-        { "s", &(parsed.s), 10, CHAR},
-        { "u8", &(parsed.u8), 1, UINT8_T},
-        { "s8", &(parsed.s8), 1, INT8_T},
-        { "u8_array", &(parsed.u8_array), 3, UINT8_T},
-        { "s8_array", &(parsed.s8_array), 3, INT8_T}
+        { "message_rate", &(parsed.message_rate), 1, UINT16_T},
+        { "stream_id", &(parsed.stream_id), 1, UINT8_T},
+        { "on_off", &(parsed.on_off), 1, UINT8_T}
     };
-    static cStruct record = {"test_types", members, 22, 17000};
+    static cStruct record = {"data_stream", members, 3, 67};
 
-    mavlink_msg_test_types_decode(message, &parsed);
+    mavlink_msg_data_stream_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_radio_calibration(const mavlink_message_t* message)
+cStruct* unbox_timesync(const mavlink_message_t* message)
 {
-    static mavlink_radio_calibration_t parsed;
+    static mavlink_timesync_t parsed;
 
     static cMember members[] = {
-        { "aileron", &(parsed.aileron), 3, UINT16_T},
-        { "elevator", &(parsed.elevator), 3, UINT16_T},
-        { "rudder", &(parsed.rudder), 3, UINT16_T},
-        { "gyro", &(parsed.gyro), 2, UINT16_T},
-        { "pitch", &(parsed.pitch), 5, UINT16_T},
-        { "throttle", &(parsed.throttle), 5, UINT16_T}
+        { "tc1", &(parsed.tc1), 1, INT64_T},
+        { "ts1", &(parsed.ts1), 1, INT64_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T}
     };
-    static cStruct record = {"radio_calibration", members, 6, 221};
+    static cStruct record = {"timesync", members, 4, 111};
 
-    mavlink_msg_radio_calibration_decode(message, &parsed);
+    mavlink_msg_timesync_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_ualberta_sys_status(const mavlink_message_t* message)
+cStruct* unbox_camera_tracking_geo_status(const mavlink_message_t* message)
 {
-    static mavlink_ualberta_sys_status_t parsed;
+    static mavlink_camera_tracking_geo_status_t parsed;
 
     static cMember members[] = {
-        { "mode", &(parsed.mode), 1, UINT8_T},
-        { "nav_mode", &(parsed.nav_mode), 1, UINT8_T},
-        { "pilot", &(parsed.pilot), 1, UINT8_T}
+        { "lat", &(parsed.lat), 1, INT32_T},
+        { "lon", &(parsed.lon), 1, INT32_T},
+        { "alt", &(parsed.alt), 1, FLOAT},
+        { "h_acc", &(parsed.h_acc), 1, FLOAT},
+        { "v_acc", &(parsed.v_acc), 1, FLOAT},
+        { "vel_n", &(parsed.vel_n), 1, FLOAT},
+        { "vel_e", &(parsed.vel_e), 1, FLOAT},
+        { "vel_d", &(parsed.vel_d), 1, FLOAT},
+        { "vel_acc", &(parsed.vel_acc), 1, FLOAT},
+        { "dist", &(parsed.dist), 1, FLOAT},
+        { "hdg", &(parsed.hdg), 1, FLOAT},
+        { "hdg_acc", &(parsed.hdg_acc), 1, FLOAT},
+        { "tracking_status", &(parsed.tracking_status), 1, UINT8_T}
     };
-    static cStruct record = {"ualberta_sys_status", members, 3, 222};
+    static cStruct record = {"camera_tracking_geo_status", members, 13, 276};
 
-    mavlink_msg_ualberta_sys_status_decode(message, &parsed);
+    mavlink_msg_camera_tracking_geo_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_nav_filter_bias(const mavlink_message_t* message)
+cStruct* unbox_gps_rtcm_data(const mavlink_message_t* message)
 {
-    static mavlink_nav_filter_bias_t parsed;
+    static mavlink_gps_rtcm_data_t parsed;
 
     static cMember members[] = {
-        { "usec", &(parsed.usec), 1, UINT64_T},
-        { "accel_0", &(parsed.accel_0), 1, FLOAT},
-        { "accel_1", &(parsed.accel_1), 1, FLOAT},
-        { "accel_2", &(parsed.accel_2), 1, FLOAT},
-        { "gyro_0", &(parsed.gyro_0), 1, FLOAT},
-        { "gyro_1", &(parsed.gyro_1), 1, FLOAT},
-        { "gyro_2", &(parsed.gyro_2), 1, FLOAT}
+        { "flags", &(parsed.flags), 1, UINT8_T},
+        { "len", &(parsed.len), 1, UINT8_T},
+        { "data", &(parsed.data), 180, UINT8_T}
     };
-    static cStruct record = {"nav_filter_bias", members, 7, 220};
+    static cStruct record = {"gps_rtcm_data", members, 3, 233};
 
-    mavlink_msg_nav_filter_bias_decode(message, &parsed);
+    mavlink_msg_gps_rtcm_data_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_hygrometer_sensor(const mavlink_message_t* message)
+cStruct* unbox_camera_settings(const mavlink_message_t* message)
 {
-    static mavlink_hygrometer_sensor_t parsed;
+    static mavlink_camera_settings_t parsed;
 
     static cMember members[] = {
-        { "temperature", &(parsed.temperature), 1, INT16_T},
-        { "humidity", &(parsed.humidity), 1, UINT16_T},
-        { "id", &(parsed.id), 1, UINT8_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "mode_id", &(parsed.mode_id), 1, UINT8_T},
+        { "zoomLevel", &(parsed.zoomLevel), 1, FLOAT},
+        { "focusLevel", &(parsed.focusLevel), 1, FLOAT}
     };
-    static cStruct record = {"hygrometer_sensor", members, 3, 12920};
+    static cStruct record = {"camera_settings", members, 4, 260};
 
-    mavlink_msg_hygrometer_sensor_decode(message, &parsed);
+    mavlink_msg_camera_settings_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_local_position_ned(const mavlink_message_t* message)
+cStruct* unbox_video_stream_information(const mavlink_message_t* message)
 {
-    static mavlink_local_position_ned_t parsed;
+    static mavlink_video_stream_information_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "x", &(parsed.x), 1, FLOAT},
-        { "y", &(parsed.y), 1, FLOAT},
-        { "z", &(parsed.z), 1, FLOAT},
-        { "vx", &(parsed.vx), 1, FLOAT},
-        { "vy", &(parsed.vy), 1, FLOAT},
-        { "vz", &(parsed.vz), 1, FLOAT}
+        { "framerate", &(parsed.framerate), 1, FLOAT},
+        { "bitrate", &(parsed.bitrate), 1, UINT32_T},
+        { "flags", &(parsed.flags), 1, UINT16_T},
+        { "resolution_h", &(parsed.resolution_h), 1, UINT16_T},
+        { "resolution_v", &(parsed.resolution_v), 1, UINT16_T},
+        { "rotation", &(parsed.rotation), 1, UINT16_T},
+        { "hfov", &(parsed.hfov), 1, UINT16_T},
+        { "stream_id", &(parsed.stream_id), 1, UINT8_T},
+        { "count", &(parsed.count), 1, UINT8_T},
+        { "type", &(parsed.type), 1, UINT8_T},
+        { "name", &(parsed.name), 32, CHAR},
+        { "uri", &(parsed.uri), 160, CHAR}
     };
-    static cStruct record = {"local_position_ned", members, 7, 32};
+    static cStruct record = {"video_stream_information", members, 12, 269};
 
-    mavlink_msg_local_position_ned_decode(message, &parsed);
+    mavlink_msg_video_stream_information_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_ais_vessel(const mavlink_message_t* message)
+cStruct* unbox_resource_request(const mavlink_message_t* message)
 {
-    static mavlink_ais_vessel_t parsed;
+    static mavlink_resource_request_t parsed;
 
     static cMember members[] = {
-        { "MMSI", &(parsed.MMSI), 1, UINT32_T},
-        { "lat", &(parsed.lat), 1, INT32_T},
-        { "lon", &(parsed.lon), 1, INT32_T},
-        { "COG", &(parsed.COG), 1, UINT16_T},
-        { "heading", &(parsed.heading), 1, UINT16_T},
-        { "velocity", &(parsed.velocity), 1, UINT16_T},
-        { "dimension_bow", &(parsed.dimension_bow), 1, UINT16_T},
-        { "dimension_stern", &(parsed.dimension_stern), 1, UINT16_T},
-        { "tslc", &(parsed.tslc), 1, UINT16_T},
-        { "flags", &(parsed.flags), 1, UINT16_T},
-        { "turn_rate", &(parsed.turn_rate), 1, INT8_T},
-        { "navigational_status", &(parsed.navigational_status), 1, UINT8_T},
-        { "type", &(parsed.type), 1, UINT8_T},
-        { "dimension_port", &(parsed.dimension_port), 1, UINT8_T},
-        { "dimension_starboard", &(parsed.dimension_starboard), 1, UINT8_T},
-        { "callsign", &(parsed.callsign), 7, CHAR},
-        { "name", &(parsed.name), 20, CHAR}
+        { "request_id", &(parsed.request_id), 1, UINT8_T},
+        { "uri_type", &(parsed.uri_type), 1, UINT8_T},
+        { "uri", &(parsed.uri), 120, UINT8_T},
+        { "transfer_type", &(parsed.transfer_type), 1, UINT8_T},
+        { "storage", &(parsed.storage), 120, UINT8_T}
     };
-    static cStruct record = {"ais_vessel", members, 17, 301};
+    static cStruct record = {"resource_request", members, 5, 142};
 
-    mavlink_msg_ais_vessel_decode(message, &parsed);
+    mavlink_msg_resource_request_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_gimbal_device_attitude_status(const mavlink_message_t* message)
+cStruct* unbox_request_data_stream(const mavlink_message_t* message)
 {
-    static mavlink_gimbal_device_attitude_status_t parsed;
+    static mavlink_request_data_stream_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "q", &(parsed.q), 4, FLOAT},
-        { "angular_velocity_x", &(parsed.angular_velocity_x), 1, FLOAT},
-        { "angular_velocity_y", &(parsed.angular_velocity_y), 1, FLOAT},
-        { "angular_velocity_z", &(parsed.angular_velocity_z), 1, FLOAT},
-        { "failure_flags", &(parsed.failure_flags), 1, UINT32_T},
-        { "flags", &(parsed.flags), 1, UINT16_T},
+        { "req_message_rate", &(parsed.req_message_rate), 1, UINT16_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "delta_yaw", &(parsed.delta_yaw), 1, FLOAT},
-        { "delta_yaw_velocity", &(parsed.delta_yaw_velocity), 1, FLOAT}
+        { "req_stream_id", &(parsed.req_stream_id), 1, UINT8_T},
+        { "start_stop", &(parsed.start_stop), 1, UINT8_T}
     };
-    static cStruct record = {"gimbal_device_attitude_status", members, 11, 285};
+    static cStruct record = {"request_data_stream", members, 5, 66};
 
-    mavlink_msg_gimbal_device_attitude_status_decode(message, &parsed);
+    mavlink_msg_request_data_stream_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_mission_write_partial_list(const mavlink_message_t* message)
+cStruct* unbox_open_drone_id_system(const mavlink_message_t* message)
 {
-    static mavlink_mission_write_partial_list_t parsed;
+    static mavlink_open_drone_id_system_t parsed;
 
     static cMember members[] = {
-        { "start_index", &(parsed.start_index), 1, INT16_T},
-        { "end_index", &(parsed.end_index), 1, INT16_T},
+        { "operator_latitude", &(parsed.operator_latitude), 1, INT32_T},
+        { "operator_longitude", &(parsed.operator_longitude), 1, INT32_T},
+        { "area_ceiling", &(parsed.area_ceiling), 1, FLOAT},
+        { "area_floor", &(parsed.area_floor), 1, FLOAT},
+        { "operator_altitude_geo", &(parsed.operator_altitude_geo), 1, FLOAT},
+        { "timestamp", &(parsed.timestamp), 1, UINT32_T},
+        { "area_count", &(parsed.area_count), 1, UINT16_T},
+        { "area_radius", &(parsed.area_radius), 1, UINT16_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "mission_type", &(parsed.mission_type), 1, UINT8_T}
+        { "id_or_mac", &(parsed.id_or_mac), 20, UINT8_T},
+        { "operator_location_type", &(parsed.operator_location_type), 1, UINT8_T},
+        { "classification_type", &(parsed.classification_type), 1, UINT8_T},
+        { "category_eu", &(parsed.category_eu), 1, UINT8_T},
+        { "class_eu", &(parsed.class_eu), 1, UINT8_T}
     };
-    static cStruct record = {"mission_write_partial_list", members, 5, 38};
+    static cStruct record = {"open_drone_id_system", members, 15, 12904};
 
-    mavlink_msg_mission_write_partial_list_decode(message, &parsed);
+    mavlink_msg_open_drone_id_system_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_scaled_imu2(const mavlink_message_t* message)
+cStruct* unbox_set_gps_global_origin(const mavlink_message_t* message)
 {
-    static mavlink_scaled_imu2_t parsed;
+    static mavlink_set_gps_global_origin_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "xacc", &(parsed.xacc), 1, INT16_T},
-        { "yacc", &(parsed.yacc), 1, INT16_T},
-        { "zacc", &(parsed.zacc), 1, INT16_T},
-        { "xgyro", &(parsed.xgyro), 1, INT16_T},
-        { "ygyro", &(parsed.ygyro), 1, INT16_T},
-        { "zgyro", &(parsed.zgyro), 1, INT16_T},
-        { "xmag", &(parsed.xmag), 1, INT16_T},
-        { "ymag", &(parsed.ymag), 1, INT16_T},
-        { "zmag", &(parsed.zmag), 1, INT16_T},
-        { "temperature", &(parsed.temperature), 1, INT16_T}
+        { "latitude", &(parsed.latitude), 1, INT32_T},
+        { "longitude", &(parsed.longitude), 1, INT32_T},
+        { "altitude", &(parsed.altitude), 1, INT32_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T}
     };
-    static cStruct record = {"scaled_imu2", members, 11, 116};
+    static cStruct record = {"set_gps_global_origin", members, 5, 48};
 
-    mavlink_msg_scaled_imu2_decode(message, &parsed);
+    mavlink_msg_set_gps_global_origin_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_vision_speed_estimate(const mavlink_message_t* message)
+cStruct* unbox_param_request_list(const mavlink_message_t* message)
 {
-    static mavlink_vision_speed_estimate_t parsed;
+    static mavlink_param_request_list_t parsed;
 
     static cMember members[] = {
-        { "usec", &(parsed.usec), 1, UINT64_T},
-        { "x", &(parsed.x), 1, FLOAT},
-        { "y", &(parsed.y), 1, FLOAT},
-        { "z", &(parsed.z), 1, FLOAT},
-        { "covariance", &(parsed.covariance), 9, FLOAT},
-        { "reset_counter", &(parsed.reset_counter), 1, UINT8_T}
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T}
     };
-    static cStruct record = {"vision_speed_estimate", members, 6, 103};
+    static cStruct record = {"param_request_list", members, 2, 21};
 
-    mavlink_msg_vision_speed_estimate_decode(message, &parsed);
+    mavlink_msg_param_request_list_decode(message, &parsed);
     return &record;
 }
 
 cStruct* unbox_serial_control(const mavlink_message_t* message)
 {
     static mavlink_serial_control_t parsed;
 
@@ -3032,180 +3191,138 @@
     };
     static cStruct record = {"serial_control", members, 8, 126};
 
     mavlink_msg_serial_control_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_mission_set_current(const mavlink_message_t* message)
-{
-    static mavlink_mission_set_current_t parsed;
-
-    static cMember members[] = {
-        { "seq", &(parsed.seq), 1, UINT16_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T}
-    };
-    static cStruct record = {"mission_set_current", members, 3, 41};
-
-    mavlink_msg_mission_set_current_decode(message, &parsed);
-    return &record;
-}
-
-cStruct* unbox_landing_target(const mavlink_message_t* message)
+cStruct* unbox_nav_controller_output(const mavlink_message_t* message)
 {
-    static mavlink_landing_target_t parsed;
+    static mavlink_nav_controller_output_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "angle_x", &(parsed.angle_x), 1, FLOAT},
-        { "angle_y", &(parsed.angle_y), 1, FLOAT},
-        { "distance", &(parsed.distance), 1, FLOAT},
-        { "size_x", &(parsed.size_x), 1, FLOAT},
-        { "size_y", &(parsed.size_y), 1, FLOAT},
-        { "target_num", &(parsed.target_num), 1, UINT8_T},
-        { "frame", &(parsed.frame), 1, UINT8_T},
-        { "x", &(parsed.x), 1, FLOAT},
-        { "y", &(parsed.y), 1, FLOAT},
-        { "z", &(parsed.z), 1, FLOAT},
-        { "q", &(parsed.q), 4, FLOAT},
-        { "type", &(parsed.type), 1, UINT8_T},
-        { "position_valid", &(parsed.position_valid), 1, UINT8_T}
+        { "nav_roll", &(parsed.nav_roll), 1, FLOAT},
+        { "nav_pitch", &(parsed.nav_pitch), 1, FLOAT},
+        { "alt_error", &(parsed.alt_error), 1, FLOAT},
+        { "aspd_error", &(parsed.aspd_error), 1, FLOAT},
+        { "xtrack_error", &(parsed.xtrack_error), 1, FLOAT},
+        { "nav_bearing", &(parsed.nav_bearing), 1, INT16_T},
+        { "target_bearing", &(parsed.target_bearing), 1, INT16_T},
+        { "wp_dist", &(parsed.wp_dist), 1, UINT16_T}
     };
-    static cStruct record = {"landing_target", members, 14, 149};
+    static cStruct record = {"nav_controller_output", members, 8, 62};
 
-    mavlink_msg_landing_target_decode(message, &parsed);
+    mavlink_msg_nav_controller_output_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_rc_channels(const mavlink_message_t* message)
+cStruct* unbox_raw_rpm(const mavlink_message_t* message)
 {
-    static mavlink_rc_channels_t parsed;
+    static mavlink_raw_rpm_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "chan1_raw", &(parsed.chan1_raw), 1, UINT16_T},
-        { "chan2_raw", &(parsed.chan2_raw), 1, UINT16_T},
-        { "chan3_raw", &(parsed.chan3_raw), 1, UINT16_T},
-        { "chan4_raw", &(parsed.chan4_raw), 1, UINT16_T},
-        { "chan5_raw", &(parsed.chan5_raw), 1, UINT16_T},
-        { "chan6_raw", &(parsed.chan6_raw), 1, UINT16_T},
-        { "chan7_raw", &(parsed.chan7_raw), 1, UINT16_T},
-        { "chan8_raw", &(parsed.chan8_raw), 1, UINT16_T},
-        { "chan9_raw", &(parsed.chan9_raw), 1, UINT16_T},
-        { "chan10_raw", &(parsed.chan10_raw), 1, UINT16_T},
-        { "chan11_raw", &(parsed.chan11_raw), 1, UINT16_T},
-        { "chan12_raw", &(parsed.chan12_raw), 1, UINT16_T},
-        { "chan13_raw", &(parsed.chan13_raw), 1, UINT16_T},
-        { "chan14_raw", &(parsed.chan14_raw), 1, UINT16_T},
-        { "chan15_raw", &(parsed.chan15_raw), 1, UINT16_T},
-        { "chan16_raw", &(parsed.chan16_raw), 1, UINT16_T},
-        { "chan17_raw", &(parsed.chan17_raw), 1, UINT16_T},
-        { "chan18_raw", &(parsed.chan18_raw), 1, UINT16_T},
-        { "chancount", &(parsed.chancount), 1, UINT8_T},
-        { "rssi", &(parsed.rssi), 1, UINT8_T}
+        { "frequency", &(parsed.frequency), 1, FLOAT},
+        { "index", &(parsed.index), 1, UINT8_T}
     };
-    static cStruct record = {"rc_channels", members, 21, 65};
+    static cStruct record = {"raw_rpm", members, 2, 339};
 
-    mavlink_msg_rc_channels_decode(message, &parsed);
+    mavlink_msg_raw_rpm_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_command_ack(const mavlink_message_t* message)
+cStruct* unbox_log_erase(const mavlink_message_t* message)
 {
-    static mavlink_command_ack_t parsed;
+    static mavlink_log_erase_t parsed;
 
     static cMember members[] = {
-        { "command", &(parsed.command), 1, UINT16_T},
-        { "result", &(parsed.result), 1, UINT8_T},
-        { "progress", &(parsed.progress), 1, UINT8_T},
-        { "result_param2", &(parsed.result_param2), 1, INT32_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T}
     };
-    static cStruct record = {"command_ack", members, 6, 77};
-
-    mavlink_msg_command_ack_decode(message, &parsed);
-    return &record;
-}
-
-cStruct* unbox_autopilot_version(const mavlink_message_t* message)
-{
-    static mavlink_autopilot_version_t parsed;
-
-    static cMember members[] = {
-        { "capabilities", &(parsed.capabilities), 1, UINT64_T},
-        { "uid", &(parsed.uid), 1, UINT64_T},
-        { "flight_sw_version", &(parsed.flight_sw_version), 1, UINT32_T},
-        { "middleware_sw_version", &(parsed.middleware_sw_version), 1, UINT32_T},
-        { "os_sw_version", &(parsed.os_sw_version), 1, UINT32_T},
-        { "board_version", &(parsed.board_version), 1, UINT32_T},
-        { "vendor_id", &(parsed.vendor_id), 1, UINT16_T},
-        { "product_id", &(parsed.product_id), 1, UINT16_T},
-        { "flight_custom_version", &(parsed.flight_custom_version), 8, UINT8_T},
-        { "middleware_custom_version", &(parsed.middleware_custom_version), 8, UINT8_T},
-        { "os_custom_version", &(parsed.os_custom_version), 8, UINT8_T},
-        { "uid2", &(parsed.uid2), 18, UINT8_T}
-    };
-    static cStruct record = {"autopilot_version", members, 12, 148};
+    static cStruct record = {"log_erase", members, 2, 121};
 
-    mavlink_msg_autopilot_version_decode(message, &parsed);
+    mavlink_msg_log_erase_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_safety_set_allowed_area(const mavlink_message_t* message)
+cStruct* unbox_high_latency2(const mavlink_message_t* message)
 {
-    static mavlink_safety_set_allowed_area_t parsed;
+    static mavlink_high_latency2_t parsed;
 
     static cMember members[] = {
-        { "p1x", &(parsed.p1x), 1, FLOAT},
-        { "p1y", &(parsed.p1y), 1, FLOAT},
-        { "p1z", &(parsed.p1z), 1, FLOAT},
-        { "p2x", &(parsed.p2x), 1, FLOAT},
-        { "p2y", &(parsed.p2y), 1, FLOAT},
-        { "p2z", &(parsed.p2z), 1, FLOAT},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "frame", &(parsed.frame), 1, UINT8_T}
+        { "timestamp", &(parsed.timestamp), 1, UINT32_T},
+        { "latitude", &(parsed.latitude), 1, INT32_T},
+        { "longitude", &(parsed.longitude), 1, INT32_T},
+        { "custom_mode", &(parsed.custom_mode), 1, UINT16_T},
+        { "altitude", &(parsed.altitude), 1, INT16_T},
+        { "target_altitude", &(parsed.target_altitude), 1, INT16_T},
+        { "target_distance", &(parsed.target_distance), 1, UINT16_T},
+        { "wp_num", &(parsed.wp_num), 1, UINT16_T},
+        { "failure_flags", &(parsed.failure_flags), 1, UINT16_T},
+        { "type", &(parsed.type), 1, UINT8_T},
+        { "autopilot", &(parsed.autopilot), 1, UINT8_T},
+        { "heading", &(parsed.heading), 1, UINT8_T},
+        { "target_heading", &(parsed.target_heading), 1, UINT8_T},
+        { "throttle", &(parsed.throttle), 1, UINT8_T},
+        { "airspeed", &(parsed.airspeed), 1, UINT8_T},
+        { "airspeed_sp", &(parsed.airspeed_sp), 1, UINT8_T},
+        { "groundspeed", &(parsed.groundspeed), 1, UINT8_T},
+        { "windspeed", &(parsed.windspeed), 1, UINT8_T},
+        { "wind_heading", &(parsed.wind_heading), 1, UINT8_T},
+        { "eph", &(parsed.eph), 1, UINT8_T},
+        { "epv", &(parsed.epv), 1, UINT8_T},
+        { "temperature_air", &(parsed.temperature_air), 1, INT8_T},
+        { "climb_rate", &(parsed.climb_rate), 1, INT8_T},
+        { "battery", &(parsed.battery), 1, INT8_T},
+        { "custom0", &(parsed.custom0), 1, INT8_T},
+        { "custom1", &(parsed.custom1), 1, INT8_T},
+        { "custom2", &(parsed.custom2), 1, INT8_T}
     };
-    static cStruct record = {"safety_set_allowed_area", members, 9, 54};
+    static cStruct record = {"high_latency2", members, 27, 235};
 
-    mavlink_msg_safety_set_allowed_area_decode(message, &parsed);
+    mavlink_msg_high_latency2_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_memory_vect(const mavlink_message_t* message)
+cStruct* unbox_storage_information(const mavlink_message_t* message)
 {
-    static mavlink_memory_vect_t parsed;
+    static mavlink_storage_information_t parsed;
 
     static cMember members[] = {
-        { "address", &(parsed.address), 1, UINT16_T},
-        { "ver", &(parsed.ver), 1, UINT8_T},
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "total_capacity", &(parsed.total_capacity), 1, FLOAT},
+        { "used_capacity", &(parsed.used_capacity), 1, FLOAT},
+        { "available_capacity", &(parsed.available_capacity), 1, FLOAT},
+        { "read_speed", &(parsed.read_speed), 1, FLOAT},
+        { "write_speed", &(parsed.write_speed), 1, FLOAT},
+        { "storage_id", &(parsed.storage_id), 1, UINT8_T},
+        { "storage_count", &(parsed.storage_count), 1, UINT8_T},
+        { "status", &(parsed.status), 1, UINT8_T},
         { "type", &(parsed.type), 1, UINT8_T},
-        { "value", &(parsed.value), 32, INT8_T}
+        { "name", &(parsed.name), 32, CHAR},
+        { "storage_usage", &(parsed.storage_usage), 1, UINT8_T}
     };
-    static cStruct record = {"memory_vect", members, 4, 249};
+    static cStruct record = {"storage_information", members, 12, 261};
 
-    mavlink_msg_memory_vect_decode(message, &parsed);
+    mavlink_msg_storage_information_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_request_event(const mavlink_message_t* message)
+cStruct* unbox_ping(const mavlink_message_t* message)
 {
-    static mavlink_request_event_t parsed;
+    static mavlink_ping_t parsed;
 
     static cMember members[] = {
-        { "first_sequence", &(parsed.first_sequence), 1, UINT16_T},
-        { "last_sequence", &(parsed.last_sequence), 1, UINT16_T},
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "seq", &(parsed.seq), 1, UINT32_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T}
     };
-    static cStruct record = {"request_event", members, 4, 412};
+    static cStruct record = {"ping", members, 4, 4};
 
-    mavlink_msg_request_event_decode(message, &parsed);
+    mavlink_msg_ping_decode(message, &parsed);
     return &record;
 }
 
 cStruct* unbox_rc_channels_scaled(const mavlink_message_t* message)
 {
     static mavlink_rc_channels_scaled_t parsed;
 
@@ -3224,284 +3341,127 @@
     };
     static cStruct record = {"rc_channels_scaled", members, 11, 34};
 
     mavlink_msg_rc_channels_scaled_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_isbd_link_status(const mavlink_message_t* message)
-{
-    static mavlink_isbd_link_status_t parsed;
-
-    static cMember members[] = {
-        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
-        { "last_heartbeat", &(parsed.last_heartbeat), 1, UINT64_T},
-        { "failed_sessions", &(parsed.failed_sessions), 1, UINT16_T},
-        { "successful_sessions", &(parsed.successful_sessions), 1, UINT16_T},
-        { "signal_quality", &(parsed.signal_quality), 1, UINT8_T},
-        { "ring_pending", &(parsed.ring_pending), 1, UINT8_T},
-        { "tx_session_pending", &(parsed.tx_session_pending), 1, UINT8_T},
-        { "rx_session_pending", &(parsed.rx_session_pending), 1, UINT8_T}
-    };
-    static cStruct record = {"isbd_link_status", members, 8, 335};
-
-    mavlink_msg_isbd_link_status_decode(message, &parsed);
-    return &record;
-}
-
-cStruct* unbox_gps_inject_data(const mavlink_message_t* message)
-{
-    static mavlink_gps_inject_data_t parsed;
-
-    static cMember members[] = {
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "len", &(parsed.len), 1, UINT8_T},
-        { "data", &(parsed.data), 110, UINT8_T}
-    };
-    static cStruct record = {"gps_inject_data", members, 4, 123};
-
-    mavlink_msg_gps_inject_data_decode(message, &parsed);
-    return &record;
-}
-
-cStruct* unbox_mission_item_int(const mavlink_message_t* message)
+cStruct* unbox_orbit_execution_status(const mavlink_message_t* message)
 {
-    static mavlink_mission_item_int_t parsed;
+    static mavlink_orbit_execution_status_t parsed;
 
     static cMember members[] = {
-        { "param1", &(parsed.param1), 1, FLOAT},
-        { "param2", &(parsed.param2), 1, FLOAT},
-        { "param3", &(parsed.param3), 1, FLOAT},
-        { "param4", &(parsed.param4), 1, FLOAT},
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "radius", &(parsed.radius), 1, FLOAT},
         { "x", &(parsed.x), 1, INT32_T},
         { "y", &(parsed.y), 1, INT32_T},
         { "z", &(parsed.z), 1, FLOAT},
-        { "seq", &(parsed.seq), 1, UINT16_T},
-        { "command", &(parsed.command), 1, UINT16_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "frame", &(parsed.frame), 1, UINT8_T},
-        { "current", &(parsed.current), 1, UINT8_T},
-        { "autocontinue", &(parsed.autocontinue), 1, UINT8_T},
-        { "mission_type", &(parsed.mission_type), 1, UINT8_T}
-    };
-    static cStruct record = {"mission_item_int", members, 15, 73};
-
-    mavlink_msg_mission_item_int_decode(message, &parsed);
-    return &record;
-}
-
-cStruct* unbox_gimbal_device_information(const mavlink_message_t* message)
-{
-    static mavlink_gimbal_device_information_t parsed;
-
-    static cMember members[] = {
-        { "uid", &(parsed.uid), 1, UINT64_T},
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "firmware_version", &(parsed.firmware_version), 1, UINT32_T},
-        { "hardware_version", &(parsed.hardware_version), 1, UINT32_T},
-        { "roll_min", &(parsed.roll_min), 1, FLOAT},
-        { "roll_max", &(parsed.roll_max), 1, FLOAT},
-        { "pitch_min", &(parsed.pitch_min), 1, FLOAT},
-        { "pitch_max", &(parsed.pitch_max), 1, FLOAT},
-        { "yaw_min", &(parsed.yaw_min), 1, FLOAT},
-        { "yaw_max", &(parsed.yaw_max), 1, FLOAT},
-        { "cap_flags", &(parsed.cap_flags), 1, UINT16_T},
-        { "custom_cap_flags", &(parsed.custom_cap_flags), 1, UINT16_T},
-        { "vendor_name", &(parsed.vendor_name), 32, CHAR},
-        { "model_name", &(parsed.model_name), 32, CHAR},
-        { "custom_name", &(parsed.custom_name), 32, CHAR}
-    };
-    static cStruct record = {"gimbal_device_information", members, 15, 283};
-
-    mavlink_msg_gimbal_device_information_decode(message, &parsed);
-    return &record;
-}
-
-cStruct* unbox_scaled_imu3(const mavlink_message_t* message)
-{
-    static mavlink_scaled_imu3_t parsed;
-
-    static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "xacc", &(parsed.xacc), 1, INT16_T},
-        { "yacc", &(parsed.yacc), 1, INT16_T},
-        { "zacc", &(parsed.zacc), 1, INT16_T},
-        { "xgyro", &(parsed.xgyro), 1, INT16_T},
-        { "ygyro", &(parsed.ygyro), 1, INT16_T},
-        { "zgyro", &(parsed.zgyro), 1, INT16_T},
-        { "xmag", &(parsed.xmag), 1, INT16_T},
-        { "ymag", &(parsed.ymag), 1, INT16_T},
-        { "zmag", &(parsed.zmag), 1, INT16_T},
-        { "temperature", &(parsed.temperature), 1, INT16_T}
-    };
-    static cStruct record = {"scaled_imu3", members, 11, 129};
-
-    mavlink_msg_scaled_imu3_decode(message, &parsed);
-    return &record;
-}
-
-cStruct* unbox_manual_setpoint(const mavlink_message_t* message)
-{
-    static mavlink_manual_setpoint_t parsed;
-
-    static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "roll", &(parsed.roll), 1, FLOAT},
-        { "pitch", &(parsed.pitch), 1, FLOAT},
-        { "yaw", &(parsed.yaw), 1, FLOAT},
-        { "thrust", &(parsed.thrust), 1, FLOAT},
-        { "mode_switch", &(parsed.mode_switch), 1, UINT8_T},
-        { "manual_override_switch", &(parsed.manual_override_switch), 1, UINT8_T}
-    };
-    static cStruct record = {"manual_setpoint", members, 7, 81};
-
-    mavlink_msg_manual_setpoint_decode(message, &parsed);
-    return &record;
-}
-
-cStruct* unbox_safety_allowed_area(const mavlink_message_t* message)
-{
-    static mavlink_safety_allowed_area_t parsed;
-
-    static cMember members[] = {
-        { "p1x", &(parsed.p1x), 1, FLOAT},
-        { "p1y", &(parsed.p1y), 1, FLOAT},
-        { "p1z", &(parsed.p1z), 1, FLOAT},
-        { "p2x", &(parsed.p2x), 1, FLOAT},
-        { "p2y", &(parsed.p2y), 1, FLOAT},
-        { "p2z", &(parsed.p2z), 1, FLOAT},
         { "frame", &(parsed.frame), 1, UINT8_T}
     };
-    static cStruct record = {"safety_allowed_area", members, 7, 55};
+    static cStruct record = {"orbit_execution_status", members, 6, 360};
 
-    mavlink_msg_safety_allowed_area_decode(message, &parsed);
+    mavlink_msg_orbit_execution_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_follow_target(const mavlink_message_t* message)
+cStruct* unbox_debug_float_array(const mavlink_message_t* message)
 {
-    static mavlink_follow_target_t parsed;
+    static mavlink_debug_float_array_t parsed;
 
     static cMember members[] = {
-        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
-        { "custom_state", &(parsed.custom_state), 1, UINT64_T},
-        { "lat", &(parsed.lat), 1, INT32_T},
-        { "lon", &(parsed.lon), 1, INT32_T},
-        { "alt", &(parsed.alt), 1, FLOAT},
-        { "vel", &(parsed.vel), 3, FLOAT},
-        { "acc", &(parsed.acc), 3, FLOAT},
-        { "attitude_q", &(parsed.attitude_q), 4, FLOAT},
-        { "rates", &(parsed.rates), 3, FLOAT},
-        { "position_cov", &(parsed.position_cov), 3, FLOAT},
-        { "est_capabilities", &(parsed.est_capabilities), 1, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "array_id", &(parsed.array_id), 1, UINT16_T},
+        { "name", &(parsed.name), 10, CHAR},
+        { "data", &(parsed.data), 58, FLOAT}
     };
-    static cStruct record = {"follow_target", members, 11, 144};
+    static cStruct record = {"debug_float_array", members, 4, 350};
 
-    mavlink_msg_follow_target_decode(message, &parsed);
+    mavlink_msg_debug_float_array_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_gps_rtcm_data(const mavlink_message_t* message)
+cStruct* unbox_command_ack(const mavlink_message_t* message)
 {
-    static mavlink_gps_rtcm_data_t parsed;
+    static mavlink_command_ack_t parsed;
 
     static cMember members[] = {
-        { "flags", &(parsed.flags), 1, UINT8_T},
-        { "len", &(parsed.len), 1, UINT8_T},
-        { "data", &(parsed.data), 180, UINT8_T}
+        { "command", &(parsed.command), 1, UINT16_T},
+        { "result", &(parsed.result), 1, UINT8_T},
+        { "progress", &(parsed.progress), 1, UINT8_T},
+        { "result_param2", &(parsed.result_param2), 1, INT32_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T}
     };
-    static cStruct record = {"gps_rtcm_data", members, 3, 233};
+    static cStruct record = {"command_ack", members, 6, 77};
 
-    mavlink_msg_gps_rtcm_data_decode(message, &parsed);
+    mavlink_msg_command_ack_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_rc_channels_raw(const mavlink_message_t* message)
+cStruct* unbox_supported_tunes(const mavlink_message_t* message)
 {
-    static mavlink_rc_channels_raw_t parsed;
+    static mavlink_supported_tunes_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "chan1_raw", &(parsed.chan1_raw), 1, UINT16_T},
-        { "chan2_raw", &(parsed.chan2_raw), 1, UINT16_T},
-        { "chan3_raw", &(parsed.chan3_raw), 1, UINT16_T},
-        { "chan4_raw", &(parsed.chan4_raw), 1, UINT16_T},
-        { "chan5_raw", &(parsed.chan5_raw), 1, UINT16_T},
-        { "chan6_raw", &(parsed.chan6_raw), 1, UINT16_T},
-        { "chan7_raw", &(parsed.chan7_raw), 1, UINT16_T},
-        { "chan8_raw", &(parsed.chan8_raw), 1, UINT16_T},
-        { "port", &(parsed.port), 1, UINT8_T},
-        { "rssi", &(parsed.rssi), 1, UINT8_T}
+        { "format", &(parsed.format), 1, UINT32_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T}
     };
-    static cStruct record = {"rc_channels_raw", members, 11, 35};
+    static cStruct record = {"supported_tunes", members, 3, 401};
 
-    mavlink_msg_rc_channels_raw_decode(message, &parsed);
+    mavlink_msg_supported_tunes_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_hil_gps(const mavlink_message_t* message)
+cStruct* unbox_adsb_vehicle(const mavlink_message_t* message)
 {
-    static mavlink_hil_gps_t parsed;
+    static mavlink_adsb_vehicle_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "ICAO_address", &(parsed.ICAO_address), 1, UINT32_T},
         { "lat", &(parsed.lat), 1, INT32_T},
         { "lon", &(parsed.lon), 1, INT32_T},
-        { "alt", &(parsed.alt), 1, INT32_T},
-        { "eph", &(parsed.eph), 1, UINT16_T},
-        { "epv", &(parsed.epv), 1, UINT16_T},
-        { "vel", &(parsed.vel), 1, UINT16_T},
-        { "vn", &(parsed.vn), 1, INT16_T},
-        { "ve", &(parsed.ve), 1, INT16_T},
-        { "vd", &(parsed.vd), 1, INT16_T},
-        { "cog", &(parsed.cog), 1, UINT16_T},
-        { "fix_type", &(parsed.fix_type), 1, UINT8_T},
-        { "satellites_visible", &(parsed.satellites_visible), 1, UINT8_T},
-        { "id", &(parsed.id), 1, UINT8_T},
-        { "yaw", &(parsed.yaw), 1, UINT16_T}
-    };
-    static cStruct record = {"hil_gps", members, 15, 113};
-
-    mavlink_msg_hil_gps_decode(message, &parsed);
-    return &record;
-}
-
-cStruct* unbox_attitude(const mavlink_message_t* message)
-{
-    static mavlink_attitude_t parsed;
-
-    static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "roll", &(parsed.roll), 1, FLOAT},
-        { "pitch", &(parsed.pitch), 1, FLOAT},
-        { "yaw", &(parsed.yaw), 1, FLOAT},
-        { "rollspeed", &(parsed.rollspeed), 1, FLOAT},
-        { "pitchspeed", &(parsed.pitchspeed), 1, FLOAT},
-        { "yawspeed", &(parsed.yawspeed), 1, FLOAT}
+        { "altitude", &(parsed.altitude), 1, INT32_T},
+        { "heading", &(parsed.heading), 1, UINT16_T},
+        { "hor_velocity", &(parsed.hor_velocity), 1, UINT16_T},
+        { "ver_velocity", &(parsed.ver_velocity), 1, INT16_T},
+        { "flags", &(parsed.flags), 1, UINT16_T},
+        { "squawk", &(parsed.squawk), 1, UINT16_T},
+        { "altitude_type", &(parsed.altitude_type), 1, UINT8_T},
+        { "callsign", &(parsed.callsign), 9, CHAR},
+        { "emitter_type", &(parsed.emitter_type), 1, UINT8_T},
+        { "tslc", &(parsed.tslc), 1, UINT8_T}
     };
-    static cStruct record = {"attitude", members, 7, 30};
+    static cStruct record = {"adsb_vehicle", members, 13, 246};
 
-    mavlink_msg_attitude_decode(message, &parsed);
+    mavlink_msg_adsb_vehicle_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_component_metadata(const mavlink_message_t* message)
+cStruct* unbox_set_home_position(const mavlink_message_t* message)
 {
-    static mavlink_component_metadata_t parsed;
+    static mavlink_set_home_position_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "file_crc", &(parsed.file_crc), 1, UINT32_T},
-        { "uri", &(parsed.uri), 100, CHAR}
+        { "latitude", &(parsed.latitude), 1, INT32_T},
+        { "longitude", &(parsed.longitude), 1, INT32_T},
+        { "altitude", &(parsed.altitude), 1, INT32_T},
+        { "x", &(parsed.x), 1, FLOAT},
+        { "y", &(parsed.y), 1, FLOAT},
+        { "z", &(parsed.z), 1, FLOAT},
+        { "q", &(parsed.q), 4, FLOAT},
+        { "approach_x", &(parsed.approach_x), 1, FLOAT},
+        { "approach_y", &(parsed.approach_y), 1, FLOAT},
+        { "approach_z", &(parsed.approach_z), 1, FLOAT},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T}
     };
-    static cStruct record = {"component_metadata", members, 3, 397};
+    static cStruct record = {"set_home_position", members, 12, 243};
 
-    mavlink_msg_component_metadata_decode(message, &parsed);
+    mavlink_msg_set_home_position_decode(message, &parsed);
     return &record;
 }
 
 cStruct* unbox_gps_raw_int(const mavlink_message_t* message)
 {
     static mavlink_gps_raw_int_t parsed;
 
@@ -3525,96 +3485,89 @@
     };
     static cStruct record = {"gps_raw_int", members, 16, 24};
 
     mavlink_msg_gps_raw_int_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_mission_clear_all(const mavlink_message_t* message)
+cStruct* unbox_mission_request_list(const mavlink_message_t* message)
 {
-    static mavlink_mission_clear_all_t parsed;
+    static mavlink_mission_request_list_t parsed;
 
     static cMember members[] = {
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T},
         { "mission_type", &(parsed.mission_type), 1, UINT8_T}
     };
-    static cStruct record = {"mission_clear_all", members, 3, 45};
+    static cStruct record = {"mission_request_list", members, 3, 43};
 
-    mavlink_msg_mission_clear_all_decode(message, &parsed);
+    mavlink_msg_mission_request_list_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_position_target_global_int(const mavlink_message_t* message)
+cStruct* unbox_servo_output_raw(const mavlink_message_t* message)
 {
-    static mavlink_position_target_global_int_t parsed;
+    static mavlink_servo_output_raw_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "lat_int", &(parsed.lat_int), 1, INT32_T},
-        { "lon_int", &(parsed.lon_int), 1, INT32_T},
-        { "alt", &(parsed.alt), 1, FLOAT},
-        { "vx", &(parsed.vx), 1, FLOAT},
-        { "vy", &(parsed.vy), 1, FLOAT},
-        { "vz", &(parsed.vz), 1, FLOAT},
-        { "afx", &(parsed.afx), 1, FLOAT},
-        { "afy", &(parsed.afy), 1, FLOAT},
-        { "afz", &(parsed.afz), 1, FLOAT},
-        { "yaw", &(parsed.yaw), 1, FLOAT},
-        { "yaw_rate", &(parsed.yaw_rate), 1, FLOAT},
-        { "type_mask", &(parsed.type_mask), 1, UINT16_T},
-        { "coordinate_frame", &(parsed.coordinate_frame), 1, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT32_T},
+        { "servo1_raw", &(parsed.servo1_raw), 1, UINT16_T},
+        { "servo2_raw", &(parsed.servo2_raw), 1, UINT16_T},
+        { "servo3_raw", &(parsed.servo3_raw), 1, UINT16_T},
+        { "servo4_raw", &(parsed.servo4_raw), 1, UINT16_T},
+        { "servo5_raw", &(parsed.servo5_raw), 1, UINT16_T},
+        { "servo6_raw", &(parsed.servo6_raw), 1, UINT16_T},
+        { "servo7_raw", &(parsed.servo7_raw), 1, UINT16_T},
+        { "servo8_raw", &(parsed.servo8_raw), 1, UINT16_T},
+        { "port", &(parsed.port), 1, UINT8_T},
+        { "servo9_raw", &(parsed.servo9_raw), 1, UINT16_T},
+        { "servo10_raw", &(parsed.servo10_raw), 1, UINT16_T},
+        { "servo11_raw", &(parsed.servo11_raw), 1, UINT16_T},
+        { "servo12_raw", &(parsed.servo12_raw), 1, UINT16_T},
+        { "servo13_raw", &(parsed.servo13_raw), 1, UINT16_T},
+        { "servo14_raw", &(parsed.servo14_raw), 1, UINT16_T},
+        { "servo15_raw", &(parsed.servo15_raw), 1, UINT16_T},
+        { "servo16_raw", &(parsed.servo16_raw), 1, UINT16_T}
     };
-    static cStruct record = {"position_target_global_int", members, 14, 87};
+    static cStruct record = {"servo_output_raw", members, 18, 36};
 
-    mavlink_msg_position_target_global_int_decode(message, &parsed);
+    mavlink_msg_servo_output_raw_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_manual_control(const mavlink_message_t* message)
+cStruct* unbox_logging_ack(const mavlink_message_t* message)
 {
-    static mavlink_manual_control_t parsed;
+    static mavlink_logging_ack_t parsed;
 
     static cMember members[] = {
-        { "x", &(parsed.x), 1, INT16_T},
-        { "y", &(parsed.y), 1, INT16_T},
-        { "z", &(parsed.z), 1, INT16_T},
-        { "r", &(parsed.r), 1, INT16_T},
-        { "buttons", &(parsed.buttons), 1, UINT16_T},
-        { "target", &(parsed.target), 1, UINT8_T},
-        { "buttons2", &(parsed.buttons2), 1, UINT16_T},
-        { "enabled_extensions", &(parsed.enabled_extensions), 1, UINT8_T},
-        { "s", &(parsed.s), 1, INT16_T},
-        { "t", &(parsed.t), 1, INT16_T}
+        { "sequence", &(parsed.sequence), 1, UINT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T}
     };
-    static cStruct record = {"manual_control", members, 10, 69};
+    static cStruct record = {"logging_ack", members, 3, 268};
 
-    mavlink_msg_manual_control_decode(message, &parsed);
+    mavlink_msg_logging_ack_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_camera_tracking_image_status(const mavlink_message_t* message)
+cStruct* unbox_can_frame(const mavlink_message_t* message)
 {
-    static mavlink_camera_tracking_image_status_t parsed;
+    static mavlink_can_frame_t parsed;
 
     static cMember members[] = {
-        { "point_x", &(parsed.point_x), 1, FLOAT},
-        { "point_y", &(parsed.point_y), 1, FLOAT},
-        { "radius", &(parsed.radius), 1, FLOAT},
-        { "rec_top_x", &(parsed.rec_top_x), 1, FLOAT},
-        { "rec_top_y", &(parsed.rec_top_y), 1, FLOAT},
-        { "rec_bottom_x", &(parsed.rec_bottom_x), 1, FLOAT},
-        { "rec_bottom_y", &(parsed.rec_bottom_y), 1, FLOAT},
-        { "tracking_status", &(parsed.tracking_status), 1, UINT8_T},
-        { "tracking_mode", &(parsed.tracking_mode), 1, UINT8_T},
-        { "target_data", &(parsed.target_data), 1, UINT8_T}
+        { "id", &(parsed.id), 1, UINT32_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "bus", &(parsed.bus), 1, UINT8_T},
+        { "len", &(parsed.len), 1, UINT8_T},
+        { "data", &(parsed.data), 8, UINT8_T}
     };
-    static cStruct record = {"camera_tracking_image_status", members, 10, 275};
+    static cStruct record = {"can_frame", members, 6, 386};
 
-    mavlink_msg_camera_tracking_image_status_decode(message, &parsed);
+    mavlink_msg_can_frame_decode(message, &parsed);
     return &record;
 }
 
 cStruct* unbox_debug(const mavlink_message_t* message)
 {
     static mavlink_debug_t parsed;
 
@@ -3625,244 +3578,71 @@
     };
     static cStruct record = {"debug", members, 3, 254};
 
     mavlink_msg_debug_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_video_stream_information(const mavlink_message_t* message)
-{
-    static mavlink_video_stream_information_t parsed;
-
-    static cMember members[] = {
-        { "framerate", &(parsed.framerate), 1, FLOAT},
-        { "bitrate", &(parsed.bitrate), 1, UINT32_T},
-        { "flags", &(parsed.flags), 1, UINT16_T},
-        { "resolution_h", &(parsed.resolution_h), 1, UINT16_T},
-        { "resolution_v", &(parsed.resolution_v), 1, UINT16_T},
-        { "rotation", &(parsed.rotation), 1, UINT16_T},
-        { "hfov", &(parsed.hfov), 1, UINT16_T},
-        { "stream_id", &(parsed.stream_id), 1, UINT8_T},
-        { "count", &(parsed.count), 1, UINT8_T},
-        { "type", &(parsed.type), 1, UINT8_T},
-        { "name", &(parsed.name), 32, CHAR},
-        { "uri", &(parsed.uri), 160, CHAR}
-    };
-    static cStruct record = {"video_stream_information", members, 12, 269};
-
-    mavlink_msg_video_stream_information_decode(message, &parsed);
-    return &record;
-}
-
-cStruct* unbox_mission_request_partial_list(const mavlink_message_t* message)
-{
-    static mavlink_mission_request_partial_list_t parsed;
-
-    static cMember members[] = {
-        { "start_index", &(parsed.start_index), 1, INT16_T},
-        { "end_index", &(parsed.end_index), 1, INT16_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "mission_type", &(parsed.mission_type), 1, UINT8_T}
-    };
-    static cStruct record = {"mission_request_partial_list", members, 5, 37};
-
-    mavlink_msg_mission_request_partial_list_decode(message, &parsed);
-    return &record;
-}
-
-cStruct* unbox_open_drone_id_arm_status(const mavlink_message_t* message)
-{
-    static mavlink_open_drone_id_arm_status_t parsed;
-
-    static cMember members[] = {
-        { "status", &(parsed.status), 1, UINT8_T},
-        { "error", &(parsed.error), 50, CHAR}
-    };
-    static cStruct record = {"open_drone_id_arm_status", members, 2, 12918};
-
-    mavlink_msg_open_drone_id_arm_status_decode(message, &parsed);
-    return &record;
-}
-
-cStruct* unbox_param_set(const mavlink_message_t* message)
-{
-    static mavlink_param_set_t parsed;
-
-    static cMember members[] = {
-        { "param_value", &(parsed.param_value), 1, FLOAT},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "param_id", &(parsed.param_id), 16, CHAR},
-        { "param_type", &(parsed.param_type), 1, UINT8_T}
-    };
-    static cStruct record = {"param_set", members, 5, 23};
-
-    mavlink_msg_param_set_decode(message, &parsed);
-    return &record;
-}
-
-cStruct* unbox_open_drone_id_authentication(const mavlink_message_t* message)
-{
-    static mavlink_open_drone_id_authentication_t parsed;
-
-    static cMember members[] = {
-        { "timestamp", &(parsed.timestamp), 1, UINT32_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "id_or_mac", &(parsed.id_or_mac), 20, UINT8_T},
-        { "authentication_type", &(parsed.authentication_type), 1, UINT8_T},
-        { "data_page", &(parsed.data_page), 1, UINT8_T},
-        { "last_page_index", &(parsed.last_page_index), 1, UINT8_T},
-        { "length", &(parsed.length), 1, UINT8_T},
-        { "authentication_data", &(parsed.authentication_data), 23, UINT8_T}
-    };
-    static cStruct record = {"open_drone_id_authentication", members, 9, 12902};
-
-    mavlink_msg_open_drone_id_authentication_decode(message, &parsed);
-    return &record;
-}
-
-cStruct* unbox_event(const mavlink_message_t* message)
+cStruct* unbox_radio_status(const mavlink_message_t* message)
 {
-    static mavlink_event_t parsed;
+    static mavlink_radio_status_t parsed;
 
     static cMember members[] = {
-        { "id", &(parsed.id), 1, UINT32_T},
-        { "event_time_boot_ms", &(parsed.event_time_boot_ms), 1, UINT32_T},
-        { "sequence", &(parsed.sequence), 1, UINT16_T},
-        { "destination_component", &(parsed.destination_component), 1, UINT8_T},
-        { "destination_system", &(parsed.destination_system), 1, UINT8_T},
-        { "log_levels", &(parsed.log_levels), 1, UINT8_T},
-        { "arguments", &(parsed.arguments), 40, UINT8_T}
+        { "rxerrors", &(parsed.rxerrors), 1, UINT16_T},
+        { "fixed", &(parsed.fixed), 1, UINT16_T},
+        { "rssi", &(parsed.rssi), 1, UINT8_T},
+        { "remrssi", &(parsed.remrssi), 1, UINT8_T},
+        { "txbuf", &(parsed.txbuf), 1, UINT8_T},
+        { "noise", &(parsed.noise), 1, UINT8_T},
+        { "remnoise", &(parsed.remnoise), 1, UINT8_T}
     };
-    static cStruct record = {"event", members, 7, 410};
+    static cStruct record = {"radio_status", members, 7, 109};
 
-    mavlink_msg_event_decode(message, &parsed);
+    mavlink_msg_radio_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_set_attitude_target(const mavlink_message_t* message)
+cStruct* unbox_gimbal_device_set_attitude(const mavlink_message_t* message)
 {
-    static mavlink_set_attitude_target_t parsed;
+    static mavlink_gimbal_device_set_attitude_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
         { "q", &(parsed.q), 4, FLOAT},
-        { "body_roll_rate", &(parsed.body_roll_rate), 1, FLOAT},
-        { "body_pitch_rate", &(parsed.body_pitch_rate), 1, FLOAT},
-        { "body_yaw_rate", &(parsed.body_yaw_rate), 1, FLOAT},
-        { "thrust", &(parsed.thrust), 1, FLOAT},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "type_mask", &(parsed.type_mask), 1, UINT8_T},
-        { "thrust_body", &(parsed.thrust_body), 3, FLOAT}
-    };
-    static cStruct record = {"set_attitude_target", members, 10, 82};
-
-    mavlink_msg_set_attitude_target_decode(message, &parsed);
-    return &record;
-}
-
-cStruct* unbox_change_operator_control(const mavlink_message_t* message)
-{
-    static mavlink_change_operator_control_t parsed;
-
-    static cMember members[] = {
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "control_request", &(parsed.control_request), 1, UINT8_T},
-        { "version", &(parsed.version), 1, UINT8_T},
-        { "passkey", &(parsed.passkey), 25, CHAR}
-    };
-    static cStruct record = {"change_operator_control", members, 4, 5};
-
-    mavlink_msg_change_operator_control_decode(message, &parsed);
-    return &record;
-}
-
-cStruct* unbox_link_node_status(const mavlink_message_t* message)
-{
-    static mavlink_link_node_status_t parsed;
-
-    static cMember members[] = {
-        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
-        { "tx_rate", &(parsed.tx_rate), 1, UINT32_T},
-        { "rx_rate", &(parsed.rx_rate), 1, UINT32_T},
-        { "messages_sent", &(parsed.messages_sent), 1, UINT32_T},
-        { "messages_received", &(parsed.messages_received), 1, UINT32_T},
-        { "messages_lost", &(parsed.messages_lost), 1, UINT32_T},
-        { "rx_parse_err", &(parsed.rx_parse_err), 1, UINT16_T},
-        { "tx_overflows", &(parsed.tx_overflows), 1, UINT16_T},
-        { "rx_overflows", &(parsed.rx_overflows), 1, UINT16_T},
-        { "tx_buf", &(parsed.tx_buf), 1, UINT8_T},
-        { "rx_buf", &(parsed.rx_buf), 1, UINT8_T}
-    };
-    static cStruct record = {"link_node_status", members, 11, 8};
-
-    mavlink_msg_link_node_status_decode(message, &parsed);
-    return &record;
-}
-
-cStruct* unbox_v2_extension(const mavlink_message_t* message)
-{
-    static mavlink_v2_extension_t parsed;
-
-    static cMember members[] = {
-        { "message_type", &(parsed.message_type), 1, UINT16_T},
-        { "target_network", &(parsed.target_network), 1, UINT8_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "payload", &(parsed.payload), 249, UINT8_T}
-    };
-    static cStruct record = {"v2_extension", members, 5, 248};
-
-    mavlink_msg_v2_extension_decode(message, &parsed);
-    return &record;
-}
-
-cStruct* unbox_camera_information(const mavlink_message_t* message)
-{
-    static mavlink_camera_information_t parsed;
-
-    static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "firmware_version", &(parsed.firmware_version), 1, UINT32_T},
-        { "focal_length", &(parsed.focal_length), 1, FLOAT},
-        { "sensor_size_h", &(parsed.sensor_size_h), 1, FLOAT},
-        { "sensor_size_v", &(parsed.sensor_size_v), 1, FLOAT},
-        { "flags", &(parsed.flags), 1, UINT32_T},
-        { "resolution_h", &(parsed.resolution_h), 1, UINT16_T},
-        { "resolution_v", &(parsed.resolution_v), 1, UINT16_T},
-        { "cam_definition_version", &(parsed.cam_definition_version), 1, UINT16_T},
-        { "vendor_name", &(parsed.vendor_name), 32, UINT8_T},
-        { "model_name", &(parsed.model_name), 32, UINT8_T},
-        { "lens_id", &(parsed.lens_id), 1, UINT8_T},
-        { "cam_definition_uri", &(parsed.cam_definition_uri), 140, CHAR}
+        { "angular_velocity_x", &(parsed.angular_velocity_x), 1, FLOAT},
+        { "angular_velocity_y", &(parsed.angular_velocity_y), 1, FLOAT},
+        { "angular_velocity_z", &(parsed.angular_velocity_z), 1, FLOAT},
+        { "flags", &(parsed.flags), 1, UINT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T}
     };
-    static cStruct record = {"camera_information", members, 13, 259};
+    static cStruct record = {"gimbal_device_set_attitude", members, 7, 284};
 
-    mavlink_msg_camera_information_decode(message, &parsed);
+    mavlink_msg_gimbal_device_set_attitude_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_attitude_quaternion_cov(const mavlink_message_t* message)
+cStruct* unbox_optical_flow(const mavlink_message_t* message)
 {
-    static mavlink_attitude_quaternion_cov_t parsed;
+    static mavlink_optical_flow_t parsed;
 
     static cMember members[] = {
         { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "q", &(parsed.q), 4, FLOAT},
-        { "rollspeed", &(parsed.rollspeed), 1, FLOAT},
-        { "pitchspeed", &(parsed.pitchspeed), 1, FLOAT},
-        { "yawspeed", &(parsed.yawspeed), 1, FLOAT},
-        { "covariance", &(parsed.covariance), 9, FLOAT}
+        { "flow_comp_m_x", &(parsed.flow_comp_m_x), 1, FLOAT},
+        { "flow_comp_m_y", &(parsed.flow_comp_m_y), 1, FLOAT},
+        { "ground_distance", &(parsed.ground_distance), 1, FLOAT},
+        { "flow_x", &(parsed.flow_x), 1, INT16_T},
+        { "flow_y", &(parsed.flow_y), 1, INT16_T},
+        { "sensor_id", &(parsed.sensor_id), 1, UINT8_T},
+        { "quality", &(parsed.quality), 1, UINT8_T},
+        { "flow_rate_x", &(parsed.flow_rate_x), 1, FLOAT},
+        { "flow_rate_y", &(parsed.flow_rate_y), 1, FLOAT}
     };
-    static cStruct record = {"attitude_quaternion_cov", members, 6, 61};
+    static cStruct record = {"optical_flow", members, 10, 100};
 
-    mavlink_msg_attitude_quaternion_cov_decode(message, &parsed);
+    mavlink_msg_optical_flow_decode(message, &parsed);
     return &record;
 }
 
 cStruct* unbox_collision(const mavlink_message_t* message)
 {
     static mavlink_collision_t parsed;
 
@@ -3877,144 +3657,148 @@
     };
     static cStruct record = {"collision", members, 7, 247};
 
     mavlink_msg_collision_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_hil_controls(const mavlink_message_t* message)
+cStruct* unbox_mission_request_int(const mavlink_message_t* message)
 {
-    static mavlink_hil_controls_t parsed;
+    static mavlink_mission_request_int_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "roll_ailerons", &(parsed.roll_ailerons), 1, FLOAT},
-        { "pitch_elevator", &(parsed.pitch_elevator), 1, FLOAT},
-        { "yaw_rudder", &(parsed.yaw_rudder), 1, FLOAT},
-        { "throttle", &(parsed.throttle), 1, FLOAT},
-        { "aux1", &(parsed.aux1), 1, FLOAT},
-        { "aux2", &(parsed.aux2), 1, FLOAT},
-        { "aux3", &(parsed.aux3), 1, FLOAT},
-        { "aux4", &(parsed.aux4), 1, FLOAT},
-        { "mode", &(parsed.mode), 1, UINT8_T},
-        { "nav_mode", &(parsed.nav_mode), 1, UINT8_T}
+        { "seq", &(parsed.seq), 1, UINT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "mission_type", &(parsed.mission_type), 1, UINT8_T}
     };
-    static cStruct record = {"hil_controls", members, 11, 91};
+    static cStruct record = {"mission_request_int", members, 4, 51};
 
-    mavlink_msg_hil_controls_decode(message, &parsed);
+    mavlink_msg_mission_request_int_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_scaled_pressure2(const mavlink_message_t* message)
+cStruct* unbox_open_drone_id_authentication(const mavlink_message_t* message)
 {
-    static mavlink_scaled_pressure2_t parsed;
+    static mavlink_open_drone_id_authentication_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "press_abs", &(parsed.press_abs), 1, FLOAT},
-        { "press_diff", &(parsed.press_diff), 1, FLOAT},
-        { "temperature", &(parsed.temperature), 1, INT16_T},
-        { "temperature_press_diff", &(parsed.temperature_press_diff), 1, INT16_T}
+        { "timestamp", &(parsed.timestamp), 1, UINT32_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "id_or_mac", &(parsed.id_or_mac), 20, UINT8_T},
+        { "authentication_type", &(parsed.authentication_type), 1, UINT8_T},
+        { "data_page", &(parsed.data_page), 1, UINT8_T},
+        { "last_page_index", &(parsed.last_page_index), 1, UINT8_T},
+        { "length", &(parsed.length), 1, UINT8_T},
+        { "authentication_data", &(parsed.authentication_data), 23, UINT8_T}
     };
-    static cStruct record = {"scaled_pressure2", members, 5, 137};
+    static cStruct record = {"open_drone_id_authentication", members, 9, 12902};
 
-    mavlink_msg_scaled_pressure2_decode(message, &parsed);
+    mavlink_msg_open_drone_id_authentication_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_gimbal_device_set_attitude(const mavlink_message_t* message)
+cStruct* unbox_generator_status(const mavlink_message_t* message)
 {
-    static mavlink_gimbal_device_set_attitude_t parsed;
+    static mavlink_generator_status_t parsed;
 
     static cMember members[] = {
-        { "q", &(parsed.q), 4, FLOAT},
-        { "angular_velocity_x", &(parsed.angular_velocity_x), 1, FLOAT},
-        { "angular_velocity_y", &(parsed.angular_velocity_y), 1, FLOAT},
-        { "angular_velocity_z", &(parsed.angular_velocity_z), 1, FLOAT},
-        { "flags", &(parsed.flags), 1, UINT16_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T}
+        { "status", &(parsed.status), 1, UINT64_T},
+        { "battery_current", &(parsed.battery_current), 1, FLOAT},
+        { "load_current", &(parsed.load_current), 1, FLOAT},
+        { "power_generated", &(parsed.power_generated), 1, FLOAT},
+        { "bus_voltage", &(parsed.bus_voltage), 1, FLOAT},
+        { "bat_current_setpoint", &(parsed.bat_current_setpoint), 1, FLOAT},
+        { "runtime", &(parsed.runtime), 1, UINT32_T},
+        { "time_until_maintenance", &(parsed.time_until_maintenance), 1, INT32_T},
+        { "generator_speed", &(parsed.generator_speed), 1, UINT16_T},
+        { "rectifier_temperature", &(parsed.rectifier_temperature), 1, INT16_T},
+        { "generator_temperature", &(parsed.generator_temperature), 1, INT16_T}
     };
-    static cStruct record = {"gimbal_device_set_attitude", members, 7, 284};
+    static cStruct record = {"generator_status", members, 11, 373};
 
-    mavlink_msg_gimbal_device_set_attitude_decode(message, &parsed);
+    mavlink_msg_generator_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_terrain_data(const mavlink_message_t* message)
+cStruct* unbox_camera_capture_status(const mavlink_message_t* message)
 {
-    static mavlink_terrain_data_t parsed;
+    static mavlink_camera_capture_status_t parsed;
 
     static cMember members[] = {
-        { "lat", &(parsed.lat), 1, INT32_T},
-        { "lon", &(parsed.lon), 1, INT32_T},
-        { "grid_spacing", &(parsed.grid_spacing), 1, UINT16_T},
-        { "data", &(parsed.data), 16, INT16_T},
-        { "gridbit", &(parsed.gridbit), 1, UINT8_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "image_interval", &(parsed.image_interval), 1, FLOAT},
+        { "recording_time_ms", &(parsed.recording_time_ms), 1, UINT32_T},
+        { "available_capacity", &(parsed.available_capacity), 1, FLOAT},
+        { "image_status", &(parsed.image_status), 1, UINT8_T},
+        { "video_status", &(parsed.video_status), 1, UINT8_T},
+        { "image_count", &(parsed.image_count), 1, INT32_T}
     };
-    static cStruct record = {"terrain_data", members, 5, 134};
+    static cStruct record = {"camera_capture_status", members, 7, 262};
 
-    mavlink_msg_terrain_data_decode(message, &parsed);
+    mavlink_msg_camera_capture_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_supported_tunes(const mavlink_message_t* message)
+cStruct* unbox_mission_request(const mavlink_message_t* message)
 {
-    static mavlink_supported_tunes_t parsed;
+    static mavlink_mission_request_t parsed;
 
     static cMember members[] = {
-        { "format", &(parsed.format), 1, UINT32_T},
+        { "seq", &(parsed.seq), 1, UINT16_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T}
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "mission_type", &(parsed.mission_type), 1, UINT8_T}
     };
-    static cStruct record = {"supported_tunes", members, 3, 401};
+    static cStruct record = {"mission_request", members, 4, 40};
 
-    mavlink_msg_supported_tunes_decode(message, &parsed);
+    mavlink_msg_mission_request_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_can_filter_modify(const mavlink_message_t* message)
+cStruct* unbox_attitude_quaternion(const mavlink_message_t* message)
 {
-    static mavlink_can_filter_modify_t parsed;
+    static mavlink_attitude_quaternion_t parsed;
 
     static cMember members[] = {
-        { "ids", &(parsed.ids), 16, UINT16_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "bus", &(parsed.bus), 1, UINT8_T},
-        { "operation", &(parsed.operation), 1, UINT8_T},
-        { "num_ids", &(parsed.num_ids), 1, UINT8_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "q1", &(parsed.q1), 1, FLOAT},
+        { "q2", &(parsed.q2), 1, FLOAT},
+        { "q3", &(parsed.q3), 1, FLOAT},
+        { "q4", &(parsed.q4), 1, FLOAT},
+        { "rollspeed", &(parsed.rollspeed), 1, FLOAT},
+        { "pitchspeed", &(parsed.pitchspeed), 1, FLOAT},
+        { "yawspeed", &(parsed.yawspeed), 1, FLOAT},
+        { "repr_offset_q", &(parsed.repr_offset_q), 4, FLOAT}
     };
-    static cStruct record = {"can_filter_modify", members, 6, 388};
+    static cStruct record = {"attitude_quaternion", members, 9, 31};
 
-    mavlink_msg_can_filter_modify_decode(message, &parsed);
+    mavlink_msg_attitude_quaternion_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_distance_sensor(const mavlink_message_t* message)
+cStruct* unbox_obstacle_distance(const mavlink_message_t* message)
 {
-    static mavlink_distance_sensor_t parsed;
+    static mavlink_obstacle_distance_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "distances", &(parsed.distances), 72, UINT16_T},
         { "min_distance", &(parsed.min_distance), 1, UINT16_T},
         { "max_distance", &(parsed.max_distance), 1, UINT16_T},
-        { "current_distance", &(parsed.current_distance), 1, UINT16_T},
-        { "type", &(parsed.type), 1, UINT8_T},
-        { "id", &(parsed.id), 1, UINT8_T},
-        { "orientation", &(parsed.orientation), 1, UINT8_T},
-        { "covariance", &(parsed.covariance), 1, UINT8_T},
-        { "horizontal_fov", &(parsed.horizontal_fov), 1, FLOAT},
-        { "vertical_fov", &(parsed.vertical_fov), 1, FLOAT},
-        { "quaternion", &(parsed.quaternion), 4, FLOAT},
-        { "signal_quality", &(parsed.signal_quality), 1, UINT8_T}
+        { "sensor_type", &(parsed.sensor_type), 1, UINT8_T},
+        { "increment", &(parsed.increment), 1, UINT8_T},
+        { "increment_f", &(parsed.increment_f), 1, FLOAT},
+        { "angle_offset", &(parsed.angle_offset), 1, FLOAT},
+        { "frame", &(parsed.frame), 1, UINT8_T}
     };
-    static cStruct record = {"distance_sensor", members, 12, 132};
+    static cStruct record = {"obstacle_distance", members, 9, 330};
 
-    mavlink_msg_distance_sensor_decode(message, &parsed);
+    mavlink_msg_obstacle_distance_decode(message, &parsed);
     return &record;
 }
 
 cStruct* unbox_hil_state(const mavlink_message_t* message)
 {
     static mavlink_hil_state_t parsed;
 
@@ -4038,280 +3822,298 @@
     };
     static cStruct record = {"hil_state", members, 16, 90};
 
     mavlink_msg_hil_state_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_camera_capture_status(const mavlink_message_t* message)
+cStruct* unbox_gimbal_manager_status(const mavlink_message_t* message)
 {
-    static mavlink_camera_capture_status_t parsed;
+    static mavlink_gimbal_manager_status_t parsed;
 
     static cMember members[] = {
         { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "image_interval", &(parsed.image_interval), 1, FLOAT},
-        { "recording_time_ms", &(parsed.recording_time_ms), 1, UINT32_T},
-        { "available_capacity", &(parsed.available_capacity), 1, FLOAT},
-        { "image_status", &(parsed.image_status), 1, UINT8_T},
-        { "video_status", &(parsed.video_status), 1, UINT8_T},
-        { "image_count", &(parsed.image_count), 1, INT32_T}
+        { "flags", &(parsed.flags), 1, UINT32_T},
+        { "gimbal_device_id", &(parsed.gimbal_device_id), 1, UINT8_T},
+        { "primary_control_sysid", &(parsed.primary_control_sysid), 1, UINT8_T},
+        { "primary_control_compid", &(parsed.primary_control_compid), 1, UINT8_T},
+        { "secondary_control_sysid", &(parsed.secondary_control_sysid), 1, UINT8_T},
+        { "secondary_control_compid", &(parsed.secondary_control_compid), 1, UINT8_T}
     };
-    static cStruct record = {"camera_capture_status", members, 7, 262};
+    static cStruct record = {"gimbal_manager_status", members, 7, 281};
 
-    mavlink_msg_camera_capture_status_decode(message, &parsed);
+    mavlink_msg_gimbal_manager_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_canfd_frame(const mavlink_message_t* message)
+cStruct* unbox_trajectory_representation_waypoints(const mavlink_message_t* message)
 {
-    static mavlink_canfd_frame_t parsed;
+    static mavlink_trajectory_representation_waypoints_t parsed;
 
     static cMember members[] = {
-        { "id", &(parsed.id), 1, UINT32_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "bus", &(parsed.bus), 1, UINT8_T},
-        { "len", &(parsed.len), 1, UINT8_T},
-        { "data", &(parsed.data), 64, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "pos_x", &(parsed.pos_x), 5, FLOAT},
+        { "pos_y", &(parsed.pos_y), 5, FLOAT},
+        { "pos_z", &(parsed.pos_z), 5, FLOAT},
+        { "vel_x", &(parsed.vel_x), 5, FLOAT},
+        { "vel_y", &(parsed.vel_y), 5, FLOAT},
+        { "vel_z", &(parsed.vel_z), 5, FLOAT},
+        { "acc_x", &(parsed.acc_x), 5, FLOAT},
+        { "acc_y", &(parsed.acc_y), 5, FLOAT},
+        { "acc_z", &(parsed.acc_z), 5, FLOAT},
+        { "pos_yaw", &(parsed.pos_yaw), 5, FLOAT},
+        { "vel_yaw", &(parsed.vel_yaw), 5, FLOAT},
+        { "command", &(parsed.command), 5, UINT16_T},
+        { "valid_points", &(parsed.valid_points), 1, UINT8_T}
     };
-    static cStruct record = {"canfd_frame", members, 6, 387};
+    static cStruct record = {"trajectory_representation_waypoints", members, 14, 332};
 
-    mavlink_msg_canfd_frame_decode(message, &parsed);
+    mavlink_msg_trajectory_representation_waypoints_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_flight_information(const mavlink_message_t* message)
+cStruct* unbox_auth_key(const mavlink_message_t* message)
 {
-    static mavlink_flight_information_t parsed;
+    static mavlink_auth_key_t parsed;
 
     static cMember members[] = {
-        { "arming_time_utc", &(parsed.arming_time_utc), 1, UINT64_T},
-        { "takeoff_time_utc", &(parsed.takeoff_time_utc), 1, UINT64_T},
-        { "flight_uuid", &(parsed.flight_uuid), 1, UINT64_T},
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T}
+        { "key", &(parsed.key), 32, CHAR}
     };
-    static cStruct record = {"flight_information", members, 4, 264};
+    static cStruct record = {"auth_key", members, 1, 7};
 
-    mavlink_msg_flight_information_decode(message, &parsed);
+    mavlink_msg_auth_key_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_logging_data_acked(const mavlink_message_t* message)
+cStruct* unbox_terrain_check(const mavlink_message_t* message)
 {
-    static mavlink_logging_data_acked_t parsed;
+    static mavlink_terrain_check_t parsed;
+
+    static cMember members[] = {
+        { "lat", &(parsed.lat), 1, INT32_T},
+        { "lon", &(parsed.lon), 1, INT32_T}
+    };
+    static cStruct record = {"terrain_check", members, 2, 135};
+
+    mavlink_msg_terrain_check_decode(message, &parsed);
+    return &record;
+}
+
+cStruct* unbox_gps_inject_data(const mavlink_message_t* message)
+{
+    static mavlink_gps_inject_data_t parsed;
 
     static cMember members[] = {
-        { "sequence", &(parsed.sequence), 1, UINT16_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "length", &(parsed.length), 1, UINT8_T},
-        { "first_message_offset", &(parsed.first_message_offset), 1, UINT8_T},
-        { "data", &(parsed.data), 249, UINT8_T}
+        { "len", &(parsed.len), 1, UINT8_T},
+        { "data", &(parsed.data), 110, UINT8_T}
     };
-    static cStruct record = {"logging_data_acked", members, 6, 267};
+    static cStruct record = {"gps_inject_data", members, 4, 123};
 
-    mavlink_msg_logging_data_acked_decode(message, &parsed);
+    mavlink_msg_gps_inject_data_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_optical_flow(const mavlink_message_t* message)
+cStruct* unbox_scaled_imu3(const mavlink_message_t* message)
 {
-    static mavlink_optical_flow_t parsed;
+    static mavlink_scaled_imu3_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "flow_comp_m_x", &(parsed.flow_comp_m_x), 1, FLOAT},
-        { "flow_comp_m_y", &(parsed.flow_comp_m_y), 1, FLOAT},
-        { "ground_distance", &(parsed.ground_distance), 1, FLOAT},
-        { "flow_x", &(parsed.flow_x), 1, INT16_T},
-        { "flow_y", &(parsed.flow_y), 1, INT16_T},
-        { "sensor_id", &(parsed.sensor_id), 1, UINT8_T},
-        { "quality", &(parsed.quality), 1, UINT8_T},
-        { "flow_rate_x", &(parsed.flow_rate_x), 1, FLOAT},
-        { "flow_rate_y", &(parsed.flow_rate_y), 1, FLOAT}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "xacc", &(parsed.xacc), 1, INT16_T},
+        { "yacc", &(parsed.yacc), 1, INT16_T},
+        { "zacc", &(parsed.zacc), 1, INT16_T},
+        { "xgyro", &(parsed.xgyro), 1, INT16_T},
+        { "ygyro", &(parsed.ygyro), 1, INT16_T},
+        { "zgyro", &(parsed.zgyro), 1, INT16_T},
+        { "xmag", &(parsed.xmag), 1, INT16_T},
+        { "ymag", &(parsed.ymag), 1, INT16_T},
+        { "zmag", &(parsed.zmag), 1, INT16_T},
+        { "temperature", &(parsed.temperature), 1, INT16_T}
     };
-    static cStruct record = {"optical_flow", members, 10, 100};
+    static cStruct record = {"scaled_imu3", members, 11, 129};
 
-    mavlink_msg_optical_flow_decode(message, &parsed);
+    mavlink_msg_scaled_imu3_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_command_cancel(const mavlink_message_t* message)
+cStruct* unbox_battery_status(const mavlink_message_t* message)
 {
-    static mavlink_command_cancel_t parsed;
+    static mavlink_battery_status_t parsed;
 
     static cMember members[] = {
-        { "command", &(parsed.command), 1, UINT16_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T}
+        { "current_consumed", &(parsed.current_consumed), 1, INT32_T},
+        { "energy_consumed", &(parsed.energy_consumed), 1, INT32_T},
+        { "temperature", &(parsed.temperature), 1, INT16_T},
+        { "voltages", &(parsed.voltages), 10, UINT16_T},
+        { "current_battery", &(parsed.current_battery), 1, INT16_T},
+        { "id", &(parsed.id), 1, UINT8_T},
+        { "battery_function", &(parsed.battery_function), 1, UINT8_T},
+        { "type", &(parsed.type), 1, UINT8_T},
+        { "battery_remaining", &(parsed.battery_remaining), 1, INT8_T},
+        { "time_remaining", &(parsed.time_remaining), 1, INT32_T},
+        { "charge_state", &(parsed.charge_state), 1, UINT8_T},
+        { "voltages_ext", &(parsed.voltages_ext), 4, UINT16_T},
+        { "mode", &(parsed.mode), 1, UINT8_T},
+        { "fault_bitmask", &(parsed.fault_bitmask), 1, UINT32_T}
     };
-    static cStruct record = {"command_cancel", members, 3, 80};
+    static cStruct record = {"battery_status", members, 14, 147};
 
-    mavlink_msg_command_cancel_decode(message, &parsed);
+    mavlink_msg_battery_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_camera_image_captured(const mavlink_message_t* message)
+cStruct* unbox_open_drone_id_basic_id(const mavlink_message_t* message)
 {
-    static mavlink_camera_image_captured_t parsed;
+    static mavlink_open_drone_id_basic_id_t parsed;
 
     static cMember members[] = {
-        { "time_utc", &(parsed.time_utc), 1, UINT64_T},
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "lat", &(parsed.lat), 1, INT32_T},
-        { "lon", &(parsed.lon), 1, INT32_T},
-        { "alt", &(parsed.alt), 1, INT32_T},
-        { "relative_alt", &(parsed.relative_alt), 1, INT32_T},
-        { "q", &(parsed.q), 4, FLOAT},
-        { "image_index", &(parsed.image_index), 1, INT32_T},
-        { "camera_id", &(parsed.camera_id), 1, UINT8_T},
-        { "capture_result", &(parsed.capture_result), 1, INT8_T},
-        { "file_url", &(parsed.file_url), 205, CHAR}
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "id_or_mac", &(parsed.id_or_mac), 20, UINT8_T},
+        { "id_type", &(parsed.id_type), 1, UINT8_T},
+        { "ua_type", &(parsed.ua_type), 1, UINT8_T},
+        { "uas_id", &(parsed.uas_id), 20, UINT8_T}
     };
-    static cStruct record = {"camera_image_captured", members, 11, 263};
+    static cStruct record = {"open_drone_id_basic_id", members, 6, 12900};
 
-    mavlink_msg_camera_image_captured_decode(message, &parsed);
+    mavlink_msg_open_drone_id_basic_id_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_set_position_target_global_int(const mavlink_message_t* message)
+cStruct* unbox_param_map_rc(const mavlink_message_t* message)
 {
-    static mavlink_set_position_target_global_int_t parsed;
+    static mavlink_param_map_rc_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "lat_int", &(parsed.lat_int), 1, INT32_T},
-        { "lon_int", &(parsed.lon_int), 1, INT32_T},
-        { "alt", &(parsed.alt), 1, FLOAT},
-        { "vx", &(parsed.vx), 1, FLOAT},
-        { "vy", &(parsed.vy), 1, FLOAT},
-        { "vz", &(parsed.vz), 1, FLOAT},
-        { "afx", &(parsed.afx), 1, FLOAT},
-        { "afy", &(parsed.afy), 1, FLOAT},
-        { "afz", &(parsed.afz), 1, FLOAT},
-        { "yaw", &(parsed.yaw), 1, FLOAT},
-        { "yaw_rate", &(parsed.yaw_rate), 1, FLOAT},
-        { "type_mask", &(parsed.type_mask), 1, UINT16_T},
+        { "param_value0", &(parsed.param_value0), 1, FLOAT},
+        { "scale", &(parsed.scale), 1, FLOAT},
+        { "param_value_min", &(parsed.param_value_min), 1, FLOAT},
+        { "param_value_max", &(parsed.param_value_max), 1, FLOAT},
+        { "param_index", &(parsed.param_index), 1, INT16_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "coordinate_frame", &(parsed.coordinate_frame), 1, UINT8_T}
+        { "param_id", &(parsed.param_id), 16, CHAR},
+        { "parameter_rc_channel_index", &(parsed.parameter_rc_channel_index), 1, UINT8_T}
     };
-    static cStruct record = {"set_position_target_global_int", members, 16, 86};
+    static cStruct record = {"param_map_rc", members, 9, 50};
 
-    mavlink_msg_set_position_target_global_int_decode(message, &parsed);
+    mavlink_msg_param_map_rc_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_set_gps_global_origin(const mavlink_message_t* message)
+cStruct* unbox_hil_controls(const mavlink_message_t* message)
 {
-    static mavlink_set_gps_global_origin_t parsed;
+    static mavlink_hil_controls_t parsed;
 
     static cMember members[] = {
-        { "latitude", &(parsed.latitude), 1, INT32_T},
-        { "longitude", &(parsed.longitude), 1, INT32_T},
-        { "altitude", &(parsed.altitude), 1, INT32_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "roll_ailerons", &(parsed.roll_ailerons), 1, FLOAT},
+        { "pitch_elevator", &(parsed.pitch_elevator), 1, FLOAT},
+        { "yaw_rudder", &(parsed.yaw_rudder), 1, FLOAT},
+        { "throttle", &(parsed.throttle), 1, FLOAT},
+        { "aux1", &(parsed.aux1), 1, FLOAT},
+        { "aux2", &(parsed.aux2), 1, FLOAT},
+        { "aux3", &(parsed.aux3), 1, FLOAT},
+        { "aux4", &(parsed.aux4), 1, FLOAT},
+        { "mode", &(parsed.mode), 1, UINT8_T},
+        { "nav_mode", &(parsed.nav_mode), 1, UINT8_T}
     };
-    static cStruct record = {"set_gps_global_origin", members, 5, 48};
+    static cStruct record = {"hil_controls", members, 11, 91};
 
-    mavlink_msg_set_gps_global_origin_decode(message, &parsed);
+    mavlink_msg_hil_controls_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_statustext(const mavlink_message_t* message)
+cStruct* unbox_gps_input(const mavlink_message_t* message)
 {
-    static mavlink_statustext_t parsed;
+    static mavlink_gps_input_t parsed;
 
     static cMember members[] = {
-        { "severity", &(parsed.severity), 1, UINT8_T},
-        { "text", &(parsed.text), 50, CHAR},
-        { "id", &(parsed.id), 1, UINT16_T},
-        { "chunk_seq", &(parsed.chunk_seq), 1, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "time_week_ms", &(parsed.time_week_ms), 1, UINT32_T},
+        { "lat", &(parsed.lat), 1, INT32_T},
+        { "lon", &(parsed.lon), 1, INT32_T},
+        { "alt", &(parsed.alt), 1, FLOAT},
+        { "hdop", &(parsed.hdop), 1, FLOAT},
+        { "vdop", &(parsed.vdop), 1, FLOAT},
+        { "vn", &(parsed.vn), 1, FLOAT},
+        { "ve", &(parsed.ve), 1, FLOAT},
+        { "vd", &(parsed.vd), 1, FLOAT},
+        { "speed_accuracy", &(parsed.speed_accuracy), 1, FLOAT},
+        { "horiz_accuracy", &(parsed.horiz_accuracy), 1, FLOAT},
+        { "vert_accuracy", &(parsed.vert_accuracy), 1, FLOAT},
+        { "ignore_flags", &(parsed.ignore_flags), 1, UINT16_T},
+        { "time_week", &(parsed.time_week), 1, UINT16_T},
+        { "gps_id", &(parsed.gps_id), 1, UINT8_T},
+        { "fix_type", &(parsed.fix_type), 1, UINT8_T},
+        { "satellites_visible", &(parsed.satellites_visible), 1, UINT8_T},
+        { "yaw", &(parsed.yaw), 1, UINT16_T}
     };
-    static cStruct record = {"statustext", members, 4, 253};
+    static cStruct record = {"gps_input", members, 19, 232};
 
-    mavlink_msg_statustext_decode(message, &parsed);
+    mavlink_msg_gps_input_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_param_request_read(const mavlink_message_t* message)
+cStruct* unbox_gps2_rtk(const mavlink_message_t* message)
 {
-    static mavlink_param_request_read_t parsed;
+    static mavlink_gps2_rtk_t parsed;
 
     static cMember members[] = {
-        { "param_index", &(parsed.param_index), 1, INT16_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "param_id", &(parsed.param_id), 16, CHAR}
+        { "time_last_baseline_ms", &(parsed.time_last_baseline_ms), 1, UINT32_T},
+        { "tow", &(parsed.tow), 1, UINT32_T},
+        { "baseline_a_mm", &(parsed.baseline_a_mm), 1, INT32_T},
+        { "baseline_b_mm", &(parsed.baseline_b_mm), 1, INT32_T},
+        { "baseline_c_mm", &(parsed.baseline_c_mm), 1, INT32_T},
+        { "accuracy", &(parsed.accuracy), 1, UINT32_T},
+        { "iar_num_hypotheses", &(parsed.iar_num_hypotheses), 1, INT32_T},
+        { "wn", &(parsed.wn), 1, UINT16_T},
+        { "rtk_receiver_id", &(parsed.rtk_receiver_id), 1, UINT8_T},
+        { "rtk_health", &(parsed.rtk_health), 1, UINT8_T},
+        { "rtk_rate", &(parsed.rtk_rate), 1, UINT8_T},
+        { "nsats", &(parsed.nsats), 1, UINT8_T},
+        { "baseline_coords_type", &(parsed.baseline_coords_type), 1, UINT8_T}
     };
-    static cStruct record = {"param_request_read", members, 4, 20};
+    static cStruct record = {"gps2_rtk", members, 13, 128};
 
-    mavlink_msg_param_request_read_decode(message, &parsed);
+    mavlink_msg_gps2_rtk_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_adsb_vehicle(const mavlink_message_t* message)
+cStruct* unbox_set_actuator_control_target(const mavlink_message_t* message)
 {
-    static mavlink_adsb_vehicle_t parsed;
+    static mavlink_set_actuator_control_target_t parsed;
 
     static cMember members[] = {
-        { "ICAO_address", &(parsed.ICAO_address), 1, UINT32_T},
-        { "lat", &(parsed.lat), 1, INT32_T},
-        { "lon", &(parsed.lon), 1, INT32_T},
-        { "altitude", &(parsed.altitude), 1, INT32_T},
-        { "heading", &(parsed.heading), 1, UINT16_T},
-        { "hor_velocity", &(parsed.hor_velocity), 1, UINT16_T},
-        { "ver_velocity", &(parsed.ver_velocity), 1, INT16_T},
-        { "flags", &(parsed.flags), 1, UINT16_T},
-        { "squawk", &(parsed.squawk), 1, UINT16_T},
-        { "altitude_type", &(parsed.altitude_type), 1, UINT8_T},
-        { "callsign", &(parsed.callsign), 9, CHAR},
-        { "emitter_type", &(parsed.emitter_type), 1, UINT8_T},
-        { "tslc", &(parsed.tslc), 1, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "controls", &(parsed.controls), 8, FLOAT},
+        { "group_mlx", &(parsed.group_mlx), 1, UINT8_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T}
     };
-    static cStruct record = {"adsb_vehicle", members, 13, 246};
+    static cStruct record = {"set_actuator_control_target", members, 5, 139};
 
-    mavlink_msg_adsb_vehicle_decode(message, &parsed);
+    mavlink_msg_set_actuator_control_target_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_high_latency(const mavlink_message_t* message)
+cStruct* unbox_named_value_float(const mavlink_message_t* message)
 {
-    static mavlink_high_latency_t parsed;
+    static mavlink_named_value_float_t parsed;
 
     static cMember members[] = {
-        { "custom_mode", &(parsed.custom_mode), 1, UINT32_T},
-        { "latitude", &(parsed.latitude), 1, INT32_T},
-        { "longitude", &(parsed.longitude), 1, INT32_T},
-        { "roll", &(parsed.roll), 1, INT16_T},
-        { "pitch", &(parsed.pitch), 1, INT16_T},
-        { "heading", &(parsed.heading), 1, UINT16_T},
-        { "heading_sp", &(parsed.heading_sp), 1, INT16_T},
-        { "altitude_amsl", &(parsed.altitude_amsl), 1, INT16_T},
-        { "altitude_sp", &(parsed.altitude_sp), 1, INT16_T},
-        { "wp_distance", &(parsed.wp_distance), 1, UINT16_T},
-        { "base_mode", &(parsed.base_mode), 1, UINT8_T},
-        { "landed_state", &(parsed.landed_state), 1, UINT8_T},
-        { "throttle", &(parsed.throttle), 1, INT8_T},
-        { "airspeed", &(parsed.airspeed), 1, UINT8_T},
-        { "airspeed_sp", &(parsed.airspeed_sp), 1, UINT8_T},
-        { "groundspeed", &(parsed.groundspeed), 1, UINT8_T},
-        { "climb_rate", &(parsed.climb_rate), 1, INT8_T},
-        { "gps_nsat", &(parsed.gps_nsat), 1, UINT8_T},
-        { "gps_fix_type", &(parsed.gps_fix_type), 1, UINT8_T},
-        { "battery_remaining", &(parsed.battery_remaining), 1, UINT8_T},
-        { "temperature", &(parsed.temperature), 1, INT8_T},
-        { "temperature_air", &(parsed.temperature_air), 1, INT8_T},
-        { "failsafe", &(parsed.failsafe), 1, UINT8_T},
-        { "wp_num", &(parsed.wp_num), 1, UINT8_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "value", &(parsed.value), 1, FLOAT},
+        { "name", &(parsed.name), 10, CHAR}
     };
-    static cStruct record = {"high_latency", members, 24, 234};
+    static cStruct record = {"named_value_float", members, 3, 251};
 
-    mavlink_msg_high_latency_decode(message, &parsed);
+    mavlink_msg_named_value_float_decode(message, &parsed);
     return &record;
 }
 
 cStruct* unbox_wheel_distance(const mavlink_message_t* message)
 {
     static mavlink_wheel_distance_t parsed;
 
@@ -4322,142 +4124,235 @@
     };
     static cStruct record = {"wheel_distance", members, 3, 9000};
 
     mavlink_msg_wheel_distance_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_extended_sys_state(const mavlink_message_t* message)
+cStruct* unbox_onboard_computer_status(const mavlink_message_t* message)
 {
-    static mavlink_extended_sys_state_t parsed;
+    static mavlink_onboard_computer_status_t parsed;
 
     static cMember members[] = {
-        { "vtol_state", &(parsed.vtol_state), 1, UINT8_T},
-        { "landed_state", &(parsed.landed_state), 1, UINT8_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "uptime", &(parsed.uptime), 1, UINT32_T},
+        { "ram_usage", &(parsed.ram_usage), 1, UINT32_T},
+        { "ram_total", &(parsed.ram_total), 1, UINT32_T},
+        { "storage_type", &(parsed.storage_type), 4, UINT32_T},
+        { "storage_usage", &(parsed.storage_usage), 4, UINT32_T},
+        { "storage_total", &(parsed.storage_total), 4, UINT32_T},
+        { "link_type", &(parsed.link_type), 6, UINT32_T},
+        { "link_tx_rate", &(parsed.link_tx_rate), 6, UINT32_T},
+        { "link_rx_rate", &(parsed.link_rx_rate), 6, UINT32_T},
+        { "link_tx_max", &(parsed.link_tx_max), 6, UINT32_T},
+        { "link_rx_max", &(parsed.link_rx_max), 6, UINT32_T},
+        { "fan_speed", &(parsed.fan_speed), 4, INT16_T},
+        { "type", &(parsed.type), 1, UINT8_T},
+        { "cpu_cores", &(parsed.cpu_cores), 8, UINT8_T},
+        { "cpu_combined", &(parsed.cpu_combined), 10, UINT8_T},
+        { "gpu_cores", &(parsed.gpu_cores), 4, UINT8_T},
+        { "gpu_combined", &(parsed.gpu_combined), 10, UINT8_T},
+        { "temperature_board", &(parsed.temperature_board), 1, INT8_T},
+        { "temperature_core", &(parsed.temperature_core), 8, INT8_T}
     };
-    static cStruct record = {"extended_sys_state", members, 2, 245};
+    static cStruct record = {"onboard_computer_status", members, 20, 390};
 
-    mavlink_msg_extended_sys_state_decode(message, &parsed);
+    mavlink_msg_onboard_computer_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_vibration(const mavlink_message_t* message)
+cStruct* unbox_rc_channels_raw(const mavlink_message_t* message)
 {
-    static mavlink_vibration_t parsed;
+    static mavlink_rc_channels_raw_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "vibration_x", &(parsed.vibration_x), 1, FLOAT},
-        { "vibration_y", &(parsed.vibration_y), 1, FLOAT},
-        { "vibration_z", &(parsed.vibration_z), 1, FLOAT},
-        { "clipping_0", &(parsed.clipping_0), 1, UINT32_T},
-        { "clipping_1", &(parsed.clipping_1), 1, UINT32_T},
-        { "clipping_2", &(parsed.clipping_2), 1, UINT32_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "chan1_raw", &(parsed.chan1_raw), 1, UINT16_T},
+        { "chan2_raw", &(parsed.chan2_raw), 1, UINT16_T},
+        { "chan3_raw", &(parsed.chan3_raw), 1, UINT16_T},
+        { "chan4_raw", &(parsed.chan4_raw), 1, UINT16_T},
+        { "chan5_raw", &(parsed.chan5_raw), 1, UINT16_T},
+        { "chan6_raw", &(parsed.chan6_raw), 1, UINT16_T},
+        { "chan7_raw", &(parsed.chan7_raw), 1, UINT16_T},
+        { "chan8_raw", &(parsed.chan8_raw), 1, UINT16_T},
+        { "port", &(parsed.port), 1, UINT8_T},
+        { "rssi", &(parsed.rssi), 1, UINT8_T}
     };
-    static cStruct record = {"vibration", members, 7, 241};
+    static cStruct record = {"rc_channels_raw", members, 11, 35};
 
-    mavlink_msg_vibration_decode(message, &parsed);
+    mavlink_msg_rc_channels_raw_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_obstacle_distance(const mavlink_message_t* message)
+cStruct* unbox_mission_item_int(const mavlink_message_t* message)
 {
-    static mavlink_obstacle_distance_t parsed;
+    static mavlink_mission_item_int_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "distances", &(parsed.distances), 72, UINT16_T},
-        { "min_distance", &(parsed.min_distance), 1, UINT16_T},
-        { "max_distance", &(parsed.max_distance), 1, UINT16_T},
-        { "sensor_type", &(parsed.sensor_type), 1, UINT8_T},
-        { "increment", &(parsed.increment), 1, UINT8_T},
-        { "increment_f", &(parsed.increment_f), 1, FLOAT},
-        { "angle_offset", &(parsed.angle_offset), 1, FLOAT},
-        { "frame", &(parsed.frame), 1, UINT8_T}
+        { "param1", &(parsed.param1), 1, FLOAT},
+        { "param2", &(parsed.param2), 1, FLOAT},
+        { "param3", &(parsed.param3), 1, FLOAT},
+        { "param4", &(parsed.param4), 1, FLOAT},
+        { "x", &(parsed.x), 1, INT32_T},
+        { "y", &(parsed.y), 1, INT32_T},
+        { "z", &(parsed.z), 1, FLOAT},
+        { "seq", &(parsed.seq), 1, UINT16_T},
+        { "command", &(parsed.command), 1, UINT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "frame", &(parsed.frame), 1, UINT8_T},
+        { "current", &(parsed.current), 1, UINT8_T},
+        { "autocontinue", &(parsed.autocontinue), 1, UINT8_T},
+        { "mission_type", &(parsed.mission_type), 1, UINT8_T}
     };
-    static cStruct record = {"obstacle_distance", members, 9, 330};
+    static cStruct record = {"mission_item_int", members, 15, 73};
 
-    mavlink_msg_obstacle_distance_decode(message, &parsed);
+    mavlink_msg_mission_item_int_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_log_entry(const mavlink_message_t* message)
+cStruct* unbox_log_request_list(const mavlink_message_t* message)
 {
-    static mavlink_log_entry_t parsed;
+    static mavlink_log_request_list_t parsed;
 
     static cMember members[] = {
-        { "time_utc", &(parsed.time_utc), 1, UINT32_T},
-        { "size", &(parsed.size), 1, UINT32_T},
-        { "id", &(parsed.id), 1, UINT16_T},
-        { "num_logs", &(parsed.num_logs), 1, UINT16_T},
-        { "last_log_num", &(parsed.last_log_num), 1, UINT16_T}
+        { "start", &(parsed.start), 1, UINT16_T},
+        { "end", &(parsed.end), 1, UINT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T}
     };
-    static cStruct record = {"log_entry", members, 5, 118};
+    static cStruct record = {"log_request_list", members, 4, 117};
 
-    mavlink_msg_log_entry_decode(message, &parsed);
+    mavlink_msg_log_request_list_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_request_data_stream(const mavlink_message_t* message)
+cStruct* unbox_safety_allowed_area(const mavlink_message_t* message)
 {
-    static mavlink_request_data_stream_t parsed;
+    static mavlink_safety_allowed_area_t parsed;
 
     static cMember members[] = {
-        { "req_message_rate", &(parsed.req_message_rate), 1, UINT16_T},
+        { "p1x", &(parsed.p1x), 1, FLOAT},
+        { "p1y", &(parsed.p1y), 1, FLOAT},
+        { "p1z", &(parsed.p1z), 1, FLOAT},
+        { "p2x", &(parsed.p2x), 1, FLOAT},
+        { "p2y", &(parsed.p2y), 1, FLOAT},
+        { "p2z", &(parsed.p2z), 1, FLOAT},
+        { "frame", &(parsed.frame), 1, UINT8_T}
+    };
+    static cStruct record = {"safety_allowed_area", members, 7, 55};
+
+    mavlink_msg_safety_allowed_area_decode(message, &parsed);
+    return &record;
+}
+
+cStruct* unbox_tunnel(const mavlink_message_t* message)
+{
+    static mavlink_tunnel_t parsed;
+
+    static cMember members[] = {
+        { "payload_type", &(parsed.payload_type), 1, UINT16_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "req_stream_id", &(parsed.req_stream_id), 1, UINT8_T},
-        { "start_stop", &(parsed.start_stop), 1, UINT8_T}
+        { "payload_length", &(parsed.payload_length), 1, UINT8_T},
+        { "payload", &(parsed.payload), 128, UINT8_T}
     };
-    static cStruct record = {"request_data_stream", members, 5, 66};
+    static cStruct record = {"tunnel", members, 5, 385};
 
-    mavlink_msg_request_data_stream_decode(message, &parsed);
+    mavlink_msg_tunnel_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_autopilot_state_for_gimbal_device(const mavlink_message_t* message)
+cStruct* unbox_global_position_int_cov(const mavlink_message_t* message)
 {
-    static mavlink_autopilot_state_for_gimbal_device_t parsed;
+    static mavlink_global_position_int_cov_t parsed;
 
     static cMember members[] = {
-        { "time_boot_us", &(parsed.time_boot_us), 1, UINT64_T},
-        { "q", &(parsed.q), 4, FLOAT},
-        { "q_estimated_delay_us", &(parsed.q_estimated_delay_us), 1, UINT32_T},
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "lat", &(parsed.lat), 1, INT32_T},
+        { "lon", &(parsed.lon), 1, INT32_T},
+        { "alt", &(parsed.alt), 1, INT32_T},
+        { "relative_alt", &(parsed.relative_alt), 1, INT32_T},
         { "vx", &(parsed.vx), 1, FLOAT},
         { "vy", &(parsed.vy), 1, FLOAT},
         { "vz", &(parsed.vz), 1, FLOAT},
-        { "v_estimated_delay_us", &(parsed.v_estimated_delay_us), 1, UINT32_T},
-        { "feed_forward_angular_velocity_z", &(parsed.feed_forward_angular_velocity_z), 1, FLOAT},
-        { "estimator_status", &(parsed.estimator_status), 1, UINT16_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "landed_state", &(parsed.landed_state), 1, UINT8_T},
-        { "angular_velocity_z", &(parsed.angular_velocity_z), 1, FLOAT}
+        { "covariance", &(parsed.covariance), 36, FLOAT},
+        { "estimator_type", &(parsed.estimator_type), 1, UINT8_T}
     };
-    static cStruct record = {"autopilot_state_for_gimbal_device", members, 13, 286};
+    static cStruct record = {"global_position_int_cov", members, 10, 63};
 
-    mavlink_msg_autopilot_state_for_gimbal_device_decode(message, &parsed);
+    mavlink_msg_global_position_int_cov_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_open_drone_id_basic_id(const mavlink_message_t* message)
+cStruct* unbox_camera_information(const mavlink_message_t* message)
 {
-    static mavlink_open_drone_id_basic_id_t parsed;
+    static mavlink_camera_information_t parsed;
 
     static cMember members[] = {
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "id_or_mac", &(parsed.id_or_mac), 20, UINT8_T},
-        { "id_type", &(parsed.id_type), 1, UINT8_T},
-        { "ua_type", &(parsed.ua_type), 1, UINT8_T},
-        { "uas_id", &(parsed.uas_id), 20, UINT8_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "firmware_version", &(parsed.firmware_version), 1, UINT32_T},
+        { "focal_length", &(parsed.focal_length), 1, FLOAT},
+        { "sensor_size_h", &(parsed.sensor_size_h), 1, FLOAT},
+        { "sensor_size_v", &(parsed.sensor_size_v), 1, FLOAT},
+        { "flags", &(parsed.flags), 1, UINT32_T},
+        { "resolution_h", &(parsed.resolution_h), 1, UINT16_T},
+        { "resolution_v", &(parsed.resolution_v), 1, UINT16_T},
+        { "cam_definition_version", &(parsed.cam_definition_version), 1, UINT16_T},
+        { "vendor_name", &(parsed.vendor_name), 32, UINT8_T},
+        { "model_name", &(parsed.model_name), 32, UINT8_T},
+        { "lens_id", &(parsed.lens_id), 1, UINT8_T},
+        { "cam_definition_uri", &(parsed.cam_definition_uri), 140, CHAR}
     };
-    static cStruct record = {"open_drone_id_basic_id", members, 6, 12900};
+    static cStruct record = {"camera_information", members, 13, 259};
 
-    mavlink_msg_open_drone_id_basic_id_decode(message, &parsed);
+    mavlink_msg_camera_information_decode(message, &parsed);
+    return &record;
+}
+
+cStruct* unbox_gimbal_device_information(const mavlink_message_t* message)
+{
+    static mavlink_gimbal_device_information_t parsed;
+
+    static cMember members[] = {
+        { "uid", &(parsed.uid), 1, UINT64_T},
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "firmware_version", &(parsed.firmware_version), 1, UINT32_T},
+        { "hardware_version", &(parsed.hardware_version), 1, UINT32_T},
+        { "roll_min", &(parsed.roll_min), 1, FLOAT},
+        { "roll_max", &(parsed.roll_max), 1, FLOAT},
+        { "pitch_min", &(parsed.pitch_min), 1, FLOAT},
+        { "pitch_max", &(parsed.pitch_max), 1, FLOAT},
+        { "yaw_min", &(parsed.yaw_min), 1, FLOAT},
+        { "yaw_max", &(parsed.yaw_max), 1, FLOAT},
+        { "cap_flags", &(parsed.cap_flags), 1, UINT16_T},
+        { "custom_cap_flags", &(parsed.custom_cap_flags), 1, UINT16_T},
+        { "vendor_name", &(parsed.vendor_name), 32, CHAR},
+        { "model_name", &(parsed.model_name), 32, CHAR},
+        { "custom_name", &(parsed.custom_name), 32, CHAR}
+    };
+    static cStruct record = {"gimbal_device_information", members, 15, 283};
+
+    mavlink_msg_gimbal_device_information_decode(message, &parsed);
+    return &record;
+}
+
+cStruct* unbox_terrain_request(const mavlink_message_t* message)
+{
+    static mavlink_terrain_request_t parsed;
+
+    static cMember members[] = {
+        { "mask", &(parsed.mask), 1, UINT64_T},
+        { "lat", &(parsed.lat), 1, INT32_T},
+        { "lon", &(parsed.lon), 1, INT32_T},
+        { "grid_spacing", &(parsed.grid_spacing), 1, UINT16_T}
+    };
+    static cStruct record = {"terrain_request", members, 4, 133};
+
+    mavlink_msg_terrain_request_decode(message, &parsed);
     return &record;
 }
 
 cStruct* unbox_command_long(const mavlink_message_t* message)
 {
     static mavlink_command_long_t parsed;
 
@@ -4476,26 +4371,178 @@
     };
     static cStruct record = {"command_long", members, 11, 76};
 
     mavlink_msg_command_long_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_named_value_int(const mavlink_message_t* message)
+cStruct* unbox_camera_tracking_image_status(const mavlink_message_t* message)
 {
-    static mavlink_named_value_int_t parsed;
+    static mavlink_camera_tracking_image_status_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "value", &(parsed.value), 1, INT32_T},
-        { "name", &(parsed.name), 10, CHAR}
+        { "point_x", &(parsed.point_x), 1, FLOAT},
+        { "point_y", &(parsed.point_y), 1, FLOAT},
+        { "radius", &(parsed.radius), 1, FLOAT},
+        { "rec_top_x", &(parsed.rec_top_x), 1, FLOAT},
+        { "rec_top_y", &(parsed.rec_top_y), 1, FLOAT},
+        { "rec_bottom_x", &(parsed.rec_bottom_x), 1, FLOAT},
+        { "rec_bottom_y", &(parsed.rec_bottom_y), 1, FLOAT},
+        { "tracking_status", &(parsed.tracking_status), 1, UINT8_T},
+        { "tracking_mode", &(parsed.tracking_mode), 1, UINT8_T},
+        { "target_data", &(parsed.target_data), 1, UINT8_T}
     };
-    static cStruct record = {"named_value_int", members, 3, 252};
+    static cStruct record = {"camera_tracking_image_status", members, 10, 275};
 
-    mavlink_msg_named_value_int_decode(message, &parsed);
+    mavlink_msg_camera_tracking_image_status_decode(message, &parsed);
+    return &record;
+}
+
+cStruct* unbox_vfr_hud(const mavlink_message_t* message)
+{
+    static mavlink_vfr_hud_t parsed;
+
+    static cMember members[] = {
+        { "airspeed", &(parsed.airspeed), 1, FLOAT},
+        { "groundspeed", &(parsed.groundspeed), 1, FLOAT},
+        { "alt", &(parsed.alt), 1, FLOAT},
+        { "climb", &(parsed.climb), 1, FLOAT},
+        { "heading", &(parsed.heading), 1, INT16_T},
+        { "throttle", &(parsed.throttle), 1, UINT16_T}
+    };
+    static cStruct record = {"vfr_hud", members, 6, 74};
+
+    mavlink_msg_vfr_hud_decode(message, &parsed);
+    return &record;
+}
+
+cStruct* unbox_log_data(const mavlink_message_t* message)
+{
+    static mavlink_log_data_t parsed;
+
+    static cMember members[] = {
+        { "ofs", &(parsed.ofs), 1, UINT32_T},
+        { "id", &(parsed.id), 1, UINT16_T},
+        { "count", &(parsed.count), 1, UINT8_T},
+        { "data", &(parsed.data), 90, UINT8_T}
+    };
+    static cStruct record = {"log_data", members, 4, 120};
+
+    mavlink_msg_log_data_decode(message, &parsed);
+    return &record;
+}
+
+cStruct* unbox_can_filter_modify(const mavlink_message_t* message)
+{
+    static mavlink_can_filter_modify_t parsed;
+
+    static cMember members[] = {
+        { "ids", &(parsed.ids), 16, UINT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "bus", &(parsed.bus), 1, UINT8_T},
+        { "operation", &(parsed.operation), 1, UINT8_T},
+        { "num_ids", &(parsed.num_ids), 1, UINT8_T}
+    };
+    static cStruct record = {"can_filter_modify", members, 6, 388};
+
+    mavlink_msg_can_filter_modify_decode(message, &parsed);
+    return &record;
+}
+
+cStruct* unbox_vicon_position_estimate(const mavlink_message_t* message)
+{
+    static mavlink_vicon_position_estimate_t parsed;
+
+    static cMember members[] = {
+        { "usec", &(parsed.usec), 1, UINT64_T},
+        { "x", &(parsed.x), 1, FLOAT},
+        { "y", &(parsed.y), 1, FLOAT},
+        { "z", &(parsed.z), 1, FLOAT},
+        { "roll", &(parsed.roll), 1, FLOAT},
+        { "pitch", &(parsed.pitch), 1, FLOAT},
+        { "yaw", &(parsed.yaw), 1, FLOAT},
+        { "covariance", &(parsed.covariance), 21, FLOAT}
+    };
+    static cStruct record = {"vicon_position_estimate", members, 8, 104};
+
+    mavlink_msg_vicon_position_estimate_decode(message, &parsed);
+    return &record;
+}
+
+cStruct* unbox_mission_request_partial_list(const mavlink_message_t* message)
+{
+    static mavlink_mission_request_partial_list_t parsed;
+
+    static cMember members[] = {
+        { "start_index", &(parsed.start_index), 1, INT16_T},
+        { "end_index", &(parsed.end_index), 1, INT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "mission_type", &(parsed.mission_type), 1, UINT8_T}
+    };
+    static cStruct record = {"mission_request_partial_list", members, 5, 37};
+
+    mavlink_msg_mission_request_partial_list_decode(message, &parsed);
+    return &record;
+}
+
+cStruct* unbox_logging_data(const mavlink_message_t* message)
+{
+    static mavlink_logging_data_t parsed;
+
+    static cMember members[] = {
+        { "sequence", &(parsed.sequence), 1, UINT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "length", &(parsed.length), 1, UINT8_T},
+        { "first_message_offset", &(parsed.first_message_offset), 1, UINT8_T},
+        { "data", &(parsed.data), 249, UINT8_T}
+    };
+    static cStruct record = {"logging_data", members, 6, 266};
+
+    mavlink_msg_logging_data_decode(message, &parsed);
+    return &record;
+}
+
+cStruct* unbox_raw_imu(const mavlink_message_t* message)
+{
+    static mavlink_raw_imu_t parsed;
+
+    static cMember members[] = {
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "xacc", &(parsed.xacc), 1, INT16_T},
+        { "yacc", &(parsed.yacc), 1, INT16_T},
+        { "zacc", &(parsed.zacc), 1, INT16_T},
+        { "xgyro", &(parsed.xgyro), 1, INT16_T},
+        { "ygyro", &(parsed.ygyro), 1, INT16_T},
+        { "zgyro", &(parsed.zgyro), 1, INT16_T},
+        { "xmag", &(parsed.xmag), 1, INT16_T},
+        { "ymag", &(parsed.ymag), 1, INT16_T},
+        { "zmag", &(parsed.zmag), 1, INT16_T},
+        { "id", &(parsed.id), 1, UINT8_T},
+        { "temperature", &(parsed.temperature), 1, INT16_T}
+    };
+    static cStruct record = {"raw_imu", members, 12, 27};
+
+    mavlink_msg_raw_imu_decode(message, &parsed);
+    return &record;
+}
+
+cStruct* unbox_open_drone_id_arm_status(const mavlink_message_t* message)
+{
+    static mavlink_open_drone_id_arm_status_t parsed;
+
+    static cMember members[] = {
+        { "status", &(parsed.status), 1, UINT8_T},
+        { "error", &(parsed.error), 50, CHAR}
+    };
+    static cStruct record = {"open_drone_id_arm_status", members, 2, 12918};
+
+    mavlink_msg_open_drone_id_arm_status_decode(message, &parsed);
     return &record;
 }
 
 cStruct* unbox_mission_item(const mavlink_message_t* message)
 {
     static mavlink_mission_item_t parsed;
 
@@ -4518,2771 +4565,2724 @@
     };
     static cStruct record = {"mission_item", members, 15, 39};
 
     mavlink_msg_mission_item_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_actuator_control_target(const mavlink_message_t* message)
+cStruct* unbox_open_drone_id_location(const mavlink_message_t* message)
 {
-    static mavlink_actuator_control_target_t parsed;
+    static mavlink_open_drone_id_location_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "controls", &(parsed.controls), 8, FLOAT},
-        { "group_mlx", &(parsed.group_mlx), 1, UINT8_T}
+        { "latitude", &(parsed.latitude), 1, INT32_T},
+        { "longitude", &(parsed.longitude), 1, INT32_T},
+        { "altitude_barometric", &(parsed.altitude_barometric), 1, FLOAT},
+        { "altitude_geodetic", &(parsed.altitude_geodetic), 1, FLOAT},
+        { "height", &(parsed.height), 1, FLOAT},
+        { "timestamp", &(parsed.timestamp), 1, FLOAT},
+        { "direction", &(parsed.direction), 1, UINT16_T},
+        { "speed_horizontal", &(parsed.speed_horizontal), 1, UINT16_T},
+        { "speed_vertical", &(parsed.speed_vertical), 1, INT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "id_or_mac", &(parsed.id_or_mac), 20, UINT8_T},
+        { "status", &(parsed.status), 1, UINT8_T},
+        { "height_reference", &(parsed.height_reference), 1, UINT8_T},
+        { "horizontal_accuracy", &(parsed.horizontal_accuracy), 1, UINT8_T},
+        { "vertical_accuracy", &(parsed.vertical_accuracy), 1, UINT8_T},
+        { "barometer_accuracy", &(parsed.barometer_accuracy), 1, UINT8_T},
+        { "speed_accuracy", &(parsed.speed_accuracy), 1, UINT8_T},
+        { "timestamp_accuracy", &(parsed.timestamp_accuracy), 1, UINT8_T}
     };
-    static cStruct record = {"actuator_control_target", members, 3, 140};
+    static cStruct record = {"open_drone_id_location", members, 19, 12901};
 
-    mavlink_msg_actuator_control_target_decode(message, &parsed);
+    mavlink_msg_open_drone_id_location_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_storage_information(const mavlink_message_t* message)
+cStruct* unbox_response_event_error(const mavlink_message_t* message)
 {
-    static mavlink_storage_information_t parsed;
+    static mavlink_response_event_error_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "total_capacity", &(parsed.total_capacity), 1, FLOAT},
-        { "used_capacity", &(parsed.used_capacity), 1, FLOAT},
-        { "available_capacity", &(parsed.available_capacity), 1, FLOAT},
-        { "read_speed", &(parsed.read_speed), 1, FLOAT},
-        { "write_speed", &(parsed.write_speed), 1, FLOAT},
-        { "storage_id", &(parsed.storage_id), 1, UINT8_T},
-        { "storage_count", &(parsed.storage_count), 1, UINT8_T},
-        { "status", &(parsed.status), 1, UINT8_T},
-        { "type", &(parsed.type), 1, UINT8_T},
-        { "name", &(parsed.name), 32, CHAR},
-        { "storage_usage", &(parsed.storage_usage), 1, UINT8_T}
+        { "sequence", &(parsed.sequence), 1, UINT16_T},
+        { "sequence_oldest_available", &(parsed.sequence_oldest_available), 1, UINT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "reason", &(parsed.reason), 1, UINT8_T}
     };
-    static cStruct record = {"storage_information", members, 12, 261};
+    static cStruct record = {"response_event_error", members, 5, 413};
 
-    mavlink_msg_storage_information_decode(message, &parsed);
+    mavlink_msg_response_event_error_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_time_estimate_to_target(const mavlink_message_t* message)
+cStruct* unbox_smart_battery_info(const mavlink_message_t* message)
 {
-    static mavlink_time_estimate_to_target_t parsed;
+    static mavlink_smart_battery_info_t parsed;
 
     static cMember members[] = {
-        { "safe_return", &(parsed.safe_return), 1, INT32_T},
-        { "land", &(parsed.land), 1, INT32_T},
-        { "mission_next_item", &(parsed.mission_next_item), 1, INT32_T},
-        { "mission_end", &(parsed.mission_end), 1, INT32_T},
-        { "commanded_action", &(parsed.commanded_action), 1, INT32_T}
+        { "capacity_full_specification", &(parsed.capacity_full_specification), 1, INT32_T},
+        { "capacity_full", &(parsed.capacity_full), 1, INT32_T},
+        { "cycle_count", &(parsed.cycle_count), 1, UINT16_T},
+        { "weight", &(parsed.weight), 1, UINT16_T},
+        { "discharge_minimum_voltage", &(parsed.discharge_minimum_voltage), 1, UINT16_T},
+        { "charging_minimum_voltage", &(parsed.charging_minimum_voltage), 1, UINT16_T},
+        { "resting_minimum_voltage", &(parsed.resting_minimum_voltage), 1, UINT16_T},
+        { "id", &(parsed.id), 1, UINT8_T},
+        { "battery_function", &(parsed.battery_function), 1, UINT8_T},
+        { "type", &(parsed.type), 1, UINT8_T},
+        { "serial_number", &(parsed.serial_number), 16, CHAR},
+        { "device_name", &(parsed.device_name), 50, CHAR},
+        { "charging_maximum_voltage", &(parsed.charging_maximum_voltage), 1, UINT16_T},
+        { "cells_in_series", &(parsed.cells_in_series), 1, UINT8_T},
+        { "discharge_maximum_current", &(parsed.discharge_maximum_current), 1, UINT32_T},
+        { "discharge_maximum_burst_current", &(parsed.discharge_maximum_burst_current), 1, UINT32_T},
+        { "manufacture_date", &(parsed.manufacture_date), 11, CHAR}
     };
-    static cStruct record = {"time_estimate_to_target", members, 5, 380};
+    static cStruct record = {"smart_battery_info", members, 17, 370};
 
-    mavlink_msg_time_estimate_to_target_decode(message, &parsed);
+    mavlink_msg_smart_battery_info_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_mission_ack(const mavlink_message_t* message)
+cStruct* unbox_mission_write_partial_list(const mavlink_message_t* message)
 {
-    static mavlink_mission_ack_t parsed;
+    static mavlink_mission_write_partial_list_t parsed;
 
     static cMember members[] = {
+        { "start_index", &(parsed.start_index), 1, INT16_T},
+        { "end_index", &(parsed.end_index), 1, INT16_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "type", &(parsed.type), 1, UINT8_T},
         { "mission_type", &(parsed.mission_type), 1, UINT8_T}
     };
-    static cStruct record = {"mission_ack", members, 4, 47};
+    static cStruct record = {"mission_write_partial_list", members, 5, 38};
 
-    mavlink_msg_mission_ack_decode(message, &parsed);
+    mavlink_msg_mission_write_partial_list_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_position_target_local_ned(const mavlink_message_t* message)
+cStruct* unbox_sim_state(const mavlink_message_t* message)
 {
-    static mavlink_position_target_local_ned_t parsed;
+    static mavlink_sim_state_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "x", &(parsed.x), 1, FLOAT},
-        { "y", &(parsed.y), 1, FLOAT},
-        { "z", &(parsed.z), 1, FLOAT},
-        { "vx", &(parsed.vx), 1, FLOAT},
-        { "vy", &(parsed.vy), 1, FLOAT},
-        { "vz", &(parsed.vz), 1, FLOAT},
-        { "afx", &(parsed.afx), 1, FLOAT},
-        { "afy", &(parsed.afy), 1, FLOAT},
-        { "afz", &(parsed.afz), 1, FLOAT},
+        { "q1", &(parsed.q1), 1, FLOAT},
+        { "q2", &(parsed.q2), 1, FLOAT},
+        { "q3", &(parsed.q3), 1, FLOAT},
+        { "q4", &(parsed.q4), 1, FLOAT},
+        { "roll", &(parsed.roll), 1, FLOAT},
+        { "pitch", &(parsed.pitch), 1, FLOAT},
         { "yaw", &(parsed.yaw), 1, FLOAT},
-        { "yaw_rate", &(parsed.yaw_rate), 1, FLOAT},
-        { "type_mask", &(parsed.type_mask), 1, UINT16_T},
-        { "coordinate_frame", &(parsed.coordinate_frame), 1, UINT8_T}
+        { "xacc", &(parsed.xacc), 1, FLOAT},
+        { "yacc", &(parsed.yacc), 1, FLOAT},
+        { "zacc", &(parsed.zacc), 1, FLOAT},
+        { "xgyro", &(parsed.xgyro), 1, FLOAT},
+        { "ygyro", &(parsed.ygyro), 1, FLOAT},
+        { "zgyro", &(parsed.zgyro), 1, FLOAT},
+        { "lat", &(parsed.lat), 1, FLOAT},
+        { "lon", &(parsed.lon), 1, FLOAT},
+        { "alt", &(parsed.alt), 1, FLOAT},
+        { "std_dev_horz", &(parsed.std_dev_horz), 1, FLOAT},
+        { "std_dev_vert", &(parsed.std_dev_vert), 1, FLOAT},
+        { "vn", &(parsed.vn), 1, FLOAT},
+        { "ve", &(parsed.ve), 1, FLOAT},
+        { "vd", &(parsed.vd), 1, FLOAT},
+        { "lat_int", &(parsed.lat_int), 1, INT32_T},
+        { "lon_int", &(parsed.lon_int), 1, INT32_T}
     };
-    static cStruct record = {"position_target_local_ned", members, 14, 85};
+    static cStruct record = {"sim_state", members, 23, 108};
 
-    mavlink_msg_position_target_local_ned_decode(message, &parsed);
+    mavlink_msg_sim_state_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_trajectory_representation_waypoints(const mavlink_message_t* message)
+cStruct* unbox_mission_count(const mavlink_message_t* message)
 {
-    static mavlink_trajectory_representation_waypoints_t parsed;
+    static mavlink_mission_count_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "pos_x", &(parsed.pos_x), 5, FLOAT},
-        { "pos_y", &(parsed.pos_y), 5, FLOAT},
-        { "pos_z", &(parsed.pos_z), 5, FLOAT},
-        { "vel_x", &(parsed.vel_x), 5, FLOAT},
-        { "vel_y", &(parsed.vel_y), 5, FLOAT},
-        { "vel_z", &(parsed.vel_z), 5, FLOAT},
-        { "acc_x", &(parsed.acc_x), 5, FLOAT},
-        { "acc_y", &(parsed.acc_y), 5, FLOAT},
-        { "acc_z", &(parsed.acc_z), 5, FLOAT},
-        { "pos_yaw", &(parsed.pos_yaw), 5, FLOAT},
-        { "vel_yaw", &(parsed.vel_yaw), 5, FLOAT},
-        { "command", &(parsed.command), 5, UINT16_T},
-        { "valid_points", &(parsed.valid_points), 1, UINT8_T}
+        { "count", &(parsed.count), 1, UINT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "mission_type", &(parsed.mission_type), 1, UINT8_T}
     };
-    static cStruct record = {"trajectory_representation_waypoints", members, 14, 332};
+    static cStruct record = {"mission_count", members, 4, 44};
 
-    mavlink_msg_trajectory_representation_waypoints_decode(message, &parsed);
+    mavlink_msg_mission_count_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_local_position_ned_cov(const mavlink_message_t* message)
+cStruct* unbox_memory_vect(const mavlink_message_t* message)
 {
-    static mavlink_local_position_ned_cov_t parsed;
+    static mavlink_memory_vect_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "x", &(parsed.x), 1, FLOAT},
-        { "y", &(parsed.y), 1, FLOAT},
-        { "z", &(parsed.z), 1, FLOAT},
+        { "address", &(parsed.address), 1, UINT16_T},
+        { "ver", &(parsed.ver), 1, UINT8_T},
+        { "type", &(parsed.type), 1, UINT8_T},
+        { "value", &(parsed.value), 32, INT8_T}
+    };
+    static cStruct record = {"memory_vect", members, 4, 249};
+
+    mavlink_msg_memory_vect_decode(message, &parsed);
+    return &record;
+}
+
+cStruct* unbox_position_target_global_int(const mavlink_message_t* message)
+{
+    static mavlink_position_target_global_int_t parsed;
+
+    static cMember members[] = {
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "lat_int", &(parsed.lat_int), 1, INT32_T},
+        { "lon_int", &(parsed.lon_int), 1, INT32_T},
+        { "alt", &(parsed.alt), 1, FLOAT},
         { "vx", &(parsed.vx), 1, FLOAT},
         { "vy", &(parsed.vy), 1, FLOAT},
         { "vz", &(parsed.vz), 1, FLOAT},
-        { "ax", &(parsed.ax), 1, FLOAT},
-        { "ay", &(parsed.ay), 1, FLOAT},
-        { "az", &(parsed.az), 1, FLOAT},
-        { "covariance", &(parsed.covariance), 45, FLOAT},
-        { "estimator_type", &(parsed.estimator_type), 1, UINT8_T}
+        { "afx", &(parsed.afx), 1, FLOAT},
+        { "afy", &(parsed.afy), 1, FLOAT},
+        { "afz", &(parsed.afz), 1, FLOAT},
+        { "yaw", &(parsed.yaw), 1, FLOAT},
+        { "yaw_rate", &(parsed.yaw_rate), 1, FLOAT},
+        { "type_mask", &(parsed.type_mask), 1, UINT16_T},
+        { "coordinate_frame", &(parsed.coordinate_frame), 1, UINT8_T}
     };
-    static cStruct record = {"local_position_ned_cov", members, 12, 64};
+    static cStruct record = {"position_target_global_int", members, 14, 87};
 
-    mavlink_msg_local_position_ned_cov_decode(message, &parsed);
+    mavlink_msg_position_target_global_int_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_control_system_state(const mavlink_message_t* message)
+cStruct* unbox_altitude(const mavlink_message_t* message)
 {
-    static mavlink_control_system_state_t parsed;
+    static mavlink_altitude_t parsed;
 
     static cMember members[] = {
         { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "x_acc", &(parsed.x_acc), 1, FLOAT},
-        { "y_acc", &(parsed.y_acc), 1, FLOAT},
-        { "z_acc", &(parsed.z_acc), 1, FLOAT},
-        { "x_vel", &(parsed.x_vel), 1, FLOAT},
-        { "y_vel", &(parsed.y_vel), 1, FLOAT},
-        { "z_vel", &(parsed.z_vel), 1, FLOAT},
-        { "x_pos", &(parsed.x_pos), 1, FLOAT},
-        { "y_pos", &(parsed.y_pos), 1, FLOAT},
-        { "z_pos", &(parsed.z_pos), 1, FLOAT},
-        { "airspeed", &(parsed.airspeed), 1, FLOAT},
-        { "vel_variance", &(parsed.vel_variance), 3, FLOAT},
-        { "pos_variance", &(parsed.pos_variance), 3, FLOAT},
-        { "q", &(parsed.q), 4, FLOAT},
-        { "roll_rate", &(parsed.roll_rate), 1, FLOAT},
-        { "pitch_rate", &(parsed.pitch_rate), 1, FLOAT},
-        { "yaw_rate", &(parsed.yaw_rate), 1, FLOAT}
+        { "altitude_monotonic", &(parsed.altitude_monotonic), 1, FLOAT},
+        { "altitude_amsl", &(parsed.altitude_amsl), 1, FLOAT},
+        { "altitude_local", &(parsed.altitude_local), 1, FLOAT},
+        { "altitude_relative", &(parsed.altitude_relative), 1, FLOAT},
+        { "altitude_terrain", &(parsed.altitude_terrain), 1, FLOAT},
+        { "bottom_clearance", &(parsed.bottom_clearance), 1, FLOAT}
     };
-    static cStruct record = {"control_system_state", members, 17, 146};
+    static cStruct record = {"altitude", members, 7, 141};
 
-    mavlink_msg_control_system_state_decode(message, &parsed);
+    mavlink_msg_altitude_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_orbit_execution_status(const mavlink_message_t* message)
+cStruct* unbox_sens_mppt(const mavlink_message_t* message)
 {
-    static mavlink_orbit_execution_status_t parsed;
+    static mavlink_sens_mppt_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "radius", &(parsed.radius), 1, FLOAT},
+        { "mppt_timestamp", &(parsed.mppt_timestamp), 1, UINT64_T},
+        { "mppt1_volt", &(parsed.mppt1_volt), 1, FLOAT},
+        { "mppt1_amp", &(parsed.mppt1_amp), 1, FLOAT},
+        { "mppt2_volt", &(parsed.mppt2_volt), 1, FLOAT},
+        { "mppt2_amp", &(parsed.mppt2_amp), 1, FLOAT},
+        { "mppt3_volt", &(parsed.mppt3_volt), 1, FLOAT},
+        { "mppt3_amp", &(parsed.mppt3_amp), 1, FLOAT},
+        { "mppt1_pwm", &(parsed.mppt1_pwm), 1, UINT16_T},
+        { "mppt2_pwm", &(parsed.mppt2_pwm), 1, UINT16_T},
+        { "mppt3_pwm", &(parsed.mppt3_pwm), 1, UINT16_T},
+        { "mppt1_status", &(parsed.mppt1_status), 1, UINT8_T},
+        { "mppt2_status", &(parsed.mppt2_status), 1, UINT8_T},
+        { "mppt3_status", &(parsed.mppt3_status), 1, UINT8_T}
+    };
+    static cStruct record = {"sens_mppt", members, 13, 8003};
+
+    mavlink_msg_sens_mppt_decode(message, &parsed);
+    return &record;
+}
+
+cStruct* unbox_command_int_stamped(const mavlink_message_t* message)
+{
+    static mavlink_command_int_stamped_t parsed;
+
+    static cMember members[] = {
+        { "vehicle_timestamp", &(parsed.vehicle_timestamp), 1, UINT64_T},
+        { "utc_time", &(parsed.utc_time), 1, UINT32_T},
+        { "param1", &(parsed.param1), 1, FLOAT},
+        { "param2", &(parsed.param2), 1, FLOAT},
+        { "param3", &(parsed.param3), 1, FLOAT},
+        { "param4", &(parsed.param4), 1, FLOAT},
         { "x", &(parsed.x), 1, INT32_T},
         { "y", &(parsed.y), 1, INT32_T},
         { "z", &(parsed.z), 1, FLOAT},
-        { "frame", &(parsed.frame), 1, UINT8_T}
+        { "command", &(parsed.command), 1, UINT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "frame", &(parsed.frame), 1, UINT8_T},
+        { "current", &(parsed.current), 1, UINT8_T},
+        { "autocontinue", &(parsed.autocontinue), 1, UINT8_T}
     };
-    static cStruct record = {"orbit_execution_status", members, 6, 360};
+    static cStruct record = {"command_int_stamped", members, 15, 223};
 
-    mavlink_msg_orbit_execution_status_decode(message, &parsed);
+    mavlink_msg_command_int_stamped_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_efi_status(const mavlink_message_t* message)
+cStruct* unbox_sens_batmon(const mavlink_message_t* message)
 {
-    static mavlink_efi_status_t parsed;
+    static mavlink_sens_batmon_t parsed;
 
     static cMember members[] = {
-        { "ecu_index", &(parsed.ecu_index), 1, FLOAT},
-        { "rpm", &(parsed.rpm), 1, FLOAT},
-        { "fuel_consumed", &(parsed.fuel_consumed), 1, FLOAT},
-        { "fuel_flow", &(parsed.fuel_flow), 1, FLOAT},
-        { "engine_load", &(parsed.engine_load), 1, FLOAT},
-        { "throttle_position", &(parsed.throttle_position), 1, FLOAT},
-        { "spark_dwell_time", &(parsed.spark_dwell_time), 1, FLOAT},
-        { "barometric_pressure", &(parsed.barometric_pressure), 1, FLOAT},
-        { "intake_manifold_pressure", &(parsed.intake_manifold_pressure), 1, FLOAT},
-        { "intake_manifold_temperature", &(parsed.intake_manifold_temperature), 1, FLOAT},
-        { "cylinder_head_temperature", &(parsed.cylinder_head_temperature), 1, FLOAT},
-        { "ignition_timing", &(parsed.ignition_timing), 1, FLOAT},
-        { "injection_time", &(parsed.injection_time), 1, FLOAT},
-        { "exhaust_gas_temperature", &(parsed.exhaust_gas_temperature), 1, FLOAT},
-        { "throttle_out", &(parsed.throttle_out), 1, FLOAT},
-        { "pt_compensation", &(parsed.pt_compensation), 1, FLOAT},
-        { "health", &(parsed.health), 1, UINT8_T},
-        { "ignition_voltage", &(parsed.ignition_voltage), 1, FLOAT},
-        { "fuel_pressure", &(parsed.fuel_pressure), 1, FLOAT}
+        { "batmon_timestamp", &(parsed.batmon_timestamp), 1, UINT64_T},
+        { "temperature", &(parsed.temperature), 1, FLOAT},
+        { "safetystatus", &(parsed.safetystatus), 1, UINT32_T},
+        { "operationstatus", &(parsed.operationstatus), 1, UINT32_T},
+        { "voltage", &(parsed.voltage), 1, UINT16_T},
+        { "current", &(parsed.current), 1, INT16_T},
+        { "batterystatus", &(parsed.batterystatus), 1, UINT16_T},
+        { "serialnumber", &(parsed.serialnumber), 1, UINT16_T},
+        { "cellvoltage1", &(parsed.cellvoltage1), 1, UINT16_T},
+        { "cellvoltage2", &(parsed.cellvoltage2), 1, UINT16_T},
+        { "cellvoltage3", &(parsed.cellvoltage3), 1, UINT16_T},
+        { "cellvoltage4", &(parsed.cellvoltage4), 1, UINT16_T},
+        { "cellvoltage5", &(parsed.cellvoltage5), 1, UINT16_T},
+        { "cellvoltage6", &(parsed.cellvoltage6), 1, UINT16_T},
+        { "SoC", &(parsed.SoC), 1, UINT8_T}
     };
-    static cStruct record = {"efi_status", members, 19, 225};
+    static cStruct record = {"sens_batmon", members, 15, 8010};
 
-    mavlink_msg_efi_status_decode(message, &parsed);
+    mavlink_msg_sens_batmon_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_debug_float_array(const mavlink_message_t* message)
+cStruct* unbox_aslctrl_debug(const mavlink_message_t* message)
 {
-    static mavlink_debug_float_array_t parsed;
+    static mavlink_aslctrl_debug_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "array_id", &(parsed.array_id), 1, UINT16_T},
-        { "name", &(parsed.name), 10, CHAR},
-        { "data", &(parsed.data), 58, FLOAT}
+        { "i32_1", &(parsed.i32_1), 1, UINT32_T},
+        { "f_1", &(parsed.f_1), 1, FLOAT},
+        { "f_2", &(parsed.f_2), 1, FLOAT},
+        { "f_3", &(parsed.f_3), 1, FLOAT},
+        { "f_4", &(parsed.f_4), 1, FLOAT},
+        { "f_5", &(parsed.f_5), 1, FLOAT},
+        { "f_6", &(parsed.f_6), 1, FLOAT},
+        { "f_7", &(parsed.f_7), 1, FLOAT},
+        { "f_8", &(parsed.f_8), 1, FLOAT},
+        { "i8_1", &(parsed.i8_1), 1, UINT8_T},
+        { "i8_2", &(parsed.i8_2), 1, UINT8_T}
     };
-    static cStruct record = {"debug_float_array", members, 4, 350};
+    static cStruct record = {"aslctrl_debug", members, 11, 8005};
 
-    mavlink_msg_debug_float_array_decode(message, &parsed);
+    mavlink_msg_aslctrl_debug_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_response_event_error(const mavlink_message_t* message)
+cStruct* unbox_sens_atmos(const mavlink_message_t* message)
 {
-    static mavlink_response_event_error_t parsed;
+    static mavlink_sens_atmos_t parsed;
 
     static cMember members[] = {
-        { "sequence", &(parsed.sequence), 1, UINT16_T},
-        { "sequence_oldest_available", &(parsed.sequence_oldest_available), 1, UINT16_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "reason", &(parsed.reason), 1, UINT8_T}
+        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
+        { "TempAmbient", &(parsed.TempAmbient), 1, FLOAT},
+        { "Humidity", &(parsed.Humidity), 1, FLOAT}
     };
-    static cStruct record = {"response_event_error", members, 5, 413};
+    static cStruct record = {"sens_atmos", members, 3, 8009};
 
-    mavlink_msg_response_event_error_decode(message, &parsed);
+    mavlink_msg_sens_atmos_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_can_frame(const mavlink_message_t* message)
+cStruct* unbox_satcom_link_status(const mavlink_message_t* message)
 {
-    static mavlink_can_frame_t parsed;
+    static mavlink_satcom_link_status_t parsed;
 
     static cMember members[] = {
-        { "id", &(parsed.id), 1, UINT32_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "bus", &(parsed.bus), 1, UINT8_T},
-        { "len", &(parsed.len), 1, UINT8_T},
-        { "data", &(parsed.data), 8, UINT8_T}
+        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
+        { "last_heartbeat", &(parsed.last_heartbeat), 1, UINT64_T},
+        { "failed_sessions", &(parsed.failed_sessions), 1, UINT16_T},
+        { "successful_sessions", &(parsed.successful_sessions), 1, UINT16_T},
+        { "signal_quality", &(parsed.signal_quality), 1, UINT8_T},
+        { "ring_pending", &(parsed.ring_pending), 1, UINT8_T},
+        { "tx_session_pending", &(parsed.tx_session_pending), 1, UINT8_T},
+        { "rx_session_pending", &(parsed.rx_session_pending), 1, UINT8_T}
     };
-    static cStruct record = {"can_frame", members, 6, 386};
+    static cStruct record = {"satcom_link_status", members, 8, 8015};
 
-    mavlink_msg_can_frame_decode(message, &parsed);
+    mavlink_msg_satcom_link_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_camera_settings(const mavlink_message_t* message)
+cStruct* unbox_fw_soaring_data(const mavlink_message_t* message)
 {
-    static mavlink_camera_settings_t parsed;
+    static mavlink_fw_soaring_data_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "mode_id", &(parsed.mode_id), 1, UINT8_T},
-        { "zoomLevel", &(parsed.zoomLevel), 1, FLOAT},
-        { "focusLevel", &(parsed.focusLevel), 1, FLOAT}
+        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
+        { "timestampModeChanged", &(parsed.timestampModeChanged), 1, UINT64_T},
+        { "xW", &(parsed.xW), 1, FLOAT},
+        { "xR", &(parsed.xR), 1, FLOAT},
+        { "xLat", &(parsed.xLat), 1, FLOAT},
+        { "xLon", &(parsed.xLon), 1, FLOAT},
+        { "VarW", &(parsed.VarW), 1, FLOAT},
+        { "VarR", &(parsed.VarR), 1, FLOAT},
+        { "VarLat", &(parsed.VarLat), 1, FLOAT},
+        { "VarLon", &(parsed.VarLon), 1, FLOAT},
+        { "LoiterRadius", &(parsed.LoiterRadius), 1, FLOAT},
+        { "LoiterDirection", &(parsed.LoiterDirection), 1, FLOAT},
+        { "DistToSoarPoint", &(parsed.DistToSoarPoint), 1, FLOAT},
+        { "vSinkExp", &(parsed.vSinkExp), 1, FLOAT},
+        { "z1_LocalUpdraftSpeed", &(parsed.z1_LocalUpdraftSpeed), 1, FLOAT},
+        { "z2_DeltaRoll", &(parsed.z2_DeltaRoll), 1, FLOAT},
+        { "z1_exp", &(parsed.z1_exp), 1, FLOAT},
+        { "z2_exp", &(parsed.z2_exp), 1, FLOAT},
+        { "ThermalGSNorth", &(parsed.ThermalGSNorth), 1, FLOAT},
+        { "ThermalGSEast", &(parsed.ThermalGSEast), 1, FLOAT},
+        { "TSE_dot", &(parsed.TSE_dot), 1, FLOAT},
+        { "DebugVar1", &(parsed.DebugVar1), 1, FLOAT},
+        { "DebugVar2", &(parsed.DebugVar2), 1, FLOAT},
+        { "ControlMode", &(parsed.ControlMode), 1, UINT8_T},
+        { "valid", &(parsed.valid), 1, UINT8_T}
     };
-    static cStruct record = {"camera_settings", members, 4, 260};
+    static cStruct record = {"fw_soaring_data", members, 25, 8011};
 
-    mavlink_msg_camera_settings_decode(message, &parsed);
+    mavlink_msg_fw_soaring_data_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_nav_controller_output(const mavlink_message_t* message)
+cStruct* unbox_aslctrl_data(const mavlink_message_t* message)
 {
-    static mavlink_nav_controller_output_t parsed;
+    static mavlink_aslctrl_data_t parsed;
 
     static cMember members[] = {
-        { "nav_roll", &(parsed.nav_roll), 1, FLOAT},
-        { "nav_pitch", &(parsed.nav_pitch), 1, FLOAT},
-        { "alt_error", &(parsed.alt_error), 1, FLOAT},
-        { "aspd_error", &(parsed.aspd_error), 1, FLOAT},
-        { "xtrack_error", &(parsed.xtrack_error), 1, FLOAT},
-        { "nav_bearing", &(parsed.nav_bearing), 1, INT16_T},
-        { "target_bearing", &(parsed.target_bearing), 1, INT16_T},
-        { "wp_dist", &(parsed.wp_dist), 1, UINT16_T}
+        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
+        { "h", &(parsed.h), 1, FLOAT},
+        { "hRef", &(parsed.hRef), 1, FLOAT},
+        { "hRef_t", &(parsed.hRef_t), 1, FLOAT},
+        { "PitchAngle", &(parsed.PitchAngle), 1, FLOAT},
+        { "PitchAngleRef", &(parsed.PitchAngleRef), 1, FLOAT},
+        { "q", &(parsed.q), 1, FLOAT},
+        { "qRef", &(parsed.qRef), 1, FLOAT},
+        { "uElev", &(parsed.uElev), 1, FLOAT},
+        { "uThrot", &(parsed.uThrot), 1, FLOAT},
+        { "uThrot2", &(parsed.uThrot2), 1, FLOAT},
+        { "nZ", &(parsed.nZ), 1, FLOAT},
+        { "AirspeedRef", &(parsed.AirspeedRef), 1, FLOAT},
+        { "YawAngle", &(parsed.YawAngle), 1, FLOAT},
+        { "YawAngleRef", &(parsed.YawAngleRef), 1, FLOAT},
+        { "RollAngle", &(parsed.RollAngle), 1, FLOAT},
+        { "RollAngleRef", &(parsed.RollAngleRef), 1, FLOAT},
+        { "p", &(parsed.p), 1, FLOAT},
+        { "pRef", &(parsed.pRef), 1, FLOAT},
+        { "r", &(parsed.r), 1, FLOAT},
+        { "rRef", &(parsed.rRef), 1, FLOAT},
+        { "uAil", &(parsed.uAil), 1, FLOAT},
+        { "uRud", &(parsed.uRud), 1, FLOAT},
+        { "aslctrl_mode", &(parsed.aslctrl_mode), 1, UINT8_T},
+        { "SpoilersEngaged", &(parsed.SpoilersEngaged), 1, UINT8_T}
     };
-    static cStruct record = {"nav_controller_output", members, 8, 62};
+    static cStruct record = {"aslctrl_data", members, 25, 8004};
 
-    mavlink_msg_nav_controller_output_decode(message, &parsed);
+    mavlink_msg_aslctrl_data_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_utm_global_position(const mavlink_message_t* message)
+cStruct* unbox_asluav_status(const mavlink_message_t* message)
 {
-    static mavlink_utm_global_position_t parsed;
+    static mavlink_asluav_status_t parsed;
 
     static cMember members[] = {
-        { "time", &(parsed.time), 1, UINT64_T},
-        { "lat", &(parsed.lat), 1, INT32_T},
-        { "lon", &(parsed.lon), 1, INT32_T},
-        { "alt", &(parsed.alt), 1, INT32_T},
-        { "relative_alt", &(parsed.relative_alt), 1, INT32_T},
-        { "next_lat", &(parsed.next_lat), 1, INT32_T},
-        { "next_lon", &(parsed.next_lon), 1, INT32_T},
-        { "next_alt", &(parsed.next_alt), 1, INT32_T},
-        { "vx", &(parsed.vx), 1, INT16_T},
-        { "vy", &(parsed.vy), 1, INT16_T},
-        { "vz", &(parsed.vz), 1, INT16_T},
-        { "h_acc", &(parsed.h_acc), 1, UINT16_T},
-        { "v_acc", &(parsed.v_acc), 1, UINT16_T},
-        { "vel_acc", &(parsed.vel_acc), 1, UINT16_T},
-        { "update_rate", &(parsed.update_rate), 1, UINT16_T},
-        { "uas_id", &(parsed.uas_id), 18, UINT8_T},
-        { "flight_state", &(parsed.flight_state), 1, UINT8_T},
-        { "flags", &(parsed.flags), 1, UINT8_T}
+        { "Motor_rpm", &(parsed.Motor_rpm), 1, FLOAT},
+        { "LED_status", &(parsed.LED_status), 1, UINT8_T},
+        { "SATCOM_status", &(parsed.SATCOM_status), 1, UINT8_T},
+        { "Servo_status", &(parsed.Servo_status), 8, UINT8_T}
     };
-    static cStruct record = {"utm_global_position", members, 18, 340};
+    static cStruct record = {"asluav_status", members, 4, 8006};
 
-    mavlink_msg_utm_global_position_decode(message, &parsed);
+    mavlink_msg_asluav_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_raw_imu(const mavlink_message_t* message)
+cStruct* unbox_sens_power_board(const mavlink_message_t* message)
 {
-    static mavlink_raw_imu_t parsed;
+    static mavlink_sens_power_board_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "xacc", &(parsed.xacc), 1, INT16_T},
-        { "yacc", &(parsed.yacc), 1, INT16_T},
-        { "zacc", &(parsed.zacc), 1, INT16_T},
-        { "xgyro", &(parsed.xgyro), 1, INT16_T},
-        { "ygyro", &(parsed.ygyro), 1, INT16_T},
-        { "zgyro", &(parsed.zgyro), 1, INT16_T},
-        { "xmag", &(parsed.xmag), 1, INT16_T},
-        { "ymag", &(parsed.ymag), 1, INT16_T},
-        { "zmag", &(parsed.zmag), 1, INT16_T},
-        { "id", &(parsed.id), 1, UINT8_T},
-        { "temperature", &(parsed.temperature), 1, INT16_T}
+        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
+        { "pwr_brd_system_volt", &(parsed.pwr_brd_system_volt), 1, FLOAT},
+        { "pwr_brd_servo_volt", &(parsed.pwr_brd_servo_volt), 1, FLOAT},
+        { "pwr_brd_digital_volt", &(parsed.pwr_brd_digital_volt), 1, FLOAT},
+        { "pwr_brd_mot_l_amp", &(parsed.pwr_brd_mot_l_amp), 1, FLOAT},
+        { "pwr_brd_mot_r_amp", &(parsed.pwr_brd_mot_r_amp), 1, FLOAT},
+        { "pwr_brd_analog_amp", &(parsed.pwr_brd_analog_amp), 1, FLOAT},
+        { "pwr_brd_digital_amp", &(parsed.pwr_brd_digital_amp), 1, FLOAT},
+        { "pwr_brd_ext_amp", &(parsed.pwr_brd_ext_amp), 1, FLOAT},
+        { "pwr_brd_aux_amp", &(parsed.pwr_brd_aux_amp), 1, FLOAT},
+        { "pwr_brd_status", &(parsed.pwr_brd_status), 1, UINT8_T},
+        { "pwr_brd_led_status", &(parsed.pwr_brd_led_status), 1, UINT8_T}
     };
-    static cStruct record = {"raw_imu", members, 12, 27};
+    static cStruct record = {"sens_power_board", members, 12, 8013};
 
-    mavlink_msg_raw_imu_decode(message, &parsed);
+    mavlink_msg_sens_power_board_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_camera_fov_status(const mavlink_message_t* message)
+cStruct* unbox_gsm_link_status(const mavlink_message_t* message)
 {
-    static mavlink_camera_fov_status_t parsed;
+    static mavlink_gsm_link_status_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "lat_camera", &(parsed.lat_camera), 1, INT32_T},
-        { "lon_camera", &(parsed.lon_camera), 1, INT32_T},
-        { "alt_camera", &(parsed.alt_camera), 1, INT32_T},
-        { "lat_image", &(parsed.lat_image), 1, INT32_T},
-        { "lon_image", &(parsed.lon_image), 1, INT32_T},
-        { "alt_image", &(parsed.alt_image), 1, INT32_T},
-        { "q", &(parsed.q), 4, FLOAT},
-        { "hfov", &(parsed.hfov), 1, FLOAT},
-        { "vfov", &(parsed.vfov), 1, FLOAT}
+        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
+        { "gsm_modem_type", &(parsed.gsm_modem_type), 1, UINT8_T},
+        { "gsm_link_type", &(parsed.gsm_link_type), 1, UINT8_T},
+        { "rssi", &(parsed.rssi), 1, UINT8_T},
+        { "rsrp_rscp", &(parsed.rsrp_rscp), 1, UINT8_T},
+        { "sinr_ecio", &(parsed.sinr_ecio), 1, UINT8_T},
+        { "rsrq", &(parsed.rsrq), 1, UINT8_T}
     };
-    static cStruct record = {"camera_fov_status", members, 10, 271};
+    static cStruct record = {"gsm_link_status", members, 7, 8014};
 
-    mavlink_msg_camera_fov_status_decode(message, &parsed);
+    mavlink_msg_gsm_link_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_hil_rc_inputs_raw(const mavlink_message_t* message)
+cStruct* unbox_command_long_stamped(const mavlink_message_t* message)
 {
-    static mavlink_hil_rc_inputs_raw_t parsed;
+    static mavlink_command_long_stamped_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "chan1_raw", &(parsed.chan1_raw), 1, UINT16_T},
-        { "chan2_raw", &(parsed.chan2_raw), 1, UINT16_T},
-        { "chan3_raw", &(parsed.chan3_raw), 1, UINT16_T},
-        { "chan4_raw", &(parsed.chan4_raw), 1, UINT16_T},
-        { "chan5_raw", &(parsed.chan5_raw), 1, UINT16_T},
-        { "chan6_raw", &(parsed.chan6_raw), 1, UINT16_T},
-        { "chan7_raw", &(parsed.chan7_raw), 1, UINT16_T},
-        { "chan8_raw", &(parsed.chan8_raw), 1, UINT16_T},
-        { "chan9_raw", &(parsed.chan9_raw), 1, UINT16_T},
-        { "chan10_raw", &(parsed.chan10_raw), 1, UINT16_T},
-        { "chan11_raw", &(parsed.chan11_raw), 1, UINT16_T},
-        { "chan12_raw", &(parsed.chan12_raw), 1, UINT16_T},
-        { "rssi", &(parsed.rssi), 1, UINT8_T}
+        { "vehicle_timestamp", &(parsed.vehicle_timestamp), 1, UINT64_T},
+        { "utc_time", &(parsed.utc_time), 1, UINT32_T},
+        { "param1", &(parsed.param1), 1, FLOAT},
+        { "param2", &(parsed.param2), 1, FLOAT},
+        { "param3", &(parsed.param3), 1, FLOAT},
+        { "param4", &(parsed.param4), 1, FLOAT},
+        { "param5", &(parsed.param5), 1, FLOAT},
+        { "param6", &(parsed.param6), 1, FLOAT},
+        { "param7", &(parsed.param7), 1, FLOAT},
+        { "command", &(parsed.command), 1, UINT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "confirmation", &(parsed.confirmation), 1, UINT8_T}
     };
-    static cStruct record = {"hil_rc_inputs_raw", members, 14, 92};
+    static cStruct record = {"command_long_stamped", members, 13, 224};
 
-    mavlink_msg_hil_rc_inputs_raw_decode(message, &parsed);
+    mavlink_msg_command_long_stamped_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_logging_ack(const mavlink_message_t* message)
+cStruct* unbox_sensor_airflow_angles(const mavlink_message_t* message)
 {
-    static mavlink_logging_ack_t parsed;
+    static mavlink_sensor_airflow_angles_t parsed;
 
     static cMember members[] = {
-        { "sequence", &(parsed.sequence), 1, UINT16_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T}
+        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
+        { "angleofattack", &(parsed.angleofattack), 1, FLOAT},
+        { "sideslip", &(parsed.sideslip), 1, FLOAT},
+        { "angleofattack_valid", &(parsed.angleofattack_valid), 1, UINT8_T},
+        { "sideslip_valid", &(parsed.sideslip_valid), 1, UINT8_T}
     };
-    static cStruct record = {"logging_ack", members, 3, 268};
+    static cStruct record = {"sensor_airflow_angles", members, 5, 8016};
 
-    mavlink_msg_logging_ack_decode(message, &parsed);
+    mavlink_msg_sensor_airflow_angles_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_timesync(const mavlink_message_t* message)
+cStruct* unbox_ekf_ext(const mavlink_message_t* message)
 {
-    static mavlink_timesync_t parsed;
+    static mavlink_ekf_ext_t parsed;
 
     static cMember members[] = {
-        { "tc1", &(parsed.tc1), 1, INT64_T},
-        { "ts1", &(parsed.ts1), 1, INT64_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T}
+        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
+        { "Windspeed", &(parsed.Windspeed), 1, FLOAT},
+        { "WindDir", &(parsed.WindDir), 1, FLOAT},
+        { "WindZ", &(parsed.WindZ), 1, FLOAT},
+        { "Airspeed", &(parsed.Airspeed), 1, FLOAT},
+        { "beta", &(parsed.beta), 1, FLOAT},
+        { "alpha", &(parsed.alpha), 1, FLOAT}
     };
-    static cStruct record = {"timesync", members, 4, 111};
+    static cStruct record = {"ekf_ext", members, 7, 8007};
 
-    mavlink_msg_timesync_decode(message, &parsed);
+    mavlink_msg_ekf_ext_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_gps_global_origin(const mavlink_message_t* message)
+cStruct* unbox_sensorpod_status(const mavlink_message_t* message)
 {
-    static mavlink_gps_global_origin_t parsed;
+    static mavlink_sensorpod_status_t parsed;
 
     static cMember members[] = {
-        { "latitude", &(parsed.latitude), 1, INT32_T},
-        { "longitude", &(parsed.longitude), 1, INT32_T},
-        { "altitude", &(parsed.altitude), 1, INT32_T},
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T}
+        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
+        { "free_space", &(parsed.free_space), 1, UINT16_T},
+        { "visensor_rate_1", &(parsed.visensor_rate_1), 1, UINT8_T},
+        { "visensor_rate_2", &(parsed.visensor_rate_2), 1, UINT8_T},
+        { "visensor_rate_3", &(parsed.visensor_rate_3), 1, UINT8_T},
+        { "visensor_rate_4", &(parsed.visensor_rate_4), 1, UINT8_T},
+        { "recording_nodes_count", &(parsed.recording_nodes_count), 1, UINT8_T},
+        { "cpu_temp", &(parsed.cpu_temp), 1, UINT8_T}
     };
-    static cStruct record = {"gps_global_origin", members, 4, 49};
+    static cStruct record = {"sensorpod_status", members, 8, 8012};
 
-    mavlink_msg_gps_global_origin_decode(message, &parsed);
+    mavlink_msg_sensorpod_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_debug_vect(const mavlink_message_t* message)
+cStruct* unbox_sens_power(const mavlink_message_t* message)
 {
-    static mavlink_debug_vect_t parsed;
+    static mavlink_sens_power_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "x", &(parsed.x), 1, FLOAT},
-        { "y", &(parsed.y), 1, FLOAT},
-        { "z", &(parsed.z), 1, FLOAT},
-        { "name", &(parsed.name), 10, CHAR}
+        { "adc121_vspb_volt", &(parsed.adc121_vspb_volt), 1, FLOAT},
+        { "adc121_cspb_amp", &(parsed.adc121_cspb_amp), 1, FLOAT},
+        { "adc121_cs1_amp", &(parsed.adc121_cs1_amp), 1, FLOAT},
+        { "adc121_cs2_amp", &(parsed.adc121_cs2_amp), 1, FLOAT}
     };
-    static cStruct record = {"debug_vect", members, 5, 250};
+    static cStruct record = {"sens_power", members, 4, 8002};
 
-    mavlink_msg_debug_vect_decode(message, &parsed);
+    mavlink_msg_sens_power_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_gimbal_manager_status(const mavlink_message_t* message)
+cStruct* unbox_asl_obctrl(const mavlink_message_t* message)
 {
-    static mavlink_gimbal_manager_status_t parsed;
+    static mavlink_asl_obctrl_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "flags", &(parsed.flags), 1, UINT32_T},
-        { "gimbal_device_id", &(parsed.gimbal_device_id), 1, UINT8_T},
-        { "primary_control_sysid", &(parsed.primary_control_sysid), 1, UINT8_T},
-        { "primary_control_compid", &(parsed.primary_control_compid), 1, UINT8_T},
-        { "secondary_control_sysid", &(parsed.secondary_control_sysid), 1, UINT8_T},
-        { "secondary_control_compid", &(parsed.secondary_control_compid), 1, UINT8_T}
+        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
+        { "uElev", &(parsed.uElev), 1, FLOAT},
+        { "uThrot", &(parsed.uThrot), 1, FLOAT},
+        { "uThrot2", &(parsed.uThrot2), 1, FLOAT},
+        { "uAilL", &(parsed.uAilL), 1, FLOAT},
+        { "uAilR", &(parsed.uAilR), 1, FLOAT},
+        { "uRud", &(parsed.uRud), 1, FLOAT},
+        { "obctrl_status", &(parsed.obctrl_status), 1, UINT8_T}
     };
-    static cStruct record = {"gimbal_manager_status", members, 7, 281};
+    static cStruct record = {"asl_obctrl", members, 8, 8008};
 
-    mavlink_msg_gimbal_manager_status_decode(message, &parsed);
+    mavlink_msg_asl_obctrl_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_actuator_output_status(const mavlink_message_t* message)
+cStruct* unbox_mag_cal_progress(const mavlink_message_t* message)
 {
-    static mavlink_actuator_output_status_t parsed;
+    static mavlink_mag_cal_progress_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "active", &(parsed.active), 1, UINT32_T},
-        { "actuator", &(parsed.actuator), 32, FLOAT}
+        { "direction_x", &(parsed.direction_x), 1, FLOAT},
+        { "direction_y", &(parsed.direction_y), 1, FLOAT},
+        { "direction_z", &(parsed.direction_z), 1, FLOAT},
+        { "compass_id", &(parsed.compass_id), 1, UINT8_T},
+        { "cal_mask", &(parsed.cal_mask), 1, UINT8_T},
+        { "cal_status", &(parsed.cal_status), 1, UINT8_T},
+        { "attempt", &(parsed.attempt), 1, UINT8_T},
+        { "completion_pct", &(parsed.completion_pct), 1, UINT8_T},
+        { "completion_mask", &(parsed.completion_mask), 10, UINT8_T}
     };
-    static cStruct record = {"actuator_output_status", members, 3, 375};
+    static cStruct record = {"mag_cal_progress", members, 9, 191};
 
-    mavlink_msg_actuator_output_status_decode(message, &parsed);
+    mavlink_msg_mag_cal_progress_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_open_drone_id_system(const mavlink_message_t* message)
+cStruct* unbox_ahrs(const mavlink_message_t* message)
 {
-    static mavlink_open_drone_id_system_t parsed;
+    static mavlink_ahrs_t parsed;
 
     static cMember members[] = {
-        { "operator_latitude", &(parsed.operator_latitude), 1, INT32_T},
-        { "operator_longitude", &(parsed.operator_longitude), 1, INT32_T},
-        { "area_ceiling", &(parsed.area_ceiling), 1, FLOAT},
-        { "area_floor", &(parsed.area_floor), 1, FLOAT},
-        { "operator_altitude_geo", &(parsed.operator_altitude_geo), 1, FLOAT},
-        { "timestamp", &(parsed.timestamp), 1, UINT32_T},
-        { "area_count", &(parsed.area_count), 1, UINT16_T},
-        { "area_radius", &(parsed.area_radius), 1, UINT16_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "id_or_mac", &(parsed.id_or_mac), 20, UINT8_T},
-        { "operator_location_type", &(parsed.operator_location_type), 1, UINT8_T},
-        { "classification_type", &(parsed.classification_type), 1, UINT8_T},
-        { "category_eu", &(parsed.category_eu), 1, UINT8_T},
-        { "class_eu", &(parsed.class_eu), 1, UINT8_T}
+        { "omegaIx", &(parsed.omegaIx), 1, FLOAT},
+        { "omegaIy", &(parsed.omegaIy), 1, FLOAT},
+        { "omegaIz", &(parsed.omegaIz), 1, FLOAT},
+        { "accel_weight", &(parsed.accel_weight), 1, FLOAT},
+        { "renorm_val", &(parsed.renorm_val), 1, FLOAT},
+        { "error_rp", &(parsed.error_rp), 1, FLOAT},
+        { "error_yaw", &(parsed.error_yaw), 1, FLOAT}
     };
-    static cStruct record = {"open_drone_id_system", members, 15, 12904};
+    static cStruct record = {"ahrs", members, 7, 163};
 
-    mavlink_msg_open_drone_id_system_decode(message, &parsed);
+    mavlink_msg_ahrs_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_altitude(const mavlink_message_t* message)
+cStruct* unbox_wind(const mavlink_message_t* message)
 {
-    static mavlink_altitude_t parsed;
+    static mavlink_wind_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "altitude_monotonic", &(parsed.altitude_monotonic), 1, FLOAT},
-        { "altitude_amsl", &(parsed.altitude_amsl), 1, FLOAT},
-        { "altitude_local", &(parsed.altitude_local), 1, FLOAT},
-        { "altitude_relative", &(parsed.altitude_relative), 1, FLOAT},
-        { "altitude_terrain", &(parsed.altitude_terrain), 1, FLOAT},
-        { "bottom_clearance", &(parsed.bottom_clearance), 1, FLOAT}
+        { "direction", &(parsed.direction), 1, FLOAT},
+        { "speed", &(parsed.speed), 1, FLOAT},
+        { "speed_z", &(parsed.speed_z), 1, FLOAT}
     };
-    static cStruct record = {"altitude", members, 7, 141};
+    static cStruct record = {"wind", members, 3, 168};
 
-    mavlink_msg_altitude_decode(message, &parsed);
+    mavlink_msg_wind_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_vfr_hud(const mavlink_message_t* message)
+cStruct* unbox_gopro_get_request(const mavlink_message_t* message)
 {
-    static mavlink_vfr_hud_t parsed;
+    static mavlink_gopro_get_request_t parsed;
 
     static cMember members[] = {
-        { "airspeed", &(parsed.airspeed), 1, FLOAT},
-        { "groundspeed", &(parsed.groundspeed), 1, FLOAT},
-        { "alt", &(parsed.alt), 1, FLOAT},
-        { "climb", &(parsed.climb), 1, FLOAT},
-        { "heading", &(parsed.heading), 1, INT16_T},
-        { "throttle", &(parsed.throttle), 1, UINT16_T}
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "cmd_id", &(parsed.cmd_id), 1, UINT8_T}
     };
-    static cStruct record = {"vfr_hud", members, 6, 74};
+    static cStruct record = {"gopro_get_request", members, 3, 216};
 
-    mavlink_msg_vfr_hud_decode(message, &parsed);
+    mavlink_msg_gopro_get_request_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_terrain_report(const mavlink_message_t* message)
+cStruct* unbox_rpm(const mavlink_message_t* message)
 {
-    static mavlink_terrain_report_t parsed;
+    static mavlink_rpm_t parsed;
 
     static cMember members[] = {
-        { "lat", &(parsed.lat), 1, INT32_T},
-        { "lon", &(parsed.lon), 1, INT32_T},
-        { "terrain_height", &(parsed.terrain_height), 1, FLOAT},
-        { "current_height", &(parsed.current_height), 1, FLOAT},
-        { "spacing", &(parsed.spacing), 1, UINT16_T},
-        { "pending", &(parsed.pending), 1, UINT16_T},
-        { "loaded", &(parsed.loaded), 1, UINT16_T}
+        { "rpm1", &(parsed.rpm1), 1, FLOAT},
+        { "rpm2", &(parsed.rpm2), 1, FLOAT}
     };
-    static cStruct record = {"terrain_report", members, 7, 136};
+    static cStruct record = {"rpm", members, 2, 226};
 
-    mavlink_msg_terrain_report_decode(message, &parsed);
+    mavlink_msg_rpm_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_gimbal_manager_information(const mavlink_message_t* message)
+cStruct* unbox_obstacle_distance_3d(const mavlink_message_t* message)
 {
-    static mavlink_gimbal_manager_information_t parsed;
+    static mavlink_obstacle_distance_3d_t parsed;
 
     static cMember members[] = {
         { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "cap_flags", &(parsed.cap_flags), 1, UINT32_T},
-        { "roll_min", &(parsed.roll_min), 1, FLOAT},
-        { "roll_max", &(parsed.roll_max), 1, FLOAT},
-        { "pitch_min", &(parsed.pitch_min), 1, FLOAT},
-        { "pitch_max", &(parsed.pitch_max), 1, FLOAT},
-        { "yaw_min", &(parsed.yaw_min), 1, FLOAT},
-        { "yaw_max", &(parsed.yaw_max), 1, FLOAT},
-        { "gimbal_device_id", &(parsed.gimbal_device_id), 1, UINT8_T}
+        { "x", &(parsed.x), 1, FLOAT},
+        { "y", &(parsed.y), 1, FLOAT},
+        { "z", &(parsed.z), 1, FLOAT},
+        { "min_distance", &(parsed.min_distance), 1, FLOAT},
+        { "max_distance", &(parsed.max_distance), 1, FLOAT},
+        { "obstacle_id", &(parsed.obstacle_id), 1, UINT16_T},
+        { "sensor_type", &(parsed.sensor_type), 1, UINT8_T},
+        { "frame", &(parsed.frame), 1, UINT8_T}
     };
-    static cStruct record = {"gimbal_manager_information", members, 9, 280};
+    static cStruct record = {"obstacle_distance_3d", members, 9, 11037};
 
-    mavlink_msg_gimbal_manager_information_decode(message, &parsed);
+    mavlink_msg_obstacle_distance_3d_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_cellular_status(const mavlink_message_t* message)
+cStruct* unbox_device_op_write_reply(const mavlink_message_t* message)
 {
-    static mavlink_cellular_status_t parsed;
+    static mavlink_device_op_write_reply_t parsed;
 
     static cMember members[] = {
-        { "mcc", &(parsed.mcc), 1, UINT16_T},
-        { "mnc", &(parsed.mnc), 1, UINT16_T},
-        { "lac", &(parsed.lac), 1, UINT16_T},
-        { "status", &(parsed.status), 1, UINT8_T},
-        { "failure_reason", &(parsed.failure_reason), 1, UINT8_T},
-        { "type", &(parsed.type), 1, UINT8_T},
-        { "quality", &(parsed.quality), 1, UINT8_T}
+        { "request_id", &(parsed.request_id), 1, UINT32_T},
+        { "result", &(parsed.result), 1, UINT8_T}
     };
-    static cStruct record = {"cellular_status", members, 7, 334};
+    static cStruct record = {"device_op_write_reply", members, 2, 11003};
 
-    mavlink_msg_cellular_status_decode(message, &parsed);
+    mavlink_msg_device_op_write_reply_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_mag_cal_report(const mavlink_message_t* message)
+cStruct* unbox_camera_feedback(const mavlink_message_t* message)
 {
-    static mavlink_mag_cal_report_t parsed;
+    static mavlink_camera_feedback_t parsed;
 
     static cMember members[] = {
-        { "fitness", &(parsed.fitness), 1, FLOAT},
-        { "ofs_x", &(parsed.ofs_x), 1, FLOAT},
-        { "ofs_y", &(parsed.ofs_y), 1, FLOAT},
-        { "ofs_z", &(parsed.ofs_z), 1, FLOAT},
-        { "diag_x", &(parsed.diag_x), 1, FLOAT},
-        { "diag_y", &(parsed.diag_y), 1, FLOAT},
-        { "diag_z", &(parsed.diag_z), 1, FLOAT},
-        { "offdiag_x", &(parsed.offdiag_x), 1, FLOAT},
-        { "offdiag_y", &(parsed.offdiag_y), 1, FLOAT},
-        { "offdiag_z", &(parsed.offdiag_z), 1, FLOAT},
-        { "compass_id", &(parsed.compass_id), 1, UINT8_T},
-        { "cal_mask", &(parsed.cal_mask), 1, UINT8_T},
-        { "cal_status", &(parsed.cal_status), 1, UINT8_T},
-        { "autosaved", &(parsed.autosaved), 1, UINT8_T},
-        { "orientation_confidence", &(parsed.orientation_confidence), 1, FLOAT},
-        { "old_orientation", &(parsed.old_orientation), 1, UINT8_T},
-        { "new_orientation", &(parsed.new_orientation), 1, UINT8_T},
-        { "scale_factor", &(parsed.scale_factor), 1, FLOAT}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "lat", &(parsed.lat), 1, INT32_T},
+        { "lng", &(parsed.lng), 1, INT32_T},
+        { "alt_msl", &(parsed.alt_msl), 1, FLOAT},
+        { "alt_rel", &(parsed.alt_rel), 1, FLOAT},
+        { "roll", &(parsed.roll), 1, FLOAT},
+        { "pitch", &(parsed.pitch), 1, FLOAT},
+        { "yaw", &(parsed.yaw), 1, FLOAT},
+        { "foc_len", &(parsed.foc_len), 1, FLOAT},
+        { "img_idx", &(parsed.img_idx), 1, UINT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "cam_idx", &(parsed.cam_idx), 1, UINT8_T},
+        { "flags", &(parsed.flags), 1, UINT8_T},
+        { "completed_captures", &(parsed.completed_captures), 1, UINT16_T}
     };
-    static cStruct record = {"mag_cal_report", members, 18, 192};
+    static cStruct record = {"camera_feedback", members, 14, 180};
 
-    mavlink_msg_mag_cal_report_decode(message, &parsed);
+    mavlink_msg_camera_feedback_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_raw_rpm(const mavlink_message_t* message)
+cStruct* unbox_meminfo(const mavlink_message_t* message)
 {
-    static mavlink_raw_rpm_t parsed;
+    static mavlink_meminfo_t parsed;
 
     static cMember members[] = {
-        { "frequency", &(parsed.frequency), 1, FLOAT},
-        { "index", &(parsed.index), 1, UINT8_T}
+        { "brkval", &(parsed.brkval), 1, UINT16_T},
+        { "freemem", &(parsed.freemem), 1, UINT16_T},
+        { "freemem32", &(parsed.freemem32), 1, UINT32_T}
     };
-    static cStruct record = {"raw_rpm", members, 2, 339};
+    static cStruct record = {"meminfo", members, 3, 152};
 
-    mavlink_msg_raw_rpm_decode(message, &parsed);
+    mavlink_msg_meminfo_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_param_value(const mavlink_message_t* message)
+cStruct* unbox_gopro_set_response(const mavlink_message_t* message)
 {
-    static mavlink_param_value_t parsed;
+    static mavlink_gopro_set_response_t parsed;
 
     static cMember members[] = {
-        { "param_value", &(parsed.param_value), 1, FLOAT},
-        { "param_count", &(parsed.param_count), 1, UINT16_T},
-        { "param_index", &(parsed.param_index), 1, UINT16_T},
-        { "param_id", &(parsed.param_id), 16, CHAR},
-        { "param_type", &(parsed.param_type), 1, UINT8_T}
+        { "cmd_id", &(parsed.cmd_id), 1, UINT8_T},
+        { "status", &(parsed.status), 1, UINT8_T}
     };
-    static cStruct record = {"param_value", members, 5, 22};
+    static cStruct record = {"gopro_set_response", members, 2, 219};
 
-    mavlink_msg_param_value_decode(message, &parsed);
+    mavlink_msg_gopro_set_response_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_highres_imu(const mavlink_message_t* message)
+cStruct* unbox_device_op_read_reply(const mavlink_message_t* message)
 {
-    static mavlink_highres_imu_t parsed;
+    static mavlink_device_op_read_reply_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "xacc", &(parsed.xacc), 1, FLOAT},
-        { "yacc", &(parsed.yacc), 1, FLOAT},
-        { "zacc", &(parsed.zacc), 1, FLOAT},
-        { "xgyro", &(parsed.xgyro), 1, FLOAT},
-        { "ygyro", &(parsed.ygyro), 1, FLOAT},
-        { "zgyro", &(parsed.zgyro), 1, FLOAT},
-        { "xmag", &(parsed.xmag), 1, FLOAT},
-        { "ymag", &(parsed.ymag), 1, FLOAT},
-        { "zmag", &(parsed.zmag), 1, FLOAT},
-        { "abs_pressure", &(parsed.abs_pressure), 1, FLOAT},
-        { "diff_pressure", &(parsed.diff_pressure), 1, FLOAT},
-        { "pressure_alt", &(parsed.pressure_alt), 1, FLOAT},
-        { "temperature", &(parsed.temperature), 1, FLOAT},
-        { "fields_updated", &(parsed.fields_updated), 1, UINT16_T},
-        { "id", &(parsed.id), 1, UINT8_T}
+        { "request_id", &(parsed.request_id), 1, UINT32_T},
+        { "result", &(parsed.result), 1, UINT8_T},
+        { "regstart", &(parsed.regstart), 1, UINT8_T},
+        { "count", &(parsed.count), 1, UINT8_T},
+        { "data", &(parsed.data), 128, UINT8_T},
+        { "bank", &(parsed.bank), 1, UINT8_T}
     };
-    static cStruct record = {"highres_imu", members, 16, 105};
+    static cStruct record = {"device_op_read_reply", members, 6, 11001};
 
-    mavlink_msg_highres_imu_decode(message, &parsed);
+    mavlink_msg_device_op_read_reply_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_hil_sensor(const mavlink_message_t* message)
+cStruct* unbox_camera_status(const mavlink_message_t* message)
 {
-    static mavlink_hil_sensor_t parsed;
+    static mavlink_camera_status_t parsed;
 
     static cMember members[] = {
         { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "xacc", &(parsed.xacc), 1, FLOAT},
-        { "yacc", &(parsed.yacc), 1, FLOAT},
-        { "zacc", &(parsed.zacc), 1, FLOAT},
-        { "xgyro", &(parsed.xgyro), 1, FLOAT},
-        { "ygyro", &(parsed.ygyro), 1, FLOAT},
-        { "zgyro", &(parsed.zgyro), 1, FLOAT},
-        { "xmag", &(parsed.xmag), 1, FLOAT},
-        { "ymag", &(parsed.ymag), 1, FLOAT},
-        { "zmag", &(parsed.zmag), 1, FLOAT},
-        { "abs_pressure", &(parsed.abs_pressure), 1, FLOAT},
-        { "diff_pressure", &(parsed.diff_pressure), 1, FLOAT},
-        { "pressure_alt", &(parsed.pressure_alt), 1, FLOAT},
-        { "temperature", &(parsed.temperature), 1, FLOAT},
-        { "fields_updated", &(parsed.fields_updated), 1, UINT32_T},
-        { "id", &(parsed.id), 1, UINT8_T}
+        { "p1", &(parsed.p1), 1, FLOAT},
+        { "p2", &(parsed.p2), 1, FLOAT},
+        { "p3", &(parsed.p3), 1, FLOAT},
+        { "p4", &(parsed.p4), 1, FLOAT},
+        { "img_idx", &(parsed.img_idx), 1, UINT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "cam_idx", &(parsed.cam_idx), 1, UINT8_T},
+        { "event_id", &(parsed.event_id), 1, UINT8_T}
     };
-    static cStruct record = {"hil_sensor", members, 16, 107};
+    static cStruct record = {"camera_status", members, 9, 179};
 
-    mavlink_msg_hil_sensor_decode(message, &parsed);
+    mavlink_msg_camera_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_rc_channels_override(const mavlink_message_t* message)
+cStruct* unbox_pid_tuning(const mavlink_message_t* message)
 {
-    static mavlink_rc_channels_override_t parsed;
+    static mavlink_pid_tuning_t parsed;
 
     static cMember members[] = {
-        { "chan1_raw", &(parsed.chan1_raw), 1, UINT16_T},
-        { "chan2_raw", &(parsed.chan2_raw), 1, UINT16_T},
-        { "chan3_raw", &(parsed.chan3_raw), 1, UINT16_T},
-        { "chan4_raw", &(parsed.chan4_raw), 1, UINT16_T},
-        { "chan5_raw", &(parsed.chan5_raw), 1, UINT16_T},
-        { "chan6_raw", &(parsed.chan6_raw), 1, UINT16_T},
-        { "chan7_raw", &(parsed.chan7_raw), 1, UINT16_T},
-        { "chan8_raw", &(parsed.chan8_raw), 1, UINT16_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "chan9_raw", &(parsed.chan9_raw), 1, UINT16_T},
-        { "chan10_raw", &(parsed.chan10_raw), 1, UINT16_T},
-        { "chan11_raw", &(parsed.chan11_raw), 1, UINT16_T},
-        { "chan12_raw", &(parsed.chan12_raw), 1, UINT16_T},
-        { "chan13_raw", &(parsed.chan13_raw), 1, UINT16_T},
-        { "chan14_raw", &(parsed.chan14_raw), 1, UINT16_T},
-        { "chan15_raw", &(parsed.chan15_raw), 1, UINT16_T},
-        { "chan16_raw", &(parsed.chan16_raw), 1, UINT16_T},
-        { "chan17_raw", &(parsed.chan17_raw), 1, UINT16_T},
-        { "chan18_raw", &(parsed.chan18_raw), 1, UINT16_T}
+        { "desired", &(parsed.desired), 1, FLOAT},
+        { "achieved", &(parsed.achieved), 1, FLOAT},
+        { "FF", &(parsed.FF), 1, FLOAT},
+        { "P", &(parsed.P), 1, FLOAT},
+        { "I", &(parsed.I), 1, FLOAT},
+        { "D", &(parsed.D), 1, FLOAT},
+        { "axis", &(parsed.axis), 1, UINT8_T},
+        { "SRate", &(parsed.SRate), 1, FLOAT},
+        { "PDmod", &(parsed.PDmod), 1, FLOAT}
     };
-    static cStruct record = {"rc_channels_override", members, 20, 70};
+    static cStruct record = {"pid_tuning", members, 9, 194};
 
-    mavlink_msg_rc_channels_override_decode(message, &parsed);
+    mavlink_msg_pid_tuning_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_cellular_config(const mavlink_message_t* message)
+cStruct* unbox_set_mag_offsets(const mavlink_message_t* message)
 {
-    static mavlink_cellular_config_t parsed;
+    static mavlink_set_mag_offsets_t parsed;
 
     static cMember members[] = {
-        { "enable_lte", &(parsed.enable_lte), 1, UINT8_T},
-        { "enable_pin", &(parsed.enable_pin), 1, UINT8_T},
-        { "pin", &(parsed.pin), 16, CHAR},
-        { "new_pin", &(parsed.new_pin), 16, CHAR},
-        { "apn", &(parsed.apn), 32, CHAR},
-        { "puk", &(parsed.puk), 16, CHAR},
-        { "roaming", &(parsed.roaming), 1, UINT8_T},
-        { "response", &(parsed.response), 1, UINT8_T}
+        { "mag_ofs_x", &(parsed.mag_ofs_x), 1, INT16_T},
+        { "mag_ofs_y", &(parsed.mag_ofs_y), 1, INT16_T},
+        { "mag_ofs_z", &(parsed.mag_ofs_z), 1, INT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T}
     };
-    static cStruct record = {"cellular_config", members, 8, 336};
+    static cStruct record = {"set_mag_offsets", members, 5, 151};
 
-    mavlink_msg_cellular_config_decode(message, &parsed);
+    mavlink_msg_set_mag_offsets_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_gps2_rtk(const mavlink_message_t* message)
+cStruct* unbox_rangefinder(const mavlink_message_t* message)
 {
-    static mavlink_gps2_rtk_t parsed;
+    static mavlink_rangefinder_t parsed;
 
     static cMember members[] = {
-        { "time_last_baseline_ms", &(parsed.time_last_baseline_ms), 1, UINT32_T},
-        { "tow", &(parsed.tow), 1, UINT32_T},
-        { "baseline_a_mm", &(parsed.baseline_a_mm), 1, INT32_T},
-        { "baseline_b_mm", &(parsed.baseline_b_mm), 1, INT32_T},
-        { "baseline_c_mm", &(parsed.baseline_c_mm), 1, INT32_T},
-        { "accuracy", &(parsed.accuracy), 1, UINT32_T},
-        { "iar_num_hypotheses", &(parsed.iar_num_hypotheses), 1, INT32_T},
-        { "wn", &(parsed.wn), 1, UINT16_T},
-        { "rtk_receiver_id", &(parsed.rtk_receiver_id), 1, UINT8_T},
-        { "rtk_health", &(parsed.rtk_health), 1, UINT8_T},
-        { "rtk_rate", &(parsed.rtk_rate), 1, UINT8_T},
-        { "nsats", &(parsed.nsats), 1, UINT8_T},
-        { "baseline_coords_type", &(parsed.baseline_coords_type), 1, UINT8_T}
+        { "distance", &(parsed.distance), 1, FLOAT},
+        { "voltage", &(parsed.voltage), 1, FLOAT}
     };
-    static cStruct record = {"gps2_rtk", members, 13, 128};
+    static cStruct record = {"rangefinder", members, 2, 173};
 
-    mavlink_msg_gps2_rtk_decode(message, &parsed);
+    mavlink_msg_rangefinder_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_trajectory_representation_bezier(const mavlink_message_t* message)
+cStruct* unbox_mount_control(const mavlink_message_t* message)
 {
-    static mavlink_trajectory_representation_bezier_t parsed;
+    static mavlink_mount_control_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "pos_x", &(parsed.pos_x), 5, FLOAT},
-        { "pos_y", &(parsed.pos_y), 5, FLOAT},
-        { "pos_z", &(parsed.pos_z), 5, FLOAT},
-        { "delta", &(parsed.delta), 5, FLOAT},
-        { "pos_yaw", &(parsed.pos_yaw), 5, FLOAT},
-        { "valid_points", &(parsed.valid_points), 1, UINT8_T}
+        { "input_a", &(parsed.input_a), 1, INT32_T},
+        { "input_b", &(parsed.input_b), 1, INT32_T},
+        { "input_c", &(parsed.input_c), 1, INT32_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "save_position", &(parsed.save_position), 1, UINT8_T}
     };
-    static cStruct record = {"trajectory_representation_bezier", members, 7, 333};
+    static cStruct record = {"mount_control", members, 6, 157};
 
-    mavlink_msg_trajectory_representation_bezier_decode(message, &parsed);
+    mavlink_msg_mount_control_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_log_request_end(const mavlink_message_t* message)
+cStruct* unbox_gimbal_torque_cmd_report(const mavlink_message_t* message)
 {
-    static mavlink_log_request_end_t parsed;
+    static mavlink_gimbal_torque_cmd_report_t parsed;
 
     static cMember members[] = {
+        { "rl_torque_cmd", &(parsed.rl_torque_cmd), 1, INT16_T},
+        { "el_torque_cmd", &(parsed.el_torque_cmd), 1, INT16_T},
+        { "az_torque_cmd", &(parsed.az_torque_cmd), 1, INT16_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T}
     };
-    static cStruct record = {"log_request_end", members, 2, 122};
+    static cStruct record = {"gimbal_torque_cmd_report", members, 5, 214};
 
-    mavlink_msg_log_request_end_decode(message, &parsed);
+    mavlink_msg_gimbal_torque_cmd_report_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_mission_request_int(const mavlink_message_t* message)
+cStruct* unbox_fence_fetch_point(const mavlink_message_t* message)
 {
-    static mavlink_mission_request_int_t parsed;
+    static mavlink_fence_fetch_point_t parsed;
 
     static cMember members[] = {
-        { "seq", &(parsed.seq), 1, UINT16_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "mission_type", &(parsed.mission_type), 1, UINT8_T}
+        { "idx", &(parsed.idx), 1, UINT8_T}
     };
-    static cStruct record = {"mission_request_int", members, 4, 51};
+    static cStruct record = {"fence_fetch_point", members, 3, 161};
 
-    mavlink_msg_mission_request_int_decode(message, &parsed);
+    mavlink_msg_fence_fetch_point_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_sys_status(const mavlink_message_t* message)
+cStruct* unbox_ekf_status_report(const mavlink_message_t* message)
 {
-    static mavlink_sys_status_t parsed;
+    static mavlink_ekf_status_report_t parsed;
 
     static cMember members[] = {
-        { "onboard_control_sensors_present", &(parsed.onboard_control_sensors_present), 1, UINT32_T},
-        { "onboard_control_sensors_enabled", &(parsed.onboard_control_sensors_enabled), 1, UINT32_T},
-        { "onboard_control_sensors_health", &(parsed.onboard_control_sensors_health), 1, UINT32_T},
-        { "load", &(parsed.load), 1, UINT16_T},
-        { "voltage_battery", &(parsed.voltage_battery), 1, UINT16_T},
-        { "current_battery", &(parsed.current_battery), 1, INT16_T},
-        { "drop_rate_comm", &(parsed.drop_rate_comm), 1, UINT16_T},
-        { "errors_comm", &(parsed.errors_comm), 1, UINT16_T},
-        { "errors_count1", &(parsed.errors_count1), 1, UINT16_T},
-        { "errors_count2", &(parsed.errors_count2), 1, UINT16_T},
-        { "errors_count3", &(parsed.errors_count3), 1, UINT16_T},
-        { "errors_count4", &(parsed.errors_count4), 1, UINT16_T},
-        { "battery_remaining", &(parsed.battery_remaining), 1, INT8_T},
-        { "onboard_control_sensors_present_extended", &(parsed.onboard_control_sensors_present_extended), 1, UINT32_T},
-        { "onboard_control_sensors_enabled_extended", &(parsed.onboard_control_sensors_enabled_extended), 1, UINT32_T},
-        { "onboard_control_sensors_health_extended", &(parsed.onboard_control_sensors_health_extended), 1, UINT32_T}
+        { "velocity_variance", &(parsed.velocity_variance), 1, FLOAT},
+        { "pos_horiz_variance", &(parsed.pos_horiz_variance), 1, FLOAT},
+        { "pos_vert_variance", &(parsed.pos_vert_variance), 1, FLOAT},
+        { "compass_variance", &(parsed.compass_variance), 1, FLOAT},
+        { "terrain_alt_variance", &(parsed.terrain_alt_variance), 1, FLOAT},
+        { "flags", &(parsed.flags), 1, UINT16_T},
+        { "airspeed_variance", &(parsed.airspeed_variance), 1, FLOAT}
     };
-    static cStruct record = {"sys_status", members, 16, 1};
+    static cStruct record = {"ekf_status_report", members, 7, 193};
 
-    mavlink_msg_sys_status_decode(message, &parsed);
+    mavlink_msg_ekf_status_report_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_global_position_int_cov(const mavlink_message_t* message)
+cStruct* unbox_data96(const mavlink_message_t* message)
 {
-    static mavlink_global_position_int_cov_t parsed;
+    static mavlink_data96_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "lat", &(parsed.lat), 1, INT32_T},
-        { "lon", &(parsed.lon), 1, INT32_T},
-        { "alt", &(parsed.alt), 1, INT32_T},
-        { "relative_alt", &(parsed.relative_alt), 1, INT32_T},
-        { "vx", &(parsed.vx), 1, FLOAT},
-        { "vy", &(parsed.vy), 1, FLOAT},
-        { "vz", &(parsed.vz), 1, FLOAT},
-        { "covariance", &(parsed.covariance), 36, FLOAT},
-        { "estimator_type", &(parsed.estimator_type), 1, UINT8_T}
+        { "type", &(parsed.type), 1, UINT8_T},
+        { "len", &(parsed.len), 1, UINT8_T},
+        { "data", &(parsed.data), 96, UINT8_T}
     };
-    static cStruct record = {"global_position_int_cov", members, 10, 63};
+    static cStruct record = {"data96", members, 3, 172};
 
-    mavlink_msg_global_position_int_cov_decode(message, &parsed);
+    mavlink_msg_data96_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_param_ext_request_list(const mavlink_message_t* message)
+cStruct* unbox_osd_param_show_config(const mavlink_message_t* message)
 {
-    static mavlink_param_ext_request_list_t parsed;
+    static mavlink_osd_param_show_config_t parsed;
 
     static cMember members[] = {
+        { "request_id", &(parsed.request_id), 1, UINT32_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T}
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "osd_screen", &(parsed.osd_screen), 1, UINT8_T},
+        { "osd_index", &(parsed.osd_index), 1, UINT8_T}
     };
-    static cStruct record = {"param_ext_request_list", members, 2, 321};
+    static cStruct record = {"osd_param_show_config", members, 5, 11035};
 
-    mavlink_msg_param_ext_request_list_decode(message, &parsed);
+    mavlink_msg_osd_param_show_config_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_sim_state(const mavlink_message_t* message)
+cStruct* unbox_ahrs3(const mavlink_message_t* message)
 {
-    static mavlink_sim_state_t parsed;
+    static mavlink_ahrs3_t parsed;
 
     static cMember members[] = {
-        { "q1", &(parsed.q1), 1, FLOAT},
-        { "q2", &(parsed.q2), 1, FLOAT},
-        { "q3", &(parsed.q3), 1, FLOAT},
-        { "q4", &(parsed.q4), 1, FLOAT},
         { "roll", &(parsed.roll), 1, FLOAT},
         { "pitch", &(parsed.pitch), 1, FLOAT},
         { "yaw", &(parsed.yaw), 1, FLOAT},
-        { "xacc", &(parsed.xacc), 1, FLOAT},
-        { "yacc", &(parsed.yacc), 1, FLOAT},
-        { "zacc", &(parsed.zacc), 1, FLOAT},
-        { "xgyro", &(parsed.xgyro), 1, FLOAT},
-        { "ygyro", &(parsed.ygyro), 1, FLOAT},
-        { "zgyro", &(parsed.zgyro), 1, FLOAT},
-        { "lat", &(parsed.lat), 1, FLOAT},
-        { "lon", &(parsed.lon), 1, FLOAT},
-        { "alt", &(parsed.alt), 1, FLOAT},
-        { "std_dev_horz", &(parsed.std_dev_horz), 1, FLOAT},
-        { "std_dev_vert", &(parsed.std_dev_vert), 1, FLOAT},
-        { "vn", &(parsed.vn), 1, FLOAT},
-        { "ve", &(parsed.ve), 1, FLOAT},
-        { "vd", &(parsed.vd), 1, FLOAT},
-        { "lat_int", &(parsed.lat_int), 1, INT32_T},
-        { "lon_int", &(parsed.lon_int), 1, INT32_T}
+        { "altitude", &(parsed.altitude), 1, FLOAT},
+        { "lat", &(parsed.lat), 1, INT32_T},
+        { "lng", &(parsed.lng), 1, INT32_T},
+        { "v1", &(parsed.v1), 1, FLOAT},
+        { "v2", &(parsed.v2), 1, FLOAT},
+        { "v3", &(parsed.v3), 1, FLOAT},
+        { "v4", &(parsed.v4), 1, FLOAT}
     };
-    static cStruct record = {"sim_state", members, 23, 108};
+    static cStruct record = {"ahrs3", members, 10, 182};
 
-    mavlink_msg_sim_state_decode(message, &parsed);
+    mavlink_msg_ahrs3_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_param_ext_set(const mavlink_message_t* message)
+cStruct* unbox_limits_status(const mavlink_message_t* message)
 {
-    static mavlink_param_ext_set_t parsed;
+    static mavlink_limits_status_t parsed;
 
     static cMember members[] = {
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "param_id", &(parsed.param_id), 16, CHAR},
-        { "param_value", &(parsed.param_value), 128, CHAR},
-        { "param_type", &(parsed.param_type), 1, UINT8_T}
+        { "last_trigger", &(parsed.last_trigger), 1, UINT32_T},
+        { "last_action", &(parsed.last_action), 1, UINT32_T},
+        { "last_recovery", &(parsed.last_recovery), 1, UINT32_T},
+        { "last_clear", &(parsed.last_clear), 1, UINT32_T},
+        { "breach_count", &(parsed.breach_count), 1, UINT16_T},
+        { "limits_state", &(parsed.limits_state), 1, UINT8_T},
+        { "mods_enabled", &(parsed.mods_enabled), 1, UINT8_T},
+        { "mods_required", &(parsed.mods_required), 1, UINT8_T},
+        { "mods_triggered", &(parsed.mods_triggered), 1, UINT8_T}
     };
-    static cStruct record = {"param_ext_set", members, 5, 323};
+    static cStruct record = {"limits_status", members, 9, 167};
 
-    mavlink_msg_param_ext_set_decode(message, &parsed);
+    mavlink_msg_limits_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_scaled_pressure(const mavlink_message_t* message)
+cStruct* unbox_gopro_set_request(const mavlink_message_t* message)
 {
-    static mavlink_scaled_pressure_t parsed;
+    static mavlink_gopro_set_request_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "press_abs", &(parsed.press_abs), 1, FLOAT},
-        { "press_diff", &(parsed.press_diff), 1, FLOAT},
-        { "temperature", &(parsed.temperature), 1, INT16_T},
-        { "temperature_press_diff", &(parsed.temperature_press_diff), 1, INT16_T}
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "cmd_id", &(parsed.cmd_id), 1, UINT8_T},
+        { "value", &(parsed.value), 4, UINT8_T}
     };
-    static cStruct record = {"scaled_pressure", members, 5, 29};
+    static cStruct record = {"gopro_set_request", members, 4, 218};
 
-    mavlink_msg_scaled_pressure_decode(message, &parsed);
+    mavlink_msg_gopro_set_request_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_terrain_request(const mavlink_message_t* message)
+cStruct* unbox_sensor_offsets(const mavlink_message_t* message)
 {
-    static mavlink_terrain_request_t parsed;
+    static mavlink_sensor_offsets_t parsed;
 
     static cMember members[] = {
-        { "mask", &(parsed.mask), 1, UINT64_T},
-        { "lat", &(parsed.lat), 1, INT32_T},
-        { "lon", &(parsed.lon), 1, INT32_T},
-        { "grid_spacing", &(parsed.grid_spacing), 1, UINT16_T}
+        { "mag_declination", &(parsed.mag_declination), 1, FLOAT},
+        { "raw_press", &(parsed.raw_press), 1, INT32_T},
+        { "raw_temp", &(parsed.raw_temp), 1, INT32_T},
+        { "gyro_cal_x", &(parsed.gyro_cal_x), 1, FLOAT},
+        { "gyro_cal_y", &(parsed.gyro_cal_y), 1, FLOAT},
+        { "gyro_cal_z", &(parsed.gyro_cal_z), 1, FLOAT},
+        { "accel_cal_x", &(parsed.accel_cal_x), 1, FLOAT},
+        { "accel_cal_y", &(parsed.accel_cal_y), 1, FLOAT},
+        { "accel_cal_z", &(parsed.accel_cal_z), 1, FLOAT},
+        { "mag_ofs_x", &(parsed.mag_ofs_x), 1, INT16_T},
+        { "mag_ofs_y", &(parsed.mag_ofs_y), 1, INT16_T},
+        { "mag_ofs_z", &(parsed.mag_ofs_z), 1, INT16_T}
     };
-    static cStruct record = {"terrain_request", members, 4, 133};
+    static cStruct record = {"sensor_offsets", members, 12, 150};
 
-    mavlink_msg_terrain_request_decode(message, &parsed);
+    mavlink_msg_sensor_offsets_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_named_value_float(const mavlink_message_t* message)
+cStruct* unbox_ahrs2(const mavlink_message_t* message)
 {
-    static mavlink_named_value_float_t parsed;
+    static mavlink_ahrs2_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "value", &(parsed.value), 1, FLOAT},
-        { "name", &(parsed.name), 10, CHAR}
+        { "roll", &(parsed.roll), 1, FLOAT},
+        { "pitch", &(parsed.pitch), 1, FLOAT},
+        { "yaw", &(parsed.yaw), 1, FLOAT},
+        { "altitude", &(parsed.altitude), 1, FLOAT},
+        { "lat", &(parsed.lat), 1, INT32_T},
+        { "lng", &(parsed.lng), 1, INT32_T}
     };
-    static cStruct record = {"named_value_float", members, 3, 251};
+    static cStruct record = {"ahrs2", members, 6, 178};
 
-    mavlink_msg_named_value_float_decode(message, &parsed);
+    mavlink_msg_ahrs2_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_radio_status(const mavlink_message_t* message)
+cStruct* unbox_data32(const mavlink_message_t* message)
 {
-    static mavlink_radio_status_t parsed;
+    static mavlink_data32_t parsed;
 
     static cMember members[] = {
-        { "rxerrors", &(parsed.rxerrors), 1, UINT16_T},
-        { "fixed", &(parsed.fixed), 1, UINT16_T},
-        { "rssi", &(parsed.rssi), 1, UINT8_T},
-        { "remrssi", &(parsed.remrssi), 1, UINT8_T},
-        { "txbuf", &(parsed.txbuf), 1, UINT8_T},
-        { "noise", &(parsed.noise), 1, UINT8_T},
-        { "remnoise", &(parsed.remnoise), 1, UINT8_T}
+        { "type", &(parsed.type), 1, UINT8_T},
+        { "len", &(parsed.len), 1, UINT8_T},
+        { "data", &(parsed.data), 32, UINT8_T}
     };
-    static cStruct record = {"radio_status", members, 7, 109};
+    static cStruct record = {"data32", members, 3, 170};
 
-    mavlink_msg_radio_status_decode(message, &parsed);
+    mavlink_msg_data32_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_wind_cov(const mavlink_message_t* message)
+cStruct* unbox_gimbal_report(const mavlink_message_t* message)
 {
-    static mavlink_wind_cov_t parsed;
+    static mavlink_gimbal_report_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "wind_x", &(parsed.wind_x), 1, FLOAT},
-        { "wind_y", &(parsed.wind_y), 1, FLOAT},
-        { "wind_z", &(parsed.wind_z), 1, FLOAT},
-        { "var_horiz", &(parsed.var_horiz), 1, FLOAT},
-        { "var_vert", &(parsed.var_vert), 1, FLOAT},
-        { "wind_alt", &(parsed.wind_alt), 1, FLOAT},
-        { "horiz_accuracy", &(parsed.horiz_accuracy), 1, FLOAT},
-        { "vert_accuracy", &(parsed.vert_accuracy), 1, FLOAT}
+        { "delta_time", &(parsed.delta_time), 1, FLOAT},
+        { "delta_angle_x", &(parsed.delta_angle_x), 1, FLOAT},
+        { "delta_angle_y", &(parsed.delta_angle_y), 1, FLOAT},
+        { "delta_angle_z", &(parsed.delta_angle_z), 1, FLOAT},
+        { "delta_velocity_x", &(parsed.delta_velocity_x), 1, FLOAT},
+        { "delta_velocity_y", &(parsed.delta_velocity_y), 1, FLOAT},
+        { "delta_velocity_z", &(parsed.delta_velocity_z), 1, FLOAT},
+        { "joint_roll", &(parsed.joint_roll), 1, FLOAT},
+        { "joint_el", &(parsed.joint_el), 1, FLOAT},
+        { "joint_az", &(parsed.joint_az), 1, FLOAT},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T}
     };
-    static cStruct record = {"wind_cov", members, 9, 231};
+    static cStruct record = {"gimbal_report", members, 12, 200};
 
-    mavlink_msg_wind_cov_decode(message, &parsed);
+    mavlink_msg_gimbal_report_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_log_request_data(const mavlink_message_t* message)
+cStruct* unbox_hwstatus(const mavlink_message_t* message)
 {
-    static mavlink_log_request_data_t parsed;
+    static mavlink_hwstatus_t parsed;
 
     static cMember members[] = {
-        { "ofs", &(parsed.ofs), 1, UINT32_T},
-        { "count", &(parsed.count), 1, UINT32_T},
-        { "id", &(parsed.id), 1, UINT16_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T}
+        { "Vcc", &(parsed.Vcc), 1, UINT16_T},
+        { "I2Cerr", &(parsed.I2Cerr), 1, UINT8_T}
     };
-    static cStruct record = {"log_request_data", members, 5, 119};
+    static cStruct record = {"hwstatus", members, 2, 165};
 
-    mavlink_msg_log_request_data_decode(message, &parsed);
+    mavlink_msg_hwstatus_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_param_ext_request_read(const mavlink_message_t* message)
+cStruct* unbox_vision_position_delta(const mavlink_message_t* message)
 {
-    static mavlink_param_ext_request_read_t parsed;
+    static mavlink_vision_position_delta_t parsed;
 
     static cMember members[] = {
-        { "param_index", &(parsed.param_index), 1, INT16_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "param_id", &(parsed.param_id), 16, CHAR}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "time_delta_usec", &(parsed.time_delta_usec), 1, UINT64_T},
+        { "angle_delta", &(parsed.angle_delta), 3, FLOAT},
+        { "position_delta", &(parsed.position_delta), 3, FLOAT},
+        { "confidence", &(parsed.confidence), 1, FLOAT}
     };
-    static cStruct record = {"param_ext_request_read", members, 4, 320};
+    static cStruct record = {"vision_position_delta", members, 5, 11011};
 
-    mavlink_msg_param_ext_request_read_decode(message, &parsed);
+    mavlink_msg_vision_position_delta_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_system_time(const mavlink_message_t* message)
+cStruct* unbox_osd_param_config(const mavlink_message_t* message)
 {
-    static mavlink_system_time_t parsed;
+    static mavlink_osd_param_config_t parsed;
 
     static cMember members[] = {
-        { "time_unix_usec", &(parsed.time_unix_usec), 1, UINT64_T},
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T}
+        { "request_id", &(parsed.request_id), 1, UINT32_T},
+        { "min_value", &(parsed.min_value), 1, FLOAT},
+        { "max_value", &(parsed.max_value), 1, FLOAT},
+        { "increment", &(parsed.increment), 1, FLOAT},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "osd_screen", &(parsed.osd_screen), 1, UINT8_T},
+        { "osd_index", &(parsed.osd_index), 1, UINT8_T},
+        { "param_id", &(parsed.param_id), 16, CHAR},
+        { "config_type", &(parsed.config_type), 1, UINT8_T}
     };
-    static cStruct record = {"system_time", members, 2, 2};
+    static cStruct record = {"osd_param_config", members, 10, 11033};
 
-    mavlink_msg_system_time_decode(message, &parsed);
+    mavlink_msg_osd_param_config_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_component_information(const mavlink_message_t* message)
+cStruct* unbox_led_control(const mavlink_message_t* message)
 {
-    static mavlink_component_information_t parsed;
+    static mavlink_led_control_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "general_metadata_file_crc", &(parsed.general_metadata_file_crc), 1, UINT32_T},
-        { "peripherals_metadata_file_crc", &(parsed.peripherals_metadata_file_crc), 1, UINT32_T},
-        { "general_metadata_uri", &(parsed.general_metadata_uri), 100, CHAR},
-        { "peripherals_metadata_uri", &(parsed.peripherals_metadata_uri), 100, CHAR}
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "instance", &(parsed.instance), 1, UINT8_T},
+        { "pattern", &(parsed.pattern), 1, UINT8_T},
+        { "custom_len", &(parsed.custom_len), 1, UINT8_T},
+        { "custom_bytes", &(parsed.custom_bytes), 24, UINT8_T}
     };
-    static cStruct record = {"component_information", members, 5, 395};
+    static cStruct record = {"led_control", members, 6, 186};
 
-    mavlink_msg_component_information_decode(message, &parsed);
+    mavlink_msg_led_control_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_global_vision_position_estimate(const mavlink_message_t* message)
+cStruct* unbox_data64(const mavlink_message_t* message)
 {
-    static mavlink_global_vision_position_estimate_t parsed;
+    static mavlink_data64_t parsed;
 
     static cMember members[] = {
-        { "usec", &(parsed.usec), 1, UINT64_T},
-        { "x", &(parsed.x), 1, FLOAT},
-        { "y", &(parsed.y), 1, FLOAT},
-        { "z", &(parsed.z), 1, FLOAT},
-        { "roll", &(parsed.roll), 1, FLOAT},
-        { "pitch", &(parsed.pitch), 1, FLOAT},
-        { "yaw", &(parsed.yaw), 1, FLOAT},
-        { "covariance", &(parsed.covariance), 21, FLOAT},
-        { "reset_counter", &(parsed.reset_counter), 1, UINT8_T}
+        { "type", &(parsed.type), 1, UINT8_T},
+        { "len", &(parsed.len), 1, UINT8_T},
+        { "data", &(parsed.data), 64, UINT8_T}
     };
-    static cStruct record = {"global_vision_position_estimate", members, 9, 101};
+    static cStruct record = {"data64", members, 3, 171};
 
-    mavlink_msg_global_vision_position_estimate_decode(message, &parsed);
+    mavlink_msg_data64_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_open_drone_id_message_pack(const mavlink_message_t* message)
+cStruct* unbox_battery2(const mavlink_message_t* message)
 {
-    static mavlink_open_drone_id_message_pack_t parsed;
+    static mavlink_battery2_t parsed;
 
     static cMember members[] = {
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "id_or_mac", &(parsed.id_or_mac), 20, UINT8_T},
-        { "single_message_size", &(parsed.single_message_size), 1, UINT8_T},
-        { "msg_pack_size", &(parsed.msg_pack_size), 1, UINT8_T},
-        { "messages", &(parsed.messages), 225, UINT8_T}
+        { "voltage", &(parsed.voltage), 1, UINT16_T},
+        { "current_battery", &(parsed.current_battery), 1, INT16_T}
     };
-    static cStruct record = {"open_drone_id_message_pack", members, 6, 12915};
+    static cStruct record = {"battery2", members, 2, 181};
 
-    mavlink_msg_open_drone_id_message_pack_decode(message, &parsed);
+    mavlink_msg_battery2_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_generator_status(const mavlink_message_t* message)
+cStruct* unbox_rally_point(const mavlink_message_t* message)
 {
-    static mavlink_generator_status_t parsed;
+    static mavlink_rally_point_t parsed;
 
     static cMember members[] = {
-        { "status", &(parsed.status), 1, UINT64_T},
-        { "battery_current", &(parsed.battery_current), 1, FLOAT},
-        { "load_current", &(parsed.load_current), 1, FLOAT},
-        { "power_generated", &(parsed.power_generated), 1, FLOAT},
-        { "bus_voltage", &(parsed.bus_voltage), 1, FLOAT},
-        { "bat_current_setpoint", &(parsed.bat_current_setpoint), 1, FLOAT},
-        { "runtime", &(parsed.runtime), 1, UINT32_T},
-        { "time_until_maintenance", &(parsed.time_until_maintenance), 1, INT32_T},
-        { "generator_speed", &(parsed.generator_speed), 1, UINT16_T},
-        { "rectifier_temperature", &(parsed.rectifier_temperature), 1, INT16_T},
-        { "generator_temperature", &(parsed.generator_temperature), 1, INT16_T}
+        { "lat", &(parsed.lat), 1, INT32_T},
+        { "lng", &(parsed.lng), 1, INT32_T},
+        { "alt", &(parsed.alt), 1, INT16_T},
+        { "break_alt", &(parsed.break_alt), 1, INT16_T},
+        { "land_dir", &(parsed.land_dir), 1, UINT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "idx", &(parsed.idx), 1, UINT8_T},
+        { "count", &(parsed.count), 1, UINT8_T},
+        { "flags", &(parsed.flags), 1, UINT8_T}
     };
-    static cStruct record = {"generator_status", members, 11, 373};
+    static cStruct record = {"rally_point", members, 10, 175};
 
-    mavlink_msg_generator_status_decode(message, &parsed);
+    mavlink_msg_rally_point_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_smart_battery_info(const mavlink_message_t* message)
+cStruct* unbox_aoa_ssa(const mavlink_message_t* message)
 {
-    static mavlink_smart_battery_info_t parsed;
+    static mavlink_aoa_ssa_t parsed;
 
     static cMember members[] = {
-        { "capacity_full_specification", &(parsed.capacity_full_specification), 1, INT32_T},
-        { "capacity_full", &(parsed.capacity_full), 1, INT32_T},
-        { "cycle_count", &(parsed.cycle_count), 1, UINT16_T},
-        { "weight", &(parsed.weight), 1, UINT16_T},
-        { "discharge_minimum_voltage", &(parsed.discharge_minimum_voltage), 1, UINT16_T},
-        { "charging_minimum_voltage", &(parsed.charging_minimum_voltage), 1, UINT16_T},
-        { "resting_minimum_voltage", &(parsed.resting_minimum_voltage), 1, UINT16_T},
-        { "id", &(parsed.id), 1, UINT8_T},
-        { "battery_function", &(parsed.battery_function), 1, UINT8_T},
-        { "type", &(parsed.type), 1, UINT8_T},
-        { "serial_number", &(parsed.serial_number), 16, CHAR},
-        { "device_name", &(parsed.device_name), 50, CHAR},
-        { "charging_maximum_voltage", &(parsed.charging_maximum_voltage), 1, UINT16_T},
-        { "cells_in_series", &(parsed.cells_in_series), 1, UINT8_T},
-        { "discharge_maximum_current", &(parsed.discharge_maximum_current), 1, UINT32_T},
-        { "discharge_maximum_burst_current", &(parsed.discharge_maximum_burst_current), 1, UINT32_T},
-        { "manufacture_date", &(parsed.manufacture_date), 11, CHAR}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "AOA", &(parsed.AOA), 1, FLOAT},
+        { "SSA", &(parsed.SSA), 1, FLOAT}
     };
-    static cStruct record = {"smart_battery_info", members, 17, 370};
+    static cStruct record = {"aoa_ssa", members, 3, 11020};
 
-    mavlink_msg_smart_battery_info_decode(message, &parsed);
+    mavlink_msg_aoa_ssa_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_esc_status(const mavlink_message_t* message)
+cStruct* unbox_deepstall(const mavlink_message_t* message)
 {
-    static mavlink_esc_status_t parsed;
+    static mavlink_deepstall_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "rpm", &(parsed.rpm), 4, INT32_T},
-        { "voltage", &(parsed.voltage), 4, FLOAT},
-        { "current", &(parsed.current), 4, FLOAT},
-        { "index", &(parsed.index), 1, UINT8_T}
+        { "landing_lat", &(parsed.landing_lat), 1, INT32_T},
+        { "landing_lon", &(parsed.landing_lon), 1, INT32_T},
+        { "path_lat", &(parsed.path_lat), 1, INT32_T},
+        { "path_lon", &(parsed.path_lon), 1, INT32_T},
+        { "arc_entry_lat", &(parsed.arc_entry_lat), 1, INT32_T},
+        { "arc_entry_lon", &(parsed.arc_entry_lon), 1, INT32_T},
+        { "altitude", &(parsed.altitude), 1, FLOAT},
+        { "expected_travel_distance", &(parsed.expected_travel_distance), 1, FLOAT},
+        { "cross_track_error", &(parsed.cross_track_error), 1, FLOAT},
+        { "stage", &(parsed.stage), 1, UINT8_T}
     };
-    static cStruct record = {"esc_status", members, 5, 291};
+    static cStruct record = {"deepstall", members, 10, 195};
 
-    mavlink_msg_esc_status_decode(message, &parsed);
+    mavlink_msg_deepstall_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_battery_status(const mavlink_message_t* message)
+cStruct* unbox_digicam_configure(const mavlink_message_t* message)
 {
-    static mavlink_battery_status_t parsed;
+    static mavlink_digicam_configure_t parsed;
 
     static cMember members[] = {
-        { "current_consumed", &(parsed.current_consumed), 1, INT32_T},
-        { "energy_consumed", &(parsed.energy_consumed), 1, INT32_T},
-        { "temperature", &(parsed.temperature), 1, INT16_T},
-        { "voltages", &(parsed.voltages), 10, UINT16_T},
-        { "current_battery", &(parsed.current_battery), 1, INT16_T},
-        { "id", &(parsed.id), 1, UINT8_T},
-        { "battery_function", &(parsed.battery_function), 1, UINT8_T},
-        { "type", &(parsed.type), 1, UINT8_T},
-        { "battery_remaining", &(parsed.battery_remaining), 1, INT8_T},
-        { "time_remaining", &(parsed.time_remaining), 1, INT32_T},
-        { "charge_state", &(parsed.charge_state), 1, UINT8_T},
-        { "voltages_ext", &(parsed.voltages_ext), 4, UINT16_T},
+        { "extra_value", &(parsed.extra_value), 1, FLOAT},
+        { "shutter_speed", &(parsed.shutter_speed), 1, UINT16_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
         { "mode", &(parsed.mode), 1, UINT8_T},
-        { "fault_bitmask", &(parsed.fault_bitmask), 1, UINT32_T}
+        { "aperture", &(parsed.aperture), 1, UINT8_T},
+        { "iso", &(parsed.iso), 1, UINT8_T},
+        { "exposure_type", &(parsed.exposure_type), 1, UINT8_T},
+        { "command_id", &(parsed.command_id), 1, UINT8_T},
+        { "engine_cut_off", &(parsed.engine_cut_off), 1, UINT8_T},
+        { "extra_param", &(parsed.extra_param), 1, UINT8_T}
     };
-    static cStruct record = {"battery_status", members, 14, 147};
+    static cStruct record = {"digicam_configure", members, 11, 154};
 
-    mavlink_msg_battery_status_decode(message, &parsed);
+    mavlink_msg_digicam_configure_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_ping(const mavlink_message_t* message)
+cStruct* unbox_remote_log_block_status(const mavlink_message_t* message)
 {
-    static mavlink_ping_t parsed;
+    static mavlink_remote_log_block_status_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "seq", &(parsed.seq), 1, UINT32_T},
+        { "seqno", &(parsed.seqno), 1, UINT32_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T}
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "status", &(parsed.status), 1, UINT8_T}
     };
-    static cStruct record = {"ping", members, 4, 4};
+    static cStruct record = {"remote_log_block_status", members, 4, 185};
 
-    mavlink_msg_ping_decode(message, &parsed);
+    mavlink_msg_remote_log_block_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_estimator_status(const mavlink_message_t* message)
+cStruct* unbox_data16(const mavlink_message_t* message)
 {
-    static mavlink_estimator_status_t parsed;
+    static mavlink_data16_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "vel_ratio", &(parsed.vel_ratio), 1, FLOAT},
-        { "pos_horiz_ratio", &(parsed.pos_horiz_ratio), 1, FLOAT},
-        { "pos_vert_ratio", &(parsed.pos_vert_ratio), 1, FLOAT},
-        { "mag_ratio", &(parsed.mag_ratio), 1, FLOAT},
-        { "hagl_ratio", &(parsed.hagl_ratio), 1, FLOAT},
-        { "tas_ratio", &(parsed.tas_ratio), 1, FLOAT},
-        { "pos_horiz_accuracy", &(parsed.pos_horiz_accuracy), 1, FLOAT},
-        { "pos_vert_accuracy", &(parsed.pos_vert_accuracy), 1, FLOAT},
-        { "flags", &(parsed.flags), 1, UINT16_T}
+        { "type", &(parsed.type), 1, UINT8_T},
+        { "len", &(parsed.len), 1, UINT8_T},
+        { "data", &(parsed.data), 16, UINT8_T}
     };
-    static cStruct record = {"estimator_status", members, 10, 230};
+    static cStruct record = {"data16", members, 3, 169};
 
-    mavlink_msg_estimator_status_decode(message, &parsed);
+    mavlink_msg_data16_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_log_erase(const mavlink_message_t* message)
+cStruct* unbox_autopilot_version_request(const mavlink_message_t* message)
 {
-    static mavlink_log_erase_t parsed;
+    static mavlink_autopilot_version_request_t parsed;
 
     static cMember members[] = {
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T}
     };
-    static cStruct record = {"log_erase", members, 2, 121};
+    static cStruct record = {"autopilot_version_request", members, 2, 183};
 
-    mavlink_msg_log_erase_decode(message, &parsed);
+    mavlink_msg_autopilot_version_request_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_button_change(const mavlink_message_t* message)
+cStruct* unbox_esc_telemetry_9_to_12(const mavlink_message_t* message)
 {
-    static mavlink_button_change_t parsed;
+    static mavlink_esc_telemetry_9_to_12_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "last_change_ms", &(parsed.last_change_ms), 1, UINT32_T},
-        { "state", &(parsed.state), 1, UINT8_T}
+        { "voltage", &(parsed.voltage), 4, UINT16_T},
+        { "current", &(parsed.current), 4, UINT16_T},
+        { "totalcurrent", &(parsed.totalcurrent), 4, UINT16_T},
+        { "rpm", &(parsed.rpm), 4, UINT16_T},
+        { "count", &(parsed.count), 4, UINT16_T},
+        { "temperature", &(parsed.temperature), 4, UINT8_T}
     };
-    static cStruct record = {"button_change", members, 3, 257};
+    static cStruct record = {"esc_telemetry_9_to_12", members, 6, 11032};
 
-    mavlink_msg_button_change_decode(message, &parsed);
+    mavlink_msg_esc_telemetry_9_to_12_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_data_stream(const mavlink_message_t* message)
+cStruct* unbox_fence_point(const mavlink_message_t* message)
 {
-    static mavlink_data_stream_t parsed;
+    static mavlink_fence_point_t parsed;
 
     static cMember members[] = {
-        { "message_rate", &(parsed.message_rate), 1, UINT16_T},
-        { "stream_id", &(parsed.stream_id), 1, UINT8_T},
-        { "on_off", &(parsed.on_off), 1, UINT8_T}
+        { "lat", &(parsed.lat), 1, FLOAT},
+        { "lng", &(parsed.lng), 1, FLOAT},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "idx", &(parsed.idx), 1, UINT8_T},
+        { "count", &(parsed.count), 1, UINT8_T}
     };
-    static cStruct record = {"data_stream", members, 3, 67};
+    static cStruct record = {"fence_point", members, 6, 160};
 
-    mavlink_msg_data_stream_decode(message, &parsed);
+    mavlink_msg_fence_point_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_set_mode(const mavlink_message_t* message)
+cStruct* unbox_compassmot_status(const mavlink_message_t* message)
 {
-    static mavlink_set_mode_t parsed;
+    static mavlink_compassmot_status_t parsed;
 
     static cMember members[] = {
-        { "custom_mode", &(parsed.custom_mode), 1, UINT32_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "base_mode", &(parsed.base_mode), 1, UINT8_T}
+        { "current", &(parsed.current), 1, FLOAT},
+        { "CompensationX", &(parsed.CompensationX), 1, FLOAT},
+        { "CompensationY", &(parsed.CompensationY), 1, FLOAT},
+        { "CompensationZ", &(parsed.CompensationZ), 1, FLOAT},
+        { "throttle", &(parsed.throttle), 1, UINT16_T},
+        { "interference", &(parsed.interference), 1, UINT16_T}
     };
-    static cStruct record = {"set_mode", members, 3, 11};
+    static cStruct record = {"compassmot_status", members, 6, 177};
 
-    mavlink_msg_set_mode_decode(message, &parsed);
+    mavlink_msg_compassmot_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_gps_status(const mavlink_message_t* message)
+cStruct* unbox_gopro_get_response(const mavlink_message_t* message)
 {
-    static mavlink_gps_status_t parsed;
+    static mavlink_gopro_get_response_t parsed;
 
     static cMember members[] = {
-        { "satellites_visible", &(parsed.satellites_visible), 1, UINT8_T},
-        { "satellite_prn", &(parsed.satellite_prn), 20, UINT8_T},
-        { "satellite_used", &(parsed.satellite_used), 20, UINT8_T},
-        { "satellite_elevation", &(parsed.satellite_elevation), 20, UINT8_T},
-        { "satellite_azimuth", &(parsed.satellite_azimuth), 20, UINT8_T},
-        { "satellite_snr", &(parsed.satellite_snr), 20, UINT8_T}
+        { "cmd_id", &(parsed.cmd_id), 1, UINT8_T},
+        { "status", &(parsed.status), 1, UINT8_T},
+        { "value", &(parsed.value), 4, UINT8_T}
     };
-    static cStruct record = {"gps_status", members, 6, 25};
+    static cStruct record = {"gopro_get_response", members, 3, 217};
 
-    mavlink_msg_gps_status_decode(message, &parsed);
+    mavlink_msg_gopro_get_response_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_attitude_quaternion(const mavlink_message_t* message)
+cStruct* unbox_mount_status(const mavlink_message_t* message)
 {
-    static mavlink_attitude_quaternion_t parsed;
+    static mavlink_mount_status_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "q1", &(parsed.q1), 1, FLOAT},
-        { "q2", &(parsed.q2), 1, FLOAT},
-        { "q3", &(parsed.q3), 1, FLOAT},
-        { "q4", &(parsed.q4), 1, FLOAT},
-        { "rollspeed", &(parsed.rollspeed), 1, FLOAT},
-        { "pitchspeed", &(parsed.pitchspeed), 1, FLOAT},
-        { "yawspeed", &(parsed.yawspeed), 1, FLOAT},
-        { "repr_offset_q", &(parsed.repr_offset_q), 4, FLOAT}
+        { "pointing_a", &(parsed.pointing_a), 1, INT32_T},
+        { "pointing_b", &(parsed.pointing_b), 1, INT32_T},
+        { "pointing_c", &(parsed.pointing_c), 1, INT32_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "mount_mode", &(parsed.mount_mode), 1, UINT8_T}
     };
-    static cStruct record = {"attitude_quaternion", members, 9, 31};
+    static cStruct record = {"mount_status", members, 6, 158};
 
-    mavlink_msg_attitude_quaternion_decode(message, &parsed);
+    mavlink_msg_mount_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_current_event_sequence(const mavlink_message_t* message)
+cStruct* unbox_radio(const mavlink_message_t* message)
 {
-    static mavlink_current_event_sequence_t parsed;
+    static mavlink_radio_t parsed;
 
     static cMember members[] = {
-        { "sequence", &(parsed.sequence), 1, UINT16_T},
-        { "flags", &(parsed.flags), 1, UINT8_T}
+        { "rxerrors", &(parsed.rxerrors), 1, UINT16_T},
+        { "fixed", &(parsed.fixed), 1, UINT16_T},
+        { "rssi", &(parsed.rssi), 1, UINT8_T},
+        { "remrssi", &(parsed.remrssi), 1, UINT8_T},
+        { "txbuf", &(parsed.txbuf), 1, UINT8_T},
+        { "noise", &(parsed.noise), 1, UINT8_T},
+        { "remnoise", &(parsed.remnoise), 1, UINT8_T}
     };
-    static cStruct record = {"current_event_sequence", members, 2, 411};
+    static cStruct record = {"radio", members, 7, 166};
 
-    mavlink_msg_current_event_sequence_decode(message, &parsed);
+    mavlink_msg_radio_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_open_drone_id_self_id(const mavlink_message_t* message)
+cStruct* unbox_osd_param_config_reply(const mavlink_message_t* message)
 {
-    static mavlink_open_drone_id_self_id_t parsed;
+    static mavlink_osd_param_config_reply_t parsed;
 
     static cMember members[] = {
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "id_or_mac", &(parsed.id_or_mac), 20, UINT8_T},
-        { "description_type", &(parsed.description_type), 1, UINT8_T},
-        { "description", &(parsed.description), 23, CHAR}
+        { "request_id", &(parsed.request_id), 1, UINT32_T},
+        { "result", &(parsed.result), 1, UINT8_T}
     };
-    static cStruct record = {"open_drone_id_self_id", members, 5, 12903};
+    static cStruct record = {"osd_param_config_reply", members, 2, 11034};
 
-    mavlink_msg_open_drone_id_self_id_decode(message, &parsed);
+    mavlink_msg_osd_param_config_reply_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_set_home_position(const mavlink_message_t* message)
+cStruct* unbox_remote_log_data_block(const mavlink_message_t* message)
 {
-    static mavlink_set_home_position_t parsed;
+    static mavlink_remote_log_data_block_t parsed;
 
     static cMember members[] = {
-        { "latitude", &(parsed.latitude), 1, INT32_T},
-        { "longitude", &(parsed.longitude), 1, INT32_T},
-        { "altitude", &(parsed.altitude), 1, INT32_T},
-        { "x", &(parsed.x), 1, FLOAT},
-        { "y", &(parsed.y), 1, FLOAT},
-        { "z", &(parsed.z), 1, FLOAT},
-        { "q", &(parsed.q), 4, FLOAT},
-        { "approach_x", &(parsed.approach_x), 1, FLOAT},
-        { "approach_y", &(parsed.approach_y), 1, FLOAT},
-        { "approach_z", &(parsed.approach_z), 1, FLOAT},
+        { "seqno", &(parsed.seqno), 1, UINT32_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T}
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "data", &(parsed.data), 200, UINT8_T}
     };
-    static cStruct record = {"set_home_position", members, 12, 243};
+    static cStruct record = {"remote_log_data_block", members, 4, 184};
 
-    mavlink_msg_set_home_position_decode(message, &parsed);
+    mavlink_msg_remote_log_data_block_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_gps_input(const mavlink_message_t* message)
+cStruct* unbox_digicam_control(const mavlink_message_t* message)
 {
-    static mavlink_gps_input_t parsed;
+    static mavlink_digicam_control_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "time_week_ms", &(parsed.time_week_ms), 1, UINT32_T},
-        { "lat", &(parsed.lat), 1, INT32_T},
-        { "lon", &(parsed.lon), 1, INT32_T},
-        { "alt", &(parsed.alt), 1, FLOAT},
-        { "hdop", &(parsed.hdop), 1, FLOAT},
-        { "vdop", &(parsed.vdop), 1, FLOAT},
-        { "vn", &(parsed.vn), 1, FLOAT},
-        { "ve", &(parsed.ve), 1, FLOAT},
-        { "vd", &(parsed.vd), 1, FLOAT},
-        { "speed_accuracy", &(parsed.speed_accuracy), 1, FLOAT},
-        { "horiz_accuracy", &(parsed.horiz_accuracy), 1, FLOAT},
-        { "vert_accuracy", &(parsed.vert_accuracy), 1, FLOAT},
-        { "ignore_flags", &(parsed.ignore_flags), 1, UINT16_T},
-        { "time_week", &(parsed.time_week), 1, UINT16_T},
-        { "gps_id", &(parsed.gps_id), 1, UINT8_T},
-        { "fix_type", &(parsed.fix_type), 1, UINT8_T},
-        { "satellites_visible", &(parsed.satellites_visible), 1, UINT8_T},
-        { "yaw", &(parsed.yaw), 1, UINT16_T}
+        { "extra_value", &(parsed.extra_value), 1, FLOAT},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "session", &(parsed.session), 1, UINT8_T},
+        { "zoom_pos", &(parsed.zoom_pos), 1, UINT8_T},
+        { "zoom_step", &(parsed.zoom_step), 1, INT8_T},
+        { "focus_lock", &(parsed.focus_lock), 1, UINT8_T},
+        { "shot", &(parsed.shot), 1, UINT8_T},
+        { "command_id", &(parsed.command_id), 1, UINT8_T},
+        { "extra_param", &(parsed.extra_param), 1, UINT8_T}
     };
-    static cStruct record = {"gps_input", members, 19, 232};
+    static cStruct record = {"digicam_control", members, 10, 155};
 
-    mavlink_msg_gps_input_decode(message, &parsed);
+    mavlink_msg_digicam_control_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_hil_state_quaternion(const mavlink_message_t* message)
+cStruct* unbox_water_depth(const mavlink_message_t* message)
 {
-    static mavlink_hil_state_quaternion_t parsed;
+    static mavlink_water_depth_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "attitude_quaternion", &(parsed.attitude_quaternion), 4, FLOAT},
-        { "rollspeed", &(parsed.rollspeed), 1, FLOAT},
-        { "pitchspeed", &(parsed.pitchspeed), 1, FLOAT},
-        { "yawspeed", &(parsed.yawspeed), 1, FLOAT},
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
         { "lat", &(parsed.lat), 1, INT32_T},
-        { "lon", &(parsed.lon), 1, INT32_T},
-        { "alt", &(parsed.alt), 1, INT32_T},
-        { "vx", &(parsed.vx), 1, INT16_T},
-        { "vy", &(parsed.vy), 1, INT16_T},
-        { "vz", &(parsed.vz), 1, INT16_T},
-        { "ind_airspeed", &(parsed.ind_airspeed), 1, UINT16_T},
-        { "true_airspeed", &(parsed.true_airspeed), 1, UINT16_T},
-        { "xacc", &(parsed.xacc), 1, INT16_T},
-        { "yacc", &(parsed.yacc), 1, INT16_T},
-        { "zacc", &(parsed.zacc), 1, INT16_T}
+        { "lng", &(parsed.lng), 1, INT32_T},
+        { "alt", &(parsed.alt), 1, FLOAT},
+        { "roll", &(parsed.roll), 1, FLOAT},
+        { "pitch", &(parsed.pitch), 1, FLOAT},
+        { "yaw", &(parsed.yaw), 1, FLOAT},
+        { "distance", &(parsed.distance), 1, FLOAT},
+        { "temperature", &(parsed.temperature), 1, FLOAT},
+        { "id", &(parsed.id), 1, UINT8_T},
+        { "healthy", &(parsed.healthy), 1, UINT8_T}
     };
-    static cStruct record = {"hil_state_quaternion", members, 16, 115};
+    static cStruct record = {"water_depth", members, 11, 11038};
 
-    mavlink_msg_hil_state_quaternion_decode(message, &parsed);
+    mavlink_msg_water_depth_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_open_drone_id_location(const mavlink_message_t* message)
+cStruct* unbox_mount_configure(const mavlink_message_t* message)
 {
-    static mavlink_open_drone_id_location_t parsed;
+    static mavlink_mount_configure_t parsed;
 
     static cMember members[] = {
-        { "latitude", &(parsed.latitude), 1, INT32_T},
-        { "longitude", &(parsed.longitude), 1, INT32_T},
-        { "altitude_barometric", &(parsed.altitude_barometric), 1, FLOAT},
-        { "altitude_geodetic", &(parsed.altitude_geodetic), 1, FLOAT},
-        { "height", &(parsed.height), 1, FLOAT},
-        { "timestamp", &(parsed.timestamp), 1, FLOAT},
-        { "direction", &(parsed.direction), 1, UINT16_T},
-        { "speed_horizontal", &(parsed.speed_horizontal), 1, UINT16_T},
-        { "speed_vertical", &(parsed.speed_vertical), 1, INT16_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "id_or_mac", &(parsed.id_or_mac), 20, UINT8_T},
-        { "status", &(parsed.status), 1, UINT8_T},
-        { "height_reference", &(parsed.height_reference), 1, UINT8_T},
-        { "horizontal_accuracy", &(parsed.horizontal_accuracy), 1, UINT8_T},
-        { "vertical_accuracy", &(parsed.vertical_accuracy), 1, UINT8_T},
-        { "barometer_accuracy", &(parsed.barometer_accuracy), 1, UINT8_T},
-        { "speed_accuracy", &(parsed.speed_accuracy), 1, UINT8_T},
-        { "timestamp_accuracy", &(parsed.timestamp_accuracy), 1, UINT8_T}
+        { "mount_mode", &(parsed.mount_mode), 1, UINT8_T},
+        { "stab_roll", &(parsed.stab_roll), 1, UINT8_T},
+        { "stab_pitch", &(parsed.stab_pitch), 1, UINT8_T},
+        { "stab_yaw", &(parsed.stab_yaw), 1, UINT8_T}
     };
-    static cStruct record = {"open_drone_id_location", members, 19, 12901};
+    static cStruct record = {"mount_configure", members, 6, 156};
 
-    mavlink_msg_open_drone_id_location_decode(message, &parsed);
+    mavlink_msg_mount_configure_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_mission_request_list(const mavlink_message_t* message)
+cStruct* unbox_esc_telemetry_5_to_8(const mavlink_message_t* message)
 {
-    static mavlink_mission_request_list_t parsed;
+    static mavlink_esc_telemetry_5_to_8_t parsed;
 
     static cMember members[] = {
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "mission_type", &(parsed.mission_type), 1, UINT8_T}
+        { "voltage", &(parsed.voltage), 4, UINT16_T},
+        { "current", &(parsed.current), 4, UINT16_T},
+        { "totalcurrent", &(parsed.totalcurrent), 4, UINT16_T},
+        { "rpm", &(parsed.rpm), 4, UINT16_T},
+        { "count", &(parsed.count), 4, UINT16_T},
+        { "temperature", &(parsed.temperature), 4, UINT8_T}
     };
-    static cStruct record = {"mission_request_list", members, 3, 43};
+    static cStruct record = {"esc_telemetry_5_to_8", members, 6, 11031};
 
-    mavlink_msg_mission_request_list_decode(message, &parsed);
+    mavlink_msg_esc_telemetry_5_to_8_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_gimbal_manager_set_pitchyaw(const mavlink_message_t* message)
+cStruct* unbox_device_op_write(const mavlink_message_t* message)
 {
-    static mavlink_gimbal_manager_set_pitchyaw_t parsed;
+    static mavlink_device_op_write_t parsed;
 
     static cMember members[] = {
-        { "flags", &(parsed.flags), 1, UINT32_T},
-        { "pitch", &(parsed.pitch), 1, FLOAT},
-        { "yaw", &(parsed.yaw), 1, FLOAT},
-        { "pitch_rate", &(parsed.pitch_rate), 1, FLOAT},
-        { "yaw_rate", &(parsed.yaw_rate), 1, FLOAT},
+        { "request_id", &(parsed.request_id), 1, UINT32_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "gimbal_device_id", &(parsed.gimbal_device_id), 1, UINT8_T}
+        { "bustype", &(parsed.bustype), 1, UINT8_T},
+        { "bus", &(parsed.bus), 1, UINT8_T},
+        { "address", &(parsed.address), 1, UINT8_T},
+        { "busname", &(parsed.busname), 40, CHAR},
+        { "regstart", &(parsed.regstart), 1, UINT8_T},
+        { "count", &(parsed.count), 1, UINT8_T},
+        { "data", &(parsed.data), 128, UINT8_T},
+        { "bank", &(parsed.bank), 1, UINT8_T}
     };
-    static cStruct record = {"gimbal_manager_set_pitchyaw", members, 8, 287};
+    static cStruct record = {"device_op_write", members, 11, 11002};
 
-    mavlink_msg_gimbal_manager_set_pitchyaw_decode(message, &parsed);
+    mavlink_msg_device_op_write_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_power_status(const mavlink_message_t* message)
+cStruct* unbox_ap_adc(const mavlink_message_t* message)
 {
-    static mavlink_power_status_t parsed;
+    static mavlink_ap_adc_t parsed;
 
     static cMember members[] = {
-        { "Vcc", &(parsed.Vcc), 1, UINT16_T},
-        { "Vservo", &(parsed.Vservo), 1, UINT16_T},
-        { "flags", &(parsed.flags), 1, UINT16_T}
+        { "adc1", &(parsed.adc1), 1, UINT16_T},
+        { "adc2", &(parsed.adc2), 1, UINT16_T},
+        { "adc3", &(parsed.adc3), 1, UINT16_T},
+        { "adc4", &(parsed.adc4), 1, UINT16_T},
+        { "adc5", &(parsed.adc5), 1, UINT16_T},
+        { "adc6", &(parsed.adc6), 1, UINT16_T}
     };
-    static cStruct record = {"power_status", members, 3, 125};
+    static cStruct record = {"ap_adc", members, 6, 153};
 
-    mavlink_msg_power_status_decode(message, &parsed);
+    mavlink_msg_ap_adc_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_hil_optical_flow(const mavlink_message_t* message)
+cStruct* unbox_device_op_read(const mavlink_message_t* message)
 {
-    static mavlink_hil_optical_flow_t parsed;
+    static mavlink_device_op_read_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "integration_time_us", &(parsed.integration_time_us), 1, UINT32_T},
-        { "integrated_x", &(parsed.integrated_x), 1, FLOAT},
-        { "integrated_y", &(parsed.integrated_y), 1, FLOAT},
-        { "integrated_xgyro", &(parsed.integrated_xgyro), 1, FLOAT},
-        { "integrated_ygyro", &(parsed.integrated_ygyro), 1, FLOAT},
-        { "integrated_zgyro", &(parsed.integrated_zgyro), 1, FLOAT},
-        { "time_delta_distance_us", &(parsed.time_delta_distance_us), 1, UINT32_T},
-        { "distance", &(parsed.distance), 1, FLOAT},
-        { "temperature", &(parsed.temperature), 1, INT16_T},
-        { "sensor_id", &(parsed.sensor_id), 1, UINT8_T},
-        { "quality", &(parsed.quality), 1, UINT8_T}
+        { "request_id", &(parsed.request_id), 1, UINT32_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "bustype", &(parsed.bustype), 1, UINT8_T},
+        { "bus", &(parsed.bus), 1, UINT8_T},
+        { "address", &(parsed.address), 1, UINT8_T},
+        { "busname", &(parsed.busname), 40, CHAR},
+        { "regstart", &(parsed.regstart), 1, UINT8_T},
+        { "count", &(parsed.count), 1, UINT8_T},
+        { "bank", &(parsed.bank), 1, UINT8_T}
     };
-    static cStruct record = {"hil_optical_flow", members, 12, 114};
+    static cStruct record = {"device_op_read", members, 10, 11000};
 
-    mavlink_msg_hil_optical_flow_decode(message, &parsed);
+    mavlink_msg_device_op_read_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_resource_request(const mavlink_message_t* message)
+cStruct* unbox_simstate(const mavlink_message_t* message)
 {
-    static mavlink_resource_request_t parsed;
+    static mavlink_simstate_t parsed;
 
     static cMember members[] = {
-        { "request_id", &(parsed.request_id), 1, UINT8_T},
-        { "uri_type", &(parsed.uri_type), 1, UINT8_T},
-        { "uri", &(parsed.uri), 120, UINT8_T},
-        { "transfer_type", &(parsed.transfer_type), 1, UINT8_T},
-        { "storage", &(parsed.storage), 120, UINT8_T}
+        { "roll", &(parsed.roll), 1, FLOAT},
+        { "pitch", &(parsed.pitch), 1, FLOAT},
+        { "yaw", &(parsed.yaw), 1, FLOAT},
+        { "xacc", &(parsed.xacc), 1, FLOAT},
+        { "yacc", &(parsed.yacc), 1, FLOAT},
+        { "zacc", &(parsed.zacc), 1, FLOAT},
+        { "xgyro", &(parsed.xgyro), 1, FLOAT},
+        { "ygyro", &(parsed.ygyro), 1, FLOAT},
+        { "zgyro", &(parsed.zgyro), 1, FLOAT},
+        { "lat", &(parsed.lat), 1, INT32_T},
+        { "lng", &(parsed.lng), 1, INT32_T}
     };
-    static cStruct record = {"resource_request", members, 5, 142};
+    static cStruct record = {"simstate", members, 11, 164};
 
-    mavlink_msg_resource_request_decode(message, &parsed);
+    mavlink_msg_simstate_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_gimbal_manager_set_attitude(const mavlink_message_t* message)
+cStruct* unbox_rally_fetch_point(const mavlink_message_t* message)
 {
-    static mavlink_gimbal_manager_set_attitude_t parsed;
+    static mavlink_rally_fetch_point_t parsed;
 
     static cMember members[] = {
-        { "flags", &(parsed.flags), 1, UINT32_T},
-        { "q", &(parsed.q), 4, FLOAT},
-        { "angular_velocity_x", &(parsed.angular_velocity_x), 1, FLOAT},
-        { "angular_velocity_y", &(parsed.angular_velocity_y), 1, FLOAT},
-        { "angular_velocity_z", &(parsed.angular_velocity_z), 1, FLOAT},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "gimbal_device_id", &(parsed.gimbal_device_id), 1, UINT8_T}
+        { "idx", &(parsed.idx), 1, UINT8_T}
     };
-    static cStruct record = {"gimbal_manager_set_attitude", members, 8, 282};
+    static cStruct record = {"rally_fetch_point", members, 3, 176};
 
-    mavlink_msg_gimbal_manager_set_attitude_decode(message, &parsed);
+    mavlink_msg_rally_fetch_point_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_vicon_position_estimate(const mavlink_message_t* message)
+cStruct* unbox_esc_telemetry_1_to_4(const mavlink_message_t* message)
 {
-    static mavlink_vicon_position_estimate_t parsed;
+    static mavlink_esc_telemetry_1_to_4_t parsed;
 
     static cMember members[] = {
-        { "usec", &(parsed.usec), 1, UINT64_T},
-        { "x", &(parsed.x), 1, FLOAT},
-        { "y", &(parsed.y), 1, FLOAT},
-        { "z", &(parsed.z), 1, FLOAT},
-        { "roll", &(parsed.roll), 1, FLOAT},
-        { "pitch", &(parsed.pitch), 1, FLOAT},
-        { "yaw", &(parsed.yaw), 1, FLOAT},
-        { "covariance", &(parsed.covariance), 21, FLOAT}
+        { "voltage", &(parsed.voltage), 4, UINT16_T},
+        { "current", &(parsed.current), 4, UINT16_T},
+        { "totalcurrent", &(parsed.totalcurrent), 4, UINT16_T},
+        { "rpm", &(parsed.rpm), 4, UINT16_T},
+        { "count", &(parsed.count), 4, UINT16_T},
+        { "temperature", &(parsed.temperature), 4, UINT8_T}
     };
-    static cStruct record = {"vicon_position_estimate", members, 8, 104};
+    static cStruct record = {"esc_telemetry_1_to_4", members, 6, 11030};
 
-    mavlink_msg_vicon_position_estimate_decode(message, &parsed);
+    mavlink_msg_esc_telemetry_1_to_4_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_set_actuator_control_target(const mavlink_message_t* message)
+cStruct* unbox_adap_tuning(const mavlink_message_t* message)
 {
-    static mavlink_set_actuator_control_target_t parsed;
+    static mavlink_adap_tuning_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "controls", &(parsed.controls), 8, FLOAT},
-        { "group_mlx", &(parsed.group_mlx), 1, UINT8_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T}
+        { "desired", &(parsed.desired), 1, FLOAT},
+        { "achieved", &(parsed.achieved), 1, FLOAT},
+        { "error", &(parsed.error), 1, FLOAT},
+        { "theta", &(parsed.theta), 1, FLOAT},
+        { "omega", &(parsed.omega), 1, FLOAT},
+        { "sigma", &(parsed.sigma), 1, FLOAT},
+        { "theta_dot", &(parsed.theta_dot), 1, FLOAT},
+        { "omega_dot", &(parsed.omega_dot), 1, FLOAT},
+        { "sigma_dot", &(parsed.sigma_dot), 1, FLOAT},
+        { "f", &(parsed.f), 1, FLOAT},
+        { "f_dot", &(parsed.f_dot), 1, FLOAT},
+        { "u", &(parsed.u), 1, FLOAT},
+        { "axis", &(parsed.axis), 1, UINT8_T}
     };
-    static cStruct record = {"set_actuator_control_target", members, 5, 139};
+    static cStruct record = {"adap_tuning", members, 13, 11010};
 
-    mavlink_msg_set_actuator_control_target_decode(message, &parsed);
+    mavlink_msg_adap_tuning_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_message_interval(const mavlink_message_t* message)
+cStruct* unbox_gopro_heartbeat(const mavlink_message_t* message)
 {
-    static mavlink_message_interval_t parsed;
+    static mavlink_gopro_heartbeat_t parsed;
 
     static cMember members[] = {
-        { "interval_us", &(parsed.interval_us), 1, INT32_T},
-        { "message_id", &(parsed.message_id), 1, UINT16_T}
+        { "status", &(parsed.status), 1, UINT8_T},
+        { "capture_mode", &(parsed.capture_mode), 1, UINT8_T},
+        { "flags", &(parsed.flags), 1, UINT8_T}
     };
-    static cStruct record = {"message_interval", members, 2, 244};
+    static cStruct record = {"gopro_heartbeat", members, 3, 215};
 
-    mavlink_msg_message_interval_decode(message, &parsed);
+    mavlink_msg_gopro_heartbeat_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_mission_current(const mavlink_message_t* message)
+cStruct* unbox_airspeed_autocal(const mavlink_message_t* message)
 {
-    static mavlink_mission_current_t parsed;
+    static mavlink_airspeed_autocal_t parsed;
 
     static cMember members[] = {
-        { "seq", &(parsed.seq), 1, UINT16_T},
-        { "total", &(parsed.total), 1, UINT16_T},
-        { "mission_state", &(parsed.mission_state), 1, UINT8_T},
-        { "mission_mode", &(parsed.mission_mode), 1, UINT8_T}
+        { "vx", &(parsed.vx), 1, FLOAT},
+        { "vy", &(parsed.vy), 1, FLOAT},
+        { "vz", &(parsed.vz), 1, FLOAT},
+        { "diff_pressure", &(parsed.diff_pressure), 1, FLOAT},
+        { "EAS2TAS", &(parsed.EAS2TAS), 1, FLOAT},
+        { "ratio", &(parsed.ratio), 1, FLOAT},
+        { "state_x", &(parsed.state_x), 1, FLOAT},
+        { "state_y", &(parsed.state_y), 1, FLOAT},
+        { "state_z", &(parsed.state_z), 1, FLOAT},
+        { "Pax", &(parsed.Pax), 1, FLOAT},
+        { "Pby", &(parsed.Pby), 1, FLOAT},
+        { "Pcz", &(parsed.Pcz), 1, FLOAT}
     };
-    static cStruct record = {"mission_current", members, 4, 42};
+    static cStruct record = {"airspeed_autocal", members, 12, 174};
 
-    mavlink_msg_mission_current_decode(message, &parsed);
+    mavlink_msg_airspeed_autocal_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_scaled_imu(const mavlink_message_t* message)
+cStruct* unbox_osd_param_show_config_reply(const mavlink_message_t* message)
 {
-    static mavlink_scaled_imu_t parsed;
+    static mavlink_osd_param_show_config_reply_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "xacc", &(parsed.xacc), 1, INT16_T},
-        { "yacc", &(parsed.yacc), 1, INT16_T},
-        { "zacc", &(parsed.zacc), 1, INT16_T},
-        { "xgyro", &(parsed.xgyro), 1, INT16_T},
-        { "ygyro", &(parsed.ygyro), 1, INT16_T},
-        { "zgyro", &(parsed.zgyro), 1, INT16_T},
-        { "xmag", &(parsed.xmag), 1, INT16_T},
-        { "ymag", &(parsed.ymag), 1, INT16_T},
-        { "zmag", &(parsed.zmag), 1, INT16_T},
-        { "temperature", &(parsed.temperature), 1, INT16_T}
+        { "request_id", &(parsed.request_id), 1, UINT32_T},
+        { "min_value", &(parsed.min_value), 1, FLOAT},
+        { "max_value", &(parsed.max_value), 1, FLOAT},
+        { "increment", &(parsed.increment), 1, FLOAT},
+        { "result", &(parsed.result), 1, UINT8_T},
+        { "param_id", &(parsed.param_id), 16, CHAR},
+        { "config_type", &(parsed.config_type), 1, UINT8_T}
     };
-    static cStruct record = {"scaled_imu", members, 11, 26};
+    static cStruct record = {"osd_param_show_config_reply", members, 7, 11036};
 
-    mavlink_msg_scaled_imu_decode(message, &parsed);
+    mavlink_msg_osd_param_show_config_reply_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_set_position_target_local_ned(const mavlink_message_t* message)
+cStruct* unbox_gimbal_control(const mavlink_message_t* message)
 {
-    static mavlink_set_position_target_local_ned_t parsed;
+    static mavlink_gimbal_control_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "x", &(parsed.x), 1, FLOAT},
-        { "y", &(parsed.y), 1, FLOAT},
-        { "z", &(parsed.z), 1, FLOAT},
-        { "vx", &(parsed.vx), 1, FLOAT},
-        { "vy", &(parsed.vy), 1, FLOAT},
-        { "vz", &(parsed.vz), 1, FLOAT},
-        { "afx", &(parsed.afx), 1, FLOAT},
-        { "afy", &(parsed.afy), 1, FLOAT},
-        { "afz", &(parsed.afz), 1, FLOAT},
-        { "yaw", &(parsed.yaw), 1, FLOAT},
-        { "yaw_rate", &(parsed.yaw_rate), 1, FLOAT},
-        { "type_mask", &(parsed.type_mask), 1, UINT16_T},
+        { "demanded_rate_x", &(parsed.demanded_rate_x), 1, FLOAT},
+        { "demanded_rate_y", &(parsed.demanded_rate_y), 1, FLOAT},
+        { "demanded_rate_z", &(parsed.demanded_rate_z), 1, FLOAT},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "coordinate_frame", &(parsed.coordinate_frame), 1, UINT8_T}
+        { "target_component", &(parsed.target_component), 1, UINT8_T}
     };
-    static cStruct record = {"set_position_target_local_ned", members, 16, 84};
+    static cStruct record = {"gimbal_control", members, 5, 201};
 
-    mavlink_msg_set_position_target_local_ned_decode(message, &parsed);
+    mavlink_msg_gimbal_control_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_hil_actuator_controls(const mavlink_message_t* message)
+cStruct* unbox_mcu_status(const mavlink_message_t* message)
 {
-    static mavlink_hil_actuator_controls_t parsed;
+    static mavlink_mcu_status_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "flags", &(parsed.flags), 1, UINT64_T},
-        { "controls", &(parsed.controls), 16, FLOAT},
-        { "mode", &(parsed.mode), 1, UINT8_T}
+        { "MCU_temperature", &(parsed.MCU_temperature), 1, INT16_T},
+        { "MCU_voltage", &(parsed.MCU_voltage), 1, UINT16_T},
+        { "MCU_voltage_min", &(parsed.MCU_voltage_min), 1, UINT16_T},
+        { "MCU_voltage_max", &(parsed.MCU_voltage_max), 1, UINT16_T},
+        { "id", &(parsed.id), 1, UINT8_T}
     };
-    static cStruct record = {"hil_actuator_controls", members, 4, 93};
+    static cStruct record = {"mcu_status", members, 5, 11039};
 
-    mavlink_msg_hil_actuator_controls_decode(message, &parsed);
+    mavlink_msg_mcu_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_command_int(const mavlink_message_t* message)
+cStruct* unbox_cubepilot_firmware_update_resp(const mavlink_message_t* message)
 {
-    static mavlink_command_int_t parsed;
+    static mavlink_cubepilot_firmware_update_resp_t parsed;
 
     static cMember members[] = {
-        { "param1", &(parsed.param1), 1, FLOAT},
-        { "param2", &(parsed.param2), 1, FLOAT},
-        { "param3", &(parsed.param3), 1, FLOAT},
-        { "param4", &(parsed.param4), 1, FLOAT},
-        { "x", &(parsed.x), 1, INT32_T},
-        { "y", &(parsed.y), 1, INT32_T},
-        { "z", &(parsed.z), 1, FLOAT},
-        { "command", &(parsed.command), 1, UINT16_T},
+        { "offset", &(parsed.offset), 1, UINT32_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "frame", &(parsed.frame), 1, UINT8_T},
-        { "current", &(parsed.current), 1, UINT8_T},
-        { "autocontinue", &(parsed.autocontinue), 1, UINT8_T}
+        { "target_component", &(parsed.target_component), 1, UINT8_T}
     };
-    static cStruct record = {"command_int", members, 13, 75};
+    static cStruct record = {"cubepilot_firmware_update_resp", members, 3, 50005};
 
-    mavlink_msg_command_int_decode(message, &parsed);
+    mavlink_msg_cubepilot_firmware_update_resp_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_play_tune_v2(const mavlink_message_t* message)
+cStruct* unbox_cubepilot_raw_rc(const mavlink_message_t* message)
 {
-    static mavlink_play_tune_v2_t parsed;
+    static mavlink_cubepilot_raw_rc_t parsed;
 
     static cMember members[] = {
-        { "format", &(parsed.format), 1, UINT32_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "tune", &(parsed.tune), 248, CHAR}
+        { "rc_raw", &(parsed.rc_raw), 32, UINT8_T}
     };
-    static cStruct record = {"play_tune_v2", members, 4, 400};
+    static cStruct record = {"cubepilot_raw_rc", members, 1, 50001};
 
-    mavlink_msg_play_tune_v2_decode(message, &parsed);
+    mavlink_msg_cubepilot_raw_rc_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_mount_orientation(const mavlink_message_t* message)
+cStruct* unbox_herelink_video_stream_information(const mavlink_message_t* message)
 {
-    static mavlink_mount_orientation_t parsed;
+    static mavlink_herelink_video_stream_information_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "roll", &(parsed.roll), 1, FLOAT},
-        { "pitch", &(parsed.pitch), 1, FLOAT},
-        { "yaw", &(parsed.yaw), 1, FLOAT},
-        { "yaw_absolute", &(parsed.yaw_absolute), 1, FLOAT}
+        { "framerate", &(parsed.framerate), 1, FLOAT},
+        { "bitrate", &(parsed.bitrate), 1, UINT32_T},
+        { "resolution_h", &(parsed.resolution_h), 1, UINT16_T},
+        { "resolution_v", &(parsed.resolution_v), 1, UINT16_T},
+        { "rotation", &(parsed.rotation), 1, UINT16_T},
+        { "camera_id", &(parsed.camera_id), 1, UINT8_T},
+        { "status", &(parsed.status), 1, UINT8_T},
+        { "uri", &(parsed.uri), 230, CHAR}
     };
-    static cStruct record = {"mount_orientation", members, 5, 265};
+    static cStruct record = {"herelink_video_stream_information", members, 8, 50002};
 
-    mavlink_msg_mount_orientation_decode(message, &parsed);
+    mavlink_msg_herelink_video_stream_information_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_global_position_int(const mavlink_message_t* message)
+cStruct* unbox_herelink_telem(const mavlink_message_t* message)
 {
-    static mavlink_global_position_int_t parsed;
+    static mavlink_herelink_telem_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "lat", &(parsed.lat), 1, INT32_T},
-        { "lon", &(parsed.lon), 1, INT32_T},
-        { "alt", &(parsed.alt), 1, INT32_T},
-        { "relative_alt", &(parsed.relative_alt), 1, INT32_T},
-        { "vx", &(parsed.vx), 1, INT16_T},
-        { "vy", &(parsed.vy), 1, INT16_T},
-        { "vz", &(parsed.vz), 1, INT16_T},
-        { "hdg", &(parsed.hdg), 1, UINT16_T}
+        { "rf_freq", &(parsed.rf_freq), 1, UINT32_T},
+        { "link_bw", &(parsed.link_bw), 1, UINT32_T},
+        { "link_rate", &(parsed.link_rate), 1, UINT32_T},
+        { "snr", &(parsed.snr), 1, INT16_T},
+        { "cpu_temp", &(parsed.cpu_temp), 1, INT16_T},
+        { "board_temp", &(parsed.board_temp), 1, INT16_T},
+        { "rssi", &(parsed.rssi), 1, UINT8_T}
     };
-    static cStruct record = {"global_position_int", members, 9, 33};
+    static cStruct record = {"herelink_telem", members, 7, 50003};
 
-    mavlink_msg_global_position_int_decode(message, &parsed);
+    mavlink_msg_herelink_telem_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_gps_rtk(const mavlink_message_t* message)
+cStruct* unbox_cubepilot_firmware_update_start(const mavlink_message_t* message)
 {
-    static mavlink_gps_rtk_t parsed;
+    static mavlink_cubepilot_firmware_update_start_t parsed;
 
     static cMember members[] = {
-        { "time_last_baseline_ms", &(parsed.time_last_baseline_ms), 1, UINT32_T},
-        { "tow", &(parsed.tow), 1, UINT32_T},
-        { "baseline_a_mm", &(parsed.baseline_a_mm), 1, INT32_T},
-        { "baseline_b_mm", &(parsed.baseline_b_mm), 1, INT32_T},
-        { "baseline_c_mm", &(parsed.baseline_c_mm), 1, INT32_T},
-        { "accuracy", &(parsed.accuracy), 1, UINT32_T},
-        { "iar_num_hypotheses", &(parsed.iar_num_hypotheses), 1, INT32_T},
-        { "wn", &(parsed.wn), 1, UINT16_T},
-        { "rtk_receiver_id", &(parsed.rtk_receiver_id), 1, UINT8_T},
-        { "rtk_health", &(parsed.rtk_health), 1, UINT8_T},
-        { "rtk_rate", &(parsed.rtk_rate), 1, UINT8_T},
-        { "nsats", &(parsed.nsats), 1, UINT8_T},
-        { "baseline_coords_type", &(parsed.baseline_coords_type), 1, UINT8_T}
+        { "size", &(parsed.size), 1, UINT32_T},
+        { "crc", &(parsed.crc), 1, UINT32_T},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T}
     };
-    static cStruct record = {"gps_rtk", members, 13, 127};
+    static cStruct record = {"cubepilot_firmware_update_start", members, 4, 50004};
 
-    mavlink_msg_gps_rtk_decode(message, &parsed);
+    mavlink_msg_cubepilot_firmware_update_start_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_setup_signing(const mavlink_message_t* message)
+cStruct* unbox_nav_filter_bias(const mavlink_message_t* message)
 {
-    static mavlink_setup_signing_t parsed;
+    static mavlink_nav_filter_bias_t parsed;
 
     static cMember members[] = {
-        { "initial_timestamp", &(parsed.initial_timestamp), 1, UINT64_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "secret_key", &(parsed.secret_key), 32, UINT8_T}
+        { "usec", &(parsed.usec), 1, UINT64_T},
+        { "accel_0", &(parsed.accel_0), 1, FLOAT},
+        { "accel_1", &(parsed.accel_1), 1, FLOAT},
+        { "accel_2", &(parsed.accel_2), 1, FLOAT},
+        { "gyro_0", &(parsed.gyro_0), 1, FLOAT},
+        { "gyro_1", &(parsed.gyro_1), 1, FLOAT},
+        { "gyro_2", &(parsed.gyro_2), 1, FLOAT}
     };
-    static cStruct record = {"setup_signing", members, 4, 256};
+    static cStruct record = {"nav_filter_bias", members, 7, 220};
 
-    mavlink_msg_setup_signing_decode(message, &parsed);
+    mavlink_msg_nav_filter_bias_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_param_ext_ack(const mavlink_message_t* message)
+cStruct* unbox_ualberta_sys_status(const mavlink_message_t* message)
 {
-    static mavlink_param_ext_ack_t parsed;
+    static mavlink_ualberta_sys_status_t parsed;
 
     static cMember members[] = {
-        { "param_id", &(parsed.param_id), 16, CHAR},
-        { "param_value", &(parsed.param_value), 128, CHAR},
-        { "param_type", &(parsed.param_type), 1, UINT8_T},
-        { "param_result", &(parsed.param_result), 1, UINT8_T}
+        { "mode", &(parsed.mode), 1, UINT8_T},
+        { "nav_mode", &(parsed.nav_mode), 1, UINT8_T},
+        { "pilot", &(parsed.pilot), 1, UINT8_T}
     };
-    static cStruct record = {"param_ext_ack", members, 4, 324};
+    static cStruct record = {"ualberta_sys_status", members, 3, 222};
 
-    mavlink_msg_param_ext_ack_decode(message, &parsed);
+    mavlink_msg_ualberta_sys_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_winch_status(const mavlink_message_t* message)
+cStruct* unbox_radio_calibration(const mavlink_message_t* message)
 {
-    static mavlink_winch_status_t parsed;
+    static mavlink_radio_calibration_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "line_length", &(parsed.line_length), 1, FLOAT},
-        { "speed", &(parsed.speed), 1, FLOAT},
-        { "tension", &(parsed.tension), 1, FLOAT},
-        { "voltage", &(parsed.voltage), 1, FLOAT},
-        { "current", &(parsed.current), 1, FLOAT},
-        { "status", &(parsed.status), 1, UINT32_T},
-        { "temperature", &(parsed.temperature), 1, INT16_T}
+        { "aileron", &(parsed.aileron), 3, UINT16_T},
+        { "elevator", &(parsed.elevator), 3, UINT16_T},
+        { "rudder", &(parsed.rudder), 3, UINT16_T},
+        { "gyro", &(parsed.gyro), 2, UINT16_T},
+        { "pitch", &(parsed.pitch), 5, UINT16_T},
+        { "throttle", &(parsed.throttle), 5, UINT16_T}
     };
-    static cStruct record = {"winch_status", members, 8, 9005};
+    static cStruct record = {"radio_calibration", members, 6, 221};
 
-    mavlink_msg_winch_status_decode(message, &parsed);
+    mavlink_msg_radio_calibration_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_fence_status(const mavlink_message_t* message)
+cStruct* unbox_icarous_heartbeat(const mavlink_message_t* message)
 {
-    static mavlink_fence_status_t parsed;
+    static mavlink_icarous_heartbeat_t parsed;
 
     static cMember members[] = {
-        { "breach_time", &(parsed.breach_time), 1, UINT32_T},
-        { "breach_count", &(parsed.breach_count), 1, UINT16_T},
-        { "breach_status", &(parsed.breach_status), 1, UINT8_T},
-        { "breach_type", &(parsed.breach_type), 1, UINT8_T},
-        { "breach_mitigation", &(parsed.breach_mitigation), 1, UINT8_T}
+        { "status", &(parsed.status), 1, UINT8_T}
     };
-    static cStruct record = {"fence_status", members, 5, 162};
+    static cStruct record = {"icarous_heartbeat", members, 1, 42000};
 
-    mavlink_msg_fence_status_decode(message, &parsed);
+    mavlink_msg_icarous_heartbeat_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_auth_key(const mavlink_message_t* message)
+cStruct* unbox_icarous_kinematic_bands(const mavlink_message_t* message)
 {
-    static mavlink_auth_key_t parsed;
+    static mavlink_icarous_kinematic_bands_t parsed;
 
     static cMember members[] = {
-        { "key", &(parsed.key), 32, CHAR}
+        { "min1", &(parsed.min1), 1, FLOAT},
+        { "max1", &(parsed.max1), 1, FLOAT},
+        { "min2", &(parsed.min2), 1, FLOAT},
+        { "max2", &(parsed.max2), 1, FLOAT},
+        { "min3", &(parsed.min3), 1, FLOAT},
+        { "max3", &(parsed.max3), 1, FLOAT},
+        { "min4", &(parsed.min4), 1, FLOAT},
+        { "max4", &(parsed.max4), 1, FLOAT},
+        { "min5", &(parsed.min5), 1, FLOAT},
+        { "max5", &(parsed.max5), 1, FLOAT},
+        { "numBands", &(parsed.numBands), 1, INT8_T},
+        { "type1", &(parsed.type1), 1, UINT8_T},
+        { "type2", &(parsed.type2), 1, UINT8_T},
+        { "type3", &(parsed.type3), 1, UINT8_T},
+        { "type4", &(parsed.type4), 1, UINT8_T},
+        { "type5", &(parsed.type5), 1, UINT8_T}
     };
-    static cStruct record = {"auth_key", members, 1, 7};
+    static cStruct record = {"icarous_kinematic_bands", members, 16, 42001};
 
-    mavlink_msg_auth_key_decode(message, &parsed);
+    mavlink_msg_icarous_kinematic_bands_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_tunnel(const mavlink_message_t* message)
+cStruct* unbox_storm32_gimbal_manager_correct_roll(const mavlink_message_t* message)
 {
-    static mavlink_tunnel_t parsed;
+    static mavlink_storm32_gimbal_manager_correct_roll_t parsed;
 
     static cMember members[] = {
-        { "payload_type", &(parsed.payload_type), 1, UINT16_T},
+        { "roll", &(parsed.roll), 1, FLOAT},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "payload_length", &(parsed.payload_length), 1, UINT8_T},
-        { "payload", &(parsed.payload), 128, UINT8_T}
+        { "gimbal_id", &(parsed.gimbal_id), 1, UINT8_T},
+        { "client", &(parsed.client), 1, UINT8_T}
     };
-    static cStruct record = {"tunnel", members, 5, 385};
+    static cStruct record = {"storm32_gimbal_manager_correct_roll", members, 5, 60014};
 
-    mavlink_msg_tunnel_decode(message, &parsed);
+    mavlink_msg_storm32_gimbal_manager_correct_roll_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_optical_flow_rad(const mavlink_message_t* message)
+cStruct* unbox_frsky_passthrough_array(const mavlink_message_t* message)
 {
-    static mavlink_optical_flow_rad_t parsed;
+    static mavlink_frsky_passthrough_array_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "integration_time_us", &(parsed.integration_time_us), 1, UINT32_T},
-        { "integrated_x", &(parsed.integrated_x), 1, FLOAT},
-        { "integrated_y", &(parsed.integrated_y), 1, FLOAT},
-        { "integrated_xgyro", &(parsed.integrated_xgyro), 1, FLOAT},
-        { "integrated_ygyro", &(parsed.integrated_ygyro), 1, FLOAT},
-        { "integrated_zgyro", &(parsed.integrated_zgyro), 1, FLOAT},
-        { "time_delta_distance_us", &(parsed.time_delta_distance_us), 1, UINT32_T},
-        { "distance", &(parsed.distance), 1, FLOAT},
-        { "temperature", &(parsed.temperature), 1, INT16_T},
-        { "sensor_id", &(parsed.sensor_id), 1, UINT8_T},
-        { "quality", &(parsed.quality), 1, UINT8_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "count", &(parsed.count), 1, UINT8_T},
+        { "packet_buf", &(parsed.packet_buf), 240, UINT8_T}
     };
-    static cStruct record = {"optical_flow_rad", members, 12, 106};
+    static cStruct record = {"frsky_passthrough_array", members, 3, 60040};
 
-    mavlink_msg_optical_flow_rad_decode(message, &parsed);
+    mavlink_msg_frsky_passthrough_array_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_local_position_ned_system_global_offset(const mavlink_message_t* message)
+cStruct* unbox_storm32_gimbal_manager_information(const mavlink_message_t* message)
 {
-    static mavlink_local_position_ned_system_global_offset_t parsed;
+    static mavlink_storm32_gimbal_manager_information_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "x", &(parsed.x), 1, FLOAT},
-        { "y", &(parsed.y), 1, FLOAT},
-        { "z", &(parsed.z), 1, FLOAT},
-        { "roll", &(parsed.roll), 1, FLOAT},
-        { "pitch", &(parsed.pitch), 1, FLOAT},
-        { "yaw", &(parsed.yaw), 1, FLOAT}
+        { "device_cap_flags", &(parsed.device_cap_flags), 1, UINT32_T},
+        { "manager_cap_flags", &(parsed.manager_cap_flags), 1, UINT32_T},
+        { "roll_min", &(parsed.roll_min), 1, FLOAT},
+        { "roll_max", &(parsed.roll_max), 1, FLOAT},
+        { "pitch_min", &(parsed.pitch_min), 1, FLOAT},
+        { "pitch_max", &(parsed.pitch_max), 1, FLOAT},
+        { "yaw_min", &(parsed.yaw_min), 1, FLOAT},
+        { "yaw_max", &(parsed.yaw_max), 1, FLOAT},
+        { "gimbal_id", &(parsed.gimbal_id), 1, UINT8_T}
     };
-    static cStruct record = {"local_position_ned_system_global_offset", members, 7, 89};
+    static cStruct record = {"storm32_gimbal_manager_information", members, 9, 60010};
 
-    mavlink_msg_local_position_ned_system_global_offset_decode(message, &parsed);
+    mavlink_msg_storm32_gimbal_manager_information_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_param_map_rc(const mavlink_message_t* message)
+cStruct* unbox_param_value_array(const mavlink_message_t* message)
 {
-    static mavlink_param_map_rc_t parsed;
+    static mavlink_param_value_array_t parsed;
 
     static cMember members[] = {
-        { "param_value0", &(parsed.param_value0), 1, FLOAT},
-        { "scale", &(parsed.scale), 1, FLOAT},
-        { "param_value_min", &(parsed.param_value_min), 1, FLOAT},
-        { "param_value_max", &(parsed.param_value_max), 1, FLOAT},
-        { "param_index", &(parsed.param_index), 1, INT16_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "param_id", &(parsed.param_id), 16, CHAR},
-        { "parameter_rc_channel_index", &(parsed.parameter_rc_channel_index), 1, UINT8_T}
+        { "param_count", &(parsed.param_count), 1, UINT16_T},
+        { "param_index_first", &(parsed.param_index_first), 1, UINT16_T},
+        { "flags", &(parsed.flags), 1, UINT16_T},
+        { "param_array_len", &(parsed.param_array_len), 1, UINT8_T},
+        { "packet_buf", &(parsed.packet_buf), 248, UINT8_T}
     };
-    static cStruct record = {"param_map_rc", members, 9, 50};
+    static cStruct record = {"param_value_array", members, 5, 60041};
 
-    mavlink_msg_param_map_rc_decode(message, &parsed);
+    mavlink_msg_param_value_array_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_log_data(const mavlink_message_t* message)
+cStruct* unbox_qshot_status(const mavlink_message_t* message)
 {
-    static mavlink_log_data_t parsed;
+    static mavlink_qshot_status_t parsed;
+
+    static cMember members[] = {
+        { "mode", &(parsed.mode), 1, UINT16_T},
+        { "shot_state", &(parsed.shot_state), 1, UINT16_T}
+    };
+    static cStruct record = {"qshot_status", members, 2, 60020};
+
+    mavlink_msg_qshot_status_decode(message, &parsed);
+    return &record;
+}
+
+cStruct* unbox_radio_rc_channels(const mavlink_message_t* message)
+{
+    static mavlink_radio_rc_channels_t parsed;
 
     static cMember members[] = {
-        { "ofs", &(parsed.ofs), 1, UINT32_T},
-        { "id", &(parsed.id), 1, UINT16_T},
         { "count", &(parsed.count), 1, UINT8_T},
-        { "data", &(parsed.data), 90, UINT8_T}
+        { "flags", &(parsed.flags), 1, UINT8_T},
+        { "channels", &(parsed.channels), 24, INT16_T}
     };
-    static cStruct record = {"log_data", members, 4, 120};
+    static cStruct record = {"radio_rc_channels", members, 3, 60045};
 
-    mavlink_msg_log_data_decode(message, &parsed);
+    mavlink_msg_radio_rc_channels_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_file_transfer_protocol(const mavlink_message_t* message)
+cStruct* unbox_storm32_gimbal_manager_control_pitchyaw(const mavlink_message_t* message)
 {
-    static mavlink_file_transfer_protocol_t parsed;
+    static mavlink_storm32_gimbal_manager_control_pitchyaw_t parsed;
 
     static cMember members[] = {
-        { "target_network", &(parsed.target_network), 1, UINT8_T},
+        { "pitch", &(parsed.pitch), 1, FLOAT},
+        { "yaw", &(parsed.yaw), 1, FLOAT},
+        { "pitch_rate", &(parsed.pitch_rate), 1, FLOAT},
+        { "yaw_rate", &(parsed.yaw_rate), 1, FLOAT},
+        { "device_flags", &(parsed.device_flags), 1, UINT16_T},
+        { "manager_flags", &(parsed.manager_flags), 1, UINT16_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "payload", &(parsed.payload), 251, UINT8_T}
+        { "gimbal_id", &(parsed.gimbal_id), 1, UINT8_T},
+        { "client", &(parsed.client), 1, UINT8_T}
     };
-    static cStruct record = {"file_transfer_protocol", members, 4, 110};
+    static cStruct record = {"storm32_gimbal_manager_control_pitchyaw", members, 10, 60013};
 
-    mavlink_msg_file_transfer_protocol_decode(message, &parsed);
+    mavlink_msg_storm32_gimbal_manager_control_pitchyaw_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_encapsulated_data(const mavlink_message_t* message)
+cStruct* unbox_storm32_gimbal_manager_status(const mavlink_message_t* message)
 {
-    static mavlink_encapsulated_data_t parsed;
+    static mavlink_storm32_gimbal_manager_status_t parsed;
 
     static cMember members[] = {
-        { "seqnr", &(parsed.seqnr), 1, UINT16_T},
-        { "data", &(parsed.data), 253, UINT8_T}
+        { "device_flags", &(parsed.device_flags), 1, UINT16_T},
+        { "manager_flags", &(parsed.manager_flags), 1, UINT16_T},
+        { "gimbal_id", &(parsed.gimbal_id), 1, UINT8_T},
+        { "supervisor", &(parsed.supervisor), 1, UINT8_T},
+        { "profile", &(parsed.profile), 1, UINT8_T}
     };
-    static cStruct record = {"encapsulated_data", members, 2, 131};
+    static cStruct record = {"storm32_gimbal_manager_status", members, 5, 60011};
 
-    mavlink_msg_encapsulated_data_decode(message, &parsed);
+    mavlink_msg_storm32_gimbal_manager_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_param_ext_value(const mavlink_message_t* message)
+cStruct* unbox_radio_link_stats(const mavlink_message_t* message)
 {
-    static mavlink_param_ext_value_t parsed;
+    static mavlink_radio_link_stats_t parsed;
 
     static cMember members[] = {
-        { "param_count", &(parsed.param_count), 1, UINT16_T},
-        { "param_index", &(parsed.param_index), 1, UINT16_T},
-        { "param_id", &(parsed.param_id), 16, CHAR},
-        { "param_value", &(parsed.param_value), 128, CHAR},
-        { "param_type", &(parsed.param_type), 1, UINT8_T}
+        { "flags", &(parsed.flags), 1, UINT8_T},
+        { "rx_LQ", &(parsed.rx_LQ), 1, UINT8_T},
+        { "rx_rssi1", &(parsed.rx_rssi1), 1, UINT8_T},
+        { "rx_snr1", &(parsed.rx_snr1), 1, INT8_T},
+        { "rx_rssi2", &(parsed.rx_rssi2), 1, UINT8_T},
+        { "rx_snr2", &(parsed.rx_snr2), 1, INT8_T},
+        { "rx_receive_antenna", &(parsed.rx_receive_antenna), 1, UINT8_T},
+        { "rx_transmit_antenna", &(parsed.rx_transmit_antenna), 1, UINT8_T},
+        { "tx_LQ", &(parsed.tx_LQ), 1, UINT8_T},
+        { "tx_rssi1", &(parsed.tx_rssi1), 1, UINT8_T},
+        { "tx_snr1", &(parsed.tx_snr1), 1, INT8_T},
+        { "tx_rssi2", &(parsed.tx_rssi2), 1, UINT8_T},
+        { "tx_snr2", &(parsed.tx_snr2), 1, INT8_T},
+        { "tx_receive_antenna", &(parsed.tx_receive_antenna), 1, UINT8_T},
+        { "tx_transmit_antenna", &(parsed.tx_transmit_antenna), 1, UINT8_T}
     };
-    static cStruct record = {"param_ext_value", members, 5, 322};
+    static cStruct record = {"radio_link_stats", members, 15, 60046};
 
-    mavlink_msg_param_ext_value_decode(message, &parsed);
+    mavlink_msg_radio_link_stats_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_mission_request(const mavlink_message_t* message)
+cStruct* unbox_storm32_gimbal_manager_control(const mavlink_message_t* message)
 {
-    static mavlink_mission_request_t parsed;
+    static mavlink_storm32_gimbal_manager_control_t parsed;
 
     static cMember members[] = {
-        { "seq", &(parsed.seq), 1, UINT16_T},
+        { "q", &(parsed.q), 4, FLOAT},
+        { "angular_velocity_x", &(parsed.angular_velocity_x), 1, FLOAT},
+        { "angular_velocity_y", &(parsed.angular_velocity_y), 1, FLOAT},
+        { "angular_velocity_z", &(parsed.angular_velocity_z), 1, FLOAT},
+        { "device_flags", &(parsed.device_flags), 1, UINT16_T},
+        { "manager_flags", &(parsed.manager_flags), 1, UINT16_T},
         { "target_system", &(parsed.target_system), 1, UINT8_T},
         { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "mission_type", &(parsed.mission_type), 1, UINT8_T}
+        { "gimbal_id", &(parsed.gimbal_id), 1, UINT8_T},
+        { "client", &(parsed.client), 1, UINT8_T}
     };
-    static cStruct record = {"mission_request", members, 4, 40};
+    static cStruct record = {"storm32_gimbal_manager_control", members, 10, 60012};
 
-    mavlink_msg_mission_request_decode(message, &parsed);
+    mavlink_msg_storm32_gimbal_manager_control_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_terrain_check(const mavlink_message_t* message)
+cStruct* unbox_figure_eight_execution_status(const mavlink_message_t* message)
 {
-    static mavlink_terrain_check_t parsed;
+    static mavlink_figure_eight_execution_status_t parsed;
 
     static cMember members[] = {
-        { "lat", &(parsed.lat), 1, INT32_T},
-        { "lon", &(parsed.lon), 1, INT32_T}
+        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
+        { "major_radius", &(parsed.major_radius), 1, FLOAT},
+        { "minor_radius", &(parsed.minor_radius), 1, FLOAT},
+        { "orientation", &(parsed.orientation), 1, FLOAT},
+        { "x", &(parsed.x), 1, INT32_T},
+        { "y", &(parsed.y), 1, INT32_T},
+        { "z", &(parsed.z), 1, FLOAT},
+        { "frame", &(parsed.frame), 1, UINT8_T}
     };
-    static cStruct record = {"terrain_check", members, 2, 135};
+    static cStruct record = {"figure_eight_execution_status", members, 8, 361};
 
-    mavlink_msg_terrain_check_decode(message, &parsed);
+    mavlink_msg_figure_eight_execution_status_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_uavcan_node_status(const mavlink_message_t* message)
+cStruct* unbox_target_absolute(const mavlink_message_t* message)
 {
-    static mavlink_uavcan_node_status_t parsed;
+    static mavlink_target_absolute_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "uptime_sec", &(parsed.uptime_sec), 1, UINT32_T},
-        { "vendor_specific_status_code", &(parsed.vendor_specific_status_code), 1, UINT16_T},
-        { "health", &(parsed.health), 1, UINT8_T},
-        { "mode", &(parsed.mode), 1, UINT8_T},
-        { "sub_mode", &(parsed.sub_mode), 1, UINT8_T}
+        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
+        { "lat", &(parsed.lat), 1, INT32_T},
+        { "lon", &(parsed.lon), 1, INT32_T},
+        { "alt", &(parsed.alt), 1, FLOAT},
+        { "vel", &(parsed.vel), 3, FLOAT},
+        { "acc", &(parsed.acc), 3, FLOAT},
+        { "q_target", &(parsed.q_target), 4, FLOAT},
+        { "rates", &(parsed.rates), 3, FLOAT},
+        { "position_std", &(parsed.position_std), 2, FLOAT},
+        { "vel_std", &(parsed.vel_std), 3, FLOAT},
+        { "acc_std", &(parsed.acc_std), 3, FLOAT},
+        { "id", &(parsed.id), 1, UINT8_T},
+        { "sensor_capabilities", &(parsed.sensor_capabilities), 1, UINT8_T}
     };
-    static cStruct record = {"uavcan_node_status", members, 6, 310};
+    static cStruct record = {"target_absolute", members, 13, 510};
 
-    mavlink_msg_uavcan_node_status_decode(message, &parsed);
+    mavlink_msg_target_absolute_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_camera_tracking_geo_status(const mavlink_message_t* message)
+cStruct* unbox_wifi_network_info(const mavlink_message_t* message)
 {
-    static mavlink_camera_tracking_geo_status_t parsed;
+    static mavlink_wifi_network_info_t parsed;
 
     static cMember members[] = {
-        { "lat", &(parsed.lat), 1, INT32_T},
-        { "lon", &(parsed.lon), 1, INT32_T},
-        { "alt", &(parsed.alt), 1, FLOAT},
-        { "h_acc", &(parsed.h_acc), 1, FLOAT},
-        { "v_acc", &(parsed.v_acc), 1, FLOAT},
-        { "vel_n", &(parsed.vel_n), 1, FLOAT},
-        { "vel_e", &(parsed.vel_e), 1, FLOAT},
-        { "vel_d", &(parsed.vel_d), 1, FLOAT},
-        { "vel_acc", &(parsed.vel_acc), 1, FLOAT},
-        { "dist", &(parsed.dist), 1, FLOAT},
-        { "hdg", &(parsed.hdg), 1, FLOAT},
-        { "hdg_acc", &(parsed.hdg_acc), 1, FLOAT},
-        { "tracking_status", &(parsed.tracking_status), 1, UINT8_T}
+        { "data_rate", &(parsed.data_rate), 1, UINT16_T},
+        { "ssid", &(parsed.ssid), 32, CHAR},
+        { "channel_id", &(parsed.channel_id), 1, UINT8_T},
+        { "signal_quality", &(parsed.signal_quality), 1, UINT8_T},
+        { "security", &(parsed.security), 1, UINT8_T}
     };
-    static cStruct record = {"camera_tracking_geo_status", members, 13, 276};
+    static cStruct record = {"wifi_network_info", members, 5, 298};
 
-    mavlink_msg_camera_tracking_geo_status_decode(message, &parsed);
+    mavlink_msg_wifi_network_info_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_uavcan_node_info(const mavlink_message_t* message)
+cStruct* unbox_mission_checksum(const mavlink_message_t* message)
 {
-    static mavlink_uavcan_node_info_t parsed;
+    static mavlink_mission_checksum_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "uptime_sec", &(parsed.uptime_sec), 1, UINT32_T},
-        { "sw_vcs_commit", &(parsed.sw_vcs_commit), 1, UINT32_T},
-        { "name", &(parsed.name), 80, CHAR},
-        { "hw_version_major", &(parsed.hw_version_major), 1, UINT8_T},
-        { "hw_version_minor", &(parsed.hw_version_minor), 1, UINT8_T},
-        { "hw_unique_id", &(parsed.hw_unique_id), 16, UINT8_T},
-        { "sw_version_major", &(parsed.sw_version_major), 1, UINT8_T},
-        { "sw_version_minor", &(parsed.sw_version_minor), 1, UINT8_T}
+        { "checksum", &(parsed.checksum), 1, UINT32_T},
+        { "mission_type", &(parsed.mission_type), 1, UINT8_T}
     };
-    static cStruct record = {"uavcan_node_info", members, 9, 311};
+    static cStruct record = {"mission_checksum", members, 2, 53};
 
-    mavlink_msg_uavcan_node_info_decode(message, &parsed);
+    mavlink_msg_mission_checksum_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_data_transmission_handshake(const mavlink_message_t* message)
+cStruct* unbox_target_relative(const mavlink_message_t* message)
 {
-    static mavlink_data_transmission_handshake_t parsed;
+    static mavlink_target_relative_t parsed;
 
     static cMember members[] = {
-        { "size", &(parsed.size), 1, UINT32_T},
-        { "width", &(parsed.width), 1, UINT16_T},
-        { "height", &(parsed.height), 1, UINT16_T},
-        { "packets", &(parsed.packets), 1, UINT16_T},
-        { "type", &(parsed.type), 1, UINT8_T},
-        { "payload", &(parsed.payload), 1, UINT8_T},
-        { "jpg_quality", &(parsed.jpg_quality), 1, UINT8_T}
+        { "timestamp", &(parsed.timestamp), 1, UINT64_T},
+        { "x", &(parsed.x), 1, FLOAT},
+        { "y", &(parsed.y), 1, FLOAT},
+        { "z", &(parsed.z), 1, FLOAT},
+        { "pos_std", &(parsed.pos_std), 3, FLOAT},
+        { "yaw_std", &(parsed.yaw_std), 1, FLOAT},
+        { "q_target", &(parsed.q_target), 4, FLOAT},
+        { "q_sensor", &(parsed.q_sensor), 4, FLOAT},
+        { "id", &(parsed.id), 1, UINT8_T},
+        { "frame", &(parsed.frame), 1, UINT8_T},
+        { "type", &(parsed.type), 1, UINT8_T}
     };
-    static cStruct record = {"data_transmission_handshake", members, 7, 130};
+    static cStruct record = {"target_relative", members, 11, 511};
 
-    mavlink_msg_data_transmission_handshake_decode(message, &parsed);
+    mavlink_msg_target_relative_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_mission_item_reached(const mavlink_message_t* message)
+cStruct* unbox_available_modes(const mavlink_message_t* message)
 {
-    static mavlink_mission_item_reached_t parsed;
+    static mavlink_available_modes_t parsed;
 
     static cMember members[] = {
-        { "seq", &(parsed.seq), 1, UINT16_T}
+        { "custom_mode", &(parsed.custom_mode), 1, UINT32_T},
+        { "number_modes", &(parsed.number_modes), 1, UINT8_T},
+        { "mode_index", &(parsed.mode_index), 1, UINT8_T},
+        { "standard_mode", &(parsed.standard_mode), 1, UINT8_T},
+        { "base_mode", &(parsed.base_mode), 1, UINT8_T},
+        { "mode_name", &(parsed.mode_name), 50, CHAR}
     };
-    static cStruct record = {"mission_item_reached", members, 1, 46};
+    static cStruct record = {"available_modes", members, 6, 435};
 
-    mavlink_msg_mission_item_reached_decode(message, &parsed);
+    mavlink_msg_available_modes_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_gps2_raw(const mavlink_message_t* message)
+cStruct* unbox_airspeed(const mavlink_message_t* message)
 {
-    static mavlink_gps2_raw_t parsed;
+    static mavlink_airspeed_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "lat", &(parsed.lat), 1, INT32_T},
-        { "lon", &(parsed.lon), 1, INT32_T},
-        { "alt", &(parsed.alt), 1, INT32_T},
-        { "dgps_age", &(parsed.dgps_age), 1, UINT32_T},
-        { "eph", &(parsed.eph), 1, UINT16_T},
-        { "epv", &(parsed.epv), 1, UINT16_T},
-        { "vel", &(parsed.vel), 1, UINT16_T},
-        { "cog", &(parsed.cog), 1, UINT16_T},
-        { "fix_type", &(parsed.fix_type), 1, UINT8_T},
-        { "satellites_visible", &(parsed.satellites_visible), 1, UINT8_T},
-        { "dgps_numch", &(parsed.dgps_numch), 1, UINT8_T},
-        { "yaw", &(parsed.yaw), 1, UINT16_T},
-        { "alt_ellipsoid", &(parsed.alt_ellipsoid), 1, INT32_T},
-        { "h_acc", &(parsed.h_acc), 1, UINT32_T},
-        { "v_acc", &(parsed.v_acc), 1, UINT32_T},
-        { "vel_acc", &(parsed.vel_acc), 1, UINT32_T},
-        { "hdg_acc", &(parsed.hdg_acc), 1, UINT32_T}
+        { "airspeed", &(parsed.airspeed), 1, FLOAT},
+        { "raw_press", &(parsed.raw_press), 1, FLOAT},
+        { "temperature", &(parsed.temperature), 1, INT16_T},
+        { "id", &(parsed.id), 1, UINT8_T},
+        { "flags", &(parsed.flags), 1, UINT8_T}
     };
-    static cStruct record = {"gps2_raw", members, 18, 124};
+    static cStruct record = {"airspeed", members, 5, 295};
 
-    mavlink_msg_gps2_raw_decode(message, &parsed);
+    mavlink_msg_airspeed_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_scaled_pressure3(const mavlink_message_t* message)
+cStruct* unbox_component_information_basic(const mavlink_message_t* message)
 {
-    static mavlink_scaled_pressure3_t parsed;
+    static mavlink_component_information_basic_t parsed;
 
     static cMember members[] = {
+        { "capabilities", &(parsed.capabilities), 1, UINT64_T},
         { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "press_abs", &(parsed.press_abs), 1, FLOAT},
-        { "press_diff", &(parsed.press_diff), 1, FLOAT},
-        { "temperature", &(parsed.temperature), 1, INT16_T},
-        { "temperature_press_diff", &(parsed.temperature_press_diff), 1, INT16_T}
+        { "vendor_name", &(parsed.vendor_name), 32, CHAR},
+        { "model_name", &(parsed.model_name), 32, CHAR},
+        { "software_version", &(parsed.software_version), 24, CHAR},
+        { "hardware_version", &(parsed.hardware_version), 24, CHAR},
+        { "serial_number", &(parsed.serial_number), 32, CHAR}
     };
-    static cStruct record = {"scaled_pressure3", members, 5, 143};
+    static cStruct record = {"component_information_basic", members, 7, 396};
 
-    mavlink_msg_scaled_pressure3_decode(message, &parsed);
+    mavlink_msg_component_information_basic_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_att_pos_mocap(const mavlink_message_t* message)
+cStruct* unbox_param_ack_transaction(const mavlink_message_t* message)
 {
-    static mavlink_att_pos_mocap_t parsed;
+    static mavlink_param_ack_transaction_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "q", &(parsed.q), 4, FLOAT},
-        { "x", &(parsed.x), 1, FLOAT},
-        { "y", &(parsed.y), 1, FLOAT},
-        { "z", &(parsed.z), 1, FLOAT},
-        { "covariance", &(parsed.covariance), 21, FLOAT}
+        { "param_value", &(parsed.param_value), 1, FLOAT},
+        { "target_system", &(parsed.target_system), 1, UINT8_T},
+        { "target_component", &(parsed.target_component), 1, UINT8_T},
+        { "param_id", &(parsed.param_id), 16, CHAR},
+        { "param_type", &(parsed.param_type), 1, UINT8_T},
+        { "param_result", &(parsed.param_result), 1, UINT8_T}
     };
-    static cStruct record = {"att_pos_mocap", members, 6, 138};
+    static cStruct record = {"param_ack_transaction", members, 6, 19};
 
-    mavlink_msg_att_pos_mocap_decode(message, &parsed);
+    mavlink_msg_param_ack_transaction_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_raw_pressure(const mavlink_message_t* message)
+cStruct* unbox_group_end(const mavlink_message_t* message)
 {
-    static mavlink_raw_pressure_t parsed;
+    static mavlink_group_end_t parsed;
 
     static cMember members[] = {
         { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "press_abs", &(parsed.press_abs), 1, INT16_T},
-        { "press_diff1", &(parsed.press_diff1), 1, INT16_T},
-        { "press_diff2", &(parsed.press_diff2), 1, INT16_T},
-        { "temperature", &(parsed.temperature), 1, INT16_T}
+        { "group_id", &(parsed.group_id), 1, UINT32_T},
+        { "mission_checksum", &(parsed.mission_checksum), 1, UINT32_T}
     };
-    static cStruct record = {"raw_pressure", members, 5, 28};
+    static cStruct record = {"group_end", members, 3, 415};
 
-    mavlink_msg_raw_pressure_decode(message, &parsed);
+    mavlink_msg_group_end_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_play_tune(const mavlink_message_t* message)
+cStruct* unbox_current_mode(const mavlink_message_t* message)
 {
-    static mavlink_play_tune_t parsed;
+    static mavlink_current_mode_t parsed;
 
     static cMember members[] = {
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "tune", &(parsed.tune), 30, CHAR},
-        { "tune2", &(parsed.tune2), 200, CHAR}
+        { "custom_mode", &(parsed.custom_mode), 1, UINT32_T},
+        { "standard_mode", &(parsed.standard_mode), 1, UINT8_T},
+        { "base_mode", &(parsed.base_mode), 1, UINT8_T}
     };
-    static cStruct record = {"play_tune", members, 4, 258};
+    static cStruct record = {"current_mode", members, 3, 436};
 
-    mavlink_msg_play_tune_decode(message, &parsed);
+    mavlink_msg_current_mode_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_high_latency2(const mavlink_message_t* message)
+cStruct* unbox_battery_status_v2(const mavlink_message_t* message)
 {
-    static mavlink_high_latency2_t parsed;
+    static mavlink_battery_status_v2_t parsed;
 
     static cMember members[] = {
-        { "timestamp", &(parsed.timestamp), 1, UINT32_T},
-        { "latitude", &(parsed.latitude), 1, INT32_T},
-        { "longitude", &(parsed.longitude), 1, INT32_T},
-        { "custom_mode", &(parsed.custom_mode), 1, UINT16_T},
-        { "altitude", &(parsed.altitude), 1, INT16_T},
-        { "target_altitude", &(parsed.target_altitude), 1, INT16_T},
-        { "target_distance", &(parsed.target_distance), 1, UINT16_T},
-        { "wp_num", &(parsed.wp_num), 1, UINT16_T},
-        { "failure_flags", &(parsed.failure_flags), 1, UINT16_T},
-        { "type", &(parsed.type), 1, UINT8_T},
-        { "autopilot", &(parsed.autopilot), 1, UINT8_T},
-        { "heading", &(parsed.heading), 1, UINT8_T},
-        { "target_heading", &(parsed.target_heading), 1, UINT8_T},
-        { "throttle", &(parsed.throttle), 1, UINT8_T},
-        { "airspeed", &(parsed.airspeed), 1, UINT8_T},
-        { "airspeed_sp", &(parsed.airspeed_sp), 1, UINT8_T},
-        { "groundspeed", &(parsed.groundspeed), 1, UINT8_T},
-        { "windspeed", &(parsed.windspeed), 1, UINT8_T},
-        { "wind_heading", &(parsed.wind_heading), 1, UINT8_T},
-        { "eph", &(parsed.eph), 1, UINT8_T},
-        { "epv", &(parsed.epv), 1, UINT8_T},
-        { "temperature_air", &(parsed.temperature_air), 1, INT8_T},
-        { "climb_rate", &(parsed.climb_rate), 1, INT8_T},
-        { "battery", &(parsed.battery), 1, INT8_T},
-        { "custom0", &(parsed.custom0), 1, INT8_T},
-        { "custom1", &(parsed.custom1), 1, INT8_T},
-        { "custom2", &(parsed.custom2), 1, INT8_T}
+        { "voltage", &(parsed.voltage), 1, FLOAT},
+        { "current", &(parsed.current), 1, FLOAT},
+        { "capacity_consumed", &(parsed.capacity_consumed), 1, FLOAT},
+        { "capacity_remaining", &(parsed.capacity_remaining), 1, FLOAT},
+        { "status_flags", &(parsed.status_flags), 1, UINT32_T},
+        { "temperature", &(parsed.temperature), 1, INT16_T},
+        { "id", &(parsed.id), 1, UINT8_T},
+        { "percent_remaining", &(parsed.percent_remaining), 1, UINT8_T}
     };
-    static cStruct record = {"high_latency2", members, 27, 235};
+    static cStruct record = {"battery_status_v2", members, 8, 369};
 
-    mavlink_msg_high_latency2_decode(message, &parsed);
+    mavlink_msg_battery_status_v2_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_camera_trigger(const mavlink_message_t* message)
+cStruct* unbox_group_start(const mavlink_message_t* message)
 {
-    static mavlink_camera_trigger_t parsed;
+    static mavlink_group_start_t parsed;
 
     static cMember members[] = {
         { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "seq", &(parsed.seq), 1, UINT32_T}
+        { "group_id", &(parsed.group_id), 1, UINT32_T},
+        { "mission_checksum", &(parsed.mission_checksum), 1, UINT32_T}
     };
-    static cStruct record = {"camera_trigger", members, 2, 112};
+    static cStruct record = {"group_start", members, 3, 414};
 
-    mavlink_msg_camera_trigger_decode(message, &parsed);
+    mavlink_msg_group_start_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_gimbal_manager_set_manual_control(const mavlink_message_t* message)
+cStruct* unbox_protocol_version(const mavlink_message_t* message)
 {
-    static mavlink_gimbal_manager_set_manual_control_t parsed;
+    static mavlink_protocol_version_t parsed;
 
     static cMember members[] = {
-        { "flags", &(parsed.flags), 1, UINT32_T},
-        { "pitch", &(parsed.pitch), 1, FLOAT},
-        { "yaw", &(parsed.yaw), 1, FLOAT},
-        { "pitch_rate", &(parsed.pitch_rate), 1, FLOAT},
-        { "yaw_rate", &(parsed.yaw_rate), 1, FLOAT},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "gimbal_device_id", &(parsed.gimbal_device_id), 1, UINT8_T}
+        { "version", &(parsed.version), 1, UINT16_T},
+        { "min_version", &(parsed.min_version), 1, UINT16_T},
+        { "max_version", &(parsed.max_version), 1, UINT16_T},
+        { "spec_version_hash", &(parsed.spec_version_hash), 8, UINT8_T},
+        { "library_version_hash", &(parsed.library_version_hash), 8, UINT8_T}
     };
-    static cStruct record = {"gimbal_manager_set_manual_control", members, 8, 288};
+    static cStruct record = {"protocol_version", members, 5, 300};
 
-    mavlink_msg_gimbal_manager_set_manual_control_decode(message, &parsed);
+    mavlink_msg_protocol_version_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_log_request_list(const mavlink_message_t* message)
+cStruct* unbox_heartbeat(const mavlink_message_t* message)
 {
-    static mavlink_log_request_list_t parsed;
+    static mavlink_heartbeat_t parsed;
 
     static cMember members[] = {
-        { "start", &(parsed.start), 1, UINT16_T},
-        { "end", &(parsed.end), 1, UINT16_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T}
+        { "custom_mode", &(parsed.custom_mode), 1, UINT32_T},
+        { "type", &(parsed.type), 1, UINT8_T},
+        { "autopilot", &(parsed.autopilot), 1, UINT8_T},
+        { "base_mode", &(parsed.base_mode), 1, UINT8_T},
+        { "system_status", &(parsed.system_status), 1, UINT8_T},
+        { "mavlink_version", &(parsed.mavlink_version), 1, UINT8_T}
     };
-    static cStruct record = {"log_request_list", members, 4, 117};
+    static cStruct record = {"heartbeat", members, 6, 0};
 
-    mavlink_msg_log_request_list_decode(message, &parsed);
+    mavlink_msg_heartbeat_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_attitude_target(const mavlink_message_t* message)
+cStruct* unbox_uavionix_adsb_transceiver_health_report(const mavlink_message_t* message)
 {
-    static mavlink_attitude_target_t parsed;
+    static mavlink_uavionix_adsb_transceiver_health_report_t parsed;
 
     static cMember members[] = {
-        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
-        { "q", &(parsed.q), 4, FLOAT},
-        { "body_roll_rate", &(parsed.body_roll_rate), 1, FLOAT},
-        { "body_pitch_rate", &(parsed.body_pitch_rate), 1, FLOAT},
-        { "body_yaw_rate", &(parsed.body_yaw_rate), 1, FLOAT},
-        { "thrust", &(parsed.thrust), 1, FLOAT},
-        { "type_mask", &(parsed.type_mask), 1, UINT8_T}
+        { "rfHealth", &(parsed.rfHealth), 1, UINT8_T}
     };
-    static cStruct record = {"attitude_target", members, 7, 83};
+    static cStruct record = {"uavionix_adsb_transceiver_health_report", members, 1, 10003};
 
-    mavlink_msg_attitude_target_decode(message, &parsed);
+    mavlink_msg_uavionix_adsb_transceiver_health_report_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_change_operator_control_ack(const mavlink_message_t* message)
+cStruct* unbox_uavionix_adsb_out_dynamic(const mavlink_message_t* message)
 {
-    static mavlink_change_operator_control_ack_t parsed;
+    static mavlink_uavionix_adsb_out_dynamic_t parsed;
 
     static cMember members[] = {
-        { "gcs_system_id", &(parsed.gcs_system_id), 1, UINT8_T},
-        { "control_request", &(parsed.control_request), 1, UINT8_T},
-        { "ack", &(parsed.ack), 1, UINT8_T}
+        { "utcTime", &(parsed.utcTime), 1, UINT32_T},
+        { "gpsLat", &(parsed.gpsLat), 1, INT32_T},
+        { "gpsLon", &(parsed.gpsLon), 1, INT32_T},
+        { "gpsAlt", &(parsed.gpsAlt), 1, INT32_T},
+        { "baroAltMSL", &(parsed.baroAltMSL), 1, INT32_T},
+        { "accuracyHor", &(parsed.accuracyHor), 1, UINT32_T},
+        { "accuracyVert", &(parsed.accuracyVert), 1, UINT16_T},
+        { "accuracyVel", &(parsed.accuracyVel), 1, UINT16_T},
+        { "velVert", &(parsed.velVert), 1, INT16_T},
+        { "velNS", &(parsed.velNS), 1, INT16_T},
+        { "VelEW", &(parsed.VelEW), 1, INT16_T},
+        { "state", &(parsed.state), 1, UINT16_T},
+        { "squawk", &(parsed.squawk), 1, UINT16_T},
+        { "gpsFix", &(parsed.gpsFix), 1, UINT8_T},
+        { "numSats", &(parsed.numSats), 1, UINT8_T},
+        { "emergencyStatus", &(parsed.emergencyStatus), 1, UINT8_T}
     };
-    static cStruct record = {"change_operator_control_ack", members, 3, 6};
+    static cStruct record = {"uavionix_adsb_out_dynamic", members, 16, 10002};
 
-    mavlink_msg_change_operator_control_ack_decode(message, &parsed);
+    mavlink_msg_uavionix_adsb_out_dynamic_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_wifi_config_ap(const mavlink_message_t* message)
+cStruct* unbox_uavionix_adsb_out_cfg(const mavlink_message_t* message)
 {
-    static mavlink_wifi_config_ap_t parsed;
+    static mavlink_uavionix_adsb_out_cfg_t parsed;
 
     static cMember members[] = {
-        { "ssid", &(parsed.ssid), 32, CHAR},
-        { "password", &(parsed.password), 64, CHAR},
-        { "mode", &(parsed.mode), 1, INT8_T},
-        { "response", &(parsed.response), 1, INT8_T}
+        { "ICAO", &(parsed.ICAO), 1, UINT32_T},
+        { "stallSpeed", &(parsed.stallSpeed), 1, UINT16_T},
+        { "callsign", &(parsed.callsign), 9, CHAR},
+        { "emitterType", &(parsed.emitterType), 1, UINT8_T},
+        { "aircraftSize", &(parsed.aircraftSize), 1, UINT8_T},
+        { "gpsOffsetLat", &(parsed.gpsOffsetLat), 1, UINT8_T},
+        { "gpsOffsetLon", &(parsed.gpsOffsetLon), 1, UINT8_T},
+        { "rfSelect", &(parsed.rfSelect), 1, UINT8_T}
     };
-    static cStruct record = {"wifi_config_ap", members, 4, 299};
+    static cStruct record = {"uavionix_adsb_out_cfg", members, 8, 10001};
 
-    mavlink_msg_wifi_config_ap_decode(message, &parsed);
+    mavlink_msg_uavionix_adsb_out_cfg_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_mission_count(const mavlink_message_t* message)
+cStruct* unbox_array_test_1(const mavlink_message_t* message)
 {
-    static mavlink_mission_count_t parsed;
+    static mavlink_array_test_1_t parsed;
 
     static cMember members[] = {
-        { "count", &(parsed.count), 1, UINT16_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "mission_type", &(parsed.mission_type), 1, UINT8_T}
+        { "ar_u32", &(parsed.ar_u32), 4, UINT32_T}
     };
-    static cStruct record = {"mission_count", members, 4, 44};
+    static cStruct record = {"array_test_1", members, 1, 17151};
 
-    mavlink_msg_mission_count_decode(message, &parsed);
+    mavlink_msg_array_test_1_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_esc_info(const mavlink_message_t* message)
+cStruct* unbox_array_test_7(const mavlink_message_t* message)
 {
-    static mavlink_esc_info_t parsed;
+    static mavlink_array_test_7_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "error_count", &(parsed.error_count), 4, UINT32_T},
-        { "counter", &(parsed.counter), 1, UINT16_T},
-        { "failure_flags", &(parsed.failure_flags), 4, UINT16_T},
-        { "temperature", &(parsed.temperature), 4, INT16_T},
-        { "index", &(parsed.index), 1, UINT8_T},
-        { "count", &(parsed.count), 1, UINT8_T},
-        { "connection_type", &(parsed.connection_type), 1, UINT8_T},
-        { "info", &(parsed.info), 1, UINT8_T}
+        { "ar_d", &(parsed.ar_d), 2, DOUBLE},
+        { "ar_f", &(parsed.ar_f), 2, FLOAT},
+        { "ar_u32", &(parsed.ar_u32), 2, UINT32_T},
+        { "ar_i32", &(parsed.ar_i32), 2, INT32_T},
+        { "ar_u16", &(parsed.ar_u16), 2, UINT16_T},
+        { "ar_i16", &(parsed.ar_i16), 2, INT16_T},
+        { "ar_u8", &(parsed.ar_u8), 2, UINT8_T},
+        { "ar_i8", &(parsed.ar_i8), 2, INT8_T},
+        { "ar_c", &(parsed.ar_c), 32, CHAR}
     };
-    static cStruct record = {"esc_info", members, 9, 290};
+    static cStruct record = {"array_test_7", members, 9, 17157};
 
-    mavlink_msg_esc_info_decode(message, &parsed);
+    mavlink_msg_array_test_7_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_param_request_list(const mavlink_message_t* message)
+cStruct* unbox_array_test_4(const mavlink_message_t* message)
 {
-    static mavlink_param_request_list_t parsed;
+    static mavlink_array_test_4_t parsed;
 
     static cMember members[] = {
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T}
+        { "ar_u32", &(parsed.ar_u32), 4, UINT32_T},
+        { "v", &(parsed.v), 1, UINT8_T}
     };
-    static cStruct record = {"param_request_list", members, 2, 21};
+    static cStruct record = {"array_test_4", members, 2, 17154};
 
-    mavlink_msg_param_request_list_decode(message, &parsed);
+    mavlink_msg_array_test_4_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_onboard_computer_status(const mavlink_message_t* message)
+cStruct* unbox_array_test_5(const mavlink_message_t* message)
 {
-    static mavlink_onboard_computer_status_t parsed;
+    static mavlink_array_test_5_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "uptime", &(parsed.uptime), 1, UINT32_T},
-        { "ram_usage", &(parsed.ram_usage), 1, UINT32_T},
-        { "ram_total", &(parsed.ram_total), 1, UINT32_T},
-        { "storage_type", &(parsed.storage_type), 4, UINT32_T},
-        { "storage_usage", &(parsed.storage_usage), 4, UINT32_T},
-        { "storage_total", &(parsed.storage_total), 4, UINT32_T},
-        { "link_type", &(parsed.link_type), 6, UINT32_T},
-        { "link_tx_rate", &(parsed.link_tx_rate), 6, UINT32_T},
-        { "link_rx_rate", &(parsed.link_rx_rate), 6, UINT32_T},
-        { "link_tx_max", &(parsed.link_tx_max), 6, UINT32_T},
-        { "link_rx_max", &(parsed.link_rx_max), 6, UINT32_T},
-        { "fan_speed", &(parsed.fan_speed), 4, INT16_T},
-        { "type", &(parsed.type), 1, UINT8_T},
-        { "cpu_cores", &(parsed.cpu_cores), 8, UINT8_T},
-        { "cpu_combined", &(parsed.cpu_combined), 10, UINT8_T},
-        { "gpu_cores", &(parsed.gpu_cores), 4, UINT8_T},
-        { "gpu_combined", &(parsed.gpu_combined), 10, UINT8_T},
-        { "temperature_board", &(parsed.temperature_board), 1, INT8_T},
-        { "temperature_core", &(parsed.temperature_core), 8, INT8_T}
+        { "c1", &(parsed.c1), 5, CHAR},
+        { "c2", &(parsed.c2), 5, CHAR}
     };
-    static cStruct record = {"onboard_computer_status", members, 20, 390};
+    static cStruct record = {"array_test_5", members, 2, 17155};
 
-    mavlink_msg_onboard_computer_status_decode(message, &parsed);
+    mavlink_msg_array_test_5_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_home_position(const mavlink_message_t* message)
+cStruct* unbox_array_test_8(const mavlink_message_t* message)
 {
-    static mavlink_home_position_t parsed;
+    static mavlink_array_test_8_t parsed;
 
     static cMember members[] = {
-        { "latitude", &(parsed.latitude), 1, INT32_T},
-        { "longitude", &(parsed.longitude), 1, INT32_T},
-        { "altitude", &(parsed.altitude), 1, INT32_T},
-        { "x", &(parsed.x), 1, FLOAT},
-        { "y", &(parsed.y), 1, FLOAT},
-        { "z", &(parsed.z), 1, FLOAT},
-        { "q", &(parsed.q), 4, FLOAT},
-        { "approach_x", &(parsed.approach_x), 1, FLOAT},
-        { "approach_y", &(parsed.approach_y), 1, FLOAT},
-        { "approach_z", &(parsed.approach_z), 1, FLOAT},
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T}
+        { "ar_d", &(parsed.ar_d), 2, DOUBLE},
+        { "v3", &(parsed.v3), 1, UINT32_T},
+        { "ar_u16", &(parsed.ar_u16), 2, UINT16_T}
     };
-    static cStruct record = {"home_position", members, 11, 242};
+    static cStruct record = {"array_test_8", members, 3, 17158};
 
-    mavlink_msg_home_position_decode(message, &parsed);
+    mavlink_msg_array_test_8_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_open_drone_id_system_update(const mavlink_message_t* message)
+cStruct* unbox_array_test_6(const mavlink_message_t* message)
 {
-    static mavlink_open_drone_id_system_update_t parsed;
+    static mavlink_array_test_6_t parsed;
 
     static cMember members[] = {
-        { "operator_latitude", &(parsed.operator_latitude), 1, INT32_T},
-        { "operator_longitude", &(parsed.operator_longitude), 1, INT32_T},
-        { "operator_altitude_geo", &(parsed.operator_altitude_geo), 1, FLOAT},
-        { "timestamp", &(parsed.timestamp), 1, UINT32_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T}
+        { "ar_d", &(parsed.ar_d), 2, DOUBLE},
+        { "v3", &(parsed.v3), 1, UINT32_T},
+        { "ar_u32", &(parsed.ar_u32), 2, UINT32_T},
+        { "ar_i32", &(parsed.ar_i32), 2, INT32_T},
+        { "ar_f", &(parsed.ar_f), 2, FLOAT},
+        { "v2", &(parsed.v2), 1, UINT16_T},
+        { "ar_u16", &(parsed.ar_u16), 2, UINT16_T},
+        { "ar_i16", &(parsed.ar_i16), 2, INT16_T},
+        { "v1", &(parsed.v1), 1, UINT8_T},
+        { "ar_u8", &(parsed.ar_u8), 2, UINT8_T},
+        { "ar_i8", &(parsed.ar_i8), 2, INT8_T},
+        { "ar_c", &(parsed.ar_c), 32, CHAR}
     };
-    static cStruct record = {"open_drone_id_system_update", members, 6, 12919};
+    static cStruct record = {"array_test_6", members, 12, 17156};
 
-    mavlink_msg_open_drone_id_system_update_decode(message, &parsed);
+    mavlink_msg_array_test_6_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_vision_position_estimate(const mavlink_message_t* message)
+cStruct* unbox_array_test_0(const mavlink_message_t* message)
 {
-    static mavlink_vision_position_estimate_t parsed;
+    static mavlink_array_test_0_t parsed;
 
     static cMember members[] = {
-        { "usec", &(parsed.usec), 1, UINT64_T},
-        { "x", &(parsed.x), 1, FLOAT},
-        { "y", &(parsed.y), 1, FLOAT},
-        { "z", &(parsed.z), 1, FLOAT},
-        { "roll", &(parsed.roll), 1, FLOAT},
-        { "pitch", &(parsed.pitch), 1, FLOAT},
-        { "yaw", &(parsed.yaw), 1, FLOAT},
-        { "covariance", &(parsed.covariance), 21, FLOAT},
-        { "reset_counter", &(parsed.reset_counter), 1, UINT8_T}
+        { "ar_u32", &(parsed.ar_u32), 4, UINT32_T},
+        { "ar_u16", &(parsed.ar_u16), 4, UINT16_T},
+        { "v1", &(parsed.v1), 1, UINT8_T},
+        { "ar_i8", &(parsed.ar_i8), 4, INT8_T},
+        { "ar_u8", &(parsed.ar_u8), 4, UINT8_T}
     };
-    static cStruct record = {"vision_position_estimate", members, 9, 102};
+    static cStruct record = {"array_test_0", members, 5, 17150};
 
-    mavlink_msg_vision_position_estimate_decode(message, &parsed);
+    mavlink_msg_array_test_0_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_video_stream_status(const mavlink_message_t* message)
+cStruct* unbox_array_test_3(const mavlink_message_t* message)
 {
-    static mavlink_video_stream_status_t parsed;
+    static mavlink_array_test_3_t parsed;
 
     static cMember members[] = {
-        { "framerate", &(parsed.framerate), 1, FLOAT},
-        { "bitrate", &(parsed.bitrate), 1, UINT32_T},
-        { "flags", &(parsed.flags), 1, UINT16_T},
-        { "resolution_h", &(parsed.resolution_h), 1, UINT16_T},
-        { "resolution_v", &(parsed.resolution_v), 1, UINT16_T},
-        { "rotation", &(parsed.rotation), 1, UINT16_T},
-        { "hfov", &(parsed.hfov), 1, UINT16_T},
-        { "stream_id", &(parsed.stream_id), 1, UINT8_T}
+        { "ar_u32", &(parsed.ar_u32), 4, UINT32_T},
+        { "v", &(parsed.v), 1, UINT8_T}
     };
-    static cStruct record = {"video_stream_status", members, 8, 270};
+    static cStruct record = {"array_test_3", members, 2, 17153};
 
-    mavlink_msg_video_stream_status_decode(message, &parsed);
+    mavlink_msg_array_test_3_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_logging_data(const mavlink_message_t* message)
+cStruct* unbox_avss_drone_position(const mavlink_message_t* message)
 {
-    static mavlink_logging_data_t parsed;
+    static mavlink_avss_drone_position_t parsed;
 
     static cMember members[] = {
-        { "sequence", &(parsed.sequence), 1, UINT16_T},
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "length", &(parsed.length), 1, UINT8_T},
-        { "first_message_offset", &(parsed.first_message_offset), 1, UINT8_T},
-        { "data", &(parsed.data), 249, UINT8_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "lat", &(parsed.lat), 1, INT32_T},
+        { "lon", &(parsed.lon), 1, INT32_T},
+        { "alt", &(parsed.alt), 1, INT32_T},
+        { "ground_alt", &(parsed.ground_alt), 1, FLOAT},
+        { "barometer_alt", &(parsed.barometer_alt), 1, FLOAT}
     };
-    static cStruct record = {"logging_data", members, 6, 266};
+    static cStruct record = {"avss_drone_position", members, 6, 60051};
 
-    mavlink_msg_logging_data_decode(message, &parsed);
+    mavlink_msg_avss_drone_position_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_odometry(const mavlink_message_t* message)
+cStruct* unbox_avss_drone_operation_mode(const mavlink_message_t* message)
 {
-    static mavlink_odometry_t parsed;
+    static mavlink_avss_drone_operation_mode_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT64_T},
-        { "x", &(parsed.x), 1, FLOAT},
-        { "y", &(parsed.y), 1, FLOAT},
-        { "z", &(parsed.z), 1, FLOAT},
-        { "q", &(parsed.q), 4, FLOAT},
-        { "vx", &(parsed.vx), 1, FLOAT},
-        { "vy", &(parsed.vy), 1, FLOAT},
-        { "vz", &(parsed.vz), 1, FLOAT},
-        { "rollspeed", &(parsed.rollspeed), 1, FLOAT},
-        { "pitchspeed", &(parsed.pitchspeed), 1, FLOAT},
-        { "yawspeed", &(parsed.yawspeed), 1, FLOAT},
-        { "pose_covariance", &(parsed.pose_covariance), 21, FLOAT},
-        { "velocity_covariance", &(parsed.velocity_covariance), 21, FLOAT},
-        { "frame_id", &(parsed.frame_id), 1, UINT8_T},
-        { "child_frame_id", &(parsed.child_frame_id), 1, UINT8_T},
-        { "reset_counter", &(parsed.reset_counter), 1, UINT8_T},
-        { "estimator_type", &(parsed.estimator_type), 1, UINT8_T},
-        { "quality", &(parsed.quality), 1, INT8_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "M300_operation_mode", &(parsed.M300_operation_mode), 1, UINT8_T},
+        { "horsefly_operation_mode", &(parsed.horsefly_operation_mode), 1, UINT8_T}
     };
-    static cStruct record = {"odometry", members, 18, 331};
+    static cStruct record = {"avss_drone_operation_mode", members, 3, 60053};
 
-    mavlink_msg_odometry_decode(message, &parsed);
+    mavlink_msg_avss_drone_operation_mode_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_servo_output_raw(const mavlink_message_t* message)
+cStruct* unbox_avss_drone_imu(const mavlink_message_t* message)
 {
-    static mavlink_servo_output_raw_t parsed;
+    static mavlink_avss_drone_imu_t parsed;
 
     static cMember members[] = {
-        { "time_usec", &(parsed.time_usec), 1, UINT32_T},
-        { "servo1_raw", &(parsed.servo1_raw), 1, UINT16_T},
-        { "servo2_raw", &(parsed.servo2_raw), 1, UINT16_T},
-        { "servo3_raw", &(parsed.servo3_raw), 1, UINT16_T},
-        { "servo4_raw", &(parsed.servo4_raw), 1, UINT16_T},
-        { "servo5_raw", &(parsed.servo5_raw), 1, UINT16_T},
-        { "servo6_raw", &(parsed.servo6_raw), 1, UINT16_T},
-        { "servo7_raw", &(parsed.servo7_raw), 1, UINT16_T},
-        { "servo8_raw", &(parsed.servo8_raw), 1, UINT16_T},
-        { "port", &(parsed.port), 1, UINT8_T},
-        { "servo9_raw", &(parsed.servo9_raw), 1, UINT16_T},
-        { "servo10_raw", &(parsed.servo10_raw), 1, UINT16_T},
-        { "servo11_raw", &(parsed.servo11_raw), 1, UINT16_T},
-        { "servo12_raw", &(parsed.servo12_raw), 1, UINT16_T},
-        { "servo13_raw", &(parsed.servo13_raw), 1, UINT16_T},
-        { "servo14_raw", &(parsed.servo14_raw), 1, UINT16_T},
-        { "servo15_raw", &(parsed.servo15_raw), 1, UINT16_T},
-        { "servo16_raw", &(parsed.servo16_raw), 1, UINT16_T}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "q1", &(parsed.q1), 1, FLOAT},
+        { "q2", &(parsed.q2), 1, FLOAT},
+        { "q3", &(parsed.q3), 1, FLOAT},
+        { "q4", &(parsed.q4), 1, FLOAT},
+        { "xacc", &(parsed.xacc), 1, FLOAT},
+        { "yacc", &(parsed.yacc), 1, FLOAT},
+        { "zacc", &(parsed.zacc), 1, FLOAT},
+        { "xgyro", &(parsed.xgyro), 1, FLOAT},
+        { "ygyro", &(parsed.ygyro), 1, FLOAT},
+        { "zgyro", &(parsed.zgyro), 1, FLOAT}
     };
-    static cStruct record = {"servo_output_raw", members, 18, 36};
+    static cStruct record = {"avss_drone_imu", members, 11, 60052};
 
-    mavlink_msg_servo_output_raw_decode(message, &parsed);
+    mavlink_msg_avss_drone_imu_decode(message, &parsed);
     return &record;
 }
 
-cStruct* unbox_open_drone_id_operator_id(const mavlink_message_t* message)
+cStruct* unbox_avss_prs_sys_status(const mavlink_message_t* message)
 {
-    static mavlink_open_drone_id_operator_id_t parsed;
+    static mavlink_avss_prs_sys_status_t parsed;
 
     static cMember members[] = {
-        { "target_system", &(parsed.target_system), 1, UINT8_T},
-        { "target_component", &(parsed.target_component), 1, UINT8_T},
-        { "id_or_mac", &(parsed.id_or_mac), 20, UINT8_T},
-        { "operator_id_type", &(parsed.operator_id_type), 1, UINT8_T},
-        { "operator_id", &(parsed.operator_id), 20, CHAR}
+        { "time_boot_ms", &(parsed.time_boot_ms), 1, UINT32_T},
+        { "error_status", &(parsed.error_status), 1, UINT32_T},
+        { "battery_status", &(parsed.battery_status), 1, UINT32_T},
+        { "arm_status", &(parsed.arm_status), 1, UINT8_T},
+        { "charge_status", &(parsed.charge_status), 1, UINT8_T}
     };
-    static cStruct record = {"open_drone_id_operator_id", members, 5, 12905};
+    static cStruct record = {"avss_prs_sys_status", members, 5, 60050};
 
-    mavlink_msg_open_drone_id_operator_id_decode(message, &parsed);
+    mavlink_msg_avss_prs_sys_status_decode(message, &parsed);
+    return &record;
+}
+
+cStruct* unbox_test_types(const mavlink_message_t* message)
+{
+    static mavlink_test_types_t parsed;
+
+    static cMember members[] = {
+        { "u64", &(parsed.u64), 1, UINT64_T},
+        { "s64", &(parsed.s64), 1, INT64_T},
+        { "d", &(parsed.d), 1, DOUBLE},
+        { "u64_array", &(parsed.u64_array), 3, UINT64_T},
+        { "s64_array", &(parsed.s64_array), 3, INT64_T},
+        { "d_array", &(parsed.d_array), 3, DOUBLE},
+        { "u32", &(parsed.u32), 1, UINT32_T},
+        { "s32", &(parsed.s32), 1, INT32_T},
+        { "f", &(parsed.f), 1, FLOAT},
+        { "u32_array", &(parsed.u32_array), 3, UINT32_T},
+        { "s32_array", &(parsed.s32_array), 3, INT32_T},
+        { "f_array", &(parsed.f_array), 3, FLOAT},
+        { "u16", &(parsed.u16), 1, UINT16_T},
+        { "s16", &(parsed.s16), 1, INT16_T},
+        { "u16_array", &(parsed.u16_array), 3, UINT16_T},
+        { "s16_array", &(parsed.s16_array), 3, INT16_T},
+        { "c", &(parsed.c), 1, CHAR},
+        { "s", &(parsed.s), 10, CHAR},
+        { "u8", &(parsed.u8), 1, UINT8_T},
+        { "s8", &(parsed.s8), 1, INT8_T},
+        { "u8_array", &(parsed.u8_array), 3, UINT8_T},
+        { "s8_array", &(parsed.s8_array), 3, INT8_T}
+    };
+    static cStruct record = {"test_types", members, 22, 17000};
+
+    mavlink_msg_test_types_decode(message, &parsed);
     return &record;
 }
 
 
 
 
 unboxer unboxers[] = {
```

### Comparing `UAVReaders-0.5.6/mavlink_introspect_gen.h` & `UAVReaders-0.6.2/mavlink_introspect_gen.h`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,360 +8,360 @@
 #include "mavlink/mavlink_types.h"
 #include "table.h"
 
 typedef cStruct*(*unboxer)(const mavlink_message_t*);
 
 extern unboxer unboxers[];
 
-cStruct* unbox_wifi_network_info(const mavlink_message_t* message);
-cStruct* unbox_target_absolute(const mavlink_message_t* message);
-cStruct* unbox_current_mode(const mavlink_message_t* message);
-cStruct* unbox_battery_status_v2(const mavlink_message_t* message);
-cStruct* unbox_group_start(const mavlink_message_t* message);
-cStruct* unbox_figure_eight_execution_status(const mavlink_message_t* message);
-cStruct* unbox_group_end(const mavlink_message_t* message);
-cStruct* unbox_mission_checksum(const mavlink_message_t* message);
-cStruct* unbox_target_relative(const mavlink_message_t* message);
-cStruct* unbox_airspeed(const mavlink_message_t* message);
-cStruct* unbox_param_ack_transaction(const mavlink_message_t* message);
-cStruct* unbox_available_modes(const mavlink_message_t* message);
-cStruct* unbox_component_information_basic(const mavlink_message_t* message);
-cStruct* unbox_icarous_kinematic_bands(const mavlink_message_t* message);
-cStruct* unbox_icarous_heartbeat(const mavlink_message_t* message);
-cStruct* unbox_sensor_airflow_angles(const mavlink_message_t* message);
-cStruct* unbox_aslctrl_debug(const mavlink_message_t* message);
-cStruct* unbox_sens_batmon(const mavlink_message_t* message);
-cStruct* unbox_asluav_status(const mavlink_message_t* message);
-cStruct* unbox_sens_power(const mavlink_message_t* message);
-cStruct* unbox_command_long_stamped(const mavlink_message_t* message);
+cStruct* unbox_local_position_ned_system_global_offset(const mavlink_message_t* message);
+cStruct* unbox_hil_actuator_controls(const mavlink_message_t* message);
+cStruct* unbox_vision_speed_estimate(const mavlink_message_t* message);
+cStruct* unbox_hil_rc_inputs_raw(const mavlink_message_t* message);
+cStruct* unbox_log_request_data(const mavlink_message_t* message);
+cStruct* unbox_hil_optical_flow(const mavlink_message_t* message);
+cStruct* unbox_open_drone_id_message_pack(const mavlink_message_t* message);
+cStruct* unbox_safety_set_allowed_area(const mavlink_message_t* message);
+cStruct* unbox_play_tune_v2(const mavlink_message_t* message);
+cStruct* unbox_follow_target(const mavlink_message_t* message);
+cStruct* unbox_odometry(const mavlink_message_t* message);
+cStruct* unbox_gps_rtk(const mavlink_message_t* message);
+cStruct* unbox_winch_status(const mavlink_message_t* message);
+cStruct* unbox_trajectory_representation_bezier(const mavlink_message_t* message);
+cStruct* unbox_param_set(const mavlink_message_t* message);
+cStruct* unbox_hil_gps(const mavlink_message_t* message);
+cStruct* unbox_wifi_config_ap(const mavlink_message_t* message);
+cStruct* unbox_vision_position_estimate(const mavlink_message_t* message);
+cStruct* unbox_rc_channels(const mavlink_message_t* message);
+cStruct* unbox_highres_imu(const mavlink_message_t* message);
+cStruct* unbox_gimbal_device_attitude_status(const mavlink_message_t* message);
+cStruct* unbox_autopilot_state_for_gimbal_device(const mavlink_message_t* message);
+cStruct* unbox_fence_status(const mavlink_message_t* message);
+cStruct* unbox_extended_sys_state(const mavlink_message_t* message);
+cStruct* unbox_open_drone_id_operator_id(const mavlink_message_t* message);
+cStruct* unbox_named_value_int(const mavlink_message_t* message);
+cStruct* unbox_message_interval(const mavlink_message_t* message);
+cStruct* unbox_param_ext_ack(const mavlink_message_t* message);
+cStruct* unbox_param_ext_set(const mavlink_message_t* message);
+cStruct* unbox_mag_cal_report(const mavlink_message_t* message);
+cStruct* unbox_current_event_sequence(const mavlink_message_t* message);
+cStruct* unbox_terrain_data(const mavlink_message_t* message);
+cStruct* unbox_request_event(const mavlink_message_t* message);
+cStruct* unbox_component_metadata(const mavlink_message_t* message);
+cStruct* unbox_actuator_control_target(const mavlink_message_t* message);
+cStruct* unbox_scaled_imu2(const mavlink_message_t* message);
+cStruct* unbox_data_transmission_handshake(const mavlink_message_t* message);
+cStruct* unbox_uavcan_node_info(const mavlink_message_t* message);
+cStruct* unbox_param_ext_value(const mavlink_message_t* message);
+cStruct* unbox_play_tune(const mavlink_message_t* message);
+cStruct* unbox_cellular_status(const mavlink_message_t* message);
+cStruct* unbox_logging_data_acked(const mavlink_message_t* message);
+cStruct* unbox_gps2_raw(const mavlink_message_t* message);
+cStruct* unbox_isbd_link_status(const mavlink_message_t* message);
+cStruct* unbox_gimbal_manager_set_manual_control(const mavlink_message_t* message);
+cStruct* unbox_camera_image_captured(const mavlink_message_t* message);
+cStruct* unbox_component_information(const mavlink_message_t* message);
+cStruct* unbox_control_system_state(const mavlink_message_t* message);
+cStruct* unbox_cellular_config(const mavlink_message_t* message);
+cStruct* unbox_uavcan_node_status(const mavlink_message_t* message);
+cStruct* unbox_distance_sensor(const mavlink_message_t* message);
+cStruct* unbox_param_ext_request_list(const mavlink_message_t* message);
+cStruct* unbox_file_transfer_protocol(const mavlink_message_t* message);
+cStruct* unbox_gimbal_manager_information(const mavlink_message_t* message);
+cStruct* unbox_manual_control(const mavlink_message_t* message);
+cStruct* unbox_setup_signing(const mavlink_message_t* message);
+cStruct* unbox_statustext(const mavlink_message_t* message);
+cStruct* unbox_command_cancel(const mavlink_message_t* message);
+cStruct* unbox_esc_info(const mavlink_message_t* message);
+cStruct* unbox_mission_set_current(const mavlink_message_t* message);
+cStruct* unbox_utm_global_position(const mavlink_message_t* message);
+cStruct* unbox_gimbal_manager_set_pitchyaw(const mavlink_message_t* message);
+cStruct* unbox_power_status(const mavlink_message_t* message);
+cStruct* unbox_param_request_read(const mavlink_message_t* message);
+cStruct* unbox_camera_fov_status(const mavlink_message_t* message);
+cStruct* unbox_mission_current(const mavlink_message_t* message);
+cStruct* unbox_mount_orientation(const mavlink_message_t* message);
+cStruct* unbox_attitude(const mavlink_message_t* message);
+cStruct* unbox_hygrometer_sensor(const mavlink_message_t* message);
+cStruct* unbox_terrain_report(const mavlink_message_t* message);
+cStruct* unbox_hil_sensor(const mavlink_message_t* message);
+cStruct* unbox_vibration(const mavlink_message_t* message);
+cStruct* unbox_scaled_pressure3(const mavlink_message_t* message);
+cStruct* unbox_change_operator_control_ack(const mavlink_message_t* message);
+cStruct* unbox_v2_extension(const mavlink_message_t* message);
+cStruct* unbox_event(const mavlink_message_t* message);
+cStruct* unbox_video_stream_status(const mavlink_message_t* message);
+cStruct* unbox_log_request_end(const mavlink_message_t* message);
+cStruct* unbox_actuator_output_status(const mavlink_message_t* message);
+cStruct* unbox_esc_status(const mavlink_message_t* message);
+cStruct* unbox_scaled_pressure2(const mavlink_message_t* message);
+cStruct* unbox_set_mode(const mavlink_message_t* message);
+cStruct* unbox_global_position_int(const mavlink_message_t* message);
+cStruct* unbox_canfd_frame(const mavlink_message_t* message);
+cStruct* unbox_optical_flow_rad(const mavlink_message_t* message);
+cStruct* unbox_gps_global_origin(const mavlink_message_t* message);
+cStruct* unbox_high_latency(const mavlink_message_t* message);
+cStruct* unbox_param_value(const mavlink_message_t* message);
+cStruct* unbox_attitude_target(const mavlink_message_t* message);
+cStruct* unbox_time_estimate_to_target(const mavlink_message_t* message);
+cStruct* unbox_camera_trigger(const mavlink_message_t* message);
+cStruct* unbox_system_time(const mavlink_message_t* message);
+cStruct* unbox_mission_item_reached(const mavlink_message_t* message);
+cStruct* unbox_log_entry(const mavlink_message_t* message);
+cStruct* unbox_link_node_status(const mavlink_message_t* message);
+cStruct* unbox_command_int(const mavlink_message_t* message);
+cStruct* unbox_position_target_local_ned(const mavlink_message_t* message);
+cStruct* unbox_rc_channels_override(const mavlink_message_t* message);
+cStruct* unbox_local_position_ned_cov(const mavlink_message_t* message);
+cStruct* unbox_raw_pressure(const mavlink_message_t* message);
+cStruct* unbox_home_position(const mavlink_message_t* message);
+cStruct* unbox_autopilot_version(const mavlink_message_t* message);
+cStruct* unbox_change_operator_control(const mavlink_message_t* message);
+cStruct* unbox_manual_setpoint(const mavlink_message_t* message);
+cStruct* unbox_scaled_imu(const mavlink_message_t* message);
+cStruct* unbox_wind_cov(const mavlink_message_t* message);
+cStruct* unbox_debug_vect(const mavlink_message_t* message);
+cStruct* unbox_gps_status(const mavlink_message_t* message);
+cStruct* unbox_flight_information(const mavlink_message_t* message);
+cStruct* unbox_scaled_pressure(const mavlink_message_t* message);
+cStruct* unbox_set_attitude_target(const mavlink_message_t* message);
+cStruct* unbox_ais_vessel(const mavlink_message_t* message);
+cStruct* unbox_att_pos_mocap(const mavlink_message_t* message);
+cStruct* unbox_hil_state_quaternion(const mavlink_message_t* message);
+cStruct* unbox_landing_target(const mavlink_message_t* message);
+cStruct* unbox_param_ext_request_read(const mavlink_message_t* message);
+cStruct* unbox_button_change(const mavlink_message_t* message);
+cStruct* unbox_attitude_quaternion_cov(const mavlink_message_t* message);
+cStruct* unbox_open_drone_id_system_update(const mavlink_message_t* message);
+cStruct* unbox_gimbal_manager_set_attitude(const mavlink_message_t* message);
+cStruct* unbox_mission_ack(const mavlink_message_t* message);
+cStruct* unbox_global_vision_position_estimate(const mavlink_message_t* message);
+cStruct* unbox_local_position_ned(const mavlink_message_t* message);
+cStruct* unbox_encapsulated_data(const mavlink_message_t* message);
+cStruct* unbox_set_position_target_local_ned(const mavlink_message_t* message);
+cStruct* unbox_open_drone_id_self_id(const mavlink_message_t* message);
+cStruct* unbox_efi_status(const mavlink_message_t* message);
+cStruct* unbox_mission_clear_all(const mavlink_message_t* message);
+cStruct* unbox_sys_status(const mavlink_message_t* message);
+cStruct* unbox_estimator_status(const mavlink_message_t* message);
+cStruct* unbox_set_position_target_global_int(const mavlink_message_t* message);
+cStruct* unbox_data_stream(const mavlink_message_t* message);
+cStruct* unbox_timesync(const mavlink_message_t* message);
+cStruct* unbox_camera_tracking_geo_status(const mavlink_message_t* message);
+cStruct* unbox_gps_rtcm_data(const mavlink_message_t* message);
+cStruct* unbox_camera_settings(const mavlink_message_t* message);
+cStruct* unbox_video_stream_information(const mavlink_message_t* message);
+cStruct* unbox_resource_request(const mavlink_message_t* message);
+cStruct* unbox_request_data_stream(const mavlink_message_t* message);
+cStruct* unbox_open_drone_id_system(const mavlink_message_t* message);
+cStruct* unbox_set_gps_global_origin(const mavlink_message_t* message);
+cStruct* unbox_param_request_list(const mavlink_message_t* message);
+cStruct* unbox_serial_control(const mavlink_message_t* message);
+cStruct* unbox_nav_controller_output(const mavlink_message_t* message);
+cStruct* unbox_raw_rpm(const mavlink_message_t* message);
+cStruct* unbox_log_erase(const mavlink_message_t* message);
+cStruct* unbox_high_latency2(const mavlink_message_t* message);
+cStruct* unbox_storage_information(const mavlink_message_t* message);
+cStruct* unbox_ping(const mavlink_message_t* message);
+cStruct* unbox_rc_channels_scaled(const mavlink_message_t* message);
+cStruct* unbox_orbit_execution_status(const mavlink_message_t* message);
+cStruct* unbox_debug_float_array(const mavlink_message_t* message);
+cStruct* unbox_command_ack(const mavlink_message_t* message);
+cStruct* unbox_supported_tunes(const mavlink_message_t* message);
+cStruct* unbox_adsb_vehicle(const mavlink_message_t* message);
+cStruct* unbox_set_home_position(const mavlink_message_t* message);
+cStruct* unbox_gps_raw_int(const mavlink_message_t* message);
+cStruct* unbox_mission_request_list(const mavlink_message_t* message);
+cStruct* unbox_servo_output_raw(const mavlink_message_t* message);
+cStruct* unbox_logging_ack(const mavlink_message_t* message);
+cStruct* unbox_can_frame(const mavlink_message_t* message);
+cStruct* unbox_debug(const mavlink_message_t* message);
+cStruct* unbox_radio_status(const mavlink_message_t* message);
+cStruct* unbox_gimbal_device_set_attitude(const mavlink_message_t* message);
+cStruct* unbox_optical_flow(const mavlink_message_t* message);
+cStruct* unbox_collision(const mavlink_message_t* message);
+cStruct* unbox_mission_request_int(const mavlink_message_t* message);
+cStruct* unbox_open_drone_id_authentication(const mavlink_message_t* message);
+cStruct* unbox_generator_status(const mavlink_message_t* message);
+cStruct* unbox_camera_capture_status(const mavlink_message_t* message);
+cStruct* unbox_mission_request(const mavlink_message_t* message);
+cStruct* unbox_attitude_quaternion(const mavlink_message_t* message);
+cStruct* unbox_obstacle_distance(const mavlink_message_t* message);
+cStruct* unbox_hil_state(const mavlink_message_t* message);
+cStruct* unbox_gimbal_manager_status(const mavlink_message_t* message);
+cStruct* unbox_trajectory_representation_waypoints(const mavlink_message_t* message);
+cStruct* unbox_auth_key(const mavlink_message_t* message);
+cStruct* unbox_terrain_check(const mavlink_message_t* message);
+cStruct* unbox_gps_inject_data(const mavlink_message_t* message);
+cStruct* unbox_scaled_imu3(const mavlink_message_t* message);
+cStruct* unbox_battery_status(const mavlink_message_t* message);
+cStruct* unbox_open_drone_id_basic_id(const mavlink_message_t* message);
+cStruct* unbox_param_map_rc(const mavlink_message_t* message);
+cStruct* unbox_hil_controls(const mavlink_message_t* message);
+cStruct* unbox_gps_input(const mavlink_message_t* message);
+cStruct* unbox_gps2_rtk(const mavlink_message_t* message);
+cStruct* unbox_set_actuator_control_target(const mavlink_message_t* message);
+cStruct* unbox_named_value_float(const mavlink_message_t* message);
+cStruct* unbox_wheel_distance(const mavlink_message_t* message);
+cStruct* unbox_onboard_computer_status(const mavlink_message_t* message);
+cStruct* unbox_rc_channels_raw(const mavlink_message_t* message);
+cStruct* unbox_mission_item_int(const mavlink_message_t* message);
+cStruct* unbox_log_request_list(const mavlink_message_t* message);
+cStruct* unbox_safety_allowed_area(const mavlink_message_t* message);
+cStruct* unbox_tunnel(const mavlink_message_t* message);
+cStruct* unbox_global_position_int_cov(const mavlink_message_t* message);
+cStruct* unbox_camera_information(const mavlink_message_t* message);
+cStruct* unbox_gimbal_device_information(const mavlink_message_t* message);
+cStruct* unbox_terrain_request(const mavlink_message_t* message);
+cStruct* unbox_command_long(const mavlink_message_t* message);
+cStruct* unbox_camera_tracking_image_status(const mavlink_message_t* message);
+cStruct* unbox_vfr_hud(const mavlink_message_t* message);
+cStruct* unbox_log_data(const mavlink_message_t* message);
+cStruct* unbox_can_filter_modify(const mavlink_message_t* message);
+cStruct* unbox_vicon_position_estimate(const mavlink_message_t* message);
+cStruct* unbox_mission_request_partial_list(const mavlink_message_t* message);
+cStruct* unbox_logging_data(const mavlink_message_t* message);
+cStruct* unbox_raw_imu(const mavlink_message_t* message);
+cStruct* unbox_open_drone_id_arm_status(const mavlink_message_t* message);
+cStruct* unbox_mission_item(const mavlink_message_t* message);
+cStruct* unbox_open_drone_id_location(const mavlink_message_t* message);
+cStruct* unbox_response_event_error(const mavlink_message_t* message);
+cStruct* unbox_smart_battery_info(const mavlink_message_t* message);
+cStruct* unbox_mission_write_partial_list(const mavlink_message_t* message);
+cStruct* unbox_sim_state(const mavlink_message_t* message);
+cStruct* unbox_mission_count(const mavlink_message_t* message);
+cStruct* unbox_memory_vect(const mavlink_message_t* message);
+cStruct* unbox_position_target_global_int(const mavlink_message_t* message);
+cStruct* unbox_altitude(const mavlink_message_t* message);
+cStruct* unbox_sens_mppt(const mavlink_message_t* message);
 cStruct* unbox_command_int_stamped(const mavlink_message_t* message);
+cStruct* unbox_sens_batmon(const mavlink_message_t* message);
+cStruct* unbox_aslctrl_debug(const mavlink_message_t* message);
 cStruct* unbox_sens_atmos(const mavlink_message_t* message);
-cStruct* unbox_gsm_link_status(const mavlink_message_t* message);
 cStruct* unbox_satcom_link_status(const mavlink_message_t* message);
-cStruct* unbox_sens_power_board(const mavlink_message_t* message);
-cStruct* unbox_sens_mppt(const mavlink_message_t* message);
-cStruct* unbox_asl_obctrl(const mavlink_message_t* message);
-cStruct* unbox_sensorpod_status(const mavlink_message_t* message);
+cStruct* unbox_fw_soaring_data(const mavlink_message_t* message);
 cStruct* unbox_aslctrl_data(const mavlink_message_t* message);
+cStruct* unbox_asluav_status(const mavlink_message_t* message);
+cStruct* unbox_sens_power_board(const mavlink_message_t* message);
+cStruct* unbox_gsm_link_status(const mavlink_message_t* message);
+cStruct* unbox_command_long_stamped(const mavlink_message_t* message);
+cStruct* unbox_sensor_airflow_angles(const mavlink_message_t* message);
 cStruct* unbox_ekf_ext(const mavlink_message_t* message);
-cStruct* unbox_fw_soaring_data(const mavlink_message_t* message);
-cStruct* unbox_avss_drone_operation_mode(const mavlink_message_t* message);
-cStruct* unbox_avss_drone_imu(const mavlink_message_t* message);
-cStruct* unbox_avss_prs_sys_status(const mavlink_message_t* message);
-cStruct* unbox_avss_drone_position(const mavlink_message_t* message);
-cStruct* unbox_osd_param_show_config_reply(const mavlink_message_t* message);
+cStruct* unbox_sensorpod_status(const mavlink_message_t* message);
+cStruct* unbox_sens_power(const mavlink_message_t* message);
+cStruct* unbox_asl_obctrl(const mavlink_message_t* message);
 cStruct* unbox_mag_cal_progress(const mavlink_message_t* message);
-cStruct* unbox_gopro_get_response(const mavlink_message_t* message);
-cStruct* unbox_data32(const mavlink_message_t* message);
-cStruct* unbox_rangefinder(const mavlink_message_t* message);
-cStruct* unbox_water_depth(const mavlink_message_t* message);
-cStruct* unbox_airspeed_autocal(const mavlink_message_t* message);
-cStruct* unbox_data96(const mavlink_message_t* message);
-cStruct* unbox_remote_log_data_block(const mavlink_message_t* message);
+cStruct* unbox_ahrs(const mavlink_message_t* message);
+cStruct* unbox_wind(const mavlink_message_t* message);
+cStruct* unbox_gopro_get_request(const mavlink_message_t* message);
+cStruct* unbox_rpm(const mavlink_message_t* message);
+cStruct* unbox_obstacle_distance_3d(const mavlink_message_t* message);
+cStruct* unbox_device_op_write_reply(const mavlink_message_t* message);
+cStruct* unbox_camera_feedback(const mavlink_message_t* message);
+cStruct* unbox_meminfo(const mavlink_message_t* message);
+cStruct* unbox_gopro_set_response(const mavlink_message_t* message);
+cStruct* unbox_device_op_read_reply(const mavlink_message_t* message);
+cStruct* unbox_camera_status(const mavlink_message_t* message);
+cStruct* unbox_pid_tuning(const mavlink_message_t* message);
 cStruct* unbox_set_mag_offsets(const mavlink_message_t* message);
-cStruct* unbox_gimbal_report(const mavlink_message_t* message);
+cStruct* unbox_rangefinder(const mavlink_message_t* message);
+cStruct* unbox_mount_control(const mavlink_message_t* message);
 cStruct* unbox_gimbal_torque_cmd_report(const mavlink_message_t* message);
-cStruct* unbox_simstate(const mavlink_message_t* message);
-cStruct* unbox_autopilot_version_request(const mavlink_message_t* message);
-cStruct* unbox_esc_telemetry_5_to_8(const mavlink_message_t* message);
-cStruct* unbox_vision_position_delta(const mavlink_message_t* message);
-cStruct* unbox_device_op_read_reply(const mavlink_message_t* message);
-cStruct* unbox_device_op_read(const mavlink_message_t* message);
 cStruct* unbox_fence_fetch_point(const mavlink_message_t* message);
-cStruct* unbox_device_op_write(const mavlink_message_t* message);
-cStruct* unbox_ahrs(const mavlink_message_t* message);
-cStruct* unbox_mount_control(const mavlink_message_t* message);
 cStruct* unbox_ekf_status_report(const mavlink_message_t* message);
-cStruct* unbox_camera_feedback(const mavlink_message_t* message);
+cStruct* unbox_data96(const mavlink_message_t* message);
+cStruct* unbox_osd_param_show_config(const mavlink_message_t* message);
+cStruct* unbox_ahrs3(const mavlink_message_t* message);
+cStruct* unbox_limits_status(const mavlink_message_t* message);
 cStruct* unbox_gopro_set_request(const mavlink_message_t* message);
-cStruct* unbox_mount_status(const mavlink_message_t* message);
-cStruct* unbox_gopro_heartbeat(const mavlink_message_t* message);
+cStruct* unbox_sensor_offsets(const mavlink_message_t* message);
+cStruct* unbox_ahrs2(const mavlink_message_t* message);
+cStruct* unbox_data32(const mavlink_message_t* message);
+cStruct* unbox_gimbal_report(const mavlink_message_t* message);
+cStruct* unbox_hwstatus(const mavlink_message_t* message);
+cStruct* unbox_vision_position_delta(const mavlink_message_t* message);
+cStruct* unbox_osd_param_config(const mavlink_message_t* message);
+cStruct* unbox_led_control(const mavlink_message_t* message);
 cStruct* unbox_data64(const mavlink_message_t* message);
-cStruct* unbox_gimbal_control(const mavlink_message_t* message);
-cStruct* unbox_mcu_status(const mavlink_message_t* message);
-cStruct* unbox_aoa_ssa(const mavlink_message_t* message);
-cStruct* unbox_rpm(const mavlink_message_t* message);
+cStruct* unbox_battery2(const mavlink_message_t* message);
 cStruct* unbox_rally_point(const mavlink_message_t* message);
-cStruct* unbox_data16(const mavlink_message_t* message);
-cStruct* unbox_limits_status(const mavlink_message_t* message);
-cStruct* unbox_pid_tuning(const mavlink_message_t* message);
-cStruct* unbox_digicam_control(const mavlink_message_t* message);
-cStruct* unbox_wind(const mavlink_message_t* message);
-cStruct* unbox_gopro_set_response(const mavlink_message_t* message);
-cStruct* unbox_compassmot_status(const mavlink_message_t* message);
-cStruct* unbox_ahrs3(const mavlink_message_t* message);
-cStruct* unbox_remote_log_block_status(const mavlink_message_t* message);
-cStruct* unbox_rally_fetch_point(const mavlink_message_t* message);
-cStruct* unbox_ahrs2(const mavlink_message_t* message);
-cStruct* unbox_osd_param_show_config(const mavlink_message_t* message);
+cStruct* unbox_aoa_ssa(const mavlink_message_t* message);
 cStruct* unbox_deepstall(const mavlink_message_t* message);
-cStruct* unbox_device_op_write_reply(const mavlink_message_t* message);
-cStruct* unbox_osd_param_config_reply(const mavlink_message_t* message);
-cStruct* unbox_camera_status(const mavlink_message_t* message);
+cStruct* unbox_digicam_configure(const mavlink_message_t* message);
+cStruct* unbox_remote_log_block_status(const mavlink_message_t* message);
+cStruct* unbox_data16(const mavlink_message_t* message);
+cStruct* unbox_autopilot_version_request(const mavlink_message_t* message);
+cStruct* unbox_esc_telemetry_9_to_12(const mavlink_message_t* message);
 cStruct* unbox_fence_point(const mavlink_message_t* message);
+cStruct* unbox_compassmot_status(const mavlink_message_t* message);
+cStruct* unbox_gopro_get_response(const mavlink_message_t* message);
+cStruct* unbox_mount_status(const mavlink_message_t* message);
 cStruct* unbox_radio(const mavlink_message_t* message);
-cStruct* unbox_obstacle_distance_3d(const mavlink_message_t* message);
-cStruct* unbox_meminfo(const mavlink_message_t* message);
+cStruct* unbox_osd_param_config_reply(const mavlink_message_t* message);
+cStruct* unbox_remote_log_data_block(const mavlink_message_t* message);
+cStruct* unbox_digicam_control(const mavlink_message_t* message);
+cStruct* unbox_water_depth(const mavlink_message_t* message);
 cStruct* unbox_mount_configure(const mavlink_message_t* message);
-cStruct* unbox_led_control(const mavlink_message_t* message);
-cStruct* unbox_adap_tuning(const mavlink_message_t* message);
-cStruct* unbox_battery2(const mavlink_message_t* message);
-cStruct* unbox_osd_param_config(const mavlink_message_t* message);
+cStruct* unbox_esc_telemetry_5_to_8(const mavlink_message_t* message);
+cStruct* unbox_device_op_write(const mavlink_message_t* message);
 cStruct* unbox_ap_adc(const mavlink_message_t* message);
-cStruct* unbox_sensor_offsets(const mavlink_message_t* message);
-cStruct* unbox_digicam_configure(const mavlink_message_t* message);
+cStruct* unbox_device_op_read(const mavlink_message_t* message);
+cStruct* unbox_simstate(const mavlink_message_t* message);
+cStruct* unbox_rally_fetch_point(const mavlink_message_t* message);
 cStruct* unbox_esc_telemetry_1_to_4(const mavlink_message_t* message);
-cStruct* unbox_esc_telemetry_9_to_12(const mavlink_message_t* message);
-cStruct* unbox_hwstatus(const mavlink_message_t* message);
-cStruct* unbox_gopro_get_request(const mavlink_message_t* message);
-cStruct* unbox_storm32_gimbal_manager_correct_roll(const mavlink_message_t* message);
-cStruct* unbox_radio_rc_channels(const mavlink_message_t* message);
-cStruct* unbox_param_value_array(const mavlink_message_t* message);
-cStruct* unbox_storm32_gimbal_manager_information(const mavlink_message_t* message);
-cStruct* unbox_radio_link_stats(const mavlink_message_t* message);
-cStruct* unbox_frsky_passthrough_array(const mavlink_message_t* message);
-cStruct* unbox_storm32_gimbal_manager_control(const mavlink_message_t* message);
-cStruct* unbox_storm32_gimbal_manager_control_pitchyaw(const mavlink_message_t* message);
-cStruct* unbox_storm32_gimbal_manager_status(const mavlink_message_t* message);
-cStruct* unbox_qshot_status(const mavlink_message_t* message);
-cStruct* unbox_cubepilot_raw_rc(const mavlink_message_t* message);
+cStruct* unbox_adap_tuning(const mavlink_message_t* message);
+cStruct* unbox_gopro_heartbeat(const mavlink_message_t* message);
+cStruct* unbox_airspeed_autocal(const mavlink_message_t* message);
+cStruct* unbox_osd_param_show_config_reply(const mavlink_message_t* message);
+cStruct* unbox_gimbal_control(const mavlink_message_t* message);
+cStruct* unbox_mcu_status(const mavlink_message_t* message);
 cStruct* unbox_cubepilot_firmware_update_resp(const mavlink_message_t* message);
+cStruct* unbox_cubepilot_raw_rc(const mavlink_message_t* message);
 cStruct* unbox_herelink_video_stream_information(const mavlink_message_t* message);
 cStruct* unbox_herelink_telem(const mavlink_message_t* message);
 cStruct* unbox_cubepilot_firmware_update_start(const mavlink_message_t* message);
-cStruct* unbox_uavionix_adsb_out_dynamic(const mavlink_message_t* message);
+cStruct* unbox_nav_filter_bias(const mavlink_message_t* message);
+cStruct* unbox_ualberta_sys_status(const mavlink_message_t* message);
+cStruct* unbox_radio_calibration(const mavlink_message_t* message);
+cStruct* unbox_icarous_heartbeat(const mavlink_message_t* message);
+cStruct* unbox_icarous_kinematic_bands(const mavlink_message_t* message);
+cStruct* unbox_storm32_gimbal_manager_correct_roll(const mavlink_message_t* message);
+cStruct* unbox_frsky_passthrough_array(const mavlink_message_t* message);
+cStruct* unbox_storm32_gimbal_manager_information(const mavlink_message_t* message);
+cStruct* unbox_param_value_array(const mavlink_message_t* message);
+cStruct* unbox_qshot_status(const mavlink_message_t* message);
+cStruct* unbox_radio_rc_channels(const mavlink_message_t* message);
+cStruct* unbox_storm32_gimbal_manager_control_pitchyaw(const mavlink_message_t* message);
+cStruct* unbox_storm32_gimbal_manager_status(const mavlink_message_t* message);
+cStruct* unbox_radio_link_stats(const mavlink_message_t* message);
+cStruct* unbox_storm32_gimbal_manager_control(const mavlink_message_t* message);
+cStruct* unbox_figure_eight_execution_status(const mavlink_message_t* message);
+cStruct* unbox_target_absolute(const mavlink_message_t* message);
+cStruct* unbox_wifi_network_info(const mavlink_message_t* message);
+cStruct* unbox_mission_checksum(const mavlink_message_t* message);
+cStruct* unbox_target_relative(const mavlink_message_t* message);
+cStruct* unbox_available_modes(const mavlink_message_t* message);
+cStruct* unbox_airspeed(const mavlink_message_t* message);
+cStruct* unbox_component_information_basic(const mavlink_message_t* message);
+cStruct* unbox_param_ack_transaction(const mavlink_message_t* message);
+cStruct* unbox_group_end(const mavlink_message_t* message);
+cStruct* unbox_current_mode(const mavlink_message_t* message);
+cStruct* unbox_battery_status_v2(const mavlink_message_t* message);
+cStruct* unbox_group_start(const mavlink_message_t* message);
+cStruct* unbox_protocol_version(const mavlink_message_t* message);
+cStruct* unbox_heartbeat(const mavlink_message_t* message);
 cStruct* unbox_uavionix_adsb_transceiver_health_report(const mavlink_message_t* message);
+cStruct* unbox_uavionix_adsb_out_dynamic(const mavlink_message_t* message);
 cStruct* unbox_uavionix_adsb_out_cfg(const mavlink_message_t* message);
-cStruct* unbox_array_test_6(const mavlink_message_t* message);
 cStruct* unbox_array_test_1(const mavlink_message_t* message);
-cStruct* unbox_array_test_3(const mavlink_message_t* message);
-cStruct* unbox_array_test_8(const mavlink_message_t* message);
 cStruct* unbox_array_test_7(const mavlink_message_t* message);
-cStruct* unbox_array_test_0(const mavlink_message_t* message);
-cStruct* unbox_array_test_5(const mavlink_message_t* message);
 cStruct* unbox_array_test_4(const mavlink_message_t* message);
-cStruct* unbox_protocol_version(const mavlink_message_t* message);
-cStruct* unbox_heartbeat(const mavlink_message_t* message);
+cStruct* unbox_array_test_5(const mavlink_message_t* message);
+cStruct* unbox_array_test_8(const mavlink_message_t* message);
+cStruct* unbox_array_test_6(const mavlink_message_t* message);
+cStruct* unbox_array_test_0(const mavlink_message_t* message);
+cStruct* unbox_array_test_3(const mavlink_message_t* message);
+cStruct* unbox_avss_drone_position(const mavlink_message_t* message);
+cStruct* unbox_avss_drone_operation_mode(const mavlink_message_t* message);
+cStruct* unbox_avss_drone_imu(const mavlink_message_t* message);
+cStruct* unbox_avss_prs_sys_status(const mavlink_message_t* message);
 cStruct* unbox_test_types(const mavlink_message_t* message);
-cStruct* unbox_radio_calibration(const mavlink_message_t* message);
-cStruct* unbox_ualberta_sys_status(const mavlink_message_t* message);
-cStruct* unbox_nav_filter_bias(const mavlink_message_t* message);
-cStruct* unbox_hygrometer_sensor(const mavlink_message_t* message);
-cStruct* unbox_local_position_ned(const mavlink_message_t* message);
-cStruct* unbox_ais_vessel(const mavlink_message_t* message);
-cStruct* unbox_gimbal_device_attitude_status(const mavlink_message_t* message);
-cStruct* unbox_mission_write_partial_list(const mavlink_message_t* message);
-cStruct* unbox_scaled_imu2(const mavlink_message_t* message);
-cStruct* unbox_vision_speed_estimate(const mavlink_message_t* message);
-cStruct* unbox_serial_control(const mavlink_message_t* message);
-cStruct* unbox_mission_set_current(const mavlink_message_t* message);
-cStruct* unbox_landing_target(const mavlink_message_t* message);
-cStruct* unbox_rc_channels(const mavlink_message_t* message);
-cStruct* unbox_command_ack(const mavlink_message_t* message);
-cStruct* unbox_autopilot_version(const mavlink_message_t* message);
-cStruct* unbox_safety_set_allowed_area(const mavlink_message_t* message);
-cStruct* unbox_memory_vect(const mavlink_message_t* message);
-cStruct* unbox_request_event(const mavlink_message_t* message);
-cStruct* unbox_rc_channels_scaled(const mavlink_message_t* message);
-cStruct* unbox_isbd_link_status(const mavlink_message_t* message);
-cStruct* unbox_gps_inject_data(const mavlink_message_t* message);
-cStruct* unbox_mission_item_int(const mavlink_message_t* message);
-cStruct* unbox_gimbal_device_information(const mavlink_message_t* message);
-cStruct* unbox_scaled_imu3(const mavlink_message_t* message);
-cStruct* unbox_manual_setpoint(const mavlink_message_t* message);
-cStruct* unbox_safety_allowed_area(const mavlink_message_t* message);
-cStruct* unbox_follow_target(const mavlink_message_t* message);
-cStruct* unbox_gps_rtcm_data(const mavlink_message_t* message);
-cStruct* unbox_rc_channels_raw(const mavlink_message_t* message);
-cStruct* unbox_hil_gps(const mavlink_message_t* message);
-cStruct* unbox_attitude(const mavlink_message_t* message);
-cStruct* unbox_component_metadata(const mavlink_message_t* message);
-cStruct* unbox_gps_raw_int(const mavlink_message_t* message);
-cStruct* unbox_mission_clear_all(const mavlink_message_t* message);
-cStruct* unbox_position_target_global_int(const mavlink_message_t* message);
-cStruct* unbox_manual_control(const mavlink_message_t* message);
-cStruct* unbox_camera_tracking_image_status(const mavlink_message_t* message);
-cStruct* unbox_debug(const mavlink_message_t* message);
-cStruct* unbox_video_stream_information(const mavlink_message_t* message);
-cStruct* unbox_mission_request_partial_list(const mavlink_message_t* message);
-cStruct* unbox_open_drone_id_arm_status(const mavlink_message_t* message);
-cStruct* unbox_param_set(const mavlink_message_t* message);
-cStruct* unbox_open_drone_id_authentication(const mavlink_message_t* message);
-cStruct* unbox_event(const mavlink_message_t* message);
-cStruct* unbox_set_attitude_target(const mavlink_message_t* message);
-cStruct* unbox_change_operator_control(const mavlink_message_t* message);
-cStruct* unbox_link_node_status(const mavlink_message_t* message);
-cStruct* unbox_v2_extension(const mavlink_message_t* message);
-cStruct* unbox_camera_information(const mavlink_message_t* message);
-cStruct* unbox_attitude_quaternion_cov(const mavlink_message_t* message);
-cStruct* unbox_collision(const mavlink_message_t* message);
-cStruct* unbox_hil_controls(const mavlink_message_t* message);
-cStruct* unbox_scaled_pressure2(const mavlink_message_t* message);
-cStruct* unbox_gimbal_device_set_attitude(const mavlink_message_t* message);
-cStruct* unbox_terrain_data(const mavlink_message_t* message);
-cStruct* unbox_supported_tunes(const mavlink_message_t* message);
-cStruct* unbox_can_filter_modify(const mavlink_message_t* message);
-cStruct* unbox_distance_sensor(const mavlink_message_t* message);
-cStruct* unbox_hil_state(const mavlink_message_t* message);
-cStruct* unbox_camera_capture_status(const mavlink_message_t* message);
-cStruct* unbox_canfd_frame(const mavlink_message_t* message);
-cStruct* unbox_flight_information(const mavlink_message_t* message);
-cStruct* unbox_logging_data_acked(const mavlink_message_t* message);
-cStruct* unbox_optical_flow(const mavlink_message_t* message);
-cStruct* unbox_command_cancel(const mavlink_message_t* message);
-cStruct* unbox_camera_image_captured(const mavlink_message_t* message);
-cStruct* unbox_set_position_target_global_int(const mavlink_message_t* message);
-cStruct* unbox_set_gps_global_origin(const mavlink_message_t* message);
-cStruct* unbox_statustext(const mavlink_message_t* message);
-cStruct* unbox_param_request_read(const mavlink_message_t* message);
-cStruct* unbox_adsb_vehicle(const mavlink_message_t* message);
-cStruct* unbox_high_latency(const mavlink_message_t* message);
-cStruct* unbox_wheel_distance(const mavlink_message_t* message);
-cStruct* unbox_extended_sys_state(const mavlink_message_t* message);
-cStruct* unbox_vibration(const mavlink_message_t* message);
-cStruct* unbox_obstacle_distance(const mavlink_message_t* message);
-cStruct* unbox_log_entry(const mavlink_message_t* message);
-cStruct* unbox_request_data_stream(const mavlink_message_t* message);
-cStruct* unbox_autopilot_state_for_gimbal_device(const mavlink_message_t* message);
-cStruct* unbox_open_drone_id_basic_id(const mavlink_message_t* message);
-cStruct* unbox_command_long(const mavlink_message_t* message);
-cStruct* unbox_named_value_int(const mavlink_message_t* message);
-cStruct* unbox_mission_item(const mavlink_message_t* message);
-cStruct* unbox_actuator_control_target(const mavlink_message_t* message);
-cStruct* unbox_storage_information(const mavlink_message_t* message);
-cStruct* unbox_time_estimate_to_target(const mavlink_message_t* message);
-cStruct* unbox_mission_ack(const mavlink_message_t* message);
-cStruct* unbox_position_target_local_ned(const mavlink_message_t* message);
-cStruct* unbox_trajectory_representation_waypoints(const mavlink_message_t* message);
-cStruct* unbox_local_position_ned_cov(const mavlink_message_t* message);
-cStruct* unbox_control_system_state(const mavlink_message_t* message);
-cStruct* unbox_orbit_execution_status(const mavlink_message_t* message);
-cStruct* unbox_efi_status(const mavlink_message_t* message);
-cStruct* unbox_debug_float_array(const mavlink_message_t* message);
-cStruct* unbox_response_event_error(const mavlink_message_t* message);
-cStruct* unbox_can_frame(const mavlink_message_t* message);
-cStruct* unbox_camera_settings(const mavlink_message_t* message);
-cStruct* unbox_nav_controller_output(const mavlink_message_t* message);
-cStruct* unbox_utm_global_position(const mavlink_message_t* message);
-cStruct* unbox_raw_imu(const mavlink_message_t* message);
-cStruct* unbox_camera_fov_status(const mavlink_message_t* message);
-cStruct* unbox_hil_rc_inputs_raw(const mavlink_message_t* message);
-cStruct* unbox_logging_ack(const mavlink_message_t* message);
-cStruct* unbox_timesync(const mavlink_message_t* message);
-cStruct* unbox_gps_global_origin(const mavlink_message_t* message);
-cStruct* unbox_debug_vect(const mavlink_message_t* message);
-cStruct* unbox_gimbal_manager_status(const mavlink_message_t* message);
-cStruct* unbox_actuator_output_status(const mavlink_message_t* message);
-cStruct* unbox_open_drone_id_system(const mavlink_message_t* message);
-cStruct* unbox_altitude(const mavlink_message_t* message);
-cStruct* unbox_vfr_hud(const mavlink_message_t* message);
-cStruct* unbox_terrain_report(const mavlink_message_t* message);
-cStruct* unbox_gimbal_manager_information(const mavlink_message_t* message);
-cStruct* unbox_cellular_status(const mavlink_message_t* message);
-cStruct* unbox_mag_cal_report(const mavlink_message_t* message);
-cStruct* unbox_raw_rpm(const mavlink_message_t* message);
-cStruct* unbox_param_value(const mavlink_message_t* message);
-cStruct* unbox_highres_imu(const mavlink_message_t* message);
-cStruct* unbox_hil_sensor(const mavlink_message_t* message);
-cStruct* unbox_rc_channels_override(const mavlink_message_t* message);
-cStruct* unbox_cellular_config(const mavlink_message_t* message);
-cStruct* unbox_gps2_rtk(const mavlink_message_t* message);
-cStruct* unbox_trajectory_representation_bezier(const mavlink_message_t* message);
-cStruct* unbox_log_request_end(const mavlink_message_t* message);
-cStruct* unbox_mission_request_int(const mavlink_message_t* message);
-cStruct* unbox_sys_status(const mavlink_message_t* message);
-cStruct* unbox_global_position_int_cov(const mavlink_message_t* message);
-cStruct* unbox_param_ext_request_list(const mavlink_message_t* message);
-cStruct* unbox_sim_state(const mavlink_message_t* message);
-cStruct* unbox_param_ext_set(const mavlink_message_t* message);
-cStruct* unbox_scaled_pressure(const mavlink_message_t* message);
-cStruct* unbox_terrain_request(const mavlink_message_t* message);
-cStruct* unbox_named_value_float(const mavlink_message_t* message);
-cStruct* unbox_radio_status(const mavlink_message_t* message);
-cStruct* unbox_wind_cov(const mavlink_message_t* message);
-cStruct* unbox_log_request_data(const mavlink_message_t* message);
-cStruct* unbox_param_ext_request_read(const mavlink_message_t* message);
-cStruct* unbox_system_time(const mavlink_message_t* message);
-cStruct* unbox_component_information(const mavlink_message_t* message);
-cStruct* unbox_global_vision_position_estimate(const mavlink_message_t* message);
-cStruct* unbox_open_drone_id_message_pack(const mavlink_message_t* message);
-cStruct* unbox_generator_status(const mavlink_message_t* message);
-cStruct* unbox_smart_battery_info(const mavlink_message_t* message);
-cStruct* unbox_esc_status(const mavlink_message_t* message);
-cStruct* unbox_battery_status(const mavlink_message_t* message);
-cStruct* unbox_ping(const mavlink_message_t* message);
-cStruct* unbox_estimator_status(const mavlink_message_t* message);
-cStruct* unbox_log_erase(const mavlink_message_t* message);
-cStruct* unbox_button_change(const mavlink_message_t* message);
-cStruct* unbox_data_stream(const mavlink_message_t* message);
-cStruct* unbox_set_mode(const mavlink_message_t* message);
-cStruct* unbox_gps_status(const mavlink_message_t* message);
-cStruct* unbox_attitude_quaternion(const mavlink_message_t* message);
-cStruct* unbox_current_event_sequence(const mavlink_message_t* message);
-cStruct* unbox_open_drone_id_self_id(const mavlink_message_t* message);
-cStruct* unbox_set_home_position(const mavlink_message_t* message);
-cStruct* unbox_gps_input(const mavlink_message_t* message);
-cStruct* unbox_hil_state_quaternion(const mavlink_message_t* message);
-cStruct* unbox_open_drone_id_location(const mavlink_message_t* message);
-cStruct* unbox_mission_request_list(const mavlink_message_t* message);
-cStruct* unbox_gimbal_manager_set_pitchyaw(const mavlink_message_t* message);
-cStruct* unbox_power_status(const mavlink_message_t* message);
-cStruct* unbox_hil_optical_flow(const mavlink_message_t* message);
-cStruct* unbox_resource_request(const mavlink_message_t* message);
-cStruct* unbox_gimbal_manager_set_attitude(const mavlink_message_t* message);
-cStruct* unbox_vicon_position_estimate(const mavlink_message_t* message);
-cStruct* unbox_set_actuator_control_target(const mavlink_message_t* message);
-cStruct* unbox_message_interval(const mavlink_message_t* message);
-cStruct* unbox_mission_current(const mavlink_message_t* message);
-cStruct* unbox_scaled_imu(const mavlink_message_t* message);
-cStruct* unbox_set_position_target_local_ned(const mavlink_message_t* message);
-cStruct* unbox_hil_actuator_controls(const mavlink_message_t* message);
-cStruct* unbox_command_int(const mavlink_message_t* message);
-cStruct* unbox_play_tune_v2(const mavlink_message_t* message);
-cStruct* unbox_mount_orientation(const mavlink_message_t* message);
-cStruct* unbox_global_position_int(const mavlink_message_t* message);
-cStruct* unbox_gps_rtk(const mavlink_message_t* message);
-cStruct* unbox_setup_signing(const mavlink_message_t* message);
-cStruct* unbox_param_ext_ack(const mavlink_message_t* message);
-cStruct* unbox_winch_status(const mavlink_message_t* message);
-cStruct* unbox_fence_status(const mavlink_message_t* message);
-cStruct* unbox_auth_key(const mavlink_message_t* message);
-cStruct* unbox_tunnel(const mavlink_message_t* message);
-cStruct* unbox_optical_flow_rad(const mavlink_message_t* message);
-cStruct* unbox_local_position_ned_system_global_offset(const mavlink_message_t* message);
-cStruct* unbox_param_map_rc(const mavlink_message_t* message);
-cStruct* unbox_log_data(const mavlink_message_t* message);
-cStruct* unbox_file_transfer_protocol(const mavlink_message_t* message);
-cStruct* unbox_encapsulated_data(const mavlink_message_t* message);
-cStruct* unbox_param_ext_value(const mavlink_message_t* message);
-cStruct* unbox_mission_request(const mavlink_message_t* message);
-cStruct* unbox_terrain_check(const mavlink_message_t* message);
-cStruct* unbox_uavcan_node_status(const mavlink_message_t* message);
-cStruct* unbox_camera_tracking_geo_status(const mavlink_message_t* message);
-cStruct* unbox_uavcan_node_info(const mavlink_message_t* message);
-cStruct* unbox_data_transmission_handshake(const mavlink_message_t* message);
-cStruct* unbox_mission_item_reached(const mavlink_message_t* message);
-cStruct* unbox_gps2_raw(const mavlink_message_t* message);
-cStruct* unbox_scaled_pressure3(const mavlink_message_t* message);
-cStruct* unbox_att_pos_mocap(const mavlink_message_t* message);
-cStruct* unbox_raw_pressure(const mavlink_message_t* message);
-cStruct* unbox_play_tune(const mavlink_message_t* message);
-cStruct* unbox_high_latency2(const mavlink_message_t* message);
-cStruct* unbox_camera_trigger(const mavlink_message_t* message);
-cStruct* unbox_gimbal_manager_set_manual_control(const mavlink_message_t* message);
-cStruct* unbox_log_request_list(const mavlink_message_t* message);
-cStruct* unbox_attitude_target(const mavlink_message_t* message);
-cStruct* unbox_change_operator_control_ack(const mavlink_message_t* message);
-cStruct* unbox_wifi_config_ap(const mavlink_message_t* message);
-cStruct* unbox_mission_count(const mavlink_message_t* message);
-cStruct* unbox_esc_info(const mavlink_message_t* message);
-cStruct* unbox_param_request_list(const mavlink_message_t* message);
-cStruct* unbox_onboard_computer_status(const mavlink_message_t* message);
-cStruct* unbox_home_position(const mavlink_message_t* message);
-cStruct* unbox_open_drone_id_system_update(const mavlink_message_t* message);
-cStruct* unbox_vision_position_estimate(const mavlink_message_t* message);
-cStruct* unbox_video_stream_status(const mavlink_message_t* message);
-cStruct* unbox_logging_data(const mavlink_message_t* message);
-cStruct* unbox_odometry(const mavlink_message_t* message);
-cStruct* unbox_servo_output_raw(const mavlink_message_t* message);
-cStruct* unbox_open_drone_id_operator_id(const mavlink_message_t* message);
```

### Comparing `UAVReaders-0.5.6/pyinterop.cpp` & `UAVReaders-0.6.2/pyinterop.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.36 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,18 +74,22 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -375,17 +379,14 @@
     operator T&() { return *ptr; }
     template<typename U> bool operator ==(U other) { return *ptr == other; }
     template<typename U> bool operator !=(U other) { return *ptr != other; }
   private:
     T *ptr;
 };
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -455,14 +456,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1953,14 +1959,31 @@
     Py_DECREF(none);
     return 0;
 #else
     return PyList_SetSlice(L, PY_SSIZE_T_MAX, PY_SSIZE_T_MAX, v);
 #endif
 }
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* None.proto */
 static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
 
 /* DivInt[long].proto */
 static CYTHON_INLINE long __Pyx_div_long(long, long);
 
 /* PySequenceContains.proto */
@@ -14660,15 +14683,15 @@
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(1, 724, __pyx_L1_error)
     }
   }
   #endif
 
@@ -20382,15 +20405,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_10UAVReaders_packet(PyObject *o) {
   struct __pyx_obj_10UAVReaders_packet *p = (struct __pyx_obj_10UAVReaders_packet *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   Py_CLEAR(p->protocol);
   PyObject_GC_Track(o);
@@ -20496,15 +20519,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_10UAVReaders_mavlink_reader(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_10UAVReaders_mavlink_reader *p;
   PyObject *o;
@@ -20522,15 +20545,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_10UAVReaders_mavlink_reader(PyObject *o) {
   struct __pyx_obj_10UAVReaders_mavlink_reader *p = (struct __pyx_obj_10UAVReaders_mavlink_reader *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -20633,15 +20656,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_10UAVReaders_data_flash_reader(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_10UAVReaders_data_flash_reader *p;
   PyObject *o;
@@ -20659,15 +20682,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_10UAVReaders_data_flash_reader(PyObject *o) {
   struct __pyx_obj_10UAVReaders_data_flash_reader *p = (struct __pyx_obj_10UAVReaders_data_flash_reader *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -20770,15 +20793,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10UAVReaders___pyx_scope_struct__thing_to_iterable *__pyx_freelist_10UAVReaders___pyx_scope_struct__thing_to_iterable[8];
 static int __pyx_freecount_10UAVReaders___pyx_scope_struct__thing_to_iterable = 0;
 
@@ -20888,15 +20911,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10UAVReaders___pyx_scope_struct_1_readFile *__pyx_freelist_10UAVReaders___pyx_scope_struct_1_readFile[8];
 static int __pyx_freecount_10UAVReaders___pyx_scope_struct_1_readFile = 0;
 
@@ -21021,15 +21044,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10UAVReaders___pyx_scope_struct_2___call__ *__pyx_freelist_10UAVReaders___pyx_scope_struct_2___call__[8];
 static int __pyx_freecount_10UAVReaders___pyx_scope_struct_2___call__ = 0;
 
@@ -21142,15 +21165,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10UAVReaders___pyx_scope_struct_3___call__ *__pyx_freelist_10UAVReaders___pyx_scope_struct_3___call__[8];
 static int __pyx_freecount_10UAVReaders___pyx_scope_struct_3___call__ = 0;
 
@@ -21263,15 +21286,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_array __pyx_vtable_array;
 
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_array_obj *p;
@@ -21292,15 +21315,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_array(PyObject *o) {
   struct __pyx_array_obj *p = (struct __pyx_array_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -21455,15 +21478,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
@@ -21477,15 +21500,15 @@
   p->name = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_Enum(PyObject *o) {
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -21577,15 +21600,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
@@ -21608,15 +21631,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_memoryview(PyObject *o) {
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -21841,15 +21864,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
@@ -21861,15 +21884,15 @@
   p->from_slice.memview = NULL;
   return o;
 }
 
 static void __pyx_tp_dealloc__memoryviewslice(PyObject *o) {
   struct __pyx_memoryviewslice_obj *p = (struct __pyx_memoryviewslice_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -21990,15 +22013,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -22545,14 +22568,19 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_512 = PyInt_FromLong(512); if (unlikely(!__pyx_int_512)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -24755,15 +24783,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -27198,15 +27229,15 @@
                         } else if (8 * sizeof(uint8_t) >= 4 * PyLong_SHIFT) {
                             return (uint8_t) (((((((((uint8_t)digits[3]) << PyLong_SHIFT) | (uint8_t)digits[2]) << PyLong_SHIFT) | (uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -27394,15 +27425,15 @@
                         } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
                             return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -28274,15 +28305,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -28470,15 +28501,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -28666,15 +28697,15 @@
                         } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
                             return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -29782,15 +29813,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_Generator_init(void) {
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
```

### Comparing `UAVReaders-0.5.6/readers.cpp` & `UAVReaders-0.6.2/readers.cpp`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.6/readers.h` & `UAVReaders-0.6.2/readers.h`

 * *Files 4% similar despite different names*

```diff
@@ -19,21 +19,23 @@
 #include "mavlink/common/mavlink.h"
 }
 
 
 namespace UAVFormatReaders {
 
 	class abstractReader {
+	public:
 		/* Interface for packet Readers */
 		virtual void parseByte(const uint8_t) = 0;
 		virtual void parseBuffer(const uint8_t *, uint64_t) = 0;
 		virtual int numAvailable() = 0;
 		virtual int bytesSeen() = 0;
 		virtual int  packetsSeen() = 0;
 		virtual introspect::Struct* getPacket() = 0;
+		virtual ~abstractReader() {};
 	};
 	
 	class dataFlashReader: public abstractReader {
 		DataFlash::DFParser parser;
 		DataFlash::DFPacket msg;
 		std::queue<introspect::Struct *> results;
 		bool hasData;
```

### Comparing `UAVReaders-0.5.6/setup.py` & `UAVReaders-0.6.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,13 +15,13 @@
         sources=["pyinterop.cpp"] + extrafiles
     )
 ]
 
 setup(
     ext_modules = cythonize(ext_modules),
     name="UAVReaders",
-    version="0.5.6",
+    version="0.6.2",
     author="Christian Clifford",
     author_email="cjclifford@alaska.edu",
     description="Parsers for UAV/Aerial Drone-related formats like MavLink and DataFlash",
     py_modules=[]
 )
```

### Comparing `UAVReaders-0.5.6/table.h` & `UAVReaders-0.6.2/table.h`

 * *Files identical despite different names*

