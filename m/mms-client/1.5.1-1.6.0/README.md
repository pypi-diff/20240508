# Comparing `tmp/mms_client-1.5.1.tar.gz` & `tmp/mms_client-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mms_client-1.5.1.tar", max compression
+gzip compressed data, was "mms_client-1.6.0.tar", max compression
```

## Comparing `mms_client-1.5.1.tar` & `mms_client-1.6.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0     1211 2024-04-30 01:57:17.676666 mms_client-1.5.1/LICENSE
--rw-r--r--   0        0        0    14703 2024-04-30 01:57:17.676666 mms_client-1.5.1/README.md
--rw-r--r--   0        0        0     2913 2024-04-30 01:57:17.680666 mms_client-1.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/__init__.py
--rw-r--r--   0        0        0      676 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/client.py
--rw-r--r--   0        0        0        0 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/py.typed
--rw-r--r--   0        0        0    10702 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl
--rw-r--r--   0        0        0     9894 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/schemas/wsdl/omi-web-service.wsdl
--rw-r--r--   0        0        0   109679 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/schemas/xsd/mi-market.xsd
--rw-r--r--   0        0        0    76166 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd
--rw-r--r--   0        0        0    13276 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/schemas/xsd/mi-report.xsd
--rw-r--r--   0        0        0    69149 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/schemas/xsd/mpr.xsd
--rw-r--r--   0        0        0    31524 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/schemas/xsd/omi.xsd
--rw-r--r--   0        0        0        0 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/security/__init__.py
--rw-r--r--   0        0        0     1489 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/security/certs.py
--rw-r--r--   0        0        0     2149 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/security/crypto.py
--rw-r--r--   0        0        0        0 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/services/__init__.py
--rw-r--r--   0        0        0    25897 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/services/base.py
--rw-r--r--   0        0        0     7684 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/services/market.py
--rw-r--r--   0        0        0      626 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/services/omi.py
--rw-r--r--   0        0        0     3815 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/services/registration.py
--rw-r--r--   0        0        0      642 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/services/report.py
--rw-r--r--   0        0        0        0 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/types/__init__.py
--rw-r--r--   0        0        0    14139 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/types/award.py
--rw-r--r--   0        0        0     9710 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/types/base.py
--rw-r--r--   0        0        0     1629 2024-04-30 01:57:17.680666 mms_client-1.5.1/src/mms_client/types/enums.py
--rw-r--r--   0        0        0    14785 2024-04-30 01:57:17.684666 mms_client-1.5.1/src/mms_client/types/fields.py
--rw-r--r--   0        0        0     2706 2024-04-30 01:57:17.684666 mms_client-1.5.1/src/mms_client/types/market.py
--rw-r--r--   0        0        0     6791 2024-04-30 01:57:17.684666 mms_client-1.5.1/src/mms_client/types/offer.py
--rw-r--r--   0        0        0     1381 2024-04-30 01:57:17.684666 mms_client-1.5.1/src/mms_client/types/registration.py
--rw-r--r--   0        0        0    65974 2024-04-30 01:57:17.684666 mms_client-1.5.1/src/mms_client/types/resource.py
--rw-r--r--   0        0        0     4399 2024-04-30 01:57:17.684666 mms_client-1.5.1/src/mms_client/types/transport.py
--rw-r--r--   0        0        0        0 2024-04-30 01:57:17.684666 mms_client-1.5.1/src/mms_client/utils/__init__.py
--rw-r--r--   0        0        0     2057 2024-04-30 01:57:17.684666 mms_client-1.5.1/src/mms_client/utils/auditing.py
--rw-r--r--   0        0        0     2579 2024-04-30 01:57:17.684666 mms_client-1.5.1/src/mms_client/utils/errors.py
--rw-r--r--   0        0        0    29638 2024-04-30 01:57:17.684666 mms_client-1.5.1/src/mms_client/utils/serialization.py
--rw-r--r--   0        0        0    10156 2024-04-30 01:57:17.684666 mms_client-1.5.1/src/mms_client/utils/web.py
--rw-r--r--   0        0        0    15987 1970-01-01 00:00:00.000000 mms_client-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-05-08 04:45:03.930758 mms_client-1.6.0/LICENSE
+-rw-r--r--   0        0        0    14741 2024-05-08 04:45:03.930758 mms_client-1.6.0/README.md
+-rw-r--r--   0        0        0     2913 2024-05-08 04:45:03.930758 mms_client-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-08 04:45:03.930758 mms_client-1.6.0/src/mms_client/__init__.py
+-rw-r--r--   0        0        0      676 2024-05-08 04:45:03.930758 mms_client-1.6.0/src/mms_client/client.py
+-rw-r--r--   0        0        0        0 2024-05-08 04:45:03.930758 mms_client-1.6.0/src/mms_client/py.typed
+-rw-r--r--   0        0        0    10702 2024-05-08 04:45:03.930758 mms_client-1.6.0/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl
+-rw-r--r--   0        0        0     9894 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/schemas/wsdl/omi-web-service.wsdl
+-rw-r--r--   0        0        0   109679 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/schemas/xsd/mi-market.xsd
+-rw-r--r--   0        0        0    76166 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd
+-rw-r--r--   0        0        0    13276 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/schemas/xsd/mi-report.xsd
+-rw-r--r--   0        0        0    69149 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/schemas/xsd/mpr.xsd
+-rw-r--r--   0        0        0    31524 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/schemas/xsd/omi.xsd
+-rw-r--r--   0        0        0        0 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/security/__init__.py
+-rw-r--r--   0        0        0     1489 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/security/certs.py
+-rw-r--r--   0        0        0     2149 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/security/crypto.py
+-rw-r--r--   0        0        0        0 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/services/__init__.py
+-rw-r--r--   0        0        0    26309 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/services/base.py
+-rw-r--r--   0        0        0     9031 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/services/market.py
+-rw-r--r--   0        0        0      626 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/services/omi.py
+-rw-r--r--   0        0        0     3815 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/services/registration.py
+-rw-r--r--   0        0        0      642 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/services/report.py
+-rw-r--r--   0        0        0        0 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/types/__init__.py
+-rw-r--r--   0        0        0    14139 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/types/award.py
+-rw-r--r--   0        0        0     9710 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/types/base.py
+-rw-r--r--   0        0        0     1629 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/types/enums.py
+-rw-r--r--   0        0        0    14785 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/types/fields.py
+-rw-r--r--   0        0        0     2706 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/types/market.py
+-rw-r--r--   0        0        0     6791 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/types/offer.py
+-rw-r--r--   0        0        0     1381 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/types/registration.py
+-rw-r--r--   0        0        0     2667 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/types/reserve.py
+-rw-r--r--   0        0        0    65974 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/types/resource.py
+-rw-r--r--   0        0        0     4399 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/types/transport.py
+-rw-r--r--   0        0        0        0 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/utils/__init__.py
+-rw-r--r--   0        0        0     2057 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/utils/auditing.py
+-rw-r--r--   0        0        0     3005 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/utils/errors.py
+-rw-r--r--   0        0        0    29638 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/utils/serialization.py
+-rw-r--r--   0        0        0    10156 2024-05-08 04:45:03.934758 mms_client-1.6.0/src/mms_client/utils/web.py
+-rw-r--r--   0        0        0    16025 1970-01-01 00:00:00.000000 mms_client-1.6.0/PKG-INFO
```

### Comparing `mms_client-1.5.1/LICENSE` & `mms_client-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/README.md` & `mms_client-1.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -173,14 +173,15 @@
 client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, plugins=[TestAuditPlugin()])
 ```
 
 This same input allows for the user to create their own plugins and add them to the Zeep client, allowing for a certain amount of extensibility.
 
 # Completeness
 This client is not complete. Currently, it supports the following endpoints:
+- MarketQuery_ReserveRequirementQuery
 - MarketSubmit_OfferData
 - MarketQuery_OfferQuery
 - MarketCancel_OfferCancel
 - MarketQuery_AwardResultsQuery
 - RegistrationSubmit_Resource
 - RegistrationQuery_Resource
```

