# Comparing `tmp/wgscovplot-1.0.1.tar.gz` & `tmp/wgscovplot-1.0.2.tar.gz`

## Comparing `wgscovplot-1.0.1.tar` & `wgscovplot-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 wgscovplot-1.0.1/web/wgscovplot.html.j2
--rw-r--r--   0        0        0   886108 2020-02-02 00:00:00.000000 wgscovplot-1.0.1/web/build/wgscovplot.js
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 wgscovplot-1.0.1/wgscovplot/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wgscovplot-1.0.1/wgscovplot/__init__.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 wgscovplot-1.0.1/wgscovplot/cli.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 wgscovplot-1.0.1/wgscovplot/colors.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 wgscovplot-1.0.1/wgscovplot/config.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 wgscovplot-1.0.1/wgscovplot/db.py
--rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 wgscovplot-1.0.1/wgscovplot/features.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 wgscovplot-1.0.1/wgscovplot/flu.py
--rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 wgscovplot-1.0.1/wgscovplot/io.py
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 wgscovplot-1.0.1/wgscovplot/rtpcr.py
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 wgscovplot-1.0.1/wgscovplot/util.py
--rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 wgscovplot-1.0.1/wgscovplot/wgscovplot.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wgscovplot-1.0.1/wgscovplot/tools/__init__.py
--rw-r--r--   0        0        0    26446 2020-02-02 00:00:00.000000 wgscovplot-1.0.1/wgscovplot/tools/variants.py
--rw-r--r--   0        0        0    10531 2020-02-02 00:00:00.000000 wgscovplot-1.0.1/wgscovplot/tools/mosdepth/__init__.py
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 wgscovplot-1.0.1/wgscovplot/tools/mosdepth/flu.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 wgscovplot-1.0.1/.gitignore
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 wgscovplot-1.0.1/LICENSE
--rw-r--r--   0        0        0    12327 2020-02-02 00:00:00.000000 wgscovplot-1.0.1/README.md
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 wgscovplot-1.0.1/hatch_build.py
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 wgscovplot-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    13485 2020-02-02 00:00:00.000000 wgscovplot-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 wgscovplot-1.0.2/web/wgscovplot.html.j2
+-rw-r--r--   0        0        0   886108 2020-02-02 00:00:00.000000 wgscovplot-1.0.2/web/build/wgscovplot.js
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 wgscovplot-1.0.2/wgscovplot/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wgscovplot-1.0.2/wgscovplot/__init__.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 wgscovplot-1.0.2/wgscovplot/cli.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 wgscovplot-1.0.2/wgscovplot/colors.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 wgscovplot-1.0.2/wgscovplot/config.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 wgscovplot-1.0.2/wgscovplot/db.py
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 wgscovplot-1.0.2/wgscovplot/features.py
+-rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 wgscovplot-1.0.2/wgscovplot/flu.py
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 wgscovplot-1.0.2/wgscovplot/io.py
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 wgscovplot-1.0.2/wgscovplot/rtpcr.py
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 wgscovplot-1.0.2/wgscovplot/util.py
+-rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 wgscovplot-1.0.2/wgscovplot/wgscovplot.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wgscovplot-1.0.2/wgscovplot/tools/__init__.py
+-rw-r--r--   0        0        0    26474 2020-02-02 00:00:00.000000 wgscovplot-1.0.2/wgscovplot/tools/variants.py
+-rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 wgscovplot-1.0.2/wgscovplot/tools/mosdepth/__init__.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 wgscovplot-1.0.2/wgscovplot/tools/mosdepth/flu.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 wgscovplot-1.0.2/.gitignore
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 wgscovplot-1.0.2/LICENSE
+-rw-r--r--   0        0        0    12327 2020-02-02 00:00:00.000000 wgscovplot-1.0.2/README.md
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 wgscovplot-1.0.2/hatch_build.py
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 wgscovplot-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    13434 2020-02-02 00:00:00.000000 wgscovplot-1.0.2/PKG-INFO
```

### Comparing `wgscovplot-1.0.1/web/wgscovplot.html.j2` & `wgscovplot-1.0.2/web/wgscovplot.html.j2`

 * *Files identical despite different names*

### Comparing `wgscovplot-1.0.1/web/build/wgscovplot.js` & `wgscovplot-1.0.2/web/build/wgscovplot.js`

 * *Files identical despite different names*

### Comparing `wgscovplot-1.0.1/wgscovplot/cli.py` & `wgscovplot-1.0.2/wgscovplot/cli.py`

 * *Files identical despite different names*

### Comparing `wgscovplot-1.0.1/wgscovplot/colors.py` & `wgscovplot-1.0.2/wgscovplot/colors.py`

 * *Files identical despite different names*

### Comparing `wgscovplot-1.0.1/wgscovplot/db.py` & `wgscovplot-1.0.2/wgscovplot/db.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,39 @@
-from typing import Dict, List
-
 from pydantic import BaseModel
 
 from wgscovplot.features import EChartsFeature
 from wgscovplot.tools.mosdepth import MosdepthDepthInfo
 from wgscovplot.tools.mosdepth.flu import FluMosdepthDepthInfo
 
 
 class DBMixin(BaseModel):
-    samples: List[str]
+    samples: list[str]
     low_coverage_threshold: int = 10
 
 
 class SegmentedGenomeDB(DBMixin):
     """Singleton class containing all data to populate HTML plots for segmented viruses.
 
     The single instance of this class will be serialized into a JS object for populating plots in the final HTML output.
     """
 
