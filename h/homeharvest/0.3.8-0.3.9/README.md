# Comparing `tmp/homeharvest-0.3.8.tar.gz` & `tmp/homeharvest-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeharvest-0.3.8.tar", max compression
+gzip compressed data, was "homeharvest-0.3.9.tar", max compression
```

## Comparing `homeharvest-0.3.8.tar` & `homeharvest-0.3.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-11-03 23:44:34.330560 homeharvest-0.3.8/LICENSE
--rw-r--r--   0        0        0     8480 2023-11-03 23:44:34.330560 homeharvest-0.3.8/README.md
--rw-r--r--   0        0        0     1956 2023-11-03 23:44:34.330560 homeharvest-0.3.8/homeharvest/__init__.py
--rw-r--r--   0        0        0     2273 2023-11-03 23:44:34.330560 homeharvest-0.3.8/homeharvest/cli.py
--rw-r--r--   0        0        0        0 2023-11-03 23:44:34.330560 homeharvest-0.3.8/homeharvest/core/__init__.py
--rw-r--r--   0        0        0     1381 2023-11-03 23:44:34.330560 homeharvest-0.3.8/homeharvest/core/scrapers/__init__.py
--rw-r--r--   0        0        0     1546 2023-11-03 23:44:34.330560 homeharvest-0.3.8/homeharvest/core/scrapers/models.py
--rw-r--r--   0        0        0    25028 2023-11-03 23:44:34.330560 homeharvest-0.3.8/homeharvest/core/scrapers/realtor/__init__.py
--rw-r--r--   0        0        0      246 2023-11-03 23:44:34.330560 homeharvest-0.3.8/homeharvest/exceptions.py
--rw-r--r--   0        0        0     2695 2023-11-03 23:44:34.330560 homeharvest-0.3.8/homeharvest/utils.py
--rw-r--r--   0        0        0      621 2023-11-03 23:44:34.330560 homeharvest-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     9125 1970-01-01 00:00:00.000000 homeharvest-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-11-08 22:56:22.779010 homeharvest-0.3.9/LICENSE
+-rw-r--r--   0        0        0     8479 2023-11-08 22:56:22.779010 homeharvest-0.3.9/README.md
+-rw-r--r--   0        0        0     1956 2023-11-08 22:56:22.779010 homeharvest-0.3.9/homeharvest/__init__.py
+-rw-r--r--   0        0        0     2273 2023-11-08 22:56:22.779010 homeharvest-0.3.9/homeharvest/cli.py
+-rw-r--r--   0        0        0        0 2023-11-08 22:56:22.779010 homeharvest-0.3.9/homeharvest/core/__init__.py
+-rw-r--r--   0        0        0     1381 2023-11-08 22:56:22.779010 homeharvest-0.3.9/homeharvest/core/scrapers/__init__.py
+-rw-r--r--   0        0        0     1546 2023-11-08 22:56:22.779010 homeharvest-0.3.9/homeharvest/core/scrapers/models.py
+-rw-r--r--   0        0        0    25249 2023-11-08 22:56:22.783011 homeharvest-0.3.9/homeharvest/core/scrapers/realtor/__init__.py
+-rw-r--r--   0        0        0      246 2023-11-08 22:56:22.783011 homeharvest-0.3.9/homeharvest/exceptions.py
+-rw-r--r--   0        0        0     2695 2023-11-08 22:56:22.783011 homeharvest-0.3.9/homeharvest/utils.py
+-rw-r--r--   0        0        0      621 2023-11-08 22:56:22.783011 homeharvest-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     9124 1970-01-01 00:00:00.000000 homeharvest-0.3.9/PKG-INFO
```

### Comparing `homeharvest-0.3.8/LICENSE` & `homeharvest-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `homeharvest-0.3.8/README.md` & `homeharvest-0.3.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 **HomeHarvest** is a simple, yet comprehensive, real estate scraping library that extracts and formats data in the style of MLS listings.
 
 [![Try with Replit](https://replit.com/badge?caption=Try%20with%20Replit)](https://replit.com/@ZacharyHampton/HomeHarvestDemo)
 
 **Not technical?** Try out the web scraping tool on our site at [tryhomeharvest.com](https://tryhomeharvest.com).
 
-*Looking to build a data-focused software product?* **[Book a call](https://calendly.com/bunsly/15min)** *to work with us.*
+*Looking to build a data-focused software product?* **[Book a call](https://bunsly.com)** *to work with us.*
 
 Check out another project we wrote: ***[JobSpy](https://github.com/Bunsly/JobSpy)** – a Python package for job scraping*
 
 ## HomeHarvest Features
 
 - **Source**: Fetches properties directly from **Realtor.com**.
 - **Data Format**: Structures data to resemble MLS listings.
@@ -87,23 +87,24 @@
 Optional
 ├── radius (decimal): Radius in miles to find comparable properties based on individual addresses.
 │    Example: 5.5 (fetches properties within a 5.5-mile radius if location is set to a specific address; otherwise, ignored)
 │
 ├── past_days (integer): Number of past days to filter properties. Utilizes 'last_sold_date' for 'sold' listing types, and 'list_date' for others (for_rent, for_sale).
 │    Example: 30 (fetches properties listed/sold in the last 30 days)
 │
-├── date_range (string tuple): Start and end dates to filter properties listed or sold, both dates are required.
+├── date_from, date_to (string): Start and end dates to filter properties listed or sold, both dates are required.
 }    (use this to get properties in chunks as there's a 10k result limit)
 │    Format for both must be "YYYY-MM-DD". 
-│    Example: ("2023-05-01", "2023-05-15") (fetches properties listed/sold between these dates)
+│    Example: "2023-05-01", "2023-05-15" (fetches properties listed/sold between these dates)
 │
 ├── mls_only (True/False): If set, fetches only MLS listings (mainly applicable to 'sold' listings)
 │
 └── proxy (string): In format 'http://user:pass@host:port'
 
+
 ```
 
 ### CLI 
 
 ```
 usage: homeharvest [-l {for_sale,for_rent,sold}] [-o {excel,csv}] [-f FILENAME] [-p PROXY] [-d DAYS] [-r RADIUS] [-m] [-c] location
                                                                                                                              
@@ -173,15 +174,15 @@
     └── parking_garage
 ```
 
 ### Exceptions
 The following exceptions may be raised when using HomeHarvest:
 
 - `InvalidListingType` - valid options: `for_sale`, `for_rent`, `sold`
