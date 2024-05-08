# Comparing `tmp/duxcocpp-0.1.7.tar.gz` & `tmp/duxcocpp-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duxcocpp-0.1.7.tar", max compression
+gzip compressed data, was "duxcocpp-0.2.2.tar", max compression
```

## Comparing `duxcocpp-0.1.7.tar` & `duxcocpp-0.2.2.tar`

### file list

```diff
@@ -1,226 +1,226 @@
--rw-r--r--   0        0        0     1075 2024-05-08 06:53:44.123794 duxcocpp-0.1.7/LICENSE
--rw-r--r--   0        0        0     6037 2024-05-08 06:53:44.123794 duxcocpp-0.1.7/README.rst
--rw-r--r--   0        0        0        0 2024-05-08 06:53:44.279794 duxcocpp-0.1.7/ocpp/__init__.py
--rw-r--r--   0        0        0    16259 2024-05-08 06:53:44.279794 duxcocpp-0.1.7/ocpp/charge_point.py
--rw-r--r--   0        0        0     4451 2024-05-08 06:53:44.279794 duxcocpp-0.1.7/ocpp/exceptions.py
--rw-r--r--   0        0        0      221 2024-05-08 06:53:44.279794 duxcocpp-0.1.7/ocpp/experimental/v21/README.rst
--rw-r--r--   0        0        0    14821 2024-05-08 06:53:44.279794 duxcocpp-0.1.7/ocpp/messages.py
--rw-r--r--   0        0        0     4106 2024-05-08 06:53:44.279794 duxcocpp-0.1.7/ocpp/routing.py
--rw-r--r--   0        0        0      186 2024-05-08 06:53:44.279794 duxcocpp-0.1.7/ocpp/v16/__init__.py
--rw-r--r--   0        0        0    20548 2024-05-08 06:53:44.279794 duxcocpp-0.1.7/ocpp/v16/call.py
--rw-r--r--   0        0        0    19232 2024-05-08 06:53:44.279794 duxcocpp-0.1.7/ocpp/v16/call_result.py
--rw-r--r--   0        0        0     3968 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/datatypes.py
--rw-r--r--   0        0        0    23663 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/enums.py
--rw-r--r--   0        0        0      306 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/Authorize.json
--rw-r--r--   0        0        0     1062 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/AuthorizeResponse.json
--rw-r--r--   0        0        0     1139 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/BootNotification.json
--rw-r--r--   0        0        0      655 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/BootNotificationResponse.json
--rw-r--r--   0        0        0      302 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/CancelReservation.json
--rw-r--r--   0        0        0      423 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/CancelReservationResponse.json
--rw-r--r--   0        0        0      352 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/CertificateSigned.json
--rw-r--r--   0        0        0      505 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/CertificateSignedResponse.json
--rw-r--r--   0        0        0      512 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/ChangeAvailability.json
--rw-r--r--   0        0        0      453 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/ChangeAvailabilityResponse.json
--rw-r--r--   0        0        0      418 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/ChangeConfiguration.json
--rw-r--r--   0        0        0      491 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/ChangeConfigurationResponse.json
--rw-r--r--   0        0        0      174 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/ClearCache.json
--rw-r--r--   0        0        0      416 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/ClearCacheResponse.json
--rw-r--r--   0        0        0      637 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/ClearChargingProfile.json
--rw-r--r--   0        0        0      425 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/ClearChargingProfileResponse.json
--rw-r--r--   0        0        0      466 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/DataTransfer.json
--rw-r--r--   0        0        0      547 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/DataTransferResponse.json
--rw-r--r--   0        0        0     1156 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/DeleteCertificate.json
--rw-r--r--   0        0        0      523 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/DeleteCertificateResponse.json
--rw-r--r--   0        0        0      491 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/DiagnosticsStatusNotification.json
--rw-r--r--   0        0        0      194 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/DiagnosticsStatusNotificationResponse.json
--rw-r--r--   0        0        0      760 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/ExtendedTriggerMessage.json
--rw-r--r--   0        0        0      530 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/ExtendedTriggerMessageResponse.json
--rw-r--r--   0        0        0      591 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/FirmwareStatusNotification.json
--rw-r--r--   0        0        0      191 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/FirmwareStatusNotificationResponse.json
--rw-r--r--   0        0        0      539 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/GetCompositeSchedule.json
--rw-r--r--   0        0        0     2139 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/GetCompositeScheduleResponse.json
--rw-r--r--   0        0        0      344 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/GetConfiguration.json
--rw-r--r--   0        0        0     1066 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/GetConfigurationResponse.json
--rw-r--r--   0        0        0      642 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/GetDiagnostics.json
--rw-r--r--   0        0        0      275 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/GetDiagnosticsResponse.json
--rw-r--r--   0        0        0      552 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/GetInstalledCertificateIds.json
--rw-r--r--   0        0        0     1566 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/GetInstalledCertificateIdsResponse.json
--rw-r--r--   0        0        0      183 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/GetLocalListVersion.json
--rw-r--r--   0        0        0      301 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/GetLocalListVersionResponse.json
--rw-r--r--   0        0        0     1184 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/GetLog.json
--rw-r--r--   0        0        0      566 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/GetLogResponse.json
--rw-r--r--   0        0        0      173 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/Heartbeat.json
--rw-r--r--   0        0        0      325 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/HeartbeatResponse.json
--rw-r--r--   0        0        0      639 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/InstallCertificate.json
--rw-r--r--   0        0        0      526 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/InstallCertificateResponse.json
--rw-r--r--   0        0        0      667 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/LogStatusNotification.json
--rw-r--r--   0        0        0      173 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/LogStatusNotificationResponse.json
--rw-r--r--   0        0        0     6758 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/MeterValues.json
--rw-r--r--   0        0        0      176 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/MeterValuesResponse.json
--rw-r--r--   0        0        0     4383 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/RemoteStartTransaction.json
--rw-r--r--   0        0        0      428 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/RemoteStartTransactionResponse.json
--rw-r--r--   0        0        0      306 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/RemoteStopTransaction.json
--rw-r--r--   0        0        0      427 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/RemoteStopTransactionResponse.json
--rw-r--r--   0        0        0      704 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/ReserveNow.json
--rw-r--r--   0        0        0      502 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/ReserveNowResponse.json
--rw-r--r--   0        0        0      398 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/Reset.json
--rw-r--r--   0        0        0      411 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/ResetResponse.json
--rw-r--r--   0        0        0      464 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/SecurityEventNotification.json
--rw-r--r--   0        0        0      177 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/SecurityEventNotificationResponse.json
--rw-r--r--   0        0        0     2146 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/SendLocalList.json
--rw-r--r--   0        0        0      484 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/SendLocalListResponse.json
--rw-r--r--   0        0        0     4310 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/SetChargingProfile.json
--rw-r--r--   0        0        0      456 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/SetChargingProfileResponse.json
--rw-r--r--   0        0        0      287 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/SignCertificate.json
--rw-r--r--   0        0        0      483 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/SignCertificateResponse.json
--rw-r--r--   0        0        0      876 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/SignedFirmwareStatusNotification.json
--rw-r--r--   0        0        0      184 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/SignedFirmwareStatusNotificationResponse.json
--rw-r--r--   0        0        0     1212 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/SignedUpdateFirmware.json
--rw-r--r--   0        0        0      590 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/SignedUpdateFirmwareResponse.json
--rw-r--r--   0        0        0      676 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/StartTransaction.json
--rw-r--r--   0        0        0     1162 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/StartTransactionResponse.json
--rw-r--r--   0        0        0     1805 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/StatusNotification.json
--rw-r--r--   0        0        0      183 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/StatusNotificationResponse.json
--rw-r--r--   0        0        0     7313 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/StopTransaction.json
--rw-r--r--   0        0        0     1023 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/StopTransactionResponse.json
--rw-r--r--   0        0        0      678 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/TriggerMessage.json
--rw-r--r--   0        0        0      454 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/TriggerMessageResponse.json
--rw-r--r--   0        0        0      296 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/UnlockConnector.json
--rw-r--r--   0        0        0      457 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/UnlockConnectorResponse.json
--rw-r--r--   0        0        0      572 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/UpdateFirmware.json
--rw-r--r--   0        0        0      179 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v16/schemas/UpdateFirmwareResponse.json
--rw-r--r--   0        0        0      189 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v201/__init__.py
--rw-r--r--   0        0        0    34073 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v201/call.py
--rw-r--r--   0        0        0    32301 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v201/call_result.py
--rw-r--r--   0        0        0    22081 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v201/datatypes.py
--rw-r--r--   0        0        0    80113 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v201/enums.py
--rw-r--r--   0        0        0     4203 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v201/schemas/AuthorizeRequest.json
--rw-r--r--   0        0        0     7208 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v201/schemas/AuthorizeResponse.json
--rw-r--r--   0        0        0     3161 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v201/schemas/BootNotificationRequest.json
--rw-r--r--   0        0        0     2270 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v201/schemas/BootNotificationResponse.json
--rw-r--r--   0        0        0      775 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v201/schemas/CancelReservationRequest.json
--rw-r--r--   0        0        0     1758 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v201/schemas/CancelReservationResponse.json
--rw-r--r--   0        0        0     1914 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v201/schemas/CertificateSignedRequest.json
--rw-r--r--   0        0        0     1752 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v201/schemas/CertificateSignedResponse.json
--rw-r--r--   0        0        0     1811 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v201/schemas/ChangeAvailabilityRequest.json
--rw-r--r--   0        0        0     1783 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v201/schemas/ChangeAvailabilityResponse.json
--rw-r--r--   0        0        0      634 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v201/schemas/ClearCacheRequest.json
--rw-r--r--   0        0        0     1735 2024-05-08 06:53:44.283794 duxcocpp-0.1.7/ocpp/v201/schemas/ClearCacheResponse.json
--rw-r--r--   0        0        0     2574 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/ClearChargingProfileRequest.json
--rw-r--r--   0        0        0     1752 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/ClearChargingProfileResponse.json
--rw-r--r--   0        0        0      787 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/ClearDisplayMessageRequest.json
--rw-r--r--   0        0        0     1735 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/ClearDisplayMessageResponse.json
--rw-r--r--   0        0        0      865 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/ClearVariableMonitoringRequest.json
--rw-r--r--   0        0        0     2327 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/ClearVariableMonitoringResponse.json
--rw-r--r--   0        0        0     1087 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/ClearedChargingLimitRequest.json
--rw-r--r--   0        0        0      634 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/ClearedChargingLimitResponse.json
--rw-r--r--   0        0        0     1121 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/CostUpdatedRequest.json
--rw-r--r--   0        0        0      634 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/CostUpdatedResponse.json
--rw-r--r--   0        0        0     4659 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/CustomerInformationRequest.json
--rw-r--r--   0        0        0     1740 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/CustomerInformationResponse.json
--rw-r--r--   0        0        0     1101 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/DataTransferRequest.json
--rw-r--r--   0        0        0     1869 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/DataTransferResponse.json
--rw-r--r--   0        0        0     1808 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/DeleteCertificateRequest.json
--rw-r--r--   0        0        0     1747 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/DeleteCertificateResponse.json
--rw-r--r--   0        0        0     1539 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/FirmwareStatusNotificationRequest.json
--rw-r--r--   0        0        0      634 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/FirmwareStatusNotificationResponse.json
--rw-r--r--   0        0        0     1424 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/Get15118EVCertificateRequest.json
--rw-r--r--   0        0        0     1915 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/Get15118EVCertificateResponse.json
--rw-r--r--   0        0        0     1105 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/GetBaseReportRequest.json
--rw-r--r--   0        0        0     1794 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/GetBaseReportResponse.json
--rw-r--r--   0        0        0     1957 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/GetCertificateStatusRequest.json
--rw-r--r--   0        0        0     2089 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/GetCertificateStatusResponse.json
--rw-r--r--   0        0        0     3622 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/GetChargingProfilesRequest.json
--rw-r--r--   0        0        0     1859 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/GetChargingProfilesResponse.json
--rw-r--r--   0        0        0     1329 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/GetCompositeScheduleRequest.json
--rw-r--r--   0        0        0     5095 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/GetCompositeScheduleResponse.json
--rw-r--r--   0        0        0     1874 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/GetDisplayMessagesRequest.json
--rw-r--r--   0        0        0     1841 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/GetDisplayMessagesResponse.json
--rw-r--r--   0        0        0     1204 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/GetInstalledCertificateIdsRequest.json
--rw-r--r--   0        0        0     3997 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/GetInstalledCertificateIdsResponse.json
--rw-r--r--   0        0        0      634 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/GetLocalListVersionRequest.json
--rw-r--r--   0        0        0      840 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/GetLocalListVersionResponse.json
--rw-r--r--   0        0        0     2802 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/GetLogRequest.json
--rw-r--r--   0        0        0     1954 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/GetLogResponse.json
--rw-r--r--   0        0        0     4175 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/GetMonitoringReportRequest.json
--rw-r--r--   0        0        0     1800 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/GetMonitoringReportResponse.json
--rw-r--r--   0        0        0     4143 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/GetReportRequest.json
--rw-r--r--   0        0        0     1800 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/GetReportResponse.json
--rw-r--r--   0        0        0      784 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/GetTransactionStatusRequest.json
--rw-r--r--   0        0        0      910 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/GetTransactionStatusResponse.json
--rw-r--r--   0        0        0     3931 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/GetVariablesRequest.json
--rw-r--r--   0        0        0     5581 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/GetVariablesResponse.json
--rw-r--r--   0        0        0      634 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/HeartbeatRequest.json
--rw-r--r--   0        0        0      802 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/HeartbeatResponse.json
--rw-r--r--   0        0        0     1226 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/InstallCertificateRequest.json
--rw-r--r--   0        0        0     1751 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/InstallCertificateResponse.json
--rw-r--r--   0        0        0     1361 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/LogStatusNotificationRequest.json
--rw-r--r--   0        0        0      634 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/LogStatusNotificationResponse.json
--rw-r--r--   0        0        0     7709 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/MeterValuesRequest.json
--rw-r--r--   0        0        0      634 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/MeterValuesResponse.json
--rw-r--r--   0        0        0    11333 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/NotifyChargingLimitRequest.json
--rw-r--r--   0        0        0      634 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/NotifyChargingLimitResponse.json
--rw-r--r--   0        0        0     1542 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/NotifyCustomerInformationRequest.json
--rw-r--r--   0        0        0      634 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/NotifyCustomerInformationResponse.json
--rw-r--r--   0        0        0     6512 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/NotifyDisplayMessagesRequest.json
--rw-r--r--   0        0        0      634 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/NotifyDisplayMessagesResponse.json
--rw-r--r--   0        0        0     5943 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/NotifyEVChargingNeedsRequest.json
--rw-r--r--   0        0        0     1870 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/NotifyEVChargingNeedsResponse.json
--rw-r--r--   0        0        0    10370 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/NotifyEVChargingScheduleRequest.json
--rw-r--r--   0        0        0     1780 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/NotifyEVChargingScheduleResponse.json
--rw-r--r--   0        0        0     6614 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/NotifyEventRequest.json
--rw-r--r--   0        0        0      634 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/NotifyEventResponse.json
--rw-r--r--   0        0        0     7005 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/NotifyMonitoringReportRequest.json
--rw-r--r--   0        0        0      634 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/NotifyMonitoringReportResponse.json
--rw-r--r--   0        0        0     8608 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/NotifyReportRequest.json
--rw-r--r--   0        0        0      634 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/NotifyReportResponse.json
--rw-r--r--   0        0        0     1668 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/PublishFirmwareRequest.json
--rw-r--r--   0        0        0     1691 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/PublishFirmwareResponse.json
--rw-r--r--   0        0        0     1631 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/PublishFirmwareStatusNotificationRequest.json
--rw-r--r--   0        0        0      634 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/PublishFirmwareStatusNotificationResponse.json
--rw-r--r--   0        0        0    14700 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/ReportChargingProfilesRequest.json
--rw-r--r--   0        0        0      634 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/ReportChargingProfilesResponse.json
--rw-r--r--   0        0        0    15964 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/RequestStartTransactionRequest.json
--rw-r--r--   0        0        0     2080 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/RequestStartTransactionResponse.json
--rw-r--r--   0        0        0      844 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/RequestStopTransactionRequest.json
--rw-r--r--   0        0        0     1760 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/RequestStopTransactionResponse.json
--rw-r--r--   0        0        0     1133 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/ReservationStatusUpdateRequest.json
--rw-r--r--   0        0        0      634 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/ReservationStatusUpdateResponse.json
--rw-r--r--   0        0        0     3649 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/ReserveNowRequest.json
--rw-r--r--   0        0        0     1758 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/ReserveNowResponse.json
--rw-r--r--   0        0        0     1144 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/ResetRequest.json
--rw-r--r--   0        0        0     1730 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/ResetResponse.json
--rw-r--r--   0        0        0     1120 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/SecurityEventNotificationRequest.json
--rw-r--r--   0        0        0      634 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/SecurityEventNotificationResponse.json
--rw-r--r--   0        0        0     7733 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/SendLocalListRequest.json
--rw-r--r--   0        0        0     1810 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/SendLocalListResponse.json
--rw-r--r--   0        0        0    13730 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/SetChargingProfileRequest.json
--rw-r--r--   0        0        0     1913 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/SetChargingProfileResponse.json
--rw-r--r--   0        0        0     5989 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/SetDisplayMessageRequest.json
--rw-r--r--   0        0        0     1848 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/SetDisplayMessageResponse.json
--rw-r--r--   0        0        0     1005 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/SetMonitoringBaseRequest.json
--rw-r--r--   0        0        0     1789 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/SetMonitoringBaseResponse.json
--rw-r--r--   0        0        0     2087 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/SetMonitoringLevelRequest.json
--rw-r--r--   0        0        0     1718 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/SetMonitoringLevelResponse.json
--rw-r--r--   0        0        0     7613 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/SetNetworkProfileRequest.json
--rw-r--r--   0        0        0     1710 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/SetNetworkProfileResponse.json
--rw-r--r--   0        0        0     5959 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/SetVariableMonitoringRequest.json
--rw-r--r--   0        0        0     6923 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/SetVariableMonitoringResponse.json
--rw-r--r--   0        0        0     4272 2024-05-08 06:53:44.287794 duxcocpp-0.1.7/ocpp/v201/schemas/SetVariablesRequest.json
--rw-r--r--   0        0        0     5035 2024-05-08 06:53:44.291794 duxcocpp-0.1.7/ocpp/v201/schemas/SetVariablesResponse.json
--rw-r--r--   0        0        0     1481 2024-05-08 06:53:44.291794 duxcocpp-0.1.7/ocpp/v201/schemas/SignCertificateRequest.json
--rw-r--r--   0        0        0     1699 2024-05-08 06:53:44.291794 duxcocpp-0.1.7/ocpp/v201/schemas/SignCertificateResponse.json
--rw-r--r--   0        0        0     1570 2024-05-08 06:53:44.291794 duxcocpp-0.1.7/ocpp/v201/schemas/StatusNotificationRequest.json
--rw-r--r--   0        0        0      634 2024-05-08 06:53:44.291794 duxcocpp-0.1.7/ocpp/v201/schemas/StatusNotificationResponse.json
--rw-r--r--   0        0        0    14824 2024-05-08 06:53:44.291794 duxcocpp-0.1.7/ocpp/v201/schemas/TransactionEventRequest.json
--rw-r--r--   0        0        0     7606 2024-05-08 06:53:44.291794 duxcocpp-0.1.7/ocpp/v201/schemas/TransactionEventResponse.json
--rw-r--r--   0        0        0     1996 2024-05-08 06:53:44.291794 duxcocpp-0.1.7/ocpp/v201/schemas/TriggerMessageRequest.json
--rw-r--r--   0        0        0     1772 2024-05-08 06:53:44.291794 duxcocpp-0.1.7/ocpp/v201/schemas/TriggerMessageResponse.json
--rw-r--r--   0        0        0      970 2024-05-08 06:53:44.291794 duxcocpp-0.1.7/ocpp/v201/schemas/UnlockConnectorRequest.json
--rw-r--r--   0        0        0     1776 2024-05-08 06:53:44.291794 duxcocpp-0.1.7/ocpp/v201/schemas/UnlockConnectorResponse.json
--rw-r--r--   0        0        0      837 2024-05-08 06:53:44.291794 duxcocpp-0.1.7/ocpp/v201/schemas/UnpublishFirmwareRequest.json
--rw-r--r--   0        0        0     1059 2024-05-08 06:53:44.291794 duxcocpp-0.1.7/ocpp/v201/schemas/UnpublishFirmwareResponse.json
--rw-r--r--   0        0        0     2765 2024-05-08 06:53:44.291794 duxcocpp-0.1.7/ocpp/v201/schemas/UpdateFirmwareRequest.json
--rw-r--r--   0        0        0     1824 2024-05-08 06:53:44.291794 duxcocpp-0.1.7/ocpp/v201/schemas/UpdateFirmwareResponse.json
--rw-r--r--   0        0        0     1617 2024-05-08 06:53:44.291794 duxcocpp-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     6889 1970-01-01 00:00:00.000000 duxcocpp-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-05-08 07:08:44.888138 duxcocpp-0.2.2/LICENSE
+-rw-r--r--   0        0        0     6032 2024-05-08 07:08:44.888138 duxcocpp-0.2.2/README.rst
+-rw-r--r--   0        0        0        0 2024-05-08 07:08:45.044139 duxcocpp-0.2.2/ocpp/__init__.py
+-rw-r--r--   0        0        0    16259 2024-05-08 07:08:45.044139 duxcocpp-0.2.2/ocpp/charge_point.py
+-rw-r--r--   0        0        0     4451 2024-05-08 07:08:45.044139 duxcocpp-0.2.2/ocpp/exceptions.py
+-rw-r--r--   0        0        0      221 2024-05-08 07:08:45.044139 duxcocpp-0.2.2/ocpp/experimental/v21/README.rst
+-rw-r--r--   0        0        0    14821 2024-05-08 07:08:45.044139 duxcocpp-0.2.2/ocpp/messages.py
+-rw-r--r--   0        0        0     4106 2024-05-08 07:08:45.044139 duxcocpp-0.2.2/ocpp/routing.py
+-rw-r--r--   0        0        0      186 2024-05-08 07:08:45.044139 duxcocpp-0.2.2/ocpp/v16/__init__.py
+-rw-r--r--   0        0        0    20548 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/call.py
+-rw-r--r--   0        0        0    19232 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/call_result.py
+-rw-r--r--   0        0        0     3968 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/datatypes.py
+-rw-r--r--   0        0        0    23663 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/enums.py
+-rw-r--r--   0        0        0      306 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/Authorize.json
+-rw-r--r--   0        0        0     1062 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/AuthorizeResponse.json
+-rw-r--r--   0        0        0     1139 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/BootNotification.json
+-rw-r--r--   0        0        0      655 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/BootNotificationResponse.json
+-rw-r--r--   0        0        0      302 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/CancelReservation.json
+-rw-r--r--   0        0        0      423 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/CancelReservationResponse.json
+-rw-r--r--   0        0        0      352 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/CertificateSigned.json
+-rw-r--r--   0        0        0      505 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/CertificateSignedResponse.json
+-rw-r--r--   0        0        0      512 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/ChangeAvailability.json
+-rw-r--r--   0        0        0      453 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/ChangeAvailabilityResponse.json
+-rw-r--r--   0        0        0      418 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/ChangeConfiguration.json
+-rw-r--r--   0        0        0      491 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/ChangeConfigurationResponse.json
+-rw-r--r--   0        0        0      174 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/ClearCache.json
+-rw-r--r--   0        0        0      416 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/ClearCacheResponse.json
+-rw-r--r--   0        0        0      637 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/ClearChargingProfile.json
+-rw-r--r--   0        0        0      425 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/ClearChargingProfileResponse.json
+-rw-r--r--   0        0        0      466 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/DataTransfer.json
+-rw-r--r--   0        0        0      547 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/DataTransferResponse.json
+-rw-r--r--   0        0        0     1156 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/DeleteCertificate.json
+-rw-r--r--   0        0        0      523 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/DeleteCertificateResponse.json
+-rw-r--r--   0        0        0      491 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/DiagnosticsStatusNotification.json
+-rw-r--r--   0        0        0      194 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/DiagnosticsStatusNotificationResponse.json
+-rw-r--r--   0        0        0      760 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/ExtendedTriggerMessage.json
+-rw-r--r--   0        0        0      530 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/ExtendedTriggerMessageResponse.json
+-rw-r--r--   0        0        0      591 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/FirmwareStatusNotification.json
+-rw-r--r--   0        0        0      191 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/FirmwareStatusNotificationResponse.json
+-rw-r--r--   0        0        0      539 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/GetCompositeSchedule.json
+-rw-r--r--   0        0        0     2139 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/GetCompositeScheduleResponse.json
+-rw-r--r--   0        0        0      344 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/GetConfiguration.json
+-rw-r--r--   0        0        0     1066 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/GetConfigurationResponse.json
+-rw-r--r--   0        0        0      642 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/GetDiagnostics.json
+-rw-r--r--   0        0        0      275 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/GetDiagnosticsResponse.json
+-rw-r--r--   0        0        0      552 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/GetInstalledCertificateIds.json
+-rw-r--r--   0        0        0     1566 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/GetInstalledCertificateIdsResponse.json
+-rw-r--r--   0        0        0      183 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/GetLocalListVersion.json
+-rw-r--r--   0        0        0      301 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/GetLocalListVersionResponse.json
+-rw-r--r--   0        0        0     1184 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/GetLog.json
+-rw-r--r--   0        0        0      566 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/GetLogResponse.json
+-rw-r--r--   0        0        0      173 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/Heartbeat.json
+-rw-r--r--   0        0        0      325 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/HeartbeatResponse.json
+-rw-r--r--   0        0        0      639 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/InstallCertificate.json
+-rw-r--r--   0        0        0      526 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/InstallCertificateResponse.json
+-rw-r--r--   0        0        0      667 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/LogStatusNotification.json
+-rw-r--r--   0        0        0      173 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/LogStatusNotificationResponse.json
+-rw-r--r--   0        0        0     6758 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/MeterValues.json
+-rw-r--r--   0        0        0      176 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/MeterValuesResponse.json
+-rw-r--r--   0        0        0     4383 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/RemoteStartTransaction.json
+-rw-r--r--   0        0        0      428 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/RemoteStartTransactionResponse.json
+-rw-r--r--   0        0        0      306 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/RemoteStopTransaction.json
+-rw-r--r--   0        0        0      427 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/RemoteStopTransactionResponse.json
+-rw-r--r--   0        0        0      704 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/ReserveNow.json
+-rw-r--r--   0        0        0      502 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/ReserveNowResponse.json
+-rw-r--r--   0        0        0      398 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/Reset.json
+-rw-r--r--   0        0        0      411 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/ResetResponse.json
+-rw-r--r--   0        0        0      464 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/SecurityEventNotification.json
+-rw-r--r--   0        0        0      177 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/SecurityEventNotificationResponse.json
+-rw-r--r--   0        0        0     2146 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/SendLocalList.json
+-rw-r--r--   0        0        0      484 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/SendLocalListResponse.json
+-rw-r--r--   0        0        0     4310 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/SetChargingProfile.json
+-rw-r--r--   0        0        0      456 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/SetChargingProfileResponse.json
+-rw-r--r--   0        0        0      287 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/SignCertificate.json
+-rw-r--r--   0        0        0      483 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/SignCertificateResponse.json
+-rw-r--r--   0        0        0      876 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/SignedFirmwareStatusNotification.json
+-rw-r--r--   0        0        0      184 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/SignedFirmwareStatusNotificationResponse.json
+-rw-r--r--   0        0        0     1212 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/SignedUpdateFirmware.json
+-rw-r--r--   0        0        0      590 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/SignedUpdateFirmwareResponse.json
+-rw-r--r--   0        0        0      676 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/StartTransaction.json
+-rw-r--r--   0        0        0     1162 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/StartTransactionResponse.json
+-rw-r--r--   0        0        0     1805 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/StatusNotification.json
+-rw-r--r--   0        0        0      183 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/StatusNotificationResponse.json
+-rw-r--r--   0        0        0     7313 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/StopTransaction.json
+-rw-r--r--   0        0        0     1023 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/StopTransactionResponse.json
+-rw-r--r--   0        0        0      678 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/TriggerMessage.json
+-rw-r--r--   0        0        0      454 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/TriggerMessageResponse.json
+-rw-r--r--   0        0        0      296 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/UnlockConnector.json
+-rw-r--r--   0        0        0      457 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/UnlockConnectorResponse.json
+-rw-r--r--   0        0        0      572 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/UpdateFirmware.json
+-rw-r--r--   0        0        0      179 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v16/schemas/UpdateFirmwareResponse.json
+-rw-r--r--   0        0        0      189 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v201/__init__.py
+-rw-r--r--   0        0        0    34073 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v201/call.py
+-rw-r--r--   0        0        0    32301 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v201/call_result.py
+-rw-r--r--   0        0        0    22081 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v201/datatypes.py
+-rw-r--r--   0        0        0    80113 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v201/enums.py
+-rw-r--r--   0        0        0     4203 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v201/schemas/AuthorizeRequest.json
+-rw-r--r--   0        0        0     7208 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v201/schemas/AuthorizeResponse.json
+-rw-r--r--   0        0        0     3161 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v201/schemas/BootNotificationRequest.json
+-rw-r--r--   0        0        0     2270 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v201/schemas/BootNotificationResponse.json
+-rw-r--r--   0        0        0      775 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v201/schemas/CancelReservationRequest.json
+-rw-r--r--   0        0        0     1758 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v201/schemas/CancelReservationResponse.json
+-rw-r--r--   0        0        0     1914 2024-05-08 07:08:45.048139 duxcocpp-0.2.2/ocpp/v201/schemas/CertificateSignedRequest.json
+-rw-r--r--   0        0        0     1752 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/CertificateSignedResponse.json
+-rw-r--r--   0        0        0     1811 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/ChangeAvailabilityRequest.json
+-rw-r--r--   0        0        0     1783 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/ChangeAvailabilityResponse.json
+-rw-r--r--   0        0        0      634 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/ClearCacheRequest.json
+-rw-r--r--   0        0        0     1735 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/ClearCacheResponse.json
+-rw-r--r--   0        0        0     2574 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/ClearChargingProfileRequest.json
+-rw-r--r--   0        0        0     1752 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/ClearChargingProfileResponse.json
+-rw-r--r--   0        0        0      787 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/ClearDisplayMessageRequest.json
+-rw-r--r--   0        0        0     1735 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/ClearDisplayMessageResponse.json
+-rw-r--r--   0        0        0      865 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/ClearVariableMonitoringRequest.json
+-rw-r--r--   0        0        0     2327 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/ClearVariableMonitoringResponse.json
+-rw-r--r--   0        0        0     1087 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/ClearedChargingLimitRequest.json
+-rw-r--r--   0        0        0      634 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/ClearedChargingLimitResponse.json
+-rw-r--r--   0        0        0     1121 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/CostUpdatedRequest.json
+-rw-r--r--   0        0        0      634 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/CostUpdatedResponse.json
+-rw-r--r--   0        0        0     4659 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/CustomerInformationRequest.json
+-rw-r--r--   0        0        0     1740 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/CustomerInformationResponse.json
+-rw-r--r--   0        0        0     1101 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/DataTransferRequest.json
+-rw-r--r--   0        0        0     1869 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/DataTransferResponse.json
+-rw-r--r--   0        0        0     1808 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/DeleteCertificateRequest.json
+-rw-r--r--   0        0        0     1747 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/DeleteCertificateResponse.json
+-rw-r--r--   0        0        0     1539 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/FirmwareStatusNotificationRequest.json
+-rw-r--r--   0        0        0      634 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/FirmwareStatusNotificationResponse.json
+-rw-r--r--   0        0        0     1424 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/Get15118EVCertificateRequest.json
+-rw-r--r--   0        0        0     1915 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/Get15118EVCertificateResponse.json
+-rw-r--r--   0        0        0     1105 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/GetBaseReportRequest.json
+-rw-r--r--   0        0        0     1794 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/GetBaseReportResponse.json
+-rw-r--r--   0        0        0     1957 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/GetCertificateStatusRequest.json
+-rw-r--r--   0        0        0     2089 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/GetCertificateStatusResponse.json
+-rw-r--r--   0        0        0     3622 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/GetChargingProfilesRequest.json
+-rw-r--r--   0        0        0     1859 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/GetChargingProfilesResponse.json
+-rw-r--r--   0        0        0     1329 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/GetCompositeScheduleRequest.json
+-rw-r--r--   0        0        0     5095 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/GetCompositeScheduleResponse.json
+-rw-r--r--   0        0        0     1874 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/GetDisplayMessagesRequest.json
+-rw-r--r--   0        0        0     1841 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/GetDisplayMessagesResponse.json
+-rw-r--r--   0        0        0     1204 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/GetInstalledCertificateIdsRequest.json
+-rw-r--r--   0        0        0     3997 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/GetInstalledCertificateIdsResponse.json
+-rw-r--r--   0        0        0      634 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/GetLocalListVersionRequest.json
+-rw-r--r--   0        0        0      840 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/GetLocalListVersionResponse.json
+-rw-r--r--   0        0        0     2802 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/GetLogRequest.json
+-rw-r--r--   0        0        0     1954 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/GetLogResponse.json
+-rw-r--r--   0        0        0     4175 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/GetMonitoringReportRequest.json
+-rw-r--r--   0        0        0     1800 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/GetMonitoringReportResponse.json
+-rw-r--r--   0        0        0     4143 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/GetReportRequest.json
+-rw-r--r--   0        0        0     1800 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/GetReportResponse.json
+-rw-r--r--   0        0        0      784 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/GetTransactionStatusRequest.json
+-rw-r--r--   0        0        0      910 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/GetTransactionStatusResponse.json
+-rw-r--r--   0        0        0     3931 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/GetVariablesRequest.json
+-rw-r--r--   0        0        0     5581 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/GetVariablesResponse.json
+-rw-r--r--   0        0        0      634 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/HeartbeatRequest.json
+-rw-r--r--   0        0        0      802 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/HeartbeatResponse.json
+-rw-r--r--   0        0        0     1226 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/InstallCertificateRequest.json
+-rw-r--r--   0        0        0     1751 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/InstallCertificateResponse.json
+-rw-r--r--   0        0        0     1361 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/LogStatusNotificationRequest.json
+-rw-r--r--   0        0        0      634 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/LogStatusNotificationResponse.json
+-rw-r--r--   0        0        0     7709 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/MeterValuesRequest.json
+-rw-r--r--   0        0        0      634 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/MeterValuesResponse.json
+-rw-r--r--   0        0        0    11333 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/NotifyChargingLimitRequest.json
+-rw-r--r--   0        0        0      634 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/NotifyChargingLimitResponse.json
+-rw-r--r--   0        0        0     1542 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/NotifyCustomerInformationRequest.json
+-rw-r--r--   0        0        0      634 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/NotifyCustomerInformationResponse.json
+-rw-r--r--   0        0        0     6512 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/NotifyDisplayMessagesRequest.json
+-rw-r--r--   0        0        0      634 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/NotifyDisplayMessagesResponse.json
+-rw-r--r--   0        0        0     5943 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/NotifyEVChargingNeedsRequest.json
+-rw-r--r--   0        0        0     1870 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/NotifyEVChargingNeedsResponse.json
+-rw-r--r--   0        0        0    10370 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/NotifyEVChargingScheduleRequest.json
+-rw-r--r--   0        0        0     1780 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/NotifyEVChargingScheduleResponse.json
+-rw-r--r--   0        0        0     6614 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/NotifyEventRequest.json
+-rw-r--r--   0        0        0      634 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/NotifyEventResponse.json
+-rw-r--r--   0        0        0     7005 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/NotifyMonitoringReportRequest.json
+-rw-r--r--   0        0        0      634 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/NotifyMonitoringReportResponse.json
+-rw-r--r--   0        0        0     8608 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/NotifyReportRequest.json
+-rw-r--r--   0        0        0      634 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/NotifyReportResponse.json
+-rw-r--r--   0        0        0     1668 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/PublishFirmwareRequest.json
+-rw-r--r--   0        0        0     1691 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/PublishFirmwareResponse.json
+-rw-r--r--   0        0        0     1631 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/PublishFirmwareStatusNotificationRequest.json
+-rw-r--r--   0        0        0      634 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/PublishFirmwareStatusNotificationResponse.json
+-rw-r--r--   0        0        0    14700 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/ReportChargingProfilesRequest.json
+-rw-r--r--   0        0        0      634 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/ReportChargingProfilesResponse.json
+-rw-r--r--   0        0        0    15964 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/RequestStartTransactionRequest.json
+-rw-r--r--   0        0        0     2080 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/RequestStartTransactionResponse.json
+-rw-r--r--   0        0        0      844 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/RequestStopTransactionRequest.json
+-rw-r--r--   0        0        0     1760 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/RequestStopTransactionResponse.json
+-rw-r--r--   0        0        0     1133 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/ReservationStatusUpdateRequest.json
+-rw-r--r--   0        0        0      634 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/ReservationStatusUpdateResponse.json
+-rw-r--r--   0        0        0     3649 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/ReserveNowRequest.json
+-rw-r--r--   0        0        0     1758 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/ReserveNowResponse.json
+-rw-r--r--   0        0        0     1144 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/ResetRequest.json
+-rw-r--r--   0        0        0     1730 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/ResetResponse.json
+-rw-r--r--   0        0        0     1120 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/SecurityEventNotificationRequest.json
+-rw-r--r--   0        0        0      634 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/SecurityEventNotificationResponse.json
+-rw-r--r--   0        0        0     7733 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/SendLocalListRequest.json
+-rw-r--r--   0        0        0     1810 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/SendLocalListResponse.json
+-rw-r--r--   0        0        0    13730 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/SetChargingProfileRequest.json
+-rw-r--r--   0        0        0     1913 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/SetChargingProfileResponse.json
+-rw-r--r--   0        0        0     5989 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/SetDisplayMessageRequest.json
+-rw-r--r--   0        0        0     1848 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/SetDisplayMessageResponse.json
+-rw-r--r--   0        0        0     1005 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/SetMonitoringBaseRequest.json
+-rw-r--r--   0        0        0     1789 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/SetMonitoringBaseResponse.json
+-rw-r--r--   0        0        0     2087 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/SetMonitoringLevelRequest.json
+-rw-r--r--   0        0        0     1718 2024-05-08 07:08:45.052139 duxcocpp-0.2.2/ocpp/v201/schemas/SetMonitoringLevelResponse.json
+-rw-r--r--   0        0        0     7613 2024-05-08 07:08:45.056139 duxcocpp-0.2.2/ocpp/v201/schemas/SetNetworkProfileRequest.json
+-rw-r--r--   0        0        0     1710 2024-05-08 07:08:45.056139 duxcocpp-0.2.2/ocpp/v201/schemas/SetNetworkProfileResponse.json
+-rw-r--r--   0        0        0     5959 2024-05-08 07:08:45.056139 duxcocpp-0.2.2/ocpp/v201/schemas/SetVariableMonitoringRequest.json
+-rw-r--r--   0        0        0     6923 2024-05-08 07:08:45.056139 duxcocpp-0.2.2/ocpp/v201/schemas/SetVariableMonitoringResponse.json
+-rw-r--r--   0        0        0     4272 2024-05-08 07:08:45.056139 duxcocpp-0.2.2/ocpp/v201/schemas/SetVariablesRequest.json
+-rw-r--r--   0        0        0     5035 2024-05-08 07:08:45.056139 duxcocpp-0.2.2/ocpp/v201/schemas/SetVariablesResponse.json
+-rw-r--r--   0        0        0     1481 2024-05-08 07:08:45.056139 duxcocpp-0.2.2/ocpp/v201/schemas/SignCertificateRequest.json
+-rw-r--r--   0        0        0     1699 2024-05-08 07:08:45.056139 duxcocpp-0.2.2/ocpp/v201/schemas/SignCertificateResponse.json
+-rw-r--r--   0        0        0     1570 2024-05-08 07:08:45.056139 duxcocpp-0.2.2/ocpp/v201/schemas/StatusNotificationRequest.json
+-rw-r--r--   0        0        0      634 2024-05-08 07:08:45.056139 duxcocpp-0.2.2/ocpp/v201/schemas/StatusNotificationResponse.json
+-rw-r--r--   0        0        0    14824 2024-05-08 07:08:45.056139 duxcocpp-0.2.2/ocpp/v201/schemas/TransactionEventRequest.json
+-rw-r--r--   0        0        0     7606 2024-05-08 07:08:45.056139 duxcocpp-0.2.2/ocpp/v201/schemas/TransactionEventResponse.json
+-rw-r--r--   0        0        0     1996 2024-05-08 07:08:45.056139 duxcocpp-0.2.2/ocpp/v201/schemas/TriggerMessageRequest.json
+-rw-r--r--   0        0        0     1772 2024-05-08 07:08:45.056139 duxcocpp-0.2.2/ocpp/v201/schemas/TriggerMessageResponse.json
+-rw-r--r--   0        0        0      970 2024-05-08 07:08:45.056139 duxcocpp-0.2.2/ocpp/v201/schemas/UnlockConnectorRequest.json
+-rw-r--r--   0        0        0     1776 2024-05-08 07:08:45.056139 duxcocpp-0.2.2/ocpp/v201/schemas/UnlockConnectorResponse.json
+-rw-r--r--   0        0        0      837 2024-05-08 07:08:45.056139 duxcocpp-0.2.2/ocpp/v201/schemas/UnpublishFirmwareRequest.json
+-rw-r--r--   0        0        0     1059 2024-05-08 07:08:45.056139 duxcocpp-0.2.2/ocpp/v201/schemas/UnpublishFirmwareResponse.json
+-rw-r--r--   0        0        0     2765 2024-05-08 07:08:45.056139 duxcocpp-0.2.2/ocpp/v201/schemas/UpdateFirmwareRequest.json
+-rw-r--r--   0        0        0     1824 2024-05-08 07:08:45.056139 duxcocpp-0.2.2/ocpp/v201/schemas/UpdateFirmwareResponse.json
+-rw-r--r--   0        0        0     1617 2024-05-08 07:08:45.056139 duxcocpp-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6884 1970-01-01 00:00:00.000000 duxcocpp-0.2.2/PKG-INFO
```

### Comparing `duxcocpp-0.1.7/LICENSE` & `duxcocpp-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/README.rst` & `duxcocpp-0.2.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 Python package implementing the JSON version of the Open Charge Point Protocol
 (OCPP). Currently OCPP 1.6 (errata v4), OCPP 2.0 and OCPP 2.0.1 (Final Version)
 are supported.
 
 You can find the documentation on `rtd`_.
 