-    segments: List[str]
-    segments_ref_id: Dict[str, Dict[str, str]]
-    segments_ref_seq: Dict[str, Dict[str, str]]
-    depths: Dict[str, Dict[str, str]]
-    mosdepth_info: Dict[str, Dict[str, FluMosdepthDepthInfo]]
-    primer_matches: Dict[str, Dict[str, List[Dict]]]
-    variants: Dict[str, Dict[str, List[Dict]]]
+    segments: list[str]
+    segments_ref_id: dict[str, dict[str, str]]
+    segments_ref_seq: dict[str, dict[str, str]]
+    depths: dict[str, dict[str, str]]
+    mosdepth_info: dict[str, dict[str, FluMosdepthDepthInfo]]
+    primer_matches: dict[str, dict[str, list[dict]]]
+    variants: dict[str, dict[str, list[dict]]]
 
 
 class DB(DBMixin):
     """Singleton class containing all data to populate HTML plots for viruses with an unsegmented genome.
 
     The single instance of this class will be serialized into a JS object for populating plots in the final HTML output.
     """
 
     ref_seq: str
-    depths: Dict[str, str]
-    amplicon_depths: Dict[str, List[Dict]]
-    mosdepth_info: Dict[str, MosdepthDepthInfo]
-    variants: Dict[str, List[Dict]]
-    echart_features: List[EChartsFeature]
+    depths: dict[str, str]
+    amplicon_depths: dict[str, list[dict]]
+    mosdepth_info: dict[str, MosdepthDepthInfo]
+    variants: dict[str, list[dict]]
+    echart_features: list[EChartsFeature]
```

### Comparing `wgscovplot-1.0.1/wgscovplot/features.py` & `wgscovplot-1.0.2/wgscovplot/features.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from itertools import cycle
-from typing import List, Optional
+from typing import Optional
 
 from pydantic import BaseModel
 
 from wgscovplot.colors import AmpliconColour, palette
 from wgscovplot.config import FeaturesProps
 from wgscovplot.util import overlap
 
@@ -38,29 +38,29 @@
 class EChartsFeature(BaseModel):
     name: str
     value: EChartsFeatureValue
     itemStyle: EChartsItemStyle  # noqa: N815
 
 
 def build_echarts_features_array(
-    gene_features: Optional[List[Feature]],
-    amplicon_features: Optional[List[Feature]],
+    gene_features: Optional[list[Feature]],
+    amplicon_features: Optional[list[Feature]],
     fp: Optional[FeaturesProps] = None,
-) -> List[EChartsFeature]:
+) -> list[EChartsFeature]:
     """Build a list of gene/amplicon feature properties for ECharts
 
     Args:
         gene_features: List of gene Feature objects parsed from GFF or Genbank
         amplicon_features: List of amplicon Feature objects parsed from amplicon BED file
         fp: Feature properties for plotting with ECharts
 
     """
     if fp is None:
         fp = FeaturesProps()
-    out: List[EChartsFeature] = []
+    out: list[EChartsFeature] = []
     colour_cycle = cycle(palette)
     fcminus = FeatureCoords()
     fcplus = FeatureCoords()
     next_plus_strand_level = fp.plus_strand_level + fp.rec_items_height + fp.gene_feature_padding
     next_minus_strand_level = fp.minus_strand_level + fp.rec_items_height + fp.gene_feature_padding
     if gene_features:
         colour_cycle = cycle(colour_cycle)
```

### Comparing `wgscovplot-1.0.1/wgscovplot/flu.py` & `wgscovplot-1.0.2/wgscovplot/flu.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 from collections import defaultdict
 from pathlib import Path
-from typing import DefaultDict, Dict
 
 import pandas as pd
 from Bio.SeqIO.FastaIO import SimpleFastaParser
 from pydantic import BaseModel
 
 from wgscovplot.tools.mosdepth import SAMPLE_NAME_CLEANUP
 from wgscovplot.util import find_file_for_each_sample, select_most_recent_file
@@ -57,30 +56,30 @@
             "ref_sequence_id",
         ],
     )
 
 
 def get_segments_ref_id(sample_top_references: list[SampleSegmentRef]) -> dict[str, dict[str, str]]:
     """Get reference id for each segment of each sample"""
-    out: DefaultDict[str, Dict[str, str]] = defaultdict(dict)
+    out: defaultdict[str, dict[str, str]] = defaultdict(dict)
     for items in sample_top_references:
         out[items.sample][items.segment] = items.ref_id
     return dict(out)
 
 
 def get_sample_segment_seqs(
     basedir: Path,
     sample_top_references: list[SampleSegmentRef],
 ) -> dict[str, dict[str, str]]:
     """Get sequence for each segment of each sample
 
     This function assumes that the nf-flu pipeline was used, so the consensus sequence would have the filename format:
     {sample}.Segment_{segment}.{ref_id}.bcftools.consensus.fasta
     """
