# Comparing `tmp/afipcaeqrdecode-0.0.8.tar.gz` & `tmp/afipcaeqrdecode-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afipcaeqrdecode-0.0.8.tar", last modified: Mon Nov 27 23:36:40 2023, max compression
+gzip compressed data, was "afipcaeqrdecode-0.0.9.tar", last modified: Tue Nov 28 21:43:58 2023, max compression
```

## Comparing `afipcaeqrdecode-0.0.8.tar` & `afipcaeqrdecode-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 mezka     (1000) mezka     (1000)        0 2023-11-27 23:36:40.041893 afipcaeqrdecode-0.0.8/
--rw-rw-r--   0 mezka     (1000) mezka     (1000)     3834 2023-11-27 23:36:40.041893 afipcaeqrdecode-0.0.8/PKG-INFO
--rw-rw-r--   0 mezka     (1000) mezka     (1000)     3535 2023-11-27 22:43:02.000000 afipcaeqrdecode-0.0.8/README.md
-drwxrwxr-x   0 mezka     (1000) mezka     (1000)        0 2023-11-27 23:36:40.041893 afipcaeqrdecode-0.0.8/afipcaeqrdecode/
--rw-rw-r--   0 mezka     (1000) mezka     (1000)       98 2023-11-26 20:32:59.000000 afipcaeqrdecode-0.0.8/afipcaeqrdecode/__init__.py
--rw-rw-r--   0 mezka     (1000) mezka     (1000)     1123 2023-11-27 23:33:26.000000 afipcaeqrdecode-0.0.8/afipcaeqrdecode/extract_qr_cae_from_invoice_pdf_and_decode.py
-drwxrwxr-x   0 mezka     (1000) mezka     (1000)        0 2023-11-27 23:36:40.041893 afipcaeqrdecode-0.0.8/afipcaeqrdecode.egg-info/
--rw-rw-r--   0 mezka     (1000) mezka     (1000)     3834 2023-11-27 23:36:40.000000 afipcaeqrdecode-0.0.8/afipcaeqrdecode.egg-info/PKG-INFO
--rw-rw-r--   0 mezka     (1000) mezka     (1000)      302 2023-11-27 23:36:40.000000 afipcaeqrdecode-0.0.8/afipcaeqrdecode.egg-info/SOURCES.txt
--rw-rw-r--   0 mezka     (1000) mezka     (1000)        1 2023-11-27 23:36:40.000000 afipcaeqrdecode-0.0.8/afipcaeqrdecode.egg-info/dependency_links.txt
--rw-rw-r--   0 mezka     (1000) mezka     (1000)       98 2023-11-27 23:36:40.000000 afipcaeqrdecode-0.0.8/afipcaeqrdecode.egg-info/requires.txt
--rw-rw-r--   0 mezka     (1000) mezka     (1000)       16 2023-11-27 23:36:40.000000 afipcaeqrdecode-0.0.8/afipcaeqrdecode.egg-info/top_level.txt
--rw-rw-r--   0 mezka     (1000) mezka     (1000)       38 2023-11-27 23:36:40.041893 afipcaeqrdecode-0.0.8/setup.cfg
--rw-rw-r--   0 mezka     (1000) mezka     (1000)      629 2023-11-27 23:35:51.000000 afipcaeqrdecode-0.0.8/setup.py
+drwxrwxr-x   0 mezka     (1000) mezka     (1000)        0 2023-11-28 21:43:58.014145 afipcaeqrdecode-0.0.9/
+-rw-rw-r--   0 mezka     (1000) mezka     (1000)     3926 2023-11-28 21:43:58.014145 afipcaeqrdecode-0.0.9/PKG-INFO
+-rw-rw-r--   0 mezka     (1000) mezka     (1000)     3627 2023-11-28 21:42:04.000000 afipcaeqrdecode-0.0.9/README.md
+drwxrwxr-x   0 mezka     (1000) mezka     (1000)        0 2023-11-28 21:43:58.014145 afipcaeqrdecode-0.0.9/afipcaeqrdecode/
+-rw-rw-r--   0 mezka     (1000) mezka     (1000)      106 2023-11-28 21:29:00.000000 afipcaeqrdecode-0.0.9/afipcaeqrdecode/__init__.py
+-rw-rw-r--   0 mezka     (1000) mezka     (1000)     1023 2023-11-28 21:40:17.000000 afipcaeqrdecode-0.0.9/afipcaeqrdecode/convert_pdf_to_image_and_detect_and_decode_qrs.py
+drwxrwxr-x   0 mezka     (1000) mezka     (1000)        0 2023-11-28 21:43:58.014145 afipcaeqrdecode-0.0.9/afipcaeqrdecode.egg-info/
+-rw-rw-r--   0 mezka     (1000) mezka     (1000)     3926 2023-11-28 21:43:57.000000 afipcaeqrdecode-0.0.9/afipcaeqrdecode.egg-info/PKG-INFO
+-rw-rw-r--   0 mezka     (1000) mezka     (1000)      306 2023-11-28 21:43:57.000000 afipcaeqrdecode-0.0.9/afipcaeqrdecode.egg-info/SOURCES.txt
+-rw-rw-r--   0 mezka     (1000) mezka     (1000)        1 2023-11-28 21:43:57.000000 afipcaeqrdecode-0.0.9/afipcaeqrdecode.egg-info/dependency_links.txt
+-rw-rw-r--   0 mezka     (1000) mezka     (1000)       83 2023-11-28 21:43:57.000000 afipcaeqrdecode-0.0.9/afipcaeqrdecode.egg-info/requires.txt
+-rw-rw-r--   0 mezka     (1000) mezka     (1000)       16 2023-11-28 21:43:57.000000 afipcaeqrdecode-0.0.9/afipcaeqrdecode.egg-info/top_level.txt
+-rw-rw-r--   0 mezka     (1000) mezka     (1000)       38 2023-11-28 21:43:58.014145 afipcaeqrdecode-0.0.9/setup.cfg
+-rw-rw-r--   0 mezka     (1000) mezka     (1000)      629 2023-11-28 21:41:28.000000 afipcaeqrdecode-0.0.9/setup.py
```

### Comparing `afipcaeqrdecode-0.0.8/PKG-INFO` & `afipcaeqrdecode-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 Metadata-Version: 2.1
 Name: afipcaeqrdecode
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package to decode and extract invoice metadata from an AFIP CAE qr code link
 Home-page: https://github.com/mezka/afipcaeqrdecode
 Author: Emiliano Mesquita
 License: GPLv3
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 [PyPI python package](https://pypi.org/project/afipcaeqrdecode/)
 
 # AFIP invoice pdf qr CAE extract and decode
 
-This is a python package that uses [PyMuPDF](https://pypi.org/project/PyMuPDF/) to dump images from your pdf invoices with an AFIP CAE QR code, and decodes them using [qreader](https://pypi.org/project/qreader/) in order to extract relevant invoice metadata like:
+This is a python package that uses [pdf2image](https://pypi.org/project/pdf2image/) to convert the first page of your AFIP invoice with an AFIP CAE QR code to an image, and then run [qreader](https://pypi.org/project/qreader/) on it in order to locate and decode the AFIP CAE QR code in order to extract relevant invoice metadata like: 
 
 - Invoice date
 - CUIT of invoice creator
 - AFIP electronic invoice point of sale (Punto de venta)
 - Invoice number
 - Amount
 - Currency
 - CUIT of inovoice recipient
 
 And other less important properties.
 
-## Why qreader instead of plain pyzbar
+## Why convert to image instead of extracting
 
-This library used just [pyzbar](https://pypi.org/project/pyzbar/) in its inception, however we came upon some QR codes that simply did not decode succesfully using just [pyzbar](https://pypi.org/project/pyzbar/).
+In its inception this library used [PyMuPDF](https://pypi.org/project/PyMuPDF/) in order to extract all images inside the invoices and then run [qreader](https://pypi.org/project/qreader/) on them, however, we came upon some invoices in which the qr code image failed to extract.
+
+## Why qreader instead of pyzbar
+
+In its inception this library used just [pyzbar](https://pypi.org/project/pyzbar/), however we came upon some QR codes which did not decode succesfully using just [pyzbar](https://pypi.org/project/pyzbar/).
 
 [qreader](https://pypi.org/project/qreader/) depends on [pyzbar](https://pypi.org/project/pyzbar/), but uses a pre-trained AI model to detect and segment QR codes, using information extracted by this AI model, it applies different image preprocessing techniques that heavily increase the decoding rate by [pyzbar](https://pypi.org/project/pyzbar/)
 
 ## Example Usage and notes about metadata
 
 Using the included sample files for demonstration (and ran from repository root using included sample file):
 
 ```
-from afipcaeqrdecode import extract_qr_cae_from_invoice_pdf_and_decode
+from afipcaeqrdecode import convert_pdf_to_image_and_detect_and_decode_qrs
 
-invoice_metadata = extract_qr_cae_from_invoice_pdf_and_decode('./tests/sample_files/2000005044986390.pdf')
+invoice_metadata = convert_pdf_to_image_and_detect_and_decode_qrs('./tests/sample_files/2000005044986390.pdf')
 ```
 
 Here, invoice metadata will evaluate to:
 
 ```python
 {
     "ver":1,
@@ -83,17 +87,14 @@
 
 `pip install afipcaeqrdecode`
 
 ## First run notice
 
 On first run [qreader](https://pypi.org/project/qreader/) will download the weights to run its QR detector AI model, then it will resume program operation automatically.
 
-## How does it work
-
-It dumps every image of the PDF invoice and then matches it with the format of the URL link that an AFIP CAE QR returns, if it matches it decodes it using `jwt.utils.base64url_decode`. If an invoice has more than one CAE QR code it will return the first one that decodes succesfully.
 
 ## WARNING
 
 This is an experimental package, USE IN PRODUCTION AT YOUR OWN RISK.
 
 It is barely even tested, i'm sharing it so I can actually import it as a PyPI package in another project that consumes it.
```

### Comparing `afipcaeqrdecode-0.0.8/README.md` & `afipcaeqrdecode-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 [PyPI python package](https://pypi.org/project/afipcaeqrdecode/)
 
 # AFIP invoice pdf qr CAE extract and decode
 
-This is a python package that uses [PyMuPDF](https://pypi.org/project/PyMuPDF/) to dump images from your pdf invoices with an AFIP CAE QR code, and decodes them using [qreader](https://pypi.org/project/qreader/) in order to extract relevant invoice metadata like:
+This is a python package that uses [pdf2image](https://pypi.org/project/pdf2image/) to convert the first page of your AFIP invoice with an AFIP CAE QR code to an image, and then run [qreader](https://pypi.org/project/qreader/) on it in order to locate and decode the AFIP CAE QR code in order to extract relevant invoice metadata like: 
 
 - Invoice date
 - CUIT of invoice creator
 - AFIP electronic invoice point of sale (Punto de venta)
 - Invoice number
 - Amount
 - Currency
 - CUIT of inovoice recipient
 
 And other less important properties.
 
-## Why qreader instead of plain pyzbar
+## Why convert to image instead of extracting
 
-This library used just [pyzbar](https://pypi.org/project/pyzbar/) in its inception, however we came upon some QR codes that simply did not decode succesfully using just [pyzbar](https://pypi.org/project/pyzbar/).
+In its inception this library used [PyMuPDF](https://pypi.org/project/PyMuPDF/) in order to extract all images inside the invoices and then run [qreader](https://pypi.org/project/qreader/) on them, however, we came upon some invoices in which the qr code image failed to extract.
+
+## Why qreader instead of pyzbar
+
+In its inception this library used just [pyzbar](https://pypi.org/project/pyzbar/), however we came upon some QR codes which did not decode succesfully using just [pyzbar](https://pypi.org/project/pyzbar/).
 
 [qreader](https://pypi.org/project/qreader/) depends on [pyzbar](https://pypi.org/project/pyzbar/), but uses a pre-trained AI model to detect and segment QR codes, using information extracted by this AI model, it applies different image preprocessing techniques that heavily increase the decoding rate by [pyzbar](https://pypi.org/project/pyzbar/)
 
 ## Example Usage and notes about metadata
 
 Using the included sample files for demonstration (and ran from repository root using included sample file):
 
 ```
-from afipcaeqrdecode import extract_qr_cae_from_invoice_pdf_and_decode
+from afipcaeqrdecode import convert_pdf_to_image_and_detect_and_decode_qrs
 
-invoice_metadata = extract_qr_cae_from_invoice_pdf_and_decode('./tests/sample_files/2000005044986390.pdf')
+invoice_metadata = convert_pdf_to_image_and_detect_and_decode_qrs('./tests/sample_files/2000005044986390.pdf')
 ```
 
 Here, invoice metadata will evaluate to:
 
 ```python
 {
     "ver":1,
@@ -73,17 +77,14 @@
 
 `pip install afipcaeqrdecode`
 
 ## First run notice
 
 On first run [qreader](https://pypi.org/project/qreader/) will download the weights to run its QR detector AI model, then it will resume program operation automatically.
 
-## How does it work
-
-It dumps every image of the PDF invoice and then matches it with the format of the URL link that an AFIP CAE QR returns, if it matches it decodes it using `jwt.utils.base64url_decode`. If an invoice has more than one CAE QR code it will return the first one that decodes succesfully.
 
 ## WARNING
 
 This is an experimental package, USE IN PRODUCTION AT YOUR OWN RISK.
 
 It is barely even tested, i'm sharing it so I can actually import it as a PyPI package in another project that consumes it.
```

### Comparing `afipcaeqrdecode-0.0.8/afipcaeqrdecode.egg-info/PKG-INFO` & `afipcaeqrdecode-0.0.9/afipcaeqrdecode.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 Metadata-Version: 2.1
 Name: afipcaeqrdecode
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package to decode and extract invoice metadata from an AFIP CAE qr code link
 Home-page: https://github.com/mezka/afipcaeqrdecode
 Author: Emiliano Mesquita
 License: GPLv3
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 [PyPI python package](https://pypi.org/project/afipcaeqrdecode/)
 
 # AFIP invoice pdf qr CAE extract and decode
 
-This is a python package that uses [PyMuPDF](https://pypi.org/project/PyMuPDF/) to dump images from your pdf invoices with an AFIP CAE QR code, and decodes them using [qreader](https://pypi.org/project/qreader/) in order to extract relevant invoice metadata like:
+This is a python package that uses [pdf2image](https://pypi.org/project/pdf2image/) to convert the first page of your AFIP invoice with an AFIP CAE QR code to an image, and then run [qreader](https://pypi.org/project/qreader/) on it in order to locate and decode the AFIP CAE QR code in order to extract relevant invoice metadata like: 
 
 - Invoice date
 - CUIT of invoice creator
 - AFIP electronic invoice point of sale (Punto de venta)
 - Invoice number
 - Amount
 - Currency
 - CUIT of inovoice recipient
 
 And other less important properties.
 
-## Why qreader instead of plain pyzbar
+## Why convert to image instead of extracting
 
-This library used just [pyzbar](https://pypi.org/project/pyzbar/) in its inception, however we came upon some QR codes that simply did not decode succesfully using just [pyzbar](https://pypi.org/project/pyzbar/).
+In its inception this library used [PyMuPDF](https://pypi.org/project/PyMuPDF/) in order to extract all images inside the invoices and then run [qreader](https://pypi.org/project/qreader/) on them, however, we came upon some invoices in which the qr code image failed to extract.
+
+## Why qreader instead of pyzbar
+
+In its inception this library used just [pyzbar](https://pypi.org/project/pyzbar/), however we came upon some QR codes which did not decode succesfully using just [pyzbar](https://pypi.org/project/pyzbar/).
 
 [qreader](https://pypi.org/project/qreader/) depends on [pyzbar](https://pypi.org/project/pyzbar/), but uses a pre-trained AI model to detect and segment QR codes, using information extracted by this AI model, it applies different image preprocessing techniques that heavily increase the decoding rate by [pyzbar](https://pypi.org/project/pyzbar/)
 
 ## Example Usage and notes about metadata
 
 Using the included sample files for demonstration (and ran from repository root using included sample file):
 
 ```
-from afipcaeqrdecode import extract_qr_cae_from_invoice_pdf_and_decode
+from afipcaeqrdecode import convert_pdf_to_image_and_detect_and_decode_qrs
 
-invoice_metadata = extract_qr_cae_from_invoice_pdf_and_decode('./tests/sample_files/2000005044986390.pdf')
+invoice_metadata = convert_pdf_to_image_and_detect_and_decode_qrs('./tests/sample_files/2000005044986390.pdf')
 ```
 
 Here, invoice metadata will evaluate to:
 
 ```python
 {
     "ver":1,
@@ -83,17 +87,14 @@
 
 `pip install afipcaeqrdecode`
 
 ## First run notice
 
 On first run [qreader](https://pypi.org/project/qreader/) will download the weights to run its QR detector AI model, then it will resume program operation automatically.
 
-## How does it work
-
-It dumps every image of the PDF invoice and then matches it with the format of the URL link that an AFIP CAE QR returns, if it matches it decodes it using `jwt.utils.base64url_decode`. If an invoice has more than one CAE QR code it will return the first one that decodes succesfully.
 
 ## WARNING
 
 This is an experimental package, USE IN PRODUCTION AT YOUR OWN RISK.
 
 It is barely even tested, i'm sharing it so I can actually import it as a PyPI package in another project that consumes it.
```

### Comparing `afipcaeqrdecode-0.0.8/setup.py` & `afipcaeqrdecode-0.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='afipcaeqrdecode',
-    version='0.0.8',
+    version='0.0.9',
     packages=find_packages(),
     install_requires=requirements,
     description='Package to decode and extract invoice metadata from an AFIP CAE qr code link',
     author='Emiliano Mesquita',
     license='GPLv3',
     url='https://github.com/mezka/afipcaeqrdecode',
     long_description=long_description,
```

