# Comparing `tmp/airbyte_source_linkedin_ads-2.0.0.tar.gz` & `tmp/airbyte_source_linkedin_ads-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_linkedin_ads-2.0.0.tar", max compression
+gzip compressed data, was "airbyte_source_linkedin_ads-2.1.0.tar", max compression
```

## Comparing `airbyte_source_linkedin_ads-2.0.0.tar` & `airbyte_source_linkedin_ads-2.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     4604 2024-04-24 16:28:31.000000 airbyte_source_linkedin_ads-2.0.0/README.md
--rw-r--r--   0        0        0      776 2024-04-24 17:04:43.951479 airbyte_source_linkedin_ads-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1179 2024-04-24 16:28:31.000000 airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/__init__.py
--rw-r--r--   0        0        0    14625 2024-04-24 16:28:31.000000 airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/analytics_streams.py
--rw-r--r--   0        0        0      246 2024-04-24 16:28:31.000000 airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/run.py
--rw-r--r--   0        0        0      512 2024-04-24 16:28:31.000000 airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/schemas/account_users.json
--rw-r--r--   0        0        0     1405 2024-04-24 16:28:31.000000 airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/schemas/accounts.json
--rw-r--r--   0        0        0     7113 2024-04-24 16:28:31.000000 airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/schemas/ad_analytics.json
--rw-r--r--   0        0        0     1399 2024-04-24 16:28:31.000000 airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/schemas/campaign_groups.json
--rw-r--r--   0        0        0     4731 2024-04-24 16:28:31.000000 airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/schemas/campaigns.json
--rw-r--r--   0        0        0     1511 2024-04-24 16:28:31.000000 airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/schemas/conversions.json
--rw-r--r--   0        0        0     1404 2024-04-24 16:28:31.000000 airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/schemas/creatives.json
--rw-r--r--   0        0        0     5505 2024-04-24 16:28:31.000000 airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/source.py
--rw-r--r--   0        0        0     6880 2024-04-24 16:28:31.000000 airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/spec.json
--rw-r--r--   0        0        0    17489 2024-04-24 16:28:31.000000 airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/streams.py
--rw-r--r--   0        0        0    11728 2024-04-24 16:28:31.000000 airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/utils.py
--rw-r--r--   0        0        0     5324 1970-01-01 00:00:00.000000 airbyte_source_linkedin_ads-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4604 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/README.md
+-rw-r--r--   0        0        0      776 2024-05-02 12:06:29.258237 airbyte_source_linkedin_ads-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1179 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/__init__.py
+-rw-r--r--   0        0        0    15085 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/analytics_streams.py
+-rw-r--r--   0        0        0      246 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/run.py
+-rw-r--r--   0        0        0      512 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/account_users.json
+-rw-r--r--   0        0        0     1405 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/accounts.json
+-rw-r--r--   0        0        0     7113 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/ad_analytics.json
+-rw-r--r--   0        0        0     1399 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/campaign_groups.json
+-rw-r--r--   0        0        0     4731 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/campaigns.json
+-rw-r--r--   0        0        0     1511 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/conversions.json
+-rw-r--r--   0        0        0     1404 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/creatives.json
+-rw-r--r--   0        0        0     5505 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/source.py
+-rw-r--r--   0        0        0     6880 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/spec.json
+-rw-r--r--   0        0        0    18463 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/streams.py
+-rw-r--r--   0        0        0    11728 2024-05-02 08:09:28.000000 airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/utils.py
+-rw-r--r--   0        0        0     5324 1970-01-01 00:00:00.000000 airbyte_source_linkedin_ads-2.1.0/PKG-INFO
```

### Comparing `airbyte_source_linkedin_ads-2.0.0/README.md` & `airbyte_source_linkedin_ads-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.0.0/pyproject.toml` & `airbyte_source_linkedin_ads-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.0.0"
+version = "2.1.0"
 name = "airbyte-source-linkedin-ads"
 description = "Source implementation for Linkedin Ads."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/__init__.py` & `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/analytics_streams.py` & `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/analytics_streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,38 +233,57 @@
         )
 
     def get_primary_key_from_slice(self, stream_slice) -> str:
         return stream_slice.get(self.primary_slice_key)
 
     def stream_slices(
         self, *, sync_mode: SyncMode, cursor_field: Optional[List[str]] = None, stream_state: Optional[Mapping[str, Any]] = None
-    ) -> Iterable[List[Mapping[str, Any]]]:
+    ) -> Iterable[Optional[Mapping[str, List[Mapping[str, Any]]]]]:
         """
         LinkedIn has a max of 20 fields per request. We make chunks by size of 19 fields to have the `dateRange` be included as well.
         https://learn.microsoft.com/en-us/linkedin/marketing/integrations/ads-reporting/ads-reporting?view=li-lms-2023-05&tabs=http#requesting-specific-metrics-in-the-analytics-finder
 
         :param sync_mode:
         :param cursor_field:
         :param stream_state:
-        :return: Iterable with List of stream slices within the same date range and chunked fields, example
-        [{'campaign_id': 123, 'fields': 'field_1,field_2,dateRange', 'dateRange': {'start.day': 1, 'start.month': 1, 'start.year': 2020, 'end.day': 30, 'end.month': 1, 'end.year': 2020}},
-        {'campaign_id': 123, 'fields': 'field_2,field_3,dateRange',  'dateRange': {'start.day': 1, 'start.month': 1, 'start.year': 2020, 'end.day': 30, 'end.month': 1, 'end.year': 2020}},
-        {'campaign_id': 123, 'fields': 'field_4,field_5,dateRange',  'dateRange': {'start.day': 1, 'start.month': 1, 'start.year': 2020, 'end.day': 30, 'end.month': 1, 'end.year': 2020}}]
+        :return: An iterable of dictionaries, each containing a single key 'field_date_chunks'. The value under 'field_date_chunks' is
+        a list of dictionaries where each dictionary represents a slice of data defined by a specific date range and chunked fields.
 
+        Example of returned data:
+        {
+            'field_date_chunks': [
+                {
+                    'campaign_id': 123,
+                    'fields': 'field_1,field_2,dateRange',
+                    'dateRange': {
+                        'start.day': 1, 'start.month': 1, 'start.year': 2020,
+                        'end.day': 30, 'end.month': 1, 'end.year': 2020
+                    }
+                },
+                {
+                    'campaign_id': 123,
+                    'fields': 'field_3,field_4,dateRange',
+                    'dateRange': {
+                        'start.day': 1, 'start.month': 1, 'start.year': 2020,
+                        'end.day': 30, 'end.month': 1, 'end.year': 2020
+                    }
+                }
+            ]
+        }
         """
         parent_stream = self.parent_stream(config=self.config)
         stream_state = stream_state or {self.cursor_field: self.config.get("start_date")}
         for record in parent_stream.read_records(sync_mode=sync_mode):
             base_slice = get_parent_stream_values(record, self.parent_values_map)
             for date_slice in self.get_date_slices(stream_state.get(self.cursor_field), self.config.get("end_date")):
                 date_slice_with_fields: List = []
                 for fields_set in self.chunk_analytics_fields():
                     base_slice["fields"] = ",".join(fields_set)
                     date_slice_with_fields.append(base_slice | date_slice)