-    out: DefaultDict[str, Dict[str, str]] = defaultdict(dict)
+    out: defaultdict[str, dict[str, str]] = defaultdict(dict)
     # Find the most recently modified FASTA file for each sample for each segment
     # Only do the glob search once rather than once for every sample and segment
     filename_to_fasta_file = find_file_for_each_sample(
         basedir,
         glob_patterns=["**/*.fasta"],
         sample_name_cleanup=[".reference", ".fasta"],
         single_entry_selector_func=select_most_recent_file,
```

### Comparing `wgscovplot-1.0.1/wgscovplot/io.py` & `wgscovplot-1.0.2/wgscovplot/io.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import logging
+from collections import OrderedDict
 from io import TextIOWrapper
 from pathlib import Path
-from typing import List, Optional, OrderedDict, Tuple, Union
+from typing import Optional, Union
 
 from BCBio import GFF
 from Bio import Entrez, SeqIO
 from Bio.SeqFeature import SeqFeature
 from Bio.SeqRecord import SeqRecord
 from jinja2 import Environment, FileSystemLoader
 
 from wgscovplot.db import DB, SegmentedGenomeDB
 from wgscovplot.features import Feature
 from wgscovplot.tools import mosdepth
+from wgscovplot.util import get_ref_name_bam
 
 logger = logging.getLogger(__name__)
 
-REF_FASTA_GLOB_PATTERN = "**/genome/**/*.fa*"
-GFF_GLOB_PATTERN = "**/genome/**/*.gff"
+REF_FASTA_GLOB_PATTERN = "*.fa*"
+GFF_GLOB_PATTERN = "*.gff"
 
 
 def write_html_coverage_plot(
     db: Union[DB, SegmentedGenomeDB],
     output_html: Path,
 ) -> None:
     """Write HTML coverage plot"""
@@ -38,51 +40,51 @@
         fout.write(
             template_file.render(
                 db=db.model_dump(),
             )
         )
 
 
-def parse_gff(path: Path) -> List[Feature]:
+def parse_gff(path: Path) -> list[Feature]:
     out = []
     with open(path) as fh:
         interest_info = {"gff_type": ["gene", "five_prime_UTR", "three_prime_UTR"]}
         rec: SeqRecord
         for rec in GFF.parse(fh, limit_info=interest_info):
             feature: SeqFeature
             for feature in rec.features:
                 start_pos = int(feature.location.start) + 1
                 end_pos = int(feature.location.end)
                 strand = int(feature.location.strand)
-                qs: OrderedDict[str, List[str]] = feature.qualifiers
+                qs: OrderedDict[str, list[str]] = feature.qualifiers
                 feature_name = qs["Name"][0] if "Name" in qs else qs["gbkey"][0]
                 out.append(Feature(start=start_pos, end=end_pos, strand=strand, name=feature_name))
     out.sort(key=lambda k: k.start)
     return out
 
 
-def parse_genbank(gb_handle_or_path: Union[Path, TextIOWrapper]) -> Tuple[str, List[Feature]]:
+def parse_genbank(gb_handle_or_path: Union[Path, TextIOWrapper]) -> tuple[str, list[Feature]]:
     """Parse sequence and features from Genbank
 
     Args:
         gb_handle_or_path: Handle or path to Genbank file
     """
-    features: List[Feature] = []
+    features: list[Feature] = []
     skip_feature = {"CDS", "source", "repeat_region", "misc_feature"}
     seq = ""
     for seq_record in SeqIO.parse(gb_handle_or_path, "gb"):
         seq = str(seq_record.seq)
         seq_feature: SeqFeature
         for seq_feature in seq_record.features:
             if seq_feature.type in skip_feature:
                 continue
             if seq_feature.type in ["5'UTR", "3'UTR"]:
                 feature_name = seq_feature.type
             else:
-                qs: OrderedDict[str, List[str]] = seq_feature.qualifiers
+                qs: OrderedDict[str, list[str]] = seq_feature.qualifiers
                 gene = qs.get("gene")
                 locus_tag = qs.get("locus_tag")
                 if gene:
                     feature_name = gene[0]
                 elif locus_tag:
                     feature_name = locus_tag[0]
                 else:
@@ -93,28 +95,36 @@
             features.append(Feature(start=start_pos, end=end_pos, strand=strand, name=feature_name))
     features.sort(key=lambda f: f.start)
     return seq, features
 
 
 def get_ref_seq_and_annotation(
     input_dir: Path,
-) -> Tuple[Optional[str], Optional[List[Feature]]]:
-    gff_path = find_ref_gff(input_dir)
+) -> tuple[Optional[str], Optional[list[Feature]]]:
+    try:
+        ref_id = mosdepth.get_refseq_id(input_dir)
+    except Exception as e:
+        logger.error(f"Error getting ref seq ID: {e}")
+        ref_id = None
+    if not ref_id:
+        ref_id = get_refseq_id_from_bam(input_dir)
+    if ref_id is None:
+        logger.error("Could not find reference sequence ID from BAM file. Exiting.")
+        return None, None
+    gff_path = find_ref_gff(input_dir, refseq_id=ref_id)
     gene_features = parse_gff(gff_path) if gff_path else None
-    fasta_path = find_ref_fasta(input_dir)
+    fasta_path = find_ref_fasta(input_dir, refseq_id=ref_id)
     ref_seq = read_first_seq_from_fasta(fasta_path) if fasta_path else None
     if ref_seq is None or gene_features is None:
-        logger.info(f"Could not find GFF or parse FASTA. Trying to get ref seq ID from {input_dir}")
-        ref_id = mosdepth.get_refseq_id(input_dir)
-        logger.info(f"Ref seq id={ref_id}")
+        logger.info(f"Could not find GFF or parse FASTA. Fetching from NCBI for ref seq ID {ref_id}")
         ref_seq, gene_features = fetch_ref_seq_from_ncbi_entrez(ref_id)
     return ref_seq, gene_features
 
 
