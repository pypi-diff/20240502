# Comparing `tmp/edgartools-2.8.3.tar.gz` & `tmp/edgartools-2.9.0.tar.gz`

## Comparing `edgartools-2.8.3.tar` & `edgartools-2.9.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/__about__.py
--rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/__init__.py
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/_codes.py
--rw-r--r--   0        0        0    32921 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/_companies.py
--rw-r--r--   0        0        0    82932 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/_filings.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/_gaap.py
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/_markdown.py
--rw-r--r--   0        0        0     7237 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/_party.py
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/_rich.py
--rw-r--r--   0        0        0    12884 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/_xbrl.py
--rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/_xml.py
--rw-r--r--   0        0        0    24163 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/company_reports.py
--rw-r--r--   0        0        0    20102 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/core.py
--rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/effect.py
--rw-r--r--   0        0        0    13828 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/financials.py
--rw-r--r--   0        0        0    20908 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/form144.py
--rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/forms.py
--rw-r--r--   0        0        0    27038 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/fundreports.py
--rw-r--r--   0        0        0    16011 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/funds.py
--rw-r--r--   0        0        0    20467 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/htmltools.py
--rw-r--r--   0        0        0    41630 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/muniadvisors.py
--rw-r--r--   0        0        0    21137 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/offerings.py
--rw-r--r--   0        0        0    47530 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/ownership.py
--rw-r--r--   0        0        0     7522 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/search.py
--rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/sgml.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/shelfofferings.py
--rw-r--r--   0        0        0    14156 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/thirteenf.py
--rw-r--r--   0        0        0  1588656 2020-02-02 00:00:00.000000 edgartools-2.8.3/edgar/data/gaap_taxonomy_2022.csv
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 edgartools-2.8.3/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 edgartools-2.8.3/LICENSE.txt
--rw-r--r--   0        0        0    24347 2020-02-02 00:00:00.000000 edgartools-2.8.3/README.md
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 edgartools-2.8.3/pyproject.toml
--rw-r--r--   0        0        0    25798 2020-02-02 00:00:00.000000 edgartools-2.8.3/PKG-INFO
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/__about__.py
+-rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/__init__.py
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/_codes.py
+-rw-r--r--   0        0        0    34952 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/_companies.py
+-rw-r--r--   0        0        0    82937 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/_filings.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/_gaap.py
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/_markdown.py
+-rw-r--r--   0        0        0     7237 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/_party.py
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/_rich.py
+-rw-r--r--   0        0        0    12884 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/_xbrl.py
+-rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/_xml.py
+-rw-r--r--   0        0        0    24163 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/company_reports.py
+-rw-r--r--   0        0        0    20626 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/core.py
+-rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/effect.py
+-rw-r--r--   0        0        0    13828 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/financials.py
+-rw-r--r--   0        0        0    20908 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/form144.py
+-rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/forms.py
+-rw-r--r--   0        0        0    27038 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/fundreports.py
+-rw-r--r--   0        0        0    16011 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/funds.py
+-rw-r--r--   0        0        0    20467 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/htmltools.py
+-rw-r--r--   0        0        0    41630 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/muniadvisors.py
+-rw-r--r--   0        0        0    21137 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/offerings.py
+-rw-r--r--   0        0        0    47530 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/ownership.py
+-rw-r--r--   0        0        0     7522 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/search.py
+-rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/sgml.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/shelfofferings.py
+-rw-r--r--   0        0        0    14156 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/thirteenf.py
+-rw-r--r--   0        0        0  1588656 2020-02-02 00:00:00.000000 edgartools-2.9.0/edgar/data/gaap_taxonomy_2022.csv
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 edgartools-2.9.0/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 edgartools-2.9.0/LICENSE.txt
+-rw-r--r--   0        0        0    24637 2020-02-02 00:00:00.000000 edgartools-2.9.0/README.md
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 edgartools-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0    26088 2020-02-02 00:00:00.000000 edgartools-2.9.0/PKG-INFO
```

### Comparing `edgartools-2.8.3/edgar/__init__.py` & `edgartools-2.9.0/edgar/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,16 @@
                               Entity,
                               EntityData,
                               find_company,
                               get_entity,
                               get_company_facts,
                               get_company_tickers,
                               get_entity_submissions,
-                              get_ticker_to_cik_lookup)
+                              get_ticker_to_cik_lookup,
+                              get_cik_lookup_data)
 from edgar._filings import (Filing,
                             Filings,
                             CurrentFilings,
                             Attachment,
                             Attachments,
                             get_filings,
                             get_current_filings,
```

### Comparing `edgartools-2.8.3/edgar/_codes.py` & `edgartools-2.9.0/edgar/_codes.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.8.3/edgar/_companies.py` & `edgartools-2.9.0/edgar/_companies.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import logging
 import re
 from dataclasses import dataclass
 from functools import lru_cache
-from typing import List, Dict, Optional, Union, Tuple
+from typing import List, Dict, Optional, Union, Tuple, Any
 
 import httpx
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import pyarrow.compute as pc
 from fastcore.basics import listify
 from rich.console import Group
 from rich.panel import Panel
 from rich.text import Text
 
 from edgar._filings import Filing, Filings, FilingsState
 from edgar._rich import df_to_rich_table, repr_rich
-from edgar.core import (http_client, log, Result, display_size,
-                        filter_by_date, IntString, InvalidDateException)
+from edgar.core import (download_json, log, Result, display_size, download_text,
+                        filter_by_date, IntString, InvalidDateException, reverse_name)
 from edgar.search import SimilaritySearchIndex
 
 __all__ = [
     'Address',
     'Entity',
     'EntityFacts',
     'EntityData',
@@ -36,15 +36,16 @@
     'CompanyConcept',
     'CompanySearchResults',
     'CompanySearchIndex',
     'get_company_facts',
     'get_company_tickers',
     'get_entity_submissions',
     'parse_entity_submissions',
-    'get_ticker_to_cik_lookup'
+    'get_ticker_to_cik_lookup',
+    'get_cik_lookup_data'
 ]
 
 
 class Address:
     def __init__(self,
                  street1: str,
                  street2: Optional[str],
@@ -313,16 +314,16 @@
                  fiscal_year_end: str,
                  entity_type: str,
                  phone: str,
                  flags: str,
                  business_address: Address,
                  mailing_address: Address,
                  filings: EntityFilings,
-                 insider_transaction_for_owner_exists: int,
-                 insider_transaction_for_issuer_exists: int,
+                 insider_transaction_for_owner_exists: bool,
+                 insider_transaction_for_issuer_exists: bool,
                  ein: str,
                  description: str,
                  website: str,
                  investor_website: str,
                  state_of_incorporation: str,
                  state_of_incorporation_description: str,
                  former_names: List[str],
@@ -337,38 +338,50 @@
         self.fiscal_year_end: str = fiscal_year_end
         self.entity_type: str = entity_type
         self.phone: str = phone
         self.flags: str = flags
         self.business_address: Address = business_address
         self.mailing_address: Address = mailing_address
         self.filings: CompanyFilings = filings
-        self.insider_transaction_for_owner_exists: int = insider_transaction_for_owner_exists
-        self.insider_transaction_for_issuer_exists: int = insider_transaction_for_issuer_exists
+        self.insider_transaction_for_owner_exists: bool = insider_transaction_for_owner_exists
+        self.insider_transaction_for_issuer_exists: bool = insider_transaction_for_issuer_exists
         self.ein: str = ein
         self.description: str = description
         self.website: str = website
         self.investor_website: str = investor_website
         self.state_of_incorporation: str = state_of_incorporation
         self.state_of_incorporation_description: str = state_of_incorporation_description
         self.former_names: List[str] = former_names
 
     @property
     def financials(self):
-        # Get the latest 10-K
-        latest_10k = self.filings.filter(form="10-K").latest()
-        if latest_10k is not None:
-            return latest_10k.obj().financials
+        if self.is_company:
+            # Get the latest 10-K
+            latest_10k = self.filings.filter(form="10-K").latest()
+            if latest_10k is not None:
+                return latest_10k.obj().financials
 
     @property
     def is_company(self) -> bool:
-        # Companies have a sic code populated, individuals do not
-        return self.sic != ''
+        # Companies have a ein, individuals do not. Oddly Warren Buffet has an EIN but not a state of incorporation
+        # There may be other edge cases
+        return not (self.ein is None or self.state_of_incorporation == '')
+
+
+
+    @property
+    @lru_cache(maxsize=1)
+    def display_name(self) -> str:
+        """Reverse the name if it is a company"""
+        if self.is_company:
+            return self.name
+        return reverse_name(self.name)
 
     @property
-    def industry(self):
+    def industry(self) -> str:
         return self.sic_description
 
     @classmethod
     def for_cik(cls, cik: int):
         return get_entity_submissions(cik)
 
     @classmethod
@@ -492,44 +505,44 @@
 
 def parse_filings(filings_json: Dict[str, object],
                   cik: int,
                   company_name: str) -> CompanyFilings:
     # Handle case of no data
     if filings_json['recent']['accessionNumber'] == []:
         # Create an empty table
-        filings_table = pa.Table.from_arrays(
-            [pa.array([], type=pa.string()),
-             pa.array([], type=pa.date32()),
-             pa.array([], type=pa.string()),
-             pa.array([], type=pa.string()),
-             pa.array([], type=pa.string()),
-             pa.array([], type=pa.string()),
-             pa.array([], type=pa.string()),
-             pa.array([], type=pa.string()),
-             pa.array([], type=pa.string()),
-             pa.array([], type=pa.string()),
-             pa.array([], type=pa.string()),
-             pa.array([], type=pa.string()),
-             pa.array([], type=pa.string()),
-             ],
-            names=['accession_number',
-                   'filing_date',
-                   'reportDate',
-                   'acceptanceDateTime',
-                   'act',
-                   'form',
-                   'fileNumber',
-                   'items',
-                   'size',
-                   'isXBRL',
-                   'isInlineXBRL',
-                   'primaryDocument',
-                   'primaryDocDescription'
-                   ]
-        )
+        filings_table = pa.Table.from_arrays(arrays=
+                                             [pa.array([], type=pa.string()),
+                                              pa.array([], type=pa.date32()),
+                                              pa.array([], type=pa.string()),
+                                              pa.array([], type=pa.string()),
+                                              pa.array([], type=pa.string()),
+                                              pa.array([], type=pa.string()),
+                                              pa.array([], type=pa.string()),
+                                              pa.array([], type=pa.string()),
+                                              pa.array([], type=pa.string()),
+                                              pa.array([], type=pa.string()),
+                                              pa.array([], type=pa.string()),
+                                              pa.array([], type=pa.string()),
+                                              pa.array([], type=pa.string()),
+                                              ],
+                                             names=['accession_number',
+                                                    'filing_date',
+                                                    'reportDate',
+                                                    'acceptanceDateTime',
+                                                    'act',
+                                                    'form',
+                                                    'fileNumber',
+                                                    'items',
+                                                    'size',
+                                                    'isXBRL',
+                                                    'isInlineXBRL',
+                                                    'primaryDocument',
+                                                    'primaryDocDescription'
+                                                    ]
+                                             )
     else:
         rjson: Dict[str, List[object]] = filings_json['recent']
 
         filings_table = pa.Table.from_arrays(
             [pa.array(rjson['accessionNumber']),
              pc.cast(pc.strptime(pa.array(rjson['filingDate']), '%Y-%m-%d', 'us'), pa.date32()),
              pa.array(rjson['reportDate']),
@@ -560,15 +573,15 @@
                    ]
         )
     return CompanyFilings(filings_table,
                           cik=cik,
                           company_name=company_name)
 
 
-def parse_entity_submissions(cjson: Dict[str, object]):
+def parse_entity_submissions(cjson: Dict[str, Any]):
     mailing_addr = cjson['addresses']['mailing']
     business_addr = cjson['addresses']['business']
     cik = cjson['cik']
     company_name = cjson["name"]
     return CompanyData(cik=int(cik),
                        name=company_name,
                        tickers=cjson['tickers'],
@@ -593,16 +606,16 @@
                            street2=business_addr['street2'],
                            city=business_addr['city'],
                            state_or_country_desc=business_addr['stateOrCountryDescription'],
                            state_or_country=business_addr['stateOrCountry'],
                            zipcode=business_addr['zipCode'],
                        ),
                        filings=parse_filings(cjson['filings'], cik=cik, company_name=company_name),
-                       insider_transaction_for_owner_exists=cjson['insiderTransactionForOwnerExists'],
-                       insider_transaction_for_issuer_exists=cjson['insiderTransactionForIssuerExists'],
+                       insider_transaction_for_owner_exists=bool(cjson['insiderTransactionForOwnerExists']),
+                       insider_transaction_for_issuer_exists=bool(cjson['insiderTransactionForIssuerExists']),
                        ein=cjson['ein'],
                        description=cjson['description'],
                        website=cjson['website'],
                        investor_website=cjson['investorWebsite'],
                        state_of_incorporation=cjson['stateOfIncorporation'],
                        state_of_incorporation_description=cjson['stateOfIncorporationDescription'],
                        former_names=cjson['formerNames'],
@@ -654,39 +667,31 @@
 
 # This is an alias for get_company allowing for this -> Company("SNOW")
 get_company = get_entity
 Company = get_entity
 Entity = get_entity
 
 
-def get_json(data_url: str):
-    with http_client() as client:
-        r = client.get(data_url)
-        if r.status_code == 200:
-            return r.json()
-        r.raise_for_status()
-
-
 @lru_cache(maxsize=32)
 def get_entity_submissions(cik: int,
                            include_old_filings: bool = True) -> EntityData:
     """Get the company filings for a given cik"""
     try:
-        submission_json = get_json(f"https://data.sec.gov/submissions/CIK{cik:010}.json")
+        submission_json = download_json(f"https://data.sec.gov/submissions/CIK{cik:010}.json")
     except httpx.HTTPStatusError as e:
         # Handle the case where the cik is invalid and not found on Edgar
         if e.response.status_code == 404:
             log.error(f"No company found for CIK {cik}")
             return None
         else:
             raise
             # check for older submission files
     if include_old_filings:
         for old_file in submission_json['filings']['files']:
-            old_sub = get_json("https://data.sec.gov/submissions/" + old_file['name'])
+            old_sub = download_json("https://data.sec.gov/submissions/" + old_file['name'])
             for column in old_sub:
                 submission_json['filings']['recent'][column] += old_sub[column]
     return parse_entity_submissions(submission_json)
 
 
 def parse_company_facts(fjson: Dict[str, object]):
     unit_dfs = []
@@ -723,15 +728,15 @@
         self.message = f"""No Company facts found for cik {cik}"""
 
 
 @lru_cache(maxsize=32)
 def get_company_facts(cik: int):
     company_facts_url = f"https://data.sec.gov/api/xbrl/companyfacts/CIK{cik:010}.json"
     try:
-        company_facts_json = get_json(company_facts_url)
+        company_facts_json = download_json(company_facts_url)
         return parse_company_facts(company_facts_json)
     except httpx.HTTPStatusError as err:
         if err.response.status_code == 404:
             logging.warning(f"No company facts found on url {company_facts_url}")
             raise NoCompanyFactsFound(cik=cik)
         else:
             raise
@@ -780,15 +785,15 @@
     def __repr__(self):
         return (f"CompanyConcept({self.concept.taxonomy}:{self.concept.tag}, {self.entity_name} - {self.cik})"
                 "\n"
                 f"{self.data}")
 
     @classmethod
     def from_json(cls,
-                  cjson: Dict[str, object]):
+                  cjson: Dict[str, Any]):
         data = pd.concat([
             (pd.DataFrame(unit_data)
              .assign(unit=unit, frame=lambda df: df.frame.replace(np.nan, None))
              .filter(['filed', 'val', 'unit', 'fy', 'fp', 'end', 'form', 'frame', 'accn'])
              .sort_values(["filed"], ascending=[False])
              .reset_index(drop=True)
              )
@@ -819,15 +824,15 @@
     https://data.sec.gov/api/xbrl/companyconcept/CIK##########/us-gaap/AccountsPayableCurrent.json
     :param cik: The company cik
     :param taxonomy: The taxonomy e.g. "us-gaap"
     :param concept: The concept or tag e.g. AccountsPayableCurrent
     :return: a CompanyConcept
     """
     try:
-        company_concept_json = get_json(
+        company_concept_json = download_json(
             f"https://data.sec.gov/api/xbrl/companyconcept/CIK{cik:010}/{taxonomy}/{concept}.json")
         company_concept: CompanyConcept = CompanyConcept.from_json(company_concept_json)
         return company_concept
     except httpx.HTTPStatusError as e:
         if e.response.status_code == 404:
             # Get the company
             company = CompanyData.for_cik(int(cik))
@@ -838,33 +843,56 @@
                                  "See https://fasb.org/xbrl")
                 log.error(error_message)
                 return Result.Fail(error=error_message)
 
 
 @lru_cache(maxsize=1)
 def get_company_tickers():
-    tickers_json = get_json(
+    tickers_json = download_json(
         "https://www.sec.gov/files/company_tickers.json"
     )
     ticker_df = (pd.DataFrame(list(tickers_json.values()))
                  .set_axis(['cik', 'ticker', 'company'], axis=1)
                  .astype({'cik': pd.Int64Dtype()})
                  )
     return ticker_df
 
 
+@lru_cache(maxsize=1)
 def get_ticker_to_cik_lookup():
-    tickers_json = get_json(
+    tickers_json = download_json(
         "https://www.sec.gov/files/company_tickers.json"
     )
     return {value['ticker']: value['cik_str']
             for value in tickers_json.values()
             }
 
 
+def _parse_cik_lookup_data(content):
+    return [
+        {
+            # for companies with : in the name
+            'name': ":".join(line.split(':')[:-2]),
+            'cik': int(line.split(':')[-2])
+        } for line in content.split("\n") if line != '']
+
+
+@lru_cache(maxsize=1)
+def get_cik_lookup_data() -> pd.DataFrame:
+    """
+    Get a dataframe of company/entity names and their cik
+    or a Dict of int(cik) to str(name)
+    DECADE CAPITAL MANAGEMENT LLC:0001426822:
+    DECADE COMPANIES INCOME PROPERTIES:0000775840:
+    """
+    content = download_text("https://www.sec.gov/Archives/edgar/cik-lookup-data.txt")
+    cik_lookup_df = pd.DataFrame(_parse_cik_lookup_data(content))
+    return cik_lookup_df
+
+
 class CompanySearchResults:
 
     def __init__(self,
                  data: pd.DataFrame,
                  query: str):
         self.data = data
         self.query = query
```

### Comparing `edgartools-2.8.3/edgar/_filings.py` & `edgartools-2.9.0/edgar/_filings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1679,3506 +1679,3506 @@
 000068e0: 756d 6265 7227 3a20 6163 6365 7373 696f  umber': accessio
 000068f0: 6e5f 6e75 6d62 6572 7d29 0a20 2020 2072  n_number}).    r
 00006900: 6574 7572 6e20 656e 7472 6965 730a 0a0a  eturn entries...
 00006910: 6465 6620 6765 745f 6375 7272 656e 745f  def get_current_
 00006920: 6669 6c69 6e67 7328 666f 726d 3a20 7374  filings(form: st
 00006930: 7220 3d20 2727 2c0a 2020 2020 2020 2020  r = '',.        
 00006940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006950: 6f77 6e65 723a 2073 7472 203d 204e 6f6e  owner: str = Non
-00006960: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00006970: 2020 2020 2020 2020 2020 2070 6167 655f             page_
-00006980: 7369 7a65 3a20 696e 7420 3d20 3430 293a  size: int = 40):
-00006990: 0a20 2020 2022 2222 0a20 2020 2047 6574  .    """.    Get
-000069a0: 2074 6865 2063 7572 7265 6e74 2066 696c   the current fil
-000069b0: 696e 6773 2066 726f 6d20 7468 6520 5345  ings from the SE
-000069c0: 430a 2020 2020 3a72 6574 7572 6e3a 2054  C.    :return: T
-000069d0: 6865 2063 7572 7265 6e74 2066 696c 696e  he current filin
-000069e0: 6773 2066 726f 6d20 7468 6520 5345 430a  gs from the SEC.
-000069f0: 2020 2020 2222 220a 2020 2020 6f77 6e65      """.    owne
-00006a00: 7220 3d20 6f77 6e65 7220 6966 206f 776e  r = owner if own
-00006a10: 6572 2069 6e20 5b27 696e 636c 7564 6527  er in ['include'
-00006a20: 2c20 2765 7863 6c75 6465 272c 2027 6f6e  , 'exclude', 'on
-00006a30: 6c79 275d 2065 6c73 6520 2769 6e63 6c75  ly'] else 'inclu
-00006a40: 6465 270a 2020 2020 7061 6765 5f73 697a  de'.    page_siz
-00006a50: 6520 3d20 7061 6765 5f73 697a 6520 6966  e = page_size if
-00006a60: 2070 6167 655f 7369 7a65 2069 6e20 5b31   page_size in [1
-00006a70: 302c 2032 302c 2034 302c 2038 302c 2031  0, 20, 40, 80, 1
-00006a80: 3030 5d20 656c 7365 2034 300a 2020 2020  00] else 40.    
-00006a90: 7374 6172 7420 3d20 300a 0a20 2020 2065  start = 0..    e
-00006aa0: 6e74 7269 6573 203d 2067 6574 5f63 7572  ntries = get_cur
-00006ab0: 7265 6e74 5f65 6e74 7269 6573 5f6f 6e5f  rent_entries_on_
-00006ac0: 7061 6765 2863 6f75 6e74 3d70 6167 655f  page(count=page_
-00006ad0: 7369 7a65 2c20 7374 6172 743d 7374 6172  size, start=star
-00006ae0: 742c 2066 6f72 6d3d 666f 726d 2c20 6f77  t, form=form, ow
-00006af0: 6e65 723d 6f77 6e65 7229 0a20 2020 2069  ner=owner).    i
-00006b00: 6620 6e6f 7420 656e 7472 6965 733a 0a20  f not entries:. 
-00006b10: 2020 2020 2020 2072 6574 7572 6e20 4375         return Cu
-00006b20: 7272 656e 7446 696c 696e 6773 2866 696c  rrentFilings(fil
-00006b30: 696e 675f 696e 6465 783d 5f65 6d70 7479  ing_index=_empty
-00006b40: 5f66 696c 696e 675f 696e 6465 7828 292c  _filing_index(),
-00006b50: 206f 776e 6572 3d6f 776e 6572 2c20 666f   owner=owner, fo
-00006b60: 726d 3d66 6f72 6d2c 2070 6167 655f 7369  rm=form, page_si
-00006b70: 7a65 3d70 6167 655f 7369 7a65 290a 2020  ze=page_size).  
-00006b80: 2020 7265 7475 726e 2043 7572 7265 6e74    return Current
-00006b90: 4669 6c69 6e67 7328 6669 6c69 6e67 5f69  Filings(filing_i
-00006ba0: 6e64 6578 3d70 612e 5461 626c 652e 6672  ndex=pa.Table.fr
-00006bb0: 6f6d 5f70 796c 6973 7428 656e 7472 6965  om_pylist(entrie
-00006bc0: 7329 2c20 6f77 6e65 723d 6f77 6e65 722c  s), owner=owner,
-00006bd0: 2066 6f72 6d3d 666f 726d 2c20 7061 6765   form=form, page
-00006be0: 5f73 697a 653d 7061 6765 5f73 697a 6529  _size=page_size)
-00006bf0: 0a0a 0a63 6c61 7373 2043 7572 7265 6e74  ...class Current
-00006c00: 4669 6c69 6e67 7328 4669 6c69 6e67 7329  Filings(Filings)
-00006c10: 3a0a 2020 2020 2222 220a 2020 2020 5468  :.    """.    Th
-00006c20: 6973 2076 6572 7369 6f6e 206f 6620 7468  is version of th
-00006c30: 6520 4669 6c69 6e67 7320 636c 6173 7320  e Filings class 
-00006c40: 6973 2075 7365 6420 746f 2067 6574 2074  is used to get t
-00006c50: 6865 2063 7572 7265 6e74 2066 696c 696e  he current filin
-00006c60: 6773 2066 726f 6d20 7468 6520 5345 430a  gs from the SEC.
-00006c70: 2020 2020 7061 6765 2062 7920 7061 6765      page by page
-00006c80: 0a20 2020 2022 2222 0a0a 2020 2020 6465  .    """..    de
-00006c90: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-00006ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006cb0: 2020 6669 6c69 6e67 5f69 6e64 6578 3a20    filing_index: 
-00006cc0: 7061 2e54 6162 6c65 2c0a 2020 2020 2020  pa.Table,.      
-00006cd0: 2020 2020 2020 2020 2020 2066 6f72 6d3a             form:
-00006ce0: 2073 7472 203d 2027 272c 0a20 2020 2020   str = '',.     
-00006cf0: 2020 2020 2020 2020 2020 2020 7374 6172              star
-00006d00: 743a 2069 6e74 203d 2031 2c0a 2020 2020  t: int = 1,.    
-00006d10: 2020 2020 2020 2020 2020 2020 2070 6167               pag
-00006d20: 655f 7369 7a65 3a20 696e 7420 3d20 3430  e_size: int = 40
-00006d30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006d40: 2020 206f 776e 6572 3a20 7374 7220 3d20     owner: str = 
-00006d50: 2765 7863 6c75 6465 2729 3a0a 2020 2020  'exclude'):.    
-00006d60: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-00006d70: 6974 5f5f 2866 696c 696e 675f 696e 6465  it__(filing_inde
-00006d80: 782c 206f 7269 6769 6e61 6c5f 7374 6174  x, original_stat
-00006d90: 653d 4e6f 6e65 290a 2020 2020 2020 2020  e=None).        
-00006da0: 7365 6c66 2e5f 7374 6172 7420 3d20 7374  self._start = st
-00006db0: 6172 740a 2020 2020 2020 2020 7365 6c66  art.        self
-00006dc0: 2e5f 7061 6765 5f73 697a 6520 3d20 7061  ._page_size = pa
-00006dd0: 6765 5f73 697a 650a 2020 2020 2020 2020  ge_size.        
-00006de0: 7365 6c66 2e6f 776e 6572 203d 206f 776e  self.owner = own
-00006df0: 6572 0a20 2020 2020 2020 2073 656c 662e  er.        self.
-00006e00: 666f 726d 203d 2066 6f72 6d0a 0a20 2020  form = form..   
-00006e10: 2064 6566 206e 6578 7428 7365 6c66 293a   def next(self):
-00006e20: 0a20 2020 2020 2020 2023 2049 6620 7468  .        # If th
-00006e30: 6520 6e75 6d62 6572 206f 6620 656e 7472  e number of entr
-00006e40: 6965 7320 6973 206c 6573 7320 7468 616e  ies is less than
-00006e50: 2074 6865 2070 6167 6520 7369 7a65 2074   the page size t
-00006e60: 6865 6e20 7765 2061 7265 2061 7420 7468  hen we are at th
-00006e70: 6520 656e 6420 6f66 2074 6865 2064 6174  e end of the dat
-00006e80: 610a 2020 2020 2020 2020 6966 206c 656e  a.        if len
-00006e90: 2873 656c 662e 6461 7461 2920 3c20 7365  (self.data) < se
-00006ea0: 6c66 2e5f 7061 6765 5f73 697a 653a 0a20  lf._page_size:. 
-00006eb0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00006ec0: 6e20 4e6f 6e65 0a20 2020 2020 2020 2073  n None.        s
-00006ed0: 7461 7274 203d 2073 656c 662e 5f73 7461  tart = self._sta
-00006ee0: 7274 202b 206c 656e 2873 656c 662e 6461  rt + len(self.da
-00006ef0: 7461 290a 2020 2020 2020 2020 6e65 7874  ta).        next
-00006f00: 5f65 6e74 7269 6573 203d 2067 6574 5f63  _entries = get_c
-00006f10: 7572 7265 6e74 5f65 6e74 7269 6573 5f6f  urrent_entries_o
-00006f20: 6e5f 7061 6765 2873 7461 7274 3d73 7461  n_page(start=sta
-00006f30: 7274 2c20 636f 756e 743d 7365 6c66 2e5f  rt, count=self._
-00006f40: 7061 6765 5f73 697a 652c 2066 6f72 6d3d  page_size, form=
-00006f50: 7365 6c66 2e66 6f72 6d29 0a20 2020 2020  self.form).     
-00006f60: 2020 2069 6620 6e65 7874 5f65 6e74 7269     if next_entri
-00006f70: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-00006f80: 2320 436f 7079 2074 6865 2076 616c 7565  # Copy the value
-00006f90: 7320 746f 2074 6869 7320 4669 6c69 6e67  s to this Filing
-00006fa0: 7320 6f62 6a65 6374 2061 6e64 2072 6574  s object and ret
-00006fb0: 7572 6e20 6974 0a20 2020 2020 2020 2020  urn it.         
-00006fc0: 2020 2073 656c 662e 6461 7461 203d 2070     self.data = p
-00006fd0: 612e 5461 626c 652e 6672 6f6d 5f70 796c  a.Table.from_pyl
-00006fe0: 6973 7428 6e65 7874 5f65 6e74 7269 6573  ist(next_entries
-00006ff0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00007000: 6c66 2e5f 7374 6172 7420 3d20 7374 6172  lf._start = star
-00007010: 740a 2020 2020 2020 2020 2020 2020 7265  t.            re
-00007020: 7475 726e 2073 656c 660a 0a20 2020 2064  turn self..    d
-00007030: 6566 2070 7265 7669 6f75 7328 7365 6c66  ef previous(self
-00007040: 293a 0a20 2020 2020 2020 2023 2049 6620  ):.        # If 
-00007050: 7374 6172 7420 3d20 3120 7468 656e 2074  start = 1 then t
-00007060: 6865 7265 2061 7265 206e 6f20 7072 6576  here are no prev
-00007070: 696f 7573 2065 6e74 7269 6573 0a20 2020  ious entries.   
-00007080: 2020 2020 2069 6620 7365 6c66 2e5f 7374       if self._st
-00007090: 6172 7420 3d3d 2031 3a0a 2020 2020 2020  art == 1:.      
-000070a0: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-000070b0: 650a 2020 2020 2020 2020 7374 6172 7420  e.        start 
-000070c0: 3d20 6d61 7828 312c 2073 656c 662e 5f73  = max(1, self._s
-000070d0: 7461 7274 202d 2073 656c 662e 5f70 6167  tart - self._pag
-000070e0: 655f 7369 7a65 290a 2020 2020 2020 2020  e_size).        
-000070f0: 7072 6576 696f 7573 5f65 6e74 7269 6573  previous_entries
-00007100: 203d 2067 6574 5f63 7572 7265 6e74 5f65   = get_current_e
-00007110: 6e74 7269 6573 5f6f 6e5f 7061 6765 2873  ntries_on_page(s
-00007120: 7461 7274 3d73 7461 7274 2c20 636f 756e  tart=start, coun
-00007130: 743d 7365 6c66 2e5f 7061 6765 5f73 697a  t=self._page_siz
-00007140: 652c 2066 6f72 6d3d 7365 6c66 2e66 6f72  e, form=self.for
-00007150: 6d29 0a20 2020 2020 2020 2069 6620 7072  m).        if pr
-00007160: 6576 696f 7573 5f65 6e74 7269 6573 3a0a  evious_entries:.
-00007170: 2020 2020 2020 2020 2020 2020 2320 436f              # Co
-00007180: 7079 2074 6865 2076 616c 7565 7320 746f  py the values to
-00007190: 2074 6869 7320 4669 6c69 6e67 7320 6f62   this Filings ob
-000071a0: 6a65 6374 2061 6e64 2072 6574 7572 6e20  ject and return 
-000071b0: 6974 0a20 2020 2020 2020 2020 2020 2073  it.            s
-000071c0: 656c 662e 6461 7461 203d 2070 612e 5461  elf.data = pa.Ta
-000071d0: 626c 652e 6672 6f6d 5f70 796c 6973 7428  ble.from_pylist(
-000071e0: 7072 6576 696f 7573 5f65 6e74 7269 6573  previous_entries
-000071f0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00007200: 6c66 2e5f 7374 6172 7420 3d20 7374 6172  lf._start = star
-00007210: 740a 2020 2020 2020 2020 2020 2020 7265  t.            re
-00007220: 7475 726e 2073 656c 660a 0a20 2020 2064  turn self..    d
-00007230: 6566 205f 5f67 6574 6974 656d 5f5f 2873  ef __getitem__(s
-00007240: 656c 662c 2069 7465 6d29 3a0a 2020 2020  elf, item):.    
-00007250: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00007260: 6765 7428 6974 656d 290a 0a20 2020 2064  get(item)..    d
-00007270: 6566 2067 6574 2873 656c 662c 2069 6e64  ef get(self, ind
-00007280: 6578 5f6f 725f 6163 6365 7373 696f 6e5f  ex_or_accession_
-00007290: 6e75 6d62 6572 3a20 496e 7453 7472 696e  number: IntStrin
-000072a0: 6729 3a0a 2020 2020 2020 2020 6966 2069  g):.        if i
-000072b0: 7369 6e73 7461 6e63 6528 696e 6465 785f  sinstance(index_
-000072c0: 6f72 5f61 6363 6573 7369 6f6e 5f6e 756d  or_accession_num
-000072d0: 6265 722c 2069 6e74 2920 6f72 2069 6e64  ber, int) or ind
-000072e0: 6578 5f6f 725f 6163 6365 7373 696f 6e5f  ex_or_accession_
-000072f0: 6e75 6d62 6572 2e69 7364 6967 6974 2829  number.isdigit()
-00007300: 3a0a 2020 2020 2020 2020 2020 2020 6964  :.            id
-00007310: 7820 3d20 696e 7428 696e 6465 785f 6f72  x = int(index_or
-00007320: 5f61 6363 6573 7369 6f6e 5f6e 756d 6265  _accession_numbe
-00007330: 7229 0a20 2020 2020 2020 2020 2020 2069  r).            i
-00007340: 6620 7365 6c66 2e5f 7374 6172 7420 2d20  f self._start - 
-00007350: 3120 3c3d 2069 6478 203c 2073 656c 662e  1 <= idx < self.
-00007360: 5f73 7461 7274 202d 2031 202b 206c 656e  _start - 1 + len
-00007370: 2873 656c 662e 6461 7461 293a 0a20 2020  (self.data):.   
-00007380: 2020 2020 2020 2020 2020 2020 2023 2057               # W
-00007390: 6865 7265 206f 6e20 7468 6973 2070 6167  here on this pag
-000073a0: 6520 6973 2074 6865 2069 6e64 6578 0a20  e is the index. 
-000073b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000073c0: 6478 5f6f 6e5f 7061 6765 203d 2069 6478  dx_on_page = idx
-000073d0: 202d 2028 7365 6c66 2e5f 7374 6172 7420   - (self._start 
-000073e0: 2d20 3129 0a20 2020 2020 2020 2020 2020  - 1).           
-000073f0: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
-00007400: 7228 292e 6765 745f 6669 6c69 6e67 5f61  r().get_filing_a
-00007410: 7428 6964 785f 6f6e 5f70 6167 6529 0a20  t(idx_on_page). 
-00007420: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00007430: 2020 2020 2020 2020 2061 6363 6573 7369           accessi
-00007440: 6f6e 5f6e 756d 6265 7220 3d20 696e 6465  on_number = inde
-00007450: 785f 6f72 5f61 6363 6573 7369 6f6e 5f6e  x_or_accession_n
-00007460: 756d 6265 722e 7374 7269 7028 290a 2020  umber.strip().  
-00007470: 2020 2020 2020 2020 2020 2320 5365 6520            # See 
-00007480: 6966 2074 6865 2066 696c 696e 6720 6973  if the filing is
-00007490: 2069 6e20 7468 6973 2070 6167 650a 2020   in this page.  
-000074a0: 2020 2020 2020 2020 2020 6669 6c69 6e67            filing
-000074b0: 203d 2073 7570 6572 2829 2e67 6574 2861   = super().get(a
-000074c0: 6363 6573 7369 6f6e 5f6e 756d 6265 7229  ccession_number)
-000074d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000074e0: 6669 6c69 6e67 3a0a 2020 2020 2020 2020  filing:.        
-000074f0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-00007500: 696c 696e 670a 0a20 2020 2020 2020 2020  iling..         
-00007510: 2020 2063 7572 7265 6e74 5f66 696c 696e     current_filin
-00007520: 6773 203d 2067 6574 5f63 7572 7265 6e74  gs = get_current
-00007530: 5f66 696c 696e 6773 2873 656c 662e 666f  _filings(self.fo
-00007540: 726d 2c20 7365 6c66 2e6f 776e 6572 2c20  rm, self.owner, 
-00007550: 7061 6765 5f73 697a 653d 3130 3029 0a20  page_size=100). 
-00007560: 2020 2020 2020 2020 2020 2066 696c 696e             filin
-00007570: 6720 3d20 4375 7272 656e 7446 696c 696e  g = CurrentFilin
-00007580: 6773 2e5f 6765 745f 6375 7272 656e 745f  gs._get_current_
-00007590: 6669 6c69 6e67 5f62 795f 6163 6365 7373  filing_by_access
-000075a0: 696f 6e5f 6e75 6d62 6572 2863 7572 7265  ion_number(curre
-000075b0: 6e74 5f66 696c 696e 6773 2e64 6174 612c  nt_filings.data,
-000075c0: 2061 6363 6573 7369 6f6e 5f6e 756d 6265   accession_numbe
-000075d0: 7229 0a20 2020 2020 2020 2020 2020 2069  r).            i
-000075e0: 6620 6669 6c69 6e67 3a0a 2020 2020 2020  f filing:.      
-000075f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00007600: 2066 696c 696e 670a 2020 2020 2020 2020   filing.        
-00007610: 2020 2020 7769 7468 2053 7461 7475 7328      with Status(
-00007620: 6622 5b62 6f6c 6420 6465 6570 5f73 6b79  f"[bold deep_sky
-00007630: 5f62 6c75 6531 5d53 6561 7263 6869 6e67  _blue1]Searching
-00007640: 2074 6872 6f75 6768 2074 6865 206d 6f73   through the mos
-00007650: 7420 7265 6365 6e74 2066 696c 696e 6773  t recent filings
-00007660: 2066 6f72 207b 6163 6365 7373 696f 6e5f   for {accession_
-00007670: 6e75 6d62 6572 7d2e 2e2e 222c 0a20 2020  number}...",.   
-00007680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007690: 2020 2020 2073 7069 6e6e 6572 3d22 646f       spinner="do
-000076a0: 7473 3222 293a 0a20 2020 2020 2020 2020  ts2"):.         
-000076b0: 2020 2020 2020 2077 6869 6c65 2054 7275         while Tru
-000076c0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000076d0: 2020 2020 2020 2063 7572 7265 6e74 5f66         current_f
-000076e0: 696c 696e 6773 203d 2063 7572 7265 6e74  ilings = current
-000076f0: 5f66 696c 696e 6773 2e6e 6578 7428 290a  _filings.next().
-00007700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007710: 2020 2020 6966 2063 7572 7265 6e74 5f66      if current_f
-00007720: 696c 696e 6773 2069 7320 4e6f 6e65 3a0a  ilings is None:.
-00007730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007740: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-00007750: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-00007760: 2020 2020 2020 2020 6669 6c69 6e67 203d          filing =
-00007770: 2043 7572 7265 6e74 4669 6c69 6e67 732e   CurrentFilings.
-00007780: 5f67 6574 5f63 7572 7265 6e74 5f66 696c  _get_current_fil
-00007790: 696e 675f 6279 5f61 6363 6573 7369 6f6e  ing_by_accession
-000077a0: 5f6e 756d 6265 7228 6375 7272 656e 745f  _number(current_
-000077b0: 6669 6c69 6e67 732e 6461 7461 2c0a 2020  filings.data,.  
-000077c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006950: 6f77 6e65 723a 2073 7472 203d 2027 696e  owner: str = 'in
+00006960: 636c 7564 6527 2c0a 2020 2020 2020 2020  clude',.        
+00006970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006980: 7061 6765 5f73 697a 653a 2069 6e74 203d  page_size: int =
+00006990: 2034 3029 3a0a 2020 2020 2222 220a 2020   40):.    """.  
+000069a0: 2020 4765 7420 7468 6520 6375 7272 656e    Get the curren
+000069b0: 7420 6669 6c69 6e67 7320 6672 6f6d 2074  t filings from t
+000069c0: 6865 2053 4543 0a20 2020 203a 7265 7475  he SEC.    :retu
+000069d0: 726e 3a20 5468 6520 6375 7272 656e 7420  rn: The current 
+000069e0: 6669 6c69 6e67 7320 6672 6f6d 2074 6865  filings from the
+000069f0: 2053 4543 0a20 2020 2022 2222 0a20 2020   SEC.    """.   
+00006a00: 206f 776e 6572 203d 206f 776e 6572 2069   owner = owner i
+00006a10: 6620 6f77 6e65 7220 696e 205b 2769 6e63  f owner in ['inc
+00006a20: 6c75 6465 272c 2027 6578 636c 7564 6527  lude', 'exclude'
+00006a30: 2c20 276f 6e6c 7927 5d20 656c 7365 2027  , 'only'] else '
+00006a40: 696e 636c 7564 6527 0a20 2020 2070 6167  include'.    pag
+00006a50: 655f 7369 7a65 203d 2070 6167 655f 7369  e_size = page_si
+00006a60: 7a65 2069 6620 7061 6765 5f73 697a 6520  ze if page_size 
+00006a70: 696e 205b 3130 2c20 3230 2c20 3430 2c20  in [10, 20, 40, 
+00006a80: 3830 2c20 3130 305d 2065 6c73 6520 3430  80, 100] else 40
+00006a90: 0a20 2020 2073 7461 7274 203d 2030 0a0a  .    start = 0..
+00006aa0: 2020 2020 656e 7472 6965 7320 3d20 6765      entries = ge
+00006ab0: 745f 6375 7272 656e 745f 656e 7472 6965  t_current_entrie
+00006ac0: 735f 6f6e 5f70 6167 6528 636f 756e 743d  s_on_page(count=
+00006ad0: 7061 6765 5f73 697a 652c 2073 7461 7274  page_size, start
+00006ae0: 3d73 7461 7274 2c20 666f 726d 3d66 6f72  =start, form=for
+00006af0: 6d2c 206f 776e 6572 3d6f 776e 6572 290a  m, owner=owner).
+00006b00: 2020 2020 6966 206e 6f74 2065 6e74 7269      if not entri
+00006b10: 6573 3a0a 2020 2020 2020 2020 7265 7475  es:.        retu
+00006b20: 726e 2043 7572 7265 6e74 4669 6c69 6e67  rn CurrentFiling
+00006b30: 7328 6669 6c69 6e67 5f69 6e64 6578 3d5f  s(filing_index=_
+00006b40: 656d 7074 795f 6669 6c69 6e67 5f69 6e64  empty_filing_ind
+00006b50: 6578 2829 2c20 6f77 6e65 723d 6f77 6e65  ex(), owner=owne
+00006b60: 722c 2066 6f72 6d3d 666f 726d 2c20 7061  r, form=form, pa
+00006b70: 6765 5f73 697a 653d 7061 6765 5f73 697a  ge_size=page_siz
+00006b80: 6529 0a20 2020 2072 6574 7572 6e20 4375  e).    return Cu
+00006b90: 7272 656e 7446 696c 696e 6773 2866 696c  rrentFilings(fil
+00006ba0: 696e 675f 696e 6465 783d 7061 2e54 6162  ing_index=pa.Tab
+00006bb0: 6c65 2e66 726f 6d5f 7079 6c69 7374 2865  le.from_pylist(e
+00006bc0: 6e74 7269 6573 292c 206f 776e 6572 3d6f  ntries), owner=o
+00006bd0: 776e 6572 2c20 666f 726d 3d66 6f72 6d2c  wner, form=form,
+00006be0: 2070 6167 655f 7369 7a65 3d70 6167 655f   page_size=page_
+00006bf0: 7369 7a65 290a 0a0a 636c 6173 7320 4375  size)...class Cu
+00006c00: 7272 656e 7446 696c 696e 6773 2846 696c  rrentFilings(Fil
+00006c10: 696e 6773 293a 0a20 2020 2022 2222 0a20  ings):.    """. 
+00006c20: 2020 2054 6869 7320 7665 7273 696f 6e20     This version 
+00006c30: 6f66 2074 6865 2046 696c 696e 6773 2063  of the Filings c
+00006c40: 6c61 7373 2069 7320 7573 6564 2074 6f20  lass is used to 
+00006c50: 6765 7420 7468 6520 6375 7272 656e 7420  get the current 
+00006c60: 6669 6c69 6e67 7320 6672 6f6d 2074 6865  filings from the
+00006c70: 2053 4543 0a20 2020 2070 6167 6520 6279   SEC.    page by
+00006c80: 2070 6167 650a 2020 2020 2222 220a 0a20   page.    """.. 
+00006c90: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00006ca0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+00006cb0: 2020 2020 2020 2066 696c 696e 675f 696e         filing_in
+00006cc0: 6465 783a 2070 612e 5461 626c 652c 0a20  dex: pa.Table,. 
+00006cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ce0: 666f 726d 3a20 7374 7220 3d20 2727 2c0a  form: str = '',.
+00006cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d00: 2073 7461 7274 3a20 696e 7420 3d20 312c   start: int = 1,
+00006d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006d20: 2020 7061 6765 5f73 697a 653a 2069 6e74    page_size: int
+00006d30: 203d 2034 302c 0a20 2020 2020 2020 2020   = 40,.         
+00006d40: 2020 2020 2020 2020 6f77 6e65 723a 2073          owner: s
+00006d50: 7472 203d 2027 696e 636c 7564 6527 293a  tr = 'include'):
+00006d60: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+00006d70: 2e5f 5f69 6e69 745f 5f28 6669 6c69 6e67  .__init__(filing
+00006d80: 5f69 6e64 6578 2c20 6f72 6967 696e 616c  _index, original
+00006d90: 5f73 7461 7465 3d4e 6f6e 6529 0a20 2020  _state=None).   
+00006da0: 2020 2020 2073 656c 662e 5f73 7461 7274       self._start
+00006db0: 203d 2073 7461 7274 0a20 2020 2020 2020   = start.       
+00006dc0: 2073 656c 662e 5f70 6167 655f 7369 7a65   self._page_size
+00006dd0: 203d 2070 6167 655f 7369 7a65 0a20 2020   = page_size.   
+00006de0: 2020 2020 2073 656c 662e 6f77 6e65 7220       self.owner 
+00006df0: 3d20 6f77 6e65 720a 2020 2020 2020 2020  = owner.        
+00006e00: 7365 6c66 2e66 6f72 6d20 3d20 666f 726d  self.form = form
+00006e10: 0a0a 2020 2020 6465 6620 6e65 7874 2873  ..    def next(s
+00006e20: 656c 6629 3a0a 2020 2020 2020 2020 2320  elf):.        # 
+00006e30: 4966 2074 6865 206e 756d 6265 7220 6f66  If the number of
+00006e40: 2065 6e74 7269 6573 2069 7320 6c65 7373   entries is less
+00006e50: 2074 6861 6e20 7468 6520 7061 6765 2073   than the page s
+00006e60: 697a 6520 7468 656e 2077 6520 6172 6520  ize then we are 
+00006e70: 6174 2074 6865 2065 6e64 206f 6620 7468  at the end of th
+00006e80: 6520 6461 7461 0a20 2020 2020 2020 2069  e data.        i
+00006e90: 6620 6c65 6e28 7365 6c66 2e64 6174 6129  f len(self.data)
+00006ea0: 203c 2073 656c 662e 5f70 6167 655f 7369   < self._page_si
+00006eb0: 7a65 3a0a 2020 2020 2020 2020 2020 2020  ze:.            
+00006ec0: 7265 7475 726e 204e 6f6e 650a 2020 2020  return None.    
+00006ed0: 2020 2020 7374 6172 7420 3d20 7365 6c66      start = self
+00006ee0: 2e5f 7374 6172 7420 2b20 6c65 6e28 7365  ._start + len(se
+00006ef0: 6c66 2e64 6174 6129 0a20 2020 2020 2020  lf.data).       
+00006f00: 206e 6578 745f 656e 7472 6965 7320 3d20   next_entries = 
+00006f10: 6765 745f 6375 7272 656e 745f 656e 7472  get_current_entr
+00006f20: 6965 735f 6f6e 5f70 6167 6528 7374 6172  ies_on_page(star
+00006f30: 743d 7374 6172 742c 2063 6f75 6e74 3d73  t=start, count=s
+00006f40: 656c 662e 5f70 6167 655f 7369 7a65 2c20  elf._page_size, 
+00006f50: 666f 726d 3d73 656c 662e 666f 726d 290a  form=self.form).
+00006f60: 2020 2020 2020 2020 6966 206e 6578 745f          if next_
+00006f70: 656e 7472 6965 733a 0a20 2020 2020 2020  entries:.       
+00006f80: 2020 2020 2023 2043 6f70 7920 7468 6520       # Copy the 
+00006f90: 7661 6c75 6573 2074 6f20 7468 6973 2046  values to this F
+00006fa0: 696c 696e 6773 206f 626a 6563 7420 616e  ilings object an
+00006fb0: 6420 7265 7475 726e 2069 740a 2020 2020  d return it.    
+00006fc0: 2020 2020 2020 2020 7365 6c66 2e64 6174          self.dat
+00006fd0: 6120 3d20 7061 2e54 6162 6c65 2e66 726f  a = pa.Table.fro
+00006fe0: 6d5f 7079 6c69 7374 286e 6578 745f 656e  m_pylist(next_en
+00006ff0: 7472 6965 7329 0a20 2020 2020 2020 2020  tries).         
+00007000: 2020 2073 656c 662e 5f73 7461 7274 203d     self._start =
+00007010: 2073 7461 7274 0a20 2020 2020 2020 2020   start.         
+00007020: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+00007030: 2020 2020 6465 6620 7072 6576 696f 7573      def previous
+00007040: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00007050: 2320 4966 2073 7461 7274 203d 2031 2074  # If start = 1 t
+00007060: 6865 6e20 7468 6572 6520 6172 6520 6e6f  hen there are no
+00007070: 2070 7265 7669 6f75 7320 656e 7472 6965   previous entrie
+00007080: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
+00007090: 662e 5f73 7461 7274 203d 3d20 313a 0a20  f._start == 1:. 
+000070a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000070b0: 6e20 4e6f 6e65 0a20 2020 2020 2020 2073  n None.        s
+000070c0: 7461 7274 203d 206d 6178 2831 2c20 7365  tart = max(1, se
+000070d0: 6c66 2e5f 7374 6172 7420 2d20 7365 6c66  lf._start - self
+000070e0: 2e5f 7061 6765 5f73 697a 6529 0a20 2020  ._page_size).   
+000070f0: 2020 2020 2070 7265 7669 6f75 735f 656e       previous_en
+00007100: 7472 6965 7320 3d20 6765 745f 6375 7272  tries = get_curr
+00007110: 656e 745f 656e 7472 6965 735f 6f6e 5f70  ent_entries_on_p
+00007120: 6167 6528 7374 6172 743d 7374 6172 742c  age(start=start,
+00007130: 2063 6f75 6e74 3d73 656c 662e 5f70 6167   count=self._pag
+00007140: 655f 7369 7a65 2c20 666f 726d 3d73 656c  e_size, form=sel
+00007150: 662e 666f 726d 290a 2020 2020 2020 2020  f.form).        
+00007160: 6966 2070 7265 7669 6f75 735f 656e 7472  if previous_entr
+00007170: 6965 733a 0a20 2020 2020 2020 2020 2020  ies:.           
+00007180: 2023 2043 6f70 7920 7468 6520 7661 6c75   # Copy the valu
+00007190: 6573 2074 6f20 7468 6973 2046 696c 696e  es to this Filin
+000071a0: 6773 206f 626a 6563 7420 616e 6420 7265  gs object and re
+000071b0: 7475 726e 2069 740a 2020 2020 2020 2020  turn it.        
+000071c0: 2020 2020 7365 6c66 2e64 6174 6120 3d20      self.data = 
+000071d0: 7061 2e54 6162 6c65 2e66 726f 6d5f 7079  pa.Table.from_py
+000071e0: 6c69 7374 2870 7265 7669 6f75 735f 656e  list(previous_en
+000071f0: 7472 6965 7329 0a20 2020 2020 2020 2020  tries).         
+00007200: 2020 2073 656c 662e 5f73 7461 7274 203d     self._start =
+00007210: 2073 7461 7274 0a20 2020 2020 2020 2020   start.         
+00007220: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+00007230: 2020 2020 6465 6620 5f5f 6765 7469 7465      def __getite
+00007240: 6d5f 5f28 7365 6c66 2c20 6974 656d 293a  m__(self, item):
+00007250: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00007260: 7365 6c66 2e67 6574 2869 7465 6d29 0a0a  self.get(item)..
+00007270: 2020 2020 6465 6620 6765 7428 7365 6c66      def get(self
+00007280: 2c20 696e 6465 785f 6f72 5f61 6363 6573  , index_or_acces
+00007290: 7369 6f6e 5f6e 756d 6265 723a 2049 6e74  sion_number: Int
+000072a0: 5374 7269 6e67 293a 0a20 2020 2020 2020  String):.       
+000072b0: 2069 6620 6973 696e 7374 616e 6365 2869   if isinstance(i
+000072c0: 6e64 6578 5f6f 725f 6163 6365 7373 696f  ndex_or_accessio
+000072d0: 6e5f 6e75 6d62 6572 2c20 696e 7429 206f  n_number, int) o
+000072e0: 7220 696e 6465 785f 6f72 5f61 6363 6573  r index_or_acces
+000072f0: 7369 6f6e 5f6e 756d 6265 722e 6973 6469  sion_number.isdi
+00007300: 6769 7428 293a 0a20 2020 2020 2020 2020  git():.         
+00007310: 2020 2069 6478 203d 2069 6e74 2869 6e64     idx = int(ind
+00007320: 6578 5f6f 725f 6163 6365 7373 696f 6e5f  ex_or_accession_
+00007330: 6e75 6d62 6572 290a 2020 2020 2020 2020  number).        
+00007340: 2020 2020 6966 2073 656c 662e 5f73 7461      if self._sta
+00007350: 7274 202d 2031 203c 3d20 6964 7820 3c20  rt - 1 <= idx < 
+00007360: 7365 6c66 2e5f 7374 6172 7420 2d20 3120  self._start - 1 
+00007370: 2b20 6c65 6e28 7365 6c66 2e64 6174 6129  + len(self.data)
+00007380: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007390: 2020 2320 5768 6572 6520 6f6e 2074 6869    # Where on thi
+000073a0: 7320 7061 6765 2069 7320 7468 6520 696e  s page is the in
+000073b0: 6465 780a 2020 2020 2020 2020 2020 2020  dex.            
+000073c0: 2020 2020 6964 785f 6f6e 5f70 6167 6520      idx_on_page 
+000073d0: 3d20 6964 7820 2d20 2873 656c 662e 5f73  = idx - (self._s
+000073e0: 7461 7274 202d 2031 290a 2020 2020 2020  tart - 1).      
+000073f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00007400: 2073 7570 6572 2829 2e67 6574 5f66 696c   super().get_fil
+00007410: 696e 675f 6174 2869 6478 5f6f 6e5f 7061  ing_at(idx_on_pa
+00007420: 6765 290a 2020 2020 2020 2020 656c 7365  ge).        else
+00007430: 3a0a 2020 2020 2020 2020 2020 2020 6163  :.            ac
+00007440: 6365 7373 696f 6e5f 6e75 6d62 6572 203d  cession_number =
+00007450: 2069 6e64 6578 5f6f 725f 6163 6365 7373   index_or_access
+00007460: 696f 6e5f 6e75 6d62 6572 2e73 7472 6970  ion_number.strip
+00007470: 2829 0a20 2020 2020 2020 2020 2020 2023  ().            #
+00007480: 2053 6565 2069 6620 7468 6520 6669 6c69   See if the fili
+00007490: 6e67 2069 7320 696e 2074 6869 7320 7061  ng is in this pa
+000074a0: 6765 0a20 2020 2020 2020 2020 2020 2066  ge.            f
+000074b0: 696c 696e 6720 3d20 7375 7065 7228 292e  iling = super().
+000074c0: 6765 7428 6163 6365 7373 696f 6e5f 6e75  get(accession_nu
+000074d0: 6d62 6572 290a 2020 2020 2020 2020 2020  mber).          
+000074e0: 2020 6966 2066 696c 696e 673a 0a20 2020    if filing:.   
+000074f0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00007500: 7572 6e20 6669 6c69 6e67 0a0a 2020 2020  urn filing..    
+00007510: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00007520: 6669 6c69 6e67 7320 3d20 6765 745f 6375  filings = get_cu
+00007530: 7272 656e 745f 6669 6c69 6e67 7328 7365  rrent_filings(se
+00007540: 6c66 2e66 6f72 6d2c 2073 656c 662e 6f77  lf.form, self.ow
+00007550: 6e65 722c 2070 6167 655f 7369 7a65 3d31  ner, page_size=1
+00007560: 3030 290a 2020 2020 2020 2020 2020 2020  00).            
+00007570: 6669 6c69 6e67 203d 2043 7572 7265 6e74  filing = Current
+00007580: 4669 6c69 6e67 732e 5f67 6574 5f63 7572  Filings._get_cur
+00007590: 7265 6e74 5f66 696c 696e 675f 6279 5f61  rent_filing_by_a
+000075a0: 6363 6573 7369 6f6e 5f6e 756d 6265 7228  ccession_number(
+000075b0: 6375 7272 656e 745f 6669 6c69 6e67 732e  current_filings.
+000075c0: 6461 7461 2c20 6163 6365 7373 696f 6e5f  data, accession_
+000075d0: 6e75 6d62 6572 290a 2020 2020 2020 2020  number).        
+000075e0: 2020 2020 6966 2066 696c 696e 673a 0a20      if filing:. 
+000075f0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00007600: 6574 7572 6e20 6669 6c69 6e67 0a20 2020  eturn filing.   
+00007610: 2020 2020 2020 2020 2077 6974 6820 5374           with St
+00007620: 6174 7573 2866 225b 626f 6c64 2064 6565  atus(f"[bold dee
+00007630: 705f 736b 795f 626c 7565 315d 5365 6172  p_sky_blue1]Sear
+00007640: 6368 696e 6720 7468 726f 7567 6820 7468  ching through th
+00007650: 6520 6d6f 7374 2072 6563 656e 7420 6669  e most recent fi
+00007660: 6c69 6e67 7320 666f 7220 7b61 6363 6573  lings for {acces
+00007670: 7369 6f6e 5f6e 756d 6265 727d 2e2e 2e22  sion_number}..."
+00007680: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007690: 2020 2020 2020 2020 2020 7370 696e 6e65            spinne
+000076a0: 723d 2264 6f74 7332 2229 3a0a 2020 2020  r="dots2"):.    
+000076b0: 2020 2020 2020 2020 2020 2020 7768 696c              whil
+000076c0: 6520 5472 7565 3a0a 2020 2020 2020 2020  e True:.        
+000076d0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+000076e0: 656e 745f 6669 6c69 6e67 7320 3d20 6375  ent_filings = cu
+000076f0: 7272 656e 745f 6669 6c69 6e67 732e 6e65  rrent_filings.ne
+00007700: 7874 2829 0a20 2020 2020 2020 2020 2020  xt().           
+00007710: 2020 2020 2020 2020 2069 6620 6375 7272           if curr
+00007720: 656e 745f 6669 6c69 6e67 7320 6973 204e  ent_filings is N
+00007730: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00007740: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00007750: 7572 6e20 4e6f 6e65 0a20 2020 2020 2020  urn None.       
+00007760: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+00007770: 696e 6720 3d20 4375 7272 656e 7446 696c  ing = CurrentFil
+00007780: 696e 6773 2e5f 6765 745f 6375 7272 656e  ings._get_curren
+00007790: 745f 6669 6c69 6e67 5f62 795f 6163 6365  t_filing_by_acce
+000077a0: 7373 696f 6e5f 6e75 6d62 6572 2863 7572  ssion_number(cur
+000077b0: 7265 6e74 5f66 696c 696e 6773 2e64 6174  rent_filings.dat
+000077c0: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
 000077d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000077e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000077f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007810: 2020 6163 6365 7373 696f 6e5f 6e75 6d62    accession_numb
-00007820: 6572 290a 2020 2020 2020 2020 2020 2020  er).            
-00007830: 2020 2020 2020 2020 6966 2066 696c 696e          if filin
-00007840: 673a 0a20 2020 2020 2020 2020 2020 2020  g:.             
-00007850: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00007860: 6e20 6669 6c69 6e67 0a0a 2020 2020 4073  n filing..    @s
-00007870: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
-00007880: 6465 6620 5f67 6574 5f63 7572 7265 6e74  def _get_current
-00007890: 5f66 696c 696e 675f 6279 5f61 6363 6573  _filing_by_acces
-000078a0: 7369 6f6e 5f6e 756d 6265 7228 6461 7461  sion_number(data
-000078b0: 3a20 7061 2e54 6162 6c65 2c20 6163 6365  : pa.Table, acce
-000078c0: 7373 696f 6e5f 6e75 6d62 6572 3a20 7374  ssion_number: st
-000078d0: 7229 3a0a 2020 2020 2020 2020 6d61 736b  r):.        mask
-000078e0: 203d 2070 632e 6571 7561 6c28 6461 7461   = pc.equal(data
-000078f0: 5b27 6163 6365 7373 696f 6e5f 6e75 6d62  ['accession_numb
-00007900: 6572 275d 2c20 6163 6365 7373 696f 6e5f  er'], accession_
-00007910: 6e75 6d62 6572 290a 2020 2020 2020 2020  number).        
-00007920: 6964 7820 3d20 6d61 736b 2e69 6e64 6578  idx = mask.index
-00007930: 2854 7275 6529 2e61 735f 7079 2829 0a20  (True).as_py(). 
-00007940: 2020 2020 2020 2069 6620 6964 7820 3e20         if idx > 
-00007950: 2d31 3a0a 2020 2020 2020 2020 2020 2020  -1:.            
-00007960: 7265 7475 726e 2046 696c 696e 6728 0a20  return Filing(. 
-00007970: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00007980: 696b 3d64 6174 615b 2763 696b 275d 5b69  ik=data['cik'][i
-00007990: 6478 5d2e 6173 5f70 7928 292c 0a20 2020  dx].as_py(),.   
-000079a0: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
-000079b0: 7061 6e79 3d64 6174 615b 2763 6f6d 7061  pany=data['compa
-000079c0: 6e79 275d 5b69 6478 5d2e 6173 5f70 7928  ny'][idx].as_py(
-000079d0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-000079e0: 2020 2066 6f72 6d3d 6461 7461 5b27 666f     form=data['fo
-000079f0: 726d 275d 5b69 6478 5d2e 6173 5f70 7928  rm'][idx].as_py(
-00007a00: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00007a10: 2020 2066 696c 696e 675f 6461 7465 3d64     filing_date=d
-00007a20: 6174 615b 2766 696c 696e 675f 6461 7465  ata['filing_date
-00007a30: 275d 5b69 6478 5d2e 6173 5f70 7928 292c  '][idx].as_py(),
-00007a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007a50: 2061 6363 6573 7369 6f6e 5f6e 6f3d 6461   accession_no=da
-00007a60: 7461 5b27 6163 6365 7373 696f 6e5f 6e75  ta['accession_nu
-00007a70: 6d62 6572 275d 5b69 6478 5d2e 6173 5f70  mber'][idx].as_p
-00007a80: 7928 292c 0a20 2020 2020 2020 2020 2020  y(),.           
-00007a90: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
-00007aa0: 6e20 4e6f 6e65 0a0a 2020 2020 6465 6620  n None..    def 
-00007ab0: 5f5f 7269 6368 5f5f 2873 656c 6629 3a0a  __rich__(self):.
-00007ac0: 2020 2020 2020 2020 7061 6765 3a20 7064          page: pd
-00007ad0: 2e44 6174 6146 7261 6d65 203d 2073 656c  .DataFrame = sel
-00007ae0: 662e 746f 5f70 616e 6461 7328 290a 0a20  f.to_pandas().. 
-00007af0: 2020 2020 2020 2023 2063 6f6d 7075 7465         # compute
-00007b00: 2074 6865 2069 6e64 6578 2066 726f 6d20   the index from 
-00007b10: 7468 6520 7374 6172 7420 616e 6420 7061  the start and pa
-00007b20: 6765 5f73 697a 6520 616e 6420 7365 7420  ge_size and set 
-00007b30: 6974 2061 7320 7468 6520 696e 6465 7820  it as the index 
-00007b40: 6f66 2074 6865 2070 6167 650a 2020 2020  of the page.    
-00007b50: 2020 2020 7061 6765 2e69 6e64 6578 203d      page.index =
-00007b60: 2072 616e 6765 2873 656c 662e 5f73 7461   range(self._sta
-00007b70: 7274 202d 2031 2c20 7365 6c66 2e5f 7374  rt - 1, self._st
-00007b80: 6172 7420 2d20 3120 2b20 6c65 6e28 7061  art - 1 + len(pa
-00007b90: 6765 2929 0a0a 2020 2020 2020 2020 7265  ge))..        re
-00007ba0: 7475 726e 2050 616e 656c 280a 2020 2020  turn Panel(.    
-00007bb0: 2020 2020 2020 2020 4772 6f75 7028 0a20          Group(. 
-00007bc0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00007bd0: 665f 746f 5f72 6963 685f 7461 626c 6528  f_to_rich_table(
-00007be0: 7061 6765 292c 0a20 2020 2020 2020 2020  page),.         
-00007bf0: 2020 2020 2020 2054 6578 7428 6622 4669         Text(f"Fi
-00007c00: 6c69 6e67 7320 7b70 6167 652e 696e 6465  lings {page.inde
-00007c10: 782e 6d69 6e28 297d 2074 6f20 7b70 6167  x.min()} to {pag
-00007c20: 652e 696e 6465 782e 6d61 7828 297d 2229  e.index.max()}")
-00007c30: 0a20 2020 2020 2020 2020 2020 2029 2c20  .            ), 
-00007c40: 7469 746c 653d 6622 4375 7272 656e 7420  title=f"Current 
-00007c50: 4669 6c69 6e67 7320 6f6e 207b 7365 6c66  Filings on {self
-00007c60: 2e73 7461 7274 5f64 6174 657d 220a 2020  .start_date}".  
-00007c70: 2020 2020 2020 290a 0a0a 406c 7275 5f63        )...@lru_c
-00007c80: 6163 6865 286d 6178 7369 7a65 3d38 290a  ache(maxsize=8).
-00007c90: 6465 6620 5f67 6574 5f63 6163 6865 645f  def _get_cached_
-00007ca0: 6669 6c69 6e67 7328 7965 6172 3a20 5965  filings(year: Ye
-00007cb0: 6172 7320 3d20 4e6f 6e65 2c0a 2020 2020  ars = None,.    
-00007cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cd0: 2020 2020 7175 6172 7465 723a 2051 7561      quarter: Qua
-00007ce0: 7274 6572 7320 3d20 4e6f 6e65 2c0a 2020  rters = None,.  
-00007cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d00: 2020 2020 2020 666f 726d 3a20 556e 696f        form: Unio
-00007d10: 6e5b 7374 722c 204c 6973 745b 496e 7453  n[str, List[IntS
-00007d20: 7472 696e 675d 5d20 3d20 4e6f 6e65 2c0a  tring]] = None,.
-00007d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d40: 2020 2020 2020 2020 616d 656e 646d 656e          amendmen
-00007d50: 7473 3a20 626f 6f6c 203d 2054 7275 652c  ts: bool = True,
-00007d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007d70: 2020 2020 2020 2020 2066 696c 696e 675f           filing_
-00007d80: 6461 7465 3a20 7374 7220 3d20 4e6f 6e65  date: str = None
-00007d90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007da0: 2020 2020 2020 2020 2020 696e 6465 783d            index=
-00007db0: 2266 6f72 6d22 2920 2d3e 2046 696c 696e  "form") -> Filin
-00007dc0: 6773 3a0a 2020 2020 2320 4765 7420 7468  gs:.    # Get th
-00007dd0: 6520 6669 6c69 6e67 7320 6275 7420 6361  e filings but ca
-00007de0: 6368 6520 7468 6520 7265 7375 6c74 0a20  che the result. 
-00007df0: 2020 2072 6574 7572 6e20 6765 745f 6669     return get_fi
-00007e00: 6c69 6e67 7328 7965 6172 3d79 6561 722c  lings(year=year,
-00007e10: 2071 7561 7274 6572 3d71 7561 7274 6572   quarter=quarter
-00007e20: 2c20 666f 726d 3d66 6f72 6d2c 2061 6d65  , form=form, ame
-00007e30: 6e64 6d65 6e74 733d 616d 656e 646d 656e  ndments=amendmen
-00007e40: 7473 2c20 6669 6c69 6e67 5f64 6174 653d  ts, filing_date=
-00007e50: 6669 6c69 6e67 5f64 6174 652c 0a20 2020  filing_date,.   
-00007e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e70: 2020 2020 696e 6465 783d 696e 6465 7829      index=index)
-00007e80: 0a0a 0a64 6566 2070 6172 7365 5f66 696c  ...def parse_fil
-00007e90: 696e 675f 6865 6164 6572 2863 6f6e 7465  ing_header(conte
-00007ea0: 6e74 293a 0a20 2020 2064 6174 6120 3d20  nt):.    data = 
-00007eb0: 7b7d 0a20 2020 2063 7572 7265 6e74 5f6b  {}.    current_k
-00007ec0: 6579 203d 204e 6f6e 650a 0a20 2020 206c  ey = None..    l
-00007ed0: 696e 6573 203d 2063 6f6e 7465 6e74 2e73  ines = content.s
-00007ee0: 706c 6974 2827 5c6e 2729 0a20 2020 2066  plit('\n').    f
-00007ef0: 6f72 206c 696e 6520 696e 206c 696e 6573  or line in lines
-00007f00: 3a0a 2020 2020 2020 2020 6966 206c 696e  :.        if lin
-00007f10: 652e 656e 6473 7769 7468 2827 3a27 293a  e.endswith(':'):
-00007f20: 0a20 2020 2020 2020 2020 2020 2063 7572  .            cur
-00007f30: 7265 6e74 5f6b 6579 203d 206c 696e 655b  rent_key = line[
-00007f40: 3a2d 315d 2020 2320 5265 6d6f 7665 2074  :-1]  # Remove t
-00007f50: 6865 2074 7261 696c 696e 6720 636f 6c6f  he trailing colo
-00007f60: 6e0a 2020 2020 2020 2020 2020 2020 6461  n.            da
-00007f70: 7461 5b63 7572 7265 6e74 5f6b 6579 5d20  ta[current_key] 
-00007f80: 3d20 7b7d 0a20 2020 2020 2020 2065 6c69  = {}.        eli
-00007f90: 6620 6375 7272 656e 745f 6b65 7920 616e  f current_key an
-00007fa0: 6420 273a 2720 696e 206c 696e 653a 0a20  d ':' in line:. 
-00007fb0: 2020 2020 2020 2020 2020 206b 6579 2c20             key, 
-00007fc0: 7661 6c75 6520 3d20 6d61 7028 7374 722e  value = map(str.
-00007fd0: 7374 7269 702c 206c 696e 652e 7370 6c69  strip, line.spli
-00007fe0: 7428 273a 272c 2031 2929 0a20 2020 2020  t(':', 1)).     
-00007ff0: 2020 2020 2020 2064 6174 615b 6375 7272         data[curr
-00008000: 656e 745f 6b65 795d 5b6b 6579 5d20 3d20  ent_key][key] = 
-00008010: 7661 6c75 650a 0a20 2020 2072 6574 7572  value..    retur
-00008020: 6e20 6461 7461 0a0a 0a40 6461 7461 636c  n data...@datacl
-00008030: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
-00008040: 0a63 6c61 7373 2043 6f6d 7061 6e79 496e  .class CompanyIn
-00008050: 666f 726d 6174 696f 6e3a 0a20 2020 206e  formation:.    n
-00008060: 616d 653a 2073 7472 0a20 2020 2063 696b  ame: str.    cik
-00008070: 3a20 7374 720a 2020 2020 7369 633a 2073  : str.    sic: s
-00008080: 7472 0a20 2020 2069 7273 5f6e 756d 6265  tr.    irs_numbe
-00008090: 723a 2073 7472 0a20 2020 2073 7461 7465  r: str.    state
-000080a0: 5f6f 665f 696e 636f 7270 6f72 6174 696f  _of_incorporatio
-000080b0: 6e3a 2073 7472 0a20 2020 2066 6973 6361  n: str.    fisca
-000080c0: 6c5f 7965 6172 5f65 6e64 3a20 7374 720a  l_year_end: str.
-000080d0: 0a20 2020 2064 6566 205f 5f72 6963 685f  .    def __rich_
-000080e0: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
-000080f0: 2074 6162 6c65 203d 2054 6162 6c65 2822   table = Table("
-00008100: 436f 6d70 616e 7922 2c20 2253 4943 222c  Company", "SIC",
-00008110: 2022 496e 636f 7270 2e22 2c20 2259 6561   "Incorp.", "Yea
-00008120: 7220 456e 6422 2c0a 2020 2020 2020 2020  r End",.        
-00008130: 2020 2020 2020 2020 2020 2020 2020 7469                ti
-00008140: 746c 653d 636f 6d70 616e 795f 7469 746c  tle=company_titl
-00008150: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00008160: 2020 2020 2020 2020 2062 6f78 3d62 6f78           box=box
-00008170: 2e53 494d 504c 4529 0a20 2020 2020 2020  .SIMPLE).       
-00008180: 2074 6162 6c65 2e61 6464 5f72 6f77 2866   table.add_row(f
-00008190: 227b 7365 6c66 2e6e 616d 657d 205b 7b73  "{self.name} [{s
-000081a0: 656c 662e 6369 6b7d 5d22 2c0a 2020 2020  elf.cik}]",.    
-000081b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081c0: 2020 7365 6c66 2e73 6963 2c0a 2020 2020    self.sic,.    
-000081d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081e0: 2020 7365 6c66 2e73 7461 7465 5f6f 665f    self.state_of_
-000081f0: 696e 636f 7270 6f72 6174 696f 6e2c 0a20  incorporation,. 
-00008200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008210: 2020 2020 2073 656c 662e 6669 7363 616c       self.fiscal
-00008220: 5f79 6561 725f 656e 6429 0a20 2020 2020  _year_end).     
-00008230: 2020 2072 6574 7572 6e20 7461 626c 650a     return table.
-00008240: 0a20 2020 2064 6566 205f 5f72 6570 725f  .    def __repr_
-00008250: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
-00008260: 2072 6574 7572 6e20 7265 7072 5f72 6963   return repr_ric
-00008270: 6828 7365 6c66 2e5f 5f72 6963 685f 5f28  h(self.__rich__(
-00008280: 2929 0a0a 0a40 6461 7461 636c 6173 7328  ))...@dataclass(
-00008290: 6672 6f7a 656e 3d54 7275 6529 0a63 6c61  frozen=True).cla
-000082a0: 7373 2046 696c 696e 6749 6e66 6f72 6d61  ss FilingInforma
-000082b0: 7469 6f6e 3a0a 2020 2020 666f 726d 3a20  tion:.    form: 
-000082c0: 7374 720a 2020 2020 6669 6c65 5f6e 756d  str.    file_num
-000082d0: 6265 723a 2073 7472 0a20 2020 2073 6563  ber: str.    sec
-000082e0: 5f61 6374 3a20 7374 720a 2020 2020 6669  _act: str.    fi
-000082f0: 6c6d 5f6e 756d 6265 723a 2073 7472 0a0a  lm_number: str..
-00008300: 2020 2020 6465 6620 5f5f 7269 6368 5f5f      def __rich__
-00008310: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00008320: 7461 626c 6520 3d20 5461 626c 6528 2246  table = Table("F
-00008330: 696c 6520 4e75 6d62 6572 222c 2022 5345  ile Number", "SE
-00008340: 4320 4163 7422 2c20 2246 696c 6d20 2322  C Act", "Film #"
-00008350: 2c20 2246 6f72 6d22 2c20 7469 746c 653d  , "Form", title=
-00008360: 6669 6c69 6e67 5f69 6e66 6f72 6d61 7469  filing_informati
-00008370: 6f6e 5f74 6974 6c65 2c20 626f 783d 626f  on_title, box=bo
-00008380: 782e 5349 4d50 4c45 290a 2020 2020 2020  x.SIMPLE).      
-00008390: 2020 7461 626c 652e 6164 645f 726f 7728    table.add_row(
-000083a0: 7365 6c66 2e66 696c 655f 6e75 6d62 6572  self.file_number
-000083b0: 2c20 7365 6c66 2e73 6563 5f61 6374 2c20  , self.sec_act, 
-000083c0: 7365 6c66 2e66 696c 6d5f 6e75 6d62 6572  self.film_number
-000083d0: 2c20 7365 6c66 2e66 6f72 6d29 0a20 2020  , self.form).   
-000083e0: 2020 2020 2072 6574 7572 6e20 7461 626c       return tabl
-000083f0: 650a 0a20 2020 2064 6566 205f 5f72 6570  e..    def __rep
-00008400: 725f 5f28 7365 6c66 293a 0a20 2020 2020  r__(self):.     
-00008410: 2020 2072 6574 7572 6e20 7265 7072 5f72     return repr_r
-00008420: 6963 6828 7365 6c66 2e5f 5f72 6963 685f  ich(self.__rich_
-00008430: 5f28 2929 0a0a 0a40 6461 7461 636c 6173  _())...@dataclas
-00008440: 7328 6672 6f7a 656e 3d54 7275 6529 0a63  s(frozen=True).c
-00008450: 6c61 7373 2046 6f72 6d65 7243 6f6d 7061  lass FormerCompa
-00008460: 6e79 3a0a 2020 2020 6e61 6d65 3a20 7374  ny:.    name: st
-00008470: 720a 2020 2020 6461 7465 5f6f 665f 6368  r.    date_of_ch
-00008480: 616e 6765 3a20 7374 720a 0a0a 4064 6174  ange: str...@dat
-00008490: 6163 6c61 7373 2866 726f 7a65 6e3d 5472  aclass(frozen=Tr
-000084a0: 7565 290a 636c 6173 7320 4669 6c65 723a  ue).class Filer:
-000084b0: 0a20 2020 2063 6f6d 7061 6e79 5f69 6e66  .    company_inf
-000084c0: 6f72 6d61 7469 6f6e 3a20 436f 6d70 616e  ormation: Compan
-000084d0: 7949 6e66 6f72 6d61 7469 6f6e 0a20 2020  yInformation.   
-000084e0: 2066 696c 696e 675f 696e 666f 726d 6174   filing_informat
-000084f0: 696f 6e3a 2046 696c 696e 6749 6e66 6f72  ion: FilingInfor
-00008500: 6d61 7469 6f6e 0a20 2020 2062 7573 696e  mation.    busin
-00008510: 6573 735f 6164 6472 6573 733a 2041 6464  ess_address: Add
-00008520: 7265 7373 0a20 2020 206d 6169 6c69 6e67  ress.    mailing
-00008530: 5f61 6464 7265 7373 3a20 4164 6472 6573  _address: Addres
-00008540: 730a 2020 2020 666f 726d 6572 5f63 6f6d  s.    former_com
-00008550: 7061 6e79 5f6e 616d 6573 3a20 4f70 7469  pany_names: Opti
-00008560: 6f6e 616c 5b4c 6973 745b 466f 726d 6572  onal[List[Former
-00008570: 436f 6d70 616e 795d 5d20 3d20 4e6f 6e65  Company]] = None
-00008580: 0a0a 2020 2020 6465 6620 5f5f 7269 6368  ..    def __rich
-00008590: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
-000085a0: 2020 6669 6c65 725f 7265 6e64 6572 6162    filer_renderab
-000085b0: 6c65 7320 3d20 5b73 656c 662e 636f 6d70  les = [self.comp
-000085c0: 616e 795f 696e 666f 726d 6174 696f 6e5d  any_information]
-000085d0: 0a20 2020 2020 2020 2023 2041 6464 7265  .        # Addre
-000085e0: 7373 6573 0a20 2020 2020 2020 2069 6620  sses.        if 
-000085f0: 7365 6c66 2e62 7573 696e 6573 735f 6164  self.business_ad
-00008600: 6472 6573 7320 6f72 2073 656c 662e 6d61  dress or self.ma
-00008610: 696c 696e 675f 6164 6472 6573 733a 0a20  iling_address:. 
-00008620: 2020 2020 2020 2020 2020 2066 696c 6572             filer
-00008630: 5f72 656e 6465 7261 626c 6573 2e61 7070  _renderables.app
-00008640: 656e 6428 5f63 7265 6174 655f 6164 6472  end(_create_addr
-00008650: 6573 735f 7461 626c 6528 7365 6c66 2e62  ess_table(self.b
-00008660: 7573 696e 6573 735f 6164 6472 6573 732c  usiness_address,
-00008670: 2073 656c 662e 6d61 696c 696e 675f 6164   self.mailing_ad
-00008680: 6472 6573 7329 290a 0a20 2020 2020 2020  dress))..       
-00008690: 2023 2046 6f72 6d65 7220 436f 6d70 616e   # Former Compan
-000086a0: 7920 4e61 6d65 730a 2020 2020 2020 2020  y Names.        
-000086b0: 6966 2073 656c 662e 666f 726d 6572 5f63  if self.former_c
-000086c0: 6f6d 7061 6e79 5f6e 616d 6573 3a0a 2020  ompany_names:.  
-000086d0: 2020 2020 2020 2020 2020 666f 726d 6572            former
-000086e0: 5f63 6f6d 7061 6e79 5f74 6162 6c65 203d  _company_table =
-000086f0: 2054 6162 6c65 2822 466f 726d 6572 204e   Table("Former N
-00008700: 616d 6522 2c20 2244 6174 6520 4368 616e  ame", "Date Chan
-00008710: 6765 6422 2c20 626f 783d 626f 782e 5349  ged", box=box.SI
-00008720: 4d50 4c45 290a 2020 2020 2020 2020 2020  MPLE).          
-00008730: 2020 666f 7220 636f 6d70 616e 7920 696e    for company in
-00008740: 2073 656c 662e 666f 726d 6572 5f63 6f6d   self.former_com
-00008750: 7061 6e79 5f6e 616d 6573 3a0a 2020 2020  pany_names:.    
-00008760: 2020 2020 2020 2020 2020 2020 666f 726d              form
-00008770: 6572 5f63 6f6d 7061 6e79 5f74 6162 6c65  er_company_table
-00008780: 2e61 6464 5f72 6f77 2863 6f6d 7061 6e79  .add_row(company
-00008790: 2e6e 616d 652c 2063 6f6d 7061 6e79 2e64  .name, company.d
-000087a0: 6174 655f 6f66 5f63 6861 6e67 6529 0a20  ate_of_change). 
-000087b0: 2020 2020 2020 2020 2020 2066 696c 6572             filer
-000087c0: 5f72 656e 6465 7261 626c 6573 2e61 7070  _renderables.app
-000087d0: 656e 6428 666f 726d 6572 5f63 6f6d 7061  end(former_compa
-000087e0: 6e79 5f74 6162 6c65 290a 0a20 2020 2020  ny_table)..     
-000087f0: 2020 2072 6574 7572 6e20 5061 6e65 6c28     return Panel(
-00008800: 0a20 2020 2020 2020 2020 2020 2047 726f  .            Gro
-00008810: 7570 282a 6669 6c65 725f 7265 6e64 6572  up(*filer_render
-00008820: 6162 6c65 7329 2c0a 2020 2020 2020 2020  ables),.        
-00008830: 2020 2020 7469 746c 653d 2246 494c 4552      title="FILER
-00008840: 220a 2020 2020 2020 2020 290a 0a20 2020  ".        )..   
-00008850: 2064 6566 205f 5f72 6570 725f 5f28 7365   def __repr__(se
-00008860: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
-00008870: 7572 6e20 7265 7072 5f72 6963 6828 7365  urn repr_rich(se
-00008880: 6c66 2e5f 5f72 6963 685f 5f28 2929 0a0a  lf.__rich__())..
-00008890: 0a40 6461 7461 636c 6173 7328 6672 6f7a  .@dataclass(froz
-000088a0: 656e 3d54 7275 6529 0a63 6c61 7373 204f  en=True).class O
-000088b0: 776e 6572 3a0a 2020 2020 6e61 6d65 3a20  wner:.    name: 
-000088c0: 7374 720a 2020 2020 6369 6b3a 2073 7472  str.    cik: str
-000088d0: 0a0a 0a40 6461 7461 636c 6173 7328 6672  ...@dataclass(fr
-000088e0: 6f7a 656e 3d54 7275 6529 0a63 6c61 7373  ozen=True).class
-000088f0: 2052 6570 6f72 7469 6e67 4f77 6e65 723a   ReportingOwner:
-00008900: 0a20 2020 206f 776e 6572 3a20 4f77 6e65  .    owner: Owne
-00008910: 720a 2020 2020 636f 6d70 616e 795f 696e  r.    company_in
-00008920: 666f 726d 6174 696f 6e3a 2043 6f6d 7061  formation: Compa
-00008930: 6e79 496e 666f 726d 6174 696f 6e0a 2020  nyInformation.  
-00008940: 2020 6669 6c69 6e67 5f69 6e66 6f72 6d61    filing_informa
-00008950: 7469 6f6e 3a20 4669 6c69 6e67 496e 666f  tion: FilingInfo
-00008960: 726d 6174 696f 6e0a 2020 2020 6275 7369  rmation.    busi
-00008970: 6e65 7373 5f61 6464 7265 7373 3a20 4164  ness_address: Ad
-00008980: 6472 6573 730a 2020 2020 6d61 696c 696e  dress.    mailin
-00008990: 675f 6164 6472 6573 733a 2041 6464 7265  g_address: Addre
-000089a0: 7373 0a0a 2020 2020 6465 6620 5f5f 7269  ss..    def __ri
-000089b0: 6368 5f5f 2873 656c 6629 3a0a 2020 2020  ch__(self):.    
-000089c0: 2020 2020 746f 705f 7265 6e64 6572 6162      top_renderab
-000089d0: 6c65 7320 3d20 5b5d 0a20 2020 2020 2020  les = [].       
-000089e0: 2072 6570 6f72 7469 6e67 5f6f 776e 6572   reporting_owner
-000089f0: 5f72 656e 6465 7261 626c 6573 203d 205b  _renderables = [
-00008a00: 5d0a 0a20 2020 2020 2020 2023 204f 776e  ]..        # Own
-00008a10: 6572 2054 6162 6c65 0a20 2020 2020 2020  er Table.       
-00008a20: 2069 6620 7365 6c66 2e6f 776e 6572 3a0a   if self.owner:.
-00008a30: 2020 2020 2020 2020 2020 2020 7265 706f              repo
-00008a40: 7274 696e 675f 6f77 6e65 725f 7461 626c  rting_owner_tabl
-00008a50: 6520 3d20 5461 626c 6528 224f 776e 6572  e = Table("Owner
-00008a60: 222c 2022 4349 4b22 2c20 626f 783d 626f  ", "CIK", box=bo
-00008a70: 782e 5349 4d50 4c45 290a 2020 2020 2020  x.SIMPLE).      
-00008a80: 2020 2020 2020 7265 706f 7274 696e 675f        reporting_
-00008a90: 6f77 6e65 725f 7461 626c 652e 6164 645f  owner_table.add_
-00008aa0: 726f 7728 7365 6c66 2e6f 776e 6572 2e6e  row(self.owner.n
-00008ab0: 616d 652c 2073 656c 662e 6f77 6e65 722e  ame, self.owner.
-00008ac0: 6369 6b29 0a0a 2020 2020 2020 2020 2020  cik)..          
-00008ad0: 2020 746f 705f 7265 6e64 6572 6162 6c65    top_renderable
-00008ae0: 7320 3d20 5b72 6570 6f72 7469 6e67 5f6f  s = [reporting_o
-00008af0: 776e 6572 5f74 6162 6c65 5d0a 2020 2020  wner_table].    
-00008b00: 2020 2020 2320 5265 706f 7274 696e 6720      # Reporting 
-00008b10: 4f77 6e65 7220 4669 6c69 6e67 2056 616c  Owner Filing Val
-00008b20: 7565 730a 2020 2020 2020 2020 6966 2073  ues.        if s
-00008b30: 656c 662e 6669 6c69 6e67 5f69 6e66 6f72  elf.filing_infor
-00008b40: 6d61 7469 6f6e 3a0a 2020 2020 2020 2020  mation:.        
-00008b50: 2020 2020 6669 6c69 6e67 5f76 616c 7565      filing_value
-00008b60: 735f 7461 626c 6520 3d20 5461 626c 6528  s_table = Table(
-00008b70: 2246 696c 6520 4e75 6d62 6572 222c 2022  "File Number", "
-00008b80: 5345 4320 4163 7422 2c20 2246 696c 6d20  SEC Act", "Film 
-00008b90: 2322 2c20 626f 783d 626f 782e 5349 4d50  #", box=box.SIMP
-00008ba0: 4c45 290a 2020 2020 2020 2020 2020 2020  LE).            
-00008bb0: 6669 6c69 6e67 5f76 616c 7565 735f 7461  filing_values_ta
-00008bc0: 626c 652e 6164 645f 726f 7728 7365 6c66  ble.add_row(self
-00008bd0: 2e66 696c 696e 675f 696e 666f 726d 6174  .filing_informat
-00008be0: 696f 6e2e 6669 6c65 5f6e 756d 6265 722c  ion.file_number,
-00008bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007810: 2020 2020 2020 2061 6363 6573 7369 6f6e         accession
+00007820: 5f6e 756d 6265 7229 0a20 2020 2020 2020  _number).       
+00007830: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00007840: 6669 6c69 6e67 3a0a 2020 2020 2020 2020  filing:.        
+00007850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007860: 7265 7475 726e 2066 696c 696e 670a 0a20  return filing.. 
+00007870: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
+00007880: 0a20 2020 2064 6566 205f 6765 745f 6375  .    def _get_cu
+00007890: 7272 656e 745f 6669 6c69 6e67 5f62 795f  rrent_filing_by_
+000078a0: 6163 6365 7373 696f 6e5f 6e75 6d62 6572  accession_number
+000078b0: 2864 6174 613a 2070 612e 5461 626c 652c  (data: pa.Table,
+000078c0: 2061 6363 6573 7369 6f6e 5f6e 756d 6265   accession_numbe
+000078d0: 723a 2073 7472 293a 0a20 2020 2020 2020  r: str):.       
+000078e0: 206d 6173 6b20 3d20 7063 2e65 7175 616c   mask = pc.equal
+000078f0: 2864 6174 615b 2761 6363 6573 7369 6f6e  (data['accession
+00007900: 5f6e 756d 6265 7227 5d2c 2061 6363 6573  _number'], acces
+00007910: 7369 6f6e 5f6e 756d 6265 7229 0a20 2020  sion_number).   
+00007920: 2020 2020 2069 6478 203d 206d 6173 6b2e       idx = mask.
+00007930: 696e 6465 7828 5472 7565 292e 6173 5f70  index(True).as_p
+00007940: 7928 290a 2020 2020 2020 2020 6966 2069  y().        if i
+00007950: 6478 203e 202d 313a 0a20 2020 2020 2020  dx > -1:.       
+00007960: 2020 2020 2072 6574 7572 6e20 4669 6c69       return Fili
+00007970: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
+00007980: 2020 2020 6369 6b3d 6461 7461 5b27 6369      cik=data['ci
+00007990: 6b27 5d5b 6964 785d 2e61 735f 7079 2829  k'][idx].as_py()
+000079a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000079b0: 2020 636f 6d70 616e 793d 6461 7461 5b27    company=data['
+000079c0: 636f 6d70 616e 7927 5d5b 6964 785d 2e61  company'][idx].a
+000079d0: 735f 7079 2829 2c0a 2020 2020 2020 2020  s_py(),.        
+000079e0: 2020 2020 2020 2020 666f 726d 3d64 6174          form=dat
+000079f0: 615b 2766 6f72 6d27 5d5b 6964 785d 2e61  a['form'][idx].a
+00007a00: 735f 7079 2829 2c0a 2020 2020 2020 2020  s_py(),.        
+00007a10: 2020 2020 2020 2020 6669 6c69 6e67 5f64          filing_d
+00007a20: 6174 653d 6461 7461 5b27 6669 6c69 6e67  ate=data['filing
+00007a30: 5f64 6174 6527 5d5b 6964 785d 2e61 735f  _date'][idx].as_
+00007a40: 7079 2829 2c0a 2020 2020 2020 2020 2020  py(),.          
+00007a50: 2020 2020 2020 6163 6365 7373 696f 6e5f        accession_
+00007a60: 6e6f 3d64 6174 615b 2761 6363 6573 7369  no=data['accessi
+00007a70: 6f6e 5f6e 756d 6265 7227 5d5b 6964 785d  on_number'][idx]
+00007a80: 2e61 735f 7079 2829 2c0a 2020 2020 2020  .as_py(),.      
+00007a90: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00007aa0: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
+00007ab0: 2064 6566 205f 5f72 6963 685f 5f28 7365   def __rich__(se
+00007ac0: 6c66 293a 0a20 2020 2020 2020 2070 6167  lf):.        pag
+00007ad0: 653a 2070 642e 4461 7461 4672 616d 6520  e: pd.DataFrame 
+00007ae0: 3d20 7365 6c66 2e74 6f5f 7061 6e64 6173  = self.to_pandas
+00007af0: 2829 0a0a 2020 2020 2020 2020 2320 636f  ()..        # co
+00007b00: 6d70 7574 6520 7468 6520 696e 6465 7820  mpute the index 
+00007b10: 6672 6f6d 2074 6865 2073 7461 7274 2061  from the start a
+00007b20: 6e64 2070 6167 655f 7369 7a65 2061 6e64  nd page_size and
+00007b30: 2073 6574 2069 7420 6173 2074 6865 2069   set it as the i
+00007b40: 6e64 6578 206f 6620 7468 6520 7061 6765  ndex of the page
+00007b50: 0a20 2020 2020 2020 2070 6167 652e 696e  .        page.in
+00007b60: 6465 7820 3d20 7261 6e67 6528 7365 6c66  dex = range(self
+00007b70: 2e5f 7374 6172 7420 2d20 312c 2073 656c  ._start - 1, sel
+00007b80: 662e 5f73 7461 7274 202d 2031 202b 206c  f._start - 1 + l
+00007b90: 656e 2870 6167 6529 290a 0a20 2020 2020  en(page))..     
+00007ba0: 2020 2072 6574 7572 6e20 5061 6e65 6c28     return Panel(
+00007bb0: 0a20 2020 2020 2020 2020 2020 2047 726f  .            Gro
+00007bc0: 7570 280a 2020 2020 2020 2020 2020 2020  up(.            
+00007bd0: 2020 2020 6466 5f74 6f5f 7269 6368 5f74      df_to_rich_t
+00007be0: 6162 6c65 2870 6167 6529 2c0a 2020 2020  able(page),.    
+00007bf0: 2020 2020 2020 2020 2020 2020 5465 7874              Text
+00007c00: 2866 2246 696c 696e 6773 207b 7061 6765  (f"Filings {page
+00007c10: 2e69 6e64 6578 2e6d 696e 2829 7d20 746f  .index.min()} to
+00007c20: 207b 7061 6765 2e69 6e64 6578 2e6d 6178   {page.index.max
+00007c30: 2829 7d22 290a 2020 2020 2020 2020 2020  ()}").          
+00007c40: 2020 292c 2074 6974 6c65 3d66 2243 7572    ), title=f"Cur
+00007c50: 7265 6e74 2046 696c 696e 6773 206f 6e20  rent Filings on 
+00007c60: 7b73 656c 662e 7374 6172 745f 6461 7465  {self.start_date
+00007c70: 7d22 0a20 2020 2020 2020 2029 0a0a 0a40  }".        )...@
+00007c80: 6c72 755f 6361 6368 6528 6d61 7873 697a  lru_cache(maxsiz
+00007c90: 653d 3829 0a64 6566 205f 6765 745f 6361  e=8).def _get_ca
+00007ca0: 6368 6564 5f66 696c 696e 6773 2879 6561  ched_filings(yea
+00007cb0: 723a 2059 6561 7273 203d 204e 6f6e 652c  r: Years = None,
+00007cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007cd0: 2020 2020 2020 2020 2071 7561 7274 6572           quarter
+00007ce0: 3a20 5175 6172 7465 7273 203d 204e 6f6e  : Quarters = Non
+00007cf0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00007d00: 2020 2020 2020 2020 2020 2066 6f72 6d3a             form:
+00007d10: 2055 6e69 6f6e 5b73 7472 2c20 4c69 7374   Union[str, List
+00007d20: 5b49 6e74 5374 7269 6e67 5d5d 203d 204e  [IntString]] = N
+00007d30: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+00007d40: 2020 2020 2020 2020 2020 2020 2061 6d65               ame
+00007d50: 6e64 6d65 6e74 733a 2062 6f6f 6c20 3d20  ndments: bool = 
+00007d60: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+00007d70: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00007d80: 6c69 6e67 5f64 6174 653a 2073 7472 203d  ling_date: str =
+00007d90: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+00007da0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00007db0: 6e64 6578 3d22 666f 726d 2229 202d 3e20  ndex="form") -> 
+00007dc0: 4669 6c69 6e67 733a 0a20 2020 2023 2047  Filings:.    # G
+00007dd0: 6574 2074 6865 2066 696c 696e 6773 2062  et the filings b
+00007de0: 7574 2063 6163 6865 2074 6865 2072 6573  ut cache the res
+00007df0: 756c 740a 2020 2020 7265 7475 726e 2067  ult.    return g
+00007e00: 6574 5f66 696c 696e 6773 2879 6561 723d  et_filings(year=
+00007e10: 7965 6172 2c20 7175 6172 7465 723d 7175  year, quarter=qu
+00007e20: 6172 7465 722c 2066 6f72 6d3d 666f 726d  arter, form=form
+00007e30: 2c20 616d 656e 646d 656e 7473 3d61 6d65  , amendments=ame
+00007e40: 6e64 6d65 6e74 732c 2066 696c 696e 675f  ndments, filing_
+00007e50: 6461 7465 3d66 696c 696e 675f 6461 7465  date=filing_date
+00007e60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007e70: 2020 2020 2020 2020 2069 6e64 6578 3d69           index=i
+00007e80: 6e64 6578 290a 0a0a 6465 6620 7061 7273  ndex)...def pars
+00007e90: 655f 6669 6c69 6e67 5f68 6561 6465 7228  e_filing_header(
+00007ea0: 636f 6e74 656e 7429 3a0a 2020 2020 6461  content):.    da
+00007eb0: 7461 203d 207b 7d0a 2020 2020 6375 7272  ta = {}.    curr
+00007ec0: 656e 745f 6b65 7920 3d20 4e6f 6e65 0a0a  ent_key = None..
+00007ed0: 2020 2020 6c69 6e65 7320 3d20 636f 6e74      lines = cont
+00007ee0: 656e 742e 7370 6c69 7428 275c 6e27 290a  ent.split('\n').
+00007ef0: 2020 2020 666f 7220 6c69 6e65 2069 6e20      for line in 
+00007f00: 6c69 6e65 733a 0a20 2020 2020 2020 2069  lines:.        i
+00007f10: 6620 6c69 6e65 2e65 6e64 7377 6974 6828  f line.endswith(
+00007f20: 273a 2729 3a0a 2020 2020 2020 2020 2020  ':'):.          
+00007f30: 2020 6375 7272 656e 745f 6b65 7920 3d20    current_key = 
+00007f40: 6c69 6e65 5b3a 2d31 5d20 2023 2052 656d  line[:-1]  # Rem
+00007f50: 6f76 6520 7468 6520 7472 6169 6c69 6e67  ove the trailing
+00007f60: 2063 6f6c 6f6e 0a20 2020 2020 2020 2020   colon.         
+00007f70: 2020 2064 6174 615b 6375 7272 656e 745f     data[current_
+00007f80: 6b65 795d 203d 207b 7d0a 2020 2020 2020  key] = {}.      
+00007f90: 2020 656c 6966 2063 7572 7265 6e74 5f6b    elif current_k
+00007fa0: 6579 2061 6e64 2027 3a27 2069 6e20 6c69  ey and ':' in li
+00007fb0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00007fc0: 6b65 792c 2076 616c 7565 203d 206d 6170  key, value = map
+00007fd0: 2873 7472 2e73 7472 6970 2c20 6c69 6e65  (str.strip, line
+00007fe0: 2e73 706c 6974 2827 3a27 2c20 3129 290a  .split(':', 1)).
+00007ff0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00008000: 5b63 7572 7265 6e74 5f6b 6579 5d5b 6b65  [current_key][ke
+00008010: 795d 203d 2076 616c 7565 0a0a 2020 2020  y] = value..    
+00008020: 7265 7475 726e 2064 6174 610a 0a0a 4064  return data...@d
+00008030: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
+00008040: 5472 7565 290a 636c 6173 7320 436f 6d70  True).class Comp
+00008050: 616e 7949 6e66 6f72 6d61 7469 6f6e 3a0a  anyInformation:.
+00008060: 2020 2020 6e61 6d65 3a20 7374 720a 2020      name: str.  
+00008070: 2020 6369 6b3a 2073 7472 0a20 2020 2073    cik: str.    s
+00008080: 6963 3a20 7374 720a 2020 2020 6972 735f  ic: str.    irs_
+00008090: 6e75 6d62 6572 3a20 7374 720a 2020 2020  number: str.    
+000080a0: 7374 6174 655f 6f66 5f69 6e63 6f72 706f  state_of_incorpo
+000080b0: 7261 7469 6f6e 3a20 7374 720a 2020 2020  ration: str.    
+000080c0: 6669 7363 616c 5f79 6561 725f 656e 643a  fiscal_year_end:
+000080d0: 2073 7472 0a0a 2020 2020 6465 6620 5f5f   str..    def __
+000080e0: 7269 6368 5f5f 2873 656c 6629 3a0a 2020  rich__(self):.  
+000080f0: 2020 2020 2020 7461 626c 6520 3d20 5461        table = Ta
+00008100: 626c 6528 2243 6f6d 7061 6e79 222c 2022  ble("Company", "
+00008110: 5349 4322 2c20 2249 6e63 6f72 702e 222c  SIC", "Incorp.",
+00008120: 2022 5965 6172 2045 6e64 222c 0a20 2020   "Year End",.   
+00008130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008140: 2020 2074 6974 6c65 3d63 6f6d 7061 6e79     title=company
+00008150: 5f74 6974 6c65 2c0a 2020 2020 2020 2020  _title,.        
+00008160: 2020 2020 2020 2020 2020 2020 2020 626f                bo
+00008170: 783d 626f 782e 5349 4d50 4c45 290a 2020  x=box.SIMPLE).  
+00008180: 2020 2020 2020 7461 626c 652e 6164 645f        table.add_
+00008190: 726f 7728 6622 7b73 656c 662e 6e61 6d65  row(f"{self.name
+000081a0: 7d20 5b7b 7365 6c66 2e63 696b 7d5d 222c  } [{self.cik}]",
+000081b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000081c0: 2020 2020 2020 2073 656c 662e 7369 632c         self.sic,
+000081d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000081e0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+000081f0: 655f 6f66 5f69 6e63 6f72 706f 7261 7469  e_of_incorporati
+00008200: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+00008210: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
+00008220: 6973 6361 6c5f 7965 6172 5f65 6e64 290a  iscal_year_end).
+00008230: 2020 2020 2020 2020 7265 7475 726e 2074          return t
+00008240: 6162 6c65 0a0a 2020 2020 6465 6620 5f5f  able..    def __
+00008250: 7265 7072 5f5f 2873 656c 6629 3a0a 2020  repr__(self):.  
+00008260: 2020 2020 2020 7265 7475 726e 2072 6570        return rep
+00008270: 725f 7269 6368 2873 656c 662e 5f5f 7269  r_rich(self.__ri
+00008280: 6368 5f5f 2829 290a 0a0a 4064 6174 6163  ch__())...@datac
+00008290: 6c61 7373 2866 726f 7a65 6e3d 5472 7565  lass(frozen=True
+000082a0: 290a 636c 6173 7320 4669 6c69 6e67 496e  ).class FilingIn
+000082b0: 666f 726d 6174 696f 6e3a 0a20 2020 2066  formation:.    f
+000082c0: 6f72 6d3a 2073 7472 0a20 2020 2066 696c  orm: str.    fil
+000082d0: 655f 6e75 6d62 6572 3a20 7374 720a 2020  e_number: str.  
+000082e0: 2020 7365 635f 6163 743a 2073 7472 0a20    sec_act: str. 
+000082f0: 2020 2066 696c 6d5f 6e75 6d62 6572 3a20     film_number: 
+00008300: 7374 720a 0a20 2020 2064 6566 205f 5f72  str..    def __r
+00008310: 6963 685f 5f28 7365 6c66 293a 0a20 2020  ich__(self):.   
+00008320: 2020 2020 2074 6162 6c65 203d 2054 6162       table = Tab
+00008330: 6c65 2822 4669 6c65 204e 756d 6265 7222  le("File Number"
+00008340: 2c20 2253 4543 2041 6374 222c 2022 4669  , "SEC Act", "Fi
+00008350: 6c6d 2023 222c 2022 466f 726d 222c 2074  lm #", "Form", t
+00008360: 6974 6c65 3d66 696c 696e 675f 696e 666f  itle=filing_info
+00008370: 726d 6174 696f 6e5f 7469 746c 652c 2062  rmation_title, b
+00008380: 6f78 3d62 6f78 2e53 494d 504c 4529 0a20  ox=box.SIMPLE). 
+00008390: 2020 2020 2020 2074 6162 6c65 2e61 6464         table.add
+000083a0: 5f72 6f77 2873 656c 662e 6669 6c65 5f6e  _row(self.file_n
+000083b0: 756d 6265 722c 2073 656c 662e 7365 635f  umber, self.sec_
+000083c0: 6163 742c 2073 656c 662e 6669 6c6d 5f6e  act, self.film_n
+000083d0: 756d 6265 722c 2073 656c 662e 666f 726d  umber, self.form
+000083e0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+000083f0: 2074 6162 6c65 0a0a 2020 2020 6465 6620   table..    def 
+00008400: 5f5f 7265 7072 5f5f 2873 656c 6629 3a0a  __repr__(self):.
+00008410: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00008420: 6570 725f 7269 6368 2873 656c 662e 5f5f  epr_rich(self.__
+00008430: 7269 6368 5f5f 2829 290a 0a0a 4064 6174  rich__())...@dat
+00008440: 6163 6c61 7373 2866 726f 7a65 6e3d 5472  aclass(frozen=Tr
+00008450: 7565 290a 636c 6173 7320 466f 726d 6572  ue).class Former
+00008460: 436f 6d70 616e 793a 0a20 2020 206e 616d  Company:.    nam
+00008470: 653a 2073 7472 0a20 2020 2064 6174 655f  e: str.    date_
+00008480: 6f66 5f63 6861 6e67 653a 2073 7472 0a0a  of_change: str..
+00008490: 0a40 6461 7461 636c 6173 7328 6672 6f7a  .@dataclass(froz
+000084a0: 656e 3d54 7275 6529 0a63 6c61 7373 2046  en=True).class F
+000084b0: 696c 6572 3a0a 2020 2020 636f 6d70 616e  iler:.    compan
+000084c0: 795f 696e 666f 726d 6174 696f 6e3a 2043  y_information: C
+000084d0: 6f6d 7061 6e79 496e 666f 726d 6174 696f  ompanyInformatio
+000084e0: 6e0a 2020 2020 6669 6c69 6e67 5f69 6e66  n.    filing_inf
+000084f0: 6f72 6d61 7469 6f6e 3a20 4669 6c69 6e67  ormation: Filing
+00008500: 496e 666f 726d 6174 696f 6e0a 2020 2020  Information.    
+00008510: 6275 7369 6e65 7373 5f61 6464 7265 7373  business_address
+00008520: 3a20 4164 6472 6573 730a 2020 2020 6d61  : Address.    ma
+00008530: 696c 696e 675f 6164 6472 6573 733a 2041  iling_address: A
+00008540: 6464 7265 7373 0a20 2020 2066 6f72 6d65  ddress.    forme
+00008550: 725f 636f 6d70 616e 795f 6e61 6d65 733a  r_company_names:
+00008560: 204f 7074 696f 6e61 6c5b 4c69 7374 5b46   Optional[List[F
+00008570: 6f72 6d65 7243 6f6d 7061 6e79 5d5d 203d  ormerCompany]] =
+00008580: 204e 6f6e 650a 0a20 2020 2064 6566 205f   None..    def _
+00008590: 5f72 6963 685f 5f28 7365 6c66 293a 0a20  _rich__(self):. 
+000085a0: 2020 2020 2020 2066 696c 6572 5f72 656e         filer_ren
+000085b0: 6465 7261 626c 6573 203d 205b 7365 6c66  derables = [self
+000085c0: 2e63 6f6d 7061 6e79 5f69 6e66 6f72 6d61  .company_informa
+000085d0: 7469 6f6e 5d0a 2020 2020 2020 2020 2320  tion].        # 
+000085e0: 4164 6472 6573 7365 730a 2020 2020 2020  Addresses.      
+000085f0: 2020 6966 2073 656c 662e 6275 7369 6e65    if self.busine
+00008600: 7373 5f61 6464 7265 7373 206f 7220 7365  ss_address or se
+00008610: 6c66 2e6d 6169 6c69 6e67 5f61 6464 7265  lf.mailing_addre
+00008620: 7373 3a0a 2020 2020 2020 2020 2020 2020  ss:.            
+00008630: 6669 6c65 725f 7265 6e64 6572 6162 6c65  filer_renderable
+00008640: 732e 6170 7065 6e64 285f 6372 6561 7465  s.append(_create
+00008650: 5f61 6464 7265 7373 5f74 6162 6c65 2873  _address_table(s
+00008660: 656c 662e 6275 7369 6e65 7373 5f61 6464  elf.business_add
+00008670: 7265 7373 2c20 7365 6c66 2e6d 6169 6c69  ress, self.maili
+00008680: 6e67 5f61 6464 7265 7373 2929 0a0a 2020  ng_address))..  
+00008690: 2020 2020 2020 2320 466f 726d 6572 2043        # Former C
+000086a0: 6f6d 7061 6e79 204e 616d 6573 0a20 2020  ompany Names.   
+000086b0: 2020 2020 2069 6620 7365 6c66 2e66 6f72       if self.for
+000086c0: 6d65 725f 636f 6d70 616e 795f 6e61 6d65  mer_company_name
+000086d0: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
+000086e0: 6f72 6d65 725f 636f 6d70 616e 795f 7461  ormer_company_ta
+000086f0: 626c 6520 3d20 5461 626c 6528 2246 6f72  ble = Table("For
+00008700: 6d65 7220 4e61 6d65 222c 2022 4461 7465  mer Name", "Date
+00008710: 2043 6861 6e67 6564 222c 2062 6f78 3d62   Changed", box=b
+00008720: 6f78 2e53 494d 504c 4529 0a20 2020 2020  ox.SIMPLE).     
+00008730: 2020 2020 2020 2066 6f72 2063 6f6d 7061         for compa
+00008740: 6e79 2069 6e20 7365 6c66 2e66 6f72 6d65  ny in self.forme
+00008750: 725f 636f 6d70 616e 795f 6e61 6d65 733a  r_company_names:
+00008760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008770: 2066 6f72 6d65 725f 636f 6d70 616e 795f   former_company_
+00008780: 7461 626c 652e 6164 645f 726f 7728 636f  table.add_row(co
+00008790: 6d70 616e 792e 6e61 6d65 2c20 636f 6d70  mpany.name, comp
+000087a0: 616e 792e 6461 7465 5f6f 665f 6368 616e  any.date_of_chan
+000087b0: 6765 290a 2020 2020 2020 2020 2020 2020  ge).            
+000087c0: 6669 6c65 725f 7265 6e64 6572 6162 6c65  filer_renderable
+000087d0: 732e 6170 7065 6e64 2866 6f72 6d65 725f  s.append(former_
+000087e0: 636f 6d70 616e 795f 7461 626c 6529 0a0a  company_table)..
+000087f0: 2020 2020 2020 2020 7265 7475 726e 2050          return P
+00008800: 616e 656c 280a 2020 2020 2020 2020 2020  anel(.          
+00008810: 2020 4772 6f75 7028 2a66 696c 6572 5f72    Group(*filer_r
+00008820: 656e 6465 7261 626c 6573 292c 0a20 2020  enderables),.   
+00008830: 2020 2020 2020 2020 2074 6974 6c65 3d22           title="
+00008840: 4649 4c45 5222 0a20 2020 2020 2020 2029  FILER".        )
+00008850: 0a0a 2020 2020 6465 6620 5f5f 7265 7072  ..    def __repr
+00008860: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
+00008870: 2020 7265 7475 726e 2072 6570 725f 7269    return repr_ri
+00008880: 6368 2873 656c 662e 5f5f 7269 6368 5f5f  ch(self.__rich__
+00008890: 2829 290a 0a0a 4064 6174 6163 6c61 7373  ())...@dataclass
+000088a0: 2866 726f 7a65 6e3d 5472 7565 290a 636c  (frozen=True).cl
+000088b0: 6173 7320 4f77 6e65 723a 0a20 2020 206e  ass Owner:.    n
+000088c0: 616d 653a 2073 7472 0a20 2020 2063 696b  ame: str.    cik
+000088d0: 3a20 7374 720a 0a0a 4064 6174 6163 6c61  : str...@datacla
+000088e0: 7373 2866 726f 7a65 6e3d 5472 7565 290a  ss(frozen=True).
+000088f0: 636c 6173 7320 5265 706f 7274 696e 674f  class ReportingO
+00008900: 776e 6572 3a0a 2020 2020 6f77 6e65 723a  wner:.    owner:
+00008910: 204f 776e 6572 0a20 2020 2063 6f6d 7061   Owner.    compa
+00008920: 6e79 5f69 6e66 6f72 6d61 7469 6f6e 3a20  ny_information: 
+00008930: 436f 6d70 616e 7949 6e66 6f72 6d61 7469  CompanyInformati
+00008940: 6f6e 0a20 2020 2066 696c 696e 675f 696e  on.    filing_in
+00008950: 666f 726d 6174 696f 6e3a 2046 696c 696e  formation: Filin
+00008960: 6749 6e66 6f72 6d61 7469 6f6e 0a20 2020  gInformation.   
+00008970: 2062 7573 696e 6573 735f 6164 6472 6573   business_addres
+00008980: 733a 2041 6464 7265 7373 0a20 2020 206d  s: Address.    m
+00008990: 6169 6c69 6e67 5f61 6464 7265 7373 3a20  ailing_address: 
+000089a0: 4164 6472 6573 730a 0a20 2020 2064 6566  Address..    def
+000089b0: 205f 5f72 6963 685f 5f28 7365 6c66 293a   __rich__(self):
+000089c0: 0a20 2020 2020 2020 2074 6f70 5f72 656e  .        top_ren
+000089d0: 6465 7261 626c 6573 203d 205b 5d0a 2020  derables = [].  
+000089e0: 2020 2020 2020 7265 706f 7274 696e 675f        reporting_
+000089f0: 6f77 6e65 725f 7265 6e64 6572 6162 6c65  owner_renderable
+00008a00: 7320 3d20 5b5d 0a0a 2020 2020 2020 2020  s = []..        
+00008a10: 2320 4f77 6e65 7220 5461 626c 650a 2020  # Owner Table.  
+00008a20: 2020 2020 2020 6966 2073 656c 662e 6f77        if self.ow
+00008a30: 6e65 723a 0a20 2020 2020 2020 2020 2020  ner:.           
+00008a40: 2072 6570 6f72 7469 6e67 5f6f 776e 6572   reporting_owner
+00008a50: 5f74 6162 6c65 203d 2054 6162 6c65 2822  _table = Table("
+00008a60: 4f77 6e65 7222 2c20 2243 494b 222c 2062  Owner", "CIK", b
+00008a70: 6f78 3d62 6f78 2e53 494d 504c 4529 0a20  ox=box.SIMPLE). 
+00008a80: 2020 2020 2020 2020 2020 2072 6570 6f72             repor
+00008a90: 7469 6e67 5f6f 776e 6572 5f74 6162 6c65  ting_owner_table
+00008aa0: 2e61 6464 5f72 6f77 2873 656c 662e 6f77  .add_row(self.ow
+00008ab0: 6e65 722e 6e61 6d65 2c20 7365 6c66 2e6f  ner.name, self.o
+00008ac0: 776e 6572 2e63 696b 290a 0a20 2020 2020  wner.cik)..     
+00008ad0: 2020 2020 2020 2074 6f70 5f72 656e 6465         top_rende
+00008ae0: 7261 626c 6573 203d 205b 7265 706f 7274  rables = [report
+00008af0: 696e 675f 6f77 6e65 725f 7461 626c 655d  ing_owner_table]
+00008b00: 0a20 2020 2020 2020 2023 2052 6570 6f72  .        # Repor
+00008b10: 7469 6e67 204f 776e 6572 2046 696c 696e  ting Owner Filin
+00008b20: 6720 5661 6c75 6573 0a20 2020 2020 2020  g Values.       
+00008b30: 2069 6620 7365 6c66 2e66 696c 696e 675f   if self.filing_
+00008b40: 696e 666f 726d 6174 696f 6e3a 0a20 2020  information:.   
+00008b50: 2020 2020 2020 2020 2066 696c 696e 675f           filing_
+00008b60: 7661 6c75 6573 5f74 6162 6c65 203d 2054  values_table = T
+00008b70: 6162 6c65 2822 4669 6c65 204e 756d 6265  able("File Numbe
+00008b80: 7222 2c20 2253 4543 2041 6374 222c 2022  r", "SEC Act", "
+00008b90: 4669 6c6d 2023 222c 2062 6f78 3d62 6f78  Film #", box=box
+00008ba0: 2e53 494d 504c 4529 0a20 2020 2020 2020  .SIMPLE).       
+00008bb0: 2020 2020 2066 696c 696e 675f 7661 6c75       filing_valu
+00008bc0: 6573 5f74 6162 6c65 2e61 6464 5f72 6f77  es_table.add_row
+00008bd0: 2873 656c 662e 6669 6c69 6e67 5f69 6e66  (self.filing_inf
+00008be0: 6f72 6d61 7469 6f6e 2e66 696c 655f 6e75  ormation.file_nu
+00008bf0: 6d62 6572 2c0a 2020 2020 2020 2020 2020  mber,.          
 00008c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c10: 2020 2020 2020 2020 2073 656c 662e 6669           self.fi
-00008c20: 6c69 6e67 5f69 6e66 6f72 6d61 7469 6f6e  ling_information
-00008c30: 2e73 6563 5f61 6374 2c0a 2020 2020 2020  .sec_act,.      
+00008c10: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00008c20: 6c66 2e66 696c 696e 675f 696e 666f 726d  lf.filing_inform
+00008c30: 6174 696f 6e2e 7365 635f 6163 742c 0a20  ation.sec_act,. 
 00008c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c60: 2020 7365 6c66 2e66 696c 696e 675f 696e    self.filing_in
-00008c70: 666f 726d 6174 696f 6e2e 6669 6c6d 5f6e  formation.film_n
-00008c80: 756d 6265 7229 0a20 2020 2020 2020 2020  umber).         
-00008c90: 2020 2074 6f70 5f72 656e 6465 7261 626c     top_renderabl
-00008ca0: 6573 2e61 7070 656e 6428 6669 6c69 6e67  es.append(filing
-00008cb0: 5f76 616c 7565 735f 7461 626c 6529 0a0a  _values_table)..
-00008cc0: 2020 2020 2020 2020 7265 706f 7274 696e          reportin
-00008cd0: 675f 6f77 6e65 725f 7265 6e64 6572 6162  g_owner_renderab
-00008ce0: 6c65 7320 3d20 5b43 6f6c 756d 6e73 2874  les = [Columns(t
-00008cf0: 6f70 5f72 656e 6465 7261 626c 6573 295d  op_renderables)]
-00008d00: 0a0a 2020 2020 2020 2020 2320 4164 6472  ..        # Addr
-00008d10: 6573 7365 730a 2020 2020 2020 2020 6966  esses.        if
-00008d20: 2073 656c 662e 6275 7369 6e65 7373 5f61   self.business_a
-00008d30: 6464 7265 7373 206f 7220 7365 6c66 2e6d  ddress or self.m
-00008d40: 6169 6c69 6e67 5f61 6464 7265 7373 3a0a  ailing_address:.
-00008d50: 2020 2020 2020 2020 2020 2020 7265 706f              repo
-00008d60: 7274 696e 675f 6f77 6e65 725f 7265 6e64  rting_owner_rend
-00008d70: 6572 6162 6c65 732e 6170 7065 6e64 285f  erables.append(_
-00008d80: 6372 6561 7465 5f61 6464 7265 7373 5f74  create_address_t
-00008d90: 6162 6c65 2873 656c 662e 6275 7369 6e65  able(self.busine
-00008da0: 7373 5f61 6464 7265 7373 2c20 7365 6c66  ss_address, self
-00008db0: 2e6d 6169 6c69 6e67 5f61 6464 7265 7373  .mailing_address
-00008dc0: 2929 0a0a 2020 2020 2020 2020 7265 7475  ))..        retu
-00008dd0: 726e 2050 616e 656c 280a 2020 2020 2020  rn Panel(.      
-00008de0: 2020 2020 2020 4772 6f75 7028 0a20 2020        Group(.   
-00008df0: 2020 2020 2020 2020 2020 2020 202a 7265               *re
-00008e00: 706f 7274 696e 675f 6f77 6e65 725f 7265  porting_owner_re
-00008e10: 6e64 6572 6162 6c65 730a 2020 2020 2020  nderables.      
-00008e20: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
-00008e30: 2020 2020 2074 6974 6c65 3d72 6570 6f72       title=repor
-00008e40: 7469 6e67 5f6f 776e 6572 5f74 6974 6c65  ting_owner_title
-00008e50: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00008e60: 6465 6620 5f5f 7265 7072 5f5f 2873 656c  def __repr__(sel
-00008e70: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-00008e80: 726e 2072 6570 725f 7269 6368 2873 656c  rn repr_rich(sel
-00008e90: 662e 5f5f 7269 6368 5f5f 2829 290a 0a0a  f.__rich__())...
-00008ea0: 4064 6174 6163 6c61 7373 2866 726f 7a65  @dataclass(froze
-00008eb0: 6e3d 5472 7565 290a 636c 6173 7320 5375  n=True).class Su
-00008ec0: 626a 6563 7443 6f6d 7061 6e79 3a0a 2020  bjectCompany:.  
-00008ed0: 2020 636f 6d70 616e 795f 696e 666f 726d    company_inform
-00008ee0: 6174 696f 6e3a 2043 6f6d 7061 6e79 496e  ation: CompanyIn
-00008ef0: 666f 726d 6174 696f 6e0a 2020 2020 6669  formation.    fi
-00008f00: 6c69 6e67 5f69 6e66 6f72 6d61 7469 6f6e  ling_information
-00008f10: 3a20 4669 6c69 6e67 496e 666f 726d 6174  : FilingInformat
-00008f20: 696f 6e0a 2020 2020 6275 7369 6e65 7373  ion.    business
-00008f30: 5f61 6464 7265 7373 3a20 4164 6472 6573  _address: Addres
-00008f40: 730a 2020 2020 6d61 696c 696e 675f 6164  s.    mailing_ad
-00008f50: 6472 6573 733a 2041 6464 7265 7373 0a20  dress: Address. 
-00008f60: 2020 2066 6f72 6d65 725f 636f 6d70 616e     former_compan
-00008f70: 795f 6e61 6d65 733a 204f 7074 696f 6e61  y_names: Optiona
-00008f80: 6c5b 4c69 7374 5b46 6f72 6d65 7243 6f6d  l[List[FormerCom
-00008f90: 7061 6e79 5d5d 203d 204e 6f6e 650a 0a20  pany]] = None.. 
-00008fa0: 2020 2064 6566 205f 5f72 6963 685f 5f28     def __rich__(
-00008fb0: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-00008fc0: 7562 6a65 6374 5f63 6f6d 7061 6e79 5f72  ubject_company_r
-00008fd0: 656e 6465 7261 626c 6573 203d 205b 5d0a  enderables = [].
-00008fe0: 0a20 2020 2020 2020 2023 2046 696c 696e  .        # Filin
-00008ff0: 6720 496e 666f 726d 6174 696f 6e0a 2020  g Information.  
-00009000: 2020 2020 2020 6966 2073 656c 662e 6669        if self.fi
-00009010: 6c69 6e67 5f69 6e66 6f72 6d61 7469 6f6e  ling_information
-00009020: 3a0a 2020 2020 2020 2020 2020 2020 7375  :.            su
-00009030: 626a 6563 745f 636f 6d70 616e 795f 7265  bject_company_re
-00009040: 6e64 6572 6162 6c65 732e 6170 7065 6e64  nderables.append
-00009050: 2873 656c 662e 6669 6c69 6e67 5f69 6e66  (self.filing_inf
-00009060: 6f72 6d61 7469 6f6e 290a 0a20 2020 2020  ormation)..     
-00009070: 2020 2073 7562 6a65 6374 5f63 6f6d 7061     subject_compa
-00009080: 6e79 5f72 656e 6465 7261 626c 6573 2e61  ny_renderables.a
-00009090: 7070 656e 6428 7365 6c66 2e63 6f6d 7061  ppend(self.compa
-000090a0: 6e79 5f69 6e66 6f72 6d61 7469 6f6e 290a  ny_information).
-000090b0: 0a20 2020 2020 2020 2023 2041 6464 7265  .        # Addre
-000090c0: 7373 6573 0a20 2020 2020 2020 2069 6620  sses.        if 
-000090d0: 7365 6c66 2e62 7573 696e 6573 735f 6164  self.business_ad
-000090e0: 6472 6573 7320 6f72 2073 656c 662e 6d61  dress or self.ma
-000090f0: 696c 696e 675f 6164 6472 6573 733a 0a20  iling_address:. 
-00009100: 2020 2020 2020 2020 2020 2073 7562 6a65             subje
-00009110: 6374 5f63 6f6d 7061 6e79 5f72 656e 6465  ct_company_rende
-00009120: 7261 626c 6573 2e61 7070 656e 6428 5f63  rables.append(_c
-00009130: 7265 6174 655f 6164 6472 6573 735f 7461  reate_address_ta
-00009140: 626c 6528 7365 6c66 2e62 7573 696e 6573  ble(self.busines
-00009150: 735f 6164 6472 6573 732c 2073 656c 662e  s_address, self.
-00009160: 6d61 696c 696e 675f 6164 6472 6573 7329  mailing_address)
-00009170: 290a 0a20 2020 2020 2020 2023 2046 6f72  )..        # For
-00009180: 6d65 7220 436f 6d70 616e 7920 4e61 6d65  mer Company Name
-00009190: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
-000091a0: 662e 666f 726d 6572 5f63 6f6d 7061 6e79  f.former_company
-000091b0: 5f6e 616d 6573 3a0a 2020 2020 2020 2020  _names:.        
-000091c0: 2020 2020 666f 726d 6572 5f63 6f6d 7061      former_compa
-000091d0: 6e79 5f74 6162 6c65 203d 2054 6162 6c65  ny_table = Table
-000091e0: 2822 466f 726d 6572 204e 616d 6522 2c20  ("Former Name", 
-000091f0: 2244 6174 6520 4368 616e 6765 6422 2c20  "Date Changed", 
-00009200: 626f 783d 626f 782e 5349 4d50 4c45 290a  box=box.SIMPLE).
-00009210: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00009220: 636f 6d70 616e 7920 696e 2073 656c 662e  company in self.
-00009230: 666f 726d 6572 5f63 6f6d 7061 6e79 5f6e  former_company_n
-00009240: 616d 6573 3a0a 2020 2020 2020 2020 2020  ames:.          
-00009250: 2020 2020 2020 666f 726d 6572 5f63 6f6d        former_com
-00009260: 7061 6e79 5f74 6162 6c65 2e61 6464 5f72  pany_table.add_r
-00009270: 6f77 2863 6f6d 7061 6e79 2e6e 616d 652c  ow(company.name,
-00009280: 2063 6f6d 7061 6e79 2e64 6174 655f 6f66   company.date_of
-00009290: 5f63 6861 6e67 6529 0a20 2020 2020 2020  _change).       
-000092a0: 2020 2020 2073 7562 6a65 6374 5f63 6f6d       subject_com
-000092b0: 7061 6e79 5f72 656e 6465 7261 626c 6573  pany_renderables
-000092c0: 2e61 7070 656e 6428 666f 726d 6572 5f63  .append(former_c
-000092d0: 6f6d 7061 6e79 5f74 6162 6c65 290a 0a20  ompany_table).. 
-000092e0: 2020 2020 2020 2072 6574 7572 6e20 5061         return Pa
-000092f0: 6e65 6c28 0a20 2020 2020 2020 2020 2020  nel(.           
-00009300: 2047 726f 7570 280a 2020 2020 2020 2020   Group(.        
-00009310: 2020 2020 2020 2020 2a73 7562 6a65 6374          *subject
-00009320: 5f63 6f6d 7061 6e79 5f72 656e 6465 7261  _company_rendera
-00009330: 626c 6573 0a20 2020 2020 2020 2020 2020  bles.           
-00009340: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-00009350: 7469 746c 653d 2253 5542 4a45 4354 2043  title="SUBJECT C
-00009360: 4f4d 5041 4e59 220a 2020 2020 2020 2020  OMPANY".        
-00009370: 290a 0a20 2020 2064 6566 205f 5f72 6570  )..    def __rep
-00009380: 725f 5f28 7365 6c66 293a 0a20 2020 2020  r__(self):.     
-00009390: 2020 2072 6574 7572 6e20 7265 7072 5f72     return repr_r
-000093a0: 6963 6828 7365 6c66 2e5f 5f72 6963 685f  ich(self.__rich_
-000093b0: 5f28 2929 0a0a 0a40 6461 7461 636c 6173  _())...@dataclas
-000093c0: 7328 6672 6f7a 656e 3d54 7275 6529 0a63  s(frozen=True).c
-000093d0: 6c61 7373 2049 7373 7565 723a 0a20 2020  lass Issuer:.   
-000093e0: 2063 6f6d 7061 6e79 5f69 6e66 6f72 6d61   company_informa
-000093f0: 7469 6f6e 3a20 436f 6d70 616e 7949 6e66  tion: CompanyInf
-00009400: 6f72 6d61 7469 6f6e 0a20 2020 2062 7573  ormation.    bus
-00009410: 696e 6573 735f 6164 6472 6573 733a 2041  iness_address: A
-00009420: 6464 7265 7373 0a20 2020 206d 6169 6c69  ddress.    maili
-00009430: 6e67 5f61 6464 7265 7373 3a20 4164 6472  ng_address: Addr
-00009440: 6573 730a 0a20 2020 2064 6566 205f 5f72  ess..    def __r
-00009450: 6963 685f 5f28 7365 6c66 293a 0a20 2020  ich__(self):.   
-00009460: 2020 2020 2069 7373 7565 725f 7461 626c       issuer_tabl
-00009470: 6520 3d20 5461 626c 6528 2243 6f6d 7061  e = Table("Compa
-00009480: 6e79 222c 2022 4349 4b22 2c20 2253 4943  ny", "CIK", "SIC
-00009490: 222c 2022 4669 7363 616c 2059 6561 7220  ", "Fiscal Year 
-000094a0: 456e 6422 2c0a 2020 2020 2020 2020 2020  End",.          
+00008c60: 2020 2020 2020 2073 656c 662e 6669 6c69         self.fili
+00008c70: 6e67 5f69 6e66 6f72 6d61 7469 6f6e 2e66  ng_information.f
+00008c80: 696c 6d5f 6e75 6d62 6572 290a 2020 2020  ilm_number).    
+00008c90: 2020 2020 2020 2020 746f 705f 7265 6e64          top_rend
+00008ca0: 6572 6162 6c65 732e 6170 7065 6e64 2866  erables.append(f
+00008cb0: 696c 696e 675f 7661 6c75 6573 5f74 6162  iling_values_tab
+00008cc0: 6c65 290a 0a20 2020 2020 2020 2072 6570  le)..        rep
+00008cd0: 6f72 7469 6e67 5f6f 776e 6572 5f72 656e  orting_owner_ren
+00008ce0: 6465 7261 626c 6573 203d 205b 436f 6c75  derables = [Colu
+00008cf0: 6d6e 7328 746f 705f 7265 6e64 6572 6162  mns(top_renderab
+00008d00: 6c65 7329 5d0a 0a20 2020 2020 2020 2023  les)]..        #
+00008d10: 2041 6464 7265 7373 6573 0a20 2020 2020   Addresses.     
+00008d20: 2020 2069 6620 7365 6c66 2e62 7573 696e     if self.busin
+00008d30: 6573 735f 6164 6472 6573 7320 6f72 2073  ess_address or s
+00008d40: 656c 662e 6d61 696c 696e 675f 6164 6472  elf.mailing_addr
+00008d50: 6573 733a 0a20 2020 2020 2020 2020 2020  ess:.           
+00008d60: 2072 6570 6f72 7469 6e67 5f6f 776e 6572   reporting_owner
+00008d70: 5f72 656e 6465 7261 626c 6573 2e61 7070  _renderables.app
+00008d80: 656e 6428 5f63 7265 6174 655f 6164 6472  end(_create_addr
+00008d90: 6573 735f 7461 626c 6528 7365 6c66 2e62  ess_table(self.b
+00008da0: 7573 696e 6573 735f 6164 6472 6573 732c  usiness_address,
+00008db0: 2073 656c 662e 6d61 696c 696e 675f 6164   self.mailing_ad
+00008dc0: 6472 6573 7329 290a 0a20 2020 2020 2020  dress))..       
+00008dd0: 2072 6574 7572 6e20 5061 6e65 6c28 0a20   return Panel(. 
+00008de0: 2020 2020 2020 2020 2020 2047 726f 7570             Group
+00008df0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00008e00: 2020 2a72 6570 6f72 7469 6e67 5f6f 776e    *reporting_own
+00008e10: 6572 5f72 656e 6465 7261 626c 6573 0a20  er_renderables. 
+00008e20: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
+00008e30: 2020 2020 2020 2020 2020 7469 746c 653d            title=
+00008e40: 7265 706f 7274 696e 675f 6f77 6e65 725f  reporting_owner_
+00008e50: 7469 746c 650a 2020 2020 2020 2020 290a  title.        ).
+00008e60: 0a20 2020 2064 6566 205f 5f72 6570 725f  .    def __repr_
+00008e70: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
+00008e80: 2072 6574 7572 6e20 7265 7072 5f72 6963   return repr_ric
+00008e90: 6828 7365 6c66 2e5f 5f72 6963 685f 5f28  h(self.__rich__(
+00008ea0: 2929 0a0a 0a40 6461 7461 636c 6173 7328  ))...@dataclass(
+00008eb0: 6672 6f7a 656e 3d54 7275 6529 0a63 6c61  frozen=True).cla
+00008ec0: 7373 2053 7562 6a65 6374 436f 6d70 616e  ss SubjectCompan
+00008ed0: 793a 0a20 2020 2063 6f6d 7061 6e79 5f69  y:.    company_i
+00008ee0: 6e66 6f72 6d61 7469 6f6e 3a20 436f 6d70  nformation: Comp
+00008ef0: 616e 7949 6e66 6f72 6d61 7469 6f6e 0a20  anyInformation. 
+00008f00: 2020 2066 696c 696e 675f 696e 666f 726d     filing_inform
+00008f10: 6174 696f 6e3a 2046 696c 696e 6749 6e66  ation: FilingInf
+00008f20: 6f72 6d61 7469 6f6e 0a20 2020 2062 7573  ormation.    bus
+00008f30: 696e 6573 735f 6164 6472 6573 733a 2041  iness_address: A
+00008f40: 6464 7265 7373 0a20 2020 206d 6169 6c69  ddress.    maili
+00008f50: 6e67 5f61 6464 7265 7373 3a20 4164 6472  ng_address: Addr
+00008f60: 6573 730a 2020 2020 666f 726d 6572 5f63  ess.    former_c
+00008f70: 6f6d 7061 6e79 5f6e 616d 6573 3a20 4f70  ompany_names: Op
+00008f80: 7469 6f6e 616c 5b4c 6973 745b 466f 726d  tional[List[Form
+00008f90: 6572 436f 6d70 616e 795d 5d20 3d20 4e6f  erCompany]] = No
+00008fa0: 6e65 0a0a 2020 2020 6465 6620 5f5f 7269  ne..    def __ri
+00008fb0: 6368 5f5f 2873 656c 6629 3a0a 2020 2020  ch__(self):.    
+00008fc0: 2020 2020 7375 626a 6563 745f 636f 6d70      subject_comp
+00008fd0: 616e 795f 7265 6e64 6572 6162 6c65 7320  any_renderables 
+00008fe0: 3d20 5b5d 0a0a 2020 2020 2020 2020 2320  = []..        # 
+00008ff0: 4669 6c69 6e67 2049 6e66 6f72 6d61 7469  Filing Informati
+00009000: 6f6e 0a20 2020 2020 2020 2069 6620 7365  on.        if se
+00009010: 6c66 2e66 696c 696e 675f 696e 666f 726d  lf.filing_inform
+00009020: 6174 696f 6e3a 0a20 2020 2020 2020 2020  ation:.         
+00009030: 2020 2073 7562 6a65 6374 5f63 6f6d 7061     subject_compa
+00009040: 6e79 5f72 656e 6465 7261 626c 6573 2e61  ny_renderables.a
+00009050: 7070 656e 6428 7365 6c66 2e66 696c 696e  ppend(self.filin
+00009060: 675f 696e 666f 726d 6174 696f 6e29 0a0a  g_information)..
+00009070: 2020 2020 2020 2020 7375 626a 6563 745f          subject_
+00009080: 636f 6d70 616e 795f 7265 6e64 6572 6162  company_renderab
+00009090: 6c65 732e 6170 7065 6e64 2873 656c 662e  les.append(self.
+000090a0: 636f 6d70 616e 795f 696e 666f 726d 6174  company_informat
+000090b0: 696f 6e29 0a0a 2020 2020 2020 2020 2320  ion)..        # 
+000090c0: 4164 6472 6573 7365 730a 2020 2020 2020  Addresses.      
+000090d0: 2020 6966 2073 656c 662e 6275 7369 6e65    if self.busine
+000090e0: 7373 5f61 6464 7265 7373 206f 7220 7365  ss_address or se
+000090f0: 6c66 2e6d 6169 6c69 6e67 5f61 6464 7265  lf.mailing_addre
+00009100: 7373 3a0a 2020 2020 2020 2020 2020 2020  ss:.            
+00009110: 7375 626a 6563 745f 636f 6d70 616e 795f  subject_company_
+00009120: 7265 6e64 6572 6162 6c65 732e 6170 7065  renderables.appe
+00009130: 6e64 285f 6372 6561 7465 5f61 6464 7265  nd(_create_addre
+00009140: 7373 5f74 6162 6c65 2873 656c 662e 6275  ss_table(self.bu
+00009150: 7369 6e65 7373 5f61 6464 7265 7373 2c20  siness_address, 
+00009160: 7365 6c66 2e6d 6169 6c69 6e67 5f61 6464  self.mailing_add
+00009170: 7265 7373 2929 0a0a 2020 2020 2020 2020  ress))..        
+00009180: 2320 466f 726d 6572 2043 6f6d 7061 6e79  # Former Company
+00009190: 204e 616d 6573 0a20 2020 2020 2020 2069   Names.        i
+000091a0: 6620 7365 6c66 2e66 6f72 6d65 725f 636f  f self.former_co
+000091b0: 6d70 616e 795f 6e61 6d65 733a 0a20 2020  mpany_names:.   
+000091c0: 2020 2020 2020 2020 2066 6f72 6d65 725f           former_
+000091d0: 636f 6d70 616e 795f 7461 626c 6520 3d20  company_table = 
+000091e0: 5461 626c 6528 2246 6f72 6d65 7220 4e61  Table("Former Na
+000091f0: 6d65 222c 2022 4461 7465 2043 6861 6e67  me", "Date Chang
+00009200: 6564 222c 2062 6f78 3d62 6f78 2e53 494d  ed", box=box.SIM
+00009210: 504c 4529 0a20 2020 2020 2020 2020 2020  PLE).           
+00009220: 2066 6f72 2063 6f6d 7061 6e79 2069 6e20   for company in 
+00009230: 7365 6c66 2e66 6f72 6d65 725f 636f 6d70  self.former_comp
+00009240: 616e 795f 6e61 6d65 733a 0a20 2020 2020  any_names:.     
+00009250: 2020 2020 2020 2020 2020 2066 6f72 6d65             forme
+00009260: 725f 636f 6d70 616e 795f 7461 626c 652e  r_company_table.
+00009270: 6164 645f 726f 7728 636f 6d70 616e 792e  add_row(company.
+00009280: 6e61 6d65 2c20 636f 6d70 616e 792e 6461  name, company.da
+00009290: 7465 5f6f 665f 6368 616e 6765 290a 2020  te_of_change).  
+000092a0: 2020 2020 2020 2020 2020 7375 626a 6563            subjec
+000092b0: 745f 636f 6d70 616e 795f 7265 6e64 6572  t_company_render
+000092c0: 6162 6c65 732e 6170 7065 6e64 2866 6f72  ables.append(for
+000092d0: 6d65 725f 636f 6d70 616e 795f 7461 626c  mer_company_tabl
+000092e0: 6529 0a0a 2020 2020 2020 2020 7265 7475  e)..        retu
+000092f0: 726e 2050 616e 656c 280a 2020 2020 2020  rn Panel(.      
+00009300: 2020 2020 2020 4772 6f75 7028 0a20 2020        Group(.   
+00009310: 2020 2020 2020 2020 2020 2020 202a 7375               *su
+00009320: 626a 6563 745f 636f 6d70 616e 795f 7265  bject_company_re
+00009330: 6e64 6572 6162 6c65 730a 2020 2020 2020  nderables.      
+00009340: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+00009350: 2020 2020 2074 6974 6c65 3d22 5355 424a       title="SUBJ
+00009360: 4543 5420 434f 4d50 414e 5922 0a20 2020  ECT COMPANY".   
+00009370: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+00009380: 5f5f 7265 7072 5f5f 2873 656c 6629 3a0a  __repr__(self):.
+00009390: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+000093a0: 6570 725f 7269 6368 2873 656c 662e 5f5f  epr_rich(self.__
+000093b0: 7269 6368 5f5f 2829 290a 0a0a 4064 6174  rich__())...@dat
+000093c0: 6163 6c61 7373 2866 726f 7a65 6e3d 5472  aclass(frozen=Tr
+000093d0: 7565 290a 636c 6173 7320 4973 7375 6572  ue).class Issuer
+000093e0: 3a0a 2020 2020 636f 6d70 616e 795f 696e  :.    company_in
+000093f0: 666f 726d 6174 696f 6e3a 2043 6f6d 7061  formation: Compa
+00009400: 6e79 496e 666f 726d 6174 696f 6e0a 2020  nyInformation.  
+00009410: 2020 6275 7369 6e65 7373 5f61 6464 7265    business_addre
+00009420: 7373 3a20 4164 6472 6573 730a 2020 2020  ss: Address.    
+00009430: 6d61 696c 696e 675f 6164 6472 6573 733a  mailing_address:
+00009440: 2041 6464 7265 7373 0a0a 2020 2020 6465   Address..    de
+00009450: 6620 5f5f 7269 6368 5f5f 2873 656c 6629  f __rich__(self)
+00009460: 3a0a 2020 2020 2020 2020 6973 7375 6572  :.        issuer
+00009470: 5f74 6162 6c65 203d 2054 6162 6c65 2822  _table = Table("
+00009480: 436f 6d70 616e 7922 2c20 2243 494b 222c  Company", "CIK",
+00009490: 2022 5349 4322 2c20 2246 6973 6361 6c20   "SIC", "Fiscal 
+000094a0: 5965 6172 2045 6e64 222c 0a20 2020 2020  Year End",.     
 000094b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094c0: 2020 2062 6f78 3d62 6f78 2e53 494d 504c     box=box.SIMPL
-000094d0: 4529 0a20 2020 2020 2020 2069 7373 7565  E).        issue
-000094e0: 725f 7461 626c 652e 6164 645f 726f 7728  r_table.add_row(
-000094f0: 7365 6c66 2e63 6f6d 7061 6e79 5f69 6e66  self.company_inf
-00009500: 6f72 6d61 7469 6f6e 2e6e 616d 652c 0a20  ormation.name,. 
-00009510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009520: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00009530: 2e63 6f6d 7061 6e79 5f69 6e66 6f72 6d61  .company_informa
-00009540: 7469 6f6e 2e63 696b 2c0a 2020 2020 2020  tion.cik,.      
+000094c0: 2020 2020 2020 2020 626f 783d 626f 782e          box=box.
+000094d0: 5349 4d50 4c45 290a 2020 2020 2020 2020  SIMPLE).        
+000094e0: 6973 7375 6572 5f74 6162 6c65 2e61 6464  issuer_table.add
+000094f0: 5f72 6f77 2873 656c 662e 636f 6d70 616e  _row(self.compan
+00009500: 795f 696e 666f 726d 6174 696f 6e2e 6e61  y_information.na
+00009510: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+00009520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009530: 2073 656c 662e 636f 6d70 616e 795f 696e   self.company_in
+00009540: 666f 726d 6174 696f 6e2e 6369 6b2c 0a20  formation.cik,. 
 00009550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009560: 2020 2020 2020 2073 656c 662e 636f 6d70         self.comp
-00009570: 616e 795f 696e 666f 726d 6174 696f 6e2e  any_information.
-00009580: 7369 632c 0a20 2020 2020 2020 2020 2020  sic,.           
+00009560: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009570: 2e63 6f6d 7061 6e79 5f69 6e66 6f72 6d61  .company_informa
+00009580: 7469 6f6e 2e73 6963 2c0a 2020 2020 2020  tion.sic,.      
 00009590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095a0: 2020 7365 6c66 2e63 6f6d 7061 6e79 5f69    self.company_i
-000095b0: 6e66 6f72 6d61 7469 6f6e 2e66 6973 6361  nformation.fisca
-000095c0: 6c5f 7965 6172 5f65 6e64 290a 0a20 2020  l_year_end)..   
-000095d0: 2020 2020 2023 2054 6865 206c 6973 7420       # The list 
-000095e0: 6f66 2072 656e 6465 7261 626c 6573 2066  of renderables f
-000095f0: 6f72 2074 6865 2069 7373 7565 7220 7061  or the issuer pa
-00009600: 6e65 6c0a 2020 2020 2020 2020 6973 7375  nel.        issu
-00009610: 6572 5f72 656e 6465 7261 626c 6573 203d  er_renderables =
-00009620: 205b 6973 7375 6572 5f74 6162 6c65 5d0a   [issuer_table].
-00009630: 0a20 2020 2020 2020 2023 2041 6464 7265  .        # Addre
-00009640: 7373 6573 0a20 2020 2020 2020 2069 6620  sses.        if 
-00009650: 7365 6c66 2e62 7573 696e 6573 735f 6164  self.business_ad
-00009660: 6472 6573 7320 6f72 2073 656c 662e 6d61  dress or self.ma
-00009670: 696c 696e 675f 6164 6472 6573 733a 0a20  iling_address:. 
-00009680: 2020 2020 2020 2020 2020 2069 7373 7565             issue
-00009690: 725f 7265 6e64 6572 6162 6c65 732e 6170  r_renderables.ap
-000096a0: 7065 6e64 285f 6372 6561 7465 5f61 6464  pend(_create_add
-000096b0: 7265 7373 5f74 6162 6c65 2873 656c 662e  ress_table(self.
-000096c0: 6275 7369 6e65 7373 5f61 6464 7265 7373  business_address
-000096d0: 2c20 7365 6c66 2e6d 6169 6c69 6e67 5f61  , self.mailing_a
-000096e0: 6464 7265 7373 2929 0a0a 2020 2020 2020  ddress))..      
-000096f0: 2020 7265 7475 726e 2050 616e 656c 280a    return Panel(.
-00009700: 2020 2020 2020 2020 2020 2020 4772 6f75              Grou
-00009710: 7028 0a20 2020 2020 2020 2020 2020 2020  p(.             
-00009720: 2020 202a 6973 7375 6572 5f72 656e 6465     *issuer_rende
-00009730: 7261 626c 6573 0a20 2020 2020 2020 2020  rables.         
-00009740: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
-00009750: 2020 7469 746c 653d 6973 7375 6572 5f74    title=issuer_t
-00009760: 6974 6c65 0a20 2020 2020 2020 2029 0a0a  itle.        )..
-00009770: 2020 2020 6465 6620 5f5f 7265 7072 5f5f      def __repr__
-00009780: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00009790: 7265 7475 726e 2072 6570 725f 7269 6368  return repr_rich
-000097a0: 2873 656c 662e 5f5f 7269 6368 5f5f 2829  (self.__rich__()
-000097b0: 290a 0a0a 2320 5469 746c 6520 7465 7874  )...# Title text
-000097c0: 0a6d 6169 6c69 6e67 5f61 6464 7265 7373  .mailing_address
-000097d0: 5f74 6974 6c65 203d 2022 5c55 3030 3031  _title = "\U0001
-000097e0: 4634 4543 204d 6169 6c69 6e67 2041 6464  F4EC Mailing Add
-000097f0: 7265 7373 220a 6275 7369 6e65 7373 5f61  ress".business_a
-00009800: 6464 7265 7373 5f74 6974 6c65 203d 2022  ddress_title = "
-00009810: 5c55 3030 3031 4634 4543 2042 7573 696e  \U0001F4EC Busin
-00009820: 6573 7320 4164 6472 6573 7322 0a63 6f6d  ess Address".com
-00009830: 7061 6e79 5f74 6974 6c65 203d 2022 5c55  pany_title = "\U
-00009840: 3030 3031 4633 4532 2043 6f6d 7061 6e79  0001F3E2 Company
-00009850: 2049 6e66 6f72 6d61 7469 6f6e 220a 6669   Information".fi
-00009860: 6c69 6e67 5f69 6e66 6f72 6d61 7469 6f6e  ling_information
-00009870: 5f74 6974 6c65 203d 2022 5c55 3030 3031  _title = "\U0001
-00009880: 4634 4431 2046 696c 696e 6720 496e 666f  F4D1 Filing Info
-00009890: 726d 6174 696f 6e22 0a72 6570 6f72 7469  rmation".reporti
-000098a0: 6e67 5f6f 776e 6572 5f74 6974 6c65 203d  ng_owner_title =
-000098b0: 2022 5c55 3030 3031 4634 3638 2052 4550   "\U0001F468 REP
-000098c0: 4f52 5449 4e47 204f 574e 4552 220a 6973  ORTING OWNER".is
-000098d0: 7375 6572 5f74 6974 6c65 203d 2022 5c55  suer_title = "\U
-000098e0: 3030 3031 4634 4235 2049 5353 5545 5222  0001F4B5 ISSUER"
-000098f0: 0a66 696c 696e 675f 7469 746c 6520 3d20  .filing_title = 
-00009900: 225c 5530 3030 3146 3444 3120 4649 4c49  "\U0001F4D1 FILI
-00009910: 4e47 220a 0a0a 6465 6620 5f63 7265 6174  NG"...def _creat
-00009920: 655f 6164 6472 6573 735f 7461 626c 6528  e_address_table(
-00009930: 6275 7369 6e65 7373 5f61 6464 7265 7373  business_address
-00009940: 3a20 4164 6472 6573 732c 206d 6169 6c69  : Address, maili
-00009950: 6e67 5f61 6464 7265 7373 3a20 4164 6472  ng_address: Addr
-00009960: 6573 7329 3a0a 2020 2020 6164 6472 6573  ess):.    addres
-00009970: 735f 7461 626c 6520 3d20 5461 626c 6528  s_table = Table(
-00009980: 2254 7970 6522 2c20 2253 7472 6565 7431  "Type", "Street1
-00009990: 222c 2022 5374 7265 6574 3222 2c20 2243  ", "Street2", "C
-000099a0: 6974 7922 2c20 2253 7461 7465 222c 2022  ity", "State", "
-000099b0: 5a69 7063 6f64 6522 2c0a 2020 2020 2020  Zipcode",.      
+000095a0: 2020 2020 2020 2073 656c 662e 636f 6d70         self.comp
+000095b0: 616e 795f 696e 666f 726d 6174 696f 6e2e  any_information.
+000095c0: 6669 7363 616c 5f79 6561 725f 656e 6429  fiscal_year_end)
+000095d0: 0a0a 2020 2020 2020 2020 2320 5468 6520  ..        # The 
+000095e0: 6c69 7374 206f 6620 7265 6e64 6572 6162  list of renderab
+000095f0: 6c65 7320 666f 7220 7468 6520 6973 7375  les for the issu
+00009600: 6572 2070 616e 656c 0a20 2020 2020 2020  er panel.       
+00009610: 2069 7373 7565 725f 7265 6e64 6572 6162   issuer_renderab
+00009620: 6c65 7320 3d20 5b69 7373 7565 725f 7461  les = [issuer_ta
+00009630: 626c 655d 0a0a 2020 2020 2020 2020 2320  ble]..        # 
+00009640: 4164 6472 6573 7365 730a 2020 2020 2020  Addresses.      
+00009650: 2020 6966 2073 656c 662e 6275 7369 6e65    if self.busine
+00009660: 7373 5f61 6464 7265 7373 206f 7220 7365  ss_address or se
+00009670: 6c66 2e6d 6169 6c69 6e67 5f61 6464 7265  lf.mailing_addre
+00009680: 7373 3a0a 2020 2020 2020 2020 2020 2020  ss:.            
+00009690: 6973 7375 6572 5f72 656e 6465 7261 626c  issuer_renderabl
+000096a0: 6573 2e61 7070 656e 6428 5f63 7265 6174  es.append(_creat
+000096b0: 655f 6164 6472 6573 735f 7461 626c 6528  e_address_table(
+000096c0: 7365 6c66 2e62 7573 696e 6573 735f 6164  self.business_ad
+000096d0: 6472 6573 732c 2073 656c 662e 6d61 696c  dress, self.mail
+000096e0: 696e 675f 6164 6472 6573 7329 290a 0a20  ing_address)).. 
+000096f0: 2020 2020 2020 2072 6574 7572 6e20 5061         return Pa
+00009700: 6e65 6c28 0a20 2020 2020 2020 2020 2020  nel(.           
+00009710: 2047 726f 7570 280a 2020 2020 2020 2020   Group(.        
+00009720: 2020 2020 2020 2020 2a69 7373 7565 725f          *issuer_
+00009730: 7265 6e64 6572 6162 6c65 730a 2020 2020  renderables.    
+00009740: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+00009750: 2020 2020 2020 2074 6974 6c65 3d69 7373         title=iss
+00009760: 7565 725f 7469 746c 650a 2020 2020 2020  uer_title.      
+00009770: 2020 290a 0a20 2020 2064 6566 205f 5f72    )..    def __r
+00009780: 6570 725f 5f28 7365 6c66 293a 0a20 2020  epr__(self):.   
+00009790: 2020 2020 2072 6574 7572 6e20 7265 7072       return repr
+000097a0: 5f72 6963 6828 7365 6c66 2e5f 5f72 6963  _rich(self.__ric
+000097b0: 685f 5f28 2929 0a0a 0a23 2054 6974 6c65  h__())...# Title
+000097c0: 2074 6578 740a 6d61 696c 696e 675f 6164   text.mailing_ad
+000097d0: 6472 6573 735f 7469 746c 6520 3d20 225c  dress_title = "\
+000097e0: 5530 3030 3146 3445 4320 4d61 696c 696e  U0001F4EC Mailin
+000097f0: 6720 4164 6472 6573 7322 0a62 7573 696e  g Address".busin
+00009800: 6573 735f 6164 6472 6573 735f 7469 746c  ess_address_titl
+00009810: 6520 3d20 225c 5530 3030 3146 3445 4320  e = "\U0001F4EC 
+00009820: 4275 7369 6e65 7373 2041 6464 7265 7373  Business Address
+00009830: 220a 636f 6d70 616e 795f 7469 746c 6520  ".company_title 
+00009840: 3d20 225c 5530 3030 3146 3345 3220 436f  = "\U0001F3E2 Co
+00009850: 6d70 616e 7920 496e 666f 726d 6174 696f  mpany Informatio
+00009860: 6e22 0a66 696c 696e 675f 696e 666f 726d  n".filing_inform
+00009870: 6174 696f 6e5f 7469 746c 6520 3d20 225c  ation_title = "\
+00009880: 5530 3030 3146 3444 3120 4669 6c69 6e67  U0001F4D1 Filing
+00009890: 2049 6e66 6f72 6d61 7469 6f6e 220a 7265   Information".re
+000098a0: 706f 7274 696e 675f 6f77 6e65 725f 7469  porting_owner_ti
+000098b0: 746c 6520 3d20 225c 5530 3030 3146 3436  tle = "\U0001F46
+000098c0: 3820 5245 504f 5254 494e 4720 4f57 4e45  8 REPORTING OWNE
+000098d0: 5222 0a69 7373 7565 725f 7469 746c 6520  R".issuer_title 
+000098e0: 3d20 225c 5530 3030 3146 3442 3520 4953  = "\U0001F4B5 IS
+000098f0: 5355 4552 220a 6669 6c69 6e67 5f74 6974  SUER".filing_tit
+00009900: 6c65 203d 2022 5c55 3030 3031 4634 4431  le = "\U0001F4D1
+00009910: 2046 494c 494e 4722 0a0a 0a64 6566 205f   FILING"...def _
+00009920: 6372 6561 7465 5f61 6464 7265 7373 5f74  create_address_t
+00009930: 6162 6c65 2862 7573 696e 6573 735f 6164  able(business_ad
+00009940: 6472 6573 733a 2041 6464 7265 7373 2c20  dress: Address, 
+00009950: 6d61 696c 696e 675f 6164 6472 6573 733a  mailing_address:
+00009960: 2041 6464 7265 7373 293a 0a20 2020 2061   Address):.    a
+00009970: 6464 7265 7373 5f74 6162 6c65 203d 2054  ddress_table = T
+00009980: 6162 6c65 2822 5479 7065 222c 2022 5374  able("Type", "St
+00009990: 7265 6574 3122 2c20 2253 7472 6565 7432  reet1", "Street2
+000099a0: 222c 2022 4369 7479 222c 2022 5374 6174  ", "City", "Stat
+000099b0: 6522 2c20 225a 6970 636f 6465 222c 0a20  e", "Zipcode",. 
 000099c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099d0: 2020 2020 7469 746c 653d 225c 5530 3030      title="\U000
-000099e0: 3146 3445 4320 4164 6472 6573 7365 7322  1F4EC Addresses"
-000099f0: 2c20 626f 783d 626f 782e 5349 4d50 4c45  , box=box.SIMPLE
-00009a00: 290a 2020 2020 6966 2062 7573 696e 6573  ).    if busines
-00009a10: 735f 6164 6472 6573 733a 0a20 2020 2020  s_address:.     
-00009a20: 2020 2061 6464 7265 7373 5f74 6162 6c65     address_table
-00009a30: 2e61 6464 5f72 6f77 2822 5c55 3030 3031  .add_row("\U0001
-00009a40: 4633 4532 2042 7573 696e 6573 7320 4164  F3E2 Business Ad
-00009a50: 6472 6573 7322 2c0a 2020 2020 2020 2020  dress",.        
+000099d0: 2020 2020 2020 2020 2074 6974 6c65 3d22           title="
+000099e0: 5c55 3030 3031 4634 4543 2041 6464 7265  \U0001F4EC Addre
+000099f0: 7373 6573 222c 2062 6f78 3d62 6f78 2e53  sses", box=box.S
+00009a00: 494d 504c 4529 0a20 2020 2069 6620 6275  IMPLE).    if bu
+00009a10: 7369 6e65 7373 5f61 6464 7265 7373 3a0a  siness_address:.
+00009a20: 2020 2020 2020 2020 6164 6472 6573 735f          address_
+00009a30: 7461 626c 652e 6164 645f 726f 7728 225c  table.add_row("\
+00009a40: 5530 3030 3146 3345 3220 4275 7369 6e65  U0001F3E2 Busine
+00009a50: 7373 2041 6464 7265 7373 222c 0a20 2020  ss Address",.   
 00009a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a70: 2020 2020 2020 6275 7369 6e65 7373 5f61        business_a
-00009a80: 6464 7265 7373 2e73 7472 6565 7431 2c0a  ddress.street1,.
-00009a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009aa0: 2020 2020 2020 2020 2020 2020 2020 6275                bu
-00009ab0: 7369 6e65 7373 5f61 6464 7265 7373 2e73  siness_address.s
-00009ac0: 7472 6565 7432 2c0a 2020 2020 2020 2020  treet2,.        
+00009a70: 2020 2020 2020 2020 2020 2062 7573 696e             busin
+00009a80: 6573 735f 6164 6472 6573 732e 7374 7265  ess_address.stre
+00009a90: 6574 312c 0a20 2020 2020 2020 2020 2020  et1,.           
+00009aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ab0: 2020 2062 7573 696e 6573 735f 6164 6472     business_addr
+00009ac0: 6573 732e 7374 7265 6574 322c 0a20 2020  ess.street2,.   
 00009ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ae0: 2020 2020 2020 6275 7369 6e65 7373 5f61        business_a
-00009af0: 6464 7265 7373 2e63 6974 792c 0a20 2020  ddress.city,.   
-00009b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b10: 2020 2020 2020 2020 2020 2062 7573 696e             busin
-00009b20: 6573 735f 6164 6472 6573 732e 7374 6174  ess_address.stat
-00009b30: 655f 6f72 5f63 6f75 6e74 7279 2c0a 2020  e_or_country,.  
-00009b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b50: 2020 2020 2020 2020 2020 2020 6275 7369              busi
-00009b60: 6e65 7373 5f61 6464 7265 7373 2e7a 6970  ness_address.zip
-00009b70: 636f 6465 290a 0a20 2020 2069 6620 6d61  code)..    if ma
-00009b80: 696c 696e 675f 6164 6472 6573 733a 0a20  iling_address:. 
-00009b90: 2020 2020 2020 2061 6464 7265 7373 5f74         address_t
-00009ba0: 6162 6c65 2e61 6464 5f72 6f77 2822 5c55  able.add_row("\U
-00009bb0: 3030 3031 4634 4544 204d 6169 6c69 6e67  0001F4ED Mailing
-00009bc0: 2041 6464 7265 7373 222c 0a20 2020 2020   Address",.     
+00009ae0: 2020 2020 2020 2020 2020 2062 7573 696e             busin
+00009af0: 6573 735f 6164 6472 6573 732e 6369 7479  ess_address.city
+00009b00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00009b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b20: 6275 7369 6e65 7373 5f61 6464 7265 7373  business_address
+00009b30: 2e73 7461 7465 5f6f 725f 636f 756e 7472  .state_or_countr
+00009b40: 792c 0a20 2020 2020 2020 2020 2020 2020  y,.             
+00009b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b60: 2062 7573 696e 6573 735f 6164 6472 6573   business_addres
+00009b70: 732e 7a69 7063 6f64 6529 0a0a 2020 2020  s.zipcode)..    
+00009b80: 6966 206d 6169 6c69 6e67 5f61 6464 7265  if mailing_addre
+00009b90: 7373 3a0a 2020 2020 2020 2020 6164 6472  ss:.        addr
+00009ba0: 6573 735f 7461 626c 652e 6164 645f 726f  ess_table.add_ro
+00009bb0: 7728 225c 5530 3030 3146 3445 4420 4d61  w("\U0001F4ED Ma
+00009bc0: 696c 696e 6720 4164 6472 6573 7322 2c0a  iling Address",.
 00009bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009be0: 2020 2020 2020 2020 206d 6169 6c69 6e67           mailing
-00009bf0: 5f61 6464 7265 7373 2e73 7472 6565 7431  _address.street1
-00009c00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00009be0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+00009bf0: 696c 696e 675f 6164 6472 6573 732e 7374  iling_address.st
+00009c00: 7265 6574 312c 0a20 2020 2020 2020 2020  reet1,.         
 00009c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c20: 6d61 696c 696e 675f 6164 6472 6573 732e  mailing_address.
-00009c30: 7374 7265 6574 322c 0a20 2020 2020 2020  street2,.       
+00009c20: 2020 2020 206d 6169 6c69 6e67 5f61 6464       mailing_add
+00009c30: 7265 7373 2e73 7472 6565 7432 2c0a 2020  ress.street2,.  
 00009c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c50: 2020 2020 2020 206d 6169 6c69 6e67 5f61         mailing_a
-00009c60: 6464 7265 7373 2e63 6974 792c 0a20 2020  ddress.city,.   
-00009c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c80: 2020 2020 2020 2020 2020 206d 6169 6c69             maili
-00009c90: 6e67 5f61 6464 7265 7373 2e73 7461 7465  ng_address.state
-00009ca0: 5f6f 725f 636f 756e 7472 792c 0a20 2020  _or_country,.   
-00009cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cc0: 2020 2020 2020 2020 2020 206d 6169 6c69             maili
-00009cd0: 6e67 5f61 6464 7265 7373 2e7a 6970 636f  ng_address.zipco
-00009ce0: 6465 290a 2020 2020 7265 7475 726e 2061  de).    return a
-00009cf0: 6464 7265 7373 5f74 6162 6c65 0a0a 0a63  ddress_table...c
-00009d00: 6c61 7373 2053 4543 4865 6164 6572 3a0a  lass SECHeader:.
-00009d10: 2020 2020 2222 220a 2020 2020 436f 6e74      """.    Cont
-00009d20: 6169 6e73 2074 6865 2070 6172 7365 6420  ains the parsed 
-00009d30: 7265 7072 6573 656e 7461 7469 6f6e 206f  representation o
-00009d40: 6620 7468 6520 5345 432d 4845 4144 4552  f the SEC-HEADER
-00009d50: 2074 6578 7420 6174 2074 6865 2074 6f70   text at the top
-00009d60: 206f 6620 7468 6520 6675 6c6c 2073 7562   of the full sub
-00009d70: 6d69 7373 696f 6e20 7465 7874 0a20 2020  mission text.   
-00009d80: 203c 5345 432d 4845 4144 4552 3e0a 0a20   <SEC-HEADER>.. 
-00009d90: 2020 203c 2f53 4543 2d48 4541 4445 523e     </SEC-HEADER>
-00009da0: 0a20 2020 2022 2222 0a0a 2020 2020 6465  .    """..    de
-00009db0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-00009dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009dd0: 2020 7465 7874 3a20 7374 722c 0a20 2020    text: str,.   
-00009de0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-00009df0: 6c69 6e67 5f6d 6574 6164 6174 613a 2044  ling_metadata: D
-00009e00: 6963 745b 7374 722c 2073 7472 5d2c 0a20  ict[str, str],. 
-00009e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e20: 6669 6c65 7273 3a20 4c69 7374 5b46 696c  filers: List[Fil
-00009e30: 6572 5d20 3d20 4e6f 6e65 2c0a 2020 2020  er] = None,.    
-00009e40: 2020 2020 2020 2020 2020 2020 2072 6570               rep
-00009e50: 6f72 7469 6e67 5f6f 776e 6572 733a 204c  orting_owners: L
-00009e60: 6973 745b 5265 706f 7274 696e 674f 776e  ist[ReportingOwn
-00009e70: 6572 5d20 3d20 4e6f 6e65 2c0a 2020 2020  er] = None,.    
-00009e80: 2020 2020 2020 2020 2020 2020 2069 7373               iss
-00009e90: 7565 7273 3a20 4c69 7374 5b49 7373 7565  uers: List[Issue
-00009ea0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-00009eb0: 2020 2020 2020 2020 2020 2020 7375 626a              subj
-00009ec0: 6563 745f 636f 6d70 616e 6965 733a 204c  ect_companies: L
-00009ed0: 6973 745b 5375 626a 6563 7443 6f6d 7061  ist[SubjectCompa
-00009ee0: 6e79 5d20 3d20 4e6f 6e65 293a 0a20 2020  ny] = None):.   
-00009ef0: 2020 2020 2073 656c 662e 7465 7874 3a20       self.text: 
-00009f00: 7374 7220 3d20 7465 7874 0a20 2020 2020  str = text.     
-00009f10: 2020 2073 656c 662e 6669 6c69 6e67 5f6d     self.filing_m
-00009f20: 6574 6164 6174 613a 2044 6963 745b 7374  etadata: Dict[st
-00009f30: 722c 2073 7472 5d20 3d20 6669 6c69 6e67  r, str] = filing
-00009f40: 5f6d 6574 6164 6174 610a 2020 2020 2020  _metadata.      
-00009f50: 2020 7365 6c66 2e66 696c 6572 733a 204c    self.filers: L
-00009f60: 6973 745b 4669 6c65 725d 203d 2066 696c  ist[Filer] = fil
-00009f70: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
-00009f80: 2e72 6570 6f72 7469 6e67 5f6f 776e 6572  .reporting_owner
-00009f90: 733a 204c 6973 745b 5265 706f 7274 696e  s: List[Reportin
-00009fa0: 674f 776e 6572 5d20 3d20 7265 706f 7274  gOwner] = report
-00009fb0: 696e 675f 6f77 6e65 7273 0a20 2020 2020  ing_owners.     
-00009fc0: 2020 2073 656c 662e 6973 7375 6572 733a     self.issuers:
-00009fd0: 204c 6973 745b 4973 7375 6572 5d20 3d20   List[Issuer] = 
-00009fe0: 6973 7375 6572 730a 2020 2020 2020 2020  issuers.        
-00009ff0: 7365 6c66 2e73 7562 6a65 6374 5f63 6f6d  self.subject_com
-0000a000: 7061 6e69 6573 3a20 4c69 7374 5b53 7562  panies: List[Sub
-0000a010: 6a65 6374 436f 6d70 616e 795d 203d 2073  jectCompany] = s
-0000a020: 7562 6a65 6374 5f63 6f6d 7061 6e69 6573  ubject_companies
-0000a030: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-0000a040: 2020 2020 6465 6620 6163 6365 7373 696f      def accessio
-0000a050: 6e5f 6e75 6d62 6572 2873 656c 6629 3a0a  n_number(self):.
-0000a060: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000a070: 656c 662e 6669 6c69 6e67 5f6d 6574 6164  elf.filing_metad
-0000a080: 6174 612e 6765 7428 2241 4343 4553 5349  ata.get("ACCESSI
-0000a090: 4f4e 204e 554d 4245 5222 290a 0a20 2020  ON NUMBER")..   
-0000a0a0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-0000a0b0: 6566 2066 6f72 6d28 7365 6c66 293a 0a20  ef form(self):. 
-0000a0c0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000a0d0: 6c66 2e66 696c 696e 675f 6d65 7461 6461  lf.filing_metada
-0000a0e0: 7461 2e67 6574 2822 434f 4e46 4f52 4d45  ta.get("CONFORME
-0000a0f0: 4420 5355 424d 4953 5349 4f4e 2054 5950  D SUBMISSION TYP
-0000a100: 4522 290a 0a20 2020 2040 7072 6f70 6572  E")..    @proper
-0000a110: 7479 0a20 2020 2064 6566 2070 6572 696f  ty.    def perio
-0000a120: 645f 6f66 5f72 6570 6f72 7428 7365 6c66  d_of_report(self
-0000a130: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-0000a140: 6e20 7365 6c66 2e66 696c 696e 675f 6d65  n self.filing_me
-0000a150: 7461 6461 7461 2e67 6574 2822 434f 4e46  tadata.get("CONF
-0000a160: 4f52 4d45 4420 5045 5249 4f44 204f 4620  ORMED PERIOD OF 
-0000a170: 5245 504f 5254 2229 0a0a 2020 2020 4070  REPORT")..    @p
-0000a180: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0000a190: 6669 6c69 6e67 5f64 6174 6528 7365 6c66  filing_date(self
-0000a1a0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-0000a1b0: 6e20 7365 6c66 2e66 696c 696e 675f 6d65  n self.filing_me
-0000a1c0: 7461 6461 7461 2e67 6574 2822 4649 4c45  tadata.get("FILE
-0000a1d0: 4420 4153 204f 4620 4441 5445 2229 0a0a  D AS OF DATE")..
-0000a1e0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-0000a1f0: 2020 6465 6620 6461 7465 5f61 735f 6f66    def date_as_of
-0000a200: 5f63 6861 6e67 6528 7365 6c66 293a 0a20  _change(self):. 
-0000a210: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000a220: 6c66 2e66 696c 696e 675f 6d65 7461 6461  lf.filing_metada
-0000a230: 7461 2e67 6574 2822 4441 5445 2041 5320  ta.get("DATE AS 
-0000a240: 4f46 2043 4841 4e47 4522 290a 0a20 2020  OF CHANGE")..   
-0000a250: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-0000a260: 6566 2064 6f63 756d 656e 745f 636f 756e  ef document_coun
-0000a270: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
-0000a280: 2072 6574 7572 6e20 7365 6c66 2e66 696c   return self.fil
-0000a290: 696e 675f 6d65 7461 6461 7461 2e67 6574  ing_metadata.get
-0000a2a0: 2822 5055 424c 4943 2044 4f43 554d 454e  ("PUBLIC DOCUMEN
-0000a2b0: 5420 434f 554e 5422 2c20 3029 0a0a 2020  T COUNT", 0)..  
-0000a2c0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-0000a2d0: 6465 6620 6163 6365 7074 616e 6365 5f64  def acceptance_d
-0000a2e0: 6174 6574 696d 6528 7365 6c66 293a 0a20  atetime(self):. 
-0000a2f0: 2020 2020 2020 2061 6363 6570 7461 6e63         acceptanc
-0000a300: 6520 3d20 7365 6c66 2e66 696c 696e 675f  e = self.filing_
-0000a310: 6d65 7461 6461 7461 2e67 6574 2822 4143  metadata.get("AC
-0000a320: 4345 5054 414e 4345 2d44 4154 4554 494d  CEPTANCE-DATETIM
-0000a330: 4522 290a 2020 2020 2020 2020 6966 2061  E").        if a
-0000a340: 6363 6570 7461 6e63 653a 0a20 2020 2020  cceptance:.     
-0000a350: 2020 2020 2020 2072 6574 7572 6e20 6461         return da
-0000a360: 7465 7469 6d65 2e73 7472 7074 696d 6528  tetime.strptime(
-0000a370: 6163 6365 7074 616e 6365 2c20 2225 5925  acceptance, "%Y%
-0000a380: 6d25 6425 4825 4d25 5322 290a 0a20 2020  m%d%H%M%S")..   
-0000a390: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-0000a3a0: 6566 2066 696c 655f 6e75 6d62 6572 7328  ef file_numbers(
-0000a3b0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-0000a3c0: 2222 5265 7475 726e 2074 6865 2066 696c  ""Return the fil
-0000a3d0: 6520 6e75 6d62 6572 7320 6173 736f 6369  e numbers associ
-0000a3e0: 6174 6564 2077 6974 6820 7468 6973 2066  ated with this f
-0000a3f0: 696c 696e 6722 2222 0a20 2020 2020 2020  iling""".       
-0000a400: 206e 756d 6265 7273 203d 205b 5d0a 2020   numbers = [].  
-0000a410: 2020 2020 2020 6966 2073 656c 662e 6669        if self.fi
-0000a420: 6c65 7273 3a0a 2020 2020 2020 2020 2020  lers:.          
-0000a430: 2020 6e75 6d62 6572 732e 6578 7465 6e64    numbers.extend
-0000a440: 285b 6669 6c65 722e 6669 6c69 6e67 5f69  ([filer.filing_i
-0000a450: 6e66 6f72 6d61 7469 6f6e 2e66 696c 655f  nformation.file_
-0000a460: 6e75 6d62 6572 2066 6f72 2066 696c 6572  number for filer
-0000a470: 2069 6e20 7365 6c66 2e66 696c 6572 735d   in self.filers]
-0000a480: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0000a490: 662e 7265 706f 7274 696e 675f 6f77 6e65  f.reporting_owne
-0000a4a0: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
-0000a4b0: 6e75 6d62 6572 732e 6578 7465 6e64 280a  numbers.extend(.
-0000a4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4d0: 5b72 6570 6f72 7469 6e67 5f6f 776e 6572  [reporting_owner
-0000a4e0: 2e66 696c 696e 675f 696e 666f 726d 6174  .filing_informat
-0000a4f0: 696f 6e2e 6669 6c65 5f6e 756d 6265 7220  ion.file_number 
-0000a500: 666f 7220 7265 706f 7274 696e 675f 6f77  for reporting_ow
-0000a510: 6e65 7220 696e 2073 656c 662e 7265 706f  ner in self.repo
-0000a520: 7274 696e 675f 6f77 6e65 7273 5d29 0a20  rting_owners]). 
-0000a530: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-0000a540: 7562 6a65 6374 5f63 6f6d 7061 6e69 6573  ubject_companies
-0000a550: 3a0a 2020 2020 2020 2020 2020 2020 6e75  :.            nu
-0000a560: 6d62 6572 732e 6578 7465 6e64 280a 2020  mbers.extend(.  
-0000a570: 2020 2020 2020 2020 2020 2020 2020 5b73                [s
-0000a580: 7562 6a65 6374 5f63 6f6d 7061 6e79 2e66  ubject_company.f
-0000a590: 696c 696e 675f 696e 666f 726d 6174 696f  iling_informatio
-0000a5a0: 6e2e 6669 6c65 5f6e 756d 6265 7220 666f  n.file_number fo
-0000a5b0: 7220 7375 626a 6563 745f 636f 6d70 616e  r subject_compan
-0000a5c0: 7920 696e 2073 656c 662e 7375 626a 6563  y in self.subjec
-0000a5d0: 745f 636f 6d70 616e 6965 735d 290a 2020  t_companies]).  
-0000a5e0: 2020 2020 2020 7265 7475 726e 206c 6973        return lis
-0000a5f0: 7428 7365 7428 6e75 6d62 6572 7329 290a  t(set(numbers)).
-0000a600: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-0000a610: 640a 2020 2020 6465 6620 7061 7273 6528  d.    def parse(
-0000a620: 636c 732c 2068 6561 6465 725f 7465 7874  cls, header_text
-0000a630: 3a20 7374 7229 3a0a 2020 2020 2020 2020  : str):.        
-0000a640: 6461 7461 203d 207b 7d0a 2020 2020 2020  data = {}.      
-0000a650: 2020 6375 7272 656e 745f 6865 6164 6572    current_header
-0000a660: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-0000a670: 6375 7272 656e 745f 7375 6268 6561 6465  current_subheade
-0000a680: 7220 3d20 4e6f 6e65 0a0a 2020 2020 2020  r = None..      
-0000a690: 2020 2320 5265 6164 2074 6865 206c 696e    # Read the lin
-0000a6a0: 6573 2069 6e20 7468 6520 636f 6e74 656e  es in the conten
-0000a6b0: 742e 2054 6869 7320 7374 6172 7473 2077  t. This starts w
-0000a6c0: 6974 6820 3c41 4343 4550 5441 4e43 452d  ith <ACCEPTANCE-
-0000a6d0: 4441 5445 5449 4d45 3e32 3032 3330 3630  DATETIME>2023060
-0000a6e0: 3632 3133 3230 340a 2020 2020 2020 2020  6213204.        
-0000a6f0: 6c69 6e65 7320 3d20 6865 6164 6572 5f74  lines = header_t
-0000a700: 6578 742e 7370 6c69 7428 275c 6e27 290a  ext.split('\n').
-0000a710: 2020 2020 2020 2020 666f 7220 696e 6465          for inde
-0000a720: 782c 206c 696e 6520 696e 2065 6e75 6d65  x, line in enume
-0000a730: 7261 7465 2868 6561 6465 725f 7465 7874  rate(header_text
-0000a740: 2e73 706c 6974 2827 5c6e 2729 293a 0a20  .split('\n')):. 
-0000a750: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-0000a760: 7420 6c69 6e65 3a0a 2020 2020 2020 2020  t line:.        
-0000a770: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-0000a780: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0000a790: 4b65 6570 2074 7261 636b 206f 6620 7468  Keep track of th
-0000a7a0: 6520 6e65 7374 696e 6720 6c65 7665 6c0a  e nesting level.
-0000a7b0: 2020 2020 2020 2020 2020 2020 6e65 7374              nest
-0000a7c0: 696e 675f 6c65 7665 6c20 3d20 6c65 6e28  ing_level = len(
-0000a7d0: 6c69 6e65 2920 2d20 6c65 6e28 6c69 6e65  line) - len(line
-0000a7e0: 2e6c 7374 7269 7028 275c 7427 2929 0a0a  .lstrip('\t'))..
-0000a7f0: 2020 2020 2020 2020 2020 2020 2320 4e65              # Ne
-0000a800: 7374 6564 2069 6e63 7265 6173 6573 0a20  sted increases. 
-0000a810: 2020 2020 2020 2020 2020 206e 6573 7469             nesti
-0000a820: 6e67 5f77 696c 6c5f 696e 6372 6561 7365  ng_will_increase
-0000a830: 203d 2069 6e64 6578 203c 206c 656e 286c   = index < len(l
-0000a840: 696e 6573 2920 2d20 3120 616e 6420 6e65  ines) - 1 and ne
-0000a850: 7374 696e 675f 6c65 7665 6c20 3c20 6c65  sting_level < le
-0000a860: 6e28 6c69 6e65 735b 696e 6465 7820 2b20  n(lines[index + 
-0000a870: 315d 2920 2d20 6c65 6e28 0a20 2020 2020  1]) - len(.     
-0000a880: 2020 2020 2020 2020 2020 206c 696e 6573             lines
-0000a890: 5b69 6e64 6578 202b 2031 5d2e 6c73 7472  [index + 1].lstr
-0000a8a0: 6970 2827 5c74 2729 290a 0a20 2020 2020  ip('\t'))..     
-0000a8b0: 2020 2020 2020 2023 2054 6865 206c 696e         # The lin
-0000a8c0: 6520 656e 6473 2077 6974 6820 6120 273a  e ends with a ':
-0000a8d0: 2720 6d65 616e 696e 6720 6e65 7374 6564  ' meaning nested
-0000a8e0: 2063 6f6e 7465 6e74 2066 6f6c 6c6f 7773   content follows
-0000a8f0: 2065 2e67 2e20 2252 4550 4f52 5449 4e47   e.g. "REPORTING
-0000a900: 2d4f 574e 4552 3a22 0a20 2020 2020 2020  -OWNER:".       
-0000a910: 2020 2020 206c 696e 655f 656e 6473 5f77       line_ends_w
-0000a920: 6974 685f 636f 6c6f 6e20 3d20 6c69 6e65  ith_colon = line
-0000a930: 2e72 7374 7269 7028 275c 7427 292e 656e  .rstrip('\t').en
-0000a940: 6473 7769 7468 2827 3a27 290a 0a20 2020  dswith(':')..   
-0000a950: 2020 2020 2020 2020 2069 735f 6865 6164           is_head
-0000a960: 6572 203d 2028 6e65 7374 696e 675f 6c65  er = (nesting_le
-0000a970: 7665 6c20 3d3d 2030 2061 6e64 206c 696e  vel == 0 and lin
-0000a980: 655f 656e 6473 5f77 6974 685f 636f 6c6f  e_ends_with_colo
-0000a990: 6e29 206f 7220 6e65 7374 696e 675f 7769  n) or nesting_wi
-0000a9a0: 6c6c 5f69 6e63 7265 6173 650a 2020 2020  ll_increase.    
-0000a9b0: 2020 2020 2020 2020 6966 2069 735f 6865          if is_he
-0000a9c0: 6164 6572 3a0a 2020 2020 2020 2020 2020  ader:.          
-0000a9d0: 2020 2020 2020 2320 4e65 7374 6564 206c        # Nested l
-0000a9e0: 696e 6520 6d65 616e 7320 6120 7375 6268  ine means a subh
-0000a9f0: 6561 6465 7220 652e 672e 2022 4f57 4e45  eader e.g. "OWNE
-0000aa00: 5220 4441 5441 3a22 0a20 2020 2020 2020  R DATA:".       
-0000aa10: 2020 2020 2020 2020 2069 6620 6c69 6e65           if line
-0000aa20: 2e73 7461 7274 7377 6974 6828 275c 7427  .startswith('\t'
-0000aa30: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000aa40: 2020 2020 2020 2063 7572 7265 6e74 5f73         current_s
-0000aa50: 7562 6865 6164 6572 203d 206c 696e 652e  ubheader = line.
-0000aa60: 7374 7269 7028 292e 7370 6c69 7428 273a  strip().split(':
-0000aa70: 2729 5b30 5d0a 2020 2020 2020 2020 2020  ')[0].          
-0000aa80: 2020 2020 2020 2020 2020 6966 2063 7572            if cur
-0000aa90: 7265 6e74 5f73 7562 6865 6164 6572 203d  rent_subheader =
-0000aaa0: 3d20 2246 4f52 4d45 5220 434f 4d50 414e  = "FORMER COMPAN
-0000aab0: 5922 3a20 2023 2053 7065 6369 616c 2063  Y":  # Special c
-0000aac0: 6173 652e 2054 6869 7320 6973 2061 206c  ase. This is a l
-0000aad0: 6973 7420 6f66 2063 6f6d 7061 6e69 6573  ist of companies
-0000aae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000aaf0: 2020 2020 2020 2020 2069 6620 6375 7272           if curr
-0000ab00: 656e 745f 7375 6268 6561 6465 7220 6e6f  ent_subheader no
-0000ab10: 7420 696e 2064 6174 615b 6375 7272 656e  t in data[curren
-0000ab20: 745f 6865 6164 6572 5d5b 2d31 5d3a 0a20  t_header][-1]:. 
-0000ab30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab40: 2020 2020 2020 2020 2020 2064 6174 615b             data[
-0000ab50: 6375 7272 656e 745f 6865 6164 6572 5d5b  current_header][
-0000ab60: 2d31 5d5b 6375 7272 656e 745f 7375 6268  -1][current_subh
-0000ab70: 6561 6465 725d 203d 205b 5d0a 2020 2020  eader] = [].    
-0000ab80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab90: 2020 2020 6461 7461 5b63 7572 7265 6e74      data[current
-0000aba0: 5f68 6561 6465 725d 5b2d 315d 5b63 7572  _header][-1][cur
-0000abb0: 7265 6e74 5f73 7562 6865 6164 6572 5d2e  rent_subheader].
-0000abc0: 6170 7065 6e64 287b 7d29 0a20 2020 2020  append({}).     
-0000abd0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000abe0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000abf0: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-0000ac00: 615b 6375 7272 656e 745f 6865 6164 6572  a[current_header
-0000ac10: 5d5b 2d31 5d5b 6375 7272 656e 745f 7375  ][-1][current_su
-0000ac20: 6268 6561 6465 725d 203d 207b 7d20 2023  bheader] = {}  #
-0000ac30: 2045 7870 6563 7420 6f6e 6c79 206f 6e65   Expect only one
-0000ac40: 2072 6563 6f72 6420 7065 7220 6b65 790a   record per key.
-0000ac50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ac60: 2023 2054 6f70 206c 6576 656c 2068 6561   # Top level hea
-0000ac70: 6465 720a 2020 2020 2020 2020 2020 2020  der.            
-0000ac80: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000ac90: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-0000aca0: 7272 656e 745f 6865 6164 6572 203d 206c  rrent_header = l
-0000acb0: 696e 652e 7374 7269 7028 292e 7370 6c69  ine.strip().spli
-0000acc0: 7428 273a 2729 5b30 5d0a 2020 2020 2020  t(':')[0].      
-0000acd0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000ace0: 2063 7572 7265 6e74 5f68 6561 6465 7220   current_header 
-0000acf0: 6e6f 7420 696e 2064 6174 613a 0a20 2020  not in data:.   
-0000ad00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad10: 2020 2020 2064 6174 615b 6375 7272 656e       data[curren
-0000ad20: 745f 6865 6164 6572 5d20 3d20 5b5d 0a20  t_header] = []. 
-0000ad30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad40: 2020 2064 6174 615b 6375 7272 656e 745f     data[current_
-0000ad50: 6865 6164 6572 5d2e 6170 7065 6e64 287b  header].append({
-0000ad60: 7d29 0a20 2020 2020 2020 2020 2020 2065  }).            e
-0000ad70: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000ad80: 2020 2020 2069 6620 6c69 6e65 2e73 7472       if line.str
-0000ad90: 6970 2829 2e73 7461 7274 7377 6974 6828  ip().startswith(
-0000ada0: 223c 2229 3a0a 2020 2020 2020 2020 2020  "<"):.          
-0000adb0: 2020 2020 2020 2020 2020 2320 5468 6520            # The 
-0000adc0: 6c69 6e65 206c 6f6f 6b73 206c 696b 6520  line looks like 
-0000add0: 7468 6973 203c 4b45 593e 5641 4c55 450a  this <KEY>VALUE.
-0000ade0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000adf0: 2020 2020 6b65 792c 2076 616c 7565 203d      key, value =
-0000ae00: 206c 696e 652e 7370 6c69 7428 273e 2729   line.split('>')
-0000ae10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ae20: 2020 2020 2023 2053 7472 6970 2074 6865       # Strip the
-0000ae30: 206c 6561 6469 6e67 2027 3c27 2066 726f   leading '<' fro
-0000ae40: 6d20 7468 6520 6b65 790a 2020 2020 2020  m the key.      
-0000ae50: 2020 2020 2020 2020 2020 2020 2020 6461                da
-0000ae60: 7461 5b6b 6579 5b31 3a5d 5d20 3d20 7661  ta[key[1:]] = va
-0000ae70: 6c75 650a 2020 2020 2020 2020 2020 2020  lue.            
-0000ae80: 2020 2020 656c 6966 2027 3a27 2069 6e20      elif ':' in 
-0000ae90: 6c69 6e65 3a0a 2020 2020 2020 2020 2020  line:.          
-0000aea0: 2020 2020 2020 2020 2020 7061 7274 7320            parts 
-0000aeb0: 3d20 6c69 6e65 2e73 7472 6970 2829 2e73  = line.strip().s
-0000aec0: 706c 6974 2827 3a27 290a 2020 2020 2020  plit(':').      
-0000aed0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000aee0: 206c 656e 2870 6172 7473 2920 3d3d 2032   len(parts) == 2
-0000aef0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000af00: 2020 2020 2020 2020 2020 6b65 792c 2076            key, v
-0000af10: 616c 7565 203d 206c 696e 652e 7374 7269  alue = line.stri
-0000af20: 7028 292e 7370 6c69 7428 273a 2729 0a20  p().split(':'). 
-0000af30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af40: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00009c50: 2020 2020 2020 2020 2020 2020 6d61 696c              mail
+00009c60: 696e 675f 6164 6472 6573 732e 6369 7479  ing_address.city
+00009c70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00009c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c90: 6d61 696c 696e 675f 6164 6472 6573 732e  mailing_address.
+00009ca0: 7374 6174 655f 6f72 5f63 6f75 6e74 7279  state_or_country
+00009cb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00009cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009cd0: 6d61 696c 696e 675f 6164 6472 6573 732e  mailing_address.
+00009ce0: 7a69 7063 6f64 6529 0a20 2020 2072 6574  zipcode).    ret
+00009cf0: 7572 6e20 6164 6472 6573 735f 7461 626c  urn address_tabl
+00009d00: 650a 0a0a 636c 6173 7320 5345 4348 6561  e...class SECHea
+00009d10: 6465 723a 0a20 2020 2022 2222 0a20 2020  der:.    """.   
+00009d20: 2043 6f6e 7461 696e 7320 7468 6520 7061   Contains the pa
+00009d30: 7273 6564 2072 6570 7265 7365 6e74 6174  rsed representat
+00009d40: 696f 6e20 6f66 2074 6865 2053 4543 2d48  ion of the SEC-H
+00009d50: 4541 4445 5220 7465 7874 2061 7420 7468  EADER text at th
+00009d60: 6520 746f 7020 6f66 2074 6865 2066 756c  e top of the ful
+00009d70: 6c20 7375 626d 6973 7369 6f6e 2074 6578  l submission tex
+00009d80: 740a 2020 2020 3c53 4543 2d48 4541 4445  t.    <SEC-HEADE
+00009d90: 523e 0a0a 2020 2020 3c2f 5345 432d 4845  R>..    </SEC-HE
+00009da0: 4144 4552 3e0a 2020 2020 2222 220a 0a20  ADER>.    """.. 
+00009db0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00009dc0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+00009dd0: 2020 2020 2020 2074 6578 743a 2073 7472         text: str
+00009de0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00009df0: 2020 2066 696c 696e 675f 6d65 7461 6461     filing_metada
+00009e00: 7461 3a20 4469 6374 5b73 7472 2c20 7374  ta: Dict[str, st
+00009e10: 725d 2c0a 2020 2020 2020 2020 2020 2020  r],.            
+00009e20: 2020 2020 2066 696c 6572 733a 204c 6973       filers: Lis
+00009e30: 745b 4669 6c65 725d 203d 204e 6f6e 652c  t[Filer] = None,
+00009e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009e50: 2020 7265 706f 7274 696e 675f 6f77 6e65    reporting_owne
+00009e60: 7273 3a20 4c69 7374 5b52 6570 6f72 7469  rs: List[Reporti
+00009e70: 6e67 4f77 6e65 725d 203d 204e 6f6e 652c  ngOwner] = None,
+00009e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009e90: 2020 6973 7375 6572 733a 204c 6973 745b    issuers: List[
+00009ea0: 4973 7375 6572 5d20 3d20 4e6f 6e65 2c0a  Issuer] = None,.
+00009eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ec0: 2073 7562 6a65 6374 5f63 6f6d 7061 6e69   subject_compani
+00009ed0: 6573 3a20 4c69 7374 5b53 7562 6a65 6374  es: List[Subject
+00009ee0: 436f 6d70 616e 795d 203d 204e 6f6e 6529  Company] = None)
+00009ef0: 3a0a 2020 2020 2020 2020 7365 6c66 2e74  :.        self.t
+00009f00: 6578 743a 2073 7472 203d 2074 6578 740a  ext: str = text.
+00009f10: 2020 2020 2020 2020 7365 6c66 2e66 696c          self.fil
+00009f20: 696e 675f 6d65 7461 6461 7461 3a20 4469  ing_metadata: Di
+00009f30: 6374 5b73 7472 2c20 7374 725d 203d 2066  ct[str, str] = f
+00009f40: 696c 696e 675f 6d65 7461 6461 7461 0a20  iling_metadata. 
+00009f50: 2020 2020 2020 2073 656c 662e 6669 6c65         self.file
+00009f60: 7273 3a20 4c69 7374 5b46 696c 6572 5d20  rs: List[Filer] 
+00009f70: 3d20 6669 6c65 7273 0a20 2020 2020 2020  = filers.       
+00009f80: 2073 656c 662e 7265 706f 7274 696e 675f   self.reporting_
+00009f90: 6f77 6e65 7273 3a20 4c69 7374 5b52 6570  owners: List[Rep
+00009fa0: 6f72 7469 6e67 4f77 6e65 725d 203d 2072  ortingOwner] = r
+00009fb0: 6570 6f72 7469 6e67 5f6f 776e 6572 730a  eporting_owners.
+00009fc0: 2020 2020 2020 2020 7365 6c66 2e69 7373          self.iss
+00009fd0: 7565 7273 3a20 4c69 7374 5b49 7373 7565  uers: List[Issue
+00009fe0: 725d 203d 2069 7373 7565 7273 0a20 2020  r] = issuers.   
+00009ff0: 2020 2020 2073 656c 662e 7375 626a 6563       self.subjec
+0000a000: 745f 636f 6d70 616e 6965 733a 204c 6973  t_companies: Lis
+0000a010: 745b 5375 626a 6563 7443 6f6d 7061 6e79  t[SubjectCompany
+0000a020: 5d20 3d20 7375 626a 6563 745f 636f 6d70  ] = subject_comp
+0000a030: 616e 6965 730a 0a20 2020 2040 7072 6f70  anies..    @prop
+0000a040: 6572 7479 0a20 2020 2064 6566 2061 6363  erty.    def acc
+0000a050: 6573 7369 6f6e 5f6e 756d 6265 7228 7365  ession_number(se
+0000a060: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
+0000a070: 7572 6e20 7365 6c66 2e66 696c 696e 675f  urn self.filing_
+0000a080: 6d65 7461 6461 7461 2e67 6574 2822 4143  metadata.get("AC
+0000a090: 4345 5353 494f 4e20 4e55 4d42 4552 2229  CESSION NUMBER")
+0000a0a0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0000a0b0: 2020 2020 6465 6620 666f 726d 2873 656c      def form(sel
+0000a0c0: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
+0000a0d0: 726e 2073 656c 662e 6669 6c69 6e67 5f6d  rn self.filing_m
+0000a0e0: 6574 6164 6174 612e 6765 7428 2243 4f4e  etadata.get("CON
+0000a0f0: 464f 524d 4544 2053 5542 4d49 5353 494f  FORMED SUBMISSIO
+0000a100: 4e20 5459 5045 2229 0a0a 2020 2020 4070  N TYPE")..    @p
+0000a110: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+0000a120: 7065 7269 6f64 5f6f 665f 7265 706f 7274  period_of_report
+0000a130: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000a140: 7265 7475 726e 2073 656c 662e 6669 6c69  return self.fili
+0000a150: 6e67 5f6d 6574 6164 6174 612e 6765 7428  ng_metadata.get(
+0000a160: 2243 4f4e 464f 524d 4544 2050 4552 494f  "CONFORMED PERIO
+0000a170: 4420 4f46 2052 4550 4f52 5422 290a 0a20  D OF REPORT").. 
+0000a180: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+0000a190: 2064 6566 2066 696c 696e 675f 6461 7465   def filing_date
+0000a1a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000a1b0: 7265 7475 726e 2073 656c 662e 6669 6c69  return self.fili
+0000a1c0: 6e67 5f6d 6574 6164 6174 612e 6765 7428  ng_metadata.get(
+0000a1d0: 2246 494c 4544 2041 5320 4f46 2044 4154  "FILED AS OF DAT
+0000a1e0: 4522 290a 0a20 2020 2040 7072 6f70 6572  E")..    @proper
+0000a1f0: 7479 0a20 2020 2064 6566 2064 6174 655f  ty.    def date_
+0000a200: 6173 5f6f 665f 6368 616e 6765 2873 656c  as_of_change(sel
+0000a210: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
+0000a220: 726e 2073 656c 662e 6669 6c69 6e67 5f6d  rn self.filing_m
+0000a230: 6574 6164 6174 612e 6765 7428 2244 4154  etadata.get("DAT
+0000a240: 4520 4153 204f 4620 4348 414e 4745 2229  E AS OF CHANGE")
+0000a250: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0000a260: 2020 2020 6465 6620 646f 6375 6d65 6e74      def document
+0000a270: 5f63 6f75 6e74 2873 656c 6629 3a0a 2020  _count(self):.  
+0000a280: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000a290: 662e 6669 6c69 6e67 5f6d 6574 6164 6174  f.filing_metadat
+0000a2a0: 612e 6765 7428 2250 5542 4c49 4320 444f  a.get("PUBLIC DO
+0000a2b0: 4355 4d45 4e54 2043 4f55 4e54 222c 2030  CUMENT COUNT", 0
+0000a2c0: 290a 0a20 2020 2040 7072 6f70 6572 7479  )..    @property
+0000a2d0: 0a20 2020 2064 6566 2061 6363 6570 7461  .    def accepta
+0000a2e0: 6e63 655f 6461 7465 7469 6d65 2873 656c  nce_datetime(sel
+0000a2f0: 6629 3a0a 2020 2020 2020 2020 6163 6365  f):.        acce
+0000a300: 7074 616e 6365 203d 2073 656c 662e 6669  ptance = self.fi
+0000a310: 6c69 6e67 5f6d 6574 6164 6174 612e 6765  ling_metadata.ge
+0000a320: 7428 2241 4343 4550 5441 4e43 452d 4441  t("ACCEPTANCE-DA
+0000a330: 5445 5449 4d45 2229 0a20 2020 2020 2020  TETIME").       
+0000a340: 2069 6620 6163 6365 7074 616e 6365 3a0a   if acceptance:.
+0000a350: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000a360: 726e 2064 6174 6574 696d 652e 7374 7270  rn datetime.strp
+0000a370: 7469 6d65 2861 6363 6570 7461 6e63 652c  time(acceptance,
+0000a380: 2022 2559 256d 2564 2548 254d 2553 2229   "%Y%m%d%H%M%S")
+0000a390: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0000a3a0: 2020 2020 6465 6620 6669 6c65 5f6e 756d      def file_num
+0000a3b0: 6265 7273 2873 656c 6629 3a0a 2020 2020  bers(self):.    
+0000a3c0: 2020 2020 2222 2252 6574 7572 6e20 7468      """Return th
+0000a3d0: 6520 6669 6c65 206e 756d 6265 7273 2061  e file numbers a
+0000a3e0: 7373 6f63 6961 7465 6420 7769 7468 2074  ssociated with t
+0000a3f0: 6869 7320 6669 6c69 6e67 2222 220a 2020  his filing""".  
+0000a400: 2020 2020 2020 6e75 6d62 6572 7320 3d20        numbers = 
+0000a410: 5b5d 0a20 2020 2020 2020 2069 6620 7365  [].        if se
+0000a420: 6c66 2e66 696c 6572 733a 0a20 2020 2020  lf.filers:.     
+0000a430: 2020 2020 2020 206e 756d 6265 7273 2e65         numbers.e
+0000a440: 7874 656e 6428 5b66 696c 6572 2e66 696c  xtend([filer.fil
+0000a450: 696e 675f 696e 666f 726d 6174 696f 6e2e  ing_information.
+0000a460: 6669 6c65 5f6e 756d 6265 7220 666f 7220  file_number for 
+0000a470: 6669 6c65 7220 696e 2073 656c 662e 6669  filer in self.fi
+0000a480: 6c65 7273 5d29 0a20 2020 2020 2020 2069  lers]).        i
+0000a490: 6620 7365 6c66 2e72 6570 6f72 7469 6e67  f self.reporting
+0000a4a0: 5f6f 776e 6572 733a 0a20 2020 2020 2020  _owners:.       
+0000a4b0: 2020 2020 206e 756d 6265 7273 2e65 7874       numbers.ext
+0000a4c0: 656e 6428 0a20 2020 2020 2020 2020 2020  end(.           
+0000a4d0: 2020 2020 205b 7265 706f 7274 696e 675f       [reporting_
+0000a4e0: 6f77 6e65 722e 6669 6c69 6e67 5f69 6e66  owner.filing_inf
+0000a4f0: 6f72 6d61 7469 6f6e 2e66 696c 655f 6e75  ormation.file_nu
+0000a500: 6d62 6572 2066 6f72 2072 6570 6f72 7469  mber for reporti
+0000a510: 6e67 5f6f 776e 6572 2069 6e20 7365 6c66  ng_owner in self
+0000a520: 2e72 6570 6f72 7469 6e67 5f6f 776e 6572  .reporting_owner
+0000a530: 735d 290a 2020 2020 2020 2020 6966 2073  s]).        if s
+0000a540: 656c 662e 7375 626a 6563 745f 636f 6d70  elf.subject_comp
+0000a550: 616e 6965 733a 0a20 2020 2020 2020 2020  anies:.         
+0000a560: 2020 206e 756d 6265 7273 2e65 7874 656e     numbers.exten
+0000a570: 6428 0a20 2020 2020 2020 2020 2020 2020  d(.             
+0000a580: 2020 205b 7375 626a 6563 745f 636f 6d70     [subject_comp
+0000a590: 616e 792e 6669 6c69 6e67 5f69 6e66 6f72  any.filing_infor
+0000a5a0: 6d61 7469 6f6e 2e66 696c 655f 6e75 6d62  mation.file_numb
+0000a5b0: 6572 2066 6f72 2073 7562 6a65 6374 5f63  er for subject_c
+0000a5c0: 6f6d 7061 6e79 2069 6e20 7365 6c66 2e73  ompany in self.s
+0000a5d0: 7562 6a65 6374 5f63 6f6d 7061 6e69 6573  ubject_companies
+0000a5e0: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
+0000a5f0: 6e20 6c69 7374 2873 6574 286e 756d 6265  n list(set(numbe
+0000a600: 7273 2929 0a0a 2020 2020 4063 6c61 7373  rs))..    @class
+0000a610: 6d65 7468 6f64 0a20 2020 2064 6566 2070  method.    def p
+0000a620: 6172 7365 2863 6c73 2c20 6865 6164 6572  arse(cls, header
+0000a630: 5f74 6578 743a 2073 7472 293a 0a20 2020  _text: str):.   
+0000a640: 2020 2020 2064 6174 6120 3d20 7b7d 0a20       data = {}. 
+0000a650: 2020 2020 2020 2063 7572 7265 6e74 5f68         current_h
+0000a660: 6561 6465 7220 3d20 4e6f 6e65 0a20 2020  eader = None.   
+0000a670: 2020 2020 2063 7572 7265 6e74 5f73 7562       current_sub
+0000a680: 6865 6164 6572 203d 204e 6f6e 650a 0a20  header = None.. 
+0000a690: 2020 2020 2020 2023 2052 6561 6420 7468         # Read th
+0000a6a0: 6520 6c69 6e65 7320 696e 2074 6865 2063  e lines in the c
+0000a6b0: 6f6e 7465 6e74 2e20 5468 6973 2073 7461  ontent. This sta
+0000a6c0: 7274 7320 7769 7468 203c 4143 4345 5054  rts with <ACCEPT
+0000a6d0: 414e 4345 2d44 4154 4554 494d 453e 3230  ANCE-DATETIME>20
+0000a6e0: 3233 3036 3036 3231 3332 3034 0a20 2020  230606213204.   
+0000a6f0: 2020 2020 206c 696e 6573 203d 2068 6561       lines = hea
+0000a700: 6465 725f 7465 7874 2e73 706c 6974 2827  der_text.split('
+0000a710: 5c6e 2729 0a20 2020 2020 2020 2066 6f72  \n').        for
+0000a720: 2069 6e64 6578 2c20 6c69 6e65 2069 6e20   index, line in 
+0000a730: 656e 756d 6572 6174 6528 6865 6164 6572  enumerate(header
+0000a740: 5f74 6578 742e 7370 6c69 7428 275c 6e27  _text.split('\n'
+0000a750: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+0000a760: 6966 206e 6f74 206c 696e 653a 0a20 2020  if not line:.   
+0000a770: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+0000a780: 7469 6e75 650a 0a20 2020 2020 2020 2020  tinue..         
+0000a790: 2020 2023 204b 6565 7020 7472 6163 6b20     # Keep track 
+0000a7a0: 6f66 2074 6865 206e 6573 7469 6e67 206c  of the nesting l
+0000a7b0: 6576 656c 0a20 2020 2020 2020 2020 2020  evel.           
+0000a7c0: 206e 6573 7469 6e67 5f6c 6576 656c 203d   nesting_level =
+0000a7d0: 206c 656e 286c 696e 6529 202d 206c 656e   len(line) - len
+0000a7e0: 286c 696e 652e 6c73 7472 6970 2827 5c74  (line.lstrip('\t
+0000a7f0: 2729 290a 0a20 2020 2020 2020 2020 2020  '))..           
+0000a800: 2023 204e 6573 7465 6420 696e 6372 6561   # Nested increa
+0000a810: 7365 730a 2020 2020 2020 2020 2020 2020  ses.            
+0000a820: 6e65 7374 696e 675f 7769 6c6c 5f69 6e63  nesting_will_inc
+0000a830: 7265 6173 6520 3d20 696e 6465 7820 3c20  rease = index < 
+0000a840: 6c65 6e28 6c69 6e65 7329 202d 2031 2061  len(lines) - 1 a
+0000a850: 6e64 206e 6573 7469 6e67 5f6c 6576 656c  nd nesting_level
+0000a860: 203c 206c 656e 286c 696e 6573 5b69 6e64   < len(lines[ind
+0000a870: 6578 202b 2031 5d29 202d 206c 656e 280a  ex + 1]) - len(.
+0000a880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a890: 6c69 6e65 735b 696e 6465 7820 2b20 315d  lines[index + 1]
+0000a8a0: 2e6c 7374 7269 7028 275c 7427 2929 0a0a  .lstrip('\t'))..
+0000a8b0: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
+0000a8c0: 6520 6c69 6e65 2065 6e64 7320 7769 7468  e line ends with
+0000a8d0: 2061 2027 3a27 206d 6561 6e69 6e67 206e   a ':' meaning n
+0000a8e0: 6573 7465 6420 636f 6e74 656e 7420 666f  ested content fo
+0000a8f0: 6c6c 6f77 7320 652e 672e 2022 5245 504f  llows e.g. "REPO
+0000a900: 5254 494e 472d 4f57 4e45 523a 220a 2020  RTING-OWNER:".  
+0000a910: 2020 2020 2020 2020 2020 6c69 6e65 5f65            line_e
+0000a920: 6e64 735f 7769 7468 5f63 6f6c 6f6e 203d  nds_with_colon =
+0000a930: 206c 696e 652e 7273 7472 6970 2827 5c74   line.rstrip('\t
+0000a940: 2729 2e65 6e64 7377 6974 6828 273a 2729  ').endswith(':')
+0000a950: 0a0a 2020 2020 2020 2020 2020 2020 6973  ..            is
+0000a960: 5f68 6561 6465 7220 3d20 286e 6573 7469  _header = (nesti
+0000a970: 6e67 5f6c 6576 656c 203d 3d20 3020 616e  ng_level == 0 an
+0000a980: 6420 6c69 6e65 5f65 6e64 735f 7769 7468  d line_ends_with
+0000a990: 5f63 6f6c 6f6e 2920 6f72 206e 6573 7469  _colon) or nesti
+0000a9a0: 6e67 5f77 696c 6c5f 696e 6372 6561 7365  ng_will_increase
+0000a9b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000a9c0: 6973 5f68 6561 6465 723a 0a20 2020 2020  is_header:.     
+0000a9d0: 2020 2020 2020 2020 2020 2023 204e 6573             # Nes
+0000a9e0: 7465 6420 6c69 6e65 206d 6561 6e73 2061  ted line means a
+0000a9f0: 2073 7562 6865 6164 6572 2065 2e67 2e20   subheader e.g. 
+0000aa00: 224f 574e 4552 2044 4154 413a 220a 2020  "OWNER DATA:".  
+0000aa10: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000aa20: 206c 696e 652e 7374 6172 7473 7769 7468   line.startswith
+0000aa30: 2827 5c74 2729 3a0a 2020 2020 2020 2020  ('\t'):.        
+0000aa40: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+0000aa50: 656e 745f 7375 6268 6561 6465 7220 3d20  ent_subheader = 
+0000aa60: 6c69 6e65 2e73 7472 6970 2829 2e73 706c  line.strip().spl
+0000aa70: 6974 2827 3a27 295b 305d 0a20 2020 2020  it(':')[0].     
+0000aa80: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000aa90: 6620 6375 7272 656e 745f 7375 6268 6561  f current_subhea
+0000aaa0: 6465 7220 3d3d 2022 464f 524d 4552 2043  der == "FORMER C
+0000aab0: 4f4d 5041 4e59 223a 2020 2320 5370 6563  OMPANY":  # Spec
+0000aac0: 6961 6c20 6361 7365 2e20 5468 6973 2069  ial case. This i
+0000aad0: 7320 6120 6c69 7374 206f 6620 636f 6d70  s a list of comp
+0000aae0: 616e 6965 730a 2020 2020 2020 2020 2020  anies.          
+0000aaf0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000ab00: 2063 7572 7265 6e74 5f73 7562 6865 6164   current_subhead
+0000ab10: 6572 206e 6f74 2069 6e20 6461 7461 5b63  er not in data[c
+0000ab20: 7572 7265 6e74 5f68 6561 6465 725d 5b2d  urrent_header][-
+0000ab30: 315d 3a0a 2020 2020 2020 2020 2020 2020  1]:.            
+0000ab40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab50: 6461 7461 5b63 7572 7265 6e74 5f68 6561  data[current_hea
+0000ab60: 6465 725d 5b2d 315d 5b63 7572 7265 6e74  der][-1][current
+0000ab70: 5f73 7562 6865 6164 6572 5d20 3d20 5b5d  _subheader] = []
+0000ab80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ab90: 2020 2020 2020 2020 2064 6174 615b 6375           data[cu
+0000aba0: 7272 656e 745f 6865 6164 6572 5d5b 2d31  rrent_header][-1
+0000abb0: 5d5b 6375 7272 656e 745f 7375 6268 6561  ][current_subhea
+0000abc0: 6465 725d 2e61 7070 656e 6428 7b7d 290a  der].append({}).
+0000abd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abe0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000abf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac00: 2020 6461 7461 5b63 7572 7265 6e74 5f68    data[current_h
+0000ac10: 6561 6465 725d 5b2d 315d 5b63 7572 7265  eader][-1][curre
+0000ac20: 6e74 5f73 7562 6865 6164 6572 5d20 3d20  nt_subheader] = 
+0000ac30: 7b7d 2020 2320 4578 7065 6374 206f 6e6c  {}  # Expect onl
+0000ac40: 7920 6f6e 6520 7265 636f 7264 2070 6572  y one record per
+0000ac50: 206b 6579 0a0a 2020 2020 2020 2020 2020   key..          
+0000ac60: 2020 2020 2020 2320 546f 7020 6c65 7665        # Top leve
+0000ac70: 6c20 6865 6164 6572 0a20 2020 2020 2020  l header.       
+0000ac80: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aca0: 2020 2063 7572 7265 6e74 5f68 6561 6465     current_heade
+0000acb0: 7220 3d20 6c69 6e65 2e73 7472 6970 2829  r = line.strip()
+0000acc0: 2e73 706c 6974 2827 3a27 295b 305d 0a20  .split(':')[0]. 
+0000acd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ace0: 2020 2069 6620 6375 7272 656e 745f 6865     if current_he
+0000acf0: 6164 6572 206e 6f74 2069 6e20 6461 7461  ader not in data
+0000ad00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000ad10: 2020 2020 2020 2020 2020 6461 7461 5b63            data[c
+0000ad20: 7572 7265 6e74 5f68 6561 6465 725d 203d  urrent_header] =
+0000ad30: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
+0000ad40: 2020 2020 2020 2020 6461 7461 5b63 7572          data[cur
+0000ad50: 7265 6e74 5f68 6561 6465 725d 2e61 7070  rent_header].app
+0000ad60: 656e 6428 7b7d 290a 2020 2020 2020 2020  end({}).        
+0000ad70: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000ad80: 2020 2020 2020 2020 2020 6966 206c 696e            if lin
+0000ad90: 652e 7374 7269 7028 292e 7374 6172 7473  e.strip().starts
+0000ada0: 7769 7468 2822 3c22 293a 0a20 2020 2020  with("<"):.     
+0000adb0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000adc0: 2054 6865 206c 696e 6520 6c6f 6f6b 7320   The line looks 
+0000add0: 6c69 6b65 2074 6869 7320 3c4b 4559 3e56  like this <KEY>V
+0000ade0: 414c 5545 0a20 2020 2020 2020 2020 2020  ALUE.           
+0000adf0: 2020 2020 2020 2020 206b 6579 2c20 7661           key, va
+0000ae00: 6c75 6520 3d20 6c69 6e65 2e73 706c 6974  lue = line.split
+0000ae10: 2827 3e27 290a 2020 2020 2020 2020 2020  ('>').          
+0000ae20: 2020 2020 2020 2020 2020 2320 5374 7269            # Stri
+0000ae30: 7020 7468 6520 6c65 6164 696e 6720 273c  p the leading '<
+0000ae40: 2720 6672 6f6d 2074 6865 206b 6579 0a20  ' from the key. 
+0000ae50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae60: 2020 2064 6174 615b 6b65 795b 313a 5d5d     data[key[1:]]
+0000ae70: 203d 2076 616c 7565 0a20 2020 2020 2020   = value.       
+0000ae80: 2020 2020 2020 2020 2065 6c69 6620 273a           elif ':
+0000ae90: 2720 696e 206c 696e 653a 0a20 2020 2020  ' in line:.     
+0000aea0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000aeb0: 6172 7473 203d 206c 696e 652e 7374 7269  arts = line.stri
+0000aec0: 7028 292e 7370 6c69 7428 273a 2729 0a20  p().split(':'). 
+0000aed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aee0: 2020 2069 6620 6c65 6e28 7061 7274 7329     if len(parts)
+0000aef0: 203d 3d20 323a 0a20 2020 2020 2020 2020   == 2:.         
+0000af00: 2020 2020 2020 2020 2020 2020 2020 206b                 k
+0000af10: 6579 2c20 7661 6c75 6520 3d20 6c69 6e65  ey, value = line
+0000af20: 2e73 7472 6970 2829 2e73 706c 6974 2827  .strip().split('
+0000af30: 3a27 290a 2020 2020 2020 2020 2020 2020  :').            
+0000af40: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
 0000af50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af60: 206b 6579 2c20 7661 6c75 6520 3d20 7061   key, value = pa
-0000af70: 7274 735b 305d 2c20 223a 222e 6a6f 696e  rts[0], ":".join
-0000af80: 2870 6172 7473 5b31 3a5d 290a 2020 2020  (parts[1:]).    
-0000af90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afa0: 7661 6c75 6520 3d20 7661 6c75 652e 7374  value = value.st
-0000afb0: 7269 7028 290a 2020 2020 2020 2020 2020  rip().          
-0000afc0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-0000afd0: 2063 7572 7265 6e74 5f68 6561 6465 723a   current_header:
-0000afe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000aff0: 2020 2020 2020 2020 2064 6174 615b 6b65           data[ke
-0000b000: 795d 203d 2076 616c 7565 0a20 2020 2020  y] = value.     
-0000b010: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000b020: 6c69 6620 6e6f 7420 6375 7272 656e 745f  lif not current_
-0000b030: 7375 6268 6561 6465 723a 0a20 2020 2020  subheader:.     
+0000af60: 2020 2020 2020 6b65 792c 2076 616c 7565        key, value
+0000af70: 203d 2070 6172 7473 5b30 5d2c 2022 3a22   = parts[0], ":"
+0000af80: 2e6a 6f69 6e28 7061 7274 735b 313a 5d29  .join(parts[1:])
+0000af90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000afa0: 2020 2020 2076 616c 7565 203d 2076 616c       value = val
+0000afb0: 7565 2e73 7472 6970 2829 0a20 2020 2020  ue.strip().     
+0000afc0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000afd0: 6620 6e6f 7420 6375 7272 656e 745f 6865  f not current_he
+0000afe0: 6164 6572 3a0a 2020 2020 2020 2020 2020  ader:.          
+0000aff0: 2020 2020 2020 2020 2020 2020 2020 6461                da
+0000b000: 7461 5b6b 6579 5d20 3d20 7661 6c75 650a  ta[key] = value.
+0000b010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b020: 2020 2020 656c 6966 206e 6f74 2063 7572      elif not cur
+0000b030: 7265 6e74 5f73 7562 6865 6164 6572 3a0a  rent_subheader:.
 0000b040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b050: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
-0000b060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b070: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000b080: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000b090: 2063 7572 7265 6e74 5f73 7562 6865 6164   current_subhead
-0000b0a0: 6572 203d 3d20 2246 4f52 4d45 5220 434f  er == "FORMER CO
-0000b0b0: 4d50 414e 5922 3a0a 2020 2020 2020 2020  MPANY":.        
+0000b050: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+0000b060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b070: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000b080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b090: 2020 2069 6620 6375 7272 656e 745f 7375     if current_su
+0000b0a0: 6268 6561 6465 7220 3d3d 2022 464f 524d  bheader == "FORM
+0000b0b0: 4552 2043 4f4d 5041 4e59 223a 0a20 2020  ER COMPANY":.   
 0000b0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0d0: 2020 2020 6461 7461 5b63 7572 7265 6e74      data[current
-0000b0e0: 5f68 6561 6465 725d 5b2d 315d 5b63 7572  _header][-1][cur
-0000b0f0: 7265 6e74 5f73 7562 6865 6164 6572 5d5b  rent_subheader][
-0000b100: 2d31 5d5b 6b65 792e 7374 7269 7028 295d  -1][key.strip()]
-0000b110: 203d 2076 616c 7565 0a20 2020 2020 2020   = value.       
+0000b0d0: 2020 2020 2020 2020 2064 6174 615b 6375           data[cu
+0000b0e0: 7272 656e 745f 6865 6164 6572 5d5b 2d31  rrent_header][-1
+0000b0f0: 5d5b 6375 7272 656e 745f 7375 6268 6561  ][current_subhea
+0000b100: 6465 725d 5b2d 315d 5b6b 6579 2e73 7472  der][-1][key.str
+0000b110: 6970 2829 5d20 3d20 7661 6c75 650a 2020  ip()] = value.  
 0000b120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b130: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000b130: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
 0000b140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b150: 2020 2064 6174 615b 6375 7272 656e 745f     data[current_
-0000b160: 6865 6164 6572 5d5b 2d31 5d5b 6375 7272  header][-1][curr
-0000b170: 656e 745f 7375 6268 6561 6465 725d 5b6b  ent_subheader][k
-0000b180: 6579 2e73 7472 6970 2829 5d20 3d20 7661  ey.strip()] = va
-0000b190: 6c75 650a 0a20 2020 2020 2020 2023 2054  lue..        # T
-0000b1a0: 6865 2066 696c 6572 0a20 2020 2020 2020  he filer.       
-0000b1b0: 2066 696c 6572 7320 3d20 5b5d 0a20 2020   filers = [].   
-0000b1c0: 2020 2020 2066 6f72 2066 696c 6572 5f76       for filer_v
-0000b1d0: 616c 7565 7320 696e 2064 6174 612e 6765  alues in data.ge
-0000b1e0: 7428 2746 494c 4552 272c 2064 6174 612e  t('FILER', data.
-0000b1f0: 6765 7428 2746 494c 4544 2042 5927 2c20  get('FILED BY', 
-0000b200: 7b7d 2929 3a0a 2020 2020 2020 2020 2020  {})):.          
-0000b210: 2020 6669 6c65 725f 636f 6d70 616e 795f    filer_company_
-0000b220: 7661 6c75 6573 203d 2066 696c 6572 5f76  values = filer_v
-0000b230: 616c 7565 732e 6765 7428 2743 4f4d 5041  alues.get('COMPA
-0000b240: 4e59 2044 4154 4127 290a 2020 2020 2020  NY DATA').      
-0000b250: 2020 2020 2020 636f 6d70 616e 795f 6f62        company_ob
-0000b260: 6a20 3d20 4e6f 6e65 0a20 2020 2020 2020  j = None.       
-0000b270: 2020 2020 2069 6620 6669 6c65 725f 636f       if filer_co
-0000b280: 6d70 616e 795f 7661 6c75 6573 3a0a 2020  mpany_values:.  
-0000b290: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000b2a0: 6d70 616e 795f 6f62 6a20 3d20 436f 6d70  mpany_obj = Comp
-0000b2b0: 616e 7949 6e66 6f72 6d61 7469 6f6e 280a  anyInformation(.
-0000b2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2d0: 2020 2020 6e61 6d65 3d66 696c 6572 5f63      name=filer_c
-0000b2e0: 6f6d 7061 6e79 5f76 616c 7565 732e 6765  ompany_values.ge
-0000b2f0: 7428 2743 4f4d 5041 4e59 2043 4f4e 464f  t('COMPANY CONFO
-0000b300: 524d 4544 204e 414d 4527 292c 0a20 2020  RMED NAME'),.   
-0000b310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b320: 2063 696b 3d66 696c 6572 5f63 6f6d 7061   cik=filer_compa
-0000b330: 6e79 5f76 616c 7565 732e 6765 7428 2743  ny_values.get('C
-0000b340: 454e 5452 414c 2049 4e44 4558 204b 4559  ENTRAL INDEX KEY
-0000b350: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-0000b360: 2020 2020 2020 2020 7369 633d 6669 6c65          sic=file
-0000b370: 725f 636f 6d70 616e 795f 7661 6c75 6573  r_company_values
-0000b380: 2e67 6574 2827 5354 414e 4441 5244 2049  .get('STANDARD I
-0000b390: 4e44 5553 5452 4941 4c20 434c 4153 5349  NDUSTRIAL CLASSI
-0000b3a0: 4649 4341 5449 4f4e 2729 2c0a 2020 2020  FICATION'),.    
-0000b3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3c0: 6972 735f 6e75 6d62 6572 3d66 696c 6572  irs_number=filer
-0000b3d0: 5f63 6f6d 7061 6e79 5f76 616c 7565 732e  _company_values.
-0000b3e0: 6765 7428 2749 5253 204e 554d 4245 5227  get('IRS NUMBER'
-0000b3f0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000b400: 2020 2020 2020 2073 7461 7465 5f6f 665f         state_of_
-0000b410: 696e 636f 7270 6f72 6174 696f 6e3d 6669  incorporation=fi
-0000b420: 6c65 725f 636f 6d70 616e 795f 7661 6c75  ler_company_valu
-0000b430: 6573 2e67 6574 2827 5354 4154 4520 4f46  es.get('STATE OF
-0000b440: 2049 4e43 4f52 504f 5241 5449 4f4e 2729   INCORPORATION')
-0000b450: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000b460: 2020 2020 2020 6669 7363 616c 5f79 6561        fiscal_yea
-0000b470: 725f 656e 643d 6669 6c65 725f 636f 6d70  r_end=filer_comp
-0000b480: 616e 795f 7661 6c75 6573 2e67 6574 2827  any_values.get('
-0000b490: 4649 5343 414c 2059 4541 5220 454e 4427  FISCAL YEAR END'
-0000b4a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000b4b0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0000b4c0: 2320 4669 6c69 6e67 2056 616c 7565 730a  # Filing Values.
-0000b4d0: 2020 2020 2020 2020 2020 2020 6669 6c69              fili
-0000b4e0: 6e67 5f76 616c 7565 735f 7465 7874 5f73  ng_values_text_s
-0000b4f0: 6563 7469 6f6e 203d 2066 696c 6572 5f76  ection = filer_v
-0000b500: 616c 7565 732e 6765 7428 2746 494c 494e  alues.get('FILIN
-0000b510: 4720 5641 4c55 4553 2729 0a20 2020 2020  G VALUES').     
-0000b520: 2020 2020 2020 2066 696c 696e 675f 7661         filing_va
-0000b530: 6c75 6573 5f6f 626a 203d 204e 6f6e 650a  lues_obj = None.
-0000b540: 2020 2020 2020 2020 2020 2020 6966 2066              if f
-0000b550: 696c 696e 675f 7661 6c75 6573 5f74 6578  iling_values_tex
-0000b560: 745f 7365 6374 696f 6e3a 0a20 2020 2020  t_section:.     
-0000b570: 2020 2020 2020 2020 2020 2066 696c 696e             filin
-0000b580: 675f 7661 6c75 6573 5f6f 626a 203d 2046  g_values_obj = F
-0000b590: 696c 696e 6749 6e66 6f72 6d61 7469 6f6e  ilingInformation
-0000b5a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000b5b0: 2020 2020 2020 666f 726d 3d66 696c 696e        form=filin
-0000b5c0: 675f 7661 6c75 6573 5f74 6578 745f 7365  g_values_text_se
-0000b5d0: 6374 696f 6e2e 6765 7428 2746 4f52 4d20  ction.get('FORM 
-0000b5e0: 5459 5045 2729 2c0a 2020 2020 2020 2020  TYPE'),.        
-0000b5f0: 2020 2020 2020 2020 2020 2020 7365 635f              sec_
-0000b600: 6163 743d 6669 6c69 6e67 5f76 616c 7565  act=filing_value
-0000b610: 735f 7465 7874 5f73 6563 7469 6f6e 2e67  s_text_section.g
-0000b620: 6574 2827 5345 4320 4143 5427 292c 0a20  et('SEC ACT'),. 
-0000b630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b640: 2020 2066 696c 655f 6e75 6d62 6572 3d66     file_number=f
-0000b650: 696c 696e 675f 7661 6c75 6573 5f74 6578  iling_values_tex
-0000b660: 745f 7365 6374 696f 6e2e 6765 7428 2753  t_section.get('S
-0000b670: 4543 2046 494c 4520 4e55 4d42 4552 2729  EC FILE NUMBER')
-0000b680: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000b690: 2020 2020 2020 6669 6c6d 5f6e 756d 6265        film_numbe
-0000b6a0: 723d 6669 6c69 6e67 5f76 616c 7565 735f  r=filing_values_
-0000b6b0: 7465 7874 5f73 6563 7469 6f6e 2e67 6574  text_section.get
-0000b6c0: 2827 4649 4c4d 204e 554d 4245 5227 290a  ('FILM NUMBER').
-0000b6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6e0: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
-0000b6f0: 4e6f 7720 6372 6561 7465 2074 6865 2066  Now create the f
-0000b700: 696c 6572 0a20 2020 2020 2020 2020 2020  iler.           
-0000b710: 2066 696c 6572 203d 2046 696c 6572 280a   filer = Filer(.
-0000b720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b730: 636f 6d70 616e 795f 696e 666f 726d 6174  company_informat
-0000b740: 696f 6e3d 636f 6d70 616e 795f 6f62 6a2c  ion=company_obj,
-0000b750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b760: 2066 696c 696e 675f 696e 666f 726d 6174   filing_informat
-0000b770: 696f 6e3d 6669 6c69 6e67 5f76 616c 7565  ion=filing_value
-0000b780: 735f 6f62 6a2c 0a20 2020 2020 2020 2020  s_obj,.         
-0000b790: 2020 2020 2020 2062 7573 696e 6573 735f         business_
-0000b7a0: 6164 6472 6573 733d 4164 6472 6573 7328  address=Address(
-0000b7b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b7c0: 2020 2020 2073 7472 6565 7431 3d66 696c       street1=fil
-0000b7d0: 6572 5f76 616c 7565 735b 2742 5553 494e  er_values['BUSIN
-0000b7e0: 4553 5320 4144 4452 4553 5327 5d2e 6765  ESS ADDRESS'].ge
-0000b7f0: 7428 2753 5452 4545 5420 3127 292c 0a20  t('STREET 1'),. 
-0000b800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b810: 2020 2073 7472 6565 7432 3d66 696c 6572     street2=filer
-0000b820: 5f76 616c 7565 735b 2742 5553 494e 4553  _values['BUSINES
-0000b830: 5320 4144 4452 4553 5327 5d2e 6765 7428  S ADDRESS'].get(
-0000b840: 2753 5452 4545 5420 3227 292c 0a20 2020  'STREET 2'),.   
-0000b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b860: 2063 6974 793d 6669 6c65 725f 7661 6c75   city=filer_valu
-0000b870: 6573 5b27 4255 5349 4e45 5353 2041 4444  es['BUSINESS ADD
-0000b880: 5245 5353 275d 2e67 6574 2827 4349 5459  RESS'].get('CITY
-0000b890: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-0000b8a0: 2020 2020 2020 2020 7374 6174 655f 6f72          state_or
-0000b8b0: 5f63 6f75 6e74 7279 3d66 696c 6572 5f76  _country=filer_v
-0000b8c0: 616c 7565 735b 2742 5553 494e 4553 5320  alues['BUSINESS 
-0000b8d0: 4144 4452 4553 5327 5d2e 6765 7428 2753  ADDRESS'].get('S
-0000b8e0: 5441 5445 2729 2c0a 2020 2020 2020 2020  TATE'),.        
-0000b8f0: 2020 2020 2020 2020 2020 2020 7a69 7063              zipc
-0000b900: 6f64 653d 6669 6c65 725f 7661 6c75 6573  ode=filer_values
-0000b910: 5b27 4255 5349 4e45 5353 2041 4444 5245  ['BUSINESS ADDRE
-0000b920: 5353 275d 2e67 6574 2827 5a49 5027 292c  SS'].get('ZIP'),
-0000b930: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b940: 2020 2920 6966 2027 4255 5349 4e45 5353    ) if 'BUSINESS
-0000b950: 2041 4444 5245 5353 2720 696e 2066 696c   ADDRESS' in fil
-0000b960: 6572 5f76 616c 7565 7320 656c 7365 204e  er_values else N
-0000b970: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-0000b980: 2020 2020 206d 6169 6c69 6e67 5f61 6464       mailing_add
-0000b990: 7265 7373 3d41 6464 7265 7373 280a 2020  ress=Address(.  
-0000b9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9b0: 2020 7374 7265 6574 313d 6669 6c65 725f    street1=filer_
-0000b9c0: 7661 6c75 6573 5b27 4d41 494c 2041 4444  values['MAIL ADD
-0000b9d0: 5245 5353 275d 2e67 6574 2827 5354 5245  RESS'].get('STRE
-0000b9e0: 4554 2031 2729 2c0a 2020 2020 2020 2020  ET 1'),.        
-0000b9f0: 2020 2020 2020 2020 2020 2020 7374 7265              stre
-0000ba00: 6574 323d 6669 6c65 725f 7661 6c75 6573  et2=filer_values
-0000ba10: 5b27 4d41 494c 2041 4444 5245 5353 275d  ['MAIL ADDRESS']
-0000ba20: 2e67 6574 2827 5354 5245 4554 2032 2729  .get('STREET 2')
-0000ba30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000ba40: 2020 2020 2020 6369 7479 3d66 696c 6572        city=filer
-0000ba50: 5f76 616c 7565 735b 274d 4149 4c20 4144  _values['MAIL AD
-0000ba60: 4452 4553 5327 5d2e 6765 7428 2743 4954  DRESS'].get('CIT
-0000ba70: 5927 292c 0a20 2020 2020 2020 2020 2020  Y'),.           
-0000ba80: 2020 2020 2020 2020 2073 7461 7465 5f6f           state_o
-0000ba90: 725f 636f 756e 7472 793d 6669 6c65 725f  r_country=filer_
-0000baa0: 7661 6c75 6573 5b27 4d41 494c 2041 4444  values['MAIL ADD
-0000bab0: 5245 5353 275d 2e67 6574 2827 5354 4154  RESS'].get('STAT
-0000bac0: 4527 292c 0a20 2020 2020 2020 2020 2020  E'),.           
-0000bad0: 2020 2020 2020 2020 207a 6970 636f 6465           zipcode
-0000bae0: 3d66 696c 6572 5f76 616c 7565 735b 274d  =filer_values['M
-0000baf0: 4149 4c20 4144 4452 4553 5327 5d2e 6765  AIL ADDRESS'].ge
-0000bb00: 7428 275a 4950 2729 2c0a 0a20 2020 2020  t('ZIP'),..     
-0000bb10: 2020 2020 2020 2020 2020 2029 2069 6620             ) if 
-0000bb20: 274d 4149 4c20 4144 4452 4553 5327 2069  'MAIL ADDRESS' i
-0000bb30: 6e20 6669 6c65 725f 7661 6c75 6573 2065  n filer_values e
-0000bb40: 6c73 6520 4e6f 6e65 2c0a 2020 2020 2020  lse None,.      
-0000bb50: 2020 2020 2020 2020 2020 666f 726d 6572            former
-0000bb60: 5f63 6f6d 7061 6e79 5f6e 616d 6573 3d5b  _company_names=[
-0000bb70: 466f 726d 6572 436f 6d70 616e 7928 6461  FormerCompany(da
-0000bb80: 7465 5f6f 665f 6368 616e 6765 3d72 6563  te_of_change=rec
-0000bb90: 6f72 642e 6765 7428 2744 4154 4520 4f46  ord.get('DATE OF
-0000bba0: 204e 414d 4520 4348 414e 4745 2729 2c0a   NAME CHANGE'),.
-0000bbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b150: 2020 2020 2020 2020 6461 7461 5b63 7572          data[cur
+0000b160: 7265 6e74 5f68 6561 6465 725d 5b2d 315d  rent_header][-1]
+0000b170: 5b63 7572 7265 6e74 5f73 7562 6865 6164  [current_subhead
+0000b180: 6572 5d5b 6b65 792e 7374 7269 7028 295d  er][key.strip()]
+0000b190: 203d 2076 616c 7565 0a0a 2020 2020 2020   = value..      
+0000b1a0: 2020 2320 5468 6520 6669 6c65 720a 2020    # The filer.  
+0000b1b0: 2020 2020 2020 6669 6c65 7273 203d 205b        filers = [
+0000b1c0: 5d0a 2020 2020 2020 2020 666f 7220 6669  ].        for fi
+0000b1d0: 6c65 725f 7661 6c75 6573 2069 6e20 6461  ler_values in da
+0000b1e0: 7461 2e67 6574 2827 4649 4c45 5227 2c20  ta.get('FILER', 
+0000b1f0: 6461 7461 2e67 6574 2827 4649 4c45 4420  data.get('FILED 
+0000b200: 4259 272c 207b 7d29 293a 0a20 2020 2020  BY', {})):.     
+0000b210: 2020 2020 2020 2066 696c 6572 5f63 6f6d         filer_com
+0000b220: 7061 6e79 5f76 616c 7565 7320 3d20 6669  pany_values = fi
+0000b230: 6c65 725f 7661 6c75 6573 2e67 6574 2827  ler_values.get('
+0000b240: 434f 4d50 414e 5920 4441 5441 2729 0a20  COMPANY DATA'). 
+0000b250: 2020 2020 2020 2020 2020 2063 6f6d 7061             compa
+0000b260: 6e79 5f6f 626a 203d 204e 6f6e 650a 2020  ny_obj = None.  
+0000b270: 2020 2020 2020 2020 2020 6966 2066 696c            if fil
+0000b280: 6572 5f63 6f6d 7061 6e79 5f76 616c 7565  er_company_value
+0000b290: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+0000b2a0: 2020 2063 6f6d 7061 6e79 5f6f 626a 203d     company_obj =
+0000b2b0: 2043 6f6d 7061 6e79 496e 666f 726d 6174   CompanyInformat
+0000b2c0: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
+0000b2d0: 2020 2020 2020 2020 206e 616d 653d 6669           name=fi
+0000b2e0: 6c65 725f 636f 6d70 616e 795f 7661 6c75  ler_company_valu
+0000b2f0: 6573 2e67 6574 2827 434f 4d50 414e 5920  es.get('COMPANY 
+0000b300: 434f 4e46 4f52 4d45 4420 4e41 4d45 2729  CONFORMED NAME')
+0000b310: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000b320: 2020 2020 2020 6369 6b3d 6669 6c65 725f        cik=filer_
+0000b330: 636f 6d70 616e 795f 7661 6c75 6573 2e67  company_values.g
+0000b340: 6574 2827 4345 4e54 5241 4c20 494e 4445  et('CENTRAL INDE
+0000b350: 5820 4b45 5927 292c 0a20 2020 2020 2020  X KEY'),.       
+0000b360: 2020 2020 2020 2020 2020 2020 2073 6963               sic
+0000b370: 3d66 696c 6572 5f63 6f6d 7061 6e79 5f76  =filer_company_v
+0000b380: 616c 7565 732e 6765 7428 2753 5441 4e44  alues.get('STAND
+0000b390: 4152 4420 494e 4455 5354 5249 414c 2043  ARD INDUSTRIAL C
+0000b3a0: 4c41 5353 4946 4943 4154 494f 4e27 292c  LASSIFICATION'),
+0000b3b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b3c0: 2020 2020 2069 7273 5f6e 756d 6265 723d       irs_number=
+0000b3d0: 6669 6c65 725f 636f 6d70 616e 795f 7661  filer_company_va
+0000b3e0: 6c75 6573 2e67 6574 2827 4952 5320 4e55  lues.get('IRS NU
+0000b3f0: 4d42 4552 2729 2c0a 2020 2020 2020 2020  MBER'),.        
+0000b400: 2020 2020 2020 2020 2020 2020 7374 6174              stat
+0000b410: 655f 6f66 5f69 6e63 6f72 706f 7261 7469  e_of_incorporati
+0000b420: 6f6e 3d66 696c 6572 5f63 6f6d 7061 6e79  on=filer_company
+0000b430: 5f76 616c 7565 732e 6765 7428 2753 5441  _values.get('STA
+0000b440: 5445 204f 4620 494e 434f 5250 4f52 4154  TE OF INCORPORAT
+0000b450: 494f 4e27 292c 0a20 2020 2020 2020 2020  ION'),.         
+0000b460: 2020 2020 2020 2020 2020 2066 6973 6361             fisca
+0000b470: 6c5f 7965 6172 5f65 6e64 3d66 696c 6572  l_year_end=filer
+0000b480: 5f63 6f6d 7061 6e79 5f76 616c 7565 732e  _company_values.
+0000b490: 6765 7428 2746 4953 4341 4c20 5945 4152  get('FISCAL YEAR
+0000b4a0: 2045 4e44 2729 0a20 2020 2020 2020 2020   END').         
+0000b4b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000b4c0: 2020 2020 2023 2046 696c 696e 6720 5661       # Filing Va
+0000b4d0: 6c75 6573 0a20 2020 2020 2020 2020 2020  lues.           
+0000b4e0: 2066 696c 696e 675f 7661 6c75 6573 5f74   filing_values_t
+0000b4f0: 6578 745f 7365 6374 696f 6e20 3d20 6669  ext_section = fi
+0000b500: 6c65 725f 7661 6c75 6573 2e67 6574 2827  ler_values.get('
+0000b510: 4649 4c49 4e47 2056 414c 5545 5327 290a  FILING VALUES').
+0000b520: 2020 2020 2020 2020 2020 2020 6669 6c69              fili
+0000b530: 6e67 5f76 616c 7565 735f 6f62 6a20 3d20  ng_values_obj = 
+0000b540: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+0000b550: 2069 6620 6669 6c69 6e67 5f76 616c 7565   if filing_value
+0000b560: 735f 7465 7874 5f73 6563 7469 6f6e 3a0a  s_text_section:.
+0000b570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b580: 6669 6c69 6e67 5f76 616c 7565 735f 6f62  filing_values_ob
+0000b590: 6a20 3d20 4669 6c69 6e67 496e 666f 726d  j = FilingInform
+0000b5a0: 6174 696f 6e28 0a20 2020 2020 2020 2020  ation(.         
+0000b5b0: 2020 2020 2020 2020 2020 2066 6f72 6d3d             form=
+0000b5c0: 6669 6c69 6e67 5f76 616c 7565 735f 7465  filing_values_te
+0000b5d0: 7874 5f73 6563 7469 6f6e 2e67 6574 2827  xt_section.get('
+0000b5e0: 464f 524d 2054 5950 4527 292c 0a20 2020  FORM TYPE'),.   
+0000b5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b600: 2073 6563 5f61 6374 3d66 696c 696e 675f   sec_act=filing_
+0000b610: 7661 6c75 6573 5f74 6578 745f 7365 6374  values_text_sect
+0000b620: 696f 6e2e 6765 7428 2753 4543 2041 4354  ion.get('SEC ACT
+0000b630: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+0000b640: 2020 2020 2020 2020 6669 6c65 5f6e 756d          file_num
+0000b650: 6265 723d 6669 6c69 6e67 5f76 616c 7565  ber=filing_value
+0000b660: 735f 7465 7874 5f73 6563 7469 6f6e 2e67  s_text_section.g
+0000b670: 6574 2827 5345 4320 4649 4c45 204e 554d  et('SEC FILE NUM
+0000b680: 4245 5227 292c 0a20 2020 2020 2020 2020  BER'),.         
+0000b690: 2020 2020 2020 2020 2020 2066 696c 6d5f             film_
+0000b6a0: 6e75 6d62 6572 3d66 696c 696e 675f 7661  number=filing_va
+0000b6b0: 6c75 6573 5f74 6578 745f 7365 6374 696f  lues_text_sectio
+0000b6c0: 6e2e 6765 7428 2746 494c 4d20 4e55 4d42  n.get('FILM NUMB
+0000b6d0: 4552 2729 0a20 2020 2020 2020 2020 2020  ER').           
+0000b6e0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000b6f0: 2020 2023 204e 6f77 2063 7265 6174 6520     # Now create 
+0000b700: 7468 6520 6669 6c65 720a 2020 2020 2020  the filer.      
+0000b710: 2020 2020 2020 6669 6c65 7220 3d20 4669        filer = Fi
+0000b720: 6c65 7228 0a20 2020 2020 2020 2020 2020  ler(.           
+0000b730: 2020 2020 2063 6f6d 7061 6e79 5f69 6e66       company_inf
+0000b740: 6f72 6d61 7469 6f6e 3d63 6f6d 7061 6e79  ormation=company
+0000b750: 5f6f 626a 2c0a 2020 2020 2020 2020 2020  _obj,.          
+0000b760: 2020 2020 2020 6669 6c69 6e67 5f69 6e66        filing_inf
+0000b770: 6f72 6d61 7469 6f6e 3d66 696c 696e 675f  ormation=filing_
+0000b780: 7661 6c75 6573 5f6f 626a 2c0a 2020 2020  values_obj,.    
+0000b790: 2020 2020 2020 2020 2020 2020 6275 7369              busi
+0000b7a0: 6e65 7373 5f61 6464 7265 7373 3d41 6464  ness_address=Add
+0000b7b0: 7265 7373 280a 2020 2020 2020 2020 2020  ress(.          
+0000b7c0: 2020 2020 2020 2020 2020 7374 7265 6574            street
+0000b7d0: 313d 6669 6c65 725f 7661 6c75 6573 5b27  1=filer_values['
+0000b7e0: 4255 5349 4e45 5353 2041 4444 5245 5353  BUSINESS ADDRESS
+0000b7f0: 275d 2e67 6574 2827 5354 5245 4554 2031  '].get('STREET 1
+0000b800: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+0000b810: 2020 2020 2020 2020 7374 7265 6574 323d          street2=
+0000b820: 6669 6c65 725f 7661 6c75 6573 5b27 4255  filer_values['BU
+0000b830: 5349 4e45 5353 2041 4444 5245 5353 275d  SINESS ADDRESS']
+0000b840: 2e67 6574 2827 5354 5245 4554 2032 2729  .get('STREET 2')
+0000b850: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000b860: 2020 2020 2020 6369 7479 3d66 696c 6572        city=filer
+0000b870: 5f76 616c 7565 735b 2742 5553 494e 4553  _values['BUSINES
+0000b880: 5320 4144 4452 4553 5327 5d2e 6765 7428  S ADDRESS'].get(
+0000b890: 2743 4954 5927 292c 0a20 2020 2020 2020  'CITY'),.       
+0000b8a0: 2020 2020 2020 2020 2020 2020 2073 7461               sta
+0000b8b0: 7465 5f6f 725f 636f 756e 7472 793d 6669  te_or_country=fi
+0000b8c0: 6c65 725f 7661 6c75 6573 5b27 4255 5349  ler_values['BUSI
+0000b8d0: 4e45 5353 2041 4444 5245 5353 275d 2e67  NESS ADDRESS'].g
+0000b8e0: 6574 2827 5354 4154 4527 292c 0a20 2020  et('STATE'),.   
+0000b8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b900: 207a 6970 636f 6465 3d66 696c 6572 5f76   zipcode=filer_v
+0000b910: 616c 7565 735b 2742 5553 494e 4553 5320  alues['BUSINESS 
+0000b920: 4144 4452 4553 5327 5d2e 6765 7428 275a  ADDRESS'].get('Z
+0000b930: 4950 2729 2c0a 0a20 2020 2020 2020 2020  IP'),..         
+0000b940: 2020 2020 2020 2029 2069 6620 2742 5553         ) if 'BUS
+0000b950: 494e 4553 5320 4144 4452 4553 5327 2069  INESS ADDRESS' i
+0000b960: 6e20 6669 6c65 725f 7661 6c75 6573 2065  n filer_values e
+0000b970: 6c73 6520 4e6f 6e65 2c0a 2020 2020 2020  lse None,.      
+0000b980: 2020 2020 2020 2020 2020 6d61 696c 696e            mailin
+0000b990: 675f 6164 6472 6573 733d 4164 6472 6573  g_address=Addres
+0000b9a0: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
+0000b9b0: 2020 2020 2020 2073 7472 6565 7431 3d66         street1=f
+0000b9c0: 696c 6572 5f76 616c 7565 735b 274d 4149  iler_values['MAI
+0000b9d0: 4c20 4144 4452 4553 5327 5d2e 6765 7428  L ADDRESS'].get(
+0000b9e0: 2753 5452 4545 5420 3127 292c 0a20 2020  'STREET 1'),.   
+0000b9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba00: 2073 7472 6565 7432 3d66 696c 6572 5f76   street2=filer_v
+0000ba10: 616c 7565 735b 274d 4149 4c20 4144 4452  alues['MAIL ADDR
+0000ba20: 4553 5327 5d2e 6765 7428 2753 5452 4545  ESS'].get('STREE
+0000ba30: 5420 3227 292c 0a20 2020 2020 2020 2020  T 2'),.         
+0000ba40: 2020 2020 2020 2020 2020 2063 6974 793d             city=
+0000ba50: 6669 6c65 725f 7661 6c75 6573 5b27 4d41  filer_values['MA
+0000ba60: 494c 2041 4444 5245 5353 275d 2e67 6574  IL ADDRESS'].get
+0000ba70: 2827 4349 5459 2729 2c0a 2020 2020 2020  ('CITY'),.      
+0000ba80: 2020 2020 2020 2020 2020 2020 2020 7374                st
+0000ba90: 6174 655f 6f72 5f63 6f75 6e74 7279 3d66  ate_or_country=f
+0000baa0: 696c 6572 5f76 616c 7565 735b 274d 4149  iler_values['MAI
+0000bab0: 4c20 4144 4452 4553 5327 5d2e 6765 7428  L ADDRESS'].get(
+0000bac0: 2753 5441 5445 2729 2c0a 2020 2020 2020  'STATE'),.      
+0000bad0: 2020 2020 2020 2020 2020 2020 2020 7a69                zi
+0000bae0: 7063 6f64 653d 6669 6c65 725f 7661 6c75  pcode=filer_valu
+0000baf0: 6573 5b27 4d41 494c 2041 4444 5245 5353  es['MAIL ADDRESS
+0000bb00: 275d 2e67 6574 2827 5a49 5027 292c 0a0a  '].get('ZIP'),..
+0000bb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb20: 2920 6966 2027 4d41 494c 2041 4444 5245  ) if 'MAIL ADDRE
+0000bb30: 5353 2720 696e 2066 696c 6572 5f76 616c  SS' in filer_val
+0000bb40: 7565 7320 656c 7365 204e 6f6e 652c 0a20  ues else None,. 
+0000bb50: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000bb60: 6f72 6d65 725f 636f 6d70 616e 795f 6e61  ormer_company_na
+0000bb70: 6d65 733d 5b46 6f72 6d65 7243 6f6d 7061  mes=[FormerCompa
+0000bb80: 6e79 2864 6174 655f 6f66 5f63 6861 6e67  ny(date_of_chang
+0000bb90: 653d 7265 636f 7264 2e67 6574 2827 4441  e=record.get('DA
+0000bba0: 5445 204f 4620 4e41 4d45 2043 4841 4e47  TE OF NAME CHANG
+0000bbb0: 4527 292c 0a20 2020 2020 2020 2020 2020  E'),.           
 0000bbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbe0: 2020 2020 6e61 6d65 3d72 6563 6f72 642e      name=record.
-0000bbf0: 6765 7428 2746 4f52 4d45 5220 434f 4e46  get('FORMER CONF
-0000bc00: 4f52 4d45 4420 4e41 4d45 2729 290a 2020  ORMED NAME')).  
-0000bc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbe0: 2020 2020 2020 2020 206e 616d 653d 7265           name=re
+0000bbf0: 636f 7264 2e67 6574 2827 464f 524d 4552  cord.get('FORMER
+0000bc00: 2043 4f4e 464f 524d 4544 204e 414d 4527   CONFORMED NAME'
+0000bc10: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
 0000bc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc30: 2020 2020 666f 7220 7265 636f 7264 2069      for record i
-0000bc40: 6e20 6669 6c65 725f 7661 6c75 6573 5b27  n filer_values['
-0000bc50: 464f 524d 4552 2043 4f4d 5041 4e59 275d  FORMER COMPANY']
-0000bc60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bc30: 2020 2020 2020 2020 2066 6f72 2072 6563           for rec
+0000bc40: 6f72 6420 696e 2066 696c 6572 5f76 616c  ord in filer_val
+0000bc50: 7565 735b 2746 4f52 4d45 5220 434f 4d50  ues['FORMER COMP
+0000bc60: 414e 5927 5d0a 2020 2020 2020 2020 2020  ANY'].          
 0000bc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc80: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-0000bc90: 2020 2020 2020 2020 2069 6620 2746 4f52           if 'FOR
-0000bca0: 4d45 5220 434f 4d50 414e 5927 2069 6e20  MER COMPANY' in 
-0000bcb0: 6669 6c65 725f 7661 6c75 6573 2065 6c73  filer_values els
-0000bcc0: 6520 4e6f 6e65 0a20 2020 2020 2020 2020  e None.         
-0000bcd0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000bce0: 2066 696c 6572 732e 6170 7065 6e64 2866   filers.append(f
-0000bcf0: 696c 6572 290a 0a20 2020 2020 2020 2023  iler)..        #
-0000bd00: 2052 6570 6f72 7469 6e67 204f 776e 6572   Reporting Owner
-0000bd10: 0a0a 2020 2020 2020 2020 7265 706f 7274  ..        report
-0000bd20: 696e 675f 6f77 6e65 7273 203d 205b 5d0a  ing_owners = [].
-0000bd30: 0a20 2020 2020 2020 2066 6f72 2072 6570  .        for rep
-0000bd40: 6f72 7469 6e67 5f6f 776e 6572 5f76 616c  orting_owner_val
-0000bd50: 7565 7320 696e 2064 6174 612e 6765 7428  ues in data.get(
-0000bd60: 2752 4550 4f52 5449 4e47 2d4f 574e 4552  'REPORTING-OWNER
-0000bd70: 272c 205b 5d29 3a0a 2020 2020 2020 2020  ', []):.        
-0000bd80: 2020 2020 7265 706f 7274 696e 675f 6f77      reporting_ow
-0000bd90: 6e65 7220 3d20 4e6f 6e65 0a0a 2020 2020  ner = None..    
-0000bda0: 2020 2020 2020 2020 6966 2072 6570 6f72          if repor
-0000bdb0: 7469 6e67 5f6f 776e 6572 5f76 616c 7565  ting_owner_value
-0000bdc0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0000bdd0: 2020 206f 776e 6572 2c20 6e61 6d65 2c20     owner, name, 
-0000bde0: 6369 6b20 3d20 4e6f 6e65 2c20 4e6f 6e65  cik = None, None
-0000bdf0: 2c20 4e6f 6e65 0a20 2020 2020 2020 2020  , None.         
-0000be00: 2020 2020 2020 2069 6620 224f 574e 4552         if "OWNER
-0000be10: 2044 4154 4122 2069 6e20 7265 706f 7274   DATA" in report
-0000be20: 696e 675f 6f77 6e65 725f 7661 6c75 6573  ing_owner_values
-0000be30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000be40: 2020 2020 2020 6e61 6d65 203d 2072 6570        name = rep
-0000be50: 6f72 7469 6e67 5f6f 776e 6572 5f76 616c  orting_owner_val
-0000be60: 7565 732e 6765 7428 274f 574e 4552 2044  ues.get('OWNER D
-0000be70: 4154 4127 292e 6765 7428 2743 4f4d 5041  ATA').get('COMPA
-0000be80: 4e59 2043 4f4e 464f 524d 4544 204e 414d  NY CONFORMED NAM
-0000be90: 4527 290a 2020 2020 2020 2020 2020 2020  E').            
-0000bea0: 2020 2020 2020 2020 6369 6b20 3d20 7265          cik = re
-0000beb0: 706f 7274 696e 675f 6f77 6e65 725f 7661  porting_owner_va
-0000bec0: 6c75 6573 2e67 6574 2827 4f57 4e45 5220  lues.get('OWNER 
-0000bed0: 4441 5441 2729 2e67 6574 2827 4345 4e54  DATA').get('CENT
-0000bee0: 5241 4c20 494e 4445 5820 4b45 5927 290a  RAL INDEX KEY').
-0000bef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf00: 656c 6966 2027 434f 4d50 414e 5920 4441  elif 'COMPANY DA
-0000bf10: 5441 2720 696e 2072 6570 6f72 7469 6e67  TA' in reporting
-0000bf20: 5f6f 776e 6572 5f76 616c 7565 733a 0a20  _owner_values:. 
-0000bf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf40: 2020 206e 616d 6520 3d20 7265 706f 7274     name = report
-0000bf50: 696e 675f 6f77 6e65 725f 7661 6c75 6573  ing_owner_values
-0000bf60: 5b27 434f 4d50 414e 5920 4441 5441 275d  ['COMPANY DATA']
-0000bf70: 2e67 6574 2827 434f 4d50 414e 5920 434f  .get('COMPANY CO
-0000bf80: 4e46 4f52 4d45 4420 4e41 4d45 2729 0a20  NFORMED NAME'). 
-0000bf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfa0: 2020 2063 696b 203d 2072 6570 6f72 7469     cik = reporti
-0000bfb0: 6e67 5f6f 776e 6572 5f76 616c 7565 735b  ng_owner_values[
-0000bfc0: 2743 4f4d 5041 4e59 2044 4154 4127 5d2e  'COMPANY DATA'].
-0000bfd0: 6765 7428 2743 454e 5452 414c 2049 4e44  get('CENTRAL IND
-0000bfe0: 4558 204b 4559 2729 0a20 2020 2020 2020  EX KEY').       
-0000bff0: 2020 2020 2020 2020 2069 6620 6369 6b3a           if cik:
-0000c000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c010: 2020 2020 2066 726f 6d20 6564 6761 722e       from edgar.
-0000c020: 5f63 6f6d 7061 6e69 6573 2069 6d70 6f72  _companies impor
-0000c030: 7420 456e 7469 7479 0a20 2020 2020 2020  t Entity.       
-0000c040: 2020 2020 2020 2020 2020 2020 2065 6e74               ent
-0000c050: 6974 793a 2045 6e74 6974 7920 3d20 456e  ity: Entity = En
-0000c060: 7469 7479 2863 696b 290a 2020 2020 2020  tity(cik).      
-0000c070: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000c080: 206e 6f74 2065 6e74 6974 792e 6973 5f63   not entity.is_c
-0000c090: 6f6d 7061 6e79 3a0a 2020 2020 2020 2020  ompany:.        
+0000bc80: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
+0000bc90: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000bca0: 2027 464f 524d 4552 2043 4f4d 5041 4e59   'FORMER COMPANY
+0000bcb0: 2720 696e 2066 696c 6572 5f76 616c 7565  ' in filer_value
+0000bcc0: 7320 656c 7365 204e 6f6e 650a 2020 2020  s else None.    
+0000bcd0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000bce0: 2020 2020 2020 6669 6c65 7273 2e61 7070        filers.app
+0000bcf0: 656e 6428 6669 6c65 7229 0a0a 2020 2020  end(filer)..    
+0000bd00: 2020 2020 2320 5265 706f 7274 696e 6720      # Reporting 
+0000bd10: 4f77 6e65 720a 0a20 2020 2020 2020 2072  Owner..        r
+0000bd20: 6570 6f72 7469 6e67 5f6f 776e 6572 7320  eporting_owners 
+0000bd30: 3d20 5b5d 0a0a 2020 2020 2020 2020 666f  = []..        fo
+0000bd40: 7220 7265 706f 7274 696e 675f 6f77 6e65  r reporting_owne
+0000bd50: 725f 7661 6c75 6573 2069 6e20 6461 7461  r_values in data
+0000bd60: 2e67 6574 2827 5245 504f 5254 494e 472d  .get('REPORTING-
+0000bd70: 4f57 4e45 5227 2c20 5b5d 293a 0a20 2020  OWNER', []):.   
+0000bd80: 2020 2020 2020 2020 2072 6570 6f72 7469           reporti
+0000bd90: 6e67 5f6f 776e 6572 203d 204e 6f6e 650a  ng_owner = None.
+0000bda0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000bdb0: 7265 706f 7274 696e 675f 6f77 6e65 725f  reporting_owner_
+0000bdc0: 7661 6c75 6573 3a0a 2020 2020 2020 2020  values:.        
+0000bdd0: 2020 2020 2020 2020 6f77 6e65 722c 206e          owner, n
+0000bde0: 616d 652c 2063 696b 203d 204e 6f6e 652c  ame, cik = None,
+0000bdf0: 204e 6f6e 652c 204e 6f6e 650a 2020 2020   None, None.    
+0000be00: 2020 2020 2020 2020 2020 2020 6966 2022              if "
+0000be10: 4f57 4e45 5220 4441 5441 2220 696e 2072  OWNER DATA" in r
+0000be20: 6570 6f72 7469 6e67 5f6f 776e 6572 5f76  eporting_owner_v
+0000be30: 616c 7565 733a 0a20 2020 2020 2020 2020  alues:.         
+0000be40: 2020 2020 2020 2020 2020 206e 616d 6520             name 
+0000be50: 3d20 7265 706f 7274 696e 675f 6f77 6e65  = reporting_owne
+0000be60: 725f 7661 6c75 6573 2e67 6574 2827 4f57  r_values.get('OW
+0000be70: 4e45 5220 4441 5441 2729 2e67 6574 2827  NER DATA').get('
+0000be80: 434f 4d50 414e 5920 434f 4e46 4f52 4d45  COMPANY CONFORME
+0000be90: 4420 4e41 4d45 2729 0a20 2020 2020 2020  D NAME').       
+0000bea0: 2020 2020 2020 2020 2020 2020 2063 696b               cik
+0000beb0: 203d 2072 6570 6f72 7469 6e67 5f6f 776e   = reporting_own
+0000bec0: 6572 5f76 616c 7565 732e 6765 7428 274f  er_values.get('O
+0000bed0: 574e 4552 2044 4154 4127 292e 6765 7428  WNER DATA').get(
+0000bee0: 2743 454e 5452 414c 2049 4e44 4558 204b  'CENTRAL INDEX K
+0000bef0: 4559 2729 0a20 2020 2020 2020 2020 2020  EY').           
+0000bf00: 2020 2020 2065 6c69 6620 2743 4f4d 5041       elif 'COMPA
+0000bf10: 4e59 2044 4154 4127 2069 6e20 7265 706f  NY DATA' in repo
+0000bf20: 7274 696e 675f 6f77 6e65 725f 7661 6c75  rting_owner_valu
+0000bf30: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+0000bf40: 2020 2020 2020 2020 6e61 6d65 203d 2072          name = r
+0000bf50: 6570 6f72 7469 6e67 5f6f 776e 6572 5f76  eporting_owner_v
+0000bf60: 616c 7565 735b 2743 4f4d 5041 4e59 2044  alues['COMPANY D
+0000bf70: 4154 4127 5d2e 6765 7428 2743 4f4d 5041  ATA'].get('COMPA
+0000bf80: 4e59 2043 4f4e 464f 524d 4544 204e 414d  NY CONFORMED NAM
+0000bf90: 4527 290a 2020 2020 2020 2020 2020 2020  E').            
+0000bfa0: 2020 2020 2020 2020 6369 6b20 3d20 7265          cik = re
+0000bfb0: 706f 7274 696e 675f 6f77 6e65 725f 7661  porting_owner_va
+0000bfc0: 6c75 6573 5b27 434f 4d50 414e 5920 4441  lues['COMPANY DA
+0000bfd0: 5441 275d 2e67 6574 2827 4345 4e54 5241  TA'].get('CENTRA
+0000bfe0: 4c20 494e 4445 5820 4b45 5927 290a 2020  L INDEX KEY').  
+0000bff0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000c000: 2063 696b 3a0a 2020 2020 2020 2020 2020   cik:.          
+0000c010: 2020 2020 2020 2020 2020 6672 6f6d 2065            from e
+0000c020: 6467 6172 2e5f 636f 6d70 616e 6965 7320  dgar._companies 
+0000c030: 696d 706f 7274 2045 6e74 6974 790a 2020  import Entity.  
+0000c040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c050: 2020 656e 7469 7479 3a20 456e 7469 7479    entity: Entity
+0000c060: 203d 2045 6e74 6974 7928 6369 6b29 0a20   = Entity(cik). 
+0000c070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c080: 2020 2069 6620 6e6f 7420 656e 7469 7479     if not entity
+0000c090: 2e69 735f 636f 6d70 616e 793a 0a20 2020  .is_company:.   
 0000c0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0b0: 6e61 6d65 203d 2072 6576 6572 7365 5f6e  name = reverse_n
-0000c0c0: 616d 6528 6e61 6d65 290a 2020 2020 2020  ame(name).      
-0000c0d0: 2020 2020 2020 2020 2020 2020 2020 6f77                ow
-0000c0e0: 6e65 7220 3d20 4f77 6e65 7228 6e61 6d65  ner = Owner(name
-0000c0f0: 3d6e 616d 652c 2063 696b 3d63 696b 290a  =name, cik=cik).
-0000c100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c110: 2023 2043 6f6d 7061 6e79 2049 6e66 6f72   # Company Infor
-0000c120: 6d61 7469 6f6e 0a20 2020 2020 2020 2020  mation.         
-0000c130: 2020 2020 2020 2063 6f6d 7061 6e79 5f69         company_i
-0000c140: 6e66 6f72 6d61 7469 6f6e 203d 2043 6f6d  nformation = Com
-0000c150: 7061 6e79 496e 666f 726d 6174 696f 6e28  panyInformation(
-0000c160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c170: 2020 2020 206e 616d 653d 7265 706f 7274       name=report
-0000c180: 696e 675f 6f77 6e65 725f 7661 6c75 6573  ing_owner_values
-0000c190: 2e67 6574 2827 434f 4d50 414e 5920 4441  .get('COMPANY DA
-0000c1a0: 5441 2729 2e67 6574 2827 434f 4d50 414e  TA').get('COMPAN
-0000c1b0: 5920 434f 4e46 4f52 4d45 4420 4e41 4d45  Y CONFORMED NAME
-0000c1c0: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-0000c1d0: 2020 2020 2020 2020 6369 6b3d 7265 706f          cik=repo
-0000c1e0: 7274 696e 675f 6f77 6e65 725f 7661 6c75  rting_owner_valu
-0000c1f0: 6573 2e67 6574 2827 434f 4d50 414e 5920  es.get('COMPANY 
-0000c200: 4441 5441 2729 2e67 6574 2827 4345 4e54  DATA').get('CENT
-0000c210: 5241 4c20 494e 4445 5820 4b45 5927 292c  RAL INDEX KEY'),
-0000c220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c230: 2020 2020 2073 6963 3d72 6570 6f72 7469       sic=reporti
-0000c240: 6e67 5f6f 776e 6572 5f76 616c 7565 732e  ng_owner_values.
-0000c250: 6765 7428 2743 4f4d 5041 4e59 2044 4154  get('COMPANY DAT
-0000c260: 4127 292e 6765 7428 2753 5441 4e44 4152  A').get('STANDAR
-0000c270: 4420 494e 4455 5354 5249 414c 2043 4c41  D INDUSTRIAL CLA
-0000c280: 5353 4946 4943 4154 494f 4e27 292c 0a20  SSIFICATION'),. 
-0000c290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2a0: 2020 2069 7273 5f6e 756d 6265 723d 7265     irs_number=re
-0000c2b0: 706f 7274 696e 675f 6f77 6e65 725f 7661  porting_owner_va
-0000c2c0: 6c75 6573 2e67 6574 2827 434f 4d50 414e  lues.get('COMPAN
-0000c2d0: 5920 4441 5441 2729 2e67 6574 2827 4952  Y DATA').get('IR
-0000c2e0: 5320 4e55 4d42 4552 2729 2c0a 2020 2020  S NUMBER'),.    
-0000c2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c300: 7374 6174 655f 6f66 5f69 6e63 6f72 706f  state_of_incorpo
-0000c310: 7261 7469 6f6e 3d72 6570 6f72 7469 6e67  ration=reporting
-0000c320: 5f6f 776e 6572 5f76 616c 7565 732e 6765  _owner_values.ge
-0000c330: 7428 2743 4f4d 5041 4e59 2044 4154 4127  t('COMPANY DATA'
-0000c340: 292e 6765 7428 2753 5441 5445 204f 4620  ).get('STATE OF 
-0000c350: 494e 434f 5250 4f52 4154 494f 4e27 292c  INCORPORATION'),
-0000c360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c370: 2020 2020 2066 6973 6361 6c5f 7965 6172       fiscal_year
-0000c380: 5f65 6e64 3d72 6570 6f72 7469 6e67 5f6f  _end=reporting_o
-0000c390: 776e 6572 5f76 616c 7565 732e 6765 7428  wner_values.get(
-0000c3a0: 2743 4f4d 5041 4e59 2044 4154 4127 292e  'COMPANY DATA').
-0000c3b0: 6765 7428 2746 4953 4341 4c20 5945 4152  get('FISCAL YEAR
-0000c3c0: 2045 4e44 2729 0a20 2020 2020 2020 2020   END').         
-0000c3d0: 2020 2020 2020 2029 2069 6620 2243 4f4d         ) if "COM
-0000c3e0: 5041 4e59 2044 4154 4122 2069 6e20 7265  PANY DATA" in re
-0000c3f0: 706f 7274 696e 675f 6f77 6e65 725f 7661  porting_owner_va
-0000c400: 6c75 6573 2065 6c73 6520 4e6f 6e65 0a0a  lues else None..
-0000c410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c420: 2320 4669 6c69 6e67 2049 6e66 6f72 6d61  # Filing Informa
-0000c430: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-0000c440: 2020 2020 2066 696c 696e 675f 696e 666f       filing_info
-0000c450: 726d 6174 696f 6e20 3d20 4669 6c69 6e67  rmation = Filing
-0000c460: 496e 666f 726d 6174 696f 6e28 0a20 2020  Information(.   
-0000c470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c480: 2066 6f72 6d3d 7265 706f 7274 696e 675f   form=reporting_
-0000c490: 6f77 6e65 725f 7661 6c75 6573 2e67 6574  owner_values.get
-0000c4a0: 2827 4649 4c49 4e47 2056 414c 5545 5327  ('FILING VALUES'
-0000c4b0: 292e 6765 7428 2746 4f52 4d20 5459 5045  ).get('FORM TYPE
-0000c4c0: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-0000c4d0: 2020 2020 2020 2020 7365 635f 6163 743d          sec_act=
-0000c4e0: 7265 706f 7274 696e 675f 6f77 6e65 725f  reporting_owner_
-0000c4f0: 7661 6c75 6573 2e67 6574 2827 4649 4c49  values.get('FILI
-0000c500: 4e47 2056 414c 5545 5327 292e 6765 7428  NG VALUES').get(
-0000c510: 2753 4543 2041 4354 2729 2c0a 2020 2020  'SEC ACT'),.    
-0000c520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c530: 6669 6c65 5f6e 756d 6265 723d 7265 706f  file_number=repo
-0000c540: 7274 696e 675f 6f77 6e65 725f 7661 6c75  rting_owner_valu
-0000c550: 6573 2e67 6574 2827 4649 4c49 4e47 2056  es.get('FILING V
-0000c560: 414c 5545 5327 292e 6765 7428 2753 4543  ALUES').get('SEC
-0000c570: 2046 494c 4520 4e55 4d42 4552 2729 2c0a   FILE NUMBER'),.
-0000c580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c590: 2020 2020 6669 6c6d 5f6e 756d 6265 723d      film_number=
-0000c5a0: 7265 706f 7274 696e 675f 6f77 6e65 725f  reporting_owner_
-0000c5b0: 7661 6c75 6573 2e67 6574 2827 4649 4c49  values.get('FILI
-0000c5c0: 4e47 2056 414c 5545 5327 292e 6765 7428  NG VALUES').get(
-0000c5d0: 2746 494c 4d20 4e55 4d42 4552 2729 0a20  'FILM NUMBER'). 
-0000c5e0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000c5f0: 2069 6620 2827 4649 4c49 4e47 2056 414c   if ('FILING VAL
-0000c600: 5545 5327 2069 6e20 7265 706f 7274 696e  UES' in reportin
-0000c610: 675f 6f77 6e65 725f 7661 6c75 6573 2061  g_owner_values a
-0000c620: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
-0000c630: 2020 2020 2020 2020 2072 6570 6f72 7469           reporti
-0000c640: 6e67 5f6f 776e 6572 5f76 616c 7565 732e  ng_owner_values.
-0000c650: 6765 7428 2746 494c 494e 4720 5641 4c55  get('FILING VALU
-0000c660: 4553 2729 2e67 6574 2827 5345 4320 4649  ES').get('SEC FI
-0000c670: 4c45 204e 554d 4245 5227 2929 2065 6c73  LE NUMBER')) els
-0000c680: 6520 4e6f 6e65 0a0a 2020 2020 2020 2020  e None..        
-0000c690: 2020 2020 2020 2020 2320 4275 7369 6e65          # Busine
-0000c6a0: 7373 2041 6464 7265 7373 0a20 2020 2020  ss Address.     
-0000c6b0: 2020 2020 2020 2020 2020 2062 7573 696e             busin
-0000c6c0: 6573 735f 6164 6472 6573 7320 3d20 4164  ess_address = Ad
-0000c6d0: 6472 6573 7328 0a20 2020 2020 2020 2020  dress(.         
-0000c6e0: 2020 2020 2020 2020 2020 2073 7472 6565             stree
-0000c6f0: 7431 3d72 6570 6f72 7469 6e67 5f6f 776e  t1=reporting_own
-0000c700: 6572 5f76 616c 7565 732e 6765 7428 2742  er_values.get('B
-0000c710: 5553 494e 4553 5320 4144 4452 4553 5327  USINESS ADDRESS'
-0000c720: 292e 6765 7428 2753 5452 4545 5420 3127  ).get('STREET 1'
-0000c730: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000c740: 2020 2020 2020 2073 7472 6565 7432 3d72         street2=r
-0000c750: 6570 6f72 7469 6e67 5f6f 776e 6572 5f76  eporting_owner_v
-0000c760: 616c 7565 732e 6765 7428 2742 5553 494e  alues.get('BUSIN
-0000c770: 4553 5320 4144 4452 4553 5327 292e 6765  ESS ADDRESS').ge
-0000c780: 7428 2753 5452 4545 5420 3227 292c 0a20  t('STREET 2'),. 
-0000c790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7a0: 2020 2063 6974 793d 7265 706f 7274 696e     city=reportin
-0000c7b0: 675f 6f77 6e65 725f 7661 6c75 6573 2e67  g_owner_values.g
-0000c7c0: 6574 2827 4255 5349 4e45 5353 2041 4444  et('BUSINESS ADD
-0000c7d0: 5245 5353 2729 2e67 6574 2827 4349 5459  RESS').get('CITY
-0000c7e0: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-0000c7f0: 2020 2020 2020 2020 7374 6174 655f 6f72          state_or
-0000c800: 5f63 6f75 6e74 7279 3d72 6570 6f72 7469  _country=reporti
-0000c810: 6e67 5f6f 776e 6572 5f76 616c 7565 732e  ng_owner_values.
-0000c820: 6765 7428 2742 5553 494e 4553 5320 4144  get('BUSINESS AD
-0000c830: 4452 4553 5327 292e 6765 7428 2753 5441  DRESS').get('STA
-0000c840: 5445 2729 2c0a 2020 2020 2020 2020 2020  TE'),.          
-0000c850: 2020 2020 2020 2020 2020 7a69 7063 6f64            zipcod
-0000c860: 653d 7265 706f 7274 696e 675f 6f77 6e65  e=reporting_owne
-0000c870: 725f 7661 6c75 6573 2e67 6574 2827 4255  r_values.get('BU
-0000c880: 5349 4e45 5353 2041 4444 5245 5353 2729  SINESS ADDRESS')
-0000c890: 2e67 6574 2827 5a49 5027 292c 0a20 2020  .get('ZIP'),.   
-0000c8a0: 2020 2020 2020 2020 2020 2020 2029 2069               ) i
-0000c8b0: 6620 2742 5553 494e 4553 5320 4144 4452  f 'BUSINESS ADDR
-0000c8c0: 4553 5327 2069 6e20 7265 706f 7274 696e  ESS' in reportin
-0000c8d0: 675f 6f77 6e65 725f 7661 6c75 6573 2065  g_owner_values e
-0000c8e0: 6c73 6520 4e6f 6e65 0a0a 2020 2020 2020  lse None..      
-0000c8f0: 2020 2020 2020 2020 2020 2320 4d61 696c            # Mail
-0000c900: 696e 6720 4164 6472 6573 730a 2020 2020  ing Address.    
-0000c910: 2020 2020 2020 2020 2020 2020 6d61 696c              mail
-0000c920: 696e 675f 6164 6472 6573 7320 3d20 4164  ing_address = Ad
-0000c930: 6472 6573 7328 0a20 2020 2020 2020 2020  dress(.         
-0000c940: 2020 2020 2020 2020 2020 2073 7472 6565             stree
-0000c950: 7431 3d72 6570 6f72 7469 6e67 5f6f 776e  t1=reporting_own
-0000c960: 6572 5f76 616c 7565 732e 6765 7428 274d  er_values.get('M
-0000c970: 4149 4c20 4144 4452 4553 5327 292e 6765  AIL ADDRESS').ge
-0000c980: 7428 2753 5452 4545 5420 3127 292c 0a20  t('STREET 1'),. 
-0000c990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9a0: 2020 2073 7472 6565 7432 3d72 6570 6f72     street2=repor
-0000c9b0: 7469 6e67 5f6f 776e 6572 5f76 616c 7565  ting_owner_value
-0000c9c0: 732e 6765 7428 274d 4149 4c20 4144 4452  s.get('MAIL ADDR
-0000c9d0: 4553 5327 292e 6765 7428 2753 5452 4545  ESS').get('STREE
-0000c9e0: 5420 3227 292c 0a20 2020 2020 2020 2020  T 2'),.         
-0000c9f0: 2020 2020 2020 2020 2020 2063 6974 793d             city=
-0000ca00: 7265 706f 7274 696e 675f 6f77 6e65 725f  reporting_owner_
-0000ca10: 7661 6c75 6573 2e67 6574 2827 4d41 494c  values.get('MAIL
-0000ca20: 2041 4444 5245 5353 2729 2e67 6574 2827   ADDRESS').get('
-0000ca30: 4349 5459 2729 2c0a 2020 2020 2020 2020  CITY'),.        
-0000ca40: 2020 2020 2020 2020 2020 2020 7374 6174              stat
-0000ca50: 655f 6f72 5f63 6f75 6e74 7279 3d72 6570  e_or_country=rep
-0000ca60: 6f72 7469 6e67 5f6f 776e 6572 5f76 616c  orting_owner_val
-0000ca70: 7565 732e 6765 7428 274d 4149 4c20 4144  ues.get('MAIL AD
-0000ca80: 4452 4553 5327 292e 6765 7428 2753 5441  DRESS').get('STA
-0000ca90: 5445 2729 2c0a 2020 2020 2020 2020 2020  TE'),.          
-0000caa0: 2020 2020 2020 2020 2020 7a69 7063 6f64            zipcod
-0000cab0: 653d 7265 706f 7274 696e 675f 6f77 6e65  e=reporting_owne
-0000cac0: 725f 7661 6c75 6573 2e67 6574 2827 4d41  r_values.get('MA
-0000cad0: 494c 2041 4444 5245 5353 2729 2e67 6574  IL ADDRESS').get
-0000cae0: 2827 5a49 5027 292c 0a20 2020 2020 2020  ('ZIP'),.       
-0000caf0: 2020 2020 2020 2020 2029 2069 6620 274d           ) if 'M
-0000cb00: 4149 4c20 4144 4452 4553 5327 2069 6e20  AIL ADDRESS' in 
-0000cb10: 7265 706f 7274 696e 675f 6f77 6e65 725f  reporting_owner_
-0000cb20: 7661 6c75 6573 2065 6c73 6520 4e6f 6e65  values else None
-0000cb30: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000cb40: 2020 2320 4e6f 7720 6372 6561 7465 2074    # Now create t
-0000cb50: 6865 2072 6570 6f72 7469 6e67 206f 776e  he reporting own
-0000cb60: 6572 0a20 2020 2020 2020 2020 2020 2020  er.             
-0000cb70: 2020 2072 6570 6f72 7469 6e67 5f6f 776e     reporting_own
-0000cb80: 6572 203d 2052 6570 6f72 7469 6e67 4f77  er = ReportingOw
-0000cb90: 6e65 7228 0a20 2020 2020 2020 2020 2020  ner(.           
-0000cba0: 2020 2020 2020 2020 206f 776e 6572 3d6f           owner=o
-0000cbb0: 776e 6572 2c0a 2020 2020 2020 2020 2020  wner,.          
-0000cbc0: 2020 2020 2020 2020 2020 636f 6d70 616e            compan
-0000cbd0: 795f 696e 666f 726d 6174 696f 6e3d 636f  y_information=co
-0000cbe0: 6d70 616e 795f 696e 666f 726d 6174 696f  mpany_informatio
-0000cbf0: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
-0000cc00: 2020 2020 2020 2066 696c 696e 675f 696e         filing_in
-0000cc10: 666f 726d 6174 696f 6e3d 6669 6c69 6e67  formation=filing
-0000cc20: 5f69 6e66 6f72 6d61 7469 6f6e 2c0a 2020  _information,.  
-0000cc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc40: 2020 6275 7369 6e65 7373 5f61 6464 7265    business_addre
-0000cc50: 7373 3d62 7573 696e 6573 735f 6164 6472  ss=business_addr
-0000cc60: 6573 732c 0a20 2020 2020 2020 2020 2020  ess,.           
-0000cc70: 2020 2020 2020 2020 206d 6169 6c69 6e67           mailing
-0000cc80: 5f61 6464 7265 7373 3d6d 6169 6c69 6e67  _address=mailing
-0000cc90: 5f61 6464 7265 7373 0a20 2020 2020 2020  _address.       
-0000cca0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000ccb0: 2020 2020 2020 2072 6570 6f72 7469 6e67         reporting
-0000ccc0: 5f6f 776e 6572 732e 6170 7065 6e64 2872  _owners.append(r
-0000ccd0: 6570 6f72 7469 6e67 5f6f 776e 6572 290a  eporting_owner).
-0000cce0: 0a20 2020 2020 2020 2023 2049 7373 7565  .        # Issue
-0000ccf0: 720a 2020 2020 2020 2020 6973 7375 6572  r.        issuer
-0000cd00: 7320 3d20 5b5d 0a20 2020 2020 2020 2066  s = [].        f
-0000cd10: 6f72 2069 7373 7565 725f 7661 6c75 6573  or issuer_values
-0000cd20: 2069 6e20 6461 7461 2e67 6574 2827 4953   in data.get('IS
-0000cd30: 5355 4552 272c 205b 5d29 3a0a 2020 2020  SUER', []):.    
-0000cd40: 2020 2020 2020 2020 6973 7375 6572 203d          issuer =
-0000cd50: 2049 7373 7565 7228 0a20 2020 2020 2020   Issuer(.       
-0000cd60: 2020 2020 2020 2020 2063 6f6d 7061 6e79           company
-0000cd70: 5f69 6e66 6f72 6d61 7469 6f6e 3d43 6f6d  _information=Com
-0000cd80: 7061 6e79 496e 666f 726d 6174 696f 6e28  panyInformation(
-0000cd90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cda0: 2020 2020 206e 616d 653d 6973 7375 6572       name=issuer
-0000cdb0: 5f76 616c 7565 732e 6765 7428 2743 4f4d  _values.get('COM
-0000cdc0: 5041 4e59 2044 4154 4127 292e 6765 7428  PANY DATA').get(
-0000cdd0: 2743 4f4d 5041 4e59 2043 4f4e 464f 524d  'COMPANY CONFORM
-0000cde0: 4544 204e 414d 4527 292c 0a20 2020 2020  ED NAME'),.     
-0000cdf0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000ce00: 696b 3d69 7373 7565 725f 7661 6c75 6573  ik=issuer_values
-0000ce10: 2e67 6574 2827 434f 4d50 414e 5920 4441  .get('COMPANY DA
-0000ce20: 5441 2729 2e67 6574 2827 4345 4e54 5241  TA').get('CENTRA
-0000ce30: 4c20 494e 4445 5820 4b45 5927 292c 0a20  L INDEX KEY'),. 
-0000ce40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce50: 2020 2073 6963 3d69 7373 7565 725f 7661     sic=issuer_va
-0000ce60: 6c75 6573 2e67 6574 2827 434f 4d50 414e  lues.get('COMPAN
-0000ce70: 5920 4441 5441 2729 2e67 6574 2827 5354  Y DATA').get('ST
-0000ce80: 414e 4441 5244 2049 4e44 5553 5452 4941  ANDARD INDUSTRIA
-0000ce90: 4c20 434c 4153 5349 4649 4341 5449 4f4e  L CLASSIFICATION
-0000cea0: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-0000ceb0: 2020 2020 2020 2020 6972 735f 6e75 6d62          irs_numb
-0000cec0: 6572 3d69 7373 7565 725f 7661 6c75 6573  er=issuer_values
-0000ced0: 2e67 6574 2827 434f 4d50 414e 5920 4441  .get('COMPANY DA
-0000cee0: 5441 2729 2e67 6574 2827 4952 5320 4e55  TA').get('IRS NU
-0000cef0: 4d42 4552 2729 2c0a 2020 2020 2020 2020  MBER'),.        
-0000cf00: 2020 2020 2020 2020 2020 2020 7374 6174              stat
-0000cf10: 655f 6f66 5f69 6e63 6f72 706f 7261 7469  e_of_incorporati
-0000cf20: 6f6e 3d69 7373 7565 725f 7661 6c75 6573  on=issuer_values
-0000cf30: 2e67 6574 2827 434f 4d50 414e 5920 4441  .get('COMPANY DA
-0000cf40: 5441 2729 2e67 6574 2827 5354 4154 4520  TA').get('STATE 
-0000cf50: 4f46 2049 4e43 4f52 504f 5241 5449 4f4e  OF INCORPORATION
-0000cf60: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-0000cf70: 2020 2020 2020 2020 6669 7363 616c 5f79          fiscal_y
-0000cf80: 6561 725f 656e 643d 6973 7375 6572 5f76  ear_end=issuer_v
-0000cf90: 616c 7565 732e 6765 7428 2743 4f4d 5041  alues.get('COMPA
-0000cfa0: 4e59 2044 4154 4127 292e 6765 7428 2746  NY DATA').get('F
-0000cfb0: 4953 4341 4c20 5945 4152 2045 4e44 2729  ISCAL YEAR END')
-0000cfc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cfd0: 2029 2069 6620 2743 4f4d 5041 4e59 2044   ) if 'COMPANY D
-0000cfe0: 4154 4127 2069 6e20 6973 7375 6572 5f76  ATA' in issuer_v
-0000cff0: 616c 7565 7320 656c 7365 204e 6f6e 652c  alues else None,
-0000d000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d010: 2062 7573 696e 6573 735f 6164 6472 6573   business_addres
-0000d020: 733d 4164 6472 6573 7328 0a20 2020 2020  s=Address(.     
-0000d030: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000d040: 7472 6565 7431 3d69 7373 7565 725f 7661  treet1=issuer_va
-0000d050: 6c75 6573 2e67 6574 2827 4255 5349 4e45  lues.get('BUSINE
-0000d060: 5353 2041 4444 5245 5353 2729 2e67 6574  SS ADDRESS').get
-0000d070: 2827 5354 5245 4554 2031 2729 2c0a 2020  ('STREET 1'),.  
-0000d080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d090: 2020 7374 7265 6574 323d 6973 7375 6572    street2=issuer
-0000d0a0: 5f76 616c 7565 732e 6765 7428 2742 5553  _values.get('BUS
-0000d0b0: 494e 4553 5320 4144 4452 4553 5327 292e  INESS ADDRESS').
-0000d0c0: 6765 7428 2753 5452 4545 5420 3227 292c  get('STREET 2'),
-0000d0d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d0e0: 2020 2020 2063 6974 793d 6973 7375 6572       city=issuer
-0000d0f0: 5f76 616c 7565 732e 6765 7428 2742 5553  _values.get('BUS
-0000d100: 494e 4553 5320 4144 4452 4553 5327 292e  INESS ADDRESS').
-0000d110: 6765 7428 2743 4954 5927 292c 0a20 2020  get('CITY'),.   
-0000d120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d130: 2073 7461 7465 5f6f 725f 636f 756e 7472   state_or_countr
-0000d140: 793d 6973 7375 6572 5f76 616c 7565 732e  y=issuer_values.
-0000d150: 6765 7428 2742 5553 494e 4553 5320 4144  get('BUSINESS AD
-0000d160: 4452 4553 5327 292e 6765 7428 2753 5441  DRESS').get('STA
-0000d170: 5445 2729 2c0a 2020 2020 2020 2020 2020  TE'),.          
-0000d180: 2020 2020 2020 2020 2020 7a69 7063 6f64            zipcod
-0000d190: 653d 6973 7375 6572 5f76 616c 7565 732e  e=issuer_values.
-0000d1a0: 6765 7428 2742 5553 494e 4553 5320 4144  get('BUSINESS AD
-0000d1b0: 4452 4553 5327 292e 6765 7428 275a 4950  DRESS').get('ZIP
-0000d1c0: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-0000d1d0: 2020 2020 2920 6966 2027 4255 5349 4e45      ) if 'BUSINE
-0000d1e0: 5353 2041 4444 5245 5353 2720 696e 2069  SS ADDRESS' in i
-0000d1f0: 7373 7565 725f 7661 6c75 6573 2065 6c73  ssuer_values els
-0000d200: 6520 4e6f 6e65 2c0a 2020 2020 2020 2020  e None,.        
-0000d210: 2020 2020 2020 2020 6d61 696c 696e 675f          mailing_
-0000d220: 6164 6472 6573 733d 4164 6472 6573 7328  address=Address(
-0000d230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d240: 2020 2020 2073 7472 6565 7431 3d69 7373       street1=iss
-0000d250: 7565 725f 7661 6c75 6573 2e67 6574 2827  uer_values.get('
-0000d260: 4d41 494c 2041 4444 5245 5353 2729 2e67  MAIL ADDRESS').g
-0000d270: 6574 2827 5354 5245 4554 2031 2729 2c0a  et('STREET 1'),.
-0000d280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d290: 2020 2020 7374 7265 6574 323d 6973 7375      street2=issu
-0000d2a0: 6572 5f76 616c 7565 732e 6765 7428 274d  er_values.get('M
-0000d2b0: 4149 4c20 4144 4452 4553 5327 292e 6765  AIL ADDRESS').ge
-0000d2c0: 7428 2753 5452 4545 5420 3227 292c 0a20  t('STREET 2'),. 
-0000d2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2e0: 2020 2063 6974 793d 6973 7375 6572 5f76     city=issuer_v
-0000d2f0: 616c 7565 732e 6765 7428 274d 4149 4c20  alues.get('MAIL 
-0000d300: 4144 4452 4553 5327 292e 6765 7428 2743  ADDRESS').get('C
-0000d310: 4954 5927 292c 0a20 2020 2020 2020 2020  ITY'),.         
-0000d320: 2020 2020 2020 2020 2020 2073 7461 7465             state
-0000d330: 5f6f 725f 636f 756e 7472 793d 6973 7375  _or_country=issu
-0000d340: 6572 5f76 616c 7565 732e 6765 7428 274d  er_values.get('M
-0000d350: 4149 4c20 4144 4452 4553 5327 292e 6765  AIL ADDRESS').ge
-0000d360: 7428 2753 5441 5445 2729 2c0a 2020 2020  t('STATE'),.    
-0000d370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d380: 7a69 7063 6f64 653d 6973 7375 6572 5f76  zipcode=issuer_v
-0000d390: 616c 7565 732e 6765 7428 274d 4149 4c20  alues.get('MAIL 
-0000d3a0: 4144 4452 4553 5327 292e 6765 7428 275a  ADDRESS').get('Z
-0000d3b0: 4950 2729 2c0a 2020 2020 2020 2020 2020  IP'),.          
-0000d3c0: 2020 2020 2020 2920 6966 2027 4d41 494c        ) if 'MAIL
-0000d3d0: 2041 4444 5245 5353 2720 696e 2069 7373   ADDRESS' in iss
-0000d3e0: 7565 725f 7661 6c75 6573 2065 6c73 6520  uer_values else 
-0000d3f0: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-0000d400: 2029 0a20 2020 2020 2020 2020 2020 2069   ).            i
-0000d410: 7373 7565 7273 2e61 7070 656e 6428 6973  ssuers.append(is
-0000d420: 7375 6572 290a 0a20 2020 2020 2020 2073  suer)..        s
-0000d430: 7562 6a65 6374 5f63 6f6d 7061 6e69 6573  ubject_companies
-0000d440: 203d 205b 5d0a 2020 2020 2020 2020 666f   = [].        fo
-0000d450: 7220 7375 626a 6563 745f 636f 6d70 616e  r subject_compan
-0000d460: 795f 7661 6c75 6573 2069 6e20 6461 7461  y_values in data
-0000d470: 2e67 6574 2827 5355 424a 4543 5420 434f  .get('SUBJECT CO
-0000d480: 4d50 414e 5927 2c20 5b5d 293a 0a20 2020  MPANY', []):.   
-0000d490: 2020 2020 2020 2020 2073 7562 6a65 6374           subject
-0000d4a0: 5f63 6f6d 7061 6e79 203d 2053 7562 6a65  _company = Subje
-0000d4b0: 6374 436f 6d70 616e 7928 0a20 2020 2020  ctCompany(.     
-0000d4c0: 2020 2020 2020 2020 2020 2063 6f6d 7061             compa
-0000d4d0: 6e79 5f69 6e66 6f72 6d61 7469 6f6e 3d43  ny_information=C
-0000d4e0: 6f6d 7061 6e79 496e 666f 726d 6174 696f  ompanyInformatio
-0000d4f0: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
-0000d500: 2020 2020 2020 206e 616d 653d 7375 626a         name=subj
-0000d510: 6563 745f 636f 6d70 616e 795f 7661 6c75  ect_company_valu
-0000d520: 6573 2e67 6574 2827 434f 4d50 414e 5920  es.get('COMPANY 
-0000d530: 4441 5441 2729 2e67 6574 2827 434f 4d50  DATA').get('COMP
-0000d540: 414e 5920 434f 4e46 4f52 4d45 4420 4e41  ANY CONFORMED NA
-0000d550: 4d45 2729 2c0a 2020 2020 2020 2020 2020  ME'),.          
-0000d560: 2020 2020 2020 2020 2020 6369 6b3d 7375            cik=su
-0000d570: 626a 6563 745f 636f 6d70 616e 795f 7661  bject_company_va
-0000d580: 6c75 6573 2e67 6574 2827 434f 4d50 414e  lues.get('COMPAN
-0000d590: 5920 4441 5441 2729 2e67 6574 2827 4345  Y DATA').get('CE
-0000d5a0: 4e54 5241 4c20 494e 4445 5820 4b45 5927  NTRAL INDEX KEY'
-0000d5b0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000d5c0: 2020 2020 2020 2073 6963 3d73 7562 6a65         sic=subje
-0000d5d0: 6374 5f63 6f6d 7061 6e79 5f76 616c 7565  ct_company_value
-0000d5e0: 732e 6765 7428 2743 4f4d 5041 4e59 2044  s.get('COMPANY D
-0000d5f0: 4154 4127 292e 6765 7428 2753 5441 4e44  ATA').get('STAND
-0000d600: 4152 4420 494e 4455 5354 5249 414c 2043  ARD INDUSTRIAL C
-0000d610: 4c41 5353 4946 4943 4154 494f 4e27 292c  LASSIFICATION'),
-0000d620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d630: 2020 2020 2069 7273 5f6e 756d 6265 723d       irs_number=
-0000d640: 7375 626a 6563 745f 636f 6d70 616e 795f  subject_company_
-0000d650: 7661 6c75 6573 2e67 6574 2827 434f 4d50  values.get('COMP
-0000d660: 414e 5920 4441 5441 2729 2e67 6574 2827  ANY DATA').get('
-0000d670: 4952 5320 4e55 4d42 4552 2729 2c0a 2020  IRS NUMBER'),.  
-0000d680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d690: 2020 7374 6174 655f 6f66 5f69 6e63 6f72    state_of_incor
-0000d6a0: 706f 7261 7469 6f6e 3d73 7562 6a65 6374  poration=subject
-0000d6b0: 5f63 6f6d 7061 6e79 5f76 616c 7565 732e  _company_values.
-0000d6c0: 6765 7428 2743 4f4d 5041 4e59 2044 4154  get('COMPANY DAT
-0000d6d0: 4127 292e 6765 7428 2753 5441 5445 204f  A').get('STATE O
-0000d6e0: 4620 494e 434f 5250 4f52 4154 494f 4e27  F INCORPORATION'
-0000d6f0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000d700: 2020 2020 2020 2066 6973 6361 6c5f 7965         fiscal_ye
-0000d710: 6172 5f65 6e64 3d73 7562 6a65 6374 5f63  ar_end=subject_c
-0000d720: 6f6d 7061 6e79 5f76 616c 7565 732e 6765  ompany_values.ge
-0000d730: 7428 2743 4f4d 5041 4e59 2044 4154 4127  t('COMPANY DATA'
-0000d740: 292e 6765 7428 2746 4953 4341 4c20 5945  ).get('FISCAL YE
-0000d750: 4152 2045 4e44 2729 0a20 2020 2020 2020  AR END').       
-0000d760: 2020 2020 2020 2020 2029 2069 6620 2743           ) if 'C
-0000d770: 4f4d 5041 4e59 2044 4154 4127 2069 6e20  OMPANY DATA' in 
-0000d780: 7375 626a 6563 745f 636f 6d70 616e 795f  subject_company_
-0000d790: 7661 6c75 6573 2065 6c73 6520 4e6f 6e65  values else None
-0000d7a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000d7b0: 2020 6669 6c69 6e67 5f69 6e66 6f72 6d61    filing_informa
-0000d7c0: 7469 6f6e 3d46 696c 696e 6749 6e66 6f72  tion=FilingInfor
-0000d7d0: 6d61 7469 6f6e 280a 2020 2020 2020 2020  mation(.        
-0000d7e0: 2020 2020 2020 2020 2020 2020 666f 726d              form
-0000d7f0: 3d73 7562 6a65 6374 5f63 6f6d 7061 6e79  =subject_company
-0000d800: 5f76 616c 7565 732e 6765 7428 2746 494c  _values.get('FIL
-0000d810: 494e 4720 5641 4c55 4553 2729 2e67 6574  ING VALUES').get
-0000d820: 2827 464f 524d 2054 5950 4527 292c 0a20  ('FORM TYPE'),. 
-0000d830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d840: 2020 2073 6563 5f61 6374 3d73 7562 6a65     sec_act=subje
-0000d850: 6374 5f63 6f6d 7061 6e79 5f76 616c 7565  ct_company_value
-0000d860: 732e 6765 7428 2746 494c 494e 4720 5641  s.get('FILING VA
-0000d870: 4c55 4553 2729 2e67 6574 2827 5345 4320  LUES').get('SEC 
-0000d880: 4143 5427 292c 0a20 2020 2020 2020 2020  ACT'),.         
-0000d890: 2020 2020 2020 2020 2020 2066 696c 655f             file_
-0000d8a0: 6e75 6d62 6572 3d73 7562 6a65 6374 5f63  number=subject_c
-0000d8b0: 6f6d 7061 6e79 5f76 616c 7565 732e 6765  ompany_values.ge
-0000d8c0: 7428 2746 494c 494e 4720 5641 4c55 4553  t('FILING VALUES
-0000d8d0: 2729 2e67 6574 2827 5345 4320 4649 4c45  ').get('SEC FILE
-0000d8e0: 204e 554d 4245 5227 292c 0a20 2020 2020   NUMBER'),.     
-0000d8f0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000d900: 696c 6d5f 6e75 6d62 6572 3d73 7562 6a65  ilm_number=subje
-0000d910: 6374 5f63 6f6d 7061 6e79 5f76 616c 7565  ct_company_value
-0000d920: 732e 6765 7428 2746 494c 494e 4720 5641  s.get('FILING VA
-0000d930: 4c55 4553 2729 2e67 6574 2827 4649 4c4d  LUES').get('FILM
-0000d940: 204e 554d 4245 5227 290a 2020 2020 2020   NUMBER').      
-0000d950: 2020 2020 2020 2020 2020 2920 6966 2027            ) if '
-0000d960: 4649 4c49 4e47 2056 414c 5545 5327 2069  FILING VALUES' i
-0000d970: 6e20 7375 626a 6563 745f 636f 6d70 616e  n subject_compan
-0000d980: 795f 7661 6c75 6573 2065 6c73 6520 4e6f  y_values else No
-0000d990: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-0000d9a0: 2020 2020 6275 7369 6e65 7373 5f61 6464      business_add
-0000d9b0: 7265 7373 3d41 6464 7265 7373 280a 2020  ress=Address(.  
-0000d9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9d0: 2020 7374 7265 6574 313d 7375 626a 6563    street1=subjec
-0000d9e0: 745f 636f 6d70 616e 795f 7661 6c75 6573  t_company_values
-0000d9f0: 2e67 6574 2827 4255 5349 4e45 5353 2041  .get('BUSINESS A
-0000da00: 4444 5245 5353 2729 2e67 6574 2827 5354  DDRESS').get('ST
-0000da10: 5245 4554 2031 2729 2c0a 0a20 2020 2020  REET 1'),..     
-0000da20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000da30: 7472 6565 7432 3d73 7562 6a65 6374 5f63  treet2=subject_c
-0000da40: 6f6d 7061 6e79 5f76 616c 7565 732e 6765  ompany_values.ge
-0000da50: 7428 2742 5553 494e 4553 5320 4144 4452  t('BUSINESS ADDR
-0000da60: 4553 5327 292e 6765 7428 2753 5452 4545  ESS').get('STREE
-0000da70: 5420 3227 292c 0a20 2020 2020 2020 2020  T 2'),.         
-0000da80: 2020 2020 2020 2020 2020 2063 6974 793d             city=
-0000da90: 7375 626a 6563 745f 636f 6d70 616e 795f  subject_company_
-0000daa0: 7661 6c75 6573 2e67 6574 2827 4255 5349  values.get('BUSI
-0000dab0: 4e45 5353 2041 4444 5245 5353 2729 2e67  NESS ADDRESS').g
-0000dac0: 6574 2827 4349 5459 2729 2c0a 2020 2020  et('CITY'),.    
-0000dad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dae0: 7374 6174 655f 6f72 5f63 6f75 6e74 7279  state_or_country
-0000daf0: 3d73 7562 6a65 6374 5f63 6f6d 7061 6e79  =subject_company
-0000db00: 5f76 616c 7565 732e 6765 7428 2742 5553  _values.get('BUS
-0000db10: 494e 4553 5320 4144 4452 4553 5327 292e  INESS ADDRESS').
-0000db20: 6765 7428 2753 5441 5445 2729 2c0a 2020  get('STATE'),.  
-0000db30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db40: 2020 7a69 7063 6f64 653d 7375 626a 6563    zipcode=subjec
-0000db50: 745f 636f 6d70 616e 795f 7661 6c75 6573  t_company_values
-0000db60: 2e67 6574 2827 4255 5349 4e45 5353 2041  .get('BUSINESS A
-0000db70: 4444 5245 5353 2729 2e67 6574 2827 5a49  DDRESS').get('ZI
-0000db80: 5027 292c 0a20 2020 2020 2020 2020 2020  P'),.           
-0000db90: 2020 2020 2029 2069 6620 2742 5553 494e       ) if 'BUSIN
-0000dba0: 4553 5320 4144 4452 4553 5327 2069 6e20  ESS ADDRESS' in 
-0000dbb0: 7375 626a 6563 745f 636f 6d70 616e 795f  subject_company_
-0000dbc0: 7661 6c75 6573 2065 6c73 6520 4e6f 6e65  values else None
-0000dbd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000dbe0: 2020 6d61 696c 696e 675f 6164 6472 6573    mailing_addres
-0000dbf0: 733d 4164 6472 6573 7328 0a20 2020 2020  s=Address(.     
-0000dc00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000dc10: 7472 6565 7431 3d73 7562 6a65 6374 5f63  treet1=subject_c
-0000dc20: 6f6d 7061 6e79 5f76 616c 7565 732e 6765  ompany_values.ge
-0000dc30: 7428 274d 4149 4c20 4144 4452 4553 5327  t('MAIL ADDRESS'
-0000dc40: 292e 6765 7428 2753 5452 4545 5420 3127  ).get('STREET 1'
-0000dc50: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000dc60: 2020 2020 2020 2073 7472 6565 7432 3d73         street2=s
-0000dc70: 7562 6a65 6374 5f63 6f6d 7061 6e79 5f76  ubject_company_v
-0000dc80: 616c 7565 732e 6765 7428 274d 4149 4c20  alues.get('MAIL 
-0000dc90: 4144 4452 4553 5327 292e 6765 7428 2753  ADDRESS').get('S
-0000dca0: 5452 4545 5420 3227 292c 0a20 2020 2020  TREET 2'),.     
-0000dcb0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000dcc0: 6974 793d 7375 626a 6563 745f 636f 6d70  ity=subject_comp
-0000dcd0: 616e 795f 7661 6c75 6573 2e67 6574 2827  any_values.get('
-0000dce0: 4d41 494c 2041 4444 5245 5353 2729 2e67  MAIL ADDRESS').g
-0000dcf0: 6574 2827 4349 5459 2729 2c0a 2020 2020  et('CITY'),.    
-0000dd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd10: 7374 6174 655f 6f72 5f63 6f75 6e74 7279  state_or_country
-0000dd20: 3d73 7562 6a65 6374 5f63 6f6d 7061 6e79  =subject_company
-0000dd30: 5f76 616c 7565 732e 6765 7428 274d 4149  _values.get('MAI
-0000dd40: 4c20 4144 4452 4553 5327 292e 6765 7428  L ADDRESS').get(
-0000dd50: 2753 5441 5445 2729 2c0a 2020 2020 2020  'STATE'),.      
-0000dd60: 2020 2020 2020 2020 2020 2020 2020 7a69                zi
-0000dd70: 7063 6f64 653d 7375 626a 6563 745f 636f  pcode=subject_co
-0000dd80: 6d70 616e 795f 7661 6c75 6573 2e67 6574  mpany_values.get
-0000dd90: 2827 4d41 494c 2041 4444 5245 5353 2729  ('MAIL ADDRESS')
-0000dda0: 2e67 6574 2827 5a49 5027 292c 0a20 2020  .get('ZIP'),.   
-0000ddb0: 2020 2020 2020 2020 2020 2020 2029 2069               ) i
-0000ddc0: 6620 274d 4149 4c20 4144 4452 4553 5327  f 'MAIL ADDRESS'
-0000ddd0: 2069 6e20 7375 626a 6563 745f 636f 6d70   in subject_comp
-0000dde0: 616e 795f 7661 6c75 6573 2065 6c73 6520  any_values else 
-0000ddf0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-0000de00: 2020 2020 2020 666f 726d 6572 5f63 6f6d        former_com
-0000de10: 7061 6e79 5f6e 616d 6573 3d5b 466f 726d  pany_names=[Form
-0000de20: 6572 436f 6d70 616e 7928 6461 7465 5f6f  erCompany(date_o
-0000de30: 665f 6368 616e 6765 3d72 6563 6f72 642e  f_change=record.
-0000de40: 6765 7428 2744 4154 4520 4f46 204e 414d  get('DATE OF NAM
-0000de50: 4520 4348 414e 4745 2729 2c0a 2020 2020  E CHANGE'),.    
-0000de60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0b0: 2020 2020 206e 616d 6520 3d20 7265 7665       name = reve
+0000c0c0: 7273 655f 6e61 6d65 286e 616d 6529 0a20  rse_name(name). 
+0000c0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0e0: 2020 206f 776e 6572 203d 204f 776e 6572     owner = Owner
+0000c0f0: 286e 616d 653d 6e61 6d65 2c20 6369 6b3d  (name=name, cik=
+0000c100: 6369 6b29 0a0a 2020 2020 2020 2020 2020  cik)..          
+0000c110: 2020 2020 2020 2320 436f 6d70 616e 7920        # Company 
+0000c120: 496e 666f 726d 6174 696f 6e0a 2020 2020  Information.    
+0000c130: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
+0000c140: 616e 795f 696e 666f 726d 6174 696f 6e20  any_information 
+0000c150: 3d20 436f 6d70 616e 7949 6e66 6f72 6d61  = CompanyInforma
+0000c160: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
+0000c170: 2020 2020 2020 2020 2020 6e61 6d65 3d72            name=r
+0000c180: 6570 6f72 7469 6e67 5f6f 776e 6572 5f76  eporting_owner_v
+0000c190: 616c 7565 732e 6765 7428 2743 4f4d 5041  alues.get('COMPA
+0000c1a0: 4e59 2044 4154 4127 292e 6765 7428 2743  NY DATA').get('C
+0000c1b0: 4f4d 5041 4e59 2043 4f4e 464f 524d 4544  OMPANY CONFORMED
+0000c1c0: 204e 414d 4527 292c 0a20 2020 2020 2020   NAME'),.       
+0000c1d0: 2020 2020 2020 2020 2020 2020 2063 696b               cik
+0000c1e0: 3d72 6570 6f72 7469 6e67 5f6f 776e 6572  =reporting_owner
+0000c1f0: 5f76 616c 7565 732e 6765 7428 2743 4f4d  _values.get('COM
+0000c200: 5041 4e59 2044 4154 4127 292e 6765 7428  PANY DATA').get(
+0000c210: 2743 454e 5452 414c 2049 4e44 4558 204b  'CENTRAL INDEX K
+0000c220: 4559 2729 2c0a 2020 2020 2020 2020 2020  EY'),.          
+0000c230: 2020 2020 2020 2020 2020 7369 633d 7265            sic=re
+0000c240: 706f 7274 696e 675f 6f77 6e65 725f 7661  porting_owner_va
+0000c250: 6c75 6573 2e67 6574 2827 434f 4d50 414e  lues.get('COMPAN
+0000c260: 5920 4441 5441 2729 2e67 6574 2827 5354  Y DATA').get('ST
+0000c270: 414e 4441 5244 2049 4e44 5553 5452 4941  ANDARD INDUSTRIA
+0000c280: 4c20 434c 4153 5349 4649 4341 5449 4f4e  L CLASSIFICATION
+0000c290: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+0000c2a0: 2020 2020 2020 2020 6972 735f 6e75 6d62          irs_numb
+0000c2b0: 6572 3d72 6570 6f72 7469 6e67 5f6f 776e  er=reporting_own
+0000c2c0: 6572 5f76 616c 7565 732e 6765 7428 2743  er_values.get('C
+0000c2d0: 4f4d 5041 4e59 2044 4154 4127 292e 6765  OMPANY DATA').ge
+0000c2e0: 7428 2749 5253 204e 554d 4245 5227 292c  t('IRS NUMBER'),
+0000c2f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c300: 2020 2020 2073 7461 7465 5f6f 665f 696e       state_of_in
+0000c310: 636f 7270 6f72 6174 696f 6e3d 7265 706f  corporation=repo
+0000c320: 7274 696e 675f 6f77 6e65 725f 7661 6c75  rting_owner_valu
+0000c330: 6573 2e67 6574 2827 434f 4d50 414e 5920  es.get('COMPANY 
+0000c340: 4441 5441 2729 2e67 6574 2827 5354 4154  DATA').get('STAT
+0000c350: 4520 4f46 2049 4e43 4f52 504f 5241 5449  E OF INCORPORATI
+0000c360: 4f4e 2729 2c0a 2020 2020 2020 2020 2020  ON'),.          
+0000c370: 2020 2020 2020 2020 2020 6669 7363 616c            fiscal
+0000c380: 5f79 6561 725f 656e 643d 7265 706f 7274  _year_end=report
+0000c390: 696e 675f 6f77 6e65 725f 7661 6c75 6573  ing_owner_values
+0000c3a0: 2e67 6574 2827 434f 4d50 414e 5920 4441  .get('COMPANY DA
+0000c3b0: 5441 2729 2e67 6574 2827 4649 5343 414c  TA').get('FISCAL
+0000c3c0: 2059 4541 5220 454e 4427 290a 2020 2020   YEAR END').    
+0000c3d0: 2020 2020 2020 2020 2020 2020 2920 6966              ) if
+0000c3e0: 2022 434f 4d50 414e 5920 4441 5441 2220   "COMPANY DATA" 
+0000c3f0: 696e 2072 6570 6f72 7469 6e67 5f6f 776e  in reporting_own
+0000c400: 6572 5f76 616c 7565 7320 656c 7365 204e  er_values else N
+0000c410: 6f6e 650a 0a20 2020 2020 2020 2020 2020  one..           
+0000c420: 2020 2020 2023 2046 696c 696e 6720 496e       # Filing In
+0000c430: 666f 726d 6174 696f 6e0a 2020 2020 2020  formation.      
+0000c440: 2020 2020 2020 2020 2020 6669 6c69 6e67            filing
+0000c450: 5f69 6e66 6f72 6d61 7469 6f6e 203d 2046  _information = F
+0000c460: 696c 696e 6749 6e66 6f72 6d61 7469 6f6e  ilingInformation
+0000c470: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000c480: 2020 2020 2020 666f 726d 3d72 6570 6f72        form=repor
+0000c490: 7469 6e67 5f6f 776e 6572 5f76 616c 7565  ting_owner_value
+0000c4a0: 732e 6765 7428 2746 494c 494e 4720 5641  s.get('FILING VA
+0000c4b0: 4c55 4553 2729 2e67 6574 2827 464f 524d  LUES').get('FORM
+0000c4c0: 2054 5950 4527 292c 0a20 2020 2020 2020   TYPE'),.       
+0000c4d0: 2020 2020 2020 2020 2020 2020 2073 6563               sec
+0000c4e0: 5f61 6374 3d72 6570 6f72 7469 6e67 5f6f  _act=reporting_o
+0000c4f0: 776e 6572 5f76 616c 7565 732e 6765 7428  wner_values.get(
+0000c500: 2746 494c 494e 4720 5641 4c55 4553 2729  'FILING VALUES')
+0000c510: 2e67 6574 2827 5345 4320 4143 5427 292c  .get('SEC ACT'),
+0000c520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c530: 2020 2020 2066 696c 655f 6e75 6d62 6572       file_number
+0000c540: 3d72 6570 6f72 7469 6e67 5f6f 776e 6572  =reporting_owner
+0000c550: 5f76 616c 7565 732e 6765 7428 2746 494c  _values.get('FIL
+0000c560: 494e 4720 5641 4c55 4553 2729 2e67 6574  ING VALUES').get
+0000c570: 2827 5345 4320 4649 4c45 204e 554d 4245  ('SEC FILE NUMBE
+0000c580: 5227 292c 0a20 2020 2020 2020 2020 2020  R'),.           
+0000c590: 2020 2020 2020 2020 2066 696c 6d5f 6e75           film_nu
+0000c5a0: 6d62 6572 3d72 6570 6f72 7469 6e67 5f6f  mber=reporting_o
+0000c5b0: 776e 6572 5f76 616c 7565 732e 6765 7428  wner_values.get(
+0000c5c0: 2746 494c 494e 4720 5641 4c55 4553 2729  'FILING VALUES')
+0000c5d0: 2e67 6574 2827 4649 4c4d 204e 554d 4245  .get('FILM NUMBE
+0000c5e0: 5227 290a 2020 2020 2020 2020 2020 2020  R').            
+0000c5f0: 2020 2020 2920 6966 2028 2746 494c 494e      ) if ('FILIN
+0000c600: 4720 5641 4c55 4553 2720 696e 2072 6570  G VALUES' in rep
+0000c610: 6f72 7469 6e67 5f6f 776e 6572 5f76 616c  orting_owner_val
+0000c620: 7565 7320 616e 640a 2020 2020 2020 2020  ues and.        
+0000c630: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000c640: 706f 7274 696e 675f 6f77 6e65 725f 7661  porting_owner_va
+0000c650: 6c75 6573 2e67 6574 2827 4649 4c49 4e47  lues.get('FILING
+0000c660: 2056 414c 5545 5327 292e 6765 7428 2753   VALUES').get('S
+0000c670: 4543 2046 494c 4520 4e55 4d42 4552 2729  EC FILE NUMBER')
+0000c680: 2920 656c 7365 204e 6f6e 650a 0a20 2020  ) else None..   
+0000c690: 2020 2020 2020 2020 2020 2020 2023 2042               # B
+0000c6a0: 7573 696e 6573 7320 4164 6472 6573 730a  usiness Address.
+0000c6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6c0: 6275 7369 6e65 7373 5f61 6464 7265 7373  business_address
+0000c6d0: 203d 2041 6464 7265 7373 280a 2020 2020   = Address(.    
+0000c6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6f0: 7374 7265 6574 313d 7265 706f 7274 696e  street1=reportin
+0000c700: 675f 6f77 6e65 725f 7661 6c75 6573 2e67  g_owner_values.g
+0000c710: 6574 2827 4255 5349 4e45 5353 2041 4444  et('BUSINESS ADD
+0000c720: 5245 5353 2729 2e67 6574 2827 5354 5245  RESS').get('STRE
+0000c730: 4554 2031 2729 2c0a 2020 2020 2020 2020  ET 1'),.        
+0000c740: 2020 2020 2020 2020 2020 2020 7374 7265              stre
+0000c750: 6574 323d 7265 706f 7274 696e 675f 6f77  et2=reporting_ow
+0000c760: 6e65 725f 7661 6c75 6573 2e67 6574 2827  ner_values.get('
+0000c770: 4255 5349 4e45 5353 2041 4444 5245 5353  BUSINESS ADDRESS
+0000c780: 2729 2e67 6574 2827 5354 5245 4554 2032  ').get('STREET 2
+0000c790: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+0000c7a0: 2020 2020 2020 2020 6369 7479 3d72 6570          city=rep
+0000c7b0: 6f72 7469 6e67 5f6f 776e 6572 5f76 616c  orting_owner_val
+0000c7c0: 7565 732e 6765 7428 2742 5553 494e 4553  ues.get('BUSINES
+0000c7d0: 5320 4144 4452 4553 5327 292e 6765 7428  S ADDRESS').get(
+0000c7e0: 2743 4954 5927 292c 0a20 2020 2020 2020  'CITY'),.       
+0000c7f0: 2020 2020 2020 2020 2020 2020 2073 7461               sta
+0000c800: 7465 5f6f 725f 636f 756e 7472 793d 7265  te_or_country=re
+0000c810: 706f 7274 696e 675f 6f77 6e65 725f 7661  porting_owner_va
+0000c820: 6c75 6573 2e67 6574 2827 4255 5349 4e45  lues.get('BUSINE
+0000c830: 5353 2041 4444 5245 5353 2729 2e67 6574  SS ADDRESS').get
+0000c840: 2827 5354 4154 4527 292c 0a20 2020 2020  ('STATE'),.     
+0000c850: 2020 2020 2020 2020 2020 2020 2020 207a                 z
+0000c860: 6970 636f 6465 3d72 6570 6f72 7469 6e67  ipcode=reporting
+0000c870: 5f6f 776e 6572 5f76 616c 7565 732e 6765  _owner_values.ge
+0000c880: 7428 2742 5553 494e 4553 5320 4144 4452  t('BUSINESS ADDR
+0000c890: 4553 5327 292e 6765 7428 275a 4950 2729  ESS').get('ZIP')
+0000c8a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000c8b0: 2020 2920 6966 2027 4255 5349 4e45 5353    ) if 'BUSINESS
+0000c8c0: 2041 4444 5245 5353 2720 696e 2072 6570   ADDRESS' in rep
+0000c8d0: 6f72 7469 6e67 5f6f 776e 6572 5f76 616c  orting_owner_val
+0000c8e0: 7565 7320 656c 7365 204e 6f6e 650a 0a20  ues else None.. 
+0000c8f0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000c900: 204d 6169 6c69 6e67 2041 6464 7265 7373   Mailing Address
+0000c910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c920: 206d 6169 6c69 6e67 5f61 6464 7265 7373   mailing_address
+0000c930: 203d 2041 6464 7265 7373 280a 2020 2020   = Address(.    
+0000c940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c950: 7374 7265 6574 313d 7265 706f 7274 696e  street1=reportin
+0000c960: 675f 6f77 6e65 725f 7661 6c75 6573 2e67  g_owner_values.g
+0000c970: 6574 2827 4d41 494c 2041 4444 5245 5353  et('MAIL ADDRESS
+0000c980: 2729 2e67 6574 2827 5354 5245 4554 2031  ').get('STREET 1
+0000c990: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+0000c9a0: 2020 2020 2020 2020 7374 7265 6574 323d          street2=
+0000c9b0: 7265 706f 7274 696e 675f 6f77 6e65 725f  reporting_owner_
+0000c9c0: 7661 6c75 6573 2e67 6574 2827 4d41 494c  values.get('MAIL
+0000c9d0: 2041 4444 5245 5353 2729 2e67 6574 2827   ADDRESS').get('
+0000c9e0: 5354 5245 4554 2032 2729 2c0a 2020 2020  STREET 2'),.    
+0000c9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca00: 6369 7479 3d72 6570 6f72 7469 6e67 5f6f  city=reporting_o
+0000ca10: 776e 6572 5f76 616c 7565 732e 6765 7428  wner_values.get(
+0000ca20: 274d 4149 4c20 4144 4452 4553 5327 292e  'MAIL ADDRESS').
+0000ca30: 6765 7428 2743 4954 5927 292c 0a20 2020  get('CITY'),.   
+0000ca40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca50: 2073 7461 7465 5f6f 725f 636f 756e 7472   state_or_countr
+0000ca60: 793d 7265 706f 7274 696e 675f 6f77 6e65  y=reporting_owne
+0000ca70: 725f 7661 6c75 6573 2e67 6574 2827 4d41  r_values.get('MA
+0000ca80: 494c 2041 4444 5245 5353 2729 2e67 6574  IL ADDRESS').get
+0000ca90: 2827 5354 4154 4527 292c 0a20 2020 2020  ('STATE'),.     
+0000caa0: 2020 2020 2020 2020 2020 2020 2020 207a                 z
+0000cab0: 6970 636f 6465 3d72 6570 6f72 7469 6e67  ipcode=reporting
+0000cac0: 5f6f 776e 6572 5f76 616c 7565 732e 6765  _owner_values.ge
+0000cad0: 7428 274d 4149 4c20 4144 4452 4553 5327  t('MAIL ADDRESS'
+0000cae0: 292e 6765 7428 275a 4950 2729 2c0a 2020  ).get('ZIP'),.  
+0000caf0: 2020 2020 2020 2020 2020 2020 2020 2920                ) 
+0000cb00: 6966 2027 4d41 494c 2041 4444 5245 5353  if 'MAIL ADDRESS
+0000cb10: 2720 696e 2072 6570 6f72 7469 6e67 5f6f  ' in reporting_o
+0000cb20: 776e 6572 5f76 616c 7565 7320 656c 7365  wner_values else
+0000cb30: 204e 6f6e 650a 0a20 2020 2020 2020 2020   None..         
+0000cb40: 2020 2020 2020 2023 204e 6f77 2063 7265         # Now cre
+0000cb50: 6174 6520 7468 6520 7265 706f 7274 696e  ate the reportin
+0000cb60: 6720 6f77 6e65 720a 2020 2020 2020 2020  g owner.        
+0000cb70: 2020 2020 2020 2020 7265 706f 7274 696e          reportin
+0000cb80: 675f 6f77 6e65 7220 3d20 5265 706f 7274  g_owner = Report
+0000cb90: 696e 674f 776e 6572 280a 2020 2020 2020  ingOwner(.      
+0000cba0: 2020 2020 2020 2020 2020 2020 2020 6f77                ow
+0000cbb0: 6e65 723d 6f77 6e65 722c 0a20 2020 2020  ner=owner,.     
+0000cbc0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000cbd0: 6f6d 7061 6e79 5f69 6e66 6f72 6d61 7469  ompany_informati
+0000cbe0: 6f6e 3d63 6f6d 7061 6e79 5f69 6e66 6f72  on=company_infor
+0000cbf0: 6d61 7469 6f6e 2c0a 2020 2020 2020 2020  mation,.        
+0000cc00: 2020 2020 2020 2020 2020 2020 6669 6c69              fili
+0000cc10: 6e67 5f69 6e66 6f72 6d61 7469 6f6e 3d66  ng_information=f
+0000cc20: 696c 696e 675f 696e 666f 726d 6174 696f  iling_informatio
+0000cc30: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
+0000cc40: 2020 2020 2020 2062 7573 696e 6573 735f         business_
+0000cc50: 6164 6472 6573 733d 6275 7369 6e65 7373  address=business
+0000cc60: 5f61 6464 7265 7373 2c0a 2020 2020 2020  _address,.      
+0000cc70: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+0000cc80: 696c 696e 675f 6164 6472 6573 733d 6d61  iling_address=ma
+0000cc90: 696c 696e 675f 6164 6472 6573 730a 2020  iling_address.  
+0000cca0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000ccb0: 2020 2020 2020 2020 2020 2020 7265 706f              repo
+0000ccc0: 7274 696e 675f 6f77 6e65 7273 2e61 7070  rting_owners.app
+0000ccd0: 656e 6428 7265 706f 7274 696e 675f 6f77  end(reporting_ow
+0000cce0: 6e65 7229 0a0a 2020 2020 2020 2020 2320  ner)..        # 
+0000ccf0: 4973 7375 6572 0a20 2020 2020 2020 2069  Issuer.        i
+0000cd00: 7373 7565 7273 203d 205b 5d0a 2020 2020  ssuers = [].    
+0000cd10: 2020 2020 666f 7220 6973 7375 6572 5f76      for issuer_v
+0000cd20: 616c 7565 7320 696e 2064 6174 612e 6765  alues in data.ge
+0000cd30: 7428 2749 5353 5545 5227 2c20 5b5d 293a  t('ISSUER', []):
+0000cd40: 0a20 2020 2020 2020 2020 2020 2069 7373  .            iss
+0000cd50: 7565 7220 3d20 4973 7375 6572 280a 2020  uer = Issuer(.  
+0000cd60: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0000cd70: 6d70 616e 795f 696e 666f 726d 6174 696f  mpany_informatio
+0000cd80: 6e3d 436f 6d70 616e 7949 6e66 6f72 6d61  n=CompanyInforma
+0000cd90: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
+0000cda0: 2020 2020 2020 2020 2020 6e61 6d65 3d69            name=i
+0000cdb0: 7373 7565 725f 7661 6c75 6573 2e67 6574  ssuer_values.get
+0000cdc0: 2827 434f 4d50 414e 5920 4441 5441 2729  ('COMPANY DATA')
+0000cdd0: 2e67 6574 2827 434f 4d50 414e 5920 434f  .get('COMPANY CO
+0000cde0: 4e46 4f52 4d45 4420 4e41 4d45 2729 2c0a  NFORMED NAME'),.
+0000cdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce00: 2020 2020 6369 6b3d 6973 7375 6572 5f76      cik=issuer_v
+0000ce10: 616c 7565 732e 6765 7428 2743 4f4d 5041  alues.get('COMPA
+0000ce20: 4e59 2044 4154 4127 292e 6765 7428 2743  NY DATA').get('C
+0000ce30: 454e 5452 414c 2049 4e44 4558 204b 4559  ENTRAL INDEX KEY
+0000ce40: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+0000ce50: 2020 2020 2020 2020 7369 633d 6973 7375          sic=issu
+0000ce60: 6572 5f76 616c 7565 732e 6765 7428 2743  er_values.get('C
+0000ce70: 4f4d 5041 4e59 2044 4154 4127 292e 6765  OMPANY DATA').ge
+0000ce80: 7428 2753 5441 4e44 4152 4420 494e 4455  t('STANDARD INDU
+0000ce90: 5354 5249 414c 2043 4c41 5353 4946 4943  STRIAL CLASSIFIC
+0000cea0: 4154 494f 4e27 292c 0a20 2020 2020 2020  ATION'),.       
+0000ceb0: 2020 2020 2020 2020 2020 2020 2069 7273               irs
+0000cec0: 5f6e 756d 6265 723d 6973 7375 6572 5f76  _number=issuer_v
+0000ced0: 616c 7565 732e 6765 7428 2743 4f4d 5041  alues.get('COMPA
+0000cee0: 4e59 2044 4154 4127 292e 6765 7428 2749  NY DATA').get('I
+0000cef0: 5253 204e 554d 4245 5227 292c 0a20 2020  RS NUMBER'),.   
+0000cf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf10: 2073 7461 7465 5f6f 665f 696e 636f 7270   state_of_incorp
+0000cf20: 6f72 6174 696f 6e3d 6973 7375 6572 5f76  oration=issuer_v
+0000cf30: 616c 7565 732e 6765 7428 2743 4f4d 5041  alues.get('COMPA
+0000cf40: 4e59 2044 4154 4127 292e 6765 7428 2753  NY DATA').get('S
+0000cf50: 5441 5445 204f 4620 494e 434f 5250 4f52  TATE OF INCORPOR
+0000cf60: 4154 494f 4e27 292c 0a20 2020 2020 2020  ATION'),.       
+0000cf70: 2020 2020 2020 2020 2020 2020 2066 6973               fis
+0000cf80: 6361 6c5f 7965 6172 5f65 6e64 3d69 7373  cal_year_end=iss
+0000cf90: 7565 725f 7661 6c75 6573 2e67 6574 2827  uer_values.get('
+0000cfa0: 434f 4d50 414e 5920 4441 5441 2729 2e67  COMPANY DATA').g
+0000cfb0: 6574 2827 4649 5343 414c 2059 4541 5220  et('FISCAL YEAR 
+0000cfc0: 454e 4427 290a 2020 2020 2020 2020 2020  END').          
+0000cfd0: 2020 2020 2020 2920 6966 2027 434f 4d50        ) if 'COMP
+0000cfe0: 414e 5920 4441 5441 2720 696e 2069 7373  ANY DATA' in iss
+0000cff0: 7565 725f 7661 6c75 6573 2065 6c73 6520  uer_values else 
+0000d000: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+0000d010: 2020 2020 2020 6275 7369 6e65 7373 5f61        business_a
+0000d020: 6464 7265 7373 3d41 6464 7265 7373 280a  ddress=Address(.
+0000d030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d040: 2020 2020 7374 7265 6574 313d 6973 7375      street1=issu
+0000d050: 6572 5f76 616c 7565 732e 6765 7428 2742  er_values.get('B
+0000d060: 5553 494e 4553 5320 4144 4452 4553 5327  USINESS ADDRESS'
+0000d070: 292e 6765 7428 2753 5452 4545 5420 3127  ).get('STREET 1'
+0000d080: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0000d090: 2020 2020 2020 2073 7472 6565 7432 3d69         street2=i
+0000d0a0: 7373 7565 725f 7661 6c75 6573 2e67 6574  ssuer_values.get
+0000d0b0: 2827 4255 5349 4e45 5353 2041 4444 5245  ('BUSINESS ADDRE
+0000d0c0: 5353 2729 2e67 6574 2827 5354 5245 4554  SS').get('STREET
+0000d0d0: 2032 2729 2c0a 2020 2020 2020 2020 2020   2'),.          
+0000d0e0: 2020 2020 2020 2020 2020 6369 7479 3d69            city=i
+0000d0f0: 7373 7565 725f 7661 6c75 6573 2e67 6574  ssuer_values.get
+0000d100: 2827 4255 5349 4e45 5353 2041 4444 5245  ('BUSINESS ADDRE
+0000d110: 5353 2729 2e67 6574 2827 4349 5459 2729  SS').get('CITY')
+0000d120: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000d130: 2020 2020 2020 7374 6174 655f 6f72 5f63        state_or_c
+0000d140: 6f75 6e74 7279 3d69 7373 7565 725f 7661  ountry=issuer_va
+0000d150: 6c75 6573 2e67 6574 2827 4255 5349 4e45  lues.get('BUSINE
+0000d160: 5353 2041 4444 5245 5353 2729 2e67 6574  SS ADDRESS').get
+0000d170: 2827 5354 4154 4527 292c 0a20 2020 2020  ('STATE'),.     
+0000d180: 2020 2020 2020 2020 2020 2020 2020 207a                 z
+0000d190: 6970 636f 6465 3d69 7373 7565 725f 7661  ipcode=issuer_va
+0000d1a0: 6c75 6573 2e67 6574 2827 4255 5349 4e45  lues.get('BUSINE
+0000d1b0: 5353 2041 4444 5245 5353 2729 2e67 6574  SS ADDRESS').get
+0000d1c0: 2827 5a49 5027 292c 0a20 2020 2020 2020  ('ZIP'),.       
+0000d1d0: 2020 2020 2020 2020 2029 2069 6620 2742           ) if 'B
+0000d1e0: 5553 494e 4553 5320 4144 4452 4553 5327  USINESS ADDRESS'
+0000d1f0: 2069 6e20 6973 7375 6572 5f76 616c 7565   in issuer_value
+0000d200: 7320 656c 7365 204e 6f6e 652c 0a20 2020  s else None,.   
+0000d210: 2020 2020 2020 2020 2020 2020 206d 6169               mai
+0000d220: 6c69 6e67 5f61 6464 7265 7373 3d41 6464  ling_address=Add
+0000d230: 7265 7373 280a 2020 2020 2020 2020 2020  ress(.          
+0000d240: 2020 2020 2020 2020 2020 7374 7265 6574            street
+0000d250: 313d 6973 7375 6572 5f76 616c 7565 732e  1=issuer_values.
+0000d260: 6765 7428 274d 4149 4c20 4144 4452 4553  get('MAIL ADDRES
+0000d270: 5327 292e 6765 7428 2753 5452 4545 5420  S').get('STREET 
+0000d280: 3127 292c 0a20 2020 2020 2020 2020 2020  1'),.           
+0000d290: 2020 2020 2020 2020 2073 7472 6565 7432           street2
+0000d2a0: 3d69 7373 7565 725f 7661 6c75 6573 2e67  =issuer_values.g
+0000d2b0: 6574 2827 4d41 494c 2041 4444 5245 5353  et('MAIL ADDRESS
+0000d2c0: 2729 2e67 6574 2827 5354 5245 4554 2032  ').get('STREET 2
+0000d2d0: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+0000d2e0: 2020 2020 2020 2020 6369 7479 3d69 7373          city=iss
+0000d2f0: 7565 725f 7661 6c75 6573 2e67 6574 2827  uer_values.get('
+0000d300: 4d41 494c 2041 4444 5245 5353 2729 2e67  MAIL ADDRESS').g
+0000d310: 6574 2827 4349 5459 2729 2c0a 2020 2020  et('CITY'),.    
+0000d320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d330: 7374 6174 655f 6f72 5f63 6f75 6e74 7279  state_or_country
+0000d340: 3d69 7373 7565 725f 7661 6c75 6573 2e67  =issuer_values.g
+0000d350: 6574 2827 4d41 494c 2041 4444 5245 5353  et('MAIL ADDRESS
+0000d360: 2729 2e67 6574 2827 5354 4154 4527 292c  ').get('STATE'),
+0000d370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d380: 2020 2020 207a 6970 636f 6465 3d69 7373       zipcode=iss
+0000d390: 7565 725f 7661 6c75 6573 2e67 6574 2827  uer_values.get('
+0000d3a0: 4d41 494c 2041 4444 5245 5353 2729 2e67  MAIL ADDRESS').g
+0000d3b0: 6574 2827 5a49 5027 292c 0a20 2020 2020  et('ZIP'),.     
+0000d3c0: 2020 2020 2020 2020 2020 2029 2069 6620             ) if 
+0000d3d0: 274d 4149 4c20 4144 4452 4553 5327 2069  'MAIL ADDRESS' i
+0000d3e0: 6e20 6973 7375 6572 5f76 616c 7565 7320  n issuer_values 
+0000d3f0: 656c 7365 204e 6f6e 650a 2020 2020 2020  else None.      
+0000d400: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000d410: 2020 2020 6973 7375 6572 732e 6170 7065      issuers.appe
+0000d420: 6e64 2869 7373 7565 7229 0a0a 2020 2020  nd(issuer)..    
+0000d430: 2020 2020 7375 626a 6563 745f 636f 6d70      subject_comp
+0000d440: 616e 6965 7320 3d20 5b5d 0a20 2020 2020  anies = [].     
+0000d450: 2020 2066 6f72 2073 7562 6a65 6374 5f63     for subject_c
+0000d460: 6f6d 7061 6e79 5f76 616c 7565 7320 696e  ompany_values in
+0000d470: 2064 6174 612e 6765 7428 2753 5542 4a45   data.get('SUBJE
+0000d480: 4354 2043 4f4d 5041 4e59 272c 205b 5d29  CT COMPANY', [])
+0000d490: 3a0a 2020 2020 2020 2020 2020 2020 7375  :.            su
+0000d4a0: 626a 6563 745f 636f 6d70 616e 7920 3d20  bject_company = 
+0000d4b0: 5375 626a 6563 7443 6f6d 7061 6e79 280a  SubjectCompany(.
+0000d4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4d0: 636f 6d70 616e 795f 696e 666f 726d 6174  company_informat
+0000d4e0: 696f 6e3d 436f 6d70 616e 7949 6e66 6f72  ion=CompanyInfor
+0000d4f0: 6d61 7469 6f6e 280a 2020 2020 2020 2020  mation(.        
+0000d500: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+0000d510: 3d73 7562 6a65 6374 5f63 6f6d 7061 6e79  =subject_company
+0000d520: 5f76 616c 7565 732e 6765 7428 2743 4f4d  _values.get('COM
+0000d530: 5041 4e59 2044 4154 4127 292e 6765 7428  PANY DATA').get(
+0000d540: 2743 4f4d 5041 4e59 2043 4f4e 464f 524d  'COMPANY CONFORM
+0000d550: 4544 204e 414d 4527 292c 0a20 2020 2020  ED NAME'),.     
+0000d560: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000d570: 696b 3d73 7562 6a65 6374 5f63 6f6d 7061  ik=subject_compa
+0000d580: 6e79 5f76 616c 7565 732e 6765 7428 2743  ny_values.get('C
+0000d590: 4f4d 5041 4e59 2044 4154 4127 292e 6765  OMPANY DATA').ge
+0000d5a0: 7428 2743 454e 5452 414c 2049 4e44 4558  t('CENTRAL INDEX
+0000d5b0: 204b 4559 2729 2c0a 2020 2020 2020 2020   KEY'),.        
+0000d5c0: 2020 2020 2020 2020 2020 2020 7369 633d              sic=
+0000d5d0: 7375 626a 6563 745f 636f 6d70 616e 795f  subject_company_
+0000d5e0: 7661 6c75 6573 2e67 6574 2827 434f 4d50  values.get('COMP
+0000d5f0: 414e 5920 4441 5441 2729 2e67 6574 2827  ANY DATA').get('
+0000d600: 5354 414e 4441 5244 2049 4e44 5553 5452  STANDARD INDUSTR
+0000d610: 4941 4c20 434c 4153 5349 4649 4341 5449  IAL CLASSIFICATI
+0000d620: 4f4e 2729 2c0a 2020 2020 2020 2020 2020  ON'),.          
+0000d630: 2020 2020 2020 2020 2020 6972 735f 6e75            irs_nu
+0000d640: 6d62 6572 3d73 7562 6a65 6374 5f63 6f6d  mber=subject_com
+0000d650: 7061 6e79 5f76 616c 7565 732e 6765 7428  pany_values.get(
+0000d660: 2743 4f4d 5041 4e59 2044 4154 4127 292e  'COMPANY DATA').
+0000d670: 6765 7428 2749 5253 204e 554d 4245 5227  get('IRS NUMBER'
+0000d680: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0000d690: 2020 2020 2020 2073 7461 7465 5f6f 665f         state_of_
+0000d6a0: 696e 636f 7270 6f72 6174 696f 6e3d 7375  incorporation=su
+0000d6b0: 626a 6563 745f 636f 6d70 616e 795f 7661  bject_company_va
+0000d6c0: 6c75 6573 2e67 6574 2827 434f 4d50 414e  lues.get('COMPAN
+0000d6d0: 5920 4441 5441 2729 2e67 6574 2827 5354  Y DATA').get('ST
+0000d6e0: 4154 4520 4f46 2049 4e43 4f52 504f 5241  ATE OF INCORPORA
+0000d6f0: 5449 4f4e 2729 2c0a 2020 2020 2020 2020  TION'),.        
+0000d700: 2020 2020 2020 2020 2020 2020 6669 7363              fisc
+0000d710: 616c 5f79 6561 725f 656e 643d 7375 626a  al_year_end=subj
+0000d720: 6563 745f 636f 6d70 616e 795f 7661 6c75  ect_company_valu
+0000d730: 6573 2e67 6574 2827 434f 4d50 414e 5920  es.get('COMPANY 
+0000d740: 4441 5441 2729 2e67 6574 2827 4649 5343  DATA').get('FISC
+0000d750: 414c 2059 4541 5220 454e 4427 290a 2020  AL YEAR END').  
+0000d760: 2020 2020 2020 2020 2020 2020 2020 2920                ) 
+0000d770: 6966 2027 434f 4d50 414e 5920 4441 5441  if 'COMPANY DATA
+0000d780: 2720 696e 2073 7562 6a65 6374 5f63 6f6d  ' in subject_com
+0000d790: 7061 6e79 5f76 616c 7565 7320 656c 7365  pany_values else
+0000d7a0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+0000d7b0: 2020 2020 2020 2066 696c 696e 675f 696e         filing_in
+0000d7c0: 666f 726d 6174 696f 6e3d 4669 6c69 6e67  formation=Filing
+0000d7d0: 496e 666f 726d 6174 696f 6e28 0a20 2020  Information(.   
+0000d7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7f0: 2066 6f72 6d3d 7375 626a 6563 745f 636f   form=subject_co
+0000d800: 6d70 616e 795f 7661 6c75 6573 2e67 6574  mpany_values.get
+0000d810: 2827 4649 4c49 4e47 2056 414c 5545 5327  ('FILING VALUES'
+0000d820: 292e 6765 7428 2746 4f52 4d20 5459 5045  ).get('FORM TYPE
+0000d830: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+0000d840: 2020 2020 2020 2020 7365 635f 6163 743d          sec_act=
+0000d850: 7375 626a 6563 745f 636f 6d70 616e 795f  subject_company_
+0000d860: 7661 6c75 6573 2e67 6574 2827 4649 4c49  values.get('FILI
+0000d870: 4e47 2056 414c 5545 5327 292e 6765 7428  NG VALUES').get(
+0000d880: 2753 4543 2041 4354 2729 2c0a 2020 2020  'SEC ACT'),.    
+0000d890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d8a0: 6669 6c65 5f6e 756d 6265 723d 7375 626a  file_number=subj
+0000d8b0: 6563 745f 636f 6d70 616e 795f 7661 6c75  ect_company_valu
+0000d8c0: 6573 2e67 6574 2827 4649 4c49 4e47 2056  es.get('FILING V
+0000d8d0: 414c 5545 5327 292e 6765 7428 2753 4543  ALUES').get('SEC
+0000d8e0: 2046 494c 4520 4e55 4d42 4552 2729 2c0a   FILE NUMBER'),.
+0000d8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d900: 2020 2020 6669 6c6d 5f6e 756d 6265 723d      film_number=
+0000d910: 7375 626a 6563 745f 636f 6d70 616e 795f  subject_company_
+0000d920: 7661 6c75 6573 2e67 6574 2827 4649 4c49  values.get('FILI
+0000d930: 4e47 2056 414c 5545 5327 292e 6765 7428  NG VALUES').get(
+0000d940: 2746 494c 4d20 4e55 4d42 4552 2729 0a20  'FILM NUMBER'). 
+0000d950: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000d960: 2069 6620 2746 494c 494e 4720 5641 4c55   if 'FILING VALU
+0000d970: 4553 2720 696e 2073 7562 6a65 6374 5f63  ES' in subject_c
+0000d980: 6f6d 7061 6e79 5f76 616c 7565 7320 656c  ompany_values el
+0000d990: 7365 204e 6f6e 652c 0a20 2020 2020 2020  se None,.       
+0000d9a0: 2020 2020 2020 2020 2062 7573 696e 6573           busines
+0000d9b0: 735f 6164 6472 6573 733d 4164 6472 6573  s_address=Addres
+0000d9c0: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
+0000d9d0: 2020 2020 2020 2073 7472 6565 7431 3d73         street1=s
+0000d9e0: 7562 6a65 6374 5f63 6f6d 7061 6e79 5f76  ubject_company_v
+0000d9f0: 616c 7565 732e 6765 7428 2742 5553 494e  alues.get('BUSIN
+0000da00: 4553 5320 4144 4452 4553 5327 292e 6765  ESS ADDRESS').ge
+0000da10: 7428 2753 5452 4545 5420 3127 292c 0a0a  t('STREET 1'),..
+0000da20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da30: 2020 2020 7374 7265 6574 323d 7375 626a      street2=subj
+0000da40: 6563 745f 636f 6d70 616e 795f 7661 6c75  ect_company_valu
+0000da50: 6573 2e67 6574 2827 4255 5349 4e45 5353  es.get('BUSINESS
+0000da60: 2041 4444 5245 5353 2729 2e67 6574 2827   ADDRESS').get('
+0000da70: 5354 5245 4554 2032 2729 2c0a 2020 2020  STREET 2'),.    
+0000da80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da90: 6369 7479 3d73 7562 6a65 6374 5f63 6f6d  city=subject_com
+0000daa0: 7061 6e79 5f76 616c 7565 732e 6765 7428  pany_values.get(
+0000dab0: 2742 5553 494e 4553 5320 4144 4452 4553  'BUSINESS ADDRES
+0000dac0: 5327 292e 6765 7428 2743 4954 5927 292c  S').get('CITY'),
+0000dad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dae0: 2020 2020 2073 7461 7465 5f6f 725f 636f       state_or_co
+0000daf0: 756e 7472 793d 7375 626a 6563 745f 636f  untry=subject_co
+0000db00: 6d70 616e 795f 7661 6c75 6573 2e67 6574  mpany_values.get
+0000db10: 2827 4255 5349 4e45 5353 2041 4444 5245  ('BUSINESS ADDRE
+0000db20: 5353 2729 2e67 6574 2827 5354 4154 4527  SS').get('STATE'
+0000db30: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0000db40: 2020 2020 2020 207a 6970 636f 6465 3d73         zipcode=s
+0000db50: 7562 6a65 6374 5f63 6f6d 7061 6e79 5f76  ubject_company_v
+0000db60: 616c 7565 732e 6765 7428 2742 5553 494e  alues.get('BUSIN
+0000db70: 4553 5320 4144 4452 4553 5327 292e 6765  ESS ADDRESS').ge
+0000db80: 7428 275a 4950 2729 2c0a 2020 2020 2020  t('ZIP'),.      
+0000db90: 2020 2020 2020 2020 2020 2920 6966 2027            ) if '
+0000dba0: 4255 5349 4e45 5353 2041 4444 5245 5353  BUSINESS ADDRESS
+0000dbb0: 2720 696e 2073 7562 6a65 6374 5f63 6f6d  ' in subject_com
+0000dbc0: 7061 6e79 5f76 616c 7565 7320 656c 7365  pany_values else
+0000dbd0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+0000dbe0: 2020 2020 2020 206d 6169 6c69 6e67 5f61         mailing_a
+0000dbf0: 6464 7265 7373 3d41 6464 7265 7373 280a  ddress=Address(.
+0000dc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc10: 2020 2020 7374 7265 6574 313d 7375 626a      street1=subj
+0000dc20: 6563 745f 636f 6d70 616e 795f 7661 6c75  ect_company_valu
+0000dc30: 6573 2e67 6574 2827 4d41 494c 2041 4444  es.get('MAIL ADD
+0000dc40: 5245 5353 2729 2e67 6574 2827 5354 5245  RESS').get('STRE
+0000dc50: 4554 2031 2729 2c0a 2020 2020 2020 2020  ET 1'),.        
+0000dc60: 2020 2020 2020 2020 2020 2020 7374 7265              stre
+0000dc70: 6574 323d 7375 626a 6563 745f 636f 6d70  et2=subject_comp
+0000dc80: 616e 795f 7661 6c75 6573 2e67 6574 2827  any_values.get('
+0000dc90: 4d41 494c 2041 4444 5245 5353 2729 2e67  MAIL ADDRESS').g
+0000dca0: 6574 2827 5354 5245 4554 2032 2729 2c0a  et('STREET 2'),.
+0000dcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dcc0: 2020 2020 6369 7479 3d73 7562 6a65 6374      city=subject
+0000dcd0: 5f63 6f6d 7061 6e79 5f76 616c 7565 732e  _company_values.
+0000dce0: 6765 7428 274d 4149 4c20 4144 4452 4553  get('MAIL ADDRES
+0000dcf0: 5327 292e 6765 7428 2743 4954 5927 292c  S').get('CITY'),
+0000dd00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dd10: 2020 2020 2073 7461 7465 5f6f 725f 636f       state_or_co
+0000dd20: 756e 7472 793d 7375 626a 6563 745f 636f  untry=subject_co
+0000dd30: 6d70 616e 795f 7661 6c75 6573 2e67 6574  mpany_values.get
+0000dd40: 2827 4d41 494c 2041 4444 5245 5353 2729  ('MAIL ADDRESS')
+0000dd50: 2e67 6574 2827 5354 4154 4527 292c 0a20  .get('STATE'),. 
+0000dd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd70: 2020 207a 6970 636f 6465 3d73 7562 6a65     zipcode=subje
+0000dd80: 6374 5f63 6f6d 7061 6e79 5f76 616c 7565  ct_company_value
+0000dd90: 732e 6765 7428 274d 4149 4c20 4144 4452  s.get('MAIL ADDR
+0000dda0: 4553 5327 292e 6765 7428 275a 4950 2729  ESS').get('ZIP')
+0000ddb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000ddc0: 2020 2920 6966 2027 4d41 494c 2041 4444    ) if 'MAIL ADD
+0000ddd0: 5245 5353 2720 696e 2073 7562 6a65 6374  RESS' in subject
+0000dde0: 5f63 6f6d 7061 6e79 5f76 616c 7565 7320  _company_values 
+0000ddf0: 656c 7365 204e 6f6e 652c 0a20 2020 2020  else None,.     
+0000de00: 2020 2020 2020 2020 2020 2066 6f72 6d65             forme
+0000de10: 725f 636f 6d70 616e 795f 6e61 6d65 733d  r_company_names=
+0000de20: 5b46 6f72 6d65 7243 6f6d 7061 6e79 2864  [FormerCompany(d
+0000de30: 6174 655f 6f66 5f63 6861 6e67 653d 7265  ate_of_change=re
+0000de40: 636f 7264 2e67 6574 2827 4441 5445 204f  cord.get('DATE O
+0000de50: 4620 4e41 4d45 2043 4841 4e47 4527 292c  F NAME CHANGE'),
+0000de60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000de70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000de80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de90: 6e61 6d65 3d72 6563 6f72 642e 6765 7428  name=record.get(
-0000dea0: 2746 4f52 4d45 5220 434f 4e46 4f52 4d45  'FORMER CONFORME
-0000deb0: 4420 4e41 4d45 2729 290a 2020 2020 2020  D NAME')).      
+0000de90: 2020 2020 206e 616d 653d 7265 636f 7264       name=record
+0000dea0: 2e67 6574 2827 464f 524d 4552 2043 4f4e  .get('FORMER CON
+0000deb0: 464f 524d 4544 204e 414d 4527 2929 0a20  FORMED NAME')). 
 0000dec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ded0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dee0: 666f 7220 7265 636f 7264 2069 6e20 7375  for record in su
-0000def0: 626a 6563 745f 636f 6d70 616e 795f 7661  bject_company_va
-0000df00: 6c75 6573 5b27 464f 524d 4552 2043 4f4d  lues['FORMER COM
-0000df10: 5041 4e59 275d 0a20 2020 2020 2020 2020  PANY'].         
+0000dee0: 2020 2020 2066 6f72 2072 6563 6f72 6420       for record 
+0000def0: 696e 2073 7562 6a65 6374 5f63 6f6d 7061  in subject_compa
+0000df00: 6e79 5f76 616c 7565 735b 2746 4f52 4d45  ny_values['FORME
+0000df10: 5220 434f 4d50 414e 5927 5d0a 2020 2020  R COMPANY'].    
 0000df20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df30: 2020 2020 2020 2020 2020 2020 205d 0a20               ]. 
-0000df40: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000df50: 6620 2746 4f52 4d45 5220 434f 4d50 414e  f 'FORMER COMPAN
-0000df60: 5927 2069 6e20 7375 626a 6563 745f 636f  Y' in subject_co
-0000df70: 6d70 616e 795f 7661 6c75 6573 2065 6c73  mpany_values els
-0000df80: 6520 4e6f 6e65 0a20 2020 2020 2020 2020  e None.         
-0000df90: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000dfa0: 2073 7562 6a65 6374 5f63 6f6d 7061 6e69   subject_compani
-0000dfb0: 6573 2e61 7070 656e 6428 7375 626a 6563  es.append(subjec
-0000dfc0: 745f 636f 6d70 616e 7929 0a0a 2020 2020  t_company)..    
-0000dfd0: 2020 2020 2320 4372 6561 7465 2061 2064      # Create a d
-0000dfe0: 6963 7420 6f66 2074 6865 2076 616c 7565  ict of the value
-0000dff0: 7320 696e 2064 6174 6120 7468 6174 2061  s in data that a
-0000e000: 7265 206e 6f74 206e 6573 7465 6420 6469  re not nested di
-0000e010: 6374 730a 2020 2020 2020 2020 6669 6c69  cts.        fili
-0000e020: 6e67 5f6d 6574 6164 6174 6120 3d20 7b6b  ng_metadata = {k
-0000e030: 6579 3a20 7661 6c75 650a 2020 2020 2020  ey: value.      
+0000df30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df40: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
+0000df50: 2020 2020 6966 2027 464f 524d 4552 2043      if 'FORMER C
+0000df60: 4f4d 5041 4e59 2720 696e 2073 7562 6a65  OMPANY' in subje
+0000df70: 6374 5f63 6f6d 7061 6e79 5f76 616c 7565  ct_company_value
+0000df80: 7320 656c 7365 204e 6f6e 650a 2020 2020  s else None.    
+0000df90: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000dfa0: 2020 2020 2020 7375 626a 6563 745f 636f        subject_co
+0000dfb0: 6d70 616e 6965 732e 6170 7065 6e64 2873  mpanies.append(s
+0000dfc0: 7562 6a65 6374 5f63 6f6d 7061 6e79 290a  ubject_company).
+0000dfd0: 0a20 2020 2020 2020 2023 2043 7265 6174  .        # Creat
+0000dfe0: 6520 6120 6469 6374 206f 6620 7468 6520  e a dict of the 
+0000dff0: 7661 6c75 6573 2069 6e20 6461 7461 2074  values in data t
+0000e000: 6861 7420 6172 6520 6e6f 7420 6e65 7374  hat are not nest
+0000e010: 6564 2064 6963 7473 0a20 2020 2020 2020  ed dicts.       
+0000e020: 2066 696c 696e 675f 6d65 7461 6461 7461   filing_metadata
+0000e030: 203d 207b 6b65 793a 2076 616c 7565 0a20   = {key: value. 
 0000e040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e050: 2020 2020 2066 6f72 206b 6579 2c20 7661       for key, va
-0000e060: 6c75 6520 696e 2064 6174 612e 6974 656d  lue in data.item
-0000e070: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-0000e080: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000e090: 6620 6973 696e 7374 616e 6365 2876 616c  f isinstance(val
-0000e0a0: 7565 2c20 7374 7229 2061 6e64 2076 616c  ue, str) and val
-0000e0b0: 7565 7d0a 0a20 2020 2020 2020 2023 2054  ue}..        # T
-0000e0c0: 6865 2068 6561 6465 7220 7465 7874 2063  he header text c
-0000e0d0: 6f6e 7461 696e 7320 3c41 4343 4550 5441  ontains <ACCEPTA
-0000e0e0: 4e43 452d 4441 5445 5449 4d45 3e32 3032  NCE-DATETIME>202
-0000e0f0: 3330 3631 3231 3732 3234 332e 2052 6570  30612172243. Rep
-0000e100: 6c61 6365 2077 6974 6820 7468 6520 666f  lace with the fo
-0000e110: 726d 6174 7465 6420 6461 7465 0a20 2020  rmatted date.   
-0000e120: 2020 2020 2068 6561 6465 725f 7465 7874       header_text
-0000e130: 203d 2072 652e 7375 6228 7227 3c41 4343   = re.sub(r'<ACC
-0000e140: 4550 5441 4e43 452d 4441 5445 5449 4d45  EPTANCE-DATETIME
-0000e150: 3e28 5c64 7b34 7d29 285c 647b 327d 2928  >(\d{4})(\d{2})(
-0000e160: 5c64 7b32 7d29 285c 647b 327d 2928 5c64  \d{2})(\d{2})(\d
-0000e170: 7b32 7d29 285c 647b 327d 2927 2c0a 2020  {2})(\d{2})',.  
-0000e180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e190: 2020 2020 2020 2020 2020 2072 2741 4343             r'ACC
-0000e1a0: 4550 5441 4e43 452d 4441 5445 5449 4d45  EPTANCE-DATETIME
-0000e1b0: 3a20 2020 2020 2020 2020 2020 205c 312d  :            \1-
-0000e1c0: 5c32 2d5c 3320 5c34 3a5c 353a 5c36 272c  \2-\3 \4:\5:\6',
-0000e1d0: 2068 6561 6465 725f 7465 7874 290a 0a20   header_text).. 
-0000e1e0: 2020 2020 2020 2023 2052 656d 6f76 6520         # Remove 
-0000e1f0: 656d 7074 7920 6c69 6e65 7320 6672 6f6d  empty lines from
-0000e200: 2068 6561 6465 725f 7465 7874 0a20 2020   header_text.   
-0000e210: 2020 2020 2068 6561 6465 725f 7465 7874       header_text
-0000e220: 203d 2027 5c6e 272e 6a6f 696e 285b 6c69   = '\n'.join([li
-0000e230: 6e65 2066 6f72 206c 696e 6520 696e 2068  ne for line in h
-0000e240: 6561 6465 725f 7465 7874 2e73 706c 6974  eader_text.split
-0000e250: 2827 5c6e 2729 2069 6620 6c69 6e65 2e73  ('\n') if line.s
-0000e260: 7472 6970 2829 5d29 0a0a 2020 2020 2020  trip()])..      
-0000e270: 2020 2320 4372 6561 7465 2074 6865 2048    # Create the H
-0000e280: 6561 6465 7220 6f62 6a65 6374 0a20 2020  eader object.   
-0000e290: 2020 2020 2072 6574 7572 6e20 636c 7328       return cls(
-0000e2a0: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
-0000e2b0: 743d 6865 6164 6572 5f74 6578 742c 0a20  t=header_text,. 
-0000e2c0: 2020 2020 2020 2020 2020 2066 696c 696e             filin
-0000e2d0: 675f 6d65 7461 6461 7461 3d66 696c 696e  g_metadata=filin
-0000e2e0: 675f 6d65 7461 6461 7461 2c0a 2020 2020  g_metadata,.    
-0000e2f0: 2020 2020 2020 2020 6669 6c65 7273 3d66          filers=f
-0000e300: 696c 6572 732c 0a20 2020 2020 2020 2020  ilers,.         
-0000e310: 2020 2072 6570 6f72 7469 6e67 5f6f 776e     reporting_own
-0000e320: 6572 733d 7265 706f 7274 696e 675f 6f77  ers=reporting_ow
-0000e330: 6e65 7273 2c0a 2020 2020 2020 2020 2020  ners,.          
-0000e340: 2020 6973 7375 6572 733d 6973 7375 6572    issuers=issuer
-0000e350: 732c 0a20 2020 2020 2020 2020 2020 2073  s,.            s
-0000e360: 7562 6a65 6374 5f63 6f6d 7061 6e69 6573  ubject_companies
-0000e370: 3d73 7562 6a65 6374 5f63 6f6d 7061 6e69  =subject_compani
-0000e380: 6573 0a20 2020 2020 2020 2029 0a0a 2020  es.        )..  
-0000e390: 2020 6465 6620 5f5f 7269 6368 5f5f 2873    def __rich__(s
-0000e3a0: 656c 6629 3a0a 0a20 2020 2020 2020 2023  elf):..        #
-0000e3b0: 2046 696c 696e 6720 4d65 7461 6461 7461   Filing Metadata
-0000e3c0: 0a20 2020 2020 2020 206d 6574 6164 6174  .        metadat
-0000e3d0: 615f 7461 626c 6520 3d20 5461 626c 6528  a_table = Table(
-0000e3e0: 726f 775f 7374 796c 6573 3d5b 2262 6f6c  row_styles=["bol
-0000e3f0: 6422 2c20 2222 5d2c 2062 6f78 3d62 6f78  d", ""], box=box
-0000e400: 2e52 4f55 4e44 4544 290a 2020 2020 2020  .ROUNDED).      
-0000e410: 2020 6d65 7461 6461 7461 5f74 6162 6c65    metadata_table
-0000e420: 2e61 6464 5f63 6f6c 756d 6e28 2222 290a  .add_column("").
-0000e430: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
-0000e440: 5f74 6162 6c65 2e61 6464 5f63 6f6c 756d  _table.add_colum
-0000e450: 6e28 2256 616c 7565 222c 2073 7479 6c65  n("Value", style
-0000e460: 3d22 626f 6c64 2229 0a20 2020 2020 2020  ="bold").       
-0000e470: 2066 6f72 206b 6579 2c20 7661 6c75 6520   for key, value 
-0000e480: 696e 2073 656c 662e 6669 6c69 6e67 5f6d  in self.filing_m
-0000e490: 6574 6164 6174 612e 6974 656d 7328 293a  etadata.items():
-0000e4a0: 0a20 2020 2020 2020 2020 2020 2023 2046  .            # F
-0000e4b0: 6f72 6d61 7420 6173 2064 6174 6573 0a20  ormat as dates. 
-0000e4c0: 2020 2020 2020 2020 2020 2069 6620 7265             if re
-0000e4d0: 2e6d 6174 6368 2872 225e 2832 307c 3139  .match(r"^(20|19
-0000e4e0: 295c 647b 3132 7d24 222c 2076 616c 7565  )\d{12}$", value
-0000e4f0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000e500: 2020 2076 616c 7565 203d 2064 6174 6566     value = datef
-0000e510: 6d74 2876 616c 7565 2c20 2225 592d 256d  mt(value, "%Y-%m
-0000e520: 2d25 6420 2548 3a25 4d3a 2553 2229 0a20  -%d %H:%M:%S"). 
-0000e530: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-0000e540: 7265 2e6d 6174 6368 2872 225e 2832 307c  re.match(r"^(20|
-0000e550: 3139 295c 647b 367d 2422 2c20 7661 6c75  19)\d{6}$", valu
-0000e560: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-0000e570: 2020 2020 7661 6c75 6520 3d20 6461 7465      value = date
-0000e580: 666d 7428 7661 6c75 652c 2022 2559 2d25  fmt(value, "%Y-%
-0000e590: 6d2d 2564 2229 0a0a 2020 2020 2020 2020  m-%d")..        
-0000e5a0: 2020 2020 6d65 7461 6461 7461 5f74 6162      metadata_tab
-0000e5b0: 6c65 2e61 6464 5f72 6f77 2866 227b 6b65  le.add_row(f"{ke
-0000e5c0: 797d 3a22 2c20 7661 6c75 6529 0a0a 2020  y}:", value)..  
-0000e5d0: 2020 2020 2020 6d65 7461 6461 7461 5f70        metadata_p
-0000e5e0: 616e 656c 203d 2050 616e 656c 280a 2020  anel = Panel(.  
-0000e5f0: 2020 2020 2020 2020 2020 6d65 7461 6461            metada
-0000e600: 7461 5f74 6162 6c65 2c20 7469 746c 653d  ta_table, title=
-0000e610: 6622 466f 726d 207b 7365 6c66 2e66 6f72  f"Form {self.for
-0000e620: 6d7d 207b 756e 6963 6f64 655f 666f 725f  m} {unicode_for_
-0000e630: 666f 726d 2873 656c 662e 666f 726d 297d  form(self.form)}
-0000e640: 2046 494c 494e 4722 0a20 2020 2020 2020   FILING".       
-0000e650: 2029 0a0a 2020 2020 2020 2020 2320 4b65   )..        # Ke
-0000e660: 6570 2061 206c 6973 7420 6f66 2072 656e  ep a list of ren
-0000e670: 6465 7261 626c 6573 2066 6f72 2072 6963  derables for ric
-0000e680: 680a 2020 2020 2020 2020 7265 6e64 6572  h.        render
-0000e690: 6162 6c65 7320 3d20 5b6d 6574 6164 6174  ables = [metadat
-0000e6a0: 615f 7061 6e65 6c5d 0a0a 2020 2020 2020  a_panel]..      
-0000e6b0: 2020 2320 5355 424a 4543 5420 434f 4d50    # SUBJECT COMP
-0000e6c0: 414e 590a 2020 2020 2020 2020 666f 7220  ANY.        for 
-0000e6d0: 7375 626a 6563 745f 636f 6d70 616e 7920  subject_company 
-0000e6e0: 696e 2073 656c 662e 7375 626a 6563 745f  in self.subject_
-0000e6f0: 636f 6d70 616e 6965 733a 0a20 2020 2020  companies:.     
-0000e700: 2020 2020 2020 2072 656e 6465 7261 626c         renderabl
-0000e710: 6573 2e61 7070 656e 6428 7375 626a 6563  es.append(subjec
-0000e720: 745f 636f 6d70 616e 792e 5f5f 7269 6368  t_company.__rich
-0000e730: 5f5f 2829 290a 0a20 2020 2020 2020 2023  __())..        #
-0000e740: 2046 494c 4552 0a20 2020 2020 2020 2066   FILER.        f
-0000e750: 6f72 2066 696c 6572 2069 6e20 7365 6c66  or filer in self
-0000e760: 2e66 696c 6572 733a 0a20 2020 2020 2020  .filers:.       
-0000e770: 2020 2020 2072 656e 6465 7261 626c 6573       renderables
-0000e780: 2e61 7070 656e 6428 6669 6c65 722e 5f5f  .append(filer.__
-0000e790: 7269 6368 5f5f 2829 290a 0a20 2020 2020  rich__())..     
-0000e7a0: 2020 2023 2052 4550 4f52 5449 4e47 204f     # REPORTING O
-0000e7b0: 574e 4552 0a20 2020 2020 2020 2066 6f72  WNER.        for
-0000e7c0: 2072 6570 6f72 7469 6e67 5f6f 776e 6572   reporting_owner
-0000e7d0: 2069 6e20 7365 6c66 2e72 6570 6f72 7469   in self.reporti
-0000e7e0: 6e67 5f6f 776e 6572 733a 0a20 2020 2020  ng_owners:.     
-0000e7f0: 2020 2020 2020 2072 656e 6465 7261 626c         renderabl
-0000e800: 6573 2e61 7070 656e 6428 7265 706f 7274  es.append(report
-0000e810: 696e 675f 6f77 6e65 722e 5f5f 7269 6368  ing_owner.__rich
-0000e820: 5f5f 2829 290a 0a20 2020 2020 2020 2023  __())..        #
-0000e830: 2049 5353 5545 520a 2020 2020 2020 2020   ISSUER.        
-0000e840: 666f 7220 6973 7375 6572 2069 6e20 7365  for issuer in se
-0000e850: 6c66 2e69 7373 7565 7273 3a0a 2020 2020  lf.issuers:.    
-0000e860: 2020 2020 2020 2020 7265 6e64 6572 6162          renderab
-0000e870: 6c65 732e 6170 7065 6e64 2869 7373 7565  les.append(issue
-0000e880: 722e 5f5f 7269 6368 5f5f 2829 290a 2020  r.__rich__()).  
-0000e890: 2020 2020 2020 7265 7475 726e 2050 616e        return Pan
-0000e8a0: 656c 280a 2020 2020 2020 2020 2020 2020  el(.            
-0000e8b0: 4772 6f75 7028 0a20 2020 2020 2020 2020  Group(.         
-0000e8c0: 2020 2020 2020 202a 7265 6e64 6572 6162         *renderab
-0000e8d0: 6c65 730a 2020 2020 2020 2020 2020 2020  les.            
-0000e8e0: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
-0000e8f0: 2064 6566 205f 5f72 6570 725f 5f28 7365   def __repr__(se
-0000e900: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
-0000e910: 7572 6e20 7265 7072 5f72 6963 6828 7365  urn repr_rich(se
-0000e920: 6c66 2e5f 5f72 6963 685f 5f28 2929 0a0a  lf.__rich__())..
-0000e930: 0a63 6c61 7373 2046 696c 696e 673a 0a20  .class Filing:. 
-0000e940: 2020 2022 2222 0a20 2020 2041 2073 696e     """.    A sin
-0000e950: 676c 6520 5345 4320 6669 6c69 6e67 2e20  gle SEC filing. 
-0000e960: 416c 6c6f 7720 796f 7520 746f 2061 6363  Allow you to acc
-0000e970: 6573 7320 7468 6520 646f 6375 6d65 6e74  ess the document
-0000e980: 7320 616e 6420 6461 7461 2066 6f72 2074  s and data for t
-0000e990: 6861 7420 6669 6c69 6e67 0a20 2020 2022  hat filing.    "
-0000e9a0: 2222 0a0a 2020 2020 6465 6620 5f5f 696e  ""..    def __in
-0000e9b0: 6974 5f5f 2873 656c 662c 0a20 2020 2020  it__(self,.     
-0000e9c0: 2020 2020 2020 2020 2020 2020 6369 6b3a              cik:
-0000e9d0: 2069 6e74 2c0a 2020 2020 2020 2020 2020   int,.          
-0000e9e0: 2020 2020 2020 2063 6f6d 7061 6e79 3a20         company: 
-0000e9f0: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
-0000ea00: 2020 2020 2020 666f 726d 3a20 7374 722c        form: str,
-0000ea10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ea20: 2020 6669 6c69 6e67 5f64 6174 653a 2073    filing_date: s
-0000ea30: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
-0000ea40: 2020 2020 2061 6363 6573 7369 6f6e 5f6e       accession_n
-0000ea50: 6f3a 2073 7472 293a 0a20 2020 2020 2020  o: str):.       
-0000ea60: 2073 656c 662e 6369 6b20 3d20 6369 6b0a   self.cik = cik.
-0000ea70: 2020 2020 2020 2020 7365 6c66 2e63 6f6d          self.com
-0000ea80: 7061 6e79 203d 2063 6f6d 7061 6e79 0a20  pany = company. 
-0000ea90: 2020 2020 2020 2073 656c 662e 666f 726d         self.form
-0000eaa0: 203d 2066 6f72 6d0a 2020 2020 2020 2020   = form.        
-0000eab0: 7365 6c66 2e66 696c 696e 675f 6461 7465  self.filing_date
-0000eac0: 203d 2066 696c 696e 675f 6461 7465 0a20   = filing_date. 
-0000ead0: 2020 2020 2020 2073 656c 662e 6163 6365         self.acce
-0000eae0: 7373 696f 6e5f 6e6f 203d 2061 6363 6573  ssion_no = acces
-0000eaf0: 7369 6f6e 5f6e 6f0a 2020 2020 2020 2020  sion_no.        
-0000eb00: 7365 6c66 2e5f 6669 6c69 6e67 5f68 6f6d  self._filing_hom
-0000eb10: 6570 6167 6520 3d20 4e6f 6e65 0a0a 2020  epage = None..  
-0000eb20: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-0000eb30: 6465 6620 646f 6375 6d65 6e74 2873 656c  def document(sel
-0000eb40: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
-0000eb50: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-0000eb60: 2054 6865 2070 7269 6d61 7279 2064 6973   The primary dis
-0000eb70: 706c 6179 2064 6f63 756d 656e 7420 6f6e  play document on
-0000eb80: 2074 6865 2066 696c 696e 672c 2067 656e   the filing, gen
-0000eb90: 6572 616c 6c79 2048 544d 4c20 6275 7420  erally HTML but 
-0000eba0: 6361 6e20 6265 2058 4854 4d4c 0a20 2020  can be XHTML.   
-0000ebb0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000ebc0: 2072 6574 7572 6e20 7365 6c66 2e68 6f6d   return self.hom
-0000ebd0: 6570 6167 652e 7072 696d 6172 795f 6874  epage.primary_ht
-0000ebe0: 6d6c 5f64 6f63 756d 656e 740a 0a20 2020  ml_document..   
-0000ebf0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-0000ec00: 6566 2070 7269 6d61 7279 5f64 6f63 756d  ef primary_docum
-0000ec10: 656e 7473 2873 656c 6629 3a0a 2020 2020  ents(self):.    
-0000ec20: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000ec30: 3a72 6574 7572 6e3a 2061 206c 6973 7420  :return: a list 
-0000ec40: 6f66 2074 6865 2070 7269 6d61 7279 2064  of the primary d
-0000ec50: 6f63 756d 656e 7473 206f 6e20 7468 6520  ocuments on the 
-0000ec60: 6669 6c69 6e67 2c20 6765 6e65 7261 6c6c  filing, generall
-0000ec70: 7920 4854 4d4c 206f 7220 5848 544d 4c20  y HTML or XHTML 
-0000ec80: 616e 6420 6f70 7469 6f6e 616c 6c79 2058  and optionally X
-0000ec90: 4d4c 0a20 2020 2020 2020 2022 2222 0a20  ML.        """. 
-0000eca0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000ecb0: 6c66 2e68 6f6d 6570 6167 652e 7072 696d  lf.homepage.prim
-0000ecc0: 6172 795f 646f 6375 6d65 6e74 730a 0a20  ary_documents.. 
-0000ecd0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-0000ece0: 2064 6566 2061 7474 6163 686d 656e 7473   def attachments
-0000ecf0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000ed00: 2320 5265 7475 726e 2061 6c6c 2074 6865  # Return all the
-0000ed10: 2061 7474 6163 686d 656e 7473 206f 6e20   attachments on 
-0000ed20: 7468 6520 6669 6c69 6e67 0a20 2020 2020  the filing.     
-0000ed30: 2020 2072 6574 7572 6e20 7365 6c66 2e68     return self.h
-0000ed40: 6f6d 6570 6167 652e 6174 7461 6368 6d65  omepage.attachme
-0000ed50: 6e74 730a 0a20 2020 2064 6566 2068 746d  nts..    def htm
-0000ed60: 6c28 7365 6c66 2920 2d3e 204f 7074 696f  l(self) -> Optio
-0000ed70: 6e61 6c5b 7374 725d 3a0a 2020 2020 2020  nal[str]:.      
-0000ed80: 2020 2222 2252 6574 7572 6e73 2074 6865    """Returns the
-0000ed90: 2068 746d 6c20 636f 6e74 656e 7473 206f   html contents o
-0000eda0: 6620 7468 6520 7072 696d 6172 7920 646f  f the primary do
-0000edb0: 6375 6d65 6e74 2069 6620 6974 2069 7320  cument if it is 
-0000edc0: 6874 6d6c 2222 220a 2020 2020 2020 2020  html""".        
-0000edd0: 6966 2073 656c 662e 646f 6375 6d65 6e74  if self.document
-0000ede0: 2e69 735f 6269 6e61 7279 2829 3a0a 2020  .is_binary():.  
-0000edf0: 2020 2020 2020 2020 2020 6c6f 672e 696e            log.in
-0000ee00: 666f 2866 2250 7269 6d61 7279 2064 6f63  fo(f"Primary doc
-0000ee10: 756d 656e 7420 7b73 656c 662e 646f 6375  ument {self.docu
-0000ee20: 6d65 6e74 2e75 726c 7d20 6973 2061 2062  ment.url} is a b
-0000ee30: 696e 6172 7920 6669 6c65 2229 0a20 2020  inary file").   
-0000ee40: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000ee50: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000ee60: 6c66 2e64 6f63 756d 656e 742e 646f 776e  lf.document.down
-0000ee70: 6c6f 6164 2829 0a0a 2020 2020 6465 6620  load()..    def 
-0000ee80: 786d 6c28 7365 6c66 2920 2d3e 204f 7074  xml(self) -> Opt
-0000ee90: 696f 6e61 6c5b 7374 725d 3a0a 2020 2020  ional[str]:.    
-0000eea0: 2020 2020 2222 2252 6574 7572 6e73 2074      """Returns t
-0000eeb0: 6865 2078 6d6c 2063 6f6e 7465 6e74 7320  he xml contents 
-0000eec0: 6f66 2074 6865 2070 7269 6d61 7279 2064  of the primary d
-0000eed0: 6f63 756d 656e 7420 6966 2069 7420 6973  ocument if it is
-0000eee0: 2078 6d6c 2222 220a 2020 2020 2020 2020   xml""".        
-0000eef0: 786d 6c5f 646f 6375 6d65 6e74 3a20 4174  xml_document: At
-0000ef00: 7461 6368 6d65 6e74 203d 2073 656c 662e  tachment = self.
-0000ef10: 686f 6d65 7061 6765 2e70 7269 6d61 7279  homepage.primary
-0000ef20: 5f78 6d6c 5f64 6f63 756d 656e 740a 2020  _xml_document.  
-0000ef30: 2020 2020 2020 6966 2078 6d6c 5f64 6f63        if xml_doc
-0000ef40: 756d 656e 743a 0a20 2020 2020 2020 2020  ument:.         
-0000ef50: 2020 2072 6574 7572 6e20 786d 6c5f 646f     return xml_do
-0000ef60: 6375 6d65 6e74 2e64 6f77 6e6c 6f61 6428  cument.download(
-0000ef70: 290a 0a20 2020 2040 6c72 755f 6361 6368  )..    @lru_cach
-0000ef80: 6528 6d61 7873 697a 653d 3429 0a20 2020  e(maxsize=4).   
-0000ef90: 2064 6566 2074 6578 7428 7365 6c66 2c20   def text(self, 
-0000efa0: 6967 6e6f 7265 5f74 6162 6c65 733d 4661  ignore_tables=Fa
-0000efb0: 6c73 652c 2073 6570 3d22 5c6e 2229 202d  lse, sep="\n") -
-0000efc0: 3e20 7374 723a 0a20 2020 2020 2020 2022  > str:.        "
-0000efd0: 2222 436f 6e76 6572 7420 7468 6520 6874  ""Convert the ht
-0000efe0: 6d6c 206f 6620 7468 6520 6d61 696e 2066  ml of the main f
-0000eff0: 696c 696e 6720 646f 6375 6d65 6e74 2074  iling document t
-0000f000: 6f20 7465 7874 2222 220a 2020 2020 2020  o text""".      
-0000f010: 2020 6874 6d6c 5f63 6f6e 7465 6e74 203d    html_content =
-0000f020: 2073 656c 662e 6874 6d6c 2829 0a20 2020   self.html().   
-0000f030: 2020 2020 2069 6620 6874 6d6c 5f63 6f6e       if html_con
-0000f040: 7465 6e74 3a0a 2020 2020 2020 2020 2020  tent:.          
-0000f050: 2020 7265 7475 726e 2068 746d 6c5f 746f    return html_to
-0000f060: 5f74 6578 7428 6874 6d6c 5f63 6f6e 7465  _text(html_conte
-0000f070: 6e74 2c20 6967 6e6f 7265 5f74 6162 6c65  nt, ignore_table
-0000f080: 733d 6967 6e6f 7265 5f74 6162 6c65 732c  s=ignore_tables,
-0000f090: 2073 6570 3d73 6570 290a 0a20 2020 2064   sep=sep)..    d
-0000f0a0: 6566 2066 756c 6c5f 7465 7874 5f73 7562  ef full_text_sub
-0000f0b0: 6d69 7373 696f 6e28 7365 6c66 2920 2d3e  mission(self) ->
-0000f0c0: 2073 7472 3a0a 2020 2020 2020 2020 2222   str:.        ""
-0000f0d0: 2252 6574 7572 6e20 7468 6520 636f 6d70  "Return the comp
-0000f0e0: 6c65 7465 2074 6578 7420 7375 626d 6973  lete text submis
-0000f0f0: 7369 6f6e 2066 696c 6522 2222 0a20 2020  sion file""".   
-0000f100: 2020 2020 2072 6574 7572 6e20 646f 776e       return down
-0000f110: 6c6f 6164 5f66 696c 6528 7365 6c66 2e74  load_file(self.t
-0000f120: 6578 745f 7572 6c29 0a0a 2020 2020 6465  ext_url)..    de
-0000f130: 6620 6d61 726b 646f 776e 2873 656c 6629  f markdown(self)
-0000f140: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
-0000f150: 2022 2222 7265 7475 726e 2074 6865 206d   """return the m
-0000f160: 6172 6b64 6f77 6e20 7665 7273 696f 6e20  arkdown version 
-0000f170: 6f66 2074 6869 7320 6669 6c69 6e67 2068  of this filing h
-0000f180: 746d 6c22 2222 0a20 2020 2020 2020 2072  tml""".        r
-0000f190: 6574 7572 6e20 6874 6d6c 5f74 6f5f 6d61  eturn html_to_ma
-0000f1a0: 726b 646f 776e 2873 656c 662e 6874 6d6c  rkdown(self.html
-0000f1b0: 2829 290a 0a20 2020 2064 6566 2076 6965  ())..    def vie
-0000f1c0: 7728 7365 6c66 293a 0a20 2020 2020 2020  w(self):.       
-0000f1d0: 2022 2222 5072 6576 6965 7720 7468 6973   """Preview this
-0000f1e0: 2066 696c 696e 6727 7320 7072 696d 6172   filing's primar
-0000f1f0: 7920 646f 6375 6d65 6e74 2061 7320 6d61  y document as ma
-0000f200: 726b 646f 776e 2e20 5468 6973 2073 686f  rkdown. This sho
-0000f210: 756c 6420 6469 7370 6c61 7920 696e 2074  uld display in t
-0000f220: 6865 2063 6f6e 736f 6c65 2222 220a 2020  he console""".  
-0000f230: 2020 2020 2020 636f 6e73 6f6c 6520 3d20        console = 
-0000f240: 436f 6e73 6f6c 6528 290a 2020 2020 2020  Console().      
-0000f250: 2020 636f 6e73 6f6c 652e 7072 696e 7428    console.print(
-0000f260: 4d61 726b 646f 776e 436f 6e74 656e 7428  MarkdownContent(
-0000f270: 7365 6c66 2e68 746d 6c28 292c 2074 6974  self.html(), tit
-0000f280: 6c65 3d66 2246 6f72 6d20 7b73 656c 662e  le=f"Form {self.
-0000f290: 666f 726d 7d20 666f 7220 7b73 656c 662e  form} for {self.
-0000f2a0: 636f 6d70 616e 797d 2229 290a 0a20 2020  company}"))..   
-0000f2b0: 2064 6566 2078 6272 6c28 7365 6c66 2920   def xbrl(self) 
-0000f2c0: 2d3e 204f 7074 696f 6e61 6c5b 4669 6c69  -> Optional[Fili
-0000f2d0: 6e67 5862 726c 5d3a 0a20 2020 2020 2020  ngXbrl]:.       
-0000f2e0: 2022 2222 0a20 2020 2020 2020 2047 6574   """.        Get
-0000f2f0: 2074 6865 2058 4252 4c20 646f 6375 6d65   the XBRL docume
-0000f300: 6e74 2066 6f72 2074 6865 2066 696c 696e  nt for the filin
-0000f310: 672c 2070 6172 7365 6420 616e 6420 6173  g, parsed and as
-0000f320: 2061 2046 696c 696e 6758 6272 6c20 6f62   a FilingXbrl ob
-0000f330: 6a65 6374 0a20 2020 2020 2020 203a 7265  ject.        :re
-0000f340: 7475 726e 3a20 4765 7420 7468 6520 5842  turn: Get the XB
-0000f350: 524c 2064 6f63 756d 656e 7420 666f 7220  RL document for 
-0000f360: 7468 6520 6669 6c69 6e67 2c20 7061 7273  the filing, pars
-0000f370: 6564 2061 6e64 2061 7320 6120 4669 6c69  ed and as a Fili
-0000f380: 6e67 5862 726c 206f 626a 6563 742c 206f  ngXbrl object, o
-0000f390: 7220 4e6f 6e65 0a20 2020 2020 2020 2022  r None.        "
-0000f3a0: 2222 0a20 2020 2020 2020 2078 6272 6c5f  "".        xbrl_
-0000f3b0: 646f 6375 6d65 6e74 203d 2073 656c 662e  document = self.
-0000f3c0: 686f 6d65 7061 6765 2e78 6272 6c5f 646f  homepage.xbrl_do
-0000f3d0: 6375 6d65 6e74 0a20 2020 2020 2020 2069  cument.        i
-0000f3e0: 6620 7862 726c 5f64 6f63 756d 656e 743a  f xbrl_document:
-0000f3f0: 0a20 2020 2020 2020 2020 2020 2078 6272  .            xbr
-0000f400: 6c5f 7465 7874 203d 2078 6272 6c5f 646f  l_text = xbrl_do
-0000f410: 6375 6d65 6e74 2e64 6f77 6e6c 6f61 6428  cument.download(
-0000f420: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-0000f430: 7475 726e 2046 696c 696e 6758 6272 6c2e  turn FilingXbrl.
-0000f440: 7061 7273 6528 7862 726c 5f74 6578 7429  parse(xbrl_text)
-0000f450: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-0000f460: 2020 2020 406c 7275 5f63 6163 6865 286d      @lru_cache(m
-0000f470: 6178 7369 7a65 3d31 290a 2020 2020 6465  axsize=1).    de
-0000f480: 6620 6865 6164 6572 2873 656c 6629 3a0a  f header(self):.
-0000f490: 2020 2020 2020 2020 7365 635f 6865 6164          sec_head
-0000f4a0: 6572 5f63 6f6e 7465 6e74 203d 2067 6574  er_content = get
-0000f4b0: 5f74 6578 745f 6265 7477 6565 6e5f 7461  _text_between_ta
-0000f4c0: 6773 2873 656c 662e 7465 7874 5f75 726c  gs(self.text_url
-0000f4d0: 2c20 2253 4543 2d48 4541 4445 5222 290a  , "SEC-HEADER").
-0000f4e0: 2020 2020 2020 2020 7265 7475 726e 2053          return S
-0000f4f0: 4543 4865 6164 6572 2e70 6172 7365 2873  ECHeader.parse(s
-0000f500: 6563 5f68 6561 6465 725f 636f 6e74 656e  ec_header_conten
-0000f510: 7429 0a0a 2020 2020 6465 6620 6461 7461  t)..    def data
-0000f520: 5f6f 626a 6563 7428 7365 6c66 293a 0a20  _object(self):. 
-0000f530: 2020 2020 2020 2022 2222 2047 6574 2074         """ Get t
-0000f540: 6869 7320 6669 6c69 6e67 2061 7320 7468  his filing as th
-0000f550: 6520 6461 7461 206f 626a 6563 7420 7468  e data object th
-0000f560: 6174 2069 7420 6d69 6768 7420 6265 2222  at it might be""
-0000f570: 220a 2020 2020 2020 2020 6672 6f6d 2065  ".        from e
-0000f580: 6467 6172 2069 6d70 6f72 7420 6f62 6a0a  dgar import obj.
-0000f590: 2020 2020 2020 2020 7265 7475 726e 206f          return o
-0000f5a0: 626a 2873 656c 6629 0a0a 2020 2020 6465  bj(self)..    de
-0000f5b0: 6620 6f62 6a28 7365 6c66 293a 0a20 2020  f obj(self):.   
-0000f5c0: 2020 2020 2022 2222 416c 6961 7320 666f       """Alias fo
-0000f5d0: 7220 6461 7461 5f6f 626a 6563 7428 2922  r data_object()"
-0000f5e0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-0000f5f0: 6e20 7365 6c66 2e64 6174 615f 6f62 6a65  n self.data_obje
-0000f600: 6374 2829 0a0a 2020 2020 6465 6620 6f70  ct()..    def op
-0000f610: 656e 5f68 6f6d 6570 6167 6528 7365 6c66  en_homepage(self
-0000f620: 293a 0a20 2020 2020 2020 2022 2222 4f70  ):.        """Op
-0000f630: 656e 2074 6865 2068 6f6d 6570 6167 6520  en the homepage 
-0000f640: 696e 2074 6865 2062 726f 7773 6572 2222  in the browser""
-0000f650: 220a 2020 2020 2020 2020 7765 6262 726f  ".        webbro
-0000f660: 7773 6572 2e6f 7065 6e28 7365 6c66 2e68  wser.open(self.h
-0000f670: 6f6d 6570 6167 655f 7572 6c29 0a0a 2020  omepage_url)..  
-0000f680: 2020 6465 6620 6f70 656e 2873 656c 6629    def open(self)
-0000f690: 3a0a 2020 2020 2020 2020 2222 224f 7065  :.        """Ope
-0000f6a0: 6e20 7468 6520 6d61 696e 2066 696c 696e  n the main filin
-0000f6b0: 6720 646f 6375 6d65 6e74 2222 220a 2020  g document""".  
-0000f6c0: 2020 2020 2020 7765 6262 726f 7773 6572        webbrowser
-0000f6d0: 2e6f 7065 6e28 7365 6c66 2e64 6f63 756d  .open(self.docum
-0000f6e0: 656e 742e 7572 6c29 0a0a 2020 2020 406c  ent.url)..    @l
-0000f6f0: 7275 5f63 6163 6865 286d 6178 7369 7a65  ru_cache(maxsize
-0000f700: 3d31 290a 2020 2020 6465 6620 7365 6374  =1).    def sect
-0000f710: 696f 6e73 2873 656c 6629 202d 3e20 4c69  ions(self) -> Li
-0000f720: 7374 5b73 7472 5d3a 0a20 2020 2020 2020  st[str]:.       
-0000f730: 2072 6574 7572 6e20 6874 6d6c 5f73 6563   return html_sec
-0000f740: 7469 6f6e 7328 7365 6c66 2e68 746d 6c28  tions(self.html(
-0000f750: 2929 0a0a 2020 2020 406c 7275 5f63 6163  ))..    @lru_cac
-0000f760: 6865 286d 6178 7369 7a65 3d31 290a 2020  he(maxsize=1).  
-0000f770: 2020 6465 6620 5f5f 6765 745f 626d 3235    def __get_bm25
-0000f780: 5f73 6561 7263 685f 696e 6465 7828 7365  _search_index(se
-0000f790: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
-0000f7a0: 7572 6e20 424d 3235 5365 6172 6368 2873  urn BM25Search(s
-0000f7b0: 656c 662e 7365 6374 696f 6e73 2829 290a  elf.sections()).
-0000f7c0: 0a20 2020 2040 6c72 755f 6361 6368 6528  .    @lru_cache(
-0000f7d0: 6d61 7873 697a 653d 3129 0a20 2020 2064  maxsize=1).    d
-0000f7e0: 6566 205f 5f67 6574 5f72 6567 6578 5f73  ef __get_regex_s
-0000f7f0: 6561 7263 685f 696e 6465 7828 7365 6c66  earch_index(self
-0000f800: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-0000f810: 6e20 5265 6765 7853 6561 7263 6828 7365  n RegexSearch(se
-0000f820: 6c66 2e73 6563 7469 6f6e 7328 2929 0a0a  lf.sections())..
-0000f830: 2020 2020 6465 6620 7365 6172 6368 2873      def search(s
-0000f840: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
-0000f850: 2020 2020 7175 6572 793a 2073 7472 2c0a      query: str,.
-0000f860: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000f870: 6567 6578 3d46 616c 7365 293a 0a20 2020  egex=False):.   
-0000f880: 2020 2020 2022 2222 5365 6172 6368 2066       """Search f
-0000f890: 6f72 2074 6865 2071 7565 7279 2073 7472  or the query str
-0000f8a0: 696e 6720 696e 2074 6865 2066 696c 696e  ing in the filin
-0000f8b0: 6720 4854 4d4c 2222 220a 2020 2020 2020  g HTML""".      
-0000f8c0: 2020 6966 2072 6567 6578 3a0a 2020 2020    if regex:.    
-0000f8d0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000f8e0: 656c 662e 5f5f 6765 745f 7265 6765 785f  elf.__get_regex_
-0000f8f0: 7365 6172 6368 5f69 6e64 6578 2829 2e73  search_index().s
-0000f900: 6561 7263 6828 7175 6572 7929 0a20 2020  earch(query).   
-0000f910: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000f920: 2e5f 5f67 6574 5f62 6d32 355f 7365 6172  .__get_bm25_sear
-0000f930: 6368 5f69 6e64 6578 2829 2e73 6561 7263  ch_index().searc
-0000f940: 6828 7175 6572 7929 0a0a 2020 2020 4070  h(query)..    @p
-0000f950: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0000f960: 686f 6d65 7061 6765 5f75 726c 2873 656c  homepage_url(sel
-0000f970: 6629 202d 3e20 7374 723a 0a20 2020 2020  f) -> str:.     
-0000f980: 2020 2072 6574 7572 6e20 6622 7b73 6563     return f"{sec
-0000f990: 5f65 6467 6172 7d2f 6461 7461 2f7b 7365  _edgar}/data/{se
-0000f9a0: 6c66 2e63 696b 7d2f 7b73 656c 662e 6163  lf.cik}/{self.ac
-0000f9b0: 6365 7373 696f 6e5f 6e6f 7d2d 696e 6465  cession_no}-inde
-0000f9c0: 782e 6874 6d6c 220a 0a20 2020 2040 7072  x.html"..    @pr
-0000f9d0: 6f70 6572 7479 0a20 2020 2064 6566 2074  operty.    def t
-0000f9e0: 6578 745f 7572 6c28 7365 6c66 2920 2d3e  ext_url(self) ->
-0000f9f0: 2073 7472 3a0a 2020 2020 2020 2020 7265   str:.        re
-0000fa00: 7475 726e 2066 227b 7365 635f 6564 6761  turn f"{sec_edga
-0000fa10: 727d 2f64 6174 612f 7b73 656c 662e 6369  r}/data/{self.ci
-0000fa20: 6b7d 2f7b 7365 6c66 2e61 6363 6573 7369  k}/{self.accessi
-0000fa30: 6f6e 5f6e 6f2e 7265 706c 6163 6528 272d  on_no.replace('-
-0000fa40: 272c 2027 2729 7d2f 7b73 656c 662e 6163  ', '')}/{self.ac
-0000fa50: 6365 7373 696f 6e5f 6e6f 7d2e 7478 7422  cession_no}.txt"
-0000fa60: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-0000fa70: 2020 2020 6465 6620 7572 6c28 7365 6c66      def url(self
-0000fa80: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
-0000fa90: 2020 7265 7475 726e 2073 656c 662e 686f    return self.ho
-0000faa0: 6d65 7061 6765 5f75 726c 0a0a 2020 2020  mepage_url..    
-0000fab0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0000fac0: 6620 686f 6d65 7061 6765 2873 656c 6629  f homepage(self)
-0000fad0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000fae0: 2020 2020 2020 4765 7420 7468 6520 686f        Get the ho
-0000faf0: 6d65 7061 6765 2066 6f72 2074 6865 2066  mepage for the f
-0000fb00: 696c 696e 670a 2020 2020 2020 2020 3a72  iling.        :r
-0000fb10: 6574 7572 6e3a 2074 6865 2046 696c 696e  eturn: the Filin
-0000fb20: 6748 6f6d 6570 6167 650a 2020 2020 2020  gHomepage.      
-0000fb30: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-0000fb40: 206e 6f74 2073 656c 662e 5f66 696c 696e   not self._filin
-0000fb50: 675f 686f 6d65 7061 6765 3a0a 2020 2020  g_homepage:.    
-0000fb60: 2020 2020 2020 2020 686f 6d65 7061 6765          homepage
-0000fb70: 5f68 746d 6c20 3d20 646f 776e 6c6f 6164  _html = download
-0000fb80: 5f74 6578 7428 7365 6c66 2e68 6f6d 6570  _text(self.homep
-0000fb90: 6167 655f 7572 6c29 0a20 2020 2020 2020  age_url).       
-0000fba0: 2020 2020 2073 656c 662e 5f66 696c 696e       self._filin
-0000fbb0: 675f 686f 6d65 7061 6765 203d 2046 696c  g_homepage = Fil
-0000fbc0: 696e 6748 6f6d 6570 6167 652e 6672 6f6d  ingHomepage.from
-0000fbd0: 5f68 746d 6c28 686f 6d65 7061 6765 5f68  _html(homepage_h
-0000fbe0: 746d 6c2c 0a20 2020 2020 2020 2020 2020  tml,.           
+0000e050: 2020 2020 2020 2020 2020 666f 7220 6b65            for ke
+0000e060: 792c 2076 616c 7565 2069 6e20 6461 7461  y, value in data
+0000e070: 2e69 7465 6d73 2829 0a20 2020 2020 2020  .items().       
+0000e080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e090: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+0000e0a0: 6528 7661 6c75 652c 2073 7472 2920 616e  e(value, str) an
+0000e0b0: 6420 7661 6c75 657d 0a0a 2020 2020 2020  d value}..      
+0000e0c0: 2020 2320 5468 6520 6865 6164 6572 2074    # The header t
+0000e0d0: 6578 7420 636f 6e74 6169 6e73 203c 4143  ext contains <AC
+0000e0e0: 4345 5054 414e 4345 2d44 4154 4554 494d  CEPTANCE-DATETIM
+0000e0f0: 453e 3230 3233 3036 3132 3137 3232 3433  E>20230612172243
+0000e100: 2e20 5265 706c 6163 6520 7769 7468 2074  . Replace with t
+0000e110: 6865 2066 6f72 6d61 7474 6564 2064 6174  he formatted dat
+0000e120: 650a 2020 2020 2020 2020 6865 6164 6572  e.        header
+0000e130: 5f74 6578 7420 3d20 7265 2e73 7562 2872  _text = re.sub(r
+0000e140: 273c 4143 4345 5054 414e 4345 2d44 4154  '<ACCEPTANCE-DAT
+0000e150: 4554 494d 453e 285c 647b 347d 2928 5c64  ETIME>(\d{4})(\d
+0000e160: 7b32 7d29 285c 647b 327d 2928 5c64 7b32  {2})(\d{2})(\d{2
+0000e170: 7d29 285c 647b 327d 2928 5c64 7b32 7d29  })(\d{2})(\d{2})
+0000e180: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+0000e190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1a0: 7227 4143 4345 5054 414e 4345 2d44 4154  r'ACCEPTANCE-DAT
+0000e1b0: 4554 494d 453a 2020 2020 2020 2020 2020  ETIME:          
+0000e1c0: 2020 5c31 2d5c 322d 5c33 205c 343a 5c35    \1-\2-\3 \4:\5
+0000e1d0: 3a5c 3627 2c20 6865 6164 6572 5f74 6578  :\6', header_tex
+0000e1e0: 7429 0a0a 2020 2020 2020 2020 2320 5265  t)..        # Re
+0000e1f0: 6d6f 7665 2065 6d70 7479 206c 696e 6573  move empty lines
+0000e200: 2066 726f 6d20 6865 6164 6572 5f74 6578   from header_tex
+0000e210: 740a 2020 2020 2020 2020 6865 6164 6572  t.        header
+0000e220: 5f74 6578 7420 3d20 275c 6e27 2e6a 6f69  _text = '\n'.joi
+0000e230: 6e28 5b6c 696e 6520 666f 7220 6c69 6e65  n([line for line
+0000e240: 2069 6e20 6865 6164 6572 5f74 6578 742e   in header_text.
+0000e250: 7370 6c69 7428 275c 6e27 2920 6966 206c  split('\n') if l
+0000e260: 696e 652e 7374 7269 7028 295d 290a 0a20  ine.strip()]).. 
+0000e270: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
+0000e280: 7468 6520 4865 6164 6572 206f 626a 6563  the Header objec
+0000e290: 740a 2020 2020 2020 2020 7265 7475 726e  t.        return
+0000e2a0: 2063 6c73 280a 2020 2020 2020 2020 2020   cls(.          
+0000e2b0: 2020 7465 7874 3d68 6561 6465 725f 7465    text=header_te
+0000e2c0: 7874 2c0a 2020 2020 2020 2020 2020 2020  xt,.            
+0000e2d0: 6669 6c69 6e67 5f6d 6574 6164 6174 613d  filing_metadata=
+0000e2e0: 6669 6c69 6e67 5f6d 6574 6164 6174 612c  filing_metadata,
+0000e2f0: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
+0000e300: 6572 733d 6669 6c65 7273 2c0a 2020 2020  ers=filers,.    
+0000e310: 2020 2020 2020 2020 7265 706f 7274 696e          reportin
+0000e320: 675f 6f77 6e65 7273 3d72 6570 6f72 7469  g_owners=reporti
+0000e330: 6e67 5f6f 776e 6572 732c 0a20 2020 2020  ng_owners,.     
+0000e340: 2020 2020 2020 2069 7373 7565 7273 3d69         issuers=i
+0000e350: 7373 7565 7273 2c0a 2020 2020 2020 2020  ssuers,.        
+0000e360: 2020 2020 7375 626a 6563 745f 636f 6d70      subject_comp
+0000e370: 616e 6965 733d 7375 626a 6563 745f 636f  anies=subject_co
+0000e380: 6d70 616e 6965 730a 2020 2020 2020 2020  mpanies.        
+0000e390: 290a 0a20 2020 2064 6566 205f 5f72 6963  )..    def __ric
+0000e3a0: 685f 5f28 7365 6c66 293a 0a0a 2020 2020  h__(self):..    
+0000e3b0: 2020 2020 2320 4669 6c69 6e67 204d 6574      # Filing Met
+0000e3c0: 6164 6174 610a 2020 2020 2020 2020 6d65  adata.        me
+0000e3d0: 7461 6461 7461 5f74 6162 6c65 203d 2054  tadata_table = T
+0000e3e0: 6162 6c65 2872 6f77 5f73 7479 6c65 733d  able(row_styles=
+0000e3f0: 5b22 626f 6c64 222c 2022 225d 2c20 626f  ["bold", ""], bo
+0000e400: 783d 626f 782e 524f 554e 4445 4429 0a20  x=box.ROUNDED). 
+0000e410: 2020 2020 2020 206d 6574 6164 6174 615f         metadata_
+0000e420: 7461 626c 652e 6164 645f 636f 6c75 6d6e  table.add_column
+0000e430: 2822 2229 0a20 2020 2020 2020 206d 6574  ("").        met
+0000e440: 6164 6174 615f 7461 626c 652e 6164 645f  adata_table.add_
+0000e450: 636f 6c75 6d6e 2822 5661 6c75 6522 2c20  column("Value", 
+0000e460: 7374 796c 653d 2262 6f6c 6422 290a 2020  style="bold").  
+0000e470: 2020 2020 2020 666f 7220 6b65 792c 2076        for key, v
+0000e480: 616c 7565 2069 6e20 7365 6c66 2e66 696c  alue in self.fil
+0000e490: 696e 675f 6d65 7461 6461 7461 2e69 7465  ing_metadata.ite
+0000e4a0: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
+0000e4b0: 2020 2320 466f 726d 6174 2061 7320 6461    # Format as da
+0000e4c0: 7465 730a 2020 2020 2020 2020 2020 2020  tes.            
+0000e4d0: 6966 2072 652e 6d61 7463 6828 7222 5e28  if re.match(r"^(
+0000e4e0: 3230 7c31 3929 5c64 7b31 327d 2422 2c20  20|19)\d{12}$", 
+0000e4f0: 7661 6c75 6529 3a0a 2020 2020 2020 2020  value):.        
+0000e500: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
+0000e510: 6461 7465 666d 7428 7661 6c75 652c 2022  datefmt(value, "
+0000e520: 2559 2d25 6d2d 2564 2025 483a 254d 3a25  %Y-%m-%d %H:%M:%
+0000e530: 5322 290a 2020 2020 2020 2020 2020 2020  S").            
+0000e540: 656c 6966 2072 652e 6d61 7463 6828 7222  elif re.match(r"
+0000e550: 5e28 3230 7c31 3929 5c64 7b36 7d24 222c  ^(20|19)\d{6}$",
+0000e560: 2076 616c 7565 293a 0a20 2020 2020 2020   value):.       
+0000e570: 2020 2020 2020 2020 2076 616c 7565 203d           value =
+0000e580: 2064 6174 6566 6d74 2876 616c 7565 2c20   datefmt(value, 
+0000e590: 2225 592d 256d 2d25 6422 290a 0a20 2020  "%Y-%m-%d")..   
+0000e5a0: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
+0000e5b0: 615f 7461 626c 652e 6164 645f 726f 7728  a_table.add_row(
+0000e5c0: 6622 7b6b 6579 7d3a 222c 2076 616c 7565  f"{key}:", value
+0000e5d0: 290a 0a20 2020 2020 2020 206d 6574 6164  )..        metad
+0000e5e0: 6174 615f 7061 6e65 6c20 3d20 5061 6e65  ata_panel = Pane
+0000e5f0: 6c28 0a20 2020 2020 2020 2020 2020 206d  l(.            m
+0000e600: 6574 6164 6174 615f 7461 626c 652c 2074  etadata_table, t
+0000e610: 6974 6c65 3d66 2246 6f72 6d20 7b73 656c  itle=f"Form {sel
+0000e620: 662e 666f 726d 7d20 7b75 6e69 636f 6465  f.form} {unicode
+0000e630: 5f66 6f72 5f66 6f72 6d28 7365 6c66 2e66  _for_form(self.f
+0000e640: 6f72 6d29 7d20 4649 4c49 4e47 220a 2020  orm)} FILING".  
+0000e650: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000e660: 2023 204b 6565 7020 6120 6c69 7374 206f   # Keep a list o
+0000e670: 6620 7265 6e64 6572 6162 6c65 7320 666f  f renderables fo
+0000e680: 7220 7269 6368 0a20 2020 2020 2020 2072  r rich.        r
+0000e690: 656e 6465 7261 626c 6573 203d 205b 6d65  enderables = [me
+0000e6a0: 7461 6461 7461 5f70 616e 656c 5d0a 0a20  tadata_panel].. 
+0000e6b0: 2020 2020 2020 2023 2053 5542 4a45 4354         # SUBJECT
+0000e6c0: 2043 4f4d 5041 4e59 0a20 2020 2020 2020   COMPANY.       
+0000e6d0: 2066 6f72 2073 7562 6a65 6374 5f63 6f6d   for subject_com
+0000e6e0: 7061 6e79 2069 6e20 7365 6c66 2e73 7562  pany in self.sub
+0000e6f0: 6a65 6374 5f63 6f6d 7061 6e69 6573 3a0a  ject_companies:.
+0000e700: 2020 2020 2020 2020 2020 2020 7265 6e64              rend
+0000e710: 6572 6162 6c65 732e 6170 7065 6e64 2873  erables.append(s
+0000e720: 7562 6a65 6374 5f63 6f6d 7061 6e79 2e5f  ubject_company._
+0000e730: 5f72 6963 685f 5f28 2929 0a0a 2020 2020  _rich__())..    
+0000e740: 2020 2020 2320 4649 4c45 520a 2020 2020      # FILER.    
+0000e750: 2020 2020 666f 7220 6669 6c65 7220 696e      for filer in
+0000e760: 2073 656c 662e 6669 6c65 7273 3a0a 2020   self.filers:.  
+0000e770: 2020 2020 2020 2020 2020 7265 6e64 6572            render
+0000e780: 6162 6c65 732e 6170 7065 6e64 2866 696c  ables.append(fil
+0000e790: 6572 2e5f 5f72 6963 685f 5f28 2929 0a0a  er.__rich__())..
+0000e7a0: 2020 2020 2020 2020 2320 5245 504f 5254          # REPORT
+0000e7b0: 494e 4720 4f57 4e45 520a 2020 2020 2020  ING OWNER.      
+0000e7c0: 2020 666f 7220 7265 706f 7274 696e 675f    for reporting_
+0000e7d0: 6f77 6e65 7220 696e 2073 656c 662e 7265  owner in self.re
+0000e7e0: 706f 7274 696e 675f 6f77 6e65 7273 3a0a  porting_owners:.
+0000e7f0: 2020 2020 2020 2020 2020 2020 7265 6e64              rend
+0000e800: 6572 6162 6c65 732e 6170 7065 6e64 2872  erables.append(r
+0000e810: 6570 6f72 7469 6e67 5f6f 776e 6572 2e5f  eporting_owner._
+0000e820: 5f72 6963 685f 5f28 2929 0a0a 2020 2020  _rich__())..    
+0000e830: 2020 2020 2320 4953 5355 4552 0a20 2020      # ISSUER.   
+0000e840: 2020 2020 2066 6f72 2069 7373 7565 7220       for issuer 
+0000e850: 696e 2073 656c 662e 6973 7375 6572 733a  in self.issuers:
+0000e860: 0a20 2020 2020 2020 2020 2020 2072 656e  .            ren
+0000e870: 6465 7261 626c 6573 2e61 7070 656e 6428  derables.append(
+0000e880: 6973 7375 6572 2e5f 5f72 6963 685f 5f28  issuer.__rich__(
+0000e890: 2929 0a20 2020 2020 2020 2072 6574 7572  )).        retur
+0000e8a0: 6e20 5061 6e65 6c28 0a20 2020 2020 2020  n Panel(.       
+0000e8b0: 2020 2020 2047 726f 7570 280a 2020 2020       Group(.    
+0000e8c0: 2020 2020 2020 2020 2020 2020 2a72 656e              *ren
+0000e8d0: 6465 7261 626c 6573 0a20 2020 2020 2020  derables.       
+0000e8e0: 2020 2020 2029 0a20 2020 2020 2020 2029       ).        )
+0000e8f0: 0a0a 2020 2020 6465 6620 5f5f 7265 7072  ..    def __repr
+0000e900: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
+0000e910: 2020 7265 7475 726e 2072 6570 725f 7269    return repr_ri
+0000e920: 6368 2873 656c 662e 5f5f 7269 6368 5f5f  ch(self.__rich__
+0000e930: 2829 290a 0a0a 636c 6173 7320 4669 6c69  ())...class Fili
+0000e940: 6e67 3a0a 2020 2020 2222 220a 2020 2020  ng:.    """.    
+0000e950: 4120 7369 6e67 6c65 2053 4543 2066 696c  A single SEC fil
+0000e960: 696e 672e 2041 6c6c 6f77 2079 6f75 2074  ing. Allow you t
+0000e970: 6f20 6163 6365 7373 2074 6865 2064 6f63  o access the doc
+0000e980: 756d 656e 7473 2061 6e64 2064 6174 6120  uments and data 
+0000e990: 666f 7220 7468 6174 2066 696c 696e 670a  for that filing.
+0000e9a0: 2020 2020 2222 220a 0a20 2020 2064 6566      """..    def
+0000e9b0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c0a   __init__(self,.
+0000e9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9d0: 2063 696b 3a20 696e 742c 0a20 2020 2020   cik: int,.     
+0000e9e0: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
+0000e9f0: 616e 793a 2073 7472 2c0a 2020 2020 2020  any: str,.      
+0000ea00: 2020 2020 2020 2020 2020 2066 6f72 6d3a             form:
+0000ea10: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
+0000ea20: 2020 2020 2020 2066 696c 696e 675f 6461         filing_da
+0000ea30: 7465 3a20 7374 722c 0a20 2020 2020 2020  te: str,.       
+0000ea40: 2020 2020 2020 2020 2020 6163 6365 7373            access
+0000ea50: 696f 6e5f 6e6f 3a20 7374 7229 3a0a 2020  ion_no: str):.  
+0000ea60: 2020 2020 2020 7365 6c66 2e63 696b 203d        self.cik =
+0000ea70: 2063 696b 0a20 2020 2020 2020 2073 656c   cik.        sel
+0000ea80: 662e 636f 6d70 616e 7920 3d20 636f 6d70  f.company = comp
+0000ea90: 616e 790a 2020 2020 2020 2020 7365 6c66  any.        self
+0000eaa0: 2e66 6f72 6d20 3d20 666f 726d 0a20 2020  .form = form.   
+0000eab0: 2020 2020 2073 656c 662e 6669 6c69 6e67       self.filing
+0000eac0: 5f64 6174 6520 3d20 6669 6c69 6e67 5f64  _date = filing_d
+0000ead0: 6174 650a 2020 2020 2020 2020 7365 6c66  ate.        self
+0000eae0: 2e61 6363 6573 7369 6f6e 5f6e 6f20 3d20  .accession_no = 
+0000eaf0: 6163 6365 7373 696f 6e5f 6e6f 0a20 2020  accession_no.   
+0000eb00: 2020 2020 2073 656c 662e 5f66 696c 696e       self._filin
+0000eb10: 675f 686f 6d65 7061 6765 203d 204e 6f6e  g_homepage = Non
+0000eb20: 650a 0a20 2020 2040 7072 6f70 6572 7479  e..    @property
+0000eb30: 0a20 2020 2064 6566 2064 6f63 756d 656e  .    def documen
+0000eb40: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+0000eb50: 2022 2222 0a20 2020 2020 2020 203a 7265   """.        :re
+0000eb60: 7475 726e 3a20 5468 6520 7072 696d 6172  turn: The primar
+0000eb70: 7920 6469 7370 6c61 7920 646f 6375 6d65  y display docume
+0000eb80: 6e74 206f 6e20 7468 6520 6669 6c69 6e67  nt on the filing
+0000eb90: 2c20 6765 6e65 7261 6c6c 7920 4854 4d4c  , generally HTML
+0000eba0: 2062 7574 2063 616e 2062 6520 5848 544d   but can be XHTM
+0000ebb0: 4c0a 2020 2020 2020 2020 2222 220a 2020  L.        """.  
+0000ebc0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000ebd0: 662e 686f 6d65 7061 6765 2e70 7269 6d61  f.homepage.prima
+0000ebe0: 7279 5f68 746d 6c5f 646f 6375 6d65 6e74  ry_html_document
+0000ebf0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0000ec00: 2020 2020 6465 6620 7072 696d 6172 795f      def primary_
+0000ec10: 646f 6375 6d65 6e74 7328 7365 6c66 293a  documents(self):
+0000ec20: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000ec30: 2020 2020 203a 7265 7475 726e 3a20 6120       :return: a 
+0000ec40: 6c69 7374 206f 6620 7468 6520 7072 696d  list of the prim
+0000ec50: 6172 7920 646f 6375 6d65 6e74 7320 6f6e  ary documents on
+0000ec60: 2074 6865 2066 696c 696e 672c 2067 656e   the filing, gen
+0000ec70: 6572 616c 6c79 2048 544d 4c20 6f72 2058  erally HTML or X
+0000ec80: 4854 4d4c 2061 6e64 206f 7074 696f 6e61  HTML and optiona
+0000ec90: 6c6c 7920 584d 4c0a 2020 2020 2020 2020  lly XML.        
+0000eca0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+0000ecb0: 726e 2073 656c 662e 686f 6d65 7061 6765  rn self.homepage
+0000ecc0: 2e70 7269 6d61 7279 5f64 6f63 756d 656e  .primary_documen
+0000ecd0: 7473 0a0a 2020 2020 4070 726f 7065 7274  ts..    @propert
+0000ece0: 790a 2020 2020 6465 6620 6174 7461 6368  y.    def attach
+0000ecf0: 6d65 6e74 7328 7365 6c66 293a 0a20 2020  ments(self):.   
+0000ed00: 2020 2020 2023 2052 6574 7572 6e20 616c       # Return al
+0000ed10: 6c20 7468 6520 6174 7461 6368 6d65 6e74  l the attachment
+0000ed20: 7320 6f6e 2074 6865 2066 696c 696e 670a  s on the filing.
+0000ed30: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000ed40: 656c 662e 686f 6d65 7061 6765 2e61 7474  elf.homepage.att
+0000ed50: 6163 686d 656e 7473 0a0a 2020 2020 6465  achments..    de
+0000ed60: 6620 6874 6d6c 2873 656c 6629 202d 3e20  f html(self) -> 
+0000ed70: 4f70 7469 6f6e 616c 5b73 7472 5d3a 0a20  Optional[str]:. 
+0000ed80: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
+0000ed90: 7320 7468 6520 6874 6d6c 2063 6f6e 7465  s the html conte
+0000eda0: 6e74 7320 6f66 2074 6865 2070 7269 6d61  nts of the prima
+0000edb0: 7279 2064 6f63 756d 656e 7420 6966 2069  ry document if i
+0000edc0: 7420 6973 2068 746d 6c22 2222 0a20 2020  t is html""".   
+0000edd0: 2020 2020 2069 6620 7365 6c66 2e64 6f63       if self.doc
+0000ede0: 756d 656e 742e 6973 5f62 696e 6172 7928  ument.is_binary(
+0000edf0: 293a 0a20 2020 2020 2020 2020 2020 206c  ):.            l
+0000ee00: 6f67 2e69 6e66 6f28 6622 5072 696d 6172  og.info(f"Primar
+0000ee10: 7920 646f 6375 6d65 6e74 207b 7365 6c66  y document {self
+0000ee20: 2e64 6f63 756d 656e 742e 7572 6c7d 2069  .document.url} i
+0000ee30: 7320 6120 6269 6e61 7279 2066 696c 6522  s a binary file"
+0000ee40: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+0000ee50: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000ee60: 726e 2073 656c 662e 646f 6375 6d65 6e74  rn self.document
+0000ee70: 2e64 6f77 6e6c 6f61 6428 290a 0a20 2020  .download()..   
+0000ee80: 2064 6566 2078 6d6c 2873 656c 6629 202d   def xml(self) -
+0000ee90: 3e20 4f70 7469 6f6e 616c 5b73 7472 5d3a  > Optional[str]:
+0000eea0: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+0000eeb0: 726e 7320 7468 6520 786d 6c20 636f 6e74  rns the xml cont
+0000eec0: 656e 7473 206f 6620 7468 6520 7072 696d  ents of the prim
+0000eed0: 6172 7920 646f 6375 6d65 6e74 2069 6620  ary document if 
+0000eee0: 6974 2069 7320 786d 6c22 2222 0a20 2020  it is xml""".   
+0000eef0: 2020 2020 2078 6d6c 5f64 6f63 756d 656e       xml_documen
+0000ef00: 743a 2041 7474 6163 686d 656e 7420 3d20  t: Attachment = 
+0000ef10: 7365 6c66 2e68 6f6d 6570 6167 652e 7072  self.homepage.pr
+0000ef20: 696d 6172 795f 786d 6c5f 646f 6375 6d65  imary_xml_docume
+0000ef30: 6e74 0a20 2020 2020 2020 2069 6620 786d  nt.        if xm
+0000ef40: 6c5f 646f 6375 6d65 6e74 3a0a 2020 2020  l_document:.    
+0000ef50: 2020 2020 2020 2020 7265 7475 726e 2078          return x
+0000ef60: 6d6c 5f64 6f63 756d 656e 742e 646f 776e  ml_document.down
+0000ef70: 6c6f 6164 2829 0a0a 2020 2020 406c 7275  load()..    @lru
+0000ef80: 5f63 6163 6865 286d 6178 7369 7a65 3d34  _cache(maxsize=4
+0000ef90: 290a 2020 2020 6465 6620 7465 7874 2873  ).    def text(s
+0000efa0: 656c 662c 2069 676e 6f72 655f 7461 626c  elf, ignore_tabl
+0000efb0: 6573 3d46 616c 7365 2c20 7365 703d 225c  es=False, sep="\
+0000efc0: 6e22 2920 2d3e 2073 7472 3a0a 2020 2020  n") -> str:.    
+0000efd0: 2020 2020 2222 2243 6f6e 7665 7274 2074      """Convert t
+0000efe0: 6865 2068 746d 6c20 6f66 2074 6865 206d  he html of the m
+0000eff0: 6169 6e20 6669 6c69 6e67 2064 6f63 756d  ain filing docum
+0000f000: 656e 7420 746f 2074 6578 7422 2222 0a20  ent to text""". 
+0000f010: 2020 2020 2020 2068 746d 6c5f 636f 6e74         html_cont
+0000f020: 656e 7420 3d20 7365 6c66 2e68 746d 6c28  ent = self.html(
+0000f030: 290a 2020 2020 2020 2020 6966 2068 746d  ).        if htm
+0000f040: 6c5f 636f 6e74 656e 743a 0a20 2020 2020  l_content:.     
+0000f050: 2020 2020 2020 2072 6574 7572 6e20 6874         return ht
+0000f060: 6d6c 5f74 6f5f 7465 7874 2868 746d 6c5f  ml_to_text(html_
+0000f070: 636f 6e74 656e 742c 2069 676e 6f72 655f  content, ignore_
+0000f080: 7461 626c 6573 3d69 676e 6f72 655f 7461  tables=ignore_ta
+0000f090: 626c 6573 2c20 7365 703d 7365 7029 0a0a  bles, sep=sep)..
+0000f0a0: 2020 2020 6465 6620 6675 6c6c 5f74 6578      def full_tex
+0000f0b0: 745f 7375 626d 6973 7369 6f6e 2873 656c  t_submission(sel
+0000f0c0: 6629 202d 3e20 7374 723a 0a20 2020 2020  f) -> str:.     
+0000f0d0: 2020 2022 2222 5265 7475 726e 2074 6865     """Return the
+0000f0e0: 2063 6f6d 706c 6574 6520 7465 7874 2073   complete text s
+0000f0f0: 7562 6d69 7373 696f 6e20 6669 6c65 2222  ubmission file""
+0000f100: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+0000f110: 2064 6f77 6e6c 6f61 645f 6669 6c65 2873   download_file(s
+0000f120: 656c 662e 7465 7874 5f75 726c 290a 0a20  elf.text_url).. 
+0000f130: 2020 2064 6566 206d 6172 6b64 6f77 6e28     def markdown(
+0000f140: 7365 6c66 2920 2d3e 2073 7472 3a0a 2020  self) -> str:.  
+0000f150: 2020 2020 2020 2222 2272 6574 7572 6e20        """return 
+0000f160: 7468 6520 6d61 726b 646f 776e 2076 6572  the markdown ver
+0000f170: 7369 6f6e 206f 6620 7468 6973 2066 696c  sion of this fil
+0000f180: 696e 6720 6874 6d6c 2222 220a 2020 2020  ing html""".    
+0000f190: 2020 2020 7265 7475 726e 2068 746d 6c5f      return html_
+0000f1a0: 746f 5f6d 6172 6b64 6f77 6e28 7365 6c66  to_markdown(self
+0000f1b0: 2e68 746d 6c28 2929 0a0a 2020 2020 6465  .html())..    de
+0000f1c0: 6620 7669 6577 2873 656c 6629 3a0a 2020  f view(self):.  
+0000f1d0: 2020 2020 2020 2222 2250 7265 7669 6577        """Preview
+0000f1e0: 2074 6869 7320 6669 6c69 6e67 2773 2070   this filing's p
+0000f1f0: 7269 6d61 7279 2064 6f63 756d 656e 7420  rimary document 
+0000f200: 6173 206d 6172 6b64 6f77 6e2e 2054 6869  as markdown. Thi
+0000f210: 7320 7368 6f75 6c64 2064 6973 706c 6179  s should display
+0000f220: 2069 6e20 7468 6520 636f 6e73 6f6c 6522   in the console"
+0000f230: 2222 0a20 2020 2020 2020 2063 6f6e 736f  "".        conso
+0000f240: 6c65 203d 2043 6f6e 736f 6c65 2829 0a20  le = Console(). 
+0000f250: 2020 2020 2020 2063 6f6e 736f 6c65 2e70         console.p
+0000f260: 7269 6e74 284d 6172 6b64 6f77 6e43 6f6e  rint(MarkdownCon
+0000f270: 7465 6e74 2873 656c 662e 6874 6d6c 2829  tent(self.html()
+0000f280: 2c20 7469 746c 653d 6622 466f 726d 207b  , title=f"Form {
+0000f290: 7365 6c66 2e66 6f72 6d7d 2066 6f72 207b  self.form} for {
+0000f2a0: 7365 6c66 2e63 6f6d 7061 6e79 7d22 2929  self.company}"))
+0000f2b0: 0a0a 2020 2020 6465 6620 7862 726c 2873  ..    def xbrl(s
+0000f2c0: 656c 6629 202d 3e20 4f70 7469 6f6e 616c  elf) -> Optional
+0000f2d0: 5b46 696c 696e 6758 6272 6c5d 3a0a 2020  [FilingXbrl]:.  
+0000f2e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000f2f0: 2020 4765 7420 7468 6520 5842 524c 2064    Get the XBRL d
+0000f300: 6f63 756d 656e 7420 666f 7220 7468 6520  ocument for the 
+0000f310: 6669 6c69 6e67 2c20 7061 7273 6564 2061  filing, parsed a
+0000f320: 6e64 2061 7320 6120 4669 6c69 6e67 5862  nd as a FilingXb
+0000f330: 726c 206f 626a 6563 740a 2020 2020 2020  rl object.      
+0000f340: 2020 3a72 6574 7572 6e3a 2047 6574 2074    :return: Get t
+0000f350: 6865 2058 4252 4c20 646f 6375 6d65 6e74  he XBRL document
+0000f360: 2066 6f72 2074 6865 2066 696c 696e 672c   for the filing,
+0000f370: 2070 6172 7365 6420 616e 6420 6173 2061   parsed and as a
+0000f380: 2046 696c 696e 6758 6272 6c20 6f62 6a65   FilingXbrl obje
+0000f390: 6374 2c20 6f72 204e 6f6e 650a 2020 2020  ct, or None.    
+0000f3a0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000f3b0: 7862 726c 5f64 6f63 756d 656e 7420 3d20  xbrl_document = 
+0000f3c0: 7365 6c66 2e68 6f6d 6570 6167 652e 7862  self.homepage.xb
+0000f3d0: 726c 5f64 6f63 756d 656e 740a 2020 2020  rl_document.    
+0000f3e0: 2020 2020 6966 2078 6272 6c5f 646f 6375      if xbrl_docu
+0000f3f0: 6d65 6e74 3a0a 2020 2020 2020 2020 2020  ment:.          
+0000f400: 2020 7862 726c 5f74 6578 7420 3d20 7862    xbrl_text = xb
+0000f410: 726c 5f64 6f63 756d 656e 742e 646f 776e  rl_document.down
+0000f420: 6c6f 6164 2829 0a20 2020 2020 2020 2020  load().         
+0000f430: 2020 2072 6574 7572 6e20 4669 6c69 6e67     return Filing
+0000f440: 5862 726c 2e70 6172 7365 2878 6272 6c5f  Xbrl.parse(xbrl_
+0000f450: 7465 7874 290a 0a20 2020 2040 7072 6f70  text)..    @prop
+0000f460: 6572 7479 0a20 2020 2040 6c72 755f 6361  erty.    @lru_ca
+0000f470: 6368 6528 6d61 7873 697a 653d 3129 0a20  che(maxsize=1). 
+0000f480: 2020 2064 6566 2068 6561 6465 7228 7365     def header(se
+0000f490: 6c66 293a 0a20 2020 2020 2020 2073 6563  lf):.        sec
+0000f4a0: 5f68 6561 6465 725f 636f 6e74 656e 7420  _header_content 
+0000f4b0: 3d20 6765 745f 7465 7874 5f62 6574 7765  = get_text_betwe
+0000f4c0: 656e 5f74 6167 7328 7365 6c66 2e74 6578  en_tags(self.tex
+0000f4d0: 745f 7572 6c2c 2022 5345 432d 4845 4144  t_url, "SEC-HEAD
+0000f4e0: 4552 2229 0a20 2020 2020 2020 2072 6574  ER").        ret
+0000f4f0: 7572 6e20 5345 4348 6561 6465 722e 7061  urn SECHeader.pa
+0000f500: 7273 6528 7365 635f 6865 6164 6572 5f63  rse(sec_header_c
+0000f510: 6f6e 7465 6e74 290a 0a20 2020 2064 6566  ontent)..    def
+0000f520: 2064 6174 615f 6f62 6a65 6374 2873 656c   data_object(sel
+0000f530: 6629 3a0a 2020 2020 2020 2020 2222 2220  f):.        """ 
+0000f540: 4765 7420 7468 6973 2066 696c 696e 6720  Get this filing 
+0000f550: 6173 2074 6865 2064 6174 6120 6f62 6a65  as the data obje
+0000f560: 6374 2074 6861 7420 6974 206d 6967 6874  ct that it might
+0000f570: 2062 6522 2222 0a20 2020 2020 2020 2066   be""".        f
+0000f580: 726f 6d20 6564 6761 7220 696d 706f 7274  rom edgar import
+0000f590: 206f 626a 0a20 2020 2020 2020 2072 6574   obj.        ret
+0000f5a0: 7572 6e20 6f62 6a28 7365 6c66 290a 0a20  urn obj(self).. 
+0000f5b0: 2020 2064 6566 206f 626a 2873 656c 6629     def obj(self)
+0000f5c0: 3a0a 2020 2020 2020 2020 2222 2241 6c69  :.        """Ali
+0000f5d0: 6173 2066 6f72 2064 6174 615f 6f62 6a65  as for data_obje
+0000f5e0: 6374 2829 2222 220a 2020 2020 2020 2020  ct()""".        
+0000f5f0: 7265 7475 726e 2073 656c 662e 6461 7461  return self.data
+0000f600: 5f6f 626a 6563 7428 290a 0a20 2020 2064  _object()..    d
+0000f610: 6566 206f 7065 6e5f 686f 6d65 7061 6765  ef open_homepage
+0000f620: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000f630: 2222 224f 7065 6e20 7468 6520 686f 6d65  """Open the home
+0000f640: 7061 6765 2069 6e20 7468 6520 6272 6f77  page in the brow
+0000f650: 7365 7222 2222 0a20 2020 2020 2020 2077  ser""".        w
+0000f660: 6562 6272 6f77 7365 722e 6f70 656e 2873  ebbrowser.open(s
+0000f670: 656c 662e 686f 6d65 7061 6765 5f75 726c  elf.homepage_url
+0000f680: 290a 0a20 2020 2064 6566 206f 7065 6e28  )..    def open(
+0000f690: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000f6a0: 2222 4f70 656e 2074 6865 206d 6169 6e20  ""Open the main 
+0000f6b0: 6669 6c69 6e67 2064 6f63 756d 656e 7422  filing document"
+0000f6c0: 2222 0a20 2020 2020 2020 2077 6562 6272  "".        webbr
+0000f6d0: 6f77 7365 722e 6f70 656e 2873 656c 662e  owser.open(self.
+0000f6e0: 646f 6375 6d65 6e74 2e75 726c 290a 0a20  document.url).. 
+0000f6f0: 2020 2040 6c72 755f 6361 6368 6528 6d61     @lru_cache(ma
+0000f700: 7873 697a 653d 3129 0a20 2020 2064 6566  xsize=1).    def
+0000f710: 2073 6563 7469 6f6e 7328 7365 6c66 2920   sections(self) 
+0000f720: 2d3e 204c 6973 745b 7374 725d 3a0a 2020  -> List[str]:.  
+0000f730: 2020 2020 2020 7265 7475 726e 2068 746d        return htm
+0000f740: 6c5f 7365 6374 696f 6e73 2873 656c 662e  l_sections(self.
+0000f750: 6874 6d6c 2829 290a 0a20 2020 2040 6c72  html())..    @lr
+0000f760: 755f 6361 6368 6528 6d61 7873 697a 653d  u_cache(maxsize=
+0000f770: 3129 0a20 2020 2064 6566 205f 5f67 6574  1).    def __get
+0000f780: 5f62 6d32 355f 7365 6172 6368 5f69 6e64  _bm25_search_ind
+0000f790: 6578 2873 656c 6629 3a0a 2020 2020 2020  ex(self):.      
+0000f7a0: 2020 7265 7475 726e 2042 4d32 3553 6561    return BM25Sea
+0000f7b0: 7263 6828 7365 6c66 2e73 6563 7469 6f6e  rch(self.section
+0000f7c0: 7328 2929 0a0a 2020 2020 406c 7275 5f63  s())..    @lru_c
+0000f7d0: 6163 6865 286d 6178 7369 7a65 3d31 290a  ache(maxsize=1).
+0000f7e0: 2020 2020 6465 6620 5f5f 6765 745f 7265      def __get_re
+0000f7f0: 6765 785f 7365 6172 6368 5f69 6e64 6578  gex_search_index
+0000f800: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000f810: 7265 7475 726e 2052 6567 6578 5365 6172  return RegexSear
+0000f820: 6368 2873 656c 662e 7365 6374 696f 6e73  ch(self.sections
+0000f830: 2829 290a 0a20 2020 2064 6566 2073 6561  ())..    def sea
+0000f840: 7263 6828 7365 6c66 2c0a 2020 2020 2020  rch(self,.      
+0000f850: 2020 2020 2020 2020 2071 7565 7279 3a20           query: 
+0000f860: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
+0000f870: 2020 2020 7265 6765 783d 4661 6c73 6529      regex=False)
+0000f880: 3a0a 2020 2020 2020 2020 2222 2253 6561  :.        """Sea
+0000f890: 7263 6820 666f 7220 7468 6520 7175 6572  rch for the quer
+0000f8a0: 7920 7374 7269 6e67 2069 6e20 7468 6520  y string in the 
+0000f8b0: 6669 6c69 6e67 2048 544d 4c22 2222 0a20  filing HTML""". 
+0000f8c0: 2020 2020 2020 2069 6620 7265 6765 783a         if regex:
+0000f8d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000f8e0: 7572 6e20 7365 6c66 2e5f 5f67 6574 5f72  urn self.__get_r
+0000f8f0: 6567 6578 5f73 6561 7263 685f 696e 6465  egex_search_inde
+0000f900: 7828 292e 7365 6172 6368 2871 7565 7279  x().search(query
+0000f910: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0000f920: 2073 656c 662e 5f5f 6765 745f 626d 3235   self.__get_bm25
+0000f930: 5f73 6561 7263 685f 696e 6465 7828 292e  _search_index().
+0000f940: 7365 6172 6368 2871 7565 7279 290a 0a20  search(query).. 
+0000f950: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+0000f960: 2064 6566 2068 6f6d 6570 6167 655f 7572   def homepage_ur
+0000f970: 6c28 7365 6c66 2920 2d3e 2073 7472 3a0a  l(self) -> str:.
+0000f980: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+0000f990: 227b 7365 635f 6564 6761 727d 2f64 6174  "{sec_edgar}/dat
+0000f9a0: 612f 7b73 656c 662e 6369 6b7d 2f7b 7365  a/{self.cik}/{se
+0000f9b0: 6c66 2e61 6363 6573 7369 6f6e 5f6e 6f7d  lf.accession_no}
+0000f9c0: 2d69 6e64 6578 2e68 746d 6c22 0a0a 2020  -index.html"..  
+0000f9d0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+0000f9e0: 6465 6620 7465 7874 5f75 726c 2873 656c  def text_url(sel
+0000f9f0: 6629 202d 3e20 7374 723a 0a20 2020 2020  f) -> str:.     
+0000fa00: 2020 2072 6574 7572 6e20 6622 7b73 6563     return f"{sec
+0000fa10: 5f65 6467 6172 7d2f 6461 7461 2f7b 7365  _edgar}/data/{se
+0000fa20: 6c66 2e63 696b 7d2f 7b73 656c 662e 6163  lf.cik}/{self.ac
+0000fa30: 6365 7373 696f 6e5f 6e6f 2e72 6570 6c61  cession_no.repla
+0000fa40: 6365 2827 2d27 2c20 2727 297d 2f7b 7365  ce('-', '')}/{se
+0000fa50: 6c66 2e61 6363 6573 7369 6f6e 5f6e 6f7d  lf.accession_no}
+0000fa60: 2e74 7874 220a 0a20 2020 2040 7072 6f70  .txt"..    @prop
+0000fa70: 6572 7479 0a20 2020 2064 6566 2075 726c  erty.    def url
+0000fa80: 2873 656c 6629 202d 3e20 7374 723a 0a20  (self) -> str:. 
+0000fa90: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000faa0: 6c66 2e68 6f6d 6570 6167 655f 7572 6c0a  lf.homepage_url.
+0000fab0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+0000fac0: 2020 2064 6566 2068 6f6d 6570 6167 6528     def homepage(
+0000fad0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000fae0: 2222 0a20 2020 2020 2020 2047 6574 2074  "".        Get t
+0000faf0: 6865 2068 6f6d 6570 6167 6520 666f 7220  he homepage for 
+0000fb00: 7468 6520 6669 6c69 6e67 0a20 2020 2020  the filing.     
+0000fb10: 2020 203a 7265 7475 726e 3a20 7468 6520     :return: the 
+0000fb20: 4669 6c69 6e67 486f 6d65 7061 6765 0a20  FilingHomepage. 
+0000fb30: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000fb40: 2020 2069 6620 6e6f 7420 7365 6c66 2e5f     if not self._
+0000fb50: 6669 6c69 6e67 5f68 6f6d 6570 6167 653a  filing_homepage:
+0000fb60: 0a20 2020 2020 2020 2020 2020 2068 6f6d  .            hom
+0000fb70: 6570 6167 655f 6874 6d6c 203d 2064 6f77  epage_html = dow
+0000fb80: 6e6c 6f61 645f 7465 7874 2873 656c 662e  nload_text(self.
+0000fb90: 686f 6d65 7061 6765 5f75 726c 290a 2020  homepage_url).  
+0000fba0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000fbb0: 6669 6c69 6e67 5f68 6f6d 6570 6167 6520  filing_homepage 
+0000fbc0: 3d20 4669 6c69 6e67 486f 6d65 7061 6765  = FilingHomepage
+0000fbd0: 2e66 726f 6d5f 6874 6d6c 2868 6f6d 6570  .from_html(homep
+0000fbe0: 6167 655f 6874 6d6c 2c0a 2020 2020 2020  age_html,.      
 0000fbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000fc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000fc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc20: 2020 7572 6c3d 7365 6c66 2e68 6f6d 6570    url=self.homep
-0000fc30: 6167 655f 7572 6c2c 0a20 2020 2020 2020  age_url,.       
+0000fc20: 2020 2020 2020 2075 726c 3d73 656c 662e         url=self.
+0000fc30: 686f 6d65 7061 6765 5f75 726c 2c0a 2020  homepage_url,.  
 0000fc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000fc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000fc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc70: 2020 2020 2020 6669 6c69 6e67 3d73 656c        filing=sel
-0000fc80: 6629 0a20 2020 2020 2020 2072 6574 7572  f).        retur
-0000fc90: 6e20 7365 6c66 2e5f 6669 6c69 6e67 5f68  n self._filing_h
-0000fca0: 6f6d 6570 6167 650a 0a20 2020 2040 7072  omepage..    @pr
-0000fcb0: 6f70 6572 7479 0a20 2020 2064 6566 2068  operty.    def h
-0000fcc0: 6f6d 6528 7365 6c66 293a 0a20 2020 2020  ome(self):.     
-0000fcd0: 2020 2022 2222 416c 6961 7320 666f 7220     """Alias for 
-0000fce0: 686f 6d65 7061 6765 2222 220a 2020 2020  homepage""".    
-0000fcf0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000fd00: 686f 6d65 7061 6765 0a0a 2020 2020 406c  homepage..    @l
-0000fd10: 7275 5f63 6163 6865 286d 6178 7369 7a65  ru_cache(maxsize
-0000fd20: 3d31 290a 2020 2020 6465 6620 6765 745f  =1).    def get_
-0000fd30: 656e 7469 7479 2873 656c 6629 3a0a 2020  entity(self):.  
-0000fd40: 2020 2020 2020 2222 2247 6574 2074 6865        """Get the
-0000fd50: 2063 6f6d 7061 6e79 2074 6f20 7768 6963   company to whic
-0000fd60: 6820 7468 6973 2066 696c 696e 6720 6265  h this filing be
-0000fd70: 6c6f 6e67 7322 2222 0a20 2020 2020 2020  longs""".       
-0000fd80: 2022 4765 7420 7468 6520 636f 6d70 616e   "Get the compan
-0000fd90: 7920 666f 7220 6369 6b2e 2043 6163 6865  y for cik. Cache
-0000fda0: 2066 6f72 2070 6572 666f 726d 616e 6365   for performance
-0000fdb0: 220a 2020 2020 2020 2020 6672 6f6d 2065  ".        from e
-0000fdc0: 6467 6172 2e5f 636f 6d70 616e 6965 7320  dgar._companies 
-0000fdd0: 696d 706f 7274 2043 6f6d 7061 6e79 4461  import CompanyDa
-0000fde0: 7461 0a20 2020 2020 2020 2072 6574 7572  ta.        retur
-0000fdf0: 6e20 436f 6d70 616e 7944 6174 612e 666f  n CompanyData.fo
-0000fe00: 725f 6369 6b28 7365 6c66 2e63 696b 290a  r_cik(self.cik).
-0000fe10: 0a20 2020 2040 6c72 755f 6361 6368 6528  .    @lru_cache(
-0000fe20: 6d61 7873 697a 653d 3129 0a20 2020 2064  maxsize=1).    d
-0000fe30: 6566 2061 735f 636f 6d70 616e 795f 6669  ef as_company_fi
-0000fe40: 6c69 6e67 2873 656c 6629 3a0a 2020 2020  ling(self):.    
-0000fe50: 2020 2020 2222 2247 6574 2074 6869 7320      """Get this 
-0000fe60: 6669 6c69 6e67 2061 7320 6120 636f 6d70  filing as a comp
-0000fe70: 616e 7920 6669 6c69 6e67 2e20 436f 6d70  any filing. Comp
-0000fe80: 616e 7920 4669 6c69 6e67 7320 6861 7665  any Filings have
-0000fe90: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
-0000fea0: 6e22 2222 0a20 2020 2020 2020 2063 6f6d  n""".        com
-0000feb0: 7061 6e79 203d 2073 656c 662e 6765 745f  pany = self.get_
-0000fec0: 656e 7469 7479 2829 0a20 2020 2020 2020  entity().       
-0000fed0: 2066 696c 696e 6773 203d 2063 6f6d 7061   filings = compa
-0000fee0: 6e79 2e67 6574 5f66 696c 696e 6773 2861  ny.get_filings(a
-0000fef0: 6363 6573 7369 6f6e 5f6e 756d 6265 723d  ccession_number=
-0000ff00: 7365 6c66 2e61 6363 6573 7369 6f6e 5f6e  self.accession_n
-0000ff10: 6f29 0a20 2020 2020 2020 2069 6620 6e6f  o).        if no
-0000ff20: 7420 6669 6c69 6e67 732e 656d 7074 793a  t filings.empty:
-0000ff30: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000ff40: 7572 6e20 6669 6c69 6e67 735b 305d 0a0a  urn filings[0]..
-0000ff50: 2020 2020 406c 7275 5f63 6163 6865 286d      @lru_cache(m
-0000ff60: 6178 7369 7a65 3d31 290a 2020 2020 6465  axsize=1).    de
-0000ff70: 6620 7265 6c61 7465 645f 6669 6c69 6e67  f related_filing
-0000ff80: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
-0000ff90: 2022 2222 4765 7420 616c 6c20 7468 6520   """Get all the 
-0000ffa0: 6669 6c69 6e67 7320 7265 6c61 7465 6420  filings related 
-0000ffb0: 746f 2074 6869 7320 6f6e 650a 2020 2020  to this one.    
-0000ffc0: 2020 2020 5468 6572 6520 6973 206e 6f20      There is no 
-0000ffd0: 6669 6c65 206e 756d 6265 7220 6f6e 2074  file number on t
-0000ffe0: 6869 7320 6261 7365 2046 696c 696e 6720  his base Filing 
-0000fff0: 636c 6173 7320 736f 2066 6972 7374 2067  class so first g
-00010000: 6574 2074 6865 2063 6f6d 7061 6e79 2c0a  et the company,.
-00010010: 0a20 2020 2020 2020 2074 6865 6e20 7468  .        then th
-00010020: 6973 2066 696c 696e 6720 7468 656e 2067  is filing then g
-00010030: 6574 2074 6865 2072 656c 6174 6564 2066  et the related f
-00010040: 696c 696e 6773 0a20 2020 2020 2020 2022  ilings.        "
-00010050: 2222 0a20 2020 2020 2020 2063 6f6d 7061  "".        compa
-00010060: 6e79 203d 2073 656c 662e 6765 745f 656e  ny = self.get_en
-00010070: 7469 7479 2829 0a20 2020 2020 2020 2066  tity().        f
-00010080: 696c 696e 6773 203d 2063 6f6d 7061 6e79  ilings = company
-00010090: 2e67 6574 5f66 696c 696e 6773 2861 6363  .get_filings(acc
-000100a0: 6573 7369 6f6e 5f6e 756d 6265 723d 7365  ession_number=se
-000100b0: 6c66 2e61 6363 6573 7369 6f6e 5f6e 6f29  lf.accession_no)
-000100c0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-000100d0: 6669 6c69 6e67 732e 656d 7074 793a 0a20  filings.empty:. 
-000100e0: 2020 2020 2020 2020 2020 2066 696c 655f             file_
-000100f0: 6e75 6d62 6572 203d 2066 696c 696e 6773  number = filings
-00010100: 5b30 5d2e 6669 6c65 5f6e 756d 6265 720a  [0].file_number.
-00010110: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00010120: 726e 2063 6f6d 7061 6e79 2e67 6574 5f66  rn company.get_f
-00010130: 696c 696e 6773 2866 696c 655f 6e75 6d62  ilings(file_numb
-00010140: 6572 3d66 696c 655f 6e75 6d62 6572 2c0a  er=file_number,.
-00010150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc70: 2020 2020 2020 2020 2020 2066 696c 696e             filin
+0000fc80: 673d 7365 6c66 290a 2020 2020 2020 2020  g=self).        
+0000fc90: 7265 7475 726e 2073 656c 662e 5f66 696c  return self._fil
+0000fca0: 696e 675f 686f 6d65 7061 6765 0a0a 2020  ing_homepage..  
+0000fcb0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+0000fcc0: 6465 6620 686f 6d65 2873 656c 6629 3a0a  def home(self):.
+0000fcd0: 2020 2020 2020 2020 2222 2241 6c69 6173          """Alias
+0000fce0: 2066 6f72 2068 6f6d 6570 6167 6522 2222   for homepage"""
+0000fcf0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000fd00: 7365 6c66 2e68 6f6d 6570 6167 650a 0a20  self.homepage.. 
+0000fd10: 2020 2040 6c72 755f 6361 6368 6528 6d61     @lru_cache(ma
+0000fd20: 7873 697a 653d 3129 0a20 2020 2064 6566  xsize=1).    def
+0000fd30: 2067 6574 5f65 6e74 6974 7928 7365 6c66   get_entity(self
+0000fd40: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
+0000fd50: 7420 7468 6520 636f 6d70 616e 7920 746f  t the company to
+0000fd60: 2077 6869 6368 2074 6869 7320 6669 6c69   which this fili
+0000fd70: 6e67 2062 656c 6f6e 6773 2222 220a 2020  ng belongs""".  
+0000fd80: 2020 2020 2020 2247 6574 2074 6865 2063        "Get the c
+0000fd90: 6f6d 7061 6e79 2066 6f72 2063 696b 2e20  ompany for cik. 
+0000fda0: 4361 6368 6520 666f 7220 7065 7266 6f72  Cache for perfor
+0000fdb0: 6d61 6e63 6522 0a20 2020 2020 2020 2066  mance".        f
+0000fdc0: 726f 6d20 6564 6761 722e 5f63 6f6d 7061  rom edgar._compa
+0000fdd0: 6e69 6573 2069 6d70 6f72 7420 436f 6d70  nies import Comp
+0000fde0: 616e 7944 6174 610a 2020 2020 2020 2020  anyData.        
+0000fdf0: 7265 7475 726e 2043 6f6d 7061 6e79 4461  return CompanyDa
+0000fe00: 7461 2e66 6f72 5f63 696b 2873 656c 662e  ta.for_cik(self.
+0000fe10: 6369 6b29 0a0a 2020 2020 406c 7275 5f63  cik)..    @lru_c
+0000fe20: 6163 6865 286d 6178 7369 7a65 3d31 290a  ache(maxsize=1).
+0000fe30: 2020 2020 6465 6620 6173 5f63 6f6d 7061      def as_compa
+0000fe40: 6e79 5f66 696c 696e 6728 7365 6c66 293a  ny_filing(self):
+0000fe50: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
+0000fe60: 7468 6973 2066 696c 696e 6720 6173 2061  this filing as a
+0000fe70: 2063 6f6d 7061 6e79 2066 696c 696e 672e   company filing.
+0000fe80: 2043 6f6d 7061 6e79 2046 696c 696e 6773   Company Filings
+0000fe90: 2068 6176 6520 6d6f 7265 2069 6e66 6f72   have more infor
+0000fea0: 6d61 7469 6f6e 2222 220a 2020 2020 2020  mation""".      
+0000feb0: 2020 636f 6d70 616e 7920 3d20 7365 6c66    company = self
+0000fec0: 2e67 6574 5f65 6e74 6974 7928 290a 2020  .get_entity().  
+0000fed0: 2020 2020 2020 6669 6c69 6e67 7320 3d20        filings = 
+0000fee0: 636f 6d70 616e 792e 6765 745f 6669 6c69  company.get_fili
+0000fef0: 6e67 7328 6163 6365 7373 696f 6e5f 6e75  ngs(accession_nu
+0000ff00: 6d62 6572 3d73 656c 662e 6163 6365 7373  mber=self.access
+0000ff10: 696f 6e5f 6e6f 290a 2020 2020 2020 2020  ion_no).        
+0000ff20: 6966 206e 6f74 2066 696c 696e 6773 2e65  if not filings.e
+0000ff30: 6d70 7479 3a0a 2020 2020 2020 2020 2020  mpty:.          
+0000ff40: 2020 7265 7475 726e 2066 696c 696e 6773    return filings
+0000ff50: 5b30 5d0a 0a20 2020 2040 6c72 755f 6361  [0]..    @lru_ca
+0000ff60: 6368 6528 6d61 7873 697a 653d 3129 0a20  che(maxsize=1). 
+0000ff70: 2020 2064 6566 2072 656c 6174 6564 5f66     def related_f
+0000ff80: 696c 696e 6773 2873 656c 6629 3a0a 2020  ilings(self):.  
+0000ff90: 2020 2020 2020 2222 2247 6574 2061 6c6c        """Get all
+0000ffa0: 2074 6865 2066 696c 696e 6773 2072 656c   the filings rel
+0000ffb0: 6174 6564 2074 6f20 7468 6973 206f 6e65  ated to this one
+0000ffc0: 0a20 2020 2020 2020 2054 6865 7265 2069  .        There i
+0000ffd0: 7320 6e6f 2066 696c 6520 6e75 6d62 6572  s no file number
+0000ffe0: 206f 6e20 7468 6973 2062 6173 6520 4669   on this base Fi
+0000fff0: 6c69 6e67 2063 6c61 7373 2073 6f20 6669  ling class so fi
+00010000: 7273 7420 6765 7420 7468 6520 636f 6d70  rst get the comp
+00010010: 616e 792c 0a0a 2020 2020 2020 2020 7468  any,..        th
+00010020: 656e 2074 6869 7320 6669 6c69 6e67 2074  en this filing t
+00010030: 6865 6e20 6765 7420 7468 6520 7265 6c61  hen get the rela
+00010040: 7465 6420 6669 6c69 6e67 730a 2020 2020  ted filings.    
+00010050: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00010060: 636f 6d70 616e 7920 3d20 7365 6c66 2e67  company = self.g
+00010070: 6574 5f65 6e74 6974 7928 290a 2020 2020  et_entity().    
+00010080: 2020 2020 6669 6c69 6e67 7320 3d20 636f      filings = co
+00010090: 6d70 616e 792e 6765 745f 6669 6c69 6e67  mpany.get_filing
+000100a0: 7328 6163 6365 7373 696f 6e5f 6e75 6d62  s(accession_numb
+000100b0: 6572 3d73 656c 662e 6163 6365 7373 696f  er=self.accessio
+000100c0: 6e5f 6e6f 290a 2020 2020 2020 2020 6966  n_no).        if
+000100d0: 206e 6f74 2066 696c 696e 6773 2e65 6d70   not filings.emp
+000100e0: 7479 3a0a 2020 2020 2020 2020 2020 2020  ty:.            
+000100f0: 6669 6c65 5f6e 756d 6265 7220 3d20 6669  file_number = fi
+00010100: 6c69 6e67 735b 305d 2e66 696c 655f 6e75  lings[0].file_nu
+00010110: 6d62 6572 0a20 2020 2020 2020 2020 2020  mber.           
+00010120: 2072 6574 7572 6e20 636f 6d70 616e 792e   return company.
+00010130: 6765 745f 6669 6c69 6e67 7328 6669 6c65  get_filings(file
+00010140: 5f6e 756d 6265 723d 6669 6c65 5f6e 756d  _number=file_num
+00010150: 6265 722c 0a20 2020 2020 2020 2020 2020  ber,.           
 00010160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010170: 2020 2020 2020 2073 6f72 745f 6279 3d5b         sort_by=[
-00010180: 2822 6669 6c69 6e67 5f64 6174 6522 2c20  ("filing_date", 
-00010190: 2261 7363 656e 6469 6e67 2229 2c20 2822  "ascending"), ("
-000101a0: 6163 6365 7373 696f 6e5f 6e75 6d62 6572  accession_number
-000101b0: 222c 2022 6173 6365 6e64 696e 6722 295d  ", "ascending")]
-000101c0: 290a 0a20 2020 2064 6566 205f 5f68 6173  )..    def __has
-000101d0: 685f 5f28 7365 6c66 293a 0a20 2020 2020  h__(self):.     
-000101e0: 2020 2072 6574 7572 6e20 6861 7368 2873     return hash(s
-000101f0: 656c 662e 6163 6365 7373 696f 6e5f 6e6f  elf.accession_no
-00010200: 290a 0a20 2020 2064 6566 205f 5f65 715f  )..    def __eq_
-00010210: 5f28 7365 6c66 2c20 6f74 6865 7229 3a0a  _(self, other):.
-00010220: 2020 2020 2020 2020 7265 7475 726e 2069          return i
-00010230: 7369 6e73 7461 6e63 6528 6f74 6865 722c  sinstance(other,
-00010240: 2046 696c 696e 6729 2061 6e64 2073 656c   Filing) and sel
-00010250: 662e 6163 6365 7373 696f 6e5f 6e6f 203d  f.accession_no =
-00010260: 3d20 6f74 6865 722e 6163 6365 7373 696f  = other.accessio
-00010270: 6e5f 6e6f 0a0a 2020 2020 6465 6620 5f5f  n_no..    def __
-00010280: 6e65 5f5f 2873 656c 662c 206f 7468 6572  ne__(self, other
-00010290: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-000102a0: 6e20 6e6f 7420 7365 6c66 203d 3d20 6f74  n not self == ot
-000102b0: 6865 720a 0a20 2020 2064 6566 2073 756d  her..    def sum
-000102c0: 6d61 7279 2873 656c 6629 202d 3e20 7064  mary(self) -> pd
-000102d0: 2e44 6174 6146 7261 6d65 3a0a 2020 2020  .DataFrame:.    
-000102e0: 2020 2020 2222 2252 6574 7572 6e20 6120      """Return a 
-000102f0: 7375 6d6d 6172 7920 6f66 2074 6869 7320  summary of this 
-00010300: 6669 6c69 6e67 2061 7320 6120 6461 7461  filing as a data
-00010310: 6672 616d 6522 2222 0a20 2020 2020 2020  frame""".       
-00010320: 2072 6574 7572 6e20 7064 2e44 6174 6146   return pd.DataF
-00010330: 7261 6d65 285b 7b22 4163 6365 7373 696f  rame([{"Accessio
-00010340: 6e20 4e75 6d62 6572 223a 2073 656c 662e  n Number": self.
-00010350: 6163 6365 7373 696f 6e5f 6e6f 2c0a 2020  accession_no,.  
-00010360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010370: 2020 2020 2020 2020 2020 2020 2246 696c              "Fil
-00010380: 696e 6720 4461 7465 223a 2073 656c 662e  ing Date": self.
-00010390: 6669 6c69 6e67 5f64 6174 652c 0a20 2020  filing_date,.   
-000103a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103b0: 2020 2020 2020 2020 2020 2022 436f 6d70             "Comp
-000103c0: 616e 7922 3a20 7365 6c66 2e63 6f6d 7061  any": self.compa
-000103d0: 6e79 2c0a 2020 2020 2020 2020 2020 2020  ny,.            
+00010170: 2020 2020 2020 2020 2020 2020 736f 7274              sort
+00010180: 5f62 793d 5b28 2266 696c 696e 675f 6461  _by=[("filing_da
+00010190: 7465 222c 2022 6173 6365 6e64 696e 6722  te", "ascending"
+000101a0: 292c 2028 2261 6363 6573 7369 6f6e 5f6e  ), ("accession_n
+000101b0: 756d 6265 7222 2c20 2261 7363 656e 6469  umber", "ascendi
+000101c0: 6e67 2229 5d29 0a0a 2020 2020 6465 6620  ng")])..    def 
+000101d0: 5f5f 6861 7368 5f5f 2873 656c 6629 3a0a  __hash__(self):.
+000101e0: 2020 2020 2020 2020 7265 7475 726e 2068          return h
+000101f0: 6173 6828 7365 6c66 2e61 6363 6573 7369  ash(self.accessi
+00010200: 6f6e 5f6e 6f29 0a0a 2020 2020 6465 6620  on_no)..    def 
+00010210: 5f5f 6571 5f5f 2873 656c 662c 206f 7468  __eq__(self, oth
+00010220: 6572 293a 0a20 2020 2020 2020 2072 6574  er):.        ret
+00010230: 7572 6e20 6973 696e 7374 616e 6365 286f  urn isinstance(o
+00010240: 7468 6572 2c20 4669 6c69 6e67 2920 616e  ther, Filing) an
+00010250: 6420 7365 6c66 2e61 6363 6573 7369 6f6e  d self.accession
+00010260: 5f6e 6f20 3d3d 206f 7468 6572 2e61 6363  _no == other.acc
+00010270: 6573 7369 6f6e 5f6e 6f0a 0a20 2020 2064  ession_no..    d
+00010280: 6566 205f 5f6e 655f 5f28 7365 6c66 2c20  ef __ne__(self, 
+00010290: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
+000102a0: 7265 7475 726e 206e 6f74 2073 656c 6620  return not self 
+000102b0: 3d3d 206f 7468 6572 0a0a 2020 2020 6465  == other..    de
+000102c0: 6620 7375 6d6d 6172 7928 7365 6c66 2920  f summary(self) 
+000102d0: 2d3e 2070 642e 4461 7461 4672 616d 653a  -> pd.DataFrame:
+000102e0: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+000102f0: 726e 2061 2073 756d 6d61 7279 206f 6620  rn a summary of 
+00010300: 7468 6973 2066 696c 696e 6720 6173 2061  this filing as a
+00010310: 2064 6174 6166 7261 6d65 2222 220a 2020   dataframe""".  
+00010320: 2020 2020 2020 7265 7475 726e 2070 642e        return pd.
+00010330: 4461 7461 4672 616d 6528 5b7b 2241 6363  DataFrame([{"Acc
+00010340: 6573 7369 6f6e 204e 756d 6265 7222 3a20  ession Number": 
+00010350: 7365 6c66 2e61 6363 6573 7369 6f6e 5f6e  self.accession_n
+00010360: 6f2c 0a20 2020 2020 2020 2020 2020 2020  o,.             
+00010370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010380: 2022 4669 6c69 6e67 2044 6174 6522 3a20   "Filing Date": 
+00010390: 7365 6c66 2e66 696c 696e 675f 6461 7465  self.filing_date
+000103a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000103b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103c0: 2243 6f6d 7061 6e79 223a 2073 656c 662e  "Company": self.
+000103d0: 636f 6d70 616e 792c 0a20 2020 2020 2020  company,.       
 000103e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103f0: 2020 2243 494b 223a 2073 656c 662e 6369    "CIK": self.ci
-00010400: 6b7d 5d29 2e73 6574 5f69 6e64 6578 2822  k}]).set_index("
-00010410: 4163 6365 7373 696f 6e20 4e75 6d62 6572  Accession Number
-00010420: 2229 0a0a 2020 2020 6465 6620 5f5f 7374  ")..    def __st
-00010430: 725f 5f28 7365 6c66 293a 0a20 2020 2020  r__(self):.     
-00010440: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-00010450: 6574 7572 6e20 6120 7374 7269 6e67 2076  eturn a string v
-00010460: 6572 7369 6f6e 206f 6620 7468 6973 2066  ersion of this f
-00010470: 696c 696e 6720 652e 672e 0a0a 2020 2020  iling e.g...    
-00010480: 2020 2020 4669 6c69 6e67 2866 6f72 6d3d      Filing(form=
-00010490: 2731 302d 4b27 2c20 6669 6c69 6e67 5f64  '10-K', filing_d
-000104a0: 6174 653d 2732 3031 382d 3033 2d30 3827  ate='2018-03-08'
-000104b0: 2c20 636f 6d70 616e 793d 2743 4152 424f  , company='CARBO
-000104c0: 2043 4552 414d 4943 5320 494e 4327 2c0a   CERAMICS INC',.
-000104d0: 2020 2020 2020 2020 2020 2020 2020 6369                ci
-000104e0: 6b3d 3130 3039 3637 322c 2061 6363 6573  k=1009672, acces
-000104f0: 7369 6f6e 5f6e 6f3d 2730 3030 3135 3634  sion_no='0001564
-00010500: 3539 302d 3138 2d30 3034 3737 3127 290a  590-18-004771').
-00010510: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00010520: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00010530: 2020 2020 2072 6574 7572 6e20 2866 2246       return (f"F
-00010540: 696c 696e 6728 666f 726d 3d27 7b73 656c  iling(form='{sel
-00010550: 662e 666f 726d 7d27 2c20 6669 6c69 6e67  f.form}', filing
-00010560: 5f64 6174 653d 277b 7365 6c66 2e66 696c  _date='{self.fil
-00010570: 696e 675f 6461 7465 7d27 2c20 636f 6d70  ing_date}', comp
-00010580: 616e 793d 277b 7365 6c66 2e63 6f6d 7061  any='{self.compa
-00010590: 6e79 7d27 2c20 220a 2020 2020 2020 2020  ny}', ".        
-000105a0: 2020 2020 2020 2020 6622 6369 6b3d 7b73          f"cik={s
-000105b0: 656c 662e 6369 6b7d 2c20 6163 6365 7373  elf.cik}, access
-000105c0: 696f 6e5f 6e6f 3d27 7b73 656c 662e 6163  ion_no='{self.ac
-000105d0: 6365 7373 696f 6e5f 6e6f 7d27 2922 290a  cession_no}')").
-000105e0: 0a20 2020 2064 6566 205f 5f72 6963 685f  .    def __rich_
-000105f0: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
-00010600: 2022 2222 0a20 2020 2020 2020 2050 726f   """.        Pro
-00010610: 6475 6365 2061 2074 6162 6c65 2076 6572  duce a table ver
-00010620: 7369 6f6e 206f 6620 7468 6973 2066 696c  sion of this fil
-00010630: 696e 6720 652e 672e 0a20 2020 2020 2020  ing e.g..       
-00010640: 20e2 948c e294 80e2 9480 e294 80e2 9480   ...............
-00010650: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00010660: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00010670: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00010680: e294 80e2 9480 e294 ace2 9480 e294 80e2  ................
-00010690: 9480 e294 80e2 9480 e294 80e2 94ac e294  ................
-000106a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000106b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000106c0: 9480 e294 ace2 9480 e294 80e2 9480 e294  ................
-000106d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000106e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000106f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00010700: 80e2 94ac e294 80e2 9480 e294 80e2 9480  ................
-00010710: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00010720: 9490 0a20 2020 2020 2020 20e2 9482 2020  ...        ...  
-00010730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010740: 2020 2020 e294 8220 666f 726d 20e2 9482      ... form ...
-00010750: 2066 696c 696e 675f 6461 7465 e294 8220   filing_date... 
-00010760: 636f 6d70 616e 7920 2020 2020 2020 2020  company         
-00010770: 2020 20e2 9482 2063 696b 2020 2020 20e2     ... cik     .
-00010780: 9482 0a20 2020 2020 2020 20e2 949c e294  ...        .....
-00010790: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000107a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000107b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000107c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000107d0: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
-000107e0: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
-000107f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00010800: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
-00010810: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00010820: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00010830: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00010840: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
-00010850: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00010860: e294 80e2 9480 e294 80e2 94a4 0a20 2020  .............   
-00010870: 2020 2020 20e2 9482 2030 3030 3135 3634       ... 0001564
-00010880: 3539 302d 3138 2d30 3034 3737 3120 e294  590-18-004771 ..
-00010890: 8220 3130 2d4b 20e2 9482 2032 3031 382d  . 10-K ... 2018-
-000108a0: 3033 2d30 3820 e294 8220 4341 5242 4f20  03-08 ... CARBO 
-000108b0: 4345 5241 4d49 4353 2049 4e43 20e2 9482  CERAMICS INC ...
-000108c0: 2031 3030 3936 3732 20e2 9482 0a20 2020   1009672 ....   
-000108d0: 2020 2020 20e2 9494 e294 80e2 9480 e294       ...........
-000108e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000108f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00010900: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00010910: 80e2 9480 e294 80e2 9480 e294 b4e2 9480  ................
-00010920: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00010930: 94b4 e294 80e2 9480 e294 80e2 9480 e294  ................
-00010940: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00010950: e294 80e2 9480 e294 b4e2 9480 e294 80e2  ................
-00010960: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00010970: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00010980: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00010990: 9480 e294 80e2 94b4 e294 80e2 9480 e294  ................
-000109a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000109b0: e294 80e2 9498 0a20 2020 2020 2020 203a  .......        :
-000109c0: 7265 7475 726e 3a20 6120 7269 6368 2074  return: a rich t
-000109d0: 6162 6c65 2076 6572 7369 6f6e 206f 6620  able version of 
-000109e0: 7468 6973 2066 696c 696e 670a 2020 2020  this filing.    
-000109f0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00010a00: 7375 6d6d 6172 795f 7461 626c 6520 3d20  summary_table = 
-00010a10: 5461 626c 6528 626f 783d 626f 782e 5349  Table(box=box.SI
-00010a20: 4d50 4c45 290a 2020 2020 2020 2020 7375  MPLE).        su
-00010a30: 6d6d 6172 795f 7461 626c 652e 6164 645f  mmary_table.add_
-00010a40: 636f 6c75 6d6e 2822 4163 6365 7373 696f  column("Accessio
-00010a50: 6e20 4e75 6d62 6572 222c 2073 7479 6c65  n Number", style
-00010a60: 3d22 626f 6c64 222c 2068 6561 6465 725f  ="bold", header_
-00010a70: 7374 796c 653d 2262 6f6c 6422 290a 2020  style="bold").  
-00010a80: 2020 2020 2020 7375 6d6d 6172 795f 7461        summary_ta
-00010a90: 626c 652e 6164 645f 636f 6c75 6d6e 2822  ble.add_column("
-00010aa0: 4669 6c69 6e67 2044 6174 6522 290a 2020  Filing Date").  
-00010ab0: 2020 2020 2020 7375 6d6d 6172 795f 7461        summary_ta
-00010ac0: 626c 652e 6164 645f 636f 6c75 6d6e 2822  ble.add_column("
-00010ad0: 436f 6d70 616e 7922 290a 2020 2020 2020  Company").      
-00010ae0: 2020 7375 6d6d 6172 795f 7461 626c 652e    summary_table.
-00010af0: 6164 645f 636f 6c75 6d6e 2822 4349 4b22  add_column("CIK"
-00010b00: 290a 2020 2020 2020 2020 7375 6d6d 6172  ).        summar
-00010b10: 795f 7461 626c 652e 6164 645f 726f 7728  y_table.add_row(
-00010b20: 7365 6c66 2e61 6363 6573 7369 6f6e 5f6e  self.accession_n
-00010b30: 6f2c 2073 7472 2873 656c 662e 6669 6c69  o, str(self.fili
-00010b40: 6e67 5f64 6174 6529 2c20 7365 6c66 2e63  ng_date), self.c
-00010b50: 6f6d 7061 6e79 2c20 7374 7228 7365 6c66  ompany, str(self
-00010b60: 2e63 696b 2929 0a0a 2020 2020 2020 2020  .cik))..        
-00010b70: 686f 6d65 7061 6765 5f75 726c 203d 2054  homepage_url = T
-00010b80: 6578 7428 6622 5c55 3030 3031 4633 4530  ext(f"\U0001F3E0
-00010b90: 207b 7365 6c66 2e68 6f6d 6570 6167 655f   {self.homepage_
-00010ba0: 7572 6c2e 7265 706c 6163 6528 272f 2f77  url.replace('//w
-00010bb0: 7777 2e27 2c20 272f 2f27 297d 2229 0a20  ww.', '//')}"). 
-00010bc0: 2020 2020 2020 2070 7269 6d61 7279 5f64         primary_d
-00010bd0: 6f63 5f75 726c 203d 2054 6578 7428 6622  oc_url = Text(f"
-00010be0: 5c55 3030 3031 4634 4334 207b 7365 6c66  \U0001F4C4 {self
-00010bf0: 2e64 6f63 756d 656e 742e 7572 6c2e 7265  .document.url.re
-00010c00: 706c 6163 6528 272f 2f77 7777 2e27 2c20  place('//www.', 
-00010c10: 272f 2f27 297d 2229 0a20 2020 2020 2020  '//')}").       
-00010c20: 2073 7562 6d69 7373 696f 6e5f 7465 7874   submission_text
-00010c30: 5f75 726c 203d 2054 6578 7428 6622 5c55  _url = Text(f"\U
-00010c40: 3030 3031 4634 4443 207b 7365 6c66 2e74  0001F4DC {self.t
-00010c50: 6578 745f 7572 6c2e 7265 706c 6163 6528  ext_url.replace(
-00010c60: 272f 2f77 7777 2e27 2c20 272f 2f27 297d  '//www.', '//')}
-00010c70: 2229 0a0a 2020 2020 2020 2020 6c69 6e6b  ")..        link
-00010c80: 735f 7461 626c 6520 3d20 5461 626c 6528  s_table = Table(
-00010c90: 0a20 2020 2020 2020 2020 2020 2022 5b62  .            "[b
-00010ca0: 5d4c 696e 6b73 5b2f 625d 3a20 5c55 3030  ]Links[/b]: \U00
-00010cb0: 3031 4633 4530 2048 6f6d 6570 6167 6520  01F3E0 Homepage 
-00010cc0: 5c55 3030 3031 4634 4334 2050 7269 6d61  \U0001F4C4 Prima
-00010cd0: 7279 2044 6f63 756d 656e 7420 5c55 3030  ry Document \U00
-00010ce0: 3031 4634 4443 2046 756c 6c20 5375 626d  01F4DC Full Subm
-00010cf0: 6973 7369 6f6e 2054 6578 7422 2c0a 2020  ission Text",.  
-00010d00: 2020 2020 2020 2020 2020 626f 783d 626f            box=bo
-00010d10: 782e 5349 4d50 4c45 290a 2020 2020 2020  x.SIMPLE).      
-00010d20: 2020 6c69 6e6b 735f 7461 626c 652e 6164    links_table.ad
-00010d30: 645f 726f 7728 686f 6d65 7061 6765 5f75  d_row(homepage_u
-00010d40: 726c 290a 2020 2020 2020 2020 6c69 6e6b  rl).        link
-00010d50: 735f 7461 626c 652e 6164 645f 726f 7728  s_table.add_row(
-00010d60: 7072 696d 6172 795f 646f 635f 7572 6c29  primary_doc_url)
-00010d70: 0a20 2020 2020 2020 206c 696e 6b73 5f74  .        links_t
-00010d80: 6162 6c65 2e61 6464 5f72 6f77 2873 7562  able.add_row(sub
-00010d90: 6d69 7373 696f 6e5f 7465 7874 5f75 726c  mission_text_url
-00010da0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00010db0: 6e20 5061 6e65 6c28 0a20 2020 2020 2020  n Panel(.       
-00010dc0: 2020 2020 2047 726f 7570 2873 756d 6d61       Group(summa
-00010dd0: 7279 5f74 6162 6c65 2c20 6c69 6e6b 735f  ry_table, links_
-00010de0: 7461 626c 6529 2c0a 2020 2020 2020 2020  table),.        
-00010df0: 2020 2020 7469 746c 653d 6622 7b73 656c      title=f"{sel
-00010e00: 662e 666f 726d 7d20 7b75 6e69 636f 6465  f.form} {unicode
-00010e10: 5f66 6f72 5f66 6f72 6d28 7365 6c66 2e66  _for_form(self.f
-00010e20: 6f72 6d29 7d20 6669 6c69 6e67 2066 6f72  orm)} filing for
-00010e30: 207b 7365 6c66 2e63 6f6d 7061 6e79 7d22   {self.company}"
-00010e40: 2c0a 2020 2020 2020 2020 2020 2020 626f  ,.            bo
-00010e50: 783d 626f 782e 524f 554e 4445 440a 2020  x=box.ROUNDED.  
-00010e60: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
-00010e70: 205f 5f72 6570 725f 5f28 7365 6c66 293a   __repr__(self):
-00010e80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00010e90: 7265 7072 5f72 6963 6828 7365 6c66 2e5f  repr_rich(self._
-00010ea0: 5f72 6963 685f 5f28 2929 0a0a 0a63 6c61  _rich__())...cla
-00010eb0: 7373 2041 7474 6163 686d 656e 7473 3a0a  ss Attachments:.
-00010ec0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00010ed0: 5f28 7365 6c66 2c20 6669 6c65 733a 2070  _(self, files: p
-00010ee0: 642e 4461 7461 4672 616d 6529 3a0a 2020  d.DataFrame):.  
-00010ef0: 2020 2020 2020 7365 6c66 2e66 696c 6573        self.files
-00010f00: 203d 2066 696c 6573 0a20 2020 2020 2020   = files.       
-00010f10: 2023 2052 6570 6c61 6365 205c 7861 3020   # Replace \xa0 
-00010f20: 7769 7468 2027 2d27 2069 6e20 7468 6520  with '-' in the 
-00010f30: 5365 710a 2020 2020 2020 2020 7365 6c66  Seq.        self
-00010f40: 2e66 696c 6573 5b27 5365 7127 5d20 3d20  .files['Seq'] = 
-00010f50: 7365 6c66 2e66 696c 6573 5b27 5365 7127  self.files['Seq'
-00010f60: 5d2e 7374 722e 7265 706c 6163 6528 275c  ].str.replace('\
-00010f70: 7861 3027 2c20 272d 2729 0a0a 2020 2020  xa0', '-')..    
-00010f80: 6465 6620 5f5f 6765 7469 7465 6d5f 5f28  def __getitem__(
-00010f90: 7365 6c66 2c20 6974 656d 293a 0a20 2020  self, item):.   
-00010fa0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00010fb0: 6365 2869 7465 6d2c 2073 7472 293a 0a20  ce(item, str):. 
-00010fc0: 2020 2020 2020 2020 2020 2072 6573 203d             res =
-00010fd0: 2073 656c 662e 6669 6c65 735b 7365 6c66   self.files[self
-00010fe0: 2e66 696c 6573 5b27 446f 6375 6d65 6e74  .files['Document
-00010ff0: 275d 203d 3d20 6974 656d 5d0a 2020 2020  '] == item].    
-00011000: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
-00011010: 6573 2e65 6d70 7479 3a0a 2020 2020 2020  es.empty:.      
-00011020: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00011030: 2041 7474 6163 686d 656e 742e 6672 6f6d   Attachment.from
-00011040: 5f64 6174 6166 7261 6d65 5f72 6f77 2872  _dataframe_row(r
-00011050: 6573 2e69 6c6f 635b 305d 290a 2020 2020  es.iloc[0]).    
-00011060: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
-00011070: 6e63 6528 6974 656d 2c20 696e 7429 3a0a  nce(item, int):.
-00011080: 2020 2020 2020 2020 2020 2020 6966 2030              if 0
-00011090: 203c 3d20 6974 656d 203c 206c 656e 2873   <= item < len(s
-000110a0: 656c 662e 6669 6c65 7329 3a0a 2020 2020  elf.files):.    
-000110b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000110c0: 726e 2041 7474 6163 686d 656e 742e 6672  rn Attachment.fr
-000110d0: 6f6d 5f64 6174 6166 7261 6d65 5f72 6f77  om_dataframe_row
-000110e0: 2873 656c 662e 6669 6c65 732e 696c 6f63  (self.files.iloc
-000110f0: 5b69 7465 6d5d 290a 0a20 2020 2064 6566  [item])..    def
-00011100: 2067 6574 2873 656c 662c 2069 7465 6d29   get(self, item)
-00011110: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00011120: 2073 656c 662e 5f5f 6765 7469 7465 6d5f   self.__getitem_
-00011130: 5f28 6974 656d 290a 0a20 2020 2064 6566  _(item)..    def
-00011140: 205f 5f6c 656e 5f5f 2873 656c 6629 3a0a   __len__(self):.
-00011150: 2020 2020 2020 2020 7265 7475 726e 206c          return l
-00011160: 656e 2873 656c 662e 6669 6c65 7329 0a0a  en(self.files)..
-00011170: 2020 2020 6465 6620 5f5f 7269 6368 5f5f      def __rich__
-00011180: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00011190: 7265 7475 726e 2064 665f 746f 5f72 6963  return df_to_ric
-000111a0: 685f 7461 626c 6528 7365 6c66 2e66 696c  h_table(self.fil
-000111b0: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
+000103f0: 2020 2020 2020 2022 4349 4b22 3a20 7365         "CIK": se
+00010400: 6c66 2e63 696b 7d5d 292e 7365 745f 696e  lf.cik}]).set_in
+00010410: 6465 7828 2241 6363 6573 7369 6f6e 204e  dex("Accession N
+00010420: 756d 6265 7222 290a 0a20 2020 2064 6566  umber")..    def
+00010430: 205f 5f73 7472 5f5f 2873 656c 6629 3a0a   __str__(self):.
+00010440: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00010450: 2020 2020 5265 7475 726e 2061 2073 7472      Return a str
+00010460: 696e 6720 7665 7273 696f 6e20 6f66 2074  ing version of t
+00010470: 6869 7320 6669 6c69 6e67 2065 2e67 2e0a  his filing e.g..
+00010480: 0a20 2020 2020 2020 2046 696c 696e 6728  .        Filing(
+00010490: 666f 726d 3d27 3130 2d4b 272c 2066 696c  form='10-K', fil
+000104a0: 696e 675f 6461 7465 3d27 3230 3138 2d30  ing_date='2018-0
+000104b0: 332d 3038 272c 2063 6f6d 7061 6e79 3d27  3-08', company='
+000104c0: 4341 5242 4f20 4345 5241 4d49 4353 2049  CARBO CERAMICS I
+000104d0: 4e43 272c 0a20 2020 2020 2020 2020 2020  NC',.           
+000104e0: 2020 2063 696b 3d31 3030 3936 3732 2c20     cik=1009672, 
+000104f0: 6163 6365 7373 696f 6e5f 6e6f 3d27 3030  accession_no='00
+00010500: 3031 3536 3435 3930 2d31 382d 3030 3437  01564590-18-0047
+00010510: 3731 2729 0a20 2020 2020 2020 203a 7265  71').        :re
+00010520: 7475 726e 3a0a 2020 2020 2020 2020 2222  turn:.        ""
+00010530: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+00010540: 2028 6622 4669 6c69 6e67 2866 6f72 6d3d   (f"Filing(form=
+00010550: 277b 7365 6c66 2e66 6f72 6d7d 272c 2066  '{self.form}', f
+00010560: 696c 696e 675f 6461 7465 3d27 7b73 656c  iling_date='{sel
+00010570: 662e 6669 6c69 6e67 5f64 6174 657d 272c  f.filing_date}',
+00010580: 2063 6f6d 7061 6e79 3d27 7b73 656c 662e   company='{self.
+00010590: 636f 6d70 616e 797d 272c 2022 0a20 2020  company}', ".   
+000105a0: 2020 2020 2020 2020 2020 2020 2066 2263               f"c
+000105b0: 696b 3d7b 7365 6c66 2e63 696b 7d2c 2061  ik={self.cik}, a
+000105c0: 6363 6573 7369 6f6e 5f6e 6f3d 277b 7365  ccession_no='{se
+000105d0: 6c66 2e61 6363 6573 7369 6f6e 5f6e 6f7d  lf.accession_no}
+000105e0: 2729 2229 0a0a 2020 2020 6465 6620 5f5f  ')")..    def __
+000105f0: 7269 6368 5f5f 2873 656c 6629 3a0a 2020  rich__(self):.  
+00010600: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00010610: 2020 5072 6f64 7563 6520 6120 7461 626c    Produce a tabl
+00010620: 6520 7665 7273 696f 6e20 6f66 2074 6869  e version of thi
+00010630: 7320 6669 6c69 6e67 2065 2e67 2e0a 2020  s filing e.g..  
+00010640: 2020 2020 2020 e294 8ce2 9480 e294 80e2        ..........
+00010650: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00010660: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00010670: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00010680: 9480 e294 80e2 9480 e294 80e2 94ac e294  ................
+00010690: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000106a0: e294 ace2 9480 e294 80e2 9480 e294 80e2  ................
+000106b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000106c0: 80e2 9480 e294 80e2 94ac e294 80e2 9480  ................
+000106d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000106e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000106f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00010700: e294 80e2 9480 e294 ace2 9480 e294 80e2  ................
+00010710: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00010720: 80e2 9480 e294 900a 2020 2020 2020 2020  ........        
+00010730: e294 8220 2020 2020 2020 2020 2020 2020  ...             
+00010740: 2020 2020 2020 2020 20e2 9482 2066 6f72           ... for
+00010750: 6d20 e294 8220 6669 6c69 6e67 5f64 6174  m ... filing_dat
+00010760: 65e2 9482 2063 6f6d 7061 6e79 2020 2020  e... company    
+00010770: 2020 2020 2020 2020 e294 8220 6369 6b20          ... cik 
+00010780: 2020 2020 e294 820a 2020 2020 2020 2020      ....        
+00010790: e294 9ce2 9480 e294 80e2 9480 e294 80e2  ................
+000107a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000107b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000107c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000107d0: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
+000107e0: 80e2 9480 e294 80e2 9480 e294 bce2 9480  ................
+000107f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00010800: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00010810: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
+00010820: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00010830: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00010840: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00010850: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
+00010860: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00010870: a40a 2020 2020 2020 2020 e294 8220 3030  ..        ... 00
+00010880: 3031 3536 3435 3930 2d31 382d 3030 3437  01564590-18-0047
+00010890: 3731 20e2 9482 2031 302d 4b20 e294 8220  71 ... 10-K ... 
+000108a0: 3230 3138 2d30 332d 3038 20e2 9482 2043  2018-03-08 ... C
+000108b0: 4152 424f 2043 4552 414d 4943 5320 494e  ARBO CERAMICS IN
+000108c0: 4320 e294 8220 3130 3039 3637 3220 e294  C ... 1009672 ..
+000108d0: 820a 2020 2020 2020 2020 e294 94e2 9480  ..        ......
+000108e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000108f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00010900: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00010910: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00010920: 94b4 e294 80e2 9480 e294 80e2 9480 e294  ................
+00010930: 80e2 9480 e294 b4e2 9480 e294 80e2 9480  ................
+00010940: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00010950: 9480 e294 80e2 9480 e294 80e2 94b4 e294  ................
+00010960: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00010970: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00010980: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00010990: 80e2 9480 e294 80e2 9480 e294 b4e2 9480  ................
+000109a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000109b0: 9480 e294 80e2 9480 e294 980a 2020 2020  ............    
+000109c0: 2020 2020 3a72 6574 7572 6e3a 2061 2072      :return: a r
+000109d0: 6963 6820 7461 626c 6520 7665 7273 696f  ich table versio
+000109e0: 6e20 6f66 2074 6869 7320 6669 6c69 6e67  n of this filing
+000109f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00010a00: 2020 2020 2073 756d 6d61 7279 5f74 6162       summary_tab
+00010a10: 6c65 203d 2054 6162 6c65 2862 6f78 3d62  le = Table(box=b
+00010a20: 6f78 2e53 494d 504c 4529 0a20 2020 2020  ox.SIMPLE).     
+00010a30: 2020 2073 756d 6d61 7279 5f74 6162 6c65     summary_table
+00010a40: 2e61 6464 5f63 6f6c 756d 6e28 2241 6363  .add_column("Acc
+00010a50: 6573 7369 6f6e 204e 756d 6265 7222 2c20  ession Number", 
+00010a60: 7374 796c 653d 2262 6f6c 6422 2c20 6865  style="bold", he
+00010a70: 6164 6572 5f73 7479 6c65 3d22 626f 6c64  ader_style="bold
+00010a80: 2229 0a20 2020 2020 2020 2073 756d 6d61  ").        summa
+00010a90: 7279 5f74 6162 6c65 2e61 6464 5f63 6f6c  ry_table.add_col
+00010aa0: 756d 6e28 2246 696c 696e 6720 4461 7465  umn("Filing Date
+00010ab0: 2229 0a20 2020 2020 2020 2073 756d 6d61  ").        summa
+00010ac0: 7279 5f74 6162 6c65 2e61 6464 5f63 6f6c  ry_table.add_col
+00010ad0: 756d 6e28 2243 6f6d 7061 6e79 2229 0a20  umn("Company"). 
+00010ae0: 2020 2020 2020 2073 756d 6d61 7279 5f74         summary_t
+00010af0: 6162 6c65 2e61 6464 5f63 6f6c 756d 6e28  able.add_column(
+00010b00: 2243 494b 2229 0a20 2020 2020 2020 2073  "CIK").        s
+00010b10: 756d 6d61 7279 5f74 6162 6c65 2e61 6464  ummary_table.add
+00010b20: 5f72 6f77 2873 656c 662e 6163 6365 7373  _row(self.access
+00010b30: 696f 6e5f 6e6f 2c20 7374 7228 7365 6c66  ion_no, str(self
+00010b40: 2e66 696c 696e 675f 6461 7465 292c 2073  .filing_date), s
+00010b50: 656c 662e 636f 6d70 616e 792c 2073 7472  elf.company, str
+00010b60: 2873 656c 662e 6369 6b29 290a 0a20 2020  (self.cik))..   
+00010b70: 2020 2020 2068 6f6d 6570 6167 655f 7572       homepage_ur
+00010b80: 6c20 3d20 5465 7874 2866 225c 5530 3030  l = Text(f"\U000
+00010b90: 3146 3345 3020 7b73 656c 662e 686f 6d65  1F3E0 {self.home
+00010ba0: 7061 6765 5f75 726c 2e72 6570 6c61 6365  page_url.replace
+00010bb0: 2827 2f2f 7777 772e 272c 2027 2f2f 2729  ('//www.', '//')
+00010bc0: 7d22 290a 2020 2020 2020 2020 7072 696d  }").        prim
+00010bd0: 6172 795f 646f 635f 7572 6c20 3d20 5465  ary_doc_url = Te
+00010be0: 7874 2866 225c 5530 3030 3146 3443 3420  xt(f"\U0001F4C4 
+00010bf0: 7b73 656c 662e 646f 6375 6d65 6e74 2e75  {self.document.u
+00010c00: 726c 2e72 6570 6c61 6365 2827 2f2f 7777  rl.replace('//ww
+00010c10: 772e 272c 2027 2f2f 2729 7d22 290a 2020  w.', '//')}").  
+00010c20: 2020 2020 2020 7375 626d 6973 7369 6f6e        submission
+00010c30: 5f74 6578 745f 7572 6c20 3d20 5465 7874  _text_url = Text
+00010c40: 2866 225c 5530 3030 3146 3444 4320 7b73  (f"\U0001F4DC {s
+00010c50: 656c 662e 7465 7874 5f75 726c 2e72 6570  elf.text_url.rep
+00010c60: 6c61 6365 2827 2f2f 7777 772e 272c 2027  lace('//www.', '
+00010c70: 2f2f 2729 7d22 290a 0a20 2020 2020 2020  //')}")..       
+00010c80: 206c 696e 6b73 5f74 6162 6c65 203d 2054   links_table = T
+00010c90: 6162 6c65 280a 2020 2020 2020 2020 2020  able(.          
+00010ca0: 2020 225b 625d 4c69 6e6b 735b 2f62 5d3a    "[b]Links[/b]:
+00010cb0: 205c 5530 3030 3146 3345 3020 486f 6d65   \U0001F3E0 Home
+00010cc0: 7061 6765 205c 5530 3030 3146 3443 3420  page \U0001F4C4 
+00010cd0: 5072 696d 6172 7920 446f 6375 6d65 6e74  Primary Document
+00010ce0: 205c 5530 3030 3146 3444 4320 4675 6c6c   \U0001F4DC Full
+00010cf0: 2053 7562 6d69 7373 696f 6e20 5465 7874   Submission Text
+00010d00: 222c 0a20 2020 2020 2020 2020 2020 2062  ",.            b
+00010d10: 6f78 3d62 6f78 2e53 494d 504c 4529 0a20  ox=box.SIMPLE). 
+00010d20: 2020 2020 2020 206c 696e 6b73 5f74 6162         links_tab
+00010d30: 6c65 2e61 6464 5f72 6f77 2868 6f6d 6570  le.add_row(homep
+00010d40: 6167 655f 7572 6c29 0a20 2020 2020 2020  age_url).       
+00010d50: 206c 696e 6b73 5f74 6162 6c65 2e61 6464   links_table.add
+00010d60: 5f72 6f77 2870 7269 6d61 7279 5f64 6f63  _row(primary_doc
+00010d70: 5f75 726c 290a 2020 2020 2020 2020 6c69  _url).        li
+00010d80: 6e6b 735f 7461 626c 652e 6164 645f 726f  nks_table.add_ro
+00010d90: 7728 7375 626d 6973 7369 6f6e 5f74 6578  w(submission_tex
+00010da0: 745f 7572 6c29 0a0a 2020 2020 2020 2020  t_url)..        
+00010db0: 7265 7475 726e 2050 616e 656c 280a 2020  return Panel(.  
+00010dc0: 2020 2020 2020 2020 2020 4772 6f75 7028            Group(
+00010dd0: 7375 6d6d 6172 795f 7461 626c 652c 206c  summary_table, l
+00010de0: 696e 6b73 5f74 6162 6c65 292c 0a20 2020  inks_table),.   
+00010df0: 2020 2020 2020 2020 2074 6974 6c65 3d66           title=f
+00010e00: 227b 7365 6c66 2e66 6f72 6d7d 207b 756e  "{self.form} {un
+00010e10: 6963 6f64 655f 666f 725f 666f 726d 2873  icode_for_form(s
+00010e20: 656c 662e 666f 726d 297d 2066 696c 696e  elf.form)} filin
+00010e30: 6720 666f 7220 7b73 656c 662e 636f 6d70  g for {self.comp
+00010e40: 616e 797d 222c 0a20 2020 2020 2020 2020  any}",.         
+00010e50: 2020 2062 6f78 3d62 6f78 2e52 4f55 4e44     box=box.ROUND
+00010e60: 4544 0a20 2020 2020 2020 2029 0a0a 2020  ED.        )..  
+00010e70: 2020 6465 6620 5f5f 7265 7072 5f5f 2873    def __repr__(s
+00010e80: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
+00010e90: 7475 726e 2072 6570 725f 7269 6368 2873  turn repr_rich(s
+00010ea0: 656c 662e 5f5f 7269 6368 5f5f 2829 290a  elf.__rich__()).
+00010eb0: 0a0a 636c 6173 7320 4174 7461 6368 6d65  ..class Attachme
+00010ec0: 6e74 733a 0a0a 2020 2020 6465 6620 5f5f  nts:..    def __
+00010ed0: 696e 6974 5f5f 2873 656c 662c 2066 696c  init__(self, fil
+00010ee0: 6573 3a20 7064 2e44 6174 6146 7261 6d65  es: pd.DataFrame
+00010ef0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00010f00: 6669 6c65 7320 3d20 6669 6c65 730a 2020  files = files.  
+00010f10: 2020 2020 2020 2320 5265 706c 6163 6520        # Replace 
+00010f20: 5c78 6130 2077 6974 6820 272d 2720 696e  \xa0 with '-' in
+00010f30: 2074 6865 2053 6571 0a20 2020 2020 2020   the Seq.       
+00010f40: 2073 656c 662e 6669 6c65 735b 2753 6571   self.files['Seq
+00010f50: 275d 203d 2073 656c 662e 6669 6c65 735b  '] = self.files[
+00010f60: 2753 6571 275d 2e73 7472 2e72 6570 6c61  'Seq'].str.repla
+00010f70: 6365 2827 5c78 6130 272c 2027 2d27 290a  ce('\xa0', '-').
+00010f80: 0a20 2020 2064 6566 205f 5f67 6574 6974  .    def __getit
+00010f90: 656d 5f5f 2873 656c 662c 2069 7465 6d29  em__(self, item)
+00010fa0: 3a0a 2020 2020 2020 2020 6966 2069 7369  :.        if isi
+00010fb0: 6e73 7461 6e63 6528 6974 656d 2c20 7374  nstance(item, st
+00010fc0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00010fd0: 7265 7320 3d20 7365 6c66 2e66 696c 6573  res = self.files
+00010fe0: 5b73 656c 662e 6669 6c65 735b 2744 6f63  [self.files['Doc
+00010ff0: 756d 656e 7427 5d20 3d3d 2069 7465 6d5d  ument'] == item]
+00011000: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00011010: 6e6f 7420 7265 732e 656d 7074 793a 0a20  not res.empty:. 
+00011020: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00011030: 6574 7572 6e20 4174 7461 6368 6d65 6e74  eturn Attachment
+00011040: 2e66 726f 6d5f 6461 7461 6672 616d 655f  .from_dataframe_
+00011050: 726f 7728 7265 732e 696c 6f63 5b30 5d29  row(res.iloc[0])
+00011060: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
+00011070: 696e 7374 616e 6365 2869 7465 6d2c 2069  instance(item, i
+00011080: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
+00011090: 2069 6620 3020 3c3d 2069 7465 6d20 3c20   if 0 <= item < 
+000110a0: 6c65 6e28 7365 6c66 2e66 696c 6573 293a  len(self.files):
+000110b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000110c0: 2072 6574 7572 6e20 4174 7461 6368 6d65   return Attachme
+000110d0: 6e74 2e66 726f 6d5f 6461 7461 6672 616d  nt.from_datafram
+000110e0: 655f 726f 7728 7365 6c66 2e66 696c 6573  e_row(self.files
+000110f0: 2e69 6c6f 635b 6974 656d 5d29 0a0a 2020  .iloc[item])..  
+00011100: 2020 6465 6620 6765 7428 7365 6c66 2c20    def get(self, 
+00011110: 6974 656d 293a 0a20 2020 2020 2020 2072  item):.        r
+00011120: 6574 7572 6e20 7365 6c66 2e5f 5f67 6574  eturn self.__get
+00011130: 6974 656d 5f5f 2869 7465 6d29 0a0a 2020  item__(item)..  
+00011140: 2020 6465 6620 5f5f 6c65 6e5f 5f28 7365    def __len__(se
+00011150: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
+00011160: 7572 6e20 6c65 6e28 7365 6c66 2e66 696c  urn len(self.fil
+00011170: 6573 290a 0a20 2020 2064 6566 205f 5f72  es)..    def __r
+00011180: 6963 685f 5f28 7365 6c66 293a 0a20 2020  ich__(self):.   
+00011190: 2020 2020 2072 6574 7572 6e20 6466 5f74       return df_t
+000111a0: 6f5f 7269 6368 5f74 6162 6c65 2873 656c  o_rich_table(sel
+000111b0: 662e 6669 6c65 730a 2020 2020 2020 2020  f.files.        
 000111c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111d0: 2020 202e 6173 7369 676e 2853 697a 653d     .assign(Size=
-000111e0: 6c61 6d62 6461 2064 663a 2064 662e 5369  lambda df: df.Si
-000111f0: 7a65 2e61 7070 6c79 2864 6973 706c 6179  ze.apply(display
-00011200: 5f73 697a 6529 290a 2020 2020 2020 2020  _size)).        
+000111d0: 2020 2020 2020 2020 2e61 7373 6967 6e28          .assign(
+000111e0: 5369 7a65 3d6c 616d 6264 6120 6466 3a20  Size=lambda df: 
+000111f0: 6466 2e53 697a 652e 6170 706c 7928 6469  df.Size.apply(di
+00011200: 7370 6c61 795f 7369 7a65 2929 0a20 2020  splay_size)).   
 00011210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011220: 2020 2020 2020 2020 2e66 696c 7465 7228          .filter(
-00011230: 5b27 4465 7363 7269 7074 696f 6e27 2c20  ['Description', 
-00011240: 2744 6f63 756d 656e 7427 2c20 2754 7970  'Document', 'Typ
-00011250: 6527 2c20 2753 697a 6527 5d29 2c20 6d61  e', 'Size']), ma
-00011260: 785f 726f 7773 3d31 3030 290a 0a20 2020  x_rows=100)..   
-00011270: 2064 6566 205f 5f72 6570 725f 5f28 7365   def __repr__(se
-00011280: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
-00011290: 7572 6e20 7265 7072 5f72 6963 6828 7365  urn repr_rich(se
-000112a0: 6c66 2e5f 5f72 6963 685f 5f28 2929 0a0a  lf.__rich__())..
-000112b0: 0a40 6461 7461 636c 6173 7328 6672 6f7a  .@dataclass(froz
-000112c0: 656e 3d54 7275 6529 0a63 6c61 7373 2041  en=True).class A
-000112d0: 7474 6163 686d 656e 743a 0a20 2020 2022  ttachment:.    "
-000112e0: 2222 0a20 2020 2041 2064 6f63 756d 656e  "".    A documen
-000112f0: 7420 6f6e 2074 6865 2066 696c 696e 670a  t on the filing.
-00011300: 0a20 2020 2022 2222 0a20 2020 2073 6571  .    """.    seq
-00011310: 3a20 696e 740a 2020 2020 6465 7363 7269  : int.    descri
-00011320: 7074 696f 6e3a 2073 7472 0a20 2020 2064  ption: str.    d
-00011330: 6f63 756d 656e 743a 2073 7472 0a20 2020  ocument: str.   
-00011340: 2066 6f72 6d3a 2073 7472 0a20 2020 2073   form: str.    s
-00011350: 697a 653a 2069 6e74 0a20 2020 2070 6174  ize: int.    pat
-00011360: 683a 2073 7472 0a0a 2020 2020 4070 726f  h: str..    @pro
-00011370: 7065 7274 790a 2020 2020 6465 6620 6578  perty.    def ex
-00011380: 7465 6e73 696f 6e28 7365 6c66 293a 0a20  tension(self):. 
-00011390: 2020 2020 2020 2022 2222 5468 6520 6163         """The ac
-000113a0: 7475 616c 2065 7874 656e 7369 6f6e 206f  tual extension o
-000113b0: 6620 7468 6520 6669 6c69 6e67 2064 6f63  f the filing doc
-000113c0: 756d 656e 740a 2020 2020 2020 2020 2055  ument.         U
-000113d0: 7375 616c 6c79 206f 6e65 206f 6620 2e78  sually one of .x
-000113e0: 6d6c 206f 7220 2e68 746d 6c20 6f72 202e  ml or .html or .
-000113f0: 7064 6620 6f72 202e 7478 7420 6f72 202e  pdf or .txt or .
-00011400: 7061 7065 720a 2020 2020 2020 2020 2022  paper.         "
-00011410: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-00011420: 6e20 6f73 2e70 6174 682e 7370 6c69 7465  n os.path.splite
-00011430: 7874 2873 656c 662e 7061 7468 295b 315d  xt(self.path)[1]
-00011440: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-00011450: 2020 2020 6465 6620 6469 7370 6c61 795f      def display_
-00011460: 6578 7465 6e73 696f 6e28 7365 6c66 2920  extension(self) 
-00011470: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
-00011480: 2222 2254 6869 7320 6973 2074 6865 2065  """This is the e
-00011490: 7874 656e 7369 6f6e 2064 6973 706c 6179  xtension display
-000114a0: 6564 2069 6e20 7468 6520 6874 6d6c 2065  ed in the html e
-000114b0: 2e67 2e20 2265 7332 3230 3239 3636 3830  .g. "es220296680
-000114c0: 5f34 2d64 6176 6973 2e68 746d 6c22 0a20  _4-davis.html". 
-000114d0: 2020 2020 2020 2054 6865 2061 6374 7561         The actua
-000114e0: 6c20 6578 7465 6e73 696f 6e20 776f 756c  l extension woul
-000114f0: 6420 6265 2022 6573 3232 3032 3936 3638  d be "es22029668
-00011500: 305f 342d 6461 7669 732e 786d 6c22 2c20  0_4-davis.xml", 
-00011510: 7468 6174 2064 6973 706c 6179 7320 6173  that displays as
-00011520: 2068 746d 6c20 696e 2074 6865 2062 726f   html in the bro
-00011530: 7773 6572 0a0a 2020 2020 2020 2020 2222  wser..        ""
-00011540: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-00011550: 206f 732e 7061 7468 2e73 706c 6974 6578   os.path.splitex
-00011560: 7428 7365 6c66 2e64 6f63 756d 656e 7429  t(self.document)
-00011570: 5b31 5d0a 0a20 2020 2040 7072 6f70 6572  [1]..    @proper
-00011580: 7479 0a20 2020 2064 6566 2075 726c 2873  ty.    def url(s
-00011590: 656c 6629 202d 3e20 7374 723a 0a20 2020  elf) -> str:.   
-000115a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000115b0: 203a 7265 7475 726e 3a20 5468 6520 6675   :return: The fu
-000115c0: 6c6c 2073 6563 2075 726c 0a20 2020 2020  ll sec url.     
-000115d0: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
-000115e0: 204e 6576 6572 2075 7365 2074 6865 2069   Never use the i
-000115f0: 7862 726c 2076 6965 7765 720a 2020 2020  xbrl viewer.    
-00011600: 2020 2020 2320 6978 2e78 6874 6d6c 3f64      # ix.xhtml?d
-00011610: 6f63 3d2f 0a20 2020 2020 2020 2066 696c  oc=/.        fil
-00011620: 696e 675f 7572 6c20 3d20 6622 7b73 6563  ing_url = f"{sec
-00011630: 5f64 6f74 5f67 6f76 7d7b 7365 6c66 2e70  _dot_gov}{self.p
-00011640: 6174 687d 220a 2020 2020 2020 2020 2320  ath}".        # 
-00011650: 5265 6d6f 7665 2022 6978 3f64 6f63 3d2f  Remove "ix?doc=/
-00011660: 2220 6f72 2022 6978 2e78 6874 6d6c 3f64  " or "ix.xhtml?d
-00011670: 6f63 3d2f 2220 6672 6f6d 2074 6865 2066  oc=/" from the f
-00011680: 696c 696e 6720 7572 6c0a 2020 2020 2020  iling url.      
-00011690: 2020 7265 7475 726e 2072 652e 7375 6228    return re.sub(
-000116a0: 7222 6978 285c 2e78 6874 6d6c 293f 5c3f  r"ix(\.xhtml)?\?
-000116b0: 646f 633d 2f22 2c20 2222 2c20 6669 6c69  doc=/", "", fili
-000116c0: 6e67 5f75 726c 290a 0a20 2020 2064 6566  ng_url)..    def
-000116d0: 206f 7065 6e28 7365 6c66 293a 0a20 2020   open(self):.   
-000116e0: 2020 2020 2022 2222 4f70 656e 2074 6865       """Open the
-000116f0: 2066 696c 696e 6720 646f 6375 6d65 6e74   filing document
-00011700: 2222 220a 2020 2020 2020 2020 7765 6262  """.        webb
-00011710: 726f 7773 6572 2e6f 7065 6e28 7365 6c66  rowser.open(self
-00011720: 2e75 726c 290a 0a20 2020 2040 7072 6f70  .url)..    @prop
-00011730: 6572 7479 0a20 2020 2064 6566 206e 616d  erty.    def nam
-00011740: 6528 7365 6c66 2920 2d3e 2073 7472 3a0a  e(self) -> str:.
-00011750: 2020 2020 2020 2020 7265 7475 726e 206f          return o
-00011760: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
-00011770: 7365 6c66 2e70 6174 6829 0a0a 2020 2020  self.path)..    
-00011780: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
-00011790: 2064 6566 2066 726f 6d5f 6461 7461 6672   def from_datafr
-000117a0: 616d 655f 726f 7728 636c 732c 2064 6174  ame_row(cls, dat
-000117b0: 6166 7261 6d65 5f72 6f77 3a20 7064 2e53  aframe_row: pd.S
-000117c0: 6572 6965 7329 3a0a 0a20 2020 2020 2020  eries):..       
-000117d0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-000117e0: 2020 7369 7a65 203d 2069 6e74 2864 6174    size = int(dat
-000117f0: 6166 7261 6d65 5f72 6f77 2e53 697a 6529  aframe_row.Size)
-00011800: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-00011810: 5661 6c75 6545 7272 6f72 3a0a 2020 2020  ValueError:.    
-00011820: 2020 2020 2020 2020 7369 7a65 203d 2030          size = 0
-00011830: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00011840: 636c 7328 7365 713d 6461 7461 6672 616d  cls(seq=datafram
-00011850: 655f 726f 772e 5365 712c 0a20 2020 2020  e_row.Seq,.     
-00011860: 2020 2020 2020 2020 2020 2020 2020 6465                de
-00011870: 7363 7269 7074 696f 6e3d 6461 7461 6672  scription=datafr
-00011880: 616d 655f 726f 772e 4465 7363 7269 7074  ame_row.Descript
-00011890: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-000118a0: 2020 2020 2020 2020 646f 6375 6d65 6e74          document
-000118b0: 3d64 6174 6166 7261 6d65 5f72 6f77 2e44  =dataframe_row.D
-000118c0: 6f63 756d 656e 742c 0a20 2020 2020 2020  ocument,.       
-000118d0: 2020 2020 2020 2020 2020 2020 666f 726d              form
-000118e0: 3d64 6174 6166 7261 6d65 5f72 6f77 2e54  =dataframe_row.T
-000118f0: 7970 652c 0a20 2020 2020 2020 2020 2020  ype,.           
-00011900: 2020 2020 2020 2020 7369 7a65 3d73 697a          size=siz
-00011910: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00011920: 2020 2020 2020 7061 7468 3d64 6174 6166        path=dataf
-00011930: 7261 6d65 5f72 6f77 2e55 726c 290a 0a20  rame_row.Url).. 
-00011940: 2020 2064 6566 2069 735f 7465 7874 2873     def is_text(s
-00011950: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00011960: 2249 7320 7468 6973 2061 2074 6578 7420  "Is this a text 
-00011970: 646f 6375 6d65 6e74 2222 220a 2020 2020  document""".    
-00011980: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00011990: 6578 7465 6e73 696f 6e20 696e 2074 6578  extension in tex
-000119a0: 745f 6578 7465 6e73 696f 6e73 0a0a 2020  t_extensions..  
-000119b0: 2020 6465 6620 6973 5f62 696e 6172 7928    def is_binary(
-000119c0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-000119d0: 2222 4973 2074 6869 7320 6120 6269 6e61  ""Is this a bina
-000119e0: 7279 2064 6f63 756d 656e 7422 2222 0a20  ry document""". 
-000119f0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00011a00: 6c66 2e65 7874 656e 7369 6f6e 2069 6e20  lf.extension in 
-00011a10: 6269 6e61 7279 5f65 7874 656e 7369 6f6e  binary_extension
-00011a20: 730a 0a20 2020 2064 6566 2064 6f77 6e6c  s..    def downl
-00011a30: 6f61 6428 7365 6c66 293a 0a20 2020 2020  oad(self):.     
-00011a40: 2020 2072 6574 7572 6e20 646f 776e 6c6f     return downlo
-00011a50: 6164 5f66 696c 6528 7365 6c66 2e75 726c  ad_file(self.url
-00011a60: 2c20 6173 5f74 6578 743d 7365 6c66 2e69  , as_text=self.i
-00011a70: 735f 7465 7874 2829 290a 0a20 2020 2064  s_text())..    d
-00011a80: 6566 2073 756d 6d61 7279 2873 656c 6629  ef summary(self)
-00011a90: 202d 3e20 7064 2e44 6174 6146 7261 6d65   -> pd.DataFrame
-00011aa0: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
-00011ab0: 7572 6e20 6120 7375 6d6d 6172 7920 6f66  urn a summary of
-00011ac0: 2074 6869 7320 6669 6c69 6e67 2061 7320   this filing as 
-00011ad0: 6120 6461 7461 6672 616d 6522 2222 0a20  a dataframe""". 
-00011ae0: 2020 2020 2020 2072 6574 7572 6e20 7064         return pd
-00011af0: 2e44 6174 6146 7261 6d65 285b 7b27 7365  .DataFrame([{'se
-00011b00: 7127 3a20 7365 6c66 2e73 6571 2c0a 2020  q': self.seq,.  
-00011b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b20: 2020 2020 2020 2020 2020 2020 2766 6f72              'for
-00011b30: 6d27 3a20 7365 6c66 2e66 6f72 6d2c 0a20  m': self.form,. 
-00011b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b50: 2020 2020 2020 2020 2020 2020 2027 646f               'do
-00011b60: 6375 6d65 6e74 273a 2073 656c 662e 646f  cument': self.do
-00011b70: 6375 6d65 6e74 2c0a 2020 2020 2020 2020  cument,.        
+00011220: 2020 2020 2020 2020 2020 2020 202e 6669               .fi
+00011230: 6c74 6572 285b 2744 6573 6372 6970 7469  lter(['Descripti
+00011240: 6f6e 272c 2027 446f 6375 6d65 6e74 272c  on', 'Document',
+00011250: 2027 5479 7065 272c 2027 5369 7a65 275d   'Type', 'Size']
+00011260: 292c 206d 6178 5f72 6f77 733d 3130 3029  ), max_rows=100)
+00011270: 0a0a 2020 2020 6465 6620 5f5f 7265 7072  ..    def __repr
+00011280: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
+00011290: 2020 7265 7475 726e 2072 6570 725f 7269    return repr_ri
+000112a0: 6368 2873 656c 662e 5f5f 7269 6368 5f5f  ch(self.__rich__
+000112b0: 2829 290a 0a0a 4064 6174 6163 6c61 7373  ())...@dataclass
+000112c0: 2866 726f 7a65 6e3d 5472 7565 290a 636c  (frozen=True).cl
+000112d0: 6173 7320 4174 7461 6368 6d65 6e74 3a0a  ass Attachment:.
+000112e0: 2020 2020 2222 220a 2020 2020 4120 646f      """.    A do
+000112f0: 6375 6d65 6e74 206f 6e20 7468 6520 6669  cument on the fi
+00011300: 6c69 6e67 0a0a 2020 2020 2222 220a 2020  ling..    """.  
+00011310: 2020 7365 713a 2069 6e74 0a20 2020 2064    seq: int.    d
+00011320: 6573 6372 6970 7469 6f6e 3a20 7374 720a  escription: str.
+00011330: 2020 2020 646f 6375 6d65 6e74 3a20 7374      document: st
+00011340: 720a 2020 2020 666f 726d 3a20 7374 720a  r.    form: str.
+00011350: 2020 2020 7369 7a65 3a20 696e 740a 2020      size: int.  
+00011360: 2020 7061 7468 3a20 7374 720a 0a20 2020    path: str..   
+00011370: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+00011380: 6566 2065 7874 656e 7369 6f6e 2873 656c  ef extension(sel
+00011390: 6629 3a0a 2020 2020 2020 2020 2222 2254  f):.        """T
+000113a0: 6865 2061 6374 7561 6c20 6578 7465 6e73  he actual extens
+000113b0: 696f 6e20 6f66 2074 6865 2066 696c 696e  ion of the filin
+000113c0: 6720 646f 6375 6d65 6e74 0a20 2020 2020  g document.     
+000113d0: 2020 2020 5573 7561 6c6c 7920 6f6e 6520      Usually one 
+000113e0: 6f66 202e 786d 6c20 6f72 202e 6874 6d6c  of .xml or .html
+000113f0: 206f 7220 2e70 6466 206f 7220 2e74 7874   or .pdf or .txt
+00011400: 206f 7220 2e70 6170 6572 0a20 2020 2020   or .paper.     
+00011410: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00011420: 7265 7475 726e 206f 732e 7061 7468 2e73  return os.path.s
+00011430: 706c 6974 6578 7428 7365 6c66 2e70 6174  plitext(self.pat
+00011440: 6829 5b31 5d0a 0a20 2020 2040 7072 6f70  h)[1]..    @prop
+00011450: 6572 7479 0a20 2020 2064 6566 2064 6973  erty.    def dis
+00011460: 706c 6179 5f65 7874 656e 7369 6f6e 2873  play_extension(s
+00011470: 656c 6629 202d 3e20 7374 723a 0a20 2020  elf) -> str:.   
+00011480: 2020 2020 2022 2222 5468 6973 2069 7320       """This is 
+00011490: 7468 6520 6578 7465 6e73 696f 6e20 6469  the extension di
+000114a0: 7370 6c61 7965 6420 696e 2074 6865 2068  splayed in the h
+000114b0: 746d 6c20 652e 672e 2022 6573 3232 3032  tml e.g. "es2202
+000114c0: 3936 3638 305f 342d 6461 7669 732e 6874  96680_4-davis.ht
+000114d0: 6d6c 220a 2020 2020 2020 2020 5468 6520  ml".        The 
+000114e0: 6163 7475 616c 2065 7874 656e 7369 6f6e  actual extension
+000114f0: 2077 6f75 6c64 2062 6520 2265 7332 3230   would be "es220
+00011500: 3239 3636 3830 5f34 2d64 6176 6973 2e78  296680_4-davis.x
+00011510: 6d6c 222c 2074 6861 7420 6469 7370 6c61  ml", that displa
+00011520: 7973 2061 7320 6874 6d6c 2069 6e20 7468  ys as html in th
+00011530: 6520 6272 6f77 7365 720a 0a20 2020 2020  e browser..     
+00011540: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+00011550: 6574 7572 6e20 6f73 2e70 6174 682e 7370  eturn os.path.sp
+00011560: 6c69 7465 7874 2873 656c 662e 646f 6375  litext(self.docu
+00011570: 6d65 6e74 295b 315d 0a0a 2020 2020 4070  ment)[1]..    @p
+00011580: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00011590: 7572 6c28 7365 6c66 2920 2d3e 2073 7472  url(self) -> str
+000115a0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000115b0: 2020 2020 2020 3a72 6574 7572 6e3a 2054        :return: T
+000115c0: 6865 2066 756c 6c20 7365 6320 7572 6c0a  he full sec url.
+000115d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000115e0: 2020 2020 2320 4e65 7665 7220 7573 6520      # Never use 
+000115f0: 7468 6520 6978 6272 6c20 7669 6577 6572  the ixbrl viewer
+00011600: 0a20 2020 2020 2020 2023 2069 782e 7868  .        # ix.xh
+00011610: 746d 6c3f 646f 633d 2f0a 2020 2020 2020  tml?doc=/.      
+00011620: 2020 6669 6c69 6e67 5f75 726c 203d 2066    filing_url = f
+00011630: 227b 7365 635f 646f 745f 676f 767d 7b73  "{sec_dot_gov}{s
+00011640: 656c 662e 7061 7468 7d22 0a20 2020 2020  elf.path}".     
+00011650: 2020 2023 2052 656d 6f76 6520 2269 783f     # Remove "ix?
+00011660: 646f 633d 2f22 206f 7220 2269 782e 7868  doc=/" or "ix.xh
+00011670: 746d 6c3f 646f 633d 2f22 2066 726f 6d20  tml?doc=/" from 
+00011680: 7468 6520 6669 6c69 6e67 2075 726c 0a20  the filing url. 
+00011690: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000116a0: 2e73 7562 2872 2269 7828 5c2e 7868 746d  .sub(r"ix(\.xhtm
+000116b0: 6c29 3f5c 3f64 6f63 3d2f 222c 2022 222c  l)?\?doc=/", "",
+000116c0: 2066 696c 696e 675f 7572 6c29 0a0a 2020   filing_url)..  
+000116d0: 2020 6465 6620 6f70 656e 2873 656c 6629    def open(self)
+000116e0: 3a0a 2020 2020 2020 2020 2222 224f 7065  :.        """Ope
+000116f0: 6e20 7468 6520 6669 6c69 6e67 2064 6f63  n the filing doc
+00011700: 756d 656e 7422 2222 0a20 2020 2020 2020  ument""".       
+00011710: 2077 6562 6272 6f77 7365 722e 6f70 656e   webbrowser.open
+00011720: 2873 656c 662e 7572 6c29 0a0a 2020 2020  (self.url)..    
+00011730: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00011740: 6620 6e61 6d65 2873 656c 6629 202d 3e20  f name(self) -> 
+00011750: 7374 723a 0a20 2020 2020 2020 2072 6574  str:.        ret
+00011760: 7572 6e20 6f73 2e70 6174 682e 6261 7365  urn os.path.base
+00011770: 6e61 6d65 2873 656c 662e 7061 7468 290a  name(self.path).
+00011780: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
+00011790: 640a 2020 2020 6465 6620 6672 6f6d 5f64  d.    def from_d
+000117a0: 6174 6166 7261 6d65 5f72 6f77 2863 6c73  ataframe_row(cls
+000117b0: 2c20 6461 7461 6672 616d 655f 726f 773a  , dataframe_row:
+000117c0: 2070 642e 5365 7269 6573 293a 0a0a 2020   pd.Series):..  
+000117d0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+000117e0: 2020 2020 2020 2073 697a 6520 3d20 696e         size = in
+000117f0: 7428 6461 7461 6672 616d 655f 726f 772e  t(dataframe_row.
+00011800: 5369 7a65 290a 2020 2020 2020 2020 6578  Size).        ex
+00011810: 6365 7074 2056 616c 7565 4572 726f 723a  cept ValueError:
+00011820: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
+00011830: 6520 3d20 300a 2020 2020 2020 2020 7265  e = 0.        re
+00011840: 7475 726e 2063 6c73 2873 6571 3d64 6174  turn cls(seq=dat
+00011850: 6166 7261 6d65 5f72 6f77 2e53 6571 2c0a  aframe_row.Seq,.
+00011860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011870: 2020 2064 6573 6372 6970 7469 6f6e 3d64     description=d
+00011880: 6174 6166 7261 6d65 5f72 6f77 2e44 6573  ataframe_row.Des
+00011890: 6372 6970 7469 6f6e 2c0a 2020 2020 2020  cription,.      
+000118a0: 2020 2020 2020 2020 2020 2020 2064 6f63               doc
+000118b0: 756d 656e 743d 6461 7461 6672 616d 655f  ument=dataframe_
+000118c0: 726f 772e 446f 6375 6d65 6e74 2c0a 2020  row.Document,.  
+000118d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000118e0: 2066 6f72 6d3d 6461 7461 6672 616d 655f   form=dataframe_
+000118f0: 726f 772e 5479 7065 2c0a 2020 2020 2020  row.Type,.      
+00011900: 2020 2020 2020 2020 2020 2020 2073 697a               siz
+00011910: 653d 7369 7a65 2c0a 2020 2020 2020 2020  e=size,.        
+00011920: 2020 2020 2020 2020 2020 2070 6174 683d             path=
+00011930: 6461 7461 6672 616d 655f 726f 772e 5572  dataframe_row.Ur
+00011940: 6c29 0a0a 2020 2020 6465 6620 6973 5f74  l)..    def is_t
+00011950: 6578 7428 7365 6c66 293a 0a20 2020 2020  ext(self):.     
+00011960: 2020 2022 2222 4973 2074 6869 7320 6120     """Is this a 
+00011970: 7465 7874 2064 6f63 756d 656e 7422 2222  text document"""
+00011980: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00011990: 7365 6c66 2e65 7874 656e 7369 6f6e 2069  self.extension i
+000119a0: 6e20 7465 7874 5f65 7874 656e 7369 6f6e  n text_extension
+000119b0: 730a 0a20 2020 2064 6566 2069 735f 6269  s..    def is_bi
+000119c0: 6e61 7279 2873 656c 6629 3a0a 2020 2020  nary(self):.    
+000119d0: 2020 2020 2222 2249 7320 7468 6973 2061      """Is this a
+000119e0: 2062 696e 6172 7920 646f 6375 6d65 6e74   binary document
+000119f0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+00011a00: 726e 2073 656c 662e 6578 7465 6e73 696f  rn self.extensio
+00011a10: 6e20 696e 2062 696e 6172 795f 6578 7465  n in binary_exte
+00011a20: 6e73 696f 6e73 0a0a 2020 2020 6465 6620  nsions..    def 
+00011a30: 646f 776e 6c6f 6164 2873 656c 6629 3a0a  download(self):.
+00011a40: 2020 2020 2020 2020 7265 7475 726e 2064          return d
+00011a50: 6f77 6e6c 6f61 645f 6669 6c65 2873 656c  ownload_file(sel
+00011a60: 662e 7572 6c2c 2061 735f 7465 7874 3d73  f.url, as_text=s
+00011a70: 656c 662e 6973 5f74 6578 7428 2929 0a0a  elf.is_text())..
+00011a80: 2020 2020 6465 6620 7375 6d6d 6172 7928      def summary(
+00011a90: 7365 6c66 2920 2d3e 2070 642e 4461 7461  self) -> pd.Data
+00011aa0: 4672 616d 653a 0a20 2020 2020 2020 2022  Frame:.        "
+00011ab0: 2222 5265 7475 726e 2061 2073 756d 6d61  ""Return a summa
+00011ac0: 7279 206f 6620 7468 6973 2066 696c 696e  ry of this filin
+00011ad0: 6720 6173 2061 2064 6174 6166 7261 6d65  g as a dataframe
+00011ae0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+00011af0: 726e 2070 642e 4461 7461 4672 616d 6528  rn pd.DataFrame(
+00011b00: 5b7b 2773 6571 273a 2073 656c 662e 7365  [{'seq': self.se
+00011b10: 712c 0a20 2020 2020 2020 2020 2020 2020  q,.             
+00011b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b30: 2027 666f 726d 273a 2073 656c 662e 666f   'form': self.fo
+00011b40: 726d 2c0a 2020 2020 2020 2020 2020 2020  rm,.            
+00011b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b60: 2020 2764 6f63 756d 656e 7427 3a20 7365    'document': se
+00011b70: 6c66 2e64 6f63 756d 656e 742c 0a20 2020  lf.document,.   
 00011b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b90: 2020 2020 2020 2764 6573 6372 6970 7469        'descripti
-00011ba0: 6f6e 273a 2073 656c 662e 6465 7363 7269  on': self.descri
-00011bb0: 7074 696f 6e7d 5d29 2e73 6574 5f69 6e64  ption}]).set_ind
-00011bc0: 6578 2822 7365 7122 290a 0a20 2020 2064  ex("seq")..    d
-00011bd0: 6566 205f 5f72 6963 685f 5f28 7365 6c66  ef __rich__(self
-00011be0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-00011bf0: 6e20 6466 5f74 6f5f 7269 6368 5f74 6162  n df_to_rich_tab
-00011c00: 6c65 2873 656c 662e 7375 6d6d 6172 7928  le(self.summary(
-00011c10: 292c 2069 6e64 6578 5f6e 616d 653d 2273  ), index_name="s
-00011c20: 6571 2229 0a0a 2020 2020 6465 6620 5f5f  eq")..    def __
-00011c30: 7265 7072 5f5f 2873 656c 6629 3a0a 2020  repr__(self):.  
-00011c40: 2020 2020 2020 7265 7475 726e 2072 6570        return rep
-00011c50: 725f 7269 6368 2873 656c 662e 5f5f 7269  r_rich(self.__ri
-00011c60: 6368 5f5f 2829 290a 0a0a 2320 5468 6573  ch__())...# Thes
-00011c70: 6520 6172 6520 7468 6520 636f 6c75 6d6e  e are the column
-00011c80: 7320 6f6e 2074 6865 2074 6162 6c65 206f  s on the table o
-00011c90: 6e20 7468 6520 6669 6c69 6e67 2068 6f6d  n the filing hom
-00011ca0: 6570 6167 650a 6669 6c69 6e67 5f66 696c  epage.filing_fil
-00011cb0: 655f 636f 6c73 203d 205b 2753 6571 272c  e_cols = ['Seq',
-00011cc0: 2027 4465 7363 7269 7074 696f 6e27 2c20   'Description', 
-00011cd0: 2744 6f63 756d 656e 7427 2c20 2754 7970  'Document', 'Typ
-00011ce0: 6527 2c20 2753 697a 6527 2c20 2755 726c  e', 'Size', 'Url
-00011cf0: 275d 0a0a 0a40 6461 7461 636c 6173 7328  ']...@dataclass(
-00011d00: 6672 6f7a 656e 3d54 7275 6529 0a63 6c61  frozen=True).cla
-00011d10: 7373 2043 6c61 7373 436f 6e74 7261 6374  ss ClassContract
-00011d20: 5365 7269 6573 3a0a 2020 2020 6369 6b3a  Series:.    cik:
-00011d30: 2073 7472 0a20 2020 2075 726c 3a20 7374   str.    url: st
-00011d40: 720a 0a0a 4064 6174 6163 6c61 7373 2866  r...@dataclass(f
-00011d50: 726f 7a65 6e3d 5472 7565 290a 636c 6173  rozen=True).clas
-00011d60: 7320 436c 6173 7343 6f6e 7472 6163 743a  s ClassContract:
-00011d70: 0a20 2020 2063 696b 3a20 7374 720a 2020  .    cik: str.  
-00011d80: 2020 6e61 6d65 3a20 7374 720a 2020 2020    name: str.    
-00011d90: 7469 636b 6572 3a20 7374 720a 2020 2020  ticker: str.    
-00011da0: 7374 6174 7573 3a20 7374 720a 0a0a 4064  status: str...@d
-00011db0: 6174 6163 6c61 7373 2866 726f 7a65 6e3d  ataclass(frozen=
-00011dc0: 5472 7565 290a 636c 6173 7320 4669 6c65  True).class File
-00011dd0: 7249 6e66 6f3a 0a20 2020 2063 6f6d 7061  rInfo:.    compa
-00011de0: 6e79 5f6e 616d 653a 2073 7472 0a20 2020  ny_name: str.   
-00011df0: 2069 6465 6e74 6966 6963 6174 696f 6e3a   identification:
-00011e00: 2073 7472 0a20 2020 2061 6464 7265 7373   str.    address
-00011e10: 6573 3a20 4c69 7374 5b73 7472 5d0a 0a20  es: List[str].. 
-00011e20: 2020 2064 6566 205f 5f72 6963 685f 5f28     def __rich__(
-00011e30: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
-00011e40: 6574 7572 6e20 5061 6e65 6c28 0a20 2020  eturn Panel(.   
-00011e50: 2020 2020 2020 2020 2043 6f6c 756d 6e73           Columns
-00011e60: 285b 7365 6c66 2e69 6465 6e74 6966 6963  ([self.identific
-00011e70: 6174 696f 6e2c 2054 6578 7428 2220 2020  ation, Text("   
-00011e80: 2229 2c20 7365 6c66 2e61 6464 7265 7373  "), self.address
-00011e90: 6573 5b30 5d2c 2073 656c 662e 6164 6472  es[0], self.addr
-00011ea0: 6573 7365 735b 315d 5d29 2c0a 2020 2020  esses[1]]),.    
-00011eb0: 2020 2020 2020 2020 7469 746c 653d 7365          title=se
-00011ec0: 6c66 2e63 6f6d 7061 6e79 5f6e 616d 650a  lf.company_name.
-00011ed0: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-00011ee0: 6566 205f 5f72 6570 725f 5f28 7365 6c66  ef __repr__(self
-00011ef0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-00011f00: 6e20 7265 7072 5f72 6963 6828 7365 6c66  n repr_rich(self
-00011f10: 2e5f 5f72 6963 685f 5f28 2929 0a0a 0a63  .__rich__())...c
-00011f20: 6c61 7373 2046 696c 696e 6748 6f6d 6570  lass FilingHomep
-00011f30: 6167 653a 0a20 2020 2022 2222 0a20 2020  age:.    """.   
-00011f40: 2041 2063 6c61 7373 2074 6861 7420 7265   A class that re
-00011f50: 7072 6573 656e 7473 2074 6865 2068 6f6d  presents the hom
-00011f60: 6570 6167 6520 666f 7220 7468 6520 6669  epage for the fi
-00011f70: 6c69 6e67 2061 6c6c 6f77 696e 6720 7573  ling allowing us
-00011f80: 2074 6f20 6765 7420 7468 6520 646f 6375   to get the docu
-00011f90: 6d65 6e74 7320 616e 6420 6461 7461 6669  ments and datafi
-00011fa0: 6c65 730a 2020 2020 2222 220a 0a20 2020  les.    """..   
-00011fb0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00011fc0: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-00011fd0: 2020 2020 2066 696c 6573 3a20 7064 2e44       files: pd.D
-00011fe0: 6174 6146 7261 6d65 2c0a 2020 2020 2020  ataFrame,.      
-00011ff0: 2020 2020 2020 2020 2020 2075 726c 3a20             url: 
-00012000: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
-00012010: 2020 2020 2020 6669 6c69 6e67 3a20 4669        filing: Fi
-00012020: 6c69 6e67 2c0a 2020 2020 2020 2020 2020  ling,.          
-00012030: 2020 2020 2020 2066 696c 6572 5f69 6e66         filer_inf
-00012040: 6f73 3a20 4c69 7374 5b46 696c 6572 496e  os: List[FilerIn
-00012050: 666f 5d29 3a0a 2020 2020 2020 2020 7365  fo]):.        se
-00012060: 6c66 2e5f 6669 6c65 733a 2070 642e 4461  lf._files: pd.Da
-00012070: 7461 4672 616d 6520 3d20 6669 6c65 730a  taFrame = files.
-00012080: 2020 2020 2020 2020 7365 6c66 2e75 726c          self.url
-00012090: 3a20 7374 7220 3d20 7572 6c0a 2020 2020  : str = url.    
-000120a0: 2020 2020 7365 6c66 2e66 696c 696e 673a      self.filing:
-000120b0: 2046 696c 696e 6720 3d20 6669 6c69 6e67   Filing = filing
-000120c0: 0a20 2020 2020 2020 2073 656c 662e 6669  .        self.fi
-000120d0: 6c65 725f 696e 666f 733a 204c 6973 745b  ler_infos: List[
-000120e0: 4669 6c65 7249 6e66 6f5d 203d 2066 696c  FilerInfo] = fil
-000120f0: 6572 5f69 6e66 6f73 0a0a 2020 2020 6465  er_infos..    de
-00012100: 6620 6765 745f 6669 6c65 2873 656c 662c  f get_file(self,
-00012110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012120: 2020 2a2c 0a20 2020 2020 2020 2020 2020    *,.           
-00012130: 2020 2020 2020 7365 713a 2069 6e74 2920        seq: int) 
-00012140: 2d3e 2041 7474 6163 686d 656e 743a 0a20  -> Attachment:. 
-00012150: 2020 2020 2020 2022 2222 2067 6574 2074         """ get t
-00012160: 6865 2066 696c 696e 6720 646f 6375 6d65  he filing docume
-00012170: 6e74 2074 6861 7420 6d61 7463 6865 7320  nt that matches 
-00012180: 7468 6520 7365 7122 2222 0a20 2020 2020  the seq""".     
-00012190: 2020 2072 6573 203d 2073 656c 662e 5f66     res = self._f
-000121a0: 696c 6573 2e71 7565 7279 2866 2253 6571  iles.query(f"Seq
-000121b0: 3d3d 277b 7365 717d 2722 290a 2020 2020  =='{seq}'").    
-000121c0: 2020 2020 6966 206e 6f74 2072 6573 2e65      if not res.e
-000121d0: 6d70 7479 3a0a 2020 2020 2020 2020 2020  mpty:.          
-000121e0: 2020 7265 7475 726e 2041 7474 6163 686d    return Attachm
-000121f0: 656e 742e 6672 6f6d 5f64 6174 6166 7261  ent.from_datafra
-00012200: 6d65 5f72 6f77 2872 6573 2e69 6c6f 635b  me_row(res.iloc[
-00012210: 305d 290a 0a20 2020 2064 6566 206f 7065  0])..    def ope
-00012220: 6e28 7365 6c66 293a 0a20 2020 2020 2020  n(self):.       
-00012230: 2077 6562 6272 6f77 7365 722e 6f70 656e   webbrowser.open
-00012240: 2873 656c 662e 7572 6c29 0a0a 2020 2020  (self.url)..    
-00012250: 6465 6620 6d69 6e5f 7365 7128 7365 6c66  def min_seq(self
-00012260: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
-00012270: 2020 2222 2247 6574 2074 6865 206d 696e    """Get the min
-00012280: 696d 756d 2064 6f63 756d 656e 7420 7365  imum document se
-00012290: 7175 656e 6365 2066 726f 6d20 7468 6520  quence from the 
-000122a0: 5365 7120 636f 6c75 6d6e 2222 220a 2020  Seq column""".  
-000122b0: 2020 2020 2020 7265 7475 726e 2073 7472        return str
-000122c0: 286d 696e 285b 696e 7428 7365 7129 2066  (min([int(seq) f
-000122d0: 6f72 2073 6571 2069 6e20 7365 6c66 2e64  or seq in self.d
-000122e0: 6f63 756d 656e 7473 2e53 6571 2e74 6f6c  ocuments.Seq.tol
-000122f0: 6973 7428 2920 6966 2073 6571 2061 6e64  ist() if seq and
-00012300: 2073 6571 2e69 7364 6967 6974 2829 5d29   seq.isdigit()])
-00012310: 290a 0a20 2020 2040 7072 6f70 6572 7479  )..    @property
-00012320: 0a20 2020 2040 6c72 755f 6361 6368 6528  .    @lru_cache(
-00012330: 6d61 7873 697a 653d 3229 0a20 2020 2064  maxsize=2).    d
-00012340: 6566 2070 7269 6d61 7279 5f64 6f63 756d  ef primary_docum
-00012350: 656e 7473 2873 656c 6629 202d 3e20 4c69  ents(self) -> Li
-00012360: 7374 5b41 7474 6163 686d 656e 745d 3a0a  st[Attachment]:.
-00012370: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012380: 2020 2020 4765 7420 7468 6520 646f 6375      Get the docu
-00012390: 6d65 6e74 7320 6c69 7374 6564 2061 7320  ments listed as 
-000123a0: 7072 696d 6172 7920 666f 7220 7468 6520  primary for the 
-000123b0: 6669 6c69 6e67 0a20 2020 2020 2020 203a  filing.        :
-000123c0: 7265 7475 726e 3a0a 2020 2020 2020 2020  return:.        
-000123d0: 2222 220a 2020 2020 2020 2020 6d69 6e5f  """.        min_
-000123e0: 7365 7120 3d20 7365 6c66 2e6d 696e 5f73  seq = self.min_s
-000123f0: 6571 2829 0a20 2020 2020 2020 2064 6f63  eq().        doc
-00012400: 5f72 6573 756c 7473 203d 2073 656c 662e  _results = self.
-00012410: 646f 6375 6d65 6e74 732e 7175 6572 7928  documents.query(
-00012420: 6622 5365 713d 3d27 7b6d 696e 5f73 6571  f"Seq=='{min_seq
-00012430: 7d27 2229 0a20 2020 2020 2020 2072 6574  }'").        ret
-00012440: 7572 6e20 5b0a 2020 2020 2020 2020 2020  urn [.          
-00012450: 2020 4174 7461 6368 6d65 6e74 2e66 726f    Attachment.fro
-00012460: 6d5f 6461 7461 6672 616d 655f 726f 7728  m_dataframe_row(
-00012470: 7365 6c66 2e64 6f63 756d 656e 7473 2e69  self.documents.i
-00012480: 6c6f 635b 696e 6465 785d 290a 2020 2020  loc[index]).    
-00012490: 2020 2020 2020 2020 666f 7220 696e 6465          for inde
-000124a0: 7820 696e 2064 6f63 5f72 6573 756c 7473  x in doc_results
-000124b0: 2e69 6e64 6578 0a20 2020 2020 2020 205d  .index.        ]
-000124c0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-000124d0: 2020 2020 6465 6620 7072 696d 6172 795f      def primary_
-000124e0: 786d 6c5f 646f 6375 6d65 6e74 2873 656c  xml_document(sel
-000124f0: 6629 202d 3e20 4f70 7469 6f6e 616c 5b41  f) -> Optional[A
-00012500: 7474 6163 686d 656e 745d 3a0a 2020 2020  ttachment]:.    
-00012510: 2020 2020 2222 2247 6574 2074 6865 2070      """Get the p
-00012520: 7269 6d61 7279 2078 6d6c 2064 6f63 756d  rimary xml docum
-00012530: 656e 7420 6f6e 2074 6865 2066 696c 696e  ent on the filin
-00012540: 6722 2222 0a20 2020 2020 2020 2066 6f72  g""".        for
-00012550: 2064 6f63 2069 6e20 7365 6c66 2e70 7269   doc in self.pri
-00012560: 6d61 7279 5f64 6f63 756d 656e 7473 3a0a  mary_documents:.
-00012570: 2020 2020 2020 2020 2020 2020 6966 2064              if d
-00012580: 6f63 2e64 6973 706c 6179 5f65 7874 656e  oc.display_exten
-00012590: 7369 6f6e 203d 3d20 222e 786d 6c22 3a0a  sion == ".xml":.
-000125a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125b0: 7265 7475 726e 2064 6f63 0a0a 2020 2020  return doc..    
-000125c0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-000125d0: 6620 7465 7874 5f64 6f63 756d 656e 7428  f text_document(
-000125e0: 7365 6c66 2920 2d3e 2041 7474 6163 686d  self) -> Attachm
-000125f0: 656e 743a 0a20 2020 2020 2020 2022 2222  ent:.        """
-00012600: 4765 7420 7468 6520 6675 6c6c 2074 6578  Get the full tex
-00012610: 7420 7375 626d 6973 7369 6f6e 2066 696c  t submission fil
-00012620: 6522 2222 0a20 2020 2020 2020 2072 6573  e""".        res
-00012630: 203d 2073 656c 662e 5f66 696c 6573 5b73   = self._files[s
-00012640: 656c 662e 5f66 696c 6573 2e44 6573 6372  elf._files.Descr
-00012650: 6970 7469 6f6e 203d 3d20 2243 6f6d 706c  iption == "Compl
-00012660: 6574 6520 7375 626d 6973 7369 6f6e 2074  ete submission t
-00012670: 6578 7420 6669 6c65 225d 0a20 2020 2020  ext file"].     
-00012680: 2020 2072 6574 7572 6e20 4174 7461 6368     return Attach
-00012690: 6d65 6e74 2e66 726f 6d5f 6461 7461 6672  ment.from_datafr
-000126a0: 616d 655f 726f 7728 7265 732e 696c 6f63  ame_row(res.iloc
-000126b0: 5b30 5d29 0a0a 2020 2020 4070 726f 7065  [0])..    @prope
-000126c0: 7274 790a 2020 2020 6465 6620 7072 696d  rty.    def prim
-000126d0: 6172 795f 6874 6d6c 5f64 6f63 756d 656e  ary_html_documen
-000126e0: 7428 7365 6c66 2920 2d3e 204f 7074 696f  t(self) -> Optio
-000126f0: 6e61 6c5b 4174 7461 6368 6d65 6e74 5d3a  nal[Attachment]:
-00012700: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
-00012710: 7468 6520 7072 696d 6172 7920 786d 6c20  the primary xml 
-00012720: 646f 6375 6d65 6e74 206f 6e20 7468 6520  document on the 
-00012730: 6669 6c69 6e67 2222 220a 2020 2020 2020  filing""".      
-00012740: 2020 666f 7220 646f 6320 696e 2073 656c    for doc in sel
-00012750: 662e 7072 696d 6172 795f 646f 6375 6d65  f.primary_docume
-00012760: 6e74 733a 0a20 2020 2020 2020 2020 2020  nts:.           
-00012770: 2069 6620 646f 632e 6469 7370 6c61 795f   if doc.display_
-00012780: 6578 7465 6e73 696f 6e20 3d3d 2022 2e68  extension == ".h
-00012790: 746d 6c22 206f 7220 646f 632e 6469 7370  tml" or doc.disp
-000127a0: 6c61 795f 6578 7465 6e73 696f 6e20 3d3d  lay_extension ==
-000127b0: 2027 2e68 746d 273a 0a20 2020 2020 2020   '.htm':.       
-000127c0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000127d0: 646f 630a 2020 2020 2020 2020 2320 5368  doc.        # Sh
-000127e0: 6f75 6c64 6e27 7420 6765 7420 6865 7265  ouldn't get here
-000127f0: 2062 7574 206a 7573 7420 6f70 656e 2074   but just open t
-00012800: 6865 2066 6972 7374 2064 6f63 756d 656e  he first documen
-00012810: 740a 2020 2020 2020 2020 7265 7475 726e  t.        return
-00012820: 2073 656c 662e 7072 696d 6172 795f 646f   self.primary_do
-00012830: 6375 6d65 6e74 735b 305d 0a0a 2020 2020  cuments[0]..    
-00012840: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00012850: 6620 7862 726c 5f64 6f63 756d 656e 7428  f xbrl_document(
-00012860: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00012870: 2222 4669 6e64 2061 6e64 2072 6574 7572  ""Find and retur
-00012880: 6e20 7468 6520 7862 726c 2064 6f63 756d  n the xbrl docum
-00012890: 656e 742e 2222 220a 0a20 2020 2020 2020  ent."""..       
-000128a0: 2023 2043 6861 6e67 6520 6672 6f6d 202e   # Change from .
-000128b0: 7175 6572 7920 7379 6e74 6178 2064 7565  query syntax due
-000128c0: 2074 6f20 6469 6666 6572 656e 6365 7320   to differences 
-000128d0: 696e 2068 6f77 2070 616e 6461 7320 6578  in how pandas ex
-000128e0: 6563 7574 6573 2071 7565 7269 6573 206f  ecutes queries o
-000128f0: 6e20 6f6e 6c69 6e65 2065 6e76 6972 6f6e  n online environ
-00012900: 6d6d 656e 7473 0a20 2020 2020 2020 206d  mments.        m
-00012910: 6174 6368 696e 675f 6669 6c65 7320 3d20  atching_files = 
-00012920: 7365 6c66 2e5f 6669 6c65 735b 7365 6c66  self._files[self
-00012930: 2e5f 6669 6c65 732e 4465 7363 7269 7074  ._files.Descript
-00012940: 696f 6e2e 6973 696e 2878 6272 6c5f 646f  ion.isin(xbrl_do
-00012950: 6375 6d65 6e74 5f74 7970 6573 295d 0a20  cument_types)]. 
-00012960: 2020 2020 2020 2069 6620 6e6f 7420 6d61         if not ma
-00012970: 7463 6869 6e67 5f66 696c 6573 2e65 6d70  tching_files.emp
-00012980: 7479 3a0a 2020 2020 2020 2020 2020 2020  ty:.            
-00012990: 7265 6320 3d20 6d61 7463 6869 6e67 5f66  rec = matching_f
-000129a0: 696c 6573 2e69 6c6f 635b 305d 0a20 2020  iles.iloc[0].   
-000129b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000129c0: 4174 7461 6368 6d65 6e74 2e66 726f 6d5f  Attachment.from_
-000129d0: 6461 7461 6672 616d 655f 726f 7728 7265  dataframe_row(re
-000129e0: 6329 0a0a 2020 2020 6465 6620 6765 745f  c)..    def get_
-000129f0: 6d61 7463 6869 6e67 5f66 696c 6573 2873  matching_files(s
-00012a00: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+00011b90: 2020 2020 2020 2020 2020 2027 6465 7363             'desc
+00011ba0: 7269 7074 696f 6e27 3a20 7365 6c66 2e64  ription': self.d
+00011bb0: 6573 6372 6970 7469 6f6e 7d5d 292e 7365  escription}]).se
+00011bc0: 745f 696e 6465 7828 2273 6571 2229 0a0a  t_index("seq")..
+00011bd0: 2020 2020 6465 6620 5f5f 7269 6368 5f5f      def __rich__
+00011be0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00011bf0: 7265 7475 726e 2064 665f 746f 5f72 6963  return df_to_ric
+00011c00: 685f 7461 626c 6528 7365 6c66 2e73 756d  h_table(self.sum
+00011c10: 6d61 7279 2829 2c20 696e 6465 785f 6e61  mary(), index_na
+00011c20: 6d65 3d22 7365 7122 290a 0a20 2020 2064  me="seq")..    d
+00011c30: 6566 205f 5f72 6570 725f 5f28 7365 6c66  ef __repr__(self
+00011c40: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+00011c50: 6e20 7265 7072 5f72 6963 6828 7365 6c66  n repr_rich(self
+00011c60: 2e5f 5f72 6963 685f 5f28 2929 0a0a 0a23  .__rich__())...#
+00011c70: 2054 6865 7365 2061 7265 2074 6865 2063   These are the c
+00011c80: 6f6c 756d 6e73 206f 6e20 7468 6520 7461  olumns on the ta
+00011c90: 626c 6520 6f6e 2074 6865 2066 696c 696e  ble on the filin
+00011ca0: 6720 686f 6d65 7061 6765 0a66 696c 696e  g homepage.filin
+00011cb0: 675f 6669 6c65 5f63 6f6c 7320 3d20 5b27  g_file_cols = ['
+00011cc0: 5365 7127 2c20 2744 6573 6372 6970 7469  Seq', 'Descripti
+00011cd0: 6f6e 272c 2027 446f 6375 6d65 6e74 272c  on', 'Document',
+00011ce0: 2027 5479 7065 272c 2027 5369 7a65 272c   'Type', 'Size',
+00011cf0: 2027 5572 6c27 5d0a 0a0a 4064 6174 6163   'Url']...@datac
+00011d00: 6c61 7373 2866 726f 7a65 6e3d 5472 7565  lass(frozen=True
+00011d10: 290a 636c 6173 7320 436c 6173 7343 6f6e  ).class ClassCon
+00011d20: 7472 6163 7453 6572 6965 733a 0a20 2020  tractSeries:.   
+00011d30: 2063 696b 3a20 7374 720a 2020 2020 7572   cik: str.    ur
+00011d40: 6c3a 2073 7472 0a0a 0a40 6461 7461 636c  l: str...@datacl
+00011d50: 6173 7328 6672 6f7a 656e 3d54 7275 6529  ass(frozen=True)
+00011d60: 0a63 6c61 7373 2043 6c61 7373 436f 6e74  .class ClassCont
+00011d70: 7261 6374 3a0a 2020 2020 6369 6b3a 2073  ract:.    cik: s
+00011d80: 7472 0a20 2020 206e 616d 653a 2073 7472  tr.    name: str
+00011d90: 0a20 2020 2074 6963 6b65 723a 2073 7472  .    ticker: str
+00011da0: 0a20 2020 2073 7461 7475 733a 2073 7472  .    status: str
+00011db0: 0a0a 0a40 6461 7461 636c 6173 7328 6672  ...@dataclass(fr
+00011dc0: 6f7a 656e 3d54 7275 6529 0a63 6c61 7373  ozen=True).class
+00011dd0: 2046 696c 6572 496e 666f 3a0a 2020 2020   FilerInfo:.    
+00011de0: 636f 6d70 616e 795f 6e61 6d65 3a20 7374  company_name: st
+00011df0: 720a 2020 2020 6964 656e 7469 6669 6361  r.    identifica
+00011e00: 7469 6f6e 3a20 7374 720a 2020 2020 6164  tion: str.    ad
+00011e10: 6472 6573 7365 733a 204c 6973 745b 7374  dresses: List[st
+00011e20: 725d 0a0a 2020 2020 6465 6620 5f5f 7269  r]..    def __ri
+00011e30: 6368 5f5f 2873 656c 6629 3a0a 2020 2020  ch__(self):.    
+00011e40: 2020 2020 7265 7475 726e 2050 616e 656c      return Panel
+00011e50: 280a 2020 2020 2020 2020 2020 2020 436f  (.            Co
+00011e60: 6c75 6d6e 7328 5b73 656c 662e 6964 656e  lumns([self.iden
+00011e70: 7469 6669 6361 7469 6f6e 2c20 5465 7874  tification, Text
+00011e80: 2822 2020 2022 292c 2073 656c 662e 6164  ("   "), self.ad
+00011e90: 6472 6573 7365 735b 305d 2c20 7365 6c66  dresses[0], self
+00011ea0: 2e61 6464 7265 7373 6573 5b31 5d5d 292c  .addresses[1]]),
+00011eb0: 0a20 2020 2020 2020 2020 2020 2074 6974  .            tit
+00011ec0: 6c65 3d73 656c 662e 636f 6d70 616e 795f  le=self.company_
+00011ed0: 6e61 6d65 0a20 2020 2020 2020 2029 0a0a  name.        )..
+00011ee0: 2020 2020 6465 6620 5f5f 7265 7072 5f5f      def __repr__
+00011ef0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00011f00: 7265 7475 726e 2072 6570 725f 7269 6368  return repr_rich
+00011f10: 2873 656c 662e 5f5f 7269 6368 5f5f 2829  (self.__rich__()
+00011f20: 290a 0a0a 636c 6173 7320 4669 6c69 6e67  )...class Filing
+00011f30: 486f 6d65 7061 6765 3a0a 2020 2020 2222  Homepage:.    ""
+00011f40: 220a 2020 2020 4120 636c 6173 7320 7468  ".    A class th
+00011f50: 6174 2072 6570 7265 7365 6e74 7320 7468  at represents th
+00011f60: 6520 686f 6d65 7061 6765 2066 6f72 2074  e homepage for t
+00011f70: 6865 2066 696c 696e 6720 616c 6c6f 7769  he filing allowi
+00011f80: 6e67 2075 7320 746f 2067 6574 2074 6865  ng us to get the
+00011f90: 2064 6f63 756d 656e 7473 2061 6e64 2064   documents and d
+00011fa0: 6174 6166 696c 6573 0a20 2020 2022 2222  atafiles.    """
+00011fb0: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00011fc0: 5f5f 2873 656c 662c 0a20 2020 2020 2020  __(self,.       
+00011fd0: 2020 2020 2020 2020 2020 6669 6c65 733a            files:
+00011fe0: 2070 642e 4461 7461 4672 616d 652c 0a20   pd.DataFrame,. 
+00011ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012000: 7572 6c3a 2073 7472 2c0a 2020 2020 2020  url: str,.      
+00012010: 2020 2020 2020 2020 2020 2066 696c 696e             filin
+00012020: 673a 2046 696c 696e 672c 0a20 2020 2020  g: Filing,.     
+00012030: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+00012040: 725f 696e 666f 733a 204c 6973 745b 4669  r_infos: List[Fi
+00012050: 6c65 7249 6e66 6f5d 293a 0a20 2020 2020  lerInfo]):.     
+00012060: 2020 2073 656c 662e 5f66 696c 6573 3a20     self._files: 
+00012070: 7064 2e44 6174 6146 7261 6d65 203d 2066  pd.DataFrame = f
+00012080: 696c 6573 0a20 2020 2020 2020 2073 656c  iles.        sel
+00012090: 662e 7572 6c3a 2073 7472 203d 2075 726c  f.url: str = url
+000120a0: 0a20 2020 2020 2020 2073 656c 662e 6669  .        self.fi
+000120b0: 6c69 6e67 3a20 4669 6c69 6e67 203d 2066  ling: Filing = f
+000120c0: 696c 696e 670a 2020 2020 2020 2020 7365  iling.        se
+000120d0: 6c66 2e66 696c 6572 5f69 6e66 6f73 3a20  lf.filer_infos: 
+000120e0: 4c69 7374 5b46 696c 6572 496e 666f 5d20  List[FilerInfo] 
+000120f0: 3d20 6669 6c65 725f 696e 666f 730a 0a20  = filer_infos.. 
+00012100: 2020 2064 6566 2067 6574 5f66 696c 6528     def get_file(
+00012110: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+00012120: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
+00012130: 2020 2020 2020 2020 2020 2073 6571 3a20             seq: 
+00012140: 696e 7429 202d 3e20 4174 7461 6368 6d65  int) -> Attachme
+00012150: 6e74 3a0a 2020 2020 2020 2020 2222 2220  nt:.        """ 
+00012160: 6765 7420 7468 6520 6669 6c69 6e67 2064  get the filing d
+00012170: 6f63 756d 656e 7420 7468 6174 206d 6174  ocument that mat
+00012180: 6368 6573 2074 6865 2073 6571 2222 220a  ches the seq""".
+00012190: 2020 2020 2020 2020 7265 7320 3d20 7365          res = se
+000121a0: 6c66 2e5f 6669 6c65 732e 7175 6572 7928  lf._files.query(
+000121b0: 6622 5365 713d 3d27 7b73 6571 7d27 2229  f"Seq=='{seq}'")
+000121c0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000121d0: 7265 732e 656d 7074 793a 0a20 2020 2020  res.empty:.     
+000121e0: 2020 2020 2020 2072 6574 7572 6e20 4174         return At
+000121f0: 7461 6368 6d65 6e74 2e66 726f 6d5f 6461  tachment.from_da
+00012200: 7461 6672 616d 655f 726f 7728 7265 732e  taframe_row(res.
+00012210: 696c 6f63 5b30 5d29 0a0a 2020 2020 6465  iloc[0])..    de
+00012220: 6620 6f70 656e 2873 656c 6629 3a0a 2020  f open(self):.  
+00012230: 2020 2020 2020 7765 6262 726f 7773 6572        webbrowser
+00012240: 2e6f 7065 6e28 7365 6c66 2e75 726c 290a  .open(self.url).
+00012250: 0a20 2020 2064 6566 206d 696e 5f73 6571  .    def min_seq
+00012260: 2873 656c 6629 202d 3e20 7374 723a 0a20  (self) -> str:. 
+00012270: 2020 2020 2020 2022 2222 4765 7420 7468         """Get th
+00012280: 6520 6d69 6e69 6d75 6d20 646f 6375 6d65  e minimum docume
+00012290: 6e74 2073 6571 7565 6e63 6520 6672 6f6d  nt sequence from
+000122a0: 2074 6865 2053 6571 2063 6f6c 756d 6e22   the Seq column"
+000122b0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+000122c0: 6e20 7374 7228 6d69 6e28 5b69 6e74 2873  n str(min([int(s
+000122d0: 6571 2920 666f 7220 7365 7120 696e 2073  eq) for seq in s
+000122e0: 656c 662e 646f 6375 6d65 6e74 732e 5365  elf.documents.Se
+000122f0: 712e 746f 6c69 7374 2829 2069 6620 7365  q.tolist() if se
+00012300: 7120 616e 6420 7365 712e 6973 6469 6769  q and seq.isdigi
+00012310: 7428 295d 2929 0a0a 2020 2020 4070 726f  t()]))..    @pro
+00012320: 7065 7274 790a 2020 2020 406c 7275 5f63  perty.    @lru_c
+00012330: 6163 6865 286d 6178 7369 7a65 3d32 290a  ache(maxsize=2).
+00012340: 2020 2020 6465 6620 7072 696d 6172 795f      def primary_
+00012350: 646f 6375 6d65 6e74 7328 7365 6c66 2920  documents(self) 
+00012360: 2d3e 204c 6973 745b 4174 7461 6368 6d65  -> List[Attachme
+00012370: 6e74 5d3a 0a20 2020 2020 2020 2022 2222  nt]:.        """
+00012380: 0a20 2020 2020 2020 2047 6574 2074 6865  .        Get the
+00012390: 2064 6f63 756d 656e 7473 206c 6973 7465   documents liste
+000123a0: 6420 6173 2070 7269 6d61 7279 2066 6f72  d as primary for
+000123b0: 2074 6865 2066 696c 696e 670a 2020 2020   the filing.    
+000123c0: 2020 2020 3a72 6574 7572 6e3a 0a20 2020      :return:.   
+000123d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000123e0: 206d 696e 5f73 6571 203d 2073 656c 662e   min_seq = self.
+000123f0: 6d69 6e5f 7365 7128 290a 2020 2020 2020  min_seq().      
+00012400: 2020 646f 635f 7265 7375 6c74 7320 3d20    doc_results = 
+00012410: 7365 6c66 2e64 6f63 756d 656e 7473 2e71  self.documents.q
+00012420: 7565 7279 2866 2253 6571 3d3d 277b 6d69  uery(f"Seq=='{mi
+00012430: 6e5f 7365 717d 2722 290a 2020 2020 2020  n_seq}'").      
+00012440: 2020 7265 7475 726e 205b 0a20 2020 2020    return [.     
+00012450: 2020 2020 2020 2041 7474 6163 686d 656e         Attachmen
+00012460: 742e 6672 6f6d 5f64 6174 6166 7261 6d65  t.from_dataframe
+00012470: 5f72 6f77 2873 656c 662e 646f 6375 6d65  _row(self.docume
+00012480: 6e74 732e 696c 6f63 5b69 6e64 6578 5d29  nts.iloc[index])
+00012490: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+000124a0: 2069 6e64 6578 2069 6e20 646f 635f 7265   index in doc_re
+000124b0: 7375 6c74 732e 696e 6465 780a 2020 2020  sults.index.    
+000124c0: 2020 2020 5d0a 0a20 2020 2040 7072 6f70      ]..    @prop
+000124d0: 6572 7479 0a20 2020 2064 6566 2070 7269  erty.    def pri
+000124e0: 6d61 7279 5f78 6d6c 5f64 6f63 756d 656e  mary_xml_documen
+000124f0: 7428 7365 6c66 2920 2d3e 204f 7074 696f  t(self) -> Optio
+00012500: 6e61 6c5b 4174 7461 6368 6d65 6e74 5d3a  nal[Attachment]:
+00012510: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
+00012520: 7468 6520 7072 696d 6172 7920 786d 6c20  the primary xml 
+00012530: 646f 6375 6d65 6e74 206f 6e20 7468 6520  document on the 
+00012540: 6669 6c69 6e67 2222 220a 2020 2020 2020  filing""".      
+00012550: 2020 666f 7220 646f 6320 696e 2073 656c    for doc in sel
+00012560: 662e 7072 696d 6172 795f 646f 6375 6d65  f.primary_docume
+00012570: 6e74 733a 0a20 2020 2020 2020 2020 2020  nts:.           
+00012580: 2069 6620 646f 632e 6469 7370 6c61 795f   if doc.display_
+00012590: 6578 7465 6e73 696f 6e20 3d3d 2022 2e78  extension == ".x
+000125a0: 6d6c 223a 0a20 2020 2020 2020 2020 2020  ml":.           
+000125b0: 2020 2020 2072 6574 7572 6e20 646f 630a       return doc.
+000125c0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+000125d0: 2020 2064 6566 2074 6578 745f 646f 6375     def text_docu
+000125e0: 6d65 6e74 2873 656c 6629 202d 3e20 4174  ment(self) -> At
+000125f0: 7461 6368 6d65 6e74 3a0a 2020 2020 2020  tachment:.      
+00012600: 2020 2222 2247 6574 2074 6865 2066 756c    """Get the ful
+00012610: 6c20 7465 7874 2073 7562 6d69 7373 696f  l text submissio
+00012620: 6e20 6669 6c65 2222 220a 2020 2020 2020  n file""".      
+00012630: 2020 7265 7320 3d20 7365 6c66 2e5f 6669    res = self._fi
+00012640: 6c65 735b 7365 6c66 2e5f 6669 6c65 732e  les[self._files.
+00012650: 4465 7363 7269 7074 696f 6e20 3d3d 2022  Description == "
+00012660: 436f 6d70 6c65 7465 2073 7562 6d69 7373  Complete submiss
+00012670: 696f 6e20 7465 7874 2066 696c 6522 5d0a  ion text file"].
+00012680: 2020 2020 2020 2020 7265 7475 726e 2041          return A
+00012690: 7474 6163 686d 656e 742e 6672 6f6d 5f64  ttachment.from_d
+000126a0: 6174 6166 7261 6d65 5f72 6f77 2872 6573  ataframe_row(res
+000126b0: 2e69 6c6f 635b 305d 290a 0a20 2020 2040  .iloc[0])..    @
+000126c0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+000126d0: 2070 7269 6d61 7279 5f68 746d 6c5f 646f   primary_html_do
+000126e0: 6375 6d65 6e74 2873 656c 6629 202d 3e20  cument(self) -> 
+000126f0: 4f70 7469 6f6e 616c 5b41 7474 6163 686d  Optional[Attachm
+00012700: 656e 745d 3a0a 2020 2020 2020 2020 2222  ent]:.        ""
+00012710: 2247 6574 2074 6865 2070 7269 6d61 7279  "Get the primary
+00012720: 2078 6d6c 2064 6f63 756d 656e 7420 6f6e   xml document on
+00012730: 2074 6865 2066 696c 696e 6722 2222 0a20   the filing""". 
+00012740: 2020 2020 2020 2066 6f72 2064 6f63 2069         for doc i
+00012750: 6e20 7365 6c66 2e70 7269 6d61 7279 5f64  n self.primary_d
+00012760: 6f63 756d 656e 7473 3a0a 2020 2020 2020  ocuments:.      
+00012770: 2020 2020 2020 6966 2064 6f63 2e64 6973        if doc.dis
+00012780: 706c 6179 5f65 7874 656e 7369 6f6e 203d  play_extension =
+00012790: 3d20 222e 6874 6d6c 2220 6f72 2064 6f63  = ".html" or doc
+000127a0: 2e64 6973 706c 6179 5f65 7874 656e 7369  .display_extensi
+000127b0: 6f6e 203d 3d20 272e 6874 6d27 3a0a 2020  on == '.htm':.  
+000127c0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000127d0: 7475 726e 2064 6f63 0a20 2020 2020 2020  turn doc.       
+000127e0: 2023 2053 686f 756c 646e 2774 2067 6574   # Shouldn't get
+000127f0: 2068 6572 6520 6275 7420 6a75 7374 206f   here but just o
+00012800: 7065 6e20 7468 6520 6669 7273 7420 646f  pen the first do
+00012810: 6375 6d65 6e74 0a20 2020 2020 2020 2072  cument.        r
+00012820: 6574 7572 6e20 7365 6c66 2e70 7269 6d61  eturn self.prima
+00012830: 7279 5f64 6f63 756d 656e 7473 5b30 5d0a  ry_documents[0].
+00012840: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+00012850: 2020 2064 6566 2078 6272 6c5f 646f 6375     def xbrl_docu
+00012860: 6d65 6e74 2873 656c 6629 3a0a 2020 2020  ment(self):.    
+00012870: 2020 2020 2222 2246 696e 6420 616e 6420      """Find and 
+00012880: 7265 7475 726e 2074 6865 2078 6272 6c20  return the xbrl 
+00012890: 646f 6375 6d65 6e74 2e22 2222 0a0a 2020  document."""..  
+000128a0: 2020 2020 2020 2320 4368 616e 6765 2066        # Change f
+000128b0: 726f 6d20 2e71 7565 7279 2073 796e 7461  rom .query synta
+000128c0: 7820 6475 6520 746f 2064 6966 6665 7265  x due to differe
+000128d0: 6e63 6573 2069 6e20 686f 7720 7061 6e64  nces in how pand
+000128e0: 6173 2065 7865 6375 7465 7320 7175 6572  as executes quer
+000128f0: 6965 7320 6f6e 206f 6e6c 696e 6520 656e  ies on online en
+00012900: 7669 726f 6e6d 6d65 6e74 730a 2020 2020  vironmments.    
+00012910: 2020 2020 6d61 7463 6869 6e67 5f66 696c      matching_fil
+00012920: 6573 203d 2073 656c 662e 5f66 696c 6573  es = self._files
+00012930: 5b73 656c 662e 5f66 696c 6573 2e44 6573  [self._files.Des
+00012940: 6372 6970 7469 6f6e 2e69 7369 6e28 7862  cription.isin(xb
+00012950: 726c 5f64 6f63 756d 656e 745f 7479 7065  rl_document_type
+00012960: 7329 5d0a 2020 2020 2020 2020 6966 206e  s)].        if n
+00012970: 6f74 206d 6174 6368 696e 675f 6669 6c65  ot matching_file
+00012980: 732e 656d 7074 793a 0a20 2020 2020 2020  s.empty:.       
+00012990: 2020 2020 2072 6563 203d 206d 6174 6368       rec = match
+000129a0: 696e 675f 6669 6c65 732e 696c 6f63 5b30  ing_files.iloc[0
+000129b0: 5d0a 2020 2020 2020 2020 2020 2020 7265  ].            re
+000129c0: 7475 726e 2041 7474 6163 686d 656e 742e  turn Attachment.
+000129d0: 6672 6f6d 5f64 6174 6166 7261 6d65 5f72  from_dataframe_r
+000129e0: 6f77 2872 6563 290a 0a20 2020 2064 6566  ow(rec)..    def
+000129f0: 2067 6574 5f6d 6174 6368 696e 675f 6669   get_matching_fi
+00012a00: 6c65 7328 7365 6c66 2c0a 2020 2020 2020  les(self,.      
 00012a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a20: 7175 6572 793a 2073 7472 2920 2d3e 2070  query: str) -> p
-00012a30: 642e 4461 7461 4672 616d 653a 0a20 2020  d.DataFrame:.   
-00012a40: 2020 2020 2022 2222 2072 6574 7572 6e20       """ return 
-00012a50: 7468 6520 6669 6c65 7320 7468 6174 206d  the files that m
-00012a60: 6174 6368 2074 6865 2071 7565 7279 2222  atch the query""
-00012a70: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-00012a80: 2073 656c 662e 5f66 696c 6573 2e71 7565   self._files.que
-00012a90: 7279 2871 7565 7279 2c20 656e 6769 6e65  ry(query, engine
-00012aa0: 3d22 7079 7468 6f6e 2229 2e72 6573 6574  ="python").reset
-00012ab0: 5f69 6e64 6578 2864 726f 703d 5472 7565  _index(drop=True
-00012ac0: 292e 6669 6c74 6572 2866 696c 696e 675f  ).filter(filing_
-00012ad0: 6669 6c65 5f63 6f6c 7329 0a0a 2020 2020  file_cols)..    
-00012ae0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00012af0: 6620 646f 6375 6d65 6e74 7328 7365 6c66  f documents(self
-00012b00: 2920 2d3e 2070 642e 4461 7461 4672 616d  ) -> pd.DataFram
-00012b10: 653a 0a20 2020 2020 2020 2022 2222 2072  e:.        """ r
-00012b20: 6574 7572 6e73 2074 6865 2066 696c 6573  eturns the files
-00012b30: 2074 6861 7420 6172 6520 696e 2074 6865   that are in the
-00012b40: 2022 446f 6375 6d65 6e74 2046 6f72 6d61   "Document Forma
-00012b50: 7420 4669 6c65 7322 2074 6162 6c65 206f  t Files" table o
-00012b60: 6620 7468 6520 686f 6d65 7061 6765 2222  f the homepage""
-00012b70: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-00012b80: 2073 656c 662e 6765 745f 6d61 7463 6869   self.get_matchi
-00012b90: 6e67 5f66 696c 6573 2822 7461 626c 653d  ng_files("table=
-00012ba0: 3d27 446f 6375 6d65 6e74 2046 6f72 6d61  ='Document Forma
-00012bb0: 7420 4669 6c65 7327 2229 0a0a 2020 2020  t Files'")..    
-00012bc0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00012bd0: 6620 6461 7461 6669 6c65 7328 7365 6c66  f datafiles(self
-00012be0: 293a 0a20 2020 2020 2020 2022 2222 2072  ):.        """ r
-00012bf0: 6574 7572 6e73 2074 6865 2066 696c 6573  eturns the files
-00012c00: 2074 6861 7420 6172 6520 696e 2074 6865   that are in the
-00012c10: 2022 4461 7461 2046 696c 6573 2220 7461   "Data Files" ta
-00012c20: 626c 6520 6f66 2074 6865 2068 6f6d 6570  ble of the homep
-00012c30: 6167 6522 2222 0a20 2020 2020 2020 2072  age""".        r
-00012c40: 6574 7572 6e20 7365 6c66 2e67 6574 5f6d  eturn self.get_m
-00012c50: 6174 6368 696e 675f 6669 6c65 7328 2274  atching_files("t
-00012c60: 6162 6c65 3d3d 2744 6174 6120 4669 6c65  able=='Data File
-00012c70: 7327 2229 0a0a 2020 2020 4070 726f 7065  s'")..    @prope
-00012c80: 7274 790a 2020 2020 406c 7275 5f63 6163  rty.    @lru_cac
-00012c90: 6865 286d 6178 7369 7a65 3d32 290a 2020  he(maxsize=2).  
-00012ca0: 2020 6465 6620 6174 7461 6368 6d65 6e74    def attachment
-00012cb0: 7328 7365 6c66 2920 2d3e 2041 7474 6163  s(self) -> Attac
-00012cc0: 686d 656e 7473 3a0a 2020 2020 2020 2020  hments:.        
-00012cd0: 7265 7475 726e 2041 7474 6163 686d 656e  return Attachmen
-00012ce0: 7473 2873 656c 662e 5f66 696c 6573 290a  ts(self._files).
-00012cf0: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00012d00: 640a 2020 2020 6465 6620 6672 6f6d 5f68  d.    def from_h
-00012d10: 746d 6c28 636c 732c 0a20 2020 2020 2020  tml(cls,.       
-00012d20: 2020 2020 2020 2020 2020 2068 6f6d 6570             homep
-00012d30: 6167 655f 6874 6d6c 3a20 7374 722c 0a20  age_html: str,. 
-00012d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d50: 2075 726c 3a20 7374 722c 0a20 2020 2020   url: str,.     
-00012d60: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-00012d70: 696e 673a 2046 696c 696e 6729 3a0a 2020  ing: Filing):.  
-00012d80: 2020 2020 2020 2222 2250 6172 7365 2074        """Parse t
-00012d90: 6865 2048 544d 4c20 616e 6420 6372 6561  he HTML and crea
-00012da0: 7465 2074 6865 2048 6f6d 6570 6167 6520  te the Homepage 
-00012db0: 6672 6f6d 2069 7422 2222 0a0a 2020 2020  from it"""..    
-00012dc0: 2020 2020 2320 4974 2069 7320 6874 6d6c      # It is html
-00012dd0: 2073 6f20 7573 6520 2268 746d 6c2e 7061   so use "html.pa
-00012de0: 7273 6572 2220 2869 6e73 7465 6164 206f  rser" (instead o
-00012df0: 6620 2278 6d6c 222c 206f 7220 226c 786d  f "xml", or "lxm
-00012e00: 6c22 290a 2020 2020 2020 2020 736f 7570  l").        soup
-00012e10: 203d 2042 6561 7574 6966 756c 536f 7570   = BeautifulSoup
-00012e20: 2868 6f6d 6570 6167 655f 6874 6d6c 2c20  (homepage_html, 
-00012e30: 2268 746d 6c2e 7061 7273 6572 2229 0a0a  "html.parser")..
-00012e40: 2020 2020 2020 2020 2320 4b65 6570 2074          # Keep t
-00012e50: 7261 636b 206f 6620 7468 6520 7461 626c  rack of the tabl
-00012e60: 6573 2061 7320 6461 7461 6672 616d 6573  es as dataframes
-00012e70: 2c20 736f 2077 6520 6361 6e20 6170 7065  , so we can appe
-00012e80: 6e64 206c 6174 6572 0a20 2020 2020 2020  nd later.       
-00012e90: 2064 6673 203d 205b 5d0a 0a20 2020 2020   dfs = []..     
-00012ea0: 2020 2023 2054 6865 2074 6162 6c65 2063     # The table c
-00012eb0: 6f6e 7461 696e 696e 2074 6865 2061 7474  ontainin the att
-00012ec0: 6163 686d 656e 7473 0a20 2020 2020 2020  achments.       
-00012ed0: 2074 6162 6c65 7320 3d20 736f 7570 2e66   tables = soup.f
-00012ee0: 696e 645f 616c 6c28 2274 6162 6c65 222c  ind_all("table",
-00012ef0: 2063 6c61 7373 5f3d 2274 6162 6c65 4669   class_="tableFi
-00012f00: 6c65 2229 0a20 2020 2020 2020 2066 6f72  le").        for
-00012f10: 2074 6162 6c65 2069 6e20 7461 626c 6573   table in tables
-00012f20: 3a0a 2020 2020 2020 2020 2020 2020 7375  :.            su
-00012f30: 6d6d 6172 7920 3d20 7461 626c 652e 6174  mmary = table.at
-00012f40: 7472 732e 6765 7428 2273 756d 6d61 7279  trs.get("summary
-00012f50: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
-00012f60: 6f77 7320 3d20 7461 626c 652e 6669 6e64  ows = table.find
-00012f70: 5f61 6c6c 2822 7472 2229 0a20 2020 2020  _all("tr").     
-00012f80: 2020 2020 2020 2063 6f6c 756d 6e5f 6e61         column_na
-00012f90: 6d65 7320 3d20 5b74 682e 7465 7874 2066  mes = [th.text f
-00012fa0: 6f72 2074 6820 696e 2072 6f77 735b 305d  or th in rows[0]
-00012fb0: 2e66 696e 645f 616c 6c28 2274 6822 295d  .find_all("th")]
-00012fc0: 202b 205b 2255 726c 225d 0a20 2020 2020   + ["Url"].     
-00012fd0: 2020 2020 2020 2072 6563 6f72 6473 203d         records =
-00012fe0: 205b 5d0a 0a20 2020 2020 2020 2020 2020   []..           
-00012ff0: 2023 2041 6464 2074 6865 2072 6f77 7320   # Add the rows 
-00013000: 6672 6f6d 2074 6865 2074 6162 6c65 0a20  from the table. 
-00013010: 2020 2020 2020 2020 2020 2066 6f72 2072             for r
-00013020: 6f77 2069 6e20 726f 7773 5b31 3a5d 3a0a  ow in rows[1:]:.
-00013030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013040: 6365 6c6c 7320 3d20 726f 772e 6669 6e64  cells = row.find
-00013050: 5f61 6c6c 2822 7464 2229 0a20 2020 2020  _all("td").     
-00013060: 2020 2020 2020 2020 2020 206c 696e 6b20             link 
-00013070: 3d20 6365 6c6c 735b 325d 2e61 0a20 2020  = cells[2].a.   
-00013080: 2020 2020 2020 2020 2020 2020 2063 656c               cel
-00013090: 6c5f 7661 6c75 6573 203d 205b 6365 6c6c  l_values = [cell
-000130a0: 2e74 6578 7420 666f 7220 6365 6c6c 2069  .text for cell i
-000130b0: 6e20 6365 6c6c 735d 202b 205b 6c69 6e6b  n cells] + [link
-000130c0: 5b22 6872 6566 225d 2069 6620 6c69 6e6b  ["href"] if link
-000130d0: 2065 6c73 6520 4e6f 6e65 5d0a 2020 2020   else None].    
-000130e0: 2020 2020 2020 2020 2020 2020 7265 636f              reco
-000130f0: 7264 732e 6170 7065 6e64 2863 656c 6c5f  rds.append(cell_
-00013100: 7661 6c75 6573 290a 0a20 2020 2020 2020  values)..       
-00013110: 2020 2020 2023 204e 6f77 2063 7265 6174       # Now creat
-00013120: 6520 7468 6520 6461 7461 6672 616d 650a  e the dataframe.
-00013130: 2020 2020 2020 2020 2020 2020 7461 626c              tabl
-00013140: 655f 6173 5f64 6620 3d20 2870 642e 4461  e_as_df = (pd.Da
-00013150: 7461 4672 616d 6528 7265 636f 7264 732c  taFrame(records,
-00013160: 2063 6f6c 756d 6e73 3d63 6f6c 756d 6e5f   columns=column_
-00013170: 6e61 6d65 7329 0a20 2020 2020 2020 2020  names).         
+00012a20: 2020 2020 2071 7565 7279 3a20 7374 7229       query: str)
+00012a30: 202d 3e20 7064 2e44 6174 6146 7261 6d65   -> pd.DataFrame
+00012a40: 3a0a 2020 2020 2020 2020 2222 2220 7265  :.        """ re
+00012a50: 7475 726e 2074 6865 2066 696c 6573 2074  turn the files t
+00012a60: 6861 7420 6d61 7463 6820 7468 6520 7175  hat match the qu
+00012a70: 6572 7922 2222 0a20 2020 2020 2020 2072  ery""".        r
+00012a80: 6574 7572 6e20 7365 6c66 2e5f 6669 6c65  eturn self._file
+00012a90: 732e 7175 6572 7928 7175 6572 792c 2065  s.query(query, e
+00012aa0: 6e67 696e 653d 2270 7974 686f 6e22 292e  ngine="python").
+00012ab0: 7265 7365 745f 696e 6465 7828 6472 6f70  reset_index(drop
+00012ac0: 3d54 7275 6529 2e66 696c 7465 7228 6669  =True).filter(fi
+00012ad0: 6c69 6e67 5f66 696c 655f 636f 6c73 290a  ling_file_cols).
+00012ae0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+00012af0: 2020 2064 6566 2064 6f63 756d 656e 7473     def documents
+00012b00: 2873 656c 6629 202d 3e20 7064 2e44 6174  (self) -> pd.Dat
+00012b10: 6146 7261 6d65 3a0a 2020 2020 2020 2020  aFrame:.        
+00012b20: 2222 2220 7265 7475 726e 7320 7468 6520  """ returns the 
+00012b30: 6669 6c65 7320 7468 6174 2061 7265 2069  files that are i
+00012b40: 6e20 7468 6520 2244 6f63 756d 656e 7420  n the "Document 
+00012b50: 466f 726d 6174 2046 696c 6573 2220 7461  Format Files" ta
+00012b60: 626c 6520 6f66 2074 6865 2068 6f6d 6570  ble of the homep
+00012b70: 6167 6522 2222 0a20 2020 2020 2020 2072  age""".        r
+00012b80: 6574 7572 6e20 7365 6c66 2e67 6574 5f6d  eturn self.get_m
+00012b90: 6174 6368 696e 675f 6669 6c65 7328 2274  atching_files("t
+00012ba0: 6162 6c65 3d3d 2744 6f63 756d 656e 7420  able=='Document 
+00012bb0: 466f 726d 6174 2046 696c 6573 2722 290a  Format Files'").
+00012bc0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+00012bd0: 2020 2064 6566 2064 6174 6166 696c 6573     def datafiles
+00012be0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00012bf0: 2222 2220 7265 7475 726e 7320 7468 6520  """ returns the 
+00012c00: 6669 6c65 7320 7468 6174 2061 7265 2069  files that are i
+00012c10: 6e20 7468 6520 2244 6174 6120 4669 6c65  n the "Data File
+00012c20: 7322 2074 6162 6c65 206f 6620 7468 6520  s" table of the 
+00012c30: 686f 6d65 7061 6765 2222 220a 2020 2020  homepage""".    
+00012c40: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00012c50: 6765 745f 6d61 7463 6869 6e67 5f66 696c  get_matching_fil
+00012c60: 6573 2822 7461 626c 653d 3d27 4461 7461  es("table=='Data
+00012c70: 2046 696c 6573 2722 290a 0a20 2020 2040   Files'")..    @
+00012c80: 7072 6f70 6572 7479 0a20 2020 2040 6c72  property.    @lr
+00012c90: 755f 6361 6368 6528 6d61 7873 697a 653d  u_cache(maxsize=
+00012ca0: 3229 0a20 2020 2064 6566 2061 7474 6163  2).    def attac
+00012cb0: 686d 656e 7473 2873 656c 6629 202d 3e20  hments(self) -> 
+00012cc0: 4174 7461 6368 6d65 6e74 733a 0a20 2020  Attachments:.   
+00012cd0: 2020 2020 2072 6574 7572 6e20 4174 7461       return Atta
+00012ce0: 6368 6d65 6e74 7328 7365 6c66 2e5f 6669  chments(self._fi
+00012cf0: 6c65 7329 0a0a 2020 2020 4063 6c61 7373  les)..    @class
+00012d00: 6d65 7468 6f64 0a20 2020 2064 6566 2066  method.    def f
+00012d10: 726f 6d5f 6874 6d6c 2863 6c73 2c0a 2020  rom_html(cls,.  
+00012d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d30: 686f 6d65 7061 6765 5f68 746d 6c3a 2073  homepage_html: s
+00012d40: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
+00012d50: 2020 2020 2020 7572 6c3a 2073 7472 2c0a        url: str,.
+00012d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d70: 2020 6669 6c69 6e67 3a20 4669 6c69 6e67    filing: Filing
+00012d80: 293a 0a20 2020 2020 2020 2022 2222 5061  ):.        """Pa
+00012d90: 7273 6520 7468 6520 4854 4d4c 2061 6e64  rse the HTML and
+00012da0: 2063 7265 6174 6520 7468 6520 486f 6d65   create the Home
+00012db0: 7061 6765 2066 726f 6d20 6974 2222 220a  page from it""".
+00012dc0: 0a20 2020 2020 2020 2023 2049 7420 6973  .        # It is
+00012dd0: 2068 746d 6c20 736f 2075 7365 2022 6874   html so use "ht
+00012de0: 6d6c 2e70 6172 7365 7222 2028 696e 7374  ml.parser" (inst
+00012df0: 6561 6420 6f66 2022 786d 6c22 2c20 6f72  ead of "xml", or
+00012e00: 2022 6c78 6d6c 2229 0a20 2020 2020 2020   "lxml").       
+00012e10: 2073 6f75 7020 3d20 4265 6175 7469 6675   soup = Beautifu
+00012e20: 6c53 6f75 7028 686f 6d65 7061 6765 5f68  lSoup(homepage_h
+00012e30: 746d 6c2c 2022 6874 6d6c 2e70 6172 7365  tml, "html.parse
+00012e40: 7222 290a 0a20 2020 2020 2020 2023 204b  r")..        # K
+00012e50: 6565 7020 7472 6163 6b20 6f66 2074 6865  eep track of the
+00012e60: 2074 6162 6c65 7320 6173 2064 6174 6166   tables as dataf
+00012e70: 7261 6d65 732c 2073 6f20 7765 2063 616e  rames, so we can
+00012e80: 2061 7070 656e 6420 6c61 7465 720a 2020   append later.  
+00012e90: 2020 2020 2020 6466 7320 3d20 5b5d 0a0a        dfs = []..
+00012ea0: 2020 2020 2020 2020 2320 5468 6520 7461          # The ta
+00012eb0: 626c 6520 636f 6e74 6169 6e69 6e20 7468  ble containin th
+00012ec0: 6520 6174 7461 6368 6d65 6e74 730a 2020  e attachments.  
+00012ed0: 2020 2020 2020 7461 626c 6573 203d 2073        tables = s
+00012ee0: 6f75 702e 6669 6e64 5f61 6c6c 2822 7461  oup.find_all("ta
+00012ef0: 626c 6522 2c20 636c 6173 735f 3d22 7461  ble", class_="ta
+00012f00: 626c 6546 696c 6522 290a 2020 2020 2020  bleFile").      
+00012f10: 2020 666f 7220 7461 626c 6520 696e 2074    for table in t
+00012f20: 6162 6c65 733a 0a20 2020 2020 2020 2020  ables:.         
+00012f30: 2020 2073 756d 6d61 7279 203d 2074 6162     summary = tab
+00012f40: 6c65 2e61 7474 7273 2e67 6574 2822 7375  le.attrs.get("su
+00012f50: 6d6d 6172 7922 290a 2020 2020 2020 2020  mmary").        
+00012f60: 2020 2020 726f 7773 203d 2074 6162 6c65      rows = table
+00012f70: 2e66 696e 645f 616c 6c28 2274 7222 290a  .find_all("tr").
+00012f80: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
+00012f90: 6d6e 5f6e 616d 6573 203d 205b 7468 2e74  mn_names = [th.t
+00012fa0: 6578 7420 666f 7220 7468 2069 6e20 726f  ext for th in ro
+00012fb0: 7773 5b30 5d2e 6669 6e64 5f61 6c6c 2822  ws[0].find_all("
+00012fc0: 7468 2229 5d20 2b20 5b22 5572 6c22 5d0a  th")] + ["Url"].
+00012fd0: 2020 2020 2020 2020 2020 2020 7265 636f              reco
+00012fe0: 7264 7320 3d20 5b5d 0a0a 2020 2020 2020  rds = []..      
+00012ff0: 2020 2020 2020 2320 4164 6420 7468 6520        # Add the 
+00013000: 726f 7773 2066 726f 6d20 7468 6520 7461  rows from the ta
+00013010: 626c 650a 2020 2020 2020 2020 2020 2020  ble.            
+00013020: 666f 7220 726f 7720 696e 2072 6f77 735b  for row in rows[
+00013030: 313a 5d3a 0a20 2020 2020 2020 2020 2020  1:]:.           
+00013040: 2020 2020 2063 656c 6c73 203d 2072 6f77       cells = row
+00013050: 2e66 696e 645f 616c 6c28 2274 6422 290a  .find_all("td").
+00013060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013070: 6c69 6e6b 203d 2063 656c 6c73 5b32 5d2e  link = cells[2].
+00013080: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
+00013090: 2020 6365 6c6c 5f76 616c 7565 7320 3d20    cell_values = 
+000130a0: 5b63 656c 6c2e 7465 7874 2066 6f72 2063  [cell.text for c
+000130b0: 656c 6c20 696e 2063 656c 6c73 5d20 2b20  ell in cells] + 
+000130c0: 5b6c 696e 6b5b 2268 7265 6622 5d20 6966  [link["href"] if
+000130d0: 206c 696e 6b20 656c 7365 204e 6f6e 655d   link else None]
+000130e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000130f0: 2072 6563 6f72 6473 2e61 7070 656e 6428   records.append(
+00013100: 6365 6c6c 5f76 616c 7565 7329 0a0a 2020  cell_values)..  
+00013110: 2020 2020 2020 2020 2020 2320 4e6f 7720            # Now 
+00013120: 6372 6561 7465 2074 6865 2064 6174 6166  create the dataf
+00013130: 7261 6d65 0a20 2020 2020 2020 2020 2020  rame.           
+00013140: 2074 6162 6c65 5f61 735f 6466 203d 2028   table_as_df = (
+00013150: 7064 2e44 6174 6146 7261 6d65 2872 6563  pd.DataFrame(rec
+00013160: 6f72 6473 2c20 636f 6c75 6d6e 733d 636f  ords, columns=co
+00013170: 6c75 6d6e 5f6e 616d 6573 290a 2020 2020  lumn_names).    
 00013180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013190: 2020 2e66 696c 7465 7228 6669 6c69 6e67    .filter(filing
-000131a0: 5f66 696c 655f 636f 6c73 290a 2020 2020  _file_cols).    
-000131b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131c0: 2020 2020 2020 202e 6173 7369 676e 2874         .assign(t
-000131d0: 6162 6c65 3d73 756d 6d61 7279 290a 2020  able=summary).  
-000131e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131f0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00013200: 2020 2020 2020 2064 6673 2e61 7070 656e         dfs.appen
-00013210: 6428 7461 626c 655f 6173 5f64 6629 0a0a  d(table_as_df)..
-00013220: 2020 2020 2020 2020 2320 4e6f 7720 636f          # Now co
-00013230: 6e63 6174 2069 6e74 6f20 6120 7369 6e67  ncat into a sing
-00013240: 6c65 2064 6174 6166 7261 6d65 0a20 2020  le dataframe.   
-00013250: 2020 2020 2066 696c 6573 203d 2070 642e       files = pd.
-00013260: 636f 6e63 6174 2864 6673 2c20 6967 6e6f  concat(dfs, igno
-00013270: 7265 5f69 6e64 6578 3d54 7275 6529 0a0a  re_index=True)..
-00013280: 2020 2020 2020 2020 6669 6c65 725f 6469          filer_di
-00013290: 7673 203d 2073 6f75 702e 6669 6e64 5f61  vs = soup.find_a
-000132a0: 6c6c 2822 6469 7622 2c20 6964 3d22 6669  ll("div", id="fi
-000132b0: 6c65 7244 6976 2229 0a20 2020 2020 2020  lerDiv").       
-000132c0: 2066 696c 6572 5f69 6e66 6f73 203d 205b   filer_infos = [
-000132d0: 5d0a 2020 2020 2020 2020 666f 7220 6669  ].        for fi
-000132e0: 6c65 725f 6469 7620 696e 2066 696c 6572  ler_div in filer
-000132f0: 5f64 6976 733a 0a0a 2020 2020 2020 2020  _divs:..        
-00013300: 2020 2020 2320 4765 7420 7468 6520 636f      # Get the co
-00013310: 6d70 616e 7920 6e61 6d65 0a20 2020 2020  mpany name.     
-00013320: 2020 2020 2020 2063 6f6d 7061 6e79 5f69         company_i
-00013330: 6e66 6f5f 6469 7620 3d20 6669 6c65 725f  nfo_div = filer_
-00013340: 6469 762e 6669 6e64 2822 6469 7622 2c20  div.find("div", 
-00013350: 636c 6173 735f 3d22 636f 6d70 616e 7949  class_="companyI
-00013360: 6e66 6f22 290a 0a20 2020 2020 2020 2020  nfo")..         
-00013370: 2020 2063 6f6d 7061 6e79 5f6e 616d 655f     company_name_
-00013380: 7370 616e 203d 2063 6f6d 7061 6e79 5f69  span = company_i
-00013390: 6e66 6f5f 6469 762e 6669 6e64 2822 7370  nfo_div.find("sp
-000133a0: 616e 222c 2063 6c61 7373 5f3d 2263 6f6d  an", class_="com
-000133b0: 7061 6e79 4e61 6d65 2229 0a20 2020 2020  panyName").     
-000133c0: 2020 2020 2020 2063 6f6d 7061 6e79 5f6e         company_n
-000133d0: 616d 6520 3d20 2872 652e 7375 6228 225c  ame = (re.sub("\
-000133e0: 6e22 2c20 2222 2c20 636f 6d70 616e 795f  n", "", company_
-000133f0: 6e61 6d65 5f73 7061 6e2e 7465 7874 2e73  name_span.text.s
-00013400: 7472 6970 2829 290a 2020 2020 2020 2020  trip()).        
+00013190: 2020 2020 2020 202e 6669 6c74 6572 2866         .filter(f
+000131a0: 696c 696e 675f 6669 6c65 5f63 6f6c 7329  iling_file_cols)
+000131b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000131c0: 2020 2020 2020 2020 2020 2020 2e61 7373              .ass
+000131d0: 6967 6e28 7461 626c 653d 7375 6d6d 6172  ign(table=summar
+000131e0: 7929 0a20 2020 2020 2020 2020 2020 2020  y).             
+000131f0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00013200: 2020 2020 2020 2020 2020 2020 6466 732e              dfs.
+00013210: 6170 7065 6e64 2874 6162 6c65 5f61 735f  append(table_as_
+00013220: 6466 290a 0a20 2020 2020 2020 2023 204e  df)..        # N
+00013230: 6f77 2063 6f6e 6361 7420 696e 746f 2061  ow concat into a
+00013240: 2073 696e 676c 6520 6461 7461 6672 616d   single datafram
+00013250: 650a 2020 2020 2020 2020 6669 6c65 7320  e.        files 
+00013260: 3d20 7064 2e63 6f6e 6361 7428 6466 732c  = pd.concat(dfs,
+00013270: 2069 676e 6f72 655f 696e 6465 783d 5472   ignore_index=Tr
+00013280: 7565 290a 0a20 2020 2020 2020 2066 696c  ue)..        fil
+00013290: 6572 5f64 6976 7320 3d20 736f 7570 2e66  er_divs = soup.f
+000132a0: 696e 645f 616c 6c28 2264 6976 222c 2069  ind_all("div", i
+000132b0: 643d 2266 696c 6572 4469 7622 290a 2020  d="filerDiv").  
+000132c0: 2020 2020 2020 6669 6c65 725f 696e 666f        filer_info
+000132d0: 7320 3d20 5b5d 0a20 2020 2020 2020 2066  s = [].        f
+000132e0: 6f72 2066 696c 6572 5f64 6976 2069 6e20  or filer_div in 
+000132f0: 6669 6c65 725f 6469 7673 3a0a 0a20 2020  filer_divs:..   
+00013300: 2020 2020 2020 2020 2023 2047 6574 2074           # Get t
+00013310: 6865 2063 6f6d 7061 6e79 206e 616d 650a  he company name.
+00013320: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
+00013330: 616e 795f 696e 666f 5f64 6976 203d 2066  any_info_div = f
+00013340: 696c 6572 5f64 6976 2e66 696e 6428 2264  iler_div.find("d
+00013350: 6976 222c 2063 6c61 7373 5f3d 2263 6f6d  iv", class_="com
+00013360: 7061 6e79 496e 666f 2229 0a0a 2020 2020  panyInfo")..    
+00013370: 2020 2020 2020 2020 636f 6d70 616e 795f          company_
+00013380: 6e61 6d65 5f73 7061 6e20 3d20 636f 6d70  name_span = comp
+00013390: 616e 795f 696e 666f 5f64 6976 2e66 696e  any_info_div.fin
+000133a0: 6428 2273 7061 6e22 2c20 636c 6173 735f  d("span", class_
+000133b0: 3d22 636f 6d70 616e 794e 616d 6522 290a  ="companyName").
+000133c0: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
+000133d0: 616e 795f 6e61 6d65 203d 2028 7265 2e73  any_name = (re.s
+000133e0: 7562 2822 5c6e 222c 2022 222c 2063 6f6d  ub("\n", "", com
+000133f0: 7061 6e79 5f6e 616d 655f 7370 616e 2e74  pany_name_span.t
+00013400: 6578 742e 7374 7269 7028 2929 0a20 2020  ext.strip()).   
 00013410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013420: 2020 2020 2e72 6570 6c61 6365 2822 2873      .replace("(s
-00013430: 6565 2061 6c6c 2063 6f6d 7061 6e79 2066  ee all company f
-00013440: 696c 696e 6773 2922 2c20 2222 292e 7273  ilings)", "").rs
-00013450: 7472 6970 2829 0a20 2020 2020 2020 2020  trip().         
+00013420: 2020 2020 2020 2020 202e 7265 706c 6163           .replac
+00013430: 6528 2228 7365 6520 616c 6c20 636f 6d70  e("(see all comp
+00013440: 616e 7920 6669 6c69 6e67 7329 222c 2022  any filings)", "
+00013450: 2229 2e72 7374 7269 7028 290a 2020 2020  ").rstrip().    
 00013460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013470: 2020 2069 6620 636f 6d70 616e 795f 6e61     if company_na
-00013480: 6d65 5f73 7061 6e20 656c 7365 2022 2229  me_span else "")
-00013490: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-000134a0: 4765 7420 7468 6520 6964 656e 7469 6669  Get the identifi
-000134b0: 6361 7469 6f6e 2069 6e66 6f72 6d61 7469  cation informati
-000134c0: 6f6e 0a20 2020 2020 2020 2020 2020 2069  on.            i
-000134d0: 6465 6e74 5f69 6e66 6f5f 6469 7620 3d20  dent_info_div = 
-000134e0: 636f 6d70 616e 795f 696e 666f 5f64 6976  company_info_div
-000134f0: 2e66 696e 6428 2270 222c 2063 6c61 7373  .find("p", class
-00013500: 5f3d 2269 6465 6e74 496e 666f 2229 0a0a  _="identInfo")..
-00013510: 2020 2020 2020 2020 2020 2020 2320 5265              # Re
-00013520: 6c61 6365 203c 6272 3e20 7769 7468 206e  lace <br> with n
-00013530: 6577 6c69 6e65 730a 2020 2020 2020 2020  ewlines.        
-00013540: 2020 2020 666f 7220 6272 2069 6e20 6964      for br in id
-00013550: 656e 745f 696e 666f 5f64 6976 2e66 696e  ent_info_div.fin
-00013560: 645f 616c 6c28 2262 7222 293a 0a20 2020  d_all("br"):.   
-00013570: 2020 2020 2020 2020 2020 2020 2062 722e               br.
-00013580: 7265 706c 6163 655f 7769 7468 2822 5c6e  replace_with("\n
-00013590: 2229 0a0a 2020 2020 2020 2020 2020 2020  ")..            
-000135a0: 6964 656e 7469 6669 6361 7469 6f6e 203d  identification =
-000135b0: 2069 6465 6e74 5f69 6e66 6f5f 6469 762e   ident_info_div.
-000135c0: 7465 7874 0a0a 2020 2020 2020 2020 2020  text..          
-000135d0: 2020 2320 4765 7420 7468 6520 6d61 696c    # Get the mail
-000135e0: 696e 6720 696e 666f 726d 6174 696f 6e0a  ing information.
-000135f0: 2020 2020 2020 2020 2020 2020 6d61 696c              mail
-00013600: 6572 5f64 6976 7320 3d20 6669 6c65 725f  er_divs = filer_
-00013610: 6469 762e 6669 6e64 5f61 6c6c 2822 6469  div.find_all("di
-00013620: 7622 2c20 636c 6173 735f 3d22 6d61 696c  v", class_="mail
-00013630: 6572 2229 0a20 2020 2020 2020 2020 2020  er").           
-00013640: 2023 2046 6f72 2065 6163 6820 6d61 696c   # For each mail
-00013650: 6564 5f64 6976 2e74 6578 7420 7265 6d6f  ed_div.text remo
-00013660: 7665 206d 7574 6970 6c65 2073 7061 6365  ve mutiple space
-00013670: 7320 6166 7465 7220 6120 6e65 776c 696e  s after a newlin
-00013680: 650a 0a20 2020 2020 2020 2020 2020 2061  e..            a
-00013690: 6464 7265 7373 6573 203d 205b 7265 2e73  ddresses = [re.s
-000136a0: 7562 2872 275c 6e5c 732b 272c 2027 5c6e  ub(r'\n\s+', '\n
-000136b0: 272c 206d 6169 6c65 725f 6469 762e 7465  ', mailer_div.te
-000136c0: 7874 2e73 7472 6970 2829 290a 2020 2020  xt.strip()).    
-000136d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000136e0: 2020 2020 2066 6f72 206d 6169 6c65 725f       for mailer_
-000136f0: 6469 7620 696e 206d 6169 6c65 725f 6469  div in mailer_di
-00013700: 7673 5d0a 0a20 2020 2020 2020 2020 2020  vs]..           
-00013710: 2023 2043 7265 6174 6520 7468 6520 6669   # Create the fi
-00013720: 6c65 7220 696e 666f 0a20 2020 2020 2020  ler info.       
-00013730: 2020 2020 2066 696c 6572 5f69 6e66 6f20       filer_info 
-00013740: 3d20 4669 6c65 7249 6e66 6f28 636f 6d70  = FilerInfo(comp
-00013750: 616e 795f 6e61 6d65 3d63 6f6d 7061 6e79  any_name=company
-00013760: 5f6e 616d 652c 2069 6465 6e74 6966 6963  _name, identific
-00013770: 6174 696f 6e3d 6964 656e 7469 6669 6361  ation=identifica
-00013780: 7469 6f6e 2c20 6164 6472 6573 7365 733d  tion, addresses=
-00013790: 6164 6472 6573 7365 7329 0a0a 2020 2020  addresses)..    
-000137a0: 2020 2020 2020 2020 6669 6c65 725f 696e          filer_in
-000137b0: 666f 732e 6170 7065 6e64 2866 696c 6572  fos.append(filer
-000137c0: 5f69 6e66 6f29 0a0a 2020 2020 2020 2020  _info)..        
-000137d0: 7265 7475 726e 2063 6c73 2866 696c 6573  return cls(files
-000137e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000137f0: 2020 2020 2075 726c 3d75 726c 2c0a 2020       url=url,.  
-00013800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013810: 2066 696c 696e 673d 6669 6c69 6e67 2c0a   filing=filing,.
-00013820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013830: 2020 2066 696c 6572 5f69 6e66 6f73 3d66     filer_infos=f
-00013840: 696c 6572 5f69 6e66 6f73 290a 0a20 2020  iler_infos)..   
-00013850: 2064 6566 205f 5f73 7472 5f5f 2873 656c   def __str__(sel
-00013860: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-00013870: 726e 2066 2248 6f6d 6570 6167 6520 666f  rn f"Homepage fo
-00013880: 7220 7b73 656c 662e 6465 7363 7269 7074  r {self.descript
-00013890: 696f 6e7d 220a 0a20 2020 2064 6566 205f  ion}"..    def _
-000138a0: 5f72 6570 725f 5f28 7365 6c66 293a 0a20  _repr__(self):. 
-000138b0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-000138c0: 7072 5f72 6963 6828 7365 6c66 2e5f 5f72  pr_rich(self.__r
-000138d0: 6963 685f 5f28 2929 0a0a 2020 2020 6465  ich__())..    de
-000138e0: 6620 5f5f 7269 6368 5f5f 2873 656c 6629  f __rich__(self)
-000138f0: 3a0a 0a20 2020 2020 2020 2072 6574 7572  :..        retur
-00013900: 6e20 5061 6e65 6c28 0a20 2020 2020 2020  n Panel(.       
-00013910: 2020 2020 2047 726f 7570 280a 2020 2020       Group(.    
-00013920: 2020 2020 2020 2020 2020 2020 6466 5f74              df_t
-00013930: 6f5f 7269 6368 5f74 6162 6c65 2873 656c  o_rich_table(sel
-00013940: 662e 6669 6c69 6e67 2e73 756d 6d61 7279  f.filing.summary
-00013950: 2829 2c20 696e 6465 785f 6e61 6d65 3d22  (), index_name="
-00013960: 4163 6365 7373 696f 6e20 4e75 6d62 6572  Accession Number
-00013970: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-00013980: 2020 2020 4772 6f75 7028 5465 7874 2822      Group(Text("
-00013990: 446f 6375 6d65 6e74 7322 2c20 7374 796c  Documents", styl
-000139a0: 653d 2262 6f6c 6422 292c 0a20 2020 2020  e="bold"),.     
+00013470: 2020 2020 2020 2020 6966 2063 6f6d 7061          if compa
+00013480: 6e79 5f6e 616d 655f 7370 616e 2065 6c73  ny_name_span els
+00013490: 6520 2222 290a 0a20 2020 2020 2020 2020  e "")..         
+000134a0: 2020 2023 2047 6574 2074 6865 2069 6465     # Get the ide
+000134b0: 6e74 6966 6963 6174 696f 6e20 696e 666f  ntification info
+000134c0: 726d 6174 696f 6e0a 2020 2020 2020 2020  rmation.        
+000134d0: 2020 2020 6964 656e 745f 696e 666f 5f64      ident_info_d
+000134e0: 6976 203d 2063 6f6d 7061 6e79 5f69 6e66  iv = company_inf
+000134f0: 6f5f 6469 762e 6669 6e64 2822 7022 2c20  o_div.find("p", 
+00013500: 636c 6173 735f 3d22 6964 656e 7449 6e66  class_="identInf
+00013510: 6f22 290a 0a20 2020 2020 2020 2020 2020  o")..           
+00013520: 2023 2052 656c 6163 6520 3c62 723e 2077   # Relace <br> w
+00013530: 6974 6820 6e65 776c 696e 6573 0a20 2020  ith newlines.   
+00013540: 2020 2020 2020 2020 2066 6f72 2062 7220           for br 
+00013550: 696e 2069 6465 6e74 5f69 6e66 6f5f 6469  in ident_info_di
+00013560: 762e 6669 6e64 5f61 6c6c 2822 6272 2229  v.find_all("br")
+00013570: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00013580: 2020 6272 2e72 6570 6c61 6365 5f77 6974    br.replace_wit
+00013590: 6828 225c 6e22 290a 0a20 2020 2020 2020  h("\n")..       
+000135a0: 2020 2020 2069 6465 6e74 6966 6963 6174       identificat
+000135b0: 696f 6e20 3d20 6964 656e 745f 696e 666f  ion = ident_info
+000135c0: 5f64 6976 2e74 6578 740a 0a20 2020 2020  _div.text..     
+000135d0: 2020 2020 2020 2023 2047 6574 2074 6865         # Get the
+000135e0: 206d 6169 6c69 6e67 2069 6e66 6f72 6d61   mailing informa
+000135f0: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+00013600: 206d 6169 6c65 725f 6469 7673 203d 2066   mailer_divs = f
+00013610: 696c 6572 5f64 6976 2e66 696e 645f 616c  iler_div.find_al
+00013620: 6c28 2264 6976 222c 2063 6c61 7373 5f3d  l("div", class_=
+00013630: 226d 6169 6c65 7222 290a 2020 2020 2020  "mailer").      
+00013640: 2020 2020 2020 2320 466f 7220 6561 6368        # For each
+00013650: 206d 6169 6c65 645f 6469 762e 7465 7874   mailed_div.text
+00013660: 2072 656d 6f76 6520 6d75 7469 706c 6520   remove mutiple 
+00013670: 7370 6163 6573 2061 6674 6572 2061 206e  spaces after a n
+00013680: 6577 6c69 6e65 0a0a 2020 2020 2020 2020  ewline..        
+00013690: 2020 2020 6164 6472 6573 7365 7320 3d20      addresses = 
+000136a0: 5b72 652e 7375 6228 7227 5c6e 5c73 2b27  [re.sub(r'\n\s+'
+000136b0: 2c20 275c 6e27 2c20 6d61 696c 6572 5f64  , '\n', mailer_d
+000136c0: 6976 2e74 6578 742e 7374 7269 7028 2929  iv.text.strip())
+000136d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000136e0: 2020 2020 2020 2020 2020 666f 7220 6d61            for ma
+000136f0: 696c 6572 5f64 6976 2069 6e20 6d61 696c  iler_div in mail
+00013700: 6572 5f64 6976 735d 0a0a 2020 2020 2020  er_divs]..      
+00013710: 2020 2020 2020 2320 4372 6561 7465 2074        # Create t
+00013720: 6865 2066 696c 6572 2069 6e66 6f0a 2020  he filer info.  
+00013730: 2020 2020 2020 2020 2020 6669 6c65 725f            filer_
+00013740: 696e 666f 203d 2046 696c 6572 496e 666f  info = FilerInfo
+00013750: 2863 6f6d 7061 6e79 5f6e 616d 653d 636f  (company_name=co
+00013760: 6d70 616e 795f 6e61 6d65 2c20 6964 656e  mpany_name, iden
+00013770: 7469 6669 6361 7469 6f6e 3d69 6465 6e74  tification=ident
+00013780: 6966 6963 6174 696f 6e2c 2061 6464 7265  ification, addre
+00013790: 7373 6573 3d61 6464 7265 7373 6573 290a  sses=addresses).
+000137a0: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
+000137b0: 6572 5f69 6e66 6f73 2e61 7070 656e 6428  er_infos.append(
+000137c0: 6669 6c65 725f 696e 666f 290a 0a20 2020  filer_info)..   
+000137d0: 2020 2020 2072 6574 7572 6e20 636c 7328       return cls(
+000137e0: 6669 6c65 732c 0a20 2020 2020 2020 2020  files,.         
+000137f0: 2020 2020 2020 2020 2020 7572 6c3d 7572            url=ur
+00013800: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
+00013810: 2020 2020 2020 6669 6c69 6e67 3d66 696c        filing=fil
+00013820: 696e 672c 0a20 2020 2020 2020 2020 2020  ing,.           
+00013830: 2020 2020 2020 2020 6669 6c65 725f 696e          filer_in
+00013840: 666f 733d 6669 6c65 725f 696e 666f 7329  fos=filer_infos)
+00013850: 0a0a 2020 2020 6465 6620 5f5f 7374 725f  ..    def __str_
+00013860: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
+00013870: 2072 6574 7572 6e20 6622 486f 6d65 7061   return f"Homepa
+00013880: 6765 2066 6f72 207b 7365 6c66 2e64 6573  ge for {self.des
+00013890: 6372 6970 7469 6f6e 7d22 0a0a 2020 2020  cription}"..    
+000138a0: 6465 6620 5f5f 7265 7072 5f5f 2873 656c  def __repr__(sel
+000138b0: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
+000138c0: 726e 2072 6570 725f 7269 6368 2873 656c  rn repr_rich(sel
+000138d0: 662e 5f5f 7269 6368 5f5f 2829 290a 0a20  f.__rich__()).. 
+000138e0: 2020 2064 6566 205f 5f72 6963 685f 5f28     def __rich__(
+000138f0: 7365 6c66 293a 0a0a 2020 2020 2020 2020  self):..        
+00013900: 7265 7475 726e 2050 616e 656c 280a 2020  return Panel(.  
+00013910: 2020 2020 2020 2020 2020 4772 6f75 7028            Group(
+00013920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013930: 2064 665f 746f 5f72 6963 685f 7461 626c   df_to_rich_tabl
+00013940: 6528 7365 6c66 2e66 696c 696e 672e 7375  e(self.filing.su
+00013950: 6d6d 6172 7928 292c 2069 6e64 6578 5f6e  mmary(), index_n
+00013960: 616d 653d 2241 6363 6573 7369 6f6e 204e  ame="Accession N
+00013970: 756d 6265 7222 292c 0a20 2020 2020 2020  umber"),.       
+00013980: 2020 2020 2020 2020 2047 726f 7570 2854           Group(T
+00013990: 6578 7428 2244 6f63 756d 656e 7473 222c  ext("Documents",
+000139a0: 2073 7479 6c65 3d22 626f 6c64 2229 2c0a   style="bold"),.
 000139b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139c0: 2064 665f 746f 5f72 6963 685f 7461 626c   df_to_rich_tabl
-000139d0: 6528 7375 6d6d 6172 697a 655f 6669 6c65  e(summarize_file
-000139e0: 7328 7365 6c66 2e64 6f63 756d 656e 7473  s(self.documents
-000139f0: 292c 2069 6e64 6578 5f6e 616d 653d 2253  ), index_name="S
-00013a00: 6571 2229 0a20 2020 2020 2020 2020 2020  eq").           
-00013a10: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
-00013a20: 2020 2020 2020 2020 2020 2020 2020 4772                Gr
-00013a30: 6f75 7028 5465 7874 2822 4461 7461 6669  oup(Text("Datafi
-00013a40: 6c65 7322 2c20 7374 796c 653d 2262 6f6c  les", style="bol
-00013a50: 6422 292c 0a20 2020 2020 2020 2020 2020  d"),.           
-00013a60: 2020 2020 2020 2020 2020 2064 665f 746f             df_to
-00013a70: 5f72 6963 685f 7461 626c 6528 7375 6d6d  _rich_table(summ
-00013a80: 6172 697a 655f 6669 6c65 7328 7365 6c66  arize_files(self
-00013a90: 2e64 6174 6166 696c 6573 292c 2069 6e64  .datafiles), ind
-00013aa0: 6578 5f6e 616d 653d 2253 6571 2229 2c0a  ex_name="Seq"),.
-00013ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ac0: 2020 2020 2020 2920 6966 2073 656c 662e        ) if self.
-00013ad0: 6461 7461 6669 6c65 7320 6973 206e 6f74  datafiles is not
-00013ae0: 204e 6f6e 6520 656c 7365 2054 6578 7428   None else Text(
-00013af0: 2222 292c 0a20 2020 2020 2020 2020 2020  ""),.           
-00013b00: 2020 2020 2047 726f 7570 280a 2020 2020       Group(.    
-00013b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b20: 2a5b 6669 6c65 725f 696e 666f 2e5f 5f72  *[filer_info.__r
-00013b30: 6963 685f 5f28 2920 666f 7220 6669 6c65  ich__() for file
-00013b40: 725f 696e 666f 2069 6e20 7365 6c66 2e66  r_info in self.f
-00013b50: 696c 6572 5f69 6e66 6f73 5d0a 2020 2020  iler_infos].    
-00013b60: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00013b70: 2020 2020 2020 2020 2020 2029 2c20 7469             ), ti
-00013b80: 746c 653d 6622 466f 726d 207b 7365 6c66  tle=f"Form {self
-00013b90: 2e66 696c 696e 672e 666f 726d 7d22 290a  .filing.form}").
-00013ba0: 0a0a 6465 6620 7375 6d6d 6172 697a 655f  ..def summarize_
-00013bb0: 6669 6c65 7328 6461 7461 3a20 7064 2e44  files(data: pd.D
-00013bc0: 6174 6146 7261 6d65 2920 2d3e 2070 642e  ataFrame) -> pd.
-00013bd0: 4461 7461 4672 616d 653a 0a20 2020 2072  DataFrame:.    r
-00013be0: 6574 7572 6e20 2864 6174 610a 2020 2020  eturn (data.    
-00013bf0: 2020 2020 2020 2020 2e66 696c 7465 7228          .filter(
-00013c00: 5b22 5365 7122 2c20 2244 6f63 756d 656e  ["Seq", "Documen
-00013c10: 7422 2c20 2244 6573 6372 6970 7469 6f6e  t", "Description
-00013c20: 222c 2022 5369 7a65 225d 290a 2020 2020  ", "Size"]).    
-00013c30: 2020 2020 2020 2020 2e61 7373 6967 6e28          .assign(
-00013c40: 5369 7a65 3d64 6174 612e 5369 7a65 2e61  Size=data.Size.a
-00013c50: 7070 6c79 2864 6973 706c 6179 5f73 697a  pply(display_siz
-00013c60: 6529 290a 2020 2020 2020 2020 2020 2020  e)).            
-00013c70: 2e73 6574 5f69 6e64 6578 2822 5365 7122  .set_index("Seq"
-00013c80: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
-00013c90: 0a0a 406c 7275 5f63 6163 6865 286d 6178  ..@lru_cache(max
-00013ca0: 7369 7a65 3d31 3629 0a64 6566 2067 6574  size=16).def get
-00013cb0: 5f62 795f 6163 6365 7373 696f 6e5f 6e75  _by_accession_nu
-00013cc0: 6d62 6572 2861 6363 6573 7369 6f6e 5f6e  mber(accession_n
-00013cd0: 756d 6265 723a 2073 7472 293a 0a20 2020  umber: str):.   
-00013ce0: 2022 2222 4669 6e64 2074 6865 2066 696c   """Find the fil
-00013cf0: 696e 6720 7573 696e 6720 7468 6520 6163  ing using the ac
-00013d00: 6365 7373 696f 6e20 6e75 6d62 6572 2222  cession number""
-00013d10: 220a 2020 2020 6173 7365 7274 2072 652e  ".    assert re.
-00013d20: 6d61 7463 6828 7222 5c64 7b31 307d 2d5c  match(r"\d{10}-\
-00013d30: 647b 327d 2d5c 647b 367d 222c 2061 6363  d{2}-\d{6}", acc
-00013d40: 6573 7369 6f6e 5f6e 756d 6265 7229 2c20  ession_number), 
-00013d50: 5c0a 2020 2020 2020 2020 6622 7b61 6363  \.        f"{acc
-00013d60: 6573 7369 6f6e 5f6e 756d 6265 727d 2069  ession_number} i
-00013d70: 7320 6e6f 7420 6120 7661 6c69 6420 6163  s not a valid ac
-00013d80: 6365 7373 696f 6e20 6e75 6d62 6572 202e  cession number .
-00013d90: 2e20 7368 6f75 6c64 2062 6520 3130 6469  . should be 10di
-00013da0: 6769 7473 2d32 6469 6769 7473 2d36 6469  gits-2digits-6di
-00013db0: 6769 7473 220a 2020 2020 7965 6172 203d  gits".    year =
-00013dc0: 2069 6e74 2822 3139 2220 2b20 6163 6365   int("19" + acce
-00013dd0: 7373 696f 6e5f 6e75 6d62 6572 5b31 313a  ssion_number[11:
-00013de0: 3133 5d29 2069 6620 6163 6365 7373 696f  13]) if accessio
-00013df0: 6e5f 6e75 6d62 6572 5b31 315d 203d 3d20  n_number[11] == 
-00013e00: 3920 656c 7365 2069 6e74 2822 3230 2220  9 else int("20" 
-00013e10: 2b20 6163 6365 7373 696f 6e5f 6e75 6d62  + accession_numb
-00013e20: 6572 5b31 313a 3133 5d29 0a0a 2020 2020  er[11:13])..    
-00013e30: 6966 2079 6561 7220 3d3d 2064 6174 6574  if year == datet
-00013e40: 696d 652e 6e6f 7728 292e 7965 6172 3a0a  ime.now().year:.
-00013e50: 2020 2020 2020 2020 2320 466f 7220 7468          # For th
-00013e60: 6520 6375 7272 656e 7420 7965 6172 2063  e current year c
-00013e70: 7265 6174 6520 6120 7261 6e67 6520 6f66  reate a range of
-00013e80: 2071 7561 7274 6572 7320 746f 2073 6561   quarters to sea
-00013e90: 7263 6820 6672 6f6d 2031 2075 7020 746f  rch from 1 up to
-00013ea0: 2074 6865 2063 7572 7265 6e74 2071 7561   the current qua
-00013eb0: 7274 6572 206f 6620 7468 6520 7965 6172  rter of the year
-00013ec0: 0a20 2020 2020 2020 2063 7572 7265 6e74  .        current
-00013ed0: 5f71 7561 7274 6572 203d 2028 6461 7465  _quarter = (date
-00013ee0: 7469 6d65 2e6e 6f77 2829 2e6d 6f6e 7468  time.now().month
-00013ef0: 202d 2031 2920 2f2f 2033 202b 2031 0a20   - 1) // 3 + 1. 
-00013f00: 2020 2020 2020 2071 7561 7274 6572 7320         quarters 
-00013f10: 3d20 7261 6e67 6528 312c 2063 7572 7265  = range(1, curre
-00013f20: 6e74 5f71 7561 7274 6572 202b 2031 290a  nt_quarter + 1).
-00013f30: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00013f40: 2020 2320 5365 6172 6368 2061 6c6c 2071    # Search all q
-00013f50: 7561 7274 6572 730a 2020 2020 2020 2020  uarters.        
-00013f60: 7175 6172 7465 7273 203d 2072 616e 6765  quarters = range
-00013f70: 2831 2c20 3529 0a0a 2020 2020 7769 7468  (1, 5)..    with
-00013f80: 2053 7461 7475 7328 6622 5b62 6f6c 6420   Status(f"[bold 
-00013f90: 6465 6570 5f73 6b79 5f62 6c75 6531 5d53  deep_sky_blue1]S
-00013fa0: 6561 7263 6869 6e67 2066 6f72 2066 696c  earching for fil
-00013fb0: 696e 6720 7b61 6363 6573 7369 6f6e 5f6e  ing {accession_n
-00013fc0: 756d 6265 727d 2e2e 2e22 2c20 7370 696e  umber}...", spin
-00013fd0: 6e65 723d 2264 6f74 7332 2229 3a0a 2020  ner="dots2"):.  
-00013fe0: 2020 2020 2020 666f 7220 7175 6172 7465        for quarte
-00013ff0: 7220 696e 2071 7561 7274 6572 733a 0a20  r in quarters:. 
-00014000: 2020 2020 2020 2020 2020 2066 696c 696e             filin
-00014010: 6773 203d 205f 6765 745f 6361 6368 6564  gs = _get_cached
-00014020: 5f66 696c 696e 6773 2879 6561 723d 7965  _filings(year=ye
-00014030: 6172 2c20 7175 6172 7465 723d 7175 6172  ar, quarter=quar
-00014040: 7465 7229 0a20 2020 2020 2020 2020 2020  ter).           
-00014050: 2069 6620 6669 6c69 6e67 733a 0a20 2020   if filings:.   
-00014060: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-00014070: 696e 6720 3d20 6669 6c69 6e67 732e 6765  ing = filings.ge
-00014080: 7428 6163 6365 7373 696f 6e5f 6e75 6d62  t(accession_numb
-00014090: 6572 290a 2020 2020 2020 2020 2020 2020  er).            
-000140a0: 2020 2020 6966 2066 696c 696e 673a 0a20      if filing:. 
-000140b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140c0: 2020 2072 6574 7572 6e20 6669 6c69 6e67     return filing
-000140d0: 0a20 2020 2023 2057 6520 6861 7665 6e27  .    # We haven'
-000140e0: 7420 666f 756e 6420 7468 6520 6669 6c69  t found the fili
-000140f0: 6e67 206e 6f72 6d61 6c6c 7920 736f 2063  ng normally so c
-00014100: 6865 636b 2074 6865 206d 6f73 7420 7265  heck the most re
-00014110: 6365 6e74 2053 4543 2066 696c 696e 6773  cent SEC filings
-00014120: 0a20 2020 2023 2043 6865 636b 2069 6620  .    # Check if 
-00014130: 7468 6520 7965 6172 2069 7320 7468 6520  the year is the 
-00014140: 6375 7272 656e 7420 7965 6172 0a20 2020  current year.   
-00014150: 2069 6620 7965 6172 203d 3d20 6461 7465   if year == date
-00014160: 7469 6d65 2e6e 6f77 2829 2e79 6561 723a  time.now().year:
-00014170: 0a20 2020 2020 2020 2023 2047 6574 2074  .        # Get t
-00014180: 6865 206d 6f73 7420 7265 6365 6e74 2066  he most recent f
-00014190: 696c 696e 6773 0a20 2020 2020 2020 2066  ilings.        f
-000141a0: 696c 696e 6773 203d 2067 6574 5f63 7572  ilings = get_cur
-000141b0: 7265 6e74 5f66 696c 696e 6773 2829 0a20  rent_filings(). 
-000141c0: 2020 2020 2020 2072 6574 7572 6e20 6669         return fi
-000141d0: 6c69 6e67 732e 6765 7428 6163 6365 7373  lings.get(access
-000141e0: 696f 6e5f 6e75 6d62 6572 290a 0a0a 6465  ion_number)...de
-000141f0: 6620 666f 726d 5f77 6974 685f 616d 656e  f form_with_amen
-00014200: 646d 656e 7473 282a 666f 726d 733a 2073  dments(*forms: s
-00014210: 7472 293a 0a20 2020 2072 6574 7572 6e20  tr):.    return 
-00014220: 6c69 7374 2866 6f72 6d73 2920 2b20 5b66  list(forms) + [f
-00014230: 227b 667d 2f41 2220 666f 7220 6620 696e  "{f}/A" for f in
-00014240: 2066 6f72 6d73 5d0a 0a0a 6261 7263 6861   forms]...barcha
-00014250: 7274 203d 2027 5c55 3030 3031 4634 4341  rt = '\U0001F4CA
-00014260: 270a 7469 636b 6574 203d 2027 5c55 3030  '.ticket = '\U00
-00014270: 3031 4633 4142 270a 7061 6765 5f66 6163  01F3AB'.page_fac
-00014280: 696e 675f 7570 203d 2027 5c55 3030 3031  ing_up = '\U0001
-00014290: 4634 4334 270a 636c 6173 7369 6361 6c5f  F4C4'.classical_
-000142a0: 6275 696c 6469 6e67 203d 2027 5c55 3030  building = '\U00
-000142b0: 3031 4633 4442 270a 0a0a 6465 6620 756e  01F3DB'...def un
-000142c0: 6963 6f64 655f 666f 725f 666f 726d 2866  icode_for_form(f
-000142d0: 6f72 6d3a 2073 7472 293a 0a20 2020 2069  orm: str):.    i
-000142e0: 6620 666f 726d 2069 6e20 5b27 3130 2d4b  f form in ['10-K
-000142f0: 272c 2027 3130 2d51 272c 2027 3130 2d4b  ', '10-Q', '10-K
-00014300: 2f41 272c 2027 3130 2d51 2f41 272c 2027  /A', '10-Q/A', '
-00014310: 362d 4b27 2c20 2736 2d4b 2f41 275d 3a0a  6-K', '6-K/A']:.
-00014320: 2020 2020 2020 2020 7265 7475 726e 2062          return b
-00014330: 6172 6368 6172 740a 2020 2020 656c 6966  archart.    elif
-00014340: 2066 6f72 6d20 696e 205b 2733 272c 2027   form in ['3', '
-00014350: 3427 2c20 2735 272c 2027 332f 4127 2c20  4', '5', '3/A', 
-00014360: 2734 2f41 272c 2027 352f 4127 5d3a 0a20  '4/A', '5/A']:. 
-00014370: 2020 2020 2020 2072 6574 7572 6e20 7469         return ti
-00014380: 636b 6574 0a20 2020 2065 6c69 6620 666f  cket.    elif fo
-00014390: 726d 2069 6e20 5b27 4d41 2d49 272c 2027  rm in ['MA-I', '
-000143a0: 4d41 2d49 2f41 272c 2027 4d41 272c 2027  MA-I/A', 'MA', '
-000143b0: 4d41 2f41 275d 3a0a 2020 2020 2020 2020  MA/A']:.        
-000143c0: 7265 7475 726e 2063 6c61 7373 6963 616c  return classical
-000143d0: 5f62 7569 6c64 696e 670a 2020 2020 7265  _building.    re
-000143e0: 7475 726e 2070 6167 655f 6661 6369 6e67  turn page_facing
-000143f0: 5f75 700a                                _up.
+000139c0: 2020 2020 2020 6466 5f74 6f5f 7269 6368        df_to_rich
+000139d0: 5f74 6162 6c65 2873 756d 6d61 7269 7a65  _table(summarize
+000139e0: 5f66 696c 6573 2873 656c 662e 646f 6375  _files(self.docu
+000139f0: 6d65 6e74 7329 2c20 696e 6465 785f 6e61  ments), index_na
+00013a00: 6d65 3d22 5365 7122 290a 2020 2020 2020  me="Seq").      
+00013a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a20: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00013a30: 2020 2047 726f 7570 2854 6578 7428 2244     Group(Text("D
+00013a40: 6174 6166 696c 6573 222c 2073 7479 6c65  atafiles", style
+00013a50: 3d22 626f 6c64 2229 2c0a 2020 2020 2020  ="bold"),.      
+00013a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a70: 6466 5f74 6f5f 7269 6368 5f74 6162 6c65  df_to_rich_table
+00013a80: 2873 756d 6d61 7269 7a65 5f66 696c 6573  (summarize_files
+00013a90: 2873 656c 662e 6461 7461 6669 6c65 7329  (self.datafiles)
+00013aa0: 2c20 696e 6465 785f 6e61 6d65 3d22 5365  , index_name="Se
+00013ab0: 7122 292c 0a20 2020 2020 2020 2020 2020  q"),.           
+00013ac0: 2020 2020 2020 2020 2020 2029 2069 6620             ) if 
+00013ad0: 7365 6c66 2e64 6174 6166 696c 6573 2069  self.datafiles i
+00013ae0: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
+00013af0: 5465 7874 2822 2229 2c0a 2020 2020 2020  Text(""),.      
+00013b00: 2020 2020 2020 2020 2020 4772 6f75 7028            Group(
+00013b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013b20: 2020 2020 202a 5b66 696c 6572 5f69 6e66       *[filer_inf
+00013b30: 6f2e 5f5f 7269 6368 5f5f 2829 2066 6f72  o.__rich__() for
+00013b40: 2066 696c 6572 5f69 6e66 6f20 696e 2073   filer_info in s
+00013b50: 656c 662e 6669 6c65 725f 696e 666f 735d  elf.filer_infos]
+00013b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013b70: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
+00013b80: 292c 2074 6974 6c65 3d66 2246 6f72 6d20  ), title=f"Form 
+00013b90: 7b73 656c 662e 6669 6c69 6e67 2e66 6f72  {self.filing.for
+00013ba0: 6d7d 2229 0a0a 0a64 6566 2073 756d 6d61  m}")...def summa
+00013bb0: 7269 7a65 5f66 696c 6573 2864 6174 613a  rize_files(data:
+00013bc0: 2070 642e 4461 7461 4672 616d 6529 202d   pd.DataFrame) -
+00013bd0: 3e20 7064 2e44 6174 6146 7261 6d65 3a0a  > pd.DataFrame:.
+00013be0: 2020 2020 7265 7475 726e 2028 6461 7461      return (data
+00013bf0: 0a20 2020 2020 2020 2020 2020 202e 6669  .            .fi
+00013c00: 6c74 6572 285b 2253 6571 222c 2022 446f  lter(["Seq", "Do
+00013c10: 6375 6d65 6e74 222c 2022 4465 7363 7269  cument", "Descri
+00013c20: 7074 696f 6e22 2c20 2253 697a 6522 5d29  ption", "Size"])
+00013c30: 0a20 2020 2020 2020 2020 2020 202e 6173  .            .as
+00013c40: 7369 676e 2853 697a 653d 6461 7461 2e53  sign(Size=data.S
+00013c50: 697a 652e 6170 706c 7928 6469 7370 6c61  ize.apply(displa
+00013c60: 795f 7369 7a65 2929 0a20 2020 2020 2020  y_size)).       
+00013c70: 2020 2020 202e 7365 745f 696e 6465 7828       .set_index(
+00013c80: 2253 6571 2229 0a20 2020 2020 2020 2020  "Seq").         
+00013c90: 2020 2029 0a0a 0a40 6c72 755f 6361 6368     )...@lru_cach
+00013ca0: 6528 6d61 7873 697a 653d 3136 290a 6465  e(maxsize=16).de
+00013cb0: 6620 6765 745f 6279 5f61 6363 6573 7369  f get_by_accessi
+00013cc0: 6f6e 5f6e 756d 6265 7228 6163 6365 7373  on_number(access
+00013cd0: 696f 6e5f 6e75 6d62 6572 3a20 7374 7229  ion_number: str)
+00013ce0: 3a0a 2020 2020 2222 2246 696e 6420 7468  :.    """Find th
+00013cf0: 6520 6669 6c69 6e67 2075 7369 6e67 2074  e filing using t
+00013d00: 6865 2061 6363 6573 7369 6f6e 206e 756d  he accession num
+00013d10: 6265 7222 2222 0a20 2020 2061 7373 6572  ber""".    asser
+00013d20: 7420 7265 2e6d 6174 6368 2872 225c 647b  t re.match(r"\d{
+00013d30: 3130 7d2d 5c64 7b32 7d2d 5c64 7b36 7d22  10}-\d{2}-\d{6}"
+00013d40: 2c20 6163 6365 7373 696f 6e5f 6e75 6d62  , accession_numb
+00013d50: 6572 292c 205c 0a20 2020 2020 2020 2066  er), \.        f
+00013d60: 227b 6163 6365 7373 696f 6e5f 6e75 6d62  "{accession_numb
+00013d70: 6572 7d20 6973 206e 6f74 2061 2076 616c  er} is not a val
+00013d80: 6964 2061 6363 6573 7369 6f6e 206e 756d  id accession num
+00013d90: 6265 7220 2e2e 2073 686f 756c 6420 6265  ber .. should be
+00013da0: 2031 3064 6967 6974 732d 3264 6967 6974   10digits-2digit
+00013db0: 732d 3664 6967 6974 7322 0a20 2020 2079  s-6digits".    y
+00013dc0: 6561 7220 3d20 696e 7428 2231 3922 202b  ear = int("19" +
+00013dd0: 2061 6363 6573 7369 6f6e 5f6e 756d 6265   accession_numbe
+00013de0: 725b 3131 3a31 335d 2920 6966 2061 6363  r[11:13]) if acc
+00013df0: 6573 7369 6f6e 5f6e 756d 6265 725b 3131  ession_number[11
+00013e00: 5d20 3d3d 2039 2065 6c73 6520 696e 7428  ] == 9 else int(
+00013e10: 2232 3022 202b 2061 6363 6573 7369 6f6e  "20" + accession
+00013e20: 5f6e 756d 6265 725b 3131 3a31 335d 290a  _number[11:13]).
+00013e30: 0a20 2020 2069 6620 7965 6172 203d 3d20  .    if year == 
+00013e40: 6461 7465 7469 6d65 2e6e 6f77 2829 2e79  datetime.now().y
+00013e50: 6561 723a 0a20 2020 2020 2020 2023 2046  ear:.        # F
+00013e60: 6f72 2074 6865 2063 7572 7265 6e74 2079  or the current y
+00013e70: 6561 7220 6372 6561 7465 2061 2072 616e  ear create a ran
+00013e80: 6765 206f 6620 7175 6172 7465 7273 2074  ge of quarters t
+00013e90: 6f20 7365 6172 6368 2066 726f 6d20 3120  o search from 1 
+00013ea0: 7570 2074 6f20 7468 6520 6375 7272 656e  up to the curren
+00013eb0: 7420 7175 6172 7465 7220 6f66 2074 6865  t quarter of the
+00013ec0: 2079 6561 720a 2020 2020 2020 2020 6375   year.        cu
+00013ed0: 7272 656e 745f 7175 6172 7465 7220 3d20  rrent_quarter = 
+00013ee0: 2864 6174 6574 696d 652e 6e6f 7728 292e  (datetime.now().
+00013ef0: 6d6f 6e74 6820 2d20 3129 202f 2f20 3320  month - 1) // 3 
+00013f00: 2b20 310a 2020 2020 2020 2020 7175 6172  + 1.        quar
+00013f10: 7465 7273 203d 2072 616e 6765 2831 2c20  ters = range(1, 
+00013f20: 6375 7272 656e 745f 7175 6172 7465 7220  current_quarter 
+00013f30: 2b20 3129 0a20 2020 2065 6c73 653a 0a20  + 1).    else:. 
+00013f40: 2020 2020 2020 2023 2053 6561 7263 6820         # Search 
+00013f50: 616c 6c20 7175 6172 7465 7273 0a20 2020  all quarters.   
+00013f60: 2020 2020 2071 7561 7274 6572 7320 3d20       quarters = 
+00013f70: 7261 6e67 6528 312c 2035 290a 0a20 2020  range(1, 5)..   
+00013f80: 2077 6974 6820 5374 6174 7573 2866 225b   with Status(f"[
+00013f90: 626f 6c64 2064 6565 705f 736b 795f 626c  bold deep_sky_bl
+00013fa0: 7565 315d 5365 6172 6368 696e 6720 666f  ue1]Searching fo
+00013fb0: 7220 6669 6c69 6e67 207b 6163 6365 7373  r filing {access
+00013fc0: 696f 6e5f 6e75 6d62 6572 7d2e 2e2e 222c  ion_number}...",
+00013fd0: 2073 7069 6e6e 6572 3d22 646f 7473 3222   spinner="dots2"
+00013fe0: 293a 0a20 2020 2020 2020 2066 6f72 2071  ):.        for q
+00013ff0: 7561 7274 6572 2069 6e20 7175 6172 7465  uarter in quarte
+00014000: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
+00014010: 6669 6c69 6e67 7320 3d20 5f67 6574 5f63  filings = _get_c
+00014020: 6163 6865 645f 6669 6c69 6e67 7328 7965  ached_filings(ye
+00014030: 6172 3d79 6561 722c 2071 7561 7274 6572  ar=year, quarter
+00014040: 3d71 7561 7274 6572 290a 2020 2020 2020  =quarter).      
+00014050: 2020 2020 2020 6966 2066 696c 696e 6773        if filings
+00014060: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014070: 2020 6669 6c69 6e67 203d 2066 696c 696e    filing = filin
+00014080: 6773 2e67 6574 2861 6363 6573 7369 6f6e  gs.get(accession
+00014090: 5f6e 756d 6265 7229 0a20 2020 2020 2020  _number).       
+000140a0: 2020 2020 2020 2020 2069 6620 6669 6c69           if fili
+000140b0: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
+000140c0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+000140d0: 696c 696e 670a 2020 2020 2320 5765 2068  iling.    # We h
+000140e0: 6176 656e 2774 2066 6f75 6e64 2074 6865  aven't found the
+000140f0: 2066 696c 696e 6720 6e6f 726d 616c 6c79   filing normally
+00014100: 2073 6f20 6368 6563 6b20 7468 6520 6d6f   so check the mo
+00014110: 7374 2072 6563 656e 7420 5345 4320 6669  st recent SEC fi
+00014120: 6c69 6e67 730a 2020 2020 2320 4368 6563  lings.    # Chec
+00014130: 6b20 6966 2074 6865 2079 6561 7220 6973  k if the year is
+00014140: 2074 6865 2063 7572 7265 6e74 2079 6561   the current yea
+00014150: 720a 2020 2020 6966 2079 6561 7220 3d3d  r.    if year ==
+00014160: 2064 6174 6574 696d 652e 6e6f 7728 292e   datetime.now().
+00014170: 7965 6172 3a0a 2020 2020 2020 2020 2320  year:.        # 
+00014180: 4765 7420 7468 6520 6d6f 7374 2072 6563  Get the most rec
+00014190: 656e 7420 6669 6c69 6e67 730a 2020 2020  ent filings.    
+000141a0: 2020 2020 6669 6c69 6e67 7320 3d20 6765      filings = ge
+000141b0: 745f 6375 7272 656e 745f 6669 6c69 6e67  t_current_filing
+000141c0: 7328 290a 2020 2020 2020 2020 7265 7475  s().        retu
+000141d0: 726e 2066 696c 696e 6773 2e67 6574 2861  rn filings.get(a
+000141e0: 6363 6573 7369 6f6e 5f6e 756d 6265 7229  ccession_number)
+000141f0: 0a0a 0a64 6566 2066 6f72 6d5f 7769 7468  ...def form_with
+00014200: 5f61 6d65 6e64 6d65 6e74 7328 2a66 6f72  _amendments(*for
+00014210: 6d73 3a20 7374 7229 3a0a 2020 2020 7265  ms: str):.    re
+00014220: 7475 726e 206c 6973 7428 666f 726d 7329  turn list(forms)
+00014230: 202b 205b 6622 7b66 7d2f 4122 2066 6f72   + [f"{f}/A" for
+00014240: 2066 2069 6e20 666f 726d 735d 0a0a 0a62   f in forms]...b
+00014250: 6172 6368 6172 7420 3d20 275c 5530 3030  archart = '\U000
+00014260: 3146 3443 4127 0a74 6963 6b65 7420 3d20  1F4CA'.ticket = 
+00014270: 275c 5530 3030 3146 3341 4227 0a70 6167  '\U0001F3AB'.pag
+00014280: 655f 6661 6369 6e67 5f75 7020 3d20 275c  e_facing_up = '\
+00014290: 5530 3030 3146 3443 3427 0a63 6c61 7373  U0001F4C4'.class
+000142a0: 6963 616c 5f62 7569 6c64 696e 6720 3d20  ical_building = 
+000142b0: 275c 5530 3030 3146 3344 4227 0a0a 0a64  '\U0001F3DB'...d
+000142c0: 6566 2075 6e69 636f 6465 5f66 6f72 5f66  ef unicode_for_f
+000142d0: 6f72 6d28 666f 726d 3a20 7374 7229 3a0a  orm(form: str):.
+000142e0: 2020 2020 6966 2066 6f72 6d20 696e 205b      if form in [
+000142f0: 2731 302d 4b27 2c20 2731 302d 5127 2c20  '10-K', '10-Q', 
+00014300: 2731 302d 4b2f 4127 2c20 2731 302d 512f  '10-K/A', '10-Q/
+00014310: 4127 2c20 2736 2d4b 272c 2027 362d 4b2f  A', '6-K', '6-K/
+00014320: 4127 5d3a 0a20 2020 2020 2020 2072 6574  A']:.        ret
+00014330: 7572 6e20 6261 7263 6861 7274 0a20 2020  urn barchart.   
+00014340: 2065 6c69 6620 666f 726d 2069 6e20 5b27   elif form in ['
+00014350: 3327 2c20 2734 272c 2027 3527 2c20 2733  3', '4', '5', '3
+00014360: 2f41 272c 2027 342f 4127 2c20 2735 2f41  /A', '4/A', '5/A
+00014370: 275d 3a0a 2020 2020 2020 2020 7265 7475  ']:.        retu
+00014380: 726e 2074 6963 6b65 740a 2020 2020 656c  rn ticket.    el
+00014390: 6966 2066 6f72 6d20 696e 205b 274d 412d  if form in ['MA-
+000143a0: 4927 2c20 274d 412d 492f 4127 2c20 274d  I', 'MA-I/A', 'M
+000143b0: 4127 2c20 274d 412f 4127 5d3a 0a20 2020  A', 'MA/A']:.   
+000143c0: 2020 2020 2072 6574 7572 6e20 636c 6173       return clas
+000143d0: 7369 6361 6c5f 6275 696c 6469 6e67 0a20  sical_building. 
+000143e0: 2020 2072 6574 7572 6e20 7061 6765 5f66     return page_f
+000143f0: 6163 696e 675f 7570 0a                   acing_up.
```

### Comparing `edgartools-2.8.3/edgar/_gaap.py` & `edgartools-2.9.0/edgar/_gaap.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.8.3/edgar/_markdown.py` & `edgartools-2.9.0/edgar/_markdown.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.8.3/edgar/_party.py` & `edgartools-2.9.0/edgar/_party.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.8.3/edgar/_rich.py` & `edgartools-2.9.0/edgar/_rich.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.8.3/edgar/_xbrl.py` & `edgartools-2.9.0/edgar/_xbrl.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.8.3/edgar/_xml.py` & `edgartools-2.9.0/edgar/_xml.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.8.3/edgar/company_reports.py` & `edgartools-2.9.0/edgar/company_reports.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.8.3/edgar/core.py` & `edgartools-2.9.0/edgar/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import datetime
 import gzip
 import logging.config
 import os
 import random
 import re
+import sys
 import threading
 import warnings
 from _thread import interrupt_main
 from dataclasses import dataclass
 from decimal import Decimal
 from functools import lru_cache
 from io import BytesIO
 from typing import Union, Optional, Tuple, List
-import sys
+
 import httpx
 import humanize
 import pandas as pd
 import pyarrow as pa
 import pyarrow.compute as pc
 from charset_normalizer import detect
 from fastcore.basics import listify
@@ -66,14 +67,15 @@
     'extract_dates',
     'get_resource',
     'get_identity',
     'pandas_version',
     'python_version',
     'set_identity',
     'download_text',
+    'download_json',
     'download_file',
     'decode_content',
     'filter_by_date',
     'filter_by_form',
     'text_extensions',
     'ask_for_identity',
     'default_page_size',
@@ -299,14 +301,21 @@
 def http_client():
     return httpx.Client(headers=client_headers(),
                         timeout=edgar_mode.http_timeout,
                         limits=edgar_mode.limits,
                         default_encoding=autodetect)
 
 
+def async_http_client():
+    return httpx.AsyncClient(headers=client_headers(),
+                             timeout=edgar_mode.http_timeout,
+                             limits=edgar_mode.limits,
+                             default_encoding=autodetect)
+
+
 def get_json(data_url: str):
     with http_client() as client:
         r = client.get(data_url)
         if r.status_code == 200:
             return r.json()
         r.raise_for_status()
 
@@ -314,16 +323,17 @@
 def decode_content(content: bytes):
     try:
         return content.decode('utf-8')
     except UnicodeDecodeError:
         return content.decode('latin-1')
 
 
-text_extensions = [".txt", ".htm", ".html", ".xsd", ".xml", "XML",  ".json", ".idx"]
-binary_extensions = [".pdf", ".jpg", ".jpeg", "png", ".gif", ".tif", ".tiff", ".bmp", ".ico", ".svg", ".webp", ".avif", ".apng"]
+text_extensions = [".txt", ".htm", ".html", ".xsd", ".xml", "XML", ".json", ".idx"]
+binary_extensions = [".pdf", ".jpg", ".jpeg", "png", ".gif", ".tif", ".tiff", ".bmp", ".ico", ".svg", ".webp", ".avif",
+                     ".apng"]
 
 
 def download_file(url: str,
                   client: Union[httpx.Client, httpx.AsyncClient] = None,
                   as_text: bool = None):
     # reason_phrase = 'Too Many Requests' status_code = 429
     if not client:
@@ -355,14 +365,22 @@
         r.raise_for_status()
 
 
 def download_text(url: str, client: Union[httpx.Client, httpx.AsyncClient] = None):
     return download_file(url, client, as_text=True)
 
 
+def download_json(data_url: str):
+    with http_client() as client:
+        r = client.get(data_url)
+        if r.status_code == 200:
+            return r.json()
+        r.raise_for_status()
+
+
 def get_text_between_tags(url: str, tag: str, client: Union[httpx.Client, httpx.AsyncClient] = None):
     if not client:
         client = http_client()
     tag_start = f'<{tag}>'
     tag_end = f'</{tag}>'
     is_header = False
     content = ""
@@ -400,15 +418,14 @@
 
 
 def get_bool(value: str = None) -> Optional[bool]:
     """Convert the value to a boolean"""
     return value in [1, "1", "Y", "true", "True", "TRUE"]
 
 
-
 class Result:
     """
     This class represents the result of an operation which can succeed or fail.
     It allows for handling the failures more gracefully that using error handling
     """
 
     def __init__(self,
@@ -597,31 +614,34 @@
 def reverse_name(name):
     # Split the name into parts
     parts = name.split()
 
     # Handle the cases where there's a 'Jr', 'Sr', 'II', 'III', 'MD', etc., or 'ET AL'
     special_parts = ['Jr', 'Sr', 'II', 'III', 'MD', 'ET', 'AL', 'et', 'al']
     special_parts_with_period = [part + '.' for part in special_parts if part not in ['II', 'III']] + special_parts
-    special_part_indices = [i for i, part in enumerate(parts) if part in special_parts_with_period or (i > 0 and parts[i-1].rstrip('.') + ' ' + part.rstrip('.') == 'ET AL')]
+    special_part_indices = [i for i, part in enumerate(parts) if part in special_parts_with_period or (
+                i > 0 and parts[i - 1].rstrip('.') + ' ' + part.rstrip('.') == 'ET AL')]
 
     # Extract the special parts and the main name parts
     special_parts_list = [parts[i] for i in special_part_indices]
     main_name_parts = [part for i, part in enumerate(parts) if i not in special_part_indices]
 
     # Handle initials in the name (e.g., 'K. Michelle')
     if '.' in main_name_parts[-2] or len(main_name_parts[-2]) == 1:
-        main_name_parts = [' '.join(main_name_parts[:-2]).title()] + [f"{main_name_parts[-1].title()} {main_name_parts[-2]}" ]
+        main_name_parts = [' '.join(main_name_parts[:-2]).title()] + [
+            f"{main_name_parts[-1].title()} {main_name_parts[-2]}"]
     else:
         main_name_parts = [part.title() if len(part) > 2 else part for part in main_name_parts]
 
     # Reverse the main name parts
     reversed_main_parts = [part for part in main_name_parts[1:]] + [main_name_parts[0]]
     reversed_name = " ".join(reversed_main_parts)
 
     # Append the special parts to the reversed name, maintaining their original case
     if special_parts_list:
         reversed_name += " " + " ".join(special_parts_list)
 
     return reversed_name
 
+
 def yes_no(value: bool) -> str:
-    return "Yes" if value else "No"
+    return "Yes" if value else "No"
```

### Comparing `edgartools-2.8.3/edgar/effect.py` & `edgartools-2.9.0/edgar/effect.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.8.3/edgar/financials.py` & `edgartools-2.9.0/edgar/financials.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.8.3/edgar/form144.py` & `edgartools-2.9.0/edgar/form144.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.8.3/edgar/forms.py` & `edgartools-2.9.0/edgar/forms.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.8.3/edgar/fundreports.py` & `edgartools-2.9.0/edgar/fundreports.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.8.3/edgar/funds.py` & `edgartools-2.9.0/edgar/funds.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.8.3/edgar/htmltools.py` & `edgartools-2.9.0/edgar/htmltools.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.8.3/edgar/muniadvisors.py` & `edgartools-2.9.0/edgar/muniadvisors.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.8.3/edgar/offerings.py` & `edgartools-2.9.0/edgar/offerings.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.8.3/edgar/ownership.py` & `edgartools-2.9.0/edgar/ownership.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.8.3/edgar/search.py` & `edgartools-2.9.0/edgar/search.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.8.3/edgar/sgml.py` & `edgartools-2.9.0/edgar/sgml.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.8.3/edgar/thirteenf.py` & `edgartools-2.9.0/edgar/thirteenf.py`

 * *Files identical despite different names*

### Comparing `edgartools-2.8.3/edgar/data/gaap_taxonomy_2022.csv` & `edgartools-2.9.0/edgar/data/gaap_taxonomy_2022.csv`

 * *Files identical despite different names*

### Comparing `edgartools-2.8.3/LICENSE.txt` & `edgartools-2.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edgartools-2.8.3/README.md` & `edgartools-2.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -631,11 +631,16 @@
 `edgartools` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
 
 ## Contact
 
 [LinkedIn](https://www.linkedin.com/in/dwight-gunning-860124/)
 
 
-
 ## Supporters
 [![Stargazers repo roster for @dgunning/edgartools](https://reporoster.com/stars/dgunning/edgartools)](https://github.com/dgunning/edgartools/stargazers)
-[![Forkers repo roster for @dgunning/edgartools](https://reporoster.com/forks/dgunning/edgartools)](https://github.com/dgunning/edgartools/network/members)
+[![Forkers repo roster for @dgunning/edgartools](https://reporoster.com/forks/dgunning/edgartools)](https://github.com/dgunning/edgartools/network/members)
+
+## Subscribe to Polar
+<picture>
+2  <source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/subscribe.svg?org=polarsource&label=Subscribe&darkmode">
+3  <img alt="Subscribe on Polar" src="https://polar.sh/embed/subscribe.svg?org=polarsource&label=Subscribe">
+4</picture>
```

#### html2text {}

```diff
@@ -270,8 +270,9 @@
 - Make sure your code lints. - Issue that pull request! # License `edgartools`
 is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html)
 license. ## Contact [LinkedIn](https://www.linkedin.com/in/dwight-gunning-
 860124/) ## Supporters [![Stargazers repo roster for @dgunning/edgartools]
 (https://reporoster.com/stars/dgunning/edgartools)](https://github.com/
 dgunning/edgartools/stargazers) [![Forkers repo roster for @dgunning/
 edgartools](https://reporoster.com/forks/dgunning/edgartools)](https://
-github.com/dgunning/edgartools/network/members)
+github.com/dgunning/edgartools/network/members) ## Subscribe to Polar 2 3
+[Subscribe on Polar]4
```

### Comparing `edgartools-2.8.3/pyproject.toml` & `edgartools-2.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 python = ["38", "39", "310", "311"]
 
 [tool.coverage.run]
 branch = true
 parallel = true
 omit = [
   "edgar/__about__.py",
+  "tests/perf*"
 ]
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
```

### Comparing `edgartools-2.8.3/PKG-INFO` & `edgartools-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgartools
-Version: 2.8.3
+Version: 2.9.0
 Summary: One of the nicest looking EDGAR libraries out there
 Project-URL: Documentation, https://dgunning.github.io/edgartools/
 Project-URL: Issues, https://github.com/dgunning/edgartools/issues
 Project-URL: Source, https://github.com/dgunning/edgartools
 Author-email: Dwight Gunning <dgunning@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -668,11 +668,16 @@
 `edgartools` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
 
 ## Contact
 
 [LinkedIn](https://www.linkedin.com/in/dwight-gunning-860124/)
 
 
-
 ## Supporters
 [![Stargazers repo roster for @dgunning/edgartools](https://reporoster.com/stars/dgunning/edgartools)](https://github.com/dgunning/edgartools/stargazers)
-[![Forkers repo roster for @dgunning/edgartools](https://reporoster.com/forks/dgunning/edgartools)](https://github.com/dgunning/edgartools/network/members)
+[![Forkers repo roster for @dgunning/edgartools](https://reporoster.com/forks/dgunning/edgartools)](https://github.com/dgunning/edgartools/network/members)
+
+## Subscribe to Polar
+<picture>
+2  <source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/subscribe.svg?org=polarsource&label=Subscribe&darkmode">
+3  <img alt="Subscribe on Polar" src="https://polar.sh/embed/subscribe.svg?org=polarsource&label=Subscribe">
+4</picture>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: edgartools Version: 2.8.3 Summary: One of the
+Metadata-Version: 2.1 Name: edgartools Version: 2.9.0 Summary: One of the
 nicest looking EDGAR libraries out there Project-URL: Documentation, https://
 dgunning.github.io/edgartools/ Project-URL: Issues, https://github.com/
 dgunning/edgartools/issues Project-URL: Source, https://github.com/dgunning/
 edgartools Author-email: Dwight Gunning
 gmail.com> License-Expression: MIT License-File: LICENSE.txt Keywords:
 company,edgar,filings,finance,financial,python,reports,sec Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
@@ -290,8 +290,9 @@
 - Make sure your code lints. - Issue that pull request! # License `edgartools`
 is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html)
 license. ## Contact [LinkedIn](https://www.linkedin.com/in/dwight-gunning-
 860124/) ## Supporters [![Stargazers repo roster for @dgunning/edgartools]
 (https://reporoster.com/stars/dgunning/edgartools)](https://github.com/
 dgunning/edgartools/stargazers) [![Forkers repo roster for @dgunning/
 edgartools](https://reporoster.com/forks/dgunning/edgartools)](https://
-github.com/dgunning/edgartools/network/members)
+github.com/dgunning/edgartools/network/members) ## Subscribe to Polar 2 3
+[Subscribe on Polar]4
```

