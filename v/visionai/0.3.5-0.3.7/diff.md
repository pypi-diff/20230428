# Comparing `tmp/visionai-0.3.5.tar.gz` & `tmp/visionai-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visionai-0.3.5.tar", max compression
+gzip compressed data, was "visionai-0.3.7.tar", max compression
```

## Comparing `visionai-0.3.5.tar` & `visionai-0.3.7.tar`

### file list

```diff
@@ -1,81 +1,89 @@
--rw-r--r--   0        0        0     5294 2023-04-27 01:34:37.077145 visionai-0.3.5/LICENSE
--rw-r--r--   0        0        0    14097 2023-04-27 01:34:37.077145 visionai-0.3.5/README.md
--rw-r--r--   0        0        0      688 2023-04-27 01:34:37.077145 visionai-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      240 2023-04-27 01:34:45.349248 visionai-0.3.5/visionai/licenses/regcode-01/license.lic
--rw-r--r--   0        0        0       36 2023-04-27 01:34:45.349248 visionai-0.3.5/visionai/licenses/regcode-01/license.lic.txt
--rw-r--r--   0        0        0    13587 2023-04-27 01:34:44.205234 visionai-0.3.5/visionai/pytransform/__init__.py
--rw-r--r--   0        0        0     1047 2023-04-27 01:34:45.989256 visionai-0.3.5/visionai/visionai/__init__.py
--rw-r--r--   0        0        0     1255 2023-04-27 01:34:46.025257 visionai-0.3.5/visionai/visionai/__main__.py
--rw-r--r--   0        0        0     9859 2023-04-27 01:34:46.061257 visionai-0.3.5/visionai/visionai/apiutils/api.py
--rw-r--r--   0        0        0     3139 2023-04-27 01:34:46.097258 visionai-0.3.5/visionai/visionai/cli/__init__.py
--rw-r--r--   0        0        0     7539 2023-04-27 01:34:46.133258 visionai-0.3.5/visionai/visionai/cli/auth_app.py
--rw-r--r--   0        0        0    40867 2023-04-27 01:34:46.173259 visionai-0.3.5/visionai/visionai/cli/camera_app.py
--rw-r--r--   0        0        0    17423 2023-04-27 01:34:46.213259 visionai-0.3.5/visionai/visionai/cli/commands.py
--rw-r--r--   0        0        0    10807 2023-04-27 01:34:46.245259 visionai-0.3.5/visionai/visionai/cli/device_app.py
--rw-r--r--   0        0        0     1135 2023-04-27 01:34:46.281260 visionai-0.3.5/visionai/visionai/cli/get_config_values.py
--rw-r--r--   0        0        0    16459 2023-04-27 01:34:46.317260 visionai-0.3.5/visionai/visionai/cli/models_app.py
--rw-r--r--   0        0        0    30327 2023-04-27 01:34:46.353261 visionai-0.3.5/visionai/visionai/cli/pipeline_app.py
--rw-r--r--   0        0        0    36319 2023-04-27 01:34:46.393261 visionai-0.3.5/visionai/visionai/cli/scenario_app.py
--rw-r--r--   0        0        0     5547 2023-04-27 01:34:46.429262 visionai-0.3.5/visionai/visionai/cli/start_stop_influx_db.py
--rw-r--r--   0        0        0     5647 2023-04-27 01:34:46.465262 visionai-0.3.5/visionai/visionai/cli/start_stop_model_server.py
--rw-r--r--   0        0        0     5675 2023-04-27 01:34:46.497263 visionai-0.3.5/visionai/visionai/cli/start_stop_redis_grafana.py
--rw-r--r--   0        0        0     5531 2023-04-27 01:34:46.533263 visionai-0.3.5/visionai/visionai/cli/start_stop_web_app.py
--rw-r--r--   0        0        0     2831 2023-04-27 01:34:46.569264 visionai-0.3.5/visionai/visionai/cli/stop_cmd.py
--rw-r--r--   0        0        0    23007 2023-04-27 01:34:46.605264 visionai-0.3.5/visionai/visionai/cli/web_app.py
--rw-r--r--   0        0        0     3843 2023-04-27 01:34:46.677265 visionai-0.3.5/visionai/visionai/config/download_schema.py
--rw-r--r--   0        0        0    17303 2023-04-27 01:34:46.645264 visionai-0.3.5/visionai/visionai/config.py
--rw-r--r--   0        0        0     1075 2023-04-27 01:34:46.713265 visionai-0.3.5/visionai/visionai/events/__init__.py
--rw-r--r--   0        0        0    16443 2023-04-27 01:34:46.749266 visionai-0.3.5/visionai/visionai/events/events_engine.py
--rw-r--r--   0        0        0    20539 2023-04-27 01:34:46.781266 visionai-0.3.5/visionai/visionai/main.py
--rw-r--r--   0        0        0     1075 2023-04-27 01:34:46.817267 visionai-0.3.5/visionai/visionai/models/__init__.py
--rw-r--r--   0        0        0    79431 2023-04-27 01:34:46.861267 visionai-0.3.5/visionai/visionai/models/common.py
--rw-r--r--   0        0        0    99883 2023-04-27 01:34:46.925268 visionai-0.3.5/visionai/visionai/models/plots.py
--rw-r--r--   0        0        0    41043 2023-04-27 01:34:46.965268 visionai-0.3.5/visionai/visionai/models/triton_client.py
--rw-r--r--   0        0        0     6651 2023-04-27 01:34:47.001269 visionai-0.3.5/visionai/visionai/models/triton_client_yolov5.py
--rw-r--r--   0        0        0    14111 2023-04-27 01:34:47.037269 visionai-0.3.5/visionai/visionai/scenarios/__init__.py
--rw-r--r--   0        0        0    22759 2023-04-27 01:34:47.081270 visionai-0.3.5/visionai/visionai/scenarios/capture_media.py
--rw-r--r--   0        0        0    37083 2023-04-27 01:34:47.121270 visionai-0.3.5/visionai/visionai/scenarios/ergonomics_detection.py
--rw-r--r--   0        0        0     9383 2023-04-27 01:34:47.157271 visionai-0.3.5/visionai/visionai/scenarios/face_blur.py
--rw-r--r--   0        0        0    13299 2023-04-27 01:34:47.197271 visionai-0.3.5/visionai/visionai/scenarios/firearms_detection.py
--rw-r--r--   0        0        0    21687 2023-04-27 01:34:47.233272 visionai-0.3.5/visionai/visionai/scenarios/occupancy_monitoring.py
--rw-r--r--   0        0        0    46379 2023-04-27 01:34:47.277272 visionai-0.3.5/visionai/visionai/scenarios/people_taking_picture_detection.py
--rw-r--r--   0        0        0    17675 2023-04-27 01:34:47.313273 visionai-0.3.5/visionai/visionai/scenarios/ppe_detection.py
--rw-r--r--   0        0        0    23607 2023-04-27 01:34:47.349273 visionai-0.3.5/visionai/visionai/scenarios/productivity_detection.py
--rw-r--r--   0        0        0    14199 2023-04-27 01:34:47.389274 visionai-0.3.5/visionai/visionai/scenarios/restricted_zone.py
--rw-r--r--   0        0        0    33975 2023-04-27 01:34:47.429274 visionai-0.3.5/visionai/visionai/scenarios/slip_and_fall_detection.py
--rw-r--r--   0        0        0    12971 2023-04-27 01:34:47.465275 visionai-0.3.5/visionai/visionai/scenarios/smoke_and_fire_detection.py
--rw-r--r--   0        0        0     9095 2023-04-27 01:34:47.501275 visionai-0.3.5/visionai/visionai/scenarios/smoking_detection.py
--rw-r--r--   0        0        0     1071 2023-04-27 01:34:47.533275 visionai-0.3.5/visionai/visionai/tests/__init__.py
--rw-r--r--   0        0        0     7751 2023-04-27 01:34:47.569276 visionai-0.3.5/visionai/visionai/tests/test_cli_auth.py
--rw-r--r--   0        0        0    30479 2023-04-27 01:34:47.609276 visionai-0.3.5/visionai/visionai/tests/test_cli_camera.py
--rw-r--r--   0        0        0    11411 2023-04-27 01:34:47.645277 visionai-0.3.5/visionai/visionai/tests/test_cli_device.py
--rw-r--r--   0        0        0    10315 2023-04-27 01:34:47.681277 visionai-0.3.5/visionai/visionai/tests/test_cli_main.py
--rw-r--r--   0        0        0     9887 2023-04-27 01:34:47.717278 visionai-0.3.5/visionai/visionai/tests/test_cli_models.py
--rw-r--r--   0        0        0    15231 2023-04-27 01:34:47.753278 visionai-0.3.5/visionai/visionai/tests/test_cli_pipeline.py
--rw-r--r--   0        0        0    13367 2023-04-27 01:34:47.789279 visionai-0.3.5/visionai/visionai/tests/test_cli_scenario.py
--rw-r--r--   0        0        0     9231 2023-04-27 01:34:47.825279 visionai-0.3.5/visionai/visionai/tests/test_cli_stop_cmd.py
--rw-r--r--   0        0        0    10115 2023-04-27 01:34:47.857279 visionai-0.3.5/visionai/visionai/tests/test_cli_web.py
--rw-r--r--   0        0        0     7475 2023-04-27 01:34:47.893280 visionai-0.3.5/visionai/visionai/tests/test_config_download_schema.py
--rw-r--r--   0        0        0     6207 2023-04-27 01:34:47.929280 visionai-0.3.5/visionai/visionai/tests/test_deps.py
--rw-r--r--   0        0        0     5399 2023-04-27 01:34:47.961281 visionai-0.3.5/visionai/visionai/tests/test_docker_cli.py
--rw-r--r--   0        0        0     5103 2023-04-27 01:34:47.997281 visionai-0.3.5/visionai/visionai/tests/test_ergonomics_scenario.py
--rw-r--r--   0        0        0     5047 2023-04-27 01:34:48.033282 visionai-0.3.5/visionai/visionai/tests/test_face_blur_scenario.py
--rw-r--r--   0        0        0     5103 2023-04-27 01:34:48.069282 visionai-0.3.5/visionai/visionai/tests/test_firearm_scenario.py
--rw-r--r--   0        0        0     5287 2023-04-27 01:34:48.113283 visionai-0.3.5/visionai/visionai/tests/test_occupancy_monitoring_scenario.py
--rw-r--r--   0        0        0     4571 2023-04-27 01:34:48.149283 visionai-0.3.5/visionai/visionai/tests/test_opencv_stream.py
--rw-r--r--   0        0        0     5291 2023-04-27 01:34:48.185284 visionai-0.3.5/visionai/visionai/tests/test_people_taking_picture_scenario.py
--rw-r--r--   0        0        0     4943 2023-04-27 01:34:48.221284 visionai-0.3.5/visionai/visionai/tests/test_ppe_scenario.py
--rw-r--r--   0        0        0     9791 2023-04-27 01:34:48.257284 visionai-0.3.5/visionai/visionai/tests/test_redis_grafana.py
--rw-r--r--   0        0        0     5091 2023-04-27 01:34:48.293285 visionai-0.3.5/visionai/visionai/tests/test_restricted_zone_scenario.py
--rw-r--r--   0        0        0    11287 2023-04-27 01:34:48.329285 visionai-0.3.5/visionai/visionai/tests/test_scenarios_json.py
--rw-r--r--   0        0        0     5239 2023-04-27 01:34:48.361286 visionai-0.3.5/visionai/visionai/tests/test_slip_and_fall_scenario.py
--rw-r--r--   0        0        0     5271 2023-04-27 01:34:48.401286 visionai-0.3.5/visionai/visionai/tests/test_smoke_and_fire_scenario.py
--rw-r--r--   0        0        0     5071 2023-04-27 01:34:48.437287 visionai-0.3.5/visionai/visionai/tests/test_smoking_scenario.py
--rw-r--r--   0        0        0    14743 2023-04-27 01:34:48.473287 visionai-0.3.5/visionai/visionai/util/__init__.py
--rw-r--r--   0        0        0    42711 2023-04-27 01:34:48.513288 visionai-0.3.5/visionai/visionai/util/docker_utils.py
--rw-r--r--   0        0        0    16951 2023-04-27 01:34:48.553288 visionai-0.3.5/visionai/visionai/util/download_models.py
--rw-r--r--   0        0        0    74399 2023-04-27 01:34:48.597289 visionai-0.3.5/visionai/visionai/util/general.py
--rw-r--r--   0        0        0    42279 2023-04-27 01:34:48.641289 visionai-0.3.5/visionai/visionai/util/image_utils.py
--rw-r--r--   0        0        0    51867 2023-04-27 01:34:48.685290 visionai-0.3.5/visionai/visionai/util/metrics.py
--rw-r--r--   0        0        0    37939 2023-04-27 01:34:48.725290 visionai-0.3.5/visionai/visionai/util/track.py
--rw-r--r--   0        0        0    14910 1970-01-01 00:00:00.000000 visionai-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     5294 2023-04-27 04:18:17.955464 visionai-0.3.7/LICENSE
+-rw-r--r--   0        0        0    14097 2023-04-27 04:18:17.955464 visionai-0.3.7/README.md
+-rw-r--r--   0        0        0      688 2023-04-27 04:18:17.955464 visionai-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/__init__.py
+-rw-r--r--   0        0        0       28 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/__main__.py
+-rw-r--r--   0        0        0     1369 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/apiutils/api.py
+-rw-r--r--   0        0        0     3742 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/cli/README.md
+-rw-r--r--   0        0        0      495 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/cli/__init__.py
+-rw-r--r--   0        0        0      941 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/cli/auth_app.py
+-rw-r--r--   0        0        0    11314 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/cli/camera_app.py
+-rw-r--r--   0        0        0     5735 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/cli/commands.py
+-rw-r--r--   0        0        0     1626 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/cli/device_app.py
+-rw-r--r--   0        0        0        0 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/cli/get_config_values.py
+-rw-r--r--   0        0        0     3326 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/cli/models_app.py
+-rw-r--r--   0        0        0     6229 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/cli/pipeline_app.py
+-rw-r--r--   0        0        0    11404 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/cli/scenario_app.py
+-rw-r--r--   0        0        0      900 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/cli/start_stop_influx_db.py
+-rw-r--r--   0        0        0      938 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/cli/start_stop_model_server.py
+-rw-r--r--   0        0        0      944 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/cli/start_stop_redis_grafana.py
+-rw-r--r--   0        0        0      894 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/cli/start_stop_web_app.py
+-rw-r--r--   0        0        0      421 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/cli/stop_cmd.py
+-rw-r--r--   0        0        0     7307 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/cli/web_app.py
+-rw-r--r--   0        0        0       87 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/config/.gitignore
+-rw-r--r--   0        0        0        0 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/config/.gitkeep
+-rw-r--r--   0        0        0     1624 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/config/camera-schema.json
+-rw-r--r--   0        0        0      475 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/config/download_schema.py
+-rw-r--r--   0        0        0     5702 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/config.py
+-rw-r--r--   0        0        0        0 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/events/__init__.py
+-rw-r--r--   0        0        0     5001 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/events/events_engine.py
+-rw-r--r--   0        0        0     4504 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/main.py
+-rw-r--r--   0        0        0        6 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/models/.gitignore
+-rw-r--r--   0        0        0     2055 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/models/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/models/__init__.py
+-rw-r--r--   0        0        0    17211 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/models/common.py
+-rw-r--r--   0        0        0    25516 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/models/plots.py
+-rw-r--r--   0        0        0    15970 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/models/triton_client.py
+-rw-r--r--   0        0        0     2260 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/models/triton_client_yolov5.py
+-rw-r--r--   0        0        0        2 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/models-repo/.gitignore
+-rw-r--r--   0        0        0        0 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/models-repo/.gitkeep
+-rw-r--r--   0        0        0    12833 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/scenarios/README.md
+-rw-r--r--   0        0        0     2676 2023-04-27 04:18:17.955464 visionai-0.3.7/visionai/scenarios/__init__.py
+-rw-r--r--   0        0        0     5741 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/scenarios/capture_media.py
+-rw-r--r--   0        0        0    10906 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/scenarios/ergonomics_detection.py
+-rw-r--r--   0        0        0     2370 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/scenarios/face_blur.py
+-rw-r--r--   0        0        0     2868 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/scenarios/firearms_detection.py
+-rw-r--r--   0        0        0     5759 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/scenarios/occupancy_monitoring.py
+-rw-r--r--   0        0        0    16207 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/scenarios/people_taking_picture_detection.py
+-rw-r--r--   0        0        0     5220 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/scenarios/ppe_detection.py
+-rw-r--r--   0        0        0     6900 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/scenarios/productivity_detection.py
+-rw-r--r--   0        0        0     3467 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/scenarios/restricted_zone.py
+-rw-r--r--   0        0        0   144646 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/scenarios/scenarios.json
+-rw-r--r--   0        0        0     9363 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/scenarios/slip_and_fall_detection.py
+-rw-r--r--   0        0        0     2842 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/scenarios/smoke_and_fire_detection.py
+-rw-r--r--   0        0        0     2021 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/scenarios/smoking_detection.py
+-rw-r--r--   0        0        0        0 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/__init__.py
+-rw-r--r--   0        0        0      660 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/docker-compose.yml
+-rw-r--r--   0        0        0      862 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_cli_auth.py
+-rw-r--r--   0        0        0     7325 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_cli_camera.py
+-rw-r--r--   0        0        0     1588 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_cli_device.py
+-rw-r--r--   0        0        0     1375 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_cli_main.py
+-rw-r--r--   0        0        0     1296 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_cli_models.py
+-rw-r--r--   0        0        0     2475 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_cli_pipeline.py
+-rw-r--r--   0        0        0     2494 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_cli_scenario.py
+-rw-r--r--   0        0        0     2656 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_cli_stop_cmd.py
+-rw-r--r--   0        0        0     2903 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_cli_web.py
+-rw-r--r--   0        0        0     1624 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_config_download_schema.py
+-rw-r--r--   0        0        0      770 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_deps.py
+-rw-r--r--   0        0        0      696 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_docker_cli.py
+-rw-r--r--   0        0        0      606 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_ergonomics_scenario.py
+-rw-r--r--   0        0        0      576 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_face_blur_scenario.py
+-rw-r--r--   0        0        0      599 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_firearm_scenario.py
+-rw-r--r--   0        0        0      630 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_occupancy_monitoring_scenario.py
+-rw-r--r--   0        0        0      768 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_opencv_stream.py
+-rw-r--r--   0        0        0      630 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_people_taking_picture_scenario.py
+-rw-r--r--   0        0        0      565 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_ppe_scenario.py
+-rw-r--r--   0        0        0     2846 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_redis_grafana.py
+-rw-r--r--   0        0        0      580 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_restricted_zone_scenario.py
+-rw-r--r--   0        0        0     2742 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_scenarios_json.py
+-rw-r--r--   0        0        0      631 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_slip_and_fall_scenario.py
+-rw-r--r--   0        0        0      722 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_smoke_and_fire_scenario.py
+-rw-r--r--   0        0        0      595 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/tests/test_smoking_scenario.py
+-rw-r--r--   0        0        0     1766 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/util/__init__.py
+-rw-r--r--   0        0        0    13339 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/util/docker_utils.py
+-rw-r--r--   0        0        0     4688 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/util/download_models.py
+-rw-r--r--   0        0        0    16148 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/util/general.py
+-rw-r--r--   0        0        0    13828 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/util/image_utils.py
+-rw-r--r--   0        0        0    14600 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/util/metrics.py
+-rw-r--r--   0        0        0     9226 2023-04-27 04:18:17.959464 visionai-0.3.7/visionai/util/track.py
+-rw-r--r--   0        0        0    14910 1970-01-01 00:00:00.000000 visionai-0.3.7/PKG-INFO
```

### Comparing `visionai-0.3.5/LICENSE` & `visionai-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `visionai-0.3.5/README.md` & `visionai-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `visionai-0.3.5/pyproject.toml` & `visionai-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "visionai"
-version = "0.3.5"
+version = "0.3.7"
 description = "Vision AI toolkit"
 authors = ["Harsh Murari <hmurari@visionify.ai>"]
 readme = "README.md"
 license = "VPSLA 1.0"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `visionai-0.3.5/PKG-INFO` & `visionai-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visionai
-Version: 0.3.5
+Version: 0.3.7
 Summary: Vision AI toolkit
 License: VPSLA 1.0
 Author: Harsh Murari
 Author-email: hmurari@visionify.ai
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: visionai Version: 0.3.5 Summary: Vision AI toolkit
+Metadata-Version: 2.1 Name: visionai Version: 0.3.7 Summary: Vision AI toolkit
 License: VPSLA 1.0 Author: Harsh Murari Author-email: hmurari@visionify.ai
 Requires-Python: >=3.7,<4.0 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: coloredlogs (>=15.0.0) Requires-Dist: docker (>=5.0.3,<7.0.0)
```