-def fetch_ref_seq_from_ncbi_entrez(ref_id: str) -> Tuple[Optional[str], Optional[List[Feature]]]:
+def fetch_ref_seq_from_ncbi_entrez(ref_id: str) -> tuple[Optional[str], Optional[list[Feature]]]:
     if not ref_id:
         logger.info("No ref seq ID provided. Cannot fetch seq from NCBI.")
         return None, None
     logger.info(f'Fetching reference sequence "{ref_id}" from NCBI Entrez')
     with Entrez.efetch(db="nucleotide", rettype="gb", retmode="text", id=ref_id) as handle:
         return parse_genbank(handle)
 
@@ -122,15 +132,47 @@
 def read_first_seq_from_fasta(fasta_path: Path) -> str:
     with open(fasta_path) as fh:
         for _, seq in SeqIO.FastaIO.SimpleFastaParser(fh):
             return seq
     return ""
 
 
-def find_ref_fasta(input_dir: Path) -> Optional[Path]:
-    ref_fasta_paths = list(input_dir.glob(REF_FASTA_GLOB_PATTERN))
-    return ref_fasta_paths[0] if ref_fasta_paths else None
+def find_ref_fasta(input_dir: Path, refseq_id: str) -> Optional[Path]:
+    for path in input_dir.rglob(REF_FASTA_GLOB_PATTERN):
+        with open(path) as fh:
+            for line in fh:
+                if line.startswith(">"):
+                    header = line.split()[0]
+                    if refseq_id in header:
+                        return path
+                    else:
+                        break
+                if line.strip() == "":
+                    continue
+                else:
+                    break
+    return None
+
+
+def find_ref_gff(input_dir: Path, refseq_id: str) -> Optional[Path]:
+    gff_paths = list(input_dir.rglob(GFF_GLOB_PATTERN))
+    for gff_path in gff_paths:
+        with open(gff_path) as fh:
+            for line in fh:
+                if line.startswith("#"):
+                    continue
+                first_col = line.split("\t")[0]
+                if refseq_id in first_col:
+                    return gff_path
+                else:
+                    break
+    return None
 
 
-def find_ref_gff(input_dir: Path) -> Optional[Path]:
-    gff_paths = list(input_dir.glob(GFF_GLOB_PATTERN))
-    return gff_paths[0] if gff_paths else None
+def get_refseq_id_from_bam(input_dir: Path) -> Optional[str]:
+    try:
+        bam_path = next(input_dir.rglob("*.bam"))
+        return get_ref_name_bam(bam_path) if bam_path else None
+    except Exception as e:
+        logger.error(f"Error getting ref seq ID from BAM file: {e}")
+        ref_id = None
+    return ref_id
```

### Comparing `wgscovplot-1.0.1/wgscovplot/rtpcr.py` & `wgscovplot-1.0.2/wgscovplot/rtpcr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from collections import defaultdict
 from pathlib import Path
-from typing import DefaultDict, Dict
 
 import edlib
 from Bio import SeqIO
 from pydantic import BaseModel
 
 from wgscovplot.util import expand_degenerate_bases
 
@@ -18,18 +17,18 @@
     other_locations: str
     query_aligned: str
     matched_aligned: str
     target_aligned: str
 
 
 def flu_rtpcr_matches(
-    primer_seq_path: Path, sample_seg_seq: Dict[str, Dict[str, str]], edit_distance_threshold: int
-) -> DefaultDict[str, DefaultDict[str, list[PrimerMatch]]]:
+    primer_seq_path: Path, sample_seg_seq: dict[str, dict[str, str]], edit_distance_threshold: int
+) -> defaultdict[str, defaultdict[str, list[PrimerMatch]]]:
     """Find real-time PCR primer/probe matches to each segment of each sample using Edlib."""
-    out: DefaultDict[str, DefaultDict[str, list[PrimerMatch]]] = defaultdict(lambda: defaultdict(list))
+    out: defaultdict[str, defaultdict[str, list[PrimerMatch]]] = defaultdict(lambda: defaultdict(list))
     primer_seq_record = [(record.id, record.seq) for record in SeqIO.parse(open(primer_seq_path), "fasta")]
     for sample, seg_seq in sample_seg_seq.items():
         for seg, seq in seg_seq.items():
             if len(seq):
                 for seq_id, primer_seq in primer_seq_record:
                     alns = []
                     for pseq in expand_degenerate_bases(primer_seq):
```

### Comparing `wgscovplot-1.0.1/wgscovplot/util.py` & `wgscovplot-1.0.2/wgscovplot/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import contextlib
 import logging
 import re
 from collections import defaultdict
 from itertools import product
 from pathlib import Path
-from typing import Any, Callable, Iterable, List, Mapping, Optional, Union
+from typing import Any, Callable, Iterable, Mapping, Optional, Union
 
 import numpy as np
 import pandas as pd
 
-ListOfStrOrPattern = Union[List[str], List[re.Pattern[str]], List[Union[str, re.Pattern[str]]]]
+ListOfStrOrPattern = Union[list[str], list[re.Pattern[str]], list[Union[str, re.Pattern[str]]]]
 
 logger = logging.getLogger(__name__)
 
 NT_MAP = {
     "A": ["A"],
     "C": ["C"],
     "G": ["G"],
@@ -30,15 +30,15 @@
     "V": ["A", "C", "G"],
     "N": ["A", "C", "G", "T"],
 }
 
 
 def find_file_for_each_sample(
     basedir: Path,
-    glob_patterns: List[str],
+    glob_patterns: list[str],
     sample_name_cleanup: Optional[ListOfStrOrPattern] = None,
     single_entry_selector_func: Optional[Callable] = None,
 ) -> Mapping[str, Path]:
     sample_files = defaultdict(list)
     for glob_pattern in glob_patterns:
         for p in basedir.glob(glob_pattern):
             sample = extract_sample_name(p.name, remove=sample_name_cleanup)
