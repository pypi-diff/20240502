# Comparing `tmp/dataextractoroeg-0.3.9.tar.gz` & `tmp/dataextractoroeg-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dataextractoroeg-0.3.9.tar", last modified: Thu May  2 08:35:53 2024, max compression
+gzip compressed data, was "dist\dataextractoroeg-0.4.0.tar", last modified: Thu May  2 10:52:23 2024, max compression
```

## Comparing `dataextractoroeg-0.3.9.tar` & `dataextractoroeg-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 08:35:53.305415 dataextractoroeg-0.3.9/
--rw-rw-rw-   0        0        0       70 2024-04-29 12:43:01.000000 dataextractoroeg-0.3.9/.gitignore
-drwxrwxrwx   0        0        0        0 2024-05-02 08:35:53.298184 dataextractoroeg-0.3.9/DataExtractorOEG.egg-info/
--rw-rw-rw-   0        0        0     3046 2024-05-02 08:35:52.000000 dataextractoroeg-0.3.9/DataExtractorOEG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      567 2024-05-02 08:35:52.000000 dataextractoroeg-0.3.9/DataExtractorOEG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 08:35:52.000000 dataextractoroeg-0.3.9/DataExtractorOEG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-02 08:35:52.000000 dataextractoroeg-0.3.9/DataExtractorOEG.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-05-02 08:35:52.000000 dataextractoroeg-0.3.9/DataExtractorOEG.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-02 08:35:52.000000 dataextractoroeg-0.3.9/DataExtractorOEG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.3.9/LICENSE.txt
--rw-rw-rw-   0        0        0     3046 2024-05-02 08:35:53.298184 dataextractoroeg-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2024-04-29 12:08:53.000000 dataextractoroeg-0.3.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 08:35:53.252202 dataextractoroeg-0.3.9/doiExtractor/
-drwxrwxrwx   0        0        0        0 2024-05-02 08:35:53.284916 dataextractoroeg-0.3.9/doiExtractor/ExistingPapers/
--rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.3.9/doiExtractor/ExistingPapers/Papers.csv
--rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.3.9/doiExtractor/ExistingPapers/name_doi_papers.csv
-drwxrwxrwx   0        0        0        0 2024-05-02 08:35:53.290180 dataextractoroeg-0.3.9/doiExtractor/Outputs/
--rw-rw-rw-   0        0        0    14166 2024-04-26 10:27:22.000000 dataextractoroeg-0.3.9/doiExtractor/Outputs/dois.txt
--rw-rw-rw-   0        0        0    77928 2024-04-25 14:42:00.000000 dataextractoroeg-0.3.9/doiExtractor/Outputs/results.csv
--rw-rw-rw-   0        0        0   123715 2024-04-29 12:01:52.000000 dataextractoroeg-0.3.9/doiExtractor/Outputs/results.json
--rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.3.9/doiExtractor/__init__.py
--rw-rw-rw-   0        0        0     8406 2024-05-02 08:32:41.000000 dataextractoroeg-0.3.9/doiExtractor/doiExtractor.py
--rw-rw-rw-   0        0        0     2365 2024-04-29 13:44:46.000000 dataextractoroeg-0.3.9/doiExtractor/main.py
--rw-rw-rw-   0        0        0     4086 2024-04-29 11:57:15.000000 dataextractoroeg-0.3.9/doiExtractor/openAlex.py
--rw-rw-rw-   0        0        0       42 2024-05-02 08:35:53.305415 dataextractoroeg-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0      592 2024-05-02 08:27:10.000000 dataextractoroeg-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 10:52:23.393151 dataextractoroeg-0.4.0/
+-rw-rw-rw-   0        0        0       70 2024-04-29 12:43:01.000000 dataextractoroeg-0.4.0/.gitignore
+drwxrwxrwx   0        0        0        0 2024-05-02 10:52:23.389054 dataextractoroeg-0.4.0/DataExtractorOEG.egg-info/
+-rw-rw-rw-   0        0        0     3046 2024-05-02 10:52:23.000000 dataextractoroeg-0.4.0/DataExtractorOEG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2024-05-02 10:52:23.000000 dataextractoroeg-0.4.0/DataExtractorOEG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 10:52:23.000000 dataextractoroeg-0.4.0/DataExtractorOEG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-02 10:52:23.000000 dataextractoroeg-0.4.0/DataExtractorOEG.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-05-02 10:52:23.000000 dataextractoroeg-0.4.0/DataExtractorOEG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-02 10:52:23.000000 dataextractoroeg-0.4.0/DataExtractorOEG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     3046 2024-05-02 10:52:23.390055 dataextractoroeg-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2024-04-29 12:08:53.000000 dataextractoroeg-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 10:52:23.371416 dataextractoroeg-0.4.0/doiExtractor/
+drwxrwxrwx   0        0        0        0 2024-05-02 10:52:23.377655 dataextractoroeg-0.4.0/doiExtractor/ExistingPapers/
+-rw-rw-rw-   0        0        0   542602 2024-04-10 16:37:25.000000 dataextractoroeg-0.4.0/doiExtractor/ExistingPapers/Papers.csv
+-rw-rw-rw-   0        0        0     4080 2024-04-12 14:53:18.000000 dataextractoroeg-0.4.0/doiExtractor/ExistingPapers/name_doi_papers.csv
+drwxrwxrwx   0        0        0        0 2024-05-02 10:52:23.381822 dataextractoroeg-0.4.0/doiExtractor/Outputs/
+-rw-rw-rw-   0        0        0        0 2024-05-02 09:14:00.000000 dataextractoroeg-0.4.0/doiExtractor/Outputs/dois.txt
+-rw-rw-rw-   0        0        0        0 2024-05-02 09:32:18.000000 dataextractoroeg-0.4.0/doiExtractor/Outputs/results.csv
+-rw-rw-rw-   0        0        0   129283 2024-05-02 08:58:23.000000 dataextractoroeg-0.4.0/doiExtractor/Outputs/results.json
+-rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.4.0/doiExtractor/__init__.py
+-rw-rw-rw-   0        0        0     8307 2024-05-02 10:51:20.000000 dataextractoroeg-0.4.0/doiExtractor/doiExtractor.py
+-rw-rw-rw-   0        0        0     2365 2024-05-02 09:09:51.000000 dataextractoroeg-0.4.0/doiExtractor/main.py
+-rw-rw-rw-   0        0        0     4109 2024-05-02 10:51:07.000000 dataextractoroeg-0.4.0/doiExtractor/openAlex.py
+-rw-rw-rw-   0        0        0       42 2024-05-02 10:52:23.393151 dataextractoroeg-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      592 2024-05-02 10:52:17.000000 dataextractoroeg-0.4.0/setup.py
```

### Comparing `dataextractoroeg-0.3.9/DataExtractorOEG.egg-info/PKG-INFO` & `dataextractoroeg-0.4.0/DataExtractorOEG.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.3.9
+Version: 0.4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
```

### Comparing `dataextractoroeg-0.3.9/DataExtractorOEG.egg-info/SOURCES.txt` & `dataextractoroeg-0.4.0/DataExtractorOEG.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.9/LICENSE.txt` & `dataextractoroeg-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.9/PKG-INFO` & `dataextractoroeg-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.3.9
+Version: 0.4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
```

### Comparing `dataextractoroeg-0.3.9/README.md` & `dataextractoroeg-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.9/doiExtractor/ExistingPapers/Papers.csv` & `dataextractoroeg-0.4.0/doiExtractor/ExistingPapers/Papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.9/doiExtractor/ExistingPapers/name_doi_papers.csv` & `dataextractoroeg-0.4.0/doiExtractor/ExistingPapers/name_doi_papers.csv`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.9/doiExtractor/Outputs/results.json` & `dataextractoroeg-0.4.0/doiExtractor/Outputs/results.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8449744463373047%*

 * *Differences: {'0': '{\'NAME\': \'"Traffic Optimization Through Waiting Prediction and Evolutive Algorithms"\'}',*

 * * '10': '{\'NAME\': \'"A Scoping Review on the Progress, Applicability, and Future of Explainable '*

 * *       'Artificial Intelligence in Medicine"\'}',*

 * * '101': '{\'NAME\': \'"Extraction and Semantic Representation of Domain-Specific Relations in '*

 * *        'Spanish Labour Law"\'}',*

 * * '102': '{\'NAME\': \'"An Overview of Drugs, Diseases, Genes and Proteins in the CORD-19 Corpus '*

 * *        '[Una visión general de los […]*

```diff
@@ -1,41 +1,36 @@
 [
     {
         "DOI": "10.9781/ijimai.2023.12.001",
-        "NAME": "Traffic Optimization Through Waiting Prediction and Evolutive Algorithms",
+        "NAME": "\"Traffic Optimization Through Waiting Prediction and Evolutive Algorithms\"",
         "PRIMARY_LOCATION": "https://doi.org/10.9781/ijimai.2023.12.001"
     },
     {
         "DOI": null,
         "NAME": "Automatic Topic Label Generation using Conversational Models",
         "PRIMARY_LOCATION": "https://doi.org/10.1145/3587259.3627574"
     },
     {
         "DOI": "10.2830/446704",
-        "NAME": "Report on Data Homogenisation for High-value Datasets",
+        "NAME": "\"Report on Data Homogenisation for High-value Datasets\"",
         "PRIMARY_LOCATION": null
     },
     {
-        "DOI": "10.1007/s11227-023-05774-3",
-        "NAME": "Interoperability of heterogeneous Systems of Systems: from requirements to a reference architecture",
-        "PRIMARY_LOCATION": "https://link.springer.com/content/pdf/10.1007/s11227-023-05774-3.pdf"
-    },
-    {
         "DOI": "10.3390/info14120631",
-        "NAME": "Is Automated Consent in Solid GDPR-Compliant? An Approach for Obtaining Valid Consent with the Solid Protocol",
+        "NAME": "\"Is Automated Consent in Solid GDPR-Compliant? An Approach for Obtaining Valid Consent with the Solid Protocol\"",
         "PRIMARY_LOCATION": "https://www.mdpi.com/2078-2489/14/12/631/pdf?version=1700836284"
     },
     {
         "DOI": null,
         "NAME": "The role of Semantic Web Technologies in Legal Terminology",
         "PRIMARY_LOCATION": "https://ceur-ws.org/Vol-1481/paper27.pdf"
     },
     {
         "DOI": "10.9781/ijimai.2023.11.001",
-        "NAME": "A Review of Bias and Fairness in Artificial Intelligence",
+        "NAME": "\"A Review of Bias and Fairness in Artificial Intelligence\"",
         "PRIMARY_LOCATION": "https://doi.org/10.9781/ijimai.2023.11.001"
     },
     {
         "DOI": null,
         "NAME": "Softalias-KG: Reconciling Software Mentions in Scientific Literature.",
         "PRIMARY_LOCATION": null
     },
@@ -47,255 +42,260 @@
     {
         "DOI": null,
         "NAME": "The Semantic Web ? ISWC 2023. 22nd International Semantic Web Conference, Athens, Greece, November 6?10, 2023, Proceedings, Part",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.1016/j.artmed.2023.102687",
-        "NAME": "Uncovering hidden therapeutic indications through drug repurposing with graph neural networks and heterogeneous data",
+        "NAME": "\"Uncovering hidden therapeutic indications through drug repurposing with graph neural networks and heterogeneous data\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.artmed.2023.102687"
     },
     {
         "DOI": "10.3390/app131910778",
-        "NAME": "A Scoping Review on the Progress, Applicability, and Future of Explainable Artificial Intelligence in Medicine",
+        "NAME": "\"A Scoping Review on the Progress, Applicability, and Future of Explainable Artificial Intelligence in Medicine\"",
         "PRIMARY_LOCATION": "https://www.mdpi.com/2076-3417/13/19/10778/pdf?version=1695880594"
     },
     {
         "DOI": "10.1109/MMUL.2023.3303393",
-        "NAME": "Encoding of Media Value Chain Processes Through Blockchains and MPEG-21 Smart Contracts for Media",
+        "NAME": "\"Encoding of Media Value Chain Processes Through Blockchains and MPEG-21 Smart Contracts for Media\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/mmul.2023.3303393"
     },
     {
         "DOI": null,
         "NAME": "Towards Assessing FAIR Research Software Best Practices in an Organization Using RDF-star.",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": null,
         "NAME": "EA-Ontology: Ethical Assessment Ontology",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.3989/redc.2023.3.1996",
-        "NAME": "Automatic thematic classification of documents based on vocabularies and use frequencies. The case of scientific dissemination articles",
+        "NAME": "\"Automatic thematic classification of documents based on vocabularies and use frequencies. The case of scientific dissemination articles\"",
         "PRIMARY_LOCATION": "https://redc.revistas.csic.es/index.php/redc/article/download/1517/2292"
     },
     {
         "DOI": "10.1145/3586078",
-        "NAME": "Experiential Observations: An Ontology Pattern-Based Study on Capturing the Potential Content within Evidences of Experiences",
+        "NAME": "\"Experiential Observations: An Ontology Pattern-Based Study on Capturing the Potential Content within Evidences of Experiences\"",
         "PRIMARY_LOCATION": "https://dl.acm.org/doi/pdf/10.1145/3586078"
     },
     {
         "DOI": "10.26342/2023-71-15",
-        "NAME": "Automatic Easy-to-Read Translation of Morphological Structures in Spanish Texts",
+        "NAME": "\"Automatic Easy-to-Read Translation of Morphological Structures in Spanish Texts\"",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.1016/j.techsoc.2023.102304",
-        "NAME": "Mind the gap: The AURORAL ecosystem for the digital transformation of smart communities and rural areas",
+        "NAME": "\"Mind the gap: The AURORAL ecosystem for the digital transformation of smart communities and rural areas\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.techsoc.2023.102304"
     },
     {
         "DOI": "10.3390/info14070351",
-        "NAME": "\u201cWho Should I Trust with My Data?\u201d Ethical and Legal Challenges for Innovation in New Decentralized Data Management Technologies",
+        "NAME": "\"\u201cWho Should I Trust with My Data?\u201d Ethical and Legal Challenges for Innovation in New Decentralized Data Management Technologies\"",
         "PRIMARY_LOCATION": "https://www.mdpi.com/2078-2489/14/7/351/pdf?version=1687339409"
     },
     {
         "DOI": null,
         "NAME": "FAIR Research Object Assessment: A landscape analysis.",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": null,
         "NAME": "MuHeQA: Zero-shot Question Answering over Multiple and Heterogeneous Knowledge Bases",
         "PRIMARY_LOCATION": "https://content.iospress.com:443/download/semantic-web/sw233379?id=semantic-web%2Fsw233379"
     },
     {
         "DOI": "10.2298/CSIS220110008V",
-        "NAME": "Multi-perspective Approach for Curating and Exploring the History of Climate Change in Latin America within Digital Newspapers",
+        "NAME": "\"Multi-perspective Approach for Curating and Exploring the History of Climate Change in Latin America within Digital Newspapers\"",
         "PRIMARY_LOCATION": "http://www.doiserbia.nb.rs/ft.aspx?id=1820-02142300008V"
     },
     {
         "DOI": "10.1109/TG.2022.3214154",
-        "NAME": "Multi-Agent Systems on Virtual Games: A Systematic Mapping Study",
+        "NAME": "\"Multi-Agent Systems on Virtual Games: A Systematic Mapping Study\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/tg.2022.3214154"
     },
     {
         "DOI": "10.1016/j.envsoft.2023.105695",
-        "NAME": "A framework for the broad dissemination of hydrological models for non-expert users",
+        "NAME": "\"A framework for the broad dissemination of hydrological models for non-expert users\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.envsoft.2023.105695"
     },
     {
         "DOI": null,
         "NAME": "Porting the One Size Fits All Model for Terminology into a Linked Data Compatible Format",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": null,
         "NAME": "Ya2ro: A tool for creating Research Objects from minimum metadata",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.3390/rs15112716",
-        "NAME": "Satellite Earth Observation for Essential Climate Variables Supporting Sustainable Development Goals: A Review on Applications",
+        "NAME": "\"Satellite Earth Observation for Essential Climate Variables Supporting Sustainable Development Goals: A Review on Applications\"",
         "PRIMARY_LOCATION": "https://www.mdpi.com/2072-4292/15/11/2716/pdf?version=1684894645"
     },
     {
         "DOI": "10.1016/j.softx.2023.101391",
-        "NAME": "TINTO: Converting Tidy Data into image for classification with 2-Dimensional Convolutional Neural Networks",
+        "NAME": "\"TINTO: Converting Tidy Data into image for classification with 2-Dimensional Convolutional Neural Networks\"",
         "PRIMARY_LOCATION": "http://www.softxjournal.com/article/S2352711023000870/pdf"
     },
     {
         "DOI": "10.1007/s11192-023-04648-y",
-        "NAME": "Gender imbalance in doctoral education: an analysis of the Spanish university system (1977\u20132021)",
+        "NAME": "\"Gender imbalance in doctoral education: an analysis of the Spanish university system (1977\u20132021)\"",
         "PRIMARY_LOCATION": "https://link.springer.com/content/pdf/10.1007/s11192-023-04648-y.pdf"
     },
     {
         "DOI": "10.26342/2023-70-12",
-        "NAME": "Widaug. Data augmentation for named entity recognition using Wikidata",
+        "NAME": "\"Widaug. Data augmentation for named entity recognition using Wikidata\"",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.1016/j.inffus.2022.09.028",
-        "NAME": "Combining heterogeneous data sources for spatio-temporal mobility demand forecasting",
+        "NAME": "\"Combining heterogeneous data sources for spatio-temporal mobility demand forecasting\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.inffus.2022.09.028"
     },
     {
         "DOI": "10.1016/j.inffus.2022.10.011",
-        "NAME": "A novel deep learning approach using blurring image techniques for Bluetooth-based indoor localisation",
+        "NAME": "\"A novel deep learning approach using blurring image techniques for Bluetooth-based indoor localisation\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.inffus.2022.10.011"
     },
     {
         "DOI": "10.1016/j.future.2022.11.004",
-        "NAME": "A scalable, secure, and semantically interoperable client for cloud-enabled Demand Response",
+        "NAME": "\"A scalable, secure, and semantically interoperable client for cloud-enabled Demand Response\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.future.2022.11.004"
     },
     {
         "DOI": "10.1007/978-3-031-21229-1_1",
-        "NAME": "Modelling of\u00a0the\u00a0Internet Computer Protocol Architecture: The Next Generation Blockchain",
+        "NAME": "\"Modelling of\u00a0the\u00a0Internet Computer Protocol Architecture: The Next Generation Blockchain\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-031-21229-1_1"
     },
     {
         "DOI": "10.1109/CCNC51644.2023.10059701",
-        "NAME": "On the Decentralization of Health Systems for Data Availability: A DLT-based Architecture",
+        "NAME": "\"On the Decentralization of Health Systems for Data Availability: A DLT-based Architecture\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/ccnc51644.2023.10059701"
     },
     {
         "DOI": "10.1145/3543873.3589756",
-        "NAME": "Trusting Decentralised Knowledge Graphs and Web Data at the Web Conference",
+        "NAME": "\"Trusting Decentralised Knowledge Graphs and Web Data at the Web Conference\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1145/3543873.3589756"
     },
     {
         "DOI": "10.1109/ACCESS.2023.3276240",
-        "NAME": "Accountable Clouds through Blockchain",
+        "NAME": "\"Accountable Clouds through Blockchain\"",
         "PRIMARY_LOCATION": "https://ieeexplore.ieee.org/ielx7/6287639/10005208/10124222.pdf"
     },
     {
         "DOI": "10.3233/SW-210451",
-        "NAME": "Applying the LOT Methodology to a Public Bus Transport Ontology aligned with Transmodel: Challenges and Results",
+        "NAME": "\"Applying the LOT Methodology to a Public Bus Transport Ontology aligned with Transmodel: Challenges and Results\"",
         "PRIMARY_LOCATION": "https://content.iospress.com:443/download/semantic-web/sw210451?id=semantic-web%2Fsw210451"
     },
     {
         "DOI": "10.3233/SW-223278",
-        "NAME": "Editorial of transport data on the web",
+        "NAME": "\"Editorial of transport data on the web\"",
         "PRIMARY_LOCATION": "https://content.iospress.com:443/download/semantic-web/sw223278?id=semantic-web%2Fsw223278"
     },
     {
         "DOI": "10.1007/978-3-031-33455-9_29",
-        "NAME": "Boosting Knowledge Graph Generation from\u00a0Tabular Data with\u00a0RML Views",
+        "NAME": "\"Boosting Knowledge Graph Generation from\u00a0Tabular Data with\u00a0RML Views\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-031-33455-9_29"
     },
     {
         "DOI": "10.5334/cstp.538",
-        "NAME": "Data Management Documentation in Citizen Science Projects: Bringing Formalisation and Transparency Together",
+        "NAME": "\"Data Management Documentation in Citizen Science Projects: Bringing Formalisation and Transparency Together\"",
         "PRIMARY_LOCATION": "https://storage.googleapis.com/jnl-up-j-cstp-files/journals/1/articles/538/647dce1d15fad.pdf"
     },
     {
         "DOI": "10.1007/978-3-031-38079-2_9",
-        "NAME": "Analysis of the Confidence in the Prediction of the Protein Folding by Artificial Intelligence",
+        "NAME": "\"Analysis of the Confidence in the Prediction of the Protein Folding by Artificial Intelligence\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-031-38079-2_9"
     },
     {
         "DOI": "10.1007/978-3-031-47240-4_15",
-        "NAME": "Comparison of\u00a0Knowledge Graph Representations for\u00a0Consumer Scenarios",
+        "NAME": "\"Comparison of\u00a0Knowledge Graph Representations for\u00a0Consumer Scenarios\"",
         "PRIMARY_LOCATION": "https://link.springer.com/content/pdf/10.1007/978-3-031-47240-4_15.pdf"
     },
     {
         "DOI": "10.1007/978-3-031-47243-5_9",
-        "NAME": "The RML Ontology: A Community-Driven Modular Redesign After a Decade of Experience in Mapping Heterogeneous Data to RDF",
+        "NAME": "\"The RML Ontology: A Community-Driven Modular Redesign After a Decade of Experience in Mapping Heterogeneous Data to RDF\"",
         "PRIMARY_LOCATION": "https://link.springer.com/content/pdf/10.1007/978-3-031-47243-5_9.pdf"
     },
     {
-        "DOI": "10.1109/CBMS58004.2023.00043",
-        "NAME": "Enhancing drug repurposing on graphs by integrating drug molecular structure as feature",
-        "PRIMARY_LOCATION": "https://www.biorxiv.org/content/biorxiv/early/2023/05/04/2023.05.03.539227.full.pdf"
+        "DOI": "10.1145/3587259.3627574",
+        "NAME": "\"Automatic Topic Label Generation using Conversational Models\"",
+        "PRIMARY_LOCATION": "https://doi.org/10.1145/3587259.3627574"
+    },
+    {
+        "DOI": "10.1109/CBMS58004.2023.00215",
+        "NAME": "\"Enhancing drug repurposing on graphs by integrating drug molecular structure as feature\"",
+        "PRIMARY_LOCATION": "https://doi.org/10.1109/cbms58004.2023.00215"
     },
     {
         "DOI": "10.1007/978-3-031-48539-8_15",
-        "NAME": "Pody: A Solid-Based Approach to\u00a0Embody Agents in\u00a0Web-Based Multi-Agent-Systems",
+        "NAME": "\"Pody: A Solid-Based Approach to\u00a0Embody Agents in\u00a0Web-Based Multi-Agent-Systems\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-031-48539-8_15"
     },
     {
         "DOI": "10.3233/FAIA230983",
-        "NAME": "Event Extraction and Semantic Representation from Spanish Workers Statute Using Large Language Models",
+        "NAME": "\"Event Extraction and Semantic Representation from Spanish Workers Statute Using Large Language Models\"",
         "PRIMARY_LOCATION": "https://ebooks.iospress.nl/pdf/doi/10.3233/FAIA230983"
     },
     {
         "DOI": "10.1016/j.jbi.2023.104382",
-        "NAME": "Lessons learned to enable question answering on knowledge graphs extracted from scientific publications: A case study on the coronavirus literature",
+        "NAME": "\"Lessons learned to enable question answering on knowledge graphs extracted from scientific publications: A case study on the coronavirus literature\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.jbi.2023.104382"
     },
     {
         "DOI": "10.1049/ntw2.12037",
-        "NAME": "Complex queries over decentralised systems for geodata retrieval",
+        "NAME": "\"Complex queries over decentralised systems for geodata retrieval\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1049/ntw2.12037"
     },
     {
         "DOI": "10.1016/j.neucom.2022.12.010",
-        "NAME": "GEnI: A framework for the generation of explanations and insights of knowledge graph embedding predictions",
+        "NAME": "\"GEnI: A framework for the generation of explanations and insights of knowledge graph embedding predictions\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.neucom.2022.12.010"
     },
     {
         "DOI": "10.1109/CIoT57267.2023.10084897",
-        "NAME": "Dimensionality-reducing classifiers for Spanish winter maintenance of roadways",
+        "NAME": "\"Dimensionality-reducing classifiers for Spanish winter maintenance of roadways\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/ciot57267.2023.10084897"
     },
     {
         "DOI": "10.1145/3543873.3587359",
-        "NAME": "Depicting Vocabulary Summaries with Devos",
+        "NAME": "\"Depicting Vocabulary Summaries with Devos\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1145/3543873.3587359"
     },
     {
         "DOI": "10.1145/3543873.3587358",
-        "NAME": "Injecting data into ODRL privacy policies dynamically with RDF mappings",
+        "NAME": "\"Injecting data into ODRL privacy policies dynamically with RDF mappings\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1145/3543873.3587358"
     },
     {
         "DOI": "10.1145/3543873.3589745",
-        "NAME": "The First International Workshop on Knowledge Graphs for Sustainability - KG4S Foreword",
+        "NAME": "\"The First International Workshop on Knowledge Graphs for Sustainability - KG4S Foreword\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1145/3543873.3589745"
     },
     {
         "DOI": "10.1145/3543873.3587628",
-        "NAME": "Practical challenges of ODRL and potential courses of action",
+        "NAME": "\"Practical challenges of ODRL and potential courses of action\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1145/3543873.3587628"
     },
     {
         "DOI": "10.1109/PDP59025.2023.00035",
-        "NAME": "Distributed training and inference of deep learning solar energy forecasting models",
+        "NAME": "\"Distributed training and inference of deep learning solar energy forecasting models\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/pdp59025.2023.00035"
     },
     {
         "DOI": "10.1002/9781119899457.ch7",
-        "NAME": "The ETSI SAREF Ontology for Smart Applications: A Long Path of Development and Evolution",
+        "NAME": "\"The ETSI SAREF Ontology for Smart Applications: A Long Path of Development and Evolution\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1002/9781119899457.ch7"
     },
     {
         "DOI": "10.1007/s10489-022-04175-y",
-        "NAME": "A combination of supervised dimensionality reduction and learning methods to forecast solar radiation",
+        "NAME": "\"A combination of supervised dimensionality reduction and learning methods to forecast solar radiation\"",
         "PRIMARY_LOCATION": "https://link.springer.com/content/pdf/10.1007/s10489-022-04175-y.pdf"
     },
     {
         "DOI": null,
         "NAME": "FAIR-IMPACT project response to\" FAIR Assessment Tools: Towards an\" Apples to Apples\" Comparisons\"",
         "PRIMARY_LOCATION": null
     },
@@ -307,15 +307,15 @@
     {
         "DOI": null,
         "NAME": "Declarative generation of RDF-star graphs from heterogeneous data",
         "PRIMARY_LOCATION": "https://content.iospress.com:443/download/semantic-web/sw243602?id=semantic-web%2Fsw243602"
     },
     {
         "DOI": "10.1007/978-3-031-34444-2_19",
-        "NAME": "Human-Friendly RDF Graph Construction: Which one do you chose?",
+        "NAME": "\"Human-Friendly RDF Graph Construction: Which one do you chose?\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-031-34444-2_19"
     },
     {
         "DOI": null,
         "NAME": "Morph-KGC: declarative generation of RDF-star graphs from heterogeneous data",
         "PRIMARY_LOCATION": null
     },
@@ -337,15 +337,15 @@
     {
         "DOI": null,
         "NAME": "Preface for the 4th Edition of the International Knowledge Graph Construction Workshop",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.1007/978-3-031-47240-4_15",
-        "NAME": "Comparison of Knowledge Graph Representations for Consumer Scenarios",
+        "NAME": "\"Comparison of Knowledge Graph Representations for Consumer Scenarios\"",
         "PRIMARY_LOCATION": "https://link.springer.com/content/pdf/10.1007/978-3-031-47240-4_15.pdf"
     },
     {
         "DOI": null,
         "NAME": "Towards a UML-based notation for OWL ontologies",
         "PRIMARY_LOCATION": null
     },
@@ -357,50 +357,50 @@
     {
         "DOI": null,
         "NAME": "Towards Assessing FAIR Research Software Best Practices in an Organization Using RDF-star",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.1007/978-3-031-47243-5_5",
-        "NAME": "TEC: Transparent Emissions Calculation Toolkit",
+        "NAME": "\"TEC: Transparent Emissions Calculation Toolkit\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-031-47243-5_5"
     },
     {
         "DOI": null,
         "NAME": "ELAINE: rELiAbility and evIdence-aware News vErifier",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.1109/ICDCSW60045.2023.00016",
-        "NAME": "Proof of Location through a Blockchain Agnostic Smart Contract Language",
+        "NAME": "\"Proof of Location through a Blockchain Agnostic Smart Contract Language\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/icdcsw60045.2023.00016"
     },
     {
         "DOI": "10.1145/3587259.3627554",
-        "NAME": "Re-Construction Impact on Metadata Representation Models",
+        "NAME": "\"Re-Construction Impact on Metadata Representation Models\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1145/3587259.3627554"
     },
     {
         "DOI": "10.1109/BCCA58897.2023.10338895",
-        "NAME": "DLT-Based Personal Data Access Control with Key-Redistribution",
+        "NAME": "\"DLT-Based Personal Data Access Control with Key-Redistribution\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/bcca58897.2023.10338895"
     },
     {
         "DOI": "10.1145/3555776.3577692",
-        "NAME": "Interoperability of Heterogeneous Systems of Systems: Review of Challenges, Emerging Requirements and Options",
+        "NAME": "\"Interoperability of Heterogeneous Systems of Systems: Review of Challenges, Emerging Requirements and Options\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1145/3555776.3577692"
     },
     {
         "DOI": "10.1109/PerComWorkshops56833.2023.10150302",
-        "NAME": "On the Use of Deep Neural Networks for Security Vulnerabilities Detection in Smart Contracts",
+        "NAME": "\"On the Use of Deep Neural Networks for Security Vulnerabilities Detection in Smart Contracts\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/percomworkshops56833.2023.10150302"
     },
     {
         "DOI": "10.1007/978-3-031-42280-5_12",
-        "NAME": "Towards an\u00a0Automatic Easy-to-Read Adaptation of\u00a0Morphological Features in\u00a0Spanish Texts",
+        "NAME": "\"Towards an\u00a0Automatic Easy-to-Read Adaptation of\u00a0Morphological Features in\u00a0Spanish Texts\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-031-42280-5_12"
     },
     {
         "DOI": null,
         "NAME": "ACM K-CAP 2023 Chairs' Welcome",
         "PRIMARY_LOCATION": null
     },
@@ -427,59 +427,64 @@
     {
         "DOI": null,
         "NAME": "Preface",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/s0304-0208(06)80001-0"
     },
     {
         "DOI": "10.1007/978-3-031-32213-6_10",
-        "NAME": "Building a\u00a0Knowledge Graph from\u00a0Historical Newspapers: A Study Case in\u00a0Ecuador",
+        "NAME": "\"Building a\u00a0Knowledge Graph from\u00a0Historical Newspapers: A Study Case in\u00a0Ecuador\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-031-32213-6_10"
     },
     {
         "DOI": null,
         "NAME": "Preface of the Joint Workshop Proceedings of the 5th Sem4Tra Workshop, and 2nd NLP4KGC Workshop co-located with SEMANTiCS 2023",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.1145/3587259.3627565",
-        "NAME": "XSD2SHACL: Capturing RDF Constraints from XML Schema",
+        "NAME": "\"XSD2SHACL: Capturing RDF Constraints from XML Schema\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1145/3587259.3627565"
     },
     {
         "DOI": null,
         "NAME": "The 4th Wikidata Workshop - Wikidata Workshop 2023",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.13052/jwe1540-9589.2284",
-        "NAME": "LUBM4OBDA: Benchmarking OBDA Systems with Inference and Meta Knowledge",
+        "NAME": "\"LUBM4OBDA: Benchmarking OBDA Systems with Inference and Meta Knowledge\"",
         "PRIMARY_LOCATION": "https://journals.riverpublishers.com/index.php/JWE/article/download/18845/19479"
     },
     {
         "DOI": null,
         "NAME": "Companion Proceedings of the 23rd International Conference on Knowledge Engineering and Knowledge Management",
         "PRIMARY_LOCATION": null
     },
     {
-        "DOI": "10.1016/j.annepidem.2022.08.036",
-        "NAME": "Phenotypes of non-alcoholic fatty liver disease (NAFLD) and all-cause mortality: unsupervised machine learning analysis of NHANES III",
-        "PRIMARY_LOCATION": "https://doi.org/10.1016/j.annepidem.2022.08.036"
+        "DOI": "10.1136/bmjopen-2022-067203",
+        "NAME": "\"Phenotypes of non-alcoholic fatty liver disease (NAFLD) and all-cause mortality: unsupervised machine learning analysis of NHANES III\"",
+        "PRIMARY_LOCATION": "https://bmjopen.bmj.com/content/bmjopen/12/11/e067203.full.pdf"
     },
     {
         "DOI": "10.9781/ijimai.2022.11.001",
-        "NAME": "OBOE: an Explainable Text Classification Framework",
+        "NAME": "\"OBOE: an Explainable Text Classification Framework\"",
         "PRIMARY_LOCATION": "https://doi.org/10.9781/ijimai.2022.11.001"
     },
     {
         "DOI": "10.12688/wellcomeopenres.16867.5",
-        "NAME": "Government plans in the 2016 and 2021 Peruvian presidential elections: A natural language processing analysis of the health chapters",
+        "NAME": "\"Government plans in the 2016 and 2021 Peruvian presidential elections: A natural language processing analysis of the health chapters\"",
         "PRIMARY_LOCATION": "https://doi.org/10.12688/wellcomeopenres.16867.5"
     },
     {
         "DOI": "10.3897/rio.8.e95943",
+        "NAME": "\"Challenges for FAIR Digital Object Assessment\"",
+        "PRIMARY_LOCATION": "https://riojournal.com/article/95943/download/pdf/"
+    },
+    {
+        "DOI": null,
         "NAME": "Challenges for FAIR Digital Object Assessment",
         "PRIMARY_LOCATION": "https://riojournal.com/article/95943/download/pdf/"
     },
     {
         "DOI": null,
         "NAME": "A Systematic Review of Ontologies for the Water Domain",
         "PRIMARY_LOCATION": "https://doi.org/10.1002/9781394171460.ch2"
@@ -497,45 +502,45 @@
     {
         "DOI": null,
         "NAME": "The implications of natural language processing for public performance management: a systematic literature review",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.26342/2022-69-9",
-        "NAME": "Extraction and Semantic Representation of Domain-Specific Relations in Spanish Labour Law",
+        "NAME": "\"Extraction and Semantic Representation of Domain-Specific Relations in Spanish Labour Law\"",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.26342/2022-69-14",
-        "NAME": "An Overview of Drugs, Diseases, Genes and Proteins in the CORD-19 Corpus [Una visi\u00f3n general de los F\u00e1rmacos, Enfermedades, Genes y Prote\u00ednas en el corpus CORD-19]",
+        "NAME": "\"An Overview of Drugs, Diseases, Genes and Proteins in the CORD-19 Corpus [Una visi\u00f3n general de los F\u00e1rmacos, Enfermedades, Genes y Prote\u00ednas en el corpus CORD-19]\"",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.26342/2022-69-6",
-        "NAME": "Multi-label Text Classification for Public Procurement in Spanish [Clasificaci\u00f3n multi-etiqueta de textos de licitaciones p\u00fablicas en espa\u00f1ol]",
+        "NAME": "\"Multi-label Text Classification for Public Procurement in Spanish [Clasificaci\u00f3n multi-etiqueta de textos de licitaciones p\u00fablicas en espa\u00f1ol]\"",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": null,
         "NAME": "WoTHive: Enabling Syntactic and Semantic Discovery in the Web of Things",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.7717/PEERJ-CS.1023",
-        "NAME": "Nine best practices for research software registries and repositories",
+        "NAME": "\"Nine best practices for research software registries and repositories\"",
         "PRIMARY_LOCATION": "https://doi.org/10.7717/peerj-cs.1023"
     },
     {
         "DOI": "10.5281/zenodo.7007495",
-        "NAME": "Ontology Management in an Industrial Environment: The BASF Governance Operational Model for Ontologies (GOMO)",
+        "NAME": "\"Ontology Management in an Industrial Environment: The BASF Governance Operational Model for Ontologies (GOMO)\"",
         "PRIMARY_LOCATION": "https://zenodo.org/records/7007495/files/bio-ontologies%20paper%20GOMO.pdf"
     },
     {
         "DOI": "10.3233/SW-223009",
-        "NAME": "Analysis of ontologies and policy languages to represent information flows in GDPR",
+        "NAME": "\"Analysis of ontologies and policy languages to represent information flows in GDPR\"",
         "PRIMARY_LOCATION": "https://content.iospress.com:443/download/semantic-web/sw223009?id=semantic-web%2Fsw223009"
     },
     {
         "DOI": null,
         "NAME": "A low-cost method for text summarization",
         "PRIMARY_LOCATION": null
     },
@@ -547,325 +552,330 @@
     {
         "DOI": null,
         "NAME": "Proceedings of the 3rd International Workshop on Semantic Digital Twins (SeDiT 2022)",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.15497/RDA00068",
-        "NAME": "FAIR Principles for Research Software (FAIR4RS Principles)",
-        "PRIMARY_LOCATION": "https://zenodo.org/records/4908919/files/FAIR4RS%20Subgroup%204%20Report%20v0.1.pdf"
+        "NAME": "\"FAIR Principles for Research Software (FAIR4RS Principles)\"",
+        "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.1016/j.is.2021.101966",
-        "NAME": "Lynx: A knowledge-based AI service platform for content processing, enrichment and analysis for the legal domain",
+        "NAME": "\"Lynx: A knowledge-based AI service platform for content processing, enrichment and analysis for the legal domain\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.is.2021.101966"
     },
     {
         "DOI": null,
         "NAME": "Technologies and Applications for Big Data Value",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-78307-5"
     },
     {
         "DOI": "10.1007/978-3-030-78307-5_12",
-        "NAME": "Using a Legal Knowledge Graph for Multilingual Compliance Services in Labor Law, Contract Management, and Geothermal Energy",
+        "NAME": "\"Using a Legal Knowledge Graph for Multilingual Compliance Services in Labor Law, Contract Management, and Geothermal Energy\"",
         "PRIMARY_LOCATION": "https://link.springer.com/content/pdf/10.1007/978-3-030-78307-5_12.pdf"
     },
     {
         "DOI": "10.1162/qss_a_00167",
-        "NAME": "A framework for creating knowledge graphs of scientific software metadata",
+        "NAME": "\"A framework for creating knowledge graphs of scientific software metadata\"",
         "PRIMARY_LOCATION": "https://direct.mit.edu/qss/article-pdf/2/4/1423/2007844/qss_a_00167.pdf"
     },
     {
         "DOI": null,
         "NAME": "Towards Smart, Digitalised Rural Regions And Communities - Policies, Best Practices And Case Studies",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": null,
         "NAME": "Proceedings of the 9th Linked Data in Architecture and Construction Workshop (LDAC2021)",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.51305/icl.cz.9788076580336.02",
-        "NAME": "Description of Postdata Poetry Ontology V1.0",
+        "NAME": "\"Description of Postdata Poetry Ontology V1.0\"",
         "PRIMARY_LOCATION": "https://www.plottingpoetry.org/books/tackling_toolkit/pdf/02_diezplatas.pdf"
     },
     {
-        "DOI": "10.7554/eLife.72930; 10.7554/eLife.72930.sa0; 10.7554/eLife.72930.sa1; 10.7554/eLife.72930.sa2",
-        "NAME": "Development, validation, and application of a machine learning model to estimate salt consumption in 54 countries",
-        "PRIMARY_LOCATION": null
+        "DOI": "10.7554/eLife.72930",
+        "NAME": "\"Development, validation, and application of a machine learning model to estimate salt consumption in 54 countries\"",
+        "PRIMARY_LOCATION": "https://doi.org/10.7554/elife.72930"
     },
     {
         "DOI": "10.7554/elife.72930.sa2",
-        "NAME": "Author response: Development, validation, and application of a machine learning model to estimate salt consumption in 54 countries",
+        "NAME": "\"Author response: Development, validation, and application of a machine learning model to estimate salt consumption in 54 countries\"",
         "PRIMARY_LOCATION": "https://doi.org/10.7554/elife.72930.sa2"
     },
     {
         "DOI": "10.7554/eLife.72930",
-        "NAME": "Estimating  salt consumption  in  49  low-  and  middle-income  countries:  Development, validation and application of a machine learning model",
+        "NAME": "\"Estimating  salt consumption  in  49  low-  and  middle-income  countries:  Development, validation and application of a machine learning model\"",
         "PRIMARY_LOCATION": "https://doi.org/10.7554/elife.72930"
     },
     {
         "DOI": "10.1002/ett.3729",
-        "NAME": "Context aware ontology-based hybrid intelligent framework for vehicle driver categorization",
+        "NAME": "\"Context aware ontology-based hybrid intelligent framework for vehicle driver categorization\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1002/ett.3729"
     },
     {
         "DOI": "10.1016/j.eswa.2021.116100",
-        "NAME": "Rule extraction in unsupervised anomaly detection for model explainability: Application to OneClass SVM[Formula presented]",
+        "NAME": "\"Rule extraction in unsupervised anomaly detection for model explainability: Application to OneClass SVM[Formula presented]\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.eswa.2021.116100"
     },
     {
         "DOI": "10.1111/tgis.12863",
-        "NAME": "Annotating OGC web feature services automatically for generating geospatial knowledge graphs",
+        "NAME": "\"Annotating OGC web feature services automatically for generating geospatial knowledge graphs\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1111/tgis.12863"
     },
     {
         "DOI": "10.1080/10095020.2021.2015250",
-        "NAME": "A graph-based representation of knowledge for managing land administration data from distributed agencies - A case study of Colombia",
+        "NAME": "\"A graph-based representation of knowledge for managing land administration data from distributed agencies - A case study of Colombia\"",
         "PRIMARY_LOCATION": "https://www.tandfonline.com/doi/pdf/10.1080/10095020.2021.2015250?needAccess=true"
     },
     {
         "DOI": "10.3233/SW-210442",
-        "NAME": "TheyBuyForYou platform and knowledge graph: Expanding horizons in public procurement with open linked data",
+        "NAME": "\"TheyBuyForYou platform and knowledge graph: Expanding horizons in public procurement with open linked data\"",
         "PRIMARY_LOCATION": "https://content.iospress.com:443/download/semantic-web/sw210442?id=semantic-web%2Fsw210442"
     },
     {
         "DOI": "10.1016/j.websem.2021.100679",
-        "NAME": "A study of the quality of Wikidata",
+        "NAME": "\"A study of the quality of Wikidata\"",
         "PRIMARY_LOCATION": "http://manuscript.elsevier.com/S1570826821000536/pdf/S1570826821000536.pdf"
     },
     {
         "DOI": "10.3390/info13020099",
-        "NAME": "Data Quality Barriers for Transparency in Public Procurement",
+        "NAME": "\"Data Quality Barriers for Transparency in Public Procurement\"",
         "PRIMARY_LOCATION": "https://www.mdpi.com/2078-2489/13/2/99/pdf?version=1645523351"
     },
     {
         "DOI": "10.1016/j.engappai.2022.104755",
-        "NAME": "LOT: An industrial oriented ontology engineering framework",
+        "NAME": "\"LOT: An industrial oriented ontology engineering framework\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.engappai.2022.104755"
     },
     {
         "DOI": "10.5220/0010945300003116",
-        "NAME": "Intelligent Human-input-based Blockchain Oracle (IHiBO)",
+        "NAME": "\"Intelligent Human-input-based Blockchain Oracle (IHiBO)\"",
         "PRIMARY_LOCATION": "https://doi.org/10.5220/0010945300003116"
     },
     {
         "DOI": "10.1007/s42979-022-01097-x",
-        "NAME": "PHDD: Corpus of Physical Health Data Disclosure on Twitter During COVID-19 Pandemic",
+        "NAME": "\"PHDD: Corpus of Physical Health Data Disclosure on Twitter During COVID-19 Pandemic\"",
         "PRIMARY_LOCATION": "https://link.springer.com/content/pdf/10.1007/s42979-022-01097-x.pdf"
     },
     {
         "DOI": "10.1016/j.neucom.2022.04.087",
-        "NAME": "Multi-object tracking in traffic environments: A systematic literature review",
+        "NAME": "\"Multi-object tracking in traffic environments: A systematic literature review\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.neucom.2022.04.087"
     },
     {
         "DOI": "10.1145/3477314.3507078",
-        "NAME": "Towards CBDC-based machine-to-machine payments in consumer IoT",
+        "NAME": "\"Towards CBDC-based machine-to-machine payments in consumer IoT\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1145/3477314.3507078"
     },
     {
         "DOI": "10.3233/SW-212895",
-        "NAME": "Handling qualitative preferences in SPARQL over virtual ontology-based data access",
+        "NAME": "\"Handling qualitative preferences in SPARQL over virtual ontology-based data access\"",
         "PRIMARY_LOCATION": "https://content.iospress.com:443/download/semantic-web/sw212895?id=semantic-web%2Fsw212895"
     },
     {
         "DOI": "10.1007/978-3-031-08473-7_14",
-        "NAME": "Extracting and Understanding Call-to-actions of Push-Notifications",
+        "NAME": "\"Extracting and Understanding Call-to-actions of Push-Notifications\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-031-08473-7_14"
     },
     {
         "DOI": "10.1145/3524842.3528497",
-        "NAME": "Inspect4py: A Knowledge Extraction Framework for Python Code Repositories",
+        "NAME": "\"Inspect4py: A Knowledge Extraction Framework for Python Code Repositories\"",
         "PRIMARY_LOCATION": "https://dl.acm.org/doi/pdf/10.1145/3524842.3528497"
     },
     {
         "DOI": "10.1109/ICBC54727.2022.9805515",
-        "NAME": "Incentivized Data Mules Based on State-Channels",
+        "NAME": "\"Incentivized Data Mules Based on State-Channels\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/icbc54727.2022.9805515"
     },
     {
         "DOI": "10.1007/978-3-031-11609-4_3",
-        "NAME": "Using the\u00a0ODRL Profile for\u00a0Access Control for\u00a0Solid Pod Resource Governance",
+        "NAME": "\"Using the\u00a0ODRL Profile for\u00a0Access Control for\u00a0Solid Pod Resource Governance\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-031-11609-4_3"
     },
     {
         "DOI": "10.1016/j.engappai.2022.105222",
-        "NAME": "Interpretable machine learning models for predicting and explaining vehicle fuel consumption anomalies",
+        "NAME": "\"Interpretable machine learning models for predicting and explaining vehicle fuel consumption anomalies\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.engappai.2022.105222"
     },
     {
         "DOI": "10.1007/s10586-022-03691-3",
-        "NAME": "Data governance through a multi-DLT architecture in view of the GDPR",
+        "NAME": "\"Data governance through a multi-DLT architecture in view of the GDPR\"",
         "PRIMARY_LOCATION": "https://link.springer.com/content/pdf/10.1007/s10586-022-03691-3.pdf"
     },
     {
         "DOI": "10.3390/s22166260",
-        "NAME": "Decentralized Personal Data Marketplaces: How Participation in a DAO Can Support the Production of Citizen-Generated Data",
+        "NAME": "\"Decentralized Personal Data Marketplaces: How Participation in a DAO Can Support the Production of Citizen-Generated Data\"",
         "PRIMARY_LOCATION": "https://www.mdpi.com/1424-8220/22/16/6260/pdf?version=1661238706"
     },
     {
         "DOI": "10.1145/3487553.3547182",
-        "NAME": "Accepted Tutorials at The Web Conference 2022",
+        "NAME": "\"Accepted Tutorials at The Web Conference 2022\"",
         "PRIMARY_LOCATION": "https://dl.acm.org/doi/pdf/10.1145/3487553.3547182"
     },
     {
         "DOI": "10.1145/3524458.3547230",
-        "NAME": "The impact of NFT profile pictures within social network communities",
+        "NAME": "\"The impact of NFT profile pictures within social network communities\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1145/3524458.3547230"
     },
     {
         "DOI": "10.1109/ICCCN54977.2022.9868916",
-        "NAME": "DLT-based Data Mules for Smart Territories",
+        "NAME": "\"DLT-based Data Mules for Smart Territories\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/icccn54977.2022.9868916"
     },
     {
         "DOI": "10.3233/SW-222885",
-        "NAME": "TermitUp: Generation and enrichment of linked terminologies",
+        "NAME": "\"TermitUp: Generation and enrichment of linked terminologies\"",
         "PRIMARY_LOCATION": "https://content.iospress.com:443/download/semantic-web/sw222885?id=semantic-web%2Fsw222885"
     },
     {
         "DOI": "10.1109/Blockchain55522.2022.00023",
-        "NAME": "Decentralized Health Data Distribution: A DLT-based Architecture for Data Protection",
+        "NAME": "\"Decentralized Health Data Distribution: A DLT-based Architecture for Data Protection\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/blockchain55522.2022.00023"
     },
     {
         "DOI": "10.1007/978-3-031-17105-5_2",
-        "NAME": "Extending Ontology Engineering Practices to\u00a0Facilitate Application Development",
+        "NAME": "\"Extending Ontology Engineering Practices to\u00a0Facilitate Application Development\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-031-17105-5_2"
     },
     {
         "DOI": "10.1007/978-3-031-17105-5_11",
-        "NAME": "EBOCA: Evidences for BiOmedical Concepts Association Ontology",
+        "NAME": "\"EBOCA: Evidences for BiOmedical Concepts Association Ontology\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-031-17105-5_11"
     },
     {
         "DOI": "10.1109/DS-RT55542.2022.9932122",
-        "NAME": "Simulation of the Internet Computer Protocol: the Next Generation Multi-Blockchain Architecture",
+        "NAME": "\"Simulation of the Internet Computer Protocol: the Next Generation Multi-Blockchain Architecture\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/ds-rt55542.2022.9932122"
     },
     {
         "DOI": "10.1007/978-3-031-07535-3_20",
-        "NAME": "Blockchain-Based Data Management for Smart Transportation",
+        "NAME": "\"Blockchain-Based Data Management for Smart Transportation\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-031-07535-3_20"
     },
     {
         "DOI": "10.3390/info13120562",
-        "NAME": "Systematic Construction of Knowledge Graphs for Research-Performing Organizations",
+        "NAME": "\"Systematic Construction of Knowledge Graphs for Research-Performing Organizations\"",
         "PRIMARY_LOCATION": "https://www.mdpi.com/2078-2489/13/12/562/pdf?version=1669804108"
     },
     {
         "DOI": "10.1109/TransAI54797.2022.00007",
-        "NAME": "Towards a Taxonomy of AI Risks in the Health Domain",
+        "NAME": "\"Towards a Taxonomy of AI Risks in the Health Domain\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/transai54797.2022.00007"
     },
     {
         "DOI": "10.1145/3565011.3569061",
-        "NAME": "Fostering trust with transparency in the data economy era: An integrated ethical, legal, and knowledge engineering approach",
+        "NAME": "\"Fostering trust with transparency in the data economy era: An integrated ethical, legal, and knowledge engineering approach\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1145/3565011.3569061"
     },
     {
         "DOI": "10.1007/978-3-031-20436-4_4",
-        "NAME": "Now, Later, Never: A Study of\u00a0Urgency in\u00a0Mobile Push-Notifications",
+        "NAME": "\"Now, Later, Never: A Study of\u00a0Urgency in\u00a0Mobile Push-Notifications\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-031-20436-4_4"
     },
     {
         "DOI": "10.12688/openreseurope.15280.1",
-        "NAME": "An extension of Thing Descriptions from the Web of Things for Digital Twins",
+        "NAME": "\"An extension of Thing Descriptions from the Web of Things for Digital Twins\"",
         "PRIMARY_LOCATION": "https://doi.org/10.12688/openreseurope.15280.1"
     },
     {
         "DOI": "10.3233/FAIA220462",
-        "NAME": "Automating the Response to GDPR's Right of Access",
+        "NAME": "\"Automating the Response to GDPR's Right of Access\"",
         "PRIMARY_LOCATION": "https://ebooks.iospress.nl/pdf/doi/10.3233/FAIA220462"
     },
     {
         "DOI": "10.3233/FAIA220470",
-        "NAME": "WhenTheFact: Extracting Events from European Legal Decisions",
+        "NAME": "\"WhenTheFact: Extracting Events from European Legal Decisions\"",
         "PRIMARY_LOCATION": "https://ebooks.iospress.nl/pdf/doi/10.3233/FAIA220470"
     },
     {
         "DOI": "10.1145/3560905.3568175",
-        "NAME": "Smart Contracts Vulnerability Classification through Deep Learning",
+        "NAME": "\"Smart Contracts Vulnerability Classification through Deep Learning\"",
         "PRIMARY_LOCATION": "https://dl.acm.org/doi/pdf/10.1145/3560905.3568175"
     },
     {
         "DOI": "10.3233/DS-210053",
-        "NAME": "Packaging research artefacts with RO-Crate",
+        "NAME": "\"Packaging research artefacts with RO-Crate\"",
         "PRIMARY_LOCATION": "https://content.iospress.com:443/download/data-science/ds210053?id=data-science%2Fds210053"
     },
     {
+        "DOI": null,
+        "NAME": "Apports des methodologies et techniques de developpement logiciel pour l'ingenierie des ontologies: Retour d'experience des contributions au developpement de l'ontologie ETSI SAREF",
+        "PRIMARY_LOCATION": null
+    },
+    {
         "DOI": "10.3390/ijgi11020086",
-        "NAME": "Bringing Federated Semantic Queries to the GIS-Based Scenario",
+        "NAME": "\"Bringing Federated Semantic Queries to the GIS-Based Scenario\"",
         "PRIMARY_LOCATION": "https://www.mdpi.com/2220-9964/11/2/86/pdf?version=1643204664"
     },
     {
         "DOI": "10.2166/hydro.2022.070",
-        "NAME": "Characterizing water quality datasets through multi-dimensional knowledge graphs: a case study of the Bogota river basin",
+        "NAME": "\"Characterizing water quality datasets through multi-dimensional knowledge graphs: a case study of the Bogota river basin\"",
         "PRIMARY_LOCATION": "https://iwaponline.com/jh/article-pdf/24/2/295/1030721/jh0240295.pdf"
     },
     {
         "DOI": "10.22201/iibi.24488321xe.2022.91.58538",
-        "NAME": "Characterization of urban risks in the press applying text mining for the enrichment of open data Luis M. Vilches-Bl\u00e1zquez and Diana Comesa\u00f1a Ocampo [Caracterizaci\u00f3n de riesgos urbanos en prensa aplicando miner\u00eda de texto para el enriquecimiento de datos abiertos]",
+        "NAME": "\"Characterization of urban risks in the press applying text mining for the enrichment of open data Luis M. Vilches-Bl\u00e1zquez and Diana Comesa\u00f1a Ocampo [Caracterizaci\u00f3n de riesgos urbanos en prensa aplicando miner\u00eda de texto para el enriquecimiento de datos abiertos]\"",
         "PRIMARY_LOCATION": "http://rev-ib.unam.mx/ib/index.php/ib/article/download/58538/52254"
     },
     {
         "DOI": "10.1016/j.ins.2021.09.011",
-        "NAME": "Ontology verification testing using lexico-syntactic patterns",
+        "NAME": "\"Ontology verification testing using lexico-syntactic patterns\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.ins.2021.09.011"
     },
     {
         "DOI": "10.1016/j.knosys.2021.108092",
-        "NAME": "Balancing coverage and specificity for semantic labelling of subject columns",
+        "NAME": "\"Balancing coverage and specificity for semantic labelling of subject columns\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.knosys.2021.108092"
     },
     {
         "DOI": "10.1142/S0218194022500036",
-        "NAME": "DockerPedia: A Knowledge Graph of Software Images and Their Metadata",
+        "NAME": "\"DockerPedia: A Knowledge Graph of Software Images and Their Metadata\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1142/s0218194022500036"
     },
     {
         "DOI": "10.1007/978-3-030-87687-6_11",
-        "NAME": "Multiagent System for the Prediction of Road Maintenance Actions",
+        "NAME": "\"Multiagent System for the Prediction of Road Maintenance Actions\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-87687-6_11"
     },
     {
         "DOI": "10.1007/978-3-030-87687-6_4",
-        "NAME": "Estimating Time Lost on Semaphores with Deep Learning",
+        "NAME": "\"Estimating Time Lost on Semaphores with Deep Learning\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-87687-6_4"
     },
     {
         "DOI": "10.1007/978-3-030-87687-6_10",
-        "NAME": "Intelligent Agent for Roadway Data Analysis",
+        "NAME": "\"Intelligent Agent for Roadway Data Analysis\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-87687-6_10"
     },
     {
         "DOI": "10.1007/978-3-031-06981-9_20",
-        "NAME": "Chowlk: from UML-Based Ontology Conceptualizations to\u00a0OWL",
+        "NAME": "\"Chowlk: from UML-Based Ontology Conceptualizations to\u00a0OWL\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-031-06981-9_20"
     },
     {
         "DOI": "10.1075/tlrp.23.07mon",
-        "NAME": "Terminology and ontologies",
+        "NAME": "\"Terminology and ontologies\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1075/tlrp.23.07mon"
     },
     {
         "DOI": "10.1007/978-3-031-08648-9_48",
-        "NAME": "First Attempt to\u00a0an\u00a0Easy-to-Read Adaptation of\u00a0Repetitions in\u00a0Captions",
+        "NAME": "\"First Attempt to\u00a0an\u00a0Easy-to-Read Adaptation of\u00a0Repetitions in\u00a0Captions\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-031-08648-9_48"
     },
     {
         "DOI": "10.23919/ANNSIM55834.2022.9859513",
-        "NAME": "On The Modeling Of P2P Systems as Temporal Networks: A Case Study With Data Streaming",
+        "NAME": "\"On The Modeling Of P2P Systems as Temporal Networks: A Case Study With Data Streaming\"",
         "PRIMARY_LOCATION": "https://doi.org/10.23919/annsim55834.2022.9859513"
     },
     {
         "DOI": "10.1007/978-3-031-16802-4_6",
-        "NAME": "FAIROs: Towards FAIR Assessment in\u00a0Research Objects",
+        "NAME": "\"FAIROs: Towards FAIR Assessment in\u00a0Research Objects\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-031-16802-4_6"
     },
     {
         "DOI": null,
         "NAME": "Declarative Description of Knowledge Graphs Construction Automation: Status & Challenges",
         "PRIMARY_LOCATION": null
     },
@@ -887,20 +897,35 @@
     {
         "DOI": null,
         "NAME": "Helio: a framework for implementing the life cycle of knowledge graphs",
         "PRIMARY_LOCATION": "https://content.iospress.com:443/download/semantic-web/sw233224?id=semantic-web%2Fsw233224"
     },
     {
         "DOI": null,
+        "NAME": "Estimating Time Lost on Semaphores with Deep Learning",
+        "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-87687-6_4"
+    },
+    {
+        "DOI": null,
+        "NAME": "Intelligent Agent for Roadway Data Analysis",
+        "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-87687-6_10"
+    },
+    {
+        "DOI": null,
+        "NAME": "Multiagent System for the Prediction of Road Maintenance Actions",
+        "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-87687-6_11"
+    },
+    {
+        "DOI": null,
         "NAME": "Representing Multilingual Terminologies with OntoLex-Lemon",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.1136/bmjopen-2022-063411",
-        "NAME": "Street images classification according to COVID-19 risk in Lima, Peru: a convolutional neural networks feasibility analysis",
+        "NAME": "\"Street images classification according to COVID-19 risk in Lima, Peru: a convolutional neural networks feasibility analysis\"",
         "PRIMARY_LOCATION": "https://bmjopen.bmj.com/content/bmjopen/12/9/e063411.full.pdf"
     },
     {
         "DOI": null,
         "NAME": "Proceedings of the 10th Linked Data in Architecture and Construction Workshop (LDAC 2022)",
         "PRIMARY_LOCATION": null
     },
@@ -947,14 +972,19 @@
     {
         "DOI": null,
         "NAME": "A Digital Twin Platform Generating Knowledge Graphs for Construction Projects",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": null,
+        "NAME": "The impact of NFT profile pictures within social network communities",
+        "PRIMARY_LOCATION": "https://doi.org/10.1145/3524458.3547230"
+    },
+    {
+        "DOI": null,
         "NAME": "ON THE MODELING OF P2P SYSTEMS AS TEMPORAL NETWORKS: A CASE STUDY WITH DATA STREAMING",
         "PRIMARY_LOCATION": "https://doi.org/10.23919/annsim55834.2022.9859513"
     },
     {
         "DOI": null,
         "NAME": "Preface - SMART 2022",
         "PRIMARY_LOCATION": "https://doi.org/10.1063/12.0017296"
@@ -962,225 +992,220 @@
     {
         "DOI": null,
         "NAME": "A Spanish Political Tweets Fine-Tuned Sentiment Analysis Model",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-031-14859-0_8"
     },
     {
         "DOI": null,
-        "NAME": "Apports des methodologies et techniques de developpement logiciel pour l'ingenierie des ontologies: Retour d'experience des contributions au developpement de l'ontologie ETSI SAREF",
-        "PRIMARY_LOCATION": null
-    },
-    {
-        "DOI": null,
         "NAME": "Enhancing Trust in Trust Services: Towards an Intelligent Human-input-based Blockchain Oracle (IHiBO)",
         "PRIMARY_LOCATION": "https://doi.org/10.24251/hicss.2022.712"
     },
     {
         "DOI": "10.1016/j.eswa.2021.115731",
-        "NAME": "A hierarchical multi-agent architecture based on virtual identities to explain black-box personalization policies",
+        "NAME": "\"A hierarchical multi-agent architecture based on virtual identities to explain black-box personalization policies\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.eswa.2021.115731"
     },
     {
         "DOI": "10.9781/ijimai.2021.08.011",
-        "NAME": "A case-based reasoning model powered by deep learning for radiology report recommendation",
+        "NAME": "\"A case-based reasoning model powered by deep learning for radiology report recommendation\"",
         "PRIMARY_LOCATION": "https://doi.org/10.9781/ijimai.2021.08.011"
     },
     {
         "DOI": "10.1080/15230406.2021.1952109",
-        "NAME": "Semantic conflation in GIScience: a systematic review",
+        "NAME": "\"Semantic conflation in GIScience: a systematic review\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1080/15230406.2021.1952109"
     },
     {
         "DOI": null,
         "NAME": "Proceedings of the Doctoral Consortium at ISWC 2021",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.1108/DTA-10-2020-0253",
-        "NAME": "An analysis of pollution Citizen Science projects from the perspective of Data Science and Open Science",
+        "NAME": "\"An analysis of pollution Citizen Science projects from the perspective of Data Science and Open Science\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1108/dta-10-2020-0253"
     },
     {
         "DOI": null,
         "NAME": "Analysing Ontological Requirements: A Journey from Requirements to Code and Back",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.26342/2021-67-2",
-        "NAME": "Impact of Text Length for Information Retrieval Tasks based on Probabilistic Topics",
+        "NAME": "\"Impact of Text Length for Information Retrieval Tasks based on Probabilistic Topics\"",
         "PRIMARY_LOCATION": "http://rua.ua.es/dspace/bitstream/10045/117485/1/PLN_67_02.pdf"
     },
     {
         "DOI": "10.3390/app11157033",
-        "NAME": "SPARQL2Flink: Evaluation of SPARQL Queries on Apache Flink",
+        "NAME": "\"SPARQL2Flink: Evaluation of SPARQL Queries on Apache Flink\"",
         "PRIMARY_LOCATION": "https://www.mdpi.com/2076-3417/11/15/7033/pdf?version=1628044316"
     },
     {
         "DOI": "10.3390/su13169168",
-        "NAME": "A Dialogical Approach to Readiness for Change towards Sustainability in Higher Education Institutions: The Case of the SDGs Seminars at the Universidad Politecnica de Madrid",
+        "NAME": "\"A Dialogical Approach to Readiness for Change towards Sustainability in Higher Education Institutions: The Case of the SDGs Seminars at the Universidad Politecnica de Madrid\"",
         "PRIMARY_LOCATION": "https://www.mdpi.com/2071-1050/13/16/9168/pdf?version=1629191461"
     },
     {
         "DOI": "10.21125/edulearn.2021.0165",
-        "NAME": "CHALLENGE-BASED LEARNING IN EXPLAINABLE ARTIFICIAL INTELLIGENCE EDUCATION",
+        "NAME": "\"CHALLENGE-BASED LEARNING IN EXPLAINABLE ARTIFICIAL INTELLIGENCE EDUCATION\"",
         "PRIMARY_LOCATION": "https://doi.org/10.21125/edulearn.2021.0165"
     },
     {
         "DOI": "10.1016/j.ins.2021.02.018",
-        "NAME": "An ontology-based deep learning approach for triple classification with out-of-knowledge-base entities",
+        "NAME": "\"An ontology-based deep learning approach for triple classification with out-of-knowledge-base entities\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.ins.2021.02.018"
     },
     {
         "DOI": "10.1016/j.websem.2021.100655",
-        "NAME": "Crossing the chasm between ontology engineering and application development: A survey",
+        "NAME": "\"Crossing the chasm between ontology engineering and application development: A survey\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.websem.2021.100655"
     },
     {
         "DOI": "10.1145/3453172",
-        "NAME": "Artificial Intelligence for Modeling Complex Systems: Taming the Complexity of Expert Models to Improve Decision Making",
+        "NAME": "\"Artificial Intelligence for Modeling Complex Systems: Taming the Complexity of Expert Models to Improve Decision Making\"",
         "PRIMARY_LOCATION": "https://dl.acm.org/doi/pdf/10.1145/3453172"
     },
     {
         "DOI": null,
         "NAME": "Proceedings of the 2nd International Workshop on Semantic Digital Twins (SeDiT 2021)",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": null,
         "NAME": "First Attempt to help People with Cognitive Disabilities to understand Micropoems",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.1016/j.trd.2021.102784",
-        "NAME": "An estimation of heavy-duty vehicle fleet CO2 emissions based on sampled data",
+        "NAME": "\"An estimation of heavy-duty vehicle fleet CO2 emissions based on sampled data\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.trd.2021.102784"
     },
     {
         "DOI": "10.1007/s10115-021-01545-9",
-        "NAME": "Towards metrics-driven ontology engineering",
+        "NAME": "\"Towards metrics-driven ontology engineering\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/s10115-021-01545-9"
     },
     {
         "DOI": "10.1093/jigpal/jzaa043",
-        "NAME": "On learning context-aware rules to link RDF datasets",
+        "NAME": "\"On learning context-aware rules to link RDF datasets\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1093/jigpal/jzaa043"
     },
     {
         "DOI": "10.1016/j.autcon.2021.103592",
-        "NAME": "An information sharing strategy based on linked data for net zero energy buildings and clusters",
+        "NAME": "\"An information sharing strategy based on linked data for net zero energy buildings and clusters\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.autcon.2021.103592"
     },
     {
         "DOI": null,
         "NAME": "Personal Data Access Control Through Distributed Authorization",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/nca51143.2020.9306721"
     },
     {
+        "DOI": "10.3233/SW-200397",
+        "NAME": "\"Typology-based semantic labeling of numeric tabular data\"",
+        "PRIMARY_LOCATION": "https://doi.org/10.3233/sw-200397"
+    },
+    {
         "DOI": "10.1109/ACCESS.2021.3051839",
-        "NAME": "A Flexible and Robust Deep Learning-Based System for Solar Irradiance Forecasting",
+        "NAME": "\"A Flexible and Robust Deep Learning-Based System for Solar Irradiance Forecasting\"",
         "PRIMARY_LOCATION": "https://ieeexplore.ieee.org/ielx7/6287639/9312710/09324830.pdf"
     },
     {
         "DOI": "10.3233/SW-200396",
-        "NAME": "Understanding the phenomenology of reading through modelling",
+        "NAME": "\"Understanding the phenomenology of reading through modelling\"",
         "PRIMARY_LOCATION": "https://doi.org/10.3233/sw-200396"
     },
     {
         "DOI": "10.1007/978-3-030-88361-4_26",
-        "NAME": "A High-Level Ontology Network for ICT Infrastructures",
+        "NAME": "\"A High-Level Ontology Network for ICT Infrastructures\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-88361-4_26"
     },
     {
         "DOI": "10.1109/ICCCN52240.2021.9522257",
-        "NAME": "MOVO: a dApp for DLT-based Smart Mobility",
+        "NAME": "\"MOVO: a dApp for DLT-based Smart Mobility\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/icccn52240.2021.9522257"
     },
     {
         "DOI": "10.1109/ICCCN52240.2021.9522165",
-        "NAME": "Towards Decentralized Complex Queries over Distributed Ledgers: a Data Marketplace Use-case",
+        "NAME": "\"Towards Decentralized Complex Queries over Distributed Ledgers: a Data Marketplace Use-case\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/icccn52240.2021.9522165"
     },
     {
         "DOI": "10.1109/ACCESS.2021.3115577",
-        "NAME": "Toward the Ontological Modeling of Smart Contracts: A Solidity Use Case",
+        "NAME": "\"Toward the Ontological Modeling of Smart Contracts: A Solidity Use Case\"",
         "PRIMARY_LOCATION": "https://ieeexplore.ieee.org/ielx7/6287639/6514899/09548044.pdf"
     },
     {
         "DOI": "10.3233/SW-210432",
-        "NAME": "Enhancing virtual ontology based access over tabular data with Morph-CSV",
+        "NAME": "\"Enhancing virtual ontology based access over tabular data with Morph-CSV\"",
         "PRIMARY_LOCATION": "https://doi.org/10.3233/sw-210432"
     },
     {
         "DOI": "10.1109/EuroSPW54576.2021.00038",
-        "NAME": "ODRL Profile for Expressing Consent through Granular Access Control Policies in Solid",
+        "NAME": "\"ODRL Profile for Expressing Consent through Granular Access Control Policies in Solid\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/eurospw54576.2021.00038"
     },
     {
         "DOI": "10.1007/978-3-030-89811-3_23",
-        "NAME": "The Use of Decentralized and Semantic Web Technologies for Personal Data Protection and Interoperability",
+        "NAME": "\"The Use of Decentralized and Semantic Web Technologies for Personal Data Protection and Interoperability\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-89811-3_23"
     },
     {
         "DOI": "10.1109/WORKS54523.2021.00016",
-        "NAME": "A Community Roadmap for Scientific Workflows Research and Development",
+        "NAME": "\"A Community Roadmap for Scientific Workflows Research and Development\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/works54523.2021.00016"
     },
     {
         "DOI": "10.1109/DS-RT52167.2021.9576121",
-        "NAME": "Simulation of Hybrid Edge Computing Architectures",
+        "NAME": "\"Simulation of Hybrid Edge Computing Architectures\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/ds-rt52167.2021.9576121"
     },
     {
         "DOI": "10.3233/SSW51",
-        "NAME": "Advances in pattern-based ontology engineering",
+        "NAME": "\"Advances in pattern-based ontology engineering\"",
         "PRIMARY_LOCATION": "https://doi.org/10.3233/ssw51"
     },
     {
         "DOI": "10.1145/3462203.3475910",
-        "NAME": "Governing decentralized complex queries through a DAO",
+        "NAME": "\"Governing decentralized complex queries through a DAO\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1145/3462203.3475910"
     },
     {
         "DOI": "10.23919/ANNSIM52504.2021.9552126",
-        "NAME": "Simulation of Dissemination Strategies on Temporal Networks",
+        "NAME": "\"Simulation of Dissemination Strategies on Temporal Networks\"",
         "PRIMARY_LOCATION": "https://doi.org/10.23919/annsim52504.2021.9552126"
     },
     {
         "DOI": "978-1-64368-201-3",
-        "NAME": "Further with Knowledge Graphs - Proceedings of the 17th International Conference on Semantic Systems",
+        "NAME": "\"Further with Knowledge Graphs - Proceedings of the 17th International Conference on Semantic Systems\"",
         "PRIMARY_LOCATION": "https://publikationen.bibliothek.kit.edu/1000139991"
     },
     {
         "DOI": "10.1111/tgis.12720",
-        "NAME": "A scoping review on the use, processing and fusion of geographic data in virtual assistants",
+        "NAME": "\"A scoping review on the use, processing and fusion of geographic data in virtual assistants\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1111/tgis.12720"
     },
     {
         "DOI": "10.3390/ijgi10060374",
-        "NAME": "An analysis of existing production frameworks for statistical and geographic information: Synergies, gaps and integration",
+        "NAME": "\"An analysis of existing production frameworks for statistical and geographic information: Synergies, gaps and integration\"",
         "PRIMARY_LOCATION": "https://www.mdpi.com/2220-9964/10/6/374/pdf?version=1622623685"
     },
     {
         "DOI": "10.1007/978-3-030-85082-1_11",
-        "NAME": "LACLICHEV: Exploring the History of Climate Change in Latin America Within Newspapers Digital Collections",
+        "NAME": "\"LACLICHEV: Exploring the History of Climate Change in Latin America Within Newspapers Digital Collections\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-85082-1_11"
     },
     {
-        "DOI": "10.3233/SW-200397",
-        "NAME": "Typology-based semantic labeling of numeric tabular data",
-        "PRIMARY_LOCATION": "https://doi.org/10.3233/sw-200397"
-    },
-    {
         "DOI": "10.1016/j.engappai.2020.104026",
-        "NAME": "Conformance testing of ontologies through ontology requirements",
+        "NAME": "\"Conformance testing of ontologies through ontology requirements\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.engappai.2020.104026"
     },
     {
         "DOI": "10.2514/6.2021-1061",
-        "NAME": "Towards the use of ontologies in remotely piloted aircraft system conceptual design: Opportunities and challenges",
+        "NAME": "\"Towards the use of ontologies in remotely piloted aircraft system conceptual design: Opportunities and challenges\"",
         "PRIMARY_LOCATION": "https://doi.org/10.2514/6.2021-1061"
     },
     {
         "DOI": null,
         "NAME": "Preface for the 2nd edition of the international knowledge graph construction workshop",
         "PRIMARY_LOCATION": null
     },
@@ -1192,105 +1217,110 @@
     {
         "DOI": null,
         "NAME": "Latest enhancements in the Spanish DBpedia",
         "PRIMARY_LOCATION": "http://ceur-ws.org/Vol-2941/paper8.pdf"
     },
     {
         "DOI": "10.1007/978-3-030-80418-3_8",
-        "NAME": "Converting UML-Based Ontology Conceptualizations to OWL with Chowlk",
+        "NAME": "\"Converting UML-Based Ontology Conceptualizations to OWL with Chowlk\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-80418-3_8"
     },
     {
         "DOI": null,
         "NAME": "R4R: Template-based REST API Framework for RDF Knowledge Graphs",
         "PRIMARY_LOCATION": "http://ceur-ws.org/Vol-2980/paper339.pdf"
     },
     {
         "DOI": "10.1007/978-3-030-89811-3_18",
-        "NAME": "TimeLex: A Suite of Tools for Processing Temporal Information in Legal Texts",
+        "NAME": "\"TimeLex: A Suite of Tools for Processing Temporal Information in Legal Texts\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-89811-3_18"
     },
     {
         "DOI": "10.1007/978-3-030-89811-3_1",
-        "NAME": "Introduction: A Hybrid Regulatory Framework and Technical Architecture for a Human-Centered and Explainable AI",
+        "NAME": "\"Introduction: A Hybrid Regulatory Framework and Technical Architecture for a Human-Centered and Explainable AI\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-89811-3_1"
     },
     {
         "DOI": null,
         "NAME": "FOOPS!: An ontology pitfall scanner for the FAIR principles",
         "PRIMARY_LOCATION": "http://ceur-ws.org/Vol-2980/paper321.pdf"
     },
     {
         "DOI": null,
         "NAME": "Creating and querying personalized versions of wikidata on a laptop",
         "PRIMARY_LOCATION": "https://arxiv.org/abs/2108.07119"
     },
     {
         "DOI": "10.1109/AICCSA53542.2021.9686935",
-        "NAME": "Supporting Demand-Response strategies with the DELTA ontology",
+        "NAME": "\"Supporting Demand-Response strategies with the DELTA ontology\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/aiccsa53542.2021.9686935"
     },
     {
         "DOI": null,
         "NAME": "Bilingual Dataset for Information Retrieval and Question Answering over the Spanish Workers Statute",
-        "PRIMARY_LOCATION": "https://zenodo.org/record/4256718"
+        "PRIMARY_LOCATION": "https://zenodo.org/record/4256717"
     },
     {
         "DOI": "10.1007/978-3-030-89811-3_22",
-        "NAME": "Challenges in the Digital Representation of Privacy Terms",
+        "NAME": "\"Challenges in the Digital Representation of Privacy Terms\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-89811-3_22"
     },
     {
         "DOI": null,
         "NAME": "Integration of building material databases for IFC-based building performance analysis",
         "PRIMARY_LOCATION": "https://doi.org/10.22260/isarc2021/0027"
     },
     {
         "DOI": "10.1109/ICSC50631.2021.9475916",
-        "NAME": "VOCEDITOR - An Integrated Environment to Visually Edit, Validate and Versioning RDF Vocabularies",
+        "NAME": "\"VOCEDITOR - An Integrated Environment to Visually Edit, Validate and Versioning RDF Vocabularies\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/icsc50631.2021.9475916"
     },
     {
         "DOI": null,
         "NAME": "ETSI SmartM2M Technical Report 103717; Study for oneM2M; Discovery and Query specification development",
         "PRIMARY_LOCATION": "https://inria.hal.science/hal-03261080/document"
     },
     {
         "DOI": null,
         "NAME": "ETSI SmartM2M Technical Report 103715; Study for oneM2M; Discovery and Query solutions analysis & selection",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.3233/SW-200398",
-        "NAME": "Link maintenance for integrity in linked open data evolution: Literature survey and open challenges",
+        "NAME": "\"Link maintenance for integrity in linked open data evolution: Literature survey and open challenges\"",
         "PRIMARY_LOCATION": "https://doi.org/10.3233/sw-200398"
     },
     {
         "DOI": "10.1145/3460210.3493579",
-        "NAME": "Knowledge Engineering of PhD Stories: A Preliminary Study",
+        "NAME": "\"Knowledge Engineering of PhD Stories: A Preliminary Study\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1145/3460210.3493579"
     },
     {
+        "DOI": "10.1016/j.ijporl.2003.08.004",
+        "NAME": "\"Preface\"",
+        "PRIMARY_LOCATION": "https://doi.org/10.1016/j.ijporl.2003.08.004"
+    },
+    {
         "DOI": "10.1007/978-3-030-89811-3_20",
-        "NAME": "Challenges in the Implementation of Privacy Enhancing Semantic Technologies (PESTs) Supporting GDPR",
+        "NAME": "\"Challenges in the Implementation of Privacy Enhancing Semantic Technologies (PESTs) Supporting GDPR\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-89811-3_20"
     },
     {
         "DOI": null,
         "NAME": "Web of things (wot) discovery",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/ccnc.2019.8651786"
     },
     {
         "DOI": null,
         "NAME": "Thesaurus enhanced extraction of Hohfeld's relations from Spanish Labour Law",
         "PRIMARY_LOCATION": "http://ceur-ws.org/Vol-2918/paper4.pdf"
     },
     {
         "DOI": "10.1109/ICSC50631.2021.00089",
-        "NAME": "VOC EDITOR - An integrated environment to visually edit, validate and versioning RDF vocabularies",
+        "NAME": "\"VOC EDITOR - An integrated environment to visually edit, validate and versioning RDF vocabularies\"",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": null,
         "NAME": "A visual SHACL shapes editor based on ontopad",
         "PRIMARY_LOCATION": "http://ceur-ws.org/Vol-2941/paper16.pdf"
     },
@@ -1302,135 +1332,140 @@
     {
         "DOI": null,
         "NAME": "RML-star: A Declarative Mapping Language for RDF-star Generation",
         "PRIMARY_LOCATION": "http://ceur-ws.org/Vol-2980/paper374.pdf"
     },
     {
         "DOI": "978-3-030-89810-6",
-        "NAME": "AI Approaches to the Complexity of Legal Systems XI-XII",
+        "NAME": "\"AI Approaches to the Complexity of Legal Systems XI-XII\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-89811-3"
     },
     {
         "DOI": "10.1016/j.websem.2020.100596",
-        "NAME": "GTFS-Madrid-Bench: A benchmark for virtual knowledge graph access in the transport domain",
+        "NAME": "\"GTFS-Madrid-Bench: A benchmark for virtual knowledge graph access in the transport domain\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.websem.2020.100596"
     },
     {
         "DOI": "10.1038/s41398-020-0705-1",
-        "NAME": "ENIGMA and global neuroscience: A decade of large-scale studies of the brain in health and disease across more than 40 countries",
+        "NAME": "\"ENIGMA and global neuroscience: A decade of large-scale studies of the brain in health and disease across more than 40 countries\"",
         "PRIMARY_LOCATION": "https://www.nature.com/articles/s41398-020-0705-1.pdf"
     },
     {
         "DOI": "10.1038/s41467-020-18367-y",
-        "NAME": "Genetic correlations and genome-wide associations of cortical structure in general population samples of 22,824 adults",
+        "NAME": "\"Genetic correlations and genome-wide associations of cortical structure in general population samples of 22,824 adults\"",
         "PRIMARY_LOCATION": "https://www.nature.com/articles/s41467-020-18367-y.pdf"
     },
     {
         "DOI": null,
         "NAME": "Best Practices for Implementing FAIR Vocabularies and Ontologies on the Web",
         "PRIMARY_LOCATION": "https://doi.org/10.3233/ssw200034"
     },
     {
         "DOI": "10.1109/NCA51143.2020.9306721",
-        "NAME": "Personal Data Access Control through Distributed Authorization",
+        "NAME": "\"Personal Data Access Control through Distributed Authorization\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/nca51143.2020.9306721"
     },
     {
+        "DOI": null,
+        "NAME": "Typology-based semantic labeling of numeric tabular data",
+        "PRIMARY_LOCATION": "https://doi.org/10.3233/sw-200397"
+    },
+    {
         "DOI": "10.1007/s12652-019-01561-2",
-        "NAME": "Using LOT methodology to develop a noise pollution ontology: a Spanish use case",
+        "NAME": "\"Using LOT methodology to develop a noise pollution ontology: a Spanish use case\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/s12652-019-01561-2"
     },
     {
         "DOI": "10.1007/s12652-019-01608-4",
-        "NAME": "A multi-agent architecture for mobile sensing systems",
+        "NAME": "\"A multi-agent architecture for mobile sensing systems\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/s12652-019-01608-4"
     },
     {
         "DOI": null,
         "NAME": "Enhancing Public Procurement in the European Union Through Constructing and Exploiting an Integrated Knowledge Graph",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-62466-8_27"
     },
     {
         "DOI": null,
         "NAME": "COMPARTIR Y GENERAR DATOS Y CONOCIMIENTO AGROECOL\u00d3GICO CON PAUSA",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.1145/3410699.3413798",
-        "NAME": "MOATcoin: Exploring challenges and legal implications of smart contracts through a gamelike DApp experiment",
+        "NAME": "\"MOATcoin: Exploring challenges and legal implications of smart contracts through a gamelike DApp experiment\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1145/3410699.3413798"
     },
     {
         "DOI": "10.1145/3410699.3413789",
-        "NAME": "Are distributed ledger technologies ready for intelligent transportation systems?",
+        "NAME": "\"Are distributed ledger technologies ready for intelligent transportation systems?\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1145/3410699.3413789"
     },
     {
         "DOI": "10.3390/s20185198",
-        "NAME": "Discovering hidden mental states in open multi-agent systems by leveraging multi-protocol regularities with machine learning",
+        "NAME": "\"Discovering hidden mental states in open multi-agent systems by leveraging multi-protocol regularities with machine learning\"",
         "PRIMARY_LOCATION": "https://www.mdpi.com/1424-8220/20/18/5198/pdf?version=1599893740"
     },
     {
         "DOI": "10.1111/hiv.12883",
-        "NAME": "Potentially inappropriate medications in older adults living with HIV",
+        "NAME": "\"Potentially inappropriate medications in older adults living with HIV\"",
         "PRIMARY_LOCATION": "https://onlinelibrary.wiley.com/doi/pdfdirect/10.1111/hiv.12883"
     },
     {
         "DOI": "10.1016/j.future.2018.07.035",
-        "NAME": "Mission possible: Unify HPC and Big Data stacks towards application-defined blobs at the storage layer",
+        "NAME": "\"Mission possible: Unify HPC and Big Data stacks towards application-defined blobs at the storage layer\"",
         "PRIMARY_LOCATION": "http://manuscript.elsevier.com/S0167739X17330583/pdf/S0167739X17330583.pdf"
     },
     {
         "DOI": "10.1007/s00500-020-05061-w",
-        "NAME": "Grammatically uniform population initialization for grammar-guided genetic programming",
+        "NAME": "\"Grammatically uniform population initialization for grammar-guided genetic programming\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/s00500-020-05061-w"
     },
     {
         "DOI": "10.1093/cid/ciz811",
-        "NAME": "Polypharmacy and Drug-Drug Interactions in People Living With Human Immunodeficiency Virus in the Region of Madrid, Spain: A Population-Based Study",
+        "NAME": "\"Polypharmacy and Drug-Drug Interactions in People Living With Human Immunodeficiency Virus in the Region of Madrid, Spain: A Population-Based Study\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1093/cid/ciz811"
     },
     {
         "DOI": "10.18293/SEKE2020",
-        "NAME": "Proceedings of the 32nd International Conference on Software Engineering and Knowledge Engineering (SEKE 2020)",
+        "NAME": "\"Proceedings of the 32nd International Conference on Software Engineering and Knowledge Engineering (SEKE 2020)\"",
         "PRIMARY_LOCATION": "https://doi.org/10.18293/seke2020"
     },
     {
         "DOI": "10.1007/s00354-020-00100-4",
-        "NAME": "An Intelligent System to Generate Chord Progressions from Colors with an Artificial Immune System",
+        "NAME": "\"An Intelligent System to Generate Chord Progressions from Colors with an Artificial Immune System\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/s00354-020-00100-4"
     },
     {
         "DOI": "10.1109/ICALT49669.2020.00091",
-        "NAME": "Accessibility and personalization in opencourseware: An inclusive development approach",
+        "NAME": "\"Accessibility and personalization in opencourseware: An inclusive development approach\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/icalt49669.2020.00091"
     },
     {
         "DOI": "10.1145/3389189.3397973",
-        "NAME": "Developing accessibility multimedia services: The case of EasyTV",
+        "NAME": "\"Developing accessibility multimedia services: The case of EasyTV\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1145/3389189.3397973"
     },
     {
         "DOI": "978-84-1324-774-8",
-        "NAME": "Enterprise Information Integration: On Discovering Links Using Genetic Programming",
+        "NAME": "\"Enterprise Information Integration: On Discovering Links Using Genetic Programming\"",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": null,
         "NAME": "Proceedings of the 1st International Workshop on Semantic Digital Twins (SeDiT 2020)",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.1142/S0218194020400070",
-        "NAME": "Exploiting Declarative Mapping Rules for Generating GraphQL Servers with Morph-GraphQL",
+        "NAME": "\"Exploiting Declarative Mapping Rules for Generating GraphQL Servers with Morph-GraphQL\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1142/s0218194020400070"
     },
     {
         "DOI": "10.1007/s10579-019-09470-8",
-        "NAME": "Spanish corpora for sentiment analysis: a survey",
+        "NAME": "\"Spanish corpora for sentiment analysis: a survey\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/s10579-019-09470-8"
     },
     {
         "DOI": null,
         "NAME": "Defying wikidata: Validation of terminological relations in the web of data",
         "PRIMARY_LOCATION": "https://www.aclweb.org/anthology/2020.lrec-1.694.pdf"
     },
@@ -1447,195 +1482,200 @@
     {
         "DOI": null,
         "NAME": "Order matters: terminological saturation is best achievable using descending citation frequency datasets",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.1126/science.aay6690",
-        "NAME": "The genetic architecture of the human cerebral cortex",
+        "NAME": "\"The genetic architecture of the human cerebral cortex\"",
         "PRIMARY_LOCATION": "http://www.bristol.ac.uk/alspac/external/documents/grant-acknowledgements.pdf"
     },
     {
         "DOI": "10.1109/MSP.2019.2955207",
-        "NAME": "The Challenge: From MPEG Intellectual Property Rights Ontologies to Smart Contracts and Blockchains [Standards in a Nutshell]",
+        "NAME": "\"The Challenge: From MPEG Intellectual Property Rights Ontologies to Smart Contracts and Blockchains [Standards in a Nutshell]\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/msp.2019.2955207"
     },
     {
         "DOI": "10.3390/info11030129",
-        "NAME": "The zaragoza's knowledge graph: Open data to harness the city knowledge",
+        "NAME": "\"The zaragoza's knowledge graph: Open data to harness the city knowledge\"",
         "PRIMARY_LOCATION": "https://www.mdpi.com/2078-2489/11/3/129/pdf"
     },
     {
         "DOI": "10.3390/app10051803",
-        "NAME": "Development Experience of a Context-Aware System for Smart Irrigation Using CASO and IRRIG Ontologies",
+        "NAME": "\"Development Experience of a Context-Aware System for Smart Irrigation Using CASO and IRRIG Ontologies\"",
         "PRIMARY_LOCATION": "https://www.mdpi.com/2076-3417/10/5/1803/pdf?version=1583938924"
     },
     {
         "DOI": "10.3390/s20030822",
-        "NAME": "EWOT: A semantic interoperability approach for heterogeneous IoT ecosystems based on the web of things",
+        "NAME": "\"EWOT: A semantic interoperability approach for heterogeneous IoT ecosystems based on the web of things\"",
         "PRIMARY_LOCATION": "https://www.mdpi.com/1424-8220/20/3/822/pdf?version=1580812003"
     },
     {
         "DOI": "10.1007/978-3-030-23887-2_15",
-        "NAME": "An ontology-based deep learning approach for knowledge graph completion with fresh entities",
+        "NAME": "\"An ontology-based deep learning approach for knowledge graph completion with fresh entities\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-23887-2_15"
     },
     {
         "DOI": "10.1109/ACCESS.2020.2998012",
-        "NAME": "A Framework Based on Distributed Ledger Technologies for Data Management and Services in Intelligent Transportation Systems",
+        "NAME": "\"A Framework Based on Distributed Ledger Technologies for Data Management and Services in Intelligent Transportation Systems\"",
         "PRIMARY_LOCATION": "https://ieeexplore.ieee.org/ielx7/6287639/8948470/09102237.pdf"
     },
     {
         "DOI": "10.1007/978-3-030-49461-2_29",
-        "NAME": "Astrea: Automatic Generation of SHACL Shapes from Ontologies",
+        "NAME": "\"Astrea: Automatic Generation of SHACL Shapes from Ontologies\"",
         "PRIMARY_LOCATION": "https://link.springer.com/content/pdf/10.1007/978-3-030-49461-2_29.pdf"
     },
     {
+        "DOI": "10.3233/SW-200373",
+        "NAME": "\"Large-scale semantic exploration of scientific literature using topic-based hashing algorithms\"",
+        "PRIMARY_LOCATION": "https://doi.org/10.3233/sw-200373"
+    },
+    {
         "DOI": "10.1109/ACCESS.2020.3030006",
-        "NAME": "Improving the Results of Citizen Science Projects Through Reputation Systems: The Case of Wolf's Number Experiment",
+        "NAME": "\"Improving the Results of Citizen Science Projects Through Reputation Systems: The Case of Wolf's Number Experiment\"",
         "PRIMARY_LOCATION": "https://ieeexplore.ieee.org/ielx7/6287639/8948470/09220105.pdf"
     },
     {
         "DOI": "10.1007/978-3-030-62419-4_16",
-        "NAME": "FunMap: Efficient Execution of Functional Mappings for Knowledge Graph Creation",
+        "NAME": "\"FunMap: Efficient Execution of Functional Mappings for Knowledge Graph Creation\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-62419-4_16"
     },
     {
         "DOI": "10.1109/SEST48500.2020.9203093",
-        "NAME": "OpenADR Ontology: Semantic Enrichment of Demand Response Strategies in Smart Grids",
+        "NAME": "\"OpenADR Ontology: Semantic Enrichment of Demand Response Strategies in Smart Grids\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/sest48500.2020.9203093"
     },
     {
         "DOI": "10.1109/SEST48500.2020.9203338",
-        "NAME": "Semantic Interoperability for DR Schemes Employing the SGAM Framework",
+        "NAME": "\"Semantic Interoperability for DR Schemes Employing the SGAM Framework\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/sest48500.2020.9203338"
     },
     {
         "DOI": "10.1109/ISCC50000.2020.9219623",
-        "NAME": "On the Efficiency of Decentralized File Storage for Personal Information Management Systems",
+        "NAME": "\"On the Efficiency of Decentralized File Storage for Personal Information Management Systems\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/iscc50000.2020.9219623"
     },
     {
         "DOI": "10.3233/FAIA200847",
-        "NAME": "Events Matter: Extraction of Events from Court Decisions",
+        "NAME": "\"Events Matter: Extraction of Events from Court Decisions\"",
         "PRIMARY_LOCATION": "https://ebooks.iospress.nl/pdf/doi/10.3233/FAIA200847"
     },
     {
         "DOI": "10.3233/SW-200380",
-        "NAME": "Editorial: Special issue on Semantic eScience: Methods, tools and applications",
+        "NAME": "\"Editorial: Special issue on Semantic eScience: Methods, tools and applications\"",
         "PRIMARY_LOCATION": "https://content.iospress.com:443/download/semantic-web/sw200380?id=semantic-web%2Fsw200380"
     },
     {
         "DOI": "10.1007/978-3-030-62466-8_18",
-        "NAME": "KGTK: A Toolkit for Large Knowledge Graph Manipulation and Analysis",
+        "NAME": "\"KGTK: A Toolkit for Large Knowledge Graph Manipulation and Analysis\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-62466-8_18"
     },
     {
         "DOI": "10.1007/978-3-030-62466-8_4",
-        "NAME": "OBA: An Ontology-Based Framework for\u00a0Creating REST APIs for Knowledge Graphs",
+        "NAME": "\"OBA: An Ontology-Based Framework for\u00a0Creating REST APIs for Knowledge Graphs\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-62466-8_4"
     },
     {
         "DOI": "10.1162/dint_a_00033",
-        "NAME": "Fair computational workflows",
+        "NAME": "\"Fair computational workflows\"",
         "PRIMARY_LOCATION": "https://www.mitpressjournals.org/doi/pdf/10.1162/dint_a_00033"
     },
     {
         "DOI": "10.26826/law-in-context.v37i1.129",
-        "NAME": "LYNX: Towards a Legal Knowledge Graph for Multilingual Europe",
+        "NAME": "\"LYNX: Towards a Legal Knowledge Graph for Multilingual Europe\"",
         "PRIMARY_LOCATION": "https://journals.latrobe.edu.au/index.php/law-in-context/article/download/129/200"
     },
     {
         "DOI": "10.1109/CCNC46108.2020.9045640",
-        "NAME": "A Distributed Ledger Based Infrastructure for Smart Transportation System and Social Good",
+        "NAME": "\"A Distributed Ledger Based Infrastructure for Smart Transportation System and Social Good\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/ccnc46108.2020.9045640"
     },
     {
         "DOI": "10.1590/1678-9865202032e180077",
-        "NAME": "Developing an ontology network about meteorological events from historical newspapers [Construcci\u00f3n de una red de ontolog\u00edas sobre eventos meteorol\u00f3gicos a partir de peri\u00f3dicos hist\u00f3ricos]",
+        "NAME": "\"Developing an ontology network about meteorological events from historical newspapers [Construcci\u00f3n de una red de ontolog\u00edas sobre eventos meteorol\u00f3gicos a partir de peri\u00f3dicos hist\u00f3ricos]\"",
         "PRIMARY_LOCATION": "http://www.scielo.br/pdf/tinf/v32/2318-0889-tinf-32-e180077.pdf"
     },
     {
         "DOI": "10.1007/s10115-019-01346-1",
-        "NAME": "A review of mobile sensing systems, applications, and opportunities",
+        "NAME": "\"A review of mobile sensing systems, applications, and opportunities\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/s10115-019-01346-1"
     },
     {
         "DOI": "10.1007/978-3-030-23990-9_2",
-        "NAME": "A moderate experiential learning approach applied on data science",
+        "NAME": "\"A moderate experiential learning approach applied on data science\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-23990-9_2"
     },
     {
         "DOI": "10.1016/j.jss.2019.110432",
-        "NAME": "Graph-based root cause analysis for service-oriented and microservice architectures",
+        "NAME": "\"Graph-based root cause analysis for service-oriented and microservice architectures\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.jss.2019.110432"
     },
     {
         "DOI": "10.3233/SW-190384",
-        "NAME": "Towards a new generation of ontology based data access",
+        "NAME": "\"Towards a new generation of ontology based data access\"",
         "PRIMARY_LOCATION": "https://doi.org/10.3233/sw-190384"
     },
     {
         "DOI": "10.1007/978-3-030-39459-2_2",
-        "NAME": "Optimized Term Extraction Method Based on Computing Merged Partial C-Values",
+        "NAME": "\"Optimized Term Extraction Method Based on Computing Merged Partial C-Values\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-39459-2_2"
     },
     {
         "DOI": "10.1007/s12652-020-01804-7",
-        "NAME": "Prediction and failure analysis of composite resin restorations in the posterior sector applied in teaching dental students",
+        "NAME": "\"Prediction and failure analysis of composite resin restorations in the posterior sector applied in teaching dental students\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/s12652-020-01804-7"
     },
     {
-        "DOI": "10.3233/SW-200373",
-        "NAME": "Large-scale semantic exploration of scientific literature using topic-based hashing algorithms",
-        "PRIMARY_LOCATION": "https://doi.org/10.3233/sw-200373"
-    },
-    {
         "DOI": "10.3233/JIFS-179865",
-        "NAME": "Annotador: a temporal tagger for Spanish",
+        "NAME": "\"Annotador: a temporal tagger for Spanish\"",
         "PRIMARY_LOCATION": "https://doi.org/10.3233/jifs-179865"
     },
     {
         "DOI": "10.1007/978-3-030-58790-1_4",
-        "NAME": "An Agent-Based Model for Exploring Pension Law and Social Security Policies",
+        "NAME": "\"An Agent-Based Model for Exploring Pension Law and Social Security Policies\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-58790-1_4"
     },
     {
         "DOI": "10.1007/978-3-030-58796-3_10",
-        "NAME": "Towards the assessment of easy-to-read guidelines using artificial intelligence techniques",
+        "NAME": "\"Towards the assessment of easy-to-read guidelines using artificial intelligence techniques\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-58796-3_10"
     },
     {
         "DOI": "10.3233/SW-200402",
-        "NAME": "SAREF4INMA: A SAREF extension for the industry and manufacturing domain",
+        "NAME": "\"SAREF4INMA: A SAREF extension for the industry and manufacturing domain\"",
         "PRIMARY_LOCATION": "https://doi.org/10.3233/sw-200402"
     },
     {
         "DOI": "10.1109/CIST49399.2021.9357197",
-        "NAME": "TermInteract: An Online Tool for Terminologists Aimed at Providing Terminology Quality Metrics",
+        "NAME": "\"TermInteract: An Online Tool for Terminologists Aimed at Providing Terminology Quality Metrics\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/cist49399.2021.9357197"
     },
     {
         "DOI": "10.1109/WIIAT50758.2020.00043",
-        "NAME": "Morph-Skyline: Virtual Ontology-Based Data Access for Skyline Queries",
+        "NAME": "\"Morph-Skyline: Virtual Ontology-Based Data Access for Skyline Queries\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/wiiat50758.2020.00043"
     },
     {
         "DOI": "10.1007/978-3-030-61244-3_18",
-        "NAME": "Coming to Terms with FAIR Ontologies",
+        "NAME": "\"Coming to Terms with FAIR Ontologies\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-61244-3_18"
     },
     {
         "DOI": "10.1007/978-3-030-65847-2_11",
-        "NAME": "Mapping the Web Ontology Language to the OpenAPI Specification",
+        "NAME": "\"Mapping the Web Ontology Language to the OpenAPI Specification\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-65847-2_11"
     },
     {
+        "DOI": "10.1007/978-3-030-62466-8_27",
+        "NAME": "\"Enhancing Public Procurement in the European Union Through Constructing and Exploiting an Integrated Knowledge Graph\"",
+        "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-62466-8_27"
+    },
+    {
         "DOI": "10.1007/978-3-030-61244-3_6",
-        "NAME": "Ontologies Supporting Research-Related Information Foraging Using Knowledge Graphs: Literature Survey and Holistic Model Mapping",
+        "NAME": "\"Ontologies Supporting Research-Related Information Foraging Using Knowledge Graphs: Literature Survey and Holistic Model Mapping\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-61244-3_6"
     },
     {
         "DOI": null,
         "NAME": "Ensuring personal data anonymity in data marketplaces through sensing-as-a-service and distributed ledger technologies",
         "PRIMARY_LOCATION": null
     },
@@ -1647,15 +1687,15 @@
     {
         "DOI": null,
         "NAME": "Foreword",
         "PRIMARY_LOCATION": "http://www.kidney-international.org/article/S0085253815538933/pdf"
     },
     {
         "DOI": "10.18293/SEKE2020-104",
-        "NAME": "Benchmarking the efficiency of RDF-based access for blockchain environments",
+        "NAME": "\"Benchmarking the efficiency of RDF-based access for blockchain environments\"",
         "PRIMARY_LOCATION": "https://dblp.uni-trier.de/db/conf/seke/seke2020.html#CimminoGC20"
     },
     {
         "DOI": null,
         "NAME": "From obXML to the OP ontology: Developing a semantic model for occupancy profile",
         "PRIMARY_LOCATION": null
     },
@@ -1681,20 +1721,35 @@
     },
     {
         "DOI": null,
         "NAME": "Best practices for implementing fair vocabularies and ontologies on the web",
         "PRIMARY_LOCATION": "https://doi.org/10.3233/ssw200034"
     },
     {
+        "DOI": "10.48550/arXiv.2012.01953",
+        "NAME": "\"Drugs4Covid: Drug-driven Knowledge Exploitation based on Scientific Publications\"",
+        "PRIMARY_LOCATION": "https://arxiv.org/abs/2012.01953"
+    },
+    {
         "DOI": null,
         "NAME": "Polypharmacy and Drug\u2013Drug Interactions in People Living With Human Immunodeficiency Virus in the Region of Madrid, Spain: A Population-Based Study",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": null,
+        "NAME": "OpenADR Ontology: Semantic Enrichment of Demand Response Strategies in Smart Grids",
+        "PRIMARY_LOCATION": "https://doi.org/10.1109/sest48500.2020.9203093"
+    },
+    {
+        "DOI": null,
+        "NAME": "Semantic Interoperability for DR Schemes Employing the SGAM Framework",
+        "PRIMARY_LOCATION": "https://doi.org/10.1109/sest48500.2020.9203338"
+    },
+    {
+        "DOI": null,
         "NAME": "Ontolog\u00edas para describir datos enlazados",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": null,
         "NAME": "Proceedings of the 10th Workshop on Ontology Design and Patterns (WOP 2019)",
         "PRIMARY_LOCATION": "http://www.diva-portal.org/smash/record.jsf?pid=diva2:1358287"
@@ -1707,135 +1762,155 @@
     {
         "DOI": null,
         "NAME": "Ontolog\u00edas y vocabularios para la normalizaci\u00f3n de datos abiertos",
         "PRIMARY_LOCATION": "https://dialnet.unirioja.es/servlet/articulo?codigo=7480703"
     },
     {
         "DOI": null,
+        "NAME": "On learning context-aware rules to link RDF datasets",
+        "PRIMARY_LOCATION": "https://doi.org/10.1093/jigpal/jzaa043"
+    },
+    {
+        "DOI": null,
         "NAME": "SIMULATION OF DISSEMINATION STRATEGIES ON TEMPORAL NETWORKS",
         "PRIMARY_LOCATION": "https://doi.org/10.23919/annsim52504.2021.9552126"
     },
     {
         "DOI": null,
+        "NAME": "A Distributed Ledger Based Infrastructure for Smart Transportation System and Social Good",
+        "PRIMARY_LOCATION": "https://doi.org/10.1109/ccnc46108.2020.9045640"
+    },
+    {
+        "DOI": null,
         "NAME": "Mapeathor: Simplifying the specification of declarative rules for knowledge graph construction",
         "PRIMARY_LOCATION": "http://ceur-ws.org/Vol-2721/paper488.pdf"
     },
     {
         "DOI": "10.1080/15230406.2020.1772113",
-        "NAME": "Unveiling the diversity of spatial data infrastructures in Latin America: evidence from an exploratory inquiry",
+        "NAME": "\"Unveiling the diversity of spatial data infrastructures in Latin America: evidence from an exploratory inquiry\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1080/15230406.2020.1772113"
     },
     {
         "DOI": "10.1007/978-3-030-59872-3_3",
-        "NAME": "A Proposal for Semantic Integration of Crime Data in Mexico City",
+        "NAME": "\"A Proposal for Semantic Integration of Crime Data in Mexico City\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-59872-3_3"
     },
     {
         "DOI": null,
         "NAME": "Morph-CSV: Virtual knowledge graph access for tabular data",
         "PRIMARY_LOCATION": "http://ceur-ws.org/Vol-2721/paper478.pdf"
     },
     {
         "DOI": "10.1007/978-3-030-45316-9_6",
-        "NAME": "Standards for the IoT",
+        "NAME": "\"Standards for the IoT\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-45316-9_6"
     },
     {
         "DOI": "10.1007/978-3-030-45316-9_5",
-        "NAME": "Ontologies for IoT Semantic Interoperability",
+        "NAME": "\"Ontologies for IoT Semantic Interoperability\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-45316-9_5"
     },
     {
         "DOI": "10.1016/j.websem.2019.03.001",
-        "NAME": "Evaluating the impact of semantic technologies on bibliographic systems: A user-centred and comparative approach",
+        "NAME": "\"Evaluating the impact of semantic technologies on bibliographic systems: A user-centred and comparative approach\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.websem.2019.03.001"
     },
     {
         "DOI": "10.1007/s11042-019-08125-8",
-        "NAME": "Ontology based E-learning framework: A personalized, adaptive and context aware model",
+        "NAME": "\"Ontology based E-learning framework: A personalized, adaptive and context aware model\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/s11042-019-08125-8"
     },
     {
         "DOI": "10.1109/BigData47090.2019.9006447",
-        "NAME": "SoMEF: A Framework for Capturing Scientific Software Metadata from its Documentation",
+        "NAME": "\"SoMEF: A Framework for Capturing Scientific Software Metadata from its Documentation\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/bigdata47090.2019.9006447"
     },
     {
         "DOI": "10.1016/j.future.2019.05.034",
-        "NAME": "Deep neural network architectures for social services diagnosis in smart cities",
+        "NAME": "\"Deep neural network architectures for social services diagnosis in smart cities\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.future.2019.05.034"
     },
     {
         "DOI": "10.1016/j.future.2019.04.037",
-        "NAME": "Survey of agent-based cloud computing applications",
+        "NAME": "\"Survey of agent-based cloud computing applications\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.future.2019.04.037"
     },
     {
         "DOI": null,
         "NAME": "Potentially inappropriate medications in older adults with HIV in the region of Madrid, Spain",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": null,
         "NAME": "Scalable Cross-lingual Document Similarity through Language-specific Concept Hierarchies",
         "PRIMARY_LOCATION": "https://doi.org/10.1145/3360901.3364444"
     },
     {
         "DOI": "10.1029/2019PA003632",
-        "NAME": "PaCTS 1.0: A Crowdsourced Reporting Standard for Paleoclimate Data",
+        "NAME": "\"PaCTS 1.0: A Crowdsourced Reporting Standard for Paleoclimate Data\"",
         "PRIMARY_LOCATION": "https://agupubs.onlinelibrary.wiley.com/doi/pdfdirect/10.1029/2019PA003632"
     },
     {
         "DOI": "10.1109/IOTSMS48152.2019.8939260",
-        "NAME": "Semantic Modelling of Plans and Execution Traces for Enhancing Transparency of IoT Systems",
+        "NAME": "\"Semantic Modelling of Plans and Execution Traces for Enhancing Transparency of IoT Systems\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/iotsms48152.2019.8939260"
     },
     {
+        "DOI": "10.1145/3360901.3364444",
+        "NAME": "\"Scalable Cross-lingual Document Similarity through Language-specific Concept Hierarchies\"",
+        "PRIMARY_LOCATION": "https://doi.org/10.1145/3360901.3364444"
+    },
+    {
         "DOI": "10.1145/3360901.3364448",
-        "NAME": "T2WML table to wikidata mapping language",
+        "NAME": "\"T2WML table to wikidata mapping language\"",
         "PRIMARY_LOCATION": "https://dl.acm.org/doi/pdf/10.1145/3360901.3364448"
     },
     {
         "DOI": "10.1007/s11192-019-03179-9",
-        "NAME": "Participation of women in doctorate, research, innovation, and management activities at Universidad Polit\u00e9cnica de Madrid: analysis of the decade 2006\u20132016",
+        "NAME": "\"Participation of women in doctorate, research, innovation, and management activities at Universidad Polit\u00e9cnica de Madrid: analysis of the decade 2006\u20132016\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/s11192-019-03179-9"
     },
     {
         "DOI": "10.1109/eScience.2019.00046",
-        "NAME": "OKG-soft: An open knowledge graph with machine readable scientific software metadata",
+        "NAME": "\"OKG-soft: An open knowledge graph with machine readable scientific software metadata\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/escience.2019.00046"
     },
     {
         "DOI": "10.1145/3357419.3357442",
-        "NAME": "Ontological Model for the Semantic Description of Syllabuses",
+        "NAME": "\"Ontological Model for the Semantic Description of Syllabuses\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1145/3357419.3357442"
     },
     {
         "DOI": "10.1016/j.websem.2018.12.010",
-        "NAME": "Why are ontologies not reused across the same domain?",
+        "NAME": "\"Why are ontologies not reused across the same domain?\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.websem.2018.12.010"
     },
     {
         "DOI": "10.1049/iet-wss.2018.5209",
-        "NAME": "Ontology evolution for personalised and adaptive activity recognition",
+        "NAME": "\"Ontology evolution for personalised and adaptive activity recognition\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1049/iet-wss.2018.5209"
     },
     {
         "DOI": "10.1016/j.websem.2018.09.003",
+        "NAME": "\"Automating ontology engineering support activities with OnToology\"",
+        "PRIMARY_LOCATION": "https://doi.org/10.1016/j.websem.2018.09.003"
+    },
+    {
+        "DOI": null,
         "NAME": "Automating ontology engineering support activities with OnToology",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.websem.2018.09.003"
     },
     {
         "DOI": "10.3233/FAIA190006",
-        "NAME": "Closing the awareness gap between it practice and it law",
+        "NAME": "\"Closing the awareness gap between it practice and it law\"",
         "PRIMARY_LOCATION": "https://doi.org/10.3233/FAIA190006"
     },
     {
         "DOI": "10.3233/FAIA190019",
-        "NAME": "Language resources as linked data for the legal domain",
+        "NAME": "\"Language resources as linked data for the legal domain\"",
         "PRIMARY_LOCATION": "https://doi.org/10.3233/FAIA190019"
     },
     {
         "DOI": null,
         "NAME": "Closing the Awareness Gap Between IT Practice and IT Law - Critical Legal Positivism Applied in the Domain of IT Law",
         "PRIMARY_LOCATION": null
     },
@@ -1847,65 +1922,65 @@
     {
         "DOI": null,
         "NAME": "Spanish Corpora for Sentiment Analysis: a Survey",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/s10579-019-09470-8"
     },
     {
         "DOI": "10.1016/j.eswa.2019.01.001",
-        "NAME": "Taxi dispatching strategies with compensations",
+        "NAME": "\"Taxi dispatching strategies with compensations\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.eswa.2019.01.001"
     },
     {
         "DOI": "10.1016/j.engappai.2019.03.007",
-        "NAME": "Retraction notice to \u201cApplying case-based reasoning in social computing to transform colors into music\u201d (Engineering Applications of Artificial Intelligence (2018) 72 (1\u20139), (S0952197618300563), (10.1016/j.engappai.2018.03.007))",
+        "NAME": "\"Retraction notice to \u201cApplying case-based reasoning in social computing to transform colors into music\u201d (Engineering Applications of Artificial Intelligence (2018) 72 (1\u20139), (S0952197618300563), (10.1016/j.engappai.2018.03.007))\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.engappai.2019.03.007"
     },
     {
         "DOI": "10.1109/DCOSS.2019.00061",
-        "NAME": "VICINITY: IoT Semantic Interoperability Based on the Web of Things",
+        "NAME": "\"VICINITY: IoT Semantic Interoperability Based on the Web of Things\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/dcoss.2019.00061"
     },
     {
         "DOI": "10.3390/s19081774",
-        "NAME": "Prediction and Decision-Making in Intelligent Environments Supported by Knowledge Graphs, A Systematic Review",
+        "NAME": "\"Prediction and Decision-Making in Intelligent Environments Supported by Knowledge Graphs, A Systematic Review\"",
         "PRIMARY_LOCATION": "https://www.mdpi.com/1424-8220/19/8/1774/pdf?version=1555141210"
     },
     {
         "DOI": "10.4271/2019-01-1278",
-        "NAME": "Calculating Heavy-Duty truck energy and fuel consumption using correlation formulas derived from vecto simulations",
+        "NAME": "\"Calculating Heavy-Duty truck energy and fuel consumption using correlation formulas derived from vecto simulations\"",
         "PRIMARY_LOCATION": "https://doi.org/10.4271/2019-01-1278"
     },
     {
         "DOI": "10.4271/2019-01-1280",
-        "NAME": "A generalized component efficiency and Input-Data generation model for creating Fleet-Representative vehicle simulation cases in vecto",
+        "NAME": "\"A generalized component efficiency and Input-Data generation model for creating Fleet-Representative vehicle simulation cases in vecto\"",
         "PRIMARY_LOCATION": "https://doi.org/10.4271/2019-01-1280"
     },
     {
         "DOI": "10.1145/3308557.3308711",
-        "NAME": "An intelligent interface for integrating climate, hydrology, agriculture, and socioeconomic models",
+        "NAME": "\"An intelligent interface for integrating climate, hydrology, agriculture, and socioeconomic models\"",
         "PRIMARY_LOCATION": "https://dl.acm.org/doi/pdf/10.1145/3308557.3308711"
     },
     {
         "DOI": "10.1186/s40965-019-0060-4",
-        "NAME": "A sustainable process and toolbox for geographical linked data generation and publication: a case study with BTN100",
+        "NAME": "\"A sustainable process and toolbox for geographical linked data generation and publication: a case study with BTN100\"",
         "PRIMARY_LOCATION": "https://opengeospatialdata.springeropen.com/track/pdf/10.1186/s40965-019-0060-4"
     },
     {
         "DOI": "10.1007/s10115-018-1230-x",
-        "NAME": "Toward proactive social inclusion powered by machine learning",
+        "NAME": "\"Toward proactive social inclusion powered by machine learning\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/s10115-018-1230-x"
     },
     {
         "DOI": "10.1016/j.autcon.2018.12.010",
-        "NAME": "Enhancing energy management at district and building levels via an EM-KPI ontology",
+        "NAME": "\"Enhancing energy management at district and building levels via an EM-KPI ontology\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.autcon.2018.12.010"
     },
     {
         "DOI": "10.1111/tgis.12496",
-        "NAME": "A framework for connecting two interoperability universes: OGC Web Feature Services and Linked Data",
+        "NAME": "\"A framework for connecting two interoperability universes: OGC Web Feature Services and Linked Data\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1111/tgis.12496"
     },
     {
         "DOI": null,
         "NAME": "ETSI TS 103 410-3. SmartM2M; Smart Appliances extension to SA",
         "PRIMARY_LOCATION": null
     },
@@ -1917,195 +1992,195 @@
     {
         "DOI": null,
         "NAME": "ETSI TS 103 410-5. SmartM2M; Smart Appliances extension to SA",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.3233/SW-180305",
-        "NAME": "Best practices for publishing, retrieving, and using spatial data on the web",
+        "NAME": "\"Best practices for publishing, retrieving, and using spatial data on the web\"",
         "PRIMARY_LOCATION": "https://doi.org/10.3233/sw-180305"
     },
     {
+        "DOI": "10.3233/SW-180324",
+        "NAME": "\"A quality assessment approach for evolving knowledge bases\"",
+        "PRIMARY_LOCATION": "https://doi.org/10.3233/sw-180324"
+    },
+    {
         "DOI": "10.1016/j.websem.2018.11.004",
-        "NAME": "Completeness and consistency analysis for evolving knowledge bases",
+        "NAME": "\"Completeness and consistency analysis for evolving knowledge bases\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.websem.2018.11.004"
     },
     {
         "DOI": "10.3233/SW-180320",
-        "NAME": "The modular SSN ontology: A joint W3C and OGC standard specifying the semantics of sensors, observations, sampling, and actuation",
+        "NAME": "\"The modular SSN ontology: A joint W3C and OGC standard specifying the semantics of sensors, observations, sampling, and actuation\"",
         "PRIMARY_LOCATION": "https://doi.org/10.3233/sw-180320"
     },
     {
         "DOI": "10.3390/app9010032",
-        "NAME": "Ontological Representation of Smart City Data: From Devices to Cities",
+        "NAME": "\"Ontological Representation of Smart City Data: From Devices to Cities\"",
         "PRIMARY_LOCATION": "https://www.mdpi.com/2076-3417/9/1/32/pdf?version=1545833153"
     },
     {
         "DOI": "10.1007/978-3-030-21348-0_29",
-        "NAME": "CORAL: A corpus of ontological requirements annotated with lexico-syntactic patterns",
+        "NAME": "\"CORAL: A corpus of ontological requirements annotated with lexico-syntactic patterns\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-21348-0_29"
     },
     {
         "DOI": "10.1007/978-3-030-01746-0_46",
-        "NAME": "Supervising attention in an e-learning system",
+        "NAME": "\"Supervising attention in an e-learning system\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-01746-0_46"
     },
     {
         "DOI": "10.1007/978-3-030-14401-2_29",
-        "NAME": "Towards a Knowledge Graph Based Platform for Public Procurement",
+        "NAME": "\"Towards a Knowledge Graph Based Platform for Public Procurement\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-14401-2_29"
     },
     {
         "DOI": "10.1007/978-3-030-21395-4_12",
-        "NAME": "Conformance Test Cases for the RDF Mapping Language (RML)",
+        "NAME": "\"Conformance Test Cases for the RDF Mapping Language (RML)\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-21395-4_12"
     },
     {
         "DOI": "10.18293/SEKE2019-117",
-        "NAME": "Themis: A tool for validating ontologies through requirements",
+        "NAME": "\"Themis: A tool for validating ontologies through requirements\"",
         "PRIMARY_LOCATION": "https://doi.org/10.18293/seke2019-117"
     },
     {
         "DOI": "10.18293/SEKE2019-055",
-        "NAME": "Morph-GraphQL: GraphQL servers generation from R2RML mappings (SESE)",
+        "NAME": "\"Morph-GraphQL: GraphQL servers generation from R2RML mappings (SESE)\"",
         "PRIMARY_LOCATION": "https://doi.org/10.18293/seke2019-055"
     },
     {
         "DOI": "10.3390/systems7030035",
-        "NAME": "Introduction to the Special Issue Artificial Intelligence Knowledge Representation",
+        "NAME": "\"Introduction to the Special Issue Artificial Intelligence Knowledge Representation\"",
         "PRIMARY_LOCATION": "https://www.mdpi.com/2079-8954/7/3/35/pdf?version=1563965423"
     },
     {
         "DOI": "10.1007/978-3-030-13363-4_4",
-        "NAME": "Towards a Linked Democracy Model",
+        "NAME": "\"Towards a Linked Democracy Model\"",
         "PRIMARY_LOCATION": "https://link.springer.com/content/pdf/10.1007%2F978-3-030-13363-4_4.pdf"
     },
     {
         "DOI": "10.1007/978-3-030-13363-4_2",
-        "NAME": "Deliberative and Epistemic Approaches to Democracy",
+        "NAME": "\"Deliberative and Epistemic Approaches to Democracy\"",
         "PRIMARY_LOCATION": "https://link.springer.com/content/pdf/10.1007%2F978-3-030-13363-4_2.pdf"
     },
     {
         "DOI": "10.1007/978-3-030-13363-4_1",
-        "NAME": "Linked Democracy Foundations, Tools, and Applications Introduction to Linked Data",
+        "NAME": "\"Linked Democracy Foundations, Tools, and Applications Introduction to Linked Data\"",
         "PRIMARY_LOCATION": "https://link.springer.com/content/pdf/10.1007%2F978-3-030-13363-4_1.pdf"
     },
     {
         "DOI": "10.1007/978-3-030-13363-4_5",
-        "NAME": "Legal Linked Data Ecosystems and the Rule of Law",
+        "NAME": "\"Legal Linked Data Ecosystems and the Rule of Law\"",
         "PRIMARY_LOCATION": "https://link.springer.com/content/pdf/10.1007%2F978-3-030-13363-4_5.pdf"
     },
     {
         "DOI": "10.1007/978-3-030-13363-4_3",
-        "NAME": "Multilayered Linked Democracy",
+        "NAME": "\"Multilayered Linked Democracy\"",
         "PRIMARY_LOCATION": "https://link.springer.com/content/pdf/10.1007%2F978-3-030-13363-4_3.pdf"
     },
     {
         "DOI": "10.1007/978-3-030-13363-4_6",
-        "NAME": "Linked Democracy Foundations, Tools, and Applications Conclusion",
+        "NAME": "\"Linked Democracy Foundations, Tools, and Applications Conclusion\"",
         "PRIMARY_LOCATION": "https://link.springer.com/content/pdf/10.1007%2F978-3-030-13363-4_6.pdf"
     },
     {
         "DOI": "10.3390/app9235180",
-        "NAME": "An Abstract Framework for Non-Cooperative Multi-Agent Planning",
+        "NAME": "\"An Abstract Framework for Non-Cooperative Multi-Agent Planning\"",
         "PRIMARY_LOCATION": "https://www.mdpi.com/2076-3417/9/23/5180/pdf?version=1575008421"
     },
     {
         "DOI": "10.1007/978-3-030-29374-1_19",
-        "NAME": "Towards an Ontology for Public Procurement Based on the Open Contracting Data Standard",
+        "NAME": "\"Towards an Ontology for Public Procurement Based on the Open Contracting Data Standard\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-29374-1_19"
     },
     {
         "DOI": "10.1007/978-3-030-32327-1_19",
-        "NAME": "SAD Generator: Eating Our Own Dog Food to Generate KGs and Websites for Academic Events",
+        "NAME": "\"SAD Generator: Eating Our Own Dog Food to Generate KGs and Websites for Academic Events\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-32327-1_19"
     },
     {
         "DOI": "10.1007/978-3-030-36691-9_19",
-        "NAME": "Towards Blockchain and Semantic Web",
+        "NAME": "\"Towards Blockchain and Semantic Web\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-36691-9_19"
     },
     {
         "DOI": "10.1145/3301275.3302324",
-        "NAME": "Towards human-guided machine learning",
+        "NAME": "\"Towards human-guided machine learning\"",
         "PRIMARY_LOCATION": "https://dl.acm.org/doi/pdf/10.1145/3301275.3302324"
     },
     {
-        "DOI": "10.3233/SW-180324",
-        "NAME": "A quality assessment approach for evolving knowledge bases",
-        "PRIMARY_LOCATION": "https://doi.org/10.3233/sw-180324"
-    },
-    {
         "DOI": "10.1007/s11042-018-6318-5",
-        "NAME": "Ontology-driven semantic unified modelling for concurrent activity recognition (OSCAR)",
+        "NAME": "\"Ontology-driven semantic unified modelling for concurrent activity recognition (OSCAR)\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/s11042-018-6318-5"
     },
     {
         "DOI": "10.1145/3318396.3318422",
-        "NAME": "Extension of the BIdo ontology to represent scientific production",
+        "NAME": "\"Extension of the BIdo ontology to represent scientific production\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1145/3318396.3318422"
     },
     {
         "DOI": "10.1007/978-3-319-94649-8_34",
-        "NAME": "Automatic music generation by deep learning",
+        "NAME": "\"Automatic music generation by deep learning\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-319-94649-8_34"
     },
     {
         "DOI": "10.1007/978-3-319-94649-8_38",
-        "NAME": "Social services diagnosis by deep learning",
+        "NAME": "\"Social services diagnosis by deep learning\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-319-94649-8_38"
     },
     {
         "DOI": "10.1007/978-3-030-13929-2_3",
-        "NAME": "Similar Terms Grouping Yields Faster Terminological Saturation",
+        "NAME": "\"Similar Terms Grouping Yields Faster Terminological Saturation\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-13929-2_3"
     },
     {
         "DOI": "10.1007/978-3-030-16187-3_20",
-        "NAME": "Using the SPAR ontology network to represent the scientific production of a university: A case study",
+        "NAME": "\"Using the SPAR ontology network to represent the scientific production of a university: A case study\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-16187-3_20"
     },
     {
         "DOI": "10.1007/978-3-030-24299-2_26",
-        "NAME": "An intelligent and autoadaptive system of virtual identities based on deep learning for the analysis of online advertising networks",
+        "NAME": "\"An intelligent and autoadaptive system of virtual identities based on deep learning for the analysis of online advertising networks\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-24299-2_26"
     },
     {
         "DOI": "10.1007/978-3-030-13363-4",
-        "NAME": "Linked Democracy Foundations, Tools, and Applications Preface",
+        "NAME": "\"Linked Democracy Foundations, Tools, and Applications Preface\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-13363-4"
     },
     {
         "DOI": "10.1017/S0269888919000195",
-        "NAME": "TempCourt: evaluation of temporal taggers on a new corpus of court decisions",
+        "NAME": "\"TempCourt: evaluation of temporal taggers on a new corpus of court decisions\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1017/s0269888919000195"
     },
     {
         "DOI": "10.1007/978-3-030-31605-1_9",
-        "NAME": "ContractFrames: Bridging the Gap Between Natural Language and Logics in Contract Law",
+        "NAME": "\"ContractFrames: Bridging the Gap Between Natural Language and Logics in Contract Law\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-31605-1_9"
     },
     {
         "DOI": "10.1007/978-3-030-33246-4_43",
-        "NAME": "What are the parameters that affect the construction of a knowledge graph?",
+        "NAME": "\"What are the parameters that affect the construction of a knowledge graph?\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-33246-4_43"
     },
     {
         "DOI": "10.1007/978-3-030-32327-1_11",
-        "NAME": "How to Validate Ontologies with Themis",
+        "NAME": "\"How to Validate Ontologies with Themis\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-32327-1_11"
     },
     {
         "DOI": "10.1109/WI.2018.00-93",
-        "NAME": "PSM-Flow: Probabilistic Subgraph Mining for Discovering Reusable Fragments in Workflows",
+        "NAME": "\"PSM-Flow: Probabilistic Subgraph Mining for Discovering Reusable Fragments in Workflows\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/wi.2018.00-93"
     },
     {
         "DOI": "10.1007/978-3-030-33752-0_18",
-        "NAME": "Towards Automated Hypothesis Testing in Neuroscience",
+        "NAME": "\"Towards Automated Hypothesis Testing in Neuroscience\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-33752-0_18"
     },
     {
         "DOI": null,
         "NAME": "Automatic enrichment of terminological resources: The IATE RDF example",
         "PRIMARY_LOCATION": "https://aran.library.nuigalway.ie/bitstream/10379/14881/1/automatic-enrichment-terminological_final.pdf"
     },
@@ -2152,15 +2227,15 @@
     {
         "DOI": null,
         "NAME": "ISWC 2019 posters & demonstrations, industry, and outrageous ideas tracks",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "9788417969059",
-        "NAME": "Building up communication skills: professional and academic training for engineers",
+        "NAME": "\"Building up communication skills: professional and academic training for engineers\"",
         "PRIMARY_LOCATION": "https://dialnet.unirioja.es/servlet/libro?codigo=825965"
     },
     {
         "DOI": null,
         "NAME": "Semantic workflows for benchmark challenges: Enhancing comparability, reusability and reproducibility",
         "PRIMARY_LOCATION": null
     },
@@ -2227,14 +2302,19 @@
     {
         "DOI": null,
         "NAME": "Ontolog\u00edas, Datos Enlazados (Linked Data) y",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": null,
+        "NAME": "Ontological Representation of Smart City Data: From Devices to Cities",
+        "PRIMARY_LOCATION": "https://www.mdpi.com/2076-3417/9/1/32/pdf?version=1545833153"
+    },
+    {
+        "DOI": null,
         "NAME": "Semantic technologies and interoperability in the built environment",
         "PRIMARY_LOCATION": "https://content.iospress.com:443/download/semantic-web/sw321?id=semantic-web%2Fsw321"
     },
     {
         "DOI": null,
         "NAME": "Proceedings of the 7th Linked Data in Architecture and Construction Workshop (LDAC2019)",
         "PRIMARY_LOCATION": "https://hal.archives-ouvertes.fr/hal-03165225"
@@ -2242,290 +2322,310 @@
     {
         "DOI": null,
         "NAME": "Enhancing the maintainability of the Bio2RDF project using declarative mappings",
         "PRIMARY_LOCATION": "http://ceur-ws.org/Vol-2849/paper-01.pdf"
     },
     {
         "DOI": "10.1109/eScience.2018.00132",
-        "NAME": "Semantic software metadata for workflow exploration and evolution",
+        "NAME": "\"Semantic software metadata for workflow exploration and evolution\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/escience.2018.00132"
     },
     {
         "DOI": "10.1017/S1351324918000347",
-        "NAME": "Models to represent linguistic linked data",
+        "NAME": "\"Models to represent linguistic linked data\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1017/s1351324918000347"
     },
     {
         "DOI": "10.1111/exsy.12275",
-        "NAME": "Modelling a smart environment for nonintrusive analysis of attention in the workplace",
+        "NAME": "\"Modelling a smart environment for nonintrusive analysis of attention in the workplace\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1111/exsy.12275"
     },
     {
         "DOI": null,
         "NAME": "Polypharmacy and drug-drug interactions in HIV-infected subjects in the region of Madrid (Spain): a population-based study",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.1109/INISTA.2018.8466303",
-        "NAME": "A Secured and Trusted Demand Response system based on Blockchain technologies",
+        "NAME": "\"A Secured and Trusted Demand Response system based on Blockchain technologies\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/inista.2018.8466303"
     },
     {
         "DOI": "10.1016/j.future.2017.07.003",
-        "NAME": "Using machine learning to optimize parallelism in big data applications",
+        "NAME": "\"Using machine learning to optimize parallelism in big data applications\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.future.2017.07.003"
     },
     {
         "DOI": "10.1016/j.future.2017.06.009",
-        "NAME": "Keeping up with storage: Decentralized, write-enabled dynamic geo-replication",
+        "NAME": "\"Keeping up with storage: Decentralized, write-enabled dynamic geo-replication\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.future.2017.06.009"
     },
     {
         "DOI": null,
         "NAME": "MAS: A Corpus of Tweets for Marketing in Spanish",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-319-98192-5_53"
     },
     {
         "DOI": "10.1109/ICDCS.2018.00152",
-        "NAME": "KerA: Scalable data ingestion for stream processing",
+        "NAME": "\"KerA: Scalable data ingestion for stream processing\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/icdcs.2018.00152"
     },
     {
         "DOI": "10.1109/ICDCS.2018.00156",
-        "NAME": "SLoG: Large-scale logging middleware for HPC and big data convergence",
+        "NAME": "\"SLoG: Large-scale logging middleware for HPC and big data convergence\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/icdcs.2018.00156"
     },
     {
         "DOI": "10.1109/CCGRID.2018.00072",
-        "NAME": "T\u00fdrFS: Increasing small files access performance with dynamic metadata replication",
+        "NAME": "\"T\u00fdrFS: Increasing small files access performance with dynamic metadata replication\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/ccgrid.2018.00072"
     },
     {
         "DOI": "10.1016/j.engappai.2018.03.007",
-        "NAME": "Applying case-based reasoning in social computing to transform colors into music",
+        "NAME": "\"Applying case-based reasoning in social computing to transform colors into music\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.engappai.2018.03.007"
     },
     {
         "DOI": "10.3390/s18051465",
-        "NAME": "Smart Waste Collection System with Low Consumption LoRaWAN Nodes and Route Optimization",
+        "NAME": "\"Smart Waste Collection System with Low Consumption LoRaWAN Nodes and Route Optimization\"",
         "PRIMARY_LOCATION": "https://www.mdpi.com/1424-8220/18/5/1465/pdf"
     },
     {
         "DOI": "10.1109/TLA.2018.8408424",
-        "NAME": "Design And Implementation Of A Low-Cost Universal Control For Intelligent Electric Wheelchairs",
+        "NAME": "\"Design And Implementation Of A Low-Cost Universal Control For Intelligent Electric Wheelchairs\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/tla.2018.8408424"
     },
     {
         "DOI": "10.1145/3167132.3167164",
-        "NAME": "Predicting incorrect mappings: A data-driven approach applied to DBpedia",
+        "NAME": "\"Predicting incorrect mappings: A data-driven approach applied to DBpedia\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1145/3167132.3167164"
     },
     {
         "DOI": "10.1145/3167132.3167341",
-        "NAME": "RDF shape induction using knowledge base profiling",
+        "NAME": "\"RDF shape induction using knowledge base profiling\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1145/3167132.3167341"
     },
     {
         "DOI": "10.1016/j.ins.2017.12.050",
-        "NAME": "Relationship recommender system in a business and employment-oriented social network",
+        "NAME": "\"Relationship recommender system in a business and employment-oriented social network\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.ins.2017.12.050"
     },
     {
         "DOI": "9783030133634",
-        "NAME": "Linked Democracy.Linked Democracy",
+        "NAME": "\"Linked Democracy.Linked Democracy\"",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.1109/IntelliSys.2017.8324287",
-        "NAME": "Drivers, standards and platforms for the IoT: Towards a digital VICINITY",
+        "NAME": "\"Drivers, standards and platforms for the IoT: Towards a digital VICINITY\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1109/intellisys.2017.8324287"
     },
     {
         "DOI": "10.3390/s18030757",
-        "NAME": "A Context-Aware Indoor Air Quality System for Sudden Infant Death Syndrome Prevention",
+        "NAME": "\"A Context-Aware Indoor Air Quality System for Sudden Infant Death Syndrome Prevention\"",
         "PRIMARY_LOCATION": "https://www.mdpi.com/1424-8220/18/3/757/pdf?version=1519986905"
     },
     {
         "DOI": "10.1007/s10115-017-1120-7",
-        "NAME": "Agent-based tool to reduce the maintenance cost of energy distribution networks",
+        "NAME": "\"Agent-based tool to reduce the maintenance cost of energy distribution networks\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/s10115-017-1120-7"
     },
     {
         "DOI": "10.1177/0735633117706047",
-        "NAME": "Students' Evaluation of a Virtual World for Procedural Training in a Tertiary-Education Course",
+        "NAME": "\"Students' Evaluation of a Virtual World for Procedural Training in a Tertiary-Education Course\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1177/0735633117706047"
     },
     {
         "DOI": "10.1111/aos.13519",
-        "NAME": "Association between CFH, CFB, ARMS2, SERPINF1, VEGFR1 and VEGF polymorphisms and anatomical and functional response to ranibizumab treatment in neovascular age-related macular degeneration",
+        "NAME": "\"Association between CFH, CFB, ARMS2, SERPINF1, VEGFR1 and VEGF polymorphisms and anatomical and functional response to ranibizumab treatment in neovascular age-related macular degeneration\"",
         "PRIMARY_LOCATION": "https://onlinelibrary.wiley.com/doi/pdfdirect/10.1111/aos.13519"
     },
     {
         "DOI": null,
         "NAME": "Cross-Evaluation of Automated Term Extraction Tools by Measuring Terminological Saturation",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-319-76168-8_7"
     },
     {
         "DOI": null,
         "NAME": "The Influence of the Order of Adding Documents to Datasets on Terminological Saturation",
         "PRIMARY_LOCATION": null
     },
     {
         "DOI": "10.3390/s18010220",
-        "NAME": "Increasing the Intensity over Time of an Electric-Assist Bike Based on the User and Route: The Bike Becomes the Gym",
+        "NAME": "\"Increasing the Intensity over Time of an Electric-Assist Bike Based on the User and Route: The Bike Becomes the Gym\"",
         "PRIMARY_LOCATION": "https://www.mdpi.com/1424-8220/18/1/220/pdf?version=1515922049"
     },
     {
         "DOI": "10.1016/j.neucom.2017.06.022",
-        "NAME": "Neural networks in distributed computing and artificial intelligence",
+        "NAME": "\"Neural networks in distributed computing and artificial intelligence\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1016/j.neucom.2017.06.022"
     },
     {
         "DOI": "10.3390/app8010067",
-        "NAME": "Multi-Agent System for Demand Prediction and Trip Visualization in Bike Sharing Systems",
+        "NAME": "\"Multi-Agent System for Demand Prediction and Trip Visualization in Bike Sharing Systems\"",
         "PRIMARY_LOCATION": "https://www.mdpi.com/2076-3417/8/1/67/pdf?version=1515142581"
     },
     {
         "DOI": "10.3390/s18010108",
-        "NAME": "Combination of Multi-Agent Systems and Wireless Sensor Networks for the Monitoring of Cattle",
+        "NAME": "\"Combination of Multi-Agent Systems and Wireless Sensor Networks for the Monitoring of Cattle\"",
         "PRIMARY_LOCATION": "https://www.mdpi.com/1424-8220/18/1/108/pdf?version=1516694198"
     },
     {
         "DOI": "10.1007/978-3-319-62410-5_16",
-        "NAME": "Predicting the risk of suffering chronic social exclusion with machine learning",
+        "NAME": "\"Predicting the risk of suffering chronic social exclusion with machine learning\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-319-62410-5_16"
     },
     {
         "DOI": "10.7717/peerj.4795",
-        "NAME": "A guideline for reporting experimental protocols in life sciences",
+        "NAME": "\"A guideline for reporting experimental protocols in life sciences\"",
         "PRIMARY_LOCATION": "https://peerj.com/articles/4795.pdf"
     },
     {
         "DOI": "10.3233/SW-170267",
-        "NAME": "A Comprehensive Quality Model for Linked Data",
+        "NAME": "\"A Comprehensive Quality Model for Linked Data\"",
         "PRIMARY_LOCATION": "https://doi.org/10.3233/sw-170267"
     },
     {
         "DOI": "10.1155/2018/2068278",
-        "NAME": "FMonE: A Flexible Monitoring Solution at the Edge",
+        "NAME": "\"FMonE: A Flexible Monitoring Solution at the Edge\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1155/2018/2068278"
     },
     {
+        "DOI": "10.3233/SW-180321",
+        "NAME": "\"Semantic technologies and interoperability in the built environment\"",
+        "PRIMARY_LOCATION": "https://content.iospress.com:443/download/semantic-web/sw321?id=semantic-web%2Fsw321"
+    },
+    {
         "DOI": "10.3233/SW-170258",
-        "NAME": "The apertium bilingual dictionaries on the web of data",
+        "NAME": "\"The apertium bilingual dictionaries on the web of data\"",
         "PRIMARY_LOCATION": "https://doi.org/10.3233/sw-170258"
     },
     {
         "DOI": "10.1155/2018/4012740",
-        "NAME": "Dealing with Demand in Electric Grids with an Adaptive Consumption Management Platform",
+        "NAME": "\"Dealing with Demand in Electric Grids with an Adaptive Consumption Management Platform\"",
         "PRIMARY_LOCATION": "http://downloads.hindawi.com/journals/complexity/2018/4012740.pdf"
     },
     {
         "DOI": "10.1155/2018/9741053",
-        "NAME": "IoT Approaches for Distributed Computing",
+        "NAME": "\"IoT Approaches for Distributed Computing\"",
         "PRIMARY_LOCATION": "http://downloads.hindawi.com/journals/wcmc/2018/9741053.pdf"
     },
     {
         "DOI": "10.3233/AIC-180772",
-        "NAME": "Classification of retinal vessels using a collaborative agent-based architecture",
+        "NAME": "\"Classification of retinal vessels using a collaborative agent-based architecture\"",
         "PRIMARY_LOCATION": "https://doi.org/10.3233/aic-180772"
     },
     {
         "DOI": "10.1007/978-3-319-73210-7_93",
-        "NAME": "Assess and Enhancing Attention in Learning Activities",
+        "NAME": "\"Assess and Enhancing Attention in Learning Activities\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-319-73210-7_93"
     },
     {
         "DOI": "10.5220/0006925300570067",
-        "NAME": "Machine learning-based query augmentation for SPARQL endpoints",
+        "NAME": "\"Machine learning-based query augmentation for SPARQL endpoints\"",
         "PRIMARY_LOCATION": "https://doi.org/10.5220/0006925300570067"
     },
     {
         "DOI": "10.1007/978-3-030-00178-0_16",
-        "NAME": "Assigning Creative Commons Licenses to Research Metadata: Issues and Cases",
+        "NAME": "\"Assigning Creative Commons Licenses to Research Metadata: Issues and Cases\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-00178-0_16"
     },
     {
         "DOI": "10.1007/978-3-030-03667-6_2",
-        "NAME": "Fuzzy semantic labeling of semi-structured numerical datasets",
+        "NAME": "\"Fuzzy semantic labeling of semi-structured numerical datasets\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-03667-6_2"
     },
     {
         "DOI": "10.1002/9781119564034.ch25",
-        "NAME": "A SAREF extension for semantic interoperability in the industry and manufacturing domain",
+        "NAME": "\"A SAREF extension for semantic interoperability in the industry and manufacturing domain\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1002/9781119564034.ch25"
     },
     {
         "DOI": "10.1145/3184558.3192316",
-        "NAME": "PROFILES & DATA: SEARCH \u2013 International Workshop on Profiling & Searching Data on the Web Chairs\u2019 Welcome",
+        "NAME": "\"PROFILES & DATA: SEARCH \u2013 International Workshop on Profiling & Searching Data on the Web Chairs\u2019 Welcome\"",
         "PRIMARY_LOCATION": "http://dl.acm.org/ft_gateway.cfm?id=3192316&type=pdf"
     },
     {
+        "DOI": null,
+        "NAME": "A Secured and Trusted Demand Response system based on Blockchain technologies",
+        "PRIMARY_LOCATION": "https://doi.org/10.1109/inista.2018.8466303"
+    },
+    {
+        "DOI": "10.1007/978-3-319-98192-5_53",
+        "NAME": "\"MAS: A Corpus of Tweets for Marketing in Spanish\"",
+        "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-319-98192-5_53"
+    },
+    {
+        "DOI": "10.1007/978-3-319-76168-8_7",
+        "NAME": "\"Cross-Evaluation of Automated Term Extraction Tools by Measuring Terminological Saturation\"",
+        "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-319-76168-8_7"
+    },
+    {
         "DOI": "10.1007/978-3-319-74433-9_2",
-        "NAME": "Semantic Discovery in the Web of Things",
+        "NAME": "\"Semantic Discovery in the Web of Things\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-319-74433-9_2"
     },
     {
         "DOI": "10.1007/978-3-319-62530-0_8",
-        "NAME": "Characterize a human-robot interaction: Robot personal assistance",
+        "NAME": "\"Characterize a human-robot interaction: Robot personal assistance\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-319-62530-0_8"
     },
     {
         "DOI": "10.1007/978-3-030-03056-8_19",
-        "NAME": "DBtravel: A tourism-oriented semantic graph",
+        "NAME": "\"DBtravel: A tourism-oriented semantic graph\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-03056-8_19"
     },
     {
         "DOI": "10.1007/978-3-030-03056-8_27",
-        "NAME": "Type prediction of RDF knowledge graphs using binary classifiers with structural data",
+        "NAME": "\"Type prediction of RDF knowledge graphs using binary classifiers with structural data\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-03056-8_27"
     },
     {
         "DOI": "10.1007/978-3-030-03056-8_17",
-        "NAME": "Publishing tourism statistics as linked data a case study of Sri Lanka",
+        "NAME": "\"Publishing tourism statistics as linked data a case study of Sri Lanka\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-03056-8_17"
     },
     {
         "DOI": "10.1007/978-3-030-03056-8_26",
-        "NAME": "Knowledge base evolution analysis: A case study in the tourism domain",
+        "NAME": "\"Knowledge base evolution analysis: A case study in the tourism domain\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-03056-8_26"
     },
     {
         "DOI": "10.1007/978-3-030-03056-8_18",
-        "NAME": "Linked-Fiestas: A knowledge graph to promote cultural tourism in Spain",
+        "NAME": "\"Linked-Fiestas: A knowledge graph to promote cultural tourism in Spain\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-03056-8_18"
     },
     {
         "DOI": "10.1007/978-3-030-00178-0_24",
-        "NAME": "Reuse and Reengineering of Non-ontological Resources in the Legal Domain",
+        "NAME": "\"Reuse and Reengineering of Non-ontological Resources in the Legal Domain\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-00178-0_24"
     },
     {
         "DOI": "10.1007/978-3-030-00178-0_28",
-        "NAME": "A Linked Data Terminology for Copyright Based on Ontolex-Lemon",
+        "NAME": "\"A Linked Data Terminology for Copyright Based on Ontolex-Lemon\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-00178-0_28"
     },
     {
         "DOI": "10.1007/978-3-030-03667-6_8",
-        "NAME": "Requirements behaviour analysis for ontology testing",
+        "NAME": "\"Requirements behaviour analysis for ontology testing\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-03667-6_8"
     },
     {
         "DOI": "10.1007/978-3-030-03667-6_21",
-        "NAME": "Inferring types on large datasets applying ontology class hierarchy classifiers: The dbpedia case",
+        "NAME": "\"Inferring types on large datasets applying ontology class hierarchy classifiers: The dbpedia case\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/978-3-030-03667-6_21"
     },
     {
         "DOI": null,
         "NAME": "CREATING AND IMPROVING EDUCATIONAL MATERIALS: AN APPROACH BASED ON CROWDSOURCING",
         "PRIMARY_LOCATION": "https://doi.org/10.21125/iceri.2018.1854"
     },
     {
         "DOI": "10.1007/s11548-018-1727-5",
-        "NAME": "Reliability and correlation analysis of computed methods to convert conventional 2D radiological hindfoot measurements to a 3D setting using weightbearing CT",
+        "NAME": "\"Reliability and correlation analysis of computed methods to convert conventional 2D radiological hindfoot measurements to a 3D setting using weightbearing CT\"",
         "PRIMARY_LOCATION": "https://doi.org/10.1007/s11548-018-1727-5"
     },
     {
         "DOI": null,
         "NAME": "LawORDate: A service for distinguishing legal references from temporal expressions",
         "PRIMARY_LOCATION": "http://ceur-ws.org/Vol-2049/04paper.pdf"
     },
@@ -2627,14 +2727,19 @@
     {
         "DOI": null,
         "NAME": "Ontological requirement specification for smart irrigation systems: a SOSA/SSN and SAREF comparison",
         "PRIMARY_LOCATION": "https://hal.science/hal-02042584/document"
     },
     {
         "DOI": null,
+        "NAME": "A SAREF extension for semantic interoperability in the industry and manufacturing domain",
+        "PRIMARY_LOCATION": "https://doi.org/10.1002/9781119564034.ch25"
+    },
+    {
+        "DOI": null,
         "NAME": "Besoins ontologiques d'un syst\u00e8me d'irrigation intelligent: comparaison entre SSN et SAREF",
         "PRIMARY_LOCATION": "https://hal.science/hal-01841316/document"
     },
     {
         "DOI": null,
         "NAME": "Enabling interoperability-as-a-service for connected IoT infrastructures and Smart Objects",
         "PRIMARY_LOCATION": null
```

### Comparing `dataextractoroeg-0.3.9/doiExtractor/doiExtractor.py` & `dataextractoroeg-0.4.0/doiExtractor/doiExtractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import pandas as pd
 import urllib.parse
 import requests
 import csv
 import os
 
 
+
 # Function to extract the DOI
 def extract_doi(url_pagina, csv_file):
     response = requests.get(url_pagina)
 
     if response.status_code == 200:
         # Extract HTML content of the page
         html_doc = response.text
@@ -41,18 +42,15 @@
                 next_sibling = doi_text.find_next_sibling(string=True)
                 if next_sibling and next_sibling.strip():
                     # Extract DOI
                     doi = next_sibling.strip()
                     if doi.startswith('https://doi.org/'):
                         doi = doi[len('https://doi.org/'):]  # Remove "https://doi.org/" from the beginning if present
                     # Write the resulting DOI to the CSV file
-                    if title.startswith('"'):
-                        csv_file.writerow([title, doi])
-                    else:
-                        csv_file.writerow(['"' + title + '"', doi])
+                    csv_file.writerow([title, doi])
                     doi_found = True
                 else:
                     csv_file.writerow([title, "None"])
                     doi_found = False
                     
         return doi_found  # Return if DOI is found or not
     else:
@@ -63,15 +61,15 @@
 # Function to search for papers in the webpage
 def search_papers(url, url_docs, csv_filename):
 
     driver = webdriver.Chrome()
     driver.get(url)
 
     with open(csv_filename, "w", newline='', encoding='utf-8') as csv_file:
-        csv_writer = csv.writer(csv_file)
+        csv_writer = csv.writer(csv_file, quoting=csv.QUOTE_ALL)
         csv_writer.writerow(["NAME", "DOI"])
 
         total_publications = 0
         publications_with_doi = 0
 
         try:
             # Wait until "Publicaciones" button is clickable
@@ -147,15 +145,15 @@
             doi = row[1]
             existing_dois.add(doi)
 
     with open(csv2, 'r', newline='', encoding='utf-8') as papers_file:
         reader = csv.reader(papers_file)
         next(reader)  # Skip header row
         with open(csv1, 'a', newline='', encoding='utf-8') as existing_csv_file:
-            csv_writer = csv.writer(existing_csv_file)
+            csv_writer = csv.writer(existing_csv_file, quoting=csv.QUOTE_ALL)
             for row in reader:
                 doi = row[1]
                 if doi not in existing_dois:
                     csv_writer.writerow(row)
 
 
 def create_txt(csv_filename, txt_filename):
```

### Comparing `dataextractoroeg-0.3.9/doiExtractor/main.py` & `dataextractoroeg-0.4.0/doiExtractor/main.py`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3.9/doiExtractor/openAlex.py` & `dataextractoroeg-0.4.0/doiExtractor/openAlex.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,11 +89,11 @@
         print("-----------------------------------------------------------------")
 
     new_columns = list(rows[0].keys())  
     if "PRIMARY_LOCATION" not in new_columns: 
         new_columns.append("PRIMARY_LOCATION")
 
     with open(csv_filename, mode='w', newline='', encoding='utf-8') as file:
-        writer = csv.DictWriter(file, fieldnames=new_columns)
+        writer = csv.DictWriter(file, quoting=csv.QUOTE_ALL, fieldnames=new_columns)
         writer.writeheader()
         writer.writerows(rows)
```

### Comparing `dataextractoroeg-0.3.9/setup.py` & `dataextractoroeg-0.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="DataExtractorOEG",
-    version="0.3.9",
+    version="0.4.0",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "beautifulsoup4",
         "selenium",
         "requests",
         "pandas"
```