### Comparing `mms_client-1.5.1/pyproject.toml` & `mms_client-1.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mms_client"
-version = "v1.5.1"
+version = "v1.6.0"
 description = "API client for accessing the MMS"
 authors = ["Ryan Wood <ryan.wood@electroroute.co.jp>"]
 readme = "README.md"
 packages = [{ include = "mms_client", from = "src" }]
 homepage = "https://github.com/ElectroRoute-Japan/mms-client"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `mms_client-1.5.1/src/mms_client/client.py` & `mms_client-1.6.0/src/mms_client/client.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl` & `mms_client-1.6.0/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/src/mms_client/schemas/wsdl/omi-web-service.wsdl` & `mms_client-1.6.0/src/mms_client/schemas/wsdl/omi-web-service.wsdl`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/src/mms_client/schemas/xsd/mi-market.xsd` & `mms_client-1.6.0/src/mms_client/schemas/xsd/mi-market.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd` & `mms_client-1.6.0/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/src/mms_client/schemas/xsd/mi-report.xsd` & `mms_client-1.6.0/src/mms_client/schemas/xsd/mi-report.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/src/mms_client/schemas/xsd/mpr.xsd` & `mms_client-1.6.0/src/mms_client/schemas/xsd/mpr.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/src/mms_client/schemas/xsd/omi.xsd` & `mms_client-1.6.0/src/mms_client/schemas/xsd/omi.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/src/mms_client/security/certs.py` & `mms_client-1.6.0/src/mms_client/security/certs.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/src/mms_client/security/crypto.py` & `mms_client-1.6.0/src/mms_client/security/crypto.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/src/mms_client/services/base.py` & `mms_client-1.6.0/src/mms_client/services/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from mms_client.types.transport import MmsRequest
 from mms_client.types.transport import MmsResponse
 from mms_client.types.transport import RequestDataType
 from mms_client.types.transport import RequestType
 from mms_client.types.transport import ResponseDataType
 from mms_client.utils.errors import AudienceError
 from mms_client.utils.errors import MMSClientError