-                yield date_slice_with_fields
+                yield {"field_date_chunks": date_slice_with_fields}
 
     @staticmethod
     def get_date_slices(start_date: str, end_date: str = None, window_in_days: int = WINDOW_IN_DAYS) -> Iterable[Mapping[str, Any]]:
         """
         Produces date slices from start_date to end_date (if specified),
         otherwise end_date will be present time.
         """
@@ -303,15 +322,15 @@
                 chunk.append("pivotValues")
         yield from chunks
 
     def read_records(
         self, stream_state: Mapping[str, Any] = None, stream_slice: Optional[Mapping[str, Any]] = None, **kwargs
     ) -> Iterable[Mapping[str, Any]]:
         merged_records = defaultdict(dict)
-        for field_slice in stream_slice:
+        for field_slice in stream_slice.get("field_date_chunks", []):
             for rec in super().read_records(stream_slice=field_slice, **kwargs):
                 merged_records[f"{rec[self.cursor_field]}-{rec['pivotValues']}"].update(rec)
         yield from merged_records.values()
 
     def parse_response(self, response: requests.Response, **kwargs) -> Iterable[Mapping]:
         """
         We need to get out the nested complex data structures for further normalization, so the transform_data method is applied.
```

### Comparing `airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/schemas/account_users.json` & `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/account_users.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/schemas/accounts.json` & `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/schemas/ad_analytics.json` & `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/ad_analytics.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/schemas/campaign_groups.json` & `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/campaign_groups.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/schemas/campaigns.json` & `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/schemas/conversions.json` & `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/conversions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/schemas/creatives.json` & `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/schemas/creatives.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/source.py` & `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/spec.json` & `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/streams.py` & `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/streams.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from airbyte_cdk.sources.streams.http import HttpStream
 from airbyte_cdk.sources.utils.transform import TransformConfig, TypeTransformer
 
 from .utils import get_parent_stream_values, transform_data
 
 logger = logging.getLogger("airbyte")
 
-LINKEDIN_VERSION_API = "202305"
+LINKEDIN_VERSION_API = "202404"
 
 
 class LinkedinAdsStream(HttpStream, ABC):
     """
     Basic class provides base functionality for all streams.
     """
 
@@ -60,47 +60,34 @@
         next_page_token: Mapping[str, Any] = None,
     ) -> str:
         """Returns the API endpoint path for stream, from `endpoint` class attribute."""
         return self.endpoint
 
     def next_page_token(self, response: requests.Response) -> Optional[Mapping[str, Any]]:
         """