@@ -50,15 +50,15 @@
             sample_file[sample] = single_entry_selector_func(files)
         else:
             # select first file if no selector func specified
             sample_file[sample] = files[0]
     return sample_file
 
 
-def select_most_recent_file(files: List[Path]) -> Path:
+def select_most_recent_file(files: list[Path]) -> Path:
     return sorted(files, key=lambda x: x.stat().st_mtime, reverse=True)[0]
 
 
 def extract_sample_name(
     filename: str,
     remove: Optional[ListOfStrOrPattern] = None,
 ) -> str:
@@ -119,33 +119,24 @@
         else:
             width = max_width_cells + offset
         if max_width:
             width = min(width, max_width)
         yield width
 
 
-def get_row_heights(df, idx, offset=0, multiplier=15):
+def get_row_heights(df: pd.DataFrame, idx: int, offset: int = 0, multiplier: int = 15):
     """Calculate row heights"""
     # get max number of newlines in the row
     newline_count = np.max(df.loc[idx, :].astype(str).str.count("\n").max())
     newline_count = max(newline_count, 1)
     height = newline_count * multiplier + offset
     logger.debug(f'idx="{idx}" height={height} newline_count={newline_count}')
     return height
 
 
-def list_get(xs: Optional[List], idx: int, default: Optional[Any] = None) -> Optional[Any]:
-    if not xs:
-        return default
-    try:
-        return xs[idx]
-    except (TypeError, IndexError):
-        return default
-
-
 def try_parse_number(s: str) -> Any:
     if "," in s:
         xs = s.split(",")
         return [try_parse_number(x) for x in xs]
     with contextlib.suppress(ValueError):
         return int(s)
     with contextlib.suppress(ValueError):
@@ -156,7 +147,21 @@
 def expand_degenerate_bases(seq: str) -> Iterable[str]:
     for x in product(*(NT_MAP[nt] for nt in seq)):
         yield "".join(x)
 
 
 def overlap(start1: int, end1: int, start2: int, end2: int) -> bool:
     return start1 < start2 < end1 or start1 < end2 < end1
+
+
+def get_ref_name_bam(path: Path) -> str:
+    import pysam
+
+    bam = pysam.AlignmentFile(path)
+    logger.info(f"BAM: {bam}")
+    ref_name = bam.get_reference_name(0)
+    logger.info(f"{ref_name=}")
+    if not ref_name:
+        for ref_name in bam.references:
+            if ref_name:
+                return ref_name
+    return ref_name
```

### Comparing `wgscovplot-1.0.1/wgscovplot/wgscovplot.py` & `wgscovplot-1.0.2/wgscovplot/wgscovplot.py`

 * *Files identical despite different names*

### Comparing `wgscovplot-1.0.1/wgscovplot/tools/variants.py` & `wgscovplot-1.0.2/wgscovplot/tools/variants.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import gzip
 import logging
 import re
 from collections import defaultdict
 from enum import Enum
 from operator import itemgetter
 from pathlib import Path
-from typing import DefaultDict, Dict, Iterable, List, Optional, Tuple, Union
+from typing import Iterable, Optional, Union
 
 import pandas as pd
 from pydantic import BaseModel
 
 from wgscovplot.flu import SampleSegmentRef
 from wgscovplot.util import find_file_for_each_sample, try_parse_number
 
@@ -182,39 +182,39 @@
     re.compile(r"\.snp[sS]ift\.table\.txt$"),
     re.compile(r"\.snp[sS]ift\.txt$"),
     re.compile(r"\.AF0\.\d+(\.filt)?"),
     re.compile(r"\.0\.\d+AF(\.filt)?"),
 ]
 
 
-def vcf_selector(paths: List[Path]) -> Optional[Path]:
+def vcf_selector(paths: list[Path]) -> Optional[Path]:
     xs = []
     for path in paths:
         variant_caller, df = read_vcf(path)
         xs.append((df.shape[0], path))
     xs.sort(reverse=True)
     try:
         return xs[0][1]
     except KeyError:
         return None
 
 
-def snpsift_selector(paths: List[Path]) -> Optional[Path]:
+def snpsift_selector(paths: list[Path]) -> Optional[Path]:
     xs = []
     for path in paths:
         df = pd.read_table(path)
         xs.append((df.shape[0], path))
     xs.sort(reverse=True)
     try:
         return xs[0][1]
     except KeyError:
         return None
 
 
-def read_vcf(vcf_file: Path) -> Tuple[str, pd.DataFrame]:
+def read_vcf(vcf_file: Path) -> tuple[str, pd.DataFrame]:
     """Read VCF file into a DataFrame"""
     gzipped = vcf_file.name.endswith(".gz")
     with gzip.open(vcf_file, "rt") if gzipped else open(vcf_file) as fh:
         vcf_cols = []
         variant_caller = ""
         for line in fh:
             if line.startswith("##source="):
