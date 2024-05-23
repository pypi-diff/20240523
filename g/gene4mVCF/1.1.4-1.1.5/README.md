# Comparing `tmp/gene4mvcf-1.1.4.tar.gz` & `tmp/gene4mvcf-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gene4mvcf-1.1.4.tar", last modified: Wed May 22 16:28:20 2024, max compression
+gzip compressed data, was "gene4mvcf-1.1.5.tar", last modified: Thu May 23 20:23:29 2024, max compression
```

## Comparing `gene4mvcf-1.1.4.tar` & `gene4mvcf-1.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-22 16:28:20.568721 gene4mvcf-1.1.4/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2798 2024-05-22 16:28:20.568721 gene4mvcf-1.1.4/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     2348 2024-05-22 16:27:06.000000 gene4mvcf-1.1.4/README.md
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-22 16:28:20.564721 gene4mvcf-1.1.4/gene4mVCF/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 11:07:18.000000 gene4mvcf-1.1.4/gene4mVCF/__init__.py
--rwxrwxr-x   0 ws2024    (1000) ws2024    (1000)     6323 2024-05-22 16:20:58.000000 gene4mvcf-1.1.4/gene4mVCF/fetchgenes.py
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-22 16:28:20.568721 gene4mvcf-1.1.4/gene4mVCF.egg-info/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2798 2024-05-22 16:28:20.000000 gene4mvcf-1.1.4/gene4mVCF.egg-info/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      264 2024-05-22 16:28:20.000000 gene4mvcf-1.1.4/gene4mVCF.egg-info/SOURCES.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-22 16:28:20.000000 gene4mvcf-1.1.4/gene4mVCF.egg-info/dependency_links.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       56 2024-05-22 16:28:20.000000 gene4mvcf-1.1.4/gene4mVCF.egg-info/entry_points.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       78 2024-05-22 16:28:20.000000 gene4mvcf-1.1.4/gene4mVCF.egg-info/requires.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-05-22 16:28:20.000000 gene4mvcf-1.1.4/gene4mVCF.egg-info/top_level.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-05-22 16:28:20.568721 gene4mvcf-1.1.4/setup.cfg
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1343 2024-05-22 16:27:50.000000 gene4mvcf-1.1.4/setup.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-23 20:23:29.946719 gene4mvcf-1.1.5/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2952 2024-05-23 20:23:29.946719 gene4mvcf-1.1.5/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     2503 2024-05-23 20:21:34.000000 gene4mvcf-1.1.5/README.md
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-23 20:23:29.942719 gene4mvcf-1.1.5/gene4mVCF/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-20 11:07:18.000000 gene4mvcf-1.1.5/gene4mVCF/__init__.py
+-rwxrwxr-x   0 ws2024    (1000) ws2024    (1000)     6515 2024-05-23 20:17:02.000000 gene4mvcf-1.1.5/gene4mVCF/fetchgenes.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-23 20:23:29.946719 gene4mvcf-1.1.5/gene4mVCF.egg-info/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2952 2024-05-23 20:23:29.000000 gene4mvcf-1.1.5/gene4mVCF.egg-info/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      264 2024-05-23 20:23:29.000000 gene4mvcf-1.1.5/gene4mVCF.egg-info/SOURCES.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-23 20:23:29.000000 gene4mvcf-1.1.5/gene4mVCF.egg-info/dependency_links.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       56 2024-05-23 20:23:29.000000 gene4mvcf-1.1.5/gene4mVCF.egg-info/entry_points.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       78 2024-05-23 20:23:29.000000 gene4mvcf-1.1.5/gene4mVCF.egg-info/requires.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-05-23 20:23:29.000000 gene4mvcf-1.1.5/gene4mVCF.egg-info/top_level.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-05-23 20:23:29.946719 gene4mvcf-1.1.5/setup.cfg
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1342 2024-05-23 20:19:30.000000 gene4mvcf-1.1.5/setup.py
```

### Comparing `gene4mvcf-1.1.4/PKG-INFO` & `gene4mvcf-1.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: gene4mVCF
-Version: 1.1.4
+Version: 1.1.5
 Summary: Description of your package
