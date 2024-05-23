# Comparing `tmp/biodata-0.0.7.tar.gz` & `tmp/biodata-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biodata-0.0.7.tar", last modified: Tue May  7 11:15:28 2024, max compression
+gzip compressed data, was "biodata-0.0.8.tar", last modified: Thu May 23 02:22:12 2024, max compression
```

## Comparing `biodata-0.0.7.tar` & `biodata-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-05-07 11:15:28.787828 biodata-0.0.7/
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)     5621 2024-05-07 11:15:28.786827 biodata-0.0.7/PKG-INFO
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)     5037 2023-01-23 06:58:01.000000 biodata-0.0.7/README.md
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-05-07 11:15:28.763826 biodata-0.0.7/biodata/
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)        0 2021-11-03 03:50:28.000000 biodata-0.0.7/biodata/__init__.py
--rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     9933 2024-05-07 11:00:55.000000 biodata-0.0.7/biodata/baseio.py
--rwxr-x---   0 kl945     (5298) hy299_0001 (80905)    11057 2023-01-03 17:37:44.000000 biodata-0.0.7/biodata/bed.py
--rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     8834 2023-01-03 16:21:18.000000 biodata-0.0.7/biodata/delimited.py
--rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     5522 2023-01-14 08:29:58.000000 biodata-0.0.7/biodata/fasta.py
--rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     5659 2023-01-23 06:58:54.000000 biodata-0.0.7/biodata/gff.py
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)     6360 2023-01-21 06:14:11.000000 biodata-0.0.7/biodata/meme.py
--rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     9483 2023-01-03 16:21:03.000000 biodata-0.0.7/biodata/old.py
-drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-05-07 11:15:28.786827 biodata-0.0.7/biodata.egg-info/
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)     5621 2024-05-07 11:15:23.000000 biodata-0.0.7/biodata.egg-info/PKG-INFO
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)      309 2024-05-07 11:15:23.000000 biodata-0.0.7/biodata.egg-info/SOURCES.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)        1 2024-05-07 11:15:23.000000 biodata-0.0.7/biodata.egg-info/dependency_links.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)       20 2024-05-07 11:15:23.000000 biodata-0.0.7/biodata.egg-info/requires.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)        8 2024-05-07 11:15:23.000000 biodata-0.0.7/biodata.egg-info/top_level.txt
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)       38 2024-05-07 11:15:28.787828 biodata-0.0.7/setup.cfg
--rw-r-----   0 kl945     (5298) hy299_0001 (80905)      842 2024-05-07 11:07:30.000000 biodata-0.0.7/setup.py
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-05-23 02:22:12.663633 biodata-0.0.8/
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     5621 2024-05-23 02:22:12.639632 biodata-0.0.8/PKG-INFO
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     5037 2023-01-23 06:58:01.000000 biodata-0.0.8/README.md
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-05-23 02:22:12.638632 biodata-0.0.8/biodata/
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)        0 2021-11-03 03:50:28.000000 biodata-0.0.8/biodata/__init__.py
+-rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     9933 2024-05-07 11:00:55.000000 biodata-0.0.8/biodata/baseio.py
+-rwxr-x---   0 kl945     (5298) hy299_0001 (80905)    11737 2024-05-23 02:18:21.000000 biodata-0.0.8/biodata/bed.py
+-rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     8834 2023-01-03 16:21:18.000000 biodata-0.0.8/biodata/delimited.py
+-rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     5522 2023-01-14 08:29:58.000000 biodata-0.0.8/biodata/fasta.py
+-rwxr-x---   0 kl945     (5298) hy299_0001 (80905)     5659 2023-01-23 06:58:54.000000 biodata-0.0.8/biodata/gff.py
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     6360 2023-01-21 06:14:11.000000 biodata-0.0.8/biodata/meme.py
+drwxr-s---   0 kl945     (5298) hy299_0001 (80905)        0 2024-05-23 02:22:12.638632 biodata-0.0.8/biodata.egg-info/
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)     5621 2024-05-23 02:22:04.000000 biodata-0.0.8/biodata.egg-info/PKG-INFO
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      294 2024-05-23 02:22:04.000000 biodata-0.0.8/biodata.egg-info/SOURCES.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)        1 2024-05-23 02:22:04.000000 biodata-0.0.8/biodata.egg-info/dependency_links.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)       20 2024-05-23 02:22:04.000000 biodata-0.0.8/biodata.egg-info/requires.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)        8 2024-05-23 02:22:04.000000 biodata-0.0.8/biodata.egg-info/top_level.txt
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)       38 2024-05-23 02:22:12.663633 biodata-0.0.8/setup.cfg
+-rw-r-----   0 kl945     (5298) hy299_0001 (80905)      842 2024-05-23 02:18:39.000000 biodata-0.0.8/setup.py
```

### Comparing `biodata-0.0.7/PKG-INFO` & `biodata-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biodata
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python package for common biological data I/O
 Home-page: https://github.com/aldenleung/biodata/
 Author: Alden Leung
 Author-email: alden.leung@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `biodata-0.0.7/README.md` & `biodata-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `biodata-0.0.7/biodata/baseio.py` & `biodata-0.0.8/biodata/baseio.py`

 * *Files identical despite different names*

### Comparing `biodata-0.0.7/biodata/bed.py` & `biodata-0.0.8/biodata/bed.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''
 Created on Dec 29, 2020
 
 @author: Alden
 '''
 
 
-# BED3, BED, BEDX, BEDGraph, BEDPE
+# BED3, BED, BEDX, BEDGraph, BEDPE and all bed-derived file formats
 
 from .baseio import BaseReader, BaseWriter
 from .baseio import BaseIReader
 from genomictools import GenomicAnnotation, StrandedGenomicAnnotation, GenomicPos, StrandedGenomicPos
 
 
 class BED3(GenomicAnnotation):
@@ -62,15 +62,19 @@
 		return BED3(chrom, chromStart, chromEnd)
 	
 class BED3Writer(BaseWriter):
 	def write(self, bed3):
 		'''
 		Output the BED3
 		'''
-		super(BED3Writer, self).write("{}\t{}\t{}\n".format(bed3.chrom, bed3.chromStart, bed3.chromEnd))
+		if isinstance(bed3, BED3):
+			super(BED3Writer, self).write("{}\t{}\t{}\n".format(bed3.chrom, bed3.chromStart, bed3.chromEnd))
+		else: # assume GenomicPos
+			r = bed3.genomic_pos
+			super(BED3Writer, self).write("{}\t{}\t{}\n".format(r.name, r.zstart, r.ostop))
 
 
 		
 	
 class BED(BED3, StrandedGenomicAnnotation):
 	'''
 	The standard 12-field BED format 
