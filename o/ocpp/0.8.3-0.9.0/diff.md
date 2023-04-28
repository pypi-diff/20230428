# Comparing `tmp/ocpp-0.8.3.tar.gz` & `tmp/ocpp-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocpp-0.8.3.tar", max compression
+gzip compressed data, was "ocpp-0.9.0.tar", max compression
```

## Comparing `ocpp-0.8.3.tar` & `ocpp-0.9.0.tar`

### file list

```diff
@@ -1,339 +1,361 @@
--rw-r--r--   0        0        0     1075 2019-05-26 10:35:41.352694 ocpp-0.8.3/LICENSE
--rw-r--r--   0        0        0     5116 2021-04-21 05:42:54.249548 ocpp-0.8.3/README.rst
--rw-r--r--   0        0        0        0 2019-06-23 11:43:56.726904 ocpp-0.8.3/ocpp/__init__.py
--rw-r--r--   0        0        0    11206 2021-04-21 15:15:51.582962 ocpp-0.8.3/ocpp/charge_point.py
--rw-r--r--   0        0        0     3167 2020-10-14 09:14:01.939596 ocpp-0.8.3/ocpp/exceptions.py
--rw-r--r--   0        0        0    15022 2020-11-14 11:33:24.085928 ocpp-0.8.3/ocpp/messages.py
--rw-r--r--   0        0        0     4084 2021-01-19 19:46:24.953892 ocpp-0.8.3/ocpp/routing.py
--rw-r--r--   0        0        0      186 2020-03-21 08:32:49.058585 ocpp-0.8.3/ocpp/v16/__init__.py
--rw-r--r--   0        0        0     4943 2020-10-29 09:03:38.585220 ocpp-0.8.3/ocpp/v16/call.py
--rw-r--r--   0        0        0     3663 2020-10-15 18:09:55.577662 ocpp-0.8.3/ocpp/v16/call_result.py
--rw-r--r--   0        0        0    17496 2020-11-13 14:00:40.618574 ocpp-0.8.3/ocpp/v16/enums.py
--rw-r--r--   0        0        0      306 2019-06-23 11:43:56.726904 ocpp-0.8.3/ocpp/v16/schemas/Authorize.json
--rw-r--r--   0        0        0     1062 2020-03-21 08:32:49.066585 ocpp-0.8.3/ocpp/v16/schemas/AuthorizeResponse.json
--rw-r--r--   0        0        0     1139 2019-06-23 11:43:56.726904 ocpp-0.8.3/ocpp/v16/schemas/BootNotification.json
--rw-r--r--   0        0        0      655 2020-03-21 08:32:49.066585 ocpp-0.8.3/ocpp/v16/schemas/BootNotificationResponse.json
--rw-r--r--   0        0        0      302 2019-06-23 11:43:56.726904 ocpp-0.8.3/ocpp/v16/schemas/CancelReservation.json
--rw-r--r--   0        0        0      423 2020-03-21 08:32:49.070585 ocpp-0.8.3/ocpp/v16/schemas/CancelReservationResponse.json
--rw-r--r--   0        0        0      512 2020-03-21 08:32:49.070585 ocpp-0.8.3/ocpp/v16/schemas/ChangeAvailability.json
--rw-r--r--   0        0        0      453 2020-03-21 08:32:49.074585 ocpp-0.8.3/ocpp/v16/schemas/ChangeAvailabilityResponse.json
--rw-r--r--   0        0        0      418 2019-06-23 11:43:56.726904 ocpp-0.8.3/ocpp/v16/schemas/ChangeConfiguration.json
--rw-r--r--   0        0        0      491 2020-03-21 08:32:49.074585 ocpp-0.8.3/ocpp/v16/schemas/ChangeConfigurationResponse.json
--rw-r--r--   0        0        0      174 2019-06-23 11:43:56.730904 ocpp-0.8.3/ocpp/v16/schemas/ClearCache.json
--rw-r--r--   0        0        0      416 2020-03-21 08:32:49.074585 ocpp-0.8.3/ocpp/v16/schemas/ClearCacheResponse.json
--rw-r--r--   0        0        0      637 2020-03-21 08:32:49.074585 ocpp-0.8.3/ocpp/v16/schemas/ClearChargingProfile.json
--rw-r--r--   0        0        0      425 2020-03-21 08:32:49.078585 ocpp-0.8.3/ocpp/v16/schemas/ClearChargingProfileResponse.json
--rw-r--r--   0        0        0      466 2019-06-23 11:43:56.730904 ocpp-0.8.3/ocpp/v16/schemas/DataTransfer.json
--rw-r--r--   0        0        0      547 2020-03-21 08:32:49.078585 ocpp-0.8.3/ocpp/v16/schemas/DataTransferResponse.json
--rw-r--r--   0        0        0      491 2020-03-21 08:32:49.078585 ocpp-0.8.3/ocpp/v16/schemas/DiagnosticsStatusNotification.json
--rw-r--r--   0        0        0      194 2019-06-23 11:43:56.730904 ocpp-0.8.3/ocpp/v16/schemas/DiagnosticsStatusNotificationResponse.json
--rw-r--r--   0        0        0      591 2020-03-21 08:32:49.078585 ocpp-0.8.3/ocpp/v16/schemas/FirmwareStatusNotification.json
--rw-r--r--   0        0        0      191 2019-06-23 11:43:56.730904 ocpp-0.8.3/ocpp/v16/schemas/FirmwareStatusNotificationResponse.json
--rw-r--r--   0        0        0      539 2020-03-21 08:32:49.082585 ocpp-0.8.3/ocpp/v16/schemas/GetCompositeSchedule.json
--rw-r--r--   0        0        0     2139 2020-03-21 08:32:49.082585 ocpp-0.8.3/ocpp/v16/schemas/GetCompositeScheduleResponse.json
--rw-r--r--   0        0        0      344 2020-03-21 08:32:49.082585 ocpp-0.8.3/ocpp/v16/schemas/GetConfiguration.json
--rw-r--r--   0        0        0     1066 2020-03-21 08:32:49.086586 ocpp-0.8.3/ocpp/v16/schemas/GetConfigurationResponse.json
--rw-r--r--   0        0        0      642 2019-06-23 11:43:56.734904 ocpp-0.8.3/ocpp/v16/schemas/GetDiagnostics.json
--rw-r--r--   0        0        0      275 2019-06-23 11:43:56.734904 ocpp-0.8.3/ocpp/v16/schemas/GetDiagnosticsResponse.json
--rw-r--r--   0        0        0      183 2019-06-23 11:43:56.734904 ocpp-0.8.3/ocpp/v16/schemas/GetLocalListVersion.json
--rw-r--r--   0        0        0      301 2019-06-23 11:43:56.734904 ocpp-0.8.3/ocpp/v16/schemas/GetLocalListVersionResponse.json
--rw-r--r--   0        0        0      173 2019-06-23 11:43:56.734904 ocpp-0.8.3/ocpp/v16/schemas/Heartbeat.json
--rw-r--r--   0        0        0      325 2019-06-23 11:43:56.734904 ocpp-0.8.3/ocpp/v16/schemas/HeartbeatResponse.json
--rw-r--r--   0        0        0     6692 2020-10-14 09:14:01.942596 ocpp-0.8.3/ocpp/v16/schemas/MeterValues.json
--rw-r--r--   0        0        0      176 2019-06-23 11:43:56.734904 ocpp-0.8.3/ocpp/v16/schemas/MeterValuesResponse.json
--rw-r--r--   0        0        0     4383 2020-03-21 08:32:49.086586 ocpp-0.8.3/ocpp/v16/schemas/RemoteStartTransaction.json
--rw-r--r--   0        0        0      428 2020-03-21 08:32:49.086586 ocpp-0.8.3/ocpp/v16/schemas/RemoteStartTransactionResponse.json
--rw-r--r--   0        0        0      306 2019-06-23 11:43:56.734904 ocpp-0.8.3/ocpp/v16/schemas/RemoteStopTransaction.json
--rw-r--r--   0        0        0      427 2020-03-21 08:32:49.090586 ocpp-0.8.3/ocpp/v16/schemas/RemoteStopTransactionResponse.json
--rw-r--r--   0        0        0      704 2019-06-23 11:43:56.734904 ocpp-0.8.3/ocpp/v16/schemas/ReserveNow.json
--rw-r--r--   0        0        0      502 2020-03-21 08:32:49.090586 ocpp-0.8.3/ocpp/v16/schemas/ReserveNowResponse.json
--rw-r--r--   0        0        0      398 2020-03-21 08:32:49.090586 ocpp-0.8.3/ocpp/v16/schemas/Reset.json
--rw-r--r--   0        0        0      411 2020-03-21 08:32:49.090586 ocpp-0.8.3/ocpp/v16/schemas/ResetResponse.json
--rw-r--r--   0        0        0     2146 2020-03-21 08:32:49.094586 ocpp-0.8.3/ocpp/v16/schemas/SendLocalList.json
--rw-r--r--   0        0        0      484 2020-03-21 08:32:49.094586 ocpp-0.8.3/ocpp/v16/schemas/SendLocalListResponse.json
--rw-r--r--   0        0        0     4310 2020-03-21 08:32:49.098586 ocpp-0.8.3/ocpp/v16/schemas/SetChargingProfile.json
--rw-r--r--   0        0        0      456 2020-03-21 08:32:49.098586 ocpp-0.8.3/ocpp/v16/schemas/SetChargingProfileResponse.json
--rw-r--r--   0        0        0      676 2019-06-23 11:43:56.734904 ocpp-0.8.3/ocpp/v16/schemas/StartTransaction.json
--rw-r--r--   0        0        0     1162 2020-03-21 08:32:49.098586 ocpp-0.8.3/ocpp/v16/schemas/StartTransactionResponse.json
--rw-r--r--   0        0        0     1805 2020-03-21 08:32:49.098586 ocpp-0.8.3/ocpp/v16/schemas/StatusNotification.json
--rw-r--r--   0        0        0      183 2019-06-23 11:43:56.738904 ocpp-0.8.3/ocpp/v16/schemas/StatusNotificationResponse.json
--rw-r--r--   0        0        0     7313 2020-03-21 08:32:49.098586 ocpp-0.8.3/ocpp/v16/schemas/StopTransaction.json
--rw-r--r--   0        0        0     1023 2020-03-21 08:32:49.102586 ocpp-0.8.3/ocpp/v16/schemas/StopTransactionResponse.json
--rw-r--r--   0        0        0      678 2020-03-21 08:32:49.102586 ocpp-0.8.3/ocpp/v16/schemas/TriggerMessage.json
--rw-r--r--   0        0        0      454 2020-03-21 08:32:49.102586 ocpp-0.8.3/ocpp/v16/schemas/TriggerMessageResponse.json
--rw-r--r--   0        0        0      296 2019-06-23 11:43:56.738904 ocpp-0.8.3/ocpp/v16/schemas/UnlockConnector.json
--rw-r--r--   0        0        0      457 2020-03-21 08:32:49.102586 ocpp-0.8.3/ocpp/v16/schemas/UnlockConnectorResponse.json
--rw-r--r--   0        0        0      572 2020-03-21 08:32:49.106586 ocpp-0.8.3/ocpp/v16/schemas/UpdateFirmware.json
--rw-r--r--   0        0        0      179 2019-06-23 11:43:56.738904 ocpp-0.8.3/ocpp/v16/schemas/UpdateFirmwareResponse.json
--rw-r--r--   0        0        0      186 2020-03-21 08:32:49.106586 ocpp-0.8.3/ocpp/v20/__init__.py
--rw-r--r--   0        0        0     7491 2020-10-15 18:09:55.577662 ocpp-0.8.3/ocpp/v20/call.py
--rw-r--r--   0        0        0     4907 2020-10-15 18:09:55.577662 ocpp-0.8.3/ocpp/v20/call_result.py
--rw-r--r--   0        0        0     2971 2020-03-21 08:32:49.110586 ocpp-0.8.3/ocpp/v20/schemas/AuthorizeRequest_v1p0.json
--rw-r--r--   0        0        0     3495 2020-03-21 08:32:49.110586 ocpp-0.8.3/ocpp/v20/schemas/AuthorizeResponse_v1p0.json
--rw-r--r--   0        0        0     1771 2020-03-21 08:32:49.110586 ocpp-0.8.3/ocpp/v20/schemas/BootNotificationRequest_v1p0.json
--rw-r--r--   0        0        0      560 2020-03-21 08:32:49.114586 ocpp-0.8.3/ocpp/v20/schemas/BootNotificationResponse_v1p0.json
--rw-r--r--   0        0        0      275 2020-03-21 08:32:49.114586 ocpp-0.8.3/ocpp/v20/schemas/CancelReservationRequest_v1p0.json
--rw-r--r--   0        0        0      365 2020-03-21 08:32:49.114586 ocpp-0.8.3/ocpp/v20/schemas/CancelReservationResponse_v1p0.json
--rw-r--r--   0        0        0      580 2020-03-21 08:32:49.114586 ocpp-0.8.3/ocpp/v20/schemas/CertificateSignedRequest_v1p0.json
--rw-r--r--   0        0        0      365 2020-03-21 08:32:49.114586 ocpp-0.8.3/ocpp/v20/schemas/CertificateSignedResponse_v1p0.json
--rw-r--r--   0        0        0      456 2020-03-21 08:32:49.114586 ocpp-0.8.3/ocpp/v20/schemas/ChangeAvailabilityRequest_v1p0.json
--rw-r--r--   0        0        0      387 2020-03-21 08:32:49.118586 ocpp-0.8.3/ocpp/v20/schemas/ChangeAvailabilityResponse_v1p0.json
--rw-r--r--   0        0        0      150 2020-03-21 08:32:49.118586 ocpp-0.8.3/ocpp/v20/schemas/ClearCacheRequest_v1p0.json
--rw-r--r--   0        0        0      365 2020-03-21 08:32:49.118586 ocpp-0.8.3/ocpp/v20/schemas/ClearCacheResponse_v1p0.json
--rw-r--r--   0        0        0     1029 2020-03-21 08:32:49.118586 ocpp-0.8.3/ocpp/v20/schemas/ClearChargingProfileRequest_v1p0.json
--rw-r--r--   0        0        0      364 2020-03-21 08:32:49.118586 ocpp-0.8.3/ocpp/v20/schemas/ClearChargingProfileResponse_v1p0.json
--rw-r--r--   0        0        0      253 2020-03-21 08:32:49.118586 ocpp-0.8.3/ocpp/v20/schemas/ClearDisplayMessageRequest_v1p0.json
--rw-r--r--   0        0        0      364 2020-03-21 08:32:49.118586 ocpp-0.8.3/ocpp/v20/schemas/ClearDisplayMessageResponse_v1p0.json
--rw-r--r--   0        0        0      361 2020-03-21 08:32:49.122586 ocpp-0.8.3/ocpp/v20/schemas/ClearVariableMonitoringRequest_v1p0.json
--rw-r--r--   0        0        0     1055 2020-03-21 08:32:49.122586 ocpp-0.8.3/ocpp/v20/schemas/ClearVariableMonitoringResponse_v1p0.json
--rw-r--r--   0        0        0      464 2020-03-21 08:32:49.122586 ocpp-0.8.3/ocpp/v20/schemas/ClearedChargingLimitRequest_v1p0.json
--rw-r--r--   0        0        0      150 2020-03-21 08:32:49.122586 ocpp-0.8.3/ocpp/v20/schemas/ClearedChargingLimitResponse_v1p0.json
--rw-r--r--   0        0        0      368 2020-03-21 08:32:49.122586 ocpp-0.8.3/ocpp/v20/schemas/CostUpdatedRequest_v1p0.json
--rw-r--r--   0        0        0      150 2020-03-21 08:32:49.122586 ocpp-0.8.3/ocpp/v20/schemas/CostUpdatedResponse_v1p0.json
--rw-r--r--   0        0        0     2862 2020-03-21 08:32:49.122586 ocpp-0.8.3/ocpp/v20/schemas/CustomerInformationRequest_v1p0.json
--rw-r--r--   0        0        0      385 2020-03-21 08:32:49.126586 ocpp-0.8.3/ocpp/v20/schemas/CustomerInformationResponse_v1p0.json
--rw-r--r--   0        0        0      382 2020-03-21 08:32:49.126586 ocpp-0.8.3/ocpp/v20/schemas/DataTransferRequest_v1p0.json
--rw-r--r--   0        0        0      439 2020-03-21 08:32:49.126586 ocpp-0.8.3/ocpp/v20/schemas/DataTransferResponse_v1p0.json
--rw-r--r--   0        0        0     1224 2020-03-21 08:32:49.126586 ocpp-0.8.3/ocpp/v20/schemas/DeleteCertificateRequest_v1p0.json
--rw-r--r--   0        0        0      384 2020-03-21 08:32:49.126586 ocpp-0.8.3/ocpp/v20/schemas/DeleteCertificateResponse_v1p0.json
--rw-r--r--   0        0        0      893 2020-03-21 08:32:49.130586 ocpp-0.8.3/ocpp/v20/schemas/FirmwareStatusNotificationRequest_v1p0.json
--rw-r--r--   0        0        0      150 2020-03-21 08:32:49.130586 ocpp-0.8.3/ocpp/v20/schemas/FirmwareStatusNotificationResponse_v1p0.json
--rw-r--r--   0        0        0      406 2020-03-21 08:32:49.130586 ocpp-0.8.3/ocpp/v20/schemas/Get15118EVCertificateRequest_v1p0.json
--rw-r--r--   0        0        0     1465 2020-03-21 08:32:49.130586 ocpp-0.8.3/ocpp/v20/schemas/Get15118EVCertificateResponse_v1p0.json
--rw-r--r--   0        0        0      492 2020-03-21 08:32:49.130586 ocpp-0.8.3/ocpp/v20/schemas/GetBaseReportRequest_v1p0.json
--rw-r--r--   0        0        0      390 2020-03-21 08:32:49.130586 ocpp-0.8.3/ocpp/v20/schemas/GetBaseReportResponse_v1p0.json
--rw-r--r--   0        0        0     1300 2020-03-21 08:32:49.134586 ocpp-0.8.3/ocpp/v20/schemas/GetCertificateStatusRequest_v1p0.json
--rw-r--r--   0        0        0      444 2020-03-21 08:32:49.134586 ocpp-0.8.3/ocpp/v20/schemas/GetCertificateStatusResponse_v1p0.json
--rw-r--r--   0        0        0     1744 2020-03-21 08:32:49.134586 ocpp-0.8.3/ocpp/v20/schemas/GetChargingProfilesRequest_v1p0.json
--rw-r--r--   0        0        0      367 2020-03-21 08:32:49.134586 ocpp-0.8.3/ocpp/v20/schemas/GetChargingProfilesResponse_v1p0.json
--rw-r--r--   0        0        0      480 2020-03-21 08:32:49.134586 ocpp-0.8.3/ocpp/v20/schemas/GetCompositeScheduleRequest_v1p0.json
--rw-r--r--   0        0        0     2510 2020-03-21 08:32:49.138587 ocpp-0.8.3/ocpp/v20/schemas/GetCompositeScheduleResponse_v1p0.json
--rw-r--r--   0        0        0      796 2020-03-21 08:32:49.138587 ocpp-0.8.3/ocpp/v20/schemas/GetDisplayMessagesRequest_v1p0.json
--rw-r--r--   0        0        0      364 2020-03-21 08:32:49.138587 ocpp-0.8.3/ocpp/v20/schemas/GetDisplayMessagesResponse_v1p0.json
--rw-r--r--   0        0        0      521 2020-03-21 08:32:49.138587 ocpp-0.8.3/ocpp/v20/schemas/GetInstalledCertificateIdsRequest_v1p0.json
--rw-r--r--   0        0        0     1598 2020-03-21 08:32:49.138587 ocpp-0.8.3/ocpp/v20/schemas/GetInstalledCertificateIdsResponse_v1p0.json
--rw-r--r--   0        0        0      150 2020-03-21 08:32:49.138587 ocpp-0.8.3/ocpp/v20/schemas/GetLocalListVersionRequest_v1p0.json
--rw-r--r--   0        0        0      275 2020-03-21 08:32:49.142587 ocpp-0.8.3/ocpp/v20/schemas/GetLocalListVersionResponse_v1p0.json
--rw-r--r--   0        0        0     1264 2020-03-21 08:32:49.142587 ocpp-0.8.3/ocpp/v20/schemas/GetLogRequest_v1p0.json
--rw-r--r--   0        0        0      470 2020-03-21 08:32:49.142587 ocpp-0.8.3/ocpp/v20/schemas/GetLogResponse_v1p0.json
--rw-r--r--   0        0        0     2467 2020-03-21 08:32:49.142587 ocpp-0.8.3/ocpp/v20/schemas/GetMonitoringReportRequest_v1p0.json
--rw-r--r--   0        0        0      390 2020-03-21 08:32:49.142587 ocpp-0.8.3/ocpp/v20/schemas/GetMonitoringReportResponse_v1p0.json
--rw-r--r--   0        0        0     2454 2020-03-21 08:32:49.146587 ocpp-0.8.3/ocpp/v20/schemas/GetReportRequest_v1p0.json
--rw-r--r--   0        0        0      390 2020-03-21 08:32:49.146587 ocpp-0.8.3/ocpp/v20/schemas/GetReportResponse_v1p0.json
--rw-r--r--   0        0        0      254 2020-03-21 08:32:49.146587 ocpp-0.8.3/ocpp/v20/schemas/GetTransactionStatusRequest_v1p0.json
--rw-r--r--   0        0        0      339 2020-03-21 08:32:49.146587 ocpp-0.8.3/ocpp/v20/schemas/GetTransactionStatusResponse_v1p0.json
--rw-r--r--   0        0        0     2322 2020-03-21 08:32:49.146587 ocpp-0.8.3/ocpp/v20/schemas/GetVariablesRequest_v1p0.json
--rw-r--r--   0        0        0     2830 2020-03-21 08:32:49.146587 ocpp-0.8.3/ocpp/v20/schemas/GetVariablesResponse_v1p0.json
--rw-r--r--   0        0        0      150 2020-03-21 08:32:49.146587 ocpp-0.8.3/ocpp/v20/schemas/HeartbeatRequest_v1p0.json
--rw-r--r--   0        0        0      300 2020-03-21 08:32:49.150587 ocpp-0.8.3/ocpp/v20/schemas/HeartbeatResponse_v1p0.json
--rw-r--r--   0        0        0      616 2020-03-21 08:32:49.150587 ocpp-0.8.3/ocpp/v20/schemas/InstallCertificateRequest_v1p0.json
--rw-r--r--   0        0        0      525 2020-03-21 08:32:49.150587 ocpp-0.8.3/ocpp/v20/schemas/InstallCertificateResponse_v1p0.json
--rw-r--r--   0        0        0      566 2020-03-21 08:32:49.150587 ocpp-0.8.3/ocpp/v20/schemas/LogStatusNotificationRequest_v1p0.json
--rw-r--r--   0        0        0      150 2020-03-21 08:32:49.150587 ocpp-0.8.3/ocpp/v20/schemas/LogStatusNotificationResponse_v1p0.json
--rw-r--r--   0        0        0     5109 2020-03-21 08:32:49.150587 ocpp-0.8.3/ocpp/v20/schemas/MeterValuesRequest_v1p0.json
--rw-r--r--   0        0        0      150 2020-03-21 08:32:49.154587 ocpp-0.8.3/ocpp/v20/schemas/MeterValuesResponse_v1p0.json
--rw-r--r--   0        0        0     4477 2020-03-21 08:32:49.154587 ocpp-0.8.3/ocpp/v20/schemas/NotifyCentralChargingNeedsRequest_v1p0.json
--rw-r--r--   0        0        0      365 2020-03-21 08:32:49.154587 ocpp-0.8.3/ocpp/v20/schemas/NotifyCentralChargingNeedsResponse_v1p0.json
--rw-r--r--   0        0        0     2690 2020-03-21 08:32:49.154587 ocpp-0.8.3/ocpp/v20/schemas/NotifyChargingLimitRequest_v1p0.json
--rw-r--r--   0        0        0      150 2020-03-21 08:32:49.154587 ocpp-0.8.3/ocpp/v20/schemas/NotifyChargingLimitResponse_v1p0.json
--rw-r--r--   0        0        0      560 2020-03-21 08:32:49.154587 ocpp-0.8.3/ocpp/v20/schemas/NotifyCustomerInformationRequest_v1p0.json
--rw-r--r--   0        0        0      150 2020-03-21 08:32:49.154587 ocpp-0.8.3/ocpp/v20/schemas/NotifyCustomerInformationResponse_v1p0.json
--rw-r--r--   0        0        0     3393 2020-03-21 08:32:49.154587 ocpp-0.8.3/ocpp/v20/schemas/NotifyDisplayMessagesRequest_v1p0.json
--rw-r--r--   0        0        0      150 2020-03-21 08:32:49.154587 ocpp-0.8.3/ocpp/v20/schemas/NotifyDisplayMessagesResponse_v1p0.json
--rw-r--r--   0        0        0     2943 2020-03-21 08:32:49.158587 ocpp-0.8.3/ocpp/v20/schemas/NotifyEVChargingNeedsRequest_v1p0.json
--rw-r--r--   0        0        0      388 2020-03-21 08:32:49.158587 ocpp-0.8.3/ocpp/v20/schemas/NotifyEVChargingNeedsResponse_v1p0.json
--rw-r--r--   0        0        0     1978 2020-03-21 08:32:49.158587 ocpp-0.8.3/ocpp/v20/schemas/NotifyEVChargingScheduleRequest_v1p0.json
--rw-r--r--   0        0        0      365 2020-03-21 08:32:49.158587 ocpp-0.8.3/ocpp/v20/schemas/NotifyEVChargingScheduleResponse_v1p0.json
--rw-r--r--   0        0        0     4157 2020-03-21 08:32:49.162587 ocpp-0.8.3/ocpp/v20/schemas/NotifyEventRequest_v1p0.json
--rw-r--r--   0        0        0      150 2020-03-21 08:32:49.162587 ocpp-0.8.3/ocpp/v20/schemas/NotifyEventResponse_v1p0.json
--rw-r--r--   0        0        0     3429 2020-03-21 08:32:49.162587 ocpp-0.8.3/ocpp/v20/schemas/NotifyMonitoringReportRequest_v1p0.json
--rw-r--r--   0        0        0      150 2020-03-21 08:32:49.162587 ocpp-0.8.3/ocpp/v20/schemas/NotifyMonitoringReportResponse_v1p0.json
--rw-r--r--   0        0        0     4752 2020-03-21 08:32:49.162587 ocpp-0.8.3/ocpp/v20/schemas/NotifyReportRequest_v1p0.json
--rw-r--r--   0        0        0      150 2020-03-21 08:32:49.162587 ocpp-0.8.3/ocpp/v20/schemas/NotifyReportResponse_v1p0.json
--rw-r--r--   0        0        0      432 2020-03-21 08:32:49.162587 ocpp-0.8.3/ocpp/v20/schemas/PublishFirmwareRequest_v1p0.json
--rw-r--r--   0        0        0      365 2020-03-21 08:32:49.162587 ocpp-0.8.3/ocpp/v20/schemas/PublishFirmwareResponse_v1p0.json
--rw-r--r--   0        0        0      637 2020-03-21 08:32:49.166587 ocpp-0.8.3/ocpp/v20/schemas/PublishFirmwareStatusNotificationRequest_v1p0.json
--rw-r--r--   0        0        0      150 2020-03-21 08:32:49.166587 ocpp-0.8.3/ocpp/v20/schemas/PublishFirmwareStatusNotificationResponse_v1p0.json
--rw-r--r--   0        0        0      614 2020-03-21 08:32:49.166587 ocpp-0.8.3/ocpp/v20/schemas/Renegotiate15118ScheduleRequest_v1p0.json
--rw-r--r--   0        0        0      365 2020-03-21 08:32:49.166587 ocpp-0.8.3/ocpp/v20/schemas/Renegotiate15118ScheduleResponse_v1p0.json
--rw-r--r--   0        0        0     4309 2020-03-21 08:32:49.166587 ocpp-0.8.3/ocpp/v20/schemas/ReportChargingProfilesRequest_v1p0.json
--rw-r--r--   0        0        0      150 2020-03-21 08:32:49.166587 ocpp-0.8.3/ocpp/v20/schemas/ReportChargingProfilesResponse_v1p0.json
--rw-r--r--   0        0        0     5216 2020-03-21 08:32:49.166587 ocpp-0.8.3/ocpp/v20/schemas/RequestStartTransactionRequest_v1p0.json
--rw-r--r--   0        0        0      445 2020-03-21 08:32:49.166587 ocpp-0.8.3/ocpp/v20/schemas/RequestStartTransactionResponse_v1p0.json
--rw-r--r--   0        0        0      298 2020-03-21 08:32:49.170587 ocpp-0.8.3/ocpp/v20/schemas/RequestStopTransactionRequest_v1p0.json
--rw-r--r--   0        0        0      365 2020-03-21 08:32:49.170587 ocpp-0.8.3/ocpp/v20/schemas/RequestStopTransactionResponse_v1p0.json
--rw-r--r--   0        0        0      476 2020-03-21 08:32:49.170587 ocpp-0.8.3/ocpp/v20/schemas/ReservationStatusUpdateRequest_v1p0.json
--rw-r--r--   0        0        0      150 2020-03-21 08:32:49.170587 ocpp-0.8.3/ocpp/v20/schemas/ReservationStatusUpdateResponse_v1p0.json
--rw-r--r--   0        0        0     3277 2020-03-21 08:32:49.170587 ocpp-0.8.3/ocpp/v20/schemas/ReserveNowRequest_v1p0.json
--rw-r--r--   0        0        0      430 2020-03-21 08:32:49.170587 ocpp-0.8.3/ocpp/v20/schemas/ReserveNowResponse_v1p0.json
--rw-r--r--   0        0        0      360 2020-03-21 08:32:49.170587 ocpp-0.8.3/ocpp/v20/schemas/ResetRequest_v1p0.json
--rw-r--r--   0        0        0      387 2020-03-21 08:32:49.174587 ocpp-0.8.3/ocpp/v20/schemas/ResetResponse_v1p0.json
--rw-r--r--   0        0        0     1049 2020-03-21 08:32:49.174587 ocpp-0.8.3/ocpp/v20/schemas/SecurityEventNotificationRequest_v1p0.json
--rw-r--r--   0        0        0      150 2020-03-21 08:32:49.174587 ocpp-0.8.3/ocpp/v20/schemas/SecurityEventNotificationResponse_v1p0.json
--rw-r--r--   0        0        0     4782 2020-03-21 08:32:49.174587 ocpp-0.8.3/ocpp/v20/schemas/SendLocalListRequest_v1p0.json
--rw-r--r--   0        0        0      391 2020-03-21 08:32:49.174587 ocpp-0.8.3/ocpp/v20/schemas/SendLocalListResponse_v1p0.json
--rw-r--r--   0        0        0     3778 2020-03-21 08:32:49.174587 ocpp-0.8.3/ocpp/v20/schemas/SetChargingProfileRequest_v1p0.json
--rw-r--r--   0        0        0      365 2020-03-21 08:32:49.174587 ocpp-0.8.3/ocpp/v20/schemas/SetChargingProfileResponse_v1p0.json
--rw-r--r--   0        0        0     3147 2020-03-21 08:32:49.178587 ocpp-0.8.3/ocpp/v20/schemas/SetDisplayMessageRequest_v1p0.json
--rw-r--r--   0        0        0      497 2020-03-21 08:32:49.178587 ocpp-0.8.3/ocpp/v20/schemas/SetDisplayMessageResponse_v1p0.json
--rw-r--r--   0        0        0      399 2020-03-21 08:32:49.178587 ocpp-0.8.3/ocpp/v20/schemas/SetMonitoringBaseRequest_v1p0.json
--rw-r--r--   0        0        0      390 2020-03-21 08:32:49.178587 ocpp-0.8.3/ocpp/v20/schemas/SetMonitoringBaseResponse_v1p0.json
--rw-r--r--   0        0        0      269 2020-03-21 08:32:49.182587 ocpp-0.8.3/ocpp/v20/schemas/SetMonitoringLevelRequest_v1p0.json
--rw-r--r--   0        0        0      369 2020-03-21 08:32:49.182587 ocpp-0.8.3/ocpp/v20/schemas/SetMonitoringLevelResponse_v1p0.json
--rw-r--r--   0        0        0     4030 2020-03-21 08:32:49.182587 ocpp-0.8.3/ocpp/v20/schemas/SetNetworkProfileRequest_v1p0.json
--rw-r--r--   0        0        0      384 2020-03-21 08:32:49.182587 ocpp-0.8.3/ocpp/v20/schemas/SetNetworkProfileResponse_v1p0.json
--rw-r--r--   0        0        0     2646 2020-03-21 08:32:49.182587 ocpp-0.8.3/ocpp/v20/schemas/SetVariableMonitoringRequest_v1p0.json
--rw-r--r--   0        0        0     2938 2020-03-21 08:32:49.182587 ocpp-0.8.3/ocpp/v20/schemas/SetVariableMonitoringResponse_v1p0.json
--rw-r--r--   0        0        0     2448 2020-03-21 08:32:49.186587 ocpp-0.8.3/ocpp/v20/schemas/SetVariablesRequest_v1p0.json
--rw-r--r--   0        0        0     2806 2020-03-21 08:32:49.186587 ocpp-0.8.3/ocpp/v20/schemas/SetVariablesResponse_v1p0.json
--rw-r--r--   0        0        0      468 2020-03-21 08:32:49.186587 ocpp-0.8.3/ocpp/v20/schemas/SignCertificateRequest_v1p0.json
--rw-r--r--   0        0        0      365 2020-03-21 08:32:49.186587 ocpp-0.8.3/ocpp/v20/schemas/SignCertificateResponse_v1p0.json
--rw-r--r--   0        0        0      689 2020-03-21 08:32:49.186587 ocpp-0.8.3/ocpp/v20/schemas/StatusNotificationRequest_v1p0.json
--rw-r--r--   0        0        0      150 2020-03-21 08:32:49.186587 ocpp-0.8.3/ocpp/v20/schemas/StatusNotificationResponse_v1p0.json
--rw-r--r--   0        0        0     9743 2020-03-21 08:32:49.186587 ocpp-0.8.3/ocpp/v20/schemas/TransactionEventRequest_v1p0.json
--rw-r--r--   0        0        0     3072 2020-03-21 08:32:49.190588 ocpp-0.8.3/ocpp/v20/schemas/TransactionEventResponse_v1p0.json
--rw-r--r--   0        0        0     1125 2020-03-21 08:32:49.190588 ocpp-0.8.3/ocpp/v20/schemas/TriggerMessageRequest_v1p0.json
--rw-r--r--   0        0        0      392 2020-03-21 08:32:49.190588 ocpp-0.8.3/ocpp/v20/schemas/TriggerMessageResponse_v1p0.json
--rw-r--r--   0        0        0      336 2020-03-21 08:32:49.190588 ocpp-0.8.3/ocpp/v20/schemas/UnlockConnectorRequest_v1p0.json
--rw-r--r--   0        0        0      369 2020-03-21 08:32:49.190588 ocpp-0.8.3/ocpp/v20/schemas/UnlockConnectorResponse_v1p0.json
--rw-r--r--   0        0        0      290 2020-03-21 08:32:49.194588 ocpp-0.8.3/ocpp/v20/schemas/UnpublishFirmwareRequest_v1p0.json
--rw-r--r--   0        0        0      398 2020-03-21 08:32:49.194588 ocpp-0.8.3/ocpp/v20/schemas/UnpublishFirmwareResponse_v1p0.json
--rw-r--r--   0        0        0      406 2020-03-21 08:32:49.194588 ocpp-0.8.3/ocpp/v20/schemas/Update15118EVCertificateRequest_v1p0.json
--rw-r--r--   0        0        0      443 2020-03-21 08:32:49.194588 ocpp-0.8.3/ocpp/v20/schemas/Update15118EVCertificateResponse_v1p0.json
--rw-r--r--   0        0        0     1219 2020-03-21 08:32:49.194588 ocpp-0.8.3/ocpp/v20/schemas/UpdateFirmwareRequest_v1p0.json
--rw-r--r--   0        0        0      394 2020-03-21 08:32:49.194588 ocpp-0.8.3/ocpp/v20/schemas/UpdateFirmwareResponse_v1p0.json
--rw-r--r--   0        0        0      189 2020-10-19 10:51:56.798577 ocpp-0.8.3/ocpp/v201/__init__.py
--rw-r--r--   0        0        0     7665 2021-02-26 14:56:21.693852 ocpp-0.8.3/ocpp/v201/call.py
--rw-r--r--   0        0        0     6013 2020-10-19 10:51:56.798577 ocpp-0.8.3/ocpp/v201/call_result.py
--rw-r--r--   0        0        0    32670 2021-04-21 07:33:07.081840 ocpp-0.8.3/ocpp/v201/enums.py
--rwxr-xr-x   0        0        0     4203 2020-10-19 10:51:56.798577 ocpp-0.8.3/ocpp/v201/schemas/AuthorizeRequest.json
--rwxr-xr-x   0        0        0     7208 2020-10-19 10:51:56.798577 ocpp-0.8.3/ocpp/v201/schemas/AuthorizeResponse.json
--rwxr-xr-x   0        0        0     3161 2020-10-19 10:51:56.798577 ocpp-0.8.3/ocpp/v201/schemas/BootNotificationRequest.json
--rwxr-xr-x   0        0        0     2270 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/BootNotificationResponse.json
--rwxr-xr-x   0        0        0      775 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/CancelReservationRequest.json
--rwxr-xr-x   0        0        0     1758 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/CancelReservationResponse.json
--rwxr-xr-x   0        0        0     1914 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/CertificateSignedRequest.json
--rwxr-xr-x   0        0        0     1752 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/CertificateSignedResponse.json
--rwxr-xr-x   0        0        0     1811 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/ChangeAvailabilityRequest.json
--rwxr-xr-x   0        0        0     1783 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/ChangeAvailabilityResponse.json
--rwxr-xr-x   0        0        0      634 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/ClearCacheRequest.json
--rwxr-xr-x   0        0        0     1735 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/ClearCacheResponse.json
--rwxr-xr-x   0        0        0     2574 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/ClearChargingProfileRequest.json
--rwxr-xr-x   0        0        0     1752 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/ClearChargingProfileResponse.json
--rwxr-xr-x   0        0        0      787 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/ClearDisplayMessageRequest.json
--rwxr-xr-x   0        0        0     1735 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/ClearDisplayMessageResponse.json
--rwxr-xr-x   0        0        0      865 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/ClearVariableMonitoringRequest.json
--rwxr-xr-x   0        0        0     2327 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/ClearVariableMonitoringResponse.json
--rwxr-xr-x   0        0        0     1087 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/ClearedChargingLimitRequest.json
--rwxr-xr-x   0        0        0      634 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/ClearedChargingLimitResponse.json
--rwxr-xr-x   0        0        0     1121 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/CostUpdatedRequest.json
--rwxr-xr-x   0        0        0      634 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/CostUpdatedResponse.json
--rwxr-xr-x   0        0        0     4659 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/CustomerInformationRequest.json
--rwxr-xr-x   0        0        0     1740 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/CustomerInformationResponse.json
--rwxr-xr-x   0        0        0     1101 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/DataTransferRequest.json
--rwxr-xr-x   0        0        0     1869 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/DataTransferResponse.json
--rwxr-xr-x   0        0        0     1808 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/DeleteCertificateRequest.json
--rwxr-xr-x   0        0        0     1747 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/DeleteCertificateResponse.json
--rwxr-xr-x   0        0        0     1539 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/FirmwareStatusNotificationRequest.json
--rwxr-xr-x   0        0        0      634 2020-10-19 10:51:56.799577 ocpp-0.8.3/ocpp/v201/schemas/FirmwareStatusNotificationResponse.json
--rwxr-xr-x   0        0        0     1424 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/Get15118EVCertificateRequest.json
--rwxr-xr-x   0        0        0     1914 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/Get15118EVCertificateResponse.json
--rwxr-xr-x   0        0        0     1105 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/GetBaseReportRequest.json
--rwxr-xr-x   0        0        0     1794 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/GetBaseReportResponse.json
--rwxr-xr-x   0        0        0     1957 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/GetCertificateStatusRequest.json
--rwxr-xr-x   0        0        0     2089 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/GetCertificateStatusResponse.json
--rwxr-xr-x   0        0        0     3622 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/GetChargingProfilesRequest.json
--rwxr-xr-x   0        0        0     1859 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/GetChargingProfilesResponse.json
--rwxr-xr-x   0        0        0     1329 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/GetCompositeScheduleRequest.json
--rwxr-xr-x   0        0        0     5095 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/GetCompositeScheduleResponse.json
--rwxr-xr-x   0        0        0     1874 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/GetDisplayMessagesRequest.json
--rwxr-xr-x   0        0        0     1841 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/GetDisplayMessagesResponse.json
--rwxr-xr-x   0        0        0     1204 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/GetInstalledCertificateIdsRequest.json
--rwxr-xr-x   0        0        0     3997 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/GetInstalledCertificateIdsResponse.json
--rwxr-xr-x   0        0        0      634 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/GetLocalListVersionRequest.json
--rwxr-xr-x   0        0        0      840 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/GetLocalListVersionResponse.json
--rwxr-xr-x   0        0        0     2802 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/GetLogRequest.json
--rwxr-xr-x   0        0        0     1954 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/GetLogResponse.json
--rwxr-xr-x   0        0        0     4175 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/GetMonitoringReportRequest.json
--rwxr-xr-x   0        0        0     1800 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/GetMonitoringReportResponse.json
--rwxr-xr-x   0        0        0     4143 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/GetReportRequest.json
--rwxr-xr-x   0        0        0     1800 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/GetReportResponse.json
--rwxr-xr-x   0        0        0      784 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/GetTransactionStatusRequest.json
--rwxr-xr-x   0        0        0      910 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/GetTransactionStatusResponse.json
--rwxr-xr-x   0        0        0     3931 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/GetVariablesRequest.json
--rwxr-xr-x   0        0        0     5581 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/GetVariablesResponse.json
--rwxr-xr-x   0        0        0      634 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/HeartbeatRequest.json
--rwxr-xr-x   0        0        0      802 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/HeartbeatResponse.json
--rwxr-xr-x   0        0        0     1226 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/InstallCertificateRequest.json
--rwxr-xr-x   0        0        0     1751 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/InstallCertificateResponse.json
--rwxr-xr-x   0        0        0     1361 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/LogStatusNotificationRequest.json
--rwxr-xr-x   0        0        0      634 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/LogStatusNotificationResponse.json
--rwxr-xr-x   0        0        0     7709 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/MeterValuesRequest.json
--rwxr-xr-x   0        0        0      634 2020-10-19 10:51:56.800577 ocpp-0.8.3/ocpp/v201/schemas/MeterValuesResponse.json
--rwxr-xr-x   0        0        0    11333 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/NotifyChargingLimitRequest.json
--rwxr-xr-x   0        0        0      634 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/NotifyChargingLimitResponse.json
--rwxr-xr-x   0        0        0     1542 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/NotifyCustomerInformationRequest.json
--rwxr-xr-x   0        0        0      634 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/NotifyCustomerInformationResponse.json
--rwxr-xr-x   0        0        0     6512 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/NotifyDisplayMessagesRequest.json
--rwxr-xr-x   0        0        0      634 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/NotifyDisplayMessagesResponse.json
--rwxr-xr-x   0        0        0     5943 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/NotifyEVChargingNeedsRequest.json
--rwxr-xr-x   0        0        0     1870 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/NotifyEVChargingNeedsResponse.json
--rwxr-xr-x   0        0        0    10370 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/NotifyEVChargingScheduleRequest.json
--rwxr-xr-x   0        0        0     1780 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/NotifyEVChargingScheduleResponse.json
--rwxr-xr-x   0        0        0     6614 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/NotifyEventRequest.json
--rwxr-xr-x   0        0        0      634 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/NotifyEventResponse.json
--rwxr-xr-x   0        0        0     7005 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/NotifyMonitoringReportRequest.json
--rwxr-xr-x   0        0        0      634 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/NotifyMonitoringReportResponse.json
--rwxr-xr-x   0        0        0     8608 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/NotifyReportRequest.json
--rwxr-xr-x   0        0        0      634 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/NotifyReportResponse.json
--rwxr-xr-x   0        0        0     1668 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/PublishFirmwareRequest.json
--rwxr-xr-x   0        0        0     1691 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/PublishFirmwareResponse.json
--rwxr-xr-x   0        0        0     1631 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/PublishFirmwareStatusNotificationRequest.json
--rwxr-xr-x   0        0        0      634 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/PublishFirmwareStatusNotificationResponse.json
--rwxr-xr-x   0        0        0    14700 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/ReportChargingProfilesRequest.json
--rwxr-xr-x   0        0        0      634 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/ReportChargingProfilesResponse.json
--rwxr-xr-x   0        0        0    15964 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/RequestStartTransactionRequest.json
--rwxr-xr-x   0        0        0     2080 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/RequestStartTransactionResponse.json
--rwxr-xr-x   0        0        0      844 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/RequestStopTransactionRequest.json
--rwxr-xr-x   0        0        0     1760 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/RequestStopTransactionResponse.json
--rwxr-xr-x   0        0        0     1133 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/ReservationStatusUpdateRequest.json
--rwxr-xr-x   0        0        0      634 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/ReservationStatusUpdateResponse.json
--rwxr-xr-x   0        0        0     3649 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/ReserveNowRequest.json
--rwxr-xr-x   0        0        0     1758 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/ReserveNowResponse.json
--rwxr-xr-x   0        0        0     1144 2020-10-19 10:51:56.801577 ocpp-0.8.3/ocpp/v201/schemas/ResetRequest.json
--rwxr-xr-x   0        0        0     1730 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/ResetResponse.json
--rwxr-xr-x   0        0        0     1120 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/SecurityEventNotificationRequest.json
--rwxr-xr-x   0        0        0      634 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/SecurityEventNotificationResponse.json
--rwxr-xr-x   0        0        0     7733 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/SendLocalListRequest.json
--rwxr-xr-x   0        0        0     1810 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/SendLocalListResponse.json
--rwxr-xr-x   0        0        0    13730 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/SetChargingProfileRequest.json
--rwxr-xr-x   0        0        0     1913 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/SetChargingProfileResponse.json
--rwxr-xr-x   0        0        0     5989 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/SetDisplayMessageRequest.json
--rwxr-xr-x   0        0        0     1848 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/SetDisplayMessageResponse.json
--rwxr-xr-x   0        0        0     1005 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/SetMonitoringBaseRequest.json
--rwxr-xr-x   0        0        0     1789 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/SetMonitoringBaseResponse.json
--rwxr-xr-x   0        0        0     2087 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/SetMonitoringLevelRequest.json
--rwxr-xr-x   0        0        0     1718 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/SetMonitoringLevelResponse.json
--rwxr-xr-x   0        0        0     7613 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/SetNetworkProfileRequest.json
--rwxr-xr-x   0        0        0     1710 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/SetNetworkProfileResponse.json
--rwxr-xr-x   0        0        0     5959 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/SetVariableMonitoringRequest.json
--rwxr-xr-x   0        0        0     6923 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/SetVariableMonitoringResponse.json
--rwxr-xr-x   0        0        0     4272 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/SetVariablesRequest.json
--rwxr-xr-x   0        0        0     5035 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/SetVariablesResponse.json
--rwxr-xr-x   0        0        0     1481 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/SignCertificateRequest.json
--rwxr-xr-x   0        0        0     1699 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/SignCertificateResponse.json
--rwxr-xr-x   0        0        0     1570 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/StatusNotificationRequest.json
--rwxr-xr-x   0        0        0      634 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/StatusNotificationResponse.json
--rwxr-xr-x   0        0        0    14824 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/TransactionEventRequest.json
--rwxr-xr-x   0        0        0     7606 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/TransactionEventResponse.json
--rwxr-xr-x   0        0        0     1996 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/TriggerMessageRequest.json
--rwxr-xr-x   0        0        0     1772 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/TriggerMessageResponse.json
--rwxr-xr-x   0        0        0      970 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/UnlockConnectorRequest.json
--rwxr-xr-x   0        0        0     1776 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/UnlockConnectorResponse.json
--rwxr-xr-x   0        0        0      837 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/UnpublishFirmwareRequest.json
--rwxr-xr-x   0        0        0     1059 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/UnpublishFirmwareResponse.json
--rwxr-xr-x   0        0        0     2765 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/UpdateFirmwareRequest.json
--rwxr-xr-x   0        0        0     1824 2020-10-19 10:51:56.802577 ocpp-0.8.3/ocpp/v201/schemas/UpdateFirmwareResponse.json
--rw-r--r--   0        0        0     1585 2021-04-21 15:17:05.607410 ocpp-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     6302 2021-04-21 15:17:48.396688 ocpp-0.8.3/setup.py
--rw-r--r--   0        0        0     6071 2021-04-21 15:17:48.397129 ocpp-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2021-05-29 12:40:10.211365 ocpp-0.9.0/LICENSE
+-rw-r--r--   0        0        0     5803 2021-05-29 12:40:10.211365 ocpp-0.9.0/README.rst
+-rw-r--r--   0        0        0        0 2021-05-29 12:40:10.338031 ocpp-0.9.0/ocpp/__init__.py
+-rw-r--r--   0        0        0    11206 2021-06-29 19:28:41.218264 ocpp-0.9.0/ocpp/charge_point.py
+-rw-r--r--   0        0        0     3168 2021-07-23 11:26:56.054943 ocpp-0.9.0/ocpp/exceptions.py
+-rw-r--r--   0        0        0    15020 2021-09-02 10:31:37.936056 ocpp-0.9.0/ocpp/messages.py
+-rw-r--r--   0        0        0     4084 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/routing.py
+-rw-r--r--   0        0        0      186 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/__init__.py
+-rw-r--r--   0        0        0     6162 2021-09-02 10:31:37.936056 ocpp-0.9.0/ocpp/v16/call.py
+-rw-r--r--   0        0        0     4773 2021-09-02 10:31:37.936056 ocpp-0.9.0/ocpp/v16/call_result.py
+-rw-r--r--   0        0        0    21190 2021-09-02 10:31:37.939390 ocpp-0.9.0/ocpp/v16/enums.py
+-rw-r--r--   0        0        0      306 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/Authorize.json
+-rw-r--r--   0        0        0     1062 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/AuthorizeResponse.json
+-rw-r--r--   0        0        0     1139 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/BootNotification.json
+-rw-r--r--   0        0        0      655 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/BootNotificationResponse.json
+-rw-r--r--   0        0        0      302 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/CancelReservation.json
+-rw-r--r--   0        0        0      423 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/CancelReservationResponse.json
+-rw-r--r--   0        0        0      352 2021-09-02 10:31:37.939390 ocpp-0.9.0/ocpp/v16/schemas/CertificateSigned.json
+-rw-r--r--   0        0        0      505 2021-09-02 10:31:37.939390 ocpp-0.9.0/ocpp/v16/schemas/CertificateSignedResponse.json
+-rw-r--r--   0        0        0      512 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/ChangeAvailability.json
+-rw-r--r--   0        0        0      453 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/ChangeAvailabilityResponse.json
+-rw-r--r--   0        0        0      418 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/ChangeConfiguration.json
+-rw-r--r--   0        0        0      491 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/ChangeConfigurationResponse.json
+-rw-r--r--   0        0        0      174 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/ClearCache.json
+-rw-r--r--   0        0        0      416 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/ClearCacheResponse.json
+-rw-r--r--   0        0        0      637 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/ClearChargingProfile.json
+-rw-r--r--   0        0        0      425 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/ClearChargingProfileResponse.json
+-rw-r--r--   0        0        0      466 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/DataTransfer.json
+-rw-r--r--   0        0        0      547 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/DataTransferResponse.json
+-rw-r--r--   0        0        0     1156 2021-09-02 10:31:37.939390 ocpp-0.9.0/ocpp/v16/schemas/DeleteCertificate.json
+-rw-r--r--   0        0        0      523 2021-09-02 10:31:37.939390 ocpp-0.9.0/ocpp/v16/schemas/DeleteCertificateResponse.json
+-rw-r--r--   0        0        0      491 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/DiagnosticsStatusNotification.json
+-rw-r--r--   0        0        0      194 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/DiagnosticsStatusNotificationResponse.json
+-rw-r--r--   0        0        0      760 2021-09-02 10:31:37.939390 ocpp-0.9.0/ocpp/v16/schemas/ExtendedTriggerMessage.json
+-rw-r--r--   0        0        0      530 2021-09-02 10:31:37.942723 ocpp-0.9.0/ocpp/v16/schemas/ExtendedTriggerMessageResponse.json
+-rw-r--r--   0        0        0      591 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/FirmwareStatusNotification.json
+-rw-r--r--   0        0        0      191 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/FirmwareStatusNotificationResponse.json
+-rw-r--r--   0        0        0      539 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/GetCompositeSchedule.json
+-rw-r--r--   0        0        0     2139 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/GetCompositeScheduleResponse.json
+-rw-r--r--   0        0        0      344 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/GetConfiguration.json
+-rw-r--r--   0        0        0     1066 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/GetConfigurationResponse.json
+-rw-r--r--   0        0        0      642 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/GetDiagnostics.json
+-rw-r--r--   0        0        0      275 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/GetDiagnosticsResponse.json
+-rw-r--r--   0        0        0      552 2021-09-02 10:31:37.942723 ocpp-0.9.0/ocpp/v16/schemas/GetInstalledCertificateIds.json
+-rw-r--r--   0        0        0     1566 2021-09-02 10:31:37.942723 ocpp-0.9.0/ocpp/v16/schemas/GetInstalledCertificateIdsResponse.json
+-rw-r--r--   0        0        0      183 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/GetLocalListVersion.json
+-rw-r--r--   0        0        0      301 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/GetLocalListVersionResponse.json
+-rw-r--r--   0        0        0     1184 2021-09-02 10:31:37.942723 ocpp-0.9.0/ocpp/v16/schemas/GetLog.json
+-rw-r--r--   0        0        0      566 2021-09-02 10:31:37.942723 ocpp-0.9.0/ocpp/v16/schemas/GetLogResponse.json
+-rw-r--r--   0        0        0      173 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/Heartbeat.json
+-rw-r--r--   0        0        0      325 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/HeartbeatResponse.json
+-rw-r--r--   0        0        0      639 2021-09-02 10:31:37.942723 ocpp-0.9.0/ocpp/v16/schemas/InstallCertificate.json
+-rw-r--r--   0        0        0      526 2021-09-02 10:31:37.942723 ocpp-0.9.0/ocpp/v16/schemas/InstallCertificateResponse.json
+-rw-r--r--   0        0        0      667 2021-09-02 10:31:37.942723 ocpp-0.9.0/ocpp/v16/schemas/LogStatusNotification.json
+-rw-r--r--   0        0        0      173 2021-09-02 10:31:37.946056 ocpp-0.9.0/ocpp/v16/schemas/LogStatusNotificationResponse.json
+-rw-r--r--   0        0        0     6758 2021-09-02 10:31:37.946056 ocpp-0.9.0/ocpp/v16/schemas/MeterValues.json
+-rw-r--r--   0        0        0      176 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/MeterValuesResponse.json
+-rw-r--r--   0        0        0     4383 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/RemoteStartTransaction.json
+-rw-r--r--   0        0        0      428 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/RemoteStartTransactionResponse.json
+-rw-r--r--   0        0        0      306 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/RemoteStopTransaction.json
+-rw-r--r--   0        0        0      427 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/RemoteStopTransactionResponse.json
+-rw-r--r--   0        0        0      704 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/ReserveNow.json
+-rw-r--r--   0        0        0      502 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/ReserveNowResponse.json
+-rw-r--r--   0        0        0      398 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/Reset.json
+-rw-r--r--   0        0        0      411 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/ResetResponse.json
+-rw-r--r--   0        0        0      464 2021-09-02 10:31:37.946056 ocpp-0.9.0/ocpp/v16/schemas/SecurityEventNotification.json
+-rw-r--r--   0        0        0      177 2021-09-02 10:31:37.946056 ocpp-0.9.0/ocpp/v16/schemas/SecurityEventNotificationResponse.json
+-rw-r--r--   0        0        0     2146 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/SendLocalList.json
+-rw-r--r--   0        0        0      484 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/SendLocalListResponse.json
+-rw-r--r--   0        0        0     4310 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/SetChargingProfile.json
+-rw-r--r--   0        0        0      456 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/SetChargingProfileResponse.json
+-rw-r--r--   0        0        0      287 2021-09-02 10:31:37.946056 ocpp-0.9.0/ocpp/v16/schemas/SignCertificate.json
+-rw-r--r--   0        0        0      483 2021-09-02 10:31:37.946056 ocpp-0.9.0/ocpp/v16/schemas/SignCertificateResponse.json
+-rw-r--r--   0        0        0      876 2021-09-02 10:31:37.946056 ocpp-0.9.0/ocpp/v16/schemas/SignedFirmwareStatusNotification.json
+-rw-r--r--   0        0        0      184 2021-09-02 10:31:37.946056 ocpp-0.9.0/ocpp/v16/schemas/SignedFirmwareStatusNotificationResponse.json
+-rw-r--r--   0        0        0     1212 2021-09-02 10:31:37.946056 ocpp-0.9.0/ocpp/v16/schemas/SignedUpdateFirmware.json
+-rw-r--r--   0        0        0      590 2021-09-02 10:31:37.946056 ocpp-0.9.0/ocpp/v16/schemas/SignedUpdateFirmwareResponse.json
+-rw-r--r--   0        0        0      676 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/StartTransaction.json
+-rw-r--r--   0        0        0     1162 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/StartTransactionResponse.json
+-rw-r--r--   0        0        0     1805 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/StatusNotification.json
+-rw-r--r--   0        0        0      183 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/StatusNotificationResponse.json
+-rw-r--r--   0        0        0     7313 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/StopTransaction.json
+-rw-r--r--   0        0        0     1023 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/StopTransactionResponse.json
+-rw-r--r--   0        0        0      678 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/TriggerMessage.json
+-rw-r--r--   0        0        0      454 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/TriggerMessageResponse.json
+-rw-r--r--   0        0        0      296 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/UnlockConnector.json
+-rw-r--r--   0        0        0      457 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/UnlockConnectorResponse.json
+-rw-r--r--   0        0        0      572 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/UpdateFirmware.json
+-rw-r--r--   0        0        0      179 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v16/schemas/UpdateFirmwareResponse.json
+-rw-r--r--   0        0        0      186 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/__init__.py
+-rw-r--r--   0        0        0     7491 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/call.py
+-rw-r--r--   0        0        0     4907 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/call_result.py
+-rw-r--r--   0        0        0     2971 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/AuthorizeRequest_v1p0.json
+-rw-r--r--   0        0        0     3495 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/AuthorizeResponse_v1p0.json
+-rw-r--r--   0        0        0     1771 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/BootNotificationRequest_v1p0.json
+-rw-r--r--   0        0        0      560 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/BootNotificationResponse_v1p0.json
+-rw-r--r--   0        0        0      275 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/CancelReservationRequest_v1p0.json
+-rw-r--r--   0        0        0      365 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/CancelReservationResponse_v1p0.json
+-rw-r--r--   0        0        0      580 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/CertificateSignedRequest_v1p0.json
+-rw-r--r--   0        0        0      365 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/CertificateSignedResponse_v1p0.json
+-rw-r--r--   0        0        0      456 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ChangeAvailabilityRequest_v1p0.json
+-rw-r--r--   0        0        0      387 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ChangeAvailabilityResponse_v1p0.json
+-rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ClearCacheRequest_v1p0.json
+-rw-r--r--   0        0        0      365 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ClearCacheResponse_v1p0.json
+-rw-r--r--   0        0        0     1029 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ClearChargingProfileRequest_v1p0.json
+-rw-r--r--   0        0        0      364 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ClearChargingProfileResponse_v1p0.json
+-rw-r--r--   0        0        0      253 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ClearDisplayMessageRequest_v1p0.json
+-rw-r--r--   0        0        0      364 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ClearDisplayMessageResponse_v1p0.json
+-rw-r--r--   0        0        0      361 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ClearVariableMonitoringRequest_v1p0.json
+-rw-r--r--   0        0        0     1055 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ClearVariableMonitoringResponse_v1p0.json
+-rw-r--r--   0        0        0      464 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ClearedChargingLimitRequest_v1p0.json
+-rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ClearedChargingLimitResponse_v1p0.json
+-rw-r--r--   0        0        0      368 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/CostUpdatedRequest_v1p0.json
+-rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/CostUpdatedResponse_v1p0.json
+-rw-r--r--   0        0        0     2862 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/CustomerInformationRequest_v1p0.json
+-rw-r--r--   0        0        0      385 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/CustomerInformationResponse_v1p0.json
+-rw-r--r--   0        0        0      382 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/DataTransferRequest_v1p0.json
+-rw-r--r--   0        0        0      439 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/DataTransferResponse_v1p0.json
+-rw-r--r--   0        0        0     1224 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/DeleteCertificateRequest_v1p0.json
+-rw-r--r--   0        0        0      384 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/DeleteCertificateResponse_v1p0.json
+-rw-r--r--   0        0        0      893 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/FirmwareStatusNotificationRequest_v1p0.json
+-rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/FirmwareStatusNotificationResponse_v1p0.json
+-rw-r--r--   0        0        0      406 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/Get15118EVCertificateRequest_v1p0.json
+-rw-r--r--   0        0        0     1465 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/Get15118EVCertificateResponse_v1p0.json
+-rw-r--r--   0        0        0      492 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetBaseReportRequest_v1p0.json
+-rw-r--r--   0        0        0      390 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetBaseReportResponse_v1p0.json
+-rw-r--r--   0        0        0     1300 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetCertificateStatusRequest_v1p0.json
+-rw-r--r--   0        0        0      444 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetCertificateStatusResponse_v1p0.json
+-rw-r--r--   0        0        0     1744 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetChargingProfilesRequest_v1p0.json
+-rw-r--r--   0        0        0      367 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetChargingProfilesResponse_v1p0.json
+-rw-r--r--   0        0        0      480 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetCompositeScheduleRequest_v1p0.json
+-rw-r--r--   0        0        0     2510 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetCompositeScheduleResponse_v1p0.json
+-rw-r--r--   0        0        0      796 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetDisplayMessagesRequest_v1p0.json
+-rw-r--r--   0        0        0      364 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetDisplayMessagesResponse_v1p0.json
+-rw-r--r--   0        0        0      521 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetInstalledCertificateIdsRequest_v1p0.json
+-rw-r--r--   0        0        0     1598 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetInstalledCertificateIdsResponse_v1p0.json
+-rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetLocalListVersionRequest_v1p0.json
+-rw-r--r--   0        0        0      275 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetLocalListVersionResponse_v1p0.json
+-rw-r--r--   0        0        0     1264 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetLogRequest_v1p0.json
+-rw-r--r--   0        0        0      470 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetLogResponse_v1p0.json
+-rw-r--r--   0        0        0     2467 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetMonitoringReportRequest_v1p0.json
+-rw-r--r--   0        0        0      390 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetMonitoringReportResponse_v1p0.json
+-rw-r--r--   0        0        0     2454 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetReportRequest_v1p0.json
+-rw-r--r--   0        0        0      390 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetReportResponse_v1p0.json
+-rw-r--r--   0        0        0      254 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetTransactionStatusRequest_v1p0.json
+-rw-r--r--   0        0        0      339 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetTransactionStatusResponse_v1p0.json
+-rw-r--r--   0        0        0     2322 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetVariablesRequest_v1p0.json
+-rw-r--r--   0        0        0     2830 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/GetVariablesResponse_v1p0.json
+-rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/HeartbeatRequest_v1p0.json
+-rw-r--r--   0        0        0      300 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/HeartbeatResponse_v1p0.json
+-rw-r--r--   0        0        0      616 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/InstallCertificateRequest_v1p0.json
+-rw-r--r--   0        0        0      525 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/InstallCertificateResponse_v1p0.json
+-rw-r--r--   0        0        0      566 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/LogStatusNotificationRequest_v1p0.json
+-rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/LogStatusNotificationResponse_v1p0.json
+-rw-r--r--   0        0        0     5109 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/MeterValuesRequest_v1p0.json
+-rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/MeterValuesResponse_v1p0.json
+-rw-r--r--   0        0        0     4477 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyCentralChargingNeedsRequest_v1p0.json
+-rw-r--r--   0        0        0      365 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyCentralChargingNeedsResponse_v1p0.json
+-rw-r--r--   0        0        0     2690 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyChargingLimitRequest_v1p0.json
+-rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyChargingLimitResponse_v1p0.json
+-rw-r--r--   0        0        0      560 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyCustomerInformationRequest_v1p0.json
+-rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyCustomerInformationResponse_v1p0.json
+-rw-r--r--   0        0        0     3393 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyDisplayMessagesRequest_v1p0.json
+-rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyDisplayMessagesResponse_v1p0.json
+-rw-r--r--   0        0        0     2943 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyEVChargingNeedsRequest_v1p0.json
+-rw-r--r--   0        0        0      388 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyEVChargingNeedsResponse_v1p0.json
+-rw-r--r--   0        0        0     1978 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyEVChargingScheduleRequest_v1p0.json
+-rw-r--r--   0        0        0      365 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyEVChargingScheduleResponse_v1p0.json
+-rw-r--r--   0        0        0     4157 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyEventRequest_v1p0.json
+-rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyEventResponse_v1p0.json
+-rw-r--r--   0        0        0     3429 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyMonitoringReportRequest_v1p0.json
+-rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyMonitoringReportResponse_v1p0.json
+-rw-r--r--   0        0        0     4752 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyReportRequest_v1p0.json
+-rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/NotifyReportResponse_v1p0.json
+-rw-r--r--   0        0        0      432 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/PublishFirmwareRequest_v1p0.json
+-rw-r--r--   0        0        0      365 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/PublishFirmwareResponse_v1p0.json
+-rw-r--r--   0        0        0      637 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/PublishFirmwareStatusNotificationRequest_v1p0.json
+-rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/PublishFirmwareStatusNotificationResponse_v1p0.json
+-rw-r--r--   0        0        0      614 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/Renegotiate15118ScheduleRequest_v1p0.json
+-rw-r--r--   0        0        0      365 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/Renegotiate15118ScheduleResponse_v1p0.json
+-rw-r--r--   0        0        0     4309 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ReportChargingProfilesRequest_v1p0.json
+-rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ReportChargingProfilesResponse_v1p0.json
+-rw-r--r--   0        0        0     5216 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/RequestStartTransactionRequest_v1p0.json
+-rw-r--r--   0        0        0      445 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/RequestStartTransactionResponse_v1p0.json
+-rw-r--r--   0        0        0      298 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/RequestStopTransactionRequest_v1p0.json
+-rw-r--r--   0        0        0      365 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/RequestStopTransactionResponse_v1p0.json
+-rw-r--r--   0        0        0      476 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ReservationStatusUpdateRequest_v1p0.json
+-rw-r--r--   0        0        0      150 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ReservationStatusUpdateResponse_v1p0.json
+-rw-r--r--   0        0        0     3277 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ReserveNowRequest_v1p0.json
+-rw-r--r--   0        0        0      430 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ReserveNowResponse_v1p0.json
+-rw-r--r--   0        0        0      360 2021-05-29 12:40:10.341364 ocpp-0.9.0/ocpp/v20/schemas/ResetRequest_v1p0.json
+-rw-r--r--   0        0        0      387 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/ResetResponse_v1p0.json
+-rw-r--r--   0        0        0     1049 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SecurityEventNotificationRequest_v1p0.json
+-rw-r--r--   0        0        0      150 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SecurityEventNotificationResponse_v1p0.json
+-rw-r--r--   0        0        0     4782 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SendLocalListRequest_v1p0.json
+-rw-r--r--   0        0        0      391 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SendLocalListResponse_v1p0.json
+-rw-r--r--   0        0        0     3778 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetChargingProfileRequest_v1p0.json
+-rw-r--r--   0        0        0      365 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetChargingProfileResponse_v1p0.json
+-rw-r--r--   0        0        0     3147 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetDisplayMessageRequest_v1p0.json
+-rw-r--r--   0        0        0      497 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetDisplayMessageResponse_v1p0.json
+-rw-r--r--   0        0        0      399 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetMonitoringBaseRequest_v1p0.json
+-rw-r--r--   0        0        0      390 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetMonitoringBaseResponse_v1p0.json
+-rw-r--r--   0        0        0      269 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetMonitoringLevelRequest_v1p0.json
+-rw-r--r--   0        0        0      369 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetMonitoringLevelResponse_v1p0.json
+-rw-r--r--   0        0        0     4030 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetNetworkProfileRequest_v1p0.json
+-rw-r--r--   0        0        0      384 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetNetworkProfileResponse_v1p0.json
+-rw-r--r--   0        0        0     2646 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetVariableMonitoringRequest_v1p0.json
+-rw-r--r--   0        0        0     2938 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetVariableMonitoringResponse_v1p0.json
+-rw-r--r--   0        0        0     2448 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetVariablesRequest_v1p0.json
+-rw-r--r--   0        0        0     2806 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SetVariablesResponse_v1p0.json
+-rw-r--r--   0        0        0      468 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SignCertificateRequest_v1p0.json
+-rw-r--r--   0        0        0      365 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/SignCertificateResponse_v1p0.json
+-rw-r--r--   0        0        0      689 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/StatusNotificationRequest_v1p0.json
+-rw-r--r--   0        0        0      150 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/StatusNotificationResponse_v1p0.json
+-rw-r--r--   0        0        0     9743 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/TransactionEventRequest_v1p0.json
+-rw-r--r--   0        0        0     3072 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/TransactionEventResponse_v1p0.json
+-rw-r--r--   0        0        0     1125 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/TriggerMessageRequest_v1p0.json
+-rw-r--r--   0        0        0      392 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/TriggerMessageResponse_v1p0.json
+-rw-r--r--   0        0        0      336 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/UnlockConnectorRequest_v1p0.json
+-rw-r--r--   0        0        0      369 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/UnlockConnectorResponse_v1p0.json
+-rw-r--r--   0        0        0      290 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/UnpublishFirmwareRequest_v1p0.json
+-rw-r--r--   0        0        0      398 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/UnpublishFirmwareResponse_v1p0.json
+-rw-r--r--   0        0        0      406 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/Update15118EVCertificateRequest_v1p0.json
+-rw-r--r--   0        0        0      443 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/Update15118EVCertificateResponse_v1p0.json
+-rw-r--r--   0        0        0     1219 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/UpdateFirmwareRequest_v1p0.json
+-rw-r--r--   0        0        0      394 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v20/schemas/UpdateFirmwareResponse_v1p0.json
+-rw-r--r--   0        0        0      189 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/__init__.py
+-rw-r--r--   0        0        0     7665 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/call.py
+-rw-r--r--   0        0        0     6013 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/call_result.py
+-rw-r--r--   0        0        0    32670 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/enums.py
+-rwxr-xr-x   0        0        0     4203 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/AuthorizeRequest.json
+-rwxr-xr-x   0        0        0     7208 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/AuthorizeResponse.json
+-rwxr-xr-x   0        0        0     3161 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/BootNotificationRequest.json
+-rwxr-xr-x   0        0        0     2270 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/BootNotificationResponse.json
+-rwxr-xr-x   0        0        0      775 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/CancelReservationRequest.json
+-rwxr-xr-x   0        0        0     1758 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/CancelReservationResponse.json
+-rwxr-xr-x   0        0        0     1914 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/CertificateSignedRequest.json
+-rwxr-xr-x   0        0        0     1752 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/CertificateSignedResponse.json
+-rwxr-xr-x   0        0        0     1811 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ChangeAvailabilityRequest.json
+-rwxr-xr-x   0        0        0     1783 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ChangeAvailabilityResponse.json
+-rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ClearCacheRequest.json
+-rwxr-xr-x   0        0        0     1735 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ClearCacheResponse.json
+-rwxr-xr-x   0        0        0     2574 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ClearChargingProfileRequest.json
+-rwxr-xr-x   0        0        0     1752 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ClearChargingProfileResponse.json
+-rwxr-xr-x   0        0        0      787 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ClearDisplayMessageRequest.json
+-rwxr-xr-x   0        0        0     1735 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ClearDisplayMessageResponse.json
+-rwxr-xr-x   0        0        0      865 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ClearVariableMonitoringRequest.json
+-rwxr-xr-x   0        0        0     2327 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ClearVariableMonitoringResponse.json
+-rwxr-xr-x   0        0        0     1087 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ClearedChargingLimitRequest.json
+-rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ClearedChargingLimitResponse.json
+-rwxr-xr-x   0        0        0     1121 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/CostUpdatedRequest.json
+-rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/CostUpdatedResponse.json
+-rwxr-xr-x   0        0        0     4659 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/CustomerInformationRequest.json
+-rwxr-xr-x   0        0        0     1740 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/CustomerInformationResponse.json
+-rwxr-xr-x   0        0        0     1101 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/DataTransferRequest.json
+-rwxr-xr-x   0        0        0     1869 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/DataTransferResponse.json
+-rwxr-xr-x   0        0        0     1808 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/DeleteCertificateRequest.json
+-rwxr-xr-x   0        0        0     1747 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/DeleteCertificateResponse.json
+-rwxr-xr-x   0        0        0     1539 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/FirmwareStatusNotificationRequest.json
+-rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/FirmwareStatusNotificationResponse.json
+-rwxr-xr-x   0        0        0     1424 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/Get15118EVCertificateRequest.json
+-rwxr-xr-x   0        0        0     1914 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/Get15118EVCertificateResponse.json
+-rwxr-xr-x   0        0        0     1105 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetBaseReportRequest.json
+-rwxr-xr-x   0        0        0     1794 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetBaseReportResponse.json
+-rwxr-xr-x   0        0        0     1957 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetCertificateStatusRequest.json
+-rwxr-xr-x   0        0        0     2089 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetCertificateStatusResponse.json
+-rwxr-xr-x   0        0        0     3622 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetChargingProfilesRequest.json
+-rwxr-xr-x   0        0        0     1859 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetChargingProfilesResponse.json
+-rwxr-xr-x   0        0        0     1329 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetCompositeScheduleRequest.json
+-rwxr-xr-x   0        0        0     5095 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetCompositeScheduleResponse.json
+-rwxr-xr-x   0        0        0     1874 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetDisplayMessagesRequest.json
+-rwxr-xr-x   0        0        0     1841 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetDisplayMessagesResponse.json
+-rwxr-xr-x   0        0        0     1204 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetInstalledCertificateIdsRequest.json
+-rwxr-xr-x   0        0        0     3997 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetInstalledCertificateIdsResponse.json
+-rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetLocalListVersionRequest.json
+-rwxr-xr-x   0        0        0      840 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetLocalListVersionResponse.json
+-rwxr-xr-x   0        0        0     2802 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetLogRequest.json
+-rwxr-xr-x   0        0        0     1954 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetLogResponse.json
+-rwxr-xr-x   0        0        0     4175 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetMonitoringReportRequest.json
+-rwxr-xr-x   0        0        0     1800 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetMonitoringReportResponse.json
+-rwxr-xr-x   0        0        0     4143 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetReportRequest.json
+-rwxr-xr-x   0        0        0     1800 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetReportResponse.json
+-rwxr-xr-x   0        0        0      784 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetTransactionStatusRequest.json
+-rwxr-xr-x   0        0        0      910 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetTransactionStatusResponse.json
+-rwxr-xr-x   0        0        0     3931 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetVariablesRequest.json
+-rwxr-xr-x   0        0        0     5581 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/GetVariablesResponse.json
+-rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/HeartbeatRequest.json
+-rwxr-xr-x   0        0        0      802 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/HeartbeatResponse.json
+-rwxr-xr-x   0        0        0     1226 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/InstallCertificateRequest.json
+-rwxr-xr-x   0        0        0     1751 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/InstallCertificateResponse.json
+-rwxr-xr-x   0        0        0     1361 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/LogStatusNotificationRequest.json
+-rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/LogStatusNotificationResponse.json
+-rwxr-xr-x   0        0        0     7709 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/MeterValuesRequest.json
+-rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/MeterValuesResponse.json
+-rwxr-xr-x   0        0        0    11333 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyChargingLimitRequest.json
+-rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyChargingLimitResponse.json
+-rwxr-xr-x   0        0        0     1542 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyCustomerInformationRequest.json
+-rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyCustomerInformationResponse.json
+-rwxr-xr-x   0        0        0     6512 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyDisplayMessagesRequest.json
+-rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyDisplayMessagesResponse.json
+-rwxr-xr-x   0        0        0     5943 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyEVChargingNeedsRequest.json
+-rwxr-xr-x   0        0        0     1870 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyEVChargingNeedsResponse.json
+-rwxr-xr-x   0        0        0    10370 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyEVChargingScheduleRequest.json
+-rwxr-xr-x   0        0        0     1780 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyEVChargingScheduleResponse.json
+-rwxr-xr-x   0        0        0     6614 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyEventRequest.json
+-rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyEventResponse.json
+-rwxr-xr-x   0        0        0     7005 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyMonitoringReportRequest.json
+-rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyMonitoringReportResponse.json
+-rwxr-xr-x   0        0        0     8608 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyReportRequest.json
+-rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/NotifyReportResponse.json
+-rwxr-xr-x   0        0        0     1668 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/PublishFirmwareRequest.json
+-rwxr-xr-x   0        0        0     1691 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/PublishFirmwareResponse.json
+-rwxr-xr-x   0        0        0     1631 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/PublishFirmwareStatusNotificationRequest.json
+-rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/PublishFirmwareStatusNotificationResponse.json
+-rwxr-xr-x   0        0        0    14700 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ReportChargingProfilesRequest.json
+-rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ReportChargingProfilesResponse.json
+-rwxr-xr-x   0        0        0    15964 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/RequestStartTransactionRequest.json
+-rwxr-xr-x   0        0        0     2080 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/RequestStartTransactionResponse.json
+-rwxr-xr-x   0        0        0      844 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/RequestStopTransactionRequest.json
+-rwxr-xr-x   0        0        0     1760 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/RequestStopTransactionResponse.json
+-rwxr-xr-x   0        0        0     1133 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ReservationStatusUpdateRequest.json
+-rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ReservationStatusUpdateResponse.json
+-rwxr-xr-x   0        0        0     3649 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ReserveNowRequest.json
+-rwxr-xr-x   0        0        0     1758 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ReserveNowResponse.json
+-rwxr-xr-x   0        0        0     1144 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ResetRequest.json
+-rwxr-xr-x   0        0        0     1730 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/ResetResponse.json
+-rwxr-xr-x   0        0        0     1120 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/SecurityEventNotificationRequest.json
+-rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.344698 ocpp-0.9.0/ocpp/v201/schemas/SecurityEventNotificationResponse.json
+-rwxr-xr-x   0        0        0     7733 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SendLocalListRequest.json
+-rwxr-xr-x   0        0        0     1810 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SendLocalListResponse.json
+-rwxr-xr-x   0        0        0    13730 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetChargingProfileRequest.json
+-rwxr-xr-x   0        0        0     1913 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetChargingProfileResponse.json
+-rwxr-xr-x   0        0        0     5989 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetDisplayMessageRequest.json
+-rwxr-xr-x   0        0        0     1848 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetDisplayMessageResponse.json
+-rwxr-xr-x   0        0        0     1005 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetMonitoringBaseRequest.json
+-rwxr-xr-x   0        0        0     1789 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetMonitoringBaseResponse.json
+-rwxr-xr-x   0        0        0     2087 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetMonitoringLevelRequest.json
+-rwxr-xr-x   0        0        0     1718 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetMonitoringLevelResponse.json
+-rwxr-xr-x   0        0        0     7613 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetNetworkProfileRequest.json
+-rwxr-xr-x   0        0        0     1710 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetNetworkProfileResponse.json
+-rwxr-xr-x   0        0        0     5959 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetVariableMonitoringRequest.json
+-rwxr-xr-x   0        0        0     6923 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetVariableMonitoringResponse.json
+-rwxr-xr-x   0        0        0     4272 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetVariablesRequest.json
+-rwxr-xr-x   0        0        0     5035 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SetVariablesResponse.json
+-rwxr-xr-x   0        0        0     1481 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SignCertificateRequest.json
+-rwxr-xr-x   0        0        0     1699 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/SignCertificateResponse.json
+-rwxr-xr-x   0        0        0     1570 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/StatusNotificationRequest.json
+-rwxr-xr-x   0        0        0      634 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/StatusNotificationResponse.json
+-rwxr-xr-x   0        0        0    14824 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/TransactionEventRequest.json
+-rwxr-xr-x   0        0        0     7606 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/TransactionEventResponse.json
+-rwxr-xr-x   0        0        0     1996 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/TriggerMessageRequest.json
+-rwxr-xr-x   0        0        0     1772 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/TriggerMessageResponse.json
+-rwxr-xr-x   0        0        0      970 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/UnlockConnectorRequest.json
+-rwxr-xr-x   0        0        0     1776 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/UnlockConnectorResponse.json
+-rwxr-xr-x   0        0        0      837 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/UnpublishFirmwareRequest.json
+-rwxr-xr-x   0        0        0     1059 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/UnpublishFirmwareResponse.json
+-rwxr-xr-x   0        0        0     2765 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/UpdateFirmwareRequest.json
+-rwxr-xr-x   0        0        0     1824 2021-05-29 12:40:10.348031 ocpp-0.9.0/ocpp/v201/schemas/UpdateFirmwareResponse.json
+-rw-r--r--   0        0        0     1585 2021-09-02 10:41:18.516842 ocpp-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     7017 2021-09-02 10:42:47.379849 ocpp-0.9.0/setup.py
+-rw-r--r--   0        0        0     6758 2021-09-02 10:42:47.380375 ocpp-0.9.0/PKG-INFO
```

### Comparing `ocpp-0.8.3/LICENSE` & `ocpp-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/README.rst` & `ocpp-0.9.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -159,14 +159,37 @@
 
            await asyncio.gather(cp.start(), cp.send_boot_notification())
 
 
     if __name__ == '__main__':
        asyncio.run(main())
 