-- `NoResultsFound` - no properties found from your search
+- `InvalidDate` - date_from or date_to is not in the format YYYY-MM-DD
   
   
 ## Frequently Asked Questions
 ---
 
 **Q: Encountering issues with your searches?**  
 **A:** Try to broaden the parameters you're using. If problems persist, [submit an issue](https://github.com/ZacharyHampton/HomeHarvest/issues).
```

### Comparing `homeharvest-0.3.8/homeharvest/__init__.py` & `homeharvest-0.3.9/homeharvest/__init__.py`

 * *Files identical despite different names*

### Comparing `homeharvest-0.3.8/homeharvest/cli.py` & `homeharvest-0.3.9/homeharvest/cli.py`

 * *Files identical despite different names*

### Comparing `homeharvest-0.3.8/homeharvest/core/scrapers/__init__.py` & `homeharvest-0.3.9/homeharvest/core/scrapers/__init__.py`

 * *Files identical despite different names*

### Comparing `homeharvest-0.3.8/homeharvest/core/scrapers/models.py` & `homeharvest-0.3.9/homeharvest/core/scrapers/models.py`

 * *Files identical despite different names*

### Comparing `homeharvest-0.3.8/homeharvest/core/scrapers/realtor/__init__.py` & `homeharvest-0.3.9/homeharvest/core/scrapers/realtor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         query = """query Listing($listing_id: ID!) {
                     listing(id: $listing_id) {
                         source {
                             id
                             listing_id
                         }
                         address {
+                            street_direction
                             street_number
                             street_name
                             street_suffix
                             unit
                             city
                             state_code
                             postal_code
@@ -211,14 +212,15 @@
                             date_updated
                             garage
                             permalink
                             year_built
                             stories
                         }
                         address {
+                            street_direction
                             street_number
                             street_name
                             street_suffix
                             unit
                             city
                             state_code
                             postal_code
@@ -311,14 +313,15 @@
                                     listing_id
                                 }
                                 hoa {
                                     fee
                                 }
                                 location {
                                     address {
+                                        street_direction
                                         street_number
                                         street_name
                                         street_suffix
                                         unit
                                         city
                                         state_code
                                         postal_code
@@ -602,14 +605,15 @@
             address = result['location']['address']
         else:
             address = result["address"]
 
         return Address(
             street=" ".join([
                 self.handle_none_safely(address.get('street_number')),
+                self.handle_none_safely(address.get('street_direction')),
                 self.handle_none_safely(address.get('street_name')),
                 self.handle_none_safely(address.get('street_suffix')),
             ]).strip(),
             unit=address["unit"],
             city=address["city"],
             state=address["state_code"],
             zip=address["postal_code"],
```

### Comparing `homeharvest-0.3.8/homeharvest/utils.py` & `homeharvest-0.3.9/homeharvest/utils.py`

 * *Files identical despite different names*

### Comparing `homeharvest-0.3.8/pyproject.toml` & `homeharvest-0.3.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "homeharvest"
-version = "0.3.8"
+version = "0.3.9"
 description = "Real estate scraping library supporting Zillow, Realtor.com & Redfin."
 authors = ["Zachary Hampton <zachary@zacharysproducts.com>", "Cullen Watson <cullen@cullen.ai>"]
 homepage = "https://github.com/Bunsly/HomeHarvest"
 readme = "README.md"
 
 [tool.poetry.scripts]
 homeharvest = "homeharvest.cli:main"
```

### Comparing `homeharvest-0.3.8/PKG-INFO` & `homeharvest-0.3.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeharvest
-Version: 0.3.8
+Version: 0.3.9
 Summary: Real estate scraping library supporting Zillow, Realtor.com & Redfin.
 Home-page: https://github.com/Bunsly/HomeHarvest
 Author: Zachary Hampton
 Author-email: zachary@zacharysproducts.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -19,15 +19,15 @@
 
 **HomeHarvest** is a simple, yet comprehensive, real estate scraping library that extracts and formats data in the style of MLS listings.
 
 [![Try with Replit](https://replit.com/badge?caption=Try%20with%20Replit)](https://replit.com/@ZacharyHampton/HomeHarvestDemo)
 
 **Not technical?** Try out the web scraping tool on our site at [tryhomeharvest.com](https://tryhomeharvest.com).
 
-*Looking to build a data-focused software product?* **[Book a call](https://calendly.com/bunsly/15min)** *to work with us.*
+*Looking to build a data-focused software product?* **[Book a call](https://bunsly.com)** *to work with us.*
 
 Check out another project we wrote: ***[JobSpy](https://github.com/Bunsly/JobSpy)** – a Python package for job scraping*
 
 ## HomeHarvest Features
 
 - **Source**: Fetches properties directly from **Realtor.com**.
 - **Data Format**: Structures data to resemble MLS listings.
@@ -104,23 +104,24 @@
 Optional
 ├── radius (decimal): Radius in miles to find comparable properties based on individual addresses.
 │    Example: 5.5 (fetches properties within a 5.5-mile radius if location is set to a specific address; otherwise, ignored)
 │
 ├── past_days (integer): Number of past days to filter properties. Utilizes 'last_sold_date' for 'sold' listing types, and 'list_date' for others (for_rent, for_sale).
 │    Example: 30 (fetches properties listed/sold in the last 30 days)
 │
-├── date_range (string tuple): Start and end dates to filter properties listed or sold, both dates are required.
+├── date_from, date_to (string): Start and end dates to filter properties listed or sold, both dates are required.
 }    (use this to get properties in chunks as there's a 10k result limit)
 │    Format for both must be "YYYY-MM-DD". 
-│    Example: ("2023-05-01", "2023-05-15") (fetches properties listed/sold between these dates)
+│    Example: "2023-05-01", "2023-05-15" (fetches properties listed/sold between these dates)
 │
 ├── mls_only (True/False): If set, fetches only MLS listings (mainly applicable to 'sold' listings)
 │
 └── proxy (string): In format 'http://user:pass@host:port'
 
+
 ```
 
 ### CLI 
 
 ```
 usage: homeharvest [-l {for_sale,for_rent,sold}] [-o {excel,csv}] [-f FILENAME] [-p PROXY] [-d DAYS] [-r RADIUS] [-m] [-c] location
                                                                                                                              
@@ -190,15 +191,15 @@
     └── parking_garage
 ```
 
 ### Exceptions
 The following exceptions may be raised when using HomeHarvest:
 
 - `InvalidListingType` - valid options: `for_sale`, `for_rent`, `sold`
-- `NoResultsFound` - no properties found from your search
+- `InvalidDate` - date_from or date_to is not in the format YYYY-MM-DD
   
   
 ## Frequently Asked Questions
 ---
 
 **Q: Encountering issues with your searches?**  
 **A:** Try to broaden the parameters you're using. If problems persist, [submit an issue](https://github.com/ZacharyHampton/HomeHarvest/issues).
```