-Home-page: https://github.com/VJ-Ulaganathan/gene4mVCF
+Home-page: https://github.com/vkulaganathan/gene4mVCF
 Author: Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: vijay-kumar.ulaganathan@uni-tuebingen.de
 Description-Content-Type: text/markdown
 Requires-Dist: pysam>=0.16.0.1
 Requires-Dist: pandas>=1.0.0
 Requires-Dist: pybedtools>=0.8.0
 Requires-Dist: tqdm>=4.47.0
@@ -37,14 +37,15 @@
  <br>`-i INPUT, --input INPUT, is bgzip compressed VCF file`</br>
  <br>`-g GENE, --genes GENE, is either a Gene name, Ensembl gene ID, or path to a genelist file with *.txt extension`</br>
 
 
 <br>optional arguments:</br>
    <br>`-h, --help show this help message and exit`</br>
    <br>`-r REFERENCE, --ref REFERENCE, is 37 or 38, based on the reference genome used for creating the VCF file`</br>
+   <br>`-f FEATURE, --feature FEATURE, is feature type(s) to filter for (e.g., exon, CDS, 5UTR, 3UTR, transcript)`</br>
   
 ## Examples
 Extract variants for a single gene using gene name:
 `$ gene4mVCF -i input.vcf.gz -g EGFR`
 
 Extract variants for a single using ensembl gene id:
 `$ gene4mVCF -i input.vcf.gz -g ENSG00000168878`
@@ -60,18 +61,24 @@
 ![Example Image](images/input.png)
 
 <br>Output file in the tab-separated format</br>
 ![Example Image](images/ACTB.png)
 
 
 ## Support
-For any issues or inquiries, please open an issue on the GitHub repository https://github.com/VJ-Ulaganathan/gene4mVCF
+For any issues or inquiries, please open an issue on the GitHub repository https://github.com/vkulaganathan/gene4mVCF
 
 
 ## Installation
 
 Installation via pip:
 
 `$ pip install gene4mVCF`
 
 
 
+
+
+<i>current version='1.1.5'</i>
+
+
+
```

### Comparing `gene4mvcf-1.1.4/README.md` & `gene4mvcf-1.1.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
  <br>`-i INPUT, --input INPUT, is bgzip compressed VCF file`</br>
  <br>`-g GENE, --genes GENE, is either a Gene name, Ensembl gene ID, or path to a genelist file with *.txt extension`</br>
 
 
 <br>optional arguments:</br>
    <br>`-h, --help show this help message and exit`</br>
    <br>`-r REFERENCE, --ref REFERENCE, is 37 or 38, based on the reference genome used for creating the VCF file`</br>
+   <br>`-f FEATURE, --feature FEATURE, is feature type(s) to filter for (e.g., exon, CDS, 5UTR, 3UTR, transcript)`</br>
   
 ## Examples
 Extract variants for a single gene using gene name:
 `$ gene4mVCF -i input.vcf.gz -g EGFR`
 
 Extract variants for a single using ensembl gene id:
 `$ gene4mVCF -i input.vcf.gz -g ENSG00000168878`
@@ -46,18 +47,24 @@
 ![Example Image](images/input.png)
 
 <br>Output file in the tab-separated format</br>
 ![Example Image](images/ACTB.png)
 
 
 ## Support
-For any issues or inquiries, please open an issue on the GitHub repository https://github.com/VJ-Ulaganathan/gene4mVCF
+For any issues or inquiries, please open an issue on the GitHub repository https://github.com/vkulaganathan/gene4mVCF
 
 
 ## Installation
 
 Installation via pip:
 
 `$ pip install gene4mVCF`
 
 
 
+
+
+<i>current version='1.1.5'</i>
+
+
+
```

### Comparing `gene4mvcf-1.1.4/gene4mVCF/fetchgenes.py` & `gene4mvcf-1.1.5/gene4mVCF/fetchgenes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import argparse
 import subprocess
 import os
 import gzip
 from tqdm import tqdm
+import pybedtools
 
-def parse_bed_file(gene_identifier, genome_version):
+def parse_bed_file(gene_identifier, genome_version, feature_filter=None):
     if genome_version == "hg38" or "GRCh38" in genome_version:
         if gene_identifier.startswith("ENSG"):
             bed_file = "hg38.ensGene.bed"
         else:
             bed_file = "hg38.ncbiRefSeq.bed"
     elif genome_version == "hg19" or "GRCh37" in genome_version:
         if gene_identifier.startswith("ENSG"):