+Debugging
+---------
+
+Python's default log level is `logging.WARNING`. As result most of the logs
+generated by this package are discarded. To see the log output of this package
+lower the log level to `logging.DEBUG`.
+
+.. code-block:: python
+
+  import logging
+  logging.basicConfig(level=logging.DEBUG)
+
+However, this approach defines the log level for the complete logging system.
+In other words: the log level of all dependencies is set to `logging.DEBUG`.
+
+To lower the logs for this package only use the following code:
+
+.. code-block:: python
+
+  import logging
+  logging.getLogger('ocpp').setLevel(level=logging.DEBUG)
+  logging.getLogger('ocpp').addHandler(logging.StreamHandler())
+
 License
 -------
 
 Except from the documents in `docs/v16` and `docs/v201` everything is licensed under MIT_.
 © `The Mobility House`_
 
 The documents in `docs/v16` and `docs/v201` are licensed under Creative Commons
```

### Comparing `ocpp-0.8.3/ocpp/charge_point.py` & `ocpp-0.9.0/ocpp/charge_point.py`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/exceptions.py` & `ocpp-0.9.0/ocpp/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     default_description = "Payload is syntactically correct but at least \
                           one field contains an invalid value"
 
 
 class OccurenceConstraintViolationError(OCPPError):
     code = "OccurenceConstraintViolation"
     default_description = "Payload for Action is syntactically correct but \
-                          at least one of the fields violates occurence \
+                          at least one of the fields violates occurrence \
                           constraints"
 
 
 class TypeConstraintViolationError(OCPPError):
     code = "TypeConstraintViolation"
     default_description = "Payload for Action is syntactically correct but at \
                           least one of the fields violates data type \
```

