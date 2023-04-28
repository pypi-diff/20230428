# Comparing `tmp/rosys-0.8.2.tar.gz` & `tmp/rosys-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosys-0.8.2.tar", max compression
+gzip compressed data, was "rosys-0.8.3.tar", max compression
```

## Comparing `rosys-0.8.2.tar` & `rosys-0.8.3.tar`

### file list

```diff
@@ -1,140 +1,140 @@
--rw-r--r--   0        0        0     1072 2023-04-04 11:04:41.743053 rosys-0.8.2/LICENSE
--rw-r--r--   0        0        0     6070 2023-04-04 11:04:41.743053 rosys-0.8.2/README.md
--rw-r--r--   0        0        0     1422 2023-04-04 11:04:52.211185 rosys-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      445 2023-04-04 11:04:41.759054 rosys-0.8.2/rosys/__init__.py
--rw-r--r--   0        0        0      581 2023-04-04 11:04:41.759054 rosys-0.8.2/rosys/analysis/__init__.py
--rw-r--r--   0        0        0    86820 2023-04-04 11:04:41.759054 rosys-0.8.2/rosys/analysis/assets/RobotoMono-Medium.ttf
--rw-r--r--   0        0        0     1833 2023-04-04 11:04:41.759054 rosys-0.8.2/rosys/analysis/asyncio_warnings.py
--rw-r--r--   0        0        0      712 2023-04-04 11:04:41.759054 rosys-0.8.2/rosys/analysis/kpi_buckets.py
--rw-r--r--   0        0        0     2089 2023-04-04 11:04:41.759054 rosys-0.8.2/rosys/analysis/kpi_logger.py
--rw-r--r--   0        0        0     3734 2023-04-04 11:04:41.759054 rosys-0.8.2/rosys/analysis/kpi_page_.py
--rw-r--r--   0        0        0        0 2023-04-04 11:04:41.759054 rosys-0.8.2/rosys/analysis/legacy/__init__.py
--rw-r--r--   0        0        0     3226 2023-04-04 11:04:41.759054 rosys-0.8.2/rosys/analysis/legacy/asyncio_monitor.py
--rw-r--r--   0        0        0     1869 2023-04-04 11:04:41.759054 rosys-0.8.2/rosys/analysis/legacy/asyncio_page.py
--rw-r--r--   0        0        0      973 2023-04-04 11:04:41.759054 rosys-0.8.2/rosys/analysis/legacy/cpu_usage.py
--rw-r--r--   0        0        0     1202 2023-04-04 11:04:41.759054 rosys-0.8.2/rosys/analysis/legacy/lizard_stats.py
--rw-r--r--   0        0        0     1970 2023-04-04 11:04:41.759054 rosys-0.8.2/rosys/analysis/legacy/network_monitor.py
--rw-r--r--   0        0        0     2959 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/analysis/legacy/objgraph_page.py
--rw-r--r--   0        0        0      717 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/analysis/legacy/pyloot_page.py
--rw-r--r--   0        0        0     2455 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/analysis/memory.py
--rw-r--r--   0        0        0     1624 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/analysis/profile_button_.py
--rw-r--r--   0        0        0     1038 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/analysis/profiling.py
--rw-r--r--   0        0        0     4266 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/analysis/timelapse_recorder.py
--rw-r--r--   0        0        0      693 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/analysis/track.py
--rw-r--r--   0        0        0      768 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/analysis/videos_page_.py
--rw-r--r--   0        0        0      232 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/automation/__init__.py
--rw-r--r--   0        0        0     5085 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/automation/app_controls_.py
--rw-r--r--   0        0        0     2752 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/automation/automation.py
--rw-r--r--   0        0        0     1642 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/automation/automation_controls_.py
--rw-r--r--   0        0        0     5643 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/automation/automator.py
--rw-r--r--   0        0        0     9369 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/automation/schedule.py
--rw-r--r--   0        0        0      531 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/config.py
--rw-r--r--   0        0        0      397 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/driving/__init__.py
--rw-r--r--   0        0        0      194 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/driving/drivable.py
--rw-r--r--   0        0        0     7882 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/driving/driver.py
--rw-r--r--   0        0        0     1979 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/driving/driver_object.py
--rw-r--r--   0        0        0      643 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/driving/joystick_.py
--rw-r--r--   0        0        0     2242 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/driving/keyboard_control_.py
--rw-r--r--   0        0        0     3532 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/driving/odometer.py
--rw-r--r--   0        0        0      169 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/driving/path_segment.py
--rw-r--r--   0        0        0     1768 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/driving/robot_object_.py
--rw-r--r--   0        0        0     3088 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/driving/steerer.py
--rw-r--r--   0        0        0     2961 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/event.py
--rw-r--r--   0        0        0      295 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/geometry/__init__.py
--rw-r--r--   0        0        0     1193 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/geometry/line.py
--rw-r--r--   0        0        0     1629 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/geometry/line_segment.py
--rw-r--r--   0        0        0     1844 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/geometry/point.py
--rw-r--r--   0        0        0      915 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/geometry/point3d.py
--rw-r--r--   0        0        0     3696 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/geometry/pose.py
--rw-r--r--   0        0        0      344 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/geometry/prism.py
--rw-r--r--   0        0        0      640 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/geometry/rectangle.py
--rw-r--r--   0        0        0     1732 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/geometry/rotation.py
--rw-r--r--   0        0        0     8874 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/geometry/spline.py
--rw-r--r--   0        0        0      142 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/geometry/velocity.py
--rw-r--r--   0        0        0      565 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/hardware/__init__.py
--rw-r--r--   0        0        0     3874 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/hardware/bms.py
--rw-r--r--   0        0        0     3105 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/hardware/bms_message.py
--rw-r--r--   0        0        0      770 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/hardware/bms_state.py
--rw-r--r--   0        0        0     2216 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/hardware/bumper.py
--rw-r--r--   0        0        0      657 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/hardware/can.py
--rw-r--r--   0        0        0      143 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/hardware/communication/__init__.py
--rw-r--r--   0        0        0      751 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/hardware/communication/communication.py
--rw-r--r--   0        0        0     3066 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/hardware/communication/serial_communication.py
--rw-r--r--   0        0        0     1434 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/hardware/communication/web_communication.py
--rw-r--r--   0        0        0     1564 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/hardware/estop.py
--rw-r--r--   0        0        0      637 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/hardware/expander.py
--rwxr-xr-x   0        0        0     1123 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/hardware/hardware_proxy.py
--rw-r--r--   0        0        0     4837 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/hardware/lizard_firmware.py
--rw-r--r--   0        0        0      830 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/hardware/module.py
--rw-r--r--   0        0        0     2609 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/hardware/robot.py
--rw-r--r--   0        0        0     8065 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/hardware/robot_brain.py
--rw-r--r--   0        0        0      607 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/hardware/serial.py
--rw-r--r--   0        0        0     4434 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/hardware/wheels.py
--rw-r--r--   0        0        0     2082 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/helpers.py
--rw-r--r--   0        0        0      260 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/__init__.py
--rw-r--r--   0        0        0      236 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/area.py
--rw-r--r--   0        0        0     1013 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/area_object_.py
--rw-r--r--   0        0        0     1372 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/binary_renderer.py
--rwxr-xr-x   0        0        0     1094 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/binary_renderer_demo.py
--rw-r--r--   0        0        0    13904 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/delaunay_planner.py
--rw-r--r--   0        0        0      220 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/delaunay_pose_group.py
--rw-r--r--   0        0        0     2831 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/demos/20220714-1.py
--rw-r--r--   0        0        0     2943 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/demos/20220714-2-A.py
--rw-r--r--   0        0        0     2939 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/demos/20220714-2-B.py
--rw-r--r--   0        0        0     2940 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/demos/20220714-3.py
--rw-r--r--   0        0        0     3196 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/demos/20220725-1.py
--rw-r--r--   0        0        0    38753 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/demos/20220825-1.py
--rw-r--r--   0        0        0    16920 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/demos/20220916-1.py
--rw-r--r--   0        0        0     3907 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/demos/20220921-1.py
--rw-r--r--   0        0        0     4217 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/demos/20221121-1.py
--rw-r--r--   0        0        0     4220 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/demos/20221203-1.py
--rw-r--r--   0        0        0    32139 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/demos/20230120-1.py
--rw-r--r--   0        0        0     2948 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/distance_map.py
--rwxr-xr-x   0        0        0     1757 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/distance_map_demo.py
--rw-r--r--   0        0        0     1815 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/experiments.py
--rwxr-xr-x   0        0        0      473 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/experiments_demo.py
--rw-r--r--   0        0        0     1885 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/fast_spline.py
--rw-r--r--   0        0        0     1980 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/grid.py
--rwxr-xr-x   0        0        0      466 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/grid_demo.py
--rw-r--r--   0        0        0      156 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/obstacle.py
--rw-r--r--   0        0        0     4126 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/obstacle_map.py
--rwxr-xr-x   0        0        0     1253 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/obstacle_map_demo.py
--rw-r--r--   0        0        0      751 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/obstacle_object_.py
--rw-r--r--   0        0        0      856 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/path_object_.py
--rw-r--r--   0        0        0     5210 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/path_planner.py
--rwxr-xr-x   0        0        0     2962 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/planner_demo.py
--rw-r--r--   0        0        0     3073 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/planner_process.py
--rw-r--r--   0        0        0     1955 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/plot_tools.py
--rwxr-xr-x   0        0        0     1237 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/plot_tools_demo.py
--rw-r--r--   0        0        0     1020 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/robot_renderer.py
--rwxr-xr-x   0        0        0      622 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/robot_renderer_demo.py
--rw-r--r--   0        0        0     2759 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/steps.py
--rwxr-xr-x   0        0        0     1749 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/pathplanning/steps_demo.py
--rw-r--r--   0        0        0     3955 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/persistence.py
--rw-r--r--   0        0        0     7764 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/rosys.py
--rw-r--r--   0        0        0     4291 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/run.py
--rw-r--r--   0        0        0      708 2023-04-04 11:04:41.763054 rosys-0.8.2/rosys/simulation_ui.py
--rw-r--r--   0        0        0       52 2023-04-04 11:04:41.767053 rosys-0.8.2/rosys/system/__init__.py
--rw-r--r--   0        0        0     2221 2023-04-04 11:04:41.767053 rosys-0.8.2/rosys/system/wifi_button_.py
--rw-r--r--   0        0        0      194 2023-04-04 11:04:41.767053 rosys-0.8.2/rosys/test/__init__.py
--rw-r--r--   0        0        0     4404 2023-04-04 11:04:41.767053 rosys-0.8.2/rosys/test/helpers.py
--rw-r--r--   0        0        0     2615 2023-04-04 11:04:41.767053 rosys-0.8.2/rosys/test/log_configuration.py
--rw-r--r--   0        0        0      728 2023-04-04 11:04:41.767053 rosys-0.8.2/rosys/vision/__init__.py
--rw-r--r--   0        0        0     5066 2023-04-04 11:04:41.767053 rosys-0.8.2/rosys/vision/calibration.py
--rw-r--r--   0        0        0     1819 2023-04-04 11:04:41.767053 rosys-0.8.2/rosys/vision/camera.py
--rw-r--r--   0        0        0     4576 2023-04-04 11:04:41.767053 rosys-0.8.2/rosys/vision/camera_objects_.py
--rw-r--r--   0        0        0     2725 2023-04-04 11:04:41.767053 rosys-0.8.2/rosys/vision/camera_projector.py
--rw-r--r--   0        0        0     2841 2023-04-04 11:04:41.767053 rosys-0.8.2/rosys/vision/camera_provider.py
--rw-r--r--   0        0        0     4214 2023-04-04 11:04:41.767053 rosys-0.8.2/rosys/vision/detections.py
--rw-r--r--   0        0        0     1497 2023-04-04 11:04:41.767053 rosys-0.8.2/rosys/vision/detector.py
--rw-r--r--   0        0        0     6059 2023-04-04 11:04:41.767053 rosys-0.8.2/rosys/vision/detector_hardware.py
--rw-r--r--   0        0        0     4598 2023-04-04 11:04:41.767053 rosys-0.8.2/rosys/vision/detector_simulation.py
--rw-r--r--   0        0        0     1325 2023-04-04 11:04:41.767053 rosys-0.8.2/rosys/vision/image.py
--rw-r--r--   0        0        0     2240 2023-04-04 11:04:41.767053 rosys-0.8.2/rosys/vision/image_route.py
--rw-r--r--   0        0        0      612 2023-04-04 11:04:41.767053 rosys-0.8.2/rosys/vision/multi_camera_provider.py
--rw-r--r--   0        0        0     1004 2023-04-04 11:04:41.767053 rosys-0.8.2/rosys/vision/uploads.py
--rw-r--r--   0        0        0     1699 2023-04-04 11:04:41.767053 rosys-0.8.2/rosys/vision/usb_camera.py
--rw-r--r--   0        0        0    11647 2023-04-04 11:04:41.767053 rosys-0.8.2/rosys/vision/usb_camera_provider_hardware.py
--rw-r--r--   0        0        0     3126 2023-04-04 11:04:41.767053 rosys-0.8.2/rosys/vision/usb_camera_provider_simulation.py
--rw-r--r--   0        0        0     7979 1970-01-01 00:00:00.000000 rosys-0.8.2/setup.py
--rw-r--r--   0        0        0     7968 1970-01-01 00:00:00.000000 rosys-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-28 14:07:16.679110 rosys-0.8.3/LICENSE
+-rw-r--r--   0        0        0     6070 2023-04-28 14:07:16.679110 rosys-0.8.3/README.md
+-rw-r--r--   0        0        0     1441 2023-04-28 14:07:28.867681 rosys-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0      445 2023-04-28 14:07:16.695111 rosys-0.8.3/rosys/__init__.py
+-rw-r--r--   0        0        0      581 2023-04-28 14:07:16.695111 rosys-0.8.3/rosys/analysis/__init__.py
+-rw-r--r--   0        0        0    86820 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/analysis/assets/RobotoMono-Medium.ttf
+-rw-r--r--   0        0        0     1833 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/analysis/asyncio_warnings.py
+-rw-r--r--   0        0        0      712 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/analysis/kpi_buckets.py
+-rw-r--r--   0        0        0     2089 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/analysis/kpi_logger.py
+-rw-r--r--   0        0        0     4477 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/analysis/kpi_page_.py
+-rw-r--r--   0        0        0        0 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/analysis/legacy/__init__.py
+-rw-r--r--   0        0        0     3226 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/analysis/legacy/asyncio_monitor.py
+-rw-r--r--   0        0        0     1869 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/analysis/legacy/asyncio_page.py
+-rw-r--r--   0        0        0      973 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/analysis/legacy/cpu_usage.py
+-rw-r--r--   0        0        0     1202 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/analysis/legacy/lizard_stats.py
+-rw-r--r--   0        0        0     1970 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/analysis/legacy/network_monitor.py
+-rw-r--r--   0        0        0     2959 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/analysis/legacy/objgraph_page.py
+-rw-r--r--   0        0        0      717 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/analysis/legacy/pyloot_page.py
+-rw-r--r--   0        0        0     2455 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/analysis/memory.py
+-rw-r--r--   0        0        0     1624 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/analysis/profile_button_.py
+-rw-r--r--   0        0        0     1038 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/analysis/profiling.py
+-rw-r--r--   0        0        0     4266 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/analysis/timelapse_recorder.py
+-rw-r--r--   0        0        0      693 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/analysis/track.py
+-rw-r--r--   0        0        0      768 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/analysis/videos_page_.py
+-rw-r--r--   0        0        0      232 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/automation/__init__.py
+-rw-r--r--   0        0        0     5085 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/automation/app_controls_.py
+-rw-r--r--   0        0        0     2752 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/automation/automation.py
+-rw-r--r--   0        0        0     1642 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/automation/automation_controls_.py
+-rw-r--r--   0        0        0     5738 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/automation/automator.py
+-rw-r--r--   0        0        0     9829 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/automation/schedule.py
+-rw-r--r--   0        0        0      531 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/config.py
+-rw-r--r--   0        0        0      397 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/driving/__init__.py
+-rw-r--r--   0        0        0      194 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/driving/drivable.py
+-rw-r--r--   0        0        0     7882 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/driving/driver.py
+-rw-r--r--   0        0        0     1979 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/driving/driver_object.py
+-rw-r--r--   0        0        0      643 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/driving/joystick_.py
+-rw-r--r--   0        0        0     2242 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/driving/keyboard_control_.py
+-rw-r--r--   0        0        0     3532 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/driving/odometer.py
+-rw-r--r--   0        0        0      169 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/driving/path_segment.py
+-rw-r--r--   0        0        0     1768 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/driving/robot_object_.py
+-rw-r--r--   0        0        0     3088 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/driving/steerer.py
+-rw-r--r--   0        0        0     2961 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/event.py
+-rw-r--r--   0        0        0      295 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/geometry/__init__.py
+-rw-r--r--   0        0        0     1193 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/geometry/line.py
+-rw-r--r--   0        0        0     1629 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/geometry/line_segment.py
+-rw-r--r--   0        0        0     1844 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/geometry/point.py
+-rw-r--r--   0        0        0      915 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/geometry/point3d.py
+-rw-r--r--   0        0        0     3696 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/geometry/pose.py
+-rw-r--r--   0        0        0      344 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/geometry/prism.py
+-rw-r--r--   0        0        0      640 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/geometry/rectangle.py
+-rw-r--r--   0        0        0     1732 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/geometry/rotation.py
+-rw-r--r--   0        0        0     8874 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/geometry/spline.py
+-rw-r--r--   0        0        0      142 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/geometry/velocity.py
+-rw-r--r--   0        0        0      565 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/hardware/__init__.py
+-rw-r--r--   0        0        0     3874 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/hardware/bms.py
+-rw-r--r--   0        0        0     3105 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/hardware/bms_message.py
+-rw-r--r--   0        0        0      770 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/hardware/bms_state.py
+-rw-r--r--   0        0        0     2216 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/hardware/bumper.py
+-rw-r--r--   0        0        0      657 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/hardware/can.py
+-rw-r--r--   0        0        0      143 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/hardware/communication/__init__.py
+-rw-r--r--   0        0        0      751 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/hardware/communication/communication.py
+-rw-r--r--   0        0        0     3066 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/hardware/communication/serial_communication.py
+-rw-r--r--   0        0        0     1434 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/hardware/communication/web_communication.py
+-rw-r--r--   0        0        0     1564 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/hardware/estop.py
+-rw-r--r--   0        0        0      637 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/hardware/expander.py
+-rwxr-xr-x   0        0        0     1123 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/hardware/hardware_proxy.py
+-rw-r--r--   0        0        0     4837 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/hardware/lizard_firmware.py
+-rw-r--r--   0        0        0      830 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/hardware/module.py
+-rw-r--r--   0        0        0     2609 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/hardware/robot.py
+-rw-r--r--   0        0        0     8065 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/hardware/robot_brain.py
+-rw-r--r--   0        0        0      607 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/hardware/serial.py
+-rw-r--r--   0        0        0     4434 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/hardware/wheels.py
+-rw-r--r--   0        0        0     2082 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/helpers.py
+-rw-r--r--   0        0        0      260 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/pathplanning/__init__.py
+-rw-r--r--   0        0        0      236 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/pathplanning/area.py
+-rw-r--r--   0        0        0     1013 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/pathplanning/area_object_.py
+-rw-r--r--   0        0        0     1372 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/pathplanning/binary_renderer.py
+-rwxr-xr-x   0        0        0     1094 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/pathplanning/binary_renderer_demo.py
+-rw-r--r--   0        0        0    13904 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/pathplanning/delaunay_planner.py
+-rw-r--r--   0        0        0      220 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/pathplanning/delaunay_pose_group.py
+-rw-r--r--   0        0        0     2831 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/pathplanning/demos/20220714-1.py
+-rw-r--r--   0        0        0     2943 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/pathplanning/demos/20220714-2-A.py
+-rw-r--r--   0        0        0     2939 2023-04-28 14:07:16.699111 rosys-0.8.3/rosys/pathplanning/demos/20220714-2-B.py
+-rw-r--r--   0        0        0     2940 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/demos/20220714-3.py
+-rw-r--r--   0        0        0     3196 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/demos/20220725-1.py
+-rw-r--r--   0        0        0    38753 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/demos/20220825-1.py
+-rw-r--r--   0        0        0    16920 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/demos/20220916-1.py
+-rw-r--r--   0        0        0     3907 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/demos/20220921-1.py
+-rw-r--r--   0        0        0     4217 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/demos/20221121-1.py
+-rw-r--r--   0        0        0     4220 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/demos/20221203-1.py
+-rw-r--r--   0        0        0    32139 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/demos/20230120-1.py
+-rw-r--r--   0        0        0     2948 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/distance_map.py
+-rwxr-xr-x   0        0        0     1757 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/distance_map_demo.py
+-rw-r--r--   0        0        0     1815 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/experiments.py
+-rwxr-xr-x   0        0        0      473 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/experiments_demo.py
+-rw-r--r--   0        0        0     1885 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/fast_spline.py
+-rw-r--r--   0        0        0     1980 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/grid.py
+-rwxr-xr-x   0        0        0      466 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/grid_demo.py
+-rw-r--r--   0        0        0      156 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/obstacle.py
+-rw-r--r--   0        0        0     4126 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/obstacle_map.py
+-rwxr-xr-x   0        0        0     1253 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/obstacle_map_demo.py
+-rw-r--r--   0        0        0      751 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/obstacle_object_.py
+-rw-r--r--   0        0        0      856 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/path_object_.py
+-rw-r--r--   0        0        0     5210 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/path_planner.py
+-rwxr-xr-x   0        0        0     2962 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/planner_demo.py
+-rw-r--r--   0        0        0     3073 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/planner_process.py
+-rw-r--r--   0        0        0     1955 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/plot_tools.py
+-rwxr-xr-x   0        0        0     1237 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/plot_tools_demo.py
+-rw-r--r--   0        0        0     1020 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/robot_renderer.py
+-rwxr-xr-x   0        0        0      622 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/robot_renderer_demo.py
+-rw-r--r--   0        0        0     2759 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/steps.py
+-rwxr-xr-x   0        0        0     1749 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/pathplanning/steps_demo.py
+-rw-r--r--   0        0        0     3959 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/persistence.py
+-rw-r--r--   0        0        0     7764 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/rosys.py
+-rw-r--r--   0        0        0     4291 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/run.py
+-rw-r--r--   0        0        0      708 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/simulation_ui.py
+-rw-r--r--   0        0        0       52 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/system/__init__.py
+-rw-r--r--   0        0        0     2221 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/system/wifi_button_.py
+-rw-r--r--   0        0        0      194 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/test/__init__.py
+-rw-r--r--   0        0        0     4404 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/test/helpers.py
+-rw-r--r--   0        0        0     2615 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/test/log_configuration.py
+-rw-r--r--   0        0        0      728 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/vision/__init__.py
+-rw-r--r--   0        0        0     5066 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/vision/calibration.py
+-rw-r--r--   0        0        0     1819 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/vision/camera.py
+-rw-r--r--   0        0        0     4576 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/vision/camera_objects_.py
+-rw-r--r--   0        0        0     2725 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/vision/camera_projector.py
+-rw-r--r--   0        0        0     2841 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/vision/camera_provider.py
+-rw-r--r--   0        0        0     4214 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/vision/detections.py
+-rw-r--r--   0        0        0     1497 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/vision/detector.py
+-rw-r--r--   0        0        0     6059 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/vision/detector_hardware.py
+-rw-r--r--   0        0        0     4620 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/vision/detector_simulation.py
+-rw-r--r--   0        0        0     1325 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/vision/image.py
+-rw-r--r--   0        0        0     2240 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/vision/image_route.py
+-rw-r--r--   0        0        0      612 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/vision/multi_camera_provider.py
+-rw-r--r--   0        0        0     1004 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/vision/uploads.py
+-rw-r--r--   0        0        0     1699 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/vision/usb_camera.py
+-rw-r--r--   0        0        0    11647 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/vision/usb_camera_provider_hardware.py
+-rw-r--r--   0        0        0     3126 2023-04-28 14:07:16.703111 rosys-0.8.3/rosys/vision/usb_camera_provider_simulation.py
+-rw-r--r--   0        0        0     8006 1970-01-01 00:00:00.000000 rosys-0.8.3/setup.py
+-rw-r--r--   0        0        0     8009 1970-01-01 00:00:00.000000 rosys-0.8.3/PKG-INFO
```

### Comparing `rosys-0.8.2/LICENSE` & `rosys-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/README.md` & `rosys-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/pyproject.toml` & `rosys-0.8.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "rosys"
-version = "v0.8.2"
+version = "v0.8.3"
 description = "Modular Robot System With Elegant Automation Capabilities"
 authors = ["Zauberzeug GmbH <info@zauberzeug.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/zauberzeug/rosys"
 keywords = ["robot", "framework", "automation", "control", "steer"]
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.12"
-nicegui = "1.2.5"
+nicegui = "1.2.10"
 asyncio = "^3.4.3"
 retry = "^0.9.2"
 aenum = "^3.1.5"
 requests = "^2.25.1"
 aiohttp = "^3.8.3"
 simplejson = "^3.17.2"
 pyserial = "^3.5"
@@ -37,14 +37,15 @@
 dataclasses-json = "^0.5.7"
 executing = "^1.0.0"
 suntime = "^1.2.5"
 line-profiler = "^4.0.2"
 yappi = "^1.4"
 pyloot = "^0.1.0"
 objgraph = "^3.5.0"
+httpx = "^0.24.0"
 
 [tool.poetry.dev-dependencies]
 autopep8 = "^1.5.5"
 pytest = "^6.2.1"
 pytest-watch = "^4.2.0"
 pytest-flakefinder = "^1.0.0"
 pytest-profiling = "^1.7.0"
```

### Comparing `rosys-0.8.2/rosys/analysis/__init__.py` & `rosys-0.8.3/rosys/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/analysis/assets/RobotoMono-Medium.ttf` & `rosys-0.8.3/rosys/analysis/assets/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/analysis/asyncio_warnings.py` & `rosys-0.8.3/rosys/analysis/asyncio_warnings.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/analysis/kpi_buckets.py` & `rosys-0.8.3/rosys/analysis/kpi_buckets.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/analysis/kpi_logger.py` & `rosys-0.8.3/rosys/analysis/kpi_logger.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/analysis/kpi_page_.py` & `rosys-0.8.3/rosys/analysis/kpi_page_.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,110 @@
+from abc import ABC, abstractmethod
 from itertools import groupby
 
 import humanize
 from matplotlib.colors import hsv_to_rgb, to_hex
 from nicegui import ui
 
 from .kpi_buckets import Month, TimeBucket, Week
 from .kpi_logger import KpiLogger, str_to_date
 
 
-def kpi_page(kpi_logger: KpiLogger,
-             *,
-             timespans: dict[int, str],
-             positives: dict[str, str],
-             negatives: dict[str, str],
-             title: str = '',
-             positive_title: str = '',
-             negative_title: str = '') -> None:
-
-    humanize.activate('de')
-
-    @ui.page('/kpis')
-    def page():
-        with ui.row().style('margin:1em'):
-            ui.markdown(f'### {title}').style('margin:1.5em;margin-top:-1.2em;')
-            toggle = ui.toggle(timespans, value=list(timespans.keys())[0], on_change=lambda e: show(e.value))
-        with ui.row():
-            positive_chart = ui.chart({
-                'title': {'text': positive_title},
-                'chart': {'type': 'column'},
-                'xAxis': {},
-                'yAxis': {'title': False},
-                'credits': False,
-                'exporting': False,
-            })
-            negative_chart = ui.chart({
-                'title': {'text': negative_title},
-                'chart': {'type': 'column'},
-                'plotOptions': {'series': {'stacking': 'normal'}},
-                'xAxis': {},
-                'yAxis': {'title': False},
-                'colors': [to_hex(hsv_to_rgb((0, 1, i / 100.0))) for i in reversed(range(20, 120, 20))],
-                'credits': False,
-                'exporting': False,
-            })
-        ui.timer(5, lambda: show(toggle.value))
-
-        def show(num_days: int) -> None:
-            if num_days <= 7:
-                time_buckets = kpi_logger.days[-num_days:]
-            elif num_days % 7 == 0:
-                weeks = [list(v) for _, v in groupby(kpi_logger.days,
-                                                     key=lambda d: str_to_date(d.date).strftime('%y-%W'))][-num_days//7:]
-                time_buckets = [Week.from_buckets(days_in_week) for days_in_week in weeks]
-            elif num_days % 30 == 0 and num_days <= 90:
-                months = [list(v) for _, v in groupby(kpi_logger.days,
-                                                      key=lambda d: str_to_date(d.date).strftime('%y-%m'))][-num_days//30:]
-                time_buckets = [Month.from_buckets(days_in_month) for days_in_month in months]
-            else:
-                raise ValueError(f'Unsupported number of days: {num_days}')
+class kpi_page(ABC):
 
-            keys = set(key for day in time_buckets for key in day.incidents if key in positives)
-            data = {positives[key]: [day.incidents.get(key, 0) for day in time_buckets] for key in keys}
-            positive_chart.options['xAxis']['categories'] = [_label(b) for b in time_buckets]
-            positive_chart.options['series'] = [{'name': k, 'data': v} for k, v in sorted(data.items())]
-            positive_chart.update()
-
-            keys = set(key for day in time_buckets for key in day.incidents if key in negatives)
-            data = {negatives[key]: [day.incidents.get(key, 0) for day in time_buckets] for key in keys}
-            negative_chart.options['xAxis']['categories'] = [_label(b) for b in time_buckets]
-            negative_chart.options['series'] = [{'name': k, 'data': v} for k, v in sorted(data.items())]
-            negative_chart.update()
+    def __init__(self, kpi_logger: KpiLogger) -> None:
+        @ui.page('/kpis')
+        def page():
+            if self.language == 'de':
+                humanize.activate('de')
+            else:
+                humanize.deactivate()
+            with ui.row().style('margin:1em'):
+                ui.markdown(f'### {self.title}').style('margin:1.5em;margin-top:-1.2em;')
+                toggle = ui.toggle(self.timespans, value=list(self.timespans)[0], on_change=lambda e: show(e.value))
+            with ui.row():
+                positive_chart = ui.chart({
+                    'title': {'text': self.positive_title},
+                    'chart': {'type': 'column'},
+                    'xAxis': {},
+                    'yAxis': {'title': False},
+                    'credits': False,
+                    'exporting': False,
+                })
+                negative_chart = ui.chart({
+                    'title': {'text': self.negative_title},
+                    'chart': {'type': 'column'},
+                    'plotOptions': {'series': {'stacking': 'normal'}},
+                    'xAxis': {},
+                    'yAxis': {'title': False},
+                    'colors': [to_hex(hsv_to_rgb((0, 1, i / 100.0))) for i in reversed(range(20, 120, 20))],
+                    'credits': False,
+                    'exporting': False,
+                })
+            ui.timer(5, lambda: show(toggle.value))
+
+            def show(num_days: int) -> None:
+                if num_days <= 7:
+                    time_buckets = kpi_logger.days[-num_days:]
+                elif num_days % 7 == 0:
+                    weeks = [list(v) for _, v in groupby(kpi_logger.days,
+                                                         key=lambda d: str_to_date(d.date).strftime('%y-%W'))][-num_days//7:]
+                    time_buckets = [Week.from_buckets(days_in_week) for days_in_week in weeks]
+                elif num_days % 30 == 0 and num_days <= 90:
+                    months = [list(v) for _, v in groupby(kpi_logger.days,
+                                                          key=lambda d: str_to_date(d.date).strftime('%y-%m'))][-num_days//30:]
+                    time_buckets = [Month.from_buckets(days_in_month) for days_in_month in months]
+                else:
+                    raise ValueError(f'Unsupported number of days: {num_days}')
+
+                keys = set(key for day in time_buckets for key in day.incidents if key in self.positives)
+                data = {self.positives[key]: [day.incidents.get(key, 0) for day in time_buckets] for key in keys}
+                positive_chart.options['xAxis']['categories'] = [_label(b) for b in time_buckets]
+                positive_chart.options['series'] = [{'name': k, 'data': v} for k, v in sorted(data.items())]
+                positive_chart.update()
+
+                keys = set(key for day in time_buckets for key in day.incidents if key in self.negatives)
+                data = {self.negatives[key]: [day.incidents.get(key, 0) for day in time_buckets] for key in keys}
+                negative_chart.options['xAxis']['categories'] = [_label(b) for b in time_buckets]
+                negative_chart.options['series'] = [{'name': k, 'data': v} for k, v in sorted(data.items())]
+                negative_chart.update()
+
+    @property
+    def language(self) -> str:
+        return 'en'
+
+    @property
+    @abstractmethod
+    def title(self) -> str:
+        pass
+
+    @property
+    @abstractmethod
+    def positive_title(self) -> str:
+        pass
+
+    @property
+    @abstractmethod
+    def negative_title(self) -> str:
+        pass
+
+    @property
+    @abstractmethod
+    def positives(self) -> dict[str, str]:
+        pass
+
+    @property
+    @abstractmethod
+    def negatives(self) -> dict[str, str]:
+        pass
+
+    @property
+    @abstractmethod
+    def timespans(self) -> dict[int, str]:
+        pass
 
 
 def _label(time_bucket: TimeBucket) -> str:
     if isinstance(time_bucket, Month):
         return str_to_date(time_bucket.date).strftime('%b')
     elif isinstance(time_bucket, Week):
         return f'#{str_to_date(time_bucket.date).isocalendar()[1]}'
```

### Comparing `rosys-0.8.2/rosys/analysis/legacy/asyncio_monitor.py` & `rosys-0.8.3/rosys/analysis/legacy/asyncio_monitor.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/analysis/legacy/asyncio_page.py` & `rosys-0.8.3/rosys/analysis/legacy/asyncio_page.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/analysis/legacy/cpu_usage.py` & `rosys-0.8.3/rosys/analysis/legacy/cpu_usage.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/analysis/legacy/lizard_stats.py` & `rosys-0.8.3/rosys/analysis/legacy/lizard_stats.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/analysis/legacy/network_monitor.py` & `rosys-0.8.3/rosys/analysis/legacy/network_monitor.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/analysis/legacy/objgraph_page.py` & `rosys-0.8.3/rosys/analysis/legacy/objgraph_page.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/analysis/legacy/pyloot_page.py` & `rosys-0.8.3/rosys/analysis/legacy/pyloot_page.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/analysis/memory.py` & `rosys-0.8.3/rosys/analysis/memory.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/analysis/profile_button_.py` & `rosys-0.8.3/rosys/analysis/profile_button_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/analysis/profiling.py` & `rosys-0.8.3/rosys/analysis/profiling.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/analysis/timelapse_recorder.py` & `rosys-0.8.3/rosys/analysis/timelapse_recorder.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/analysis/track.py` & `rosys-0.8.3/rosys/analysis/track.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/analysis/videos_page_.py` & `rosys-0.8.3/rosys/analysis/videos_page_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/automation/app_controls_.py` & `rosys-0.8.3/rosys/automation/app_controls_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/automation/automation.py` & `rosys-0.8.3/rosys/automation/automation.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/automation/automation_controls_.py` & `rosys-0.8.3/rosys/automation/automation_controls_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/automation/automator.py` & `rosys-0.8.3/rosys/automation/automator.py`

 * *Files 13% similar despite different names*

```diff
@@ -68,31 +68,33 @@
     def is_running(self) -> bool:
         return self.automation is not None and self.automation.is_running
 
     @property
     def is_paused(self) -> bool:
         return self.automation is not None and self.automation.is_paused
 
-    def start(self, coro: Optional[Coroutine] = None) -> None:
+    def start(self, coro: Optional[Coroutine] = None, *, paused: bool = False) -> None:
         """Starts a new automation.
 
         You can pass any coroutine.
         The automator will make sure it can be paused, resumed and stopped.
         """
         if coro is None:
-            self.start(self.default_automation())
+            self.start(self.default_automation(), paused=paused)
             return
         if not self.enabled:
             coro.close()
             return
         self.stop(because='new automation starts')
         self.automation = Automation(coro, self._handle_exception, on_complete=self._on_complete)
         rosys.background_tasks.create(self.automation.__await__(), name='automation')
         self.AUTOMATION_STARTED.emit()
         rosys.notify('automation started')
+        if paused:
+            self.automation.pause()
 
     def pause(self, because: str) -> None:
         """Pauses the current automation.
 
         You need to provide a cause which will be used as notification message.
         """
         if self.is_running:
```

### Comparing `rosys-0.8.2/rosys/automation/schedule.py` & `rosys-0.8.3/rosys/automation/schedule.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,35 @@
 import suntime
 from nicegui import ui
 
 from .. import persistence, rosys
 from ..event import Event
 from .automator import Automator
 
-DAYS = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
+
+class Translator:
+    Location = 'Location'
+    Sunrise_offset = 'Sunrise offset'
+    Sunset_offset = 'Sunset offset'
+    min = 'min'
+    enabled = 'enabled'
+    Mon = 'Mon'
+    Tue = 'Tue'
+    Wed = 'Wed'
+    Thu = 'Thu'
+    Fri = 'Fri'
+    Sat = 'Sat'
+    Sun = 'Sun'
 
 
 class Schedule:
 
     def __init__(self,
                  automator: Automator, *,
+                 translator: Optional[Translator] = None,
                  on_activate: Optional[Callable] = None,
                  on_deactivate: Optional[Callable] = None,
                  location: Optional[tuple[float, float]] = None,
                  locations: Optional[dict[tuple[float, float], str]] = None,
                  sunrise_offset: float = 0.0,
                  sunset_offset: float = 0.0,
                  is_enabled: bool = False,
@@ -36,14 +50,15 @@
         """
         self.log = logging.getLogger('rosys.schedule')
 
         self.SCHEDULE_CHANGED = Event()
         """the schedule has changed"""
 
         self.automator = automator
+        self.translator = translator or Translator()
         self.on_activate = on_activate
         self.on_deactivate = on_deactivate
         self.location = location
         self.locations = locations
         self.sunrise_offset = sunrise_offset
         self.sunset_offset = sunset_offset
         self.is_enabled = is_enabled
@@ -109,21 +124,21 @@
     def step(self) -> None:
         if not self.is_enabled:
             return
         if not self._is_active and self.can_be_active():
             self.log.info('activate')
             if self.on_activate:
                 self.log.info('start automation')
-                self.automator.start(self.on_activate())
+                self.automator.start(self.on_activate(), paused=self.automator.is_paused)
             self._is_active = True
         if self._is_active and not self.can_be_active():
             self.log.info('deactivate')
             if self.on_deactivate:
                 self.log.info('start automation')
-                self.automator.start(self.on_deactivate())
+                self.automator.start(self.on_deactivate(), paused=self.automator.is_paused)
             self._is_active = False
 
     def ui(self) -> ui.row:
         def update() -> None:
             def color(weekday: int, hour: int, minutes: list[int]) -> str:
                 # https://maketintsandshades.com/#21ba45,c10015
                 if all(self.is_dark(hour, minute) for minute in minutes):
@@ -139,29 +154,30 @@
             for d in range(7):
                 for h in range(24):
                     b0, b1, b2 = buttons[d * 24 + h]
                     b0.classes(replace=f'!bg-[{color(d, h, [0, 30, 60])}]')
                     b1.classes(replace=f'!bg-[{color(d, h, [0, 30])}]')
                     b2.classes(replace=f'!bg-[{color(d, h, [30, 60])}]')
 
+        t = self.translator
         buttons: list[tuple[ui.button, ui.button, ui.button]] = []
         with ui.column() as grid:
             with ui.row().classes('fit items-center justify-between'):
-                ui.switch('enabled').bind_value(self, 'is_enabled')
+                ui.switch(t.enabled).bind_value(self, 'is_enabled')
                 if self.locations:
-                    ui.select(self.locations, label='Location', on_change=lambda e: self.set_location(e.value)) \
+                    ui.select(self.locations, label=t.Location, on_change=lambda e: self.set_location(e.value)) \
                         .bind_value(self, 'location').style('width: 21em')
-                    ui.number('Sunrise offset', format='%.0f', on_change=self.invalidate) \
-                        .bind_value(self, 'sunrise_offset').props('suffix=min').style('width:100px')
-                    ui.number('Sunset offset', format='%.0f', on_change=self.invalidate) \
-                        .bind_value(self, 'sunset_offset').props('suffix=min').style('width:100px')
+                    ui.number(t.Sunrise_offset, format='%.0f', on_change=self.invalidate, suffix=t.min) \
+                        .bind_value(self, 'sunrise_offset').style('width:100px')
+                    ui.number(t.Sunset_offset, format='%.0f', on_change=self.invalidate, suffix=t.min) \
+                        .bind_value(self, 'sunset_offset').style('width:100px')
             with ui.column().style('gap: 0.3em'):
-                for d in range(7):
+                for d, day in enumerate([t.Mon, t.Tue, t.Wed, t.Thu, t.Fri, t.Sat, t.Sun]):
                     with ui.row().style('gap: 0.3em'):
-                        ui.label(DAYS[d]).classes('mt-2').style('width: 2em')
+                        ui.label(day).classes('mt-2').style('width: 2em')
                         for h in range(24):
                             with ui.column().style('gap: 0.1em'):
                                 hour = ui.button(f'{h:02d}', on_click=lambda _, d=d, h=h: self._toggle(d, h)) \
                                     .props('unelevated dense')
                                 with ui.row().style('gap: 0.1em'):
                                     first_half = ui.button(on_click=lambda _, d=d, h=h: self._toggle(d, h, 0)) \
                                         .props('unelevated dense').style('height: 1em; width: 0.8em')
```

### Comparing `rosys-0.8.2/rosys/config.py` & `rosys-0.8.3/rosys/config.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/driving/driver.py` & `rosys-0.8.3/rosys/driving/driver.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/driving/driver_object.py` & `rosys-0.8.3/rosys/driving/driver_object.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/driving/joystick_.py` & `rosys-0.8.3/rosys/driving/joystick_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/driving/keyboard_control_.py` & `rosys-0.8.3/rosys/driving/keyboard_control_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/driving/odometer.py` & `rosys-0.8.3/rosys/driving/odometer.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/driving/robot_object_.py` & `rosys-0.8.3/rosys/driving/robot_object_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/driving/steerer.py` & `rosys-0.8.3/rosys/driving/steerer.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/event.py` & `rosys-0.8.3/rosys/event.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/geometry/line.py` & `rosys-0.8.3/rosys/geometry/line.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/geometry/line_segment.py` & `rosys-0.8.3/rosys/geometry/line_segment.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/geometry/point.py` & `rosys-0.8.3/rosys/geometry/point.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/geometry/point3d.py` & `rosys-0.8.3/rosys/geometry/point3d.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/geometry/pose.py` & `rosys-0.8.3/rosys/geometry/pose.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/geometry/rectangle.py` & `rosys-0.8.3/rosys/geometry/rectangle.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/geometry/rotation.py` & `rosys-0.8.3/rosys/geometry/rotation.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/geometry/spline.py` & `rosys-0.8.3/rosys/geometry/spline.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/hardware/__init__.py` & `rosys-0.8.3/rosys/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/hardware/bms.py` & `rosys-0.8.3/rosys/hardware/bms.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/hardware/bms_message.py` & `rosys-0.8.3/rosys/hardware/bms_message.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/hardware/bms_state.py` & `rosys-0.8.3/rosys/hardware/bms_state.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/hardware/bumper.py` & `rosys-0.8.3/rosys/hardware/bumper.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/hardware/can.py` & `rosys-0.8.3/rosys/hardware/can.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/hardware/communication/communication.py` & `rosys-0.8.3/rosys/hardware/communication/communication.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/hardware/communication/serial_communication.py` & `rosys-0.8.3/rosys/hardware/communication/serial_communication.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/hardware/communication/web_communication.py` & `rosys-0.8.3/rosys/hardware/communication/web_communication.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/hardware/estop.py` & `rosys-0.8.3/rosys/hardware/estop.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/hardware/expander.py` & `rosys-0.8.3/rosys/hardware/expander.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/hardware/hardware_proxy.py` & `rosys-0.8.3/rosys/hardware/hardware_proxy.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/hardware/lizard_firmware.py` & `rosys-0.8.3/rosys/hardware/lizard_firmware.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/hardware/module.py` & `rosys-0.8.3/rosys/hardware/module.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/hardware/robot.py` & `rosys-0.8.3/rosys/hardware/robot.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/hardware/robot_brain.py` & `rosys-0.8.3/rosys/hardware/robot_brain.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/hardware/serial.py` & `rosys-0.8.3/rosys/hardware/serial.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/hardware/wheels.py` & `rosys-0.8.3/rosys/hardware/wheels.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/helpers.py` & `rosys-0.8.3/rosys/helpers.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/area_object_.py` & `rosys-0.8.3/rosys/pathplanning/area_object_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/binary_renderer.py` & `rosys-0.8.3/rosys/pathplanning/binary_renderer.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/binary_renderer_demo.py` & `rosys-0.8.3/rosys/pathplanning/binary_renderer_demo.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/delaunay_planner.py` & `rosys-0.8.3/rosys/pathplanning/delaunay_planner.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/demos/20220714-1.py` & `rosys-0.8.3/rosys/pathplanning/demos/20220714-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/demos/20220714-2-A.py` & `rosys-0.8.3/rosys/pathplanning/demos/20220714-2-A.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/demos/20220714-2-B.py` & `rosys-0.8.3/rosys/pathplanning/demos/20220714-2-B.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/demos/20220714-3.py` & `rosys-0.8.3/rosys/pathplanning/demos/20220714-3.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/demos/20220725-1.py` & `rosys-0.8.3/rosys/pathplanning/demos/20220725-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/demos/20220825-1.py` & `rosys-0.8.3/rosys/pathplanning/demos/20220825-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/demos/20220916-1.py` & `rosys-0.8.3/rosys/pathplanning/demos/20220916-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/demos/20220921-1.py` & `rosys-0.8.3/rosys/pathplanning/demos/20220921-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/demos/20221121-1.py` & `rosys-0.8.3/rosys/pathplanning/demos/20221121-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/demos/20221203-1.py` & `rosys-0.8.3/rosys/pathplanning/demos/20221203-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/demos/20230120-1.py` & `rosys-0.8.3/rosys/pathplanning/demos/20230120-1.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/distance_map.py` & `rosys-0.8.3/rosys/pathplanning/distance_map.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/distance_map_demo.py` & `rosys-0.8.3/rosys/pathplanning/distance_map_demo.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/experiments.py` & `rosys-0.8.3/rosys/pathplanning/experiments.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/fast_spline.py` & `rosys-0.8.3/rosys/pathplanning/fast_spline.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/grid.py` & `rosys-0.8.3/rosys/pathplanning/grid.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/obstacle_map.py` & `rosys-0.8.3/rosys/pathplanning/obstacle_map.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/obstacle_map_demo.py` & `rosys-0.8.3/rosys/pathplanning/obstacle_map_demo.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/obstacle_object_.py` & `rosys-0.8.3/rosys/pathplanning/obstacle_object_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/path_object_.py` & `rosys-0.8.3/rosys/pathplanning/path_object_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/path_planner.py` & `rosys-0.8.3/rosys/pathplanning/path_planner.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/planner_demo.py` & `rosys-0.8.3/rosys/pathplanning/planner_demo.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/planner_process.py` & `rosys-0.8.3/rosys/pathplanning/planner_process.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/plot_tools.py` & `rosys-0.8.3/rosys/pathplanning/plot_tools.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/plot_tools_demo.py` & `rosys-0.8.3/rosys/pathplanning/plot_tools_demo.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/robot_renderer.py` & `rosys-0.8.3/rosys/pathplanning/robot_renderer.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/robot_renderer_demo.py` & `rosys-0.8.3/rosys/pathplanning/robot_renderer_demo.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/steps.py` & `rosys-0.8.3/rosys/pathplanning/steps.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/pathplanning/steps_demo.py` & `rosys-0.8.3/rosys/pathplanning/steps_demo.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/persistence.py` & `rosys-0.8.3/rosys/persistence.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 
 def export_button(title: str = 'Export', route: str = '/export', tmp_filepath: str = '/tmp/export.json') -> ui.button:
     @app.get(route)
     def get_export() -> FileResponse:
         with open(tmp_filepath, 'w') as f:
             json.dump({name: module.backup() for name, module in modules.items()}, f, indent=4)
         return FileResponse(tmp_filepath, filename='export.json')
-    ui.button(title, on_click=lambda: ui.open(route[1:]))
+    ui.button(title, on_click=lambda: ui.download(route[1:]))
 
 
 def import_button(title: str = 'Import', after_import: Optional[Callable] = None) -> ui.button:
     async def restore_from_file(e: UploadEventArguments) -> None:
         all_data = json.load(e.content)
         assert isinstance(all_data, dict)
         for name, data in all_data.items():
```

### Comparing `rosys-0.8.2/rosys/rosys.py` & `rosys-0.8.3/rosys/rosys.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/run.py` & `rosys-0.8.3/rosys/run.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/simulation_ui.py` & `rosys-0.8.3/rosys/simulation_ui.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/system/wifi_button_.py` & `rosys-0.8.3/rosys/system/wifi_button_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/test/helpers.py` & `rosys-0.8.3/rosys/test/helpers.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/test/log_configuration.py` & `rosys-0.8.3/rosys/test/log_configuration.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/vision/__init__.py` & `rosys-0.8.3/rosys/vision/__init__.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/vision/calibration.py` & `rosys-0.8.3/rosys/vision/calibration.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/vision/camera.py` & `rosys-0.8.3/rosys/vision/camera.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/vision/camera_objects_.py` & `rosys-0.8.3/rosys/vision/camera_objects_.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/vision/camera_projector.py` & `rosys-0.8.3/rosys/vision/camera_projector.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/vision/camera_provider.py` & `rosys-0.8.3/rosys/vision/camera_provider.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/vision/detections.py` & `rosys-0.8.3/rosys/vision/detections.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/vision/detector.py` & `rosys-0.8.3/rosys/vision/detector.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/vision/detector_hardware.py` & `rosys-0.8.3/rosys/vision/detector_hardware.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/vision/detector_simulation.py` & `rosys-0.8.3/rosys/vision/detector_simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     def uploads(self) -> Uploads:
         return self._uploads
 
     def step(self) -> None:
         self._uploads.queue.clear()
         self._uploads.priority_queue.clear()
 
-    async def detect(self, image: Image, autoupload: Autoupload = Autoupload.FILTERED) -> Optional[Detections]:
+    async def detect(self, image: Image, autoupload: Autoupload = Autoupload.FILTERED, tags: list[str] = []) -> Optional[Detections]:
         is_blocked = image.camera_id in self.blocked_cameras
         await rosys.sleep(0.4)
         image.detections = Detections()
         if not is_blocked:
             self.update_simulated_objects(image)
             self.detect_from_simulated_objects(image)
         self.NEW_DETECTIONS.emit(image)
```

### Comparing `rosys-0.8.2/rosys/vision/image.py` & `rosys-0.8.3/rosys/vision/image.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/vision/image_route.py` & `rosys-0.8.3/rosys/vision/image_route.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/vision/multi_camera_provider.py` & `rosys-0.8.3/rosys/vision/multi_camera_provider.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/vision/uploads.py` & `rosys-0.8.3/rosys/vision/uploads.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/vision/usb_camera.py` & `rosys-0.8.3/rosys/vision/usb_camera.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/vision/usb_camera_provider_hardware.py` & `rosys-0.8.3/rosys/vision/usb_camera_provider_hardware.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/rosys/vision/usb_camera_provider_simulation.py` & `rosys-0.8.3/rosys/vision/usb_camera_provider_simulation.py`

 * *Files identical despite different names*

### Comparing `rosys-0.8.2/setup.py` & `rosys-0.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,20 +24,21 @@
  'aiocache>=0.11.1,<0.12.0',
  'aiohttp>=3.8.3,<4.0.0',
  'aioserial>=1.3.0,<2.0.0',
  'asyncio>=3.4.3,<4.0.0',
  'coloredlogs>=15.0.1,<16.0.0',
  'dataclasses-json>=0.5.7,<0.6.0',
  'executing>=1.0.0,<2.0.0',
+ 'httpx>=0.24.0,<0.25.0',
  'humanize>=4.0.0,<5.0.0',
  'line-profiler>=4.0.2,<5.0.0',
  'more-itertools>=8.10.0,<9.0.0',
  'msgpack>=1.0.3,<2.0.0',
  'networkx>=2.6.2,<3.0.0',
- 'nicegui==1.2.5',
+ 'nicegui==1.2.10',
  'numpy>=1.20.1,<2.0.0',
  'objgraph>=3.5.0,<4.0.0',
  'opencv-contrib-python-headless>=4.5.4,<5.0.0',
  'opencv-python>=4.5.5,<5.0.0',
  'psutil>=5.9.0,<6.0.0',
  'pyloot>=0.1.0,<0.2.0',
  'pyserial>=3.5,<4.0',
@@ -50,15 +51,15 @@
  'tabulate>=0.8.9,<0.9.0',
  'ujson==5.4.0',
  'uvloop>=0.17.0,<0.18.0',
  'yappi>=1.4,<2.0']
 
 setup_kwargs = {
     'name': 'rosys',
-    'version': '0.8.2',
+    'version': '0.8.3',
     'description': 'Modular Robot System With Elegant Automation Capabilities',
     'long_description': '# RoSys - The Robot System\n\nRoSys provides an easy-to-use robot system.\nIts purpose is similar to [ROS](https://www.ros.org/).\nBut RoSys is fully based on modern web technologies and focusses on mobile robotics.\n\nThe full documentation is available at [rosys.io](https://rosys.io/).\n\n## Principles\n\n### All Python\n\nPython is great to write business logic.\nComputation-heavy tasks are wrapped in processes, accessed through WebSockets or called via C++ bindings.\nLike you would do in any other Python program.\n\n### Modularity\n\nYou can structure your code as you please.\nRoSys provides its magic without assuming a specific file structure, configuration files or enforced naming.\n\n### Event Loop\n\nThanks to [asyncio](https://docs.python.org/3/library/asyncio.html) you can write your business logic without locks and mutexes.\nThe execution is [parallel but not concurrent](https://realpython.com/python-concurrency/) which makes it easier to read, write and debug.\nIn real-case scenarios this is also much faster than [ROS](https://www.ros.org/).\nIts multiprocessing architecture requires too much inter-process communication.\n\n### Web UI\n\nMost machines need some kind of human interaction.\nRoSys is built from the ground up to make sure your robot can be operated fully off the grid with any web browser.\nThis is done by incorporating [NiceGUI](https://nicegui.io/), a wonderful all-Python UI web framework.\nIt is also possible to proxy the user interface through a gateway for remote operation.\n\n### Simulation\n\nRobot hardware is often slower than your own computer.\nTo rapidly test out new behavior and algorithms, RoSys provides a simulation mode.\nHere, all hardware is mocked and can even be manipulated to test wheel blockages and similar.\n\n### Testing\n\nYou can use [pytest](https://docs.pytest.org/) to write high-level integration tests.\nIt is based on the above-described simulation mode and accelerates the robot\'s time for super fast execution.\n\n## Architecture and Features\n\n### Modules\n\nRoSys modules are just Python modules which encapsulate certain functionality.\nThey can hold their own state, register lifecycle hooks, run methods repeatedly and subscribe to or raise [events](#events).\nModules can depend on other modules which is mostly implemented by passing them into the constructor.\n\n### Lifecycle Hooks and Loops\n\nModules can register functions for being called `on_startup` or `on_shutdown` as well as repeatedly with a given interval with `on_repeat`.\n\n### Events\n\nModules can provide events to allow connecting otherwise separated modules of the system.\nFor example, one module might read sensor data and raise an event `NEW_SENSOR_DATA`, without knowing of any consumers.\nAnother module can register on `NEW_SENSOR_DATA` and act accordingly when being called.\n\n### Automations\n\nRoSys provides an `Automator` module for running "automations".\nAutomations are coroutines that can not only be started and stopped, but also paused and resumed, e.g. using `AutomationControls`.\nHave a look at our [Click-and-drive](examples/click-and-drive.md) example.\n\n### Persistence\n\nModules can register backup and restore methods to read and write their state to disk.\n\n### Time\n\nRoSys uses its own time which is accessible through `rosys.time`.\nThis way the time can advance much faster in simulation and tests if no CPU-intensive operation is performed.\nTo delay the execution of a coroutine, you should invoke `await rosys.sleep(seconds: float)`.\nThis creates a delay until the provided amount of _RoSys time_ has elapsed.\n\n### Threading and Multiprocessing\n\nRoSys makes extensive use of [async/await](#async) to achieve parallelism without threading or multiprocessing.\nBut not every piece of code you want to integrate is offering an asyncio interface.\nTherefore RoSys provides two handy wrappers:\n\nIO-bound:\nIf you need to read from an external device or use a non-async HTTP library like [requests](https://requests.readthedocs.io/),\nyou should wrap the code in a function and await it with `await rosys.run.io_bound(...)`.\n\nCPU-bound:\nIf you need to do some heavy computation and want to spawn another process,\nyou should wrap the code in a function and await it with `await rosys.run.cpu_bound(...)`.\n\n### Safety\n\nPython (and Linux) is fast enough for most high-level logic, but has no realtime guarantees.\nSafety-relevant behavior should therefore be put on a suitable microcontroller.\nIt governs the hardware of the robot and must be able to perform safety actions like triggering emergency hold etc.\n\nWe suggest to use an industrial PC with an integrated controller like the [Zauberzeug Robot Brain](https://www.zauberzeug.com/robot-brain.html).\nIt provides a Linux system to run RoSys, offers AI acceleration via NVidia Jetson, two integrated [ESP32](https://www.espressif.com/en/products/socs/esp32) microcontrollers and six I/O sockets with up to 24 GPIOs for digital I/Os, CAN, RS485, SPI, I2C, etc.\nIt also has two hardware ENABLE switches and one which is controllable via software.\n\nTo have flexible configuration for the microcontroller we created another open source project called [Lizard](https://lizard.dev/).\nIt is a domain-specific language interpreted by the microcontroller which enables you to write reactive hardware behavior without recompiling and flashing.\n\n### User Interface\n\nRoSys builds upon the open source project [NiceGUI](https://nicegui.io/) and offers many robot-related UI elements.\nNiceGUI is a high-level UI framework for the web.\nThis means you can write all UI code in Python and the state is automatically reflected in the browser through WebSockets.\nSee any of our [examples](examples/steering.md).\n\nRoSys can also be used with other user interfaces or interaction models if required, for example a completely app-based control through Bluetooth Low Energy with Flutter.\n\n### Notifications\n\nModules can notify the user through `rosys.notify(\'message to the user\')`.\nWhen using NiceGUI, the notifications will show as snackbar messages.\nThe history of notifications is stored in the list `rosys.notifications`.\n',
     'author': 'Zauberzeug GmbH',
     'author_email': 'info@zauberzeug.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/zauberzeug/rosys',
```

### Comparing `rosys-0.8.2/PKG-INFO` & `rosys-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosys
-Version: 0.8.2
+Version: 0.8.3
 Summary: Modular Robot System With Elegant Automation Capabilities
 Home-page: https://github.com/zauberzeug/rosys
 License: MIT
 Keywords: robot,framework,automation,control,steer
 Author: Zauberzeug GmbH
 Author-email: info@zauberzeug.com
 Requires-Python: >=3.10,<3.12
@@ -16,20 +16,21 @@
 Requires-Dist: aiocache (>=0.11.1,<0.12.0)
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: aioserial (>=1.3.0,<2.0.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
 Requires-Dist: executing (>=1.0.0,<2.0.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: humanize (>=4.0.0,<5.0.0)
 Requires-Dist: line-profiler (>=4.0.2,<5.0.0)
 Requires-Dist: more-itertools (>=8.10.0,<9.0.0)
 Requires-Dist: msgpack (>=1.0.3,<2.0.0)
 Requires-Dist: networkx (>=2.6.2,<3.0.0)
-Requires-Dist: nicegui (==1.2.5)
+Requires-Dist: nicegui (==1.2.10)
 Requires-Dist: numpy (>=1.20.1,<2.0.0)
 Requires-Dist: objgraph (>=3.5.0,<4.0.0)
 Requires-Dist: opencv-contrib-python-headless (>=4.5.4,<5.0.0)
 Requires-Dist: opencv-python (>=4.5.5,<5.0.0)
 Requires-Dist: psutil (>=5.9.0,<6.0.0)
 Requires-Dist: pyloot (>=0.1.0,<0.2.0)
 Requires-Dist: pyserial (>=3.5,<4.0)
```