+from mms_client.utils.errors import MMSServerError
 from mms_client.utils.errors import MMSValidationError
 from mms_client.utils.serialization import Serializer
 from mms_client.utils.web import ClientType
 from mms_client.utils.web import Interface
 from mms_client.utils.web import Plugin
 from mms_client.utils.web import ZWrapper
 
@@ -455,15 +456,19 @@
         Arguments:
         resp (MmsResponse):     The MMS response to verify.
 
         Raises:
         MMSClientError: If the response is not valid.
         """
         # Verify that the response is in the correct format. If it's not, raise an error.
-        if resp.data_type != ResponseDataType.XML:
+        # NOTE: We're disabling the no-else-raise rule here because both comparisons are on the same enum so if one is
+        # removed then the other will raise an error. This is a false positive.
+        if resp.data_type == ResponseDataType.TXT:  # pylint: disable=no-else-raise
+            raise MMSServerError(config.name, resp.payload.decode("UTF-8"))
+        elif resp.data_type != ResponseDataType.XML:
             raise MMSClientError(
                 config.name,
                 f"Invalid MMS response data type: {resp.data_type.name}. Only XML is supported.",
             )
         if resp.compressed:
             raise MMSClientError(config.name, "Invalid MMS response. Compressed responses are not supported.")
```

### Comparing `mms_client-1.5.1/src/mms_client/services/market.py` & `mms_client-1.6.0/src/mms_client/services/market.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 from mms_client.types.market import MarketCancel
 from mms_client.types.market import MarketQuery
 from mms_client.types.market import MarketSubmit
 from mms_client.types.market import MarketType
 from mms_client.types.offer import OfferCancel
 from mms_client.types.offer import OfferData
 from mms_client.types.offer import OfferQuery
+from mms_client.types.reserve import ReserveRequirement
+from mms_client.types.reserve import ReserveRequirementQuery
 from mms_client.types.transport import RequestType
 from mms_client.utils.serialization import SchemaType
 from mms_client.utils.serialization import Serializer
 from mms_client.utils.web import ClientType
 from mms_client.utils.web import Interface
 
 # Set the default logger for the MMS client
@@ -30,14 +32,43 @@
 
 class MarketClientMixin:  # pylint: disable=unused-argument
     """Market client for the MMS server."""
 
     # The configuration for the market service
     config = ServiceConfiguration(Interface.MI, Serializer(SchemaType.MARKET, "MarketData"))
 
+    @mms_endpoint(
+        "MarketQuery_ReserveRequirementQuery",
+        config,
+        RequestType.INFO,
+        resp_envelope_type=MarketSubmit,
+        resp_data_type=ReserveRequirement,
+    )
+    def query_reserve_requirements(
+        self: ClientProto, request: ReserveRequirementQuery, date: Optional[Date] = None
+    ) -> List[ReserveRequirement]:
+        """Query the MMS server for reserve requirements.
+
+        This endpoint is accessible to all client types.
+
+        Arguments:
+        request (ReserveRequirementQuery):  The query to submit to the MMS server.
+        date (Date):                        The date of the transaction in the format "YYYY-MM-DD". This value defaults
+                                            to the current date.
+
+        Returns:    A list of reserve requirements that match the query.
+        """
+        # NOTE: The return type does not match the method definition but the decorator will return the correct type
+        return MarketQuery(  # type: ignore[return-value]
+            date=date or Date.today(),
+            participant=self.participant,
+            user=self.user,
+            days=1,
+        )
+
     @mms_endpoint("MarketSubmit_OfferData", config, RequestType.INFO, [ClientType.BSP])
     def put_offer(
         self: ClientProto, request: OfferData, market_type: MarketType, days: int, date: Optional[Date] = None
     ) -> OfferData:
         """Submit an offer to the MMS server.
 
         This endpoint is only accessible to BSPs.
