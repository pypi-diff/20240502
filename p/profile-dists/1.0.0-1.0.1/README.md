# Comparing `tmp/profile_dists-1.0.0.tar.gz` & `tmp/profile_dists-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/profile_dists-1.0.0.tar", last modified: Thu Oct 19 19:16:53 2023, max compression
+gzip compressed data, was "profile_dists-1.0.1.tar", last modified: Thu May  2 15:56:00 2024, max compression
```

## Comparing `profile_dists-1.0.0.tar` & `profile_dists-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-10-19 19:16:53.000000 profile_dists-1.0.0/
--rw-r--r--   0 jrobertson   (502) staff       (20)    11357 2023-10-19 19:15:57.000000 profile_dists-1.0.0/LICENSE
--rw-r--r--   0 jrobertson   (502) staff       (20)        0 2023-10-19 19:15:57.000000 profile_dists-1.0.0/MANIFEST.in
--rw-r--r--   0 jrobertson   (502) staff       (20)      999 2023-10-19 19:16:53.000000 profile_dists-1.0.0/PKG-INFO
--rw-r--r--   0 jrobertson   (502) staff       (20)     9763 2023-10-19 19:15:57.000000 profile_dists-1.0.0/README.md
-drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-10-19 19:16:53.000000 profile_dists-1.0.0/profile_dists/
--rw-r--r--   0 jrobertson   (502) staff       (20)        0 2023-10-19 19:15:57.000000 profile_dists-1.0.0/profile_dists/__init__.py
--rw-r--r--   0 jrobertson   (502) staff       (20)      853 2023-10-19 19:15:57.000000 profile_dists-1.0.0/profile_dists/constants.py
--rw-r--r--   0 jrobertson   (502) staff       (20)    16210 2023-10-19 19:15:57.000000 profile_dists-1.0.0/profile_dists/main.py
-drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-10-19 19:16:53.000000 profile_dists-1.0.0/profile_dists/test_data/
--rw-r--r--   0 jrobertson   (502) staff       (20)        0 2023-10-19 19:15:57.000000 profile_dists-1.0.0/profile_dists/test_data/__init__.py
--rw-r--r--   0 jrobertson   (502) staff       (20)    24702 2023-10-19 19:15:57.000000 profile_dists-1.0.0/profile_dists/utils.py
--rw-r--r--   0 jrobertson   (502) staff       (20)       21 2023-10-19 19:15:57.000000 profile_dists-1.0.0/profile_dists/version.py
-drwxr-xr-x   0 jrobertson   (502) staff       (20)        0 2023-10-19 19:16:53.000000 profile_dists-1.0.0/profile_dists.egg-info/
--rw-r--r--   0 jrobertson   (502) staff       (20)      999 2023-10-19 19:16:53.000000 profile_dists-1.0.0/profile_dists.egg-info/PKG-INFO
--rw-r--r--   0 jrobertson   (502) staff       (20)      421 2023-10-19 19:16:53.000000 profile_dists-1.0.0/profile_dists.egg-info/SOURCES.txt
--rw-r--r--   0 jrobertson   (502) staff       (20)        1 2023-10-19 19:16:53.000000 profile_dists-1.0.0/profile_dists.egg-info/dependency_links.txt
--rw-r--r--   0 jrobertson   (502) staff       (20)       58 2023-10-19 19:16:53.000000 profile_dists-1.0.0/profile_dists.egg-info/entry_points.txt
--rw-r--r--   0 jrobertson   (502) staff       (20)      113 2023-10-19 19:16:53.000000 profile_dists-1.0.0/profile_dists.egg-info/requires.txt
--rw-r--r--   0 jrobertson   (502) staff       (20)       14 2023-10-19 19:16:53.000000 profile_dists-1.0.0/profile_dists.egg-info/top_level.txt
--rw-r--r--   0 jrobertson   (502) staff       (20)       38 2023-10-19 19:16:53.000000 profile_dists-1.0.0/setup.cfg
--rw-r--r--   0 jrobertson   (502) staff       (20)     1890 2023-10-19 19:16:35.000000 profile_dists-1.0.0/setup.py
+drwxr-xr-x   0 mwells    (1000) mwells    (1000)        0 2024-05-02 15:56:00.236650 profile_dists-1.0.1/
+-rw-r--r--   0 mwells    (1000) mwells    (1000)    11357 2024-05-02 15:47:56.000000 profile_dists-1.0.1/LICENSE
+-rw-r--r--   0 mwells    (1000) mwells    (1000)        0 2024-05-02 15:47:56.000000 profile_dists-1.0.1/MANIFEST.in
+-rw-r--r--   0 mwells    (1000) mwells    (1000)     1235 2024-05-02 15:56:00.236650 profile_dists-1.0.1/PKG-INFO
+-rw-r--r--   0 mwells    (1000) mwells    (1000)    12290 2024-05-02 15:47:56.000000 profile_dists-1.0.1/README.md
+drwxr-xr-x   0 mwells    (1000) mwells    (1000)        0 2024-05-02 15:56:00.236650 profile_dists-1.0.1/profile_dists/
+-rw-r--r--   0 mwells    (1000) mwells    (1000)        0 2024-05-02 15:47:56.000000 profile_dists-1.0.1/profile_dists/__init__.py
+-rw-r--r--   0 mwells    (1000) mwells    (1000)      853 2024-05-02 15:47:56.000000 profile_dists-1.0.1/profile_dists/constants.py
+-rwxr-xr-x   0 mwells    (1000) mwells    (1000)    16344 2024-05-02 15:47:56.000000 profile_dists-1.0.1/profile_dists/main.py
+drwxr-xr-x   0 mwells    (1000) mwells    (1000)        0 2024-05-02 15:56:00.236650 profile_dists-1.0.1/profile_dists/test_data/
+-rw-r--r--   0 mwells    (1000) mwells    (1000)        0 2024-05-02 15:47:56.000000 profile_dists-1.0.1/profile_dists/test_data/__init__.py
+-rw-r--r--   0 mwells    (1000) mwells    (1000)    24434 2024-05-02 15:47:56.000000 profile_dists-1.0.1/profile_dists/utils.py
+-rw-r--r--   0 mwells    (1000) mwells    (1000)       22 2024-05-02 15:48:41.000000 profile_dists-1.0.1/profile_dists/version.py
+drwxr-xr-x   0 mwells    (1000) mwells    (1000)        0 2024-05-02 15:56:00.236650 profile_dists-1.0.1/profile_dists.egg-info/
+-rw-r--r--   0 mwells    (1000) mwells    (1000)     1235 2024-05-02 15:56:00.000000 profile_dists-1.0.1/profile_dists.egg-info/PKG-INFO
+-rw-r--r--   0 mwells    (1000) mwells    (1000)      421 2024-05-02 15:56:00.000000 profile_dists-1.0.1/profile_dists.egg-info/SOURCES.txt
+-rw-r--r--   0 mwells    (1000) mwells    (1000)        1 2024-05-02 15:56:00.000000 profile_dists-1.0.1/profile_dists.egg-info/dependency_links.txt
+-rw-r--r--   0 mwells    (1000) mwells    (1000)       58 2024-05-02 15:56:00.000000 profile_dists-1.0.1/profile_dists.egg-info/entry_points.txt
+-rw-r--r--   0 mwells    (1000) mwells    (1000)      113 2024-05-02 15:56:00.000000 profile_dists-1.0.1/profile_dists.egg-info/requires.txt
+-rw-r--r--   0 mwells    (1000) mwells    (1000)       14 2024-05-02 15:56:00.000000 profile_dists-1.0.1/profile_dists.egg-info/top_level.txt
+-rw-r--r--   0 mwells    (1000) mwells    (1000)       38 2024-05-02 15:56:00.236650 profile_dists-1.0.1/setup.cfg
+-rw-r--r--   0 mwells    (1000) mwells    (1000)     1894 2024-05-02 15:48:25.000000 profile_dists-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `profile_dists-1.0.0/LICENSE` & `profile_dists-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `profile_dists-1.0.0/README.md` & `profile_dists-1.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,129 @@
 [![PyPI](https://img.shields.io/badge/Install%20with-PyPI-blue)](https://pypi.org/project/profile_dists/#description)
 [![Bioconda](https://img.shields.io/badge/Install%20with-bioconda-green)](https://anaconda.org/bioconda/profile_dists)
 [![Conda](https://img.shields.io/conda/dn/bioconda/profile_dists?color=green)](https://anaconda.org/bioconda/profile_dists)
 [![License: Apache-2.0](https://img.shields.io/github/license/phac-nml/profile_dists)](https://www.apache.org/licenses/LICENSE-2.0)
 
 
-## Profile Dists
+# Profile Dists
+![alt text](https://github.com/phac-nml/profile_dists/blob/main/logo.png?raw=true)
 
-## Contents
 
-- [Introduction](#introduction)
-- [Installation](#installation)
-- [Usage](#usage)
-- [Quick Start](#quick-start)
-- [FAQ](#faq)
-- [Citation](#citation)
-- [Legal](#legal)
-- [Contact](#contact)
-
-## Introduction
+# Introduction
 
 Surveillance and outbreak analysis of pathogens has been operationalized by multiple public health laboratories around 
 the world using gene-by-gene approaches. Gene by gene comparisons can be considered the next iteration of multi-locus seuence typing 
 (MLST) due to the compression of large amounts of sequence information into a set of integer allele identifiers according to a 
 defined schema. There are a variety of software approaches available to call allele profiles from schemes such as 
 [chewBBACA](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5885018/). Additionally there are tools available which can calculate 
 a distant matrix using the standardized allele profile format of ['name', 'locus_1','locus_2'...'locus_n'] in the form of 
 [GrapeTree](https://github.com/achtman-lab/GrapeTree). However, this method is not tolerant of non-integer data in loci columns and
 one of the strengths of chewBBACA is that it will provide additional information in columns in the case of partial matches etc.
 Furthermore, there is interest in utilizing hashing of allele sequences for deterministic labelling of alleles without the need
 for a centralized allele nomenclature service. Additionally, GrapeTree does not provide functionality for querying samples against
 a database of samples. Furthermore, the memory requirements of GrapeTree grow significantly with the number of samples being compared
 as the distance matrix is held in memory. As datasets grow, using text based formats such as CSV, TSV represent significant amounts of runtime in terms
 of reading, parsing and writing.  New formats such as [parquet](https://parquet.apache.org/) support compression and are optimized for 
-efficiency of storage and retreiveal of data.
+efficiency of storage and retrieval of data.
 <br><br>
 To address needs of users within our team we have designed an integrated solution for calculating distance matricies and querying of genetically
 similar samples within a defined threshold to support outbreak and surveillance activities. We provide the flexibility to have standard text 
 based outputs as well as parquet. It is implemented in pure python and currently is only available in a single threaded version but later
 refinements may include the support for multiprocessing. To facilitate integration of the tool into larger workflows it will also be implemented 
 as a nextflow workflow.
 
 
-## Installation
+## Citation
+
+Robertson, James, Wells, Matthew, Schonfeld, Justin, Reimer, Aleisha. Profile Dists: Convenient package for comparing genetic similarity of samples based on allelic profiles. 2023. https://github.com/phac-nml/profile_dists
+
+## Contact
+
+For any questions, issues or comments please make a Github issue or reach out to [**James Robertson**](james.robertson@phac-aspc.gc.ca).
+
+# Install
 
 Install the latest released version from conda:
 
         conda create -c bioconda -c conda-forge -n profile_dists profile_dists
 
 Install using pip:
 
         pip install profile_dists
 
 Install the latest master branch version directly from Github:
 
         pip install git+https://github.com/phac-nml/profile_dists.git
 
+### Compatibility
+
+All required packages are listed in the setup.py. The package does require [Numba](https://numba.pydata.org/) to JIT compile certain functions, if any issues during installation are encountered please make an issue on the repository.
 
+# Getting Started
 
 ## Usage
-If you run ``profile_dists``, you should see the following usage statement:
 
-    usage: dist.py [-h] --query QUERY --ref REF --outdir OUTDIR [--outfmt OUTFMT]
-                   [--file_type FILE_TYPE] [--distm DISTM]
-                   [--missing_thresh MISSING_THRESH]
-                   [--sample_qual_thresh SAMPLE_QUAL_THRESH]
-                   [--match_threshold MATCH_THRESHOLD]
-                   [--mapping_file MAPPING_FILE] [--force] [-s] [-V]
+### Command Line Options
+If you run ``profile_dists --help``, you should see the following usage statement describing each parameter `profile_dists` accepts:
+
+        Profile Dists: Calculate genetic distances based on allele profiles v. 1.0.0
+
+        options:
+                -h, --help            show this help message and exit
+                --query QUERY, -q QUERY
+                                        Query allelic profiles (default: None)
+                --ref REF, -r REF     Reference allelic profiles (default: None)
+                --outdir OUTDIR, -o OUTDIR
+                                        Result output files (default: None)
+                --outfmt OUTFMT, -u OUTFMT
+                                        Out format [matrix, pairwise] (default: matrix)
+                --file_type FILE_TYPE, -e FILE_TYPE
+                                        Out format [text, parquet] (default: text)
+                --distm DISTM, -d DISTM
+                                        Distance method raw hamming or scaled difference [hamming, scaled] (default: scaled)
+                --missing_thresh MISSING_THRESH, -t MISSING_THRESH
+                                        Maximum percentage of missing data allowed per locus (0 - 1) (default: 1.0)
+                --sample_qual_thresh SAMPLE_QUAL_THRESH, -c SAMPLE_QUAL_THRESH
+                                        Maximum percentage of missing data allowed per sample (0 - 1) (default: 1.0)
+                --match_threshold MATCH_THRESHOLD, -a MATCH_THRESHOLD
+                                        Either a integer or float depending on what distance method is used (only used with pairwise format (default: -1)
+                --mapping_file MAPPING_FILE, -m MAPPING_FILE
+                                        json formatted allele mapping (default: None)
+                --batch_size BATCH_SIZE
+                                        Manual selection of how many records should be included in a batch, default=auto (default: None)
+                --max_mem MAX_MEM     Maximum amount of memory to use (default: None)
+                --force, -f           Overwrite existing directory (default: False)
+                -s, --skip            Skip QA/QC steps (default: False)
+                --columns COLUMNS     Single column file with one column name per line or list of columns comma separate (default: None)
+                -n, --count_missing   Count missing as differences (default: False)
+                -p CPUS, --cpus CPUS  Count missing as differences (default: 1)
+                -V, --version         show program's version number and exit 
+
+### Quick start
+
+#### **Distance matrix calculation**
+
+The default behaviour of profile dists is to construct a pairwise distance matrix with the columns representing the
+reference sequences and rows representing the query sequences. For clustering analysis, you can construct a symmertic/square
+distance matrix by supplying the same profile as reference and query.
+
+```
+profile_dists --query samples.profile --ref samples.profile --outdir results
+```
+
+#### Fast Matching
+
+Profile dists also suports querying of a set of sample profiles against a reference database and reporting that as either a
+matrix or three column table of [ query_id, reference_id, dist ]
 
+```
+profile_dists --query queries.profile --ref reference.profile --outdir results --match_threshold 10
+```
+
+## Data Input/Formats
 Supported profile formats
 =====
 **Native**
 
 |  id  |  locus_1  |  locus_2  |  locus_3  |  locus_4  |  locus_5  |  locus_6  |  locus_7  | 
 | ----------- | ----------- |----------- | ----------- | ----------- |----------- | ----------- | ----------- |
 |  S1  |	1  |  1  |  1  |  1  |  1  |  1  |  1  | 
@@ -105,70 +158,46 @@
 |  S3  |	dc0a04880d1ad381ffd54ce9f6ad1e7a  |  04d45219ee5f6065caf426ba740215e5  |  9fc502308c616ae34146d7f7b0081bd8  |  4577dec2c840472800a3b104c88bb0ef  |  80c8156d77d724ac0bb16ec60993bc84  |  874225c0dec5219dd64584ba32938dbd  |  e1ee776b32c2f6131a7238ce50b75469  | 
 |  S4  |	dc0a04880d1ad381ffd54ce9f6ad1e7a  |  -  |  e79562c280691c321612ecdf0dadad9e  |  4577dec2c840472800a3b104c88bb0ef  |  80c8156d77d724ac0bb16ec60993bc84  |  c8087ad8b01d9f88e8eb2c3775ef2e64  |  e1ee776b32c2f6131a7238ce50b75469  | 
 |  S5  |	dc0a04880d1ad381ffd54ce9f6ad1e7a  |  04d45219ee5f6065caf426ba740215e5  |  -  |  4577dec2c840472800a3b104c88bb0ef  |  80c8156d77d724ac0bb16ec60993bc84  |  4d547ea59e90173e8385005e706aae96  | e1ee776b32c2f6131a7238ce50b75469  | 
 |  S6  |	8214e9d02d1b11e6239d6a55d4acd993  |  -  |  e79562c280691c321612ecdf0dadad9e  |  -  |  -  |  e3088425be5e7de8d9a95da8e59a9ea8  |  -  | 
 
 - Direct support for missing data in the form of ?, 0, - or space
 
-Output Profile
+## Output/Results
+
+### Output Profile
 =====
 **Native**
 
 |  id  |  locus_1  |  locus_2  |  locus_3  |  locus_4  |  locus_5  |  locus_6  |  locus_7  | 
 | ----------- | ----------- |----------- | ----------- | ----------- |----------- | ----------- | ----------- |
 |  S1  |	1  |  1  |  1  |  1  |  1  |  1  |  1  | 
 |  S2  |	1  |  1  |  2  |  2  |  0  |  4  |  1  | 
 |  S3  |	1  |  2  |  2  |  2  |  1  |  5  |  1  | 
 |  S4  |	1  |  2  |  3  |  2  |  1  |  6  |  1  | 
 |  S5  |	1  |  2  |  0  |  2  |  1  |  8  |  1  | 
 |  S6  |	2  |  3 |  3  |  0  |  0  |  9  |  0  | 
 
 - All columns are converted to contain only integers with missing data represented as a 0
 
-
-Quick start
-=====
-**Distance matrix calculation**
-
-The default behaviour of profile dists is to construct a pairwise distance matrix with the columns representing the
-reference sequences and rows representing the query sequences. For clustering analysis, you can construct a symmertic/square
-distance matrix by supplying the same profile as reference and query.
-
-<br />
-
-        profile_dists --query samples.profile --ref samples.profile --outdir results
-
-Profile dists also suports querying of a set of sample profiles against a reference database and reporting that as either a
-matrix or three column table of [ query_id, reference_id, dist ]
-
-<br />
-
-        profile_dists --query queries.profile --ref reference.profile --outdir results --match_threshold 10
-
-**Outputs:**
+### Output Directory Structure
 
 ```
 {Output folder name}
 ├── allele_map.json - Mapping of allele hash string to integer id, can be use for reruning of analyses or masking specific alleles
 ├── query_profile.{text|parquet}  - Standardized allele profile for query sequences
 ├── ref_profile.{text|parquet}  - Standardized allele profile for reference sequences
 ├── results.{text|parquet} - Either symmetric distance matrix or three column file of [query_id, ref_if, distance]
 └── run.json - Contains logging information for the run including parameters and quality information
 ```
-## Benchmarks
 
-Coming soon
+## Troubleshooting and FAQs:
 
-## FAQ
+No issues are currently reported.
 
-Coming soon
-
-## Citation
-
-Robertson, James, Wells, Matthew, Schonfeld, Justin, Reimer, Aleisha. Profile Dists: Convenient package for comparing genetic similarity of samples based on allelic profiles. 2023. https://github.com/phac-nml/profile_dists
 
 ## Legal
 
 Copyright Government of Canada 2023
 
 Written by: National Microbiology Laboratory, Public Health Agency of Canada
 
@@ -180,10 +209,10 @@
 
 Unless required by applicable law or agreed to in writing, software distributed
 under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
 CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 
 
-## Contact
+# Updates and Release Notes:
 
-**James Robertson**: james.robertson@phac-aspc.gc.ca
+v1.0.0
```

### Comparing `profile_dists-1.0.0/profile_dists/constants.py` & `profile_dists-1.0.1/profile_dists/constants.py`

 * *Files identical despite different names*

### Comparing `profile_dists-1.0.0/profile_dists/main.py` & `profile_dists-1.0.1/profile_dists/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     count_missing_sites = cmd_args.count_missing
     max_mem = cmd_args.max_mem
     batch_size = cmd_args.batch_size
     num_cpus = cmd_args.cpus
     columns = cmd_args.columns
 
 
+
     try:
         sys_num_cpus = len(os.sched_getaffinity(0))
     except AttributeError:
         sys_num_cpus = cpu_count()
 
     if num_cpus > sys_num_cpus:
         num_cpus = sys_num_cpus
@@ -239,14 +240,19 @@
             qdf = filter_columns(qdf, cols_to_remove)
             rdf = filter_columns(rdf, cols_to_remove)
 
     #convert profiles for fast dist calculations
     qlabels,qprofiles = convert_profiles(qdf)
     rlabels,rprofiles = convert_profiles(rdf)
 
+    samples = set(qlabels) | set(rlabels)
+    num_samples = len(samples)
+    if num_samples < 100:
+        batch_size = num_samples
+
     run_data['query_profile_info']['num_samples'] = len(qlabels)
     run_data['query_profile_info']['num_samples_pass'] = run_data['query_profile_info']['num_samples']
     run_data['ref_profile_info']['num_samples'] = len(qlabels)
     run_data['ref_profile_info']['num_samples_pass'] = run_data['ref_profile_info']['num_samples']
 
     if not skip:
         print(f'Performing QA/QC on input sample profiles')
```

### Comparing `profile_dists-1.0.0/profile_dists/utils.py` & `profile_dists-1.0.1/profile_dists/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,14 +202,15 @@
     column_dtypes = df.dtypes.tolist()
     is_correct_format = is_all_columns_int(column_dtypes)
 
     #If all columns are already integers then skip the extra processing steps
     if is_correct_format:
         return (column_mapping, df)
 
+    df = df.fillna('0')
     df = df.replace('?', '0', regex=False)
     df = df.replace(' ', '0', regex=False)
     df = df.replace('-', '0', regex=False)
     df = df.replace('', '0', regex=False)
 
     for column in columns:
         unique_col_values = sorted(df[column].unique().tolist())
@@ -454,18 +455,15 @@
     #Clear an existing file as this can cause unexpected behaviour
     if os.path.isfile(parquet_file):
         os.remove(parquet_file)
 
     for i in range(0, num_query_profiles):
         d = [ query_labels[i] ]
         for k in range(0, num_ref_profiles):
-            if i != k:
                 d.append(get_distance_scaled(query_profiles[i], ref_profiles[k]))
-            else:
-                d.append(0)
         dists.append(d)
         count += 1
 
         if count == batch_size:
             sys.stderr.write(f"{i} batch\n")
             df = pd.DataFrame(dists, columns=columns)
             if not os.path.isfile(parquet_file):
@@ -506,18 +504,16 @@
     #Clear an existing file as this can cause unexpected behaviour
     if os.path.isfile(parquet_file):
         os.remove(parquet_file)
 
     for i in range(0, num_query_profiles):
         d = [ query_labels[i] ]
         for k in range(0, num_ref_profiles):
-            if i != k:
-                d.append(get_distance_scaled_missing(query_profiles[i], ref_profiles[k]))
-            else:
-                d.append(0)
+            d.append(get_distance_scaled_missing(query_profiles[i], ref_profiles[k]))
+
         dists.append(d)
         count += 1
 
         if count == batch_size:
             df = pd.DataFrame(dists, columns=columns)
             if not os.path.isfile(parquet_file):
                 fp.write(parquet_file, df, compression='GZIP')
@@ -530,15 +526,15 @@
     if not os.path.isfile(parquet_file):
         fp.write(parquet_file, df, compression='GZIP')
     else:
         fp.write(parquet_file, df, append=True, compression='GZIP')
 
 def calc_distances_hamming(query_profiles,query_labels,ref_profiles,ref_labels,parquet_file,batch_size=1):
     '''
-    Calculates pairwise hamming distances between ref and query with  with missing data ignored
+    Calculates pairwise hamming distances between ref and query with missing data ignored
     :param query_profiles: list of integer numpy profiles
     :param query_labels:  list of data labels for query
     :param ref_profiles: list of integer numpy profiles
     :param ref_labels: list of data labels for ref
     :param parquet_file: string path
     :param batch_size: int number of records to process concurrently
     :return: None
@@ -552,18 +548,16 @@
     #Clear an existing file as this can cause unexpected behaviour
     if os.path.isfile(parquet_file):
         os.remove(parquet_file)
 
     for i in range(0, num_query_profiles):
         d = [ query_labels[i] ]
         for k in range(0, num_ref_profiles):
-            if i != k:
-                d.append(get_distance_raw(query_profiles[i], ref_profiles[k]))
-            else:
-                d.append(0)
+            d.append(get_distance_raw(query_profiles[i], ref_profiles[k]))
+
         dists.append(d)
         count += 1
 
         if count == batch_size:
             df = pd.DataFrame(dists, columns=columns)
             if not os.path.isfile(parquet_file):
                 fp.write(parquet_file, df, compression='GZIP')
@@ -599,18 +593,15 @@
     #Clear an existing file as this can cause unexpected behaviour
     if os.path.isfile(parquet_file):
         os.remove(parquet_file)
 
     for i in range(0, num_query_profiles):
         d = [ query_labels[i] ]
         for k in range(0, num_ref_profiles):
-            if i != k:
-                d.append(get_distance_raw_missing(query_profiles[i], ref_profiles[k]))
-            else:
-                d.append(0)
+            d.append(get_distance_raw_missing(query_profiles[i], ref_profiles[k]))
         dists.append(d)
         count += 1
 
         if count == batch_size:
             df = pd.DataFrame(dists, columns=columns)
             if not os.path.isfile(parquet_file):
                 fp.write(parquet_file, df, compression='GZIP')
```

### Comparing `profile_dists-1.0.0/setup.py` & `profile_dists-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 exec(open('profile_dists/version.py').read())
 
 setup(
     name='profile_dists',
     include_package_data=True,
     version=__version__,
-    python_requires='>=3.8.2,<4',
+    python_requires='>=3.8.2,<3.12',
     setup_requires=['pytest-runner'],
     tests_require=['pytest'],
     packages=find_packages(exclude=['tests']),
     url='https://github.com/phac-nml/profile_dists',
     license='GPLv3',
     author='James Robertson',
     author_email='james.robertson@phac-aspc.gc.ca',
@@ -60,8 +60,8 @@
     ],
 
     entry_points={
         'console_scripts': [
             'profile_dists=profile_dists.main:main',
         ],
     },
-)
+)
```