### Comparing `ocpp-0.8.3/ocpp/messages.py` & `ocpp-0.9.0/ocpp/messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
         # Both the schema and the payload must be parsed using the different
         # parser for floats.
         if ocpp_version == '1.6' and (
             (type(message) == Call and
                 message.action in ['SetChargingProfile', 'RemoteStartTransaction'])  # noqa
             or
             (type(message) == CallResult and
-                message.action == ['GetCompositeSchedule'])
+                message.action == 'GetCompositeSchedule')
         ):
             validator = get_validator(
                 message.message_type_id, message.action,
                 ocpp_version, parse_float=decimal.Decimal
             )
 
             message.payload = json.loads(
```

### Comparing `ocpp-0.8.3/ocpp/routing.py` & `ocpp-0.9.0/ocpp/routing.py`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v16/call.py` & `ocpp-0.9.0/ocpp/v16/call.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,17 @@
     ChargingRateUnitType,
     DiagnosticsStatus,
     FirmwareStatus,
     MessageTrigger,
     Reason,
     ResetType,
     UpdateType,
+    CertificateUse,
+    Log,
+    UploadLogStatus,
 )
 
 # Most types of CALL messages can originate from only 1 source, either
 # from a Charge Point or Central System, but not from both.
 #
 # Take for example the CALL for an ChangeConfiguration action. This type of
 # CALL can only be send from a Central System to Charging Station, not
@@ -35,14 +38,19 @@
 
 @dataclass
 class CancelReservationPayload:
     reservation_id: int
 
 
 @dataclass
+class CertificateSignedPayload:
+    certificate_chain: str
+
+
+@dataclass
 class ChangeAvailabilityPayload:
     connector_id: int
     type: AvailabilityType
 
 
 @dataclass
 class ChangeConfigurationPayload:
@@ -60,14 +68,25 @@
     id: Optional[int] = None
     connector_id: Optional[int] = None
     charging_profile_purpose: Optional[ChargingProfilePurposeType] = None
     stack_level: Optional[int] = None
 
 
 @dataclass
+class DeleteCertificatePayload:
+    certificate_hash_data: Dict
+
+
+@dataclass
+class ExtendedTriggerMessagePayload:
+    requested_message: MessageTrigger
+    connector_id: Optional[int] = None
+
+
+@dataclass
 class GetCompositeSchedulePayload:
     connector_id: int
     duration: int
     charging_rate_unit: Optional[ChargingRateUnitType] = None
 
 
 @dataclass
@@ -81,19 +100,39 @@
     retries: Optional[int] = None
     retry_interval: Optional[int] = None
     start_time: Optional[str] = None
     stop_time: Optional[str] = None
 
 
 @dataclass
+class GetInstalledCertificateIdsPayload:
+    certificate_type: CertificateUse
+
+
+@dataclass
 class GetLocalListVersionPayload:
     pass
 
 
 @dataclass
+class GetLogPayload:
+    log: Dict
+    log_type: Log
+    request_id: int
+    retries: Optional[int] = None
+    retry_interval: Optional[int] = None
+
+
+@dataclass
+class InstallCertificatePayload:
+    certificate_type: CertificateUse
+    certificate: str
+
+
+@dataclass
 class RemoteStartTransactionPayload:
     id_tag: str
     connector_id: Optional[int] = None
     charging_profile: Optional[Dict] = None
 
 
 @dataclass
@@ -125,14 +164,22 @@
 @dataclass
 class SetChargingProfilePayload:
     connector_id: int
     cs_charging_profiles: Dict
 
 
 @dataclass
+class SignedUpdateFirmwarePayload:
+    request_id: int
+    firmware: Dict
+    retries: Optional[int] = None
+    retry_interval: Optional[int] = None
+
+
+@dataclass
 class TriggerMessagePayload:
     requested_message: MessageTrigger
     connector_id: Optional[int] = None
 
 
 @dataclass
 class UnlockConnectorPayload:
@@ -180,21 +227,45 @@
 
 @dataclass
 class HeartbeatPayload:
     pass
 
 
 @dataclass
+class LogStatusNotificationPayload:
+    status: UploadLogStatus
+    request_id: int
+
+
+@dataclass
 class MeterValuesPayload:
     connector_id: int
     meter_value: List = field(default_factory=list)
     transaction_id: Optional[int] = None
 
 
 @dataclass
+class SecurityEventNotificationPayload:
+    type: str
+    timestamp: str
+    tech_info: Optional[str]
+
+
+@dataclass
+class SignCertificatePayload:
+    csr: str
+
+
+@dataclass
+class SignedFirmwareStatusNotificationPayload:
+    status: FirmwareStatus
+    request_id: int
+
+
+@dataclass
 class StartTransactionPayload:
     connector_id: int
     id_tag: str
     meter_start: int
     timestamp: str
     reservation_id: Optional[int] = None
```

### Comparing `ocpp-0.8.3/ocpp/v16/call_result.py` & `ocpp-0.9.0/ocpp/v16/call_result.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,22 +4,30 @@
 from ocpp.v16.enums import (
     AvailabilityStatus,
     CancelReservationStatus,
     ChargingProfileStatus,
     ClearCacheStatus,
     ClearChargingProfileStatus,
     ConfigurationStatus,
+    DataTransferStatus,
     GetCompositeScheduleStatus,
     RegistrationStatus,
     RemoteStartStopStatus,
     ReservationStatus,
     ResetStatus,
     TriggerMessageStatus,
     UpdateStatus,
     UnlockStatus,
+    CertificateSignedStatus,
+    CertificateStatus,
+    DeleteCertificateStatus,
+    GenericStatus,
+    GetInstalledCertificateStatus,
+    LogStatus,
+    UpdateFirmwareStatus
 )
 
 # Most types of CALLRESULT messages can originate from only 1 source, either
 # from a Charge Point or Central System, but not from both.
 #
 # Take for example the CALLRESULT for an Authorize action. This type of
 # CALLRESULT can only be send from a Central System to Charging Station, not
@@ -60,14 +68,29 @@
 
 @dataclass
 class HeartbeatPayload:
     current_time: str
 
 
 @dataclass
+class LogStatusNotificationPayload:
+    pass
+
+
+@dataclass
+class SecurityEventNotificationPayload:
+    pass
+
+
+@dataclass
+class SignCertificatePayload:
+    status: GenericStatus
+
+
+@dataclass
 class MeterValuesPayload:
     pass
 
 
 @dataclass
 class StartTransactionPayload:
     transaction_id: int
@@ -90,14 +113,19 @@
 
 @dataclass
 class CancelReservationPayload:
     status: CancelReservationStatus
 
 
 @dataclass
+class CertificateSignedPayload:
+    status: CertificateSignedStatus
+
+
+@dataclass
 class ChangeAvailabilityPayload:
     status: AvailabilityStatus
 
 
 @dataclass
 class ChangeConfigurationPayload:
     status: ConfigurationStatus
@@ -110,14 +138,30 @@
 
 @dataclass
 class ClearChargingProfilePayload:
     status: ClearChargingProfileStatus
 
 
 @dataclass
+class DeleteCertificatePayload:
+    status: DeleteCertificateStatus
+
+
+@dataclass
+class ExtendedTriggerMessagePayload:
+    status: TriggerMessageStatus
+
+
+@dataclass
+class GetInstalledCertificateIdsPayload:
+    status: GetInstalledCertificateStatus
+    certificate_hash_data: Optional[List] = None
+
+
+@dataclass
 class GetCompositeSchedulePayload:
     status: GetCompositeScheduleStatus
     connector_id: Optional[int] = None
     schedule_start: Optional[str] = None
     charging_schedule: Optional[Dict] = None
 
 
@@ -134,14 +178,25 @@
 
 @dataclass
 class GetLocalListVersionPayload:
     list_version: int
 
 
 @dataclass
+class GetLogPayload:
+    status: LogStatus
+    filename: Optional[str] = None
+
+
+@dataclass
+class InstallCertificatePayload:
+    status: CertificateStatus
+
+
+@dataclass
 class RemoteStartTransactionPayload:
     status: RemoteStartStopStatus
 
 
 @dataclass
 class RemoteStopTransactionPayload:
     status: RemoteStartStopStatus
@@ -164,14 +219,24 @@
 
 @dataclass
 class SetChargingProfilePayload:
     status: ChargingProfileStatus
 
 
 @dataclass
+class SignedFirmwareStatusNotificationPayload:
+    pass
+
+
+@dataclass
+class SignedUpdateFirmwarePayload:
+    status: UpdateFirmwareStatus
+
+
+@dataclass
 class TriggerMessagePayload:
     status: TriggerMessageStatus
 
 
 @dataclass
 class UnlockConnectorPayload:
     status: UnlockStatus
@@ -184,9 +249,9 @@
 
 # The DataTransfer CALLRESULT can be send both from Central System as well as
 # from a Charge Point.
 
 
 @dataclass
 class DataTransferPayload:
-    status: str
+    status: DataTransferStatus
     data: Optional[str] = None
```

### Comparing `ocpp-0.8.3/ocpp/v16/enums.py` & `ocpp-0.9.0/ocpp/v16/enums.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,33 +2,44 @@
 
 
 class Action(str, Enum):
     """ An Action is a required part of a Call message. """
     Authorize = "Authorize"
     BootNotification = "BootNotification"
     CancelReservation = "CancelReservation"
+    CertificateSigned = "CertificateSigned"
     ChangeAvailability = "ChangeAvailability"
     ChangeConfiguration = "ChangeConfiguration"
     ClearCache = "ClearCache"
     ClearChargingProfile = "ClearChargingProfile"
     DataTransfer = "DataTransfer"
+    DeleteCertificate = "DeleteCertificate"
     DiagnosticsStatusNotification = "DiagnosticsStatusNotification"
+    ExtendedTriggerMessage = "ExtendedTriggerMessage"
     FirmwareStatusNotification = "FirmwareStatusNotification"
     GetCompositeSchedule = "GetCompositeSchedule"
     GetConfiguration = "GetConfiguration"
     GetDiagnostics = "GetDiagnostics"
+    GetInstalledCertificateIds = "GetInstalledCertificateIds"
     GetLocalListVersion = "GetLocalListVersion"
+    GetLog = "GetLog"
     Heartbeat = "Heartbeat"
+    InstallCertificate = "InstallCertificate"
+    LogStatusNotification = "LogStatusNotification"
     MeterValues = "MeterValues"
     RemoteStartTransaction = "RemoteStartTransaction"
     RemoteStopTransaction = "RemoteStopTransaction"
     ReserveNow = "ReserveNow"
     Reset = "Reset"
+    SecurityEventNotification = "SecurityEventNotification"
     SendLocalList = "SendLocalList"
     SetChargingProfile = "SetChargingProfile"
+    SignCertificate = "SignCertificate"
+    SignedFirmwareStatusNotification = "SignedFirmwareStatusNotification"
+    SignedUpdateFirmware = "SignedUpdateFirmware"
     StartTransaction = "StartTransaction"
     StatusNotification = "StatusNotification"
     StopTransaction = "StopTransaction"
     TriggerMessage = "TriggerMessage"
     UnlockConnector = "UnlockConnector"
     UpdateFirmware = "UpdateFirmware"
 
@@ -69,14 +80,43 @@
     Status in CancelReservation.conf.
     """
 
     accepted = "Accepted"
     rejected = "Rejected"
 
 
+class CertificateSignedStatus(str, Enum):
+    """
+    CertificateSignedStatusEnumType is used by: CertificateSigned.conf
+    """
+
+    accepted = "Accepted"
+    rejected = "Rejected"
+
+
+class CertificateStatus(str, Enum):
+    """
+    CertificateStatusEnumType is used by: InstallCertificate.conf
+    """
+
+    accepted = "Accepted"
+    rejected = "Rejected"
+    failed = "Failed"
+
+
+class CertificateUse(str, Enum):
+    """
+    CertificateUseEnumType is used by: GetInstalledCertificateIds.req,
+    InstallCertificate.req
+    """
+
+    central_system_root_certificate = "CentralSystemRootCertificate"
+    manufacturer_root_certificate = "ManufacturerRootCertificate"
+
+
 class ChargePointErrorCode(str, Enum):
     """
     Charge Point status reported in StatusNotification.req.
     """
 
     connector_lock_failure = "ConnectorLockFailure"
     ev_communication_error = "EVCommunicationError"
@@ -266,14 +306,24 @@
     unknown_vendor_id = "UnknownVendorId"
 
     # Soon to be deprecated enums
     unknownMessageId = "UnknownMessageId"
     unknownVendorId = "UnknownVendorId"
 
 
+class DeleteCertificateStatus(str, Enum):
+    """
+    DeleteCertificateStatusEnumType is used by: DeleteCertificate.conf
+    """
+
+    accepted = "Accepted"
+    failed = "Failed"
+    not_found = "NotFound"
+
+
 class DiagnosticsStatus(str, Enum):
     """
     Status in DiagnosticsStatusNotification.req.
     """
 
     idle = "Idle"
     uploaded = "Uploaded"
@@ -285,49 +335,108 @@
 
 
 class FirmwareStatus(str, Enum):
     """
     Status of a firmware download as reported in FirmwareStatusNotification.req
     """
 
+    # Common for:
+    # FirmwareStatusNotification.req and SignedFirmwareStatusNotification.req
     downloaded = "Downloaded"
     download_failed = "DownloadFailed"
     downloading = "Downloading"
     idle = "Idle"
     installation_failed = "InstallationFailed"
     installing = "Installing"
     installed = "Installed"
 
+    # Only for SignedFirmwareStatusNotification.reg
+    download_scheduled = "DownloadScheduled"
+    download_paused = "DownloadPaused"
+    install_rebooting = "InstallRebooting"
+    install_scheduled = "InstallScheduled"
+    install_verification_failed = "InstallVerificationFailed"
+    invalid_signature = "InvalidSignature"
+    signature_verified = "SignatureVerified"
+
     # Soon to be deprecated enums
     downloadFailed = "DownloadFailed"
     installationFailed = "InstallationFailed"
 
 
+class GenericStatus(str, Enum):
+    """
+    Generic message response status
+    """
+
+    accepted = "Accepted"
+    rejected = "Rejected"
+
+
 class GetCompositeScheduleStatus(str, Enum):
     """
     Status returned in response to GetCompositeSchedule.req
     """
 
     accepted = "Accepted"
     rejected = "Rejected"
 
 
+class GetInstalledCertificateStatus(str, Enum):
+    """
+    GetInstalledCertificateStatusEnumType is used by:
+    GetInstalledCertificateIds.conf
+    """
+
+    accepted = "Accepted"
+    not_found = "NotFound"
+
+
+class HashAlgorithm(str, Enum):
+    """
+    HashAlgorithmEnumType is used by: CertificateHashDataType
+    """
+
+    sha256 = "SHA256"
+    sha384 = "SHA384"
+    sha512 = "SHA512"
+
+
 class Location(str, Enum):
     """
     Allowable values of the optional "location" field of a value element in
     SampledValue.
     """
 
     inlet = "Inlet"
     outlet = "Outlet"
     body = "Body"
     cable = "Cable"
     ev = "EV"
 
 
+class Log(str, Enum):
+    """
+    LogEnumType is used by GetLog.req
+    """
+
+    diagnostics_log = "DiagnosticsLog"
+    security_log = "SecurityLog"
+
+
+class LogStatus(str, Enum):
+    """
+    LogStatusEnumType is used by: GetLog.conf
+    """
+
+    accepted = "Accepted"
+    rejected = "Rejected"
+    accepted_canceled = "AcceptedCanceled"
+
+
 class Measurand(str, Enum):
     """
     Allowable values of the optional "measurand" field of a Value element, as
     used in MeterValues.req and StopTransaction.req messages. Default value of
     "measurand" is always "Energy.Active.Import.Register"
     """
 
@@ -375,21 +484,28 @@
 
 
 class MessageTrigger(str, Enum):
     """
     Type of request to be triggered in a TriggerMessage.req
     """
 
+    # Common for TriggerMessage.req and ExtendedTriggerMessage.req
     boot_notification = "BootNotification"
-    diagnostics_status_notification = "DiagnosticsStatusNotification"
     firmware_status_notification = "FirmwareStatusNotification"
     heartbeat = "Heartbeat"
     meter_values = "MeterValues"
     status_notification = "StatusNotification"
 
+    # Only for TriggerMessage.req
+    diagnostics_status_notification = "DiagnosticsStatusNotification"
+
+    # Only for ExtendedTriggerMessage.req
+    log_status_notification = "LogStatusNotification"
+    sign_charge_point_certificate = "SignChargePointCertificate"
+
     # Soon to be deprecated enums
     bootNotification = "BootNotification"
     diagnosticsStatusNotification = "DiagnosticsStatusNotification"
     firmwareStatusNotification = "FirmwareStatusNotification"
     meterValues = "MeterValues"
     statusNotification = "StatusNotification"
 
@@ -493,14 +609,15 @@
 
 
 class RemoteStartStopStatus(str, Enum):
     """
     The result of a RemoteStartTransaction.req or RemoteStopTransaction.req
     request.
     """
+
     accepted = "Accepted"
     rejected = "Rejected"
 
 
 class ReservationStatus(str, Enum):
     """
     Status in ReserveNow.conf.
@@ -580,14 +697,40 @@
     not_supported = "NotSupported"
 
     # Soon to be deprecated enums
     unlockFailed = "UnlockFailed"
     notSupported = "NotSupported"
 
 
+class UpdateFirmwareStatus(str, Enum):
+    """
+    UpdateFirmwareStatusEnumType is used by: SignedUpdateFirmware.conf
+    """
+
+    accepted = "Accepted"
+    rejected = "Rejected"
+    accepted_canceled = "AcceptedCanceled"
+    invalid_certificate = "InvalidCertificate"
+    revoked_certificate = "RevokedCertificate"
+
+
+class UploadLogStatus(str, Enum):
+    """
+    UploadLogStatusEnumType is used by: LogStatusNotification.req
+    """
+
+    bad_message = "BadMessage"
+    idle = "Idle"
+    not_supported_operation = "NotSupportedOperation"
+    permission_denied = "PermissionDenied"
+    uploaded = "Uploaded"
+    upload_failure = "UploadFailure"
+    uploading = "Uploading"
+
+
 class UpdateStatus(str, Enum):
     """
     Type of update for a SendLocalList.req.
     """
 
     accepted = "Accepted"
     failed = "Failed"
```

### Comparing `ocpp-0.8.3/ocpp/v16/schemas/AuthorizeResponse.json` & `ocpp-0.9.0/ocpp/v16/schemas/AuthorizeResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v16/schemas/BootNotification.json` & `ocpp-0.9.0/ocpp/v16/schemas/BootNotification.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v16/schemas/BootNotificationResponse.json` & `ocpp-0.9.0/ocpp/v16/schemas/BootNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v16/schemas/ChangeAvailability.json` & `ocpp-0.9.0/ocpp/v16/schemas/ChangeAvailability.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v16/schemas/ClearChargingProfile.json` & `ocpp-0.9.0/ocpp/v16/schemas/ClearChargingProfile.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v16/schemas/DataTransferResponse.json` & `ocpp-0.9.0/ocpp/v16/schemas/DataTransferResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v16/schemas/FirmwareStatusNotification.json` & `ocpp-0.9.0/ocpp/v16/schemas/FirmwareStatusNotification.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v16/schemas/GetCompositeSchedule.json` & `ocpp-0.9.0/ocpp/v16/schemas/GetCompositeSchedule.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v16/schemas/GetCompositeScheduleResponse.json` & `ocpp-0.9.0/ocpp/v16/schemas/GetCompositeScheduleResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v16/schemas/GetConfigurationResponse.json` & `ocpp-0.9.0/ocpp/v16/schemas/GetConfigurationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v16/schemas/GetDiagnostics.json` & `ocpp-0.9.0/ocpp/v16/schemas/GetDiagnostics.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v16/schemas/MeterValues.json` & `ocpp-0.9.0/ocpp/v16/schemas/MeterValues.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9953462577160493%*

 * *Differences: {"'properties'": "{'meterValue': {'items': {'properties': {'sampledValue': {'minItems': 1}}}, "*

 * *                 "'minItems': 1}}"}*

```diff
@@ -119,27 +119,29 @@
                                 }
                             },
                             "required": [
                                 "value"
                             ],
                             "type": "object"
                         },
+                        "minItems": 1,
                         "type": "array"
                     },
                     "timestamp": {
                         "format": "date-time",
                         "type": "string"
                     }
                 },
                 "required": [
                     "timestamp",
                     "sampledValue"
                 ],
                 "type": "object"
             },
+            "minItems": 1,
             "type": "array"
         },
         "transactionId": {
             "type": "integer"
         }
     },
     "required": [
```

### Comparing `ocpp-0.8.3/ocpp/v16/schemas/RemoteStartTransaction.json` & `ocpp-0.9.0/ocpp/v16/schemas/RemoteStartTransaction.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v16/schemas/ReserveNow.json` & `ocpp-0.9.0/ocpp/v16/schemas/ReserveNow.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v16/schemas/SendLocalList.json` & `ocpp-0.9.0/ocpp/v16/schemas/SendLocalList.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v16/schemas/SetChargingProfile.json` & `ocpp-0.9.0/ocpp/v16/schemas/SetChargingProfile.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v16/schemas/StartTransaction.json` & `ocpp-0.9.0/ocpp/v16/schemas/StartTransaction.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v16/schemas/StartTransactionResponse.json` & `ocpp-0.9.0/ocpp/v16/schemas/StartTransactionResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v16/schemas/StatusNotification.json` & `ocpp-0.9.0/ocpp/v16/schemas/StatusNotification.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v16/schemas/StopTransaction.json` & `ocpp-0.9.0/ocpp/v16/schemas/StopTransaction.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v16/schemas/StopTransactionResponse.json` & `ocpp-0.9.0/ocpp/v16/schemas/StopTransactionResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v16/schemas/TriggerMessage.json` & `ocpp-0.9.0/ocpp/v16/schemas/TriggerMessage.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v16/schemas/UpdateFirmware.json` & `ocpp-0.9.0/ocpp/v16/schemas/UpdateFirmware.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/call.py` & `ocpp-0.9.0/ocpp/v20/call.py`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/call_result.py` & `ocpp-0.9.0/ocpp/v20/call_result.py`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/AuthorizeRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/AuthorizeRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/AuthorizeResponse_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/AuthorizeResponse_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/BootNotificationRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/BootNotificationRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/BootNotificationResponse_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/BootNotificationResponse_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/CertificateSignedRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/CertificateSignedRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/ClearChargingProfileRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/ClearChargingProfileRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/ClearVariableMonitoringResponse_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/ClearVariableMonitoringResponse_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/CustomerInformationRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/CustomerInformationRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/DeleteCertificateRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/DeleteCertificateRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/FirmwareStatusNotificationRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/FirmwareStatusNotificationRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/Get15118EVCertificateResponse_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/Get15118EVCertificateResponse_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/GetCertificateStatusRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/GetCertificateStatusRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/GetChargingProfilesRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/GetChargingProfilesRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/GetCompositeScheduleResponse_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/GetCompositeScheduleResponse_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/GetDisplayMessagesRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/GetDisplayMessagesRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/GetInstalledCertificateIdsRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/GetInstalledCertificateIdsRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/GetInstalledCertificateIdsResponse_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/GetInstalledCertificateIdsResponse_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/GetLogRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/GetLogRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/GetMonitoringReportRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/GetMonitoringReportRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/GetReportRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/GetReportRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/GetVariablesRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/GetVariablesRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/GetVariablesResponse_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/GetVariablesResponse_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/InstallCertificateRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/InstallCertificateRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/InstallCertificateResponse_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/InstallCertificateResponse_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/LogStatusNotificationRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/LogStatusNotificationRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/MeterValuesRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/MeterValuesRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/NotifyCentralChargingNeedsRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/NotifyCentralChargingNeedsRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/NotifyChargingLimitRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/NotifyChargingLimitRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/NotifyCustomerInformationRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/NotifyCustomerInformationRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/NotifyDisplayMessagesRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/NotifyDisplayMessagesRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/NotifyEVChargingNeedsRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/NotifyEVChargingNeedsRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/NotifyEVChargingScheduleRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/NotifyEVChargingScheduleRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/NotifyEventRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/NotifyEventRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/NotifyMonitoringReportRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/NotifyMonitoringReportRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/NotifyReportRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/NotifyReportRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/PublishFirmwareStatusNotificationRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/PublishFirmwareStatusNotificationRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/Renegotiate15118ScheduleRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/Renegotiate15118ScheduleRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/ReportChargingProfilesRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/ReportChargingProfilesRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/RequestStartTransactionRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/RequestStartTransactionRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/ReserveNowRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/ReserveNowRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/SecurityEventNotificationRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/SecurityEventNotificationRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/SendLocalListRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/SendLocalListRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/SetChargingProfileRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/SetChargingProfileRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/SetDisplayMessageRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/SetDisplayMessageRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/SetNetworkProfileRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/SetNetworkProfileRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/SetVariableMonitoringRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/SetVariableMonitoringRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/SetVariableMonitoringResponse_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/SetVariableMonitoringResponse_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/SetVariablesRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/SetVariablesRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/SetVariablesResponse_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/SetVariablesResponse_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/StatusNotificationRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/StatusNotificationRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/TransactionEventRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/TransactionEventRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/TransactionEventResponse_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/TransactionEventResponse_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/TriggerMessageRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/TriggerMessageRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v20/schemas/UpdateFirmwareRequest_v1p0.json` & `ocpp-0.9.0/ocpp/v20/schemas/UpdateFirmwareRequest_v1p0.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/call.py` & `ocpp-0.9.0/ocpp/v201/call.py`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/call_result.py` & `ocpp-0.9.0/ocpp/v201/call_result.py`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/enums.py` & `ocpp-0.9.0/ocpp/v201/enums.py`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/AuthorizeRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/AuthorizeRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/AuthorizeResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/AuthorizeResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/BootNotificationRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/BootNotificationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/BootNotificationResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/BootNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/CancelReservationRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/CancelReservationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/CancelReservationResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/CancelReservationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/CertificateSignedRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/CertificateSignedRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/CertificateSignedResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/CertificateSignedResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/ChangeAvailabilityRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/ChangeAvailabilityRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/ChangeAvailabilityResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/ChangeAvailabilityResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/ClearCacheRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/ClearCacheRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/ClearCacheResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/ClearCacheResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/ClearChargingProfileRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/ClearChargingProfileRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/ClearChargingProfileResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/ClearChargingProfileResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/ClearDisplayMessageRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/ClearDisplayMessageRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/ClearDisplayMessageResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/ClearDisplayMessageResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/ClearVariableMonitoringRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/ClearVariableMonitoringRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/ClearVariableMonitoringResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/ClearVariableMonitoringResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/ClearedChargingLimitRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/ClearedChargingLimitRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/ClearedChargingLimitResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/ClearedChargingLimitResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/CostUpdatedRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/CostUpdatedRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/CostUpdatedResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/CostUpdatedResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/CustomerInformationRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/CustomerInformationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/CustomerInformationResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/CustomerInformationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/DataTransferRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/DataTransferRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/DataTransferResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/DataTransferResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/DeleteCertificateRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/DeleteCertificateRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/DeleteCertificateResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/DeleteCertificateResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/FirmwareStatusNotificationRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/FirmwareStatusNotificationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/FirmwareStatusNotificationResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/FirmwareStatusNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/Get15118EVCertificateRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/Get15118EVCertificateRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/Get15118EVCertificateResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/Get15118EVCertificateResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/GetBaseReportRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/GetBaseReportRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/GetBaseReportResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/GetBaseReportResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/GetCertificateStatusRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/GetCertificateStatusRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/GetCertificateStatusResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/GetCertificateStatusResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/GetChargingProfilesRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/GetChargingProfilesRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/GetChargingProfilesResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/GetChargingProfilesResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/GetCompositeScheduleRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/GetCompositeScheduleRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/GetCompositeScheduleResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/GetCompositeScheduleResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/GetDisplayMessagesRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/GetDisplayMessagesRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/GetDisplayMessagesResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/GetDisplayMessagesResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/GetInstalledCertificateIdsRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/GetInstalledCertificateIdsRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/GetInstalledCertificateIdsResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/GetInstalledCertificateIdsResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/GetLocalListVersionRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/GetLocalListVersionRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/GetLocalListVersionResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/GetLocalListVersionResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/GetLogRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/GetLogRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/GetLogResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/GetLogResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/GetMonitoringReportRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/GetMonitoringReportRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/GetMonitoringReportResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/GetMonitoringReportResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/GetReportRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/GetReportRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/GetReportResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/GetReportResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/GetTransactionStatusRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/GetTransactionStatusRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/GetTransactionStatusResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/GetTransactionStatusResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/GetVariablesRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/GetVariablesRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/GetVariablesResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/GetVariablesResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/HeartbeatRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/HeartbeatRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/HeartbeatResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/HeartbeatResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/InstallCertificateRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/InstallCertificateRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/InstallCertificateResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/InstallCertificateResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/LogStatusNotificationRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/LogStatusNotificationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/LogStatusNotificationResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/LogStatusNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/MeterValuesRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/MeterValuesRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/MeterValuesResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/MeterValuesResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/NotifyChargingLimitRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/NotifyChargingLimitRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/NotifyChargingLimitResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/NotifyChargingLimitResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/NotifyCustomerInformationRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/NotifyCustomerInformationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/NotifyCustomerInformationResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/NotifyCustomerInformationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/NotifyDisplayMessagesRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/NotifyDisplayMessagesRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/NotifyDisplayMessagesResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/NotifyDisplayMessagesResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/NotifyEVChargingNeedsRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/NotifyEVChargingNeedsRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/NotifyEVChargingNeedsResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/NotifyEVChargingNeedsResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/NotifyEVChargingScheduleRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/NotifyEVChargingScheduleRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/NotifyEVChargingScheduleResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/NotifyEVChargingScheduleResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/NotifyEventRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/NotifyEventRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/NotifyEventResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/NotifyEventResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/NotifyMonitoringReportRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/NotifyMonitoringReportRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/NotifyMonitoringReportResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/NotifyMonitoringReportResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/NotifyReportRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/NotifyReportRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/NotifyReportResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/NotifyReportResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/PublishFirmwareRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/PublishFirmwareRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/PublishFirmwareResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/PublishFirmwareResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/PublishFirmwareStatusNotificationRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/PublishFirmwareStatusNotificationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/PublishFirmwareStatusNotificationResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/PublishFirmwareStatusNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/ReportChargingProfilesRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/ReportChargingProfilesRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/ReportChargingProfilesResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/ReportChargingProfilesResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/RequestStartTransactionRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/RequestStartTransactionRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/RequestStartTransactionResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/RequestStartTransactionResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/RequestStopTransactionRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/RequestStopTransactionRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/RequestStopTransactionResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/RequestStopTransactionResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/ReservationStatusUpdateRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/ReservationStatusUpdateRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/ReservationStatusUpdateResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/ReservationStatusUpdateResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/ReserveNowRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/ReserveNowRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/ReserveNowResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/ReserveNowResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/ResetRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/ResetRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/ResetResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/ResetResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/SecurityEventNotificationRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/SecurityEventNotificationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/SecurityEventNotificationResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/SecurityEventNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/SendLocalListRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/SendLocalListRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/SendLocalListResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/SendLocalListResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/SetChargingProfileRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/SetChargingProfileRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/SetChargingProfileResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/SetChargingProfileResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/SetDisplayMessageRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/SetDisplayMessageRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/SetDisplayMessageResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/SetDisplayMessageResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/SetMonitoringBaseRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/SetMonitoringBaseRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/SetMonitoringBaseResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/SetMonitoringBaseResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/SetMonitoringLevelRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/SetMonitoringLevelRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/SetMonitoringLevelResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/SetMonitoringLevelResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/SetNetworkProfileRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/SetNetworkProfileRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/SetNetworkProfileResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/SetNetworkProfileResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/SetVariableMonitoringRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/SetVariableMonitoringRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/SetVariableMonitoringResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/SetVariableMonitoringResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/SetVariablesRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/SetVariablesRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/SetVariablesResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/SetVariablesResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/SignCertificateRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/SignCertificateRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/SignCertificateResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/SignCertificateResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/StatusNotificationRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/StatusNotificationRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/StatusNotificationResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/StatusNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/TransactionEventRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/TransactionEventRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/TransactionEventResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/TransactionEventResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/TriggerMessageRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/TriggerMessageRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/TriggerMessageResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/TriggerMessageResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/UnlockConnectorRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/UnlockConnectorRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/UnlockConnectorResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/UnlockConnectorResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/UnpublishFirmwareRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/UnpublishFirmwareRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/UnpublishFirmwareResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/UnpublishFirmwareResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/UpdateFirmwareRequest.json` & `ocpp-0.9.0/ocpp/v201/schemas/UpdateFirmwareRequest.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/ocpp/v201/schemas/UpdateFirmwareResponse.json` & `ocpp-0.9.0/ocpp/v201/schemas/UpdateFirmwareResponse.json`

 * *Files identical despite different names*

### Comparing `ocpp-0.8.3/pyproject.toml` & `ocpp-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ocpp"
-version = "0.8.3"
+version = "0.9.0"
 description = "Python package implementing the JSON version of the Open Charge Point Protocol (OCPP)."
 authors = [
 	"Andre Duarte <andre.duarte@mobilityhouse.com>",
 	"Auke Willem Oosterhoff <aukewillem.oosterhoff@mobilityhouse.com>",
 	"Greg Lutostanski <greg.lutostanski@mobilityhouse.com>",
 	"Jonathan Herrmann <jonathan.herrmann@mobilityhouse.com>",
 	"Laysa Uchoa <laysa.uchoadasilva@mobilityhouse.com>",
```

### Comparing `ocpp-0.8.3/setup.py` & `ocpp-0.9.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 ['jsonschema>=3.0,<4.0']
 
 extras_require = \
 {':python_version >= "3.6" and python_version < "3.7"': ['dataclasses>=0.6,<0.7']}
 
 setup_kwargs = {
     'name': 'ocpp',
-    'version': '0.8.3',
+    'version': '0.9.0',
     'description': 'Python package implementing the JSON version of the Open Charge Point Protocol (OCPP).',
-    'long_description': '.. image:: https://circleci.com/gh/mobilityhouse/ocpp/tree/master.svg?style=svg\n   :target: https://circleci.com/gh/mobilityhouse/ocpp/tree/master\n\n.. image:: https://img.shields.io/pypi/pyversions/ocpp.svg\n   :target: https://pypi.org/project/ocpp/\n\n.. image:: https://img.shields.io/readthedocs/ocpp.svg\n   :target: https://ocpp.readthedocs.io/en/latest/\n\nOCPP\n----\n\nPython package implementing the JSON version of the Open Charge Point Protocol\n(OCPP). Currently OCPP 1.6 (errata v4), OCPP 2.0 and OCPP 2.0.1 (Final Version)\nare supported.\n\nYou can find the documentation on `rtd`_.\n\nInstallation\n------------\n\nYou can either the project install from Pypi:\n\n.. code-block:: bash\n\n   $ pip install ocpp\n\nOr clone the project and install it manually using:\n\n.. code-block:: bash\n\n   $ pip install .\n\nQuick start\n-----------\n\nBelow you can find examples on how to create a simple OCPP 2.0 central system as\nwell as an OCPP 2.0 charge point.\n\n.. note::\n\n   To run these examples the dependency websockets_ is required! Install it by running:\n\n   .. code-block:: bash\n\n      $ pip install websockets\n\nCentral system\n~~~~~~~~~~~~~~\n\nThe code snippet below creates a simple OCPP 2.0 central system which is able\nto handle BootNotification calls. You can find a detailed explanation of the\ncode in the `Central System documentation_`.\n\n\n.. code-block:: python\n\n    import asyncio\n    import logging\n    import websockets\n    from datetime import datetime\n\n    from ocpp.routing import on\n    from ocpp.v201 import ChargePoint as cp\n    from ocpp.v201 import call_result\n\n    logging.basicConfig(level=logging.INFO)\n\n\n    class ChargePoint(cp):\n        @on(\'BootNotification\')\n        async def on_boot_notification(self, charging_station, reason, **kwargs):\n            return call_result.BootNotificationPayload(\n                current_time=datetime.utcnow().isoformat(),\n                interval=10,\n                status=\'Accepted\'\n            )\n\n\n    async def on_connect(websocket, path):\n        """ For every new charge point that connects, create a ChargePoint\n        instance and start listening for messages.\n        """\n        try:\n            requested_protocols = websocket.request_headers[\n                \'Sec-WebSocket-Protocol\']\n        except KeyError:\n            logging.info("Client hasn\'t requested any Subprotocol. "\n                     "Closing Connection")\n        if websocket.subprotocol:\n            logging.info("Protocols Matched: %s", websocket.subprotocol)\n        else:\n            # In the websockets lib if no subprotocols are supported by the\n            # client and the server, it proceeds without a subprotocol,\n            # so we have to manually close the connection.\n            logging.warning(\'Protocols Mismatched | Expected Subprotocols: %s,\'\n                            \' but client supports  %s | Closing connection\',\n                            websocket.available_subprotocols,\n                            requested_protocols)\n            return await websocket.close()\n\n        charge_point_id = path.strip(\'/\')\n        cp = ChargePoint(charge_point_id, websocket)\n\n        await cp.start()\n\n\n    async def main():\n        server = await websockets.serve(\n            on_connect,\n            \'0.0.0.0\',\n            9000,\n            subprotocols=[\'ocpp2.0.1\']\n        )\n        logging.info("WebSocket Server Started")\n        await server.wait_closed()\n\n    if __name__ == \'__main__\':\n        asyncio.run(main())\n\nCharge point\n~~~~~~~~~~~~\n\n.. code-block:: python\n\n    import asyncio\n    import logging\n    import websockets\n\n    from ocpp.v201 import call\n    from ocpp.v201 import ChargePoint as cp\n\n    logging.basicConfig(level=logging.INFO)\n\n\n    class ChargePoint(cp):\n\n       async def send_boot_notification(self):\n           request = call.BootNotificationPayload(\n                   charging_station={\n                       \'model\': \'Wallbox XYZ\',\n                       \'vendor_name\': \'anewone\'\n                   },\n                   reason="PowerUp"\n           )\n           response = await self.call(request)\n\n           if response.status == \'Accepted\':\n               print("Connected to central system.")\n\n\n    async def main():\n       async with websockets.connect(\n           \'ws://localhost:9000/CP_1\',\n            subprotocols=[\'ocpp2.0.1\']\n       ) as ws:\n\n           cp = ChargePoint(\'CP_1\', ws)\n\n           await asyncio.gather(cp.start(), cp.send_boot_notification())\n\n\n    if __name__ == \'__main__\':\n       asyncio.run(main())\n\nLicense\n-------\n\nExcept from the documents in `docs/v16` and `docs/v201` everything is licensed under MIT_.\n© `The Mobility House`_\n\nThe documents in `docs/v16` and `docs/v201` are licensed under Creative Commons\nAttribution-NoDerivatives 4.0 International Public License.\n\n.. _Central System documentation: https://ocpp.readthedocs.io/en/latest/central_system.html\n.. _MIT: https://github.com/mobilityhouse/ocpp/blob/master/LICENSE\n.. _rtd: https://ocpp.readthedocs.io/en/latest/index.html\n.. _The Mobility House: https://www.mobilityhouse.com/int_en/\n.. _websockets: https://pypi.org/project/websockets/\n',
+    'long_description': '.. image:: https://circleci.com/gh/mobilityhouse/ocpp/tree/master.svg?style=svg\n   :target: https://circleci.com/gh/mobilityhouse/ocpp/tree/master\n\n.. image:: https://img.shields.io/pypi/pyversions/ocpp.svg\n   :target: https://pypi.org/project/ocpp/\n\n.. image:: https://img.shields.io/readthedocs/ocpp.svg\n   :target: https://ocpp.readthedocs.io/en/latest/\n\nOCPP\n----\n\nPython package implementing the JSON version of the Open Charge Point Protocol\n(OCPP). Currently OCPP 1.6 (errata v4), OCPP 2.0 and OCPP 2.0.1 (Final Version)\nare supported.\n\nYou can find the documentation on `rtd`_.\n\nInstallation\n------------\n\nYou can either the project install from Pypi:\n\n.. code-block:: bash\n\n   $ pip install ocpp\n\nOr clone the project and install it manually using:\n\n.. code-block:: bash\n\n   $ pip install .\n\nQuick start\n-----------\n\nBelow you can find examples on how to create a simple OCPP 2.0 central system as\nwell as an OCPP 2.0 charge point.\n\n.. note::\n\n   To run these examples the dependency websockets_ is required! Install it by running:\n\n   .. code-block:: bash\n\n      $ pip install websockets\n\nCentral system\n~~~~~~~~~~~~~~\n\nThe code snippet below creates a simple OCPP 2.0 central system which is able\nto handle BootNotification calls. You can find a detailed explanation of the\ncode in the `Central System documentation_`.\n\n\n.. code-block:: python\n\n    import asyncio\n    import logging\n    import websockets\n    from datetime import datetime\n\n    from ocpp.routing import on\n    from ocpp.v201 import ChargePoint as cp\n    from ocpp.v201 import call_result\n\n    logging.basicConfig(level=logging.INFO)\n\n\n    class ChargePoint(cp):\n        @on(\'BootNotification\')\n        async def on_boot_notification(self, charging_station, reason, **kwargs):\n            return call_result.BootNotificationPayload(\n                current_time=datetime.utcnow().isoformat(),\n                interval=10,\n                status=\'Accepted\'\n            )\n\n\n    async def on_connect(websocket, path):\n        """ For every new charge point that connects, create a ChargePoint\n        instance and start listening for messages.\n        """\n        try:\n            requested_protocols = websocket.request_headers[\n                \'Sec-WebSocket-Protocol\']\n        except KeyError:\n            logging.info("Client hasn\'t requested any Subprotocol. "\n                     "Closing Connection")\n        if websocket.subprotocol:\n            logging.info("Protocols Matched: %s", websocket.subprotocol)\n        else:\n            # In the websockets lib if no subprotocols are supported by the\n            # client and the server, it proceeds without a subprotocol,\n            # so we have to manually close the connection.\n            logging.warning(\'Protocols Mismatched | Expected Subprotocols: %s,\'\n                            \' but client supports  %s | Closing connection\',\n                            websocket.available_subprotocols,\n                            requested_protocols)\n            return await websocket.close()\n\n        charge_point_id = path.strip(\'/\')\n        cp = ChargePoint(charge_point_id, websocket)\n\n        await cp.start()\n\n\n    async def main():\n        server = await websockets.serve(\n            on_connect,\n            \'0.0.0.0\',\n            9000,\n            subprotocols=[\'ocpp2.0.1\']\n        )\n        logging.info("WebSocket Server Started")\n        await server.wait_closed()\n\n    if __name__ == \'__main__\':\n        asyncio.run(main())\n\nCharge point\n~~~~~~~~~~~~\n\n.. code-block:: python\n\n    import asyncio\n    import logging\n    import websockets\n\n    from ocpp.v201 import call\n    from ocpp.v201 import ChargePoint as cp\n\n    logging.basicConfig(level=logging.INFO)\n\n\n    class ChargePoint(cp):\n\n       async def send_boot_notification(self):\n           request = call.BootNotificationPayload(\n                   charging_station={\n                       \'model\': \'Wallbox XYZ\',\n                       \'vendor_name\': \'anewone\'\n                   },\n                   reason="PowerUp"\n           )\n           response = await self.call(request)\n\n           if response.status == \'Accepted\':\n               print("Connected to central system.")\n\n\n    async def main():\n       async with websockets.connect(\n           \'ws://localhost:9000/CP_1\',\n            subprotocols=[\'ocpp2.0.1\']\n       ) as ws:\n\n           cp = ChargePoint(\'CP_1\', ws)\n\n           await asyncio.gather(cp.start(), cp.send_boot_notification())\n\n\n    if __name__ == \'__main__\':\n       asyncio.run(main())\n\nDebugging\n---------\n\nPython\'s default log level is `logging.WARNING`. As result most of the logs\ngenerated by this package are discarded. To see the log output of this package\nlower the log level to `logging.DEBUG`.\n\n.. code-block:: python\n\n  import logging\n  logging.basicConfig(level=logging.DEBUG)\n\nHowever, this approach defines the log level for the complete logging system.\nIn other words: the log level of all dependencies is set to `logging.DEBUG`.\n\nTo lower the logs for this package only use the following code:\n\n.. code-block:: python\n\n  import logging\n  logging.getLogger(\'ocpp\').setLevel(level=logging.DEBUG)\n  logging.getLogger(\'ocpp\').addHandler(logging.StreamHandler())\n\nLicense\n-------\n\nExcept from the documents in `docs/v16` and `docs/v201` everything is licensed under MIT_.\n© `The Mobility House`_\n\nThe documents in `docs/v16` and `docs/v201` are licensed under Creative Commons\nAttribution-NoDerivatives 4.0 International Public License.\n\n.. _Central System documentation: https://ocpp.readthedocs.io/en/latest/central_system.html\n.. _MIT: https://github.com/mobilityhouse/ocpp/blob/master/LICENSE\n.. _rtd: https://ocpp.readthedocs.io/en/latest/index.html\n.. _The Mobility House: https://www.mobilityhouse.com/int_en/\n.. _websockets: https://pypi.org/project/websockets/\n',
     'author': 'Andre Duarte',
     'author_email': 'andre.duarte@mobilityhouse.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/mobilityhouse/ocpp',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `ocpp-0.8.3/PKG-INFO` & `ocpp-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocpp
-Version: 0.8.3
+Version: 0.9.0
 Summary: Python package implementing the JSON version of the Open Charge Point Protocol (OCPP).
 Home-page: https://github.com/mobilityhouse/ocpp
 License: MIT
 Author: Andre Duarte
 Author-email: andre.duarte@mobilityhouse.com
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -181,14 +181,37 @@
 
            await asyncio.gather(cp.start(), cp.send_boot_notification())
 
 
     if __name__ == '__main__':
        asyncio.run(main())
 
+Debugging
+---------
+
+Python's default log level is `logging.WARNING`. As result most of the logs
+generated by this package are discarded. To see the log output of this package
+lower the log level to `logging.DEBUG`.
+
+.. code-block:: python
+
+  import logging
+  logging.basicConfig(level=logging.DEBUG)
+
+However, this approach defines the log level for the complete logging system.
+In other words: the log level of all dependencies is set to `logging.DEBUG`.
+
+To lower the logs for this package only use the following code:
+
+.. code-block:: python
+
+  import logging
+  logging.getLogger('ocpp').setLevel(level=logging.DEBUG)
+  logging.getLogger('ocpp').addHandler(logging.StreamHandler())
+
 License
 -------
 
 Except from the documents in `docs/v16` and `docs/v201` everything is licensed under MIT_.
 © `The Mobility House`_
 
 The documents in `docs/v16` and `docs/v201` are licensed under Creative Commons
```

