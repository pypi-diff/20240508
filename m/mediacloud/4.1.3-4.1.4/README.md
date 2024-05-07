# Comparing `tmp/mediacloud-4.1.3.tar.gz` & `tmp/mediacloud-4.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediacloud-4.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mediacloud-4.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mediacloud-4.1.3.tar` & `mediacloud-4.1.4.tar`

### file list

```diff
@@ -1,23 +1,15 @@
--rw-r--r--   0        0        0      135 2023-12-12 19:22:48.146813 mediacloud-4.1.3/.flake8
--rw-r--r--   0        0        0      645 2023-12-23 20:05:11.608768 mediacloud-4.1.3/.github/workflows/pytest.yml
--rw-r--r--   0        0        0       87 2022-02-12 02:08:18.629678 mediacloud-4.1.3/.gitignore
--rw-r--r--   0        0        0      683 2023-12-12 19:22:48.152524 mediacloud-4.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0       13 2022-02-12 02:08:18.629922 mediacloud-4.1.3/.python-version
--rw-r--r--   0        0        0       92 2022-12-15 15:47:58.429996 mediacloud-4.1.3/.travis.yml
--rw-r--r--   0        0        0     8736 2024-02-06 20:39:13.376320 mediacloud-4.1.3/CHANGELOG.md
--rw-r--r--   0        0        0    11358 2023-12-04 20:09:33.162065 mediacloud-4.1.3/LICENSE
--rw-r--r--   0        0        0     3305 2024-02-01 13:42:29.505109 mediacloud-4.1.3/README.md
--rwxr-xr-x   0        0        0        0 2023-12-12 19:22:48.153502 mediacloud-4.1.3/mediacloud/__init__.py
--rw-r--r--   0        0        0     9029 2024-02-06 20:35:25.109657 mediacloud-4.1.3/mediacloud/api.py
--rw-r--r--   0        0        0      679 2023-12-11 18:46:40.183455 mediacloud-4.1.3/mediacloud/error.py
--rwxr-xr-x   0        0        0       99 2022-12-15 15:47:58.431704 mediacloud-4.1.3/mediacloud/test/__init__.py
--rw-r--r--   0        0        0      613 2023-12-12 19:22:48.156127 mediacloud-4.1.3/mediacloud/test/api_base_test.py
--rw-r--r--   0        0        0     3926 2024-01-23 20:46:30.613727 mediacloud-4.1.3/mediacloud/test/api_directory_test.py
--rw-r--r--   0        0        0    10526 2024-02-06 20:44:56.059625 mediacloud-4.1.3/mediacloud/test/api_search_test.py
--rw-r--r--   0        0        0     5897 2022-02-12 02:08:18.632429 mediacloud-4.1.3/mediacloud/test/fixtures/sample_story_ap.txt
--rw-r--r--   0        0        0     2907 2022-02-12 02:08:18.632535 mediacloud-4.1.3/mediacloud/test/fixtures/sample_story_not_ap.txt
--rw-r--r--   0        0        0    10007 2022-02-12 02:08:18.632650 mediacloud-4.1.3/mediacloud/test/fixtures/sentences_by_story_1.json
--rw-r--r--   0        0        0    10165 2022-02-12 02:08:18.632746 mediacloud-4.1.3/mediacloud/test/fixtures/sentences_by_story_2.json
--rw-r--r--   0        0        0     3064 2022-02-12 02:08:18.632828 mediacloud-4.1.3/mediacloud/test/fixtures/story_27456565.json
--rw-r--r--   0        0        0      922 2024-02-06 20:39:13.376602 mediacloud-4.1.3/pyproject.toml
--rw-r--r--   0        0        0     4347 1970-01-01 00:00:00.000000 mediacloud-4.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3305 2024-05-07 22:21:09.115739 mediacloud-4.1.4/README.md
+-rwxr-xr-x   0        0        0        0 2024-05-07 22:21:09.115739 mediacloud-4.1.4/mediacloud/__init__.py
+-rw-r--r--   0        0        0     8902 2024-05-07 22:21:09.115739 mediacloud-4.1.4/mediacloud/api.py
+-rw-r--r--   0        0        0      679 2024-05-07 22:21:09.115739 mediacloud-4.1.4/mediacloud/error.py
+-rwxr-xr-x   0        0        0       99 2024-05-07 22:21:09.115739 mediacloud-4.1.4/mediacloud/test/__init__.py
+-rw-r--r--   0        0        0      613 2024-05-07 22:21:09.115739 mediacloud-4.1.4/mediacloud/test/api_base_test.py
+-rw-r--r--   0        0        0     3926 2024-05-07 22:21:09.115739 mediacloud-4.1.4/mediacloud/test/api_directory_test.py
+-rw-r--r--   0        0        0    13266 2024-05-07 22:21:09.115739 mediacloud-4.1.4/mediacloud/test/api_search_test.py
+-rw-r--r--   0        0        0     5897 2024-05-07 22:21:09.115739 mediacloud-4.1.4/mediacloud/test/fixtures/sample_story_ap.txt
+-rw-r--r--   0        0        0     2907 2024-05-07 22:21:09.115739 mediacloud-4.1.4/mediacloud/test/fixtures/sample_story_not_ap.txt
+-rw-r--r--   0        0        0    10007 2024-05-07 22:21:09.115739 mediacloud-4.1.4/mediacloud/test/fixtures/sentences_by_story_1.json
+-rw-r--r--   0        0        0    10165 2024-05-07 22:21:09.115739 mediacloud-4.1.4/mediacloud/test/fixtures/sentences_by_story_2.json
+-rw-r--r--   0        0        0     3064 2024-05-07 22:21:09.115739 mediacloud-4.1.4/mediacloud/test/fixtures/story_27456565.json
+-rw-r--r--   0        0        0      922 2024-05-07 22:21:09.115739 mediacloud-4.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4347 1970-01-01 00:00:00.000000 mediacloud-4.1.4/PKG-INFO
```