-        To paginate through results, begin with a start value of 0 and a count value of N.
-        To get the next page, set start value to N, while the count value stays the same.
-        We have reached the end of the dataset when the response contains fewer elements than the `count` parameter request.
-        https://docs.microsoft.com/en-us/linkedin/shared/api-guide/concepts/pagination?context=linkedin/marketing/context
+        Cursor based pagination using the pageSize and pageToken parameters.
         """
         parsed_response = response.json()
-        is_elements_less_than_limit = len(parsed_response.get("elements")) < self.records_limit
-
-        # Note: The API might return fewer records than requested within the limits during pagination.
-        # This behavior is documented at: https://github.com/airbytehq/airbyte/issues/34164
-        paging_params = parsed_response.get("paging", {})
-        is_end_of_records = (
-            paging_params["total"] - paging_params["start"] <= self.records_limit
-            if all(param in paging_params for param in ("total", "start"))
-            else True
-        )
-
-        if is_elements_less_than_limit and is_end_of_records:
+        if parsed_response.get("metadata", {}).get("nextPageToken"):
+            return {"pageToken": parsed_response["metadata"]["nextPageToken"]}
+        else:
             return None
-        return {"start": paging_params.get("start") + self.records_limit}
 
     def request_headers(
         self, stream_state: Mapping[str, Any], stream_slice: Mapping[str, Any] = None, next_page_token: Mapping[str, Any] = None
     ) -> Mapping[str, Any]:
         return {"Linkedin-Version": LINKEDIN_VERSION_API}
 
     def request_params(
         self,
         stream_state: Mapping[str, Any],
         stream_slice: Mapping[str, Any] = None,
         next_page_token: Mapping[str, Any] = None,
     ) -> MutableMapping[str, Any]:
-        params = {"count": self.records_limit, "q": "search"}
+        params = {"pageSize": self.records_limit, "q": "search"}
         if next_page_token:
             params.update(**next_page_token)
         return params
 
     def parse_response(self, response: requests.Response, **kwargs) -> Iterable[Mapping]:
         """
         We need to get out the nested complex data structures for further normalization, so the transform_data method is applied.
@@ -126,14 +113,52 @@
                 f"You can find more information here https://docs.airbyte.com/integrations/sources/linkedin-ads. "
                 f"Also quotas and usage are here: https://www.linkedin.com/developers/apps."
             )
             self.logger.error(error_message)
         return super().should_retry(response)
 
 
