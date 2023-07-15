# Comparing `tmp/rosys-0.8.5.tar.gz` & `tmp/rosys-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosys-0.8.5.tar", max compression
+gzip compressed data, was "rosys-0.9.0.tar", max compression
```

## Comparing `rosys-0.8.5.tar` & `rosys-0.9.0.tar`

### file list

```diff
@@ -1,141 +1,147 @@
--rw-r--r--   0        0        0     1072 2023-06-08 12:01:04.604179 rosys-0.8.5/LICENSE
--rw-r--r--   0        0        0     6070 2023-06-08 12:01:04.604179 rosys-0.8.5/README.md
--rw-r--r--   0        0        0     1441 2023-06-08 12:01:21.784432 rosys-0.8.5/pyproject.toml
--rw-r--r--   0        0        0      445 2023-06-08 12:01:04.620179 rosys-0.8.5/rosys/__init__.py
--rw-r--r--   0        0        0      581 2023-06-08 12:01:04.620179 rosys-0.8.5/rosys/analysis/__init__.py
--rw-r--r--   0        0        0    86820 2023-06-08 12:01:04.620179 rosys-0.8.5/rosys/analysis/assets/RobotoMono-Medium.ttf
--rw-r--r--   0        0        0     1833 2023-06-08 12:01:04.620179 rosys-0.8.5/rosys/analysis/asyncio_warnings.py
--rw-r--r--   0        0        0      712 2023-06-08 12:01:04.620179 rosys-0.8.5/rosys/analysis/kpi_buckets.py
--rw-r--r--   0        0        0     2089 2023-06-08 12:01:04.620179 rosys-0.8.5/rosys/analysis/kpi_logger.py
--rw-r--r--   0        0        0     4477 2023-06-08 12:01:04.620179 rosys-0.8.5/rosys/analysis/kpi_page_.py
--rw-r--r--   0        0        0        0 2023-06-08 12:01:04.620179 rosys-0.8.5/rosys/analysis/legacy/__init__.py
--rw-r--r--   0        0        0     3226 2023-06-08 12:01:04.620179 rosys-0.8.5/rosys/analysis/legacy/asyncio_monitor.py
--rw-r--r--   0        0        0     1869 2023-06-08 12:01:04.620179 rosys-0.8.5/rosys/analysis/legacy/asyncio_page.py
--rw-r--r--   0        0        0      973 2023-06-08 12:01:04.620179 rosys-0.8.5/rosys/analysis/legacy/cpu_usage.py
--rw-r--r--   0        0        0     1202 2023-06-08 12:01:04.620179 rosys-0.8.5/rosys/analysis/legacy/lizard_stats.py
--rw-r--r--   0        0        0     1970 2023-06-08 12:01:04.620179 rosys-0.8.5/rosys/analysis/legacy/network_monitor.py
--rw-r--r--   0        0        0     2959 2023-06-08 12:01:04.620179 rosys-0.8.5/rosys/analysis/legacy/objgraph_page.py
--rw-r--r--   0        0        0      717 2023-06-08 12:01:04.620179 rosys-0.8.5/rosys/analysis/legacy/pyloot_page.py
--rw-r--r--   0        0        0     2455 2023-06-08 12:01:04.620179 rosys-0.8.5/rosys/analysis/memory.py
--rw-r--r--   0        0        0     1624 2023-06-08 12:01:04.620179 rosys-0.8.5/rosys/analysis/profile_button_.py
--rw-r--r--   0        0        0     1038 2023-06-08 12:01:04.620179 rosys-0.8.5/rosys/analysis/profiling.py
--rw-r--r--   0        0        0     4266 2023-06-08 12:01:04.620179 rosys-0.8.5/rosys/analysis/timelapse_recorder.py
--rw-r--r--   0        0        0      693 2023-06-08 12:01:04.620179 rosys-0.8.5/rosys/analysis/track.py
--rw-r--r--   0        0        0      768 2023-06-08 12:01:04.620179 rosys-0.8.5/rosys/analysis/videos_page_.py
--rw-r--r--   0        0        0      232 2023-06-08 12:01:04.620179 rosys-0.8.5/rosys/automation/__init__.py
--rw-r--r--   0        0        0     5083 2023-06-08 12:01:04.620179 rosys-0.8.5/rosys/automation/app_controls_.py
--rw-r--r--   0        0        0     2752 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/automation/automation.py
--rw-r--r--   0        0        0     1642 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/automation/automation_controls_.py
--rw-r--r--   0        0        0     5738 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/automation/automator.py
--rw-r--r--   0        0        0     9829 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/automation/schedule.py
--rw-r--r--   0        0        0      531 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/config.py
--rw-r--r--   0        0        0      397 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/driving/__init__.py
--rw-r--r--   0        0        0      194 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/driving/drivable.py
--rw-r--r--   0        0        0     7882 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/driving/driver.py
--rw-r--r--   0        0        0     1979 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/driving/driver_object.py
--rw-r--r--   0        0        0      643 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/driving/joystick_.py
--rw-r--r--   0        0        0     2242 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/driving/keyboard_control_.py
--rw-r--r--   0        0        0     3532 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/driving/odometer.py
--rw-r--r--   0        0        0      169 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/driving/path_segment.py
--rw-r--r--   0        0        0     1768 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/driving/robot_object_.py
--rw-r--r--   0        0        0     3088 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/driving/steerer.py
--rw-r--r--   0        0        0     2961 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/event.py
--rw-r--r--   0        0        0      295 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/geometry/__init__.py
--rw-r--r--   0        0        0     1193 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/geometry/line.py
--rw-r--r--   0        0        0     1629 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/geometry/line_segment.py
--rw-r--r--   0        0        0     1844 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/geometry/point.py
--rw-r--r--   0        0        0      915 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/geometry/point3d.py
--rw-r--r--   0        0        0     3696 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/geometry/pose.py
--rw-r--r--   0        0        0      344 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/geometry/prism.py
--rw-r--r--   0        0        0      640 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/geometry/rectangle.py
--rw-r--r--   0        0        0     1732 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/geometry/rotation.py
--rw-r--r--   0        0        0     8874 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/geometry/spline.py
--rw-r--r--   0        0        0      142 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/geometry/velocity.py
--rw-r--r--   0        0        0      606 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/hardware/__init__.py
--rw-r--r--   0        0        0      341 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/hardware/bluetooth.py
--rw-r--r--   0        0        0     3874 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/hardware/bms.py
--rw-r--r--   0        0        0     3105 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/hardware/bms_message.py
--rw-r--r--   0        0        0      770 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/hardware/bms_state.py
--rw-r--r--   0        0        0     2216 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/hardware/bumper.py
--rw-r--r--   0        0        0      657 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/hardware/can.py
--rw-r--r--   0        0        0      143 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/hardware/communication/__init__.py
--rw-r--r--   0        0        0      751 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/hardware/communication/communication.py
--rw-r--r--   0        0        0     3066 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/hardware/communication/serial_communication.py
--rw-r--r--   0        0        0     1434 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/hardware/communication/web_communication.py
--rw-r--r--   0        0        0     1564 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/hardware/estop.py
--rw-r--r--   0        0        0      637 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/hardware/expander.py
--rwxr-xr-x   0        0        0     1123 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/hardware/hardware_proxy.py
--rw-r--r--   0        0        0     4837 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/hardware/lizard_firmware.py
--rw-r--r--   0        0        0      830 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/hardware/module.py
--rw-r--r--   0        0        0     2609 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/hardware/robot.py
--rw-r--r--   0        0        0     8065 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/hardware/robot_brain.py
--rw-r--r--   0        0        0      607 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/hardware/serial.py
--rw-r--r--   0        0        0     4434 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/hardware/wheels.py
--rw-r--r--   0        0        0     2082 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/helpers.py
--rw-r--r--   0        0        0      260 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/__init__.py
--rw-r--r--   0        0        0      236 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/area.py
--rw-r--r--   0        0        0     1013 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/area_object_.py
--rw-r--r--   0        0        0     1372 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/binary_renderer.py
--rwxr-xr-x   0        0        0     1094 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/binary_renderer_demo.py
--rw-r--r--   0        0        0    13904 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/delaunay_planner.py
--rw-r--r--   0        0        0      220 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/delaunay_pose_group.py
--rw-r--r--   0        0        0     2831 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/demos/20220714-1.py
--rw-r--r--   0        0        0     2943 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/demos/20220714-2-A.py
--rw-r--r--   0        0        0     2939 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/demos/20220714-2-B.py
--rw-r--r--   0        0        0     2940 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/demos/20220714-3.py
--rw-r--r--   0        0        0     3196 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/demos/20220725-1.py
--rw-r--r--   0        0        0    38753 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/demos/20220825-1.py
--rw-r--r--   0        0        0    16920 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/demos/20220916-1.py
--rw-r--r--   0        0        0     3907 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/demos/20220921-1.py
--rw-r--r--   0        0        0     4217 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/demos/20221121-1.py
--rw-r--r--   0        0        0     4220 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/demos/20221203-1.py
--rw-r--r--   0        0        0    32139 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/demos/20230120-1.py
--rw-r--r--   0        0        0     2948 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/distance_map.py
--rwxr-xr-x   0        0        0     1757 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/distance_map_demo.py
--rw-r--r--   0        0        0     1815 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/experiments.py
--rwxr-xr-x   0        0        0      473 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/experiments_demo.py
--rw-r--r--   0        0        0     1885 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/fast_spline.py
--rw-r--r--   0        0        0     1980 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/grid.py
--rwxr-xr-x   0        0        0      466 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/grid_demo.py
--rw-r--r--   0        0        0      156 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/obstacle.py
--rw-r--r--   0        0        0     4126 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/obstacle_map.py
--rwxr-xr-x   0        0        0     1253 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/obstacle_map_demo.py
--rw-r--r--   0        0        0      751 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/obstacle_object_.py
--rw-r--r--   0        0        0      856 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/path_object_.py
--rw-r--r--   0        0        0     5210 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/path_planner.py
--rwxr-xr-x   0        0        0     2962 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/planner_demo.py
--rw-r--r--   0        0        0     3073 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/planner_process.py
--rw-r--r--   0        0        0     1955 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/plot_tools.py
--rwxr-xr-x   0        0        0     1237 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/plot_tools_demo.py
--rw-r--r--   0        0        0     1020 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/robot_renderer.py
--rwxr-xr-x   0        0        0      622 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/robot_renderer_demo.py
--rw-r--r--   0        0        0     2759 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/steps.py
--rwxr-xr-x   0        0        0     1749 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/pathplanning/steps_demo.py
--rw-r--r--   0        0        0     3959 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/persistence.py
--rw-r--r--   0        0        0     7764 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/rosys.py
--rw-r--r--   0        0        0     4291 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/run.py
--rw-r--r--   0        0        0      708 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/simulation_ui.py
--rw-r--r--   0        0        0       52 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/system/__init__.py
--rw-r--r--   0        0        0     2221 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/system/wifi_button_.py
--rw-r--r--   0        0        0      194 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/test/__init__.py
--rw-r--r--   0        0        0     4404 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/test/helpers.py
--rw-r--r--   0        0        0     2615 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/test/log_configuration.py
--rw-r--r--   0        0        0      728 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/vision/__init__.py
--rw-r--r--   0        0        0     5066 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/vision/calibration.py
--rw-r--r--   0        0        0     1819 2023-06-08 12:01:04.624179 rosys-0.8.5/rosys/vision/camera.py
--rw-r--r--   0        0        0     4576 2023-06-08 12:01:04.628179 rosys-0.8.5/rosys/vision/camera_objects_.py
--rw-r--r--   0        0        0     2725 2023-06-08 12:01:04.628179 rosys-0.8.5/rosys/vision/camera_projector.py
--rw-r--r--   0        0        0     2841 2023-06-08 12:01:04.628179 rosys-0.8.5/rosys/vision/camera_provider.py
--rw-r--r--   0        0        0     4214 2023-06-08 12:01:04.628179 rosys-0.8.5/rosys/vision/detections.py
--rw-r--r--   0        0        0     1497 2023-06-08 12:01:04.628179 rosys-0.8.5/rosys/vision/detector.py
--rw-r--r--   0        0        0     6059 2023-06-08 12:01:04.628179 rosys-0.8.5/rosys/vision/detector_hardware.py
--rw-r--r--   0        0        0     4620 2023-06-08 12:01:04.628179 rosys-0.8.5/rosys/vision/detector_simulation.py
--rw-r--r--   0        0        0     1325 2023-06-08 12:01:04.628179 rosys-0.8.5/rosys/vision/image.py
--rw-r--r--   0        0        0     2240 2023-06-08 12:01:04.628179 rosys-0.8.5/rosys/vision/image_route.py
--rw-r--r--   0        0        0      612 2023-06-08 12:01:04.628179 rosys-0.8.5/rosys/vision/multi_camera_provider.py
--rw-r--r--   0        0        0     1004 2023-06-08 12:01:04.628179 rosys-0.8.5/rosys/vision/uploads.py
--rw-r--r--   0        0        0     1699 2023-06-08 12:01:04.628179 rosys-0.8.5/rosys/vision/usb_camera.py
--rw-r--r--   0        0        0    11647 2023-06-08 12:01:04.628179 rosys-0.8.5/rosys/vision/usb_camera_provider_hardware.py
--rw-r--r--   0        0        0     3126 2023-06-08 12:01:04.628179 rosys-0.8.5/rosys/vision/usb_camera_provider_simulation.py
--rw-r--r--   0        0        0     8006 1970-01-01 00:00:00.000000 rosys-0.8.5/setup.py
--rw-r--r--   0        0        0     8009 1970-01-01 00:00:00.000000 rosys-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-15 05:19:47.596301 rosys-0.9.0/LICENSE
+-rw-r--r--   0        0        0     6070 2023-07-15 05:19:47.596301 rosys-0.9.0/README.md
+-rw-r--r--   0        0        0     1545 2023-07-15 05:19:58.940461 rosys-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      445 2023-07-15 05:19:47.616301 rosys-0.9.0/rosys/__init__.py
+-rw-r--r--   0        0        0      581 2023-07-15 05:19:47.616301 rosys-0.9.0/rosys/analysis/__init__.py
+-rw-r--r--   0        0        0    86820 2023-07-15 05:19:47.616301 rosys-0.9.0/rosys/analysis/assets/RobotoMono-Medium.ttf
+-rw-r--r--   0        0        0     1833 2023-07-15 05:19:47.616301 rosys-0.9.0/rosys/analysis/asyncio_warnings.py
+-rw-r--r--   0        0        0      721 2023-07-15 05:19:47.616301 rosys-0.9.0/rosys/analysis/kpi_buckets.py
+-rw-r--r--   0        0        0     2089 2023-07-15 05:19:47.616301 rosys-0.9.0/rosys/analysis/kpi_logger.py
+-rw-r--r--   0        0        0     4477 2023-07-15 05:19:47.616301 rosys-0.9.0/rosys/analysis/kpi_page_.py
+-rw-r--r--   0        0        0        0 2023-07-15 05:19:47.616301 rosys-0.9.0/rosys/analysis/legacy/__init__.py
+-rw-r--r--   0        0        0     3226 2023-07-15 05:19:47.616301 rosys-0.9.0/rosys/analysis/legacy/asyncio_monitor.py
+-rw-r--r--   0        0        0     1869 2023-07-15 05:19:47.616301 rosys-0.9.0/rosys/analysis/legacy/asyncio_page.py
+-rw-r--r--   0        0        0      973 2023-07-15 05:19:47.616301 rosys-0.9.0/rosys/analysis/legacy/cpu_usage.py
+-rw-r--r--   0        0        0     1202 2023-07-15 05:19:47.616301 rosys-0.9.0/rosys/analysis/legacy/lizard_stats.py
+-rw-r--r--   0        0        0     1970 2023-07-15 05:19:47.616301 rosys-0.9.0/rosys/analysis/legacy/network_monitor.py
+-rw-r--r--   0        0        0     2959 2023-07-15 05:19:47.616301 rosys-0.9.0/rosys/analysis/legacy/objgraph_page.py
+-rw-r--r--   0        0        0      717 2023-07-15 05:19:47.616301 rosys-0.9.0/rosys/analysis/legacy/pyloot_page.py
+-rw-r--r--   0        0        0     2455 2023-07-15 05:19:47.616301 rosys-0.9.0/rosys/analysis/memory.py
+-rw-r--r--   0        0        0     1624 2023-07-15 05:19:47.616301 rosys-0.9.0/rosys/analysis/profile_button_.py
+-rw-r--r--   0        0        0     1046 2023-07-15 05:19:47.616301 rosys-0.9.0/rosys/analysis/profiling.py
+-rw-r--r--   0        0        0     4266 2023-07-15 05:19:47.616301 rosys-0.9.0/rosys/analysis/timelapse_recorder.py
+-rw-r--r--   0        0        0      693 2023-07-15 05:19:47.616301 rosys-0.9.0/rosys/analysis/track.py
+-rw-r--r--   0        0        0      768 2023-07-15 05:19:47.616301 rosys-0.9.0/rosys/analysis/videos_page_.py
+-rw-r--r--   0        0        0      232 2023-07-15 05:19:47.616301 rosys-0.9.0/rosys/automation/__init__.py
+-rw-r--r--   0        0        0     5083 2023-07-15 05:19:47.616301 rosys-0.9.0/rosys/automation/app_controls_.py
+-rw-r--r--   0        0        0     2752 2023-07-15 05:19:47.616301 rosys-0.9.0/rosys/automation/automation.py
+-rw-r--r--   0        0        0     1642 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/automation/automation_controls_.py
+-rw-r--r--   0        0        0     5972 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/automation/automator.py
+-rw-r--r--   0        0        0     9829 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/automation/schedule.py
+-rw-r--r--   0        0        0      599 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/config.py
+-rw-r--r--   0        0        0      397 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/driving/__init__.py
+-rw-r--r--   0        0        0      194 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/driving/drivable.py
+-rw-r--r--   0        0        0     7707 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/driving/driver.py
+-rw-r--r--   0        0        0     1979 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/driving/driver_object.py
+-rw-r--r--   0        0        0      643 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/driving/joystick_.py
+-rw-r--r--   0        0        0     2242 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/driving/keyboard_control_.py
+-rw-r--r--   0        0        0     3532 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/driving/odometer.py
+-rw-r--r--   0        0        0      169 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/driving/path_segment.py
+-rw-r--r--   0        0        0     1768 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/driving/robot_object_.py
+-rw-r--r--   0        0        0     3088 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/driving/steerer.py
+-rw-r--r--   0        0        0     3054 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/event.py
+-rw-r--r--   0        0        0      295 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/geometry/__init__.py
+-rw-r--r--   0        0        0     1193 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/geometry/line.py
+-rw-r--r--   0        0        0     1629 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/geometry/line_segment.py
+-rw-r--r--   0        0        0     1844 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/geometry/point.py
+-rw-r--r--   0        0        0      915 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/geometry/point3d.py
+-rw-r--r--   0        0        0     3954 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/geometry/pose.py
+-rw-r--r--   0        0        0      344 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/geometry/prism.py
+-rw-r--r--   0        0        0      658 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/geometry/rectangle.py
+-rw-r--r--   0        0        0     1746 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/geometry/rotation.py
+-rw-r--r--   0        0        0     8874 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/geometry/spline.py
+-rw-r--r--   0        0        0      142 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/geometry/velocity.py
+-rw-r--r--   0        0        0      687 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/hardware/__init__.py
+-rw-r--r--   0        0        0     1058 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/hardware/battery_control.py
+-rw-r--r--   0        0        0      341 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/hardware/bluetooth.py
+-rw-r--r--   0        0        0     3874 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/hardware/bms.py
+-rw-r--r--   0        0        0     3105 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/hardware/bms_message.py
+-rw-r--r--   0        0        0      770 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/hardware/bms_state.py
+-rw-r--r--   0        0        0     2226 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/hardware/bumper.py
+-rw-r--r--   0        0        0      657 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/hardware/can.py
+-rw-r--r--   0        0        0      143 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/hardware/communication/__init__.py
+-rw-r--r--   0        0        0      751 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/hardware/communication/communication.py
+-rw-r--r--   0        0        0     3858 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/hardware/communication/serial_communication.py
+-rw-r--r--   0        0        0     1454 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/hardware/communication/web_communication.py
+-rw-r--r--   0        0        0     1564 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/hardware/estop.py
+-rw-r--r--   0        0        0      637 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/hardware/expander.py
+-rwxr-xr-x   0        0        0     1123 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/hardware/hardware_proxy.py
+-rw-r--r--   0        0        0      266 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/hardware/imu.py
+-rw-r--r--   0        0        0     4837 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/hardware/lizard_firmware.py
+-rw-r--r--   0        0        0      858 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/hardware/module.py
+-rw-r--r--   0        0        0     2613 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/hardware/robot.py
+-rw-r--r--   0        0        0     8065 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/hardware/robot_brain.py
+-rw-r--r--   0        0        0      607 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/hardware/serial.py
+-rw-r--r--   0        0        0     4113 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/hardware/wheels.py
+-rw-r--r--   0        0        0     2906 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/helpers.py
+-rw-r--r--   0        0        0      260 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/__init__.py
+-rw-r--r--   0        0        0      236 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/area.py
+-rw-r--r--   0        0        0     1013 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/area_object_.py
+-rw-r--r--   0        0        0     1372 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/binary_renderer.py
+-rwxr-xr-x   0        0        0     1094 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/binary_renderer_demo.py
+-rw-r--r--   0        0        0    13904 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/delaunay_planner.py
+-rw-r--r--   0        0        0      220 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/delaunay_pose_group.py
+-rw-r--r--   0        0        0     2831 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/demos/20220714-1.py
+-rw-r--r--   0        0        0     2943 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/demos/20220714-2-A.py
+-rw-r--r--   0        0        0     2939 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/demos/20220714-2-B.py
+-rw-r--r--   0        0        0     2940 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/demos/20220714-3.py
+-rw-r--r--   0        0        0     3196 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/demos/20220725-1.py
+-rw-r--r--   0        0        0    38753 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/demos/20220825-1.py
+-rw-r--r--   0        0        0    16920 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/demos/20220916-1.py
+-rw-r--r--   0        0        0     3907 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/demos/20220921-1.py
+-rw-r--r--   0        0        0     4217 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/demos/20221121-1.py
+-rw-r--r--   0        0        0     4220 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/demos/20221203-1.py
+-rw-r--r--   0        0        0    32139 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/demos/20230120-1.py
+-rw-r--r--   0        0        0     3876 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/demos/20230605-1.py
+-rw-r--r--   0        0        0     2948 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/distance_map.py
+-rwxr-xr-x   0        0        0     1757 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/distance_map_demo.py
+-rw-r--r--   0        0        0     1815 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/experiments.py
+-rwxr-xr-x   0        0        0      473 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/experiments_demo.py
+-rw-r--r--   0        0        0     1885 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/fast_spline.py
+-rw-r--r--   0        0        0     1980 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/grid.py
+-rwxr-xr-x   0        0        0      466 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/grid_demo.py
+-rw-r--r--   0        0        0      156 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/obstacle.py
+-rw-r--r--   0        0        0     4126 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/obstacle_map.py
+-rwxr-xr-x   0        0        0     1253 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/obstacle_map_demo.py
+-rw-r--r--   0        0        0      751 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/obstacle_object_.py
+-rw-r--r--   0        0        0      856 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/path_object_.py
+-rw-r--r--   0        0        0     5210 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/path_planner.py
+-rwxr-xr-x   0        0        0     2974 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/planner_demo.py
+-rw-r--r--   0        0        0     3094 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/planner_process.py
+-rw-r--r--   0        0        0     1962 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/plot_tools.py
+-rwxr-xr-x   0        0        0     1237 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/plot_tools_demo.py
+-rw-r--r--   0        0        0     1020 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/robot_renderer.py
+-rwxr-xr-x   0        0        0      622 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/robot_renderer_demo.py
+-rw-r--r--   0        0        0     2759 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/steps.py
+-rwxr-xr-x   0        0        0     1749 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/pathplanning/steps_demo.py
+-rw-r--r--   0        0        0     3966 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/persistence.py
+-rw-r--r--   0        0        0     7766 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/rosys.py
+-rw-r--r--   0        0        0     4486 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/run.py
+-rw-r--r--   0        0        0      632 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/simulation_ui.py
+-rw-r--r--   0        0        0       52 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/system/__init__.py
+-rw-r--r--   0        0        0     2221 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/system/wifi_button_.py
+-rw-r--r--   0        0        0      194 2023-07-15 05:19:47.620301 rosys-0.9.0/rosys/test/__init__.py
+-rw-r--r--   0        0        0     4404 2023-07-15 05:19:47.624301 rosys-0.9.0/rosys/test/helpers.py
+-rw-r--r--   0        0        0     2615 2023-07-15 05:19:47.624301 rosys-0.9.0/rosys/test/log_configuration.py
+-rw-r--r--   0        0        0      897 2023-07-15 05:19:47.624301 rosys-0.9.0/rosys/vision/__init__.py
+-rw-r--r--   0        0        0     5066 2023-07-15 05:19:47.624301 rosys-0.9.0/rosys/vision/calibration.py
+-rw-r--r--   0        0        0     1951 2023-07-15 05:19:47.624301 rosys-0.9.0/rosys/vision/camera.py
+-rw-r--r--   0        0        0     4764 2023-07-15 05:19:47.624301 rosys-0.9.0/rosys/vision/camera_objects_.py
+-rw-r--r--   0        0        0     2771 2023-07-15 05:19:47.624301 rosys-0.9.0/rosys/vision/camera_projector.py
+-rw-r--r--   0        0        0     2909 2023-07-15 05:19:47.624301 rosys-0.9.0/rosys/vision/camera_provider.py
+-rw-r--r--   0        0        0      438 2023-07-15 05:19:47.624301 rosys-0.9.0/rosys/vision/combining_camera_provider.py
+-rw-r--r--   0        0        0     4282 2023-07-15 05:19:47.624301 rosys-0.9.0/rosys/vision/detections.py
+-rw-r--r--   0        0        0     1497 2023-07-15 05:19:47.624301 rosys-0.9.0/rosys/vision/detector.py
+-rw-r--r--   0        0        0     6059 2023-07-15 05:19:47.624301 rosys-0.9.0/rosys/vision/detector_hardware.py
+-rw-r--r--   0        0        0     4780 2023-07-15 05:19:47.624301 rosys-0.9.0/rosys/vision/detector_simulation.py
+-rw-r--r--   0        0        0     1325 2023-07-15 05:19:47.624301 rosys-0.9.0/rosys/vision/image.py
+-rw-r--r--   0        0        0     2240 2023-07-15 05:19:47.624301 rosys-0.9.0/rosys/vision/image_route.py
+-rw-r--r--   0        0        0      612 2023-07-15 05:19:47.624301 rosys-0.9.0/rosys/vision/multi_camera_provider.py
+-rw-r--r--   0        0        0     2549 2023-07-15 05:19:47.624301 rosys-0.9.0/rosys/vision/rtsp_camera.py
+-rw-r--r--   0        0        0     9184 2023-07-15 05:19:47.624301 rosys-0.9.0/rosys/vision/rtsp_camera_provider_hardware.py
+-rw-r--r--   0        0        0     1004 2023-07-15 05:19:47.624301 rosys-0.9.0/rosys/vision/uploads.py
+-rw-r--r--   0        0        0     1699 2023-07-15 05:19:47.624301 rosys-0.9.0/rosys/vision/usb_camera.py
+-rw-r--r--   0        0        0    11945 2023-07-15 05:19:47.624301 rosys-0.9.0/rosys/vision/usb_camera_provider_hardware.py
+-rw-r--r--   0        0        0     3126 2023-07-15 05:19:47.624301 rosys-0.9.0/rosys/vision/usb_camera_provider_simulation.py
+-rw-r--r--   0        0        0     8086 1970-01-01 00:00:00.000000 rosys-0.9.0/setup.py
+-rw-r--r--   0        0        0     8131 1970-01-01 00:00:00.000000 rosys-0.9.0/PKG-INFO
```

### Comparing `rosys-0.8.5/LICENSE` & `rosys-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/README.md` & `rosys-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/pyproject.toml` & `rosys-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "rosys"
-version = "v0.8.5"
+version = "v0.9.0"
 description = "Modular Robot System With Elegant Automation Capabilities"
 authors = ["Zauberzeug GmbH <info@zauberzeug.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/zauberzeug/rosys"
 keywords = ["robot", "framework", "automation", "control", "steer"]
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.12"
-nicegui = "1.2.17"
+nicegui = ">=1.3.2"
 asyncio = "^3.4.3"
 retry = "^0.9.2"
 aenum = "^3.1.5"
 requests = "^2.25.1"
 aiohttp = "^3.8.3"
 simplejson = "^3.17.2"
 pyserial = "^3.5"
@@ -33,19 +33,22 @@
 aiocache = "^0.11.1"
 ujson = "5.4.0"
 msgpack = "^1.0.3"
 uvloop = "^0.17.0"
 dataclasses-json = "^0.5.7"
 executing = "^1.0.0"
 suntime = "^1.2.5"
-line-profiler = "^4.0.2"
+line-profiler = "^4.0.3"
 yappi = "^1.4"
 pyloot = "^0.1.0"
 objgraph = "^3.5.0"
+imgsize = "^2.1"
+netifaces = "^0.11.0"
 httpx = "^0.24.0"
+matplotlib = "^3.7.2"
 
 [tool.poetry.dev-dependencies]
 autopep8 = "^1.5.5"
 pytest = "^6.2.1"
 pytest-watch = "^4.2.0"
 pytest-flakefinder = "^1.0.0"
 pytest-profiling = "^1.7.0"
@@ -58,7 +61,10 @@
 
 [build-system]
 requires = [
     "setuptools>=30.3.0,<50",
     "poetry-core>=1.0.0"
 ]
 build-backend = "poetry.core.masonry.api"
+
+[tool.mypy]
+ignore_missing_imports = true
```

### Comparing `rosys-0.8.5/rosys/analysis/__init__.py` & `rosys-0.9.0/rosys/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/analysis/assets/RobotoMono-Medium.ttf` & `rosys-0.9.0/rosys/analysis/assets/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/analysis/asyncio_warnings.py` & `rosys-0.9.0/rosys/analysis/asyncio_warnings.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/analysis/kpi_buckets.py` & `rosys-0.9.0/rosys/analysis/kpi_buckets.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 @dataclass(slots=True, kw_only=True)
 class TimeBucket:
     date: str
     incidents: dict[str, int] = field(default_factory=dict)
 
     @classmethod
     def from_buckets(cls, sources: list[TimeBucket]) -> TimeBucket:
-        counter = Counter()
+        counter: Counter = Counter()
         for source in sources:
             counter.update(source.incidents)
         return cls(date=sources[0].date, incidents=dict(counter))
 
 
 @dataclass(slots=True, kw_only=True)
 class Day(TimeBucket):
```

### Comparing `rosys-0.8.5/rosys/analysis/kpi_logger.py` & `rosys-0.9.0/rosys/analysis/kpi_logger.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/analysis/kpi_page_.py` & `rosys-0.9.0/rosys/analysis/kpi_page_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/analysis/legacy/asyncio_monitor.py` & `rosys-0.9.0/rosys/analysis/legacy/asyncio_monitor.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/analysis/legacy/asyncio_page.py` & `rosys-0.9.0/rosys/analysis/legacy/asyncio_page.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/analysis/legacy/cpu_usage.py` & `rosys-0.9.0/rosys/analysis/legacy/cpu_usage.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/analysis/legacy/lizard_stats.py` & `rosys-0.9.0/rosys/analysis/legacy/lizard_stats.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/analysis/legacy/network_monitor.py` & `rosys-0.9.0/rosys/analysis/legacy/network_monitor.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/analysis/legacy/objgraph_page.py` & `rosys-0.9.0/rosys/analysis/legacy/objgraph_page.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/analysis/legacy/pyloot_page.py` & `rosys-0.9.0/rosys/analysis/legacy/pyloot_page.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/analysis/memory.py` & `rosys-0.9.0/rosys/analysis/memory.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/analysis/profile_button_.py` & `rosys-0.9.0/rosys/analysis/profile_button_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/analysis/profiling.py` & `rosys-0.9.0/rosys/analysis/profiling.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Optional
 
 from line_profiler import LineProfiler as PyUtilsLineProfiler
 
 
 class LineProfiler:
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.functions: list[list] = []
         self.line_profiler: Optional[PyUtilsLineProfiler] = None
 
     def __call__(self, func):
         index = len(self.functions)
 
         @wraps(func)
```

### Comparing `rosys-0.8.5/rosys/analysis/timelapse_recorder.py` & `rosys-0.9.0/rosys/analysis/timelapse_recorder.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/analysis/track.py` & `rosys-0.9.0/rosys/analysis/track.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/analysis/videos_page_.py` & `rosys-0.9.0/rosys/analysis/videos_page_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/automation/app_controls_.py` & `rosys-0.9.0/rosys/automation/app_controls_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/automation/automation.py` & `rosys-0.9.0/rosys/automation/automation.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/automation/automation_controls_.py` & `rosys-0.9.0/rosys/automation/automation_controls_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/automation/automator.py` & `rosys-0.9.0/rosys/automation/automator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Callable, Coroutine, Optional
+from typing import Callable, Coroutine, Optional, cast
 
 from .. import rosys
 from ..analysis import track
 from ..driving import Steerer
 from ..event import Event
 from .automation import Automation
 
@@ -51,16 +51,16 @@
         self.enabled: bool = True
         self.automation: Optional[Automation] = None
 
         if steerer:
             steerer.STEERING_STARTED.register(lambda: self.pause(because='steering started'))
 
         if on_interrupt:
-            self.AUTOMATION_PAUSED.register(lambda _: rosys.background_tasks.create(on_interrupt()))
-            self.AUTOMATION_STOPPED.register(lambda _: rosys.background_tasks.create(on_interrupt()))
+            self.AUTOMATION_PAUSED.register(lambda _: rosys.background_tasks.create(cast(Callable, on_interrupt)()))
+            self.AUTOMATION_STOPPED.register(lambda _: rosys.background_tasks.create(cast(Callable, on_interrupt)()))
 
         rosys.on_shutdown(lambda: self.stop(because='automator is shutting down'))
 
     @property
     def is_stopped(self) -> bool:
         return self.automation is None or self.automation.is_stopped
 
@@ -75,14 +75,15 @@
     def start(self, coro: Optional[Coroutine] = None, *, paused: bool = False) -> None:
         """Starts a new automation.
 
         You can pass any coroutine.
         The automator will make sure it can be paused, resumed and stopped.
         """
         if coro is None:
+            assert self.default_automation is not None
             self.start(self.default_automation(), paused=paused)
             return
         if not self.enabled:
             coro.close()
             return
         self.stop(because='new automation starts')
         self.automation = Automation(coro, self._handle_exception, on_complete=self._on_complete)
@@ -94,33 +95,36 @@
 
     def pause(self, because: str) -> None:
         """Pauses the current automation.
 
         You need to provide a cause which will be used as notification message.
         """
         if self.is_running:
+            assert self.automation is not None
             self.automation.pause()
             self.AUTOMATION_PAUSED.emit(because)
             rosys.notify(f'automation paused because {because}')
 
     def resume(self) -> None:
         """Resumes the current automation."""
         if not self.enabled:
             return
         if self.is_paused:
+            assert self.automation is not None
             self.automation.resume()
             self.AUTOMATION_RESUMED.emit()
             rosys.notify('automation resumed')
 
     def stop(self, because: str) -> None:
         """Stops the current automation.
 
         You need to provide a cause which will be used as notification message.
         """
         if not self.is_stopped:
+            assert self.automation is not None
             self.automation.stop()
             self.AUTOMATION_STOPPED.emit(because)
             track.reset()
             rosys.notify(f'automation stopped because {because}')
 
     def enable(self) -> None:
         """Enables the automator.
```

### Comparing `rosys-0.8.5/rosys/automation/schedule.py` & `rosys-0.9.0/rosys/automation/schedule.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/driving/driver.py` & `rosys-0.9.0/rosys/driving/driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,16 +118,18 @@
                 curvature = (-1 if curvature < 0 else 1) / self.parameters.minimum_turning_radius
 
             drive_backward = hook.projected_distance(carrot.offset_point, self.odometer.prediction.yaw) < 0
             if drive_backward and not self.parameters.can_drive_backwards:
                 drive_backward = False
                 curvature = (-1 if curvature > 0 else 1) / max(self.parameters.minimum_turning_radius, 0.001)
             linear = -1 if drive_backward else 1
-            if carrot.t > 1.0 and throttle_at_end:
-                linear *= ramp(carrot.target_distance, 0.5, 0.0, 1.0, 0.5)
+            t = spline.closest_point(hook.x, hook.y)
+            if t >= 1.0 and throttle_at_end:
+                target_distance = self.odometer.prediction.projected_distance(spline.pose(1.0))
+                linear *= ramp(target_distance, self.parameters.hook_offset, 0.0, 1.0, 0.01, clip=True)
             angular = linear * curvature
 
             self.state = DriveState(
                 carrot_pose=carrot.pose,
                 curvature=curvature,
                 backward=drive_backward,
                 turn_angle=turn_angle,
@@ -170,15 +172,14 @@
 
 
 @dataclass(slots=True, kw_only=True)
 class Carrot:
     spline: Spline
     offset: Point = field(default_factory=lambda: Point(x=0, y=0))
     t: float = 0
-    target_distance: Optional[float] = None
 
     @property
     def pose(self) -> Pose:
         if self.t < 1.0:
             return self.spline.pose(self.t)
         else:
             return Pose(
@@ -187,25 +188,17 @@
                 yaw=self.spline.yaw(1.0),
             )
 
     @property
     def offset_point(self) -> Point:
         return self.pose.transform(self.offset)
 
-    def move(self, hook: Point, distance: float = 1.0, move_threshold: float = 0.01) -> bool:
-        end_pose = self.spline.pose(1.0)
-        end_point = end_pose.point
-        end_yaw = end_pose.yaw
-
+    def move(self, hook: Point, distance: float) -> bool:
         while hook.distance(self.offset_point) < distance:
             self.t += 0.01
-            if self.t < 1.0:
-                continue
-            self.target_distance = hook.projected_distance(end_point, end_yaw)
-            if self.target_distance <= move_threshold:
+            if self.t >= 1.0:
                 return False
-
         return True
 
     def move_by_foot(self, pose: Pose) -> bool:
         self.t = self.spline.closest_point(pose.x, pose.y, t_min=self.t, t_max=1.0)
         return self.t < 1.0
```

### Comparing `rosys-0.8.5/rosys/driving/driver_object.py` & `rosys-0.9.0/rosys/driving/driver_object.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/driving/joystick_.py` & `rosys-0.9.0/rosys/driving/joystick_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/driving/keyboard_control_.py` & `rosys-0.9.0/rosys/driving/keyboard_control_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/driving/odometer.py` & `rosys-0.9.0/rosys/driving/odometer.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/driving/robot_object_.py` & `rosys-0.9.0/rosys/driving/robot_object_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/driving/steerer.py` & `rosys-0.9.0/rosys/driving/steerer.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/event.py` & `rosys-0.9.0/rosys/event.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,16 +31,19 @@
         self.listeners: list[EventListener] = list()
         events.append(self)
 
     def register(self, callback: Callable) -> Event:
         if not callable(callback):
             raise Exception('non-callable callback')
         if any(l.callback == callback for l in self.listeners):
-            return  # NOTE: don't add duplicate listeners
-        frame = inspect.currentframe().f_back
+            return self  # NOTE: don't add duplicate listeners
+        frame = inspect.currentframe()
+        assert frame is not None
+        frame = frame.f_back
+        assert frame is not None
         self.listeners.append(EventListener(callback=callback, filepath=frame.f_code.co_filename, line=frame.f_lineno))
         return self
 
     def register_ui(self, callback: Callable) -> Event:
         self.register(callback)
         client = nicegui_globals.get_client()
         if not client.shared:
```

### Comparing `rosys-0.8.5/rosys/geometry/line.py` & `rosys-0.9.0/rosys/geometry/line.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     @property
     def tuple(self) -> tuple[float, float, float]:
         return (self.a, self.b, self.c)
 
     @property
     def yaw(self) -> float:
-        return np.arctan2(self.b, self.a) + np.pi / 2
+        return np.arctan2(self.b, self.a) - np.pi / 2
 
     @staticmethod
     def from_points(point1: Point, point2: Point) -> Line:
         l = skew(point1.x, point1.y, 1) @ [point2.x, point2.y, 1]
         return Line(a=l[0], b=l[1], c=l[2])
 
     def intersect(self, other: Line) -> Point:
```

### Comparing `rosys-0.8.5/rosys/geometry/line_segment.py` & `rosys-0.9.0/rosys/geometry/line_segment.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/geometry/point.py` & `rosys-0.9.0/rosys/geometry/point.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/geometry/point3d.py` & `rosys-0.9.0/rosys/geometry/point3d.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/geometry/pose.py` & `rosys-0.9.0/rosys/geometry/pose.py`

 * *Files 7% similar despite different names*

```diff
@@ -101,14 +101,20 @@
     def transform_line(self, line: Line) -> Line:
         a, b, c = self.inv_matrix.T @ line.tuple
         return Line(a=a, b=b, c=c)
 
     def relative_pose(self, other: Pose) -> Pose:
         return Pose.from_matrix(self.inv_matrix @ other.matrix)
 
+    def relative_point(self, other: Point) -> Point:
+        dx = other.x - self.x
+        dy = other.y - self.y
+        return Point(x=dx * np.cos(-self.yaw) - dy * np.sin(-self.yaw),
+                     y=dx * np.sin(-self.yaw) + dy * np.cos(-self.yaw))
+
     def rotate(self, angle: float) -> Pose:
         return Pose(x=self.x, y=self.y, yaw=self.yaw+angle, time=self.time)
 
     def interpolate(self, other: Pose, t: float) -> Pose:
         return Pose(
             x=(1 - t) * self.x + t * other.x,
             y=(1 - t) * self.y + t * other.y,
```

### Comparing `rosys-0.8.5/rosys/geometry/rectangle.py` & `rosys-0.9.0/rosys/geometry/rectangle.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     x: float
     y: float
     width: float
     height: float
 
     @property
     def tuple(self) -> tuple[float, float, float, float]:
-        return (self.x, self.y, self.w, self.h)
+        return (self.x, self.y, self.width, self.height)
 
     def contains(self, point: Point) -> bool:
         return (self.x <= point.x <= self.x + self.width and
                 self.y <= point.y <= self.y + self.height)
 
     def __str__(self) -> str:
-        return f'Rectangle({round(self.x, 2)}, {round(self.y, 2)}, {round(self.w, 2)}, {round(self.h, 2)})'
+        return f'Rectangle({round(self.x, 2)}, {round(self.y, 2)}, {round(self.width, 2)}, {round(self.height, 2)})'
```

### Comparing `rosys-0.8.5/rosys/geometry/rotation.py` & `rosys-0.9.0/rosys/geometry/rotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         return Rotation(R=np.dot(self.R, other.R).tolist())
 
     @property
     def T(self) -> Rotation:
         return Rotation(R=np.array(self.R).T.tolist())
 
     @property
-    def euler(self) -> tuple[float]:
+    def euler(self) -> tuple[float, float, float]:
         return (
             np.arctan2(self.R[2][1], self.R[2][2]),
             np.arctan2(-self.R[2][0], np.sqrt(self.R[2][1]**2 + self.R[2][2]**2)),
             np.arctan2(self.R[1][0], self.R[0][0]),
         )
 
     @property
```

### Comparing `rosys-0.8.5/rosys/geometry/spline.py` & `rosys-0.9.0/rosys/geometry/spline.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/hardware/__init__.py` & `rosys-0.9.0/rosys/hardware/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from .battery_control import BatteryControlHardware
 from .bluetooth import BluetoothHardware
 from .bms import Bms, BmsHardware, BmsSimulation
 from .bumper import Bumper, BumperHardware, BumperSimulation
 from .can import CanHardware
 from .communication import Communication, SerialCommunication, WebCommunication
 from .estop import EStop, EStopHardware, EStopSimulation
 from .expander import ExpanderHardware
+from .imu import ImuHardware
 from .module import Module, ModuleHardware, ModuleSimulation
 from .robot import Robot, RobotHardware, RobotSimulation
 from .robot_brain import RobotBrain
 from .serial import SerialHardware
 from .wheels import Wheels, WheelsHardware, WheelsSimulation
```

### Comparing `rosys-0.8.5/rosys/hardware/bms.py` & `rosys-0.9.0/rosys/hardware/bms.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/hardware/bms_message.py` & `rosys-0.9.0/rosys/hardware/bms_message.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/hardware/bms_state.py` & `rosys-0.9.0/rosys/hardware/bms_state.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/hardware/bumper.py` & `rosys-0.9.0/rosys/hardware/bumper.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .module import Module, ModuleHardware, ModuleSimulation
 from .robot_brain import RobotBrain
 
 
 class Bumper(Module, abc.ABC):
     """A module that detects when a bumper is triggered."""
 
-    def __init__(self, estop: EStop, **kwargs) -> None:
+    def __init__(self, estop: Optional[EStop], **kwargs) -> None:
         self.estop = estop
         super().__init__(**kwargs)
 
         self.BUMPER_TRIGGERED = Event()
         """a bumper was triggered (argument: the bumper name)"""
 
         self.active_bumpers: list[str] = []
```

### Comparing `rosys-0.8.5/rosys/hardware/can.py` & `rosys-0.9.0/rosys/hardware/can.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/hardware/communication/communication.py` & `rosys-0.9.0/rosys/hardware/communication/communication.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/hardware/communication/serial_communication.py` & `rosys-0.9.0/rosys/hardware/communication/serial_communication.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from collections import deque
 from typing import Optional
 
 import serial
 from nicegui import ui
 from nicegui.events import ValueChangeEventArguments
 
 from ... import rosys
@@ -26,14 +27,16 @@
         self.device_path = self.get_device_path()
         if self.device_path is None:
             raise Exception('No serial port found')
         self.log.debug(f'connecting serial on {self.device_path} with baud rate {baud_rate}')
         self.serial = serial.Serial(self.device_path, baud_rate)
         self.buffer = ''
         self.log_io: bool = False
+        self.undo_queue = deque(maxlen=100)
+        self.redo_queue = deque(maxlen=100)
 
     @staticmethod
     def is_possible() -> bool:
         return SerialCommunication.get_device_path() is not None
 
     @staticmethod
     def get_device_path() -> Optional[str]:
@@ -72,22 +75,39 @@
         self.serial.write(f'{line}\n'.encode())
         if self.log_io:
             self.log.debug(f'send: {line}')
 
     def debug_ui(self) -> None:
         super().debug_ui()
 
-        async def submit_input() -> None:
-            await self.send(input.value)
-            input.value = ''
+        async def input_enter() -> None:
+            await self.send(command.value)
+            while self.redo_queue:
+                self.undo_queue.append(self.redo_queue.pop())
+            self.undo_queue.append(command.value)
+            command.value = ''
+
+        def input_up() -> None:
+            if self.undo_queue:
+                if command.value:
+                    self.redo_queue.append(command.value)
+                command.value = self.undo_queue.pop()
+
+        def input_down() -> None:
+            if command.value:
+                self.undo_queue.append(command.value)
+            command.value = self.redo_queue.pop() if self.redo_queue else ''
 
         def toggle(e: ValueChangeEventArguments) -> None:
             if e.value:
                 self.connect()
                 rosys.notify('connected to Lizard')
             else:
                 self.disconnect()
                 rosys.notify('disconnected from Lizard')
 
         ui.switch('Serial Communication', value=self.serial.isOpen(), on_change=toggle)
         ui.switch('Serial Logging').bind_value(self, 'log_io')
-        input = ui.input('Serial Command', on_change=submit_input)
+        command = ui.input('Serial Command')
+        command.on('keydown.enter', input_enter)
+        command.on('keydown.up', input_up)
+        command.on('keydown.down', input_down)
```

### Comparing `rosys-0.8.5/rosys/hardware/communication/web_communication.py` & `rosys-0.9.0/rosys/hardware/communication/web_communication.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,13 +40,14 @@
             return False
 
     async def read(self) -> Optional[str]:
         if not self.sio.connected:
             await self.sio.connect(self.host)
         if self.buffer:
             return self.buffer.pop()
+        return None
 
     async def send(self, line: str) -> None:
         await self.sio.emit('write', line)
 
     async def tear_down(self) -> None:
         await self.sio.disconnect()
```

### Comparing `rosys-0.8.5/rosys/hardware/estop.py` & `rosys-0.9.0/rosys/hardware/estop.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/hardware/expander.py` & `rosys-0.9.0/rosys/hardware/expander.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/hardware/hardware_proxy.py` & `rosys-0.9.0/rosys/hardware/hardware_proxy.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/hardware/lizard_firmware.py` & `rosys-0.9.0/rosys/hardware/lizard_firmware.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/hardware/module.py` & `rosys-0.9.0/rosys/hardware/module.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import abc
 import logging
+from typing import Callable
 
 from .robot_brain import RobotBrain
 
 
 class Module(abc.ABC):
 
     def __init__(self) -> None:
@@ -14,15 +15,15 @@
 
     def __init__(self, robot_brain: RobotBrain, lizard_code: str, core_message_fields: list[str] = [],
                  **kwargs) -> None:
         super().__init__(**kwargs)
         self.robot_brain = robot_brain
         self.lizard_code = lizard_code
         self.core_message_fields: list[str] = core_message_fields
-        self.message_hooks: dict[str, callable] = {}
+        self.message_hooks: dict[str, Callable] = {}
 
     def handle_core_output(self, time: float, words: list[str]) -> None:
         pass
 
 
 class ModuleSimulation(Module):
```

### Comparing `rosys-0.8.5/rosys/hardware/robot.py` & `rosys-0.9.0/rosys/hardware/robot.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,18 +30,18 @@
         for module in self.modules:
             code += cast(ModuleHardware, module).lizard_code + '\n'
         output_fields = []
         for module in self.modules:
             output_fields.extend(cast(ModuleHardware, module).core_message_fields)
         code += remove_indentation(f'''
             core.output("core.millis {' '.join(output_fields)}")
-            en = Output(15)
-            v24 = Output(12)
-            en.on()
-            v24.on()
+            rdyp = Output(15)
+            en3 = Output(12)
+            rdyp.on()
+            en3.on()
         ''')
         return code
 
     async def update(self) -> None:
         for time, line in await self.robot_brain.read_lines():
             words = line.split()
             if not words:
```

### Comparing `rosys-0.8.5/rosys/hardware/robot_brain.py` & `rosys-0.9.0/rosys/hardware/robot_brain.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/hardware/serial.py` & `rosys-0.9.0/rosys/hardware/serial.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/hardware/wheels.py` & `rosys-0.9.0/rosys/hardware/wheels.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,18 +27,16 @@
         rosys.on_shutdown(self.stop)
 
     @abc.abstractmethod
     async def drive(self, linear: float, angular: float) -> None:
         self.linear_target_speed = linear
         self.angular_target_speed = angular
 
-    @abc.abstractmethod
     async def stop(self) -> None:
-        self.linear_target_speed = 0.0
-        self.angular_target_speed = 0.0
+        await self.drive(0.0, 0.0)
 
 
 class WheelsHardware(Wheels, ModuleHardware):
     """This module implements wheels hardware.
 
     Drive and stop commands are forwarded to a given Robot Brain.
     Velocities are read and emitted regularly.
@@ -67,18 +65,14 @@
         core_message_fields = [f'{self.name}.linear_speed:3', f'{self.name}.angular_speed:3']
         super().__init__(robot_brain=robot_brain, lizard_code=lizard_code, core_message_fields=core_message_fields)
 
     async def drive(self, linear: float, angular: float) -> None:
         await super().drive(linear, angular)
         await self.robot_brain.send(f'{self.name}.speed({linear}, {angular})')
 
-    async def stop(self) -> None:
-        await super().stop()
-        await self.robot_brain.send(f'{self.name}.off()')
-
     def handle_core_output(self, time: float, words: list[str]) -> None:
         velocity = Velocity(linear=float(words.pop(0)), angular=float(words.pop(0)), time=time)
         self.VELOCITY_MEASURED.emit([velocity])
 
 
 class WheelsSimulation(Wheels, ModuleSimulation):
     """This module simulates two wheels.
@@ -99,17 +93,12 @@
 
     async def drive(self, linear: float, angular: float) -> None:
         await super().drive(linear, angular)
         f = self.inertia_factor
         self.linear_velocity = 0 if self.is_blocking else f * self.linear_velocity + (1 - f) * linear
         self.angular_velocity = 0 if self.is_blocking else f * self.angular_velocity + (1 - f) * angular
 
-    async def stop(self) -> None:
-        await super().stop()
-        self.linear_velocity = 0
-        self.angular_velocity = 0
-
     async def step(self, dt: float) -> None:
         if not self.is_slipping:
             self.pose += PoseStep(linear=dt*self.linear_velocity, angular=dt*self.angular_velocity, time=rosys.time())
         velocity = Velocity(linear=self.linear_velocity, angular=self.angular_velocity, time=rosys.time())
         self.VELOCITY_MEASURED.emit([velocity])
```

### Comparing `rosys-0.8.5/rosys/pathplanning/area_object_.py` & `rosys-0.9.0/rosys/pathplanning/area_object_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/binary_renderer.py` & `rosys-0.9.0/rosys/pathplanning/binary_renderer.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/binary_renderer_demo.py` & `rosys-0.9.0/rosys/pathplanning/binary_renderer_demo.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/delaunay_planner.py` & `rosys-0.9.0/rosys/pathplanning/delaunay_planner.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/demos/20220714-1.py` & `rosys-0.9.0/rosys/pathplanning/demos/20220714-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/demos/20220714-2-A.py` & `rosys-0.9.0/rosys/pathplanning/demos/20220714-2-A.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/demos/20220714-2-B.py` & `rosys-0.9.0/rosys/pathplanning/demos/20220714-2-B.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/demos/20220714-3.py` & `rosys-0.9.0/rosys/pathplanning/demos/20220714-3.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/demos/20220725-1.py` & `rosys-0.9.0/rosys/pathplanning/demos/20220725-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/demos/20220825-1.py` & `rosys-0.9.0/rosys/pathplanning/demos/20220825-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/demos/20220916-1.py` & `rosys-0.9.0/rosys/pathplanning/demos/20220916-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/demos/20220921-1.py` & `rosys-0.9.0/rosys/pathplanning/demos/20220921-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/demos/20221121-1.py` & `rosys-0.9.0/rosys/pathplanning/demos/20221121-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/demos/20221203-1.py` & `rosys-0.9.0/rosys/pathplanning/demos/20221203-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/demos/20230120-1.py` & `rosys-0.9.0/rosys/pathplanning/demos/20230120-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/distance_map.py` & `rosys-0.9.0/rosys/pathplanning/distance_map.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/distance_map_demo.py` & `rosys-0.9.0/rosys/pathplanning/distance_map_demo.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/experiments.py` & `rosys-0.9.0/rosys/pathplanning/experiments.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/fast_spline.py` & `rosys-0.9.0/rosys/pathplanning/fast_spline.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/grid.py` & `rosys-0.9.0/rosys/pathplanning/grid.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/obstacle_map.py` & `rosys-0.9.0/rosys/pathplanning/obstacle_map.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/obstacle_map_demo.py` & `rosys-0.9.0/rosys/pathplanning/obstacle_map_demo.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/obstacle_object_.py` & `rosys-0.9.0/rosys/pathplanning/obstacle_object_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/path_object_.py` & `rosys-0.9.0/rosys/pathplanning/path_object_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/path_planner.py` & `rosys-0.9.0/rosys/pathplanning/path_planner.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/planner_demo.py` & `rosys-0.9.0/rosys/pathplanning/planner_demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     robot_outline = i.robot_outline
 
 planner = DelaunayPlanner(robot_outline)
 
 
 def run() -> None:
     t = time.time()
-    planner.update_map(cmd.areas, cmd.obstacles, [cmd.start, cmd.goal], deadline=time.time()+10.0)
+    planner.update_map(cmd.areas, cmd.obstacles, [cmd.start.point, cmd.goal.point], deadline=time.time()+10.0)
     dt0 = time.time() - t
 
     t = time.time()
     try:
         path = planner.search(cmd.start, cmd.goal)
     except RuntimeError:
         logging.exception('could not find path')
```

### Comparing `rosys-0.8.5/rosys/pathplanning/planner_process.py` & `rosys-0.9.0/rosys/pathplanning/planner_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         self.connection = connection
         self.planner = DelaunayPlanner(robot_outline)
 
     def run(self) -> None:
         while True:
             try:
                 cmd = self.connection.recv()
-            except EOFError:
+            except (EOFError, KeyboardInterrupt):
                 self.log.info('PlannerProcess stopped')
                 return
             try:
                 if isinstance(cmd, PlannerSearchCommand):
                     self.log.info(cmd)
                     additional_points = [cmd.start.point, cmd.goal.point]
                     self.planner.update_map(cmd.areas, cmd.obstacles, additional_points, cmd.deadline)
```

### Comparing `rosys-0.8.5/rosys/pathplanning/plot_tools.py` & `rosys-0.9.0/rosys/pathplanning/plot_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 
 def plot_spline(spline, *args, backward=False, **kwargs) -> None:
     t = np.linspace(0, 1, 20)
     pl.plot(spline.x(t), spline.y(t), *args, alpha=0.5 if backward else 1.0, **kwargs)
 
 
 def plot_path(path, *args, **kwargs) -> None:
-    [plot_spline(step.spline, *args, backward=step.backward, **kwargs) for step in path]
+    for step in path:
+        plot_spline(step.spline, *args, backward=step.backward, **kwargs)
 
 
 def show_obstacle_map(obstacle_map):
     cmap = pl.matplotlib.colors.ListedColormap([[0, 0, 0, 0.1], 'C3'])
     extent = bbox_to_extent(obstacle_map.grid.bbox)
     pl.imshow(obstacle_map.map, cmap=cmap, interpolation='nearest', extent=extent, alpha=0.5)
     plot_bbox(obstacle_map.grid.bbox, 'C0--', lw=0.2, dashes=[20, 20])
```

### Comparing `rosys-0.8.5/rosys/pathplanning/plot_tools_demo.py` & `rosys-0.9.0/rosys/pathplanning/plot_tools_demo.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/robot_renderer.py` & `rosys-0.9.0/rosys/pathplanning/robot_renderer.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/robot_renderer_demo.py` & `rosys-0.9.0/rosys/pathplanning/robot_renderer_demo.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/steps.py` & `rosys-0.9.0/rosys/pathplanning/steps.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/pathplanning/steps_demo.py` & `rosys-0.9.0/rosys/pathplanning/steps_demo.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/persistence.py` & `rosys-0.9.0/rosys/persistence.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 
 def export_button(title: str = 'Export', route: str = '/export', tmp_filepath: str = '/tmp/export.json') -> ui.button:
     @app.get(route)
     def get_export() -> FileResponse:
         with open(tmp_filepath, 'w') as f:
             json.dump({name: module.backup() for name, module in modules.items()}, f, indent=4)
         return FileResponse(tmp_filepath, filename='export.json')
-    ui.button(title, on_click=lambda: ui.download(route[1:]))
+    return ui.button(title, on_click=lambda: ui.download(route[1:]))
 
 
 def import_button(title: str = 'Import', after_import: Optional[Callable] = None) -> ui.button:
     async def restore_from_file(e: UploadEventArguments) -> None:
         all_data = json.load(e.content)
         assert isinstance(all_data, dict)
         for name, data in all_data.items():
```

### Comparing `rosys-0.8.5/rosys/rosys.py` & `rosys-0.9.0/rosys/rosys.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 startup_handlers: list[Callable] = []
 shutdown_handlers: list[Callable] = []
 tasks: list[asyncio.Task] = []
 
 
 def notify(message: str, type: Optional[Literal['positive', 'negative', 'warning', 'info', 'ongoing']] = None) -> None:
     log.info(message)
-    notifications.append(Notification(time=time, message=message))
+    notifications.append(Notification(time=time(), message=message))
     NEW_NOTIFICATION.emit(message)
     # NOTE show notifications on all pages
     for client in nicegui_globals.clients.values():
         with client:
             try:
                 ui.notify(message, type=type)
             except Exception:
```

### Comparing `rosys-0.8.5/rosys/run.py` & `rosys-0.9.0/rosys/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 import subprocess
 import uuid
 from asyncio.subprocess import Process
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 from concurrent.futures.process import BrokenProcessPool
 from contextlib import contextmanager
 from functools import partial, wraps
-from typing import Callable, Generator, Optional
+from typing import Any, Callable, Generator, Optional
 
 from psutil import Popen
 
 from . import rosys
 
 process_pool = ProcessPoolExecutor()
 thread_pool = ThreadPoolExecutor(thread_name_prefix='run.py thread_pool')
-running_cpu_bound_processes: list[int] = []  # NOTE is used in tests to advance time slower until computation is done
+running_cpu_bound_processes: list[str] = []  # NOTE is used in tests to advance time slower until computation is done
 running_sh_processes: list[Process] = []
 log = logging.getLogger('rosys.run')
 
 
-async def io_bound(callback: Callable, *args: any, **kwargs: any):
+async def io_bound(callback: Callable, *args: Any, **kwargs: Any):
     if rosys.is_stopping():
         return
     loop = asyncio.get_running_loop()
     try:
         return await loop.run_in_executor(thread_pool, partial(callback, *args, **kwargs))
     except RuntimeError as e:
         if 'cannot schedule new futures after shutdown' not in str(e):
@@ -40,15 +40,15 @@
     """decorator to wrap a normal function into an asyncio coroutine"""
     @wraps(func)
     async def inner(*args, **kwargs):
         return await io_bound(func, *args, **kwargs)
     return inner
 
 
-async def cpu_bound(callback: Callable, *args: any):
+async def cpu_bound(callback: Callable, *args: Any):
     if rosys.is_stopping():
         return
     with cpu():
         try:
             loop = asyncio.get_running_loop()
             return await loop.run_in_executor(process_pool, callback, *args)
         except BrokenProcessPool:
@@ -83,34 +83,39 @@
     def popen() -> str:
         if shell:  # convert to string
             cmd = ' '.join(command) if isinstance(command, list) else command
         else:  # convert to list
             cmd = shlex.split(command) if isinstance(command, str) else command
         if timeout is not None:
             if shell:
-                cmd = f'timeout {timeout} {cmd}'
+                cmd = f'timeout --signal=SIGKILL {timeout} {cmd}'
             else:
-                cmd = ['timeout', str(timeout)] + cmd
+                cmd = ['timeout', '--signal=SIGKILL', str(timeout)] + cmd
         # log.info(f'running sh: "{cmd}"')
         proc = subprocess.Popen(
             cmd,
             cwd=working_dir,
-            stdout=asyncio.subprocess.PIPE,
-            stderr=asyncio.subprocess.STDOUT,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
             shell=shell,
             start_new_session=True,
         )
         running_sh_processes.append(proc)
         stdout, *_ = proc.communicate()
         _kill(proc)
         running_sh_processes.remove(proc)
         return stdout.decode('utf-8')
+
     if rosys.is_stopping():
         return
-    return await io_bound(popen)
+    try:
+        return await asyncio.wait_for(io_bound(popen), timeout)
+    except asyncio.TimeoutError:
+        log.warning(f'Command "{command}" timed out after {timeout} seconds.')
+        return ''
 
 
 def _kill(proc: Popen) -> None:
     try:
         os.killpg(os.getpgid(proc.pid), signal.SIGTERM)
         log.info(f'killed {proc.pid}')
     except ProcessLookupError:
```

### Comparing `rosys-0.8.5/rosys/simulation_ui.py` & `rosys-0.9.0/rosys/simulation_ui.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,18 +5,15 @@
 from . import rosys
 
 
 class simulation_ui:
 
     def __init__(self) -> None:
         ui.label('Simulation speed')
-        ui.slider(min=0, max=10, value=1, step=0.1, on_change=self.request_backup) \
+        ui.slider(min=0, max=10, value=1, step=0.1, on_change=rosys.config.invalidate) \
             .bind_value(rosys.config, 'simulation_speed').props('label-always')
         self.simulation_time = ui.label()
         self.startup_time = rosys.time()
         ui.timer(0.1, self.update_simulation_time)
 
-    def request_backup(self) -> None:
-        rosys.config.needs_backup = True
-
     def update_simulation_time(self) -> None:
         self.simulation_time.set_text(f'Running for {timedelta(seconds=int(rosys.time() - self.startup_time))}')
```

### Comparing `rosys-0.8.5/rosys/system/wifi_button_.py` & `rosys-0.9.0/rosys/system/wifi_button_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/test/helpers.py` & `rosys-0.9.0/rosys/test/helpers.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/test/log_configuration.py` & `rosys-0.9.0/rosys/test/log_configuration.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/vision/calibration.py` & `rosys-0.9.0/rosys/vision/calibration.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/vision/camera.py` & `rosys-0.9.0/rosys/vision/camera.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 from __future__ import annotations
 
 import abc
 from dataclasses import dataclass, field
 from typing import Optional
 
 import numpy as np
+
 from rosys import persistence
 
 from ..geometry import Rotation
 from .calibration import Calibration, Extrinsics, Intrinsics
 from .image import Image, ImageSize
 
 
 @dataclass(slots=True, kw_only=True)
 class Camera(abc.ABC):
     id: str
     calibration: Optional[Calibration] = None
     images: list[Image] = field(default_factory=list, metadata=persistence.exclude)
     focal_length: Optional[float] = None
+    name: Optional[str] = None
+
+    def __post_init__(self) -> None:
+        if self.name is None:
+            self.name = self.id
 
     @property
     def captured_images(self) -> list[Image]:
         return [i for i in self.images if i.data]
 
     @property
     def latest_captured_image(self) -> Optional[Image]:
```

### Comparing `rosys-0.8.5/rosys/vision/camera_objects_.py` & `rosys-0.9.0/rosys/vision/camera_objects_.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,58 +47,62 @@
 
     async def update_cameras(self) -> None:
         camera_groups = self.find_objects('camera')
         for uid, camera_group in camera_groups.items():
             if uid not in self.calibrated_cameras:
                 camera_group.delete()
         for uid, camera in self.calibrated_cameras.items():
+            assert camera.calibration is not None
             if uid not in camera_groups:
-                with Group().with_name(f'camera_{uid}') as camera_groups[uid]:
-                    with Group() as pyramid:
-                        Cylinder(0, np.sqrt(0.5), 1, 4) \
-                            .rotate(-np.pi / 2, 0, np.pi / 4) \
-                            .move(z=0.5) \
-                            .material('#0088ff')
-                        if self.debug:
-                            Text(uid)
-                    pyramid.scale(
-                        camera.calibration.intrinsics.size.width / self.px_per_m,
-                        camera.calibration.intrinsics.size.height / self.px_per_m,
-                        camera.calibration.intrinsics.matrix[0][0] / self.px_per_m,
-                    )
+                with self:
+                    with Group().with_name(f'camera_{uid}') as camera_groups[uid]:
+                        with Group() as pyramid:
+                            Cylinder(0, np.sqrt(0.5), 1, 4) \
+                                .rotate(-np.pi / 2, 0, np.pi / 4) \
+                                .move(z=0.5) \
+                                .material('#0088ff')
+                            if self.debug:
+                                Text(uid)
+                        pyramid.scale(
+                            camera.calibration.intrinsics.size.width / self.px_per_m,
+                            camera.calibration.intrinsics.size.height / self.px_per_m,
+                            camera.calibration.intrinsics.matrix[0][0] / self.px_per_m,
+                        )
             camera_groups[uid].move(*camera.calibration.extrinsics.translation)
             camera_groups[uid].rotate_R(await run.cpu_bound(self.get_rotation, camera.calibration))
 
     @staticmethod
     def get_rotation(calibration: Calibration) -> list[list[float]]:
         return calibration.rotation.R  # computing euler rotation is cpu expensive
 
     async def update_images(self) -> None:
-        newest_images = [camera.latest_captured_image for camera in self.calibrated_cameras.values()]
-        newest_images = [i for i in newest_images if i is not None]
+        newest_images = [camera.latest_captured_image
+                         for camera in self.calibrated_cameras.values()
+                         if camera.latest_captured_image is not None]
 
         current_uids = [image.camera_id for image in newest_images]
         for uid, texture in list(self.textures.items()):
             if uid not in current_uids:
                 texture.delete()
                 del self.textures[uid]
 
-        z = 0
+        z = 0.0
         for image in sorted(newest_images, key=lambda i: i.time):
             camera = self.calibrated_cameras.get(image.camera_id)
             if camera is None:
                 continue
             projection = self.camera_projector.projections.get(camera.id)
             if projection is None:
                 continue
             coordinates = [[point and [point[0], point[1], 0] for point in row] for row in projection.coordinates]
 
             url = self.camera_provider.get_image_url(image)
             if image.camera_id not in self.textures:
-                self.textures[image.camera_id] = Texture(url, coordinates).with_name(f'image_{image.id}')
+                with self:
+                    self.textures[image.camera_id] = Texture(url, coordinates).with_name(f'image_{image.id}')
             texture = self.textures[image.camera_id]
 
             z += 0.001
             texture.move(z=z)
             if texture.args[0] != url:
                 texture.set_url(url)
             if not await run.cpu_bound(CameraProjector.allclose, texture.args[1], coordinates):
```

### Comparing `rosys-0.8.5/rosys/vision/camera_projector.py` & `rosys-0.9.0/rosys/vision/camera_projector.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
                 camera_id=id,
                 camera_calibration=deepcopy(camera.calibration),
                 coordinates=self.project(camera),
             )
 
     @staticmethod
     def project(camera: Camera, rows: int = 12, columns: int = 16) -> ProjectionCoordinates:
+        assert camera.calibration is not None
         c, r = np.meshgrid(np.linspace(0, camera.calibration.intrinsics.size.width, columns),
                            np.linspace(0, camera.calibration.intrinsics.size.height, rows))
         image_points = np.stack((c.flatten(), r.flatten()), axis=1)
         floor_points = camera.calibration.project_array_from_image(image_points).reshape(rows, columns, 3)
         invalid = np.isnan(floor_points).any(axis=2)
         return [
             [
```

### Comparing `rosys-0.8.5/rosys/vision/camera_provider.py` & `rosys-0.9.0/rosys/vision/camera_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,7 +77,10 @@
     def prune_images(self, max_age_seconds: Optional[float] = None):
         for camera in self.cameras.values():
             if max_age_seconds is None:
                 camera.images.clear()
             else:
                 while camera.images and camera.images[0].time < rosys.time() - max_age_seconds:
                     del camera.images[0]
+
+    def invalidate(self) -> None:
+        self.needs_backup = True
```

### Comparing `rosys-0.8.5/rosys/vision/detections.py` & `rosys-0.9.0/rosys/vision/detections.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from dataclasses import dataclass, field
+from dataclasses import asdict, dataclass, field
 
 from ..geometry import Point
 
 
 @dataclass(slots=True, kw_only=True)
 class Detection:
     category_name: str
@@ -121,7 +121,10 @@
     segmentations: list[SegmentationDetection] = field(default_factory=list)
 
     def to_svg(self, shrink: int = 1) -> str:
         return '\n'.join(
             b.to_svg(shrink) for b in self.boxes) + '\n' + '\n'.join(
             p.to_svg(shrink) for p in self.points) + '\n' + '\n'.join(
             s.to_svg(shrink) for s in self.segmentations)
+
+    def to_dict(self) -> dict:
+        return asdict(self)
```

### Comparing `rosys-0.8.5/rosys/vision/detector.py` & `rosys-0.9.0/rosys/vision/detector.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/vision/detector_hardware.py` & `rosys-0.9.0/rosys/vision/detector_hardware.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/vision/detector_simulation.py` & `rosys-0.9.0/rosys/vision/detector_simulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 from .uploads import Uploads
 
 
 @dataclass(slots=True, kw_only=True)
 class SimulatedObject:
     category_name: str
     position: Point3d
-    size: Optional[tuple[float]] = None
+    size: Optional[tuple[float, float, float]] = None
     uuid: str = field(init=False)
+    confidence: float = 1.0
 
     def __post_init__(self) -> None:
         self.uuid = str(uuid4())
 
 
 class DetectorSimulation(Detector):
     """This detector simulates object detection.
@@ -70,28 +71,30 @@
     def update_simulated_objects(self, image: Image) -> None:
         pass
 
     def detect_from_simulated_objects(self, image: Image) -> None:
         if image.camera_id not in self.camera_provider.cameras:
             return
         camera = self.camera_provider.cameras[image.camera_id]
+        assert camera.calibration is not None
+        assert image.detections is not None
         for object in self.simulated_objects:
             viewing_direction = np.array(camera.calibration.extrinsics.rotation.R)[:, 2]
             object_direction = np.array(object.position.tuple) - camera.calibration.extrinsics.translation
             if np.dot(viewing_direction, object_direction) < 0:
                 continue
             image_point = camera.calibration.project_to_image(object.position)
             if not (0 <= image_point.x < image.size.width and 0 <= image_point.y < image.size.height):
                 continue
 
             if object.size is None:
                 image.detections.points.append(PointDetection(
                     category_name=object.category_name,
                     model_name='simulation',
-                    confidence=1.0,
+                    confidence=object.confidence,
                     x=image_point.x + self.noise * np.random.randn(),
                     y=image_point.y + self.noise * np.random.randn(),
                     uuid=object.uuid,
                 ))
             else:
                 world_points = np.array([
                     [object.position.x + dx, object.position.y + dy, object.position.z + dz]
@@ -99,14 +102,14 @@
                     for dy in [-object.size[1] / 2, object.size[1] / 2]
                     for dz in [-object.size[2] / 2, object.size[2] / 2]
                 ])
                 image_points = camera.calibration.project_array_to_image(world_points)
                 image.detections.boxes.append(BoxDetection(
                     category_name=object.category_name,
                     model_name='simulation',
-                    confidence=1.0,
+                    confidence=object.confidence,
                     x=image_points[:, 0].min() + self.noise * np.random.randn(),
                     y=image_points[:, 1].min() + self.noise * np.random.randn(),
                     width=image_points[:, 0].max() - image_points[:, 0].min() + self.noise * np.random.randn(),
                     height=image_points[:, 1].max() - image_points[:, 1].min() + self.noise * np.random.randn(),
                     uuid=object.uuid,
                 ))
```

### Comparing `rosys-0.8.5/rosys/vision/image.py` & `rosys-0.9.0/rosys/vision/image.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/vision/image_route.py` & `rosys-0.9.0/rosys/vision/image_route.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/vision/multi_camera_provider.py` & `rosys-0.9.0/rosys/vision/multi_camera_provider.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/vision/uploads.py` & `rosys-0.9.0/rosys/vision/uploads.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/vision/usb_camera.py` & `rosys-0.9.0/rosys/vision/usb_camera.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/rosys/vision/usb_camera_provider_hardware.py` & `rosys-0.9.0/rosys/vision/usb_camera_provider_hardware.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,23 +119,28 @@
                     continue
                 if 'MJPG' in device.video_formats:
                     bytes = await rosys.run.io_bound(to_bytes, image)
                     if camera.crop or camera.rotation != ImageRotation.NONE:
                         bytes = await rosys.run.cpu_bound(process_jpeg_image, bytes, camera.rotation, camera.crop)
                 else:
                     bytes = await rosys.run.cpu_bound(process_ndarray_image, image, camera.rotation, camera.crop)
-                size = camera.resolution or ImageSize(width=800, height=600)
+                if camera.crop:
+                    size = ImageSize(width=camera.crop.width, height=camera.crop.height)
+                elif camera.resolution:
+                    size = camera.resolution
+                else:
+                    size = ImageSize(width=800, height=600)
                 camera.images.append(Image(camera_id=uid, data=bytes, time=rosys.time(), size=size))
             except Exception:
                 self.log.exception(f'could not capture image from {uid}')
                 await self.deactivate(camera)
 
     async def update_parameters(self) -> None:
         for uid, camera in self._cameras.items():
-            if camera.active and uid in self.devices:
+            if camera.active and uid in self.devices and self.devices[uid].capture is not None:
                 await rosys.run.io_bound(self.set_parameters, camera, self.devices[uid])
 
     def capture_image(self, id) -> Any:
         _, image = self.devices[id].capture.read()
         return image
 
     async def activate(self, uid: str) -> None:
@@ -201,14 +206,15 @@
         self.devices.clear()
 
     @staticmethod
     def is_operable() -> bool:
         return shutil.which('v4l2-ctl') is not None
 
     def set_parameters(self, camera: UsbCamera, device: Device) -> None:
+        assert device.capture is not None
         camera.fps = int(device.capture.get(cv2.CAP_PROP_FPS))
         if not camera.auto_exposure and camera.exposure is None and device.exposure_max > 0:
             camera.exposure = device.exposure_default / device.exposure_max
         if 'MJPG' in device.video_formats:
             # NOTE enforcing motion jpeg for now
             if device.capture.get(cv2.CAP_PROP_FOURCC) != MJPG:
                 device.capture.set(cv2.CAP_PROP_FOURCC, MJPG)
@@ -249,15 +255,15 @@
             device.has_manual_exposure = True
             device.exposure_min = int(match.group(1))
             device.exposure_max = int(match.group(2))
             device.exposure_default = int(match.group(3))
         else:
             device.has_manual_exposure = False
         output = await self.run_v4l(device, '--list-formats')
-        match = re.finditer(r"$.*'(.*)'.*", output)
-        for m in match:
+        matches = re.finditer(r"$.*'(.*)'.*", output)
+        for m in matches:
             device.video_formats.add(m.group(1))
 
-    async def run_v4l(self, device: Device, *args) -> None:
+    async def run_v4l(self, device: Device, *args) -> str:
         cmd = ['v4l2-ctl', '-d', str(device.video_id)]
         cmd.extend(args)
         return await rosys.run.sh(cmd)
```

### Comparing `rosys-0.8.5/rosys/vision/usb_camera_provider_simulation.py` & `rosys-0.9.0/rosys/vision/usb_camera_provider_simulation.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.5/setup.py` & `rosys-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,19 +26,22 @@
  'aioserial>=1.3.0,<2.0.0',
  'asyncio>=3.4.3,<4.0.0',
  'coloredlogs>=15.0.1,<16.0.0',
  'dataclasses-json>=0.5.7,<0.6.0',
  'executing>=1.0.0,<2.0.0',
  'httpx>=0.24.0,<0.25.0',
  'humanize>=4.0.0,<5.0.0',
- 'line-profiler>=4.0.2,<5.0.0',
+ 'imgsize>=2.1,<3.0',
+ 'line-profiler>=4.0.3,<5.0.0',
+ 'matplotlib>=3.7.2,<4.0.0',
  'more-itertools>=8.10.0,<9.0.0',
  'msgpack>=1.0.3,<2.0.0',
+ 'netifaces>=0.11.0,<0.12.0',
  'networkx>=2.6.2,<3.0.0',
- 'nicegui==1.2.17',
+ 'nicegui>=1.3.2',
  'numpy>=1.20.1,<2.0.0',
  'objgraph>=3.5.0,<4.0.0',
  'opencv-contrib-python-headless>=4.5.4,<5.0.0',
  'opencv-python>=4.5.5,<5.0.0',
  'psutil>=5.9.0,<6.0.0',
  'pyloot>=0.1.0,<0.2.0',
  'pyserial>=3.5,<4.0',
@@ -51,15 +54,15 @@
  'tabulate>=0.8.9,<0.9.0',
  'ujson==5.4.0',
  'uvloop>=0.17.0,<0.18.0',
  'yappi>=1.4,<2.0']
 
 setup_kwargs = {
     'name': 'rosys',
-    'version': '0.8.5',
+    'version': '0.9.0',
     'description': 'Modular Robot System With Elegant Automation Capabilities',
     'long_description': '# RoSys - The Robot System\n\nRoSys provides an easy-to-use robot system.\nIts purpose is similar to [ROS](https://www.ros.org/).\nBut RoSys is fully based on modern web technologies and focusses on mobile robotics.\n\nThe full documentation is available at [rosys.io](https://rosys.io/).\n\n## Principles\n\n### All Python\n\nPython is great to write business logic.\nComputation-heavy tasks are wrapped in processes, accessed through WebSockets or called via C++ bindings.\nLike you would do in any other Python program.\n\n### Modularity\n\nYou can structure your code as you please.\nRoSys provides its magic without assuming a specific file structure, configuration files or enforced naming.\n\n### Event Loop\n\nThanks to [asyncio](https://docs.python.org/3/library/asyncio.html) you can write your business logic without locks and mutexes.\nThe execution is [parallel but not concurrent](https://realpython.com/python-concurrency/) which makes it easier to read, write and debug.\nIn real-case scenarios this is also much faster than [ROS](https://www.ros.org/).\nIts multiprocessing architecture requires too much inter-process communication.\n\n### Web UI\n\nMost machines need some kind of human interaction.\nRoSys is built from the ground up to make sure your robot can be operated fully off the grid with any web browser.\nThis is done by incorporating [NiceGUI](https://nicegui.io/), a wonderful all-Python UI web framework.\nIt is also possible to proxy the user interface through a gateway for remote operation.\n\n### Simulation\n\nRobot hardware is often slower than your own computer.\nTo rapidly test out new behavior and algorithms, RoSys provides a simulation mode.\nHere, all hardware is mocked and can even be manipulated to test wheel blockages and similar.\n\n### Testing\n\nYou can use [pytest](https://docs.pytest.org/) to write high-level integration tests.\nIt is based on the above-described simulation mode and accelerates the robot\'s time for super fast execution.\n\n## Architecture and Features\n\n### Modules\n\nRoSys modules are just Python modules which encapsulate certain functionality.\nThey can hold their own state, register lifecycle hooks, run methods repeatedly and subscribe to or raise [events](#events).\nModules can depend on other modules which is mostly implemented by passing them into the constructor.\n\n### Lifecycle Hooks and Loops\n\nModules can register functions for being called `on_startup` or `on_shutdown` as well as repeatedly with a given interval with `on_repeat`.\n\n### Events\n\nModules can provide events to allow connecting otherwise separated modules of the system.\nFor example, one module might read sensor data and raise an event `NEW_SENSOR_DATA`, without knowing of any consumers.\nAnother module can register on `NEW_SENSOR_DATA` and act accordingly when being called.\n\n### Automations\n\nRoSys provides an `Automator` module for running "automations".\nAutomations are coroutines that can not only be started and stopped, but also paused and resumed, e.g. using `AutomationControls`.\nHave a look at our [Click-and-drive](examples/click-and-drive.md) example.\n\n### Persistence\n\nModules can register backup and restore methods to read and write their state to disk.\n\n### Time\n\nRoSys uses its own time which is accessible through `rosys.time`.\nThis way the time can advance much faster in simulation and tests if no CPU-intensive operation is performed.\nTo delay the execution of a coroutine, you should invoke `await rosys.sleep(seconds: float)`.\nThis creates a delay until the provided amount of _RoSys time_ has elapsed.\n\n### Threading and Multiprocessing\n\nRoSys makes extensive use of [async/await](#async) to achieve parallelism without threading or multiprocessing.\nBut not every piece of code you want to integrate is offering an asyncio interface.\nTherefore RoSys provides two handy wrappers:\n\nIO-bound:\nIf you need to read from an external device or use a non-async HTTP library like [requests](https://requests.readthedocs.io/),\nyou should wrap the code in a function and await it with `await rosys.run.io_bound(...)`.\n\nCPU-bound:\nIf you need to do some heavy computation and want to spawn another process,\nyou should wrap the code in a function and await it with `await rosys.run.cpu_bound(...)`.\n\n### Safety\n\nPython (and Linux) is fast enough for most high-level logic, but has no realtime guarantees.\nSafety-relevant behavior should therefore be put on a suitable microcontroller.\nIt governs the hardware of the robot and must be able to perform safety actions like triggering emergency hold etc.\n\nWe suggest to use an industrial PC with an integrated controller like the [Zauberzeug Robot Brain](https://www.zauberzeug.com/robot-brain.html).\nIt provides a Linux system to run RoSys, offers AI acceleration via NVidia Jetson, two integrated [ESP32](https://www.espressif.com/en/products/socs/esp32) microcontrollers and six I/O sockets with up to 24 GPIOs for digital I/Os, CAN, RS485, SPI, I2C, etc.\nIt also has two hardware ENABLE switches and one which is controllable via software.\n\nTo have flexible configuration for the microcontroller we created another open source project called [Lizard](https://lizard.dev/).\nIt is a domain-specific language interpreted by the microcontroller which enables you to write reactive hardware behavior without recompiling and flashing.\n\n### User Interface\n\nRoSys builds upon the open source project [NiceGUI](https://nicegui.io/) and offers many robot-related UI elements.\nNiceGUI is a high-level UI framework for the web.\nThis means you can write all UI code in Python and the state is automatically reflected in the browser through WebSockets.\nSee any of our [examples](examples/steering.md).\n\nRoSys can also be used with other user interfaces or interaction models if required, for example a completely app-based control through Bluetooth Low Energy with Flutter.\n\n### Notifications\n\nModules can notify the user through `rosys.notify(\'message to the user\')`.\nWhen using NiceGUI, the notifications will show as snackbar messages.\nThe history of notifications is stored in the list `rosys.notifications`.\n',
     'author': 'Zauberzeug GmbH',
     'author_email': 'info@zauberzeug.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/zauberzeug/rosys',
```

### Comparing `rosys-0.8.5/PKG-INFO` & `rosys-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosys
-Version: 0.8.5
+Version: 0.9.0
 Summary: Modular Robot System With Elegant Automation Capabilities
 Home-page: https://github.com/zauberzeug/rosys
 License: MIT
 Keywords: robot,framework,automation,control,steer
 Author: Zauberzeug GmbH
 Author-email: info@zauberzeug.com
 Requires-Python: >=3.10,<3.12
@@ -18,19 +18,22 @@
 Requires-Dist: aioserial (>=1.3.0,<2.0.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
 Requires-Dist: executing (>=1.0.0,<2.0.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: humanize (>=4.0.0,<5.0.0)
-Requires-Dist: line-profiler (>=4.0.2,<5.0.0)
+Requires-Dist: imgsize (>=2.1,<3.0)
+Requires-Dist: line-profiler (>=4.0.3,<5.0.0)
+Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
 Requires-Dist: more-itertools (>=8.10.0,<9.0.0)
 Requires-Dist: msgpack (>=1.0.3,<2.0.0)
+Requires-Dist: netifaces (>=0.11.0,<0.12.0)
 Requires-Dist: networkx (>=2.6.2,<3.0.0)
-Requires-Dist: nicegui (==1.2.17)
+Requires-Dist: nicegui (>=1.3.2)
 Requires-Dist: numpy (>=1.20.1,<2.0.0)
 Requires-Dist: objgraph (>=3.5.0,<4.0.0)
 Requires-Dist: opencv-contrib-python-headless (>=4.5.4,<5.0.0)
 Requires-Dist: opencv-python (>=4.5.5,<5.0.0)
 Requires-Dist: psutil (>=5.9.0,<6.0.0)
 Requires-Dist: pyloot (>=0.1.0,<0.2.0)
 Requires-Dist: pyserial (>=3.5,<4.0)
```