@@ -17,59 +18,55 @@
             bed_file = "hg19.ncbiRefSeq.bed"
     else:
         # Default to hg19 if genome version cannot be determined
         if gene_identifier.startswith("ENSG"):
             bed_file = "hg19.ensGene.bed"
         else:
             bed_file = "hg19.ncbiRefSeq.bed"
-    
+
     print("Selected BED file:", bed_file)  # Add this line for debugging
 
     gene_regions = {}
     gene_chromosomes = {}
-    with open(bed_file, 'r') as file:
-        lines = file.readlines()
-        for line in tqdm(lines, desc="Reading BED file"):
-            fields = line.strip().split('\t')
-            chrom = fields[0].lstrip("chr")
-            start = int(fields[1])
-            end = int(fields[2])
-            gene_name = fields[3]
-            feature = fields[7]
-
-            if gene_identifier.startswith("ENSG"):
-                if fields[3] == gene_identifier:
-                    gene_regions[(chrom, start, end)] = (gene_name, feature)
-                    gene_chromosomes[gene_identifier] = chrom
-            else:
-                if fields[3] == gene_identifier:
-                    gene_regions[(chrom, start, end)] = (gene_name, feature)
-                    gene_chromosomes[gene_identifier] = chrom
+
+    bed_tool = pybedtools.BedTool(bed_file)
+    for entry in tqdm(bed_tool, desc="Reading BED file"):
+        chrom = entry.chrom.lstrip("chr")
+        start = int(entry.start)
+        end = int(entry.end)
+        gene_name = entry.name
+        feature = entry.fields[7] if len(entry.fields) > 7 else 'exon'  # Default to exon if feature not specified
+
+        if gene_identifier.startswith("ENSG"):
+            if gene_name == gene_identifier and (feature_filter is None or feature in feature_filter):
+                gene_regions[(chrom, start, end)] = (gene_name, feature)
+                gene_chromosomes[gene_identifier] = chrom
+        else:
+            if gene_name == gene_identifier and (feature_filter is None or feature in feature_filter):
+                gene_regions[(chrom, start, end)] = (gene_name, feature)
+                gene_chromosomes[gene_identifier] = chrom
 
     if not gene_regions:
         raise ValueError(f"Gene {gene_identifier} not found in {bed_file}")
     return gene_regions, gene_chromosomes
 
 def get_reference_genome(vcf_path):
     reference_genome = None
     with gzip.open(vcf_path, 'rt') as file:
         for line in file:
             if line.startswith("##contig="):
-                if "assembly=gnomAD_GRCh38" in line:
-                    reference_genome = "GRCh38"
-                elif "assembly=GRCh38" in line:
+                if "assembly=gnomAD_GRCh38" in line or "assembly=GRCh38" in line:
                     reference_genome = "GRCh38"
                 break
             elif line.startswith("#CHROM"):
                 reference_genome = "GRCh37"  # Default to GRCh37, as genome version could not be determined from the given vcf file
                 break
-                
+
     if reference_genome is None:
-        # Default to GRCh37 if genome version cannot be determined
-        reference_genome = "GRCh37"
+        reference_genome = "GRCh37"  # Default to GRCh37 if genome version cannot be determined
         print("Reference genome could not be determined from the VCF file, defaulting to GRCh37")
 
     return reference_genome
 
 def get_gene_info(chrom, pos, gene_regions):
     for (region_chrom, start, end), (gene_name, feature) in gene_regions.items():
         if region_chrom == chrom and start <= pos <= end:
@@ -77,14 +74,15 @@
     return "", ""
 
 def main():
     parser = argparse.ArgumentParser(description='Extract variant entries for a specific gene or list of genes from a VCF file.')
     parser.add_argument('-i', '--input', required=True, help='Input VCF file')
     parser.add_argument('-g', '--genes', required=True, help='Gene name, Ensembl gene ID, or path to a gene list file')
     parser.add_argument('-r', '--ref', choices=['37', '38'], help='Reference genome version (optional)')
+    parser.add_argument('-f', '--feature', nargs='+', help='Feature type(s) to filter for (e.g., exon, CDS, 5UTR, 3UTR, transcript)')
 
     args = parser.parse_args()
 
     if args.ref:
         genome_version = "hg19" if args.ref == "37" else "hg38"
     else:
         genome_version = get_reference_genome(args.input)