@@ -222,16 +222,19 @@
             if line.startswith("##nanopolish"):
                 variant_caller = "nanopolish"
             if line.startswith("##medaka_version"):
                 variant_caller = "medaka"
             if line.startswith("#CHROM"):
                 vcf_cols = line[1:].strip().split("\t")
                 break
-        df = pd.read_table(fh, comment="#", header=None, names=vcf_cols)
-        df = df[~df.duplicated(["CHROM", "POS", "ID", "REF", "ALT", "FILTER"], keep="first")]
+        try:
+            df = pd.read_table(fh, comment="#", header=None, names=vcf_cols)
+            df = df[~df.duplicated(["CHROM", "POS", "ID", "REF", "ALT", "FILTER"], keep="first")]
+        except pd.errors.EmptyDataError:
+            return variant_caller, pd.DataFrame()
     return variant_caller, df
 
 
 def parse_aa(gene: str, ref: str, alt: str, nt_pos: int, snpeff_aa: str, effect: str) -> str:
     if snpeff_aa == ".":
         return f"{ref}{nt_pos}{alt}"
     m: Optional[re.Match[str]] = re.match(r"p\.([a-zA-Z]+)(\d+)([a-zA-Z]+)", snpeff_aa)
@@ -352,15 +355,15 @@
         # depth only applies to the first base in the ref allele rather than over the entire allele so the depth can be
         # misleading for deletions
         # See iVar issue: https://github.com/andersen-lab/ivar/issues/86
         infos = parse_vcf_info(row.INFO)
         total_dp = infos["DP"]
         ks = row.FORMAT.split(":")
         vs = row[-1].split(":")
-        record: Dict[str, Union[float, int, str]] = {k: try_parse_number(v) for k, v in zip(ks, vs)}
+        record: dict[str, Union[float, int, str]] = {k: try_parse_number(v) for k, v in zip(ks, vs)}
         ref_dp = int(record["REF_DP"])
         alt_dp = int(record["ALT_DP"])
         # if the sum of the ref and alt dp does not equal the total dp reported by iVar then recalculate the ref dp
         # since it is likely only reporting the ref dp for the first base of a longer deletion. SNPs should be fine.
         sum_ref_alt_dp = ref_dp + alt_dp
         if sum_ref_alt_dp != total_dp:
             record["REF_DP"] = total_dp - alt_dp
@@ -515,55 +518,54 @@
         out[key] = try_parse_number(val_str)
     return out
 
 
 def parse_clair3_vcf(
     df: pd.DataFrame,
     sample: str,
-) -> List[Dict[str, Union[str, float, int]]]:
+) -> Optional[pd.DataFrame]:
     if df.empty:
-        return []
+        return None
     df["Sample"] = sample
     df["ALT_FREQ"] = df["SAMPLE"].apply(lambda x: x.split(":")[-1])
     df.drop(columns=["ID", "INFO", "QUAL", "FILTER", "INFO", "FORMAT", "SAMPLE"], inplace=True)
     df = df.reindex(columns=["Sample", "Segment", "Segment Length", "CHROM", "POS", "REF", "ALT", "ALT_FREQ"])
     df.rename(columns={"CHROM": "REF_ID", "ALT": "ALT_SEQ", "REF": "REF_SEQ"}, inplace=True)
     df = df.astype({"POS": int, "ALT_FREQ": float})
-    return df.to_dict(orient="records")
+    return df
 
 
 def get_nf_flu_variant_info(
     basedir: Path,
-    req_seq: Dict[str, Dict[str, str]],
+    req_seq: dict[str, dict[str, str]],
     sample_top_references: list[SampleSegmentRef],
-) -> DefaultDict[str, Dict[str, List[Dict]]]:
-    out: DefaultDict[str, Dict[str, List[Dict]]] = defaultdict(dict)
+) -> defaultdict[str, dict[str, list[dict]]]:
+    out: defaultdict[str, dict[str, list[dict]]] = defaultdict(dict)
     for items in sample_top_references:
         segment = items.segment
         ref_id = items.ref_id
         sample = items.sample
         vcf_files = basedir.glob(f"**/variants/**/{sample}.Segment_{segment}.{ref_id}.no_frameshifts.vcf")
         ref_seq_len = 0
         if req_seq[sample][segment]:
             ref_seq_len = len(req_seq[sample][segment])
         for vcf_file in vcf_files:
             variants_caller, df_vcf = read_vcf(vcf_file)
             vcf_infos = parse_clair3_vcf(df_vcf, sample)
-            if vcf_infos:
-                for vcf_info in vcf_infos:
-                    vcf_info["Segment"] = segment
-                    vcf_info["Segment Length"] = ref_seq_len
-                out[sample][segment] = vcf_infos
+            if vcf_infos is not None:
+                vcf_infos["Segment"] = segment
+                vcf_infos["Segment Length"] = ref_seq_len
+                out[sample][segment] = vcf_infos.to_dict(orient="records")
     return out
 
 
 def get_info(
     basedir: Path,
     min_coverage: int = 10,
-) -> Dict[str, pd.DataFrame]:
+) -> dict[str, pd.DataFrame]:
     sample_vcf = find_file_for_each_sample(
         basedir=basedir,
         glob_patterns=VCF_GLOB_PATTERNS,
         sample_name_cleanup=VCF_SAMPLE_NAME_CLEANUP,
         single_entry_selector_func=vcf_selector,
     )
     sample_dfvcf = {}