@@ -120,14 +151,16 @@
 
         Arguments:
         request (OfferCancel):      The offer to cancel in the MMS server.
         market_type (MarketType):   The type of market for which the offer was submitted.
         days (int):                 The number of days ahead for which the data is being cancelled.
         date (Date):                The date of the transaction in the format "YYYY-MM-DD". This value defaults to the
                                     current date.
+
+        Returns:    Data identifying the offer that was cancelled.
         """
         # NOTE: The return type does not match the method definition but the decorator will return the correct type
         return MarketCancel(  # type: ignore[return-value]
             date=date or Date.today(),
             participant=self.participant,
             user=self.user,
             market_type=market_type,
```

### Comparing `mms_client-1.5.1/src/mms_client/services/omi.py` & `mms_client-1.6.0/src/mms_client/services/omi.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/src/mms_client/services/registration.py` & `mms_client-1.6.0/src/mms_client/services/registration.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/src/mms_client/services/report.py` & `mms_client-1.6.0/src/mms_client/services/report.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/src/mms_client/types/award.py` & `mms_client-1.6.0/src/mms_client/types/award.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/src/mms_client/types/base.py` & `mms_client-1.6.0/src/mms_client/types/base.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/src/mms_client/types/enums.py` & `mms_client-1.6.0/src/mms_client/types/enums.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/src/mms_client/types/fields.py` & `mms_client-1.6.0/src/mms_client/types/fields.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/src/mms_client/types/market.py` & `mms_client-1.6.0/src/mms_client/types/market.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/src/mms_client/types/offer.py` & `mms_client-1.6.0/src/mms_client/types/offer.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/src/mms_client/types/registration.py` & `mms_client-1.6.0/src/mms_client/types/registration.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/src/mms_client/types/resource.py` & `mms_client-1.6.0/src/mms_client/types/resource.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/src/mms_client/types/transport.py` & `mms_client-1.6.0/src/mms_client/types/transport.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/src/mms_client/utils/auditing.py` & `mms_client-1.6.0/src/mms_client/utils/auditing.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/src/mms_client/utils/errors.py` & `mms_client-1.6.0/src/mms_client/utils/errors.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,29 @@
         self.method = method
         self.message = f"{method}: Invalid client type, '{audience.name}' provided. Only {inner} supported."
         self.allowed = allowed
         self.audience = audience
         super().__init__(self.message)
 
 
+class MMSServerError(RuntimeError):
+    """Error raised when the MMS server returns an error."""
+
+    def __init__(self, method: str, message: str):
+        """Initialize the error.
+
+        Arguments:
+        method (str):   The method that caused the error.
+        message (str):  The error message.
+        """
+        super().__init__(f"{method}: {message}")
+        self.message = message
+        self.method = method
+
+
 class MMSClientError(RuntimeError):
     """Base class for MMS client errors."""
 
     def __init__(self, method: str, message: str):
         """Initialize the error.
 
         Arguments:
```

### Comparing `mms_client-1.5.1/src/mms_client/utils/serialization.py` & `mms_client-1.6.0/src/mms_client/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/src/mms_client/utils/web.py` & `mms_client-1.6.0/src/mms_client/utils/web.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.5.1/PKG-INFO` & `mms_client-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mms-client
-Version: 1.5.1
+Version: 1.6.0
 Summary: API client for accessing the MMS
 Home-page: https://github.com/ElectroRoute-Japan/mms-client
 Author: Ryan Wood
 Author-email: ryan.wood@electroroute.co.jp
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pydantic :: 2
@@ -205,14 +205,15 @@
 client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, plugins=[TestAuditPlugin()])
 ```
 
 This same input allows for the user to create their own plugins and add them to the Zeep client, allowing for a certain amount of extensibility.
 
 # Completeness
 This client is not complete. Currently, it supports the following endpoints:
+- MarketQuery_ReserveRequirementQuery
 - MarketSubmit_OfferData
 - MarketQuery_OfferQuery
 - MarketCancel_OfferCancel
 - MarketQuery_AwardResultsQuery
 - RegistrationSubmit_Resource
 - RegistrationQuery_Resource
```