### Comparing `mediacloud-4.1.3/README.md` & `mediacloud-4.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mediacloud-4.1.3/mediacloud/api.py` & `mediacloud-4.1.4/mediacloud/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 class SearchApi(BaseApi):
     PROVIDER = "onlinenews-mediacloud"
 
     def _prep_default_params(self, query: str, start_date: dt.date, end_date: dt.date,
                              collection_ids: Optional[List[int]] = [], source_ids: Optional[List[int]] = [],
                              platform: Optional[str] = None):
         params: Dict[Any, Any] = dict(start=start_date.isoformat(), end=end_date.isoformat(), q=query,
-                                      platform=self.PROVIDER)
+                                      platform=(platform or self.PROVIDER))
         if len(source_ids):
             params['ss'] = ",".join([str(sid) for sid in source_ids]),
         if len(collection_ids):
             params['cs'] = ",".join([str(cid) for cid in collection_ids]),
         return params
 
     def story_count(self, query: str, start_date: dt.date, end_date: dt.date, collection_ids: Optional[List[int]] = [],
@@ -136,32 +136,29 @@
         for d in results['count_over_time']['counts']:
             d['date'] = dt.date.fromisoformat(d['date'][:10])
         return results['count_over_time']['counts']
 
     def story_list(self, query: str, start_date: dt.date, end_date: dt.date, collection_ids: Optional[List[int]] = [],
                    source_ids: Optional[List[int]] = [], platform: Optional[str] = None,
                    expanded: Optional[bool] = None, pagination_token: Optional[str] = None,
-                   sort_field: Optional[str] = None, sort_order: Optional[str] = None,
+                   sort_order: Optional[str] = None,
                    page_size: Optional[int] = None) -> tuple[List[Dict], Optional[str]]:
         params = self._prep_default_params(query, start_date, end_date, collection_ids, source_ids, platform)
         if expanded:
             params['expanded'] = 1
         if pagination_token:
             params['pagination_token'] = pagination_token
-        if sort_field:
-            params['sort_field'] = sort_field
         if sort_order:
             params['sort_order'] = sort_order
         if page_size:
             params['page_size'] = page_size
         results = self._query('search/story-list', params)
         for s in results['stories']:
             s['publish_date'] = dt.date.fromisoformat(s['publish_date'][:10]) if s['publish_date'] else None
-            s['indexed_date'] = dt.datetime.strptime(s['indexed_date'][:19], '%Y-%m-%d %H:%M:%S')\
-                if s['indexed_date'] else None
+            s['indexed_date'] = dt.datetime.fromisoformat(s['indexed_date']) if s['indexed_date'] else None
         return results['stories'], results['pagination_token']
 
     def story(self, story_id: str) -> Dict:
         params = dict(storyId=story_id, platform=self.PROVIDER)
         results = self._query('search/story', params)
         return results['story']
```

### Comparing `mediacloud-4.1.3/mediacloud/error.py` & `mediacloud-4.1.4/mediacloud/error.py`

 * *Files identical despite different names*

### Comparing `mediacloud-4.1.3/mediacloud/test/api_base_test.py` & `mediacloud-4.1.4/mediacloud/test/api_base_test.py`

 * *Files identical despite different names*

### Comparing `mediacloud-4.1.3/mediacloud/test/api_directory_test.py` & `mediacloud-4.1.4/mediacloud/test/api_directory_test.py`

 * *Files identical despite different names*

### Comparing `mediacloud-4.1.3/mediacloud/test/api_search_test.py` & `mediacloud-4.1.4/mediacloud/test/api_search_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 import os
 from unittest import TestCase
 
 import mediacloud.api
 
 COLLECTION_US_NATIONAL = 34412234
 AU_BROADCAST_COMPANY = 20775
-TOMORROW = dt.date.today() + dt.timedelta(days=1)
 TOMORROW_TIME = dt.datetime.today() + dt.timedelta(days=1)
 
 
-class DirectoryTest(TestCase):
+class SearchTest(TestCase):
 
     START_DATE = dt.date(2023, 11, 1)
     END_DATE = dt.date(2023, 12, 1)
 
     def setUp(self):
         self._mc_api_key = os.getenv("MC_API_TOKEN")
         self._search = mediacloud.api.SearchApi(self._mc_api_key)
+        self._mc_api_admin_key = os.getenv("MC_API_ADMIN_TOKEN")
+        self._admin_search = mediacloud.api.SearchApi(self._mc_api_admin_key)
 
     def test_story_count(self):
         results = self._search.story_count(query="weather", start_date=self.START_DATE, end_date=self.END_DATE,
                                            collection_ids=[COLLECTION_US_NATIONAL], source_ids=[AU_BROADCAST_COMPANY])
         assert 'relevant' in results
         assert results['relevant'] > 0
         assert 'total' in results
@@ -39,15 +40,15 @@
             assert 'total_count' in day
             assert day['count'] <= day['total_count']
             assert 'ratio' in day
             assert day['ratio'] < 1
 
     def test_story(self):
         # Note: Expected to fail right now
-        story_id = 'eebfb686618e34a9bc6e87e87e90c54b'  # not sure this is a valid id
+        story_id = '9f734354744a651e9b99e4fcd93ee9eaee12ed134ba74dcda13b30234f528535'
         story = self._search.story(story_id)
         assert 'id' in story
         assert story['id'] == story_id
         assert 'title' in story
         assert 'url' in story
         assert 'language' in story
         assert 'publish_date' in story
@@ -100,59 +101,41 @@
                                                              pagination_token=next_page_token1)
         assert len(results2) == 1000
         assert next_page_token2 is not None
         assert next_page_token1 != next_page_token2
 
     def test_story_list_expanded(self):
         # note - requires staff API token