```

### Comparing `wgscovplot-1.0.1/wgscovplot/tools/mosdepth/__init__.py` & `wgscovplot-1.0.2/wgscovplot/tools/mosdepth/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import base64
 import logging
 from collections import defaultdict
 from pathlib import Path
-from typing import Dict, List, Tuple, Union
+from typing import Union
 
 import numpy as np
 import pandas as pd
 from pydantic import BaseModel
 
 from wgscovplot.colors import AmpliconColour
 from wgscovplot.features import Feature
-from wgscovplot.util import find_file_for_each_sample
+from wgscovplot.util import find_file_for_each_sample, get_ref_name_bam
 
 logger = logging.getLogger(__name__)
 
 SAMPLE_NAME_CLEANUP = [
     ".genome.per-base.bed.gz",
     ".amplicon.per-base.bed.gz",
     ".per-base.bed.gz",
@@ -59,15 +59,15 @@
     genome_coverage: float
     mean_coverage: float
     median_coverage: float
     ref_seq_length: int
     max_depth: int
 
 
-def get_samples_name(basedir: Path, is_genome_segmented: bool) -> List:
+def get_samples_name(basedir: Path, is_genome_segmented: bool) -> list:
     glob_patterns = TOP_REFERENCE_PATTERNS if is_genome_segmented else PER_BASE_PATTERNS
     sample_beds = find_file_for_each_sample(
         basedir, glob_patterns=glob_patterns, sample_name_cleanup=SAMPLE_NAME_CLEANUP
     )
     out = list(sample_beds.keys())
     return sorted(out)
 
@@ -135,28 +135,14 @@
 def depth_array(df: pd.DataFrame) -> np.ndarray:
     arr = np.zeros(df.end_idx.max(), dtype=np.uint16)
     for row in df.itertuples():
         arr[row.start_idx : row.end_idx] = row.depth
     return arr
 
 
-def get_ref_name_bam(path: Path) -> str:
-    import pysam
-
-    bam = pysam.AlignmentFile(path)
-    logger.info(f"BAM: {bam}")
-    ref_name = bam.get_reference_name(0)
-    logger.info(f"{ref_name=}")
-    if not ref_name:
-        for ref_name in bam.references:
-            if ref_name:
-                return ref_name
-    return ref_name
-
-
 def get_refseq_id(basedir: Path) -> str:
     sample_paths = find_file_for_each_sample(
         basedir, glob_patterns=PER_BASE_PATTERNS, sample_name_cleanup=SAMPLE_NAME_CLEANUP
     )
     refseq_id = ""
     for path in sample_paths.values():
         if path.suffix == ".bam":
@@ -165,15 +151,15 @@
         df = read_mosdepth_bed(path)
         refseq_id = df["genome"][0] if df is not None and not df.empty else ""
         if not refseq_id:
             return refseq_id
     return refseq_id
 
 
-def get_amplicon_depths(basedir: Path) -> Dict[str, List]:
+def get_amplicon_depths(basedir: Path) -> dict[str, list]:
     sample_path = find_file_for_each_sample(
         basedir, glob_patterns=REGIONS_PATTERNS, sample_name_cleanup=SAMPLE_NAME_CLEANUP
     )
     out = defaultdict(list)
     sample = None
     try:
         for sample, path in sample_path.items():
@@ -192,15 +178,15 @@
         return dict(out)
     except Exception as e:
         logger.error(e, exc_info=True)
         logger.warning(f"{sample} No Region Amplicon Depth Found")
         return {}
 
 
-def get_region_amplicon(basedir: Path) -> List[Feature]:
+def get_region_amplicon(basedir: Path) -> list[Feature]:
     sample_path = find_file_for_each_sample(
         basedir, glob_patterns=REGIONS_PATTERNS, sample_name_cleanup=SAMPLE_NAME_CLEANUP
     )
     try:
         for path in sample_path.values():
             if path.suffix == ".bam":
                 break
@@ -216,15 +202,15 @@
     except Warning:
         logger.warning("No Region Amplicon Found")
     return []
 
 
 def get_info(
     basedir: Path, low_coverage_threshold: int = 5
-) -> Tuple[Dict[str, MosdepthDepthInfo], Dict[str, np.ndarray]]:
+) -> tuple[dict[str, MosdepthDepthInfo], dict[str, np.ndarray]]:
     sample_beds = find_file_for_each_sample(
         basedir, glob_patterns=PER_BASE_PATTERNS, sample_name_cleanup=SAMPLE_NAME_CLEANUP
     )
     out = {}
     sample_depths = {}
     for sample, path in sample_beds.items():
         logger.info(f"{sample=} {path=}")
