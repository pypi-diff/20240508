# Comparing `tmp/delphai_fastapi-3.0.2.tar.gz` & `tmp/delphai_fastapi-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delphai_fastapi-3.0.2.tar", max compression
+gzip compressed data, was "delphai_fastapi-3.0.3.tar", max compression
```

## Comparing `delphai_fastapi-3.0.2.tar` & `delphai_fastapi-3.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       86 2024-03-28 16:11:19.358566 delphai_fastapi-3.0.2/delphai_fastapi/__init__.py
--rw-r--r--   0        0        0     2652 2024-03-28 16:11:19.358566 delphai_fastapi-3.0.2/delphai_fastapi/app.py
--rw-r--r--   0        0        0     5713 2024-03-28 16:11:19.358566 delphai_fastapi-3.0.2/delphai_fastapi/auth.py
--rw-r--r--   0        0        0        0 2024-03-28 16:11:19.358566 delphai_fastapi-3.0.2/delphai_fastapi/companies/__init__.py
--rw-r--r--   0        0        0     5582 2024-03-28 16:11:19.358566 delphai_fastapi-3.0.2/delphai_fastapi/companies/models.py
--rw-r--r--   0        0        0      375 2024-03-28 16:11:19.358566 delphai_fastapi-3.0.2/delphai_fastapi/decorators.py
--rw-r--r--   0        0        0        0 2024-03-28 16:11:19.358566 delphai_fastapi-3.0.2/delphai_fastapi/funding_rounds/__init__.py
--rw-r--r--   0        0        0     1623 2024-03-28 16:11:19.358566 delphai_fastapi-3.0.2/delphai_fastapi/funding_rounds/models.py
--rw-r--r--   0        0        0     1314 2024-03-28 16:11:19.358566 delphai_fastapi-3.0.2/delphai_fastapi/instrumentation.py
--rw-r--r--   0        0        0        0 2024-03-28 16:11:19.358566 delphai_fastapi-3.0.2/delphai_fastapi/job_posts/__init__.py
--rw-r--r--   0        0        0     1485 2024-03-28 16:11:19.358566 delphai_fastapi-3.0.2/delphai_fastapi/job_posts/models.py
--rw-r--r--   0        0        0     1386 2024-03-28 16:11:19.358566 delphai_fastapi-3.0.2/delphai_fastapi/models.py
--rw-r--r--   0        0        0        0 2024-03-28 16:11:19.358566 delphai_fastapi-3.0.2/delphai_fastapi/news_articles/__init__.py
--rw-r--r--   0        0        0     1120 2024-03-28 16:11:19.358566 delphai_fastapi-3.0.2/delphai_fastapi/news_articles/models.py
--rw-r--r--   0        0        0        0 2024-03-28 16:11:19.362566 delphai_fastapi-3.0.2/delphai_fastapi/projects/__init__.py
--rw-r--r--   0        0        0     1523 2024-03-28 16:11:19.362566 delphai_fastapi-3.0.2/delphai_fastapi/projects/models.py
--rw-r--r--   0        0        0      405 2024-03-28 16:11:19.362566 delphai_fastapi-3.0.2/delphai_fastapi/server.py
--rw-r--r--   0        0        0     2909 2024-03-28 16:11:19.362566 delphai_fastapi-3.0.2/delphai_fastapi/types.py
--rw-r--r--   0        0        0      590 2024-03-28 16:11:19.362566 delphai_fastapi-3.0.2/pyproject.toml
--rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 delphai_fastapi-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0       86 2024-05-08 08:29:26.428718 delphai_fastapi-3.0.3/delphai_fastapi/__init__.py
+-rw-r--r--   0        0        0     2652 2024-05-08 08:29:26.428718 delphai_fastapi-3.0.3/delphai_fastapi/app.py
+-rw-r--r--   0        0        0     5713 2024-05-08 08:29:26.428718 delphai_fastapi-3.0.3/delphai_fastapi/auth.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:29:26.428718 delphai_fastapi-3.0.3/delphai_fastapi/companies/__init__.py
+-rw-r--r--   0        0        0     5582 2024-05-08 08:29:26.428718 delphai_fastapi-3.0.3/delphai_fastapi/companies/models.py
+-rw-r--r--   0        0        0      375 2024-05-08 08:29:26.428718 delphai_fastapi-3.0.3/delphai_fastapi/decorators.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:29:26.428718 delphai_fastapi-3.0.3/delphai_fastapi/funding_rounds/__init__.py
+-rw-r--r--   0        0        0     1623 2024-05-08 08:29:26.428718 delphai_fastapi-3.0.3/delphai_fastapi/funding_rounds/models.py
+-rw-r--r--   0        0        0     1314 2024-05-08 08:29:26.428718 delphai_fastapi-3.0.3/delphai_fastapi/instrumentation.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:29:26.428718 delphai_fastapi-3.0.3/delphai_fastapi/job_posts/__init__.py
+-rw-r--r--   0        0        0     2820 2024-05-08 08:29:26.432718 delphai_fastapi-3.0.3/delphai_fastapi/job_posts/models.py
+-rw-r--r--   0        0        0     1386 2024-05-08 08:29:26.432718 delphai_fastapi-3.0.3/delphai_fastapi/models.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:29:26.432718 delphai_fastapi-3.0.3/delphai_fastapi/news_articles/__init__.py
+-rw-r--r--   0        0        0     1120 2024-05-08 08:29:26.432718 delphai_fastapi-3.0.3/delphai_fastapi/news_articles/models.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:29:26.432718 delphai_fastapi-3.0.3/delphai_fastapi/projects/__init__.py
+-rw-r--r--   0        0        0     1523 2024-05-08 08:29:26.432718 delphai_fastapi-3.0.3/delphai_fastapi/projects/models.py
+-rw-r--r--   0        0        0      405 2024-05-08 08:29:26.432718 delphai_fastapi-3.0.3/delphai_fastapi/server.py
+-rw-r--r--   0        0        0     2909 2024-05-08 08:29:26.432718 delphai_fastapi-3.0.3/delphai_fastapi/types.py
+-rw-r--r--   0        0        0      590 2024-05-08 08:29:26.432718 delphai_fastapi-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 delphai_fastapi-3.0.3/PKG-INFO
```

### Comparing `delphai_fastapi-3.0.2/delphai_fastapi/app.py` & `delphai_fastapi-3.0.3/delphai_fastapi/app.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.2/delphai_fastapi/auth.py` & `delphai_fastapi-3.0.3/delphai_fastapi/auth.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.2/delphai_fastapi/companies/models.py` & `delphai_fastapi-3.0.3/delphai_fastapi/companies/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.2/delphai_fastapi/funding_rounds/models.py` & `delphai_fastapi-3.0.3/delphai_fastapi/funding_rounds/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.2/delphai_fastapi/instrumentation.py` & `delphai_fastapi-3.0.3/delphai_fastapi/instrumentation.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.2/delphai_fastapi/job_posts/models.py` & `delphai_fastapi-3.0.3/delphai_fastapi/job_posts/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,31 +10,64 @@
 class JobDescription(CamelModel):
     default: str = Field(..., description="Description of the postion")
     original: Optional[str] = Field(
         None, description="Original description of the position"
     )
 
 