@@ -141,14 +145,15 @@
 				raise Exception("Inconsistent blockCount and blockStarts")
 			if blockStarts[0] != 0:
 				raise Exception("First block must start at 0")
 			if chromStart + blockStarts[-1] + blockSizes[-1] != chromEnd:
 				raise Exception("Last block must end at chromEnd")		 
 		
 		return BED(chrom, chromStart, chromEnd, name, score, strand, thickStart, thickEnd, itemRgb, blockCount, blockSizes, blockStarts)
+
 	
 	
 class BEDWriter(BaseWriter):
 	def write(self, bed):
 		'''
 		Output the BEDNode
 		'''
@@ -219,14 +224,18 @@
 		self.dataValue = dataValue
 		
 class BEDGraphReader(BaseReader):
 	
 	def __init__(self, arg, dataValueType=float):
 		super(BEDGraphReader, self).__init__(arg)
 		self.dataValueType = dataValueType
+	def _metainfo_reader(self):
+		self._proceed_next_line()
+		while self._line is not None and (self._line.startswith("track") or self._line.startswith("browser")):
+			self._proceed_next_line()
 	
 	def _read(self):
 		line = self._line
 		if line is None:
 			return None
 		self._proceed_next_line() 
 		words_array = line.split('\t')
@@ -244,16 +253,14 @@
 		self.dataValueFunc = dataValueFunc
 		
 	def write(self, bedgraph):
 		'''
 		Output the BEDGraph
 		'''
 		super(BEDGraphWriter, self).write("{}\t{}\t{}\t{}\n".format(bedgraph.chrom, bedgraph.chromStart, bedgraph.chromEnd, self.dataValueFunc(bedgraph.dataValue)))
-		
-		
 	
 
 
 class BEDPE():
 	'''
 	'''
 	def __init__(self, chrom1, start1, stop1, chrom2, start2, stop2, name=None, score=None, strand1=None, strand2=None):
@@ -279,14 +286,24 @@
 	@property
 	def stranded_genomic_pos2(self):
 		return StrandedGenomicPos(self.chrom2, self.start2 + 1, self.stop2, self.strand2)
 	
 class BEDPEReader(BaseReader):
 	def __init__(self, arg):
 		super(BEDPEReader, self).__init__(arg)
+	def _proceed_next_line(self):
+		while True:
+			line = self.f.readline()
+			if line == '':
+				self._line = None
+				break
+			line = line.rstrip("\r\n") # Auto-stripping
+			if line != '' and not line.startswith("#"): # Auto comment removal. Blank lines are skipped by default
+				self._line = line
+				break
 			
 	def _read(self):
 		if self._line is None:
 			return None
 		words_array = self._line.split('\t')
 		self._proceed_next_line()
 		name = None
@@ -308,15 +325,14 @@
 		if len(words_array) >= 10:
 			strand2 = words_array[9]
 		return BEDPE(chrom1, start1, stop1, chrom2, start2, stop2, name, score, strand1, strand2)
 		
 	
 	
 class BEDPEWriter(BaseWriter):
-	# Untested
 	def __init__(self, arg):
 		super(BEDPEWriter, self).__init__(arg)
 			
 	def write(self, bedpe):
 		'''
 		Output the BEDPENode
 		Note that the start position is stored in 1-based but output in 0-based
```

### Comparing `biodata-0.0.7/biodata/delimited.py` & `biodata-0.0.8/biodata/delimited.py`

 * *Files identical despite different names*

### Comparing `biodata-0.0.7/biodata/fasta.py` & `biodata-0.0.8/biodata/fasta.py`

 * *Files identical despite different names*

### Comparing `biodata-0.0.7/biodata/gff.py` & `biodata-0.0.8/biodata/gff.py`

 * *Files identical despite different names*

### Comparing `biodata-0.0.7/biodata/meme.py` & `biodata-0.0.8/biodata/meme.py`

 * *Files identical despite different names*

### Comparing `biodata-0.0.7/biodata.egg-info/PKG-INFO` & `biodata-0.0.8/biodata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biodata
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python package for common biological data I/O
 Home-page: https://github.com/aldenleung/biodata/
 Author: Alden Leung
 Author-email: alden.leung@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `biodata-0.0.7/setup.py` & `biodata-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as readme_file:
 	readme = readme_file.read()
 
 requirements = ["genomictools>=0.0.5"]
 
 setup(
 	name="biodata",
-	version="0.0.7",
+	version="0.0.8",
 	author="Alden Leung",
 	author_email="alden.leung@gmail.com",
 	description="A python package for common biological data I/O",
 	long_description=readme,
 	long_description_content_type="text/markdown",
 	url="https://github.com/aldenleung/biodata/",
 	packages=find_packages(),
```

