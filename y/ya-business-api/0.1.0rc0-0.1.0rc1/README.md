# Comparing `tmp/ya_business_api-0.1.0rc0.tar.gz` & `tmp/ya_business_api-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ya_business_api-0.1.0rc0.tar", max compression
+gzip compressed data, was "ya_business_api-0.1.0rc1.tar", max compression
```

## Comparing `ya_business_api-0.1.0rc0.tar` & `ya_business_api-0.1.0rc1.tar`

### file list

```diff
@@ -1,25 +1,33 @@
--rw-r--r--   0        0        0     1070 2024-05-07 08:01:38.613562 ya_business_api-0.1.0rc0/LICENSE
--rw-r--r--   0        0        0     3575 2024-05-07 08:01:38.613562 ya_business_api-0.1.0rc0/README.md
--rw-r--r--   0        0        0      744 2024-05-07 08:01:38.613562 ya_business_api-0.1.0rc0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-07 08:01:38.617562 ya_business_api-0.1.0rc0/ya_business_api/__init__.py
--rw-r--r--   0        0        0     1002 2024-05-07 08:01:38.617562 ya_business_api-0.1.0rc0/ya_business_api/async_api.py
--rw-r--r--   0        0        0        0 2024-05-07 08:01:38.617562 ya_business_api-0.1.0rc0/ya_business_api/core/__init__.py
--rw-r--r--   0        0        0      243 2024-05-07 08:01:38.617562 ya_business_api-0.1.0rc0/ya_business_api/core/base_api.py
--rw-r--r--   0        0        0      346 2024-05-07 08:01:38.617562 ya_business_api-0.1.0rc0/ya_business_api/core/constants.py
--rw-r--r--   0        0        0      733 2024-05-07 08:01:38.617562 ya_business_api-0.1.0rc0/ya_business_api/core/dataclasses.py
--rw-r--r--   0        0        0      221 2024-05-07 08:01:38.617562 ya_business_api-0.1.0rc0/ya_business_api/core/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-07 08:01:38.617562 ya_business_api-0.1.0rc0/ya_business_api/core/mixins/__init__.py
--rw-r--r--   0        0        0      703 2024-05-07 08:01:38.617562 ya_business_api-0.1.0rc0/ya_business_api/core/mixins/asynchronous.py
--rw-r--r--   0        0        0      714 2024-05-07 08:01:38.617562 ya_business_api-0.1.0rc0/ya_business_api/core/mixins/synchronous.py
--rw-r--r--   0        0        0       47 2024-05-07 08:01:38.617562 ya_business_api-0.1.0rc0/ya_business_api/core/router.py
--rw-r--r--   0        0        0        0 2024-05-07 08:01:38.617562 ya_business_api-0.1.0rc0/ya_business_api/reviews/__init__.py
--rw-r--r--   0        0        0     2051 2024-05-07 08:01:38.617562 ya_business_api-0.1.0rc0/ya_business_api/reviews/async_api.py
--rw-r--r--   0        0        0      437 2024-05-07 08:01:38.617562 ya_business_api-0.1.0rc0/ya_business_api/reviews/base_api.py
--rw-r--r--   0        0        0      204 2024-05-07 08:01:38.617562 ya_business_api-0.1.0rc0/ya_business_api/reviews/constants.py
--rw-r--r--   0        0        0        0 2024-05-07 08:01:38.617562 ya_business_api-0.1.0rc0/ya_business_api/reviews/dataclasses/__init__.py
--rw-r--r--   0        0        0      585 2024-05-07 08:01:38.617562 ya_business_api-0.1.0rc0/ya_business_api/reviews/dataclasses/requests.py
--rw-r--r--   0        0        0     3939 2024-05-07 08:01:38.617562 ya_business_api-0.1.0rc0/ya_business_api/reviews/dataclasses/reviews.py
--rw-r--r--   0        0        0      393 2024-05-07 08:01:38.617562 ya_business_api-0.1.0rc0/ya_business_api/reviews/router.py
--rw-r--r--   0        0        0     2021 2024-05-07 08:01:38.617562 ya_business_api-0.1.0rc0/ya_business_api/reviews/sync_api.py
--rw-r--r--   0        0        0      936 2024-05-07 08:01:38.617562 ya_business_api-0.1.0rc0/ya_business_api/sync_api.py
--rw-r--r--   0        0        0     4338 1970-01-01 00:00:00.000000 ya_business_api-0.1.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-08 13:25:47.400904 ya_business_api-0.1.0rc1/LICENSE
+-rw-r--r--   0        0        0     4627 2024-05-08 13:25:47.400904 ya_business_api-0.1.0rc1/README.md
+-rw-r--r--   0        0        0      744 2024-05-08 13:25:47.404904 ya_business_api-0.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-08 13:25:47.404904 ya_business_api-0.1.0rc1/ya_business_api/__init__.py
+-rw-r--r--   0        0        0     1029 2024-05-08 13:25:47.404904 ya_business_api-0.1.0rc1/ya_business_api/async_api.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:25:47.404904 ya_business_api-0.1.0rc1/ya_business_api/companies/__init__.py
+-rw-r--r--   0        0        0      745 2024-05-08 13:25:47.404904 ya_business_api-0.1.0rc1/ya_business_api/companies/async_api.py
+-rw-r--r--   0        0        0      242 2024-05-08 13:25:47.404904 ya_business_api-0.1.0rc1/ya_business_api/companies/base_api.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:25:47.404904 ya_business_api-0.1.0rc1/ya_business_api/companies/dataclasses/__init__.py
+-rw-r--r--   0        0        0    10477 2024-05-08 13:25:47.404904 ya_business_api-0.1.0rc1/ya_business_api/companies/dataclasses/companies.py
+-rw-r--r--   0        0        0      325 2024-05-08 13:25:47.404904 ya_business_api-0.1.0rc1/ya_business_api/companies/dataclasses/requests.py
+-rw-r--r--   0        0        0      198 2024-05-08 13:25:47.404904 ya_business_api-0.1.0rc1/ya_business_api/companies/router.py
+-rw-r--r--   0        0        0      713 2024-05-08 13:25:47.404904 ya_business_api-0.1.0rc1/ya_business_api/companies/sync_api.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:25:47.404904 ya_business_api-0.1.0rc1/ya_business_api/core/__init__.py
+-rw-r--r--   0        0        0      243 2024-05-08 13:25:47.404904 ya_business_api-0.1.0rc1/ya_business_api/core/base_api.py
+-rw-r--r--   0        0        0      346 2024-05-08 13:25:47.404904 ya_business_api-0.1.0rc1/ya_business_api/core/constants.py
+-rw-r--r--   0        0        0     1151 2024-05-08 13:25:47.404904 ya_business_api-0.1.0rc1/ya_business_api/core/dataclasses.py
+-rw-r--r--   0        0        0      221 2024-05-08 13:25:47.408904 ya_business_api-0.1.0rc1/ya_business_api/core/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:25:47.408904 ya_business_api-0.1.0rc1/ya_business_api/core/mixins/__init__.py
+-rw-r--r--   0        0        0      703 2024-05-08 13:25:47.408904 ya_business_api-0.1.0rc1/ya_business_api/core/mixins/asynchronous.py
+-rw-r--r--   0        0        0      714 2024-05-08 13:25:47.408904 ya_business_api-0.1.0rc1/ya_business_api/core/mixins/synchronous.py
+-rw-r--r--   0        0        0       47 2024-05-08 13:25:47.408904 ya_business_api-0.1.0rc1/ya_business_api/core/router.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:25:47.408904 ya_business_api-0.1.0rc1/ya_business_api/reviews/__init__.py
+-rw-r--r--   0        0        0     1953 2024-05-08 13:25:47.408904 ya_business_api-0.1.0rc1/ya_business_api/reviews/async_api.py
+-rw-r--r--   0        0        0      347 2024-05-08 13:25:47.408904 ya_business_api-0.1.0rc1/ya_business_api/reviews/base_api.py
+-rw-r--r--   0        0        0      204 2024-05-08 13:25:47.408904 ya_business_api-0.1.0rc1/ya_business_api/reviews/constants.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:25:47.408904 ya_business_api-0.1.0rc1/ya_business_api/reviews/dataclasses/__init__.py
+-rw-r--r--   0        0        0      604 2024-05-08 13:25:47.408904 ya_business_api-0.1.0rc1/ya_business_api/reviews/dataclasses/requests.py
+-rw-r--r--   0        0        0     3637 2024-05-08 13:25:47.408904 ya_business_api-0.1.0rc1/ya_business_api/reviews/dataclasses/reviews.py
+-rw-r--r--   0        0        0      303 2024-05-08 13:25:47.408904 ya_business_api-0.1.0rc1/ya_business_api/reviews/router.py
+-rw-r--r--   0        0        0     1923 2024-05-08 13:25:47.408904 ya_business_api-0.1.0rc1/ya_business_api/reviews/sync_api.py
+-rw-r--r--   0        0        0      925 2024-05-08 13:25:47.408904 ya_business_api-0.1.0rc1/ya_business_api/sync_api.py
+-rw-r--r--   0        0        0     5390 1970-01-01 00:00:00.000000 ya_business_api-0.1.0rc1/PKG-INFO
```

### Comparing `ya_business_api-0.1.0rc0/LICENSE` & `ya_business_api-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ya_business_api-0.1.0rc0/README.md` & `ya_business_api-0.1.0rc1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -17,37 +17,34 @@
 ```python
 from ya_business_api.sync_api import SyncAPI		# Sync mode
 from ya_business_api.async_api import AsyncAPI		# Async mode
 
 
 def main() -> None:
 	api = SyncAPI.build(
-		permanent_id=...,
 		csrf_token=...,
 		session_id=...,
 		session_id2=...,
 	)
 
 	# Do things here...
 
 
 async def main() -> None:
 	api = await AsyncAPI.build(
-		permanent_id=...,
 		csrf_token=...,
 		session_id=...,
 		session_id2=...,
 	)
 
 	# Do things here...
 
 	await api.session.close()
 ```
 