-class JobPost(CamelModel):
-    job_post_id: ObjectId = Field(..., description="Internal job post ID")
-    company_id: ObjectId = Field(..., description="Internal company ID")
+class JobClassification(CamelModel):
+    isco_code: int = Field(..., description="ISCO code of the position")
+    delphai_label: str = Field(..., description="Delphai label of the position")
+
+
+class BaseJobPost(CamelModel):
     url: str = Field(..., description="Job post URL")
     published: datetime = Field(..., description="When the job post was published")
+    title: str = Field(..., description="Position title")
     location: Optional[str] = Field(None, description="Location of the position")
-    job_description: Optional[str] = Field(
-        None, description="Description of the position"
-    )
     language: Optional[str] = Field(
         None, description="Original language of the job post"
     )
-    title: str = Field(..., description="Position title")
-    added: datetime = Field(..., description="When the job post was added to delphai")
     deactivated: Optional[datetime] = Field(
         None, description="When the job post deactivated"
     )
+
+
+class JobPost(BaseJobPost):
+    job_post_id: ObjectId = Field(..., description="Internal job post ID")
+    company_id: ObjectId = Field(..., description="Internal company ID")
+    added: datetime = Field(..., description="When the job post was added to delphai")
     is_active: bool = Field(..., description="Whether the job post is active or not")
+    job_description: Optional[str] = Field(
+        None, description="Description of the position"
+    )
     description: Optional[JobDescription] = None
+    classifications: Optional[List[JobClassification]] = None
+
+
+class AddJobPost(BaseJobPost):
+    company_id: ObjectId = Field(None, description="Internal company ID")
+    original_description: Optional[str] = Field(
+        None, description="Description in original language"
+    )
+    translated_description: Optional[str] = Field(
+        None,
+        description="Translated description in english. Only necessary if original language is not english",
+    )
+    html_blob_reference: Optional[str] = Field(
+        None, description="Reference to the blob that stores the HTML of the job post"
+    )
+    name_matched: Optional[bool] = Field(
+        None,
+        description="Whether the company of the job post was assigned using the names-matcher",
+    )
+    company_url: Optional[str] = Field(
+        None, description="URL of the company posting the job post"
+    )
+    country: Optional[str] = Field(None, description="Country of the position")
+    state: Optional[str] = Field(None, description="State of the position")
+    city: Optional[str] = Field(None, description="City of the position")
 
 
 class JobPosts(CamelModel):
     results: List[JobPost]
     total: int = Field(..., description="Number of results")
```

### Comparing `delphai_fastapi-3.0.2/delphai_fastapi/models.py` & `delphai_fastapi-3.0.3/delphai_fastapi/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.2/delphai_fastapi/news_articles/models.py` & `delphai_fastapi-3.0.3/delphai_fastapi/news_articles/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.2/delphai_fastapi/projects/models.py` & `delphai_fastapi-3.0.3/delphai_fastapi/projects/models.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.2/delphai_fastapi/types.py` & `delphai_fastapi-3.0.3/delphai_fastapi/types.py`

 * *Files identical despite different names*

### Comparing `delphai_fastapi-3.0.2/pyproject.toml` & `delphai_fastapi-3.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "delphai-fastapi"
-version = "3.0.2"
+version = "3.0.3"
 description = "Package for fastAPI models"
 authors = ["Berinike Tech <berinike@delphai.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fastapi = "^0"
 pymongo = ">3"
```

### Comparing `delphai_fastapi-3.0.2/PKG-INFO` & `delphai_fastapi-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delphai-fastapi
-Version: 3.0.2
+Version: 3.0.3
 Summary: Package for fastAPI models
 Author: Berinike Tech
 Author-email: berinike@delphai.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