@@ -250,16 +236,16 @@
             max_depth=arr.max(initial=0),
         )
         out[sample] = depth_info
     return out, sample_depths
 
 
 def get_base64_encoded_depth_arrays(
-    sample_depths: Union[Dict[str, np.ndarray], Dict[str, Dict[str, np.ndarray]]]
-) -> Union[Dict[str, str], Dict[str, Dict[str, str]]]:
+    sample_depths: Union[dict[str, np.ndarray], dict[str, dict[str, np.ndarray]]]
+) -> Union[dict[str, str], dict[str, dict[str, str]]]:
     """Encode depth arrays as base64 strings
 
     Instead of dumping a list of numbers to a JSON list, the float32 array will be base64 encoded so
     that it can be decoded into a Float32Array in JS. The base64 encoding will compress the numbers
     significantly (~60% of the size of dumping list to JSON).
 
     ```python
```

### Comparing `wgscovplot-1.0.1/wgscovplot/tools/mosdepth/flu.py` & `wgscovplot-1.0.2/wgscovplot/tools/mosdepth/flu.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 from collections import defaultdict
 from pathlib import Path
-from typing import DefaultDict, Dict, List, Tuple
 
 import numpy as np
 import pandas as pd
 
 from wgscovplot.flu import SampleSegmentRef
 from wgscovplot.tools.mosdepth import (
     MosdepthDepthInfo,
@@ -20,19 +19,19 @@
 
 class FluMosdepthDepthInfo(MosdepthDepthInfo):
     segment: str
 
 
 def get_flu_mosdepth_info(
     basedir: Path,
-    sample_top_references: List[SampleSegmentRef],
+    sample_top_references: list[SampleSegmentRef],
     low_coverage_threshold: int = 5,
-) -> Tuple[Dict[str, Dict[str, FluMosdepthDepthInfo]], Dict[str, Dict[str, np.ndarray]]]:
-    sample_segment_depths: DefaultDict[str, Dict] = defaultdict(dict)
-    sample_segment_depth_info: DefaultDict[str, Dict] = defaultdict(dict)
+) -> tuple[dict[str, dict[str, FluMosdepthDepthInfo]], dict[str, dict[str, np.ndarray]]]:
+    sample_segment_depths: defaultdict[str, dict] = defaultdict(dict)
+    sample_segment_depth_info: defaultdict[str, dict] = defaultdict(dict)
     for item in sample_top_references:
         segment = item.segment
         ref_id = item.ref_id
         sample = item.sample
         bed_files = list(basedir.glob(f"**/mosdepth/**/{sample}.Segment_{segment}.{ref_id}.per-base.bed.gz"))
         if not bed_files:
             logger.error(f'No Mosdepth BED file found for sample "{sample}" and segment "{segment}" ({ref_id}).')
```

### Comparing `wgscovplot-1.0.1/.gitignore` & `wgscovplot-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `wgscovplot-1.0.1/LICENSE` & `wgscovplot-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wgscovplot-1.0.1/README.md` & `wgscovplot-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `wgscovplot-1.0.1/hatch_build.py` & `wgscovplot-1.0.2/hatch_build.py`

 * *Files identical despite different names*

### Comparing `wgscovplot-1.0.1/pyproject.toml` & `wgscovplot-1.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,28 +3,27 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "wgscovplot"
 dynamic = ["version"]
 description = "Create interactive comparative sequencing coverage plots from virus sequencing data."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = "Apache-2.0"
 keywords = []
 authors = [
     { name = "Hai Hoang Nguyen", email = "hoanghai.nguyen@inspection.gc.ca" },
     { name = "Peter Kruczkiewicz", email = "peter.kruczkiewicz@gmail.com" },
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
 dependencies = [
     "typer",
     "rich",
     "pandas",
     'biopython',
@@ -94,15 +93,15 @@
 ]
 cov = [
     "test-cov",
     "cov-report",
 ]
 
 [[tool.hatch.envs.all.matrix]]
-python = ["3.8", "3.9", "3.10", "3.11"]
+python = ["3.9", "3.10", "3.11"]
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
     "black>=23.1.0",
     "mypy>=1.0.0",
     "ruff>=0.0.243",
@@ -120,21 +119,22 @@
 ]
 all = [
     "style",
     "typing",
 ]
 
 [tool.black]
-target-version = ["py38"]
+target-version = ["py311"]
 line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
-target-version = "py38"
+target-version = "py311"
 line-length = 120
+[tool.ruff.lint]
 select = [
     "A",
     "ARG",
     "B",
     "C",
     "DTZ",
     "E",
@@ -170,27 +170,33 @@
     "FBT002",
     # Allow boolean positional values in function calls, like `dict.get(... True)`
     "FBT003",
     # Ignore checks for possible passwords
     "S105", "S106", "S107",
     # Ignore complexity
     "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
+    # Ignore "Use `X | Y` for type annotations"
+    "UP007",
+    # Ignore "Import from `collections.abc` instead: `Iterable`, `Mapping`, `Callable`"
+    "UP035",
+    # Ignore "B905 [*] `zip()` without an explicit `strict=` parameter"
+    "B905",
 ]
 unfixable = [
     # Don't touch unused imports
     "F401",
 ]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["wgscovplot"]
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
 [tool.coverage.run]
 source_pkgs = ["wgscovplot", "tests"]
 branch = true
 parallel = true
```

### Comparing `wgscovplot-1.0.1/PKG-INFO` & `wgscovplot-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: wgscovplot
-Version: 1.0.1
+Version: 1.0.2
 Summary: Create interactive comparative sequencing coverage plots from virus sequencing data.
 Project-URL: Documentation, https://github.com/CFIA-NCFAD/wgscovplot#readme
 Project-URL: Issues, https://github.com/CFIA-NCFAD/wgscovplot/issues
 Project-URL: Source, https://github.com/CFIA-NCFAD/wgscovplot
 Author-email: Hai Hoang Nguyen <hoanghai.nguyen@inspection.gc.ca>, Peter Kruczkiewicz <peter.kruczkiewicz@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Requires-Dist: bcbio-gff
 Requires-Dist: biopython
 Requires-Dist: edlib
 Requires-Dist: jinja2
 Requires-Dist: pandas
 Requires-Dist: pydantic>=2.0.0
 Requires-Dist: pysam
```