-
 ### Where can I get the data for the client?
 On the reviews page (https://yandex.ru/sprav/.../edit/reviews), open the developer console (usually `F12`) from the first request, copy values of cookies (`Session_id` and `sessionid2`).
 
 In the console, run the following script:
 ```JS
 function getData() {
 	console.info({
@@ -59,46 +56,57 @@
 getData()
 
 /**
  * {CSRFToken: "...", PermanentId: 00000000000}
 */
 ```
 
+### ⚠️WARNING⚠️
+The `CSRFToken` and `PermanentId` belong to certain companies and cannot be used to respond to reviews from another company.
+
 ## Reviews
 ### Reviews fetching
 ```python
 # Sync mode
 from ya_business_api.sync_api import SyncAPI
+from ya_business_api.reviews.dataclasses.requests import ReviewsRequest
 
 
 api = SyncAPI.build(**kwargs)
-response = api.reviews.get_reviews()
+request = ReviewsRequest(permanent_id=<permanent_id>)
+response = api.reviews.get_reviews(request)
 
 # Async mode
 from ya_business_api.async_api import AsyncAPI
+from ya_business_api.reviews.dataclasses.requests import ReviewsRequest
 
 
 api = await AsyncAPI.build(**kwargs)
-response = await api.reviews.get_reviews()
+request = ReviewsRequest(permanent_id=<permanent_id>)
+response = await api.reviews.get_reviews(request)
 await api.session.close()
 ```
 
 #### Filtering and ordering
 ```python
 from ya_business_api.sync_api import SyncAPI
 from ya_business_api.reviews.dataclasses.requests import ReviewsRequest
 from ya_business_api.reviews.constants import Ranking
 
 
 api = SyncAPI.build(**kwargs)
-request = ReviewsRequest(ranking=Ranking.BY_RATING_DESC, unread=True, page=5)
+request = ReviewsRequest(
+	permanent_id=<permanent_id>,
+	ranking=Ranking.BY_RATING_DESC,
+	unread=True,
+	page=5,
+)
 response = api.reviews.get_reviews(request)
 ```
 
-
 ### Answering to reviews
 ```python
 # Sync mode
 from ya_business_api.sync_api import SyncAPI
 from ya_business_api.reviews.dataclasses.requests import AnswerRequest
 
 
@@ -125,14 +133,44 @@
 	reviews_csrf_token=reviews.list.csrf_token,
 	answer_csrf_token=reviews.list.items[0].business_answer_csrf_token,
 )
 response = await api.reviews.send_answer(request)
 await api.session.close()
 ```
 
+## Companies
+### Receiving companies
+```python
+# Sync mode
+from ya_business_api.sync_api import SyncAPI
+
+
+api = SyncAPI.build(**kwargs)
+response = api.companies.get_companies()
+
+# Async mode
+from ya_business_api.async_mode
+
+
+api = await AsyncAPI.build(**kwargs)
+response = await api.companies.get_companies()
+
+await api.session.close()
+```
+
+#### Filtering and pagination
+```python
+from ya_business_api.sync_api import SyncAPI
+from ya_business_api.companies.dataclasses.requests import CompaniesRequest
+
+
+api = SyncAPI.build(**kwargs)
+request = CompaniesRequest(filter="My Company", page=5)
+response = api.companies.get_companies(request)
+```
 
 ## Shortcuts
 ### Answers deleting
 ```python
 api.reviews.send_answer(AnswerRequest(text="", **kwargs))
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ya_business_api-0.1.0rc0/pyproject.toml` & `ya_business_api-0.1.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ya-business-api"
-version = "0.1.0-rc0"
+version = "0.1.0-rc1"
 description = "Yandex business API client"
 authors = ["Kirill_Lekhov <kirill.lekhov@mail.ru>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "ya_business_api"}]
 
 [tool.poetry.dependencies]
```

### Comparing `ya_business_api-0.1.0rc0/ya_business_api/async_api.py` & `ya_business_api-0.1.0rc1/ya_business_api/async_api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from ya_business_api.reviews.async_api import AsyncReviewsAPI
 from ya_business_api.core.constants import Cookie
+from ya_business_api.companies.async_api import AsyncCompaniesAPI
 
 from aiohttp.client import ClientSession
 
 
 class AsyncAPI:
-	permanent_id: int
 	reviews: AsyncReviewsAPI
+	companies: AsyncCompaniesAPI
 	session: ClientSession
 	csrf_token: str
 
-	def __init__(self, permanent_id: int, csrf_token: str, session: ClientSession) -> None:
-		self.permanent_id = permanent_id
+	def __init__(self, csrf_token: str, session: ClientSession) -> None:
 		self.csrf_token = csrf_token
 		self.session = session
-		self.reviews = AsyncReviewsAPI(permanent_id, csrf_token, session)
+		self.reviews = AsyncReviewsAPI(csrf_token, session)
+		self.companies = AsyncCompaniesAPI(self.session)
 
 	@classmethod
-	async def build(cls, permanent_id: int, csrf_token: str, session_id: str, session_id2: str) -> "AsyncAPI":
+	async def build(cls, csrf_token: str, session_id: str, session_id2: str) -> "AsyncAPI":
 		session = await cls.make_session(session_id, session_id2)
-		return cls(permanent_id, csrf_token, session)
+		return cls(csrf_token, session)
 
 	@staticmethod
 	async def make_session(session_id: str, session_id2: str) -> ClientSession:
 		session = ClientSession()
 		session.cookie_jar.update_cookies({
 			Cookie.SESSION_ID.value: session_id,
 			Cookie.SESSION_ID2.value: session_id2,
```

### Comparing `ya_business_api-0.1.0rc0/ya_business_api/core/mixins/asynchronous.py` & `ya_business_api-0.1.0rc1/ya_business_api/core/mixins/asynchronous.py`

 * *Files identical despite different names*

### Comparing `ya_business_api-0.1.0rc0/ya_business_api/core/mixins/synchronous.py` & `ya_business_api-0.1.0rc1/ya_business_api/core/mixins/synchronous.py`

 * *Files identical despite different names*

### Comparing `ya_business_api-0.1.0rc0/ya_business_api/reviews/async_api.py` & `ya_business_api-0.1.0rc1/ya_business_api/reviews/async_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,26 +3,24 @@
 from ya_business_api.reviews.base_api import BaseReviewsAPI
 from ya_business_api.reviews.constants import SUCCESS_ANSWER_RESPONSE
 from ya_business_api.reviews.dataclasses.reviews import ReviewsResponse
 from ya_business_api.reviews.dataclasses.requests import AnswerRequest, ReviewsRequest
 
 from time import monotonic
 from logging import getLogger; log = getLogger(__name__)
-from typing import Optional
 
 from aiohttp.client import ClientSession
 
 
 class AsyncReviewsAPI(AsyncAPIMixin, BaseReviewsAPI):
-	def __init__(self, permanent_id: int, csrf_token: str, session: ClientSession) -> None:
-		super().__init__(session, permanent_id, csrf_token)
+	def __init__(self, csrf_token: str, session: ClientSession) -> None:
+		super().__init__(session, csrf_token)
 
-	async def get_reviews(self, request: Optional[ReviewsRequest] = None) -> ReviewsResponse:
-		url = self.router.reviews()
-		request = request or ReviewsRequest()
+	async def get_reviews(self, request: ReviewsRequest) -> ReviewsResponse:
+		url = self.router.reviews(request.permanent_id)
 		time_start = monotonic()
 
 		async with self.session.get(url, params=request.as_query_params(), allow_redirects=False) as response:
 			log.debug(f"A:REVIEWS[{response.status}] {monotonic() - time_start:.1f}s")
 			self.check_response(response)
 			response = ReviewsResponse.from_dict(await response.json())
```

### Comparing `ya_business_api-0.1.0rc0/ya_business_api/reviews/dataclasses/requests.py` & `ya_business_api-0.1.0rc1/ya_business_api/reviews/dataclasses/requests.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 	text: str
 	reviews_csrf_token: str
 	answer_csrf_token: str
 
 
 @dataclass
 class ReviewsRequest(ValidatedMixin):
+	permanent_id: int
 	ranking: Ranking = Ranking.BY_TIME
 	unread: bool = False
 	page: int = 1
 	# aspectId: ???
 
 	def as_query_params(self) -> dict:
 		params = {"ranking": self.ranking.value, "page": self.page}
```

### Comparing `ya_business_api-0.1.0rc0/ya_business_api/reviews/sync_api.py` & `ya_business_api-0.1.0rc1/ya_business_api/reviews/sync_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,26 +2,24 @@
 from ya_business_api.core.constants import Cookie
 from ya_business_api.reviews.base_api import BaseReviewsAPI
 from ya_business_api.reviews.constants import SUCCESS_ANSWER_RESPONSE
 from ya_business_api.reviews.dataclasses.reviews import ReviewsResponse
 from ya_business_api.reviews.dataclasses.requests import AnswerRequest, ReviewsRequest
 
 from logging import getLogger; log = getLogger(__name__)
-from typing import Optional
 
 from requests.sessions import Session
 
 
 class SyncReviewsAPI(SyncAPIMixin, BaseReviewsAPI):
-	def __init__(self, permanent_id: int, csrf_token: str, session: Session) -> None:
-		super().__init__(session, permanent_id, csrf_token)
+	def __init__(self, csrf_token: str, session: Session) -> None:
+		super().__init__(session, csrf_token)
 
-	def get_reviews(self, request: Optional[ReviewsRequest] = None) -> ReviewsResponse:
-		url = self.router.reviews()
-		request = request or ReviewsRequest()
+	def get_reviews(self, request: ReviewsRequest) -> ReviewsResponse:
+		url = self.router.reviews(request.permanent_id)
 		response = self.session.get(url, params=request.as_query_params(), allow_redirects=False)
 		log.debug(f"REVIEWS[{response.status_code}] {response.elapsed.total_seconds()}s")
 		self.check_response(response)
 
 		return ReviewsResponse.from_dict(response.json())
 
 	def send_answer(self, request: AnswerRequest) -> bool:
```

### Comparing `ya_business_api-0.1.0rc0/ya_business_api/sync_api.py` & `ya_business_api-0.1.0rc1/ya_business_api/sync_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from ya_business_api.reviews.sync_api import SyncReviewsAPI
+from ya_business_api.companies.sync_api import SyncCompaniesAPI
 from ya_business_api.core.constants import Cookie
 
 from requests.sessions import Session
 
 
 class SyncAPI:
-	permanent_id: int
 	reviews: SyncReviewsAPI
 	session: Session
 	csrf_token: str
 
-	def __init__(self, permanent_id: int, csrf_token: str, session: Session) -> None:
-		self.permanent_id = permanent_id
+	def __init__(self, csrf_token: str, session: Session) -> None:
 		self.csrf_token = csrf_token
 		self.session = session
-		self.reviews = SyncReviewsAPI(permanent_id, csrf_token, session)
+		self.reviews = SyncReviewsAPI(csrf_token, session)
+		self.companies = SyncCompaniesAPI(session)
 
 	@classmethod
-	def build(cls, permanent_id: int, csrf_token: str, session_id: str, session_id2: str) -> "SyncAPI":
+	def build(cls, csrf_token: str, session_id: str, session_id2: str) -> "SyncAPI":
 		session = cls.make_session(session_id, session_id2)
-		return cls(permanent_id, csrf_token, session)
+		return cls(csrf_token, session)
 
 	@staticmethod
 	def make_session(session_id, session_id2) -> Session:
 		session = Session()
 		session.cookies.set(Cookie.SESSION_ID.value, session_id)
 		session.cookies.set(Cookie.SESSION_ID2.value, session_id2)
```

### Comparing `ya_business_api-0.1.0rc0/PKG-INFO` & `ya_business_api-0.1.0rc1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ya-business-api
-Version: 0.1.0rc0
+Version: 0.1.0rc1
 Summary: Yandex business API client
 License: MIT
 Author: Kirill_Lekhov
 Author-email: kirill.lekhov@mail.ru
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -38,37 +38,34 @@
 ```python
 from ya_business_api.sync_api import SyncAPI		# Sync mode
 from ya_business_api.async_api import AsyncAPI		# Async mode
 
 
 def main() -> None:
 	api = SyncAPI.build(
-		permanent_id=...,
 		csrf_token=...,
 		session_id=...,
 		session_id2=...,
 	)
 
 	# Do things here...
 
 
 async def main() -> None:
 	api = await AsyncAPI.build(
-		permanent_id=...,
 		csrf_token=...,
 		session_id=...,
 		session_id2=...,
 	)
 
 	# Do things here...
 
 	await api.session.close()
 ```
 
-
 ### Where can I get the data for the client?
 On the reviews page (https://yandex.ru/sprav/.../edit/reviews), open the developer console (usually `F12`) from the first request, copy values of cookies (`Session_id` and `sessionid2`).
 
 In the console, run the following script:
 ```JS
 function getData() {
 	console.info({
@@ -80,46 +77,57 @@
 getData()
 
 /**
  * {CSRFToken: "...", PermanentId: 00000000000}
 */
 ```
 
+### ⚠️WARNING⚠️
+The `CSRFToken` and `PermanentId` belong to certain companies and cannot be used to respond to reviews from another company.
+
 ## Reviews
 ### Reviews fetching
 ```python
 # Sync mode
 from ya_business_api.sync_api import SyncAPI
+from ya_business_api.reviews.dataclasses.requests import ReviewsRequest
 
 
 api = SyncAPI.build(**kwargs)
-response = api.reviews.get_reviews()
+request = ReviewsRequest(permanent_id=<permanent_id>)
+response = api.reviews.get_reviews(request)
 
 # Async mode
 from ya_business_api.async_api import AsyncAPI
+from ya_business_api.reviews.dataclasses.requests import ReviewsRequest
 
 
 api = await AsyncAPI.build(**kwargs)
-response = await api.reviews.get_reviews()
+request = ReviewsRequest(permanent_id=<permanent_id>)
+response = await api.reviews.get_reviews(request)
 await api.session.close()
 ```
 
 #### Filtering and ordering
 ```python
 from ya_business_api.sync_api import SyncAPI
 from ya_business_api.reviews.dataclasses.requests import ReviewsRequest
 from ya_business_api.reviews.constants import Ranking
 
 
 api = SyncAPI.build(**kwargs)
-request = ReviewsRequest(ranking=Ranking.BY_RATING_DESC, unread=True, page=5)
+request = ReviewsRequest(
+	permanent_id=<permanent_id>,
+	ranking=Ranking.BY_RATING_DESC,
+	unread=True,
+	page=5,
+)
 response = api.reviews.get_reviews(request)
 ```
 
-
 ### Answering to reviews
 ```python
 # Sync mode
 from ya_business_api.sync_api import SyncAPI
 from ya_business_api.reviews.dataclasses.requests import AnswerRequest
 
 
@@ -146,14 +154,44 @@
 	reviews_csrf_token=reviews.list.csrf_token,
 	answer_csrf_token=reviews.list.items[0].business_answer_csrf_token,
 )
 response = await api.reviews.send_answer(request)
 await api.session.close()
 ```
 
+## Companies
+### Receiving companies
+```python
+# Sync mode
+from ya_business_api.sync_api import SyncAPI
+
+
+api = SyncAPI.build(**kwargs)
+response = api.companies.get_companies()
+
+# Async mode
+from ya_business_api.async_mode
+
+
+api = await AsyncAPI.build(**kwargs)
+response = await api.companies.get_companies()
+
+await api.session.close()
+```
+
+#### Filtering and pagination
+```python
+from ya_business_api.sync_api import SyncAPI
+from ya_business_api.companies.dataclasses.requests import CompaniesRequest
+
+
+api = SyncAPI.build(**kwargs)
+request = CompaniesRequest(filter="My Company", page=5)
+response = api.companies.get_companies(request)
+```
 
 ## Shortcuts
 ### Answers deleting
 ```python
 api.reviews.send_answer(AnswerRequest(text="", **kwargs))
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

