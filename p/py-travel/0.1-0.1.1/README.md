# Comparing `tmp/py_travel-0.1.tar.gz` & `tmp/py_travel-0.1.1.tar.gz`

## Comparing `py_travel-0.1.tar` & `py_travel-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,25 @@
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 py_travel-0.1/requirements.txt
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 py_travel-0.1/.github/workflows/commit.yml
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 py_travel-0.1/.github/workflows/linting.yml
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 py_travel-0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 py_travel-0.1/.idea/.gitignore
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 py_travel-0.1/.idea/misc.xml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 py_travel-0.1/.idea/modules.xml
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 py_travel-0.1/.idea/py-travel.iml
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 py_travel-0.1/.idea/vcs.xml
--rw-r--r--   0        0        0    25366 2020-02-02 00:00:00.000000 py_travel-0.1/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 py_travel-0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 py_travel-0.1/.idea/shelf/Uncommitted_changes_before_Checkout_at_06_05_2024_15_44__Changes_.xml
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 py_travel-0.1/.idea/shelf/Uncommitted_changes_before_Update_at_06_05_2024_15_57__Changes_.xml
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 py_travel-0.1/.idea/shelf/Uncommitted_changes_before_Update_at_06_05_2024_16_28__Changes_.xml
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 py_travel-0.1/.idea/shelf/Uncommitted_changes_before_Update_at_07_05_2024_12_07__Changes_.xml
--rw-r--r--   0        0        0    25558 2020-02-02 00:00:00.000000 py_travel-0.1/.idea/shelf/Uncommitted_changes_before_Checkout_at_06_05_2024_15_44_[Changes]/shelved.patch
--rw-r--r--   0        0        0    26875 2020-02-02 00:00:00.000000 py_travel-0.1/.idea/shelf/Uncommitted_changes_before_Update_at_06_05_2024_15_57_[Changes]/shelved.patch
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 py_travel-0.1/.idea/shelf/Uncommitted_changes_before_Update_at_06_05_2024_16_28_[Changes]/shelved.patch
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 py_travel-0.1/.idea/shelf/Uncommitted_changes_before_Update_at_07_05_2024_12_07_[Changes]/shelved.patch
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 py_travel-0.1/py_travel/__init__.py
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 py_travel-0.1/py_travel/client.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 py_travel-0.1/py_travel/exceptions.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 py_travel-0.1/py_travel/location.py
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 py_travel-0.1/py_travel/utils.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 py_travel-0.1/py_travel/vars.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 py_travel-0.1/py_travel/trip/__init__.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 py_travel-0.1/py_travel/trip/stop.py
--rw-r--r--   0        0        0    19329 2020-02-02 00:00:00.000000 py_travel-0.1/py_travel/trip/trip.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 py_travel-0.1/py_travel/trip/trip_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_travel-0.1/tests/__init__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 py_travel-0.1/tests/conftest.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 py_travel-0.1/tests/fixtures.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 py_travel-0.1/tests/mock_client.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 py_travel-0.1/tests/test_trip.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 py_travel-0.1/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 py_travel-0.1/LICENSE
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 py_travel-0.1/README.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 py_travel-0.1/pyproject.toml
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 py_travel-0.1/PKG-INFO
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 py_travel-0.1.1/requirements.txt
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 py_travel-0.1.1/.github/workflows/commit.yml
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 py_travel-0.1.1/.github/workflows/linting.yml
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 py_travel-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 py_travel-0.1.1/.github/workflows/upload.yml
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 py_travel-0.1.1/py_travel/__init__.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 py_travel-0.1.1/py_travel/client.py
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 py_travel-0.1.1/py_travel/exceptions.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 py_travel-0.1.1/py_travel/location.py
+-rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 py_travel-0.1.1/py_travel/utils.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 py_travel-0.1.1/py_travel/vars.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 py_travel-0.1.1/py_travel/trip/__init__.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 py_travel-0.1.1/py_travel/trip/stop.py
+-rw-r--r--   0        0        0    18805 2020-02-02 00:00:00.000000 py_travel-0.1.1/py_travel/trip/trip.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 py_travel-0.1.1/py_travel/trip/trip_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_travel-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 py_travel-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 py_travel-0.1.1/tests/fixtures.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 py_travel-0.1.1/tests/mock_client.py
+-rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 py_travel-0.1.1/tests/test_trip.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 py_travel-0.1.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 py_travel-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 py_travel-0.1.1/README.md
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 py_travel-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 py_travel-0.1.1/PKG-INFO
```

### Comparing `py_travel-0.1/py_travel/__init__.py` & `py_travel-0.1.1/py_travel/__init__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-"""
-Python Travel Library.
-
-This package tries to make it easier to use the Google Maps API for trip planning and a less JSON oriented way of
-working with the API.
-
-Modules:
-    trip: Provides the tools and classes used to interact with the Google Maps API for trip planning.
-
-Classes:
-    Client: Provides a wrapper for the googlemaps client class.
-
-    Location: Represents a location in the globe. Contains the coordinates and the address.
-
-    TravelWarnings: Collection of warnings raised by the trip class.
-
-Functions:
-    init_clients: Initializes all the library classes' clients with the ones provided by this library.
-
-Exceptions:
-    ClientNotInitializedError: Raised when no client capable of requesting the Google Maps API is found (Trip class).
-
-    InvalidResponseError: Raised when the API response does not contain some expected field or value (Trip class).
-
-    ApiError: Raised when the Google Maps API returns an error (Client subclasses).
-
-    LocationNotFoundError: Raised when the Google Maps API cannot find a location (Client subclasses).
-
-    InvalidRequestError: Raised when an invalid request is sent to the Google Maps API (Client subclasses).
-
-"""
-
-# Export client
-from .client import Client
-
-# Export exceptions
-from .exceptions import (
-    TravelWarnings, ClientNotInitializedError, InvalidResponseError, InvalidRequestError, ApiError,
-    LocationNotFoundError
-)
-
-# Export location
-from .location import Location
-
-# Export init_clients
-from .utils import init_clients
-
-__all__ = [
-    "TravelWarnings", "ClientNotInitializedError", "InvalidResponseError", "InvalidRequestError", "ApiError",
-    "LocationNotFoundError", "Client", "Location", "init_clients"
-]
+"""
+Python Travel Library.
+
+This package tries to make it easier to use the Google Maps API for trip planning and a less JSON oriented way of
+working with the API.
+
+Modules:
+    trip: Provides the tools and classes used to interact with the Google Maps API for trip planning.
+
+Classes:
+    Client: Provides a wrapper for the googlemaps client class.
+
+    Location: Represents a location in the globe. Contains the coordinates and the address.
+
+    TravelWarnings: Collection of warnings raised by the trip class.
+
+Functions:
+    init_clients: Initializes all the library classes' clients with the ones provided by this library.
+
+Exceptions:
+    ClientNotInitializedError: Raised when no client capable of requesting the Google Maps API is found (Trip class).
+
+    InvalidResponseError: Raised when the API response does not contain some expected field or value (Trip class).
+
+    ApiError: Raised when the Google Maps API returns an error (Client subclasses).
+
+    LocationNotFoundError: Raised when the Google Maps API cannot find a location (Client subclasses).
+
+    InvalidRequestError: Raised when an invalid request is sent to the Google Maps API (Client subclasses).
+
+"""
+
+# Export client
+from .client import Client
+
+# Export exceptions
+from .exceptions import (
+    TravelWarnings, ClientNotInitializedError, InvalidResponseError, InvalidRequestError, ApiError,
+    LocationNotFoundError
+)
+
+# Export location
+from .location import Location
+
+# Export init_clients
+from .utils import init_clients
+
+__all__ = [
+    "TravelWarnings", "ClientNotInitializedError", "InvalidResponseError", "InvalidRequestError", "ApiError",
+    "LocationNotFoundError", "Client", "Location", "init_clients"
+]
```

### Comparing `py_travel-0.1/py_travel/client.py` & `py_travel-0.1.1/py_travel/client.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-from typing import Tuple, TYPE_CHECKING, List, Dict
-from googlemaps.exceptions import ApiError as GoogleMapsApiError
-from googlemaps.client import Client as GoogleMapsClient
-from py_travel.exceptions import LocationNotFoundError, ApiError, InvalidRequestError
-
-if TYPE_CHECKING:  # pragma: no cover
-    from datetime import datetime
-
-
-class Client:
-    """
-    Base Client Class for all Google Maps API clients
-
-    Attributes:
-        client: Google Maps API client (class attribute)
-    """
-    def __init__(self, api_key: str) -> None:
-        self.__client = GoogleMapsClient(key=api_key)
-
-    @property
-    def client(self) -> GoogleMapsClient:
-        return self.__client
-
-    @client.setter
-    def client(self, api_key: str) -> None:
-        """
-        Set Google Maps Client
-
-        :param api_key: API key for Google Maps
-        """
-        self.client = GoogleMapsClient(key=api_key)
-
-    def directions(
-            self,
-            origin: Tuple[float, float] | str,
-            destination: Tuple[float, float] | str,
-            departure_time: 'datetime' = None,
-            arrival_time: 'datetime' = None,
-            mode: str = None,
-            avoid: str = None,
-            units: str = None,
-            transit_mode: List[str] | str = None,
-            transit_routing_preference: str = None,
-            traffic_model: str = None
-    ) -> Dict:
-        """
-        Directions API method
-
-        Information about the parameters can be found here:
-        https://googlemaps.github.io/google-maps-services-python/docs/index.html#googlemaps.Client.directions
-
-        :return: The Google Maps Directions API response
-        """
-
-        try:
-            response = self.__client.directions(
-                origin=origin,
-                destination=destination,
-                departure_time=departure_time,
-                arrival_time=arrival_time,
-                mode=mode,
-                avoid=avoid,
-                units=units,
-                transit_mode=transit_mode,
-                transit_routing_preference=transit_routing_preference,
-                traffic_model=traffic_model
-            )
-        except GoogleMapsApiError as e:
-            if e.status == "NOT_FOUND":
-                raise LocationNotFoundError() from None
-            elif e.status == "INVALID_REQUEST":
-                raise InvalidRequestError(e.message) from None
-            else:
-                raise ApiError(e.status, e.message) from None
-
-        return response
-
+from typing import Tuple, TYPE_CHECKING, List, Dict
+from googlemaps.exceptions import ApiError as GoogleMapsApiError
+from googlemaps.client import Client as GoogleMapsClient
+from py_travel.exceptions import LocationNotFoundError, ApiError, InvalidRequestError
+
+if TYPE_CHECKING:  # pragma: no cover
+    from datetime import datetime
+
+
+class Client:
+    """
+    Base Client Class for all Google Maps API clients
+
+    Attributes:
+        client: Google Maps API client (class attribute)
+    """
+    def __init__(self, api_key: str) -> None:
+        self.__client = GoogleMapsClient(key=api_key)
+
+    @property
+    def client(self) -> GoogleMapsClient:
+        return self.__client
+
+    @client.setter
+    def client(self, api_key: str) -> None:
+        """
+        Set Google Maps Client
+
+        :param api_key: API key for Google Maps
+        """
+        self.client = GoogleMapsClient(key=api_key)
+
+    def directions(
+            self,
+            origin: Tuple[float, float] | str,
+            destination: Tuple[float, float] | str,
+            departure_time: 'datetime' = None,
+            arrival_time: 'datetime' = None,
+            mode: str = None,
+            avoid: str = None,
+            units: str = None,
+            transit_mode: List[str] | str = None,
+            transit_routing_preference: str = None,
+            traffic_model: str = None
+    ) -> Dict:
+        """
+        Directions API method
+
+        Information about the parameters can be found here:
+        https://googlemaps.github.io/google-maps-services-python/docs/index.html#googlemaps.Client.directions
+
+        :return: The Google Maps Directions API response
+        """
+
+        try:
+            response = self.__client.directions(
+                origin=origin,
+                destination=destination,
+                departure_time=departure_time,
+                arrival_time=arrival_time,
+                mode=mode,
+                avoid=avoid,
+                units=units,
+                transit_mode=transit_mode,
+                transit_routing_preference=transit_routing_preference,
+                traffic_model=traffic_model
+            )
+        except GoogleMapsApiError as e:
+            if e.status == "NOT_FOUND":
+                raise LocationNotFoundError() from None
+            elif e.status == "INVALID_REQUEST":
+                raise InvalidRequestError(e.message) from None
+            else:
+                raise ApiError(e.status, e.message) from None
+
+        return response
+
```

### Comparing `py_travel-0.1/py_travel/exceptions.py` & `py_travel-0.1.1/py_travel/exceptions.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-"""
-Exceptions and warnings raised by the package
-"""
-
-import warnings
-
-
-class TravelWarnings:
-    """
-    Class wrapping all warnings raised by the Trip class
-    """
-
-    @staticmethod
-    def ignore_field(field: str, message: str) -> None:
-        """
-        Warning raised when a field is ignored by a method
-
-        :param field: Ignored field name
-        :param message: Message to display
-        """
-
-        warn_message = f"IGNORED FIELD '{field}': {message}"
-        warnings.warn(warn_message, UserWarning, stacklevel=3)
-
-    @staticmethod
-    def update_date(date_name: str, message: str) -> None:
-        """
-        Warning raised when a date is automatically updated by a method
-        :param date_name: Field date name
-        :param message: Message to display
-        """
-
-        warn_message = f"UPDATED {date_name.upper()} DATE: {message}"
-        warnings.warn(warn_message, UserWarning, stacklevel=3)
-
-
-class ClientNotInitializedError(Exception):
-    """Exception raised when the Google Maps API client has not been initialized
-
-    Attributes:
-        message: Explanation of the exception (optional)
-
-    """
-
-    def __init__(self, message: str = "Client not initialized") -> None:
-        self.message = message
-        super().__init__(self.message)
-
-
-class InvalidResponseError(Exception):
-    """Exception raised when the Google Maps API response does not contain the expected fields
-
-    Attributes:
-        field: Missing field
-        message: Explanation of the exception (optional)
-    """
-
-    def __init__(self, field: str, message: str = "Invalid API response") -> None:
-        self.field = field
-        self.message = message
-        super().__init__(self.message)
-
-
-class ApiError(Exception):
-    """Exception raised when the Google Maps API fails
-
-    Attributes:
-        status: Error status of the API call (optional)
-        message: Explanation of the exception (optional)
-    """
-
-    def __init__(self, status: str = None, message: str = None) -> None:
-        self.status = "Unknown error" if not status else status
-        self.message = "An API error occurred" if not message else message
-        super().__init__(f"{self.status}: {self.message}")
-
-
-class LocationNotFoundError(Exception):
-    """Exception raised when the Google Maps API cannot find a location
-
-    Attributes:
-        message: Explanation of the exception (optional)
-    """
-
-    def __init__(self, message: str = "Location not found") -> None:
-        self.message = message
-        super().__init__(self.message)
-
-
-class InvalidRequestError(Exception):
-    """Exception raised when an invalid request is sent to the Google Maps API
-    Attributes:
-        message: Explanation of the exception (optional)
-    """
-
-    def __init__(self, message: str = "Request was invalid, check parameters") -> None:
-        self.message = message
-        super().__init__(f"Invalid API request: {self.message}")
+"""
+Exceptions and warnings raised by the package
+"""
+
+import warnings
+
+
+class TravelWarnings:
+    """
+    Class wrapping all warnings raised by the Trip class
+    """
+
+    @staticmethod
+    def ignore_field(field: str, message: str) -> None:
+        """
+        Warning raised when a field is ignored by a method
+
+        :param field: Ignored field name
+        :param message: Message to display
+        """
+
+        warn_message = f"IGNORED FIELD '{field}': {message}"
+        warnings.warn(warn_message, UserWarning, stacklevel=3)
+
+    @staticmethod
+    def update_date(date_name: str, message: str) -> None:
+        """
+        Warning raised when a date is automatically updated by a method
+        :param date_name: Field date name
+        :param message: Message to display
+        """
+
+        warn_message = f"UPDATED {date_name.upper()} DATE: {message}"
+        warnings.warn(warn_message, UserWarning, stacklevel=3)
+
+
+class ClientNotInitializedError(Exception):
+    """Exception raised when the Google Maps API client has not been initialized
+
+    Attributes:
+        message: Explanation of the exception (optional)
+
+    """
+
+    def __init__(self, message: str = "Client not initialized") -> None:
+        self.message = message
+        super().__init__(self.message)
+
+
+class InvalidResponseError(Exception):
+    """Exception raised when the Google Maps API response does not contain the expected fields
+
+    Attributes:
+        field: Missing field
+        message: Explanation of the exception (optional)
+    """
+
+    def __init__(self, field: str, message: str = "Invalid API response") -> None:
+        self.field = field
+        self.message = message
+        super().__init__(self.message)
+
+
+class ApiError(Exception):
+    """Exception raised when the Google Maps API fails
+
+    Attributes:
+        status: Error status of the API call (optional)
+        message: Explanation of the exception (optional)
+    """
+
+    def __init__(self, status: str = None, message: str = None) -> None:
+        self.status = "Unknown error" if not status else status
+        self.message = "An API error occurred" if not message else message
+        super().__init__(f"{self.status}: {self.message}")
+
+
+class LocationNotFoundError(Exception):
+    """Exception raised when the Google Maps API cannot find a location
+
+    Attributes:
+        message: Explanation of the exception (optional)
+    """
+
+    def __init__(self, message: str = "Location not found") -> None:
+        self.message = message
+        super().__init__(self.message)
+
+
+class InvalidRequestError(Exception):
+    """Exception raised when an invalid request is sent to the Google Maps API
+    Attributes:
+        message: Explanation of the exception (optional)
+    """
+
+    def __init__(self, message: str = "Request was invalid, check parameters") -> None:
+        self.message = message
+        super().__init__(f"Invalid API request: {self.message}")
```

### Comparing `py_travel-0.1/py_travel/location.py` & `py_travel-0.1.1/py_travel/location.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-"""
-Location class.
-
-Classes:
-    Location: Represents a location in the globe.
-
-Functions:
-    input_to_location: Transforms a coordinates tuple or an address into a Location object.
-"""
-
-from dataclasses import dataclass
-from typing import Tuple
-
-
-@dataclass
-class Location:
-    """
-    Represents a location in the globe
-
-    Attributes:
-        lat: Latitude of the location (optional)
-        lng: Longitude of the location (optional)
-        address: Address of the location with that coordinates (optional)
-    """
-
-    lat: float | None = None
-    lng: float | None = None
-    address: str | None = None
-
-    @property
-    def coords(self) -> Tuple[float, float] | None:
-        """
-        Returns the coordinates of the location if it has them
-
-        :return: The latitude and longitude of the location as a tuple
-        """
-        if self.lat and self.lng:
-            return self.lat, self.lng
-        else:
-            return None
-
-    def get_data(self) -> Tuple[float, float] | str:
-        """
-        Yields the most precise data available for the location.
-
-        :return: The coordinates if they are present, otherwise the address
-        """
-        return self.coords if self.coords else self.address
-
-
-def input_to_location(data: Tuple[float, float] | str | Location) -> Location:
-    """
-    Converts a given 'Location' into a location object
-
-    :param data: Tuple with (latitude, longitude), string address or Location object
-    :return: A Location object from the given data
-    """
-    if isinstance(data, Location):
-        return data
-    if isinstance(data, str):
-        return Location(address=data)
-    if isinstance(data, tuple):
-        return Location(lat=data[0], lng=data[1])
-    else:
-        raise TypeError("Argument must be a string or a tuple containing two floats")
+"""
+Location class.
+
+Classes:
+    Location: Represents a location in the globe.
+
+Functions:
+    input_to_location: Transforms a coordinates tuple or an address into a Location object.
+"""
+
+from dataclasses import dataclass
+from typing import Tuple
+
+
+@dataclass
+class Location:
+    """
+    Represents a location in the globe
+
+    Attributes:
+        lat: Latitude of the location (optional)
+        lng: Longitude of the location (optional)
+        address: Address of the location with that coordinates (optional)
+    """
+
+    lat: float | None = None
+    lng: float | None = None
+    address: str | None = None
+
+    @property
+    def coords(self) -> Tuple[float, float] | None:
+        """
+        Returns the coordinates of the location if it has them
+
+        :return: The latitude and longitude of the location as a tuple
+        """
+        if self.lat and self.lng:
+            return self.lat, self.lng
+        else:
+            return None
+
+    def get_data(self) -> Tuple[float, float] | str:
+        """
+        Yields the most precise data available for the location.
+
+        :return: The coordinates if they are present, otherwise the address
+        """
+        return self.coords if self.coords else self.address
+
+
+def input_to_location(data: Tuple[float, float] | str | Location) -> Location:
+    """
+    Converts a given 'Location' into a location object
+
+    :param data: Tuple with (latitude, longitude), string address or Location object
+    :return: A Location object from the given data
+    """
+    if isinstance(data, Location):
+        return data
+    if isinstance(data, str):
+        return Location(address=data)
+    if isinstance(data, tuple):
+        return Location(lat=data[0], lng=data[1])
+    else:
+        raise TypeError("Argument must be a string or a tuple containing two floats")
```

### Comparing `py_travel-0.1/py_travel/vars.py` & `py_travel-0.1.1/py_travel/vars.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-"""
-Global constants used throughout the package
-"""
-from typing import Literal
-
-METERS_IN_MILE = 1609.344  # Meters in a mile
-
-TRIP_MODES = Literal["driving", "walking", "bicycling", "transit"]  # Trip modes
-AVOID_FEATURES = Literal["tolls", "highways", "ferries", "indoor"]  # Road features to avoid
-TRANSIT_MODES = Literal["bus", "subway", "train", "tram", "rail"]  # Transit modes
-TRANSIT_PREFERENCES = Literal["less_walking", "fewer_transfers"]  # Transit preferences
-TRAFFIC_MODE = Literal["best_guess", "optimistic", "pessimistic"]  # Traffic model
-METRIC_SYSTEMS = Literal["metric", "imperial"]  # Metric system
+"""
+Global constants used throughout the package
+"""
+from typing import Literal
+
+METERS_IN_MILE = 1609.344  # Meters in a mile
+
+TRIP_MODES = Literal["driving", "walking", "bicycling", "transit"]  # Trip modes
+AVOID_FEATURES = Literal["tolls", "highways", "ferries", "indoor"]  # Road features to avoid
+TRANSIT_MODES = Literal["bus", "subway", "train", "tram", "rail"]  # Transit modes
+TRANSIT_PREFERENCES = Literal["less_walking", "fewer_transfers"]  # Transit preferences
+TRAFFIC_MODE = Literal["best_guess", "optimistic", "pessimistic"]  # Traffic model
+METRIC_SYSTEMS = Literal["metric", "imperial"]  # Metric system
```

### Comparing `py_travel-0.1/py_travel/trip/trip.py` & `py_travel-0.1.1/py_travel/trip/trip.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,524 +1,524 @@
-from datetime import datetime, date, timedelta
-from typing import Tuple, List, Dict, Any
-
-from py_travel.exceptions import ClientNotInitializedError, TravelWarnings, InvalidResponseError
-from py_travel.location import Location, input_to_location
-from py_travel.utils import meters_to_miles, get_distance, get_duration, get_steps, calculate_stage_steps
-from .trip_config import TripConfig
-from .stop import Stop
-
-
-class Trip:
-    """
-    Trip class
-
-    Attributes:
-        client: Client object for the Google Maps API calls
-        origin: Origin of the trip
-        destination: Destination of the trip
-        departure_date: Start date of the trip
-        arrival_date: End date of the trip
-        stops: List of stops associated with the trip
-        updated: Boolean indicating if the object needs to call the Google Maps API to get the results
-        api_response: Raw Google Maps API response
-    """
-
-    client: Any = None
-
-    def __init__(
-        self,
-        origin: Tuple[float, float] | str | Location,
-        destination: Tuple[float, float] | str | Location,
-        stops: List[Tuple[Tuple[float, float] | str | Location, datetime]] = None,
-        departure_date: datetime = None,
-        arrival_date: datetime = None,
-        config: TripConfig = None,
-    ) -> None:
-        """
-        Initialize Trip object
-
-        :param origin: Origin of the trip in pair (latitude, longitude) or address or Location object
-        :param destination: Destination of the trip in pair (latitude, longitude) or address or Location object
-        :param stops: A list of tuples containing the stop location (either a tuple containing the coordinates, the
-            address or a Location object) and the departure date from the stop
-        :param departure_date: Start date of the trip (optional)
-        :param arrival_date: End date of the trip (optional)
-        :param config: Trip configuration either as a dictionary or as a TripConfig object (optional)
-        """
-
-        self.__origin = input_to_location(origin)
-        self.__destination = input_to_location(destination)
-
-        self.__stops = (
-            [Stop(input_to_location(loc), dep_date) for loc, dep_date in stops]
-            if stops
-            else []
-        )
-        self.__stops.sort(key=lambda stop: stop.departure_date)
-
-        self.__departure_date = departure_date
-        self.__arrival_date = arrival_date
-
-        self.__config = config if config else {}
-
-        self.__api_response: Dict = {}
-        self.__updated = True
-
-    @property
-    def origin(self) -> Location:
-        """
-        :return: The origin location of the trip
-        """
-        return self.__origin
-
-    @origin.setter
-    def origin(self, new_origin: Tuple[float, float] | str | Location) -> None:
-        """
-        Sets the origin location of the trip
-
-        Warning: This will mark the trip as updated, possibly causing calls to the Google Maps API in the future.
-
-        :param new_origin: Origin of the trip in pair (latitude, longitude), string with address or Location object
-        """
-        self.__origin = input_to_location(new_origin)
-        self.__updated = True
-
-    @property
-    def destination(self) -> Location:
-        """
-        :return: The destination location of the trip
-        """
-        return self.__destination
-
-    @destination.setter
-    def destination(
-        self, new_destination: Tuple[float, float] | str | Location
-    ) -> None:
-        """
-        Sets the destination location of the trip
-
-        Warning: This will mark the trip as updated, possibly causing calls to the Google Maps API in the future.
-
-        :param new_destination: Destination of the trip in pair (latitude, longitude), string with address or Location
-            object
-        """
-        self.__destination = input_to_location(new_destination)
-        self.__updated = True
-
-    @property
-    def stops(self) -> List[Stop]:
-        """
-        :return: The list of stops
-        """
-        return self.__stops
-
-    @stops.setter
-    def stops(
-        self, stops: List[Tuple[Tuple[float, float] | str | Location, datetime]] | List[Stop]
-    ) -> None:
-        """
-        Sets the stops for the trip
-
-        Warning: This will mark the trip as updated, possibly causing calls to the Google Maps API in the future.
-
-        :param stops: A list of tuples containing the stop location (either a tuple containing the coordinates, the
-            address or a Location object) and the departure date from the stop, or a list of Stop objects
-        """
-
-        self.__stops = []
-        for stop in stops:
-            if isinstance(stop, Stop):
-                self.__stops.append(stop)
-            else:
-                self.__stops.append(Stop(input_to_location(stop[0]), stop[1]))
-
-        self.__stops.sort(key=lambda s: s.departure_date)
-        self.__updated = True
-
-    @property
-    def departure_date(self) -> datetime:
-        """
-        :return: The departure date of the trip
-        """
-        return self.__departure_date
-
-    @departure_date.setter
-    def departure_date(self, new_departure_date: datetime) -> None:
-        """
-        Sets the departure date of the trip
-
-        Warning: This will mark the trip as updated, possibly causing calls to the Google Maps API in the future.
-
-        :param new_departure_date: The departure date of the trip
-        """
-        self.__departure_date = new_departure_date
-        self.__updated = True
-
-    @property
-    def arrival_date(self) -> datetime:
-        """
-        :return: The arrival date of the trip
-        """
-        return self.__arrival_date
-
-    @arrival_date.setter
-    def arrival_date(self, new_arrival_date: datetime) -> None:
-        """
-        Sets the arrival date of the trip
-
-        Warning: This will mark the trip as updated, possibly causing calls to the Google Maps API in the future.
-
-        :param new_arrival_date: The arrival date of the trip
-        """
-        self.__arrival_date = new_arrival_date
-        self.__updated = True
-
-    @property
-    def config(self) -> TripConfig:
-        """
-        :return: The configuration parameters of the trip
-        """
-        return self.__config
-
-    @config.setter
-    def config(self, new_config: TripConfig) -> None:
-        """
-        Set the configuration for the calculations
-
-        Warning: This method will mark the trip as updated, possibly causing calls to the Google Maps API in the future.
-
-        :param new_config: Trip configuration
-        """
-
-        self.__config = new_config
-        self.__updated = True
-
-    @property
-    def api_response(self) -> Dict:
-        """
-        :return: The response from the Google Maps API
-        """
-        return self.__api_response
-
-    @property
-    def distance(self) -> float:
-        """
-        Warning: If the trip is marked as updated, it will first calculate the trip
-        :return: The total distance of the trip in the unit given in the config ('metric' if not configured).
-        """
-
-        if self.__updated:
-            self.calculate_trip()
-
-        if self.__stops:
-            meters = sum(get_distance(stage) for stage in self.__api_response.values())
-        else:
-            meters = get_distance(self.__api_response)
-
-        return (
-            meters / 1000
-            if self.__config.get("units", "metric") == "metric"
-            else meters_to_miles(meters)
-        )
-
-    @property
-    def seconds(self) -> int:
-        """
-        Warning: If the trip is marked as updated, it will first calculate the trip
-        :return: The amount of seconds travelled in the trip
-        """
-
-        if self.__updated:
-            self.calculate_trip()
-
-        if self.__stops:
-            seconds = sum(get_duration(stage) for stage in self.__api_response.values())
-        else:
-            seconds = get_duration(self.__api_response)
-
-        return seconds
-
-    @property
-    def days(self) -> int:
-        """
-        Warning: If the trip is marked as updated, it will first calculate the trip
-        :return: Duration in days of the trip (rounded up)
-        """
-
-        if self.__updated:
-            self.calculate_trip()  # This will call update_dates()
-
-        return (self.__arrival_date.date() - self.__departure_date.date()).days + 1
-
-    @property
-    def stages_distances(self) -> List[float]:
-        """
-        Returns the distances between the locations of the trip in a list starting from origin - 1st stop and ending
-        with last stop - destination. If the trip does not contain stops, the list will be of size 1.
-
-        Warning: If the trip is marked as updated, it will first calculate the trip
-
-        :return: A list of distances between the locations of the trip in order
-        """
-
-        if self.__updated:
-            self.calculate_trip()
-
-        distances: List[float] = []
-        if self.__stops:
-            for stage in self.__api_response.values():
-                stage_meters = (
-                    stage.get("legs", [{}])[0].get("distance", {}).get("value", None)
-                )
-                if not stage_meters:
-                    raise InvalidResponseError("legs[0].distance.value")
-
-                distances.append(stage_meters)
-        else:
-            meters = (
-                self.__api_response.get("legs", [{}])[0]
-                .get("distance", {})
-                .get("value", None)
-            )
-            if not meters:
-                raise InvalidResponseError("legs[0].distance.value")
-            distances.append(meters)
-
-        return [
-            (
-                distance / 1000
-                if self.__config.get("units", "metric") == "metric"
-                else meters_to_miles(distance)
-            )
-            for distance in distances
-        ]
-
-    @property
-    def stages_seconds(self) -> List[int]:
-        """
-        Returns the seconds travelled between the locations of the trip in a list starting from origin - 1st stop and
-        ending last stop - destination. If the trip does not contain stops, the list will be of size 1.
-
-        Warning: If the trip is marked as updated, it will first calculate the trip
-
-        :return: A list of seconds between the locations of the trip in order
-        """
-
-        if self.__updated:
-            self.calculate_trip()
-
-        seconds: List[int] = []
-        if self.__stops:
-            for stage in self.__api_response.values():
-                stage_seconds = (
-                    stage.get("legs", [{}])[0].get("duration", {}).get("value", None)
-                )
-                if not stage_seconds:
-                    raise InvalidResponseError("legs[0].duration.value")
-
-                seconds.append(stage_seconds)
-        else:
-            seconds_trip = (
-                self.__api_response.get("legs", [{}])[0]
-                .get("duration", {})
-                .get("value", None)
-            )
-            if not seconds_trip:
-                raise InvalidResponseError("legs[0].duration.value")
-            seconds.append(seconds_trip)
-
-        return seconds
-
-    @property
-    def trip_calendar(self) -> List[Tuple[date, float]]:
-        """
-        Creates a list of pairs day-distance travelled from the trip.
-
-        Because the Google Maps API does not provide exact data for this calculation, the distances travelled will be
-        an estimation.
-
-        Warning: If the trip is marked as updated, it will first calculate the trip
-
-        :return: A list of pairs day-distance travelled in the unit given in the config ('metric' if not configured).
-        """
-
-        if self.__updated:
-            self.calculate_trip()
-
-        # Create calendar
-        calendar = {
-            self.__departure_date.date() + timedelta(days=i): 0.0
-            for i in range(self.days)
-        }
-
-        # Calculate kms travelled per day
-        if self.__stops:
-            current_date = self.__departure_date
-            for index, stage in enumerate(self.__api_response.values()):
-                steps = get_steps(stage)
-                calendar = calculate_stage_steps(steps, current_date, calendar)
-                current_date = self.__stops[index].departure_date if index < len(self.__stops) else None  # :)
-
-        else:
-            steps = get_steps(self.__api_response)
-            calendar = calculate_stage_steps(steps, self.__departure_date, calendar)
-
-        return [
-            (
-                day,
-                meters / 1000 if self.__config.get("units", "metric") == "metric" else meters_to_miles(meters)
-            )
-            for day, meters in calendar.items() if meters > 0
-        ]
-
-    @classmethod
-    def set_client(cls, client: Any) -> None:
-        """
-        Initializes the client for the directions request
-
-        :param client: A client object. Must contain a method called 'directions' that returns the raw Google Maps
-            Directions API response and takes the following parameters: origin, destination, mode, avoid, units,
-            departure_time, arrival_time, transit_mode, transit_routing_preference and traffic_model
-        """
-
-        cls.client = client
-
-    def calculate_trip(self, trip_config: TripConfig = None) -> Dict:
-        """
-        Calls the Google Maps API to calculate the trip, only if the trip needs to be updated.
-
-        This method will make at least one call to the Google Maps API and at most 1 + the number of stops.
-
-        :param trip_config: Trip configuration
-        :return: The raw API response if no stops are provided, otherwise a dictionary with the raw API responses
-        :raises ClientNotInitializedError: If the googlemaps client is not initialized
-        :raises TripWarning: If a trip attribute is ignored based on the config given
-        """
-
-        if trip_config:
-            self.config = trip_config
-
-        if not self.__updated:
-            return self.__api_response
-
-        if not self.client:
-            raise ClientNotInitializedError()
-
-        if self.__arrival_date and self.__stops:
-            TravelWarnings.ignore_field("arrival_date", "Ignored for trips with stops")
-        elif (
-            self.__arrival_date
-            and not self.__config.get("mode", "not_configured") == "transit"
-        ):
-            TravelWarnings.ignore_field("arrival_date", "Only used for transit mode")
-
-        # Make calls to the API
-        if self.__stops:
-            current_location = self.__origin.get_data()
-            current_date = (
-                self.__departure_date if self.__departure_date else datetime.now()
-            )  # Fixes HTTP 400 error
-
-            # Call for each stop
-            for index, stop in enumerate(self.__stops):
-                key = f"stage_{index}" if index > 0 else "departure"
-
-                self.__api_response[key] = self.client.directions(
-                    origin=current_location,
-                    destination=stop.location.get_data(),
-                    departure_time=current_date,
-                    **self.__config,
-                )[0]
-
-                current_location = stop.location.get_data()
-                current_date = stop.departure_date
-
-            # Call for last stage of the trip
-            self.__api_response["arrival"] = self.client.directions(
-                origin=current_location,
-                destination=self.__destination.get_data(),
-                departure_time=current_date,
-                **self.__config,
-            )[0]
-
-        else:
-            # Date argument depending on the given fields and configuration
-            if self.__departure_date:
-                date_argument = {"departure_time": self.__departure_date}
-            elif (
-                self.__arrival_date
-                and self.__config.get("mode", "not_configured") == "transit"
-            ):
-                date_argument = {"arrival_time": self.__arrival_date}
-            else:
-                date_argument = {
-                    "departure_time": datetime.now()
-                }  # Fixes HTTP 400 error
-
-            self.__api_response = self.client.directions(
-                origin=self.__origin.get_data(),
-                destination=self.__destination.get_data(),
-                **date_argument,
-                **self.__config,
-            )[0]
-
-        self.__updated = False
-        self.update_dates()  # Update dates
-        return self.__api_response
-
-    def update_dates(self) -> None:
-        """
-        Checks the given dates make sense and updates the ones that don't. If both departure and arrival dates are
-        found, departure date has preference for conflict resolution.
-
-        Warning: If the trip is marked as updated, it will first calculate the trip
-        """
-
-        if self.__updated:
-            self.calculate_trip()
-
-        travel_times = self.stages_seconds
-
-        # Check departure date
-        if not self.__departure_date and not self.__arrival_date:
-            self.__departure_date = datetime.now()
-            TravelWarnings.update_date("departure", "No departure date provided")
-        elif not self.__departure_date:
-            if not self.__stops:
-                self.__departure_date = self.__arrival_date - timedelta(
-                    seconds=travel_times[0]
-                )
-            else:
-                self.__departure_date = self.__stops[0].departure_date - timedelta(
-                    seconds=travel_times[0]
-                )
-            TravelWarnings.update_date("departure", "No departure date provided")
-
-        # Check stop dates
-        if self.__stops:
-            current_date = self.__departure_date
-            for index, stop in enumerate(self.__stops):
-                stop_arrival = current_date + timedelta(seconds=travel_times[index])
-                if stop.departure_date < stop_arrival:
-                    TravelWarnings.update_date(
-                        "stop", "Calculated arrival before departure date"
-                    )
-                    self.__stops[index] = Stop(stop.location, stop_arrival)
-                    current_date = stop_arrival
-                else:
-                    current_date = stop.departure_date
-
-        # Check arrival date
-        if not self.__stops:
-            new_arrival = self.__departure_date + timedelta(seconds=travel_times[0])
-        else:
-            new_arrival = self.__stops[-1].departure_date + timedelta(
-                seconds=travel_times[-1]
-            )
-
-        if not self.__arrival_date:
-            self.__arrival_date = new_arrival
-            TravelWarnings.update_date("arrival", "No arrival date provided")
-        elif self.__arrival_date != new_arrival:
-            self.__arrival_date = new_arrival
-            TravelWarnings.update_date("arrival", "Calculated arrival does not match")
+from datetime import datetime, date, timedelta
+from typing import Tuple, List, Dict, Any
+
+from py_travel.exceptions import ClientNotInitializedError, TravelWarnings, InvalidResponseError
+from py_travel.location import Location, input_to_location
+from py_travel.utils import meters_to_miles, get_distance, get_duration, get_steps, calculate_stage_steps
+from .trip_config import TripConfig
+from .stop import Stop
+
+
+class Trip:
+    """
+    Trip class
+
+    Attributes:
+        client: Client object for the Google Maps API calls
+        origin: Origin of the trip
+        destination: Destination of the trip
+        departure_date: Start date of the trip
+        arrival_date: End date of the trip
+        stops: List of stops associated with the trip
+        updated: Boolean indicating if the object needs to call the Google Maps API to get the results
+        api_response: Raw Google Maps API response
+    """
+
+    client: Any = None
+
+    def __init__(
+        self,
+        origin: Tuple[float, float] | str | Location,
+        destination: Tuple[float, float] | str | Location,
+        stops: List[Tuple[Tuple[float, float] | str | Location, datetime]] = None,
+        departure_date: datetime = None,
+        arrival_date: datetime = None,
+        config: TripConfig = None,
+    ) -> None:
+        """
+        Initialize Trip object
+
+        :param origin: Origin of the trip in pair (latitude, longitude) or address or Location object
+        :param destination: Destination of the trip in pair (latitude, longitude) or address or Location object
+        :param stops: A list of tuples containing the stop location (either a tuple containing the coordinates, the
+            address or a Location object) and the departure date from the stop
+        :param departure_date: Start date of the trip (optional)
+        :param arrival_date: End date of the trip (optional)
+        :param config: Trip configuration either as a dictionary or as a TripConfig object (optional)
+        """
+
+        self.__origin = input_to_location(origin)
+        self.__destination = input_to_location(destination)
+
+        self.__stops = (
+            [Stop(input_to_location(loc), dep_date) for loc, dep_date in stops]
+            if stops
+            else []
+        )
+        self.__stops.sort(key=lambda stop: stop.departure_date)
+
+        self.__departure_date = departure_date
+        self.__arrival_date = arrival_date
+
+        self.__config = config if config else {}
+
+        self.__api_response: Dict = {}
+        self.__updated = True
+
+    @property
+    def origin(self) -> Location:
+        """
+        :return: The origin location of the trip
+        """
+        return self.__origin
+
+    @origin.setter
+    def origin(self, new_origin: Tuple[float, float] | str | Location) -> None:
+        """
+        Sets the origin location of the trip
+
+        Warning: This will mark the trip as updated, possibly causing calls to the Google Maps API in the future.
+
+        :param new_origin: Origin of the trip in pair (latitude, longitude), string with address or Location object
+        """
+        self.__origin = input_to_location(new_origin)
+        self.__updated = True
+
+    @property
+    def destination(self) -> Location:
+        """
+        :return: The destination location of the trip
+        """
+        return self.__destination
+
+    @destination.setter
+    def destination(
+        self, new_destination: Tuple[float, float] | str | Location
+    ) -> None:
+        """
+        Sets the destination location of the trip
+
+        Warning: This will mark the trip as updated, possibly causing calls to the Google Maps API in the future.
+
+        :param new_destination: Destination of the trip in pair (latitude, longitude), string with address or Location
+            object
+        """
+        self.__destination = input_to_location(new_destination)
+        self.__updated = True
+
+    @property
+    def stops(self) -> List[Stop]:
+        """
+        :return: The list of stops
+        """
+        return self.__stops
+
+    @stops.setter
+    def stops(
+        self, stops: List[Tuple[Tuple[float, float] | str | Location, datetime]] | List[Stop]
+    ) -> None:
+        """
+        Sets the stops for the trip
+
+        Warning: This will mark the trip as updated, possibly causing calls to the Google Maps API in the future.
+
+        :param stops: A list of tuples containing the stop location (either a tuple containing the coordinates, the
+            address or a Location object) and the departure date from the stop, or a list of Stop objects
+        """
+
+        self.__stops = []
+        for stop in stops:
+            if isinstance(stop, Stop):
+                self.__stops.append(stop)
+            else:
+                self.__stops.append(Stop(input_to_location(stop[0]), stop[1]))
+
+        self.__stops.sort(key=lambda s: s.departure_date)
+        self.__updated = True
+
+    @property
+    def departure_date(self) -> datetime:
+        """
+        :return: The departure date of the trip
+        """
+        return self.__departure_date
+
+    @departure_date.setter
+    def departure_date(self, new_departure_date: datetime) -> None:
+        """
+        Sets the departure date of the trip
+
+        Warning: This will mark the trip as updated, possibly causing calls to the Google Maps API in the future.
+
+        :param new_departure_date: The departure date of the trip
+        """
+        self.__departure_date = new_departure_date
+        self.__updated = True
+
+    @property
+    def arrival_date(self) -> datetime:
+        """
+        :return: The arrival date of the trip
+        """
+        return self.__arrival_date
+
+    @arrival_date.setter
+    def arrival_date(self, new_arrival_date: datetime) -> None:
+        """
+        Sets the arrival date of the trip
+
+        Warning: This will mark the trip as updated, possibly causing calls to the Google Maps API in the future.
+
+        :param new_arrival_date: The arrival date of the trip
+        """
+        self.__arrival_date = new_arrival_date
+        self.__updated = True
+
+    @property
+    def config(self) -> TripConfig:
+        """
+        :return: The configuration parameters of the trip
+        """
+        return self.__config
+
+    @config.setter
+    def config(self, new_config: TripConfig) -> None:
+        """
+        Set the configuration for the calculations
+
+        Warning: This method will mark the trip as updated, possibly causing calls to the Google Maps API in the future.
+
+        :param new_config: Trip configuration
+        """
+
+        self.__config = new_config
+        self.__updated = True
+
+    @property
+    def api_response(self) -> Dict:
+        """
+        :return: The response from the Google Maps API
+        """
+        return self.__api_response
+
+    @property
+    def distance(self) -> float:
+        """
+        Warning: If the trip is marked as updated, it will first calculate the trip
+        :return: The total distance of the trip in the unit given in the config ('metric' if not configured).
+        """
+
+        if self.__updated:
+            self.calculate_trip()
+
+        if self.__stops:
+            meters = sum(get_distance(stage) for stage in self.__api_response.values())
+        else:
+            meters = get_distance(self.__api_response)
+
+        return (
+            meters / 1000
+            if self.__config.get("units", "metric") == "metric"
+            else meters_to_miles(meters)
+        )
+
+    @property
+    def seconds(self) -> int:
+        """
+        Warning: If the trip is marked as updated, it will first calculate the trip
+        :return: The amount of seconds travelled in the trip
+        """
+
+        if self.__updated:
+            self.calculate_trip()
+
+        if self.__stops:
+            seconds = sum(get_duration(stage) for stage in self.__api_response.values())
+        else:
+            seconds = get_duration(self.__api_response)
+
+        return seconds
+
+    @property
+    def days(self) -> int:
+        """
+        Warning: If the trip is marked as updated, it will first calculate the trip
+        :return: Duration in days of the trip (rounded up)
+        """
+
+        if self.__updated:
+            self.calculate_trip()  # This will call update_dates()
+
+        return (self.__arrival_date.date() - self.__departure_date.date()).days + 1
+
+    @property
+    def stages_distances(self) -> List[float]:
+        """
+        Returns the distances between the locations of the trip in a list starting from origin - 1st stop and ending
+        with last stop - destination. If the trip does not contain stops, the list will be of size 1.
+
+        Warning: If the trip is marked as updated, it will first calculate the trip
+
+        :return: A list of distances between the locations of the trip in order
+        """
+
+        if self.__updated:
+            self.calculate_trip()
+
+        distances: List[float] = []
+        if self.__stops:
+            for stage in self.__api_response.values():
+                stage_meters = (
+                    stage.get("legs", [{}])[0].get("distance", {}).get("value", None)
+                )
+                if not stage_meters:
+                    raise InvalidResponseError("legs[0].distance.value")
+
+                distances.append(stage_meters)
+        else:
+            meters = (
+                self.__api_response.get("legs", [{}])[0]
+                .get("distance", {})
+                .get("value", None)
+            )
+            if not meters:
+                raise InvalidResponseError("legs[0].distance.value")
+            distances.append(meters)
+
+        return [
+            (
+                distance / 1000
+                if self.__config.get("units", "metric") == "metric"
+                else meters_to_miles(distance)
+            )
+            for distance in distances
+        ]
+
+    @property
+    def stages_seconds(self) -> List[int]:
+        """
+        Returns the seconds travelled between the locations of the trip in a list starting from origin - 1st stop and
+        ending last stop - destination. If the trip does not contain stops, the list will be of size 1.
+
+        Warning: If the trip is marked as updated, it will first calculate the trip
+
+        :return: A list of seconds between the locations of the trip in order
+        """
+
+        if self.__updated:
+            self.calculate_trip()
+
+        seconds: List[int] = []
+        if self.__stops:
+            for stage in self.__api_response.values():
+                stage_seconds = (
+                    stage.get("legs", [{}])[0].get("duration", {}).get("value", None)
+                )
+                if not stage_seconds:
+                    raise InvalidResponseError("legs[0].duration.value")
+
+                seconds.append(stage_seconds)
+        else:
+            seconds_trip = (
+                self.__api_response.get("legs", [{}])[0]
+                .get("duration", {})
+                .get("value", None)
+            )
+            if not seconds_trip:
+                raise InvalidResponseError("legs[0].duration.value")
+            seconds.append(seconds_trip)
+
+        return seconds
+
+    @property
+    def trip_calendar(self) -> List[Tuple[date, float]]:
+        """
+        Creates a list of pairs day-distance travelled from the trip.
+
+        Because the Google Maps API does not provide exact data for this calculation, the distances travelled will be
+        an estimation.
+
+        Warning: If the trip is marked as updated, it will first calculate the trip
+
+        :return: A list of pairs day-distance travelled in the unit given in the config ('metric' if not configured).
+        """
+
+        if self.__updated:
+            self.calculate_trip()
+
+        # Create calendar
+        calendar = {
+            self.__departure_date.date() + timedelta(days=i): 0.0
+            for i in range(self.days)
+        }
+
+        # Calculate kms travelled per day
+        if self.__stops:
+            current_date = self.__departure_date
+            for index, stage in enumerate(self.__api_response.values()):
+                steps = get_steps(stage)
+                calendar = calculate_stage_steps(steps, current_date, calendar)
+                current_date = self.__stops[index].departure_date if index < len(self.__stops) else None  # :)
+
+        else:
+            steps = get_steps(self.__api_response)
+            calendar = calculate_stage_steps(steps, self.__departure_date, calendar)
+
+        return [
+            (
+                day,
+                meters / 1000 if self.__config.get("units", "metric") == "metric" else meters_to_miles(meters)
+            )
+            for day, meters in calendar.items() if meters > 0
+        ]
+
+    @classmethod
+    def set_client(cls, client: Any) -> None:
+        """
+        Initializes the client for the directions request
+
+        :param client: A client object. Must contain a method called 'directions' that returns the raw Google Maps
+            Directions API response and takes the following parameters: origin, destination, mode, avoid, units,
+            departure_time, arrival_time, transit_mode, transit_routing_preference and traffic_model
+        """
+
+        cls.client = client
+
+    def calculate_trip(self, trip_config: TripConfig = None) -> Dict:
+        """
+        Calls the Google Maps API to calculate the trip, only if the trip needs to be updated.
+
+        This method will make at least one call to the Google Maps API and at most 1 + the number of stops.
+
+        :param trip_config: Trip configuration
+        :return: The raw API response if no stops are provided, otherwise a dictionary with the raw API responses
+        :raises ClientNotInitializedError: If the googlemaps client is not initialized
+        :raises TripWarning: If a trip attribute is ignored based on the config given
+        """
+
+        if trip_config:
+            self.config = trip_config
+
+        if not self.__updated:
+            return self.__api_response
+
+        if not self.client:
+            raise ClientNotInitializedError()
+
+        if self.__arrival_date and self.__stops:
+            TravelWarnings.ignore_field("arrival_date", "Ignored for trips with stops")
+        elif (
+            self.__arrival_date
+            and not self.__config.get("mode", "not_configured") == "transit"
+        ):
+            TravelWarnings.ignore_field("arrival_date", "Only used for transit mode")
+
+        # Make calls to the API
+        if self.__stops:
+            current_location = self.__origin.get_data()
+            current_date = (
+                self.__departure_date if self.__departure_date else datetime.now()
+            )  # Fixes HTTP 400 error
+
+            # Call for each stop
+            for index, stop in enumerate(self.__stops):
+                key = f"stage_{index}" if index > 0 else "departure"
+
+                self.__api_response[key] = self.client.directions(
+                    origin=current_location,
+                    destination=stop.location.get_data(),
+                    departure_time=current_date,
+                    **self.__config,
+                )[0]
+
+                current_location = stop.location.get_data()
+                current_date = stop.departure_date
+
+            # Call for last stage of the trip
+            self.__api_response["arrival"] = self.client.directions(
+                origin=current_location,
+                destination=self.__destination.get_data(),
+                departure_time=current_date,
+                **self.__config,
+            )[0]
+
+        else:
+            # Date argument depending on the given fields and configuration
+            if self.__departure_date:
+                date_argument = {"departure_time": self.__departure_date}
+            elif (
+                self.__arrival_date
+                and self.__config.get("mode", "not_configured") == "transit"
+            ):
+                date_argument = {"arrival_time": self.__arrival_date}
+            else:
+                date_argument = {
+                    "departure_time": datetime.now()
+                }  # Fixes HTTP 400 error
+
+            self.__api_response = self.client.directions(
+                origin=self.__origin.get_data(),
+                destination=self.__destination.get_data(),
+                **date_argument,
+                **self.__config,
+            )[0]
+
+        self.__updated = False
+        self.update_dates()  # Update dates
+        return self.__api_response
+
+    def update_dates(self) -> None:
+        """
+        Checks the given dates make sense and updates the ones that don't. If both departure and arrival dates are
+        found, departure date has preference for conflict resolution.
+
+        Warning: If the trip is marked as updated, it will first calculate the trip
+        """
+
+        if self.__updated:
+            self.calculate_trip()
+
+        travel_times = self.stages_seconds
+
+        # Check departure date
+        if not self.__departure_date and not self.__arrival_date:
+            self.__departure_date = datetime.now()
+            TravelWarnings.update_date("departure", "No departure date provided")
+        elif not self.__departure_date:
+            if not self.__stops:
+                self.__departure_date = self.__arrival_date - timedelta(
+                    seconds=travel_times[0]
+                )
+            else:
+                self.__departure_date = self.__stops[0].departure_date - timedelta(
+                    seconds=travel_times[0]
+                )
+            TravelWarnings.update_date("departure", "No departure date provided")
+
+        # Check stop dates
+        if self.__stops:
+            current_date = self.__departure_date
+            for index, stop in enumerate(self.__stops):
+                stop_arrival = current_date + timedelta(seconds=travel_times[index])
+                if stop.departure_date < stop_arrival:
+                    TravelWarnings.update_date(
+                        "stop", "Calculated arrival before departure date"
+                    )
+                    self.__stops[index] = Stop(stop.location, stop_arrival)
+                    current_date = stop_arrival
+                else:
+                    current_date = stop.departure_date
+
+        # Check arrival date
+        if not self.__stops:
+            new_arrival = self.__departure_date + timedelta(seconds=travel_times[0])
+        else:
+            new_arrival = self.__stops[-1].departure_date + timedelta(
+                seconds=travel_times[-1]
+            )
+
+        if not self.__arrival_date:
+            self.__arrival_date = new_arrival
+            TravelWarnings.update_date("arrival", "No arrival date provided")
+        elif self.__arrival_date != new_arrival:
+            self.__arrival_date = new_arrival
+            TravelWarnings.update_date("arrival", "Calculated arrival does not match")
```

### Comparing `py_travel-0.1/py_travel/trip/trip_config.py` & `py_travel-0.1.1/py_travel/trip/trip_config.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from typing import TypedDict, List
-
-from py_travel.vars import TRIP_MODES, AVOID_FEATURES, METRIC_SYSTEMS, TRANSIT_MODES, TRANSIT_PREFERENCES, TRAFFIC_MODE
-
-
-class TripConfig(TypedDict, total=False):
-    """
-    Contains the trip configuration variables
-
-    Attributes:
-        mode: Trip mode: driving, walking, bicycling or transit.
-        avoid: Features to avoid: tolls, highways, ferries, indoor or a combination of them
-        units: Unit system for the calculations: metric or imperial.
-        transit_mode: Transit mode if the mode is 'transit': bus, subway, train, tram, rail or a combination of them.
-        transit_routing_preference: Preference in calculations for transit: less_walking or fewer_transfer.
-        traffic_model: Traffic model to use if mode is 'driving': best_guess, optimistic or pessimistic.
-    """
-
-    mode: TRIP_MODES
-    avoid: List[AVOID_FEATURES] | AVOID_FEATURES
-    units: METRIC_SYSTEMS
-    transit_mode: List[TRANSIT_MODES] | TRANSIT_MODES
-    transit_routing_preference: TRANSIT_PREFERENCES
-    traffic_model: TRAFFIC_MODE
+from typing import TypedDict, List
+
+from py_travel.vars import TRIP_MODES, AVOID_FEATURES, METRIC_SYSTEMS, TRANSIT_MODES, TRANSIT_PREFERENCES, TRAFFIC_MODE
+
+
+class TripConfig(TypedDict, total=False):
+    """
+    Contains the trip configuration variables
+
+    Attributes:
+        mode: Trip mode: driving, walking, bicycling or transit.
+        avoid: Features to avoid: tolls, highways, ferries, indoor or a combination of them
+        units: Unit system for the calculations: metric or imperial.
+        transit_mode: Transit mode if the mode is 'transit': bus, subway, train, tram, rail or a combination of them.
+        transit_routing_preference: Preference in calculations for transit: less_walking or fewer_transfer.
+        traffic_model: Traffic model to use if mode is 'driving': best_guess, optimistic or pessimistic.
+    """
+
+    mode: TRIP_MODES
+    avoid: List[AVOID_FEATURES] | AVOID_FEATURES
+    units: METRIC_SYSTEMS
+    transit_mode: List[TRANSIT_MODES] | TRANSIT_MODES
+    transit_routing_preference: TRANSIT_PREFERENCES
+    traffic_model: TRAFFIC_MODE
```

### Comparing `py_travel-0.1/tests/mock_client.py` & `py_travel-0.1.1/tests/mock_client.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-from typing import List, TYPE_CHECKING, Dict
-
-if TYPE_CHECKING:  # pragma: no cover
-    from datetime import datetime
-
-# ----------------------------------------------------------------------------------------------------------------------
-# Mock constants
-TEST_METERS = 1800
-TEST_SECONDS = 3600
-MOCK_N_STEPS = 10
-MOCK_DISTANCE = {"distance": {"value": TEST_METERS}}
-MOCK_TIME = {"duration": {"value": TEST_SECONDS}}
-MOCK_STEP = {**MOCK_DISTANCE, **MOCK_TIME}
-
-
-# ----------------------------------------------------------------------------------------------------------------------
-# Mock classes
-class ClientNotInitializedError(Exception):
-    pass
-
-
-class TestClient:
-    """
-    Test client to avoid calls to the Google Maps API in testing
-    """
-
-    def __init__(self, key: str = None):
-        """
-        Initialize the client
-
-        :param key: Mock API key
-        """
-
-        if not isinstance(key, str):
-            raise ValueError("Key must be a string")
-
-        self.key = key
-
-    def directions(
-        self,
-        origin: str,
-        destination: str,
-        mode: str = None,
-        avoid: List[str] | str = None,
-        units: str = None,
-        departure_time: "datetime" = None,
-        arrival_time: "datetime" = None,
-        transit_mode: List[str] | str = None,
-        transit_routing_preference: str = None,
-        traffic_model: str = None,
-    ) -> List[Dict]:
-        """
-        Mocks the Google Maps API 'directions' method
-        """
-
-        if not self.key:
-            raise ClientNotInitializedError()
-
-        response = {
-            "input": {
-                "origin": origin,
-                "destination": destination,
-                "mode": mode,
-                "avoid": avoid,
-                "units": units,
-                "departure_time": departure_time,
-                "arrival_time": arrival_time,
-                "transit_mode": transit_mode,
-                "transit_routing_preference": transit_routing_preference,
-                "traffic_model": traffic_model,
-            },
-            "legs": [{
-                **MOCK_DISTANCE,
-                **MOCK_TIME,
-                "steps": [{**MOCK_STEP}] * MOCK_N_STEPS
-            }]
-        }
-
+from typing import List, TYPE_CHECKING, Dict
+
+if TYPE_CHECKING:  # pragma: no cover
+    from datetime import datetime
+
+# ----------------------------------------------------------------------------------------------------------------------
+# Mock constants
+TEST_METERS = 1800
+TEST_SECONDS = 3600
+MOCK_N_STEPS = 10
+MOCK_DISTANCE = {"distance": {"value": TEST_METERS}}
+MOCK_TIME = {"duration": {"value": TEST_SECONDS}}
+MOCK_STEP = {**MOCK_DISTANCE, **MOCK_TIME}
+
+
+# ----------------------------------------------------------------------------------------------------------------------
+# Mock classes
+class ClientNotInitializedError(Exception):
+    pass
+
+
+class TestClient:
+    """
+    Test client to avoid calls to the Google Maps API in testing
+    """
+
+    def __init__(self, key: str = None):
+        """
+        Initialize the client
+
+        :param key: Mock API key
+        """
+
+        if not isinstance(key, str):
+            raise ValueError("Key must be a string")
+
+        self.key = key
+
+    def directions(
+        self,
+        origin: str,
+        destination: str,
+        mode: str = None,
+        avoid: List[str] | str = None,
+        units: str = None,
+        departure_time: "datetime" = None,
+        arrival_time: "datetime" = None,
+        transit_mode: List[str] | str = None,
+        transit_routing_preference: str = None,
+        traffic_model: str = None,
+    ) -> List[Dict]:
+        """
+        Mocks the Google Maps API 'directions' method
+        """
+
+        if not self.key:
+            raise ClientNotInitializedError()
+
+        response = {
+            "input": {
+                "origin": origin,
+                "destination": destination,
+                "mode": mode,
+                "avoid": avoid,
+                "units": units,
+                "departure_time": departure_time,
+                "arrival_time": arrival_time,
+                "transit_mode": transit_mode,
+                "transit_routing_preference": transit_routing_preference,
+                "traffic_model": traffic_model,
+            },
+            "legs": [{
+                **MOCK_DISTANCE,
+                **MOCK_TIME,
+                "steps": [{**MOCK_STEP}] * MOCK_N_STEPS
+            }]
+        }
+
         return [response]