-        page, _ = self._search.story_list(query="weather", start_date=self.START_DATE, end_date=self.END_DATE,
-                                          collection_ids=[COLLECTION_US_NATIONAL])
+        page, _ = self._admin_search.story_list(query="weather", start_date=self.START_DATE, end_date=self.END_DATE,
+                                                collection_ids=[COLLECTION_US_NATIONAL])
         for story in page:
             assert 'text' not in story
-        page, _ = self._search.story_list(query="weather", start_date=self.START_DATE, end_date=self.END_DATE,
-                                          expanded=True, collection_ids=[COLLECTION_US_NATIONAL])
+        page, _ = self._admin_search.story_list(query="weather", start_date=self.START_DATE, end_date=self.END_DATE,
+                                                expanded=True, collection_ids=[COLLECTION_US_NATIONAL])
         for story in page:
             assert 'text' in story
             assert len(story['text']) > 0
 
     def test_story_list_sort_order(self):
         # desc
         page, _ = self._search.story_list(query="weather", start_date=self.START_DATE, end_date=self.END_DATE,
                                           collection_ids=[COLLECTION_US_NATIONAL])
-        last_pub_date = TOMORROW
+        last_date = TOMORROW_TIME
         for story in page:
-            assert 'publish_date' in story
-            assert story['publish_date'] <= last_pub_date
-            last_pub_date = story['publish_date']
+            assert 'indexed_date' in story
+            assert story['indexed_date'] <= last_date
+            last_date = story['indexed_date']
         # asc
         page, _ = self._search.story_list(query="weather", start_date=self.START_DATE, end_date=self.END_DATE,
                                           collection_ids=[COLLECTION_US_NATIONAL], sort_order='asc')