+class OffsetPaginationMixin:
+    """Mixin for offset based pagination for endpoints tha tdoesnt support cursor based pagination"""
+
+    def request_params(
+        self,
+        stream_state: Mapping[str, Any],
+        stream_slice: Mapping[str, Any] = None,
+        next_page_token: Mapping[str, Any] = None,
+    ) -> MutableMapping[str, Any]:
+        params = {"count": self.records_limit, "q": "search"}
+        if next_page_token:
+            params.update(**next_page_token)
+        return params
+
+    def next_page_token(self, response: requests.Response) -> Optional[Mapping[str, Any]]:
+        """
+        To paginate through results, begin with a start value of 0 and a count value of N.
+        To get the next page, set start value to N, while the count value stays the same.
+        We have reached the end of the dataset when the response contains fewer elements than the `count` parameter request.
+        https://docs.microsoft.com/en-us/linkedin/shared/api-guide/concepts/pagination?context=linkedin/marketing/context
+        """
+        parsed_response = response.json()
+        is_elements_less_than_limit = len(parsed_response.get("elements")) < self.records_limit
+
+        # Note: The API might return fewer records than requested within the limits during pagination.
+        # This behavior is documented at: https://github.com/airbytehq/airbyte/issues/34164
+        paging_params = parsed_response.get("paging", {})
+        is_end_of_records = (
+            paging_params["total"] - paging_params["start"] <= self.records_limit
+            if all(param in paging_params for param in ("total", "start"))
+            else True
+        )
+
+        if is_elements_less_than_limit and is_end_of_records:
+            return None
+        return {"start": paging_params.get("start") + self.records_limit}
+
+
 class Accounts(LinkedinAdsStream):
     """
     Get Accounts data. More info about LinkedIn Ads / Accounts:
     https://learn.microsoft.com/en-us/linkedin/marketing/integrations/ads/account-structure/create-and-manage-accounts?tabs=http&view=li-lms-2023-05#search-for-accounts
     """
 
     endpoint = "adAccounts"
@@ -223,15 +248,15 @@
         stream_state = stream_state or {}
         parent_stream = self.parent_stream(config=self.config)
         for record in parent_stream.read_records(**kwargs):
             child_stream_slice = super().read_records(stream_slice=get_parent_stream_values(record, self.parent_values_map), **kwargs)
             yield from self.filter_records_newer_than_state(stream_state=stream_state, records_slice=child_stream_slice)
 
 
-class AccountUsers(LinkedInAdsStreamSlicing):
+class AccountUsers(OffsetPaginationMixin, LinkedInAdsStreamSlicing):
     """
     Get AccountUsers data using `account_id` slicing. More info about LinkedIn Ads / AccountUsers:
     https://learn.microsoft.com/en-us/linkedin/marketing/integrations/ads/account-structure/create-and-manage-account-users?tabs=http&view=li-lms-2023-05#find-ad-account-users-by-accounts
     """
 
     endpoint = "adAccountUsers"
     # Account_users stream doesn't have `id` property, so the "account" is used instead.
@@ -361,15 +386,15 @@
             {self.cursor_field: pendulum.parse(self.config.get("start_date")).format("x")}
             if not current_stream_state
             else current_stream_state
         )
         return {self.cursor_field: max(latest_record.get(self.cursor_field), int(current_stream_state.get(self.cursor_field)))}
 
 
-class Conversions(LinkedInAdsStreamSlicing):
+class Conversions(OffsetPaginationMixin, LinkedInAdsStreamSlicing):
     """
     Get Conversions data using `account_id` slicing.
     https://learn.microsoft.com/en-us/linkedin/marketing/integrations/ads-reporting/conversion-tracking?view=li-lms-2023-05&tabs=curl#find-conversions-by-ad-account
     """
 
     endpoint = "conversions"
     search_param = "account"
```

### Comparing `airbyte_source_linkedin_ads-2.0.0/source_linkedin_ads/utils.py` & `airbyte_source_linkedin_ads-2.1.0/source_linkedin_ads/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_linkedin_ads-2.0.0/PKG-INFO` & `airbyte_source_linkedin_ads-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-linkedin-ads
-Version: 2.0.0
+Version: 2.1.0
 Summary: Source implementation for Linkedin Ads.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