```

### Comparing `py_travel-0.1/tests/test_trip.py` & `py_travel-0.1.1/tests/test_trip.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-import pytest
-from datetime import datetime
-
-from py_travel.location import Location
-from py_travel.trip import Trip
-from tests.mock_client import TEST_METERS, TEST_SECONDS
-
-
-TEST_KMS = TEST_METERS / 1000
-
-
-class TestTrip:
-    @pytest.mark.parametrize(
-        "test_input",
-        [
-            # Coordinates
-            {"origin": (0.0, 0.0), "destination": (0.0, 0.0)},
-            # Address
-            {"origin": "Test Origin", "destination": "Test Destination"},
-            # Location object
-            {
-                "origin": Location(0.0, 0.0, "Test Origin"),
-                "destination": Location(0.0, 0.0, "Test Destination"),
-            },
-        ],
-    )
-    def test_create_trip(self, test_input):
-        """
-        Test that a Trip object can be instantiated
-        """
-        try:
-            Trip(**test_input)
-        except TypeError:
-            pytest.fail("Invalid parameter")
-
-    def test_distance(self, basic_trip, trip_stop):
-        """
-        Test that the distance calculation works
-        """
-        assert basic_trip.distance == TEST_KMS
-        assert trip_stop.distance == TEST_KMS * 2
-
-    def test_distances(self, basic_trip, trip_stop):
-        """
-        Test that the partial distances calculation works
-        """
-        assert basic_trip.stages_distances == [TEST_KMS]
-        assert trip_stop.stages_distances == [TEST_KMS, TEST_KMS]
-
-    def test_travel_time(self, basic_trip, trip_stop):
-        """
-        Test that the duration calculation works
-        """
-        assert basic_trip.seconds == TEST_SECONDS
-        assert trip_stop.seconds == TEST_SECONDS * 2
-
-    def test_travel_times(self, basic_trip, trip_stop):
-        """
-        Test that the partial duration calculation works
-        """
-        assert basic_trip.stages_seconds == [TEST_SECONDS]
-        assert trip_stop.stages_seconds == [TEST_SECONDS, TEST_SECONDS]
-
-    def test_days(self, basic_trip, trip_stop, trip_stops):
-        """
-        Test that the days calculation works
-        """
-        assert basic_trip.days == 1
-        assert trip_stop.days == 1
-        assert trip_stops.days == 4
-
-    @pytest.mark.parametrize(
-        ("departure", "arrival"),
-        [
-            # No dates
-            (None, None),
-            # Only departure
-            (datetime.now(), None),
-            # Only arrival
-            (None, datetime.now()),
-            # Departure & arrival
-            (datetime.now(), datetime.now()),
-        ],
-    )
-    def test_updated_dates(self, departure, arrival):
-        """
-        Test that the dates are updated after trip calculations
-        """
-
-        old_departure = departure
-        old_arrival = arrival
-        trip = Trip("", "", departure_date=departure, arrival_date=arrival)
-        trip.calculate_trip()
-
-        if not departure:
-            assert trip.departure_date != old_departure
-        if not arrival or (departure and arrival):
-            assert trip.arrival_date != old_arrival
-
-    def test_updated_dates_stops(self, trip_stop):
-        """
-        Test that the dates are updated after trip calculations for a trip with stops
-        """
-
-        stop_date = trip_stop.stops[0].departure_date
-
-        trip_stop.calculate_trip()
-
-        assert trip_stop.stops[0].departure_date != stop_date
-
-    def test_calendar_no_stops(self, basic_trip):
-        """
-        Test that the trip calendar works with no stops
-        """
-
-        trip_calendar = basic_trip.trip_calendar
-
-        assert len(trip_calendar) == 1
-        assert trip_calendar[0][0] == basic_trip.departure_date.date()
-
-    def test_calendar_stops(self, trip_stops):
-        """
-        Test that the trip calendar works with no stops
-        """
-
-        trip_calendar = trip_stops.trip_calendar
-
-        assert len(trip_calendar) == 4
-        assert trip_calendar[0][0] == trip_stops.departure_date.date()
+import pytest
+from datetime import datetime
+
+from py_travel.location import Location
+from py_travel.trip import Trip
+from tests.mock_client import TEST_METERS, TEST_SECONDS
+
+
+TEST_KMS = TEST_METERS / 1000
+
+
+class TestTrip:
+    @pytest.mark.parametrize(
+        "test_input",
+        [
+            # Coordinates
+            {"origin": (0.0, 0.0), "destination": (0.0, 0.0)},
+            # Address
+            {"origin": "Test Origin", "destination": "Test Destination"},
+            # Location object
+            {
+                "origin": Location(0.0, 0.0, "Test Origin"),
+                "destination": Location(0.0, 0.0, "Test Destination"),
+            },
+        ],
+    )
+    def test_create_trip(self, test_input):
+        """
+        Test that a Trip object can be instantiated
+        """
+        try:
+            Trip(**test_input)
+        except TypeError:
+            pytest.fail("Invalid parameter")
+
+    def test_distance(self, basic_trip, trip_stop):
+        """
+        Test that the distance calculation works
+        """
+        assert basic_trip.distance == TEST_KMS
+        assert trip_stop.distance == TEST_KMS * 2
+
+    def test_distances(self, basic_trip, trip_stop):
+        """
+        Test that the partial distances calculation works
+        """
+        assert basic_trip.stages_distances == [TEST_KMS]
+        assert trip_stop.stages_distances == [TEST_KMS, TEST_KMS]
+
+    def test_travel_time(self, basic_trip, trip_stop):
+        """
+        Test that the duration calculation works
+        """
+        assert basic_trip.seconds == TEST_SECONDS
+        assert trip_stop.seconds == TEST_SECONDS * 2
+
+    def test_travel_times(self, basic_trip, trip_stop):
+        """
+        Test that the partial duration calculation works
+        """
+        assert basic_trip.stages_seconds == [TEST_SECONDS]
+        assert trip_stop.stages_seconds == [TEST_SECONDS, TEST_SECONDS]
+
+    def test_days(self, basic_trip, trip_stop, trip_stops):
+        """
+        Test that the days calculation works
+        """
+        assert basic_trip.days == 1
+        assert trip_stop.days == 1
+        assert trip_stops.days == 4
+
+    @pytest.mark.parametrize(
+        ("departure", "arrival"),
+        [
+            # No dates
+            (None, None),
+            # Only departure
+            (datetime.now(), None),
+            # Only arrival
+            (None, datetime.now()),
+            # Departure & arrival
+            (datetime.now(), datetime.now()),
+        ],
+    )
+    def test_updated_dates(self, departure, arrival):
+        """
+        Test that the dates are updated after trip calculations
+        """
+
+        old_departure = departure
+        old_arrival = arrival
+        trip = Trip("", "", departure_date=departure, arrival_date=arrival)
+        trip.calculate_trip()
+
+        if not departure:
+            assert trip.departure_date != old_departure
+        if not arrival or (departure and arrival):
+            assert trip.arrival_date != old_arrival
+
+    def test_updated_dates_stops(self, trip_stop):
+        """
+        Test that the dates are updated after trip calculations for a trip with stops
+        """
+
+        stop_date = trip_stop.stops[0].departure_date
+
+        trip_stop.calculate_trip()
+
+        assert trip_stop.stops[0].departure_date != stop_date
+
+    def test_calendar_no_stops(self, basic_trip):
+        """
+        Test that the trip calendar works with no stops
+        """
+
+        trip_calendar = basic_trip.trip_calendar
+
+        assert len(trip_calendar) == 1
+        assert trip_calendar[0][0] == basic_trip.departure_date.date()
+
+    def test_calendar_stops(self, trip_stops):
+        """
+        Test that the trip calendar works with no stops
+        """
+
+        trip_calendar = trip_stops.trip_calendar
+
+        assert len(trip_calendar) == 4
+        assert trip_calendar[0][0] == trip_stops.departure_date.date()
```

### Comparing `py_travel-0.1/LICENSE` & `py_travel-0.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `py_travel-0.1/README.md` & `py_travel-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,98 +1,110 @@
-# Python travelling library
-
-![GitHub License](https://img.shields.io/github/license/diagmatrix/py-travel)
-![Python ^3.10](https://img.shields.io/badge/Python-3.10%2B-blue)
-![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/diagmatrix/py-travel/commit.yml)
-![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/diagmatrix/py-travel)
-
-
-This is a Python library to use in conjunction with the 
-[Google Maps API](https://github.com/googlemaps/google-maps-services-python) (at least for now) in order to plan trips
-and much more! It tries to bring a less JSON-oriented way of using the API.
-
-## Roadmap
-
- 1. Distance and timing calculations for trips. ✔️
- 2. Geocoding and decoding locations in the globe.
- 3. Support for static map images.
- 4. Drop `googlemaps` dependency.
- 5. Investigate other APIs to use.
- 6. ...
-
-
-## Getting started
-
-These instructions will get you a copy of the project up and running on your local machine for development and testing
-purposes.
-
-### Prerequisites
-
-You will need the following:
-
- - Python >= 3.10
- - A Google Maps API key (for testing outside the testing environment)
-
-### Installing
-
-For a local installation, just clone this repository inside the parent directory of your project.
-
-````bash
-git clone https://github.com/diagmatrix/py-travel.git
-git checkout main
-````
-
-Then install the dependencies of **py-travel**.
-
-````bash
-pip install -r requirements.txt
-````
-
-And there you have it! You can now use this library freely.
-
-## Usage
-
-There are currently two ways of using the classes provided in the package: by using the built-in
-Google Maps API clients or by using the `googlemaps` client directly. The first method will initialize an API client for
-each of the classes of **py-travel** that use them, while the second approach will give you more control on which ones
-can access it.
-
-### Using built-in client
-
-````python
-from py_travel import init_clients
-from py_travel.trip import Trip
-
-init_clients(api_key="<API KEY>")  # Initialize all API clients
-my_trip = Trip(origin=(39.25, -4.47), destination="Aveiro, Portugal", config={'mode': 'walking'})
-
-# Get the kms between the points
-kms = my_trip.distance
-````
-
-### Using `googlemaps` directly
-
-````python
-from py_travel.trip import Trip
-import googlemaps
-
-cli = googlemaps.Client(key="<API KEY>")
-Trip.set_client(cli)  # Initialize client for the trip class
-my_trip = Trip(origin=(39.25, -4.47), destination="Aveiro, Portugal", config={'mode': 'walking'})
-
-# Get the kms between the points
-kms = my_trip.distance
-````
-
-## Running the tests
-
-In order to run the tests you will first need to install the python package `pytest`. Then, place yourself in the parent 
-branch of the repository and run the following command:
-
-````bash
-pytest
-````
-For linting tests, this project uses the default `ruff` configuration.
-
-## Contributing
-
-Work in progress
+# Python travelling library
+
+![GitHub License](https://img.shields.io/github/license/diagmatrix/py-travel)
+![Python ^3.10](https://img.shields.io/badge/Python-3.10%2B-blue)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/diagmatrix/py-travel/commit.yml)
+![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/diagmatrix/py-travel)
+![PyPI - Status](https://img.shields.io/pypi/status/py_travel)
+
+
+This is a Python library to use in conjunction with the 
+[Google Maps API](https://github.com/googlemaps/google-maps-services-python) (at least for now) in order to plan trips
+and much more! It tries to bring a less JSON-oriented way of using the API.
+
+## Roadmap
+
+ 1. Distance and timing calculations for trips. ✔️
+ 2. Geocoding and decoding locations in the globe.
+ 3. Support for static map images.
+ 4. Drop `googlemaps` dependency.
+ 5. Investigate other APIs to use.
+ 6. ...
+
+
+## Getting started
+
+These instructions will get you a copy of the project up and running on your local machine for development and testing
+purposes.
+
+### Local installation
+
+#### Prerequisites
+
+You will need the following:
+
+ - Python >= 3.10
+ - A Google Maps API key (for testing outside the testing environment)
+
+#### Installing
+
+For a local installation, just clone this repository inside the parent directory of your project.
+
+````bash
+git clone https://github.com/diagmatrix/py-travel.git
+git checkout main
+````
+
+Then install the dependencies of **py-travel**.
+
+````bash
+pip install -r requirements.txt
+````
+
+And there you have it! You can now use this library freely.
+
+### Installation
+
+This project is available in [PyPy](https://pypi.org/project/py-travel/), so you can install it using
+pip.
+
+````bash
+pip install py-travel
+````
+
+## Usage
+
+There are currently two ways of using the classes provided in the package: by using the built-in
+Google Maps API clients or by using the `googlemaps` client directly. The first method will initialize an API client for
+each of the classes of **py-travel** that use them, while the second approach will give you more control on which ones
+can access it.
+
+### Using built-in client
+
+````python
+from py_travel import init_clients
+from py_travel.trip import Trip
+
+init_clients(api_key="<API KEY>")  # Initialize all API clients
+my_trip = Trip(origin=(39.25, -4.47), destination="Aveiro, Portugal", config={'mode': 'walking'})
+
+# Get the kms between the points
+kms = my_trip.distance
+````
+
+### Using `googlemaps` directly
+
+````python
+from py_travel.trip import Trip
+import googlemaps
+
+cli = googlemaps.Client(key="<API KEY>")
+Trip.set_client(cli)  # Initialize client for the trip class
+my_trip = Trip(origin=(39.25, -4.47), destination="Aveiro, Portugal", config={'mode': 'walking'})
+
+# Get the kms between the points
+kms = my_trip.distance
+````
+
+## Running the tests
+
+In order to run the tests you will first need to install the python package `pytest`. Then, place yourself in the parent 
+branch of the repository and run the following command:
+
+````bash
+pytest
+````
+For linting tests, this project uses the default `ruff` configuration.
+
+## Contributing
+
+Work in progress
```