-        a_long_time_ago = dt.date(2000, 1, 1)
-        last_pub_date = a_long_time_ago
-        for story in page:
-            assert 'publish_date' in story
-            assert story['publish_date'] >= last_pub_date
-            last_pub_date = story['publish_date']
-
-    def test_story_list_sort_field(self):
-        # publish_date
-        page, _ = self._search.story_list(query="weather", start_date=self.START_DATE, end_date=self.END_DATE,
-                                          collection_ids=[COLLECTION_US_NATIONAL])
-        last_date = TOMORROW
-        for story in page:
-            assert 'publish_date' in story
-            assert story['publish_date'] <= last_date
-            last_date = story['publish_date']
-        # indexed date
-        page, _ = self._search.story_list(query="weather", start_date=self.START_DATE, end_date=self.END_DATE,
-                                          collection_ids=[COLLECTION_US_NATIONAL], sort_field="indexed_date")
-        last_date = TOMORROW_TIME
+        a_long_time_ago = dt.datetime(2000, 1, 1, 0, 0, 0)
+        last_date = a_long_time_ago
         for story in page:
             assert 'indexed_date' in story
-            assert story['indexed_date'] <= last_date
+            assert story['indexed_date'] >= last_date
             last_date = story['indexed_date']
 
     def test_search_by_indexed_date(self):
         # compare results with indexed_date clause to those without it
         results1 = self._search.story_count(query="weather", start_date=self.START_DATE, end_date=self.END_DATE)
         assert results1['total'] > 0
         results2 = self._search.story_count(query="weather and indexed_date:[{} TO {}]".format(
@@ -208,7 +191,95 @@
             assert s['source'] in domains
         # now check urls for a page of matches and make sure they're all in collection list of domains
         results, _ = self._search.story_list(query="weather", start_date=self.START_DATE, end_date=self.END_DATE,
                                              collection_ids=[COLLECTION_US_NATIONAL])
         assert len(results) > 0
         for s in results:
             assert s['media_url'] in domains
+
+
+class SearchSyntaxTest(TestCase):
+
+    START_DATE = dt.date(2024, 1, 1)
+    END_DATE = dt.date(2024, 1, 30)
+
+    def setUp(self):
+        self._mc_api_key = os.getenv("MC_API_TOKEN")
+        self._search = mediacloud.api.SearchApi(self._mc_api_key)
+
+    def _count_query(self, query: str) -> int:
+        return self._search.story_count(query=query, start_date=self.START_DATE, end_date=self.END_DATE,
+                                        collection_ids=[COLLECTION_US_NATIONAL])['relevant']
+
+    def test_title_search(self):
+        all_results = self._count_query(query="biden")
+        assert all_results > 0
+        title_results = self._count_query(query="article_title:biden")
+        assert title_results > 0
+        assert all_results >= title_results
+
+    def test_single_char_wildcard_search(self):
+        women_count = self._count_query(query="women")
+        assert women_count > 0
+        woman_count = self._count_query(query="woman")
+        assert woman_count > 0
+        wildcarded_count = self._count_query(query="wom?n")
+        assert wildcarded_count > 0
+        assert wildcarded_count >= women_count
+        assert wildcarded_count >= woman_count
+
+    def test_multiple_char_wildcard_search(self):
+        women_count = self._count_query(query="women")
+        assert women_count > 0
+        woman_count = self._count_query(query="woman")
+        assert woman_count > 0
+        wildcarded_count = self._count_query(query="wom*n")
+        assert wildcarded_count > 0
+        assert wildcarded_count >= women_count
+        assert wildcarded_count >= woman_count
+        wildcarded2_count = self._count_query(query="wom*")
+        assert wildcarded2_count > 0
+        assert wildcarded2_count >= women_count
+        assert wildcarded2_count >= woman_count
+
+    def test_or_search(self):
+        women_count = self._count_query(query="women")
+        assert women_count > 0
+        woman_count = self._count_query(query="woman")
+        assert woman_count > 0
+        ord_count = self._count_query(query="(woman OR women)")  # NOTE: this needs parentheses
+        assert ord_count >= women_count
+        assert ord_count >= woman_count
+
+    def test_and_search(self):
+        women_count = self._count_query(query="women")
+        assert women_count > 0
+        woman_count = self._count_query(query="woman")
+        assert woman_count > 0
+        anded_count = self._count_query(query="woman AND women")
+        assert anded_count <= women_count
+        assert anded_count <= woman_count
+
+    def test_proximity_search(self):
+        woman_count = self._count_query(query="woman")
+        killed_count = self._count_query(query="killed")
+        and_count = self._count_query(query="woman AND killed")
+        proximity_count = self._count_query(query='"woman killed"~10')
+        assert woman_count > and_count
+        assert killed_count > and_count
+        assert proximity_count < and_count
+
+    def test_default_search(self):
+        default_count = self._count_query(query="banana monkey")
+        and_count = self._count_query(query="banana AND monkey")
+        assert default_count > 0
+        assert and_count > 0
+        assert default_count == and_count
+
+    def test_negation_source(self):
+        all_count = self._count_query(query="gaza")
+        not_count = self._count_query(query="gaza NOT hamas")
+        minus_count = self._count_query(query="gaza -hamas")
+        assert all_count > 0
+        assert not_count > 0
+        assert not_count < all_count
+        assert minus_count == not_count
```

### Comparing `mediacloud-4.1.3/mediacloud/test/fixtures/sample_story_ap.txt` & `mediacloud-4.1.4/mediacloud/test/fixtures/sample_story_ap.txt`

 * *Files identical despite different names*

### Comparing `mediacloud-4.1.3/mediacloud/test/fixtures/sample_story_not_ap.txt` & `mediacloud-4.1.4/mediacloud/test/fixtures/sample_story_not_ap.txt`

 * *Files identical despite different names*

### Comparing `mediacloud-4.1.3/mediacloud/test/fixtures/sentences_by_story_1.json` & `mediacloud-4.1.4/mediacloud/test/fixtures/sentences_by_story_1.json`

 * *Files identical despite different names*

### Comparing `mediacloud-4.1.3/mediacloud/test/fixtures/sentences_by_story_2.json` & `mediacloud-4.1.4/mediacloud/test/fixtures/sentences_by_story_2.json`

 * *Files identical despite different names*

### Comparing `mediacloud-4.1.3/mediacloud/test/fixtures/story_27456565.json` & `mediacloud-4.1.4/mediacloud/test/fixtures/story_27456565.json`

 * *Files identical despite different names*

### Comparing `mediacloud-4.1.3/pyproject.toml` & `mediacloud-4.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "mediacloud"
-version = "4.1.3"
+version = "4.1.4"
 authors = [
     {name = "Rahul Bhargava", email = "r.bhargava@northeastern.edu"},
 ]
 description = "Media Cloud API Client Library"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `mediacloud-4.1.3/PKG-INFO` & `mediacloud-4.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediacloud
-Version: 4.1.3
+Version: 4.1.4
 Summary: Media Cloud API Client Library
 Author-email: Rahul Bhargava <r.bhargava@northeastern.edu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