-
 Installation
 ------------
 
 You can either the project install from Pypi:
 
 .. code-block:: bash
 
@@ -31,16 +30,16 @@
 .. code-block:: bash
 
    $ pip install .
 
 Quick start
 -----------
 
-Below you can find examples on how to create a simple OCPP 2.0 central system as
-well as an OCPP 2.0 charge point.
+Below you can find examples on how to create a simple OCPP 1.6 or 2.0.1 Central
+Charging Station/Charge Point.
 
 .. note::
 
    To run these examples the dependency websockets_ is required! Install it by running:
 
    .. code-block:: bash
```

### Comparing `duxcocpp-0.1.7/ocpp/charge_point.py` & `duxcocpp-0.2.2/ocpp/charge_point.py`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/exceptions.py` & `duxcocpp-0.2.2/ocpp/exceptions.py`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/messages.py` & `duxcocpp-0.2.2/ocpp/messages.py`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/routing.py` & `duxcocpp-0.2.2/ocpp/routing.py`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/call.py` & `duxcocpp-0.2.2/ocpp/v16/call.py`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/call_result.py` & `duxcocpp-0.2.2/ocpp/v16/call_result.py`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/datatypes.py` & `duxcocpp-0.2.2/ocpp/v16/datatypes.py`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/enums.py` & `duxcocpp-0.2.2/ocpp/v16/enums.py`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/AuthorizeResponse.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/AuthorizeResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/BootNotification.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/BootNotification.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/BootNotificationResponse.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/BootNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/ChangeAvailability.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/ChangeAvailability.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/ClearChargingProfile.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/ClearChargingProfile.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/DataTransferResponse.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/DataTransferResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/DeleteCertificate.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/DeleteCertificate.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/DeleteCertificateResponse.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/DeleteCertificateResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/ExtendedTriggerMessage.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/ExtendedTriggerMessage.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/ExtendedTriggerMessageResponse.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/ExtendedTriggerMessageResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/FirmwareStatusNotification.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/FirmwareStatusNotification.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/GetCompositeSchedule.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/GetCompositeSchedule.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/GetCompositeScheduleResponse.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/GetCompositeScheduleResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/GetConfigurationResponse.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/GetConfigurationResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/GetDiagnostics.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/GetDiagnostics.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/GetInstalledCertificateIds.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/GetInstalledCertificateIds.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/GetInstalledCertificateIdsResponse.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/GetInstalledCertificateIdsResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/GetLog.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/GetLog.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/GetLogResponse.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/GetLogResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/InstallCertificate.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/InstallCertificate.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/InstallCertificateResponse.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/InstallCertificateResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/LogStatusNotification.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/LogStatusNotification.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/MeterValues.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/MeterValues.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/RemoteStartTransaction.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/RemoteStartTransaction.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/ReserveNow.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/ReserveNow.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/SendLocalList.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/SendLocalList.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/SetChargingProfile.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/SetChargingProfile.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/SignedFirmwareStatusNotification.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/SignedFirmwareStatusNotification.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/SignedUpdateFirmware.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/SignedUpdateFirmware.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/SignedUpdateFirmwareResponse.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/SignedUpdateFirmwareResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/StartTransaction.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/StartTransaction.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/StartTransactionResponse.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/StartTransactionResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/StatusNotification.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/StatusNotification.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/StopTransaction.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/StopTransaction.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/StopTransactionResponse.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/StopTransactionResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/TriggerMessage.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/TriggerMessage.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v16/schemas/UpdateFirmware.json` & `duxcocpp-0.2.2/ocpp/v16/schemas/UpdateFirmware.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/call.py` & `duxcocpp-0.2.2/ocpp/v201/call.py`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/call_result.py` & `duxcocpp-0.2.2/ocpp/v201/call_result.py`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/datatypes.py` & `duxcocpp-0.2.2/ocpp/v201/datatypes.py`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/enums.py` & `duxcocpp-0.2.2/ocpp/v201/enums.py`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/AuthorizeRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/AuthorizeRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/AuthorizeResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/AuthorizeResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/BootNotificationRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/BootNotificationRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/BootNotificationResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/BootNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/CancelReservationRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/CancelReservationRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/CancelReservationResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/CancelReservationResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/CertificateSignedRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/CertificateSignedRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/CertificateSignedResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/CertificateSignedResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/ChangeAvailabilityRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/ChangeAvailabilityRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/ChangeAvailabilityResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/ChangeAvailabilityResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/ClearCacheRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/ClearCacheRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/ClearCacheResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/ClearCacheResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/ClearChargingProfileRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/ClearChargingProfileRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/ClearChargingProfileResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/ClearChargingProfileResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/ClearDisplayMessageRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/ClearDisplayMessageRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/ClearDisplayMessageResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/ClearDisplayMessageResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/ClearVariableMonitoringRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/ClearVariableMonitoringRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/ClearVariableMonitoringResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/ClearVariableMonitoringResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/ClearedChargingLimitRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/ClearedChargingLimitRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/ClearedChargingLimitResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/ClearedChargingLimitResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/CostUpdatedRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/CostUpdatedRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/CostUpdatedResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/CostUpdatedResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/CustomerInformationRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/CustomerInformationRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/CustomerInformationResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/CustomerInformationResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/DataTransferRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/DataTransferRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/DataTransferResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/DataTransferResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/DeleteCertificateRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/DeleteCertificateRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/DeleteCertificateResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/DeleteCertificateResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/FirmwareStatusNotificationRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/FirmwareStatusNotificationRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/FirmwareStatusNotificationResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/FirmwareStatusNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/Get15118EVCertificateRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/Get15118EVCertificateRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/Get15118EVCertificateResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/Get15118EVCertificateResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/GetBaseReportRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/GetBaseReportRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/GetBaseReportResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/GetBaseReportResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/GetCertificateStatusRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/GetCertificateStatusRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/GetCertificateStatusResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/GetCertificateStatusResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/GetChargingProfilesRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/GetChargingProfilesRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/GetChargingProfilesResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/GetChargingProfilesResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/GetCompositeScheduleRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/GetCompositeScheduleRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/GetCompositeScheduleResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/GetCompositeScheduleResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/GetDisplayMessagesRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/GetDisplayMessagesRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/GetDisplayMessagesResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/GetDisplayMessagesResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/GetInstalledCertificateIdsRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/GetInstalledCertificateIdsRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/GetInstalledCertificateIdsResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/GetInstalledCertificateIdsResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/GetLocalListVersionRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/GetLocalListVersionRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/GetLocalListVersionResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/GetLocalListVersionResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/GetLogRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/GetLogRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/GetLogResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/GetLogResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/GetMonitoringReportRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/GetMonitoringReportRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/GetMonitoringReportResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/GetMonitoringReportResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/GetReportRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/GetReportRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/GetReportResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/GetReportResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/GetTransactionStatusRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/GetTransactionStatusRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/GetTransactionStatusResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/GetTransactionStatusResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/GetVariablesRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/GetVariablesRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/GetVariablesResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/GetVariablesResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/HeartbeatRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/HeartbeatRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/HeartbeatResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/HeartbeatResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/InstallCertificateRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/InstallCertificateRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/InstallCertificateResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/InstallCertificateResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/LogStatusNotificationRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/LogStatusNotificationRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/LogStatusNotificationResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/LogStatusNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/MeterValuesRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/MeterValuesRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/MeterValuesResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/MeterValuesResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/NotifyChargingLimitRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/NotifyChargingLimitRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/NotifyChargingLimitResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/NotifyChargingLimitResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/NotifyCustomerInformationRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/NotifyCustomerInformationRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/NotifyCustomerInformationResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/NotifyCustomerInformationResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/NotifyDisplayMessagesRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/NotifyDisplayMessagesRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/NotifyDisplayMessagesResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/NotifyDisplayMessagesResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/NotifyEVChargingNeedsRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/NotifyEVChargingNeedsRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/NotifyEVChargingNeedsResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/NotifyEVChargingNeedsResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/NotifyEVChargingScheduleRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/NotifyEVChargingScheduleRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/NotifyEVChargingScheduleResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/NotifyEVChargingScheduleResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/NotifyEventRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/NotifyEventRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/NotifyEventResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/NotifyEventResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/NotifyMonitoringReportRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/NotifyMonitoringReportRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/NotifyMonitoringReportResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/NotifyMonitoringReportResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/NotifyReportRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/NotifyReportRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/NotifyReportResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/NotifyReportResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/PublishFirmwareRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/PublishFirmwareRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/PublishFirmwareResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/PublishFirmwareResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/PublishFirmwareStatusNotificationRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/PublishFirmwareStatusNotificationRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/PublishFirmwareStatusNotificationResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/PublishFirmwareStatusNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/ReportChargingProfilesRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/ReportChargingProfilesRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/ReportChargingProfilesResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/ReportChargingProfilesResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/RequestStartTransactionRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/RequestStartTransactionRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/RequestStartTransactionResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/RequestStartTransactionResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/RequestStopTransactionRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/RequestStopTransactionRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/RequestStopTransactionResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/RequestStopTransactionResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/ReservationStatusUpdateRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/ReservationStatusUpdateRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/ReservationStatusUpdateResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/ReservationStatusUpdateResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/ReserveNowRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/ReserveNowRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/ReserveNowResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/ReserveNowResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/ResetRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/ResetRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/ResetResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/ResetResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/SecurityEventNotificationRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/SecurityEventNotificationRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/SecurityEventNotificationResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/SecurityEventNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/SendLocalListRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/SendLocalListRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/SendLocalListResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/SendLocalListResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/SetChargingProfileRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/SetChargingProfileRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/SetChargingProfileResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/SetChargingProfileResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/SetDisplayMessageRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/SetDisplayMessageRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/SetDisplayMessageResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/SetDisplayMessageResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/SetMonitoringBaseRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/SetMonitoringBaseRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/SetMonitoringBaseResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/SetMonitoringBaseResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/SetMonitoringLevelRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/SetMonitoringLevelRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/SetMonitoringLevelResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/SetMonitoringLevelResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/SetNetworkProfileRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/SetNetworkProfileRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/SetNetworkProfileResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/SetNetworkProfileResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/SetVariableMonitoringRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/SetVariableMonitoringRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/SetVariableMonitoringResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/SetVariableMonitoringResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/SetVariablesRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/SetVariablesRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/SetVariablesResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/SetVariablesResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/SignCertificateRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/SignCertificateRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/SignCertificateResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/SignCertificateResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/StatusNotificationRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/StatusNotificationRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/StatusNotificationResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/StatusNotificationResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/TransactionEventRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/TransactionEventRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/TransactionEventResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/TransactionEventResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/TriggerMessageRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/TriggerMessageRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/TriggerMessageResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/TriggerMessageResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/UnlockConnectorRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/UnlockConnectorRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/UnlockConnectorResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/UnlockConnectorResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/UnpublishFirmwareRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/UnpublishFirmwareRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/UnpublishFirmwareResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/UnpublishFirmwareResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/UpdateFirmwareRequest.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/UpdateFirmwareRequest.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/ocpp/v201/schemas/UpdateFirmwareResponse.json` & `duxcocpp-0.2.2/ocpp/v201/schemas/UpdateFirmwareResponse.json`

 * *Files identical despite different names*

### Comparing `duxcocpp-0.1.7/pyproject.toml` & `duxcocpp-0.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "duxcocpp"
-version = "0.1.7"
+version = "0.2.2"
 description = "Python package implementing the JSON version of the Open Charge Point Protocol (OCPP)."
 authors = [
 	"André Duarte <andre15x@gmail.com>",
 	"Auke Willem Oosterhoff <aukewillem.oosterhoff@mobilityhouse.com>",
 	"Greg Lutostanski <greg.luto@gmail.com>",
 	"Jared Newell <jared.newell@mobilityhouse.com>",
 	"Jonathan Herrmann <jonathan.herrmann@mobilityhouse.com>",
```

### Comparing `duxcocpp-0.1.7/PKG-INFO` & `duxcocpp-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duxcocpp
-Version: 0.1.7
+Version: 0.2.2
 Summary: Python package implementing the JSON version of the Open Charge Point Protocol (OCPP).
 Home-page: https://github.com/duxincai/ocpp
 License: MIT
 Author: André Duarte
 Author-email: andre15x@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -33,15 +33,14 @@
 
 Python package implementing the JSON version of the Open Charge Point Protocol
 (OCPP). Currently OCPP 1.6 (errata v4), OCPP 2.0 and OCPP 2.0.1 (Final Version)
 are supported.
 
 You can find the documentation on `rtd`_.
 
-
 Installation
 ------------
 
 You can either the project install from Pypi:
 
 .. code-block:: bash
 
@@ -52,16 +51,16 @@
 .. code-block:: bash
 
    $ pip install .
 
 Quick start
 -----------
 
-Below you can find examples on how to create a simple OCPP 2.0 central system as
-well as an OCPP 2.0 charge point.
+Below you can find examples on how to create a simple OCPP 1.6 or 2.0.1 Central
+Charging Station/Charge Point.
 
 .. note::
 
    To run these examples the dependency websockets_ is required! Install it by running:
 
    .. code-block:: bash
```