@@ -97,15 +95,15 @@
             gene_list = [line.strip() for line in gene_list_file]
     else:
         gene_list = [args.genes]
 
     gene_regions = {}
     gene_chromosomes = {}
     for gene_identifier in tqdm(gene_list, desc="Processing genes"):
-        regions, chromosomes = parse_bed_file(gene_identifier, genome_version)
+        regions, chromosomes = parse_bed_file(gene_identifier, genome_version, feature_filter=args.feature)
         gene_regions.update(regions)
         gene_chromosomes.update(chromosomes)
 
     # Create index file for the input VCF file
     index_file = args.input + ".tbi"
     if not os.path.exists(index_file):
         subprocess.run(["tabix", "-p", "vcf", args.input], check=True)
```

### Comparing `gene4mvcf-1.1.4/gene4mVCF.egg-info/PKG-INFO` & `gene4mvcf-1.1.5/gene4mVCF.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: gene4mVCF
-Version: 1.1.4
+Version: 1.1.5
 Summary: Description of your package
-Home-page: https://github.com/VJ-Ulaganathan/gene4mVCF
+Home-page: https://github.com/vkulaganathan/gene4mVCF
 Author: Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: vijay-kumar.ulaganathan@uni-tuebingen.de
 Description-Content-Type: text/markdown
 Requires-Dist: pysam>=0.16.0.1
 Requires-Dist: pandas>=1.0.0
 Requires-Dist: pybedtools>=0.8.0
 Requires-Dist: tqdm>=4.47.0
@@ -37,14 +37,15 @@
  <br>`-i INPUT, --input INPUT, is bgzip compressed VCF file`</br>
  <br>`-g GENE, --genes GENE, is either a Gene name, Ensembl gene ID, or path to a genelist file with *.txt extension`</br>
 
 
 <br>optional arguments:</br>
    <br>`-h, --help show this help message and exit`</br>
    <br>`-r REFERENCE, --ref REFERENCE, is 37 or 38, based on the reference genome used for creating the VCF file`</br>
+   <br>`-f FEATURE, --feature FEATURE, is feature type(s) to filter for (e.g., exon, CDS, 5UTR, 3UTR, transcript)`</br>
   
 ## Examples
 Extract variants for a single gene using gene name:
 `$ gene4mVCF -i input.vcf.gz -g EGFR`
 
 Extract variants for a single using ensembl gene id:
 `$ gene4mVCF -i input.vcf.gz -g ENSG00000168878`
@@ -60,18 +61,24 @@
 ![Example Image](images/input.png)
 
 <br>Output file in the tab-separated format</br>
 ![Example Image](images/ACTB.png)
 
 
 ## Support
-For any issues or inquiries, please open an issue on the GitHub repository https://github.com/VJ-Ulaganathan/gene4mVCF
+For any issues or inquiries, please open an issue on the GitHub repository https://github.com/vkulaganathan/gene4mVCF
 
 
 ## Installation
 
 Installation via pip:
 
 `$ pip install gene4mVCF`
 
 
 
+
+
+<i>current version='1.1.5'</i>
+
+
+
```

### Comparing `gene4mvcf-1.1.4/setup.py` & `gene4mvcf-1.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 
 # Check if all required commands exist
 if not all(command_exists(cmd) for cmd in required_commands):
     raise RuntimeError("Please install the following dependencies: bcftools, bgzip, tabix")
 
 setup(
     name='gene4mVCF',
-    version='1.1.4',
+    version='1.1.5',
     description='Description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Pr (France). Dr. rer. nat. Vijay K. ULAGANATHAN',
     author_email='vijay-kumar.ulaganathan@uni-tuebingen.de',
-    url='https://github.com/VJ-Ulaganathan/gene4mVCF',
+    url='https://github.com/vkulaganathan/gene4mVCF',
     packages=find_packages(),
     package_data={'gene4mVCF': ['hg19.ensGene.bed', 'hg19.ncbiRefSeq.bed', 'hg38.ensGene.bed', 'hg38.ncbiRefSeq.bed']},
     install_requires=[
         'pysam>=0.16.0.1',
         'pandas>=1.0.0',
         'pybedtools>=0.8.0',
         'tqdm>=4.47.0',
```