### Comparing `py_travel-0.1/pyproject.toml` & `py_travel-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "py_travel"
-version = "0.1"
-authors = [
-  { name="diagmatrix", email="manuel.gachs@gmail.com" },
-]
-description = "Plan trips using the Google Maps API"
-readme = "README.md"
-requires-python = ">=3.10"
-dependencies = ["googlemaps>=4.10.0"]
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "Development Status :: 3 - Alpha",
-    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-Homepage = "https://github.com/diagmatrix/py_travel"
-Issues = "https://github.com/diagmatrix/py_travel/issues"
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "py_travel"
+version = "0.1.1"
+authors = [
+  { name="diagmatrix", email="manuel.gachs@gmail.com" },
+]
+description = "Plan trips using the Google Maps API"
+readme = "README.md"
+requires-python = ">=3.10"
+dependencies = ["googlemaps>=4.10.0"]
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "Development Status :: 3 - Alpha",
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+Homepage = "https://github.com/diagmatrix/py_travel"
+Issues = "https://github.com/diagmatrix/py_travel/issues"
```

### Comparing `py_travel-0.1/PKG-INFO` & `py_travel-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: py_travel
-Version: 0.1
+Version: 0.1.1
 Summary: Plan trips using the Google Maps API
 Project-URL: Homepage, https://github.com/diagmatrix/py_travel
 Project-URL: Issues, https://github.com/diagmatrix/py_travel/issues
 Author-email: diagmatrix <manuel.gachs@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -16,14 +16,15 @@
 
 # Python travelling library
 
 ![GitHub License](https://img.shields.io/github/license/diagmatrix/py-travel)
 ![Python ^3.10](https://img.shields.io/badge/Python-3.10%2B-blue)
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/diagmatrix/py-travel/commit.yml)
 ![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/diagmatrix/py-travel)
+![PyPI - Status](https://img.shields.io/pypi/status/py_travel)
 
 
 This is a Python library to use in conjunction with the 
 [Google Maps API](https://github.com/googlemaps/google-maps-services-python) (at least for now) in order to plan trips
 and much more! It tries to bring a less JSON-oriented way of using the API.
 
 ## Roadmap
@@ -37,22 +38,24 @@
 
 
 ## Getting started
 
 These instructions will get you a copy of the project up and running on your local machine for development and testing
 purposes.
 
-### Prerequisites
+### Local installation
+
+#### Prerequisites
 
 You will need the following:
 
  - Python >= 3.10
  - A Google Maps API key (for testing outside the testing environment)
 
-### Installing
+#### Installing
 
 For a local installation, just clone this repository inside the parent directory of your project.
 
 ````bash
 git clone https://github.com/diagmatrix/py-travel.git
 git checkout main
 ````
@@ -61,14 +64,23 @@
 
 ````bash
 pip install -r requirements.txt
 ````
 
 And there you have it! You can now use this library freely.
 
+### Installation
+
+This project is available in [PyPy](https://pypi.org/project/py-travel/), so you can install it using
+pip.
+
+````bash
+pip install py-travel
+````
+
 ## Usage
 
 There are currently two ways of using the classes provided in the package: by using the built-in
 Google Maps API clients or by using the `googlemaps` client directly. The first method will initialize an API client for
 each of the classes of **py-travel** that use them, while the second approach will give you more control on which ones
 can access it.
```

